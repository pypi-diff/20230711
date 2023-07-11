# Comparing `tmp/tap_exact-0.5.4.tar.gz` & `tmp/tap_exact-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_exact-0.5.4.tar", max compression
+gzip compressed data, was "tap_exact-0.6.0.tar", max compression
```

## Comparing `tap_exact-0.5.4.tar` & `tap_exact-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      932 2023-06-28 13:01:11.047380 tap_exact-0.5.4/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.5.4/tap_exact/__init__.py
--rw-r--r--   0        0        0     2469 2023-06-06 11:29:41.864014 tap_exact-0.5.4/tap_exact/client.py
--rw-r--r--   0        0        0    37730 2023-06-28 13:02:02.287380 tap_exact-0.5.4/tap_exact/streams.py
--rw-r--r--   0        0        0     1917 2023-06-06 09:27:46.919611 tap_exact-0.5.4/tap_exact/tap.py
--rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.5.4/tap_exact/tests/__init__.py
--rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.5.4/tap_exact/tests/test_core.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.5.4/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      932 2023-07-11 09:16:27.876571 tap_exact-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.6.0/tap_exact/__init__.py
+-rw-r--r--   0        0        0     2469 2023-06-06 11:29:41.864014 tap_exact-0.6.0/tap_exact/client.py
+-rw-r--r--   0        0        0    40284 2023-07-11 09:15:38.936571 tap_exact-0.6.0/tap_exact/streams.py
+-rw-r--r--   0        0        0     1994 2023-07-11 09:16:15.866571 tap_exact-0.6.0/tap_exact/tap.py
+-rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.6.0/tap_exact/tests/__init__.py
+-rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.6.0/tap_exact/tests/test_core.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.6.0/setup.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.6.0/PKG-INFO
```

### Comparing `tap_exact-0.5.4/pyproject.toml` & `tap_exact-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-exact"
-version = "0.5.4"
+version = "0.6.0"
 description = "`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK."
 authors = ["Janick Otten"]
 keywords = [
     "ELT",
     "Exact Online",
 ]
 license = "Apache 2.0"
```

### Comparing `tap_exact-0.5.4/tap_exact/client.py` & `tap_exact-0.6.0/tap_exact/client.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.5.4/tap_exact/streams.py` & `tap_exact-0.6.0/tap_exact/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -1047,14 +1047,92 @@
             filter_path = f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&"
         
         path = f"/cashflow/Receivables?{filter_path if 'filter_path' in locals() else ''}" \
             "$select=ID,Account,AccountCode,AmountDC,AmountDiscountDC,Created,Description,DiscountDueDate,DocumentNumber,DocumentSubject,DueDate,InvoiceDate,InvoiceNumber,PaymentCondition,Status,YourRef,Modified"
 
         return path
 
+class TransactionLinesStream(ExactOnlineStream):
+    """Define custom stream."""
+
+    name = "transaction_lines"
+    primary_keys = ["ID"]
+    replication_key = "Modified"
+    date_fields = ['Date', 'Modified']
+    # Optionally, you may also use `schema_filepath` in place of `schema`:
+    # schema_filepath = SCHEMAS_DIR / "users.json"
+    schema = th.PropertiesList(
+        th.Property(
+            "ID",
+            th.StringType,
+            description="The unique identifier of the line"
+        ),
+        th.Property(
+            "AccountCode",
+            th.StringType,
+            description="The unique code of the corresponding CRM account"
+        ),
+        th.Property(
+            "AccountName",
+            th.StringType,
+            description="The name of the account"
+        ),
+        th.Property(
+            "GLAccount",
+            th.StringType,
+            description="The unique identifier of the corresponding GL account"
+        ),
+        th.Property(
+            "GLAccountCode",
+            th.StringType,
+            description="The unique code of the corresponding GL account"
+        ),
+        th.Property(
+            "Date",
+            th.DateTimeType,
+            description="THe date of the statement line"
+        ),
+        th.Property(
+            "Description",
+            th.StringType,
+            description="The description of the entry"
+        ),
+        th.Property(
+            "LineNumber",
+            th.IntegerType,
+            description="The line number of the entry"
+        ),
+        th.Property(
+            "AmountDC",
+            th.StringType,
+            description="The amount in the default currency of the company"
+        ),
+        th.Property(
+            "AmountVATBaseFc",
+            th.StringType,
+            description="The amount of VAT in the default currency of the company"
+        ),
+        th.Property(
+            "Modified",
+            th.DateTimeType,
+            description="Last modified date"
+        ),
+    ).to_dict()
+
+    def get_path(self, context: Optional[dict]) -> str:
+        """Return the path of the Exact API"""
+
+        replication_key_value = self.get_starting_timestamp(context).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
+        
+        path = "/financialtransaction/TransactionLines?" \
+            f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&" \
+            "$select=ID,AccountCode,AccountName,GLAccount,GLAccountCode,Date,Description,LineNumber,AmountDC,AmountVATBaseFC,Modified"
+
+        return path
+
 # class SystemUsersStream(ExactOnlineStream):
 #     """Define custom stream."""
 
 #     name = "system_users"
 #     primary_keys = ["UserID"]
 #     replication_key = "Modified"
 #     date_fields = ['StartDate', 'EndDate', 'Modified']
```

### Comparing `tap_exact-0.5.4/tap_exact/tap.py` & `tap_exact-0.6.0/tap_exact/tap.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,40 +6,42 @@
 from singer_sdk import typing as th  # JSON schema typing helpers
 # TODO: Import your custom stream types here:
 from tap_exact.streams import (
     ExactOnlineStream,
     SalesInvoicesStream,
     PurchaseInvoicesStream,
     GeneralLedgerAccountsStream,
-    BankEntryLinesStream,
-    CashEntryLinesStream,
-    GeneralJournalEntryLinesStream,
-    PurchaseEntriesStream,
-    SalesEntriesStream,
+    # BankEntryLinesStream,
+    # CashEntryLinesStream,
+    # GeneralJournalEntryLinesStream,
+    # PurchaseEntriesStream,
+    # SalesEntriesStream,
     CrmAccountsStream,
     CashflowPaymentConditionsStream,
     CashflowPaymentsStream,
-    CashflowReceivablesStream
+    CashflowReceivablesStream,
+    TransactionLinesStream,
     # SystemUsersStream
 )
 # TODO: Compile a list of custom stream types here
 #       OR rewrite discover_streams() below with your custom logic.
 STREAM_TYPES = [
     SalesInvoicesStream,
     PurchaseInvoicesStream,
     GeneralLedgerAccountsStream,
-    BankEntryLinesStream,
-    CashEntryLinesStream,
-    GeneralJournalEntryLinesStream,
-    PurchaseEntriesStream,
-    SalesEntriesStream,
+    # BankEntryLinesStream,
+    # CashEntryLinesStream,
+    # GeneralJournalEntryLinesStream,
+    # PurchaseEntriesStream,
+    # SalesEntriesStream,
     CrmAccountsStream,
     CashflowPaymentConditionsStream,
     CashflowPaymentsStream,
-    CashflowReceivablesStream
+    CashflowReceivablesStream,
+    TransactionLinesStream
     # SystemUsersStream
 ]
 
 
 class TapExactOnline(Tap):
     """ExactOnline tap class."""
     name = "tap-exact"
```

### Comparing `tap_exact-0.5.4/tap_exact/tests/test_core.py` & `tap_exact-0.6.0/tap_exact/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.5.4/setup.py` & `tap_exact-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'s3': ['fs-s3fs>=1.1.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['tap-exact = tap_exact.tap:TapExactOnline.cli']}
 
 setup_kwargs = {
     'name': 'tap-exact',
-    'version': '0.5.4',
+    'version': '0.6.0',
     'description': '`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.',
     'long_description': 'None',
     'author': 'Janick Otten',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tap_exact-0.5.4/PKG-INFO` & `tap_exact-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-exact
-Version: 0.5.4
+Version: 0.6.0
 Summary: `tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Exact Online
 Author: Janick Otten
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

