# Comparing `tmp/kount_ris_sdk-3.4.2.tar.gz` & `tmp/kount_ris_sdk-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kount_ris_sdk-3.4.2.tar", last modified: Wed Apr 12 17:39:18 2023, max compression
+gzip compressed data, was "kount_ris_sdk-3.4.3.tar", last modified: Tue Jul 11 15:52:06 2023, max compression
```

## Comparing `kount_ris_sdk-3.4.2.tar` & `kount_ris_sdk-3.4.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-04-12 17:39:18.169129 kount_ris_sdk-3.4.2/
--rw-rw-rw-   0 root         (0) nogroup  (65534)     4919 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/LICENSE
--rw-rw-rw-   0 root         (0) nogroup  (65534)       76 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) nogroup  (65534)     1408 2023-04-12 17:39:18.173129 kount_ris_sdk-3.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) nogroup  (65534)      600 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/README.md
--rw-rw-rw-   0 root         (0) nogroup  (65534)      300 2023-04-12 17:39:18.177129 kount_ris_sdk-3.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) nogroup  (65534)     2972 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/setup.py
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-04-12 17:39:18.169129 kount_ris_sdk-3.4.2/src/
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-04-12 17:39:18.169129 kount_ris_sdk-3.4.2/src/kount/
--rw-rw-rw-   0 root         (0) nogroup  (65534)      543 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/__init__.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     3540 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/client.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     2145 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/config.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     9396 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/inquiry.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)    13833 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/request.py
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-04-12 17:39:18.169129 kount_ris_sdk-3.4.2/src/kount/resources/
--rw-rw-rw-   0 root         (0) nogroup  (65534)      373 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/resources/__init__.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)      564 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/resources/correct_key_cryp.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)    21008 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/response.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)      178 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/settings.py
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-04-12 17:39:18.169129 kount_ris_sdk-3.4.2/src/kount/util/
--rw-rw-rw-   0 root         (0) nogroup  (65534)      529 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/util/__init__.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)      371 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/util/a85.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     1532 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/util/address.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     1483 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/util/cartitem.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)     4917 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/util/khash.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)    10011 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/util/payment.py
--rw-rw-rw-   0 root         (0) nogroup  (65534)       87 2023-04-12 17:39:12.000000 kount_ris_sdk-3.4.2/src/kount/version.py
-drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-04-12 17:39:18.169129 kount_ris_sdk-3.4.2/src/kount_ris_sdk.egg-info/
--rw-r--r--   0 root         (0) nogroup  (65534)     1408 2023-04-12 17:39:18.000000 kount_ris_sdk-3.4.2/src/kount_ris_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) nogroup  (65534)      645 2023-04-12 17:39:18.000000 kount_ris_sdk-3.4.2/src/kount_ris_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) nogroup  (65534)        1 2023-04-12 17:39:18.000000 kount_ris_sdk-3.4.2/src/kount_ris_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) nogroup  (65534)      317 2023-04-12 17:39:18.000000 kount_ris_sdk-3.4.2/src/kount_ris_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) nogroup  (65534)        6 2023-04-12 17:39:18.000000 kount_ris_sdk-3.4.2/src/kount_ris_sdk.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-07-11 15:52:06.347776 kount_ris_sdk-3.4.3/
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     4919 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/LICENSE
+-rw-rw-rw-   0 root         (0) nogroup  (65534)       76 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) nogroup  (65534)     1408 2023-07-11 15:52:06.347776 kount_ris_sdk-3.4.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      600 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/README.md
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      300 2023-07-11 15:52:06.347776 kount_ris_sdk-3.4.3/setup.cfg
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     2972 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/setup.py
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-07-11 15:52:06.343776 kount_ris_sdk-3.4.3/src/
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-07-11 15:52:06.347776 kount_ris_sdk-3.4.3/src/kount/
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      543 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/__init__.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     3540 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/client.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     2145 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/config.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     9396 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/inquiry.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)    13902 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/request.py
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-07-11 15:52:06.347776 kount_ris_sdk-3.4.3/src/kount/resources/
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      373 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/resources/__init__.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      564 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/resources/correct_key_cryp.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)    21008 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/response.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      178 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/settings.py
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-07-11 15:52:06.347776 kount_ris_sdk-3.4.3/src/kount/util/
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      529 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/util/__init__.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)      371 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/util/a85.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     1532 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/util/address.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     1483 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/util/cartitem.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)     4917 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/util/khash.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)    10011 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/util/payment.py
+-rw-rw-rw-   0 root         (0) nogroup  (65534)       87 2023-07-11 15:52:01.000000 kount_ris_sdk-3.4.3/src/kount/version.py
+drwxr-sr-x   0 root         (0) nogroup  (65534)        0 2023-07-11 15:52:06.347776 kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/
+-rw-r--r--   0 root         (0) nogroup  (65534)     1408 2023-07-11 15:52:06.000000 kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) nogroup  (65534)      645 2023-07-11 15:52:06.000000 kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) nogroup  (65534)        1 2023-07-11 15:52:06.000000 kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) nogroup  (65534)      317 2023-07-11 15:52:06.000000 kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) nogroup  (65534)        6 2023-07-11 15:52:06.000000 kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/top_level.txt
```

### Comparing `kount_ris_sdk-3.4.2/LICENSE` & `kount_ris_sdk-3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.2/PKG-INFO` & `kount_ris_sdk-3.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kount_ris_sdk
-Version: 3.4.2
+Version: 3.4.3
 Summary: Kount Python RIS SDK
 Home-page: https://github.com/Kount/kount-ris-python-sdk
 Author: Kount
 Author-email: sdkadmin@kount.com
 License: Kount
 Keywords: kount,sdk,ris
 Platform: any
```

### Comparing `kount_ris_sdk-3.4.2/README.md` & `kount_ris_sdk-3.4.3/README.md`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.2/setup.py` & `kount_ris_sdk-3.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.2/src/kount/__init__.py` & `kount_ris_sdk-3.4.3/src/kount/__init__.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.2/src/kount/client.py` & `kount_ris_sdk-3.4.3/src/kount/client.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.2/src/kount/config.py` & `kount_ris_sdk-3.4.3/src/kount/config.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.2/src/kount/inquiry.py` & `kount_ris_sdk-3.4.3/src/kount/inquiry.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.2/src/kount/request.py` & `kount_ris_sdk-3.4.3/src/kount/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,17 +315,18 @@
         The payment type parameter provided is checked
         if it's one of the predefined payment types
         and Payment is created appropriately
         Args: ptyp - See SDK documentation for a list of accepted payment types
         ptok - The payment token
         """
         cls = {
-            "BLML": payments.BillMeLaterPayment,
+            'BLML': payments.BillMeLaterPayment,
             'CARD': payments.CardPayment,
-            'CHECK': payments.CheckPayment,
+            'CHECK': payments.CheckPayment, # backwards compatibility
+            'CHEK': payments.CheckPayment,
             'GIFT': payments.GiftCardPayment,
             'GOOG': payments.GooglePayment,
             'GDMP': payments.GreenDotMoneyPakPayment,
             'NONE': payments.NoPayment,
             'PYPL': payments.PaypalPayment,
         }.get(ptyp)
         if cls is None:
```

### Comparing `kount_ris_sdk-3.4.2/src/kount/resources/correct_key_cryp.py` & `kount_ris_sdk-3.4.3/src/kount/resources/correct_key_cryp.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.2/src/kount/response.py` & `kount_ris_sdk-3.4.3/src/kount/response.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.2/src/kount/util/__init__.py` & `kount_ris_sdk-3.4.3/src/kount/util/__init__.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.2/src/kount/util/address.py` & `kount_ris_sdk-3.4.3/src/kount/util/address.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.2/src/kount/util/cartitem.py` & `kount_ris_sdk-3.4.3/src/kount/util/cartitem.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.2/src/kount/util/khash.py` & `kount_ris_sdk-3.4.3/src/kount/util/khash.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.2/src/kount/util/payment.py` & `kount_ris_sdk-3.4.3/src/kount/util/payment.py`

 * *Files identical despite different names*

### Comparing `kount_ris_sdk-3.4.2/src/kount_ris_sdk.egg-info/PKG-INFO` & `kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kount-ris-sdk
-Version: 3.4.2
+Version: 3.4.3
 Summary: Kount Python RIS SDK
 Home-page: https://github.com/Kount/kount-ris-python-sdk
 Author: Kount
 Author-email: sdkadmin@kount.com
 License: Kount
 Keywords: kount,sdk,ris
 Platform: any
```

### Comparing `kount_ris_sdk-3.4.2/src/kount_ris_sdk.egg-info/SOURCES.txt` & `kount_ris_sdk-3.4.3/src/kount_ris_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

