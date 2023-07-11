# Comparing `tmp/configdict-2.8.1-py3-none-any.whl.zip` & `tmp/configdict-2.8.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 32550 bytes, number of entries: 9
+Zip file size: 32564 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx       25 b- defN 21-Nov-25 01:23 configdict/__init__.py
--rw-rw-r--  2.0 unx    67583 b- defN 23-Jul-08 11:13 configdict/configdict.py
+-rw-rw-r--  2.0 unx    67758 b- defN 23-Jul-11 14:11 configdict/configdict.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Nov-25 01:23 configdict/py.typed
 -rw-rw-r--  2.0 unx    22699 b- defN 21-Nov-25 01:23 configdict/__pycache__/configdict.cpython-38.pyc
--rw-rw-r--  2.0 unx     1060 b- defN 23-Jul-11 13:09 configdict-2.8.1.dist-info/LICENSE.md
--rw-rw-r--  2.0 unx     3883 b- defN 23-Jul-11 13:09 configdict-2.8.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 13:09 configdict-2.8.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jul-11 13:09 configdict-2.8.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      742 b- defN 23-Jul-11 13:09 configdict-2.8.1.dist-info/RECORD
-9 files, 96095 bytes uncompressed, 31264 bytes compressed:  67.5%
+-rw-rw-r--  2.0 unx     1060 b- defN 23-Jul-11 14:39 configdict-2.8.2.dist-info/LICENSE.md
+-rw-rw-r--  2.0 unx     3883 b- defN 23-Jul-11 14:39 configdict-2.8.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 14:39 configdict-2.8.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jul-11 14:39 configdict-2.8.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      742 b- defN 23-Jul-11 14:39 configdict-2.8.2.dist-info/RECORD
+9 files, 96270 bytes uncompressed, 31278 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: configdict/py.typed
 Comment: 
 
 Filename: configdict/__pycache__/configdict.cpython-38.pyc
 Comment: 
 
-Filename: configdict-2.8.1.dist-info/LICENSE.md
+Filename: configdict-2.8.2.dist-info/LICENSE.md
 Comment: 
 
-Filename: configdict-2.8.1.dist-info/METADATA
+Filename: configdict-2.8.2.dist-info/METADATA
 Comment: 
 
-Filename: configdict-2.8.1.dist-info/WHEEL
+Filename: configdict-2.8.2.dist-info/WHEEL
 Comment: 
 
-Filename: configdict-2.8.1.dist-info/top_level.txt
+Filename: configdict-2.8.2.dist-info/top_level.txt
 Comment: 
 
-Filename: configdict-2.8.1.dist-info/RECORD
+Filename: configdict-2.8.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## configdict/configdict.py

```diff
@@ -26,26 +26,27 @@
 .. code::
 
     from configdict import ConfigDict
 
     config = ConfigDict("myproj.subproj")
     config.addKey("keyA", 10, doc="documentaion of keyA")
     config.addKey("keyB", 0.5, range=(0, 1))
-    config.addKey("keyC", "blue", choices=("blue", "red"), doc="documentation of keyC")
+    config.addKey("keyC", "blue", choices=("blue", "red"), 
+                  doc="documentation of keyC")
     config.load()
 
 Alternativaly, a :class:`ConfigDict` or a :class:`CheckedDict` can be built
 via a context manager::
 
     with ConfigDict("plotting") as cfg:
         # While building a config, __call__ is equivalent to addKey
         cfg('backend', 'matplotlib', choices={'matlotlib'})
         cfg('spectrogram.figsize', (24, 8))
         cfg('spectrogram.maxfreq', 12000,
-          doc="Highest frequency in a spectrogram")
+            doc="Highest frequency in a spectrogram")
         cfg('spectrogram.window', 'hamming', choices={'hamming', 'hanning'})
         # no need to call .load, it is called automatically
 
 A :class:`ConfigDict` can be created all at once
 
 .. code::
 
@@ -679,16 +680,16 @@
 
         Args:
             key: a string key
             value: a default value
             type: the type accepted, as passed to isinstance (can be a tuple)
             choices: a set/tuple of possible values
             range: a (min, max) tuple defining an allowed range for this value
-            validatefunc: a function ``(config: dict, key:str, value) -> bool``, should return
-                `True` if value is valid for `key` or False otherwise
+            validatefunc: a function ``(config: dict, key:str, value) -> bool``,
+                should return `True` if value is valid for `key` or False otherwise
             doc: documentation for this key
 
         """
         self.default[key] = value
         self._allowedkeys.add(key)
         validator = self._validator
         if type:
@@ -806,15 +807,16 @@
             key (str): the key to query for a validate function
 
         Returns:
             The validate function, or None
 
         """
         func = self._validator.get(key, None)
-        assert func is None or callable(func), f"Validate func should be callable for key {key}, got {func}"
+        assert func is None or callable(func), \
+            f"Validate func should be callable for key {key}, got {func}"
         return func
 
     def getChoices(self, key: str) -> Optional[list]:
         """
         Return a seq. of possible values for key ``k`` or ``None``
         """
         if key not in self._allowedkeys:
@@ -1067,15 +1069,16 @@
             except KeyboardInterrupt:
                 logger.debug("Editing aborted")
                 return
         else:
             _waitForClick(title=self.name)
         self.load(configfile)
 
-    def _saveAsYaml(self, path: str, header: str = '', sortKeys=False, separateAdvancedKeys=True) -> None:
+    def _saveAsYaml(self, path: str, header: str = '', sortKeys=False,
+                    separateAdvancedKeys=True) -> None:
         yamlstr = self.asYaml(sortKeys=sortKeys)
         folder = os.path.split(path)[0]
         os.makedirs(folder, exist_ok=True)
         with open(path, "w") as f:
             if header:
                 f.write(header)
                 f.write("\n")
@@ -1094,15 +1097,17 @@
         parts = [f'<div><h4>{type(self).__name__}</h4>']
         parts.append("<br>")
         rows = []
         keys = self._sortedKeys()
         for k in keys:
             v = self[k]
             rows.append((k, str(v), self._infoStr(k), self.getDoc(k)))
-        table = _htmlTable(rows, headers=('Key', 'Value', 'Type', 'Descr'), maxwidths=[0, 0, 150, 400],
+        table = _htmlTable(rows,
+                           headers=('Key', 'Value', 'Type', 'Descr'),
+                           maxwidths=[0, 0, 150, 400],
                            rowstyles=('strong', 'code', None, None))
         parts.append(table)
         parts.append("</div>")
         return "".join(parts)
 
 
 def _loadJson(path:str) -> Optional[dict]:
@@ -1239,15 +1244,17 @@
                          validator=validator,
                          docs=docs)
         # no need to call .load in this case
 
         # Using inheritance
         class MyConfig(ConfigDict):
             def __init__(self):
-                super().__init__(name="myconfig", default=default, validator=validator,
+                super().__init__(name="myconfig",
+                                 default=default,
+                                 validator=validator,
                                  docs=docs)
 
         cfg = MyConfig()
 
     """
 
     _registry: dict[str, ConfigDict] = {}
```

## Comparing `configdict-2.8.1.dist-info/LICENSE.md` & `configdict-2.8.2.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `configdict-2.8.1.dist-info/METADATA` & `configdict-2.8.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configdict
-Version: 2.8.1
+Version: 2.8.2
 Summary: A supercharged dict used as configuration
 Author-email: Eduardo Moguillansky <eduardo.moguillansky@gmail.com>
 License: Copyright (c) 2011-2017 GitHub Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

## Comparing `configdict-2.8.1.dist-info/RECORD` & `configdict-2.8.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 configdict/__init__.py,sha256=CI6gyI6isoSmOxiaMKQ1zJMLWzFYn6bOTnUcJtMAMRQ,25
-configdict/configdict.py,sha256=Qht1PryaIhut6ymAoxDdq8akQfJLgO7d4QD_XnjcVrc,67583
+configdict/configdict.py,sha256=iVf83Vo7smtCk0LlRCFzVHYQ_WheLPCCSQ3DEUmXaqs,67758
 configdict/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 configdict/__pycache__/configdict.cpython-38.pyc,sha256=pmenTOMg3mEukCVKrOf7lNx1TTPjNga5bTXY_VRnSFU,22699
-configdict-2.8.1.dist-info/LICENSE.md,sha256=vjYMqYMp4lDhS_QWyPhZxn-MqGDF45oVUfgZIERh6cQ,1060
-configdict-2.8.1.dist-info/METADATA,sha256=0Yd3jWA-wG5Bz2bHPMRKzQ7CrC9GZIM1OuFqtx4kDRg,3883
-configdict-2.8.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-configdict-2.8.1.dist-info/top_level.txt,sha256=6D1On6cX6fbtbBo94S0tXrjpLkb2YyQpRPiJOA-8RnY,11
-configdict-2.8.1.dist-info/RECORD,,
+configdict-2.8.2.dist-info/LICENSE.md,sha256=vjYMqYMp4lDhS_QWyPhZxn-MqGDF45oVUfgZIERh6cQ,1060
+configdict-2.8.2.dist-info/METADATA,sha256=cBzIez8BXGq8TUvj4ik3QxzTKM4l6XLEsuAia2XqWI8,3883
+configdict-2.8.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+configdict-2.8.2.dist-info/top_level.txt,sha256=6D1On6cX6fbtbBo94S0tXrjpLkb2YyQpRPiJOA-8RnY,11
+configdict-2.8.2.dist-info/RECORD,,
```

