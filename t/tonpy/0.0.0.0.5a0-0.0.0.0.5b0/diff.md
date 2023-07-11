# Comparing `tmp/tonpy-0.0.0.0.5a0-cp39-cp39-win_amd64.whl.zip` & `tmp/tonpy-0.0.0.0.5b0-cp310-cp310-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,19 @@
-Zip file size: 14763 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat       27 b- defN 23-Jul-09 13:43 tonpy-0.0.0.0.5a0.data/purelib/tonpy/__init__.py
--rw-rw-rw-  2.0 fat      168 b- defN 23-Jul-09 13:43 tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/__init__.py
--rw-rw-rw-  2.0 fat     1418 b- defN 23-Jul-09 13:43 tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/cell.py
--rw-rw-rw-  2.0 fat    10198 b- defN 23-Jul-09 13:43 tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/cellbuilder.py
--rw-rw-rw-  2.0 fat    11943 b- defN 23-Jul-09 13:43 tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/cellslice.py
--rw-rw-rw-  2.0 fat    10169 b- defN 23-Jul-09 13:43 tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/vmdict.py
--rw-rw-rw-  2.0 fat     9870 b- defN 23-Jul-09 13:44 tonpy-0.0.0.0.5a0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3323 b- defN 23-Jul-09 13:44 tonpy-0.0.0.0.5a0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-09 13:44 tonpy-0.0.0.0.5a0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-09 13:44 tonpy-0.0.0.0.5a0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1064 b- defN 23-Jul-09 13:44 tonpy-0.0.0.0.5a0.dist-info/RECORD
-11 files, 48286 bytes uncompressed, 12915 bytes compressed:  73.3%
+Zip file size: 17219 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat       27 b- defN 23-Jul-11 06:28 tonpy-0.0.0.0.5b0.data/purelib/tonpy/__init__.py
+-rw-rw-rw-  2.0 fat       49 b- defN 23-Jul-11 06:28 tonpy-0.0.0.0.5b0.data/purelib/tonpy/tlb_gen/__init__.py
+-rw-rw-rw-  2.0 fat     1140 b- defN 23-Jul-11 06:28 tonpy-0.0.0.0.5b0.data/purelib/tonpy/tlb_gen/py.py
+-rw-rw-rw-  2.0 fat      213 b- defN 23-Jul-11 06:28 tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/__init__.py
+-rw-rw-rw-  2.0 fat     1418 b- defN 23-Jul-11 06:28 tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/cell.py
+-rw-rw-rw-  2.0 fat    10309 b- defN 23-Jul-11 06:28 tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/cellbuilder.py
+-rw-rw-rw-  2.0 fat    11943 b- defN 23-Jul-11 06:28 tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/cellslice.py
+-rw-rw-rw-  2.0 fat      112 b- defN 23-Jul-11 06:28 tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/tlb.py
+-rw-rw-rw-  2.0 fat    10169 b- defN 23-Jul-11 06:28 tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/vmdict.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-11 06:28 tonpy-0.0.0.0.5b0.data/purelib/tonpy/utils/__init__.py
+-rw-rw-rw-  2.0 fat      802 b- defN 23-Jul-11 06:28 tonpy-0.0.0.0.5b0.data/purelib/tonpy/utils/bit_converter.py
+-rw-rw-rw-  2.0 fat      176 b- defN 23-Jul-11 06:28 tonpy-0.0.0.0.5b0.data/purelib/tonpy/utils/bit_int.py
+-rw-rw-rw-  2.0 fat     9870 b- defN 23-Jul-11 06:30 tonpy-0.0.0.0.5b0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3318 b- defN 23-Jul-11 06:30 tonpy-0.0.0.0.5b0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Jul-11 06:30 tonpy-0.0.0.0.5b0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-11 06:30 tonpy-0.0.0.0.5b0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1719 b- defN 23-Jul-11 06:30 tonpy-0.0.0.0.5b0.dist-info/RECORD
+17 files, 51373 bytes uncompressed, 14273 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -1,34 +1,52 @@
-Filename: tonpy-0.0.0.0.5a0.data/purelib/tonpy/__init__.py
+Filename: tonpy-0.0.0.0.5b0.data/purelib/tonpy/__init__.py
 Comment: 
 
-Filename: tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/__init__.py
+Filename: tonpy-0.0.0.0.5b0.data/purelib/tonpy/tlb_gen/__init__.py
 Comment: 
 
-Filename: tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/cell.py
+Filename: tonpy-0.0.0.0.5b0.data/purelib/tonpy/tlb_gen/py.py
 Comment: 
 
-Filename: tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/cellbuilder.py
+Filename: tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/__init__.py
 Comment: 
 
-Filename: tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/cellslice.py
+Filename: tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/cell.py
 Comment: 
 
-Filename: tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/vmdict.py
+Filename: tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/cellbuilder.py
 Comment: 
 
-Filename: tonpy-0.0.0.0.5a0.dist-info/LICENSE
+Filename: tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/cellslice.py
 Comment: 
 
-Filename: tonpy-0.0.0.0.5a0.dist-info/METADATA
+Filename: tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/tlb.py
 Comment: 
 
-Filename: tonpy-0.0.0.0.5a0.dist-info/WHEEL
+Filename: tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/vmdict.py
 Comment: 
 
-Filename: tonpy-0.0.0.0.5a0.dist-info/top_level.txt
+Filename: tonpy-0.0.0.0.5b0.data/purelib/tonpy/utils/__init__.py
 Comment: 
 
-Filename: tonpy-0.0.0.0.5a0.dist-info/RECORD
+Filename: tonpy-0.0.0.0.5b0.data/purelib/tonpy/utils/bit_converter.py
+Comment: 
+
+Filename: tonpy-0.0.0.0.5b0.data/purelib/tonpy/utils/bit_int.py
+Comment: 
+
+Filename: tonpy-0.0.0.0.5b0.dist-info/LICENSE
+Comment: 
+
+Filename: tonpy-0.0.0.0.5b0.dist-info/METADATA
+Comment: 
+
+Filename: tonpy-0.0.0.0.5b0.dist-info/WHEEL
+Comment: 
+
+Filename: tonpy-0.0.0.0.5b0.dist-info/top_level.txt
+Comment: 
+
+Filename: tonpy-0.0.0.0.5b0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/cell.py` & `tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/cell.py`

 * *Files identical despite different names*

## Comparing `tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/cellbuilder.py` & `tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/cellbuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,18 @@
 
         test_value_len(uint_, uint_bits)
 
         # Large ints need to be converted to string to be parsed in C++
         self.builder.store_uint_str(str(uint_), uint_bits)
         return self
 
+    def store_uint_big(self, a, b):
+        self.builder.store_256uint_str(str(a), b)
+        return self
+
     def begin_parse(self) -> CellSlice:
         """Convert CellBuilder to CellSlice"""
 
         return self.end_cell().begin_parse()
 
     def store_int(self, int_: int, int_bits: int) -> "CellBuilder":
         """
```

## Comparing `tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/cellslice.py` & `tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/cellslice.py`

 * *Files identical despite different names*

## Comparing `tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/vmdict.py` & `tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/vmdict.py`

 * *Files identical despite different names*

## Comparing `tonpy-0.0.0.0.5a0.dist-info/LICENSE` & `tonpy-0.0.0.0.5b0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tonpy-0.0.0.0.5a0.dist-info/METADATA` & `tonpy-0.0.0.0.5b0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonpy
-Version: 0.0.0.0.5a0
+Version: 0.0.0.0.5b0
 Summary: Types / API for TON blockchain
 Home-page: https://github.com/disintar/tonpy
 Author: Disintar LLP
 Author-email: andrey@head-labs.com
 Project-URL: Bug Tracker, https://github.com/disintar/tonpy/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -57,16 +57,15 @@
 some python code on top of C++ bindings.
 
 ## Installation
 
 One command: `pip install tonpy`
 
 Complex installation for not supported systems and python versions are described in [documentation](https://tonpy.dton.io/installation.html#development-setup-compile-from-sources)
-AZ
-]
+
 ## Documentation
 
 Documentation can be found on [tonpy.dton.io](https://tonpy.dton.io)
 
 ## Donation
 
 If you want to support our work, send any coins to:
```

## Comparing `tonpy-0.0.0.0.5a0.dist-info/RECORD` & `tonpy-0.0.0.0.5b0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,17 @@
-tonpy-0.0.0.0.5a0.data/purelib/tonpy/__init__.py,sha256=X0IKqN1VrJxaGR1qzGuq1R8lzadLHG9PxFQWV-shq44,27
-tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/__init__.py,sha256=vNJsMyVSzt_panP3aZZ7PlvNgouk9niQDbYL6TOD4lQ,168
-tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/cell.py,sha256=XdGmUxgcKsZbM8J9ZrM1QukneABRFlZ1gSdgBZ028FY,1418
-tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/cellbuilder.py,sha256=NVEJ8hxwAe7DJA6PNaLEGZhON02_FdhyJGA4zwdDoVo,10198
-tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/cellslice.py,sha256=jimHiatbuCLp2EGLmyVIXswBg7D24or4eP9APJhcge0,11943
-tonpy-0.0.0.0.5a0.data/purelib/tonpy/types/vmdict.py,sha256=j05yA-Pd7UG252VP5mCmRsT3jUdEZCAAbjR5G-F_O40,10169
-tonpy-0.0.0.0.5a0.dist-info/LICENSE,sha256=RSxBv9jtUwgzgMzGSLAU7hHWYFKlIuhjL-qstAk6-IU,9870
-tonpy-0.0.0.0.5a0.dist-info/METADATA,sha256=MNYI2TtX0Mc6zBaC5nHO16Rak_uwwP-bw1hes80lDU4,3323
-tonpy-0.0.0.0.5a0.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-tonpy-0.0.0.0.5a0.dist-info/top_level.txt,sha256=_VfnkAqcmXm2AiZSPM83S72oXsZLEM4s-yxRZk87TYs,6
-tonpy-0.0.0.0.5a0.dist-info/RECORD,,
+tonpy-0.0.0.0.5b0.data/purelib/tonpy/__init__.py,sha256=X0IKqN1VrJxaGR1qzGuq1R8lzadLHG9PxFQWV-shq44,27
+tonpy-0.0.0.0.5b0.data/purelib/tonpy/tlb_gen/__init__.py,sha256=zf0KqEha0qXA0NXZcVOJEB-z3Tz__tcM05RX5pyU9ks,49
+tonpy-0.0.0.0.5b0.data/purelib/tonpy/tlb_gen/py.py,sha256=bYOy5zNtdaXr6ggQwgAAItFNRUpnjfq9XuC6reGQIw8,1140
+tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/__init__.py,sha256=BQgGyyF_ShsEKTWV_Bv4OCqWuZ4J6j5rZknsMBIsOLs,213
+tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/cell.py,sha256=XdGmUxgcKsZbM8J9ZrM1QukneABRFlZ1gSdgBZ028FY,1418
+tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/cellbuilder.py,sha256=WvCdETbTkcmUKFCgeADbz07l4RS4pnR2uysl7fie5zw,10309
+tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/cellslice.py,sha256=jimHiatbuCLp2EGLmyVIXswBg7D24or4eP9APJhcge0,11943
+tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/tlb.py,sha256=7a_NiFuebZ-JGTNqubFT8iJcsPKIJx4niR4pK1xscno,112
+tonpy-0.0.0.0.5b0.data/purelib/tonpy/types/vmdict.py,sha256=j05yA-Pd7UG252VP5mCmRsT3jUdEZCAAbjR5G-F_O40,10169
+tonpy-0.0.0.0.5b0.data/purelib/tonpy/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tonpy-0.0.0.0.5b0.data/purelib/tonpy/utils/bit_converter.py,sha256=Y_CypT1CLZYION_XwMhWbMVAA8gOkcR7fFlSzGyEJDs,802
+tonpy-0.0.0.0.5b0.data/purelib/tonpy/utils/bit_int.py,sha256=k1YL5fnmDMTZdymHYOniW5V2omllHpvQuQiDfuz4KtY,176
+tonpy-0.0.0.0.5b0.dist-info/LICENSE,sha256=RSxBv9jtUwgzgMzGSLAU7hHWYFKlIuhjL-qstAk6-IU,9870
+tonpy-0.0.0.0.5b0.dist-info/METADATA,sha256=gu0rjZ6Y4evl2KQ-9cjHOFNo5rr8xNKbQEkM1sH15NE,3318
+tonpy-0.0.0.0.5b0.dist-info/WHEEL,sha256=jrOhEbqKwvzRFSJcbYXlJCyVkgVdHg4_7__YHrdTUfw,102
+tonpy-0.0.0.0.5b0.dist-info/top_level.txt,sha256=_VfnkAqcmXm2AiZSPM83S72oXsZLEM4s-yxRZk87TYs,6
+tonpy-0.0.0.0.5b0.dist-info/RECORD,,
```

