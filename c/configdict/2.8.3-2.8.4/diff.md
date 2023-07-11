# Comparing `tmp/configdict-2.8.3-py3-none-any.whl.zip` & `tmp/configdict-2.8.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 32567 bytes, number of entries: 9
+Zip file size: 32566 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx       25 b- defN 21-Nov-25 01:23 configdict/__init__.py
--rw-rw-r--  2.0 unx    67751 b- defN 23-Jul-11 15:35 configdict/configdict.py
+-rw-rw-r--  2.0 unx    67754 b- defN 23-Jul-11 15:38 configdict/configdict.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Nov-25 01:23 configdict/py.typed
 -rw-rw-r--  2.0 unx    22699 b- defN 21-Nov-25 01:23 configdict/__pycache__/configdict.cpython-38.pyc
--rw-rw-r--  2.0 unx     1060 b- defN 23-Jul-11 15:36 configdict-2.8.3.dist-info/LICENSE.md
--rw-rw-r--  2.0 unx     3883 b- defN 23-Jul-11 15:36 configdict-2.8.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 15:36 configdict-2.8.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jul-11 15:36 configdict-2.8.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      742 b- defN 23-Jul-11 15:36 configdict-2.8.3.dist-info/RECORD
-9 files, 96263 bytes uncompressed, 31281 bytes compressed:  67.5%
+-rw-rw-r--  2.0 unx     1060 b- defN 23-Jul-11 15:39 configdict-2.8.4.dist-info/LICENSE.md
+-rw-rw-r--  2.0 unx     3883 b- defN 23-Jul-11 15:39 configdict-2.8.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 15:39 configdict-2.8.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jul-11 15:39 configdict-2.8.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      742 b- defN 23-Jul-11 15:39 configdict-2.8.4.dist-info/RECORD
+9 files, 96266 bytes uncompressed, 31280 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: configdict/py.typed
 Comment: 
 
 Filename: configdict/__pycache__/configdict.cpython-38.pyc
 Comment: 
 
-Filename: configdict-2.8.3.dist-info/LICENSE.md
+Filename: configdict-2.8.4.dist-info/LICENSE.md
 Comment: 
 
-Filename: configdict-2.8.3.dist-info/METADATA
+Filename: configdict-2.8.4.dist-info/METADATA
 Comment: 
 
-Filename: configdict-2.8.3.dist-info/WHEEL
+Filename: configdict-2.8.4.dist-info/WHEEL
 Comment: 
 
-Filename: configdict-2.8.3.dist-info/top_level.txt
+Filename: configdict-2.8.4.dist-info/top_level.txt
 Comment: 
 
-Filename: configdict-2.8.3.dist-info/RECORD
+Filename: configdict-2.8.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## configdict/configdict.py

```diff
@@ -861,15 +861,15 @@
             if error:
                 print(error)
         """
         if not self._validator:
             logger.debug(f"Validator not set, cannot check value {value} (key '{key}')")
             return
 
-        for validatortype in self.validatorTypes():
+        for validatortype in self.validatorTypes(key):
             if validatortype == 'choices':
                 choices = self.getChoices(key)
                 if choices is not None and value not in choices:
                     return f"key {key} should be one of {choices}, got {value}"
             elif validatortype == 'func':
                 error = self.getValidateFunc(key)(self, key, value)
                 if error is False:
```

## Comparing `configdict-2.8.3.dist-info/LICENSE.md` & `configdict-2.8.4.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `configdict-2.8.3.dist-info/METADATA` & `configdict-2.8.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configdict
-Version: 2.8.3
+Version: 2.8.4
 Summary: A supercharged dict used as configuration
 Author-email: Eduardo Moguillansky <eduardo.moguillansky@gmail.com>
 License: Copyright (c) 2011-2017 GitHub Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

## Comparing `configdict-2.8.3.dist-info/RECORD` & `configdict-2.8.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 configdict/__init__.py,sha256=CI6gyI6isoSmOxiaMKQ1zJMLWzFYn6bOTnUcJtMAMRQ,25
-configdict/configdict.py,sha256=MtgJcD6HB4oLWUgKAf5r4PAyo3Frzy2gjKB6k2BJ76c,67751
+configdict/configdict.py,sha256=uMlbMr-aO6803NWDfTgRIjWBVtL-7U3q2iRLRHk2dQE,67754
 configdict/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 configdict/__pycache__/configdict.cpython-38.pyc,sha256=pmenTOMg3mEukCVKrOf7lNx1TTPjNga5bTXY_VRnSFU,22699
-configdict-2.8.3.dist-info/LICENSE.md,sha256=vjYMqYMp4lDhS_QWyPhZxn-MqGDF45oVUfgZIERh6cQ,1060
-configdict-2.8.3.dist-info/METADATA,sha256=L54wCDd5CekM3VoJ1Rewv9CN4dM5wms0IWUlSW3BZfY,3883
-configdict-2.8.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-configdict-2.8.3.dist-info/top_level.txt,sha256=6D1On6cX6fbtbBo94S0tXrjpLkb2YyQpRPiJOA-8RnY,11
-configdict-2.8.3.dist-info/RECORD,,
+configdict-2.8.4.dist-info/LICENSE.md,sha256=vjYMqYMp4lDhS_QWyPhZxn-MqGDF45oVUfgZIERh6cQ,1060
+configdict-2.8.4.dist-info/METADATA,sha256=CciTS_I8_UgYXOO-3o1pBmUh6qVCNSZPK5WDn8u6Xjs,3883
+configdict-2.8.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+configdict-2.8.4.dist-info/top_level.txt,sha256=6D1On6cX6fbtbBo94S0tXrjpLkb2YyQpRPiJOA-8RnY,11
+configdict-2.8.4.dist-info/RECORD,,
```

