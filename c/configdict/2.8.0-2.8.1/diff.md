# Comparing `tmp/configdict-2.8.0-py3-none-any.whl.zip` & `tmp/configdict-2.8.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 32179 bytes, number of entries: 9
+Zip file size: 32550 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx       25 b- defN 21-Nov-25 01:23 configdict/__init__.py
--rw-rw-r--  2.0 unx    65970 b- defN 23-Jul-04 12:25 configdict/configdict.py
+-rw-rw-r--  2.0 unx    67583 b- defN 23-Jul-08 11:13 configdict/configdict.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Nov-25 01:23 configdict/py.typed
 -rw-rw-r--  2.0 unx    22699 b- defN 21-Nov-25 01:23 configdict/__pycache__/configdict.cpython-38.pyc
--rw-rw-r--  2.0 unx     1060 b- defN 23-Jul-04 12:31 configdict-2.8.0.dist-info/LICENSE.md
--rw-rw-r--  2.0 unx     3883 b- defN 23-Jul-04 12:31 configdict-2.8.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 12:31 configdict-2.8.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jul-04 12:31 configdict-2.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      742 b- defN 23-Jul-04 12:31 configdict-2.8.0.dist-info/RECORD
-9 files, 94482 bytes uncompressed, 30893 bytes compressed:  67.3%
+-rw-rw-r--  2.0 unx     1060 b- defN 23-Jul-11 13:09 configdict-2.8.1.dist-info/LICENSE.md
+-rw-rw-r--  2.0 unx     3883 b- defN 23-Jul-11 13:09 configdict-2.8.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 13:09 configdict-2.8.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jul-11 13:09 configdict-2.8.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      742 b- defN 23-Jul-11 13:09 configdict-2.8.1.dist-info/RECORD
+9 files, 96095 bytes uncompressed, 31264 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: configdict/py.typed
 Comment: 
 
 Filename: configdict/__pycache__/configdict.cpython-38.pyc
 Comment: 
 
-Filename: configdict-2.8.0.dist-info/LICENSE.md
+Filename: configdict-2.8.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: configdict-2.8.0.dist-info/METADATA
+Filename: configdict-2.8.1.dist-info/METADATA
 Comment: 
 
-Filename: configdict-2.8.0.dist-info/WHEEL
+Filename: configdict-2.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: configdict-2.8.0.dist-info/top_level.txt
+Filename: configdict-2.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: configdict-2.8.0.dist-info/RECORD
+Filename: configdict-2.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## configdict/configdict.py

```diff
@@ -858,38 +858,70 @@
             error = config.checkType(key, value)
             if error:
                 print(error)
         """
         if not self._validator:
             logger.debug(f"Validator not set, cannot check value {value} (key '{key}')")
             return
-        choices = self.getChoices(key)
-        if choices is not None and value not in choices:
-            return f"key {key} should be one of {choices}, got {value}"
-        func = self.getValidateFunc(key)
-        if func:
-            error = func(self, key, value)
-            if not error:
-                return f"{value} is not valid for key {key}"
-            elif isinstance(error, str):
-                return f"{value} is not valid for key {key}: {error}"
-        t = self.getType(key)
-        if t == float:
-            if not _isfloaty(value):
-                return f"Expected floatlike for key {key}, got {type(value).__name__}"
-        elif t == str and not isinstance(value, (bytes, str)):
-            return f"Expected str or bytes for key {key}, got {type(value).__name__}"
-        elif not isinstance(value, t):
-            return f"Expected {t.__name__} for key {key}, got {type(value).__name__}"
-
-        r = self.getRange(key)
-        if r and not (r[0] <= value <= r[1]):
-            return f"Value for key {key} should be within range {r}, got {value}"
+
+        for validatortype in self.getValidateFunc(key):
+            if validatortype == 'choices':
+                choices = self.getChoices(key)
+                if choices is not None and value not in choices:
+                    return f"key {key} should be one of {choices}, got {value}"
+            elif validatortype == 'func':
+                error = self.getValidateFunc(key)(self, key, value)
+                if error is False:
+                    return f"{value} is not valid for key {key}"
+                elif isinstance(error, str) and error:
+                    return f"{value} is not valid for key {key}: {error}"
+            elif validatortype == 'type':
+                t = self.getType(key)
+                if t == float:
+                    if not _isfloaty(value):
+                        return f"Expected floatlike for key {key}, got {type(value).__name__}"
+                elif t == str:
+                    if not isinstance(value, (bytes, str)):
+                        return f"Expected str or bytes for key {key}, got {type(value).__name__}"
+                elif not isinstance(value, t):
+                    return f"Expected {t.__name__} for key {key}, got {type(value).__name__}"
+            elif validatortype == 'range':
+                if (r := self.getRange(key)) and not (r[0] <= value <= r[1]):
+                    return f"Value for key {key} should be within range {r}, got {value}"
         return None
 
+    @cache
+    def getValidatorTypes(self, key: str) -> list[str]:
+        """
+        Return the validator types for a given key
+
+        A validator type for a given key can be a choices validator, where a set of
+        possible values is given for a given key; it can be a range, where the
+        value must be within a given range; a type, where a value must be of
+        a certain type; or a function, which must return True if the value
+        is valid, or False or an error message as string if the value is invalid
+
+        Args:
+            key: the key to query
+
+        Returns:
+            a list of validator types, where each item is one of 'choices',
+            'range', 'type', 'func'
+        """
+        validators = []
+        if f"{key}::choices" in self._validator:
+            validators.append('choices')
+        if f"{key}::range" in self._validator:
+            validators.append('range')
+        if key in self._validator:
+            validators.append('func')
+        if f"{key}::type" in self._validator:
+            validators.append('type')
+        return validators
+
     def getRange(self, key: str) -> Optional[tuple]:
         """
         Returns the valid range for this key's value, if specified.
 
         Args:
             key: the key to get the range from.
 
@@ -1132,15 +1164,14 @@
 
                 {
                   'keyA::choices': ['foo', 'bar'],
                   'keyB::type': float,
                   'keyB::range': (10, 30)
                 }
 
-
             Choices can be defined lazyly by giving a lambda
 
         docs: a dict containing documentation for each key
 
         persistent: if True, any change to the dict will be automatically saved.
             Otherwise a dict can be saved manually via :meth:`ConfigDict.save`
 
@@ -1151,14 +1182,16 @@
 
         precallback: function `(dict, key, oldvalue, newvalue) -> None|newvalue`,
             If given, it is called *before* the modification is done. This function
             should return **None** to allow modification, **any value** to modify the 
             value, or **raise ValueError** to stop the transaction
 
         sortKeys: if True, keys are sorted whenever the dict is saved/edited.
+        advancedPrefix: keys with this prefix are marked as advanced. Whenever the dict
+            is displayed or edited, these keys appear after all the other keys
 
 
     Example
     =======
 
     .. code::
```

## Comparing `configdict-2.8.0.dist-info/LICENSE.md` & `configdict-2.8.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `configdict-2.8.0.dist-info/METADATA` & `configdict-2.8.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configdict
-Version: 2.8.0
+Version: 2.8.1
 Summary: A supercharged dict used as configuration
 Author-email: Eduardo Moguillansky <eduardo.moguillansky@gmail.com>
 License: Copyright (c) 2011-2017 GitHub Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

