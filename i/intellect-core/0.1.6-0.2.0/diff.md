# Comparing `tmp/intellect_core-0.1.6.tar.gz` & `tmp/intellect_core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intellect_core-0.1.6.tar", max compression
+gzip compressed data, was "intellect_core-0.2.0.tar", max compression
```

## Comparing `intellect_core-0.1.6.tar` & `intellect_core-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      186 2023-06-16 13:35:23.642011 intellect_core-0.1.6/LICENSE
--rw-r--r--   0        0        0      171 2023-06-16 13:35:23.642011 intellect_core-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-06-16 13:35:23.642011 intellect_core-0.1.6/intellect_core/dto/__init__.py
--rw-r--r--   0        0        0     2365 2023-06-16 13:35:23.642011 intellect_core-0.1.6/intellect_core/dto/dto.py
--rw-r--r--   0        0        0     1023 2023-06-16 13:35:23.642011 intellect_core-0.1.6/intellect_core/handler.py
--rw-r--r--   0        0        0     5575 2023-06-16 13:48:23.616950 intellect_core-0.1.6/intellect_core/intelletct_server.py
--rw-r--r--   0        0        0      307 2023-06-16 13:35:52.589973 intellect_core-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-07-04 13:46:17.485985 intellect_core-0.2.0/LICENSE
+-rw-r--r--   0        0        0      171 2023-07-04 13:46:17.485985 intellect_core-0.2.0/README.md
+-rw-r--r--   0        0        0     4669 2023-07-11 08:28:49.672801 intellect_core-0.2.0/intellect_core/core.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:46:17.485985 intellect_core-0.2.0/intellect_core/dto/__init__.py
+-rw-r--r--   0        0        0     2455 2023-07-11 08:10:50.016455 intellect_core-0.2.0/intellect_core/dto/dto.py
+-rw-r--r--   0        0        0     1023 2023-07-11 08:28:49.676801 intellect_core-0.2.0/intellect_core/handler.py
+-rw-r--r--   0        0        0     5677 2023-07-10 14:37:51.809736 intellect_core-0.2.0/intellect_core/intelletct_server.py
+-rw-r--r--   0        0        0      366 2023-07-11 08:49:59.238211 intellect_core-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.2.0/PKG-INFO
```

### Comparing `intellect_core-0.1.6/intellect_core/dto/dto.py` & `intellect_core-0.2.0/intellect_core/dto/dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,18 @@
 class IntellectConfigDto(BaseModel):
     intellect_host: str
     intellect_port: int
     host_user: str
     host_password: str
     token_expires: int  # seconds
     access_level: int
-    access_department_id: int  # for temp pass
+    access_department_id: int
+    https: bool = False
+    certificate_path: str | None = None
+    retry_to_connection_in_minute: int = 2
     enable_integration: bool
 
 
 class IntellectVisitDto:
     class Create(BaseModel):
         objid: int
         name: str | None  # second_name
```

### Comparing `intellect_core-0.1.6/intellect_core/handler.py` & `intellect_core-0.2.0/intellect_core/handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from enum import Enum
 from typing import Dict
 
 
-
 class IntellectError(Exception):
     error_type: str = "IntellectIntegrationError"
     default_class: int = 999
     default_subclass: int = 999
     context: Dict[str, str | int] = None
 
     def __init__(self, ex=None, message=None, context=None):
@@ -34,8 +33,8 @@
 class ErrorClass(Enum):
     CREATE_OR_UPDATE = 1
     DELETE = 2
 
 
 class ErrorSubClass(Enum):
     DTO_NOT_FOUND = 1
-    OBJECT_ID_NOT_FOUND = 2
+    OBJECT_ID_NOT_FOUND = 2
```

### Comparing `intellect_core-0.1.6/intellect_core/intelletct_server.py` & `intellect_core-0.2.0/intellect_core/intelletct_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,21 +10,23 @@
     ObjectType, \
     IntellectVisitDto, \
     AutarizationInfo, \
     IntellectDepartmentDto
 from intellect_core.handler import IntellectError, ErrorClass, ErrorSubClass
 
 
-class IntellectWebServer:
+class IntellectDefault:
     log_debug: bool = False
     config: IntellectConfigDto
     autarization_info: AutarizationInfo | None
     expire_token_date: str
 
 
+class IntellectWebServer(IntellectDefault):
+
     # =====================================================================================================================
 
     async def _wrap_response(self, response: ClientResponse):
         await response.read()
         if (await response.json()).get("Status") == "ERROR":
             logger.error(await response.json())
         if self.log_debug:
@@ -44,15 +46,14 @@
         else:
             url = url + f"objid<{objid}>"
             return url
 
     # =====================================================================================================================
     async def autorization(self):
         timeout = ClientTimeout(total=10)
-
         async with ClientSession(timeout=timeout) as session:
             url = f"http://{self.config.host_user}:{self.config.host_password}@{self.config.intellect_host}:{self.config.intellect_port}/token?expires_in={self.config.token_expires}"
             logger.debug(url)
             try:
                 async with session.request(method="GET", url=url) as response:
                     string = "{" + (await response.text()).replace("\n", ",")[2:-2] + "}"
                     self.autarization_info = AutarizationInfo(**json.loads(string))
@@ -78,30 +79,30 @@
                          IntellectDepartmentDto.Update = None,
                     objid: int = None) -> None:
         session = ClientSession()
         match command:
             case CoreCommand.CREATE | CoreCommand.UPDATE:
                 if dto:
                     dto.level_id = self.config.access_level
-                    url = self._get_url(object_type, command, dto, None)
+                    url = self._get_url(object_type=object_type, command=command, dto=dto, objid=None)
                     try:
                         async with session.request(method="GET", url=url) as response:
                             await self._wrap_response(response)
                             await session.close()
                     except OSError as e:
                         await session.close()
                         logger.error(f"Intellect connection error: {e}")
                 else:
                     await session.close()
                     raise IntellectError(message="You need set dto for update or create object",
                                          context={"class": ErrorClass.CREATE_OR_UPDATE,
                                                   "subclass": ErrorSubClass.DTO_NOT_FOUND})
             case CoreCommand.DELETE:
                 if objid:
-                    url = self._get_url(object_type, command, None, objid)
+                    url = self._get_url(object_type=object_type, command=command, dto=None, objid=objid)
                     try:
                         async with session.request(method="GET",
                                                    url=url) as response:
                             await self._wrap_response(response)
                             await session.close()
                     except OSError as e:
                         await session.close()
```

### Comparing `intellect_core-0.1.6/PKG-INFO` & `intellect_core-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intellect-core
-Version: 0.1.6
+Version: 0.2.0
 Summary: Модуль интеграции с Интеллект
 Author: Mrkorogod
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

