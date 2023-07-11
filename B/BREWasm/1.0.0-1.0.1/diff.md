# Comparing `tmp/BREWasm-1.0.0.tar.gz` & `tmp/BREWasm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BREWasm-1.0.0.tar", last modified: Tue Jul 11 03:21:28 2023, max compression
+gzip compressed data, was "BREWasm-1.0.1.tar", last modified: Tue Jul 11 04:01:24 2023, max compression
```

## Comparing `BREWasm-1.0.0.tar` & `BREWasm-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,32 @@
-drwxrwxr-x   0 obfuscator  (1000) obfuscator  (1000)        0 2023-07-11 03:21:28.539031 BREWasm-1.0.0/
-drwxrwxr-x   0 obfuscator  (1000) obfuscator  (1000)        0 2023-07-11 03:21:28.531031 BREWasm-1.0.0/BREWasm/
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)      228 2023-07-09 04:04:29.000000 BREWasm-1.0.0/BREWasm/__init__.py
-drwxrwxr-x   0 obfuscator  (1000) obfuscator  (1000)        0 2023-07-11 03:21:28.531031 BREWasm-1.0.0/BREWasm/parser/
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)       12 2023-07-09 04:09:33.000000 BREWasm-1.0.0/BREWasm/parser/__init__.py
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)      562 2023-07-09 02:40:53.000000 BREWasm-1.0.0/BREWasm/parser/errors.py
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)      892 2023-07-09 02:40:53.000000 BREWasm-1.0.0/BREWasm/parser/instruction.py
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     1996 2023-07-09 02:40:53.000000 BREWasm-1.0.0/BREWasm/parser/leb128.py
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     5355 2023-07-09 12:13:08.000000 BREWasm-1.0.0/BREWasm/parser/module.py
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     2845 2023-07-08 13:22:42.000000 BREWasm-1.0.0/BREWasm/parser/opcodes.py
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     5778 2023-07-08 13:26:01.000000 BREWasm-1.0.0/BREWasm/parser/opnames.py
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)    24366 2023-07-09 02:45:19.000000 BREWasm-1.0.0/BREWasm/parser/reader.py
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     3108 2023-07-09 13:57:22.000000 BREWasm-1.0.0/BREWasm/parser/types.py
-drwxrwxr-x   0 obfuscator  (1000) obfuscator  (1000)        0 2023-07-11 03:21:28.539031 BREWasm-1.0.0/BREWasm/rewriter/
--rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)      286 2023-07-10 07:44:10.000000 BREWasm-1.0.0/BREWasm/rewriter/BREWasm.py
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)      229 2023-07-10 07:02:44.000000 BREWasm-1.0.0/BREWasm/rewriter/__init__.py
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     4969 2023-07-10 08:14:40.000000 BREWasm-1.0.0/BREWasm/rewriter/defination.py
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     4957 2023-07-08 14:01:07.000000 BREWasm-1.0.0/BREWasm/rewriter/indices_fixer.py
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)    51167 2023-07-10 07:47:32.000000 BREWasm-1.0.0/BREWasm/rewriter/modify_binary.py
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)    60694 2023-07-10 14:32:56.000000 BREWasm-1.0.0/BREWasm/rewriter/section_rewriter.py
--rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)    21928 2023-07-10 13:03:32.000000 BREWasm-1.0.0/BREWasm/rewriter/semantics_rewriter.py
-drwxrwxr-x   0 obfuscator  (1000) obfuscator  (1000)        0 2023-07-11 03:21:28.531031 BREWasm-1.0.0/BREWasm.egg-info/
--rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)     3442 2023-07-11 03:21:28.000000 BREWasm-1.0.0/BREWasm.egg-info/PKG-INFO
--rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)      678 2023-07-11 03:21:28.000000 BREWasm-1.0.0/BREWasm.egg-info/SOURCES.txt
--rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)        1 2023-07-11 03:21:28.000000 BREWasm-1.0.0/BREWasm.egg-info/dependency_links.txt
--rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)        8 2023-07-11 03:21:28.000000 BREWasm-1.0.0/BREWasm.egg-info/top_level.txt
--rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)     3442 2023-07-11 03:21:28.539031 BREWasm-1.0.0/PKG-INFO
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     6404 2023-07-09 14:59:48.000000 BREWasm-1.0.0/README.md
-drwxrwxr-x   0 obfuscator  (1000) obfuscator  (1000)        0 2023-07-11 03:21:28.539031 BREWasm-1.0.0/doc/
--rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)   123854 2023-07-08 02:18:35.000000 BREWasm-1.0.0/doc/Definition.png
--rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)       38 2023-07-11 03:21:28.539031 BREWasm-1.0.0/setup.cfg
--rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)      651 2023-07-11 03:21:23.000000 BREWasm-1.0.0/setup.py
-drwxrwxr-x   0 obfuscator  (1000) obfuscator  (1000)        0 2023-07-11 03:21:28.539031 BREWasm-1.0.0/test/
--rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)     3794 2023-07-10 14:34:25.000000 BREWasm-1.0.0/test/test.py
--rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)       35 2023-07-10 14:00:23.000000 BREWasm-1.0.0/test/test_other.py
+drwxrwxrwx   0        0        0        0 2023-07-11 04:01:24.105033 BREWasm-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-07-11 04:01:24.075916 BREWasm-1.0.1/BREWasm/
+-rw-rw-rw-   0        0        0      232 2023-07-10 12:40:17.000000 BREWasm-1.0.1/BREWasm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 04:01:24.092510 BREWasm-1.0.1/BREWasm/parser/
+-rw-rw-rw-   0        0        0       12 2023-07-10 12:40:17.000000 BREWasm-1.0.1/BREWasm/parser/__init__.py
+-rw-rw-rw-   0        0        0      587 2023-07-10 12:40:17.000000 BREWasm-1.0.1/BREWasm/parser/errors.py
+-rw-rw-rw-   0        0        0      947 2023-07-10 12:40:17.000000 BREWasm-1.0.1/BREWasm/parser/instruction.py
+-rw-rw-rw-   0        0        0     2070 2023-07-10 12:40:17.000000 BREWasm-1.0.1/BREWasm/parser/leb128.py
+-rw-rw-rw-   0        0        0     5607 2023-07-10 12:40:17.000000 BREWasm-1.0.1/BREWasm/parser/module.py
+-rw-rw-rw-   0        0        0     3024 2023-07-10 12:40:17.000000 BREWasm-1.0.1/BREWasm/parser/opcodes.py
+-rw-rw-rw-   0        0        0     5960 2023-07-10 12:40:17.000000 BREWasm-1.0.1/BREWasm/parser/opnames.py
+-rw-rw-rw-   0        0        0    25050 2023-07-10 12:40:17.000000 BREWasm-1.0.1/BREWasm/parser/reader.py
+-rw-rw-rw-   0        0        0     3244 2023-07-10 12:40:17.000000 BREWasm-1.0.1/BREWasm/parser/types.py
+drwxrwxrwx   0        0        0        0 2023-07-11 04:01:24.101034 BREWasm-1.0.1/BREWasm/rewriter/
+-rw-rw-rw-   0        0        0      297 2023-07-11 03:58:12.000000 BREWasm-1.0.1/BREWasm/rewriter/BREWasm.py
+-rw-rw-rw-   0        0        0      230 2023-07-10 12:40:17.000000 BREWasm-1.0.1/BREWasm/rewriter/__init__.py
+-rw-rw-rw-   0        0        0     5164 2023-07-11 03:58:07.000000 BREWasm-1.0.1/BREWasm/rewriter/defination.py
+-rw-rw-rw-   0        0        0     5073 2023-07-11 03:58:00.000000 BREWasm-1.0.1/BREWasm/rewriter/indices_fixer.py
+-rw-rw-rw-   0        0        0    52278 2023-07-11 03:57:45.000000 BREWasm-1.0.1/BREWasm/rewriter/modify_binary.py
+-rw-rw-rw-   0        0        0    61990 2023-07-11 03:57:14.000000 BREWasm-1.0.1/BREWasm/rewriter/section_rewriter.py
+-rw-rw-rw-   0        0        0    22552 2023-07-11 03:56:55.000000 BREWasm-1.0.1/BREWasm/rewriter/semantics_rewriter.py
+drwxrwxrwx   0        0        0        0 2023-07-11 04:01:24.080438 BREWasm-1.0.1/BREWasm.egg-info/
+-rw-rw-rw-   0        0        0     3568 2023-07-11 04:01:24.000000 BREWasm-1.0.1/BREWasm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      646 2023-07-11 04:01:24.000000 BREWasm-1.0.1/BREWasm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 04:01:24.000000 BREWasm-1.0.1/BREWasm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 04:01:24.000000 BREWasm-1.0.1/BREWasm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3568 2023-07-11 04:01:24.104032 BREWasm-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6454 2023-07-10 12:40:17.000000 BREWasm-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 04:01:24.102033 BREWasm-1.0.1/doc/
+-rw-rw-rw-   0        0        0   123854 2023-07-10 12:40:17.000000 BREWasm-1.0.1/doc/Definition.png
+-rw-rw-rw-   0        0        0       42 2023-07-11 04:01:24.105033 BREWasm-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      668 2023-07-11 04:01:11.000000 BREWasm-1.0.1/setup.py
```

### Comparing `BREWasm-1.0.0/BREWasm/parser/errors.py` & `BREWasm-1.0.1/BREWasm/parser/errors.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-class ErrUnexpectedEnd(Exception):
-
-    def __init__(self):
-        super().__init__("unexpected end of section or function")
-
-    def __str__(self):
-        print("unexpected end of section or function")
-
-
-class ErrIntTooLong(Exception):
-
-    def __init__(self):
-        super().__init__("integer representation too long")
-
-    def __str__(self):
-        print("integer representation too long")
-
-
-class ErrIntTooLarge(Exception):
-
-    def __init__(self):
-        super().__init__("integer too large")
-
-    def __str__(self):
-        print("integer too large")
+class ErrUnexpectedEnd(Exception):
+
+    def __init__(self):
+        super().__init__("unexpected end of section or function")
+
+    def __str__(self):
+        print("unexpected end of section or function")
+
+
+class ErrIntTooLong(Exception):
+
+    def __init__(self):
+        super().__init__("integer representation too long")
+
+    def __str__(self):
+        print("integer representation too long")
+
+
+class ErrIntTooLarge(Exception):
+
+    def __init__(self):
+        super().__init__("integer too large")
+
+    def __str__(self):
+        print("integer too large")
```

### Comparing `BREWasm-1.0.0/BREWasm/parser/leb128.py` & `BREWasm-1.0.1/BREWasm/parser/leb128.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-from ..parser.errors import *
-
-
-def decode_var_uint(reader, size: int):
-    result = 0
-    i = 0
-    while True:
-        a = reader.read(1)
-        b = int.from_bytes(a, "little")
-
-        if i == size / 7:
-            if b & 0x80 != 0:
-                raise ErrIntTooLong
-            if b >> (size - i * 7) > 0:
-                raise ErrIntTooLarge
-        result |= (b & 0x7f) << (i * 7)
-        if b & 0x80 == 0:
-            return result, i + 1
-        i += 1
-    raise ErrUnexpectedEnd
-
-
-def decode_var_uint111(data, size: int):
-    result = 0
-    i = 0
-    while True:
-        b = int.from_bytes(data[:1], "little")
-        data = data[1:]
-
-        if i == size / 7:
-            if b & 0x80 != 0:
-                raise ErrIntTooLong
-            if b >> (size - i * 7) > 0:
-                raise ErrIntTooLarge
-        result |= (b & 0x7f) << (i * 7)
-        if b & 0x80 == 0:
-            return result, i + 1
-        i += 1
-    raise ErrUnexpectedEnd
-
-
-def decode_var_int(reader, size):
-    result = 0
-    i = 0
-    while True:
-        b = int.from_bytes(reader.read(1), "little")
-
-        if i == size / 7:
-            if b & 0x80 != 0:
-                raise ErrIntTooLong
-            if b & 0x40 == 0 and b >> (size - i * 7 - 1) != 0 or \
-                    b & 0x40 != 0 and int(b | 0x80) >> (size - i * 7 - 1) != -1:
-                raise ErrIntTooLarge
-        result |= (b & 0x7f) << (i * 7)
-        if b & 0x80 == 0:
-            if (i * 7 < size) and (b & 0x40 != 0):
-                result |= -1 << ((i + 1) * 7)
-            return result, i + 1
-        i += 1
-    raise ErrUnexpectedEnd
-
-
-def decode_var_uint_from_data(data, size: int):
-    result = 0
-    for i, b in enumerate(data):
-        if i == size / 7:
-            if b & 0x80 != 0:
-                raise ErrIntTooLong
-            if b >> (size - i * 7) > 0:
-                raise ErrIntTooLarge
-        result |= (b & 0x7f) << (i * 7)
-        if b & 0x80 == 0:
-            return result, i + 1
-    raise ErrUnexpectedEnd
+from ..parser.errors import *
+
+
+def decode_var_uint(reader, size: int):
+    result = 0
+    i = 0
+    while True:
+        a = reader.read(1)
+        b = int.from_bytes(a, "little")
+
+        if i == size / 7:
+            if b & 0x80 != 0:
+                raise ErrIntTooLong
+            if b >> (size - i * 7) > 0:
+                raise ErrIntTooLarge
+        result |= (b & 0x7f) << (i * 7)
+        if b & 0x80 == 0:
+            return result, i + 1
+        i += 1
+    raise ErrUnexpectedEnd
+
+
+def decode_var_uint111(data, size: int):
+    result = 0
+    i = 0
+    while True:
+        b = int.from_bytes(data[:1], "little")
+        data = data[1:]
+
+        if i == size / 7:
+            if b & 0x80 != 0:
+                raise ErrIntTooLong
+            if b >> (size - i * 7) > 0:
+                raise ErrIntTooLarge
+        result |= (b & 0x7f) << (i * 7)
+        if b & 0x80 == 0:
+            return result, i + 1
+        i += 1
+    raise ErrUnexpectedEnd
+
+
+def decode_var_int(reader, size):
+    result = 0
+    i = 0
+    while True:
+        b = int.from_bytes(reader.read(1), "little")
+
+        if i == size / 7:
+            if b & 0x80 != 0:
+                raise ErrIntTooLong
+            if b & 0x40 == 0 and b >> (size - i * 7 - 1) != 0 or \
+                    b & 0x40 != 0 and int(b | 0x80) >> (size - i * 7 - 1) != -1:
+                raise ErrIntTooLarge
+        result |= (b & 0x7f) << (i * 7)
+        if b & 0x80 == 0:
+            if (i * 7 < size) and (b & 0x40 != 0):
+                result |= -1 << ((i + 1) * 7)
+            return result, i + 1
+        i += 1
+    raise ErrUnexpectedEnd
+
+
+def decode_var_uint_from_data(data, size: int):
+    result = 0
+    for i, b in enumerate(data):
+        if i == size / 7:
+            if b & 0x80 != 0:
+                raise ErrIntTooLong
+            if b >> (size - i * 7) > 0:
+                raise ErrIntTooLarge
+        result |= (b & 0x7f) << (i * 7)
+        if b & 0x80 == 0:
+            return result, i + 1
+    raise ErrUnexpectedEnd
```

### Comparing `BREWasm-1.0.0/BREWasm/parser/opnames.py` & `BREWasm-1.0.1/BREWasm/parser/opnames.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-from ..parser.opcodes import *
-
-opnames = [""] * 256
-
-opnames[Unreachable] = "unreachable"
-opnames[Nop] = "nop"
-opnames[Block] = "block"
-opnames[Loop] = "loop"
-opnames[If] = "if"
-opnames[Else_] = "else"
-opnames[End_] = "end"
-opnames[Br] = "br"
-opnames[BrIf] = "br_if"
-opnames[BrTable] = "br_table"
-opnames[Return] = "return"
-opnames[Call] = "call"
-opnames[CallIndirect] = "call_indirect"
-opnames[Drop] = "drop"
-opnames[Select] = "select"
-opnames[LocalGet] = "local.get"
-opnames[LocalSet] = "local.set"
-opnames[LocalTee] = "local.tee"
-opnames[GlobalGet] = "global.get"
-opnames[GlobalSet] = "global.set"
-opnames[I32Load] = "i32.load"
-opnames[I64Load] = "i64.load"
-opnames[F32Load] = "f32.load"
-opnames[F64Load] = "f64.load"
-opnames[I32Load8S] = "i32.load8_s"
-opnames[I32Load8U] = "i32.load8_u"
-opnames[I32Load16S] = "i32.load16_s"
-opnames[I32Load16U] = "i32.load16_u"
-opnames[I64Load8S] = "i64.load8_s"
-opnames[I64Load8U] = "i64.load8_u"
-opnames[I64Load16S] = "i64.load16_s"
-opnames[I64Load16U] = "i64.load16_u"
-opnames[I64Load32S] = "i64.load32_s"
-opnames[I64Load32U] = "i64.load32_u"
-opnames[I32Store] = "i32.store"
-opnames[I64Store] = "i64.store"
-opnames[F32Store] = "f32.store"
-opnames[F64Store] = "f64.store"
-opnames[I32Store8] = "i32.store8"
-opnames[I32Store16] = "i32.store16"
-opnames[I64Store8] = "i64.store8"
-opnames[I64Store16] = "i64.store16"
-opnames[I64Store32] = "i64.store32"
-opnames[MemorySize] = "memory.size"
-opnames[MemoryGrow] = "memory.grow"
-opnames[I32Const] = "i32.const"
-opnames[I64Const] = "i64.const"
-opnames[F32Const] = "f32.const"
-opnames[F64Const] = "f64.const"
-opnames[I32Eqz] = "i32.eqz"
-opnames[I32Eq] = "i32.eq"
-opnames[I32Ne] = "i32.ne"
-opnames[I32LtS] = "i32.lt_s"
-opnames[I32LtU] = "i32.lt_u"
-opnames[I32GtS] = "i32.gt_s"
-opnames[I32GtU] = "i32.gt_u"
-opnames[I32LeS] = "i32.le_s"
-opnames[I32LeU] = "i32.le_u"
-opnames[I32GeS] = "i32.ge_s"
-opnames[I32GeU] = "i32.ge_u"
-opnames[I64Eqz] = "i64.eqz"
-opnames[I64Eq] = "i64.eq"
-opnames[I64Ne] = "i64.ne"
-opnames[I64LtS] = "i64.lt_s"
-opnames[I64LtU] = "i64.lt_u"
-opnames[I64GtS] = "i64.gt_s"
-opnames[I64GtU] = "i64.gt_u"
-opnames[I64LeS] = "i64.le_s"
-opnames[I64LeU] = "i64.le_u"
-opnames[I64GeS] = "i64.ge_s"
-opnames[I64GeU] = "i64.ge_u"
-opnames[F32Eq] = "f32.eq"
-opnames[F32Ne] = "f32.ne"
-opnames[F32Lt] = "f32.lt"
-opnames[F32Gt] = "f32.gt"
-opnames[F32Le] = "f32.le"
-opnames[F32Ge] = "f32.ge"
-opnames[F64Eq] = "f64.eq"
-opnames[F64Ne] = "f64.ne"
-opnames[F64Lt] = "f64.lt"
-opnames[F64Gt] = "f64.gt"
-opnames[F64Le] = "f64.le"
-opnames[F64Ge] = "f64.ge"
-opnames[I32Clz] = "i32.clz"
-opnames[I32Ctz] = "i32.ctz"
-opnames[I32PopCnt] = "i32.popcnt"
-opnames[I32Add] = "i32.add"
-opnames[I32Sub] = "i32.sub"
-opnames[I32Mul] = "i32.mul"
-opnames[I32DivS] = "i32.div_s"
-opnames[I32DivU] = "i32.div_u"
-opnames[I32RemS] = "i32.rem_s"
-opnames[I32RemU] = "i32.rem_u"
-opnames[I32And] = "i32.and"
-opnames[I32Or] = "i32.or"
-opnames[I32Xor] = "i32.xor"
-opnames[I32Shl] = "i32.shl"
-opnames[I32ShrS] = "i32.shr_s"
-opnames[I32ShrU] = "i32.shr_u"
-opnames[I32Rotl] = "i32.rotl"
-opnames[I32Rotr] = "i32.rotr"
-opnames[I64Clz] = "i64.clz"
-opnames[I64Ctz] = "i64.ctz"
-opnames[I64PopCnt] = "i64.popcnt"
-opnames[I64Add] = "i64.add"
-opnames[I64Sub] = "i64.sub"
-opnames[I64Mul] = "i64.mul"
-opnames[I64DivS] = "i64.div_s"
-opnames[I64DivU] = "i64.div_u"
-opnames[I64RemS] = "i64.rem_s"
-opnames[I64RemU] = "i64.rem_u"
-opnames[I64And] = "i64.and"
-opnames[I64Or] = "i64.or"
-opnames[I64Xor] = "i64.xor"
-opnames[I64Shl] = "i64.shl"
-opnames[I64ShrS] = "i64.shr_s"
-opnames[I64ShrU] = "i64.shr_u"
-opnames[I64Rotl] = "i64.rotl"
-opnames[I64Rotr] = "i64.rotr"
-opnames[F32Abs] = "f32.abs"
-opnames[F32Neg] = "f32.neg"
-opnames[F32Ceil] = "f32.ceil"
-opnames[F32Floor] = "f32.floor"
-opnames[F32Trunc] = "f32.trunc"
-opnames[F32Nearest] = "f32.nearest"
-opnames[F32Sqrt] = "f32.sqrt"
-opnames[F32Add] = "f32.add"
-opnames[F32Sub] = "f32.sub"
-opnames[F32Mul] = "f32.mul"
-opnames[F32Div] = "f32.div"
-opnames[F32Min] = "f32.min"
-opnames[F32Max] = "f32.max"
-opnames[F32CopySign] = "f32.copysign"
-opnames[F64Abs] = "f64.abs"
-opnames[F64Neg] = "f64.neg"
-opnames[F64Ceil] = "f64.ceil"
-opnames[F64Floor] = "f64.floor"
-opnames[F64Trunc] = "f64.trunc"
-opnames[F64Nearest] = "f64.nearest"
-opnames[F64Sqrt] = "f64.sqrt"
-opnames[F64Add] = "f64.add"
-opnames[F64Sub] = "f64.sub"
-opnames[F64Mul] = "f64.mul"
-opnames[F64Div] = "f64.div"
-opnames[F64Min] = "f64.min"
-opnames[F64Max] = "f64.max"
-opnames[F64CopySign] = "f64.copysign"
-opnames[I32WrapI64] = "i32.wrap_i64"
-opnames[I32TruncF32S] = "i32.trunc_f32_s"
-opnames[I32TruncF32U] = "i32.trunc_f32_u"
-opnames[I32TruncF64S] = "i32.trunc_f64_s"
-opnames[I32TruncF64U] = "i32.trunc_f64_u"
-opnames[I64ExtendI32S] = "i64.extend_i32_s"
-opnames[I64ExtendI32U] = "i64.extend_i32_u"
-opnames[I64TruncF32S] = "i64.trunc_f32_s"
-opnames[I64TruncF32U] = "i64.trunc_f32_u"
-opnames[I64TruncF64S] = "i64.trunc_f64_s"
-opnames[I64TruncF64U] = "i64.trunc_f64_u"
-opnames[F32ConvertI32S] = "f32.convert_i32_s"
-opnames[F32ConvertI32U] = "f32.convert_i32_u"
-opnames[F32ConvertI64S] = "f32.convert_i64_s"
-opnames[F32ConvertI64U] = "f32.convert_i64_u"
-opnames[F32DemoteF64] = "f32.demote_f64"
-opnames[F64ConvertI32S] = "f64.convert_i32_s"
-opnames[F64ConvertI32U] = "f64.convert_i32_u"
-opnames[F64ConvertI64S] = "f64.convert_i64_s"
-opnames[F64ConvertI64U] = "f64.convert_i64_u"
-opnames[F64PromoteF32] = "f64.promote_f32"
-opnames[I32ReinterpretF32] = "i32.reinterpret_f32"
-opnames[I64ReinterpretF64] = "i64.reinterpret_f64"
-opnames[F32ReinterpretI32] = "f32.reinterpret_i32"
-opnames[F64ReinterpretI64] = "f64.reinterpret_i64"
-opnames[I32Extend8S] = "i32.extend8_s"
-opnames[I32Extend16S] = "i32.extend16_s"
-opnames[I64Extend8S] = "i64.extend8_s"
-opnames[I64Extend16S] = "i64.extend16_s"
-opnames[I64Extend32S] = "i64.extend32_s"
-opnames[TruncSat] = "trunc_sat"
+from ..parser.opcodes import *
+
+opnames = [""] * 256
+
+opnames[Unreachable] = "unreachable"
+opnames[Nop] = "nop"
+opnames[Block] = "block"
+opnames[Loop] = "loop"
+opnames[If] = "if"
+opnames[Else_] = "else"
+opnames[End_] = "end"
+opnames[Br] = "br"
+opnames[BrIf] = "br_if"
+opnames[BrTable] = "br_table"
+opnames[Return] = "return"
+opnames[Call] = "call"
+opnames[CallIndirect] = "call_indirect"
+opnames[Drop] = "drop"
+opnames[Select] = "select"
+opnames[LocalGet] = "local.get"
+opnames[LocalSet] = "local.set"
+opnames[LocalTee] = "local.tee"
+opnames[GlobalGet] = "global.get"
+opnames[GlobalSet] = "global.set"
+opnames[I32Load] = "i32.load"
+opnames[I64Load] = "i64.load"
+opnames[F32Load] = "f32.load"
+opnames[F64Load] = "f64.load"
+opnames[I32Load8S] = "i32.load8_s"
+opnames[I32Load8U] = "i32.load8_u"
+opnames[I32Load16S] = "i32.load16_s"
+opnames[I32Load16U] = "i32.load16_u"
+opnames[I64Load8S] = "i64.load8_s"
+opnames[I64Load8U] = "i64.load8_u"
+opnames[I64Load16S] = "i64.load16_s"
+opnames[I64Load16U] = "i64.load16_u"
+opnames[I64Load32S] = "i64.load32_s"
+opnames[I64Load32U] = "i64.load32_u"
+opnames[I32Store] = "i32.store"
+opnames[I64Store] = "i64.store"
+opnames[F32Store] = "f32.store"
+opnames[F64Store] = "f64.store"
+opnames[I32Store8] = "i32.store8"
+opnames[I32Store16] = "i32.store16"
+opnames[I64Store8] = "i64.store8"
+opnames[I64Store16] = "i64.store16"
+opnames[I64Store32] = "i64.store32"
+opnames[MemorySize] = "memory.size"
+opnames[MemoryGrow] = "memory.grow"
+opnames[I32Const] = "i32.const"
+opnames[I64Const] = "i64.const"
+opnames[F32Const] = "f32.const"
+opnames[F64Const] = "f64.const"
+opnames[I32Eqz] = "i32.eqz"
+opnames[I32Eq] = "i32.eq"
+opnames[I32Ne] = "i32.ne"
+opnames[I32LtS] = "i32.lt_s"
+opnames[I32LtU] = "i32.lt_u"
+opnames[I32GtS] = "i32.gt_s"
+opnames[I32GtU] = "i32.gt_u"
+opnames[I32LeS] = "i32.le_s"
+opnames[I32LeU] = "i32.le_u"
+opnames[I32GeS] = "i32.ge_s"
+opnames[I32GeU] = "i32.ge_u"
+opnames[I64Eqz] = "i64.eqz"
+opnames[I64Eq] = "i64.eq"
+opnames[I64Ne] = "i64.ne"
+opnames[I64LtS] = "i64.lt_s"
+opnames[I64LtU] = "i64.lt_u"
+opnames[I64GtS] = "i64.gt_s"
+opnames[I64GtU] = "i64.gt_u"
+opnames[I64LeS] = "i64.le_s"
+opnames[I64LeU] = "i64.le_u"
+opnames[I64GeS] = "i64.ge_s"
+opnames[I64GeU] = "i64.ge_u"
+opnames[F32Eq] = "f32.eq"
+opnames[F32Ne] = "f32.ne"
+opnames[F32Lt] = "f32.lt"
+opnames[F32Gt] = "f32.gt"
+opnames[F32Le] = "f32.le"
+opnames[F32Ge] = "f32.ge"
+opnames[F64Eq] = "f64.eq"
+opnames[F64Ne] = "f64.ne"
+opnames[F64Lt] = "f64.lt"
+opnames[F64Gt] = "f64.gt"
+opnames[F64Le] = "f64.le"
+opnames[F64Ge] = "f64.ge"
+opnames[I32Clz] = "i32.clz"
+opnames[I32Ctz] = "i32.ctz"
+opnames[I32PopCnt] = "i32.popcnt"
+opnames[I32Add] = "i32.add"
+opnames[I32Sub] = "i32.sub"
+opnames[I32Mul] = "i32.mul"
+opnames[I32DivS] = "i32.div_s"
+opnames[I32DivU] = "i32.div_u"
+opnames[I32RemS] = "i32.rem_s"
+opnames[I32RemU] = "i32.rem_u"
+opnames[I32And] = "i32.and"
+opnames[I32Or] = "i32.or"
+opnames[I32Xor] = "i32.xor"
+opnames[I32Shl] = "i32.shl"
+opnames[I32ShrS] = "i32.shr_s"
+opnames[I32ShrU] = "i32.shr_u"
+opnames[I32Rotl] = "i32.rotl"
+opnames[I32Rotr] = "i32.rotr"
+opnames[I64Clz] = "i64.clz"
+opnames[I64Ctz] = "i64.ctz"
+opnames[I64PopCnt] = "i64.popcnt"
+opnames[I64Add] = "i64.add"
+opnames[I64Sub] = "i64.sub"
+opnames[I64Mul] = "i64.mul"
+opnames[I64DivS] = "i64.div_s"
+opnames[I64DivU] = "i64.div_u"
+opnames[I64RemS] = "i64.rem_s"
+opnames[I64RemU] = "i64.rem_u"
+opnames[I64And] = "i64.and"
+opnames[I64Or] = "i64.or"
+opnames[I64Xor] = "i64.xor"
+opnames[I64Shl] = "i64.shl"
+opnames[I64ShrS] = "i64.shr_s"
+opnames[I64ShrU] = "i64.shr_u"
+opnames[I64Rotl] = "i64.rotl"
+opnames[I64Rotr] = "i64.rotr"
+opnames[F32Abs] = "f32.abs"
+opnames[F32Neg] = "f32.neg"
+opnames[F32Ceil] = "f32.ceil"
+opnames[F32Floor] = "f32.floor"
+opnames[F32Trunc] = "f32.trunc"
+opnames[F32Nearest] = "f32.nearest"
+opnames[F32Sqrt] = "f32.sqrt"
+opnames[F32Add] = "f32.add"
+opnames[F32Sub] = "f32.sub"
+opnames[F32Mul] = "f32.mul"
+opnames[F32Div] = "f32.div"
+opnames[F32Min] = "f32.min"
+opnames[F32Max] = "f32.max"
+opnames[F32CopySign] = "f32.copysign"
+opnames[F64Abs] = "f64.abs"
+opnames[F64Neg] = "f64.neg"
+opnames[F64Ceil] = "f64.ceil"
+opnames[F64Floor] = "f64.floor"
+opnames[F64Trunc] = "f64.trunc"
+opnames[F64Nearest] = "f64.nearest"
+opnames[F64Sqrt] = "f64.sqrt"
+opnames[F64Add] = "f64.add"
+opnames[F64Sub] = "f64.sub"
+opnames[F64Mul] = "f64.mul"
+opnames[F64Div] = "f64.div"
+opnames[F64Min] = "f64.min"
+opnames[F64Max] = "f64.max"
+opnames[F64CopySign] = "f64.copysign"
+opnames[I32WrapI64] = "i32.wrap_i64"
+opnames[I32TruncF32S] = "i32.trunc_f32_s"
+opnames[I32TruncF32U] = "i32.trunc_f32_u"
+opnames[I32TruncF64S] = "i32.trunc_f64_s"
+opnames[I32TruncF64U] = "i32.trunc_f64_u"
+opnames[I64ExtendI32S] = "i64.extend_i32_s"
+opnames[I64ExtendI32U] = "i64.extend_i32_u"
+opnames[I64TruncF32S] = "i64.trunc_f32_s"
+opnames[I64TruncF32U] = "i64.trunc_f32_u"
+opnames[I64TruncF64S] = "i64.trunc_f64_s"
+opnames[I64TruncF64U] = "i64.trunc_f64_u"
+opnames[F32ConvertI32S] = "f32.convert_i32_s"
+opnames[F32ConvertI32U] = "f32.convert_i32_u"
+opnames[F32ConvertI64S] = "f32.convert_i64_s"
+opnames[F32ConvertI64U] = "f32.convert_i64_u"
+opnames[F32DemoteF64] = "f32.demote_f64"
+opnames[F64ConvertI32S] = "f64.convert_i32_s"
+opnames[F64ConvertI32U] = "f64.convert_i32_u"
+opnames[F64ConvertI64S] = "f64.convert_i64_s"
+opnames[F64ConvertI64U] = "f64.convert_i64_u"
+opnames[F64PromoteF32] = "f64.promote_f32"
+opnames[I32ReinterpretF32] = "i32.reinterpret_f32"
+opnames[I64ReinterpretF64] = "i64.reinterpret_f64"
+opnames[F32ReinterpretI32] = "f32.reinterpret_i32"
+opnames[F64ReinterpretI64] = "f64.reinterpret_i64"
+opnames[I32Extend8S] = "i32.extend8_s"
+opnames[I32Extend16S] = "i32.extend16_s"
+opnames[I64Extend8S] = "i64.extend8_s"
+opnames[I64Extend16S] = "i64.extend16_s"
+opnames[I64Extend32S] = "i64.extend32_s"
+opnames[TruncSat] = "trunc_sat"
```

### Comparing `BREWasm-1.0.0/BREWasm/parser/types.py` & `BREWasm-1.0.1/BREWasm/parser/types.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-I32 = 0x7F
-
-I64 = 0x7E
-
-F32 = 0x7D
-
-F64 = 0x7C
-
-BlockTypeI32 = -1
-BlockTypeI64 = -2
-BlockTypeF32 = -3
-BlockTypeF64 = -4
-BlockTypeEmpty = -64
-
-FtTag = 0x60
-FuncRef = 0x70
-
-MutConst = 0
-MutVar = 1
-
-
-class FuncType:
-
-    def __init__(self, tag=0, param_types=None, result_types=None):
-        if result_types is None:
-            result_types = []
-        if param_types is None:
-            param_types = []
-        self.tag = tag
-
-        self.param_types = param_types
-
-        self.result_types = result_types
-
-    def equal(self, ft2) -> bool:
-        if len(self.param_types) != len(ft2.param_types) \
-                or len(self.result_types) != len(ft2.result_types):
-            return False
-        for i, vt in enumerate(self.param_types):
-            if vt != ft2.param_types[i]:
-                return False
-        for i, vt in enumerate(self.result_types):
-            if vt != ft2.result_types[i]:
-                return False
-        return True
-
-    def print_signature(self) -> str:
-        sb = "("
-        sb += ",".join([val_type_to_str(vt) for vt in self.param_types])
-        sb += ")->("
-        sb += ",".join([val_type_to_str(vt) for vt in self.result_types])
-        sb += ")"
-        return sb
-
-    def get_signature(self):
-        arg_types = []
-        ret_types = []
-        for valtype in self.param_types:
-            if valtype == I32:
-                arg_types.append("i32")
-            elif valtype == I64:
-                arg_types.append("i64")
-            elif valtype == F32:
-                arg_types.append("f32")
-            elif valtype == F64:
-                arg_types.append("f64")
-        for valtype in self.result_types:
-            if valtype == I32:
-                ret_types.append("i32")
-            elif valtype == I64:
-                ret_types.append("i64")
-            elif valtype == F32:
-                ret_types.append("f32")
-            elif valtype == F64:
-                ret_types.append("f64")
-        return arg_types, ret_types
-
-    def __str__(self):
-        return self.print_signature()
-
-
-class Limits:
-
-    def __init__(self, tag=0, min=0, max=0):
-        self.tag = tag
-        self.min = min
-        self.max = max
-
-    def __str__(self):
-        return "{min: %d, max: %d}" % (self.min, self.max)
-
-
-MemType = Limits
-
-
-class TableType:
-
-    def __init__(self, elem_type=0x70, limits=None):
-        self.elem_type = elem_type
-
-        self.limits = limits
-
-
-class GlobalType:
-
-    def __init__(self, val_type=0, mut=0):
-        self.val_type = val_type
-
-        self.mut = mut
-
-    def __str__(self):
-        return "{type: %s, mut: %d}" % (val_type_to_str(self.val_type), self.mut)
-
-
-class NameAssoc:
-
-    def __init__(self, idx=0, name=None):
-        self.idx = idx
-
-        self.name = name
-
-    def __str__(self):
-        return "{id: %d, name: %s}" % (self.idx, self.name)
-
-
-def val_type_to_str(vt) -> str:
-    if vt == I32:
-        return "i32"
-    elif vt == I64:
-        return "i64"
-    elif vt == F32:
-        return "f32"
-    elif vt == F64:
-        return "f64"
-    else:
-        raise Exception("invalid valtype: %d" % vt)
+I32 = 0x7F
+
+I64 = 0x7E
+
+F32 = 0x7D
+
+F64 = 0x7C
+
+BlockTypeI32 = -1
+BlockTypeI64 = -2
+BlockTypeF32 = -3
+BlockTypeF64 = -4
+BlockTypeEmpty = -64
+
+FtTag = 0x60
+FuncRef = 0x70
+
+MutConst = 0
+MutVar = 1
+
+
+class FuncType:
+
+    def __init__(self, tag=0, param_types=None, result_types=None):
+        if result_types is None:
+            result_types = []
+        if param_types is None:
+            param_types = []
+        self.tag = tag
+
+        self.param_types = param_types
+
+        self.result_types = result_types
+
+    def equal(self, ft2) -> bool:
+        if len(self.param_types) != len(ft2.param_types) \
+                or len(self.result_types) != len(ft2.result_types):
+            return False
+        for i, vt in enumerate(self.param_types):
+            if vt != ft2.param_types[i]:
+                return False
+        for i, vt in enumerate(self.result_types):
+            if vt != ft2.result_types[i]:
+                return False
+        return True
+
+    def print_signature(self) -> str:
+        sb = "("
+        sb += ",".join([val_type_to_str(vt) for vt in self.param_types])
+        sb += ")->("
+        sb += ",".join([val_type_to_str(vt) for vt in self.result_types])
+        sb += ")"
+        return sb
+
+    def get_signature(self):
+        arg_types = []
+        ret_types = []
+        for valtype in self.param_types:
+            if valtype == I32:
+                arg_types.append("i32")
+            elif valtype == I64:
+                arg_types.append("i64")
+            elif valtype == F32:
+                arg_types.append("f32")
+            elif valtype == F64:
+                arg_types.append("f64")
+        for valtype in self.result_types:
+            if valtype == I32:
+                ret_types.append("i32")
+            elif valtype == I64:
+                ret_types.append("i64")
+            elif valtype == F32:
+                ret_types.append("f32")
+            elif valtype == F64:
+                ret_types.append("f64")
+        return arg_types, ret_types
+
+    def __str__(self):
+        return self.print_signature()
+
+
+class Limits:
+
+    def __init__(self, tag=0, min=0, max=0):
+        self.tag = tag
+        self.min = min
+        self.max = max
+
+    def __str__(self):
+        return "{min: %d, max: %d}" % (self.min, self.max)
+
+
+MemType = Limits
+
+
+class TableType:
+
+    def __init__(self, elem_type=0x70, limits=None):
+        self.elem_type = elem_type
+
+        self.limits = limits
+
+
+class GlobalType:
+
+    def __init__(self, val_type=0, mut=0):
+        self.val_type = val_type
+
+        self.mut = mut
+
+    def __str__(self):
+        return "{type: %s, mut: %d}" % (val_type_to_str(self.val_type), self.mut)
+
+
+class NameAssoc:
+
+    def __init__(self, idx=0, name=None):
+        self.idx = idx
+
+        self.name = name
+
+    def __str__(self):
+        return "{id: %d, name: %s}" % (self.idx, self.name)
+
+
+def val_type_to_str(vt) -> str:
+    if vt == I32:
+        return "i32"
+    elif vt == I64:
+        return "i64"
+    elif vt == F32:
+        return "f32"
+    elif vt == F64:
+        return "f64"
+    else:
+        raise Exception("invalid valtype: %d" % vt)
```

### Comparing `BREWasm-1.0.0/BREWasm/rewriter/defination.py` & `BREWasm-1.0.1/BREWasm/rewriter/defination.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-from enum import Enum
-
-from ..parser.module import Export as OriginExport
-from ..parser.module import ExportDesc
-from ..parser.module import Global as OriginGlobal
-from ..parser.module import Import as OriginImport
-from ..parser.module import ImportDesc
-from ..parser.module import Locals
-from ..parser.types import *
-
-FunctionName = 0
-GlobalName = 1
-DataName = 2
-
-
-class SectionName(Enum):
-    CustomSec = 0
-    TypeSec = 1
-    ImportSec = 2
-    FuncSec = 3
-    TableSec = 4
-    MemSec = 5
-    GlobalSec = 6
-    ExportSec = 7
-    StartSec = 8
-    ElemSec = 9
-    CodeSec = 10
-    DataSec = 11
-    DataCountSec = 12
-
-
-class ValType(Enum):
-    I32 = 0x7F
-
-    I64 = 0x7E
-
-    F32 = 0x7D
-
-    F64 = 0x7C
-
-
-class Type:
-
-    def __init__(self, typeidx=None, arg_types=None, ret_types=None):
-        self.typeidx = typeidx
-
-        self.arg_types = arg_types
-
-        self.ret_types = ret_types
-
-    def convert(self):
-        param_types = []
-        result_types = []
-        if self.arg_types is not None:
-            for arg in self.arg_types:
-                match arg:
-                    # I32
-                    case 127:
-                        param_types.append(I32)
-                    # I64
-                    case 126:
-                        param_types.append(I64)
-                    # F32
-                    case 125:
-                        param_types.append(F32)
-                    # F64
-                    case 124:
-                        param_types.append(F64)
-
-        if self.ret_types is not None:
-            for arg in self.ret_types:
-                match arg:
-                    # I32
-                    case 127:
-                        result_types.append(I32)
-                    # I64
-                    case 126:
-                        result_types.append(I64)
-                    # F32
-                    case 125:
-                        result_types.append(F32)
-                    # F64
-                    case 124:
-                        result_types.append(F64)
-
-        return FuncType(FtTag, param_types, result_types)
-
-
-class Import:
-
-    def __init__(self, importidx=None, module=None, name=None, typeidx=None):
-        self.importidx = importidx
-        self.module = module
-        self.name = name
-        self.typeidx = typeidx
-
-    def convert(self):
-        return OriginImport(self.module, self.name, ImportDesc(0, func_type=self.typeidx))
-
-
-class Export:
-
-    def __init__(self, exportidx=None, name=None, funcidx=None):
-        self.exportidx = exportidx
-        self.name = name
-        self.funcidx = funcidx
-
-    def convert(self):
-        return OriginExport(self.name, ExportDesc(0, idx=self.funcidx))
-
-
-class Function:
-    def __init__(self, funcidx=None, typeidx=None):
-        self.funcidx = funcidx
-        self.typeidx = typeidx
-
-    def convert(self):
-        return self.typeidx
-
-
-class Table:
-    def __init__(self, min=None, max=None):
-        self.min = min
-        self.max = max
-
-
-class Memory:
-    def __init__(self, min=None, max=None):
-        self.min = min
-        self.max = max
-
-
-class Global:
-    def __init__(self, globalidx=None, valtype=None, mut=None, val=None):
-        self.globalidx = globalidx
-        self.valtype = valtype
-        self.mut = mut
-        self.val = val
-
-    def convert(self):
-        return OriginGlobal(GlobalType(val_type=self.valtype, mut=self.mut), init=self.val)
-
-
-class Element:
-    def __init__(self, elemidx=None, tableidx=None, offset=None, funcidx_list=None):
-        self.elemidx = elemidx
-        self.tableidx = tableidx
-        self.offset = offset
-        self.funcidx_list = funcidx_list
-
-
-class Code:
-    def __init__(self, funcidx=None, local_vec=None, instr_list=None):
-        self.funcidx = funcidx
-        self.local_vec = local_vec
-        self.instr_list = instr_list
-
-    def convert_local_vec(self):
-        locals_list = []
-        for _, local in enumerate(self.local_vec):
-            match local.valtype:
-                case ValType.I32.value:
-                    locals_list.append(Locals(1, ValType.I32.value))
-                case ValType.I64.value:
-                    locals_list.append(Locals(1, ValType.I64.value))
-                case ValType.F32.value:
-                    locals_list.append(Locals(1, ValType.F32.value))
-                case ValType.F64.value:
-                    locals_list.append(Locals(1, ValType.F64.value))
-        return locals_list
-
-
-class Local:
-    def __init__(self, localidx=None, valtype=None):
-        self.localidx = localidx
-        self.valtype = valtype
-
-
-class Start:
-    def __init__(self, funcidx=None):
-        self.funcidx = funcidx
-
-
-class Data:
-    def __init__(self, dataidx=None, offset=None, init_data=None):
-        self.dataidx = dataidx
-        self.offset = offset
-        self.init_data = init_data
-
-
-class CustomName:
-    def __init__(self, name_type=None, idx=None, name=None):
-        self.name_type = name_type
-        self.idx = idx
-        self.name = name
+from enum import Enum
+
+from ..parser.module import Export as OriginExport
+from ..parser.module import ExportDesc
+from ..parser.module import Global as OriginGlobal
+from ..parser.module import Import as OriginImport
+from ..parser.module import ImportDesc
+from ..parser.module import Locals
+from ..parser.types import *
+
+FunctionName = 0
+GlobalName = 1
+DataName = 2
+
+
+class SectionName(Enum):
+    CustomSec = 0
+    TypeSec = 1
+    ImportSec = 2
+    FuncSec = 3
+    TableSec = 4
+    MemSec = 5
+    GlobalSec = 6
+    ExportSec = 7
+    StartSec = 8
+    ElemSec = 9
+    CodeSec = 10
+    DataSec = 11
+    DataCountSec = 12
+
+
+class ValType(Enum):
+    I32 = 0x7F
+
+    I64 = 0x7E
+
+    F32 = 0x7D
+
+    F64 = 0x7C
+
+
+class Type:
+
+    def __init__(self, typeidx=None, arg_types=None, ret_types=None):
+        self.typeidx = typeidx
+
+        self.arg_types = arg_types
+
+        self.ret_types = ret_types
+
+    def convert(self):
+        param_types = []
+        result_types = []
+        if self.arg_types is not None:
+            for arg in self.arg_types:
+                match arg:
+                    # I32
+                    case 127:
+                        param_types.append(I32)
+                    # I64
+                    case 126:
+                        param_types.append(I64)
+                    # F32
+                    case 125:
+                        param_types.append(F32)
+                    # F64
+                    case 124:
+                        param_types.append(F64)
+
+        if self.ret_types is not None:
+            for arg in self.ret_types:
+                match arg:
+                    # I32
+                    case 127:
+                        result_types.append(I32)
+                    # I64
+                    case 126:
+                        result_types.append(I64)
+                    # F32
+                    case 125:
+                        result_types.append(F32)
+                    # F64
+                    case 124:
+                        result_types.append(F64)
+
+        return FuncType(FtTag, param_types, result_types)
+
+
+class Import:
+
+    def __init__(self, importidx=None, module=None, name=None, typeidx=None):
+        self.importidx = importidx
+        self.module = module
+        self.name = name
+        self.typeidx = typeidx
+
+    def convert(self):
+        return OriginImport(self.module, self.name, ImportDesc(0, func_type=self.typeidx))
+
+
+class Export:
+
+    def __init__(self, exportidx=None, name=None, funcidx=None):
+        self.exportidx = exportidx
+        self.name = name
+        self.funcidx = funcidx
+
+    def convert(self):
+        return OriginExport(self.name, ExportDesc(0, idx=self.funcidx))
+
+
+class Function:
+    def __init__(self, funcidx=None, typeidx=None):
+        self.funcidx = funcidx
+        self.typeidx = typeidx
+
+    def convert(self):
+        return self.typeidx
+
+
+class Table:
+    def __init__(self, min=None, max=None):
+        self.min = min
+        self.max = max
+
+
+class Memory:
+    def __init__(self, min=None, max=None):
+        self.min = min
+        self.max = max
+
+
+class Global:
+    def __init__(self, globalidx=None, valtype=None, mut=None, val=None):
+        self.globalidx = globalidx
+        self.valtype = valtype
+        self.mut = mut
+        self.val = val
+
+    def convert(self):
+        return OriginGlobal(GlobalType(val_type=self.valtype, mut=self.mut), init=self.val)
+
+
+class Element:
+    def __init__(self, elemidx=None, tableidx=None, offset=None, funcidx_list=None):
+        self.elemidx = elemidx
+        self.tableidx = tableidx
+        self.offset = offset
+        self.funcidx_list = funcidx_list
+
+
+class Code:
+    def __init__(self, funcidx=None, local_vec=None, instr_list=None):
+        self.funcidx = funcidx
+        self.local_vec = local_vec
+        self.instr_list = instr_list
+
+    def convert_local_vec(self):
+        locals_list = []
+        for _, local in enumerate(self.local_vec):
+            match local.valtype:
+                case ValType.I32.value:
+                    locals_list.append(Locals(1, ValType.I32.value))
+                case ValType.I64.value:
+                    locals_list.append(Locals(1, ValType.I64.value))
+                case ValType.F32.value:
+                    locals_list.append(Locals(1, ValType.F32.value))
+                case ValType.F64.value:
+                    locals_list.append(Locals(1, ValType.F64.value))
+        return locals_list
+
+
+class Local:
+    def __init__(self, localidx=None, valtype=None):
+        self.localidx = localidx
+        self.valtype = valtype
+
+
+class Start:
+    def __init__(self, funcidx=None):
+        self.funcidx = funcidx
+
+
+class Data:
+    def __init__(self, dataidx=None, offset=None, init_data=None):
+        self.dataidx = dataidx
+        self.offset = offset
+        self.init_data = init_data
+
+
+class CustomName:
+    def __init__(self, name_type=None, idx=None, name=None):
+        self.name_type = name_type
+        self.idx = idx
+        self.name = name
```

### Comparing `BREWasm-1.0.0/BREWasm/rewriter/modify_binary.py` & `BREWasm-1.0.1/BREWasm/rewriter/modify_binary.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,1111 +1,1111 @@
-import os
-import struct
-
-from leb128 import LEB128U, LEB128S
-from shutil import copyfile
-from BREWasm.parser import reader
-from BREWasm.parser.instruction import Instruction
-from BREWasm.parser.module import *
-from BREWasm.parser.opcodes import *
-from BREWasm.parser.types import val_type_to_str, GlobalType
-
-
-class ModifyBinary:
-
-    def __init__(self,  path, module=None):
-        if module is None:
-            module, err = reader.decode_file(path)
-            if err is not None:
-                print(err.args)
-                print("=================================")
-                raise Exception("Failed to read the wasm file!")
-
-            self.module = module
-            self.module.path = path
-
-            self.func_name = []
-            for custom in self.module.custom_secs:
-                if custom.name == "name":
-                    if custom.name_data.funcNameSubSec is not None:
-
-                        for func_name_item in custom.name_data.funcNameSubSec[self.get_import_func_num():]:
-                            self.func_name.append(func_name_item.name)
-        else:
-            self.module = module
-            self.module.path = path
-
-    def emit_binary(self, path):
-        file_path = self.module.path
-        
-        if not os.path.exists(path):
-            copyfile(self.module.path, path)
-            file_path = path
-        elif not os.path.samefile(self.module.path, path):
-            if os.path.isfile(path):
-                os.remove(path)
-            copyfile(self.module.path, path)
-            file_path = path
-
-        self.change_custom_name_section(self.module.custom_secs, file_path)
-        self.change_type_section(self.module.type_sec, file_path)
-        self.change_import_section(self.module.import_sec, file_path)
-        self.change_export_section(self.module.export_sec, file_path)
-        self.change_func_section(self.module.func_sec, file_path)
-        self.change_code_section(self.module.code_sec, file_path)
-        self.change_table_section(self.module.table_sec, file_path)
-        self.change_elem_section(self.module.elem_sec, file_path)
-        self.change_memory_section(self.module.mem_sec, file_path)
-        self.change_data_section(self.module.data_sec, file_path)
-        self.change_global_section(self.module.global_sec, file_path)
-
-    def get_import_func_list(self):
-        import_func_list = []
-        for import_item in self.module.import_sec:
-            if import_item.desc.func_type is not None:
-                import_func_list.append(import_item)
-
-        return import_func_list
-
-    def get_import_func_num(self):
-
-        num = 0
-        for _, import_item in enumerate(self.module.import_sec):
-            if import_item.desc.func_type != None:
-                num += 1
-
-        return num
-
-    def dump_functions(self, func_id=None):
-
-        if func_id is not None:
-            self.print_function(func_id)
-            return
-
-        for code_idx in range(len(self.module.code_sec)):
-            self.print_function(code_idx)
-
-    def print_function(self, func_id):
-
-        type_id = self.module.func_sec[func_id]
-        if len(self.func_name) == 0:
-            print("(func %d (type %d) " % (func_id, type_id), end="")
-        else:
-
-            print("(func %s (type %d) " % (self.func_name[func_id], type_id), end="")
-        param_types_str = ""
-        result_types_str = ""
-        print("=======" + str(type_id))
-        if self.module.type_sec[type_id].param_types:
-            for i in self.module.type_sec[type_id].param_types:
-                param_types_str += (val_type_to_str(i) + " ")
-        if self.module.type_sec[type_id].result_types:
-            for i in self.module.type_sec[type_id].result_types:
-                result_types_str += (val_type_to_str(i) + " ")
-
-        print("(param %s)" % param_types_str, end="")
-        print("(result %s)" % result_types_str)
-
-        if self.module.code_sec[func_id].locals is not None:
-            print("(locals", end=" ")
-            for local in self.module.code_sec[func_id].locals:
-                print((val_type_to_str(local.type) + " ") * local.n, end="")
-            print(")")
-        self.dump_expr("    ", self.module.code_sec[func_id].expr)
-        print(")")
-
-    def add_import(self, import_func_item, import_func_type):
-
-        for i, import_item in enumerate(self.module.import_sec):
-            if import_item.module == import_func_item.module and import_item.name == import_func_item.name:
-                return i
-
-        functype_id = self.add_functype_for_import(import_func_type)
-
-        import_func_item.desc.func_type = functype_id
-
-        self.module.import_sec.append(import_func_item)
-
-        import_func_id = len(self.module.import_sec) - 1
-
-        for _, code in enumerate(self.module.code_sec):
-            self.fix_instruction_from_expr(code.expr, import_func_id, functype_id, False)
-
-        self.fix_elem_section(import_func_id)
-
-        self.fix_export_section_for_import(import_func_id)
-
-        self.change_type_section(self.module.type_sec)
-
-        self.change_import_section(self.module.import_sec)
-
-        return import_func_id
-
-    def add_function(self, functype, local_vec, func_instrs, obfuscated_func_id=None):
-
-        is_new_functype = False
-        functype_id = get_functype_idx(self.module, functype)
-        if functype_id is None:
-            is_new_functype = True
-            functype_id = self.add_functype(functype)
-        if obfuscated_func_id is not None:
-
-            func_id = self.add_func_sec_type(functype_id, is_new_functype, obfuscated_func_id)
-        else:
-
-            func_id = self.add_func_sec_type(functype_id, is_new_functype)
-        return self.insert_function(functype_id, func_id, local_vec, func_instrs, is_new_functype)
-
-    def insert_function(self, type_id, func_id, local_vec, func_instrs, is_new_functype):
-
-        insert_code = Code(local_vec, func_instrs)
-        import_func_num = self.get_import_func_num()
-
-        for _, code in enumerate(self.module.code_sec):
-            self.fix_instruction_from_expr(code.expr, func_id + import_func_num, type_id, is_new_functype)
-
-        self.fix_elem_section(func_id + import_func_num)
-
-        self.module.code_sec.insert(func_id, insert_code)
-
-        self.change_code_section(self.module.code_sec)
-        return (func_id + import_func_num)
-
-    def add_functype(self, functype):
-
-        functype_len = len(self.module.type_sec)
-
-        insert_index = len(self.module.type_sec)
-        self.module.type_sec.append(functype)
-
-        self.change_type_section(self.module.type_sec)
-        return insert_index
-
-    def append_global_variable(self, valtype, value):
-        global_type = GlobalType(mut=1, val_type=valtype)
-        global_variable = Global(global_type=global_type, init=[Instruction(I64Const, value)])
-        self.module.global_sec.append(global_variable)
-
-        import_global_variable_num = 0
-        for import_item in self.module.import_sec:
-            if import_item.desc.global_type is not None:
-                import_global_variable_num += 1
-
-        return import_global_variable_num + len(self.module.global_sec) - 1
-
-    def add_functype_for_import(self, functype):
-
-        for _, bt in enumerate(self.module.type_sec):
-            if functype == bt:
-                return _
-
-        self.module.type_sec.append(functype)
-        return len(self.module.type_sec) - 1
-
-    def add_func_sec_type(self, func_sec_type, is_new_funcType, obfuscated_func_id=None):
-
-        func_count = len(self.module.func_sec)
-
-        func_id = func_count
-
-        if is_new_funcType is True:
-            self.fix_func_section(func_sec_type)
-
-        self.fix_export_section(func_id)
-        if func_id == func_count:
-            self.module.func_sec.append(func_sec_type)
-        else:
-            self.module.func_sec.insert(func_id, func_sec_type)
-
-        self.change_func_section(self.module.func_sec)
-
-        return func_id
-
-    def fix_export_section(self, func_id):
-
-        for export_item in self.module.export_sec:
-            if export_item.desc.tag == 0 and export_item.desc.idx >= (func_id + self.get_import_func_num()):
-                export_item.desc.idx += 1
-
-        self.change_export_section(self.module.export_sec)
-
-    def fix_export_section_for_import(self, func_id):
-
-        for export_item in self.module.export_sec:
-            if export_item.desc.tag == 0 and export_item.desc.idx >= func_id:
-                export_item.desc.idx += 1
-
-        self.change_export_section(self.module.export_sec)
-
-    def add_new_local_to_func(self, func_id, local_type):
-        self.module.code_sec[func_id].locals.append(Locals(1, local_type))
-
-        locals_num = 0
-        for item in self.module.code_sec[func_id].locals:
-            locals_num += item.n
-
-        return len(self.module.type_sec[self.module.func_sec[func_id]].param_types) + locals_num - 1
-
-    def dump_expr(self, indentation, expr):
-
-        for _, instr in enumerate(expr):
-            if instr.opcode in [Block, Loop]:
-                args = instr.args
-                bt = self.module.get_block_type(args.bt)
-                print("%s%s %s" % (indentation, instr.get_opname(), bt))
-                self.dump_expr(indentation + "  ", args.instrs)
-                print("%s%s" % (indentation, "end"))
-            elif instr.opcode == If:
-                args = instr.args
-                bt = self.module.get_block_type(args.bt)
-                print("%s%s %s" % (indentation, "if", bt))
-                self.dump_expr(indentation + "  ", args.instrs1)
-                print("%s%s" % (indentation, "else"))
-                self.dump_expr(indentation + "  ", args.instrs2)
-                print("%s%s" % (indentation, "end"))
-            else:
-                if instr.args is not None:
-                    if 0x36 <= instr.opcode <= 0x3E or 0x28 <= instr.opcode <= 0x35:
-                        print("{}{} align={} offset={} ".format(indentation, instr.get_opname(), instr.args.align,
-                                                                instr.args.offset))
-                    else:
-                        print("{}{} {}".format(indentation, instr.get_opname(), instr.args))
-                elif instr.args is None:
-                    print("{}{}".format(indentation, instr.get_opname()))
-
-    def get_instruction(self, func_id, instr_idx):
-
-        instr, expr = self.get_instruction_from_expr(self.module.code_sec[func_id].expr, instr_idx + 1)
-        return instr
-
-    def insert_instructions(self, func_id, instr_idx, instr):
-
-        if type(instr) is not list:
-            target_instr, expr = self.get_instruction_from_expr(self.module.code_sec[func_id].expr, instr_idx + 1)
-            instr_position = expr.index(target_instr)
-            expr.insert(instr_position, instr)
-        elif type(instr) is list:
-            if instr_idx >= len(self.module.code_sec[func_id].expr):
-                return
-            target_instr, expr = self.get_instruction_from_expr(self.module.code_sec[func_id].expr, instr_idx + 1)
-            instr_position = expr.index(target_instr)
-            for i in instr:
-                expr.insert(instr_position, i)
-                instr_position += 1
-
-    def get_instruction_from_expr(self, expr, instr_idx, current_instr_idx=0):
-
-        for _, instr in enumerate(expr):
-            current_instr_idx += 1
-            if instr.opcode in [Block, Loop]:
-                if instr_idx == current_instr_idx:
-                    raise Exception("block can not be changed")
-                args = instr.args
-                return self.get_instruction_from_expr(args.instrs, instr_idx, current_instr_idx=current_instr_idx)
-
-                current_instr_idx += 1
-                if instr_idx == current_instr_idx:
-                    raise Exception("end can not be changed")
-            elif instr.opcode == If:
-                if instr_idx == current_instr_idx:
-                    raise Exception("if can not be changed")
-                args = instr.args
-                return self.get_instruction_from_expr(args.instrs1, instr_idx, current_instr_idx=current_instr_idx)
-
-                current_instr_idx += 1
-                if instr_idx == current_instr_idx:
-                    raise Exception("else can not be changed")
-                return self.get_instruction_from_expr(args.instrs2, instr_idx, current_instr_idx=current_instr_idx)
-
-                current_instr_idx += 1
-                if instr_idx == current_instr_idx:
-                    raise Exception("end can not be changed")
-            else:
-                if current_instr_idx == instr_idx:
-                    return instr, expr
-
-    def fix_func_section(self, func_sec_type):
-
-        for _, func_type in enumerate(self.module.func_sec):
-            if func_type >= func_sec_type:
-                self.module.func_sec[_] += 1
-
-    def fix_elem_section(self, func_id):
-
-        for elem in self.module.elem_sec:
-            for _, func_idx in enumerate(elem.init):
-                if func_idx >= func_id:
-                    elem.init[_] += 1
-        self.change_elem_section(self.module.elem_sec)
-
-    def fix_instruction_from_expr(self, expr, func_id, type_id, is_new_functype):
-
-        for _, instr in enumerate(expr):
-            if instr.opcode in [Block, Loop]:
-                args = instr.args
-                self.fix_instruction_from_expr(args.instrs, func_id, type_id, is_new_functype)
-            elif instr.opcode == If:
-                args = instr.args
-                self.fix_instruction_from_expr(args.instrs1, func_id, type_id, is_new_functype)
-                self.fix_instruction_from_expr(args.instrs2, func_id, type_id, is_new_functype)
-            else:
-                if instr.args is not None:
-                    if (instr.opcode == Call and instr.args >= func_id):
-                        print(instr.args)
-                        print(func_id)
-                        instr.args += 1
-                    elif instr.opcode == CallIndirect and instr.args >= type_id and is_new_functype is True:
-                        print("type=======")
-                        print(instr.args)
-                        print(func_id)
-                        instr.args += 1
-
-    def hook_call_from_expr(self, expr, func_id, new_func_id=None):
-
-        for _, instr in enumerate(expr):
-            if instr.opcode in [Block, Loop]:
-                args = instr.args
-                return self.hook_call_from_expr(args.instrs, func_id, new_func_id)
-            elif instr.opcode == If:
-                args = instr.args
-                return self.hook_call_from_expr(args.instrs1, func_id, new_func_id)
-                return self.hook_call_from_expr(args.instrs2, func_id, new_func_id)
-            else:
-                if instr.args is not None:
-                    if instr.opcode == Call and instr.args == func_id and new_func_id is not None:
-                        print(instr.args)
-                        print(func_id)
-                        instr.args = new_func_id
-
-    def fix_import_sec(self, type_id):
-
-        for i in self.module.import_sec:
-            if i.desc.func_type >= type_id:
-                i.desc.func_type += 1
-        self.change_import_section(self.module.import_sec)
-
-    def fix_section_range(self, sec_id, change, start, custom_sec_id=None):
-
-        if sec_id != SecCustomID:
-            for i in range(sec_id + 1, 12):
-                if self.module.section_range[i].start != self.module.section_range[i].end:
-                    self.module.section_range[i].start += change
-                    self.module.section_range[i].end += change
-
-            if self.module.section_range[0] != []:
-                for custom in self.module.section_range[0]:
-                    if start <= custom.start:
-                        custom.start += change
-                        custom.end += change
-        elif sec_id == SecCustomID:
-            for i in range(1, 12):
-                if self.module.section_range[i].start != self.module.section_range[i].end and start <= \
-                        self.module.section_range[i].start:
-                    self.module.section_range[i].start += change
-                    self.module.section_range[i].end += change
-            for _, custom in enumerate(self.module.section_range[0]):
-                if _ != custom_sec_id and start <= custom.start:
-                    custom.start += change
-                    custom.end += change
-
-    def change_custom_name_section(self, custom_vec: list, file_path):
-
-        for _, custom in enumerate(custom_vec):
-            if custom.name == "name":
-                name_section_bytes = bytes()
-                name_section_bytes += LEB128U.encode(len(custom.name))
-                name_section_bytes += bytes(custom.name, encoding="utf-8")
-                if custom.name_data.moduleNameSubSec != None:
-                    name_section_bytes += bytes([0x00])
-                    name_section_bytes += LEB128U.encode(len(custom.name_data.moduleNameSubSec))
-                    name_section_bytes += custom.name_data.moduleNameSubSec
-                if custom.name_data.funcNameSubSec != []:
-
-                    funcname_bytes = bytes()
-                    funcname_bytes += LEB128U.encode(len(custom.name_data.funcNameSubSec))
-                    for funcname in custom.name_data.funcNameSubSec:
-                        funcname_bytes += LEB128U.encode(funcname.idx)
-                        funcname_bytes += LEB128U.encode(len(funcname.name))
-                        funcname_bytes += bytes(funcname.name, encoding="utf-8")
-                    name_section_bytes += (bytes([0x01]) + LEB128U.encode(len(funcname_bytes))) + funcname_bytes
-
-                if custom.name_data.localNameSubSec != None:
-                    name_section_bytes += bytes([0x02])
-                    name_section_bytes += LEB128U.encode(len(custom.name_data.localNameSubSec))
-                    name_section_bytes += custom.name_data.localNameSubSec
-                if custom.name_data.labelsNameSubSec != None:
-                    name_section_bytes += bytes([0x03])
-                    name_section_bytes += LEB128U.encode(len(custom.name_data.labelsNameSubSec))
-                    name_section_bytes += custom.name_data.labelsNameSubSec
-                if custom.name_data.typeNameSubSec != None:
-                    name_section_bytes += bytes([0x04])
-                    name_section_bytes += LEB128U.encode(len(custom.name_data.typeNameSubSec))
-                    name_section_bytes += custom.name_data.typeNameSubSec
-                if custom.name_data.tableNameSubSec != []:
-                    tablename_bytes = bytes()
-                    tablename_bytes += LEB128U.encode(len(custom.name_data.tableNameSubSec))
-                    for tablename in custom.name_data.tableNameSubSec:
-                        tablename_bytes += LEB128U.encode(tablename.idx)
-                        tablename_bytes += LEB128U.encode(len(tablename.name))
-                        tablename_bytes += bytes(tablename.name, encoding="utf-8")
-                    name_section_bytes += (bytes([0x05]) + LEB128U.encode(len(tablename_bytes))) + tablename_bytes
-                if custom.name_data.memoryNameSubSec != None:
-                    name_section_bytes += bytes([0x06])
-                    name_section_bytes += LEB128U.encode(len(custom.name_data.memoryNameSubSec))
-                    name_section_bytes += custom.name_data.memoryNameSubSec
-                if custom.name_data.globalNameSubSec != []:
-                    globalname_bytes = bytes()
-                    globalname_bytes += LEB128U.encode(len(custom.name_data.globalNameSubSec))
-                    for globalname in custom.name_data.globalNameSubSec:
-                        globalname_bytes += LEB128U.encode(globalname.idx)
-                        globalname_bytes += LEB128U.encode(len(globalname.name))
-                        globalname_bytes += bytes(globalname.name, encoding="utf-8")
-                    name_section_bytes += (bytes([0x07]) + LEB128U.encode(len(globalname_bytes))) + globalname_bytes
-                if custom.name_data.elemNameSubSec != None:
-                    name_section_bytes += bytes([0x08])
-                    name_section_bytes += LEB128U.encode(len(custom.name_data.elemNameSubSec))
-                    name_section_bytes += custom.name_data.elemNameSubSec
-                if custom.name_data.dataNameSubSec != []:
-                    dataname_bytes = bytes()
-                    dataname_bytes += LEB128U.encode(len(custom.name_data.dataNameSubSec))
-                    for dataname in custom.name_data.dataNameSubSec:
-                        dataname_bytes += LEB128U.encode(dataname.idx)
-                        dataname_bytes += LEB128U.encode(len(dataname.name))
-                        dataname_bytes += bytes(dataname.name, encoding="utf-8")
-                    name_section_bytes += (bytes([0x09]) + LEB128U.encode(len(dataname_bytes))) + dataname_bytes
-
-                with open(os.path.abspath(file_path), "rb+") as f:
-                    file_bytes = f.read()
-                    custom = self.module.section_range[SecCustomID][_]
-                    start = custom.start
-                    end = custom.end
-                    name_section_bytes = bytes([0x00]) + LEB128U.encode(len(name_section_bytes)) + name_section_bytes
-                    file_new_bytes = file_bytes[:start] + name_section_bytes + file_bytes[end:]
-                    change = len(name_section_bytes) - (end - start)
-
-                    custom.end = custom.start + len(name_section_bytes)
-                    self.fix_section_range(SecCustomID, change, custom.start, _)
-                    f.seek(0)
-                    f.truncate()
-                    f.write(file_new_bytes)
-            else:
-                custom_section_bytes = bytes()
-                custom_section_bytes += LEB128U.encode(len(custom.name))
-                custom_section_bytes += bytes(custom.name, encoding="utf-8")
-                custom_section_bytes += custom.custom_sec_data
-
-                with open(os.path.abspath(file_path), "rb+") as f:
-                    file_bytes = f.read()
-                    custom = self.module.section_range[SecCustomID][_]
-                    start = custom.start
-                    end = custom.end
-                    custom_section_bytes = bytes([0x00]) + LEB128U.encode(
-                        len(custom_section_bytes)) + custom_section_bytes
-                    file_new_bytes = file_bytes[:start] + custom_section_bytes + file_bytes[end:]
-                    change = len(custom_section_bytes) - (end - start)
-
-                    custom.end = custom.start + len(custom_section_bytes)
-                    self.fix_section_range(SecCustomID, change, custom.start, _)
-                    f.seek(0)
-                    f.truncate()
-                    f.write(file_new_bytes)
-
-        return None
-
-    def change_import_section(self, import_vec: list, file_path):
-
-        import_vec_len = len(import_vec)
-        import_vec_len_bytes = LEB128U.encode(import_vec_len)
-        import_vec_bytes = bytes()
-        import_vec_bytes += import_vec_len_bytes
-        if import_vec == []:
-            return
-        for i in import_vec:
-            import_vec_bytes += LEB128U.encode(len(i.module))
-            import_vec_bytes += bytes(i.module, encoding="utf-8")
-            import_vec_bytes += LEB128U.encode(len(i.name))
-            import_vec_bytes += bytes(i.name, encoding="utf-8")
-            import_vec_bytes += LEB128U.encode(i.desc.tag)
-            if i.desc.func_type is not None:
-                import_vec_bytes += LEB128U.encode(i.desc.func_type)
-            elif i.desc.table is not None:
-                import_vec_bytes += self.write_table_type(i.desc.table)
-            elif i.desc.mem is not None:
-                import_vec_bytes += self.write_limits(i.desc.mem)
-            elif i.desc.global_type is not None:
-                import_vec_bytes += self.write_global_type(i.desc.global_type)
-        import_section_bytes = bytes([0x02]) + LEB128U.encode(len(import_vec_bytes)) + import_vec_bytes
-
-        with open(os.path.abspath(file_path), "rb+") as f:
-            file_bytes = f.read()
-            file_new_bytes = file_bytes[
-                             :self.module.section_range[SecImportID].start] + import_section_bytes + file_bytes[
-                                                                                                     self.module.section_range[
-                                                                                                         SecImportID].end:]
-            change = len(import_section_bytes) - (
-                    self.module.section_range[SecImportID].end - self.module.section_range[SecImportID].start)
-
-            self.module.section_range[SecImportID].end = self.module.section_range[SecImportID].start + len(
-                import_section_bytes)
-            self.fix_section_range(SecImportID, change, self.module.section_range[SecImportID].start)
-            f.seek(0)
-            f.truncate()
-            f.write(file_new_bytes)
-
-        return import_section_bytes
-
-    def change_export_section(self, export_vec: list, file_path):
-        export_vec_len = len(export_vec)
-        export_vec_len_bytes = LEB128U.encode(export_vec_len)
-        export_vec_bytes = bytes()
-        export_vec_bytes += export_vec_len_bytes
-        if export_vec == []:
-            return
-        for export_item in export_vec:
-            export_vec_bytes += LEB128U.encode(len(export_item.name))
-            export_vec_bytes += bytes(export_item.name, encoding="utf-8")
-            export_vec_bytes += LEB128U.encode(export_item.desc.tag)
-            export_vec_bytes += LEB128U.encode(export_item.desc.idx)
-
-        export_section_bytes = bytes([0x07]) + LEB128U.encode(len(export_vec_bytes)) + export_vec_bytes
-
-        with open(os.path.abspath(file_path), "rb+") as f:
-            file_bytes = f.read()
-            file_new_bytes = file_bytes[
-                             :self.module.section_range[SecExportID].start] + export_section_bytes + file_bytes[
-                                                                                                     self.module.section_range[
-                                                                                                         SecExportID].end:]
-            change = len(export_section_bytes) - (
-                    self.module.section_range[SecExportID].end - self.module.section_range[SecExportID].start)
-
-            self.module.section_range[SecExportID].end = self.module.section_range[SecExportID].start + len(
-                export_section_bytes)
-            self.fix_section_range(SecExportID, change, self.module.section_range[SecExportID].start)
-            f.seek(0)
-            f.truncate()
-            f.write(file_new_bytes)
-
-        return export_section_bytes
-
-    def change_start_section(self, export_vec: list, file_path):
-        export_vec_len = len(export_vec)
-        export_vec_len_bytes = LEB128U.encode(export_vec_len)
-        export_vec_bytes = bytes()
-        export_vec_bytes += export_vec_len_bytes
-        if export_vec == []:
-            return
-        for export_item in export_vec:
-            export_vec_bytes += LEB128U.encode(len(export_item.name))
-            export_vec_bytes += bytes(export_item.name, encoding="utf-8")
-            export_vec_bytes += LEB128U.encode(export_item.desc.tag)
-            export_vec_bytes += LEB128U.encode(export_item.desc.idx)
-
-        export_section_bytes = bytes([0x07]) + LEB128U.encode(len(export_vec_bytes)) + export_vec_bytes
-
-        with open(os.path.abspath(file_path), "rb+") as f:
-            file_bytes = f.read()
-            file_new_bytes = file_bytes[
-                             :self.module.section_range[SecExportID].start] + export_section_bytes + file_bytes[
-                                                                                                     self.module.section_range[
-                                                                                                         SecExportID].end:]
-            change = len(export_section_bytes) - (
-                    self.module.section_range[SecExportID].end - self.module.section_range[SecExportID].start)
-
-            self.module.section_range[SecExportID].end = self.module.section_range[SecExportID].start + len(
-                export_section_bytes)
-            self.fix_section_range(SecExportID, change, self.module.section_range[SecExportID].start)
-            f.seek(0)
-            f.truncate()
-            f.write(file_new_bytes)
-
-        return export_section_bytes
-
-    def change_memory_section(self, memory_vec: list, file_path):
-        memory_vec_len = len(memory_vec)
-        memory_vec_len_bytes = LEB128U.encode(memory_vec_len)
-        memory_vec_bytes = bytes()
-        memory_vec_bytes += memory_vec_len_bytes
-        if memory_vec == []:
-            return
-        for memory_item in memory_vec:
-            memory_item_bytes = bytes()
-            memory_item_bytes += bytes([memory_item.tag])
-            memory_item_bytes += LEB128U.encode(memory_item.min)
-            if memory_item.max != 0:
-                memory_item_bytes += LEB128U.encode(memory_item.max)
-            memory_vec_bytes += memory_item_bytes
-
-        memroy_section_bytes = bytes([SecMemID]) + LEB128U.encode(len(memory_vec_bytes)) + memory_vec_bytes
-
-        with open(os.path.abspath(file_path), "rb+") as f:
-            file_bytes = f.read()
-            file_new_bytes = file_bytes[
-                             :self.module.section_range[SecMemID].start] + memroy_section_bytes + file_bytes[
-                                                                                                  self.module.section_range[
-                                                                                                      SecMemID].end:]
-            change = len(memroy_section_bytes) - (
-                    self.module.section_range[SecMemID].end - self.module.section_range[SecMemID].start)
-
-            self.module.section_range[SecMemID].end = self.module.section_range[SecMemID].start + len(
-                memroy_section_bytes)
-            self.fix_section_range(SecMemID, change, self.module.section_range[SecMemID].start)
-            f.seek(0)
-            f.truncate()
-            f.write(file_new_bytes)
-
-        return memroy_section_bytes
-
-    def change_data_section(self, data_vec: list, file_path):
-        data_vec_len = len(data_vec)
-        data_vec_len_bytes = LEB128U.encode(data_vec_len)
-        data_vec_bytes = bytes()
-        data_vec_bytes += data_vec_len_bytes
-        if not data_vec:
-            return
-        for data_item in data_vec:
-            data_item_bytes = bytes()
-            data_item_bytes += LEB128U.encode(data_item.mem)
-            data_item_bytes += self.write_expr(data_item.offset)
-            data_item_bytes += LEB128U.encode(len(data_item.init))
-            data_item_bytes += data_item.init
-
-            data_vec_bytes += data_item_bytes
-
-        data_section_bytes = bytes([SecDataID]) + LEB128U.encode(len(data_vec_bytes)) + data_vec_bytes
-
-        with open(os.path.abspath(file_path), "rb+") as f:
-            file_bytes = f.read()
-            file_new_bytes = file_bytes[
-                             :self.module.section_range[SecDataID].start] + data_section_bytes + file_bytes[
-                                                                                                 self.module.section_range[
-                                                                                                     SecDataID].end:]
-            change = len(data_section_bytes) - (
-                    self.module.section_range[SecDataID].end - self.module.section_range[SecDataID].start)
-
-            self.module.section_range[SecDataID].end = self.module.section_range[SecDataID].start + len(
-                data_section_bytes)
-            self.fix_section_range(SecDataID, change, self.module.section_range[SecDataID].start)
-            f.seek(0)
-            f.truncate()
-            f.write(file_new_bytes)
-
-        return data_section_bytes
-
-    def change_elem_section(self, elem_vec: list, file_path):
-
-        elem_vec_len = len(elem_vec)
-        elem_vec_len_bytes = LEB128U.encode(elem_vec_len)
-        elem_vec_bytes = bytes()
-        elem_vec_bytes += elem_vec_len_bytes
-        if elem_vec == []:
-            return
-        for elem in elem_vec:
-            elem_vec_bytes += LEB128U.encode(elem.table)
-            elem_vec_bytes += self.write_expr(elem.offset)
-            elem_vec_bytes += LEB128U.encode(len(elem.init))
-            for func_idx in elem.init:
-                elem_vec_bytes += LEB128U.encode(func_idx)
-        elem_section_bytes = bytes([SecElemID]) + LEB128U.encode(len(elem_vec_bytes)) + elem_vec_bytes
-
-        with open(os.path.abspath(file_path), "rb+") as f:
-            file_bytes = f.read()
-            binary_start = self.module.section_range[SecElemID].start
-            binary_end = self.module.section_range[SecElemID].end
-            if binary_start == binary_end:
-                for i in reversed(range(SecElemID)):
-                    if self.module.section_range[i].start != self.module.section_range[i].end:
-                        file_new_bytes = file_bytes[
-                                         :self.module.section_range[i].end] + elem_section_bytes + file_bytes[
-                                                                                                   self.module.section_range[
-                                                                                                       i].end:]
-                        change = len(elem_section_bytes) - (
-                                self.module.section_range[SecElemID].end - self.module.section_range[SecElemID].start)
-                        self.module.section_range[SecElemID].start = self.module.section_range[i].end
-                        self.module.section_range[SecElemID].end = self.module.section_range[i].end + len(
-                            elem_section_bytes)
-                        self.fix_section_range(SecElemID, change, self.module.section_range[SecElemID].start)
-                        f.seek(0)
-                        f.truncate()
-                        f.write(file_new_bytes)
-                        break
-            else:
-                file_new_bytes = file_bytes[
-                                 :self.module.section_range[SecElemID].start] + elem_section_bytes + file_bytes[
-                                                                                                     self.module.section_range[
-                                                                                                         SecElemID].end:]
-                change = len(elem_section_bytes) - (
-                        self.module.section_range[SecElemID].end - self.module.section_range[SecElemID].start)
-
-                self.module.section_range[SecElemID].end = self.module.section_range[SecElemID].start + len(
-                    elem_section_bytes)
-                self.fix_section_range(SecElemID, change, self.module.section_range[SecElemID].start)
-                f.seek(0)
-                f.truncate()
-                f.write(file_new_bytes)
-
-        return elem_section_bytes
-
-    def change_type_section(self, functype_vec: list, file_path):
-
-        functype_vec_len = len(functype_vec)
-        functype_vec_len_bytes = LEB128U.encode(functype_vec_len)
-        functype_vec_bytes = bytes()
-        functype_vec_bytes += functype_vec_len_bytes
-        if functype_vec == []:
-            return
-        for functype in functype_vec:
-            functype_bytes = bytes()
-            functype_bytes += bytes([0x60])
-            functype_bytes += self.write_val_types(functype.param_types)
-            functype_bytes += self.write_val_types(functype.result_types)
-            functype_vec_bytes += functype_bytes
-        type_section_bytes = bytes([0x01]) + LEB128U.encode(len(functype_vec_bytes)) + functype_vec_bytes
-
-        with open(os.path.abspath(file_path), "rb+") as f:
-            file_bytes = f.read()
-            file_new_bytes = file_bytes[:self.module.section_range[SecTypeID].start] + type_section_bytes + file_bytes[
-                                                                                                            self.module.section_range[
-                                                                                                                SecTypeID].end:]
-            change = len(type_section_bytes) - (
-                    self.module.section_range[SecTypeID].end - self.module.section_range[SecTypeID].start)
-
-            self.module.section_range[SecTypeID].end = self.module.section_range[SecTypeID].start + len(
-                type_section_bytes)
-            self.fix_section_range(SecTypeID, change, self.module.section_range[SecTypeID].start)
-            f.seek(0)
-            f.truncate()
-            f.write(file_new_bytes)
-
-        return type_section_bytes
-
-    def change_global_section(self, global_vec: list, file_path):
-
-        global_vec_len = len(global_vec)
-        global_vec_len_bytes = LEB128U.encode(global_vec_len)
-        global_vec_bytes = bytes()
-        global_vec_bytes += global_vec_len_bytes
-        if global_vec == []:
-            return
-        for global_item in global_vec:
-            global_bytes = bytes()
-            global_bytes += self.write_global(global_item)
-            global_vec_bytes += global_bytes
-
-        global_section_bytes = bytes([0x06]) + LEB128U.encode(len(global_vec_bytes)) + global_vec_bytes
-
-        with open(os.path.abspath(file_path), "rb+") as f:
-            file_bytes = f.read()
-            if self.module.section_range[SecGlobalID].start == 0:
-                for section in range(1, SecGlobalID):
-                    if self.module.section_range[section].start != 0:
-                        self.module.section_range[SecGlobalID].start = self.module.section_range[section].end
-                        self.module.section_range[SecGlobalID].end = self.module.section_range[SecGlobalID].start
-            file_new_bytes = file_bytes[
-                             :self.module.section_range[SecGlobalID].start] + global_section_bytes + file_bytes[
-                                                                                                     self.module.section_range[
-                                                                                                         SecGlobalID].end:]
-            change = len(global_section_bytes) - (
-                    self.module.section_range[SecGlobalID].end - self.module.section_range[SecGlobalID].start)
-
-            self.module.section_range[SecGlobalID].end = self.module.section_range[SecGlobalID].start + len(
-                global_section_bytes)
-            self.fix_section_range(SecGlobalID, change, self.module.section_range[SecGlobalID].start)
-            f.seek(0)
-            f.truncate()
-            f.write(file_new_bytes)
-
-        return global_section_bytes
-
-    def change_func_section(self, type_vec, file_path):
-
-        type_vec_len = len(type_vec)
-        type_vec_len_bytes = LEB128U.encode(type_vec_len)
-        type_vec_bytes = bytes()
-        type_vec_bytes += type_vec_len_bytes
-        if type_vec == []:
-            return
-        for type_item in type_vec:
-            type_vec_bytes += LEB128U.encode(type_item)
-
-        func_section_bytes = bytes([0x03]) + LEB128U.encode(len(type_vec_bytes)) + type_vec_bytes
-        with open(os.path.abspath(file_path), "rb+") as f:
-            file_bytes = f.read()
-            file_new_bytes = file_bytes[:self.module.section_range[SecFuncID].start] + func_section_bytes + file_bytes[
-                                                                                                            self.module.section_range[
-                                                                                                                SecFuncID].end:]
-            change = len(func_section_bytes) - (
-                    self.module.section_range[SecFuncID].end - self.module.section_range[SecFuncID].start)
-
-            self.module.section_range[SecFuncID].end = self.module.section_range[SecFuncID].start + len(
-                func_section_bytes)
-            self.fix_section_range(SecFuncID, change, self.module.section_range[SecFuncID].start)
-            f.seek(0)
-            f.truncate()
-            f.write(file_new_bytes)
-
-    def change_code_section(self, code_vec: list, file_path):
-
-        code_vec_len = len(code_vec)
-        code_vec_len_bytes = LEB128U.encode(code_vec_len)
-        code_vec_bytes = bytes()
-        code_vec_bytes += code_vec_len_bytes
-        if code_vec == []:
-            return
-        for code in code_vec:
-            code_bytes = bytes()
-            locals_vec_len = len(code.locals)
-            locals_vec_len_bytes = LEB128U.encode(locals_vec_len)
-            locals_vec_bytes = bytes()
-            expr_bytes = bytes()
-
-            for local in code.locals:
-                local_count = local.n
-                local_type = local.type
-                locals_vec_bytes += LEB128U.encode(local_count)
-                locals_vec_bytes += bytes([local_type])
-
-            expr_bytes += self.write_expr(code.expr)
-            code_bytes += (locals_vec_len_bytes + locals_vec_bytes + expr_bytes)
-            code_vec_bytes += LEB128U.encode(len(code_bytes)) + code_bytes
-        code_section_bytes = bytes([0x0A]) + LEB128U.encode(len(code_vec_bytes)) + code_vec_bytes
-
-        with open(os.path.abspath(file_path), "rb+") as f:
-            file_bytes = f.read()
-            file_new_bytes = file_bytes[:self.module.section_range[SecCodeID].start] + code_section_bytes + file_bytes[
-                                                                                                            self.module.section_range[
-                                                                                                                SecCodeID].end:]
-            change = len(code_section_bytes) - (
-                    self.module.section_range[SecCodeID].end - self.module.section_range[SecCodeID].start)
-
-            self.module.section_range[SecCodeID].end = self.module.section_range[SecCodeID].start + len(
-                code_section_bytes)
-            self.fix_section_range(SecCodeID, change, self.module.section_range[SecCodeID].start)
-            f.seek(0)
-            f.truncate()
-            f.write(file_new_bytes)
-
-        return code_section_bytes
-
-    def change_table_section(self, table_vec: list, file_path):
-
-        table_vec_len = len(table_vec)
-        table_vec_len_bytes = LEB128U.encode(table_vec_len)
-        table_vec_bytes = bytes()
-        table_vec_bytes += table_vec_len_bytes
-        if table_vec == []:
-            return
-        for table_type in table_vec:
-            table_type_bytes = bytes()
-            table_type_bytes += bytes([table_type.elem_type])
-            table_type_bytes += bytes([table_type.limits.tag])
-            table_type_bytes += LEB128U.encode(table_type.limits.min)
-            if 0 != table_type.limits.max:
-                table_type_bytes += LEB128U.encode(table_type.limits.max)
-            table_vec_bytes += table_type_bytes
-
-        table_section_bytes = bytes([0x04]) + LEB128U.encode(len(table_vec_bytes)) + table_vec_bytes
-
-        with open(os.path.abspath(file_path), "rb+") as f:
-            file_bytes = f.read()
-            binary_start = self.module.section_range[SecTableID].start
-            binary_end = self.module.section_range[SecTableID].end
-            if binary_start == binary_end:
-                for i in reversed(range(SecTableID)):
-                    if self.module.section_range[i].start != self.module.section_range[i].end:
-                        file_new_bytes = file_bytes[
-                                         :self.module.section_range[i].end] + table_section_bytes + file_bytes[
-                                                                                                    self.module.section_range[
-                                                                                                        i].end:]
-                        change = len(table_section_bytes) - (
-                                self.module.section_range[SecTableID].end - self.module.section_range[
-                            SecTableID].start)
-                        self.module.section_range[SecTableID].start = self.module.section_range[i].end
-                        self.module.section_range[SecTableID].end = self.module.section_range[i].end + len(
-                            table_section_bytes)
-                        self.fix_section_range(SecTableID, change, self.module.section_range[SecTableID].start)
-                        f.seek(0)
-                        f.truncate()
-                        f.write(file_new_bytes)
-                        break
-            else:
-                file_new_bytes = file_bytes[
-                                 :self.module.section_range[SecTableID].start] + table_section_bytes + file_bytes[
-                                                                                                       self.module.section_range[
-                                                                                                           SecTableID].end:]
-                change = len(table_section_bytes) - (
-                        self.module.section_range[SecTableID].end - self.module.section_range[SecTableID].start)
-
-                self.module.section_range[SecTableID].end = self.module.section_range[SecTableID].start + len(
-                    table_section_bytes)
-                self.fix_section_range(SecTableID, change, self.module.section_range[SecTableID].start)
-                f.seek(0)
-                f.truncate()
-                f.write(file_new_bytes)
-
-        return table_section_bytes
-
-    def write_expr(self, expr: list):
-
-        instructions_bytes = self.write_instructions(expr)
-        expr_bytes = instructions_bytes + bytes([0x0b])
-
-        return expr_bytes
-
-    def write_instructions(self, expr: list):
-
-        instructions_bytes = bytes()
-        for index in range(len(expr)):
-            instructions_bytes += self.write_instruction(expr[index])
-
-        return instructions_bytes
-
-    def write_instruction(self, instr):
-
-        instruction_bytes = bytes()
-        instruction_bytes += bytes([instr.opcode])
-        args_bytes = self.write_args(instr)
-        if args_bytes is not None:
-            instruction_bytes += args_bytes
-
-        return instruction_bytes
-
-    def write_args(self, instr):
-
-        opcode = instr.opcode
-        if opcode in [Block, Loop]:
-            return self.write_block_args(instr)
-        elif opcode == If:
-            return self.write_if_args(instr)
-        elif opcode in [Br, BrIf]:
-            return LEB128U.encode(instr.args)
-        elif opcode == BrTable:
-            return self.write_br_table_args(instr)
-        elif opcode == Call:
-            return LEB128U.encode(instr.args)
-        elif opcode == CallIndirect:
-            return self.write_call_indirect_args(instr)
-        elif opcode in [LocalGet, LocalSet, LocalTee]:
-            return LEB128U.encode(instr.args)
-        elif opcode in [GlobalGet, GlobalSet]:
-            return LEB128U.encode(instr.args)
-        elif opcode in [MemorySize, MemoryGrow]:
-            return bytes([0x00])
-        elif opcode == I32Const:
-            return LEB128S.encode(instr.args)
-        elif opcode == I64Const:
-            return LEB128S.encode(instr.args)
-        elif opcode == F32Const:
-            return struct.pack('<f', instr.args)
-        elif opcode == F64Const:
-            return struct.pack('<d', instr.args)
-        elif opcode == TruncSat:
-            return bytes([instr.args])
-        else:
-            if I32Load <= instr.opcode <= I64Store32:
-                return self.write_mem_arg(instr)
-            return None
-
-    def write_block_args(self, instr):
-
-        args_bytes = bytes()
-        args_bytes += LEB128S.encode(instr.args.bt)
-        args_bytes += self.write_instructions(instr.args.instrs)
-        args_bytes += bytes([0x0b])
-
-        return args_bytes
-
-    def write_if_args(self, instr):
-
-        args_bytes = bytes()
-        args_bytes += LEB128S.encode(instr.args.bt)
-        args_bytes += self.write_instructions(instr.args.instrs1)
-        if instr.args.instrs2:
-            args_bytes += bytes([0x05])
-            args_bytes += self.write_instructions(instr.args.instrs2)
-            args_bytes += bytes([0x0b])
-        else:
-            args_bytes += bytes([0x0b])
-
-        return args_bytes
-
-    @staticmethod
-    def write_br_table_args(instr):
-
-        args_bytes = bytes()
-        args_bytes += LEB128U.encode(len(instr.args.labels))
-        for label in instr.args.labels:
-            args_bytes += LEB128U.encode(label)
-        args_bytes += LEB128U.encode(instr.args.default)
-
-        return args_bytes
-
-    @staticmethod
-    def write_call_indirect_args(instr):
-
-        args_bytes = bytes()
-        args_bytes += LEB128U.encode(instr.args)
-        args_bytes += bytes([0x00])
-
-        return args_bytes
-
-    @staticmethod
-    def write_mem_arg(instr):
-
-        args_bytes = bytes()
-        args_bytes += LEB128U.encode(instr.args.align)
-        args_bytes += LEB128U.encode(instr.args.offset)
-
-        return args_bytes
-
-    @staticmethod
-    def write_val_types(val_types):
-
-        val_types_bytes = bytes()
-        val_types_bytes += LEB128U.encode(len(val_types))
-        for val in val_types:
-            val_types_bytes += bytes([val])
-
-        return val_types_bytes
-
-    @staticmethod
-    def write_global_type(global_type):
-
-        global_type_bytes = bytes()
-        global_type_bytes += bytes([global_type.val_type])
-        global_type_bytes += bytes([global_type.mut])
-        return global_type_bytes
-
-    @staticmethod
-    def write_limits(mem):
-
-        mem_bytes = bytes()
-        mem_bytes += bytes([mem.tag])
-        mem_bytes += LEB128U.encode(mem.min)
-        if mem.tag == 1:
-            mem_bytes += LEB128U.encode(mem.max)
-        return mem_bytes
-
-    @staticmethod
-    def write_table_type(table_type):
-
-        table_type_bytes = bytes()
-        table_type_bytes += bytes([table_type.elem_type])
-        table_type_bytes += bytes([table_type.limits.tag])
-        if table_type.limits.min != 0:
-            table_type_bytes += LEB128U.encode(table_type.limits.min)
-        if table_type.limits.max != 0:
-            table_type_bytes += LEB128U.encode(table_type.limits.max)
-        return table_type_bytes
-
-    def write_global(self, global_item):
-        global_bytes = bytes()
-        global_bytes += self.write_global_type(global_item.type)
-        global_bytes += self.write_expr(global_item.init)
-        return global_bytes
-
-
-def get_functype_idx(module, functype):
-    functype_id = None
-    for _, i in enumerate(module.type_sec):
-        if i.equal(functype) is True:
-            functype_id = _
-    return functype_id
+import os
+import struct
+
+from leb128 import LEB128U, LEB128S
+from shutil import copyfile
+from BREWasm.parser import reader
+from BREWasm.parser.instruction import Instruction
+from BREWasm.parser.module import *
+from BREWasm.parser.opcodes import *
+from BREWasm.parser.types import val_type_to_str, GlobalType
+
+
+class ModifyBinary:
+
+    def __init__(self,  path, module=None):
+        if module is None:
+            module, err = reader.decode_file(path)
+            if err is not None:
+                print(err.args)
+                print("=================================")
+                raise Exception("Failed to read the wasm file!")
+
+            self.module = module
+            self.module.path = path
+
+            self.func_name = []
+            for custom in self.module.custom_secs:
+                if custom.name == "name":
+                    if custom.name_data.funcNameSubSec is not None:
+
+                        for func_name_item in custom.name_data.funcNameSubSec[self.get_import_func_num():]:
+                            self.func_name.append(func_name_item.name)
+        else:
+            self.module = module
+            self.module.path = path
+
+    def emit_binary(self, path):
+        file_path = self.module.path
+        
+        if not os.path.exists(path):
+            copyfile(self.module.path, path)
+            file_path = path
+        elif not os.path.samefile(self.module.path, path):
+            if os.path.isfile(path):
+                os.remove(path)
+            copyfile(self.module.path, path)
+            file_path = path
+
+        self.change_custom_name_section(self.module.custom_secs, file_path)
+        self.change_type_section(self.module.type_sec, file_path)
+        self.change_import_section(self.module.import_sec, file_path)
+        self.change_export_section(self.module.export_sec, file_path)
+        self.change_func_section(self.module.func_sec, file_path)
+        self.change_code_section(self.module.code_sec, file_path)
+        self.change_table_section(self.module.table_sec, file_path)
+        self.change_elem_section(self.module.elem_sec, file_path)
+        self.change_memory_section(self.module.mem_sec, file_path)
+        self.change_data_section(self.module.data_sec, file_path)
+        self.change_global_section(self.module.global_sec, file_path)
+
+    def get_import_func_list(self):
+        import_func_list = []
+        for import_item in self.module.import_sec:
+            if import_item.desc.func_type is not None:
+                import_func_list.append(import_item)
+
+        return import_func_list
+
+    def get_import_func_num(self):
+
+        num = 0
+        for _, import_item in enumerate(self.module.import_sec):
+            if import_item.desc.func_type != None:
+                num += 1
+
+        return num
+
+    def dump_functions(self, func_id=None):
+
+        if func_id is not None:
+            self.print_function(func_id)
+            return
+
+        for code_idx in range(len(self.module.code_sec)):
+            self.print_function(code_idx)
+
+    def print_function(self, func_id):
+
+        type_id = self.module.func_sec[func_id]
+        if len(self.func_name) == 0:
+            print("(func %d (type %d) " % (func_id, type_id), end="")
+        else:
+
+            print("(func %s (type %d) " % (self.func_name[func_id], type_id), end="")
+        param_types_str = ""
+        result_types_str = ""
+        print("=======" + str(type_id))
+        if self.module.type_sec[type_id].param_types:
+            for i in self.module.type_sec[type_id].param_types:
+                param_types_str += (val_type_to_str(i) + " ")
+        if self.module.type_sec[type_id].result_types:
+            for i in self.module.type_sec[type_id].result_types:
+                result_types_str += (val_type_to_str(i) + " ")
+
+        print("(param %s)" % param_types_str, end="")
+        print("(result %s)" % result_types_str)
+
+        if self.module.code_sec[func_id].locals is not None:
+            print("(locals", end=" ")
+            for local in self.module.code_sec[func_id].locals:
+                print((val_type_to_str(local.type) + " ") * local.n, end="")
+            print(")")
+        self.dump_expr("    ", self.module.code_sec[func_id].expr)
+        print(")")
+
+    def add_import(self, import_func_item, import_func_type):
+
+        for i, import_item in enumerate(self.module.import_sec):
+            if import_item.module == import_func_item.module and import_item.name == import_func_item.name:
+                return i
+
+        functype_id = self.add_functype_for_import(import_func_type)
+
+        import_func_item.desc.func_type = functype_id
+
+        self.module.import_sec.append(import_func_item)
+
+        import_func_id = len(self.module.import_sec) - 1
+
+        for _, code in enumerate(self.module.code_sec):
+            self.fix_instruction_from_expr(code.expr, import_func_id, functype_id, False)
+
+        self.fix_elem_section(import_func_id)
+
+        self.fix_export_section_for_import(import_func_id)
+
+        self.change_type_section(self.module.type_sec)
+
+        self.change_import_section(self.module.import_sec)
+
+        return import_func_id
+
+    def add_function(self, functype, local_vec, func_instrs, obfuscated_func_id=None):
+
+        is_new_functype = False
+        functype_id = get_functype_idx(self.module, functype)
+        if functype_id is None:
+            is_new_functype = True
+            functype_id = self.add_functype(functype)
+        if obfuscated_func_id is not None:
+
+            func_id = self.add_func_sec_type(functype_id, is_new_functype, obfuscated_func_id)
+        else:
+
+            func_id = self.add_func_sec_type(functype_id, is_new_functype)
+        return self.insert_function(functype_id, func_id, local_vec, func_instrs, is_new_functype)
+
+    def insert_function(self, type_id, func_id, local_vec, func_instrs, is_new_functype):
+
+        insert_code = Code(local_vec, func_instrs)
+        import_func_num = self.get_import_func_num()
+
+        for _, code in enumerate(self.module.code_sec):
+            self.fix_instruction_from_expr(code.expr, func_id + import_func_num, type_id, is_new_functype)
+
+        self.fix_elem_section(func_id + import_func_num)
+
+        self.module.code_sec.insert(func_id, insert_code)
+
+        self.change_code_section(self.module.code_sec)
+        return (func_id + import_func_num)
+
+    def add_functype(self, functype):
+
+        functype_len = len(self.module.type_sec)
+
+        insert_index = len(self.module.type_sec)
+        self.module.type_sec.append(functype)
+
+        self.change_type_section(self.module.type_sec)
+        return insert_index
+
+    def append_global_variable(self, valtype, value):
+        global_type = GlobalType(mut=1, val_type=valtype)
+        global_variable = Global(global_type=global_type, init=[Instruction(I64Const, value)])
+        self.module.global_sec.append(global_variable)
+
+        import_global_variable_num = 0
+        for import_item in self.module.import_sec:
+            if import_item.desc.global_type is not None:
+                import_global_variable_num += 1
+
+        return import_global_variable_num + len(self.module.global_sec) - 1
+
+    def add_functype_for_import(self, functype):
+
+        for _, bt in enumerate(self.module.type_sec):
+            if functype == bt:
+                return _
+
+        self.module.type_sec.append(functype)
+        return len(self.module.type_sec) - 1
+
+    def add_func_sec_type(self, func_sec_type, is_new_funcType, obfuscated_func_id=None):
+
+        func_count = len(self.module.func_sec)
+
+        func_id = func_count
+
+        if is_new_funcType is True:
+            self.fix_func_section(func_sec_type)
+
+        self.fix_export_section(func_id)
+        if func_id == func_count:
+            self.module.func_sec.append(func_sec_type)
+        else:
+            self.module.func_sec.insert(func_id, func_sec_type)
+
+        self.change_func_section(self.module.func_sec)
+
+        return func_id
+
+    def fix_export_section(self, func_id):
+
+        for export_item in self.module.export_sec:
+            if export_item.desc.tag == 0 and export_item.desc.idx >= (func_id + self.get_import_func_num()):
+                export_item.desc.idx += 1
+
+        self.change_export_section(self.module.export_sec)
+
+    def fix_export_section_for_import(self, func_id):
+
+        for export_item in self.module.export_sec:
+            if export_item.desc.tag == 0 and export_item.desc.idx >= func_id:
+                export_item.desc.idx += 1
+
+        self.change_export_section(self.module.export_sec)
+
+    def add_new_local_to_func(self, func_id, local_type):
+        self.module.code_sec[func_id].locals.append(Locals(1, local_type))
+
+        locals_num = 0
+        for item in self.module.code_sec[func_id].locals:
+            locals_num += item.n
+
+        return len(self.module.type_sec[self.module.func_sec[func_id]].param_types) + locals_num - 1
+
+    def dump_expr(self, indentation, expr):
+
+        for _, instr in enumerate(expr):
+            if instr.opcode in [Block, Loop]:
+                args = instr.args
+                bt = self.module.get_block_type(args.bt)
+                print("%s%s %s" % (indentation, instr.get_opname(), bt))
+                self.dump_expr(indentation + "  ", args.instrs)
+                print("%s%s" % (indentation, "end"))
+            elif instr.opcode == If:
+                args = instr.args
+                bt = self.module.get_block_type(args.bt)
+                print("%s%s %s" % (indentation, "if", bt))
+                self.dump_expr(indentation + "  ", args.instrs1)
+                print("%s%s" % (indentation, "else"))
+                self.dump_expr(indentation + "  ", args.instrs2)
+                print("%s%s" % (indentation, "end"))
+            else:
+                if instr.args is not None:
+                    if 0x36 <= instr.opcode <= 0x3E or 0x28 <= instr.opcode <= 0x35:
+                        print("{}{} align={} offset={} ".format(indentation, instr.get_opname(), instr.args.align,
+                                                                instr.args.offset))
+                    else:
+                        print("{}{} {}".format(indentation, instr.get_opname(), instr.args))
+                elif instr.args is None:
+                    print("{}{}".format(indentation, instr.get_opname()))
+
+    def get_instruction(self, func_id, instr_idx):
+
+        instr, expr = self.get_instruction_from_expr(self.module.code_sec[func_id].expr, instr_idx + 1)
+        return instr
+
+    def insert_instructions(self, func_id, instr_idx, instr):
+
+        if type(instr) is not list:
+            target_instr, expr = self.get_instruction_from_expr(self.module.code_sec[func_id].expr, instr_idx + 1)
+            instr_position = expr.index(target_instr)
+            expr.insert(instr_position, instr)
+        elif type(instr) is list:
+            if instr_idx >= len(self.module.code_sec[func_id].expr):
+                return
+            target_instr, expr = self.get_instruction_from_expr(self.module.code_sec[func_id].expr, instr_idx + 1)
+            instr_position = expr.index(target_instr)
+            for i in instr:
+                expr.insert(instr_position, i)
+                instr_position += 1
+
+    def get_instruction_from_expr(self, expr, instr_idx, current_instr_idx=0):
+
+        for _, instr in enumerate(expr):
+            current_instr_idx += 1
+            if instr.opcode in [Block, Loop]:
+                if instr_idx == current_instr_idx:
+                    raise Exception("block can not be changed")
+                args = instr.args
+                return self.get_instruction_from_expr(args.instrs, instr_idx, current_instr_idx=current_instr_idx)
+
+                current_instr_idx += 1
+                if instr_idx == current_instr_idx:
+                    raise Exception("end can not be changed")
+            elif instr.opcode == If:
+                if instr_idx == current_instr_idx:
+                    raise Exception("if can not be changed")
+                args = instr.args
+                return self.get_instruction_from_expr(args.instrs1, instr_idx, current_instr_idx=current_instr_idx)
+
+                current_instr_idx += 1
+                if instr_idx == current_instr_idx:
+                    raise Exception("else can not be changed")
+                return self.get_instruction_from_expr(args.instrs2, instr_idx, current_instr_idx=current_instr_idx)
+
+                current_instr_idx += 1
+                if instr_idx == current_instr_idx:
+                    raise Exception("end can not be changed")
+            else:
+                if current_instr_idx == instr_idx:
+                    return instr, expr
+
+    def fix_func_section(self, func_sec_type):
+
+        for _, func_type in enumerate(self.module.func_sec):
+            if func_type >= func_sec_type:
+                self.module.func_sec[_] += 1
+
+    def fix_elem_section(self, func_id):
+
+        for elem in self.module.elem_sec:
+            for _, func_idx in enumerate(elem.init):
+                if func_idx >= func_id:
+                    elem.init[_] += 1
+        self.change_elem_section(self.module.elem_sec)
+
+    def fix_instruction_from_expr(self, expr, func_id, type_id, is_new_functype):
+
+        for _, instr in enumerate(expr):
+            if instr.opcode in [Block, Loop]:
+                args = instr.args
+                self.fix_instruction_from_expr(args.instrs, func_id, type_id, is_new_functype)
+            elif instr.opcode == If:
+                args = instr.args
+                self.fix_instruction_from_expr(args.instrs1, func_id, type_id, is_new_functype)
+                self.fix_instruction_from_expr(args.instrs2, func_id, type_id, is_new_functype)
+            else:
+                if instr.args is not None:
+                    if (instr.opcode == Call and instr.args >= func_id):
+                        print(instr.args)
+                        print(func_id)
+                        instr.args += 1
+                    elif instr.opcode == CallIndirect and instr.args >= type_id and is_new_functype is True:
+                        print("type=======")
+                        print(instr.args)
+                        print(func_id)
+                        instr.args += 1
+
+    def hook_call_from_expr(self, expr, func_id, new_func_id=None):
+
+        for _, instr in enumerate(expr):
+            if instr.opcode in [Block, Loop]:
+                args = instr.args
+                return self.hook_call_from_expr(args.instrs, func_id, new_func_id)
+            elif instr.opcode == If:
+                args = instr.args
+                return self.hook_call_from_expr(args.instrs1, func_id, new_func_id)
+                return self.hook_call_from_expr(args.instrs2, func_id, new_func_id)
+            else:
+                if instr.args is not None:
+                    if instr.opcode == Call and instr.args == func_id and new_func_id is not None:
+                        print(instr.args)
+                        print(func_id)
+                        instr.args = new_func_id
+
+    def fix_import_sec(self, type_id):
+
+        for i in self.module.import_sec:
+            if i.desc.func_type >= type_id:
+                i.desc.func_type += 1
+        self.change_import_section(self.module.import_sec)
+
+    def fix_section_range(self, sec_id, change, start, custom_sec_id=None):
+
+        if sec_id != SecCustomID:
+            for i in range(sec_id + 1, 12):
+                if self.module.section_range[i].start != self.module.section_range[i].end:
+                    self.module.section_range[i].start += change
+                    self.module.section_range[i].end += change
+
+            if self.module.section_range[0] != []:
+                for custom in self.module.section_range[0]:
+                    if start <= custom.start:
+                        custom.start += change
+                        custom.end += change
+        elif sec_id == SecCustomID:
+            for i in range(1, 12):
+                if self.module.section_range[i].start != self.module.section_range[i].end and start <= \
+                        self.module.section_range[i].start:
+                    self.module.section_range[i].start += change
+                    self.module.section_range[i].end += change
+            for _, custom in enumerate(self.module.section_range[0]):
+                if _ != custom_sec_id and start <= custom.start:
+                    custom.start += change
+                    custom.end += change
+
+    def change_custom_name_section(self, custom_vec: list, file_path):
+
+        for _, custom in enumerate(custom_vec):
+            if custom.name == "name":
+                name_section_bytes = bytes()
+                name_section_bytes += LEB128U.encode(len(custom.name))
+                name_section_bytes += bytes(custom.name, encoding="utf-8")
+                if custom.name_data.moduleNameSubSec != None:
+                    name_section_bytes += bytes([0x00])
+                    name_section_bytes += LEB128U.encode(len(custom.name_data.moduleNameSubSec))
+                    name_section_bytes += custom.name_data.moduleNameSubSec
+                if custom.name_data.funcNameSubSec != []:
+
+                    funcname_bytes = bytes()
+                    funcname_bytes += LEB128U.encode(len(custom.name_data.funcNameSubSec))
+                    for funcname in custom.name_data.funcNameSubSec:
+                        funcname_bytes += LEB128U.encode(funcname.idx)
+                        funcname_bytes += LEB128U.encode(len(funcname.name))
+                        funcname_bytes += bytes(funcname.name, encoding="utf-8")
+                    name_section_bytes += (bytes([0x01]) + LEB128U.encode(len(funcname_bytes))) + funcname_bytes
+
+                if custom.name_data.localNameSubSec != None:
+                    name_section_bytes += bytes([0x02])
+                    name_section_bytes += LEB128U.encode(len(custom.name_data.localNameSubSec))
+                    name_section_bytes += custom.name_data.localNameSubSec
+                if custom.name_data.labelsNameSubSec != None:
+                    name_section_bytes += bytes([0x03])
+                    name_section_bytes += LEB128U.encode(len(custom.name_data.labelsNameSubSec))
+                    name_section_bytes += custom.name_data.labelsNameSubSec
+                if custom.name_data.typeNameSubSec != None:
+                    name_section_bytes += bytes([0x04])
+                    name_section_bytes += LEB128U.encode(len(custom.name_data.typeNameSubSec))
+                    name_section_bytes += custom.name_data.typeNameSubSec
+                if custom.name_data.tableNameSubSec != []:
+                    tablename_bytes = bytes()
+                    tablename_bytes += LEB128U.encode(len(custom.name_data.tableNameSubSec))
+                    for tablename in custom.name_data.tableNameSubSec:
+                        tablename_bytes += LEB128U.encode(tablename.idx)
+                        tablename_bytes += LEB128U.encode(len(tablename.name))
+                        tablename_bytes += bytes(tablename.name, encoding="utf-8")
+                    name_section_bytes += (bytes([0x05]) + LEB128U.encode(len(tablename_bytes))) + tablename_bytes
+                if custom.name_data.memoryNameSubSec != None:
+                    name_section_bytes += bytes([0x06])
+                    name_section_bytes += LEB128U.encode(len(custom.name_data.memoryNameSubSec))
+                    name_section_bytes += custom.name_data.memoryNameSubSec
+                if custom.name_data.globalNameSubSec != []:
+                    globalname_bytes = bytes()
+                    globalname_bytes += LEB128U.encode(len(custom.name_data.globalNameSubSec))
+                    for globalname in custom.name_data.globalNameSubSec:
+                        globalname_bytes += LEB128U.encode(globalname.idx)
+                        globalname_bytes += LEB128U.encode(len(globalname.name))
+                        globalname_bytes += bytes(globalname.name, encoding="utf-8")
+                    name_section_bytes += (bytes([0x07]) + LEB128U.encode(len(globalname_bytes))) + globalname_bytes
+                if custom.name_data.elemNameSubSec != None:
+                    name_section_bytes += bytes([0x08])
+                    name_section_bytes += LEB128U.encode(len(custom.name_data.elemNameSubSec))
+                    name_section_bytes += custom.name_data.elemNameSubSec
+                if custom.name_data.dataNameSubSec != []:
+                    dataname_bytes = bytes()
+                    dataname_bytes += LEB128U.encode(len(custom.name_data.dataNameSubSec))
+                    for dataname in custom.name_data.dataNameSubSec:
+                        dataname_bytes += LEB128U.encode(dataname.idx)
+                        dataname_bytes += LEB128U.encode(len(dataname.name))
+                        dataname_bytes += bytes(dataname.name, encoding="utf-8")
+                    name_section_bytes += (bytes([0x09]) + LEB128U.encode(len(dataname_bytes))) + dataname_bytes
+
+                with open(os.path.abspath(file_path), "rb+") as f:
+                    file_bytes = f.read()
+                    custom = self.module.section_range[SecCustomID][_]
+                    start = custom.start
+                    end = custom.end
+                    name_section_bytes = bytes([0x00]) + LEB128U.encode(len(name_section_bytes)) + name_section_bytes
+                    file_new_bytes = file_bytes[:start] + name_section_bytes + file_bytes[end:]
+                    change = len(name_section_bytes) - (end - start)
+
+                    custom.end = custom.start + len(name_section_bytes)
+                    self.fix_section_range(SecCustomID, change, custom.start, _)
+                    f.seek(0)
+                    f.truncate()
+                    f.write(file_new_bytes)
+            else:
+                custom_section_bytes = bytes()
+                custom_section_bytes += LEB128U.encode(len(custom.name))
+                custom_section_bytes += bytes(custom.name, encoding="utf-8")
+                custom_section_bytes += custom.custom_sec_data
+
+                with open(os.path.abspath(file_path), "rb+") as f:
+                    file_bytes = f.read()
+                    custom = self.module.section_range[SecCustomID][_]
+                    start = custom.start
+                    end = custom.end
+                    custom_section_bytes = bytes([0x00]) + LEB128U.encode(
+                        len(custom_section_bytes)) + custom_section_bytes
+                    file_new_bytes = file_bytes[:start] + custom_section_bytes + file_bytes[end:]
+                    change = len(custom_section_bytes) - (end - start)
+
+                    custom.end = custom.start + len(custom_section_bytes)
+                    self.fix_section_range(SecCustomID, change, custom.start, _)
+                    f.seek(0)
+                    f.truncate()
+                    f.write(file_new_bytes)
+
+        return None
+
+    def change_import_section(self, import_vec: list, file_path):
+
+        import_vec_len = len(import_vec)
+        import_vec_len_bytes = LEB128U.encode(import_vec_len)
+        import_vec_bytes = bytes()
+        import_vec_bytes += import_vec_len_bytes
+        if import_vec == []:
+            return
+        for i in import_vec:
+            import_vec_bytes += LEB128U.encode(len(i.module))
+            import_vec_bytes += bytes(i.module, encoding="utf-8")
+            import_vec_bytes += LEB128U.encode(len(i.name))
+            import_vec_bytes += bytes(i.name, encoding="utf-8")
+            import_vec_bytes += LEB128U.encode(i.desc.tag)
+            if i.desc.func_type is not None:
+                import_vec_bytes += LEB128U.encode(i.desc.func_type)
+            elif i.desc.table is not None:
+                import_vec_bytes += self.write_table_type(i.desc.table)
+            elif i.desc.mem is not None:
+                import_vec_bytes += self.write_limits(i.desc.mem)
+            elif i.desc.global_type is not None:
+                import_vec_bytes += self.write_global_type(i.desc.global_type)
+        import_section_bytes = bytes([0x02]) + LEB128U.encode(len(import_vec_bytes)) + import_vec_bytes
+
+        with open(os.path.abspath(file_path), "rb+") as f:
+            file_bytes = f.read()
+            file_new_bytes = file_bytes[
+                             :self.module.section_range[SecImportID].start] + import_section_bytes + file_bytes[
+                                                                                                     self.module.section_range[
+                                                                                                         SecImportID].end:]
+            change = len(import_section_bytes) - (
+                    self.module.section_range[SecImportID].end - self.module.section_range[SecImportID].start)
+
+            self.module.section_range[SecImportID].end = self.module.section_range[SecImportID].start + len(
+                import_section_bytes)
+            self.fix_section_range(SecImportID, change, self.module.section_range[SecImportID].start)
+            f.seek(0)
+            f.truncate()
+            f.write(file_new_bytes)
+
+        return import_section_bytes
+
+    def change_export_section(self, export_vec: list, file_path):
+        export_vec_len = len(export_vec)
+        export_vec_len_bytes = LEB128U.encode(export_vec_len)
+        export_vec_bytes = bytes()
+        export_vec_bytes += export_vec_len_bytes
+        if export_vec == []:
+            return
+        for export_item in export_vec:
+            export_vec_bytes += LEB128U.encode(len(export_item.name))
+            export_vec_bytes += bytes(export_item.name, encoding="utf-8")
+            export_vec_bytes += LEB128U.encode(export_item.desc.tag)
+            export_vec_bytes += LEB128U.encode(export_item.desc.idx)
+
+        export_section_bytes = bytes([0x07]) + LEB128U.encode(len(export_vec_bytes)) + export_vec_bytes
+
+        with open(os.path.abspath(file_path), "rb+") as f:
+            file_bytes = f.read()
+            file_new_bytes = file_bytes[
+                             :self.module.section_range[SecExportID].start] + export_section_bytes + file_bytes[
+                                                                                                     self.module.section_range[
+                                                                                                         SecExportID].end:]
+            change = len(export_section_bytes) - (
+                    self.module.section_range[SecExportID].end - self.module.section_range[SecExportID].start)
+
+            self.module.section_range[SecExportID].end = self.module.section_range[SecExportID].start + len(
+                export_section_bytes)
+            self.fix_section_range(SecExportID, change, self.module.section_range[SecExportID].start)
+            f.seek(0)
+            f.truncate()
+            f.write(file_new_bytes)
+
+        return export_section_bytes
+
+    def change_start_section(self, export_vec: list, file_path):
+        export_vec_len = len(export_vec)
+        export_vec_len_bytes = LEB128U.encode(export_vec_len)
+        export_vec_bytes = bytes()
+        export_vec_bytes += export_vec_len_bytes
+        if export_vec == []:
+            return
+        for export_item in export_vec:
+            export_vec_bytes += LEB128U.encode(len(export_item.name))
+            export_vec_bytes += bytes(export_item.name, encoding="utf-8")
+            export_vec_bytes += LEB128U.encode(export_item.desc.tag)
+            export_vec_bytes += LEB128U.encode(export_item.desc.idx)
+
+        export_section_bytes = bytes([0x07]) + LEB128U.encode(len(export_vec_bytes)) + export_vec_bytes
+
+        with open(os.path.abspath(file_path), "rb+") as f:
+            file_bytes = f.read()
+            file_new_bytes = file_bytes[
+                             :self.module.section_range[SecExportID].start] + export_section_bytes + file_bytes[
+                                                                                                     self.module.section_range[
+                                                                                                         SecExportID].end:]
+            change = len(export_section_bytes) - (
+                    self.module.section_range[SecExportID].end - self.module.section_range[SecExportID].start)
+
+            self.module.section_range[SecExportID].end = self.module.section_range[SecExportID].start + len(
+                export_section_bytes)
+            self.fix_section_range(SecExportID, change, self.module.section_range[SecExportID].start)
+            f.seek(0)
+            f.truncate()
+            f.write(file_new_bytes)
+
+        return export_section_bytes
+
+    def change_memory_section(self, memory_vec: list, file_path):
+        memory_vec_len = len(memory_vec)
+        memory_vec_len_bytes = LEB128U.encode(memory_vec_len)
+        memory_vec_bytes = bytes()
+        memory_vec_bytes += memory_vec_len_bytes
+        if memory_vec == []:
+            return
+        for memory_item in memory_vec:
+            memory_item_bytes = bytes()
+            memory_item_bytes += bytes([memory_item.tag])
+            memory_item_bytes += LEB128U.encode(memory_item.min)
+            if memory_item.max != 0:
+                memory_item_bytes += LEB128U.encode(memory_item.max)
+            memory_vec_bytes += memory_item_bytes
+
+        memroy_section_bytes = bytes([SecMemID]) + LEB128U.encode(len(memory_vec_bytes)) + memory_vec_bytes
+
+        with open(os.path.abspath(file_path), "rb+") as f:
+            file_bytes = f.read()
+            file_new_bytes = file_bytes[
+                             :self.module.section_range[SecMemID].start] + memroy_section_bytes + file_bytes[
+                                                                                                  self.module.section_range[
+                                                                                                      SecMemID].end:]
+            change = len(memroy_section_bytes) - (
+                    self.module.section_range[SecMemID].end - self.module.section_range[SecMemID].start)
+
+            self.module.section_range[SecMemID].end = self.module.section_range[SecMemID].start + len(
+                memroy_section_bytes)
+            self.fix_section_range(SecMemID, change, self.module.section_range[SecMemID].start)
+            f.seek(0)
+            f.truncate()
+            f.write(file_new_bytes)
+
+        return memroy_section_bytes
+
+    def change_data_section(self, data_vec: list, file_path):
+        data_vec_len = len(data_vec)
+        data_vec_len_bytes = LEB128U.encode(data_vec_len)
+        data_vec_bytes = bytes()
+        data_vec_bytes += data_vec_len_bytes
+        if not data_vec:
+            return
+        for data_item in data_vec:
+            data_item_bytes = bytes()
+            data_item_bytes += LEB128U.encode(data_item.mem)
+            data_item_bytes += self.write_expr(data_item.offset)
+            data_item_bytes += LEB128U.encode(len(data_item.init))
+            data_item_bytes += data_item.init
+
+            data_vec_bytes += data_item_bytes
+
+        data_section_bytes = bytes([SecDataID]) + LEB128U.encode(len(data_vec_bytes)) + data_vec_bytes
+
+        with open(os.path.abspath(file_path), "rb+") as f:
+            file_bytes = f.read()
+            file_new_bytes = file_bytes[
+                             :self.module.section_range[SecDataID].start] + data_section_bytes + file_bytes[
+                                                                                                 self.module.section_range[
+                                                                                                     SecDataID].end:]
+            change = len(data_section_bytes) - (
+                    self.module.section_range[SecDataID].end - self.module.section_range[SecDataID].start)
+
+            self.module.section_range[SecDataID].end = self.module.section_range[SecDataID].start + len(
+                data_section_bytes)
+            self.fix_section_range(SecDataID, change, self.module.section_range[SecDataID].start)
+            f.seek(0)
+            f.truncate()
+            f.write(file_new_bytes)
+
+        return data_section_bytes
+
+    def change_elem_section(self, elem_vec: list, file_path):
+
+        elem_vec_len = len(elem_vec)
+        elem_vec_len_bytes = LEB128U.encode(elem_vec_len)
+        elem_vec_bytes = bytes()
+        elem_vec_bytes += elem_vec_len_bytes
+        if elem_vec == []:
+            return
+        for elem in elem_vec:
+            elem_vec_bytes += LEB128U.encode(elem.table)
+            elem_vec_bytes += self.write_expr(elem.offset)
+            elem_vec_bytes += LEB128U.encode(len(elem.init))
+            for func_idx in elem.init:
+                elem_vec_bytes += LEB128U.encode(func_idx)
+        elem_section_bytes = bytes([SecElemID]) + LEB128U.encode(len(elem_vec_bytes)) + elem_vec_bytes
+
+        with open(os.path.abspath(file_path), "rb+") as f:
+            file_bytes = f.read()
+            binary_start = self.module.section_range[SecElemID].start
+            binary_end = self.module.section_range[SecElemID].end
+            if binary_start == binary_end:
+                for i in reversed(range(SecElemID)):
+                    if self.module.section_range[i].start != self.module.section_range[i].end:
+                        file_new_bytes = file_bytes[
+                                         :self.module.section_range[i].end] + elem_section_bytes + file_bytes[
+                                                                                                   self.module.section_range[
+                                                                                                       i].end:]
+                        change = len(elem_section_bytes) - (
+                                self.module.section_range[SecElemID].end - self.module.section_range[SecElemID].start)
+                        self.module.section_range[SecElemID].start = self.module.section_range[i].end
+                        self.module.section_range[SecElemID].end = self.module.section_range[i].end + len(
+                            elem_section_bytes)
+                        self.fix_section_range(SecElemID, change, self.module.section_range[SecElemID].start)
+                        f.seek(0)
+                        f.truncate()
+                        f.write(file_new_bytes)
+                        break
+            else:
+                file_new_bytes = file_bytes[
+                                 :self.module.section_range[SecElemID].start] + elem_section_bytes + file_bytes[
+                                                                                                     self.module.section_range[
+                                                                                                         SecElemID].end:]
+                change = len(elem_section_bytes) - (
+                        self.module.section_range[SecElemID].end - self.module.section_range[SecElemID].start)
+
+                self.module.section_range[SecElemID].end = self.module.section_range[SecElemID].start + len(
+                    elem_section_bytes)
+                self.fix_section_range(SecElemID, change, self.module.section_range[SecElemID].start)
+                f.seek(0)
+                f.truncate()
+                f.write(file_new_bytes)
+
+        return elem_section_bytes
+
+    def change_type_section(self, functype_vec: list, file_path):
+
+        functype_vec_len = len(functype_vec)
+        functype_vec_len_bytes = LEB128U.encode(functype_vec_len)
+        functype_vec_bytes = bytes()
+        functype_vec_bytes += functype_vec_len_bytes
+        if functype_vec == []:
+            return
+        for functype in functype_vec:
+            functype_bytes = bytes()
+            functype_bytes += bytes([0x60])
+            functype_bytes += self.write_val_types(functype.param_types)
+            functype_bytes += self.write_val_types(functype.result_types)
+            functype_vec_bytes += functype_bytes
+        type_section_bytes = bytes([0x01]) + LEB128U.encode(len(functype_vec_bytes)) + functype_vec_bytes
+
+        with open(os.path.abspath(file_path), "rb+") as f:
+            file_bytes = f.read()
+            file_new_bytes = file_bytes[:self.module.section_range[SecTypeID].start] + type_section_bytes + file_bytes[
+                                                                                                            self.module.section_range[
+                                                                                                                SecTypeID].end:]
+            change = len(type_section_bytes) - (
+                    self.module.section_range[SecTypeID].end - self.module.section_range[SecTypeID].start)
+
+            self.module.section_range[SecTypeID].end = self.module.section_range[SecTypeID].start + len(
+                type_section_bytes)
+            self.fix_section_range(SecTypeID, change, self.module.section_range[SecTypeID].start)
+            f.seek(0)
+            f.truncate()
+            f.write(file_new_bytes)
+
+        return type_section_bytes
+
+    def change_global_section(self, global_vec: list, file_path):
+
+        global_vec_len = len(global_vec)
+        global_vec_len_bytes = LEB128U.encode(global_vec_len)
+        global_vec_bytes = bytes()
+        global_vec_bytes += global_vec_len_bytes
+        if global_vec == []:
+            return
+        for global_item in global_vec:
+            global_bytes = bytes()
+            global_bytes += self.write_global(global_item)
+            global_vec_bytes += global_bytes
+
+        global_section_bytes = bytes([0x06]) + LEB128U.encode(len(global_vec_bytes)) + global_vec_bytes
+
+        with open(os.path.abspath(file_path), "rb+") as f:
+            file_bytes = f.read()
+            if self.module.section_range[SecGlobalID].start == 0:
+                for section in range(1, SecGlobalID):
+                    if self.module.section_range[section].start != 0:
+                        self.module.section_range[SecGlobalID].start = self.module.section_range[section].end
+                        self.module.section_range[SecGlobalID].end = self.module.section_range[SecGlobalID].start
+            file_new_bytes = file_bytes[
+                             :self.module.section_range[SecGlobalID].start] + global_section_bytes + file_bytes[
+                                                                                                     self.module.section_range[
+                                                                                                         SecGlobalID].end:]
+            change = len(global_section_bytes) - (
+                    self.module.section_range[SecGlobalID].end - self.module.section_range[SecGlobalID].start)
+
+            self.module.section_range[SecGlobalID].end = self.module.section_range[SecGlobalID].start + len(
+                global_section_bytes)
+            self.fix_section_range(SecGlobalID, change, self.module.section_range[SecGlobalID].start)
+            f.seek(0)
+            f.truncate()
+            f.write(file_new_bytes)
+
+        return global_section_bytes
+
+    def change_func_section(self, type_vec, file_path):
+
+        type_vec_len = len(type_vec)
+        type_vec_len_bytes = LEB128U.encode(type_vec_len)
+        type_vec_bytes = bytes()
+        type_vec_bytes += type_vec_len_bytes
+        if type_vec == []:
+            return
+        for type_item in type_vec:
+            type_vec_bytes += LEB128U.encode(type_item)
+
+        func_section_bytes = bytes([0x03]) + LEB128U.encode(len(type_vec_bytes)) + type_vec_bytes
+        with open(os.path.abspath(file_path), "rb+") as f:
+            file_bytes = f.read()
+            file_new_bytes = file_bytes[:self.module.section_range[SecFuncID].start] + func_section_bytes + file_bytes[
+                                                                                                            self.module.section_range[
+                                                                                                                SecFuncID].end:]
+            change = len(func_section_bytes) - (
+                    self.module.section_range[SecFuncID].end - self.module.section_range[SecFuncID].start)
+
+            self.module.section_range[SecFuncID].end = self.module.section_range[SecFuncID].start + len(
+                func_section_bytes)
+            self.fix_section_range(SecFuncID, change, self.module.section_range[SecFuncID].start)
+            f.seek(0)
+            f.truncate()
+            f.write(file_new_bytes)
+
+    def change_code_section(self, code_vec: list, file_path):
+
+        code_vec_len = len(code_vec)
+        code_vec_len_bytes = LEB128U.encode(code_vec_len)
+        code_vec_bytes = bytes()
+        code_vec_bytes += code_vec_len_bytes
+        if code_vec == []:
+            return
+        for code in code_vec:
+            code_bytes = bytes()
+            locals_vec_len = len(code.locals)
+            locals_vec_len_bytes = LEB128U.encode(locals_vec_len)
+            locals_vec_bytes = bytes()
+            expr_bytes = bytes()
+
+            for local in code.locals:
+                local_count = local.n
+                local_type = local.type
+                locals_vec_bytes += LEB128U.encode(local_count)
+                locals_vec_bytes += bytes([local_type])
+
+            expr_bytes += self.write_expr(code.expr)
+            code_bytes += (locals_vec_len_bytes + locals_vec_bytes + expr_bytes)
+            code_vec_bytes += LEB128U.encode(len(code_bytes)) + code_bytes
+        code_section_bytes = bytes([0x0A]) + LEB128U.encode(len(code_vec_bytes)) + code_vec_bytes
+
+        with open(os.path.abspath(file_path), "rb+") as f:
+            file_bytes = f.read()
+            file_new_bytes = file_bytes[:self.module.section_range[SecCodeID].start] + code_section_bytes + file_bytes[
+                                                                                                            self.module.section_range[
+                                                                                                                SecCodeID].end:]
+            change = len(code_section_bytes) - (
+                    self.module.section_range[SecCodeID].end - self.module.section_range[SecCodeID].start)
+
+            self.module.section_range[SecCodeID].end = self.module.section_range[SecCodeID].start + len(
+                code_section_bytes)
+            self.fix_section_range(SecCodeID, change, self.module.section_range[SecCodeID].start)
+            f.seek(0)
+            f.truncate()
+            f.write(file_new_bytes)
+
+        return code_section_bytes
+
+    def change_table_section(self, table_vec: list, file_path):
+
+        table_vec_len = len(table_vec)
+        table_vec_len_bytes = LEB128U.encode(table_vec_len)
+        table_vec_bytes = bytes()
+        table_vec_bytes += table_vec_len_bytes
+        if table_vec == []:
+            return
+        for table_type in table_vec:
+            table_type_bytes = bytes()
+            table_type_bytes += bytes([table_type.elem_type])
+            table_type_bytes += bytes([table_type.limits.tag])
+            table_type_bytes += LEB128U.encode(table_type.limits.min)
+            if 0 != table_type.limits.max:
+                table_type_bytes += LEB128U.encode(table_type.limits.max)
+            table_vec_bytes += table_type_bytes
+
+        table_section_bytes = bytes([0x04]) + LEB128U.encode(len(table_vec_bytes)) + table_vec_bytes
+
+        with open(os.path.abspath(file_path), "rb+") as f:
+            file_bytes = f.read()
+            binary_start = self.module.section_range[SecTableID].start
+            binary_end = self.module.section_range[SecTableID].end
+            if binary_start == binary_end:
+                for i in reversed(range(SecTableID)):
+                    if self.module.section_range[i].start != self.module.section_range[i].end:
+                        file_new_bytes = file_bytes[
+                                         :self.module.section_range[i].end] + table_section_bytes + file_bytes[
+                                                                                                    self.module.section_range[
+                                                                                                        i].end:]
+                        change = len(table_section_bytes) - (
+                                self.module.section_range[SecTableID].end - self.module.section_range[
+                            SecTableID].start)
+                        self.module.section_range[SecTableID].start = self.module.section_range[i].end
+                        self.module.section_range[SecTableID].end = self.module.section_range[i].end + len(
+                            table_section_bytes)
+                        self.fix_section_range(SecTableID, change, self.module.section_range[SecTableID].start)
+                        f.seek(0)
+                        f.truncate()
+                        f.write(file_new_bytes)
+                        break
+            else:
+                file_new_bytes = file_bytes[
+                                 :self.module.section_range[SecTableID].start] + table_section_bytes + file_bytes[
+                                                                                                       self.module.section_range[
+                                                                                                           SecTableID].end:]
+                change = len(table_section_bytes) - (
+                        self.module.section_range[SecTableID].end - self.module.section_range[SecTableID].start)
+
+                self.module.section_range[SecTableID].end = self.module.section_range[SecTableID].start + len(
+                    table_section_bytes)
+                self.fix_section_range(SecTableID, change, self.module.section_range[SecTableID].start)
+                f.seek(0)
+                f.truncate()
+                f.write(file_new_bytes)
+
+        return table_section_bytes
+
+    def write_expr(self, expr: list):
+
+        instructions_bytes = self.write_instructions(expr)
+        expr_bytes = instructions_bytes + bytes([0x0b])
+
+        return expr_bytes
+
+    def write_instructions(self, expr: list):
+
+        instructions_bytes = bytes()
+        for index in range(len(expr)):
+            instructions_bytes += self.write_instruction(expr[index])
+
+        return instructions_bytes
+
+    def write_instruction(self, instr):
+
+        instruction_bytes = bytes()
+        instruction_bytes += bytes([instr.opcode])
+        args_bytes = self.write_args(instr)
+        if args_bytes is not None:
+            instruction_bytes += args_bytes
+
+        return instruction_bytes
+
+    def write_args(self, instr):
+
+        opcode = instr.opcode
+        if opcode in [Block, Loop]:
+            return self.write_block_args(instr)
+        elif opcode == If:
+            return self.write_if_args(instr)
+        elif opcode in [Br, BrIf]:
+            return LEB128U.encode(instr.args)
+        elif opcode == BrTable:
+            return self.write_br_table_args(instr)
+        elif opcode == Call:
+            return LEB128U.encode(instr.args)
+        elif opcode == CallIndirect:
+            return self.write_call_indirect_args(instr)
+        elif opcode in [LocalGet, LocalSet, LocalTee]:
+            return LEB128U.encode(instr.args)
+        elif opcode in [GlobalGet, GlobalSet]:
+            return LEB128U.encode(instr.args)
+        elif opcode in [MemorySize, MemoryGrow]:
+            return bytes([0x00])
+        elif opcode == I32Const:
+            return LEB128S.encode(instr.args)
+        elif opcode == I64Const:
+            return LEB128S.encode(instr.args)
+        elif opcode == F32Const:
+            return struct.pack('<f', instr.args)
+        elif opcode == F64Const:
+            return struct.pack('<d', instr.args)
+        elif opcode == TruncSat:
+            return bytes([instr.args])
+        else:
+            if I32Load <= instr.opcode <= I64Store32:
+                return self.write_mem_arg(instr)
+            return None
+
+    def write_block_args(self, instr):
+
+        args_bytes = bytes()
+        args_bytes += LEB128S.encode(instr.args.bt)
+        args_bytes += self.write_instructions(instr.args.instrs)
+        args_bytes += bytes([0x0b])
+
+        return args_bytes
+
+    def write_if_args(self, instr):
+
+        args_bytes = bytes()
+        args_bytes += LEB128S.encode(instr.args.bt)
+        args_bytes += self.write_instructions(instr.args.instrs1)
+        if instr.args.instrs2:
+            args_bytes += bytes([0x05])
+            args_bytes += self.write_instructions(instr.args.instrs2)
+            args_bytes += bytes([0x0b])
+        else:
+            args_bytes += bytes([0x0b])
+
+        return args_bytes
+
+    @staticmethod
+    def write_br_table_args(instr):
+
+        args_bytes = bytes()
+        args_bytes += LEB128U.encode(len(instr.args.labels))
+        for label in instr.args.labels:
+            args_bytes += LEB128U.encode(label)
+        args_bytes += LEB128U.encode(instr.args.default)
+
+        return args_bytes
+
+    @staticmethod
+    def write_call_indirect_args(instr):
+
+        args_bytes = bytes()
+        args_bytes += LEB128U.encode(instr.args)
+        args_bytes += bytes([0x00])
+
+        return args_bytes
+
+    @staticmethod
+    def write_mem_arg(instr):
+
+        args_bytes = bytes()
+        args_bytes += LEB128U.encode(instr.args.align)
+        args_bytes += LEB128U.encode(instr.args.offset)
+
+        return args_bytes
+
+    @staticmethod
+    def write_val_types(val_types):
+
+        val_types_bytes = bytes()
+        val_types_bytes += LEB128U.encode(len(val_types))
+        for val in val_types:
+            val_types_bytes += bytes([val])
+
+        return val_types_bytes
+
+    @staticmethod
+    def write_global_type(global_type):
+
+        global_type_bytes = bytes()
+        global_type_bytes += bytes([global_type.val_type])
+        global_type_bytes += bytes([global_type.mut])
+        return global_type_bytes
+
+    @staticmethod
+    def write_limits(mem):
+
+        mem_bytes = bytes()
+        mem_bytes += bytes([mem.tag])
+        mem_bytes += LEB128U.encode(mem.min)
+        if mem.tag == 1:
+            mem_bytes += LEB128U.encode(mem.max)
+        return mem_bytes
+
+    @staticmethod
+    def write_table_type(table_type):
+
+        table_type_bytes = bytes()
+        table_type_bytes += bytes([table_type.elem_type])
+        table_type_bytes += bytes([table_type.limits.tag])
+        if table_type.limits.min != 0:
+            table_type_bytes += LEB128U.encode(table_type.limits.min)
+        if table_type.limits.max != 0:
+            table_type_bytes += LEB128U.encode(table_type.limits.max)
+        return table_type_bytes
+
+    def write_global(self, global_item):
+        global_bytes = bytes()
+        global_bytes += self.write_global_type(global_item.type)
+        global_bytes += self.write_expr(global_item.init)
+        return global_bytes
+
+
+def get_functype_idx(module, functype):
+    functype_id = None
+    for _, i in enumerate(module.type_sec):
+        if i.equal(functype) is True:
+            functype_id = _
+    return functype_id
```

### Comparing `BREWasm-1.0.0/BREWasm/rewriter/section_rewriter.py` & `BREWasm-1.0.1/BREWasm/rewriter/section_rewriter.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,1296 +1,1296 @@
-from BREWasm.parser import module
-from BREWasm.rewriter.modify_binary import ModifyBinary
-from BREWasm.rewriter.defination import *
-from BREWasm.rewriter.indices_fixer import *
-from BREWasm.parser.instruction import Instruction
-from BREWasm.rewriter.indices_fixer import IndicesFixer
-
-
-# class RetInstrs:
-#     def __init__(self, index, instr, instrs):
-#         self.index = index
-#         self.instr = instr
-#         self.instrs = instrs
-
-
-class SectionRewriter:
-
-    def __init__(self, module, **section):
-        """
-
-        Args:
-            module:
-            **section:
-        """
-
-        allowed_params = ['typesec', 'importsec', 'funcsec', 'tablesec', 'memsec',
-                          'globalsec', 'exportsec', 'startsec', 'elemsec', 'codesec',
-                          'datasec', 'datacountsec', 'customsec']
-
-        if len(section) != 1:
-            raise ValueError("Only one parameter should be provided")
-
-        param_name = next(iter(section.keys()))
-        if param_name not in allowed_params:
-            raise ValueError("Invalid parameter")
-
-        self.module = module
-        self.typesec = None
-        self.importsec = None
-        self.funcsec = None
-        self.tablesec = None
-        self.memsec = None
-        self.globalsec = None
-        self.exportsec = None
-        self.startsec = None
-        self.elemsec = None
-        self.codesec = None
-        self.datasec = None
-        self.datacountsec = None
-        self.customsec = None
-        self.indices_fixer = IndicesFixer(module)
-
-        setattr(self, param_name, section[param_name])
-
-    def select(self, query):
-        if self.typesec is not None and isinstance(query, Type):
-            type_list = []
-            for idx, item in enumerate(self.module.type_sec):
-                param_types, result_types = item.get_signature()
-                if all(
-                        (query.typeidx is None or query.typeidx == idx,
-                         query.arg_types is None or query.arg_types == param_types,
-                         query.ret_types is None or query.ret_types == result_types,)
-                ):
-                    type_list.append(Type(idx, param_types, result_types))
-            return type_list
-
-        elif self.importsec is not None and isinstance(query, Import):
-
-            import_list = []
-            for idx, item in enumerate(self.module.import_sec):
-                if item.desc.func_type is not None:
-                    if all(
-                            (query.importidx is None or query.importidx == idx,
-                             query.module is None or query.module == item.module,
-                             query.name is None or query.name == item.name,
-                             query.typeidx is None or query.typeidx == item.desc.func_type)
-                    ):
-                        import_list.append(Import(idx, item.module, item.name, item.desc.func_type))
-            return import_list
-
-        elif self.funcsec is not None and isinstance(query, Function):
-            function_list = []
-
-            # get import func num
-            import_func_num = 0
-            for import_func in self.module.import_sec:
-                if import_func.desc.func_type is not None:
-                    import_func_num += 1
-
-            if query.funcidx is not None:
-                query.funcidx -= import_func_num
-
-            for idx, item in enumerate(self.module.func_sec):
-                if all(
-                        (query.funcidx is None or query.funcidx == idx,
-                         query.typeidx is None or query.typeidx == item)
-                ):
-                    function_list.append(Function(idx + import_func_num, item))
-            return function_list
-
-        elif self.tablesec is not None and isinstance(query, Table):
-            # 如何表示无穷
-            table_list = []
-            for idx, item in enumerate(self.module.table_sec):
-                if all(
-                        (query.min is None or query.min == item.limits.min,
-                         query.max is None or query.max == item.limits.max)
-                ):
-                    table_list.append(Table(item.limits.min, item.limits.max))
-            return table_list
-
-        elif self.memsec is not None and isinstance(query, Memory):
-
-            # 如何表示无穷
-            mem_list = []
-            for idx, item in enumerate(self.module.mem_sec):
-                if all(
-                        (query.min is None or query.min == item.min,
-                         query.max is None or query.max == item.max)
-                ):
-                    mem_list.append(Memory(item.min, item.max))
-            return mem_list
-
-        elif self.globalsec is not None and isinstance(query, Global):
-            global_list = []
-            for idx, item in enumerate(self.module.global_sec):
-                if all(
-                        (query.globalidx is None or query.globalidx == idx,
-                         query.valtype is None or query.valtype == item.type.val_type,
-                         query.mut is None or query.mut == item.type.mut,
-                         query.val is None or query.val == item.init[0].args)
-                ):
-                    global_list.append(Global(idx, item.type.val_type, item.type.mut, item.init[0].args))
-            return global_list
-
-        elif self.exportsec is not None and isinstance(query, Export):
-            export_list = []
-            for idx, item in enumerate(self.module.export_sec):
-                if all(
-                        (query.exportidx is None or query.exportidx == idx,
-                         query.name is None or query.name == item.name,
-                         # The tag of function is 0
-                         query.funcidx is None or query.funcidx == item.desc.idx)
-                ) and item.desc.tag == 0:
-                    export_list.append(Export(idx, name=item.name, funcidx=item.desc.idx))
-            return export_list
-
-        elif self.startsec is not None and isinstance(query, Start):
-            match query:
-                case Start(funcidx=funcidx):
-                    return Start(self.module.start_sec)
-                case Start():
-                    return Start(self.module.start_sec)
-
-        elif self.elemsec is not None and isinstance(query, Element):
-            element_list = []
-            for idx, item in enumerate(self.module.elem_sec):
-                if all(
-                        (query.elemidx is None or query.elemidx == idx,
-                         query.tableidx is None or query.tableidx == item.table,
-                         query.offset is None or query.offset == item.offset[0].args)
-                ):
-                    element_list.append(
-                        Element(idx, tableidx=item.table, offset=item.offset[0].args, funcidx_list=item.init))
-            return element_list
-
-        elif self.codesec is not None and isinstance(query, Code):
-            code_list = []
-            # get import func num
-            import_func_num = 0
-            for import_func in self.module.import_sec:
-                if import_func.desc.func_type is not None:
-                    import_func_num += 1
-            if query.funcidx < import_func_num:
-                raise Exception("Import function!")
-            query.funcidx -= import_func_num
-            for idx, item in enumerate(self.module.code_sec):
-                if query.funcidx is None or query.funcidx == idx:
-                    # locals
-                    locals = []
-                    i = 0
-                    for local in item.locals:
-                        for j in range(i, i + local.n):
-                            locals.append(Local(j, local.type))
-                        i += local.n
-                    # instrs
-                    instrs = self.get_flat_instrs(item.expr)
-                    code_list.append(Code(idx + import_func_num, locals, instrs))
-            return code_list
-
-        elif self.datasec is not None and isinstance(query, Data):
-            data_list = []
-            for idx, item in enumerate(self.module.data_sec):
-                if all(
-                        (query.dataidx is None or query.dataidx == idx,
-                         query.offset is None or query.offset == item.offset[0].args)
-                ):
-                    data_list.append(Data(idx, item.offset[0].args, item.init))
-            return data_list
-
-        elif self.datacountsec is not None:
-            pass
-        elif self.customsec is not None and isinstance(query, CustomName):
-            name_list = []
-            match query.name_type:
-                # func 0
-                case 0:
-                    for custom in self.module.custom_secs:
-                        if custom.name == "name":
-                            for idx, item in enumerate(custom.name_data.funcNameSubSec):
-                                if all(
-                                        (query.idx is None or query.idx == item.idx,
-                                         query.name is None or query.name == item.name)
-                                ):
-                                    name_list.append(CustomName(FunctionName, item.idx, item.name))
-                case 1:
-                    for custom in self.module.custom_secs:
-                        if custom.name == "name":
-                            for idx, item in enumerate(custom.name_data.globalNameSubSec):
-                                if all(
-                                        (query.idx is None or query.idx == item.idx,
-                                         query.name is None or query.name == item.name)
-                                ):
-                                    name_list.append(CustomName(GlobalName, item.idx, item.name))
-                case 2:
-                    for custom in self.module.custom_secs:
-                        if custom.name == "name":
-                            for idx, item in enumerate(custom.name_data.dataNameSubSec):
-                                if all(
-                                        (query.idx is None or query.idx == item.idx,
-                                         query.name is None or query.name == item.name)
-                                ):
-                                    name_list.append(CustomName(DataName, item.idx, item.name))
-                case _:
-                    pass
-            return name_list
-        else:
-            raise Exception("error")
-
-    def insert(self, query, inserted_item):
-
-        if self.typesec is not None and isinstance(inserted_item, Type):
-            if query is None:
-                # append
-                self.module.type_sec.append(inserted_item.convert())
-            elif isinstance(query, Type):
-                type_list = []
-                for idx, item in enumerate(self.module.type_sec):
-                    param_types, result_types = item.get_signature()
-                    if all(
-                            (query.typeidx is None or query.typeidx == idx,
-                             query.arg_types is None or query.arg_types == param_types,
-                             query.ret_types is None or query.ret_types == result_types,)
-                    ):
-                        type_list.append(Type(idx, param_types, result_types))
-                if len(type_list) != 1:
-                    raise Exception("error")
-
-                idx = type_list[0].typeidx
-                # insert
-                self.module.type_sec.insert(idx, inserted_item.convert())
-
-                # fix
-                self.indices_fixer.fix_func_functypeidx(self.module.func_sec, idx)
-                self.indices_fixer.fix_import_func_functypeidx(self.module.import_sec, idx)
-
-        elif self.importsec is not None and isinstance(inserted_item, Import):
-            if query is None:
-                self.module.import_sec.append(module.Import(inserted_item.module, inserted_item.name,
-                                                            module.ImportDesc(tag=0,
-                                                                              func_type=inserted_item.typeidx)))
-            elif isinstance(query, Import):
-                import_list = []
-                for idx, item in enumerate(self.module.import_sec):
-                    if item.desc.func_type is not None:
-                        if all(
-                                (query.importidx is None or query.importidx == idx,
-                                 query.module is None or query.module == item.module,
-                                 query.name is None or query.name == item.name,
-                                 query.typeidx is None or query.typeidx == item.desc.func_type)
-                        ):
-                            import_list.append(Import(idx, item.module, item.name, item.desc.func_type))
-
-                if len(import_list) != 1:
-                    raise Exception("error")
-
-                idx = import_list[0].importidx
-
-                self.module.import_sec.insert(idx, module.Import(inserted_item.module, inserted_item.name,
-                                                                 module.ImportDesc(tag=0,
-                                                                                   func_type=inserted_item.typeidx)))
-
-            # fix
-            import_func_id = None
-            for i, import_item in enumerate([i for i in self.module.import_sec if i.desc.func_type is not None]):
-                if import_item.module == inserted_item.module and import_item.name == inserted_item.name:
-                    import_func_id = i
-            for _, code in enumerate(self.module.code_sec):
-                self.indices_fixer.fix_call_instructions(code.expr, import_func_id)
-            self.indices_fixer.fix_elem_funcidx(self.module.elem_sec, import_func_id)
-            self.indices_fixer.fix_export_funcidx(self.module.export_sec, import_func_id)
-
-        elif self.funcsec is not None and isinstance(inserted_item, Function):
-            if query is None:
-                self.module.func_sec.append(inserted_item.typeidx)
-            elif isinstance(query, Function):
-                function_list = []
-
-                # get import func num
-                import_func_num = 0
-                for import_func in self.module.import_sec:
-                    if import_func.desc.func_type is not None:
-                        import_func_num += 1
-
-                if query.funcidx is not None:
-                    query.funcidx -= import_func_num
-
-                for idx, item in enumerate(self.module.func_sec):
-                    if all(
-                            (query.funcidx is None or query.funcidx == idx,
-                             query.typeidx is None or query.typeidx == item)
-                    ):
-                        function_list.append(Function(idx + import_func_num, item))
-
-                if len(function_list) != 1:
-                    raise Exception("error")
-
-                idx = function_list[0].funcidx
-                # insert
-                self.module.func_sec.insert(idx - import_func_num, inserted_item.typeidx)
-
-                # fix
-                self.indices_fixer.fix_export_funcidx(self.module.export_sec, idx)
-                self.indices_fixer.fix_elem_funcidx(self.module.elem_sec, idx)
-                for _, code in enumerate(self.module.code_sec):
-                    self.indices_fixer.fix_call_instructions(code.expr, idx)
-
-
-        # table 和 memory 段暂时不能修改
-        # elif self.tablesec is not None and isinstance(query, Table):
-        #     # 如何表示无穷
-        #     table_list = []
-        #     for idx, item in enumerate(self.module.table_sec):
-        #         if all(
-        #                 (query.min is None or query.min == item.limits.min,
-        #                  query.max is None or query.max == item.limits.max)
-        #         ):
-        #             table_list.append(Table(item.limits.min, item.limits.max))
-        #
-        #     if len(table_list) != 1:
-        #         raise Exception("error")
-        #
-        #     idx = table_list[0]
-        #
-        #     return table_list
-        #
-        # elif self.memsec is not None and isinstance(query, Memory):
-        #
-        #     # 如何表示无穷
-        #     mem_list = []
-        #     for idx, item in enumerate(self.module.mem_sec):
-        #         if all(
-        #                 (query.min is None or query.min == item.min,
-        #                  query.max is None or query.max == item.max)
-        #         ):
-        #             mem_list.append(Memory(item.min, item.max))
-        #     return mem_list
-
-        elif self.globalsec is not None and isinstance(inserted_item, Global):
-            if inserted_item.valtype == I32:
-                init_value_instr = Instruction(I32Const, inserted_item.val)
-            elif inserted_item.valtype == I64:
-                init_value_instr = Instruction(I64Const, inserted_item.val)
-            elif inserted_item.valtype == F32:
-                init_value_instr = Instruction(F32Const, inserted_item.val)
-            elif inserted_item.valtype == F64:
-                init_value_instr = Instruction(F64Const, inserted_item.val)
-            else:
-                raise Exception("global type error!")
-
-            # The default mutable attribute is 0
-            if inserted_item.mut is None:
-                inserted_item.mut = 0
-
-            if query is None:
-                self.module.global_sec.append(module.Global(GlobalType(inserted_item.valtype, inserted_item.mut),
-                                                            [init_value_instr]))
-            elif isinstance(query, Global):
-                global_list = []
-                for idx, item in enumerate(self.module.global_sec):
-                    if all(
-                            (query.globalidx is None or query.globalidx == idx,
-                             query.valtype is None or query.valtype == item.type.val_type,
-                             query.mut is None or query.mut == item.type.mut,
-                             query.val is None or query.val == item.init[0].args)
-                    ):
-                        global_list.append(Global(idx, item.type.val_type, item.type.mut, item.init[0].args))
-
-                if len(global_list) != 1:
-                    raise Exception("error")
-                idx = global_list[0].globalidx
-                # insert
-                self.module.global_sec.insert(idx, module.Global(GlobalType(inserted_item.valtype, inserted_item.mut),
-                                                                 [init_value_instr]))
-
-                # fix
-                self.indices_fixer.fix_export_globalidx(self.module.export_sec, idx)
-                for code in self.module.code_sec:
-                    self.indices_fixer.fix_global_instructions(code.expr, idx)
-
-        elif self.exportsec is not None and isinstance(inserted_item, Export):
-            if query is None:
-                self.module.export_sec.append(
-                    module.Export(inserted_item.name, module.ExportDesc(0, inserted_item.funcidx)))
-            elif isinstance(query, Export):
-                export_list = []
-                for idx, item in enumerate(self.module.export_sec):
-                    if all(
-                            (query.exportidx is None or query.exportidx == idx,
-                             query.name is None or query.name == item.name,
-                             # The tag of function is 0
-                             query.funcidx is None or query.funcidx == item.desc.idx)
-                    ):
-                        export_list.append(Export(idx, name=item.name, funcidx=item.desc.idx))
-
-                if len(export_list) != 1:
-                    raise Exception("error")
-
-                idx = export_list[0].exportidx
-                self.module.export_sec.insert(idx, module.Export(inserted_item.name,
-                                                                 module.ExportDesc(0, inserted_item.funcidx)))
-
-        elif self.startsec is not None and isinstance(inserted_item, Start):
-            match query:
-                case Start(funcidx=funcidx):
-                    return Start(self.module.start_sec)
-                case Start():
-                    return Start(self.module.start_sec)
-
-        elif self.elemsec is not None and isinstance(inserted_item, Element):
-            element_list = []
-            for idx, item in enumerate(self.module.elem_sec):
-                if all(
-                        (query.elemidx is None or query.elemidx == idx,
-                         query.tableidx is None or query.tableidx == item.table,
-                         query.offset is None or query.offset == item.offset[0].args)
-                ):
-                    element_list.append(
-                        Element(idx, tableidx=item.table, offset=item.offset[0].args, funcidx_list=item.init))
-            return element_list
-
-        elif self.codesec is not None and isinstance(inserted_item, Code):
-            locals = inserted_item.convert_local_vec()
-            fold_instrs = self.get_fold_instrs(inserted_item.instr_list)
-
-            if query is None:
-                self.module.code_sec.append(module.Code(locals, fold_instrs))
-            elif isinstance(query, Code):
-
-                code_list = []
-                # get import func num
-                import_func_num = 0
-                for import_func in self.module.import_sec:
-                    if import_func.desc.func_type is not None:
-                        import_func_num += 1
-                if query.funcidx < import_func_num:
-                    raise Exception("Import function!")
-                query.funcidx -= import_func_num
-                for idx, item in enumerate(self.module.code_sec):
-                    if query.funcidx is None or query.funcidx == idx:
-                        # locals
-                        local_vec = []
-                        i = 0
-                        for local in item.locals:
-                            for j in range(i, i + local.n):
-                                local_vec.append(Local(j, local.type))
-                            i += local.n
-                        # instrs
-                        instrs = self.get_flat_instrs(item.expr)
-                        code_list.append(Code(idx + import_func_num, local_vec, instrs))
-
-                if len(code_list) != 1:
-                    raise Exception("error")
-
-                idx = code_list[0].funcidx - import_func_num
-
-                self.module.code_sec.insert(idx, module.Code(locals, fold_instrs))
-
-        elif self.datasec is not None and isinstance(inserted_item, Data):
-            data_list = []
-            for idx, item in enumerate(self.module.data_sec):
-                if all(
-                        (query.dataidx is None or query.dataidx == idx,
-                         query.offset is None or query.offset == item.offset[0].args)
-                ):
-                    data_list.append(Data(idx, item.offset[0].args, item.init))
-            return data_list
-
-        elif self.datacountsec is not None:
-            pass
-        elif self.customsec is not None and isinstance(inserted_item, CustomName):
-            name_list = []
-            match query.name_type:
-                # func 0
-                case 0:
-                    for custom in self.module.custom_secs:
-                        if custom.name == "name":
-                            for idx, item in enumerate(custom.name_data.funcNameSubSec):
-                                if all(
-                                        (query.idx is None or query.idx == item.idx,
-                                         query.name is None or query.name == item.name)
-                                ):
-                                    name_list.append(CustomName(FunctionName, item.idx, item.name))
-                case 1:
-                    for custom in self.module.custom_secs:
-                        if custom.name == "name":
-                            for idx, item in enumerate(custom.name_data.globalNameSubSec):
-                                if all(
-                                        (query.idx is None or query.idx == item.idx,
-                                         query.name is None or query.name == item.name)
-                                ):
-                                    name_list.append(CustomName(GlobalName, item.idx, item.name))
-                case 2:
-                    for custom in self.module.custom_secs:
-                        if custom.name == "name":
-                            for idx, item in enumerate(custom.name_data.dataNameSubSec):
-                                if all(
-                                        (query.idx is None or query.idx == item.idx,
-                                         query.name is None or query.name == item.name)
-                                ):
-                                    name_list.append(CustomName(DataName, item.idx, item.name))
-                case _:
-                    pass
-            return name_list
-        else:
-            raise Exception("error")
-
-    def delete(self, query):
-
-        if self.typesec is not None and isinstance(query, Type):
-            type_list = []
-            for idx, item in enumerate(self.module.type_sec):
-                param_types, result_types = item.get_signature()
-                if all(
-                        (query.typeidx is None or query.typeidx == idx,
-                         query.arg_types is None or query.arg_types == param_types,
-                         query.ret_types is None or query.ret_types == result_types,)
-                ):
-                    type_list.append(Type(idx, param_types, result_types))
-            if len(type_list) != 1:
-                raise Exception("error")
-
-            idx = type_list[0].typeidx
-            # delete
-            self.module.type_sec.pop(idx)
-
-            # fix
-            self.indices_fixer.fix_func_functypeidx(self.module.func_sec, idx, type=Delete)
-            self.indices_fixer.fix_import_func_functypeidx(self.module.import_sec, idx, type=Delete)
-
-        elif self.importsec is not None and isinstance(query, Import):
-
-            import_list = []
-            for idx, item in enumerate(self.module.import_sec):
-                if item.desc.func_type is not None:
-                    if all(
-                            (query.importidx is None or query.importidx == idx,
-                             query.module is None or query.module == item.module,
-                             query.name is None or query.name == item.name,
-                             query.typeidx is None or query.typeidx == item.desc.func_type)
-                    ):
-                        import_list.append(Import(idx, item.module, item.name, item.desc.func_type))
-
-            if len(import_list) != 1:
-                raise Exception("error")
-
-            idx = import_list[0].importidx
-
-            self.module.import_sec.pop(idx)
-
-            # fix
-            import_func_id = None
-            for i, import_item in enumerate([i for i in self.module.import_sec if i.desc.func_type is not None]):
-                if import_item.module == item.module and import_item.name == item.name:
-                    import_func_id = i
-            for _, code in enumerate(self.module.code_sec):
-                self.indices_fixer.fix_call_instructions(code.expr, import_func_id, type=Delete)
-            self.indices_fixer.fix_elem_funcidx(self.module.elem_sec, import_func_id, type=Delete)
-            self.indices_fixer.fix_export_funcidx(self.module.export_sec, import_func_id, type=Delete)
-
-        elif self.funcsec is not None and isinstance(query, Function):
-            function_list = []
-
-            # get import func num
-            import_func_num = 0
-            for import_func in self.module.import_sec:
-                if import_func.desc.func_type is not None:
-                    import_func_num += 1
-
-            if query.funcidx is not None:
-                query.funcidx -= import_func_num
-
-            for idx, item in enumerate(self.module.func_sec):
-                if all(
-                        (query.funcidx is None or query.funcidx == idx,
-                         query.typeidx is None or query.typeidx == item)
-                ):
-                    function_list.append(Function(idx + import_func_num, item))
-
-            if len(function_list) != 1:
-                raise Exception("error")
-
-            idx = function_list[0].funcidx
-            # delete
-            self.module.func_sec.pop(idx - import_func_num)
-
-            # fix
-            self.indices_fixer.fix_export_funcidx(self.module.export_sec, idx, type=Delete)
-            self.indices_fixer.fix_elem_funcidx(self.module.elem_sec, idx, type=Delete)
-            for _, code in enumerate(self.module.code_sec):
-                self.indices_fixer.fix_call_instructions(code.expr, idx, type=Delete)
-
-
-        # table 和 memory 段暂时不能修改
-        # elif self.tablesec is not None and isinstance(query, Table):
-        #     # 如何表示无穷
-        #     table_list = []
-        #     for idx, item in enumerate(self.module.table_sec):
-        #         if all(
-        #                 (query.min is None or query.min == item.limits.min,
-        #                  query.max is None or query.max == item.limits.max)
-        #         ):
-        #             table_list.append(Table(item.limits.min, item.limits.max))
-        #
-        #     if len(table_list) != 1:
-        #         raise Exception("error")
-        #
-        #     idx = table_list[0]
-        #
-        #     return table_list
-        #
-        # elif self.memsec is not None and isinstance(query, Memory):
-        #
-        #     # 如何表示无穷
-        #     mem_list = []
-        #     for idx, item in enumerate(self.module.mem_sec):
-        #         if all(
-        #                 (query.min is None or query.min == item.min,
-        #                  query.max is None or query.max == item.max)
-        #         ):
-        #             mem_list.append(Memory(item.min, item.max))
-        #     return mem_list
-
-        elif self.globalsec is not None and isinstance(query, Global):
-            global_list = []
-            for idx, item in enumerate(self.module.global_sec):
-                if all(
-                        (query.globalidx is None or query.globalidx == idx,
-                         query.valtype is None or query.valtype == item.type.val_type,
-                         query.mut is None or query.mut == item.type.mut,
-                         query.val is None or query.val == item.init[0].args)
-                ):
-                    global_list.append(Global(idx, item.type.val_type, item.type.mut, item.init[0].args))
-
-            if len(global_list) != 1:
-                raise Exception("error")
-            idx = global_list[0].globalidx
-
-            self.module.global_sec.pop(idx)
-
-            # fix
-            self.indices_fixer.fix_export_globalidx(self.module.export_sec, idx, type=Delete)
-            for code in self.module.code_sec:
-                self.indices_fixer.fix_global_instructions(code.expr, idx, type=Delete)
-
-        elif self.exportsec is not None and isinstance(query, Export):
-            export_list = []
-            for idx, item in enumerate(self.module.export_sec):
-                if all(
-                        (query.exportidx is None or query.exportidx == idx,
-                         query.name is None or query.name == item.name,
-                         # The tag of function is 0
-                         query.funcidx is None or query.funcidx == item.desc.idx)
-                ) and item.desc.tag == 0:
-                    export_list.append(Export(idx, name=item.name, funcidx=item.desc.idx))
-
-            if len(export_list) != 1:
-                raise Exception("error")
-
-            idx = export_list[0].exportidx
-            self.module.export_sec.pop(idx)
-
-        elif self.startsec is not None and isinstance(query, Start):
-            match query:
-                case Start(funcidx=funcidx):
-                    return Start(self.module.start_sec)
-                case Start():
-                    return Start(self.module.start_sec)
-
-        elif self.elemsec is not None and isinstance(query, Element):
-            element_list = []
-            for idx, item in enumerate(self.module.elem_sec):
-                if all(
-                        (query.elemidx is None or query.elemidx == idx,
-                         query.tableidx is None or query.tableidx == item.table,
-                         query.offset is None or query.offset == item.offset[0].args)
-                ):
-                    element_list.append(
-                        Element(idx, tableidx=item.table, offset=item.offset[0].args, funcidx_list=item.init))
-            return element_list
-
-        elif self.codesec is not None and isinstance(query, Code):
-            code_list = []
-            # get import func num
-            import_func_num = 0
-            for import_func in self.module.import_sec:
-                if import_func.desc.func_type is not None:
-                    import_func_num += 1
-            if query.funcidx < import_func_num:
-                raise Exception("Import function!")
-            query.funcidx -= import_func_num
-            for idx, item in enumerate(self.module.code_sec):
-                if query.funcidx is None or query.funcidx == idx:
-                    # locals
-                    locals = []
-                    i = 0
-                    for local in item.locals:
-                        for j in range(i, i + local.n):
-                            locals.append(Local(j, local.type))
-                        i += local.n
-                    # instrs
-                    instrs = self.get_flat_instrs(item.expr)
-                    code_list.append(Code(idx + import_func_num, locals, instrs))
-
-            if len(code_list) != 1:
-                raise Exception("error")
-
-            idx = code_list[0].funcidx
-
-            self.module.code_sec.pop(idx)
-
-        elif self.datasec is not None and isinstance(query, Data):
-            data_list = []
-            for idx, item in enumerate(self.module.data_sec):
-                if all(
-                        (query.dataidx is None or query.dataidx == idx,
-                         query.offset is None or query.offset == item.offset[0].args)
-                ):
-                    # delete
-                    self.module.data_sec.pop(idx)
-            return data_list
-
-        elif self.datacountsec is not None:
-            pass
-        elif self.customsec is not None and isinstance(query, CustomName):
-            name_list = []
-            match query.name_type:
-                # func 0
-                case 0:
-                    for custom in self.module.custom_secs:
-                        if custom.name == "name":
-                            for idx, item in enumerate(custom.name_data.funcNameSubSec):
-                                if all(
-                                        (query.idx is None or query.idx == item.idx,
-                                         query.name is None or query.name == item.name)
-                                ):
-                                    # delete
-                                    custom.name_data.funcNameSubSec.pop(idx)
-                case 1:
-                    for custom in self.module.custom_secs:
-                        if custom.name == "name":
-                            for idx, item in enumerate(custom.name_data.globalNameSubSec):
-                                if all(
-                                        (query.idx is None or query.idx == item.idx,
-                                         query.name is None or query.name == item.name)
-                                ):
-                                    # delete
-                                    custom.name_data.globalNameSubSec.pop(idx)
-                case 2:
-                    for custom in self.module.custom_secs:
-                        if custom.name == "name":
-                            for idx, item in enumerate(custom.name_data.dataNameSubSec):
-                                if all(
-                                        (query.idx is None or query.idx == item.idx,
-                                         query.name is None or query.name == item.name)
-                                ):
-                                    # delete
-                                    custom.name_data.dataNameSubSec.pop(idx)
-                case _:
-                    pass
-            return name_list
-        else:
-            raise Exception("error")
-
-    def update(self, query, new_item):
-
-        if self.typesec is not None and isinstance(query, Type):
-            type_list = []
-            for idx, item in enumerate(self.module.type_sec):
-                param_types, result_types = item.get_signature()
-                if all(
-                        (query.typeidx is None or query.typeidx == idx,
-                         query.arg_types is None or query.arg_types == param_types,
-                         query.ret_types is None or query.ret_types == result_types,)
-                ):
-                    type_list.append(Type(idx, param_types, result_types))
-
-            # update
-            for t in type_list:
-                if new_item.arg_types is not None:
-                    param_types = []
-                    for arg in new_item.arg_types:
-                        match arg:
-                            case "i32":
-                                param_types.append(I32)
-                            case "i64":
-                                param_types.append(I64)
-                            case "f32":
-                                param_types.append(F32)
-                            case "f64":
-                                param_types.append(F64)
-                    self.module.type_sec[t.typeidx].param_types = param_types
-
-                if new_item.ret_types is not None:
-                    result_types = []
-                    for arg in new_item.ret_types:
-                        match arg:
-                            case "i32":
-                                result_types.append(I32)
-                            case "i64":
-                                result_types.append(I64)
-                            case "f32":
-                                result_types.append(F32)
-                            case "f64":
-                                result_types.append(F64)
-                    t.result_types = result_types
-                    self.module.type_sec[t.typeidx].result_types = result_types
-
-        elif self.importsec is not None and isinstance(query, Import):
-
-            import_list = []
-            for idx, item in enumerate(self.module.import_sec):
-                if item.desc.func_type is not None:
-                    if all(
-                            (query.importidx is None or query.importidx == idx,
-                             query.module is None or query.module == item.module,
-                             query.name is None or query.name == item.name,
-                             query.typeidx is None or query.typeidx == item.desc.func_type)
-                    ):
-                        import_list.append(Import(idx, item.module, item.name, item.desc.func_type))
-
-            # update
-            for i in import_list:
-                if new_item.module is not None:
-                    self.module.import_sec[i.importidx].module = new_item.module
-                if new_item.name is not None:
-                    self.module.import_sec[i.importidx].name = new_item.name
-                if new_item.typeidx is not None:
-                    self.module.import_sec[i.importidx].desc.func_type = new_item.typeidx
-
-        elif self.funcsec is not None and isinstance(query, Function):
-            function_list = []
-
-            # get import func num
-            import_func_num = 0
-            for import_func in self.module.import_sec:
-                if import_func.desc.func_type is not None:
-                    import_func_num += 1
-
-            if query.funcidx is not None:
-                query.funcidx -= import_func_num
-
-            for idx, item in enumerate(self.module.func_sec):
-                if all(
-                        (query.funcidx is None or query.funcidx == idx,
-                         query.typeidx is None or query.typeidx == item)
-                ):
-                    function_list.append(Function(idx + import_func_num, item))
-
-            # update
-            for f in function_list:
-                if new_item.typeidx is not None:
-                    self.module.func_sec[f.funcidx - import_func_num] = new_item.typeidx
-
-        elif self.tablesec is not None and isinstance(query, Table):
-            # 如何表示无穷
-            table_list = []
-            for idx, item in enumerate(self.module.table_sec):
-                if all(
-                        (query.min is None or query.min == item.limits.min,
-                         query.max is None or query.max == item.limits.max)
-                ):
-                    table_list.append({
-                        "idx": idx,
-                        "table": Table(item.limits.min, item.limits.max)
-                    })
-
-            # update
-            for t in table_list:
-                if new_item.min is not None:
-                    self.module.table_sec[t["idx"]].limits.min = new_item.min
-                if new_item.max is not None:
-                    self.module.table_sec[t["idx"]].limits.max = new_item.max
-
-        elif self.memsec is not None and isinstance(query, Memory):
-
-            # 如何表示无穷
-            mem_list = []
-            for idx, item in enumerate(self.module.mem_sec):
-                if all(
-                        (query.min is None or query.min == item.min,
-                         query.max is None or query.max == item.max)
-                ):
-                    mem_list.append({
-                        "idx": idx,
-                        "memory": Memory(item.min, item.max)
-                    })
-
-            # update
-            for m in mem_list:
-                if new_item.min is not None:
-                    self.module.mem_sec[m["idx"]].min = new_item.min
-                if new_item.max is not None:
-                    self.module.mem_sec[m["idx"]].max = new_item.max
-
-        elif self.globalsec is not None and isinstance(query, Global):
-            global_list = []
-            for idx, item in enumerate(self.module.global_sec):
-                if all(
-                        (query.globalidx is None or query.globalidx == idx,
-                         query.valtype is None or query.valtype == item.type.val_type,
-                         query.mut is None or query.mut == item.type.mut,
-                         query.val is None or query.val == item.init[0].args)
-                ):
-                    global_list.append(Global(idx, item.type.val_type, item.type.mut, item.init[0].args))
-
-            for g in global_list:
-                if new_item.valtype is not None:
-                    self.module.global_sec[g.globalidx].type.val_type = new_item.valtype
-                if new_item.mut is not None:
-                    self.module.global_sec[g.globalidx].type.mut = new_item.mut
-                if new_item.val is not None:
-                    if self.module.global_sec[g.globalidx].type.val_type == I32:
-                        init_value_instr = Instruction(I32Const, new_item.val)
-                    elif self.module.global_sec[g.globalidx].type.val_type == I64:
-                        init_value_instr = Instruction(I64Const, new_item.val)
-                    elif self.module.global_sec[g.globalidx].type.val_type == F32:
-                        init_value_instr = Instruction(F32Const, new_item.val)
-                    elif self.module.global_sec[g.globalidx].type.val_type == F64:
-                        init_value_instr = Instruction(F64Const, new_item.val)
-                    self.module.global_sec[g.globalidx].init[0] = init_value_instr
-
-        elif self.exportsec is not None and isinstance(query, Export):
-            export_list = []
-            for idx, item in enumerate(self.module.export_sec):
-                if all(
-                        (query.exportidx is None or query.exportidx == idx,
-                         query.name is None or query.name == item.name,
-                         # The tag of function is 0
-                         query.funcidx is None or query.funcidx == item.desc.idx)
-                ) and item.desc.tag == 0:
-                    export_list.append(Export(idx, name=item.name, funcidx=item.desc.idx))
-
-            # update
-            for e in export_list:
-                if new_item.name is not None:
-                    self.module.export_sec[e.exportidx].name = new_item.name
-                if new_item.funcidx is not None:
-                    self.module.export_sec[e.exportidx].desc.idx = new_item.funcidx
-
-        # elif self.startsec is not None and isinstance(query, Start):
-        #     match query:
-        #         case Start(funcidx=funcidx):
-        #             return Start(self.module.start_sec)
-        #         case Start():
-        #             return Start(self.module.start_sec)
-
-        elif self.elemsec is not None and isinstance(query, Element):
-            element_list = []
-            for idx, item in enumerate(self.module.elem_sec):
-                if all(
-                        (query.elemidx is None or query.elemidx == idx,
-                         query.tableidx is None or query.tableidx == item.table,
-                         query.offset is None or query.offset == item.offset[0].args)
-                ):
-                    element_list.append(
-                        Element(idx, tableidx=item.table, offset=item.offset[0].args, funcidx_list=item.init))
-
-            # update
-            for e in element_list:
-                if new_item.tableidx is not None:
-                    self.module.elem_sec[e.elemidx].table = new_item.tableidx
-                if new_item.offset is not None:
-                    self.module.elem_sec[e.elemidx].offset = [Instruction(I32Const, new_item.offset)]
-                if new_item.funcidx_list is not None:
-                    self.module.elem_sec[e.elemidx].init = new_item.funcidx_list
-
-                indirect_func_list = e.funcidx_list
-                self.indices_fixer.fix_table_limits(self.module.table_sec, len(indirect_func_list) + 1)
-
-        elif self.codesec is not None and isinstance(query, Code):
-            code_list = []
-            # get import func num
-            import_func_num = 0
-            for import_func in self.module.import_sec:
-                if import_func.desc.func_type is not None:
-                    import_func_num += 1
-            if query.funcidx < import_func_num:
-                raise Exception("Import function!")
-            query.funcidx -= import_func_num
-            for idx, item in enumerate(self.module.code_sec):
-                if query.funcidx is None or query.funcidx == idx:
-                    # locals
-                    locals = []
-                    i = 0
-                    for local in item.locals:
-                        for j in range(i, i + local.n):
-                            locals.append(Local(j, local.type))
-                        i += local.n
-                    # instrs
-                    instrs = self.get_flat_instrs(item.expr)
-                    code_list.append(Code(idx + import_func_num, locals, instrs))
-
-            # update
-            for c in code_list:
-                if new_item.local_vec is not None:
-                    self.module.code_sec[c.funcidx - import_func_num].locals = new_item.convert_local_vec()
-                if new_item.instr_list is not None:
-                    self.module.code_sec[c.funcidx - import_func_num].expr = self.get_fold_instrs(new_item.instr_list)
-
-
-
-        elif self.datasec is not None and isinstance(query, Data):
-            data_list = []
-            for idx, item in enumerate(self.module.data_sec):
-                if all(
-                        (query.dataidx is None or query.dataidx == idx,
-                         query.offset is None or query.offset == item.offset[0].args)
-                ):
-                    data_list.append(Data(idx, item.offset[0].args, item.init))
-
-            # update
-            for d in data_list:
-                if new_item.offset is not None:
-                    self.module.data_sec[d.dataidx].offset = [Instruction(I32Const, new_item.offset)]
-                if new_item.init_data is not None:
-                    self.module.data_sec[d.dataidx].init = new_item.init_data
-
-        elif self.datacountsec is not None:
-            pass
-        elif self.customsec is not None and isinstance(query, CustomName):
-            name_list = []
-            match query.name_type:
-                # func 0
-                case 0:
-                    for custom in self.module.custom_secs:
-                        if custom.name == "name":
-                            for idx, item in enumerate(custom.name_data.funcNameSubSec):
-                                if all(
-                                        (query.idx is None or query.idx == item.idx,
-                                         query.name is None or query.name == item.name)
-                                ):
-                                    name_list.append(CustomName(FunctionName, item.idx, item.name))
-                case 1:
-                    for custom in self.module.custom_secs:
-                        if custom.name == "name":
-                            for idx, item in enumerate(custom.name_data.globalNameSubSec):
-                                if all(
-                                        (query.idx is None or query.idx == item.idx,
-                                         query.name is None or query.name == item.name)
-                                ):
-                                    name_list.append(CustomName(GlobalName, item.idx, item.name))
-                case 2:
-                    for custom in self.module.custom_secs:
-                        if custom.name == "name":
-                            for idx, item in enumerate(custom.name_data.dataNameSubSec):
-                                if all(
-                                        (query.idx is None or query.idx == item.idx,
-                                         query.name is None or query.name == item.name)
-                                ):
-                                    name_list.append(CustomName(DataName, item.idx, item.name))
-                case _:
-                    pass
-
-            # update
-            name_section_idx = None
-            for i, custom_sec in enumerate(self.module.custom_secs):
-                if custom_sec.name == "name":
-                    name_section_idx = i
-
-            for n in name_list:
-                if new_item.name is not None:
-                    match n.name_type:
-                        case 0:
-                            self.module.custom_secs[name_section_idx].name_data.funcNameSubSec[
-                                n.idx].name = new_item.name
-                        case 1:
-                            self.module.custom_secs[name_section_idx].name_data.globalNameSubSec[
-                                n.idx].name = new_item.name
-                        case 2:
-                            self.module.custom_secs[name_section_idx].name_data.dataNameSubSec[
-                                n.idx].name = new_item.name
-                        case _:
-                            pass
-
-        else:
-            raise Exception("error")
-
-    def emit_binary(self, path: str):
-        ModifyBinary(self.module, self.module.path).emit_binary(path)
-
-    # 这里的end没有算作指令
-    def get_flat_instrs(self, instrs):
-        ret_instrs = []
-        for _, i in enumerate(instrs):
-            if i.opcode in [Block, Loop]:
-                ret_instrs.append(i)
-                args = i.args
-                ret_instrs.extend(self.get_flat_instrs(args.instrs))
-                ret_instrs.append(Instruction(End_))
-            elif i.opcode == If:
-                ret_instrs.append(i)
-                args = i.args
-                ret_instrs.extend(self.get_flat_instrs(args.instrs1))
-                ret_instrs.append(Instruction(Else_))
-                ret_instrs.extend(self.get_flat_instrs(args.instrs2))
-                ret_instrs.append(Instruction(End_))
-            else:
-                ret_instrs.append(i)
-        return ret_instrs
-
-    def get_fold_instrs(self, instrs):
-        ret_instrs = []
-        i = 0
-        while i < len(instrs):
-            if instrs[i].opcode in [Block, Loop]:
-                j = i
-                args_instrs_length = self.get_flat_Block_length(instrs[i:]) - 2
-                instrs[i].args.instrs = self.get_fold_instrs(instrs[i + 1: i + 1 + args_instrs_length])
-                i = i + args_instrs_length + 2
-                ret_instrs.append(instrs[j])
-            elif instrs[i].opcode == If:
-                j = i
-                else_offset, length = self.get_flat_If_length(instrs[i:]) - 2
-                instrs[j].args.instrs1 = self.get_fold_instrs(instrs[i + 1, i + else_offset])
-                i = i + else_offset
-                instrs[j].args.instrs2 = self.get_fold_instrs(instrs[i + 1, i + length - 1])
-                i = j + length
-                ret_instrs.append(instrs[j])
-            else:
-                ret_instrs.append(instrs[i])
-                i += 1
-        return ret_instrs
-
-    def get_flat_Block_length(self, instrs):
-
-        if instrs[0].opcode in [Block, Loop]:
-            instr_queue = [instrs[0]]
-            i = 1
-            while i < len(instrs):
-                if instrs[i].opcode in [Block, Loop]:
-                    instr_queue.append(instrs[i])
-                    i += 1
-                elif instrs[i].opcode in [If, Else_]:
-                    instr_queue.append(instrs[i])
-                    i += 1
-                elif instrs[i].opcode == End_:
-                    instr_queue.append(instrs[i])
-                    i += 1
-                    if instr_queue[-2].opcode == Else_:
-                        instr_queue = instr_queue[0: -3]
-                    elif instr_queue[-2].opcode in [Block, Loop]:
-                        instr_queue = instr_queue[0: -2]
-                    if instr_queue == []:
-                        length = i
-                        return length
-                else:
-                    i += 1
-        else:
-            raise Exception("error")
-
-    def get_flat_If_length(self, instrs):
-
-        if instrs[0].opcode in [If]:
-            instr_queue = [{
-                        "offset": 0,
-                        "instr": instrs[0]
-                    }]
-            i = 1
-            while i < len(instrs):
-                if instrs[i].opcode in [Block, Loop]:
-                    instr_queue.append({
-                        "offset": i,
-                        "instr": instrs[i]
-                    })
-                    i += 1
-                elif instrs[i].opcode in [If, Else_]:
-                    instr_queue.append({
-                        "offset": i,
-                        "instr": instrs[i]
-                    })
-                    i += 1
-                elif instrs[i].opcode == End_:
-                    instr_queue.append({
-                        "offset": i,
-                        "instr": instrs[i]
-                    })
-                    i += 1
-                    if instr_queue[-2].opcode == Else_ and len(instr_queue) != 3:
-                        instr_queue = instr_queue[0: -3]
-                    elif instr_queue[-2].opcode in [Block, Loop]:
-                        instr_queue = instr_queue[0: -2]
-                    elif instr_queue[-2].opcode == Else_ and len(instr_queue) == 3:
-                        else_offset = instr_queue[1]["offset"]
-                        length = i
-                        return else_offset, length
-                else:
-                    i += 1
-        else:
-            raise Exception("error")
-
-    # def _get_instrs_instr(self, instrs, offset=None, current_offset=-1, instr=None, ret_instrs=[]):
-    #     if offset is not None:
-    #         for _, i in enumerate(instrs):
-    #             current_offset += 1
-    #             if i.opcode in [Block, Loop]:
-    #                 if offset == current_offset:
-    #                     return RetInstrs(_, i, instrs)
-    #                 args = i.args
-    #                 return self._get_instrs_instr(args.instrs, offset=offset, current_offset=current_offset, instr=instr)
-    #                 # 将end也算一个指令
-    #                 current_offset += 1
-    #                 if offset == current_offset:
-    #                     raise Exception("end can not be get")
-    #             elif i.opcode == If:
-    #                 if offset == current_offset:
-    #                     return RetInstrs(_, i, instrs)
-    #                 args = i.args
-    #                 return self._get_instrs_instr(args.instrs1, offset=offset, current_offset=current_offset,
-    #                                               instr=instr)
-    #                 # 将else也算一个指令
-    #                 current_offset += 1
-    #                 if offset == current_offset:
-    #                     raise Exception("else can not be get")
-    #                 return self._get_instrs_instr(args.instrs2, offset=offset, current_offset=current_offset,
-    #                                               instr=instr)
-    #                 # 将end也算一个指令
-    #                 current_offset += 1
-    #                 if offset == current_offset:
-    #                     raise Exception("end can not be get")
-    #             else:
-    #                 if current_offset == offset:
-    #                     return RetInstrs(_, i, instrs)
-    #     elif instr is not None and instr.args is None:
-    #         ret_instrs = []
-    #         for _, i in enumerate(instrs):
-    #             if i.opcode in [Block, Loop]:
-    #                 if i.opcode == instr.opcode:
-    #                     ret_instrs.append(RetInstrs(_, i, instrs))
-    #                 args = i.args
-    #                 ret_instrs.extend(
-    #                     self._get_instrs_instr(args.instrs, offset=offset, current_offset=current_offset, instr=instr))
-    #             elif i.opcode == If:
-    #                 if i.opcode == instr.opcode:
-    #                     ret_instrs.append(RetInstrs(_, i, instrs))
-    #                 args = i.args
-    #                 ret_instrs.extend(
-    #                     self._get_instrs_instr(args.instrs1, offset=offset, current_offset=current_offset, instr=instr))
-    #                 ret_instrs.extend(
-    #                     self._get_instrs_instr(args.instrs2, offset=offset, current_offset=current_offset, instr=instr))
-    #             else:
-    #                 if i.opcode == instr.opcode:
-    #                     ret_instrs.append(RetInstrs(_, i, instrs))
-    #         return ret_instrs
-    #     elif instr is not None:
-    #         ret_instrs = []
-    #         for _, i in enumerate(instrs):
-    #             if i.opcode in [Block, Loop]:
-    #                 if i.opcode == instr.opcode and i.args == instr.args:
-    #                     ret_instrs.append(RetInstrs(_, i, instrs))
-    #                 args = i.args
-    #                 ret_instrs.extend(
-    #                     self._get_instrs_instr(args.instrs, offset=offset, current_offset=current_offset, instr=instr))
-    #             elif i.opcode == If:
-    #                 if i.opcode == instr.opcode and i.args == instr.args:
-    #                     ret_instrs.append(RetInstrs(_, i, instrs))
-    #                 args = i.args
-    #                 ret_instrs.extend(
-    #                     self._get_instrs_instr(args.instrs1, offset=offset, current_offset=current_offset, instr=instr))
-    #                 ret_instrs.extend(
-    #                     self._get_instrs_instr(args.instrs2, offset=offset, current_offset=current_offset, instr=instr))
-    #             else:
-    #                 if i.opcode == instr.opcode and i.args == instr.args:
-    #                     ret_instrs.append(RetInstrs(_, i, instrs))
-    #         return ret_instrs
+from BREWasm.parser import module
+from BREWasm.rewriter.modify_binary import ModifyBinary
+from BREWasm.rewriter.defination import *
+from BREWasm.rewriter.indices_fixer import *
+from BREWasm.parser.instruction import Instruction
+from BREWasm.rewriter.indices_fixer import IndicesFixer
+
+
+# class RetInstrs:
+#     def __init__(self, index, instr, instrs):
+#         self.index = index
+#         self.instr = instr
+#         self.instrs = instrs
+
+
+class SectionRewriter:
+
+    def __init__(self, module, **section):
+        """
+
+        Args:
+            module:
+            **section:
+        """
+
+        allowed_params = ['typesec', 'importsec', 'funcsec', 'tablesec', 'memsec',
+                          'globalsec', 'exportsec', 'startsec', 'elemsec', 'codesec',
+                          'datasec', 'datacountsec', 'customsec']
+
+        if len(section) != 1:
+            raise ValueError("Only one parameter should be provided")
+
+        param_name = next(iter(section.keys()))
+        if param_name not in allowed_params:
+            raise ValueError("Invalid parameter")
+
+        self.module = module
+        self.typesec = None
+        self.importsec = None
+        self.funcsec = None
+        self.tablesec = None
+        self.memsec = None
+        self.globalsec = None
+        self.exportsec = None
+        self.startsec = None
+        self.elemsec = None
+        self.codesec = None
+        self.datasec = None
+        self.datacountsec = None
+        self.customsec = None
+        self.indices_fixer = IndicesFixer(module)
+
+        setattr(self, param_name, section[param_name])
+
+    def select(self, query):
+        if self.typesec is not None and isinstance(query, Type):
+            type_list = []
+            for idx, item in enumerate(self.module.type_sec):
+                param_types, result_types = item.get_signature()
+                if all(
+                        (query.typeidx is None or query.typeidx == idx,
+                         query.arg_types is None or query.arg_types == param_types,
+                         query.ret_types is None or query.ret_types == result_types,)
+                ):
+                    type_list.append(Type(idx, param_types, result_types))
+            return type_list
+
+        elif self.importsec is not None and isinstance(query, Import):
+
+            import_list = []
+            for idx, item in enumerate(self.module.import_sec):
+                if item.desc.func_type is not None:
+                    if all(
+                            (query.importidx is None or query.importidx == idx,
+                             query.module is None or query.module == item.module,
+                             query.name is None or query.name == item.name,
+                             query.typeidx is None or query.typeidx == item.desc.func_type)
+                    ):
+                        import_list.append(Import(idx, item.module, item.name, item.desc.func_type))
+            return import_list
+
+        elif self.funcsec is not None and isinstance(query, Function):
+            function_list = []
+
+            # get import func num
+            import_func_num = 0
+            for import_func in self.module.import_sec:
+                if import_func.desc.func_type is not None:
+                    import_func_num += 1
+
+            if query.funcidx is not None:
+                query.funcidx -= import_func_num
+
+            for idx, item in enumerate(self.module.func_sec):
+                if all(
+                        (query.funcidx is None or query.funcidx == idx,
+                         query.typeidx is None or query.typeidx == item)
+                ):
+                    function_list.append(Function(idx + import_func_num, item))
+            return function_list
+
+        elif self.tablesec is not None and isinstance(query, Table):
+            # 如何表示无穷
+            table_list = []
+            for idx, item in enumerate(self.module.table_sec):
+                if all(
+                        (query.min is None or query.min == item.limits.min,
+                         query.max is None or query.max == item.limits.max)
+                ):
+                    table_list.append(Table(item.limits.min, item.limits.max))
+            return table_list
+
+        elif self.memsec is not None and isinstance(query, Memory):
+
+            # 如何表示无穷
+            mem_list = []
+            for idx, item in enumerate(self.module.mem_sec):
+                if all(
+                        (query.min is None or query.min == item.min,
+                         query.max is None or query.max == item.max)
+                ):
+                    mem_list.append(Memory(item.min, item.max))
+            return mem_list
+
+        elif self.globalsec is not None and isinstance(query, Global):
+            global_list = []
+            for idx, item in enumerate(self.module.global_sec):
+                if all(
+                        (query.globalidx is None or query.globalidx == idx,
+                         query.valtype is None or query.valtype == item.type.val_type,
+                         query.mut is None or query.mut == item.type.mut,
+                         query.val is None or query.val == item.init[0].args)
+                ):
+                    global_list.append(Global(idx, item.type.val_type, item.type.mut, item.init[0].args))
+            return global_list
+
+        elif self.exportsec is not None and isinstance(query, Export):
+            export_list = []
+            for idx, item in enumerate(self.module.export_sec):
+                if all(
+                        (query.exportidx is None or query.exportidx == idx,
+                         query.name is None or query.name == item.name,
+                         # The tag of function is 0
+                         query.funcidx is None or query.funcidx == item.desc.idx)
+                ) and item.desc.tag == 0:
+                    export_list.append(Export(idx, name=item.name, funcidx=item.desc.idx))
+            return export_list
+
+        elif self.startsec is not None and isinstance(query, Start):
+            match query:
+                case Start(funcidx=funcidx):
+                    return Start(self.module.start_sec)
+                case Start():
+                    return Start(self.module.start_sec)
+
+        elif self.elemsec is not None and isinstance(query, Element):
+            element_list = []
+            for idx, item in enumerate(self.module.elem_sec):
+                if all(
+                        (query.elemidx is None or query.elemidx == idx,
+                         query.tableidx is None or query.tableidx == item.table,
+                         query.offset is None or query.offset == item.offset[0].args)
+                ):
+                    element_list.append(
+                        Element(idx, tableidx=item.table, offset=item.offset[0].args, funcidx_list=item.init))
+            return element_list
+
+        elif self.codesec is not None and isinstance(query, Code):
+            code_list = []
+            # get import func num
+            import_func_num = 0
+            for import_func in self.module.import_sec:
+                if import_func.desc.func_type is not None:
+                    import_func_num += 1
+            if query.funcidx < import_func_num:
+                raise Exception("Import function!")
+            query.funcidx -= import_func_num
+            for idx, item in enumerate(self.module.code_sec):
+                if query.funcidx is None or query.funcidx == idx:
+                    # locals
+                    locals = []
+                    i = 0
+                    for local in item.locals:
+                        for j in range(i, i + local.n):
+                            locals.append(Local(j, local.type))
+                        i += local.n
+                    # instrs
+                    instrs = self.get_flat_instrs(item.expr)
+                    code_list.append(Code(idx + import_func_num, locals, instrs))
+            return code_list
+
+        elif self.datasec is not None and isinstance(query, Data):
+            data_list = []
+            for idx, item in enumerate(self.module.data_sec):
+                if all(
+                        (query.dataidx is None or query.dataidx == idx,
+                         query.offset is None or query.offset == item.offset[0].args)
+                ):
+                    data_list.append(Data(idx, item.offset[0].args, item.init))
+            return data_list
+
+        elif self.datacountsec is not None:
+            pass
+        elif self.customsec is not None and isinstance(query, CustomName):
+            name_list = []
+            match query.name_type:
+                # func 0
+                case 0:
+                    for custom in self.module.custom_secs:
+                        if custom.name == "name":
+                            for idx, item in enumerate(custom.name_data.funcNameSubSec):
+                                if all(
+                                        (query.idx is None or query.idx == item.idx,
+                                         query.name is None or query.name == item.name)
+                                ):
+                                    name_list.append(CustomName(FunctionName, item.idx, item.name))
+                case 1:
+                    for custom in self.module.custom_secs:
+                        if custom.name == "name":
+                            for idx, item in enumerate(custom.name_data.globalNameSubSec):
+                                if all(
+                                        (query.idx is None or query.idx == item.idx,
+                                         query.name is None or query.name == item.name)
+                                ):
+                                    name_list.append(CustomName(GlobalName, item.idx, item.name))
+                case 2:
+                    for custom in self.module.custom_secs:
+                        if custom.name == "name":
+                            for idx, item in enumerate(custom.name_data.dataNameSubSec):
+                                if all(
+                                        (query.idx is None or query.idx == item.idx,
+                                         query.name is None or query.name == item.name)
+                                ):
+                                    name_list.append(CustomName(DataName, item.idx, item.name))
+                case _:
+                    pass
+            return name_list
+        else:
+            raise Exception("error")
+
+    def insert(self, query, inserted_item):
+
+        if self.typesec is not None and isinstance(inserted_item, Type):
+            if query is None:
+                # append
+                self.module.type_sec.append(inserted_item.convert())
+            elif isinstance(query, Type):
+                type_list = []
+                for idx, item in enumerate(self.module.type_sec):
+                    param_types, result_types = item.get_signature()
+                    if all(
+                            (query.typeidx is None or query.typeidx == idx,
+                             query.arg_types is None or query.arg_types == param_types,
+                             query.ret_types is None or query.ret_types == result_types,)
+                    ):
+                        type_list.append(Type(idx, param_types, result_types))
+                if len(type_list) != 1:
+                    raise Exception("error")
+
+                idx = type_list[0].typeidx
+                # insert
+                self.module.type_sec.insert(idx, inserted_item.convert())
+
+                # fix
+                self.indices_fixer.fix_func_functypeidx(self.module.func_sec, idx)
+                self.indices_fixer.fix_import_func_functypeidx(self.module.import_sec, idx)
+
+        elif self.importsec is not None and isinstance(inserted_item, Import):
+            if query is None:
+                self.module.import_sec.append(module.Import(inserted_item.module, inserted_item.name,
+                                                            module.ImportDesc(tag=0,
+                                                                              func_type=inserted_item.typeidx)))
+            elif isinstance(query, Import):
+                import_list = []
+                for idx, item in enumerate(self.module.import_sec):
+                    if item.desc.func_type is not None:
+                        if all(
+                                (query.importidx is None or query.importidx == idx,
+                                 query.module is None or query.module == item.module,
+                                 query.name is None or query.name == item.name,
+                                 query.typeidx is None or query.typeidx == item.desc.func_type)
+                        ):
+                            import_list.append(Import(idx, item.module, item.name, item.desc.func_type))
+
+                if len(import_list) != 1:
+                    raise Exception("error")
+
+                idx = import_list[0].importidx
+
+                self.module.import_sec.insert(idx, module.Import(inserted_item.module, inserted_item.name,
+                                                                 module.ImportDesc(tag=0,
+                                                                                   func_type=inserted_item.typeidx)))
+
+            # fix
+            import_func_id = None
+            for i, import_item in enumerate([i for i in self.module.import_sec if i.desc.func_type is not None]):
+                if import_item.module == inserted_item.module and import_item.name == inserted_item.name:
+                    import_func_id = i
+            for _, code in enumerate(self.module.code_sec):
+                self.indices_fixer.fix_call_instructions(code.expr, import_func_id)
+            self.indices_fixer.fix_elem_funcidx(self.module.elem_sec, import_func_id)
+            self.indices_fixer.fix_export_funcidx(self.module.export_sec, import_func_id)
+
+        elif self.funcsec is not None and isinstance(inserted_item, Function):
+            if query is None:
+                self.module.func_sec.append(inserted_item.typeidx)
+            elif isinstance(query, Function):
+                function_list = []
+
+                # get import func num
+                import_func_num = 0
+                for import_func in self.module.import_sec:
+                    if import_func.desc.func_type is not None:
+                        import_func_num += 1
+
+                if query.funcidx is not None:
+                    query.funcidx -= import_func_num
+
+                for idx, item in enumerate(self.module.func_sec):
+                    if all(
+                            (query.funcidx is None or query.funcidx == idx,
+                             query.typeidx is None or query.typeidx == item)
+                    ):
+                        function_list.append(Function(idx + import_func_num, item))
+
+                if len(function_list) != 1:
+                    raise Exception("error")
+
+                idx = function_list[0].funcidx
+                # insert
+                self.module.func_sec.insert(idx - import_func_num, inserted_item.typeidx)
+
+                # fix
+                self.indices_fixer.fix_export_funcidx(self.module.export_sec, idx)
+                self.indices_fixer.fix_elem_funcidx(self.module.elem_sec, idx)
+                for _, code in enumerate(self.module.code_sec):
+                    self.indices_fixer.fix_call_instructions(code.expr, idx)
+
+
+        # table 和 memory 段暂时不能修改
+        # elif self.tablesec is not None and isinstance(query, Table):
+        #     # 如何表示无穷
+        #     table_list = []
+        #     for idx, item in enumerate(self.module.table_sec):
+        #         if all(
+        #                 (query.min is None or query.min == item.limits.min,
+        #                  query.max is None or query.max == item.limits.max)
+        #         ):
+        #             table_list.append(Table(item.limits.min, item.limits.max))
+        #
+        #     if len(table_list) != 1:
+        #         raise Exception("error")
+        #
+        #     idx = table_list[0]
+        #
+        #     return table_list
+        #
+        # elif self.memsec is not None and isinstance(query, Memory):
+        #
+        #     # 如何表示无穷
+        #     mem_list = []
+        #     for idx, item in enumerate(self.module.mem_sec):
+        #         if all(
+        #                 (query.min is None or query.min == item.min,
+        #                  query.max is None or query.max == item.max)
+        #         ):
+        #             mem_list.append(Memory(item.min, item.max))
+        #     return mem_list
+
+        elif self.globalsec is not None and isinstance(inserted_item, Global):
+            if inserted_item.valtype == I32:
+                init_value_instr = Instruction(I32Const, inserted_item.val)
+            elif inserted_item.valtype == I64:
+                init_value_instr = Instruction(I64Const, inserted_item.val)
+            elif inserted_item.valtype == F32:
+                init_value_instr = Instruction(F32Const, inserted_item.val)
+            elif inserted_item.valtype == F64:
+                init_value_instr = Instruction(F64Const, inserted_item.val)
+            else:
+                raise Exception("global type error!")
+
+            # The default mutable attribute is 0
+            if inserted_item.mut is None:
+                inserted_item.mut = 0
+
+            if query is None:
+                self.module.global_sec.append(module.Global(GlobalType(inserted_item.valtype, inserted_item.mut),
+                                                            [init_value_instr]))
+            elif isinstance(query, Global):
+                global_list = []
+                for idx, item in enumerate(self.module.global_sec):
+                    if all(
+                            (query.globalidx is None or query.globalidx == idx,
+                             query.valtype is None or query.valtype == item.type.val_type,
+                             query.mut is None or query.mut == item.type.mut,
+                             query.val is None or query.val == item.init[0].args)
+                    ):
+                        global_list.append(Global(idx, item.type.val_type, item.type.mut, item.init[0].args))
+
+                if len(global_list) != 1:
+                    raise Exception("error")
+                idx = global_list[0].globalidx
+                # insert
+                self.module.global_sec.insert(idx, module.Global(GlobalType(inserted_item.valtype, inserted_item.mut),
+                                                                 [init_value_instr]))
+
+                # fix
+                self.indices_fixer.fix_export_globalidx(self.module.export_sec, idx)
+                for code in self.module.code_sec:
+                    self.indices_fixer.fix_global_instructions(code.expr, idx)
+
+        elif self.exportsec is not None and isinstance(inserted_item, Export):
+            if query is None:
+                self.module.export_sec.append(
+                    module.Export(inserted_item.name, module.ExportDesc(0, inserted_item.funcidx)))
+            elif isinstance(query, Export):
+                export_list = []
+                for idx, item in enumerate(self.module.export_sec):
+                    if all(
+                            (query.exportidx is None or query.exportidx == idx,
+                             query.name is None or query.name == item.name,
+                             # The tag of function is 0
+                             query.funcidx is None or query.funcidx == item.desc.idx)
+                    ):
+                        export_list.append(Export(idx, name=item.name, funcidx=item.desc.idx))
+
+                if len(export_list) != 1:
+                    raise Exception("error")
+
+                idx = export_list[0].exportidx
+                self.module.export_sec.insert(idx, module.Export(inserted_item.name,
+                                                                 module.ExportDesc(0, inserted_item.funcidx)))
+
+        elif self.startsec is not None and isinstance(inserted_item, Start):
+            match query:
+                case Start(funcidx=funcidx):
+                    return Start(self.module.start_sec)
+                case Start():
+                    return Start(self.module.start_sec)
+
+        elif self.elemsec is not None and isinstance(inserted_item, Element):
+            element_list = []
+            for idx, item in enumerate(self.module.elem_sec):
+                if all(
+                        (query.elemidx is None or query.elemidx == idx,
+                         query.tableidx is None or query.tableidx == item.table,
+                         query.offset is None or query.offset == item.offset[0].args)
+                ):
+                    element_list.append(
+                        Element(idx, tableidx=item.table, offset=item.offset[0].args, funcidx_list=item.init))
+            return element_list
+
+        elif self.codesec is not None and isinstance(inserted_item, Code):
+            locals = inserted_item.convert_local_vec()
+            fold_instrs = self.get_fold_instrs(inserted_item.instr_list)
+
+            if query is None:
+                self.module.code_sec.append(module.Code(locals, fold_instrs))
+            elif isinstance(query, Code):
+
+                code_list = []
+                # get import func num
+                import_func_num = 0
+                for import_func in self.module.import_sec:
+                    if import_func.desc.func_type is not None:
+                        import_func_num += 1
+                if query.funcidx < import_func_num:
+                    raise Exception("Import function!")
+                query.funcidx -= import_func_num
+                for idx, item in enumerate(self.module.code_sec):
+                    if query.funcidx is None or query.funcidx == idx:
+                        # locals
+                        local_vec = []
+                        i = 0
+                        for local in item.locals:
+                            for j in range(i, i + local.n):
+                                local_vec.append(Local(j, local.type))
+                            i += local.n
+                        # instrs
+                        instrs = self.get_flat_instrs(item.expr)
+                        code_list.append(Code(idx + import_func_num, local_vec, instrs))
+
+                if len(code_list) != 1:
+                    raise Exception("error")
+
+                idx = code_list[0].funcidx - import_func_num
+
+                self.module.code_sec.insert(idx, module.Code(locals, fold_instrs))
+
+        elif self.datasec is not None and isinstance(inserted_item, Data):
+            data_list = []
+            for idx, item in enumerate(self.module.data_sec):
+                if all(
+                        (query.dataidx is None or query.dataidx == idx,
+                         query.offset is None or query.offset == item.offset[0].args)
+                ):
+                    data_list.append(Data(idx, item.offset[0].args, item.init))
+            return data_list
+
+        elif self.datacountsec is not None:
+            pass
+        elif self.customsec is not None and isinstance(inserted_item, CustomName):
+            name_list = []
+            match query.name_type:
+                # func 0
+                case 0:
+                    for custom in self.module.custom_secs:
+                        if custom.name == "name":
+                            for idx, item in enumerate(custom.name_data.funcNameSubSec):
+                                if all(
+                                        (query.idx is None or query.idx == item.idx,
+                                         query.name is None or query.name == item.name)
+                                ):
+                                    name_list.append(CustomName(FunctionName, item.idx, item.name))
+                case 1:
+                    for custom in self.module.custom_secs:
+                        if custom.name == "name":
+                            for idx, item in enumerate(custom.name_data.globalNameSubSec):
+                                if all(
+                                        (query.idx is None or query.idx == item.idx,
+                                         query.name is None or query.name == item.name)
+                                ):
+                                    name_list.append(CustomName(GlobalName, item.idx, item.name))
+                case 2:
+                    for custom in self.module.custom_secs:
+                        if custom.name == "name":
+                            for idx, item in enumerate(custom.name_data.dataNameSubSec):
+                                if all(
+                                        (query.idx is None or query.idx == item.idx,
+                                         query.name is None or query.name == item.name)
+                                ):
+                                    name_list.append(CustomName(DataName, item.idx, item.name))
+                case _:
+                    pass
+            return name_list
+        else:
+            raise Exception("error")
+
+    def delete(self, query):
+
+        if self.typesec is not None and isinstance(query, Type):
+            type_list = []
+            for idx, item in enumerate(self.module.type_sec):
+                param_types, result_types = item.get_signature()
+                if all(
+                        (query.typeidx is None or query.typeidx == idx,
+                         query.arg_types is None or query.arg_types == param_types,
+                         query.ret_types is None or query.ret_types == result_types,)
+                ):
+                    type_list.append(Type(idx, param_types, result_types))
+            if len(type_list) != 1:
+                raise Exception("error")
+
+            idx = type_list[0].typeidx
+            # delete
+            self.module.type_sec.pop(idx)
+
+            # fix
+            self.indices_fixer.fix_func_functypeidx(self.module.func_sec, idx, type=Delete)
+            self.indices_fixer.fix_import_func_functypeidx(self.module.import_sec, idx, type=Delete)
+
+        elif self.importsec is not None and isinstance(query, Import):
+
+            import_list = []
+            for idx, item in enumerate(self.module.import_sec):
+                if item.desc.func_type is not None:
+                    if all(
+                            (query.importidx is None or query.importidx == idx,
+                             query.module is None or query.module == item.module,
+                             query.name is None or query.name == item.name,
+                             query.typeidx is None or query.typeidx == item.desc.func_type)
+                    ):
+                        import_list.append(Import(idx, item.module, item.name, item.desc.func_type))
+
+            if len(import_list) != 1:
+                raise Exception("error")
+
+            idx = import_list[0].importidx
+
+            self.module.import_sec.pop(idx)
+
+            # fix
+            import_func_id = None
+            for i, import_item in enumerate([i for i in self.module.import_sec if i.desc.func_type is not None]):
+                if import_item.module == item.module and import_item.name == item.name:
+                    import_func_id = i
+            for _, code in enumerate(self.module.code_sec):
+                self.indices_fixer.fix_call_instructions(code.expr, import_func_id, type=Delete)
+            self.indices_fixer.fix_elem_funcidx(self.module.elem_sec, import_func_id, type=Delete)
+            self.indices_fixer.fix_export_funcidx(self.module.export_sec, import_func_id, type=Delete)
+
+        elif self.funcsec is not None and isinstance(query, Function):
+            function_list = []
+
+            # get import func num
+            import_func_num = 0
+            for import_func in self.module.import_sec:
+                if import_func.desc.func_type is not None:
+                    import_func_num += 1
+
+            if query.funcidx is not None:
+                query.funcidx -= import_func_num
+
+            for idx, item in enumerate(self.module.func_sec):
+                if all(
+                        (query.funcidx is None or query.funcidx == idx,
+                         query.typeidx is None or query.typeidx == item)
+                ):
+                    function_list.append(Function(idx + import_func_num, item))
+
+            if len(function_list) != 1:
+                raise Exception("error")
+
+            idx = function_list[0].funcidx
+            # delete
+            self.module.func_sec.pop(idx - import_func_num)
+
+            # fix
+            self.indices_fixer.fix_export_funcidx(self.module.export_sec, idx, type=Delete)
+            self.indices_fixer.fix_elem_funcidx(self.module.elem_sec, idx, type=Delete)
+            for _, code in enumerate(self.module.code_sec):
+                self.indices_fixer.fix_call_instructions(code.expr, idx, type=Delete)
+
+
+        # table 和 memory 段暂时不能修改
+        # elif self.tablesec is not None and isinstance(query, Table):
+        #     # 如何表示无穷
+        #     table_list = []
+        #     for idx, item in enumerate(self.module.table_sec):
+        #         if all(
+        #                 (query.min is None or query.min == item.limits.min,
+        #                  query.max is None or query.max == item.limits.max)
+        #         ):
+        #             table_list.append(Table(item.limits.min, item.limits.max))
+        #
+        #     if len(table_list) != 1:
+        #         raise Exception("error")
+        #
+        #     idx = table_list[0]
+        #
+        #     return table_list
+        #
+        # elif self.memsec is not None and isinstance(query, Memory):
+        #
+        #     # 如何表示无穷
+        #     mem_list = []
+        #     for idx, item in enumerate(self.module.mem_sec):
+        #         if all(
+        #                 (query.min is None or query.min == item.min,
+        #                  query.max is None or query.max == item.max)
+        #         ):
+        #             mem_list.append(Memory(item.min, item.max))
+        #     return mem_list
+
+        elif self.globalsec is not None and isinstance(query, Global):
+            global_list = []
+            for idx, item in enumerate(self.module.global_sec):
+                if all(
+                        (query.globalidx is None or query.globalidx == idx,
+                         query.valtype is None or query.valtype == item.type.val_type,
+                         query.mut is None or query.mut == item.type.mut,
+                         query.val is None or query.val == item.init[0].args)
+                ):
+                    global_list.append(Global(idx, item.type.val_type, item.type.mut, item.init[0].args))
+
+            if len(global_list) != 1:
+                raise Exception("error")
+            idx = global_list[0].globalidx
+
+            self.module.global_sec.pop(idx)
+
+            # fix
+            self.indices_fixer.fix_export_globalidx(self.module.export_sec, idx, type=Delete)
+            for code in self.module.code_sec:
+                self.indices_fixer.fix_global_instructions(code.expr, idx, type=Delete)
+
+        elif self.exportsec is not None and isinstance(query, Export):
+            export_list = []
+            for idx, item in enumerate(self.module.export_sec):
+                if all(
+                        (query.exportidx is None or query.exportidx == idx,
+                         query.name is None or query.name == item.name,
+                         # The tag of function is 0
+                         query.funcidx is None or query.funcidx == item.desc.idx)
+                ) and item.desc.tag == 0:
+                    export_list.append(Export(idx, name=item.name, funcidx=item.desc.idx))
+
+            if len(export_list) != 1:
+                raise Exception("error")
+
+            idx = export_list[0].exportidx
+            self.module.export_sec.pop(idx)
+
+        elif self.startsec is not None and isinstance(query, Start):
+            match query:
+                case Start(funcidx=funcidx):
+                    return Start(self.module.start_sec)
+                case Start():
+                    return Start(self.module.start_sec)
+
+        elif self.elemsec is not None and isinstance(query, Element):
+            element_list = []
+            for idx, item in enumerate(self.module.elem_sec):
+                if all(
+                        (query.elemidx is None or query.elemidx == idx,
+                         query.tableidx is None or query.tableidx == item.table,
+                         query.offset is None or query.offset == item.offset[0].args)
+                ):
+                    element_list.append(
+                        Element(idx, tableidx=item.table, offset=item.offset[0].args, funcidx_list=item.init))
+            return element_list
+
+        elif self.codesec is not None and isinstance(query, Code):
+            code_list = []
+            # get import func num
+            import_func_num = 0
+            for import_func in self.module.import_sec:
+                if import_func.desc.func_type is not None:
+                    import_func_num += 1
+            if query.funcidx < import_func_num:
+                raise Exception("Import function!")
+            query.funcidx -= import_func_num
+            for idx, item in enumerate(self.module.code_sec):
+                if query.funcidx is None or query.funcidx == idx:
+                    # locals
+                    locals = []
+                    i = 0
+                    for local in item.locals:
+                        for j in range(i, i + local.n):
+                            locals.append(Local(j, local.type))
+                        i += local.n
+                    # instrs
+                    instrs = self.get_flat_instrs(item.expr)
+                    code_list.append(Code(idx + import_func_num, locals, instrs))
+
+            if len(code_list) != 1:
+                raise Exception("error")
+
+            idx = code_list[0].funcidx
+
+            self.module.code_sec.pop(idx)
+
+        elif self.datasec is not None and isinstance(query, Data):
+            data_list = []
+            for idx, item in enumerate(self.module.data_sec):
+                if all(
+                        (query.dataidx is None or query.dataidx == idx,
+                         query.offset is None or query.offset == item.offset[0].args)
+                ):
+                    # delete
+                    self.module.data_sec.pop(idx)
+            return data_list
+
+        elif self.datacountsec is not None:
+            pass
+        elif self.customsec is not None and isinstance(query, CustomName):
+            name_list = []
+            match query.name_type:
+                # func 0
+                case 0:
+                    for custom in self.module.custom_secs:
+                        if custom.name == "name":
+                            for idx, item in enumerate(custom.name_data.funcNameSubSec):
+                                if all(
+                                        (query.idx is None or query.idx == item.idx,
+                                         query.name is None or query.name == item.name)
+                                ):
+                                    # delete
+                                    custom.name_data.funcNameSubSec.pop(idx)
+                case 1:
+                    for custom in self.module.custom_secs:
+                        if custom.name == "name":
+                            for idx, item in enumerate(custom.name_data.globalNameSubSec):
+                                if all(
+                                        (query.idx is None or query.idx == item.idx,
+                                         query.name is None or query.name == item.name)
+                                ):
+                                    # delete
+                                    custom.name_data.globalNameSubSec.pop(idx)
+                case 2:
+                    for custom in self.module.custom_secs:
+                        if custom.name == "name":
+                            for idx, item in enumerate(custom.name_data.dataNameSubSec):
+                                if all(
+                                        (query.idx is None or query.idx == item.idx,
+                                         query.name is None or query.name == item.name)
+                                ):
+                                    # delete
+                                    custom.name_data.dataNameSubSec.pop(idx)
+                case _:
+                    pass
+            return name_list
+        else:
+            raise Exception("error")
+
+    def update(self, query, new_item):
+
+        if self.typesec is not None and isinstance(query, Type):
+            type_list = []
+            for idx, item in enumerate(self.module.type_sec):
+                param_types, result_types = item.get_signature()
+                if all(
+                        (query.typeidx is None or query.typeidx == idx,
+                         query.arg_types is None or query.arg_types == param_types,
+                         query.ret_types is None or query.ret_types == result_types,)
+                ):
+                    type_list.append(Type(idx, param_types, result_types))
+
+            # update
+            for t in type_list:
+                if new_item.arg_types is not None:
+                    param_types = []
+                    for arg in new_item.arg_types:
+                        match arg:
+                            case "i32":
+                                param_types.append(I32)
+                            case "i64":
+                                param_types.append(I64)
+                            case "f32":
+                                param_types.append(F32)
+                            case "f64":
+                                param_types.append(F64)
+                    self.module.type_sec[t.typeidx].param_types = param_types
+
+                if new_item.ret_types is not None:
+                    result_types = []
+                    for arg in new_item.ret_types:
+                        match arg:
+                            case "i32":
+                                result_types.append(I32)
+                            case "i64":
+                                result_types.append(I64)
+                            case "f32":
+                                result_types.append(F32)
+                            case "f64":
+                                result_types.append(F64)
+                    t.result_types = result_types
+                    self.module.type_sec[t.typeidx].result_types = result_types
+
+        elif self.importsec is not None and isinstance(query, Import):
+
+            import_list = []
+            for idx, item in enumerate(self.module.import_sec):
+                if item.desc.func_type is not None:
+                    if all(
+                            (query.importidx is None or query.importidx == idx,
+                             query.module is None or query.module == item.module,
+                             query.name is None or query.name == item.name,
+                             query.typeidx is None or query.typeidx == item.desc.func_type)
+                    ):
+                        import_list.append(Import(idx, item.module, item.name, item.desc.func_type))
+
+            # update
+            for i in import_list:
+                if new_item.module is not None:
+                    self.module.import_sec[i.importidx].module = new_item.module
+                if new_item.name is not None:
+                    self.module.import_sec[i.importidx].name = new_item.name
+                if new_item.typeidx is not None:
+                    self.module.import_sec[i.importidx].desc.func_type = new_item.typeidx
+
+        elif self.funcsec is not None and isinstance(query, Function):
+            function_list = []
+
+            # get import func num
+            import_func_num = 0
+            for import_func in self.module.import_sec:
+                if import_func.desc.func_type is not None:
+                    import_func_num += 1
+
+            if query.funcidx is not None:
+                query.funcidx -= import_func_num
+
+            for idx, item in enumerate(self.module.func_sec):
+                if all(
+                        (query.funcidx is None or query.funcidx == idx,
+                         query.typeidx is None or query.typeidx == item)
+                ):
+                    function_list.append(Function(idx + import_func_num, item))
+
+            # update
+            for f in function_list:
+                if new_item.typeidx is not None:
+                    self.module.func_sec[f.funcidx - import_func_num] = new_item.typeidx
+
+        elif self.tablesec is not None and isinstance(query, Table):
+            # 如何表示无穷
+            table_list = []
+            for idx, item in enumerate(self.module.table_sec):
+                if all(
+                        (query.min is None or query.min == item.limits.min,
+                         query.max is None or query.max == item.limits.max)
+                ):
+                    table_list.append({
+                        "idx": idx,
+                        "table": Table(item.limits.min, item.limits.max)
+                    })
+
+            # update
+            for t in table_list:
+                if new_item.min is not None:
+                    self.module.table_sec[t["idx"]].limits.min = new_item.min
+                if new_item.max is not None:
+                    self.module.table_sec[t["idx"]].limits.max = new_item.max
+
+        elif self.memsec is not None and isinstance(query, Memory):
+
+            # 如何表示无穷
+            mem_list = []
+            for idx, item in enumerate(self.module.mem_sec):
+                if all(
+                        (query.min is None or query.min == item.min,
+                         query.max is None or query.max == item.max)
+                ):
+                    mem_list.append({
+                        "idx": idx,
+                        "memory": Memory(item.min, item.max)
+                    })
+
+            # update
+            for m in mem_list:
+                if new_item.min is not None:
+                    self.module.mem_sec[m["idx"]].min = new_item.min
+                if new_item.max is not None:
+                    self.module.mem_sec[m["idx"]].max = new_item.max
+
+        elif self.globalsec is not None and isinstance(query, Global):
+            global_list = []
+            for idx, item in enumerate(self.module.global_sec):
+                if all(
+                        (query.globalidx is None or query.globalidx == idx,
+                         query.valtype is None or query.valtype == item.type.val_type,
+                         query.mut is None or query.mut == item.type.mut,
+                         query.val is None or query.val == item.init[0].args)
+                ):
+                    global_list.append(Global(idx, item.type.val_type, item.type.mut, item.init[0].args))
+
+            for g in global_list:
+                if new_item.valtype is not None:
+                    self.module.global_sec[g.globalidx].type.val_type = new_item.valtype
+                if new_item.mut is not None:
+                    self.module.global_sec[g.globalidx].type.mut = new_item.mut
+                if new_item.val is not None:
+                    if self.module.global_sec[g.globalidx].type.val_type == I32:
+                        init_value_instr = Instruction(I32Const, new_item.val)
+                    elif self.module.global_sec[g.globalidx].type.val_type == I64:
+                        init_value_instr = Instruction(I64Const, new_item.val)
+                    elif self.module.global_sec[g.globalidx].type.val_type == F32:
+                        init_value_instr = Instruction(F32Const, new_item.val)
+                    elif self.module.global_sec[g.globalidx].type.val_type == F64:
+                        init_value_instr = Instruction(F64Const, new_item.val)
+                    self.module.global_sec[g.globalidx].init[0] = init_value_instr
+
+        elif self.exportsec is not None and isinstance(query, Export):
+            export_list = []
+            for idx, item in enumerate(self.module.export_sec):
+                if all(
+                        (query.exportidx is None or query.exportidx == idx,
+                         query.name is None or query.name == item.name,
+                         # The tag of function is 0
+                         query.funcidx is None or query.funcidx == item.desc.idx)
+                ) and item.desc.tag == 0:
+                    export_list.append(Export(idx, name=item.name, funcidx=item.desc.idx))
+
+            # update
+            for e in export_list:
+                if new_item.name is not None:
+                    self.module.export_sec[e.exportidx].name = new_item.name
+                if new_item.funcidx is not None:
+                    self.module.export_sec[e.exportidx].desc.idx = new_item.funcidx
+
+        # elif self.startsec is not None and isinstance(query, Start):
+        #     match query:
+        #         case Start(funcidx=funcidx):
+        #             return Start(self.module.start_sec)
+        #         case Start():
+        #             return Start(self.module.start_sec)
+
+        elif self.elemsec is not None and isinstance(query, Element):
+            element_list = []
+            for idx, item in enumerate(self.module.elem_sec):
+                if all(
+                        (query.elemidx is None or query.elemidx == idx,
+                         query.tableidx is None or query.tableidx == item.table,
+                         query.offset is None or query.offset == item.offset[0].args)
+                ):
+                    element_list.append(
+                        Element(idx, tableidx=item.table, offset=item.offset[0].args, funcidx_list=item.init))
+
+            # update
+            for e in element_list:
+                if new_item.tableidx is not None:
+                    self.module.elem_sec[e.elemidx].table = new_item.tableidx
+                if new_item.offset is not None:
+                    self.module.elem_sec[e.elemidx].offset = [Instruction(I32Const, new_item.offset)]
+                if new_item.funcidx_list is not None:
+                    self.module.elem_sec[e.elemidx].init = new_item.funcidx_list
+
+                indirect_func_list = e.funcidx_list
+                self.indices_fixer.fix_table_limits(self.module.table_sec, len(indirect_func_list) + 1)
+
+        elif self.codesec is not None and isinstance(query, Code):
+            code_list = []
+            # get import func num
+            import_func_num = 0
+            for import_func in self.module.import_sec:
+                if import_func.desc.func_type is not None:
+                    import_func_num += 1
+            if query.funcidx < import_func_num:
+                raise Exception("Import function!")
+            query.funcidx -= import_func_num
+            for idx, item in enumerate(self.module.code_sec):
+                if query.funcidx is None or query.funcidx == idx:
+                    # locals
+                    locals = []
+                    i = 0
+                    for local in item.locals:
+                        for j in range(i, i + local.n):
+                            locals.append(Local(j, local.type))
+                        i += local.n
+                    # instrs
+                    instrs = self.get_flat_instrs(item.expr)
+                    code_list.append(Code(idx + import_func_num, locals, instrs))
+
+            # update
+            for c in code_list:
+                if new_item.local_vec is not None:
+                    self.module.code_sec[c.funcidx - import_func_num].locals = new_item.convert_local_vec()
+                if new_item.instr_list is not None:
+                    self.module.code_sec[c.funcidx - import_func_num].expr = self.get_fold_instrs(new_item.instr_list)
+
+
+
+        elif self.datasec is not None and isinstance(query, Data):
+            data_list = []
+            for idx, item in enumerate(self.module.data_sec):
+                if all(
+                        (query.dataidx is None or query.dataidx == idx,
+                         query.offset is None or query.offset == item.offset[0].args)
+                ):
+                    data_list.append(Data(idx, item.offset[0].args, item.init))
+
+            # update
+            for d in data_list:
+                if new_item.offset is not None:
+                    self.module.data_sec[d.dataidx].offset = [Instruction(I32Const, new_item.offset)]
+                if new_item.init_data is not None:
+                    self.module.data_sec[d.dataidx].init = new_item.init_data
+
+        elif self.datacountsec is not None:
+            pass
+        elif self.customsec is not None and isinstance(query, CustomName):
+            name_list = []
+            match query.name_type:
+                # func 0
+                case 0:
+                    for custom in self.module.custom_secs:
+                        if custom.name == "name":
+                            for idx, item in enumerate(custom.name_data.funcNameSubSec):
+                                if all(
+                                        (query.idx is None or query.idx == item.idx,
+                                         query.name is None or query.name == item.name)
+                                ):
+                                    name_list.append(CustomName(FunctionName, item.idx, item.name))
+                case 1:
+                    for custom in self.module.custom_secs:
+                        if custom.name == "name":
+                            for idx, item in enumerate(custom.name_data.globalNameSubSec):
+                                if all(
+                                        (query.idx is None or query.idx == item.idx,
+                                         query.name is None or query.name == item.name)
+                                ):
+                                    name_list.append(CustomName(GlobalName, item.idx, item.name))
+                case 2:
+                    for custom in self.module.custom_secs:
+                        if custom.name == "name":
+                            for idx, item in enumerate(custom.name_data.dataNameSubSec):
+                                if all(
+                                        (query.idx is None or query.idx == item.idx,
+                                         query.name is None or query.name == item.name)
+                                ):
+                                    name_list.append(CustomName(DataName, item.idx, item.name))
+                case _:
+                    pass
+
+            # update
+            name_section_idx = None
+            for i, custom_sec in enumerate(self.module.custom_secs):
+                if custom_sec.name == "name":
+                    name_section_idx = i
+
+            for n in name_list:
+                if new_item.name is not None:
+                    match n.name_type:
+                        case 0:
+                            self.module.custom_secs[name_section_idx].name_data.funcNameSubSec[
+                                n.idx].name = new_item.name
+                        case 1:
+                            self.module.custom_secs[name_section_idx].name_data.globalNameSubSec[
+                                n.idx].name = new_item.name
+                        case 2:
+                            self.module.custom_secs[name_section_idx].name_data.dataNameSubSec[
+                                n.idx].name = new_item.name
+                        case _:
+                            pass
+
+        else:
+            raise Exception("error")
+
+    def emit_binary(self, path: str):
+        ModifyBinary(self.module, self.module.path).emit_binary(path)
+
+    # 这里的end没有算作指令
+    def get_flat_instrs(self, instrs):
+        ret_instrs = []
+        for _, i in enumerate(instrs):
+            if i.opcode in [Block, Loop]:
+                ret_instrs.append(i)
+                args = i.args
+                ret_instrs.extend(self.get_flat_instrs(args.instrs))
+                ret_instrs.append(Instruction(End_))
+            elif i.opcode == If:
+                ret_instrs.append(i)
+                args = i.args
+                ret_instrs.extend(self.get_flat_instrs(args.instrs1))
+                ret_instrs.append(Instruction(Else_))
+                ret_instrs.extend(self.get_flat_instrs(args.instrs2))
+                ret_instrs.append(Instruction(End_))
+            else:
+                ret_instrs.append(i)
+        return ret_instrs
+
+    def get_fold_instrs(self, instrs):
+        ret_instrs = []
+        i = 0
+        while i < len(instrs):
+            if instrs[i].opcode in [Block, Loop]:
+                j = i
+                args_instrs_length = self.get_flat_Block_length(instrs[i:]) - 2
+                instrs[i].args.instrs = self.get_fold_instrs(instrs[i + 1: i + 1 + args_instrs_length])
+                i = i + args_instrs_length + 2
+                ret_instrs.append(instrs[j])
+            elif instrs[i].opcode == If:
+                j = i
+                else_offset, length = self.get_flat_If_length(instrs[i:]) - 2
+                instrs[j].args.instrs1 = self.get_fold_instrs(instrs[i + 1, i + else_offset])
+                i = i + else_offset
+                instrs[j].args.instrs2 = self.get_fold_instrs(instrs[i + 1, i + length - 1])
+                i = j + length
+                ret_instrs.append(instrs[j])
+            else:
+                ret_instrs.append(instrs[i])
+                i += 1
+        return ret_instrs
+
+    def get_flat_Block_length(self, instrs):
+
+        if instrs[0].opcode in [Block, Loop]:
+            instr_queue = [instrs[0]]
+            i = 1
+            while i < len(instrs):
+                if instrs[i].opcode in [Block, Loop]:
+                    instr_queue.append(instrs[i])
+                    i += 1
+                elif instrs[i].opcode in [If, Else_]:
+                    instr_queue.append(instrs[i])
+                    i += 1
+                elif instrs[i].opcode == End_:
+                    instr_queue.append(instrs[i])
+                    i += 1
+                    if instr_queue[-2].opcode == Else_:
+                        instr_queue = instr_queue[0: -3]
+                    elif instr_queue[-2].opcode in [Block, Loop]:
+                        instr_queue = instr_queue[0: -2]
+                    if instr_queue == []:
+                        length = i
+                        return length
+                else:
+                    i += 1
+        else:
+            raise Exception("error")
+
+    def get_flat_If_length(self, instrs):
+
+        if instrs[0].opcode in [If]:
+            instr_queue = [{
+                        "offset": 0,
+                        "instr": instrs[0]
+                    }]
+            i = 1
+            while i < len(instrs):
+                if instrs[i].opcode in [Block, Loop]:
+                    instr_queue.append({
+                        "offset": i,
+                        "instr": instrs[i]
+                    })
+                    i += 1
+                elif instrs[i].opcode in [If, Else_]:
+                    instr_queue.append({
+                        "offset": i,
+                        "instr": instrs[i]
+                    })
+                    i += 1
+                elif instrs[i].opcode == End_:
+                    instr_queue.append({
+                        "offset": i,
+                        "instr": instrs[i]
+                    })
+                    i += 1
+                    if instr_queue[-2].opcode == Else_ and len(instr_queue) != 3:
+                        instr_queue = instr_queue[0: -3]
+                    elif instr_queue[-2].opcode in [Block, Loop]:
+                        instr_queue = instr_queue[0: -2]
+                    elif instr_queue[-2].opcode == Else_ and len(instr_queue) == 3:
+                        else_offset = instr_queue[1]["offset"]
+                        length = i
+                        return else_offset, length
+                else:
+                    i += 1
+        else:
+            raise Exception("error")
+
+    # def _get_instrs_instr(self, instrs, offset=None, current_offset=-1, instr=None, ret_instrs=[]):
+    #     if offset is not None:
+    #         for _, i in enumerate(instrs):
+    #             current_offset += 1
+    #             if i.opcode in [Block, Loop]:
+    #                 if offset == current_offset:
+    #                     return RetInstrs(_, i, instrs)
+    #                 args = i.args
+    #                 return self._get_instrs_instr(args.instrs, offset=offset, current_offset=current_offset, instr=instr)
+    #                 # 将end也算一个指令
+    #                 current_offset += 1
+    #                 if offset == current_offset:
+    #                     raise Exception("end can not be get")
+    #             elif i.opcode == If:
+    #                 if offset == current_offset:
+    #                     return RetInstrs(_, i, instrs)
+    #                 args = i.args
+    #                 return self._get_instrs_instr(args.instrs1, offset=offset, current_offset=current_offset,
+    #                                               instr=instr)
+    #                 # 将else也算一个指令
+    #                 current_offset += 1
+    #                 if offset == current_offset:
+    #                     raise Exception("else can not be get")
+    #                 return self._get_instrs_instr(args.instrs2, offset=offset, current_offset=current_offset,
+    #                                               instr=instr)
+    #                 # 将end也算一个指令
+    #                 current_offset += 1
+    #                 if offset == current_offset:
+    #                     raise Exception("end can not be get")
+    #             else:
+    #                 if current_offset == offset:
+    #                     return RetInstrs(_, i, instrs)
+    #     elif instr is not None and instr.args is None:
+    #         ret_instrs = []
+    #         for _, i in enumerate(instrs):
+    #             if i.opcode in [Block, Loop]:
+    #                 if i.opcode == instr.opcode:
+    #                     ret_instrs.append(RetInstrs(_, i, instrs))
+    #                 args = i.args
+    #                 ret_instrs.extend(
+    #                     self._get_instrs_instr(args.instrs, offset=offset, current_offset=current_offset, instr=instr))
+    #             elif i.opcode == If:
+    #                 if i.opcode == instr.opcode:
+    #                     ret_instrs.append(RetInstrs(_, i, instrs))
+    #                 args = i.args
+    #                 ret_instrs.extend(
+    #                     self._get_instrs_instr(args.instrs1, offset=offset, current_offset=current_offset, instr=instr))
+    #                 ret_instrs.extend(
+    #                     self._get_instrs_instr(args.instrs2, offset=offset, current_offset=current_offset, instr=instr))
+    #             else:
+    #                 if i.opcode == instr.opcode:
+    #                     ret_instrs.append(RetInstrs(_, i, instrs))
+    #         return ret_instrs
+    #     elif instr is not None:
+    #         ret_instrs = []
+    #         for _, i in enumerate(instrs):
+    #             if i.opcode in [Block, Loop]:
+    #                 if i.opcode == instr.opcode and i.args == instr.args:
+    #                     ret_instrs.append(RetInstrs(_, i, instrs))
+    #                 args = i.args
+    #                 ret_instrs.extend(
+    #                     self._get_instrs_instr(args.instrs, offset=offset, current_offset=current_offset, instr=instr))
+    #             elif i.opcode == If:
+    #                 if i.opcode == instr.opcode and i.args == instr.args:
+    #                     ret_instrs.append(RetInstrs(_, i, instrs))
+    #                 args = i.args
+    #                 ret_instrs.extend(
+    #                     self._get_instrs_instr(args.instrs1, offset=offset, current_offset=current_offset, instr=instr))
+    #                 ret_instrs.extend(
+    #                     self._get_instrs_instr(args.instrs2, offset=offset, current_offset=current_offset, instr=instr))
+    #             else:
+    #                 if i.opcode == instr.opcode and i.args == instr.args:
+    #                     ret_instrs.append(RetInstrs(_, i, instrs))
+    #         return ret_instrs
```

### Comparing `BREWasm-1.0.0/BREWasm/rewriter/semantics_rewriter.py` & `BREWasm-1.0.1/BREWasm/rewriter/semantics_rewriter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,438 +1,443 @@
-from BREWasm.parser.instruction import Instruction
-from BREWasm.rewriter.indices_fixer import IndicesFixer
-from BREWasm.rewriter.section_rewriter import *
-
-
-class SemanticsRewriter:
-
-    class GlobalVariable:
-        def __init__(self, module):
-            self.module = module
-
-        def insert_global_variable(self, idx, global_type, init_value):
-            global_rewriter = SectionRewriter(self.module, globalsec=self.module.global_sec)
-            global_rewriter.insert(Global(globalidx=idx), Global(valtype=global_type, val=init_value))
-
-        def append_global_variable(self, global_type, init_value):
-            global_rewriter = SectionRewriter(self.module, globalsec=self.module.global_sec)
-            global_rewriter.insert(None, inserted_item=Global(valtype=global_type, val=init_value))
-
-        def modify_global_variable(self, idx, global_type, init_value):
-            global_rewriter = SectionRewriter(self.module, globalsec=self.module.global_sec)
-            global_rewriter.update(Global(globalidx=idx), Global(valtype=global_type, val=init_value))
-
-        def delete_global_variable(self, idx=None, global_type=None, init_value=None):
-            if idx is not None:
-                global_rewriter = SectionRewriter(self.module, globalsec=self.module.global_sec)
-                global_rewriter.delete(Global(globalidx=idx))
-                return
-            if global_type is not None and init_value is not None:
-                global_rewriter = SectionRewriter(self.module, globalsec=self.module.global_sec)
-                global_variable = global_rewriter.select(Global(valtype=global_type, val=init_value))
-                global_rewriter.delete(global_variable[0].globalidx)
-
-    class ImportExport:
-        def __init__(self, module):
-            self.module = module
-
-        def insert_import_function(self, idx, module_name, func_name, params_type, results_type):
-
-            type_rewriter = SectionRewriter(self.module, typesec=self.module.type_sec)
-            result = type_rewriter.select(Type(arg_types=params_type, ret_types=results_type))
-            if result == []:
-                type_rewriter.insert(None, inserted_item=Type(arg_types=params_type, ret_types=results_type))
-                typeidx = type_rewriter.select(Type())[-1].typeidx
-            else:
-                typeidx = result[0].typeidx
-
-            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
-            import_rewriter.insert(Import(importidx=idx),
-                                   Import(module=module_name, name=func_name, typeidx=typeidx))
-
-        def delete_import_function(self, idx=None, module_name=None, func_name=None):
-
-            if idx is not None:
-                import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
-                import_rewriter.delete(Import(importidx=idx))
-                return
-            if module_name is not None and func_name is not None:
-                import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
-                import_function = import_rewriter.select(Import(module=module_name, name=func_name))
-                import_rewriter.delete(import_function[0].importidx)
-
-        def modify_import_function(self, idx, module_name, func_name, params_type, results_type):
-            type_rewriter = SectionRewriter(self.module, typesec=self.module.type_sec)
-            result = type_rewriter.select(Type(arg_types=params_type, ret_types=results_type))
-            if result == []:
-                type_rewriter.insert(None, inserted_item=Type(arg_types=params_type, ret_types=results_type))
-                typeidx = type_rewriter.select(Type())[-1].typeidx
-            else:
-                typeidx = result[0].typeidx
-
-            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
-            import_rewriter.update(Import(importidx=idx), Import(module=module_name, name=func_name, typeidx=typeidx))
-
-        def append_import_function(self, module_name, func_name, params_type, results_type):
-            type_rewriter = SectionRewriter(self.module, typesec=self.module.type_sec)
-            result = type_rewriter.select(Type(arg_types=params_type, ret_types=results_type))
-            if result == []:
-                type_rewriter.insert(None, inserted_item=Type(arg_types=params_type, ret_types=results_type))
-                typeidx = type_rewriter.select(Type())[-1].typeidx
-            else:
-                typeidx = result[0].typeidx
-
-            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
-            import_rewriter.insert(None, inserted_item=Import(module=module_name, name=func_name, typeidx=typeidx))
-
-        def insert_export_function(self, idx, func_name, funcidx):
-
-            export_rewriter = SectionRewriter(self.module, exportsec=self.module.export_sec)
-            export_rewriter.insert(Export(exportidx=idx), Export(name=func_name, funcidx=funcidx))
-
-        def modify_export_function(self, idx, func_name, funcidx):
-
-            export_rewriter = SectionRewriter(self.module, exportsec=self.module.export_sec)
-            export_rewriter.update(Export(exportidx=idx), Export(name=func_name, funcidx=funcidx))
-
-        def delete_export_function(self, idx=None, func_name=None):
-
-            if idx is not None:
-                export_rewriter = SectionRewriter(self.module, exportsec=self.module.export_sec)
-                export_rewriter.delete(Export(exportidx=idx))
-                return
-            if func_name is not None:
-                export_rewriter = SectionRewriter(self.module, exportsec=self.module.export_sec)
-                export_function = export_rewriter.select(Export(name=func_name))
-                export_rewriter.delete(export_function[0].exportidx)
-
-        def append_export_function(self, func_name, funcidx):
-
-            export_rewriter = SectionRewriter(self.module, exportsec=self.module.export_sec)
-            export_rewriter.insert(None, inserted_item=Export(name=func_name, funcidx=funcidx))
-
-        # def insert_import_global_variable(self, idx, module_name, variable_name, valtype):
-        #     import_variable = Import(module_name, variable_name, ImportDesc(3, global_type=valtype))
-        #     for _, import_item in enumerate(self.module.import_sec):
-        #         if import_item == import_variable:
-        #             raise Exception("The global variable already exists")
-        #     self.section_rewriter.insert_importsec_import(idx, import_variable)
-        #
-        #     # fix
-        #     pass
-        #
-        # def modify_import_global_variable(self, idx, module_name, variable_name, valtype):
-        #     import_variable = Import(module_name, variable_name, ImportDesc(3, global_type=valtype))
-        #     for _, import_item in enumerate(self.module.import_sec):
-        #         if import_item == import_variable:
-        #             raise Exception("The global variable already exists")
-        #     self.module.import_sec[idx] = import_variable
-        #
-        #     # fix
-        #     for code in self.section_rewriter.get_codesec_code_list():
-        #         self.indices_fixer.fix_global_instructions(code.expr, idx)
-        #
-        # def insert_import_memory(self, idx, module_name, memory_name, limits):
-        #     mem_list = self.section_rewriter.get_mem_list()
-        #     memidx = None
-        #     for _, mem in enumerate(mem_list):
-        #         if mem == limits:
-        #             memidx = _
-        #     if memidx is None:
-        #         memidx = self.section_rewriter.append_memsec_mem(limits)
-        #
-        #     import_mem = Import(module_name, memory_name, ImportDesc(2, mem=memidx))
-        #     self.section_rewriter.insert_importsec_import(idx, import_mem)
-        #
-        #     # fix
-        #     pass
-        #
-        # def modify_import_memory(self, idx, module_name, memory_name, limits):
-        #     mem_list = self.section_rewriter.get_mem_list()
-        #     memidx = None
-        #     for _, mem in enumerate(mem_list):
-        #         if mem == limits:
-        #             memidx = _
-        #     if memidx is None:
-        #         memidx = self.section_rewriter.append_memsec_mem(limits)
-        #
-        #     import_mem = Import(module_name, memory_name, ImportDesc(2, mem=memidx))
-        #     self.module.import_sec[idx] = import_mem
-        #
-        # def insert_import_table(self, idx, module_name, table_name, limits):
-        #     table_list = self.section_rewriter.get_table_list()
-        #     tableidx = None
-        #     for _, table in enumerate(table_list):
-        #         if table == limits:
-        #             tableidx = _
-        #     if tableidx is None:
-        #         tableidx = self.section_rewriter.append_tablesec_table(limits)
-        #
-        #     import_table = Import(module_name, table_name, ImportDesc(1, table=tableidx))
-        #     self.section_rewriter.insert_importsec_import(idx, import_table)
-        #
-        # def modify_import_table(self, idx, module_name, table_name, limits):
-        #     table_list = self.section_rewriter.get_table_list()
-        #     tableidx = None
-        #     for _, table in enumerate(table_list):
-        #         if table == limits:
-        #             tableidx = _
-        #     if tableidx is None:
-        #         tableidx = self.section_rewriter.append_tablesec_table(limits)
-        #
-        #     import_table = Import(module_name, table_name, ImportDesc(1, table=tableidx))
-        #     self.module.import_sec[idx] = import_table
-
-    class LinearMemory:
-        def __init__(self, module):
-            self.module = module
-            self.indices_fixer = IndicesFixer(self.module)
-
-        def insert_linear_memory(self, offset, bytes):
-            memory_rewriter = SectionRewriter(self.module, memsec=self.module.mem_sec)
-            memory_list = memory_rewriter.select(Memory())
-
-            if memory_list[0].max != 0 and offset + len(bytes) + 1 > memory_list[0].max * 65536:
-                raise Exception("Memory out of bounds")
-
-            data_rewriter = SectionRewriter(self.module, datasec=self.module.data_sec)
-
-            is_overlap = False
-            length = len(bytes)
-            for data_item in data_rewriter.select(Data()):
-                if offset + length < data_item.offset:
-                    is_overlap = False
-                elif data_item.offset + len(data_item.init_data) < offset:
-                    is_overlap = False
-                elif offset + length >= data_item.offset:
-                    is_overlap = True
-                    if offset >= data_item.offset:
-                        data_item.init_data = data_item.init_data[:(offset - data_item.offset)] + bytearray(
-                            bytes) + data_item.init_data[(offset - data_item.offset):]
-                    else:
-                        data_item.offset -= (offset - data_item.offset)
-                        data_item.init_data = bytearray(bytes) + data_item.init_data
-
-                self.indices_fixer.fix_memory_limits(self.module.mem_sec, offset + length)
-
-            if data_rewriter.select(Data()) is [] or is_overlap is False:
-                data_rewriter.insert(None, inserted_item=Data(offset=offset, init_data=bytes))
-
-        def append_linear_memory(self, page_num):
-            memory_rewriter = SectionRewriter(self.module, memsec=self.module.mem_sec)
-            mem_list = memory_rewriter.select(Memory())
-
-            if mem_list[0].max != 0:
-                mem_list[0].max += page_num
-
-        def modify_linear_memory(self, offset, bytes):
-            memory_rewriter = SectionRewriter(self.module, memsec=self.module.mem_sec)
-            mem_list = memory_rewriter.select(Memory())
-
-            if mem_list[0].max != 0 and offset + len(bytes) + 1 > mem_list[0].max * 65536:
-                raise Exception("Memory out of bounds")
-
-            data_rewriter = SectionRewriter(self.module, datasec=self.module.data_sec)
-            data_rewriter.insert(None, inserted_item=Data(offset=offset, init_data=bytes))
-
-    class Function:
-        def __init__(self, module):
-            self.module = module
-
-        def insert_internal_function(self, idx, params_type, results_type, local_vec, func_body):
-
-            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
-            import_func_num = len(import_rewriter.select(Import()))
-
-            if import_func_num > idx:
-                raise Exception("The idx of internal function less than import function")
-
-            type_rewriter = SectionRewriter(self.module, typesec=self.module.type_sec)
-            result = type_rewriter.select(Type(arg_types=params_type, ret_types=results_type))
-            if result == []:
-                type_rewriter.insert(None, inserted_item=Type(arg_types=params_type, ret_types=results_type))
-                typeidx = type_rewriter.select(Type())[-1].typeidx
-            else:
-                typeidx = result[0].typeidx
-
-            function_rewriter = SectionRewriter(self.module, funcsec=self.module.func_sec)
-            function_rewriter.insert(Function(funcidx=idx), Function(typeidx=typeidx))
-
-            code_rewriter = SectionRewriter(self.module, codesec=self.module.code_sec)
-            code_rewriter.insert(Code(funcidx=idx), Code(local_vec=local_vec, instr_list=func_body))
-
-        def insert_indirect_function(self, idx, params_type, results_type, local_vec, func_body):
-
-            self.insert_internal_function(idx, params_type, results_type, local_vec, func_body)
-
-            element_rewriter = SectionRewriter(self.module, elemsec=self.module.elem_sec)
-
-            # get original indirect function list
-            indirect_func_list = []
-            for elem in element_rewriter.select(Element()):
-                indirect_func_list.extend(elem.funcidx_list)
-
-            element_list = element_rewriter.select(Element())
-
-            if not element_list:
-                element_rewriter.insert(None, inserted_item=Element(tableidx=0, offset=1, funcidx_list=[idx]))
-            else:
-                element_list[0].funcidx_list.append(idx)
-                element_rewriter.update(Element(elemidx=element_list[0].elemidx), element_list[0])
-
-        def insert_hook_function(self, hooked_funcidx, idx, params_type, results_type, locals_vec, func_body):
-            self.insert_internal_function(idx, params_type, results_type, locals_vec, func_body)
-
-            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
-            import_func_num = len(import_rewriter.select(Import()))
-
-            code_rewriter = SectionRewriter(self.module, codesec=self.module.code_sec)
-
-            for funcidx in range(import_func_num, import_func_num + len(code_rewriter.select(Code()))):
-                if funcidx != idx:
-                    code = code_rewriter.select(Code(funcidx=funcidx))
-                    for instr in code.instr_list:
-                        if instr == Instruction(Call, hooked_funcidx):
-                            instr.opcode = Call
-                            instr.args = idx
-                    code_rewriter.update(Code(funcidx=funcidx), Code(instr_list=code.instr_list))
-
-            return idx
-
-        # def change_func_instr(self, binary, funcidx, offset, instr):
-        #     import_func_num = self.section_rewriter.get_import_func_num()
-        #     if funcidx < import_func_num:
-        #         raise Exception("funcidx error")
-        #     code = self.section_rewriter.get_codesec_code(binary, funcidx - import_func_num)
-        #
-        #     self.section_rewriter.modify_code_instr(code, offset, instr)
-
-        def delete_func_instr(self, funcidx, offset):
-
-            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
-            import_func_num = len(import_rewriter.select(Import()))
-
-            if funcidx < import_func_num:
-                raise Exception("funcidx error")
-
-            code_rewriter = SectionRewriter(self.module, codesec=self.module.code_sec)
-            code_list = code_rewriter.select(Code(funcidx=funcidx))
-
-            code_list[0].instr_list.pop(offset)
-            code_rewriter.update(Code(funcidx=funcidx), code_list[0])
-
-        def insert_func_instrs(self, funcidx, offset, instrs: list):
-
-            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
-            import_func_num = len(import_rewriter.select(Import()))
-
-            if funcidx < import_func_num:
-                raise Exception("funcidx error")
-
-            code_rewriter = SectionRewriter(self.module, codesec=self.module.code_sec)
-            code_list = code_rewriter.select(Code(funcidx=funcidx))
-
-            for i in reversed(instrs):
-                code_list[0].instr_list.insert(offset, i)
-
-            code_rewriter.update(Code(funcidx=funcidx), code_list[0])
-
-        def append_func_instrs(self, funcidx, instrs: list):
-
-            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
-            import_func_num = len(import_rewriter.select(Import()))
-
-            if funcidx < import_func_num:
-                raise Exception("funcidx error")
-
-            code_rewriter = SectionRewriter(self.module, codesec=self.module.code_sec)
-            code_list = code_rewriter.select(Code(funcidx=funcidx))
-
-            code_list[0].instr_list.extend(instrs)
-            code_rewriter.update(Code(funcidx=funcidx), code_list[0])
-
-        def modify_func_instrs(self, funcidx, instr, instrs: list):
-            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
-            import_func_num = len(import_rewriter.select(Import()))
-
-            if funcidx < import_func_num:
-                raise Exception("funcidx error")
-
-            code_rewriter = SectionRewriter(self.module, codesec=self.module.code_sec)
-            code_list = code_rewriter.select(Code(funcidx=funcidx))
-
-            for index, i in enumerate(code_list[0].instr_list):
-                if i == instr:
-                    code_list[0].instr_list.pop(index)
-                    for j in reversed(instrs):
-                        code_list[0].instr_list.insert(index, j)
-
-            code_rewriter.update(Code(funcidx=funcidx), Code(instr_list=code_list[0].instr_list))
-
-        def append_func_local(self, funcidx, valtype):
-            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
-            import_func_num = len(import_rewriter.select(Import()))
-
-            if funcidx < import_func_num:
-                raise Exception("funcidx error")
-
-            code_rewriter = SectionRewriter(self.module, codesec=self.module.code_sec)
-            code = code_rewriter.select(Code(funcidx=funcidx))
-            code.local_vec.append(Local(len(code.local_vec), valtype))
-
-            code_rewriter.update(Code(funcidx=funcidx), Code(instr_list=code.instr_list))
-
-    class CustomContent:
-        def __init__(self, module):
-            self.module = module
-
-        def modify_func_name(self, funcidx, name):
-            namesec = self.section_rewriter.get_customsec_custom(name="name")
-            funcname_list = self.section_rewriter.get_namesec_funcname_list(namesec)
-            for _, funcname in enumerate(funcname_list):
-                if funcname.idx == funcidx:
-                    funcname_list[_].name = name
-
-        def delete_func_name(self, funcidx):
-            namesec = self.section_rewriter.get_customsec_custom(name="name")
-            funcname_list = self.section_rewriter.get_namesec_funcname_list(namesec)
-            for _, funcname in enumerate(funcname_list):
-                if funcname.idx == funcidx:
-                    funcname_list.pop(_)
-
-        def insert_func_name(self, funcidx, name):
-            namesec = self.section_rewriter.get_customsec_custom(name="name")
-            funcname_list = self.section_rewriter.get_namesec_funcname_list(namesec)
-            for _, funcname in enumerate(funcname_list):
-                if funcname.idx == (funcidx - 1):
-                    funcname_list.insert(_ + 1, NameAssoc(funcidx, name))
-                    return
-
-        def insert_global_name(self, globalidx, name):
-            namesec = self.section_rewriter.get_customsec_custom(name="name")
-            globalname_list = self.section_rewriter.get_namesec_globalname_list(namesec)
-            globalname_list.insert(globalidx, NameAssoc(globalidx, name))
-
-        def delete_global_name(self, globalidx):
-            namesec = self.section_rewriter.get_customsec_custom(name="name")
-            globalname_list = self.section_rewriter.get_namesec_globalname_list(namesec)
-            globalname_list.pop(globalidx)
-
-        def modify_global_name(self, globalidx, name):
-            namesec = self.section_rewriter.get_customsec_custom(name="name")
-            globalname_list = self.section_rewriter.get_namesec_globalname_list(namesec)
-            globalname_list[globalidx].name = name
-
-        def insert_data_name(self, dataidx, name):
-            namesec = self.section_rewriter.get_customsec_custom(name="name")
-            dataname_list = self.section_rewriter.get_namesec_dataname_list(namesec)
-            dataname_list.insert(dataidx, NameAssoc(dataidx, name))
-
-        def delete_data_name(self, dataidx):
-            namesec = self.section_rewriter.get_customsec_custom(name="name")
-            dataname_list = self.section_rewriter.get_namesec_dataname_list(namesec)
-            dataname_list.pop(dataidx)
-
-        def modify_data_name(self, dataidx, name):
-            namesec = self.section_rewriter.get_customsec_custom(name="name")
-            dataname_list = self.section_rewriter.get_namesec_dataname_list(namesec)
-            dataname_list[dataidx].name = name
+from BREWasm.parser.instruction import Instruction
+from BREWasm.rewriter.indices_fixer import IndicesFixer
+from BREWasm.rewriter.section_rewriter import *
+
+
+class SemanticsRewriter:
+
+    class GlobalVariable:
+        def __init__(self, module):
+            self.module = module
+
+        def insert_global_variable(self, idx, global_type, init_value):
+            global_rewriter = SectionRewriter(self.module, globalsec=self.module.global_sec)
+            global_rewriter.insert(Global(globalidx=idx), Global(valtype=global_type, val=init_value))
+
+        def append_global_variable(self, global_type, init_value):
+            global_rewriter = SectionRewriter(self.module, globalsec=self.module.global_sec)
+            global_rewriter.insert(None, inserted_item=Global(valtype=global_type, val=init_value))
+
+        def modify_global_variable(self, idx, global_type, init_value):
+            global_rewriter = SectionRewriter(self.module, globalsec=self.module.global_sec)
+            global_rewriter.update(Global(globalidx=idx), Global(valtype=global_type, val=init_value))
+
+        def delete_global_variable(self, idx=None, global_type=None, init_value=None):
+            if idx is not None:
+                global_rewriter = SectionRewriter(self.module, globalsec=self.module.global_sec)
+                global_rewriter.delete(Global(globalidx=idx))
+                return
+            if global_type is not None and init_value is not None:
+                global_rewriter = SectionRewriter(self.module, globalsec=self.module.global_sec)
+                global_variable = global_rewriter.select(Global(valtype=global_type, val=init_value))
+                global_rewriter.delete(global_variable[0].globalidx)
+
+    class ImportExport:
+        def __init__(self, module):
+            self.module = module
+
+        def insert_import_function(self, idx, module_name, func_name, params_type, results_type):
+
+            type_rewriter = SectionRewriter(self.module, typesec=self.module.type_sec)
+            result = type_rewriter.select(Type(arg_types=params_type, ret_types=results_type))
+            if result == []:
+                type_rewriter.insert(None, inserted_item=Type(arg_types=params_type, ret_types=results_type))
+                typeidx = type_rewriter.select(Type())[-1].typeidx
+            else:
+                typeidx = result[0].typeidx
+
+            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
+            import_rewriter.insert(Import(importidx=idx),
+                                   Import(module=module_name, name=func_name, typeidx=typeidx))
+
+        def delete_import_function(self, idx=None, module_name=None, func_name=None):
+
+            if idx is not None:
+                import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
+                import_rewriter.delete(Import(importidx=idx))
+                return
+            if module_name is not None and func_name is not None:
+                import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
+                import_function = import_rewriter.select(Import(module=module_name, name=func_name))
+                import_rewriter.delete(import_function[0].importidx)
+
+        def modify_import_function(self, idx, module_name, func_name, params_type, results_type):
+            type_rewriter = SectionRewriter(self.module, typesec=self.module.type_sec)
+            result = type_rewriter.select(Type(arg_types=params_type, ret_types=results_type))
+            if result == []:
+                type_rewriter.insert(None, inserted_item=Type(arg_types=params_type, ret_types=results_type))
+                typeidx = type_rewriter.select(Type())[-1].typeidx
+            else:
+                typeidx = result[0].typeidx
+
+            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
+            import_rewriter.update(Import(importidx=idx), Import(module=module_name, name=func_name, typeidx=typeidx))
+
+        def append_import_function(self, module_name, func_name, params_type, results_type):
+            type_rewriter = SectionRewriter(self.module, typesec=self.module.type_sec)
+            result = type_rewriter.select(Type(arg_types=params_type, ret_types=results_type))
+            if result == []:
+                type_rewriter.insert(None, inserted_item=Type(arg_types=params_type, ret_types=results_type))
+                typeidx = type_rewriter.select(Type())[-1].typeidx
+            else:
+                typeidx = result[0].typeidx
+
+            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
+            import_rewriter.insert(None, inserted_item=Import(module=module_name, name=func_name, typeidx=typeidx))
+
+        def insert_export_function(self, idx, func_name, funcidx):
+
+            export_rewriter = SectionRewriter(self.module, exportsec=self.module.export_sec)
+            export_rewriter.insert(Export(exportidx=idx), Export(name=func_name, funcidx=funcidx))
+
+        def modify_export_function(self, idx, func_name, funcidx):
+
+            export_rewriter = SectionRewriter(self.module, exportsec=self.module.export_sec)
+            export_rewriter.update(Export(exportidx=idx), Export(name=func_name, funcidx=funcidx))
+
+        def delete_export_function(self, idx=None, func_name=None):
+
+            if idx is not None:
+                export_rewriter = SectionRewriter(self.module, exportsec=self.module.export_sec)
+                export_rewriter.delete(Export(exportidx=idx))
+                return
+            if func_name is not None:
+                export_rewriter = SectionRewriter(self.module, exportsec=self.module.export_sec)
+                export_function = export_rewriter.select(Export(name=func_name))
+                export_rewriter.delete(export_function[0].exportidx)
+
+        def append_export_function(self, func_name, funcidx):
+
+            export_rewriter = SectionRewriter(self.module, exportsec=self.module.export_sec)
+            export_rewriter.insert(None, inserted_item=Export(name=func_name, funcidx=funcidx))
+
+        # def insert_import_global_variable(self, idx, module_name, variable_name, valtype):
+        #     import_variable = Import(module_name, variable_name, ImportDesc(3, global_type=valtype))
+        #     for _, import_item in enumerate(self.module.import_sec):
+        #         if import_item == import_variable:
+        #             raise Exception("The global variable already exists")
+        #     self.section_rewriter.insert_importsec_import(idx, import_variable)
+        #
+        #     # fix
+        #     pass
+        #
+        # def modify_import_global_variable(self, idx, module_name, variable_name, valtype):
+        #     import_variable = Import(module_name, variable_name, ImportDesc(3, global_type=valtype))
+        #     for _, import_item in enumerate(self.module.import_sec):
+        #         if import_item == import_variable:
+        #             raise Exception("The global variable already exists")
+        #     self.module.import_sec[idx] = import_variable
+        #
+        #     # fix
+        #     for code in self.section_rewriter.get_codesec_code_list():
+        #         self.indices_fixer.fix_global_instructions(code.expr, idx)
+        #
+        # def insert_import_memory(self, idx, module_name, memory_name, limits):
+        #     mem_list = self.section_rewriter.get_mem_list()
+        #     memidx = None
+        #     for _, mem in enumerate(mem_list):
+        #         if mem == limits:
+        #             memidx = _
+        #     if memidx is None:
+        #         memidx = self.section_rewriter.append_memsec_mem(limits)
+        #
+        #     import_mem = Import(module_name, memory_name, ImportDesc(2, mem=memidx))
+        #     self.section_rewriter.insert_importsec_import(idx, import_mem)
+        #
+        #     # fix
+        #     pass
+        #
+        # def modify_import_memory(self, idx, module_name, memory_name, limits):
+        #     mem_list = self.section_rewriter.get_mem_list()
+        #     memidx = None
+        #     for _, mem in enumerate(mem_list):
+        #         if mem == limits:
+        #             memidx = _
+        #     if memidx is None:
+        #         memidx = self.section_rewriter.append_memsec_mem(limits)
+        #
+        #     import_mem = Import(module_name, memory_name, ImportDesc(2, mem=memidx))
+        #     self.module.import_sec[idx] = import_mem
+        #
+        # def insert_import_table(self, idx, module_name, table_name, limits):
+        #     table_list = self.section_rewriter.get_table_list()
+        #     tableidx = None
+        #     for _, table in enumerate(table_list):
+        #         if table == limits:
+        #             tableidx = _
+        #     if tableidx is None:
+        #         tableidx = self.section_rewriter.append_tablesec_table(limits)
+        #
+        #     import_table = Import(module_name, table_name, ImportDesc(1, table=tableidx))
+        #     self.section_rewriter.insert_importsec_import(idx, import_table)
+        #
+        # def modify_import_table(self, idx, module_name, table_name, limits):
+        #     table_list = self.section_rewriter.get_table_list()
+        #     tableidx = None
+        #     for _, table in enumerate(table_list):
+        #         if table == limits:
+        #             tableidx = _
+        #     if tableidx is None:
+        #         tableidx = self.section_rewriter.append_tablesec_table(limits)
+        #
+        #     import_table = Import(module_name, table_name, ImportDesc(1, table=tableidx))
+        #     self.module.import_sec[idx] = import_table
+
+    class LinearMemory:
+        def __init__(self, module):
+            self.module = module
+            self.indices_fixer = IndicesFixer(self.module)
+
+        def insert_linear_memory(self, offset, bytes):
+            memory_rewriter = SectionRewriter(self.module, memsec=self.module.mem_sec)
+            memory_list = memory_rewriter.select(Memory())
+
+            if memory_list[0].max != 0 and offset + len(bytes) + 1 > memory_list[0].max * 65536:
+                raise Exception("Memory out of bounds")
+
+            data_rewriter = SectionRewriter(self.module, datasec=self.module.data_sec)
+
+            is_overlap = False
+            length = len(bytes)
+            for data_item in data_rewriter.select(Data()):
+                if offset + length < data_item.offset:
+                    is_overlap = False
+                elif data_item.offset + len(data_item.init_data) < offset:
+                    is_overlap = False
+                elif offset + length >= data_item.offset:
+                    is_overlap = True
+                    if offset >= data_item.offset:
+                        data_item.init_data = data_item.init_data[:(offset - data_item.offset)] + bytearray(
+                            bytes) + data_item.init_data[(offset - data_item.offset):]
+                    else:
+                        data_item.offset -= (offset - data_item.offset)
+                        data_item.init_data = bytearray(bytes) + data_item.init_data
+
+                self.indices_fixer.fix_memory_limits(self.module.mem_sec, offset + length)
+
+            if data_rewriter.select(Data()) is [] or is_overlap is False:
+                data_rewriter.insert(None, inserted_item=Data(offset=offset, init_data=bytes))
+
+        def append_linear_memory(self, page_num):
+            memory_rewriter = SectionRewriter(self.module, memsec=self.module.mem_sec)
+            mem_list = memory_rewriter.select(Memory())
+
+            if mem_list[0].max != 0:
+                mem_list[0].max += page_num
+
+        def modify_linear_memory(self, offset, bytes):
+            memory_rewriter = SectionRewriter(self.module, memsec=self.module.mem_sec)
+            mem_list = memory_rewriter.select(Memory())
+
+            if mem_list[0].max != 0 and offset + len(bytes) + 1 > mem_list[0].max * 65536:
+                raise Exception("Memory out of bounds")
+
+            data_rewriter = SectionRewriter(self.module, datasec=self.module.data_sec)
+            data_rewriter.insert(None, inserted_item=Data(offset=offset, init_data=bytes))
+
+    class Function:
+        def __init__(self, module):
+            self.module = module
+
+        def insert_internal_function(self, idx, params_type, results_type, local_vec, func_body):
+
+            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
+            import_func_num = len(import_rewriter.select(Import()))
+
+            if import_func_num > idx:
+                raise Exception("The idx of internal function less than import function")
+
+            type_rewriter = SectionRewriter(self.module, typesec=self.module.type_sec)
+            result = type_rewriter.select(Type(arg_types=params_type, ret_types=results_type))
+            if result == []:
+                type_rewriter.insert(None, inserted_item=Type(arg_types=params_type, ret_types=results_type))
+                typeidx = type_rewriter.select(Type())[-1].typeidx
+            else:
+                typeidx = result[0].typeidx
+
+            function_rewriter = SectionRewriter(self.module, funcsec=self.module.func_sec)
+            function_rewriter.insert(Function(funcidx=idx), Function(typeidx=typeidx))
+
+            code_rewriter = SectionRewriter(self.module, codesec=self.module.code_sec)
+            code_rewriter.insert(Code(funcidx=idx), Code(local_vec=local_vec, instr_list=func_body))
+
+        def insert_indirect_function(self, idx, params_type, results_type, local_vec, func_body):
+
+            self.insert_internal_function(idx, params_type, results_type, local_vec, func_body)
+
+            element_rewriter = SectionRewriter(self.module, elemsec=self.module.elem_sec)
+
+            # get original indirect function list
+            indirect_func_list = []
+            for elem in element_rewriter.select(Element()):
+                indirect_func_list.extend(elem.funcidx_list)
+
+            element_list = element_rewriter.select(Element())
+
+            if not element_list:
+                element_rewriter.insert(None, inserted_item=Element(tableidx=0, offset=1, funcidx_list=[idx]))
+            else:
+                element_list[0].funcidx_list.append(idx)
+                element_rewriter.update(Element(elemidx=element_list[0].elemidx), element_list[0])
+
+        def insert_hook_function(self, hooked_funcidx, idx, params_type, results_type, locals_vec, func_body):
+            self.insert_internal_function(idx, params_type, results_type, locals_vec, func_body)
+
+            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
+            import_func_num = len(import_rewriter.select(Import()))
+
+            code_rewriter = SectionRewriter(self.module, codesec=self.module.code_sec)
+
+            for funcidx in range(import_func_num, import_func_num + len(code_rewriter.select(Code()))):
+                if funcidx != idx:
+                    code = code_rewriter.select(Code(funcidx=funcidx))
+                    for instr in code.instr_list:
+                        if instr == Instruction(Call, hooked_funcidx):
+                            instr.opcode = Call
+                            instr.args = idx
+                    code_rewriter.update(Code(funcidx=funcidx), Code(instr_list=code.instr_list))
+
+            return idx
+
+        # def change_func_instr(self, binary, funcidx, offset, instr):
+        #     import_func_num = self.section_rewriter.get_import_func_num()
+        #     if funcidx < import_func_num:
+        #         raise Exception("funcidx error")
+        #     code = self.section_rewriter.get_codesec_code(binary, funcidx - import_func_num)
+        #
+        #     self.section_rewriter.modify_code_instr(code, offset, instr)
+
+        def delete_func_instr(self, funcidx, offset):
+
+            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
+            import_func_num = len(import_rewriter.select(Import()))
+
+            if funcidx < import_func_num:
+                raise Exception("funcidx error")
+
+            code_rewriter = SectionRewriter(self.module, codesec=self.module.code_sec)
+            code_list = code_rewriter.select(Code(funcidx=funcidx))
+
+            code_list[0].instr_list.pop(offset)
+            code_rewriter.update(Code(funcidx=funcidx), code_list[0])
+
+        def insert_func_instrs(self, funcidx, offset, instrs: list):
+
+            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
+            import_func_num = len(import_rewriter.select(Import()))
+
+            if funcidx < import_func_num:
+                raise Exception("funcidx error")
+
+            code_rewriter = SectionRewriter(self.module, codesec=self.module.code_sec)
+            code_list = code_rewriter.select(Code(funcidx=funcidx))
+
+            for i in reversed(instrs):
+                code_list[0].instr_list.insert(offset, i)
+
+            code_rewriter.update(Code(funcidx=funcidx), code_list[0])
+
+        def append_func_instrs(self, funcidx, instrs: list):
+
+            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
+            import_func_num = len(import_rewriter.select(Import()))
+
+            if funcidx < import_func_num:
+                raise Exception("funcidx error")
+
+            code_rewriter = SectionRewriter(self.module, codesec=self.module.code_sec)
+            code_list = code_rewriter.select(Code(funcidx=funcidx))
+
+            code_list[0].instr_list.extend(instrs)
+            code_rewriter.update(Code(funcidx=funcidx), code_list[0])
+
+        def modify_func_instrs(self, funcidx, instr, instrs: list):
+            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
+            import_func_num = len(import_rewriter.select(Import()))
+
+            if funcidx < import_func_num:
+                raise Exception("funcidx error")
+
+            code_rewriter = SectionRewriter(self.module, codesec=self.module.code_sec)
+            code_list = code_rewriter.select(Code(funcidx=funcidx))
+
+            i = 0
+            while i < len(code_list[0].instr_list):
+                if code_list[0].instr_list[i].opcode == instr.opcode and code_list[0].instr_list[i].args == instr.args:
+                    code_list[0].instr_list.pop(i)
+                    for j in reversed(instrs):
+                        code_list[0].instr_list.insert(i, j)
+                    i += len(instrs)
+                else:
+                    i += 1
+
+
+            code_rewriter.update(Code(funcidx=funcidx), Code(instr_list=code_list[0].instr_list))
+
+        def append_func_local(self, funcidx, valtype):
+            import_rewriter = SectionRewriter(self.module, importsec=self.module.import_sec)
+            import_func_num = len(import_rewriter.select(Import()))
+
+            if funcidx < import_func_num:
+                raise Exception("funcidx error")
+
+            code_rewriter = SectionRewriter(self.module, codesec=self.module.code_sec)
+            code = code_rewriter.select(Code(funcidx=funcidx))
+            code[0].local_vec.append(Local(len(code[0].local_vec), valtype))
+
+            code_rewriter.update(Code(funcidx=funcidx), Code(local_vec=code[0].local_vec))
+
+    class CustomContent:
+        def __init__(self, module):
+            self.module = module
+
+        def modify_func_name(self, funcidx, name):
+            namesec = self.section_rewriter.get_customsec_custom(name="name")
+            funcname_list = self.section_rewriter.get_namesec_funcname_list(namesec)
+            for _, funcname in enumerate(funcname_list):
+                if funcname.idx == funcidx:
+                    funcname_list[_].name = name
+
+        def delete_func_name(self, funcidx):
+            namesec = self.section_rewriter.get_customsec_custom(name="name")
+            funcname_list = self.section_rewriter.get_namesec_funcname_list(namesec)
+            for _, funcname in enumerate(funcname_list):
+                if funcname.idx == funcidx:
+                    funcname_list.pop(_)
+
+        def insert_func_name(self, funcidx, name):
+            namesec = self.section_rewriter.get_customsec_custom(name="name")
+            funcname_list = self.section_rewriter.get_namesec_funcname_list(namesec)
+            for _, funcname in enumerate(funcname_list):
+                if funcname.idx == (funcidx - 1):
+                    funcname_list.insert(_ + 1, NameAssoc(funcidx, name))
+                    return
+
+        def insert_global_name(self, globalidx, name):
+            namesec = self.section_rewriter.get_customsec_custom(name="name")
+            globalname_list = self.section_rewriter.get_namesec_globalname_list(namesec)
+            globalname_list.insert(globalidx, NameAssoc(globalidx, name))
+
+        def delete_global_name(self, globalidx):
+            namesec = self.section_rewriter.get_customsec_custom(name="name")
+            globalname_list = self.section_rewriter.get_namesec_globalname_list(namesec)
+            globalname_list.pop(globalidx)
+
+        def modify_global_name(self, globalidx, name):
+            namesec = self.section_rewriter.get_customsec_custom(name="name")
+            globalname_list = self.section_rewriter.get_namesec_globalname_list(namesec)
+            globalname_list[globalidx].name = name
+
+        def insert_data_name(self, dataidx, name):
+            namesec = self.section_rewriter.get_customsec_custom(name="name")
+            dataname_list = self.section_rewriter.get_namesec_dataname_list(namesec)
+            dataname_list.insert(dataidx, NameAssoc(dataidx, name))
+
+        def delete_data_name(self, dataidx):
+            namesec = self.section_rewriter.get_customsec_custom(name="name")
+            dataname_list = self.section_rewriter.get_namesec_dataname_list(namesec)
+            dataname_list.pop(dataidx)
+
+        def modify_data_name(self, dataidx, name):
+            namesec = self.section_rewriter.get_customsec_custom(name="name")
+            dataname_list = self.section_rewriter.get_namesec_dataname_list(namesec)
+            dataname_list[dataidx].name = name
```

### Comparing `BREWasm-1.0.0/BREWasm.egg-info/PKG-INFO` & `BREWasm-1.0.1/BREWasm.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-Metadata-Version: 2.1
-Name: BREWasm
-Version: 1.0.0
-Summary: A general purpose static binary rewriting framework for Wasm, which aims at reducing the complexity of the Wasm
-Home-page: https://github.com/BREWasm/brewasm-project
-Author: BREWasm
-License: MIT
-Keywords: BINARY,REWRITER,WASM
-Description-Content-Type: text/markdown
-
-﻿# BREWasm
-
-BREWasm: A general purpose static binary rewriting framework for Wasm, which aims at reducing the complexity of the Wasm
-binary format.
-
-## Features
-
-BREWasm consists of four key components: the Wasm Parser, section rewriter, semantics rewriter, and Wasm Encoder. The
-Wasm parser and encoder are built using our abstraction of the Wasm binary, which is represented as a formal format
-comprising a list of objects. The parser and encoder effectively convert the Wasm binary and an array of objects into
-each other, with each object containing multiple attributes.
-
-<div align=center>
-<img src="doc/Definition.png" width="600">
-  <div style="margin-top: 10px; margin-bottom: 10px">
-    <b>Formal definition of sections, elements and fields in Wasm.</b>
-  </div>
-</div>  
-
-- The section rewriter directly interacts with the formal definition, e.g., inserting/deleting a new object or modifying
-  attributes of existing objects. It packs these fine-grained rewriting functions into APIs.
-- The semantics rewriter further combines the fine-grained APIs of section rewriter and offers another set of high-level
-  APIs, where each of them possesses rich semantics as following, like inserting a function, and append a piece of
-  linear memory.
-    - Global Variables
-    - Import & Export
-    - Linear Memory
-    - Function
-    - Custom Content
-
-## Installation
-
-### Python package
-
-BREWasm is currently available on PIP repositories.
-
-Install BREWasm::
-
-```
-pip install BREWasm
-```
-
-
-## Examples
-
-### Section Rewriter
-
-The basic operation of the section rewriter is `select`, `insert`, `update` and `delete`.
-
-```python
-# ---------- some_tests.py ----------
-from BREWasm import *
-
-binary = BREWasm('a.wasm')  # Open a Wasm binary file
-
-# Initialize a section rewriter of the global section. 
-global_rewriter = SectionRewriter(self.binary.module, self.binary.module.global_sec)
-
-# Select all the items in global section
-global_list = global_rewriter.select()
-# Get the attribute globalidx of a global item, whose index is one.
-idx = global_list[1].globalidx
-# Insert a new global item at the index idx of the global section
-global_rewriter.insert(Global(idx), Global(valtype=I32, val=100))
-# Delete the global item whose index is idx.
-global_rewriter.delete(Global(idx))
-# Emit a new binary file
-binary.emit_binary('b.wasm')
-```
-
-### Semantics Rewriter
-
-```python
-from BREWasm import *
-
-binary = BREWasm('a.wasm')  # Open a Wasm binary file
-
-# Initialize a semantics rewriter of the function semantics
-function_rewriter = SemanticRewriter.Function(binary)
-# Define the instructions of function
-funcbody = [Instruction(LocalGet, 0), Instruction(LocalGet, 1), Instruction(I32Add, 0), Instruction(Nop)]
-# Insert a internal function in the binary
-function_rewriter.insert_internal_function(idx=1, params_type=[I32, I32], results_type=[I32],
-                                           local_vec=[Local(0, I32), Local(1, I64)], funcbody)
-# Emit a new binary file
-binary.emit_binary('b.wasm')
-```
-
-## Documentation
-
-The complete documentation can be found [here](https://brewasm-project.readthedocs.io/en/latest/).
+Metadata-Version: 2.1
+Name: BREWasm
+Version: 1.0.1
+Summary: A general purpose static binary rewriting framework for Wasm, which aims at reducing the complexity of the Wasm
+Home-page: https://github.com/BREWasm/brewasm-project
+Author: BREWasm
+License: MIT
+Keywords: BINARY,REWRITER,WASM
+Description-Content-Type: text/markdown
+
+﻿# BREWasm
+
+BREWasm: A general purpose static binary rewriting framework for Wasm, which aims at reducing the complexity of the Wasm
+binary format.
+
+## Features
+
+BREWasm consists of four key components: the Wasm Parser, section rewriter, semantics rewriter, and Wasm Encoder. The
+Wasm parser and encoder are built using our abstraction of the Wasm binary, which is represented as a formal format
+comprising a list of objects. The parser and encoder effectively convert the Wasm binary and an array of objects into
+each other, with each object containing multiple attributes.
+
+<div align=center>
+<img src="doc/Definition.png" width="600">
+  <div style="margin-top: 10px; margin-bottom: 10px">
+    <b>Formal definition of sections, elements and fields in Wasm.</b>
+  </div>
+</div>  
+
+- The section rewriter directly interacts with the formal definition, e.g., inserting/deleting a new object or modifying
+  attributes of existing objects. It packs these fine-grained rewriting functions into APIs.
+- The semantics rewriter further combines the fine-grained APIs of section rewriter and offers another set of high-level
+  APIs, where each of them possesses rich semantics as following, like inserting a function, and append a piece of
+  linear memory.
+    - Global Variables
+    - Import & Export
+    - Linear Memory
+    - Function
+    - Custom Content
+
+## Installation
+
+### Python package
+
+BREWasm is currently available on PIP repositories.
+
+Install BREWasm::
+
+```
+pip install BREWasm
+```
+
+
+## Examples
+
+### Section Rewriter
+
+The basic operation of the section rewriter is `select`, `insert`, `update` and `delete`.
+
+```python
+# ---------- some_tests.py ----------
+from BREWasm import *
+
+binary = BREWasm('a.wasm')  # Open a Wasm binary file
+
+# Initialize a section rewriter of the global section. 
+global_rewriter = SectionRewriter(self.binary.module, globalsec=self.binary.module.global_sec)
+
+# Select all the items in global section
+global_list = global_rewriter.select(Global())
+# Get the attribute globalidx of a global item, whose index is one.
+idx = global_list[1].globalidx
+# Insert a new global item at the index idx of the global section
+global_rewriter.insert(Global(idx), Global(valtype=I32, val=100))
+# Delete the global item whose index is idx.
+global_rewriter.delete(Global(idx))
+# Emit a new binary file
+binary.emit_binary('b.wasm')
+```
+
+### Semantics Rewriter
+
+```python
+from BREWasm import *
+
+binary = BREWasm('a.wasm')  # Open a Wasm binary file
+
+# Initialize a semantics rewriter of the function semantics
+function_rewriter = SemanticRewriter.Function(binary.module)
+# Define the instructions of function
+funcbody = [Instruction(LocalGet, 0), Instruction(LocalGet, 1), Instruction(I32Add, 0), Instruction(Nop)]
+# Insert a internal function in the binary
+function_rewriter.insert_internal_function(idx=1, params_type=[I32, I32], results_type=[I32],
+                                           local_vec=[Local(0, I32), Local(1, I64)], funcbody)
+# Emit a new binary file
+binary.emit_binary('b.wasm')
+```
+
+## Documentation
+
+The complete documentation can be found [here](https://brewasm-project.readthedocs.io/en/latest/).
```

### Comparing `BREWasm-1.0.0/BREWasm.egg-info/SOURCES.txt` & `BREWasm-1.0.1/BREWasm.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -17,10 +17,8 @@
 BREWasm/rewriter/BREWasm.py
 BREWasm/rewriter/__init__.py
 BREWasm/rewriter/defination.py
 BREWasm/rewriter/indices_fixer.py
 BREWasm/rewriter/modify_binary.py
 BREWasm/rewriter/section_rewriter.py
 BREWasm/rewriter/semantics_rewriter.py
-doc/Definition.png
-test/test.py
-test/test_other.py
+doc/Definition.png
```

### Comparing `BREWasm-1.0.0/PKG-INFO` & `BREWasm-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-Metadata-Version: 2.1
-Name: BREWasm
-Version: 1.0.0
-Summary: A general purpose static binary rewriting framework for Wasm, which aims at reducing the complexity of the Wasm
-Home-page: https://github.com/BREWasm/brewasm-project
-Author: BREWasm
-License: MIT
-Keywords: BINARY,REWRITER,WASM
-Description-Content-Type: text/markdown
-
-﻿# BREWasm
-
-BREWasm: A general purpose static binary rewriting framework for Wasm, which aims at reducing the complexity of the Wasm
-binary format.
-
-## Features
-
-BREWasm consists of four key components: the Wasm Parser, section rewriter, semantics rewriter, and Wasm Encoder. The
-Wasm parser and encoder are built using our abstraction of the Wasm binary, which is represented as a formal format
-comprising a list of objects. The parser and encoder effectively convert the Wasm binary and an array of objects into
-each other, with each object containing multiple attributes.
-
-<div align=center>
-<img src="doc/Definition.png" width="600">
-  <div style="margin-top: 10px; margin-bottom: 10px">
-    <b>Formal definition of sections, elements and fields in Wasm.</b>
-  </div>
-</div>  
-
-- The section rewriter directly interacts with the formal definition, e.g., inserting/deleting a new object or modifying
-  attributes of existing objects. It packs these fine-grained rewriting functions into APIs.
-- The semantics rewriter further combines the fine-grained APIs of section rewriter and offers another set of high-level
-  APIs, where each of them possesses rich semantics as following, like inserting a function, and append a piece of
-  linear memory.
-    - Global Variables
-    - Import & Export
-    - Linear Memory
-    - Function
-    - Custom Content
-
-## Installation
-
-### Python package
-
-BREWasm is currently available on PIP repositories.
-
-Install BREWasm::
-
-```
-pip install BREWasm
-```
-
-
-## Examples
-
-### Section Rewriter
-
-The basic operation of the section rewriter is `select`, `insert`, `update` and `delete`.
-
-```python
-# ---------- some_tests.py ----------
-from BREWasm import *
-
-binary = BREWasm('a.wasm')  # Open a Wasm binary file
-
-# Initialize a section rewriter of the global section. 
-global_rewriter = SectionRewriter(self.binary.module, self.binary.module.global_sec)
-
-# Select all the items in global section
-global_list = global_rewriter.select()
-# Get the attribute globalidx of a global item, whose index is one.
-idx = global_list[1].globalidx
-# Insert a new global item at the index idx of the global section
-global_rewriter.insert(Global(idx), Global(valtype=I32, val=100))
-# Delete the global item whose index is idx.
-global_rewriter.delete(Global(idx))
-# Emit a new binary file
-binary.emit_binary('b.wasm')
-```
-
-### Semantics Rewriter
-
-```python
-from BREWasm import *
-
-binary = BREWasm('a.wasm')  # Open a Wasm binary file
-
-# Initialize a semantics rewriter of the function semantics
-function_rewriter = SemanticRewriter.Function(binary)
-# Define the instructions of function
-funcbody = [Instruction(LocalGet, 0), Instruction(LocalGet, 1), Instruction(I32Add, 0), Instruction(Nop)]
-# Insert a internal function in the binary
-function_rewriter.insert_internal_function(idx=1, params_type=[I32, I32], results_type=[I32],
-                                           local_vec=[Local(0, I32), Local(1, I64)], funcbody)
-# Emit a new binary file
-binary.emit_binary('b.wasm')
-```
-
-## Documentation
-
-The complete documentation can be found [here](https://brewasm-project.readthedocs.io/en/latest/).
+Metadata-Version: 2.1
+Name: BREWasm
+Version: 1.0.1
+Summary: A general purpose static binary rewriting framework for Wasm, which aims at reducing the complexity of the Wasm
+Home-page: https://github.com/BREWasm/brewasm-project
+Author: BREWasm
+License: MIT
+Keywords: BINARY,REWRITER,WASM
+Description-Content-Type: text/markdown
+
+﻿# BREWasm
+
+BREWasm: A general purpose static binary rewriting framework for Wasm, which aims at reducing the complexity of the Wasm
+binary format.
+
+## Features
+
+BREWasm consists of four key components: the Wasm Parser, section rewriter, semantics rewriter, and Wasm Encoder. The
+Wasm parser and encoder are built using our abstraction of the Wasm binary, which is represented as a formal format
+comprising a list of objects. The parser and encoder effectively convert the Wasm binary and an array of objects into
+each other, with each object containing multiple attributes.
+
+<div align=center>
+<img src="doc/Definition.png" width="600">
+  <div style="margin-top: 10px; margin-bottom: 10px">
+    <b>Formal definition of sections, elements and fields in Wasm.</b>
+  </div>
+</div>  
+
+- The section rewriter directly interacts with the formal definition, e.g., inserting/deleting a new object or modifying
+  attributes of existing objects. It packs these fine-grained rewriting functions into APIs.
+- The semantics rewriter further combines the fine-grained APIs of section rewriter and offers another set of high-level
+  APIs, where each of them possesses rich semantics as following, like inserting a function, and append a piece of
+  linear memory.
+    - Global Variables
+    - Import & Export
+    - Linear Memory
+    - Function
+    - Custom Content
+
+## Installation
+
+### Python package
+
+BREWasm is currently available on PIP repositories.
+
+Install BREWasm::
+
+```
+pip install BREWasm
+```
+
+
+## Examples
+
+### Section Rewriter
+
+The basic operation of the section rewriter is `select`, `insert`, `update` and `delete`.
+
+```python
+# ---------- some_tests.py ----------
+from BREWasm import *
+
+binary = BREWasm('a.wasm')  # Open a Wasm binary file
+
+# Initialize a section rewriter of the global section. 
+global_rewriter = SectionRewriter(self.binary.module, globalsec=self.binary.module.global_sec)
+
+# Select all the items in global section
+global_list = global_rewriter.select(Global())
+# Get the attribute globalidx of a global item, whose index is one.
+idx = global_list[1].globalidx
+# Insert a new global item at the index idx of the global section
+global_rewriter.insert(Global(idx), Global(valtype=I32, val=100))
+# Delete the global item whose index is idx.
+global_rewriter.delete(Global(idx))
+# Emit a new binary file
+binary.emit_binary('b.wasm')
+```
+
+### Semantics Rewriter
+
+```python
+from BREWasm import *
+
+binary = BREWasm('a.wasm')  # Open a Wasm binary file
+
+# Initialize a semantics rewriter of the function semantics
+function_rewriter = SemanticRewriter.Function(binary.module)
+# Define the instructions of function
+funcbody = [Instruction(LocalGet, 0), Instruction(LocalGet, 1), Instruction(I32Add, 0), Instruction(Nop)]
+# Insert a internal function in the binary
+function_rewriter.insert_internal_function(idx=1, params_type=[I32, I32], results_type=[I32],
+                                           local_vec=[Local(0, I32), Local(1, I64)], funcbody)
+# Emit a new binary file
+binary.emit_binary('b.wasm')
+```
+
+## Documentation
+
+The complete documentation can be found [here](https://brewasm-project.readthedocs.io/en/latest/).
```

### Comparing `BREWasm-1.0.0/README.md` & `BREWasm-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,18 +50,18 @@
 ```python
 # ---------- some_tests.py ----------
 from BREWasm import *
 
 binary = BREWasm('a.wasm')  # Open a Wasm binary file
 
 # Initialize a section rewriter of the global section. 
-global_rewriter = SectionRewriter(self.binary.module, self.binary.module.global_sec)
+global_rewriter = SectionRewriter(self.binary.module, globalsec=self.binary.module.global_sec)
 
 # Select all the items in global section
-global_list = global_rewriter.select()
+global_list = global_rewriter.select(Global())
 # Get the attribute globalidx of a global item, whose index is one.
 idx = global_list[1].globalidx
 # Insert a new global item at the index idx of the global section
 global_rewriter.insert(Global(idx), Global(valtype=I32, val=100))
 # Delete the global item whose index is idx.
 global_rewriter.delete(Global(idx))
 # Emit a new binary file
@@ -72,15 +72,15 @@
 
 ```python
 from BREWasm import *
 
 binary = BREWasm('a.wasm')  # Open a Wasm binary file
 
 # Initialize a semantics rewriter of the function semantics
-function_rewriter = SemanticRewriter.Function(binary)
+function_rewriter = SemanticRewriter.Function(binary.module)
 # Define the instructions of function
 funcbody = [Instruction(LocalGet, 0), Instruction(LocalGet, 1), Instruction(I32Add, 0), Instruction(Nop)]
 # Insert a internal function in the binary
 function_rewriter.insert_internal_function(idx=1, params_type=[I32, I32], results_type=[I32],
                                            local_vec=[Local(0, I32), Local(1, I64)], funcbody)
 # Emit a new binary file
 binary.emit_binary('b.wasm')
```

### Comparing `BREWasm-1.0.0/doc/Definition.png` & `BREWasm-1.0.1/doc/Definition.png`

 * *Files identical despite different names*

### Comparing `BREWasm-1.0.0/setup.py` & `BREWasm-1.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# setup.py
-from setuptools import setup, find_packages
-
-with open('README.md', encoding='UTF-16LE') as f:
-  long_description = f.read()
-
-setup(name='BREWasm',
-      version='1.0.0',
-      description='A general purpose static binary rewriting framework for Wasm, which aims at reducing the complexity of the Wasm',
-      long_description=long_description,
-      long_description_content_type='text/markdown',
-      packages=find_packages(),
-      url='https://github.com/BREWasm/brewasm-project',
-      author='BREWasm',
-      license='MIT',
-      keywords=['BINARY', 'REWRITER', 'WASM'],
-      data_files=[('images', ['doc/Definition.png'])],
+# setup.py
+from setuptools import setup, find_packages
+
+with open('README.md', encoding='UTF-16LE') as f:
+  long_description = f.read()
+
+setup(name='BREWasm',
+      version='1.0.1',
+      description='A general purpose static binary rewriting framework for Wasm, which aims at reducing the complexity of the Wasm',
+      long_description=long_description,
+      long_description_content_type='text/markdown',
+      packages=find_packages(),
+      url='https://github.com/BREWasm/brewasm-project',
+      author='BREWasm',
+      license='MIT',
+      keywords=['BINARY', 'REWRITER', 'WASM'],
+      data_files=[('images', ['doc/Definition.png'])],
       )
```

