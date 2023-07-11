# Comparing `tmp/iota_sdk-0.1.0-py3-none-any.whl.zip` & `tmp/iota_sdk-1.0.0rc0-cp310-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,38 @@
-Zip file size: 1038 bytes, number of entries: 4
--rw-rw-r--  2.0 unx      268 b- defN 23-Apr-18 16:00 iota_sdk-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 16:00 iota_sdk-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 23-Apr-18 16:00 iota_sdk-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      300 b- defN 23-Apr-18 16:00 iota_sdk-0.1.0.dist-info/RECORD
-4 files, 661 bytes uncompressed, 448 bytes compressed:  32.2%
+Zip file size: 7407457 bytes, number of entries: 36
+-rw-r--r--  4.6 unx     3512 b- defN 23-Jul-11 14:12 iota_sdk-1.0.0rc0.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 23-Jul-11 14:12 iota_sdk-1.0.0rc0.dist-info/WHEEL
+-rw-r--r--  4.6 unx    20184 b- defN 23-Jul-11 14:12 iota_sdk/client/client.py
+-rw-r--r--  4.6 unx     6975 b- defN 23-Jul-11 14:12 iota_sdk/client/_high_level_api.py
+-rw-r--r--  4.6 unx     6114 b- defN 23-Jul-11 14:12 iota_sdk/client/_node_core_api.py
+-rw-r--r--  4.6 unx     4036 b- defN 23-Jul-11 14:12 iota_sdk/client/_node_indexer_api.py
+-rw-r--r--  4.6 unx     1768 b- defN 23-Jul-11 14:12 iota_sdk/client/_utils.py
+-rw-r--r--  4.6 unx      323 b- defN 23-Jul-11 14:12 iota_sdk/prefix_hex.py
+-rw-r--r--  4.6 unx     8385 b- defN 23-Jul-11 14:12 iota_sdk/secret_manager/secret_manager.py
+-rw-r--r--  4.6 unx     1494 b- defN 23-Jul-11 14:12 iota_sdk/types/address.py
+-rw-r--r--  4.6 unx     1425 b- defN 23-Jul-11 14:12 iota_sdk/types/balance.py
+-rw-r--r--  4.6 unx     2153 b- defN 23-Jul-11 14:12 iota_sdk/types/block.py
+-rw-r--r--  4.6 unx     2006 b- defN 23-Jul-11 14:12 iota_sdk/types/burn.py
+-rw-r--r--  4.6 unx     2190 b- defN 23-Jul-11 14:12 iota_sdk/types/common.py
+-rw-r--r--  4.6 unx      303 b- defN 23-Jul-11 14:12 iota_sdk/types/event.py
+-rw-r--r--  4.6 unx     2579 b- defN 23-Jul-11 14:12 iota_sdk/types/feature.py
+-rw-r--r--  4.6 unx      224 b- defN 23-Jul-11 14:12 iota_sdk/types/native_token.py
+-rw-r--r--  4.6 unx     2081 b- defN 23-Jul-11 14:12 iota_sdk/types/node_info.py
+-rw-r--r--  4.6 unx     3142 b- defN 23-Jul-11 14:12 iota_sdk/types/output.py
+-rw-r--r--  4.6 unx      553 b- defN 23-Jul-11 14:12 iota_sdk/types/output_data.py
+-rw-r--r--  4.6 unx     1700 b- defN 23-Jul-11 14:12 iota_sdk/types/output_id.py
+-rw-r--r--  4.6 unx     2566 b- defN 23-Jul-11 14:12 iota_sdk/types/payload.py
+-rw-r--r--  4.6 unx      256 b- defN 23-Jul-11 14:12 iota_sdk/types/signature.py
+-rw-r--r--  4.6 unx      760 b- defN 23-Jul-11 14:12 iota_sdk/types/token_scheme.py
+-rw-r--r--  4.6 unx     1115 b- defN 23-Jul-11 14:12 iota_sdk/types/transaction.py
+-rw-r--r--  4.6 unx     1858 b- defN 23-Jul-11 14:12 iota_sdk/types/transaction_options.py
+-rw-r--r--  4.6 unx     3701 b- defN 23-Jul-11 14:12 iota_sdk/types/unlock_condition.py
+-rw-r--r--  4.6 unx     7063 b- defN 23-Jul-11 14:12 iota_sdk/utils.py
+-rw-r--r--  4.6 unx    17168 b- defN 23-Jul-11 14:12 iota_sdk/wallet/account.py
+-rw-r--r--  4.6 unx     2514 b- defN 23-Jul-11 14:12 iota_sdk/wallet/common.py
+-rw-r--r--  4.6 unx     2403 b- defN 23-Jul-11 14:12 iota_sdk/wallet/prepared_transaction_data.py
+-rw-r--r--  4.6 unx     3010 b- defN 23-Jul-11 14:12 iota_sdk/wallet/sync_options.py
+-rw-r--r--  4.6 unx     8695 b- defN 23-Jul-11 14:12 iota_sdk/wallet/wallet.py
+-rw-r--r--  4.6 unx     1075 b- defN 23-Jul-11 14:12 iota_sdk/__init__.py
+-rwxr-xr-x  4.6 unx 17735168 b- defN 23-Jul-11 14:12 iota_sdk/iota_sdk.cp310-win_amd64.pyd
+-rw-r--r--  4.6 unx     3026 b- defN 23-Jul-11 14:12 iota_sdk-1.0.0rc0.dist-info/RECORD
+36 files, 17861620 bytes uncompressed, 7402639 bytes compressed:  58.6%
```

## zipnote {}

```diff
@@ -1,13 +1,109 @@
-Filename: iota_sdk-0.1.0.dist-info/METADATA
+Filename: iota_sdk-1.0.0rc0.dist-info/METADATA
 Comment: 
 
-Filename: iota_sdk-0.1.0.dist-info/WHEEL
+Filename: iota_sdk-1.0.0rc0.dist-info/WHEEL
 Comment: 
 
-Filename: iota_sdk-0.1.0.dist-info/top_level.txt
+Filename: iota_sdk/client/client.py
 Comment: 
 
-Filename: iota_sdk-0.1.0.dist-info/RECORD
+Filename: iota_sdk/client/_high_level_api.py
+Comment: 
+
+Filename: iota_sdk/client/_node_core_api.py
+Comment: 
+
+Filename: iota_sdk/client/_node_indexer_api.py
+Comment: 
+
+Filename: iota_sdk/client/_utils.py
+Comment: 
+
+Filename: iota_sdk/prefix_hex.py
+Comment: 
+
+Filename: iota_sdk/secret_manager/secret_manager.py
+Comment: 
+
+Filename: iota_sdk/types/address.py
+Comment: 
+
+Filename: iota_sdk/types/balance.py
+Comment: 
+
+Filename: iota_sdk/types/block.py
+Comment: 
+
+Filename: iota_sdk/types/burn.py
+Comment: 
+
+Filename: iota_sdk/types/common.py
+Comment: 
+
+Filename: iota_sdk/types/event.py
+Comment: 
+
+Filename: iota_sdk/types/feature.py
+Comment: 
+
+Filename: iota_sdk/types/native_token.py
+Comment: 
+
+Filename: iota_sdk/types/node_info.py
+Comment: 
+
+Filename: iota_sdk/types/output.py
+Comment: 
+
+Filename: iota_sdk/types/output_data.py
+Comment: 
+
+Filename: iota_sdk/types/output_id.py
+Comment: 
+
+Filename: iota_sdk/types/payload.py
+Comment: 
+
+Filename: iota_sdk/types/signature.py
+Comment: 
+
+Filename: iota_sdk/types/token_scheme.py
+Comment: 
+
+Filename: iota_sdk/types/transaction.py
+Comment: 
+
+Filename: iota_sdk/types/transaction_options.py
+Comment: 
+
+Filename: iota_sdk/types/unlock_condition.py
+Comment: 
+
+Filename: iota_sdk/utils.py
+Comment: 
+
+Filename: iota_sdk/wallet/account.py
+Comment: 
+
+Filename: iota_sdk/wallet/common.py
+Comment: 
+
+Filename: iota_sdk/wallet/prepared_transaction_data.py
+Comment: 
+
+Filename: iota_sdk/wallet/sync_options.py
+Comment: 
+
+Filename: iota_sdk/wallet/wallet.py
+Comment: 
+
+Filename: iota_sdk/__init__.py
+Comment: 
+
+Filename: iota_sdk/iota_sdk.cp310-win_amd64.pyd
+Comment: 
+
+Filename: iota_sdk-1.0.0rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

