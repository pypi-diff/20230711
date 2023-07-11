# Comparing `tmp/bolt11-1.0.1.tar.gz` & `tmp/bolt11-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bolt11-1.0.1.tar", max compression
+gzip compressed data, was "bolt11-1.0.2.tar", max compression
```

## Comparing `bolt11-1.0.1.tar` & `bolt11-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1112 2023-07-10 21:30:03.466005 bolt11-1.0.1/LICENSE
--rwxr-xr-x   0        0        0     3119 2023-07-10 21:30:03.466005 bolt11-1.0.1/README.md
--rw-r--r--   0        0        0      353 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/__init__.py
--rw-r--r--   0        0        0     1127 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/bit_utils.py
--rw-r--r--   0        0        0      599 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/cli.py
--rw-r--r--   0        0        0      243 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/compat.py
--rw-r--r--   0        0        0     3932 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/decode.py
--rw-r--r--   0        0        0     2926 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/encode.py
--rw-r--r--   0        0        0     2850 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/models/fallback.py
--rw-r--r--   0        0        0     3486 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/models/features.py
--rw-r--r--   0        0        0     1768 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/models/routehint.py
--rw-r--r--   0        0        0     2322 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/models/signature.py
--rw-r--r--   0        0        0       26 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/py.typed
--rw-r--r--   0        0        0     3940 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/types.py
--rw-r--r--   0        0        0     1947 2023-07-10 21:30:03.466005 bolt11-1.0.1/bolt11/utils.py
--rw-r--r--   0        0        0     1545 2023-07-10 21:30:03.466005 bolt11-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3924 1970-01-01 00:00:00.000000 bolt11-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1112 2023-07-11 07:15:44.389912 bolt11-1.0.2/LICENSE
+-rwxr-xr-x   0        0        0     3119 2023-07-11 07:15:44.389912 bolt11-1.0.2/README.md
+-rw-r--r--   0        0        0      353 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/__init__.py
+-rw-r--r--   0        0        0     1127 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/bit_utils.py
+-rw-r--r--   0        0        0      599 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/cli.py
+-rw-r--r--   0        0        0      243 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/compat.py
+-rw-r--r--   0        0        0     3932 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/decode.py
+-rw-r--r--   0        0        0     2926 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/encode.py
+-rw-r--r--   0        0        0     2850 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/models/fallback.py
+-rw-r--r--   0        0        0     3486 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/models/features.py
+-rw-r--r--   0        0        0     1768 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/models/routehint.py
+-rw-r--r--   0        0        0     2322 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/models/signature.py
+-rw-r--r--   0        0        0       26 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/py.typed
+-rw-r--r--   0        0        0     3962 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/types.py
+-rw-r--r--   0        0        0     1947 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/utils.py
+-rw-r--r--   0        0        0     1545 2023-07-11 07:15:44.389912 bolt11-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3924 1970-01-01 00:00:00.000000 bolt11-1.0.2/PKG-INFO
```

### Comparing `bolt11-1.0.1/LICENSE` & `bolt11-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.1/README.md` & `bolt11-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.1/bolt11/bit_utils.py` & `bolt11-1.0.2/bolt11/bit_utils.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.1/bolt11/cli.py` & `bolt11-1.0.2/bolt11/cli.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.1/bolt11/decode.py` & `bolt11-1.0.2/bolt11/decode.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.1/bolt11/encode.py` & `bolt11-1.0.2/bolt11/encode.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.1/bolt11/models/fallback.py` & `bolt11-1.0.2/bolt11/models/fallback.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.1/bolt11/models/features.py` & `bolt11-1.0.2/bolt11/models/features.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.1/bolt11/models/routehint.py` & `bolt11-1.0.2/bolt11/models/routehint.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.1/bolt11/models/signature.py` & `bolt11-1.0.2/bolt11/models/signature.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.1/bolt11/types.py` & `bolt11-1.0.2/bolt11/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     @property
     def min_final_cltv_expiry(self) -> Optional[int]:
         return self.tags["c"] if "c" in self.tags else 9
 
     @property
     def payment_hash(self) -> Optional[str]:
-        return self.tags["p"] or None
+        return self.tags["p"] if "p" in self.tags else None
 
     @property
     def payment_secret(self) -> Optional[str]:
         return self.tags["s"] if "s" in self.tags else None
 
     @property
     def payee(self) -> Optional[str]:
```

### Comparing `bolt11-1.0.1/bolt11/utils.py` & `bolt11-1.0.2/bolt11/utils.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.1/pyproject.toml` & `bolt11-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bolt11"
-version = "1.0.1"
+version = "1.0.2"
 description = "A library for encoding and decoding BOLT11 payment requests."
 repository = "https://github.com/lnbits/bolt11"
 authors = [
     "eillarra <eneko@illarra.com>",
     "Alan Bits <alan@lnbits.com>"
 ]
 license = "MIT"
```

### Comparing `bolt11-1.0.1/PKG-INFO` & `bolt11-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bolt11
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library for encoding and decoding BOLT11 payment requests.
 Home-page: https://github.com/lnbits/bolt11
 License: MIT
 Author: eillarra
 Author-email: eneko@illarra.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

