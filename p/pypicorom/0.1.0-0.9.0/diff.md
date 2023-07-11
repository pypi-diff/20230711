# Comparing `tmp/pypicorom-0.1.0.tar.gz` & `tmp/pypicorom-0.9.0.tar.gz`

## Comparing `pypicorom-0.1.0.tar` & `pypicorom-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      246 1970-01-01 00:00:00.000000 pypicorom-0.1.0/local_dependencies/picolink/Cargo.toml
--rw-r--r--   0     1001      123    12985 2023-07-11 03:48:36.000000 pypicorom-0.1.0/local_dependencies/picolink/src/lib.rs
--rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 pypicorom-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123      325 2023-07-11 03:48:36.000000 pypicorom-0.1.0/.env/pyvenv.cfg
--rw-r--r--   0     1001      123     2807 2023-07-11 03:48:36.000000 pypicorom-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-07-11 03:48:36.000000 pypicorom-0.1.0/.gitignore
--rw-r--r--   0     1001      123      370 2023-07-11 03:48:36.000000 pypicorom-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123     3923 2023-07-11 03:48:36.000000 pypicorom-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123    12956 2023-07-11 03:48:42.000000 pypicorom-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pypicorom-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      246 1970-01-01 00:00:00.000000 pypicorom-0.9.0/local_dependencies/picolink/Cargo.toml
+-rw-r--r--   0     1001      123    12985 2023-07-11 15:31:20.000000 pypicorom-0.9.0/local_dependencies/picolink/src/lib.rs
+-rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 pypicorom-0.9.0/Cargo.toml
+-rw-r--r--   0     1001      123      325 2023-07-11 15:31:20.000000 pypicorom-0.9.0/.env/pyvenv.cfg
+-rw-r--r--   0     1001      123     2807 2023-07-11 15:31:20.000000 pypicorom-0.9.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-07-11 15:31:20.000000 pypicorom-0.9.0/.gitignore
+-rw-r--r--   0     1001      123      370 2023-07-11 15:31:20.000000 pypicorom-0.9.0/pyproject.toml
+-rw-r--r--   0     1001      123     3923 2023-07-11 15:31:20.000000 pypicorom-0.9.0/src/lib.rs
+-rw-r--r--   0     1001      123    12956 2023-07-11 15:31:25.000000 pypicorom-0.9.0/Cargo.lock
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pypicorom-0.9.0/PKG-INFO
```

### Comparing `pypicorom-0.1.0/local_dependencies/picolink/src/lib.rs` & `pypicorom-0.9.0/local_dependencies/picolink/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pypicorom-0.1.0/.github/workflows/CI.yml` & `pypicorom-0.9.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pypicorom-0.1.0/.gitignore` & `pypicorom-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pypicorom-0.1.0/src/lib.rs` & `pypicorom-0.9.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pypicorom-0.1.0/Cargo.lock` & `pypicorom-0.9.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "picolink"
-version = "0.1.0"
+version = "0.9.0"
 dependencies = [
  "anyhow",
  "num-derive",
  "num-traits",
  "serialport",
 ]
 
@@ -282,15 +282,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pypicorom"
-version = "0.1.0"
+version = "0.9.0"
 dependencies = [
  "picolink",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
@@ -395,17 +395,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.8"
+version = "0.12.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
+checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
```

