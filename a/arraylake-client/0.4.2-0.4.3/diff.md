# Comparing `tmp/arraylake_client-0.4.2.tar.gz` & `tmp/arraylake_client-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraylake_client-0.4.2.tar", max compression
+gzip compressed data, was "arraylake_client-0.4.3.tar", max compression
```

## Comparing `arraylake_client-0.4.2.tar` & `arraylake_client-0.4.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      654 2023-06-22 20:23:42.538357 arraylake_client-0.4.2/README.md
--rw-r--r--   0        0        0      357 2023-06-07 16:41:28.210985 arraylake_client-0.4.2/arraylake_client/__init__.py
--rw-r--r--   0        0        0       70 2023-06-07 16:41:28.212174 arraylake_client-0.4.2/arraylake_client/__main__.py
--rw-r--r--   0        0        0    15359 2023-06-27 00:27:20.947227 arraylake_client-0.4.2/arraylake_client/api_utils.py
--rw-r--r--   0        0        0     2381 2023-06-16 17:29:47.000000 arraylake_client-0.4.2/arraylake_client/async_utils.py
--rw-r--r--   0        0        0      630 2023-06-07 16:41:28.212923 arraylake_client-0.4.2/arraylake_client/chunkstore/__init__.py
--rw-r--r--   0        0        0     1534 2023-06-07 16:41:28.213251 arraylake_client-0.4.2/arraylake_client/chunkstore/abc.py
--rw-r--r--   0        0        0     5201 2023-06-07 16:41:28.213373 arraylake_client-0.4.2/arraylake_client/chunkstore/s3chunkstore.py
--rw-r--r--   0        0        0        0 2023-06-07 16:41:28.213456 arraylake_client-0.4.2/arraylake_client/cli/__init__.py
--rw-r--r--   0        0        0     3822 2023-06-07 16:41:28.213758 arraylake_client-0.4.2/arraylake_client/cli/auth.py
--rw-r--r--   0        0        0     4762 2023-06-07 16:41:28.213838 arraylake_client-0.4.2/arraylake_client/cli/config.py
--rw-r--r--   0        0        0     1155 2023-06-07 16:41:28.213908 arraylake_client-0.4.2/arraylake_client/cli/main.py
--rw-r--r--   0        0        0     3568 2023-06-22 20:23:42.539238 arraylake_client-0.4.2/arraylake_client/cli/repo.py
--rw-r--r--   0        0        0     3390 2023-06-07 16:41:28.214762 arraylake_client-0.4.2/arraylake_client/cli/utils.py
--rw-r--r--   0        0        0     7327 2023-07-08 00:39:33.338130 arraylake_client-0.4.2/arraylake_client/client.py
--rw-r--r--   0        0        0     7098 2023-06-13 00:03:11.755118 arraylake_client-0.4.2/arraylake_client/commits.py
--rw-r--r--   0        0        0      538 2023-06-07 16:41:28.215453 arraylake_client-0.4.2/arraylake_client/config.py
--rw-r--r--   0        0        0      105 2023-06-07 16:41:28.215671 arraylake_client-0.4.2/arraylake_client/config.yaml
--rw-r--r--   0        0        0      192 2023-06-07 18:29:47.978531 arraylake_client-0.4.2/arraylake_client/exceptions.py
--rw-r--r--   0        0        0     1110 2023-06-16 17:29:47.000000 arraylake_client-0.4.2/arraylake_client/log_util.py
--rw-r--r--   0        0        0      282 2023-06-22 20:23:42.540028 arraylake_client-0.4.2/arraylake_client/metastore/__init__.py
--rw-r--r--   0        0        0     8188 2023-07-08 00:39:33.338322 arraylake_client-0.4.2/arraylake_client/metastore/abc.py
--rw-r--r--   0        0        0    12464 2023-07-08 00:39:33.338491 arraylake_client-0.4.2/arraylake_client/metastore/http_metastore.py
--rw-r--r--   0        0        0    51546 2023-07-08 00:40:14.647940 arraylake_client-0.4.2/arraylake_client/repo.py
--rw-r--r--   0        0        0     1227 2023-06-22 20:23:42.540945 arraylake_client-0.4.2/arraylake_client/spec.py
--rw-r--r--   0        0        0     4166 2023-06-07 16:41:28.218150 arraylake_client-0.4.2/arraylake_client/token.py
--rw-r--r--   0        0        0     9753 2023-06-22 20:23:42.541106 arraylake_client-0.4.2/arraylake_client/types.py
--rw-r--r--   0        0        0    10315 2023-06-27 00:27:16.448369 arraylake_client-0.4.2/arraylake_client/virtual.py
--rw-r--r--   0        0        0      851 2023-06-16 17:29:47.000000 arraylake_client-0.4.2/arraylake_client/zarr_util.py
--rw-r--r--   0        0        0     2337 2023-07-08 00:43:08.120935 arraylake_client-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2043 1970-01-01 00:00:00.000000 arraylake_client-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      633 2023-07-11 00:45:35.236162 arraylake_client-0.4.3/README.md
+-rw-r--r--   0        0        0      357 2023-06-07 16:41:28.210985 arraylake_client-0.4.3/arraylake_client/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-07 16:41:28.212174 arraylake_client-0.4.3/arraylake_client/__main__.py
+-rw-r--r--   0        0        0    15553 2023-07-11 00:45:35.238345 arraylake_client-0.4.3/arraylake_client/api_utils.py
+-rw-r--r--   0        0        0     2381 2023-06-16 17:29:47.000000 arraylake_client-0.4.3/arraylake_client/async_utils.py
+-rw-r--r--   0        0        0      630 2023-06-07 16:41:28.212923 arraylake_client-0.4.3/arraylake_client/chunkstore/__init__.py
+-rw-r--r--   0        0        0     1534 2023-06-07 16:41:28.213251 arraylake_client-0.4.3/arraylake_client/chunkstore/abc.py
+-rw-r--r--   0        0        0     5201 2023-06-07 16:41:28.213373 arraylake_client-0.4.3/arraylake_client/chunkstore/s3chunkstore.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:41:28.213456 arraylake_client-0.4.3/arraylake_client/cli/__init__.py
+-rw-r--r--   0        0        0     3973 2023-07-11 00:45:35.238508 arraylake_client-0.4.3/arraylake_client/cli/auth.py
+-rw-r--r--   0        0        0     4762 2023-06-07 16:41:28.213838 arraylake_client-0.4.3/arraylake_client/cli/config.py
+-rw-r--r--   0        0        0     1155 2023-06-07 16:41:28.213908 arraylake_client-0.4.3/arraylake_client/cli/main.py
+-rw-r--r--   0        0        0     3568 2023-06-22 20:23:42.539238 arraylake_client-0.4.3/arraylake_client/cli/repo.py
+-rw-r--r--   0        0        0     3390 2023-06-07 16:41:28.214762 arraylake_client-0.4.3/arraylake_client/cli/utils.py
+-rw-r--r--   0        0        0     7621 2023-07-11 00:45:35.239080 arraylake_client-0.4.3/arraylake_client/client.py
+-rw-r--r--   0        0        0     7098 2023-06-13 00:03:11.755118 arraylake_client-0.4.3/arraylake_client/commits.py
+-rw-r--r--   0        0        0      538 2023-06-07 16:41:28.215453 arraylake_client-0.4.3/arraylake_client/config.py
+-rw-r--r--   0        0        0      105 2023-06-07 16:41:28.215671 arraylake_client-0.4.3/arraylake_client/config.yaml
+-rw-r--r--   0        0        0      192 2023-06-07 18:29:47.978531 arraylake_client-0.4.3/arraylake_client/exceptions.py
+-rw-r--r--   0        0        0     1110 2023-06-16 17:29:47.000000 arraylake_client-0.4.3/arraylake_client/log_util.py
+-rw-r--r--   0        0        0      282 2023-06-22 20:23:42.540028 arraylake_client-0.4.3/arraylake_client/metastore/__init__.py
+-rw-r--r--   0        0        0     8188 2023-07-08 00:39:33.338322 arraylake_client-0.4.3/arraylake_client/metastore/abc.py
+-rw-r--r--   0        0        0    12667 2023-07-11 00:45:35.239261 arraylake_client-0.4.3/arraylake_client/metastore/http_metastore.py
+-rw-r--r--   0        0        0    52115 2023-07-08 00:45:35.560450 arraylake_client-0.4.3/arraylake_client/repo.py
+-rw-r--r--   0        0        0     1227 2023-06-22 20:23:42.540945 arraylake_client-0.4.3/arraylake_client/spec.py
+-rw-r--r--   0        0        0     4550 2023-07-11 00:45:35.239407 arraylake_client-0.4.3/arraylake_client/token.py
+-rw-r--r--   0        0        0     9753 2023-06-22 20:23:42.541106 arraylake_client-0.4.3/arraylake_client/types.py
+-rw-r--r--   0        0        0    10315 2023-06-27 00:27:16.448369 arraylake_client-0.4.3/arraylake_client/virtual.py
+-rw-r--r--   0        0        0      851 2023-06-16 17:29:47.000000 arraylake_client-0.4.3/arraylake_client/zarr_util.py
+-rw-r--r--   0        0        0     2337 2023-07-11 00:49:57.966500 arraylake_client-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 arraylake_client-0.4.3/PKG-INFO
```

### Comparing `arraylake_client-0.4.2/README.md` & `arraylake_client-0.4.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # arraylake-client
 
 <p align="center">
-<img src="https://preview.earthmover.io/img/Earthmover_Main_Logo_1130x625.png" width="200" alt="Earthmover">
+<img src="https://earthmover-web-assets.s3.amazonaws.com/04-Arraylake-Lockup-Midnight-RGB-LARGE.png" width="200" alt="Arraylake">
 </p>
 
 <p align="center">
-  <a href="https://preview.earthmover.io" rel="nofollow">earthmover.io</a> -
-  <a href="https://preview.earthmover.io/docs/overview" rel="nofollow">documentation</a>
+  <a href="https://earthmover.io" rel="nofollow">earthmover.io</a> -
+  <a href="https://docs.earthmover.io" rel="nofollow">documentation</a>
 </p>
 
 Arraylake is a cloud-based platform that understands a wide array of multidimensional scientific data. Organize, analyze, build, and collaborate—effortlessly.
 
-Checkout the [documentation](https://preview.earthmover.io/docs/overview) to get started.
+Checkout the [documentation](https://docs.earthmover.io) to get started.
 
 ## Install
 
 ```
 pip install "arraylake_client[cli]"
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
 # arraylake-client
-                                 [Earthmover]
+                                  [Arraylake]
                          earthmover.io - documentation
 Arraylake is a cloud-based platform that understands a wide array of
 multidimensional scientific data. Organize, analyze, build, and
 collaborateâeffortlessly. Checkout the [documentation](https://
-preview.earthmover.io/docs/overview) to get started. ## Install ``` pip install
+docs.earthmover.io) to get started. ## Install ``` pip install
 "arraylake_client[cli]" ```
```

### Comparing `arraylake_client-0.4.2/arraylake_client/api_utils.py` & `arraylake_client-0.4.3/arraylake_client/api_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,22 +67,24 @@
     return results
 
 
 class ArraylakeHttpClient:
     """Base class to centralize interacting with Arraylake REST API"""
 
     api_url: str
+    hint: str = None
     token: str = field(default=None, repr=False)  # machine token. id/access/refresh tokens are managed by CustomOauth
     timeout: int = HTTP_TIMEOUT
 
     _client: Optional[httpx.AsyncClient]  # set in __aenter__
     _OPEN: bool
 
-    def __init__(self, api_url: str, token: str = None):
+    def __init__(self, api_url: str, hint: str = None, token: str = None):
         self.api_url = api_url
+        self.hint = hint
         self.token = token
 
         self._default_headers = {
             "accept": "application/vnd.earthmover+json",
             # technically we don't enforce this, for now it's for debugging purposes
             "client-name": "arraylake-python-client",
             "client-version": arraylake_client.__version__,
@@ -102,15 +104,15 @@
         transport = AsyncRetryTransport()
 
         if self.token:
             # if a token is presented, just use that token for all all Authentication headers
             auth = TokenAuth(self.token)
         else:
             # otherwise, assume we are using OAuth tokens stored on disk
-            auth = UserAuth(self.api_url)
+            auth = UserAuth(self.api_url, self.hint)
 
         self._client = await httpx.AsyncClient(
             base_url=self.api_url, transport=transport, headers=self._default_headers, auth=auth, timeout=self.timeout
         ).__aenter__()
         self._OPEN = True
         return self
 
@@ -203,32 +205,34 @@
     Parameters
     ----------
     api_endpoint : str
     """
 
     requires_response_body = True
 
-    def __init__(self, api_endpoint: str):
+    def __init__(self, api_endpoint: str, hint: str = None):
         self.api_endpoint = api_endpoint
-
+        self.hint = hint
         self._refresh_url = f"{api_endpoint}/refresh_token"
 
         # self._sync_lock = threading.RLock()  # uncomment when we need sync_auth_flow
         self._async_lock = asyncio.Lock()
 
-        self._token_handler = TokenHandler(api_endpoint=api_endpoint, raise_if_not_logged_in=True)
+        self._token_handler = TokenHandler(api_endpoint=api_endpoint, hint=self.hint, raise_if_not_logged_in=True)
 
     @property
     def _bearer_token(self):
         token = self._token_handler.tokens.id_token.get_secret_value()
         return f"Bearer {token}"
 
     def build_refresh_request(self) -> httpx.Request:
         # Return an `httpx.Request` for refreshing tokens.
         params = {"token": self._token_handler.tokens.refresh_token.get_secret_value()}
+        if self.hint:
+            params["hint"] = self.hint
         request = httpx.Request("GET", self._refresh_url, params=params)
         return request
 
     async def async_auth_flow(self, request: httpx.Request) -> httpx.Request:
         request.headers["Authorization"] = self._bearer_token
         response = yield request
         if response.status_code == httpx.codes.UNAUTHORIZED:
```

### Comparing `arraylake_client-0.4.2/arraylake_client/async_utils.py` & `arraylake_client-0.4.3/arraylake_client/async_utils.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/arraylake_client/chunkstore/__init__.py` & `arraylake_client-0.4.3/arraylake_client/chunkstore/__init__.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/arraylake_client/chunkstore/abc.py` & `arraylake_client-0.4.3/arraylake_client/chunkstore/abc.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/arraylake_client/chunkstore/s3chunkstore.py` & `arraylake_client-0.4.3/arraylake_client/chunkstore/s3chunkstore.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/arraylake_client/cli/auth.py` & `arraylake_client-0.4.3/arraylake_client/cli/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,41 +9,44 @@
 from arraylake_client.cli.utils import coro, error_console, print_logo, rich_console
 from arraylake_client.token import AuthException, TokenHandler
 from arraylake_client.types import ApiTokenInfo, UserInfo
 
 auth = typer.Typer(help="Manage Arraylake authentication")
 
 
-def _get_auth_handler() -> TokenHandler:
-    return TokenHandler(api_endpoint=config.get("service.uri"))
+def _get_auth_handler(org: str = None) -> TokenHandler:
+    return TokenHandler(api_endpoint=config.get("service.uri"), hint=org or config.get("user.org", None))
 
 
 async def _get_user() -> Union[ApiTokenInfo, UserInfo]:
     async with ArraylakeHttpClient(api_url=config.get("service.uri")) as client:
         user = await client.get_user()
     return user
 
 
 @auth.command()
 @coro
-async def login(browser: bool = typer.Option(True, help="Whether to automatically open a browser window.")):
+async def login(
+    browser: bool = typer.Option(True, help="Whether to automatically open a browser window."),
+    org: str = typer.Option(None, help="Org identifier for custom login provider"),
+):
     """**Log in** to Arraylake
 
     This will automatically open a browser window. If **--no-browser** is specified, a link will be printed.
 
     **Examples**
 
     - Log in without automatically opening a browser window
 
         ```
         $ arraylake auth login --no-browser
         ```
     """
     print_logo()
-    handler = _get_auth_handler()
+    handler = _get_auth_handler(org)
     if handler.tokens is not None:
         await handler.refresh_token()
     else:
         url = await handler.get_authorize_url()
 
         if browser:
             open_new(url)
```

### Comparing `arraylake_client-0.4.2/arraylake_client/cli/config.py` & `arraylake_client-0.4.3/arraylake_client/cli/config.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/arraylake_client/cli/main.py` & `arraylake_client-0.4.3/arraylake_client/cli/main.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/arraylake_client/cli/repo.py` & `arraylake_client-0.4.3/arraylake_client/cli/repo.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/arraylake_client/cli/utils.py` & `arraylake_client-0.4.3/arraylake_client/cli/utils.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/arraylake_client/client.py` & `arraylake_client-0.4.3/arraylake_client/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,41 +49,43 @@
     Args:
         service_uri (str): [Optional] The service URI to target.
         token (str): [Optional] API token for service account authentication.
     """
 
     service_uri: Optional[str] = None
     token: Optional[str] = field(default=None, repr=False)
+    auth_org: Optional[str] = None
 
     def __post_init__(self):
         if self.service_uri is None:
             self.service_uri = config.get("service.uri")
+        self.auth_org = self.auth_org or config.get("user.org", None)
 
     # TODO: replace the return type with a stricted type around repo listing object
     async def list_repos(self, org: str) -> Sequence[dict]:
         """List all repositories for the specified org
 
         Args:
             org: Name of the org
         """
 
         _validate_org(org)
-        mstore = HttpMetastore(HttpMetastoreConfig(self.service_uri, org, self.token))
+        mstore = HttpMetastore(HttpMetastoreConfig(self.service_uri, org, self.token, self.auth_org))
         repo_names = await mstore.list_databases()
         return repo_names
 
     async def get_repo(self, name: str) -> AsyncRepo:
         """Get a repo by name
 
         Args:
             name: Full name of the repo (of the form {ORG}/{REPO})
         """
 
         org, repo_name = _parse_org_and_repo(name)
-        mstore = HttpMetastore(HttpMetastoreConfig(self.service_uri, org, self.token))
+        mstore = HttpMetastore(HttpMetastoreConfig(self.service_uri, org, self.token, self.auth_org))
         db = await mstore.open_database(repo_name)
 
         s3_uri = config.get("chunkstore.uri")
         client_kws = config.get("s3", {})
         cstore = chunkstore(s3_uri, **client_kws)
 
         async with mstore:
@@ -109,15 +111,15 @@
         """Create a new repo
 
         Args:
             name: Full name of the repo to create (of the form {ORG}/{REPO})
         """
 
         org, repo_name = _parse_org_and_repo(name)
-        mstore = HttpMetastore(HttpMetastoreConfig(self.service_uri, org, self.token))
+        mstore = HttpMetastore(HttpMetastoreConfig(self.service_uri, org, self.token, self.auth_org))
 
         s3_uri = config.get("chunkstore.uri")
         client_kws = config.get("s3", {})
         cstore = chunkstore(s3_uri, **client_kws)
 
         async with mstore:
             user = await mstore.get_user()
@@ -132,15 +134,15 @@
         """Delete a repo
 
         Args:
             name: Full name of the repo to delete (of the form {ORG}/{REPO})
         """
 
         org, repo_name = _parse_org_and_repo(name)
-        mstore = HttpMetastore(HttpMetastoreConfig(self.service_uri, org, self.token))
+        mstore = HttpMetastore(HttpMetastoreConfig(self.service_uri, org, self.token, self.auth_org))
         await mstore.delete_database(repo_name, imsure=imsure, imreallysure=imreallysure)
 
 
 # This version of synchronize is different from the one in repo.py.
 # That version stores the global portal on the Repo object itself.
 # This version also uses the global portal but enters and exits the context for each call.
 # This is undoubtedly slower (a new thread is started and stopped on each call.)
@@ -162,20 +164,22 @@
     Args:
         service_uri (str): [Optional] The service URI to target.
         token (str): [Optional] API token for service account authentication.
     """
 
     service_uri: Optional[str] = None
     token: Optional[str] = field(default=None, repr=False)
+    auth_org: Optional[str] = None
 
     def __post_init__(self):
         if self.service_uri is None:
             self.service_uri = config.get("service.uri")
+        self.auth_org = self.auth_org or config.get("user.org", None)
 
-        self.aclient = AsyncClient(self.service_uri, token=self.token)
+        self.aclient = AsyncClient(self.service_uri, token=self.token, auth_org=self.auth_org)
 
     def list_repos(self, org: str) -> Sequence[str]:
         """List all repositories for the specified org
 
         Args:
             org: Name of the org
         """
```

### Comparing `arraylake_client-0.4.2/arraylake_client/commits.py` & `arraylake_client-0.4.3/arraylake_client/commits.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/arraylake_client/config.py` & `arraylake_client-0.4.3/arraylake_client/config.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/arraylake_client/log_util.py` & `arraylake_client-0.4.3/arraylake_client/log_util.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/arraylake_client/metastore/abc.py` & `arraylake_client-0.4.3/arraylake_client/metastore/abc.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/arraylake_client/metastore/http_metastore.py` & `arraylake_client-0.4.3/arraylake_client/metastore/http_metastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 @dataclass
 class HttpMetastoreConfig:
     """Encapsulates the configuration for the HttpMetastore"""
 
     api_service_url: str
     org: str
     token: str = field(default=None, repr=False)  # machine token. id/access/refresh tokens are managed by CustomOauth
+    auth_org: str = None
 
 
 class HttpMetastore(ArraylakeHttpClient, Metastore):
     """ArrayLake's HTTP Metastore
 
     This metastore connects to ArrayLake over HTTP
 
@@ -72,15 +73,15 @@
     Authenticated calls require an Authorization header. Run ``arraylake auth login`` to login before using this metastore.
     :::
     """
 
     _config: HttpMetastoreConfig
 
     def __init__(self, config: HttpMetastoreConfig):
-        super().__init__(config.api_service_url, token=config.token)
+        super().__init__(config.api_service_url, token=config.token, hint=config.auth_org)
 
         self._config = config
         self.api_url = config.api_service_url
 
     async def ping(self) -> dict:
         async with self:
             response = await self._request("GET", "user")
@@ -144,28 +145,34 @@
         args:
             config: config for the metastore database
 
         :::note
         Authenticated calls require an Authorization header. Run ``arraylake auth login`` to login before using this metastore.
         :::
         """
-        super().__init__(config.http_metastore_config.api_service_url, token=config.http_metastore_config.token)
+        super().__init__(
+            config.http_metastore_config.api_service_url,
+            token=config.http_metastore_config.token,
+            hint=config.http_metastore_config.auth_org,
+        )
 
         self._config = config
         self._setup()
 
     def _setup(self):
         self._repo_path = f"/repos/{self._config.http_metastore_config.org}/{self._config.repo}"
         self._doc_cache = LRUCache(maxsize=10000)
 
     def __getstate__(self):
         return self._config
 
     def __setstate__(self, state):
-        super().__init__(state.http_metastore_config.api_service_url, token=state.http_metastore_config.token)
+        super().__init__(
+            state.http_metastore_config.api_service_url, token=state.http_metastore_config.token, hint=state.http_metastore_config.auth_org
+        )
         self._config = state
         self._setup()
 
     def __repr__(self):
         status = "OPEN" if self._OPEN else "CLOSED"
         full_name = f"{self._config.http_metastore_config.org}/{self._config.repo}"
         return f"<arraylake_client.http_metastore.HttpMetastoreDatabase repo_name='{full_name}' status={status}>"
```

### Comparing `arraylake_client-0.4.2/arraylake_client/repo.py` & `arraylake_client-0.4.3/arraylake_client/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 from arraylake_client.async_utils import (
     BlockingPortal,
     BlockingPortalGenerator,
     cached_portal,
 )
 from arraylake_client.chunkstore import Chunkstore
-from arraylake_client.commits import CommitData, CommitLog, CommitTree
+from arraylake_client.commits import CommitData, CommitLog
 from arraylake_client.exceptions import (
     CommitFailedError,
     DocumentNotFoundError,
     InvalidPrefixError,
 )
 from arraylake_client.log_util import get_logger
 from arraylake_client.metastore import MetastoreDatabase
@@ -179,37 +179,47 @@
         return self
 
     async def __aexit__(self, *args, **kwargs):
         await self.db.__aexit__(*args, **kwargs)
         await self.chunkstore.__aexit__(*args, **kwargs)
         self._OPEN = False
 
+    def __getstate__(self):
+        return self.db, self.chunkstore, self.repo_name, self.author, self._session, self._OPEN, self._writable
+
+    def __setstate__(self, state):
+        self.db, self.chunkstore, self.repo_name, self.author, self._session, self._OPEN, self._writable = state
+        # commit_data can be large and is not needed for most operations, therefore we omit it during serialization.
+        self._commit_data = None
+
     def __repr__(self):
         repo_name = self.repo_name
         status = "OPEN" if self._OPEN else "CLOSED"
         return f"<arraylake_client.repo.AsyncRepo name='{repo_name}' status={status}>"
 
     @property
     def session(self) -> SessionInfo:
         # accessing the session via this property makes mypy happy
         if self._session is None:
             raise ValueError("There is no session active. You have to call checkout first.")
         return self._session
 
-    @property
-    def commit_data(self) -> CommitData:
+    async def commit_data(self) -> CommitData:
+        """Returns the #CommitData for the current session."""
         if self._commit_data is None:
-            raise ValueError("You check out a branch to see the commit log.")
+            if not self._OPEN:
+                raise ValueError("must be in async context to fetch commit_data")
+            # lazily refresh commit data
+            await self._refresh_commit_data()
         return self._commit_data
 
-    @property
-    def commit_log(self) -> CommitLog:
+    async def commit_log(self) -> CommitLog:
         """Returns the #CommitLog for the current session."""
 
-        return CommitLog(self.repo_name, self.session["base_commit"], self.commit_data)
+        return CommitLog(self.repo_name, self.session["base_commit"], await self.commit_data())
 
     async def status(self, limit: int = 1000) -> SessionStatus:
         """Returns the #SessionStatus for the current session.
 
         Args:
             limit (int): [Optional] The number of modified paths to return. Defaults to 1000, passing 0
             is equivalent to setting no limit.
@@ -239,28 +249,26 @@
             ref: Commit, branch, or tag name
 
         Returns:
             commit: #CommitID
         """
 
         await self._refresh_commit_data()
-        commit_data = self.commit_data
-        commit, branch = self.commit_data.get_ref(ref)
+        commit, branch = (await self.commit_data()).get_ref(ref)
 
         session_start_time = datetime.datetime.utcnow()
         # TODO: replace this with a pydantic model
         self._session = {"id": SessionID(uuid.uuid4().hex), "start_time": session_start_time, "base_commit": commit, "branch": branch}
 
         if branch is None:
             warnings.warn("You are not on a branch tip, so you can't commit changes.")
             self._writable = False
         else:
             self._writable = True
 
-        self._commit_tree = CommitTree(commit, commit_data.commits) if commit else None
         return commit
 
     async def commit(self, message: str, auto_ff=True) -> CommitID:
         """Commit this session's changes and start a new session.
 
         Args:
             message: Commit message
@@ -299,15 +307,15 @@
         except ValueError as err:
             if str(err).startswith("No changes to commit"):
                 warnings.warn(str(err))
                 return self.session.get("base_commit", None)
             else:
                 raise err
 
-        new_branch = (self.session["branch"] not in self.commit_data.branches) or (self.session["base_commit"] is None)
+        new_branch = (self.session["branch"] not in (await self.commit_data()).branches) or (self.session["base_commit"] is None)
         try:
             await self.db.update_branch(
                 self.session["branch"], base_commit=self.session["base_commit"], new_commit=new_commit, new_branch=new_branch
             )
         except Exception:
             raise CommitFailedError(f"Failed to update branch {self.session['branch']} to point to commit {new_commit}")
 
@@ -332,15 +340,15 @@
         # returns the ID to ff to
 
         if self.session["branch"] is None:
             raise RuntimeError("Fast-forward unavailable: You are not on a branch tip")
 
         await self._refresh_commit_data()
         branch = self.session["branch"]
-        branch_latest_commit = self._commit_data.branches.get(branch, None)
+        branch_latest_commit = (await self.commit_data()).branches.get(branch, None)
         session_base_commit = self._session["base_commit"]
 
         if branch_latest_commit is None:
             # that branch has seen no commits yet
             return branch_latest_commit
 
         if branch_latest_commit == session_base_commit:
@@ -352,41 +360,41 @@
         # paths of other sessions later in the logic of fast forwarding
         modified_paths = set([spr.path async for spr in self._modified(limit=0)])
         if len(modified_paths) == 0:
             # nothing changed; nothing to do
             return branch_latest_commit
 
         # this is different from self.commit_log because it starts from branch_latest_commit
-        commit_log = CommitLog(self.repo_name, branch_latest_commit, self.commit_data)
+        commit_log = CommitLog(self.repo_name, branch_latest_commit, await self.commit_data())
         upstream_modifications = set()
         for commit in commit_log:
             if commit.id == session_base_commit:
                 # we can stop iterating
                 break
             for collection in (metadata_collection, chunks_collection):
                 upstream_modifications.update(
                     {response.path async for response in self.db.get_all_paths_for_session(commit.session_id, collection=collection)}
                 )
         conflicting_paths = upstream_modifications & modified_paths
         if conflicting_paths:
             raise RuntimeError(f"Can't fast-forward due to conflicting paths {conflicting_paths}.")
         return branch_latest_commit
 
-    def new_branch(self, branch_name: str) -> None:
+    async def new_branch(self, branch_name: str) -> None:
         """Create a new branch based on the current session reference
 
         Args:
             branch_name: New branch name
         """
 
         branch = BranchName(branch_name)
         if self._session is None:
             # this was added to make mypy happy but is not covered by tests
             raise ValueError("There is no session active. You have to call checkout first.")
-        if branch in self.commit_data.branches or branch == self.session["branch"]:
+        if branch in (await self.commit_data()).branches or branch == self.session["branch"]:
             raise ValueError(f"Branch {branch} already exists.")
         self._session["branch"] = branch
 
     @_write_op
     async def _set_doc(self, path: Path, *, content: dict) -> None:
         """Write a single document to the metastore
 
@@ -1024,15 +1032,15 @@
     def new_branch(self, branch: str) -> None:
         """Create a new branch based on the current session reference
 
         Args:
             branch_name: New branch name
         """
 
-        return self._arepo.new_branch(branch)
+        return self._synchronize(self._arepo.new_branch, branch)
 
     # TODO: figure out some clever metaclass way of wrapping all of these methods
     # For now it's faster to just plug and chug
     def _set_doc(self, path: Path, *, content: dict) -> None:
         return self._synchronize(self._arepo._set_doc, path, content=content)
 
     def _set_docs(self, items: Mapping[str, dict]) -> None:
@@ -1113,15 +1121,15 @@
         Args:
            limit (int): [Optional] The number of modified paths to return. Defaults to 1000, passing 0
            is equivalent to setting no limit."""
         return self._synchronize(self._arepo.status, limit=limit)
 
     @property
     def commit_log(self):
-        return self._arepo.commit_log
+        return self._synchronize(self._arepo.commit_log)
 
     def add_virtual_hdf(self, path: Path, hdf_uri: str) -> None:
         """Add a virtual HDF5 dataset to the arraylake.
 
         Args:
             path: The path with the repo where the virtual HDF5 dataset should be created.
             hdf_uri: The path to the HDF5 file. Only `s3://` URIs are supported at the moment.
```

### Comparing `arraylake_client-0.4.2/arraylake_client/spec.py` & `arraylake_client-0.4.3/arraylake_client/spec.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/arraylake_client/token.py` & `arraylake_client-0.4.3/arraylake_client/token.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,19 +20,21 @@
 
     token_path: pathlib.Path
     tokens: Optional[OauthTokens]
 
     def __init__(
         self,
         api_endpoint: str = "https://api.earthmover.io",
+        hint: str = None,
         scopes: List[str] = ["email", "openid", "profile"],
         raise_if_not_logged_in: bool = False,
     ):
         self.api_endpoint = api_endpoint
         self.scopes = scopes
+        self.hint = hint
 
         self.token_path = pathlib.Path(config.get("service.token_path", None) or "~/.arraylake/token.json").expanduser()
         self.default_headers = {"accept": "application/vnd.earthmover+json"}
 
         # get cached tokens
         self.tokens = None
         try:
@@ -43,31 +45,36 @@
         except FileNotFoundError:
             if raise_if_not_logged_in:
                 raise AuthException("Not logged in, please log in with `arraylake auth login`")
 
     async def get_authorize_url(self) -> str:
         body = {"scopes": self.scopes}
         async with httpx.AsyncClient() as client:
-            response = await client.post(f"{self.api_endpoint}/login", json=body, headers=self.default_headers)
+            params = {"hint": self.hint} if self.hint else {}
+            response = await client.post(f"{self.api_endpoint}/login", json=body, headers=self.default_headers, params=params)
         if response.status_code != httpx.codes.OK:
             raise AuthException("failed to get authorization url")
 
         return response.json()["url"]
 
     async def get_token(self, code: str):
         params = {"code": code}
+        if self.hint:
+            params["hint"] = self.hint
         async with httpx.AsyncClient() as client:
             response = await client.get(f"{self.api_endpoint}/token", params=params, headers=self.default_headers)
         if response.status_code != httpx.codes.OK:
             raise AuthException("unable to get token")
         new_token_data = OauthTokens.parse_obj(response.json())
         self.update(new_token_data)
 
     async def refresh_token(self):
         params = {"token": self.tokens.refresh_token.get_secret_value()}
+        if self.hint:
+            params["hint"] = self.hint
         async with httpx.AsyncClient() as client:
             response = await client.get(f"{self.api_endpoint}/refresh_token", params=params, headers=self.default_headers)
         if response.status_code == httpx.codes.OK:
             # a refresh token is persisted over time
             # performing a fresh yields a new id + access token
             # perform an update with the new values, but maintain
             # the refresh token
@@ -96,12 +103,16 @@
             raise ValueError("Error saving tokens, no tokens to cache")
         self.token_path.parent.mkdir(exist_ok=True)
         with self.token_path.open(mode="w") as fp:
             fp.write(self.tokens.json(exclude_unset=True))
         self.token_path.chmod(0o100600)  # -rw-------
 
     def get_logout_url(self) -> str:
-        return f"{self.api_endpoint}/logout"
+        endpoint = f"{self.api_endpoint}/logout"
+        if self.hint:
+            return f"{self.api_endpoint}/logout?hint={self.hint}"
+        else:
+            return endpoint
 
     def purge_cache(self):
         self.token_path.unlink()
         self.tokens = None
```

### Comparing `arraylake_client-0.4.2/arraylake_client/types.py` & `arraylake_client-0.4.3/arraylake_client/types.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/arraylake_client/virtual.py` & `arraylake_client-0.4.3/arraylake_client/virtual.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/arraylake_client/zarr_util.py` & `arraylake_client-0.4.3/arraylake_client/zarr_util.py`

 * *Files identical despite different names*

### Comparing `arraylake_client-0.4.2/pyproject.toml` & `arraylake_client-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "arraylake-client"
-version = "0.4.2"  # placeholder
+version = "0.4.3"  # placeholder
 description = "Python client for ArrayLake"
 authors = ["Joe Hamman <joe@earthmover.io>"]
 readme = "README.md"
 packages = [{include = "arraylake_client"}]
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `arraylake_client-0.4.2/PKG-INFO` & `arraylake_client-0.4.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arraylake-client
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python client for ArrayLake
 Author: Joe Hamman
 Author-email: joe@earthmover.io
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -32,25 +32,25 @@
 Requires-Dist: types-aiobotocore (>=2.4.0,<3.0.0)
 Requires-Dist: zarr (>=2.14,<2.15)
 Description-Content-Type: text/markdown
 
 # arraylake-client
 
 <p align="center">
-<img src="https://preview.earthmover.io/img/Earthmover_Main_Logo_1130x625.png" width="200" alt="Earthmover">
+<img src="https://earthmover-web-assets.s3.amazonaws.com/04-Arraylake-Lockup-Midnight-RGB-LARGE.png" width="200" alt="Arraylake">
 </p>
 
 <p align="center">
-  <a href="https://preview.earthmover.io" rel="nofollow">earthmover.io</a> -
-  <a href="https://preview.earthmover.io/docs/overview" rel="nofollow">documentation</a>
+  <a href="https://earthmover.io" rel="nofollow">earthmover.io</a> -
+  <a href="https://docs.earthmover.io" rel="nofollow">documentation</a>
 </p>
 
 Arraylake is a cloud-based platform that understands a wide array of multidimensional scientific data. Organize, analyze, build, and collaborate—effortlessly.
 
-Checkout the [documentation](https://preview.earthmover.io/docs/overview) to get started.
+Checkout the [documentation](https://docs.earthmover.io) to get started.
 
 ## Install
 
 ```
 pip install "arraylake_client[cli]"
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: arraylake-client Version: 0.4.2 Summary: Python
+Metadata-Version: 2.1 Name: arraylake-client Version: 0.4.3 Summary: Python
 client for ArrayLake Author: Joe Hamman Author-email: joe@earthmover.io
 Requires-Python: >=3.8,<3.11 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: cli Provides-Extra: virtual Provides-Extra: widgets Requires-
 Dist: aiobotocore[boto3] (>=2.4.0,<3.0.0) Requires-Dist: anyio (>=3.6.1,<4.0.0)
 Requires-Dist: cachetools (>=5.3.0,<6.0.0) Requires-Dist: donfig (>=0.7,<1.0)
@@ -13,14 +13,14 @@
 Requires-Dist: pydantic[email] (>=1.10,<2.0) Requires-Dist: pymongo
 (>=4.2.0,<5.0.0) Requires-Dist: rich (>=12.6,<14.0) ; extra == "cli" Requires-
 Dist: ruamel-yaml (>=0.17,<1.0) ; extra == "cli" Requires-Dist: s3fs
 (>=2022.11.0) ; extra == "virtual" Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Requires-Dist: typer (>=0.6.1,<1.0) ; extra == "cli" Requires-Dist: types-
 aiobotocore (>=2.4.0,<3.0.0) Requires-Dist: zarr (>=2.14,<2.15) Description-
 Content-Type: text/markdown # arraylake-client
-                                 [Earthmover]
+                                  [Arraylake]
                          earthmover.io - documentation
 Arraylake is a cloud-based platform that understands a wide array of
 multidimensional scientific data. Organize, analyze, build, and
 collaborateâeffortlessly. Checkout the [documentation](https://
-preview.earthmover.io/docs/overview) to get started. ## Install ``` pip install
+docs.earthmover.io) to get started. ## Install ``` pip install
 "arraylake_client[cli]" ```
```

