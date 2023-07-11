# Comparing `tmp/pybigbuy-3.17.0.tar.gz` & `tmp/pybigbuy-3.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybigbuy-3.17.0.tar", max compression
+gzip compressed data, was "pybigbuy-3.18.0.tar", max compression
```

## Comparing `pybigbuy-3.17.0.tar` & `pybigbuy-3.18.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1062 2022-11-08 15:07:30.679412 pybigbuy-3.17.0/LICENSE
--rw-r--r--   0        0        0      456 2022-11-08 15:07:30.679412 pybigbuy-3.17.0/README.md
--rw-r--r--   0        0        0      630 2022-11-08 15:07:30.679412 pybigbuy-3.17.0/bigbuy/__init__.py
--rw-r--r--   0        0        0    24145 2022-11-08 15:07:30.679412 pybigbuy-3.17.0/bigbuy/api.py
--rw-r--r--   0        0        0    12934 2022-11-08 15:07:30.679412 pybigbuy-3.17.0/bigbuy/exceptions.py
--rw-r--r--   0        0        0        0 2022-11-08 15:07:30.679412 pybigbuy-3.17.0/bigbuy/py.typed
--rw-r--r--   0        0        0     1403 2022-11-08 15:07:30.679412 pybigbuy-3.17.0/bigbuy/rate_limit.py
--rw-r--r--   0        0        0      952 2022-11-08 15:07:30.679412 pybigbuy-3.17.0/pyproject.toml
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 pybigbuy-3.17.0/setup.py
--rw-r--r--   0        0        0     1165 1970-01-01 00:00:00.000000 pybigbuy-3.17.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/LICENSE
+-rw-r--r--   0        0        0      456 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/README.md
+-rw-r--r--   0        0        0      649 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/bigbuy/__init__.py
+-rw-r--r--   0        0        0    24609 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/bigbuy/api.py
+-rw-r--r--   0        0        0    12700 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/bigbuy/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/bigbuy/py.typed
+-rw-r--r--   0        0        0     1403 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/bigbuy/rate_limit.py
+-rw-r--r--   0        0        0      952 2023-07-11 11:03:13.718534 pybigbuy-3.18.0/pyproject.toml
+-rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 pybigbuy-3.18.0/PKG-INFO
```

### Comparing `pybigbuy-3.17.0/LICENSE` & `pybigbuy-3.18.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright © 2020-2022 – Bixoto.com
+Copyright © 2020-2023 – Bixoto.com
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `pybigbuy-3.17.0/bigbuy/__init__.py` & `pybigbuy-3.18.0/bigbuy/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 Bigbuy
 -------
 
 Bigbuy is a library for Python that wraps the BigBuy API.
 """
 
 __author__ = 'Bixoto <info@bixoto.com>'
-__version__ = '3.17.0'
+__version__ = '3.18.0'
 
 from .api import BigBuy
 from .exceptions import (
     BBError, BBResponseError, BBPackError, BBExportError, BBProductError, BBStockError,
     BBNoCarrierError, BBBankWireTooLowError, BBMoneyBoxTooLowError, BBTemporaryOrderError, BBOrderAlreadyExistsError,
     BBOrderTooLowError, BBIncorrectRefError, BBInvalidPaymentError, BBZipcodeFormatError, BBProductNotFoundError,
-    BBServerError, BBRateLimitError, BBValidationError,
-    wait_rate_limit,
+    BBServerError, BBRateLimitError, BBValidationError, BBWarehouseSplitError, BBShippingError,
 )
 from .rate_limit import RateLimit
```

### Comparing `pybigbuy-3.17.0/bigbuy/api.py` & `pybigbuy-3.18.0/bigbuy/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,18 @@
         """Get a single product by sku."""
         return self.get_json_api(f'catalog/productinformationbysku/{sku}', params=params)
 
     def get_products(self, **params):
         """Returns all products."""
         return self.get_json_api('catalog/products', params=params)
 
+    def get_new_products(self, **params):
+        """Returns new or republished products in the last 7 days."""
+        return self.get_json_api('catalog/new-products', params=params)
+
     def get_products_categories(self, **params):
         """Returns all products categories."""
         return self.get_json_api('catalog/productscategories', params=params)
 
     def get_products_images(self, **params):
         """Returns all products images."""
         return self.get_json_api('catalog/productsimages', params=params)
@@ -205,15 +209,15 @@
         payload = {
             "product_stock_request": {
                 "products": [{"sku": sku} for sku in skus],
             }
         }
         return self.post_api('catalog/productsstockbyreference', json=payload).json()
 
-    def get_products_tags(self, **params):
+    def get_products_tags(self, **params) -> List[dict]:
         """Lists all product tags."""
         return self.get_json_api('catalog/productstags', params=params)
 
     def get_product_stock(self, product_id: Id, **params):
         """Get a single product stock."""
         return self.get_json_api(f'catalog/productstock/{product_id}', params=params)
 
@@ -229,35 +233,35 @@
         """Returns all products variations stock by handling days."""
         return self.get_json_api('catalog/productsvariationsstockbyhandlingdays', params=params)
 
     def get_products_variations_stock_available(self, **params):
         """Returns all products variations stock available."""
         return self.get_json_api('catalog/productsvariationsstockavailable', params=params)
 
-    def get_product_tags(self, product_id: Id, **params):
-        """Get a single ProductTag."""
+    def get_product_tags(self, product_id: Id, **params) -> List[dict]:
+        """Get tags for a single product."""
         return self.get_json_api(f'catalog/producttags/{product_id}', params=params)
 
     def get_product_variations(self, product_id: Id, **params):
         """Get a single Product variations."""
         return self.get_json_api(f'catalog/productvariations/{product_id}', params=params)
 
     def get_product_variations_stock(self, product_id: Id, **params):
         """Get a single product variation stock."""
         return self.get_json_api(f'catalog/productvariationsstock/{product_id}', params=params)
 
-    def get_tag(self, tag_id: Id, **params):
+    def get_tag(self, tag_id: Id, **params) -> dict:
         """Get a single tag."""
         return self.get_json_api(f'catalog/tag/{tag_id}', params=params)
 
-    def get_tag_all_languages(self, tag_id: Id, **params):
+    def get_tag_all_languages(self, tag_id: Id, **params) -> List[dict]:
         """Get a single tag in all languages."""
         return self.get_json_api(f'catalog/tagalllanguages/{tag_id}', params=params)
 
-    def get_tags(self, **params):
+    def get_tags(self, **params) -> List[dict]:
         """Lists all tags."""
         return self.get_json_api('catalog/tags', params=params)
 
     def get_variation(self, variation_id: Id, **params):
         """Get a single variation."""
         return self.get_json_api(f'catalog/variation/{variation_id}', params=params)
 
@@ -475,14 +479,18 @@
             content = f.read()
 
         base64_content = base64.b64encode(content).decode("utf-8")
 
         return self.upload_order_invoice(order_id=order_id, file_b64_content=base64_content, mime_type=mime_type,
                                          concept=concept, amount=amount, **params)
 
+    def get_order_statuses(self, **params) -> List[JSONDict]:
+        """Get order statuses, as a list of dicts with "id" and "name" keys."""
+        return self.get_json_api("order/orderstatuses", **params)
+
     # tracking
     def get_tracking_carriers(self, **params):
         """Get the list of available carriers."""
         return self.get_json_api('tracking/carriers', **params)
 
     def get_tracking_order(self, order_id: Id, **params):
         """Get the list of available trackings."""
```

### Comparing `pybigbuy-3.17.0/bigbuy/exceptions.py` & `pybigbuy-3.18.0/bigbuy/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,22 +36,14 @@
 
 class BBRateLimitError(BBResponseError):
     def __init__(self, text: str, response: Response):
         super().__init__(text, response)
         self.rate_limit = RateLimit.from_response(response)
 
     # backward compatibility
-    @property
-    def reset_time(self):
-        if self.rate_limit is not None:
-            return self.rate_limit.reset_time
-
-        return None
-
-    # backward compatibility
     def reset_timedelta(self, utcnow: Optional[datetime] = None):
         if self.rate_limit is not None:
             dt = self.rate_limit.reset_timedelta(utcnow=utcnow)
             if dt <= timedelta(0):
                 return None
             return dt
 
@@ -124,18 +116,14 @@
 
 class BBWarehouseSplitError(BBShippingError):
     def __init__(self, *args, warehouses: Sequence[dict] = (), **kwargs):
         super().__init__(*args, **kwargs)
         self.warehouses = warehouses
 
 
-# Backward compatibility
-BBWarehouseError = BBWarehouseSplitError
-
-
 class BBInvalidPaymentError(BBResponseError):
     pass
 
 
 class BBBankWireTooLowError(BBResponseError):
     """
     bb_data: ``{"minBankwire": 0.00}``
@@ -256,15 +244,15 @@
 
 
 def raise_for_response(response: Response):
     """
     Equivalent of request.Response#raise_for_status() that raises an exception based on the response's status.
     This may modify its argument to fix the status code if the response is a soft error.
     """
-    text = response.text
+    text = response.text.strip()
     content = json_or_none(text)
 
     # BigBuy may return soft errors (with a '200 OK' code)
     if response.ok:
         # BigBuy may return soft errors (with a '200 OK' code)
         if isinstance(content, dict) and set(content) - {"error_detail", } == {"code", "message"}:
             code = content["code"]
@@ -299,31 +287,34 @@
                 text == "Bad Gateway":
             error_class = BBServerError
         else:
             error_class = BBResponseError
 
         # Trim what we can.
         if text.startswith("<html>") or text.startswith("<!DOCTYPE html>"):
-            # We may want to go further:
-            #   '<div class="container">
-            #       <h1>Oops! An Error Occurred</h1>
-            #       <h2>The server returned a "500 Internal Server Error".</h2>
-            #
-            #       <p>
-            #           Something is broken. Please let us know what you were doing when this error occurred.
-            #           We will fix it as soon as possible. Sorry for any inconvenience caused.
-            #       </p>
-            #   </div>'
             if m := re.match(r".+<body>(.+)</body>\s*</html>\s*", text, re.DOTALL):
                 text = m.group(1).strip()
 
                 # Trim "<h1>504 Gateway Time-out</h1>"
                 if m := re.match(r"<h1>5\d\d .+?</h1>(.+)$", text, re.DOTALL):
                     text = m.group(1).strip()
 
+                # <div class="container">
+                #    <h1>Oops! An Error Occurred</h1>
+                #    <h2>The server returned a "500 Internal Server Error".</h2>
+                #    <p>
+                #        Something is broken. Please let us know what you were doing when this error occurred.
+                #        We will fix it as soon as possible. Sorry for any inconvenience caused.
+                #    </p>
+                # </div>
+                if m := re.match(r'<div class="container">\s*<h1>Oops! An Error Occurred</h1>\s*'
+                                 r'<h2>The server returned a "500 Internal Server Error".</h2>\s*'
+                                 r'<p>(.+)</p>\s*</div>$', text, re.DOTALL):
+                    text = m.group(1).strip()
+
         raise error_class(text, response)
 
     content = cast(dict, response.json())
 
     bb_code = "unknown"
     message = str(content)
 
@@ -399,15 +390,7 @@
             # If there's only one error message, use it to clarify the unhelpful 'Products error'.
             if len(bb_data) == 1:
                 text = f"Products error: {bb_data[0]['message']}"
 
             raise BBProductError(text, response, bb_code, bb_data, skus=skus)
 
     raise error_class(text, response, bb_code=bb_code, bb_data=bb_data)
-
-
-# deprecated
-def wait_rate_limit(e: BBRateLimitError, wait_function=time.sleep, additional_delay=0.01):
-    if not isinstance(e, BBRateLimitError):
-        return False
-
-    return e.wait_until_expiration(wait_function=wait_function, additional_delay=additional_delay)
```

### Comparing `pybigbuy-3.17.0/bigbuy/rate_limit.py` & `pybigbuy-3.18.0/bigbuy/rate_limit.py`

 * *Files identical despite different names*

### Comparing `pybigbuy-3.17.0/pyproject.toml` & `pybigbuy-3.18.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybigbuy"
-version = "3.17.0"
+version = "3.18.0"
 description = "BigBuy API client in Python"
 authors = ["Bixoto <info@bixoto.com>"]
 license = "MIT"
 include = ["bigbuy/py.typed"]
 readme = "README.md"
 # https://github.com/python-poetry/poetry/issues/705#issuecomment-444742697
 packages = [
@@ -18,15 +18,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.25.1"
 api-session = "^1.3.2"
 
 [tool.poetry.dev-dependencies]
-mypy = "^0"
+mypy = "^1"
 types-requests = "^2.25.0"
 pytest = "^7.1.0"
 pytest-coverage = "^0.0"
 responses = "^0.21.0"
 
 [tool.coverage.report]
 omit = ["tests/*", "conftest.py"]
```

### Comparing `pybigbuy-3.17.0/PKG-INFO` & `pybigbuy-3.18.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: pybigbuy
-Version: 3.17.0
+Version: 3.18.0
 Summary: BigBuy API client in Python
 License: MIT
 Author: Bixoto
 Author-email: info@bixoto.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: api-session (>=1.3.2,<2.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # PyBigBuy
 
 **PyBigBuy** is a Python client for BigBuy’s REST API.
@@ -45,9 +44,9 @@
 
 
 client = BigBuy("your-API-token", "production")
 ```
 
 ## License
 
-Copyright 2020-2022 [Bixoto](https://bixoto.com/).
+Copyright 2020-2023 [Bixoto](https://bixoto.com/).
```

