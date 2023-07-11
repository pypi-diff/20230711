# Comparing `tmp/pymagento-1.7.3.tar.gz` & `tmp/pymagento-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymagento-1.7.3.tar", max compression
+gzip compressed data, was "pymagento-1.7.4.tar", max compression
```

## Comparing `pymagento-1.7.3.tar` & `pymagento-1.7.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-07-10 08:43:14.596912 pymagento-1.7.3/LICENSE
--rw-r--r--   0        0        0      908 2023-07-10 08:43:14.596912 pymagento-1.7.3/README.md
--rw-r--r--   0        0        0     1189 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/__init__.py
--rw-r--r--   0        0        0     4773 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/attributes.py
--rw-r--r--   0        0        0     3849 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/batches.py
--rw-r--r--   0        0        0    37320 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/client.py
--rw-r--r--   0        0        0     1768 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/exceptions.py
--rw-r--r--   0        0        0      963 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/order_helpers.py
--rw-r--r--   0        0        0        0 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/py.typed
--rw-r--r--   0        0        0     3374 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/queries.py
--rw-r--r--   0        0        0      357 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/types.py
--rw-r--r--   0        0        0       22 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/version.py
--rw-r--r--   0        0        0     1219 2023-07-10 08:43:14.596912 pymagento-1.7.3/pyproject.toml
--rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 pymagento-1.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-11 10:24:57.697958 pymagento-1.7.4/LICENSE
+-rw-r--r--   0        0        0      908 2023-07-11 10:24:57.697958 pymagento-1.7.4/README.md
+-rw-r--r--   0        0        0     1189 2023-07-11 10:24:57.697958 pymagento-1.7.4/magento/__init__.py
+-rw-r--r--   0        0        0     4773 2023-07-11 10:24:57.697958 pymagento-1.7.4/magento/attributes.py
+-rw-r--r--   0        0        0     3849 2023-07-11 10:24:57.697958 pymagento-1.7.4/magento/batches.py
+-rw-r--r--   0        0        0    38318 2023-07-11 10:24:57.697958 pymagento-1.7.4/magento/client.py
+-rw-r--r--   0        0        0     1768 2023-07-11 10:24:57.697958 pymagento-1.7.4/magento/exceptions.py
+-rw-r--r--   0        0        0      963 2023-07-11 10:24:57.697958 pymagento-1.7.4/magento/order_helpers.py
+-rw-r--r--   0        0        0        0 2023-07-11 10:24:57.697958 pymagento-1.7.4/magento/py.typed
+-rw-r--r--   0        0        0     3374 2023-07-11 10:24:57.697958 pymagento-1.7.4/magento/queries.py
+-rw-r--r--   0        0        0      357 2023-07-11 10:24:57.697958 pymagento-1.7.4/magento/types.py
+-rw-r--r--   0        0        0       22 2023-07-11 10:24:57.697958 pymagento-1.7.4/magento/version.py
+-rw-r--r--   0        0        0     1218 2023-07-11 10:24:57.697958 pymagento-1.7.4/pyproject.toml
+-rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 pymagento-1.7.4/PKG-INFO
```

### Comparing `pymagento-1.7.3/LICENSE` & `pymagento-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.3/README.md` & `pymagento-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.3/magento/__init__.py` & `pymagento-1.7.4/magento/__init__.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.3/magento/attributes.py` & `pymagento-1.7.4/magento/attributes.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.3/magento/batches.py` & `pymagento-1.7.4/magento/batches.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.3/magento/client.py` & `pymagento-1.7.4/magento/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from json.decoder import JSONDecodeError
 from logging import Logger
 import time
 from os import environ
 from typing import Optional, Sequence, Dict, Union, cast, Iterator, Iterable, List
-from datetime import timedelta
+
 from api_session import APISession, JSONDict
 import requests
 from requests.exceptions import HTTPError
 
 from magento.types import Product, SourceItem, Sku, Category, MediaEntry, MagentoEntity, Order, PathId
 from magento.version import __version__
 from magento.exceptions import MagentoException, MagentoAssertionError
@@ -84,51 +84,56 @@
     """
     Client for the Magento API.
     """
     # default batch size for paginated requests
     # Note increasing it doesn’t create a significant time improvement.
     # For example, in one test on Bixoto in 2021, getting 2k products using a page size of 1k took 28s.
     # The same query with a page size of 2k still took 26s.
+    # Magento supports setting hard limits on this:
+    #   https://developer.adobe.com/commerce/webapi/get-started/api-security/
     PAGE_SIZE = 1000
 
-    # default is 4 hours for admin tokens (the ones we use)
-    TOKEN_LIFETIME = timedelta(hours=3)
-
     def __init__(self,
                  token: Optional[str] = None,
                  base_url: Optional[str] = None,
                  scope: Optional[str] = None,
                  logger: Optional[Logger] = None,
                  read_only=False,
                  user_agent=None,
+                 *,
+                 batch_page_size: Optional[int] = None,
                  **kwargs):
         """
         Create a Magento client instance. All arguments are optional and fall back on environment variables named
         ``PYMAGENTO_ + argument.upper()`` (``PYMAGENTO_TOKEN``, ``PYMAGENTO_BASE_URL``, etc).
         The ``token`` and ``base_url`` **must** be given either as arguments or environment variables.
 
         :param token: API integration token
         :param base_url: base URL of the Magento instance
-        :param scope: API scope
+        :param scope: API scope. Default on ``PYMAGENTO_SCOPE`` if set, or ``"all"``
+        :param batch_page_size: if set, override the default page size used for batch queries.
         :param logger: optional logger.
-        :param read_only: if True,
+        :param read_only:
         :param user_agent: User-Agent
         """
         token = token or environ.get("PYMAGENTO_TOKEN")
         base_url = base_url or environ.get("PYMAGENTO_BASE_URL")
         scope = scope or environ.get("PYMAGENTO_SCOPE") or DEFAULT_SCOPE
         user_agent = user_agent or environ.get("PYMAGENTO_USER_AGENT") or USER_AGENT
 
         if token is None:
             raise RuntimeError("Missing API token")
         if base_url is None:
             raise RuntimeError("Missing API base URL")
 
         super().__init__(base_url=base_url, user_agent=user_agent, read_only=read_only, **kwargs)
 
+        if batch_page_size is not None:
+            self.PAGE_SIZE = batch_page_size
+
         self.scope = scope
         self.logger = logger
         self.headers["Authorization"] = f"Bearer {token}"
 
     # Attributes
     # ==========
 
@@ -202,17 +207,14 @@
         Yield all categories.
         """
         return self.get_paginated("/V1/categories/list", query=query, limit=limit, **kwargs)
 
     def get_category(self, category_id: PathId) -> Optional[Category]:
         """
         Return a category given its id.
-
-        :param category_id:
-        :return:
         """
         return self.get_json_api(f"/V1/categories/{category_id}")
 
     def get_category_by_name(self, name: str) -> Optional[Category]:
         """
         Return the first category with the given name.
 
@@ -363,33 +365,50 @@
         Get an order given its (entity) id.
         """
         return self.get_api(f"/V1/orders/{order_id}", throw=throw).json()
 
     def get_order_by_increment_id(self, increment_id: str) -> Optional[Order]:
         """
         Get an order given its increment id. Return ``None`` if the order doesn’t exist.
-
-        :param increment_id:
-        :return:
         """
         query = make_field_value_query("increment_id", increment_id)
         for order in self.get_orders(query=query, limit=1):
             return order
         return None
 
     def hold_order(self, order_id: str, **kwargs):
+        """
+        Hold an order. This is the opposite of ``unhold_order``.
+
+        :param order_id: order id (not increment id)
+        """
         return self.post_api(f"/V1/orders/{order_id}/hold", **kwargs)
 
     def unhold_order(self, order_id: str, **kwargs):
+        """
+        Un-hold an order. This is the opposite of ``hold_order``.
+
+        :param order_id: order id (not increment id)
+        """
         return self.post_api(f"/V1/orders/{order_id}/unhold", **kwargs)
 
     def save_order(self, order: Order):
+        """Save an order."""
         return self.post_api(f"/V1/orders", json={"entity": order})
 
     def set_order_status(self, order: Order, status: str, *, external_order_id: Optional[str] = None):
+        """
+        Change the status of an order, and optionally set its ``ext_order_id``. This is a convenient wrapper around
+        ``save_order``.
+
+        :param order: order payload
+        :param status: new status
+        :param external_order_id: optional external order id
+        :return:
+        """
         payload = {
             "entity_id": order["entity_id"],
             "status": status,
             "increment_id": order["increment_id"],  # we need to repeat increment_id, otherwise it is regenerated
         }
         if external_order_id is not None:
             payload["ext_order_id"] = external_order_id
@@ -431,17 +450,14 @@
 
     # Special Prices
     # --------------
 
     def get_special_prices(self, skus: Sequence[Sku]) -> List[MagentoEntity]:
         """
         Get special prices for a sequence of SKUs.
-
-        :param skus:
-        :return:
         """
         return self.post_api("/V1/products/special-price-information",
                              json={"skus": skus}, throw=True, bypass_read_only=True).json()
 
     def save_special_prices(self, special_prices: Sequence[MagentoEntity]):
         """
         Save a sequence of special prices.
@@ -457,26 +473,20 @@
         :return:
         """
         return self.post_api("/V1/products/special-price", json={"prices": special_prices})
 
     def delete_special_prices(self, special_prices: Sequence[MagentoEntity]):
         """
         Delete a sequence of special prices.
-
-        :param special_prices:
-        :return:
         """
         return self.post_api("/V1/products/special-price-delete", json={"prices": special_prices})
 
     def delete_special_prices_by_sku(self, skus: Sequence[Sku]):
         """
-        Equivalent of `delete_special_prices(get_special_prices(skus))`.
-
-        :param skus:
-        :return:
+        Equivalent of ``delete_special_prices(get_special_prices(skus))``.
         """
         special_prices = self.get_special_prices(skus)
         return self.delete_special_prices(special_prices)
 
     # Products
     # ========
 
@@ -550,27 +560,39 @@
         """
         Return a gallery entry.
 
         :param sku: SKU of the product.
         :param entry_id:
         :return:
         """
+        # TODO: s/entry_id/media_id
         return self.get_json_api(f"/V1/products/{escape_path(sku)}/media/{entry_id}")
 
     def save_product_media(self, sku: Sku, media_entry: MediaEntry):
+        """
+        Save a product media.
+        """
         return self.post_api(f"/V1/products/{escape_path(sku)}/media", json={"entry": media_entry}, throw=True).json()
 
     def delete_product_media(self, sku: Sku, media_id: PathId, throw=False):
+        """
+        Delete a media associated with a product.
+
+        :param sku: SKU of the product
+        :param media_id:
+        :param throw:
+        :return:
+        """
         return self.delete_api(f"/V1/products/{escape_path(sku)}/media/{media_id}", throw=throw)
 
     def save_product(self, product, *, save_options: Optional[bool] = None) -> Product:
         """
         Save a product.
 
-        :param product: (partial) product to save.
+        :param product: product to save (can be partial).
         :param save_options: set the `saveOptions` attribute.
         :return:
         """
         payload: JSONDict = {"product": product}
         if save_options is not None:
             payload["saveOptions"] = save_options
 
@@ -752,15 +774,15 @@
         """Get all sales rules (generator)."""
         return self.get_paginated("/V1/salesRules/search", query=query, limit=limit, **kwargs)
 
     # Shipments
     # =========
 
     def get_shipments(self, *, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
-        """Return shipments."""
+        """Return shipments (generator)."""
         return self.get_paginated("/V1/shipments", query=query, limit=limit, **kwargs)
 
     def ship_order(self, order_id: PathId, payload: MagentoEntity):
         """
         Ship an order.
         """
         return self.post_api(f"/V1/order/{order_id}/ship", json=payload)
```

### Comparing `pymagento-1.7.3/magento/exceptions.py` & `pymagento-1.7.4/magento/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.3/magento/order_helpers.py` & `pymagento-1.7.4/magento/order_helpers.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.3/magento/queries.py` & `pymagento-1.7.4/magento/queries.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.3/pyproject.toml` & `pymagento-1.7.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymagento"
-version = "1.7.3"
+version = "1.7.4"
 description = "Python client for the Magento 2 API"
 authors = ["Bixoto <tech@bixoto.com>"]
 license = "MIT"
 homepage = "https://github.com/Bixoto/PyMagento"
 include = ["magento/py.typed"]
 readme = "README.md"
 packages = [
@@ -20,21 +20,21 @@
 python = "^3.8"
 api-session = "^1.3.2"
 # https://github.com/readthedocs/readthedocs.org/issues/4912
 # https://github.com/jacopok/mlgw_bns/commit/50e82ad2e218873d1b3a8732b6cbeb5f692dd14c
 Sphinx = {version="^4.4.0", optional=true}
 sphinx-rtd-theme = {version="^1.0.0", optional=true}
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 mypy = "^1"
-coverage = "^6.2"
-types-requests = "^2.26.2"
-pytest = "^6.2.5"
-pytest-mock = "^3.6.1"
-pytest-cov = "^3.0.0"
+coverage = "^7.2"
+types-requests = "^2.31"
+pytest = "^7.4"
+pytest-mock = "^3.11"
+pytest-cov = "^4.1"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinx-rtd-theme"]
 
 [tool.coverage.report]
 omit = ["tests/*"]
 exclude_lines = [
```

### Comparing `pymagento-1.7.3/PKG-INFO` & `pymagento-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymagento
-Version: 1.7.3
+Version: 1.7.4
 Summary: Python client for the Magento 2 API
 Home-page: https://github.com/Bixoto/PyMagento
 License: MIT
 Author: Bixoto
 Author-email: tech@bixoto.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

