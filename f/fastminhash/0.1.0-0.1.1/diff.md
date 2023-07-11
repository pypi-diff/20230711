# Comparing `tmp/fastminhash-0.1.0.tar.gz` & `tmp/fastminhash-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastminhash-0.1.0.tar", last modified: Tue Jul 11 15:20:05 2023, max compression
+gzip compressed data, was "fastminhash-0.1.1.tar", last modified: Tue Jul 11 15:50:13 2023, max compression
```

## Comparing `fastminhash-0.1.0.tar` & `fastminhash-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lidongruixuan   (501) staff       (20)        0 2023-07-11 15:20:05.928759 fastminhash-0.1.0/
--rw-r--r--   0 lidongruixuan   (501) staff       (20)     1067 2023-07-11 15:07:06.000000 fastminhash-0.1.0/LICENSE.txt
--rw-r--r--   0 lidongruixuan   (501) staff       (20)      250 2023-07-11 15:20:05.928547 fastminhash-0.1.0/PKG-INFO
--rw-r--r--   0 lidongruixuan   (501) staff       (20)      666 2023-07-11 15:19:07.000000 fastminhash-0.1.0/README.md
-drwxr-xr-x   0 lidongruixuan   (501) staff       (20)        0 2023-07-11 15:20:05.927471 fastminhash-0.1.0/fastminhash.egg-info/
--rw-r--r--   0 lidongruixuan   (501) staff       (20)      250 2023-07-11 15:20:05.000000 fastminhash-0.1.0/fastminhash.egg-info/PKG-INFO
--rw-r--r--   0 lidongruixuan   (501) staff       (20)      282 2023-07-11 15:20:05.000000 fastminhash-0.1.0/fastminhash.egg-info/SOURCES.txt
--rw-r--r--   0 lidongruixuan   (501) staff       (20)        1 2023-07-11 15:20:05.000000 fastminhash-0.1.0/fastminhash.egg-info/dependency_links.txt
--rw-r--r--   0 lidongruixuan   (501) staff       (20)       12 2023-07-11 15:20:05.000000 fastminhash-0.1.0/fastminhash.egg-info/requires.txt
--rw-r--r--   0 lidongruixuan   (501) staff       (20)        8 2023-07-11 15:20:05.000000 fastminhash-0.1.0/fastminhash.egg-info/top_level.txt
-drwxr-xr-x   0 lidongruixuan   (501) staff       (20)        0 2023-07-11 15:20:05.928215 fastminhash-0.1.0/minhash/
--rw-r--r--   0 lidongruixuan   (501) staff       (20)     1043 2023-07-11 14:40:26.000000 fastminhash-0.1.0/minhash/__init__.py
--rw-r--r--   0 lidongruixuan   (501) staff       (20)     1026 2023-07-11 14:33:17.000000 fastminhash-0.1.0/minhash/minhash.c
--rw-r--r--   0 lidongruixuan   (501) staff       (20)      552 2023-07-11 14:33:01.000000 fastminhash-0.1.0/minhash/minhash_build.py
--rw-r--r--   0 lidongruixuan   (501) staff       (20)       95 2023-07-11 15:05:05.000000 fastminhash-0.1.0/pyproject.toml
--rw-r--r--   0 lidongruixuan   (501) staff       (20)       38 2023-07-11 15:20:05.928826 fastminhash-0.1.0/setup.cfg
--rw-r--r--   0 lidongruixuan   (501) staff       (20)      464 2023-07-11 15:19:58.000000 fastminhash-0.1.0/setup.py
+drwxr-xr-x   0 lidongruixuan   (501) staff       (20)        0 2023-07-11 15:50:13.315583 fastminhash-0.1.1/
+-rw-r--r--   0 lidongruixuan   (501) staff       (20)     1067 2023-07-11 15:07:06.000000 fastminhash-0.1.1/LICENSE.txt
+-rw-r--r--   0 lidongruixuan   (501) staff       (20)      250 2023-07-11 15:50:13.315746 fastminhash-0.1.1/PKG-INFO
+-rw-r--r--   0 lidongruixuan   (501) staff       (20)      722 2023-07-11 15:34:13.000000 fastminhash-0.1.1/README.md
+drwxr-xr-x   0 lidongruixuan   (501) staff       (20)        0 2023-07-11 15:50:13.314231 fastminhash-0.1.1/fastminhash.egg-info/
+-rw-r--r--   0 lidongruixuan   (501) staff       (20)      250 2023-07-11 15:50:13.000000 fastminhash-0.1.1/fastminhash.egg-info/PKG-INFO
+-rw-r--r--   0 lidongruixuan   (501) staff       (20)      292 2023-07-11 15:50:13.000000 fastminhash-0.1.1/fastminhash.egg-info/SOURCES.txt
+-rw-r--r--   0 lidongruixuan   (501) staff       (20)        1 2023-07-11 15:50:13.000000 fastminhash-0.1.1/fastminhash.egg-info/dependency_links.txt
+-rw-r--r--   0 lidongruixuan   (501) staff       (20)       12 2023-07-11 15:50:13.000000 fastminhash-0.1.1/fastminhash.egg-info/requires.txt
+-rw-r--r--   0 lidongruixuan   (501) staff       (20)        8 2023-07-11 15:50:13.000000 fastminhash-0.1.1/fastminhash.egg-info/top_level.txt
+drwxr-xr-x   0 lidongruixuan   (501) staff       (20)        0 2023-07-11 15:50:13.315307 fastminhash-0.1.1/minhash/
+-rw-r--r--   0 lidongruixuan   (501) staff       (20)     1085 2023-07-11 15:31:07.000000 fastminhash-0.1.1/minhash/__init__.py
+-rw-r--r--   0 lidongruixuan   (501) staff       (20)     1085 2023-07-11 15:31:58.000000 fastminhash-0.1.1/minhash/minhash.c
+-rw-r--r--   0 lidongruixuan   (501) staff       (20)      576 2023-07-11 15:31:35.000000 fastminhash-0.1.1/minhash/minhash_build.py
+-rw-r--r--   0 lidongruixuan   (501) staff       (20)       95 2023-07-11 15:05:05.000000 fastminhash-0.1.1/pyproject.toml
+-rw-r--r--   0 lidongruixuan   (501) staff       (20)       79 2023-07-11 15:50:13.316145 fastminhash-0.1.1/setup.cfg
+-rw-r--r--   0 lidongruixuan   (501) staff       (20)      464 2023-07-11 15:35:12.000000 fastminhash-0.1.1/setup.py
```

### Comparing `fastminhash-0.1.0/LICENSE.txt` & `fastminhash-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastminhash-0.1.0/README.md` & `fastminhash-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 ```
 
 ### Usage
 
 ```python3
 from minhash import minhash, minhash_all
 
-# `n` means to hash every n-grams, `token_max_value` is the maximum value of each token, `coeff1` and `coeff2` are two constants for hash function construction, `tokens` is the list of tokens
-hash = minhash(5, 100276, 12345, 54321, [32352, 33513, 1864, 3626, 12763, 27125, 23981])
+# `n` means to hash every n-grams, `token_max_value` is the maximum value of each token, `coeff1`, `coeff2`, `modulo` are constants for hash function `(coeff1 * token + coeff2) % modulo` construction, `tokens` is the list of tokens
+hash = minhash(5, 100276, 100279, 12345, 54321, [32352, 33513, 1864, 3626, 12763, 27125, 23981])
 
 # You can calculate multiple minhashes at once by using multiple coeffs
-hashes = minhash_all(5, 100276, [(12345, 54321), (23456, 65432)], [32352, 33513, 1864, 3626, 12763, 27125, 23981])
+hashes = minhash_all(5, 100276, 100279, [(12345, 54321), (23456, 65432)], [32352, 33513, 1864, 3626, 12763, 27125, 23981])
 ```
```

### Comparing `fastminhash-0.1.0/minhash/__init__.py` & `fastminhash-0.1.1/minhash/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from ._minhash.lib import minhash as minhash_impl, minhash_all as minhash_all_impl
 from ._minhash import ffi
 from typing import List, Tuple
 
-def minhash(n: int, token_max_value: int, coeff1: int, coeff2: int, tokens: List[int]) -> int:
+def minhash(n: int, token_max_value: int, modulo: int, coeff1: int, coeff2: int, tokens: List[int]) -> int:
     tokens_in = ffi.new("int[]", len(tokens))
     for i in range(len(tokens)):
         tokens_in[i] = tokens[i]
-    return minhash_impl(n, token_max_value, coeff1, coeff2, len(tokens), tokens_in)
+    return minhash_impl(n, token_max_value, modulo, coeff1, coeff2, len(tokens), tokens_in)
 
-def minhash_all(n: int, token_max_value: int, coeffs: List[Tuple[int, int]], tokens: List[int]) -> List[int]:
+def minhash_all(n: int, token_max_value: int, modulo: int, coeffs: List[Tuple[int, int]], tokens: List[int]) -> List[int]:
     coeffs_in = ffi.new("hash_coeff[]", len(coeffs))
     for i in range(len(coeffs)):
         coeffs_in[i].coeff1 = coeffs[i][0]
         coeffs_in[i].coeff2 = coeffs[i][1]
     tokens_in = ffi.new("int[]", len(tokens))
     for i in range(len(tokens)):
         tokens_in[i] = tokens[i]
     results_out = ffi.new("unsigned long long[]", len(coeffs_in))
-    minhash_all_impl(n, token_max_value, len(coeffs), coeffs_in, len(tokens), tokens_in, results_out)
+    minhash_all_impl(n, token_max_value, modulo, len(coeffs), coeffs_in, len(tokens), tokens_in, results_out)
     return ffi.unpack(results_out, len(coeffs))
```

### Comparing `fastminhash-0.1.0/minhash/minhash.c` & `fastminhash-0.1.1/minhash/minhash.c`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 typedef struct {
     int coeff1, coeff2;
 } hash_coeff;
 
-unsigned long long minhash(int n, int tokenMaxValue, int coeff1, int coeff2, int tokenCnt, int *tokens) {
+unsigned long long minhash(int n, int tokenMaxValue, int modulo, int coeff1, int coeff2, int tokenCnt, int *tokens) {
     unsigned long long hash = 0, prevHashFactor = 1;
     for (int i = 0; i < n && i < tokenCnt; i++) {
         hash *= tokenMaxValue;
-        hash += (unsigned long long)coeff1 * tokens[i] + coeff2;
+        hash += (unsigned long long)coeff1 * tokens[i] % modulo + coeff2;
         prevHashFactor *= tokenMaxValue;
     }
     unsigned long long result = hash;
     for (int i = n; i < tokenCnt; i++) {
         hash *= tokenMaxValue;
-        hash -= ((unsigned long long)coeff1 * tokens[i-n] + coeff2) * prevHashFactor;
-        hash += (unsigned long long)coeff1 * tokens[i] + coeff2;
+        hash -= ((unsigned long long)coeff1 * tokens[i-n] % modulo + coeff2) * prevHashFactor;
+        hash += (unsigned long long)coeff1 * tokens[i] % modulo + coeff2;
         result = hash < result ? hash : result;
     }
     return result;
 }
 
-void minhash_all(int n, int tokenMaxValue, int coeffCnt, hash_coeff *coeffs, int tokenCnt, int *tokens, unsigned long long *result) {
+void minhash_all(int n, int tokenMaxValue, int modulo, int coeffCnt, hash_coeff *coeffs, int tokenCnt, int *tokens, unsigned long long *result) {
     for(int i = 0; i < coeffCnt; i++){
-        result[i] = minhash(n, tokenMaxValue, coeffs[i].coeff1, coeffs[i].coeff2, tokenCnt, tokens);
+        result[i] = minhash(n, tokenMaxValue, modulo, coeffs[i].coeff1, coeffs[i].coeff2, tokenCnt, tokens);
     }
 }
```

### Comparing `fastminhash-0.1.0/minhash/minhash_build.py` & `fastminhash-0.1.1/minhash/minhash_build.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from cffi import FFI
 
 signature = """
 typedef struct {
     int coeff1, coeff2;
 } hash_coeff;
-unsigned long long minhash(int n, int tokenMaxValue, int coeff1, int coeff2, int tokenCnt, int *tokens);
-void minhash_all(int n, int tokenMaxValue, int coeffCnt, hash_coeff *coeffs, int tokenCnt, int *tokens, unsigned long long *result);
+unsigned long long minhash(int n, int tokenMaxValue, int modulo, int coeff1, int coeff2, int tokenCnt, int *tokens);
+void minhash_all(int n, int tokenMaxValue, int modulo, int coeffCnt, hash_coeff *coeffs, int tokenCnt, int *tokens, unsigned long long *result);
 """
 
 ffibuilder = FFI()
 ffibuilder.cdef(signature)
 ffibuilder.set_source("minhash._minhash", signature,
     sources=['minhash/minhash.c'],
     libraries=[])
```

