# Comparing `tmp/visafx-0.1.3-py3-none-any.whl.zip` & `tmp/visafx-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3140 bytes, number of entries: 7
+Zip file size: 3173 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 visafx/__init__.py
--rw-r--r--  2.0 unx     2242 b- defN 80-Jan-01 00:00 visafx/rates.py
+-rw-r--r--  2.0 unx     2493 b- defN 80-Jan-01 00:00 visafx/rates.py
 -rw-r--r--  2.0 unx      503 b- defN 80-Jan-01 00:00 visafx/test_rates.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 visafx-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      515 b- defN 80-Jan-01 00:00 visafx-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 visafx-0.1.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx      510 b- defN 16-Jan-01 00:00 visafx-0.1.3.dist-info/RECORD
-7 files, 4949 bytes uncompressed, 2244 bytes compressed:  54.7%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 visafx-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      515 b- defN 80-Jan-01 00:00 visafx-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 visafx-0.1.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx      510 b- defN 16-Jan-01 00:00 visafx-0.1.4.dist-info/RECORD
+7 files, 5200 bytes uncompressed, 2277 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: visafx/rates.py
 Comment: 
 
 Filename: visafx/test_rates.py
 Comment: 
 
-Filename: visafx-0.1.3.dist-info/LICENSE
+Filename: visafx-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: visafx-0.1.3.dist-info/METADATA
+Filename: visafx-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: visafx-0.1.3.dist-info/WHEEL
+Filename: visafx-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: visafx-0.1.3.dist-info/RECORD
+Filename: visafx-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## visafx/rates.py

```diff
@@ -1,15 +1,15 @@
 import json
 from datetime import datetime
 from datetime import timedelta
 
 import cloudscraper
 from loguru import logger
 from pydantic import BaseModel
-from retry import retry
+from retry.api import retry_call
 
 
 class OriginalValues(BaseModel):
     fromCurrency: str
     fromCurrencyName: str
     toCurrency: str
     toCurrencyName: str
@@ -62,35 +62,44 @@
     scraper = cloudscraper.create_scraper()
 
     resp = scraper.get(url=url, params=params)
 
     return Response.parse_obj(resp.json())
 
 
-@retry(delay=1)
 def rates(amount: float = 1.0,
           from_curr: str = 'TWD',
           to_curr: str = 'USD',
           fee: float = 0.0,
           date: datetime = None) -> Response:
     if date is None:
         date = datetime.now()
 
     try:
-        resp = _rates(
-            amount=amount,
-            from_curr=from_curr,
-            to_curr=to_curr,
-            fee=fee,
-            date=date,
+        resp = retry_call(
+            _rates,
+            fkwargs=dict(
+                amount=amount,
+                from_curr=from_curr,
+                to_curr=to_curr,
+                fee=fee,
+                date=date,
+            ),
+            tries=100,
+            delay=1,
         )
     except json.decoder.JSONDecodeError as e:
         logger.error(e)
-        resp = _rates(
-            amount=amount,
-            from_curr=from_curr,
-            to_curr=to_curr,
-            fee=fee,
-            date=date - timedelta(days=1),
+        resp = retry_call(
+            _rates,
+            fkwargs=dict(
+                amount=amount,
+                from_curr=from_curr,
+                to_curr=to_curr,
+                fee=fee,
+                date=date - timedelta(days=1),
+            ),
+            tries=100,
+            delay=1,
         )
 
     return resp
```

## Comparing `visafx-0.1.3.dist-info/LICENSE` & `visafx-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `visafx-0.1.3.dist-info/METADATA` & `visafx-0.1.4.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visafx
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: なるみ
 Author-email: toucans-cutouts0f@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

