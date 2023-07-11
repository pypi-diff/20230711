# Comparing `tmp/stigg_api_client_v2-0.477.0.tar.gz` & `tmp/stigg_api_client_v2-0.481.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.477.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.481.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.477.0.tar` & `stigg_api_client_v2-0.481.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0     1644 2023-07-09 16:10:36.165369 stigg_api_client_v2-0.477.0/README.md
--rw-r--r--   0        0        0      432 2023-07-09 16:11:26.844503 stigg_api_client_v2-0.477.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-09 16:10:36.165369 stigg_api_client_v2-0.477.0/stigg/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-09 16:10:36.165369 stigg_api_client_v2-0.477.0/stigg/client.py
--rw-r--r--   0        0        0    39793 2023-07-09 16:11:24.848450 stigg_api_client_v2-0.477.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0     7303 2023-07-09 16:11:24.408421 stigg_api_client_v2-0.477.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    66833 2023-07-09 16:11:24.660437 stigg_api_client_v2-0.477.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-07-09 16:11:18.696077 stigg_api_client_v2-0.477.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-07-09 16:11:24.408421 stigg_api_client_v2-0.477.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-07-09 16:11:23.368352 stigg_api_client_v2-0.477.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-07-09 16:11:23.388353 stigg_api_client_v2-0.477.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    66418 2023-07-09 16:11:18.940091 stigg_api_client_v2-0.477.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-07-09 16:11:23.416355 stigg_api_client_v2-0.477.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    24176 2023-07-09 16:11:20.704194 stigg_api_client_v2-0.477.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-07-09 16:11:23.372352 stigg_api_client_v2-0.477.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-07-09 16:11:23.380353 stigg_api_client_v2-0.477.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-07-09 16:11:24.412421 stigg_api_client_v2-0.477.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    54916 2023-07-09 16:11:24.408421 stigg_api_client_v2-0.477.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-07-09 16:11:23.440357 stigg_api_client_v2-0.477.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-07-09 16:11:23.448357 stigg_api_client_v2-0.477.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-07-09 16:11:23.432356 stigg_api_client_v2-0.477.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-07-09 16:11:23.492360 stigg_api_client_v2-0.477.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-07-09 16:11:23.468359 stigg_api_client_v2-0.477.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-07-09 16:11:23.460358 stigg_api_client_v2-0.477.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-07-09 16:11:23.504361 stigg_api_client_v2-0.477.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-07-09 16:11:23.456358 stigg_api_client_v2-0.477.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-07-09 16:11:23.476359 stigg_api_client_v2-0.477.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-07-09 16:11:23.488360 stigg_api_client_v2-0.477.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-07-09 16:11:23.328349 stigg_api_client_v2-0.477.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-07-09 16:11:23.320349 stigg_api_client_v2-0.477.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-07-09 16:11:23.352351 stigg_api_client_v2-0.477.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   126250 2023-07-09 16:11:23.300348 stigg_api_client_v2-0.477.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-07-09 16:11:23.424356 stigg_api_client_v2-0.477.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-07-09 16:11:23.316349 stigg_api_client_v2-0.477.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-07-09 16:11:23.344350 stigg_api_client_v2-0.477.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-07-09 16:11:23.408355 stigg_api_client_v2-0.477.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-07-09 16:11:23.404354 stigg_api_client_v2-0.477.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-07-09 16:11:23.396354 stigg_api_client_v2-0.477.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-07-09 16:11:24.416421 stigg_api_client_v2-0.477.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-07-09 16:11:23.336350 stigg_api_client_v2-0.477.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-07-09 16:11:23.360352 stigg_api_client_v2-0.477.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-07-09 16:11:23.512362 stigg_api_client_v2-0.477.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.477.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-07-11 06:55:39.621086 stigg_api_client_v2-0.481.0/README.md
+-rw-r--r--   0        0        0      432 2023-07-11 06:56:31.177080 stigg_api_client_v2-0.481.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-11 06:55:39.621086 stigg_api_client_v2-0.481.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-11 06:55:39.621086 stigg_api_client_v2-0.481.0/stigg/client.py
+-rw-r--r--   0        0        0    39986 2023-07-11 06:56:29.513084 stigg_api_client_v2-0.481.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-11 06:56:28.173087 stigg_api_client_v2-0.481.0/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0     7303 2023-07-11 06:56:29.009085 stigg_api_client_v2-0.481.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    67443 2023-07-11 06:56:29.225085 stigg_api_client_v2-0.481.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-07-11 06:56:24.169113 stigg_api_client_v2-0.481.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-07-11 06:56:29.009085 stigg_api_client_v2-0.481.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-07-11 06:56:28.117087 stigg_api_client_v2-0.481.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-07-11 06:56:28.137087 stigg_api_client_v2-0.481.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    67016 2023-07-11 06:56:24.377113 stigg_api_client_v2-0.481.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-07-11 06:56:28.161087 stigg_api_client_v2-0.481.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24302 2023-07-11 06:56:25.885107 stigg_api_client_v2-0.481.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-07-11 06:56:28.125087 stigg_api_client_v2-0.481.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-07-11 06:56:28.133087 stigg_api_client_v2-0.481.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-07-11 06:56:29.009085 stigg_api_client_v2-0.481.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    54916 2023-07-11 06:56:29.009085 stigg_api_client_v2-0.481.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-07-11 06:56:28.185087 stigg_api_client_v2-0.481.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-07-11 06:56:28.197087 stigg_api_client_v2-0.481.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-07-11 06:56:28.181087 stigg_api_client_v2-0.481.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-07-11 06:56:28.233087 stigg_api_client_v2-0.481.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-07-11 06:56:28.209087 stigg_api_client_v2-0.481.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-07-11 06:56:28.205087 stigg_api_client_v2-0.481.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-07-11 06:56:28.245087 stigg_api_client_v2-0.481.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-07-11 06:56:28.201087 stigg_api_client_v2-0.481.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-07-11 06:56:28.217087 stigg_api_client_v2-0.481.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-07-11 06:56:28.229087 stigg_api_client_v2-0.481.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-07-11 06:56:28.085087 stigg_api_client_v2-0.481.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-07-11 06:56:28.081087 stigg_api_client_v2-0.481.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-07-11 06:56:28.105087 stigg_api_client_v2-0.481.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   126898 2023-07-11 06:56:28.061087 stigg_api_client_v2-0.481.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-07-11 06:56:28.169087 stigg_api_client_v2-0.481.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-07-11 06:56:28.073087 stigg_api_client_v2-0.481.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-07-11 06:56:28.101087 stigg_api_client_v2-0.481.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-07-11 06:56:28.153087 stigg_api_client_v2-0.481.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-07-11 06:56:28.149087 stigg_api_client_v2-0.481.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-07-11 06:56:28.145087 stigg_api_client_v2-0.481.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-07-11 06:56:29.013085 stigg_api_client_v2-0.481.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-07-11 06:56:28.089087 stigg_api_client_v2-0.481.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-07-11 06:56:28.113087 stigg_api_client_v2-0.481.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-07-11 06:56:28.249087 stigg_api_client_v2-0.481.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.481.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.477.0/README.md` & `stigg_api_client_v2-0.481.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.477.0/stigg/client.py` & `stigg_api_client_v2-0.481.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.481.0/stigg/generated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 
+from .archive_customer import ArchiveCustomer, ArchiveCustomerArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
     CancelSubscriptionCancelSubscription,
 )
@@ -334,14 +335,15 @@
     AddonFilter,
     AddonSort,
     AddonUpdateInput,
     Address,
     ApiKeyFilter,
     ApiKeySort,
     ArchiveCouponInput,
+    ArchiveCustomerInput,
     ArchivePlanInput,
     AttachCustomerPaymentMethodInput,
     BillableFeatureInput,
     BillingModelFilterComparison,
     BillingPeriodFilterComparison,
     BooleanFieldComparison,
     CheckoutOptions,
@@ -623,14 +625,17 @@
     "AggregationFunction",
     "Alignment",
     "ApiKeyFilter",
     "ApiKeySort",
     "ApiKeySortFields",
     "ApiKeyType",
     "ArchiveCouponInput",
+    "ArchiveCustomer",
+    "ArchiveCustomerArchiveCustomer",
+    "ArchiveCustomerInput",
     "ArchivePlanInput",
     "AsyncBaseClient",
     "AsyncClient",
     "AttachCustomerPaymentMethodInput",
     "BaseModel",
     "BillableFeatureInput",
     "BillingAnchor",
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.481.0/stigg/generated/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/async_client.py` & `stigg_api_client_v2-0.481.0/stigg/generated/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
+from .archive_customer import ArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
 from .estimate_subscription import EstimateSubscription
 from .estimate_subscription_update import EstimateSubscriptionUpdate
 from .get_active_subscriptions import GetActiveSubscriptions
@@ -17,14 +18,15 @@
 from .get_paywall import GetPaywall
 from .get_products import GetProducts
 from .get_sdk_configuration import GetSdkConfiguration
 from .import_customer import ImportCustomer
 from .import_customer_bulk import ImportCustomerBulk
 from .import_subscriptions_bulk import ImportSubscriptionsBulk
 from .input_types import (
+    ArchiveCustomerInput,
     CustomerPortalInput,
     EntitlementCheckRequested,
     EstimateSubscriptionInput,
     EstimateSubscriptionUpdateInput,
     FetchEntitlementQuery,
     FetchEntitlementsQuery,
     GetActiveSubscriptionsInput,
@@ -888,14 +890,29 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return MigrateSubscriptionToLatest.parse_obj(data)
 
+    async def archive_customer(self, input: ArchiveCustomerInput) -> ArchiveCustomer:
+        query = gql(
+            """
+            mutation ArchiveCustomer($input: ArchiveCustomerInput!) {
+              archiveCustomer(input: $input) {
+                customerId
+              }
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return ArchiveCustomer.parse_obj(data)
+
     async def get_customer_by_id(
         self, input: GetCustomerByRefIdInput
     ) -> GetCustomerById:
         query = gql(
             """
             query GetCustomerById($input: GetCustomerByRefIdInput!) {
               getCustomerByRefId(input: $input) {
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/base_client.py` & `stigg_api_client_v2-0.481.0/stigg/generated/base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.481.0/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.481.0/stigg/generated/cancel_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/client.py` & `stigg_api_client_v2-0.481.0/stigg/generated/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
+from .archive_customer import ArchiveCustomer
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
 from .estimate_subscription import EstimateSubscription
 from .estimate_subscription_update import EstimateSubscriptionUpdate
 from .get_active_subscriptions import GetActiveSubscriptions
@@ -17,14 +18,15 @@
 from .get_paywall import GetPaywall
 from .get_products import GetProducts
 from .get_sdk_configuration import GetSdkConfiguration
 from .import_customer import ImportCustomer
 from .import_customer_bulk import ImportCustomerBulk
 from .import_subscriptions_bulk import ImportSubscriptionsBulk
 from .input_types import (
+    ArchiveCustomerInput,
     CustomerPortalInput,
     EntitlementCheckRequested,
     EstimateSubscriptionInput,
     EstimateSubscriptionUpdateInput,
     FetchEntitlementQuery,
     FetchEntitlementsQuery,
     GetActiveSubscriptionsInput,
@@ -882,14 +884,29 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return MigrateSubscriptionToLatest.parse_obj(data)
 
+    def archive_customer(self, input: ArchiveCustomerInput) -> ArchiveCustomer:
+        query = gql(
+            """
+            mutation ArchiveCustomer($input: ArchiveCustomerInput!) {
+              archiveCustomer(input: $input) {
+                customerId
+              }
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return ArchiveCustomer.parse_obj(data)
+
     def get_customer_by_id(self, input: GetCustomerByRefIdInput) -> GetCustomerById:
         query = gql(
             """
             query GetCustomerById($input: GetCustomerByRefIdInput!) {
               getCustomerByRefId(input: $input) {
                 ...CustomerWithSubscriptionsFragment
               }
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.481.0/stigg/generated/update_subscription.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
 
 
-class CreateSubscription(BaseModel):
-    create_subscription: "CreateSubscriptionCreateSubscription" = Field(
-        alias="createSubscription"
+class UpdateSubscription(BaseModel):
+    update_subscription: "UpdateSubscriptionUpdateSubscription" = Field(
+        alias="updateSubscription"
     )
 
 
-class CreateSubscriptionCreateSubscription(SlimSubscriptionFragment):
+class UpdateSubscriptionUpdateSubscription(SlimSubscriptionFragment):
     pass
 
 
-CreateSubscription.update_forward_refs()
-CreateSubscriptionCreateSubscription.update_forward_refs()
+UpdateSubscription.update_forward_refs()
+UpdateSubscriptionUpdateSubscription.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.481.0/stigg/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
+    CustomerIsArchived = "CustomerIsArchived"
     CustomerNotFound = "CustomerNotFound"
     CustomerResourceNotFound = "CustomerResourceNotFound"
     FeatureNotFound = "FeatureNotFound"
     NoActiveSubscription = "NoActiveSubscription"
     NoFeatureEntitlementInSubscription = "NoFeatureEntitlementInSubscription"
     RequestedUsageExceedingLimit = "RequestedUsageExceedingLimit"
     Unknown = "Unknown"
@@ -243,14 +244,15 @@
 class CustomerSortFields(str, Enum):
     billingId = "billingId"
     createdAt = "createdAt"
     crmHubspotCompanyId = "crmHubspotCompanyId"
     crmHubspotCompanyUrl = "crmHubspotCompanyUrl"
     crmId = "crmId"
     customerId = "customerId"
+    deletedAt = "deletedAt"
     email = "email"
     environmentId = "environmentId"
     id = "id"
     name = "name"
     refId = "refId"
     updatedAt = "updatedAt"
 
@@ -350,14 +352,15 @@
     CustomerResourceNotFound = "CustomerResourceNotFound"
     DowngradeBillingPeriodNotSupportedError = "DowngradeBillingPeriodNotSupportedError"
     DraftPlanCantBeArchived = "DraftPlanCantBeArchived"
     DuplicatedEntityNotAllowed = "DuplicatedEntityNotAllowed"
     EditAllowedOnDraftPackageOnlyError = "EditAllowedOnDraftPackageOnlyError"
     EntitlementsMustBelongToSamePackage = "EntitlementsMustBelongToSamePackage"
     EntityIdDifferentFromRefIdError = "EntityIdDifferentFromRefIdError"
+    EntityIsArchivedError = "EntityIsArchivedError"
     EnvironmentMissing = "EnvironmentMissing"
     ExperimentAlreadyRunning = "ExperimentAlreadyRunning"
     ExperimentNotFoundError = "ExperimentNotFoundError"
     ExperimentStatusError = "ExperimentStatusError"
     FailedToCreateCheckoutSessionError = "FailedToCreateCheckoutSessionError"
     FailedToImportCustomer = "FailedToImportCustomer"
     FeatureNotFound = "FeatureNotFound"
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.481.0/stigg/generated/estimate_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.481.0/stigg/generated/estimate_subscription_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.481.0/stigg/generated/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.481.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -32,36 +32,14 @@
     VendorIdentifier,
     WeeklyAccordingTo,
     WidgetType,
     experimentGroupType,
 )
 
 
-class PackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    feature_id: str = Field(alias="featureId")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    is_custom: Optional[bool] = Field(alias="isCustom")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: "PackageEntitlementFragmentFeature"
-
-
-class PackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class PriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -77,14 +55,36 @@
 class PriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
+class PackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    feature_id: str = Field(alias="featureId")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    is_custom: Optional[bool] = Field(alias="isCustom")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: "PackageEntitlementFragmentFeature"
+
+
+class PackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class AddonFragment(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     billing_id: Optional[str] = Field(alias="billingId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
@@ -124,25 +124,14 @@
     status: SyncStatus
 
 
 class CouponFragmentCustomers(BaseModel):
     id: str
 
 
-class SlimCustomerFragment(BaseModel):
-    id: str
-    name: Optional[str]
-    email: Optional[str]
-    created_at: Optional[Any] = Field(alias="createdAt")
-    updated_at: Any = Field(alias="updatedAt")
-    ref_id: str = Field(alias="refId")
-    billing_id: Optional[str] = Field(alias="billingId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class PromotionalEntitlementFragment(BaseModel):
     status: PromotionalEntitlementStatus
     usage_limit: Optional[float] = Field(alias="usageLimit")
     feature_id: str = Field(alias="featureId")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -157,14 +146,25 @@
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     ref_id: str = Field(alias="refId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
 
 
+class SlimCustomerFragment(BaseModel):
+    id: str
+    name: Optional[str]
+    email: Optional[str]
+    created_at: Optional[Any] = Field(alias="createdAt")
+    updated_at: Any = Field(alias="updatedAt")
+    ref_id: str = Field(alias="refId")
+    billing_id: Optional[str] = Field(alias="billingId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class CustomerFragment(SlimCustomerFragment):
     has_payment_method: bool = Field(alias="hasPaymentMethod")
     has_active_subscription: bool = Field(alias="hasActiveSubscription")
     default_payment_expiration_month: Optional[int] = Field(
         alias="defaultPaymentExpirationMonth"
     )
     default_payment_expiration_year: Optional[int] = Field(
@@ -328,21 +328,23 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
-class CustomerPortalPromotionalEntitlement(BaseModel):
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
     display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
+    quantity: int
 
 
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
@@ -388,21 +390,14 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
-    display_name: str = Field(alias="displayName")
-    quantity: int
-
-
 class CustomerPortalSubscriptionPriceFragment(BaseModel):
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     billing_model: Optional[BillingModel] = Field(alias="billingModel")
     price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
     feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
 
 
@@ -500,16 +495,21 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
+class CustomerPortalPromotionalEntitlement(BaseModel):
+    display_name: str = Field(alias="displayName")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
 
 
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
@@ -842,14 +842,34 @@
 class LayoutConfigurationFragment(BaseModel):
     alignment: Optional[Alignment]
     plan_width: Optional[float] = Field(alias="planWidth")
     plan_margin: Optional[float] = Field(alias="planMargin")
     plan_padding: Optional[float] = Field(alias="planPadding")
 
 
+class MockPaywallPackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
+
+
+class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class MockPaywallPriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -864,34 +884,14 @@
 
 class MockPaywallPriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
 
 
-class MockPaywallPackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: bool = Field(alias="hasUnlimitedUsage")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: Optional["MockPaywallPackageEntitlementFragmentFeature"]
-
-
-class MockPaywallPackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class MockPaywallAddonFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     billing_id: Optional[str] = Field(alias="billingId")
     entitlements: List["MockPaywallAddonFragmentEntitlements"]
@@ -1311,28 +1311,28 @@
 
 class UsageHistoryFragmentUsageMeasurements(BaseModel):
     date: Any
     value: float
     is_reset_point: Optional[bool] = Field(alias="isResetPoint")
 
 
-PackageEntitlementFragment.update_forward_refs()
-PackageEntitlementFragmentFeature.update_forward_refs()
 PriceFragment.update_forward_refs()
 PriceFragmentPrice.update_forward_refs()
 PriceFragmentFeature.update_forward_refs()
+PackageEntitlementFragment.update_forward_refs()
+PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
-SlimCustomerFragment.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
 PromotionalEntitlementFragmentFeature.update_forward_refs()
+SlimCustomerFragment.update_forward_refs()
 CustomerFragment.update_forward_refs()
 CustomerFragmentTrialedPlans.update_forward_refs()
 CustomerFragmentExperimentInfo.update_forward_refs()
 CustomerFragmentCoupon.update_forward_refs()
 CustomerFragmentEligibleForTrial.update_forward_refs()
 CustomerFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalBillingInformation.update_forward_refs()
@@ -1346,21 +1346,21 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionPriceFragment.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPrices.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
@@ -1368,15 +1368,15 @@
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
-CustomerResourceFragment.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
@@ -1418,19 +1418,19 @@
 UsageUpdatedFragment.update_forward_refs()
 EntitlementUsageUpdated.update_forward_refs()
 EntitlementUsageUpdatedUsage.update_forward_refs()
 EntitlementUsageUpdatedEntitlement.update_forward_refs()
 EntitlementsUpdatedPayload.update_forward_refs()
 EntitlementsUpdatedPayloadEntitlements.update_forward_refs()
 LayoutConfigurationFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragment.update_forward_refs()
+MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallPriceFragment.update_forward_refs()
 MockPaywallPriceFragmentPrice.update_forward_refs()
 MockPaywallPriceFragmentFeature.update_forward_refs()
-MockPaywallPackageEntitlementFragment.update_forward_refs()
-MockPaywallPackageEntitlementFragmentFeature.update_forward_refs()
 MockPaywallAddonFragment.update_forward_refs()
 MockPaywallAddonFragmentEntitlements.update_forward_refs()
 MockPaywallAddonFragmentPrices.update_forward_refs()
 MockPaywallPlanFragment.update_forward_refs()
 MockPaywallPlanFragmentProduct.update_forward_refs()
 MockPaywallPlanFragmentBasePlan.update_forward_refs()
 MockPaywallPlanFragmentEntitlements.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.481.0/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.481.0/stigg/generated/get_coupons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.481.0/stigg/generated/get_customer_by_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.481.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.481.0/stigg/generated/get_mock_paywall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.481.0/stigg/generated/get_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.481.0/stigg/generated/get_sdk_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.481.0/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -152,14 +152,19 @@
 
 
 class ArchiveCouponInput(BaseModel):
     environment_id: Optional[str] = Field(alias="environmentId")
     ref_id: str = Field(alias="refId")
 
 
+class ArchiveCustomerInput(BaseModel):
+    customer_id: str = Field(alias="customerId")
+    environment_id: Optional[str] = Field(alias="environmentId")
+
+
 class ArchivePlanInput(BaseModel):
     environment_id: Optional[str] = Field(alias="environmentId")
     id: str
 
 
 class AttachCustomerPaymentMethodInput(BaseModel):
     customer_id: Optional[str] = Field(alias="customerId")
@@ -259,14 +264,15 @@
         alias="crmHubspotCompanyId"
     )
     crm_hubspot_company_url: Optional["StringFieldComparison"] = Field(
         alias="crmHubspotCompanyUrl"
     )
     crm_id: Optional["StringFieldComparison"] = Field(alias="crmId")
     customer_id: Optional["StringFieldComparison"] = Field(alias="customerId")
+    deleted_at: Optional["DateFieldComparison"] = Field(alias="deletedAt")
     email: Optional["StringFieldComparison"]
     environment_id: Optional["StringFieldComparison"] = Field(alias="environmentId")
     id: Optional["StringFieldComparison"]
     name: Optional["StringFieldComparison"]
     or_: Optional[List["CouponFilterCustomerFilter"]] = Field(alias="or")
     ref_id: Optional["StringFieldComparison"] = Field(alias="refId")
     updated_at: Optional["DateFieldComparison"] = Field(alias="updatedAt")
@@ -448,14 +454,15 @@
         alias="crmHubspotCompanyId"
     )
     crm_hubspot_company_url: Optional["StringFieldComparison"] = Field(
         alias="crmHubspotCompanyUrl"
     )
     crm_id: Optional["StringFieldComparison"] = Field(alias="crmId")
     customer_id: Optional["StringFieldComparison"] = Field(alias="customerId")
+    deleted_at: Optional["DateFieldComparison"] = Field(alias="deletedAt")
     email: Optional["StringFieldComparison"]
     environment_id: Optional["StringFieldComparison"] = Field(alias="environmentId")
     id: Optional["StringFieldComparison"]
     name: Optional["StringFieldComparison"]
     or_: Optional[List["CustomerFilter"]] = Field(alias="or")
     promotional_entitlements: Optional[
         "CustomerFilterPromotionalEntitlementFilter"
@@ -565,14 +572,15 @@
         alias="crmHubspotCompanyId"
     )
     crm_hubspot_company_url: Optional["StringFieldComparison"] = Field(
         alias="crmHubspotCompanyUrl"
     )
     crm_id: Optional["StringFieldComparison"] = Field(alias="crmId")
     customer_id: Optional["StringFieldComparison"] = Field(alias="customerId")
+    deleted_at: Optional["DateFieldComparison"] = Field(alias="deletedAt")
     email: Optional["StringFieldComparison"]
     environment_id: Optional["StringFieldComparison"] = Field(alias="environmentId")
     id: Optional["StringFieldComparison"]
     name: Optional["StringFieldComparison"]
     or_: Optional[List["CustomerResourceFilterCustomerFilter"]] = Field(alias="or")
     ref_id: Optional["StringFieldComparison"] = Field(alias="refId")
     updated_at: Optional["DateFieldComparison"] = Field(alias="updatedAt")
@@ -666,14 +674,15 @@
         alias="crmHubspotCompanyId"
     )
     crm_hubspot_company_url: Optional["StringFieldComparison"] = Field(
         alias="crmHubspotCompanyUrl"
     )
     crm_id: Optional["StringFieldComparison"] = Field(alias="crmId")
     customer_id: Optional["StringFieldComparison"] = Field(alias="customerId")
+    deleted_at: Optional["DateFieldComparison"] = Field(alias="deletedAt")
     email: Optional["StringFieldComparison"]
     environment_id: Optional["StringFieldComparison"] = Field(alias="environmentId")
     id: Optional["StringFieldComparison"]
     name: Optional["StringFieldComparison"]
     or_: Optional[List["CustomerSubscriptionFilterCustomerFilter"]] = Field(alias="or")
     ref_id: Optional["StringFieldComparison"] = Field(alias="refId")
     updated_at: Optional["DateFieldComparison"] = Field(alias="updatedAt")
@@ -948,14 +957,15 @@
         alias="crmHubspotCompanyId"
     )
     crm_hubspot_company_url: Optional["StringFieldComparison"] = Field(
         alias="crmHubspotCompanyUrl"
     )
     crm_id: Optional["StringFieldComparison"] = Field(alias="crmId")
     customer_id: Optional["StringFieldComparison"] = Field(alias="customerId")
+    deleted_at: Optional["DateFieldComparison"] = Field(alias="deletedAt")
     email: Optional["StringFieldComparison"]
     environment_id: Optional["StringFieldComparison"] = Field(alias="environmentId")
     id: Optional["StringFieldComparison"]
     name: Optional["StringFieldComparison"]
     or_: Optional[List["ExperimentFilterCustomerFilter"]] = Field(alias="or")
     ref_id: Optional["StringFieldComparison"] = Field(alias="refId")
     updated_at: Optional["DateFieldComparison"] = Field(alias="updatedAt")
@@ -2692,14 +2702,15 @@
         alias="crmHubspotCompanyId"
     )
     crm_hubspot_company_url: Optional["StringFieldComparison"] = Field(
         alias="crmHubspotCompanyUrl"
     )
     crm_id: Optional["StringFieldComparison"] = Field(alias="crmId")
     customer_id: Optional["StringFieldComparison"] = Field(alias="customerId")
+    deleted_at: Optional["DateFieldComparison"] = Field(alias="deletedAt")
     email: Optional["StringFieldComparison"]
     environment_id: Optional["StringFieldComparison"] = Field(alias="environmentId")
     id: Optional["StringFieldComparison"]
     name: Optional["StringFieldComparison"]
     or_: Optional[List["UsageMeasurementFilterCustomerFilter"]] = Field(alias="or")
     ref_id: Optional["StringFieldComparison"] = Field(alias="refId")
     updated_at: Optional["DateFieldComparison"] = Field(alias="updatedAt")
@@ -2770,14 +2781,15 @@
 AddonFilter.update_forward_refs()
 AddonSort.update_forward_refs()
 AddonUpdateInput.update_forward_refs()
 Address.update_forward_refs()
 ApiKeyFilter.update_forward_refs()
 ApiKeySort.update_forward_refs()
 ArchiveCouponInput.update_forward_refs()
+ArchiveCustomerInput.update_forward_refs()
 ArchivePlanInput.update_forward_refs()
 AttachCustomerPaymentMethodInput.update_forward_refs()
 BillableFeatureInput.update_forward_refs()
 BillingModelFilterComparison.update_forward_refs()
 BillingPeriodFilterComparison.update_forward_refs()
 BooleanFieldComparison.update_forward_refs()
 CheckoutOptions.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.481.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.481.0/stigg/generated/provision_customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.481.0/stigg/generated/provision_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.477.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.481.0/stigg/generated/report_usage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-09 16:11
+# Generated by ariadne-codegen on 2023-07-11 06:56
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.477.0/PKG-INFO` & `stigg_api_client_v2-0.481.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.477.0
+Version: 0.481.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

