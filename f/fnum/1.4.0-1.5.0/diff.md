# Comparing `tmp/fnum-1.4.0-py3-none-any.whl.zip` & `tmp/fnum-1.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 5953 bytes, number of entries: 11
--rw-r--r--  2.0 unx     4271 b- defN 23-Jul-09 19:55 fnum/__init__.py
--rw-r--r--  2.0 unx       29 b- defN 23-Jul-09 19:55 fnum/__main__.py
--rw-r--r--  2.0 unx     2511 b- defN 23-Jul-09 19:55 fnum/cli.py
--rw-r--r--  2.0 unx       41 b- defN 23-Jul-09 19:55 fnum/exceptions.py
--rw-r--r--  2.0 unx     2116 b- defN 23-Jul-09 19:55 fnum/metadata.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-09 19:56 fnum-1.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1038 b- defN 23-Jul-09 19:56 fnum-1.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 19:56 fnum-1.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-09 19:56 fnum-1.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-09 19:56 fnum-1.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      820 b- defN 23-Jul-09 19:56 fnum-1.4.0.dist-info/RECORD
-11 files, 12030 bytes uncompressed, 4579 bytes compressed:  61.9%
+Zip file size: 6859 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      626 b- defN 23-Jul-11 03:55 fnum/__init__.py
+-rw-r--r--  2.0 unx       29 b- defN 23-Jul-11 03:55 fnum/__main__.py
+-rw-r--r--  2.0 unx     7196 b- defN 23-Jul-11 03:55 fnum/_orchestrator.py
+-rw-r--r--  2.0 unx     2464 b- defN 23-Jul-11 03:55 fnum/cli.py
+-rw-r--r--  2.0 unx       41 b- defN 23-Jul-11 03:55 fnum/exceptions.py
+-rw-r--r--  2.0 unx     2116 b- defN 23-Jul-11 03:55 fnum/metadata.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-11 03:55 fnum-1.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1038 b- defN 23-Jul-11 03:55 fnum-1.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 03:55 fnum-1.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-11 03:55 fnum-1.5.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-11 03:55 fnum-1.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      897 b- defN 23-Jul-11 03:55 fnum-1.5.0.dist-info/RECORD
+12 files, 15611 bytes uncompressed, 5367 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -1,34 +1,37 @@
 Filename: fnum/__init__.py
 Comment: 
 
 Filename: fnum/__main__.py
 Comment: 
 
+Filename: fnum/_orchestrator.py
+Comment: 
+
 Filename: fnum/cli.py
 Comment: 
 
 Filename: fnum/exceptions.py
 Comment: 
 
 Filename: fnum/metadata.py
 Comment: 
 
-Filename: fnum-1.4.0.dist-info/LICENSE
+Filename: fnum-1.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: fnum-1.4.0.dist-info/METADATA
+Filename: fnum-1.5.0.dist-info/METADATA
 Comment: 
 
-Filename: fnum-1.4.0.dist-info/WHEEL
+Filename: fnum-1.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: fnum-1.4.0.dist-info/entry_points.txt
+Filename: fnum-1.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: fnum-1.4.0.dist-info/top_level.txt
+Filename: fnum-1.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fnum-1.4.0.dist-info/RECORD
+Filename: fnum-1.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fnum/__init__.py

```diff
@@ -1,134 +1,26 @@
 import logging
-from pathlib import Path
-from contextlib import contextmanager
-from imeta import ImageMetadata
 
-from .exceptions import FnumException
+from ._orchestrator import _NumberOrchestrator
 from .metadata import FnumMetadata, FnumMax
 
 
-__version__ = "1.4.0"
+__version__ = "1.5.0"
 
 _log = logging.getLogger(__name__)
 
 
-def number_files(dirpath, suffixes, include_imeta=False):
-    dirpath = Path(dirpath)
+def number_files(
+    dirpath, suffixes, write_metadata=False, write_max=False, include_imeta=False
+):
     _log.info("Analyzing files...")
+    orchestrator = _NumberOrchestrator(
+        dirpath, suffixes, write_metadata, write_max, include_imeta
+    )
+    orchestrator.find_ordered()
+    orchestrator.find_movable()
 
-    try:
-        metadata = FnumMetadata.from_file(dirpath)
-        regen_meta = False
-    except FileNotFoundError:
-        metadata = FnumMetadata.get_default()
-        regen_meta = True
-
-    num = 1
-
-    def numpath(suffix):
-        return dirpath / (str(num) + suffix)
-
-    # Find what files we already have in order
-    while used_suffixes := tuple(
-        suffix for suffix in suffixes if numpath(suffix).exists()
-    ):
-        if len(used_suffixes) > 1:
-            raise FnumException(
-                f"Unexpectedly found multiple existing files with number {num}"
-            )
-        if regen_meta:
-            filepath = numpath(used_suffixes[0])
-            metadata.order.append(filepath.name)
-            metadata.originals[filepath.name] = filepath.name
-        num += 1
-
-    # Shift down existing ordered files so new ones are added at the end
-    nummax = num - 1
-    for filepath in dirpath.iterdir():
-        if not filepath.is_file() or filepath.suffix not in suffixes:
-            continue
-
-        try:
-            filenum = int(filepath.stem)
-        except ValueError:
-            continue
-
-        if filenum > nummax:
-            nummax = filenum
-
-    def move_file(filepath):
-        newpath = numpath(filepath.suffix)
-        if newpath.exists():
-            raise FnumException("Can't override existing file {newpath.name}")
-
-        try:
-            order_index = metadata.order.index(filepath.name)
-            metadata.order[order_index] = newpath.name
-        except ValueError:
-            metadata.order.append(newpath.name)
-        try:
-            original_index = tuple(metadata.originals.values()).index(filepath.name)
-            original_key = tuple(metadata.originals.keys())[original_index]
-            metadata.originals[original_key] = newpath.name
-        except ValueError:
-            metadata.originals[filepath.name] = newpath.name
-
-        filepath.rename(newpath)
-        if include_imeta:
-            metapath = Path(ImageMetadata.for_image(str(filepath)))
-            newmetapath = metapath.parents[0] / f"{newpath.stem}{metapath.suffix}"
-            try:
-                metapath.rename(newmetapath)
-            except FileNotFoundError:
-                pass
-
-    for filenum in range(num, nummax + 1):
-        possible_names = tuple(dirpath / f"{filenum}{suffix}" for suffix in suffixes)
-        used_suffixes = tuple(
-            filepath for filepath in possible_names if filepath.exists()
-        )
-        if len(used_suffixes) > 1:
-            raise FnumException(
-                f"Unexpectedly found multiple existing files with number {filenum}"
-            )
-
-        if not used_suffixes:
-            for filepath in possible_names:
-                name = filepath.name
-                if name in metadata.order or name in metadata.originals.values():
-                    try:
-                        metadata.order.remove(name)
-                    except ValueError:
-                        pass
-                    try:
-                        original_index = tuple(metadata.originals.values()).index(name)
-                        original_key = tuple(metadata.originals.keys())[original_index]
-                        del metadata.originals[original_key]
-                    except ValueError:
-                        pass
-
-                    break
-            continue
-
-        filepath = used_suffixes[0]
-        move_file(filepath)
-        num += 1
-        if int(filepath.stem) == nummax:
-            break
-
-    # Find new files
     _log.info("Processing files...")
-    for filepath in dirpath.iterdir():
-        if not filepath.is_file() or filepath.suffix not in suffixes:
-            continue
-        try:
-            if int(filepath.stem) <= num:
-                continue
-        except ValueError:
-            pass
-
-        move_file(filepath)
-        num += 1
+    orchestrator.move_numbered()
+    orchestrator.move_new()
 
-    metadata.max = num - 1
-    return metadata
+    orchestrator.maybe_write_metadata()
```

## fnum/cli.py

```diff
@@ -61,22 +61,19 @@
     _log.setLevel(logging.INFO)
     handler = logging.StreamHandler(io.StringIO())
     handler.setFormatter(_ClickFormatter())
     _log.addHandler(handler)
 
     try:
         try:
-            metadata = number_files(
+            number_files(
                 dirpath=dirpath,
                 suffixes=suffixes,
+                write_metadata=kwargs["write_metadata"],
+                write_max=kwargs["write_max"],
                 include_imeta=kwargs["include_imeta"],
             )
         finally:
             _log.removeHandler(handler)
     except (FnumException, FileNotFoundError) as e:
         click.echo(str(e), err=True)
         sys.exit(1)
-
-    if kwargs["write_max"]:
-        metadata.get_max().to_file(dirpath)
-    if kwargs["write_metadata"]:
-        metadata.to_file(dirpath)
```

## Comparing `fnum-1.4.0.dist-info/LICENSE` & `fnum-1.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fnum-1.4.0.dist-info/METADATA` & `fnum-1.5.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnum
-Version: 1.4.0
+Version: 1.5.0
 Summary: Renames files in a directory using sequential integers
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/fnum
 Keywords: fnum,cli,utility,file,rename,sequential,order
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

