# Comparing `tmp/supGecko-0.1.0a2.tar.gz` & `tmp/supGecko-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supGecko-0.1.0a2.tar", last modified: Tue Jul 11 07:55:16 2023, max compression
+gzip compressed data, was "supGecko-0.1.0a3.tar", last modified: Tue Jul 11 17:14:48 2023, max compression
```

## Comparing `supGecko-0.1.0a2.tar` & `supGecko-0.1.0a3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 07:55:16.954265 supGecko-0.1.0a2/
--rw-rw-rw-   0        0        0     1083 2023-07-11 07:31:46.000000 supGecko-0.1.0a2/LICENSE
--rw-rw-rw-   0        0        0      694 2023-07-11 07:55:16.954265 supGecko-0.1.0a2/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-07-11 07:41:27.000000 supGecko-0.1.0a2/README.md
--rw-rw-rw-   0        0        0       88 2022-10-14 08:59:04.000000 supGecko-0.1.0a2/pyproject.toml
--rw-rw-rw-   0        0        0      623 2023-07-11 07:55:16.954769 supGecko-0.1.0a2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-11 07:55:16.942551 supGecko-0.1.0a2/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 07:55:16.945592 supGecko-0.1.0a2/src/supGecko/
--rw-rw-rw-   0        0        0       24 2023-07-11 07:36:14.000000 supGecko-0.1.0a2/src/supGecko/__init__.py
--rw-rw-rw-   0        0        0     8608 2023-07-11 07:54:08.000000 supGecko-0.1.0a2/src/supGecko/lib.py
-drwxrwxrwx   0        0        0        0 2023-07-11 07:55:16.953262 supGecko-0.1.0a2/src/supGecko.egg-info/
--rw-rw-rw-   0        0        0      694 2023-07-11 07:55:16.000000 supGecko-0.1.0a2/src/supGecko.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-07-11 07:55:16.000000 supGecko-0.1.0a2/src/supGecko.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 07:55:16.000000 supGecko-0.1.0a2/src/supGecko.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-11 07:55:16.000000 supGecko-0.1.0a2/src/supGecko.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 17:14:48.815069 supGecko-0.1.0a3/
+-rw-rw-rw-   0        0        0     1083 2023-07-11 07:31:46.000000 supGecko-0.1.0a3/LICENSE
+-rw-rw-rw-   0        0        0      694 2023-07-11 17:14:48.815069 supGecko-0.1.0a3/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-07-11 07:41:27.000000 supGecko-0.1.0a3/README.md
+-rw-rw-rw-   0        0        0       88 2022-10-14 08:59:04.000000 supGecko-0.1.0a3/pyproject.toml
+-rw-rw-rw-   0        0        0      623 2023-07-11 17:14:48.818068 supGecko-0.1.0a3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 17:14:48.802068 supGecko-0.1.0a3/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 17:14:48.807070 supGecko-0.1.0a3/src/supGecko/
+-rw-rw-rw-   0        0        0       88 2023-07-11 16:14:27.000000 supGecko-0.1.0a3/src/supGecko/__init__.py
+-rw-rw-rw-   0        0        0     2675 2023-07-11 17:13:46.000000 supGecko-0.1.0a3/src/supGecko/asm.py
+-rw-rw-rw-   0        0        0     9895 2023-07-11 17:12:22.000000 supGecko-0.1.0a3/src/supGecko/gecko.py
+drwxrwxrwx   0        0        0        0 2023-07-11 17:14:48.814068 supGecko-0.1.0a3/src/supGecko.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-07-11 17:14:48.000000 supGecko-0.1.0a3/src/supGecko.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-07-11 17:14:48.000000 supGecko-0.1.0a3/src/supGecko.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 17:14:48.000000 supGecko-0.1.0a3/src/supGecko.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-11 17:14:48.000000 supGecko-0.1.0a3/src/supGecko.egg-info/top_level.txt
```

### Comparing `supGecko-0.1.0a2/LICENSE` & `supGecko-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `supGecko-0.1.0a2/PKG-INFO` & `supGecko-0.1.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supGecko
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A helper library to write Gecko code
 Home-page: https://github.com/sup39/supGecko
 Author: sup39
 Author-email: sms@sup39.dev
 License: MIT
 Project-URL: Bug Tracker, https://github.com/sup39/supGecko/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `supGecko-0.1.0a2/setup.cfg` & `supGecko-0.1.0a3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7570 4765 636b 6f0d 0a76 6572   = supGecko..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e30 6132 0d0a  sion = 0.1.0a2..
+00000020: 7369 6f6e 203d 2030 2e31 2e30 6133 0d0a  sion = 0.1.0a3..
 00000030: 6175 7468 6f72 203d 2073 7570 3339 0d0a  author = sup39..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2073  author_email = s
 00000050: 6d73 4073 7570 3339 2e64 6576 0d0a 6465  ms@sup39.dev..de
 00000060: 7363 7269 7074 696f 6e20 3d20 4120 6865  scription = A he
 00000070: 6c70 6572 206c 6962 7261 7279 2074 6f20  lper library to 
 00000080: 7772 6974 6520 4765 636b 6f20 636f 6465  write Gecko code
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `supGecko-0.1.0a2/src/supGecko/lib.py` & `supGecko-0.1.0a3/src/supGecko/gecko.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2023 sup39
+
+from .asm import compile
+
 def cw_addr(ct, addr, po, endif=False):
   return (ct+0x10 if po else ct)<<24 | (addr+1 if endif else addr)&0x1ff_ffff
 def cw_go(ct, if_, n):
   return ct<<24 | [True, False, None].index(if_)<<20 | n&0xffff
 def parse_regop(ct, lhs, op, rhs):
   if op.endswith('='): op = op[:-1] # drop trailing =
   lhs, lhs_flag = parse_bracket_operand(lhs, 'lhs')
@@ -9,19 +14,28 @@
   cw = ct<<24 | REGOP_IDX[op]<<20 | lhs_flag<<16 | rhs_flag<<17 | lhs&0xf
   return cw, rhs
 def parse_regidx(ct, x, name):
   if x == 'ba': x = 0xf
   elif x == 'po': x = 0xf; ct |= 0x10
   else: x &= 0xf; assert x!=0xf, f'{name} cannot be F'
   return ct, x
-def parse_bracket_operand(x, name):
+def parse_bracket_operand(x, name): # returns (value, hasBracket)
   if type(x) == list:
     assert len(x)==1, f'`{name}` must be "x" or "[x]"'
     return x, 1
   return x, 0
+def make_asm_code(input_path, raw, kwargs):
+  if raw is not None: # raw code
+    code = parse_binarg(raw)
+    assert len(code)%4 == 0, \
+      f'len(raw) should a multiple of 4, got {len(raw)}'
+  else: # compile from file
+    assert input_path is not None, 'either `input_path` or `raw` should be set'
+    code, symbols = compile(input_path, **kwargs)
+  return code
 
 parse_binarg = lambda x: \
   b''.join(map(parse_binarg, x)) if type(x)==list else \
   bytes.fromhex(x) if type(x)==str else \
     x.to_bytes(4, 'big') if type(x)==int else x
 
 CMP_IDX = {'==': 0, '!=': 2, '>': 4, '<': 6}
@@ -40,14 +54,15 @@
   'srw': 6, '>>': 6,
   'rol': 7,
   'asr': 8,
   'fadds': 9,
   'fmuls': 10,
 }
 
+# TODO: assert range of arg
 class Gecko():
   def __init__(self):
     self.code = bytearray()
   def append(self, *payloads):
     self.code += b''.join(map(parse_binarg, payloads))
     return self
   def dump_txt(self, indent=''):
@@ -215,30 +230,26 @@
   def if16_cnt(self, cnt, op, val, reset_on_true, mask=-1, endif=False):
     T = (8 if reset_on_true else 0) + (1 if endif else 0)
     return self.append(
       (0xA8 | CMP_IDX[op])<<24 | (cnt&0xffff)<<4 | T,
       ~mask<<16 | val&0xffff,
     )
   ''' C0 '''
-  def C0(self, body):
-    body = parse_binarg(body)
-    assert len(body)%4 == 0, \
-      f'len(body) should a multiple of 4, got {len(body)}'
-    if len(body)%8 == 4:
-      body += '\x00\x00\x00\x00'
-    return self.append(0xC000_0000, len(body)>>3, body)
+  def C0(self, input_path=None, raw=None, **kwargs):
+    code = make_asm_code(input_path, raw, kwargs)
+    if len(code)%8 == 4: # pad code with blr
+      code += b'\x4E\x80\x00\x20'
+    return self.append(0xC000_0000, len(code)>>3, code)
   ''' C2 '''
-  def C2(self, addr, body, po=False):
-    body = parse_binarg(body)
-    assert len(body)%4 == 0, \
-      f'len(body) should a multiple of 4, got {len(body)}'
-    if len(body)%8 == 0:
-      body += '\x60\x00\x00\x00'
-    body += '\x00\x00\x00\x00'
-    return self.append(cw_addr(0xC2, addr, po), len(body)>>3, body)
+  def C2(self, addr, input_path, raw=None, po=False, **kwargs):
+    code = make_asm_code(input_path, raw, kwargs)
+    if len(code)%8 == 0: # pad code with nop
+      code += b'\x60\x00\x00\x00'
+    code += b'\x00\x00\x00\x00' # append 0
+    return self.append(cw_addr(0xC2, addr, po), len(code)>>3, code)
   ''' C6 '''
   def branch(self, addr, dst, po=False):
     return self.append(cw_addr(0xC6, addr, po), dst&0xffffffff)
   ''' CC '''
   def onoff_switch(self):
     return self.append(0xCC00_0000, 0)
   ''' CE '''
@@ -258,7 +269,26 @@
     return self.append(
       0xE200_0000 | (0x1_000_00 if else_ else 0) | count&0xff,
       (ba&0xffff)<<16 | (po&0xffff),
     )
   ''' F0 '''
   def end_of_code(self):
     return self.append(0xF000_0000, 0)
+
+  ''' C Kit '''
+  def c_kit(self, addr_code, input_path, entries, **kwargs):
+    code, symbols = compile(input_path, addr_code, **kwargs)
+    # 06
+    self.write_string(addr_code, code, po=False)
+    # 04/C6
+    for addr_src, action, name in entries:
+      assert name in symbols, f'symbol "{name}" is not found in the .text section of {input_path}'
+      addr_dst = symbols[name]
+      if action == 'b':
+        self.branch(addr_src, addr_dst, po=False)
+      elif action == 'bl':
+        d_addr = addr_dst - addr_src
+        assert -0x200_0000 <= d_addr < 0x200_0000, 'cannot bl from %08X to %08X'%(addr_src, addr_dst)
+        inst = 0x4800_0001 | d_addr&0x3ff_fffc
+        self.write32(addr_src, inst, po=False)
+      else: assert False, '`action` should be "b" or "bl", got "{action}"'
+    return self
```

### Comparing `supGecko-0.1.0a2/src/supGecko.egg-info/PKG-INFO` & `supGecko-0.1.0a3/src/supGecko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supGecko
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A helper library to write Gecko code
 Home-page: https://github.com/sup39/supGecko
 Author: sup39
 Author-email: sms@sup39.dev
 License: MIT
 Project-URL: Bug Tracker, https://github.com/sup39/supGecko/issues
 Classifier: Programming Language :: Python :: 3
```

