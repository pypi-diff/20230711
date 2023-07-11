# Comparing `tmp/ruspy-0.1.0.tar.gz` & `tmp/ruspy-0.1.1.tar.gz`

## Comparing `ruspy-0.1.0.tar` & `ruspy-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0      298 1970-01-01 00:00:00.000000 ruspy-0.1.0/Cargo.toml
--rw-r--r--   0      501       20       40 2023-07-09 22:21:54.000000 ruspy-0.1.0/.gitignore
--rw-r--r--   0      501       20     1075 2023-07-09 21:30:49.000000 ruspy-0.1.0/LICENSE
--rw-r--r--   0      501       20      717 2023-07-09 22:28:02.000000 ruspy-0.1.0/Makefile
--rw-r--r--   0      501       20      726 2023-07-09 22:28:14.000000 ruspy-0.1.0/README.md
--rw-r--r--   0      501       20        0 2023-06-28 03:03:18.000000 ruspy-0.1.0/build/lib/test/__init__.py
--rw-r--r--   0      501       20      592 2023-07-09 22:28:14.000000 ruspy-0.1.0/build/lib/test/test_rumpy.py
--rw-r--r--   0      501       20      501 2023-07-09 22:28:02.000000 ruspy-0.1.0/pyproject.toml
--rw-r--r--   0      501       20      126 2023-07-09 21:27:04.000000 ruspy-0.1.0/requirements.txt
--rw-r--r--   0      501       20      395 2023-07-09 22:28:02.000000 ruspy-0.1.0/rumpy.egg-info/PKG-INFO
--rw-r--r--   0      501       20      193 2023-07-09 22:28:02.000000 ruspy-0.1.0/rumpy.egg-info/SOURCES.txt
--rw-r--r--   0      501       20        1 2023-07-09 22:11:47.000000 ruspy-0.1.0/rumpy.egg-info/dependency_links.txt
--rw-r--r--   0      501       20        5 2023-07-09 22:11:47.000000 ruspy-0.1.0/rumpy.egg-info/top_level.txt
--rw-r--r--   0      501       20     3793 2023-07-09 21:21:13.000000 ruspy-0.1.0/src/array.rs
--rw-r--r--   0      501       20     1554 2023-07-09 22:13:17.000000 ruspy-0.1.0/src/fft.rs
--rw-r--r--   0      501       20      387 2023-07-09 22:28:02.000000 ruspy-0.1.0/src/lib.rs
--rw-r--r--   0      501       20        0 2023-06-28 03:03:18.000000 ruspy-0.1.0/test/__init__.py
--rw-r--r--   0      501       20        6 2023-07-09 21:18:03.000000 ruspy-0.1.0/test/requirements.txt
--rw-r--r--   0      501       20      592 2023-07-09 22:28:14.000000 ruspy-0.1.0/test/test_rumpy.py
--rw-r--r--   0      501       20     7899 2023-07-09 22:28:03.000000 ruspy-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1111 1970-01-01 00:00:00.000000 ruspy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 ruspy-0.1.1/Cargo.toml
+-rw-r--r--   0      501       20       40 2023-07-09 22:21:54.000000 ruspy-0.1.1/.gitignore
+-rw-r--r--   0      501       20     1075 2023-07-09 21:30:49.000000 ruspy-0.1.1/LICENSE
+-rw-r--r--   0      501       20      717 2023-07-09 22:28:02.000000 ruspy-0.1.1/Makefile
+-rw-r--r--   0      501       20      726 2023-07-09 22:28:14.000000 ruspy-0.1.1/README.md
+-rw-r--r--   0      501       20        0 2023-06-28 03:03:18.000000 ruspy-0.1.1/build/lib/test/__init__.py
+-rw-r--r--   0      501       20      592 2023-07-09 22:28:14.000000 ruspy-0.1.1/build/lib/test/test_rumpy.py
+-rw-r--r--   0      501       20      501 2023-07-11 20:22:37.000000 ruspy-0.1.1/pyproject.toml
+-rw-r--r--   0      501       20      126 2023-07-09 21:27:04.000000 ruspy-0.1.1/requirements.txt
+-rw-r--r--   0      501       20      395 2023-07-09 22:28:02.000000 ruspy-0.1.1/rumpy.egg-info/PKG-INFO
+-rw-r--r--   0      501       20      193 2023-07-09 22:28:02.000000 ruspy-0.1.1/rumpy.egg-info/SOURCES.txt
+-rw-r--r--   0      501       20        1 2023-07-09 22:11:47.000000 ruspy-0.1.1/rumpy.egg-info/dependency_links.txt
+-rw-r--r--   0      501       20        5 2023-07-09 22:11:47.000000 ruspy-0.1.1/rumpy.egg-info/top_level.txt
+-rw-r--r--   0      501       20     9581 2023-07-10 19:28:49.000000 ruspy-0.1.1/src/array.rs
+-rw-r--r--   0      501       20     2257 2023-07-11 20:18:24.000000 ruspy-0.1.1/src/fft.rs
+-rw-r--r--   0      501       20      782 2023-07-11 20:16:21.000000 ruspy-0.1.1/src/lib.rs
+-rw-r--r--   0      501       20      490 2023-07-09 22:50:30.000000 ruspy-0.1.1/src/math.rs
+-rw-r--r--   0      501       20     1599 2023-07-11 20:12:31.000000 ruspy-0.1.1/src/test.rs
+-rw-r--r--   0      501       20        0 2023-06-28 03:03:18.000000 ruspy-0.1.1/test/__init__.py
+-rw-r--r--   0      501       20        6 2023-07-09 21:18:03.000000 ruspy-0.1.1/test/requirements.txt
+-rw-r--r--   0      501       20      592 2023-07-09 22:28:14.000000 ruspy-0.1.1/test/test_ruspy.py
+-rw-r--r--   0      501       20     9369 2023-07-11 20:12:59.000000 ruspy-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1111 1970-01-01 00:00:00.000000 ruspy-0.1.1/PKG-INFO
```

### Comparing `ruspy-0.1.0/LICENSE` & `ruspy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ruspy-0.1.0/Makefile` & `ruspy-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `ruspy-0.1.0/README.md` & `ruspy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ruspy-0.1.0/build/lib/test/test_rumpy.py` & `ruspy-0.1.1/build/lib/test/test_rumpy.py`

 * *Files identical despite different names*

### Comparing `ruspy-0.1.0/test/test_rumpy.py` & `ruspy-0.1.1/test/test_ruspy.py`

 * *Files identical despite different names*

### Comparing `ruspy-0.1.0/Cargo.lock` & `ruspy-0.1.1/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -57,14 +57,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "num-integer"
+version = "0.1.45"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+dependencies = [
+ "autocfg",
+ "num-traits",
+]
+
+[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
@@ -95,14 +105,23 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
+name = "primal-check"
+version = "0.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9df7f93fd637f083201473dab4fee2db4c429d32e55e3299980ab3957ab916a0"
+dependencies = [
+ "num-integer",
+]
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
@@ -187,15 +206,32 @@
 
 [[package]]
 name = "ruspy"
 version = "0.1.0"
 dependencies = [
  "libc",
  "num-complex",
+ "num-traits",
  "pyo3",
+ "rustfft",
+]
+
+[[package]]
+name = "rustfft"
+version = "6.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e17d4f6cbdb180c9f4b2a26bbf01c4e647f1e1dea22fe8eb9db54198b32f9434"
+dependencies = [
+ "num-complex",
+ "num-integer",
+ "num-traits",
+ "primal-check",
+ "strength_reduce",
+ "transpose",
+ "version_check",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
@@ -203,14 +239,20 @@
 [[package]]
 name = "smallvec"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
+name = "strength_reduce"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fe895eb47f22e2ddd4dabc02bce419d2e643c8e3b585c78158b349195bc24d82"
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -220,26 +262,42 @@
 [[package]]
 name = "target-lexicon"
 version = "0.12.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
 
 [[package]]
+name = "transpose"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6522d49d03727ffb138ae4cbc1283d3774f0d10aa7f9bf52e6784c45daf9b23"
+dependencies = [
+ "num-integer",
+ "strength_reduce",
+]
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "version_check"
+version = "0.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
+
+[[package]]
 name = "windows-targets"
 version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
```

### Comparing `ruspy-0.1.0/PKG-INFO` & `ruspy-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruspy
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: POSIX :: Linux
 License-File: LICENSE
 Summary: Data analysis powered by Rust
 Author: Manas Verma <manas.verma@gmail.com>
 Author-email: Manas Verma <manas.verma@gmail.com>
 Requires-Python: >=3.7
```

