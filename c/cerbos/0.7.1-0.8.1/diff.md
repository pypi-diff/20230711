# Comparing `tmp/cerbos-0.7.1.tar.gz` & `tmp/cerbos-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbos-0.7.1.tar", last modified: Wed Jun  7 09:41:56 2023, max compression
+gzip compressed data, was "cerbos-0.8.1.tar", last modified: Tue Jul 11 14:52:08 2023, max compression
```

## Comparing `cerbos-0.7.1.tar` & `cerbos-0.8.1.tar`

### file list

```diff
@@ -1,37 +1,74 @@
--rw-r--r--   0        0        0    11357 2023-06-07 09:41:27.981043 cerbos-0.7.1/LICENSE
--rw-r--r--   0        0        0     2999 2023-06-07 09:41:27.981043 cerbos-0.7.1/README.md
--rw-r--r--   0        0        0      167 2023-06-07 09:41:27.981043 cerbos-0.7.1/cerbos/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 09:41:27.981043 cerbos-0.7.1/cerbos/sdk/__init__.py
--rw-r--r--   0        0        0    12680 2023-06-07 09:41:27.981043 cerbos-0.7.1/cerbos/sdk/_async/client.py
--rw-r--r--   0        0        0    12492 2023-06-07 09:41:55.481730 cerbos-0.7.1/cerbos/sdk/_sync/client.py
--rw-r--r--   0        0        0      485 2023-06-07 09:41:27.981043 cerbos-0.7.1/cerbos/sdk/client.py
--rw-r--r--   0        0        0      759 2023-06-07 09:41:27.981043 cerbos-0.7.1/cerbos/sdk/container.py
--rw-r--r--   0        0        0     6414 2023-06-07 09:41:27.981043 cerbos-0.7.1/cerbos/sdk/model.py
--rw-r--r--   0        0        0     1800 2023-06-07 09:41:27.981043 cerbos-0.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 09:41:27.981043 cerbos-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0     1303 2023-06-07 09:41:27.981043 cerbos-0.7.1/tests/check.py
--rw-r--r--   0        0        0     2017 2023-06-07 09:41:27.981043 cerbos-0.7.1/tests/conftest.py
--rw-r--r--   0        0        0      578 2023-06-07 09:41:27.981043 cerbos-0.7.1/tests/store/_schemas/leave_request.json
--rw-r--r--   0        0        0     1030 2023-06-07 09:41:27.981043 cerbos-0.7.1/tests/store/_schemas/principal.json
--rw-r--r--   0        0        0      402 2023-06-07 09:41:27.981043 cerbos-0.7.1/tests/store/_schemas/purchase_order.json
--rw-r--r--   0        0        0      387 2023-06-07 09:41:27.981043 cerbos-0.7.1/tests/store/_schemas/salary_record.json
--rw-r--r--   0        0        0      451 2023-06-07 09:41:27.981043 cerbos-0.7.1/tests/store/derived_roles/common_roles.yaml
--rw-r--r--   0        0        0      323 2023-06-07 09:41:27.981043 cerbos-0.7.1/tests/store/derived_roles/derived_roles_01.yaml
--rw-r--r--   0        0        0      492 2023-06-07 09:41:27.981043 cerbos-0.7.1/tests/store/derived_roles/derived_roles_02.yaml
--rw-r--r--   0        0        0      599 2023-06-07 09:41:27.981043 cerbos-0.7.1/tests/store/derived_roles/derived_roles_03.yaml
--rw-r--r--   0        0        0      577 2023-06-07 09:41:27.981043 cerbos-0.7.1/tests/store/principal_policies/policy_01.yaml
--rw-r--r--   0        0        0      300 2023-06-07 09:41:27.981043 cerbos-0.7.1/tests/store/principal_policies/policy_02.yaml
--rw-r--r--   0        0        0      226 2023-06-07 09:41:27.981043 cerbos-0.7.1/tests/store/principal_policies/policy_02_acme.hr.yaml
--rw-r--r--   0        0        0      499 2023-06-07 09:41:27.981043 cerbos-0.7.1/tests/store/principal_policies/policy_02_acme.yaml
--rw-r--r--   0        0        0     2090 2023-06-07 09:41:27.985043 cerbos-0.7.1/tests/store/resource_policies/policy_01.yaml
--rw-r--r--   0        0        0      624 2023-06-07 09:41:27.985043 cerbos-0.7.1/tests/store/resource_policies/policy_02.yaml
--rw-r--r--   0        0        0      526 2023-06-07 09:41:27.985043 cerbos-0.7.1/tests/store/resource_policies/policy_03.yaml
--rw-r--r--   0        0        0      689 2023-06-07 09:41:27.985043 cerbos-0.7.1/tests/store/resource_policies/policy_04.yaml
--rw-r--r--   0        0        0      377 2023-06-07 09:41:27.985043 cerbos-0.7.1/tests/store/resource_policies/policy_05.yaml
--rw-r--r--   0        0        0      704 2023-06-07 09:41:27.985043 cerbos-0.7.1/tests/store/resource_policies/policy_05_acme.hr.uk.yaml
--rw-r--r--   0        0        0     1138 2023-06-07 09:41:27.985043 cerbos-0.7.1/tests/store/resource_policies/policy_05_acme.hr.yaml
--rw-r--r--   0        0        0      535 2023-06-07 09:41:27.985043 cerbos-0.7.1/tests/store/resource_policies/policy_05_acme.yaml
--rw-r--r--   0        0        0      450 2023-06-07 09:41:27.985043 cerbos-0.7.1/tests/store/tests/policy_04_test.yaml
--rw-r--r--   0        0        0    20302 2023-06-07 09:41:27.985043 cerbos-0.7.1/tests/test_client.py
--rw-r--r--   0        0        0     2061 2023-06-07 09:41:27.985043 cerbos-0.7.1/tests/test_plan_response.py
--rw-r--r--   0        0        0     3538 1970-01-01 00:00:00.000000 cerbos-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 14:51:34.962167 cerbos-0.8.1/LICENSE
+-rw-r--r--   0        0        0     6175 2023-07-11 14:51:34.962167 cerbos-0.8.1/README.md
+-rw-r--r--   0        0        0      167 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/__init__.py
+-rw-r--r--   0        0        0     5052 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/audit/v1/audit_pb2.py
+-rw-r--r--   0        0        0     5463 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/audit/v1/audit_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/audit/v1/audit_pb2_grpc.py
+-rw-r--r--   0        0        0     1537 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/effect/v1/effect_pb2.py
+-rw-r--r--   0        0        0      541 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/effect/v1/effect_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/effect/v1/effect_pb2_grpc.py
+-rw-r--r--   0        0        0    24465 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/engine/v1/engine_pb2.py
+-rw-r--r--   0        0        0    18348 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/engine/v1/engine_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/engine/v1/engine_pb2_grpc.py
+-rw-r--r--   0        0        0    33169 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/policy/v1/policy_pb2.py
+-rw-r--r--   0        0        0    29198 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/policy/v1/policy_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/policy/v1/policy_pb2_grpc.py
+-rw-r--r--   0        0        0    40721 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/request/v1/request_pb2.py
+-rw-r--r--   0        0        0    14880 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/request/v1/request_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/request/v1/request_pb2_grpc.py
+-rw-r--r--   0        0        0    40197 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/response/v1/response_pb2.py
+-rw-r--r--   0        0        0    20863 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/response/v1/response_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/response/v1/response_pb2_grpc.py
+-rw-r--r--   0        0        0     3055 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/schema/v1/schema_pb2.py
+-rw-r--r--   0        0        0     1614 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/schema/v1/schema_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/schema/v1/schema_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/_async/__init__.py
+-rw-r--r--   0        0        0    24037 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/_async/_grpc.py
+-rw-r--r--   0        0        0    12739 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/_async/_http.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:52:05.371922 cerbos-0.8.1/cerbos/sdk/_sync/__init__.py
+-rw-r--r--   0        0        0    23695 2023-07-11 14:52:06.371980 cerbos-0.8.1/cerbos/sdk/_sync/_grpc.py
+-rw-r--r--   0        0        0    12551 2023-07-11 14:52:05.371922 cerbos-0.8.1/cerbos/sdk/_sync/_http.py
+-rw-r--r--   0        0        0      481 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/client.py
+-rw-r--r--   0        0        0      881 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/container.py
+-rw-r--r--   0        0        0      491 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/grpc/client.py
+-rw-r--r--   0        0        0      702 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/grpc/utils.py
+-rw-r--r--   0        0        0      106 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/http/client.py
+-rw-r--r--   0        0        0     6501 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/sdk/model.py
+-rw-r--r--   0        0        0    14057 2023-07-11 14:51:34.962167 cerbos-0.8.1/cerbos/svc/v1/svc_pb2.py
+-rw-r--r--   0        0        0      449 2023-07-11 14:51:34.966168 cerbos-0.8.1/cerbos/svc/v1/svc_pb2.pyi
+-rw-r--r--   0        0        0    38288 2023-07-11 14:51:34.966168 cerbos-0.8.1/cerbos/svc/v1/svc_pb2_grpc.py
+-rw-r--r--   0        0        0     9422 2023-07-11 14:51:34.966168 cerbos-0.8.1/cerbos/telemetry/v1/telemetry_pb2.py
+-rw-r--r--   0        0        0    10796 2023-07-11 14:51:34.966168 cerbos-0.8.1/cerbos/telemetry/v1/telemetry_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-11 14:51:34.966168 cerbos-0.8.1/cerbos/telemetry/v1/telemetry_pb2_grpc.py
+-rw-r--r--   0        0        0     2695 2023-07-11 14:52:08.268090 cerbos-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/__init__.py
+-rw-r--r--   0        0        0     1303 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/check.py
+-rw-r--r--   0        0        0     4868 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/conftest.py
+-rw-r--r--   0        0        0     6496 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/grpc/test_grpc_admin_client.py
+-rw-r--r--   0        0        0    15671 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/grpc/test_grpc_client.py
+-rw-r--r--   0        0        0    20088 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/http/test_http_client.py
+-rw-r--r--   0        0        0     2061 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/http/test_http_plan_response.py
+-rw-r--r--   0        0        0      758 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/conf.yaml
+-rw-r--r--   0        0        0      578 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/_schemas/leave_request.json
+-rw-r--r--   0        0        0     1030 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/_schemas/principal.json
+-rw-r--r--   0        0        0      402 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/_schemas/purchase_order.json
+-rw-r--r--   0        0        0      387 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/_schemas/salary_record.json
+-rw-r--r--   0        0        0      451 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/derived_roles/common_roles.yaml
+-rw-r--r--   0        0        0      323 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/derived_roles/derived_roles_01.yaml
+-rw-r--r--   0        0        0      492 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/derived_roles/derived_roles_02.yaml
+-rw-r--r--   0        0        0      599 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/derived_roles/derived_roles_03.yaml
+-rw-r--r--   0        0        0      577 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/principal_policies/policy_01.yaml
+-rw-r--r--   0        0        0      300 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/principal_policies/policy_02.yaml
+-rw-r--r--   0        0        0      226 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/principal_policies/policy_02_acme.hr.yaml
+-rw-r--r--   0        0        0      499 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/principal_policies/policy_02_acme.yaml
+-rw-r--r--   0        0        0     2090 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_01.yaml
+-rw-r--r--   0        0        0      624 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_02.yaml
+-rw-r--r--   0        0        0      526 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_03.yaml
+-rw-r--r--   0        0        0      689 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_04.yaml
+-rw-r--r--   0        0        0      377 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_05.yaml
+-rw-r--r--   0        0        0      704 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_05_acme.hr.uk.yaml
+-rw-r--r--   0        0        0     1138 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_05_acme.hr.yaml
+-rw-r--r--   0        0        0      535 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/resource_policies/policy_05_acme.yaml
+-rw-r--r--   0        0        0      450 2023-07-11 14:51:34.966168 cerbos-0.8.1/tests/store/policies/tests/policy_04_test.yaml
+-rw-r--r--   0        0        0     6987 1970-01-01 00:00:00.000000 cerbos-0.8.1/PKG-INFO
```

### Comparing `cerbos-0.7.1/LICENSE` & `cerbos-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cerbos-0.7.1/cerbos/sdk/_async/client.py` & `cerbos-0.8.1/cerbos/sdk/_async/_http.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,18 @@
         resp = await self.check_resources(
             principal=principal,
             resources=ResourceList().add(resource, {action}),
             request_id=request_id,
             aux_data=aux_data,
         )
 
-        return resp.get_resource(resource.id).is_allowed(action)
+        if (r := resp.get_resource(resource.id)) is not None:
+            return r.is_allowed(action)
+
+        return False
 
     async def plan_resources(
         self,
         action: str,
         principal: Principal,
         resource: ResourceDesc,
         request_id: Optional[str] = None,
```

### Comparing `cerbos-0.7.1/cerbos/sdk/_sync/client.py` & `cerbos-0.8.1/cerbos/sdk/_sync/_http.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,15 +229,18 @@
         resp = self.check_resources(
             principal=principal,
             resources=ResourceList().add(resource, {action}),
             request_id=request_id,
             aux_data=aux_data,
         )
 
-        return resp.get_resource(resource.id).is_allowed(action)
+        if (r := resp.get_resource(resource.id)) is not None:
+            return r.is_allowed(action)
+
+        return False
 
     def plan_resources(
         self,
         action: str,
         principal: Principal,
         resource: ResourceDesc,
         request_id: Optional[str] = None,
```

### Comparing `cerbos-0.7.1/cerbos/sdk/container.py` & `cerbos-0.8.1/cerbos/sdk/container.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,9 +12,12 @@
     def __init__(self, image: str = "ghcr.io/cerbos/cerbos:latest"):
         super(CerbosContainer, self).__init__(image)
         self.with_exposed_ports(self.HTTP_PORT, self.GRPC_PORT)
 
     def http_host(self, protocol: str = "http") -> str:
         return f"{protocol}://{self.get_container_host_ip()}:{self.get_exposed_port(self.HTTP_PORT)}"
 
+    def grpc_host(self) -> str:
+        return f"{self.get_container_host_ip()}:{self.get_exposed_port(self.GRPC_PORT)}"
+
     def wait_until_ready(self, timeout_secs: float = 30):
         wait_for_logs(self, r"Starting HTTP server at", timeout=timeout_secs)
```

### Comparing `cerbos-0.7.1/cerbos/sdk/model.py` & `cerbos-0.8.1/cerbos/sdk/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,7 +266,15 @@
 
 class CerbosRequestException(Exception):
     def __init__(self, error: Optional[APIError]):
         msg = "unexpected error" if error is None else error.message
         super(CerbosRequestException, self).__init__(msg)
 
         self.error = error
+
+
+class CerbosTLSError(Exception):
+    ...
+
+
+class CerbosTypeError(Exception):
+    ...
```

### Comparing `cerbos-0.7.1/tests/check.py` & `cerbos-0.8.1/tests/check.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.7.1/tests/store/_schemas/leave_request.json` & `cerbos-0.8.1/tests/store/policies/_schemas/leave_request.json`

 * *Files identical despite different names*

### Comparing `cerbos-0.7.1/tests/store/_schemas/principal.json` & `cerbos-0.8.1/tests/store/policies/_schemas/principal.json`

 * *Files identical despite different names*

### Comparing `cerbos-0.7.1/tests/store/derived_roles/derived_roles_03.yaml` & `cerbos-0.8.1/tests/store/policies/derived_roles/derived_roles_03.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.7.1/tests/store/principal_policies/policy_01.yaml` & `cerbos-0.8.1/tests/store/policies/principal_policies/policy_01.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.7.1/tests/store/resource_policies/policy_01.yaml` & `cerbos-0.8.1/tests/store/policies/resource_policies/policy_01.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.7.1/tests/store/resource_policies/policy_02.yaml` & `cerbos-0.8.1/tests/store/policies/resource_policies/policy_02.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.7.1/tests/store/resource_policies/policy_03.yaml` & `cerbos-0.8.1/tests/store/policies/resource_policies/policy_03.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.7.1/tests/store/resource_policies/policy_04.yaml` & `cerbos-0.8.1/tests/store/policies/resource_policies/policy_04.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.7.1/tests/store/resource_policies/policy_05_acme.hr.uk.yaml` & `cerbos-0.8.1/tests/store/policies/resource_policies/policy_05_acme.hr.uk.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.7.1/tests/store/resource_policies/policy_05_acme.hr.yaml` & `cerbos-0.8.1/tests/store/policies/resource_policies/policy_05_acme.hr.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.7.1/tests/store/resource_policies/policy_05_acme.yaml` & `cerbos-0.8.1/tests/store/policies/resource_policies/policy_05_acme.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.7.1/tests/test_client.py` & `cerbos-0.8.1/tests/http/test_http_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,21 +526,16 @@
 def _assert_check_resources_principal_override_with_output(
     have: CheckResourcesResponse,
 ):
     xx125 = have.get_resource(
         "XX125", predicate=lambda r: r.policy_version == "20210210"
     )
     assert xx125 is not None
-    assert len(xx125.outputs) == 2
-    s = next(filter(lambda x: isinstance(x.val, str), xx125.outputs))
+    assert len(xx125.outputs) == 1
     d = next(filter(lambda x: isinstance(x.val, dict), xx125.outputs))
-    assert s.to_dict() == {
-        "src": "principal.donald_duck.v20210210#dev_admin",
-        "val": "dev_record_override:donald_duck",
-    }
     assert d.to_dict() == {
         "src": "resource.leave_request.v20210210#public-view",
         "val": {
             "formatted_string": "id:donald_duck",
             "keys": "XX125",
             "pID": "donald_duck",
             "some_bool": True,
```

### Comparing `cerbos-0.7.1/tests/test_plan_response.py` & `cerbos-0.8.1/tests/http/test_http_plan_response.py`

 * *Files identical despite different names*

