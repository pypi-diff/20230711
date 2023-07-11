# Comparing `tmp/idownload-1.1.0-py3-none-any.whl.zip` & `tmp/idownload-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5610 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-09 20:11 idownload/__init__.py
--rw-r--r--  2.0 unx       29 b- defN 23-Jul-09 20:11 idownload/__main__.py
--rw-r--r--  2.0 unx     1018 b- defN 23-Jul-09 20:11 idownload/cli.py
--rw-r--r--  2.0 unx      241 b- defN 23-Jul-09 20:11 idownload/exceptions.py
--rw-r--r--  2.0 unx       69 b- defN 23-Jul-09 20:11 idownload/sources/__init__.py
--rw-r--r--  2.0 unx     3965 b- defN 23-Jul-09 20:11 idownload/sources/pinterest.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-09 20:11 idownload-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1351 b- defN 23-Jul-09 20:11 idownload-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 20:11 idownload-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Jul-09 20:11 idownload-1.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-09 20:11 idownload-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      968 b- defN 23-Jul-09 20:11 idownload-1.1.0.dist-info/RECORD
-12 files, 8882 bytes uncompressed, 3974 bytes compressed:  55.3%
+Zip file size: 5653 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-11 04:14 idownload/__init__.py
+-rw-r--r--  2.0 unx       29 b- defN 23-Jul-11 04:14 idownload/__main__.py
+-rw-r--r--  2.0 unx     1019 b- defN 23-Jul-11 04:14 idownload/cli.py
+-rw-r--r--  2.0 unx      241 b- defN 23-Jul-11 04:14 idownload/exceptions.py
+-rw-r--r--  2.0 unx       69 b- defN 23-Jul-11 04:14 idownload/sources/__init__.py
+-rw-r--r--  2.0 unx     4173 b- defN 23-Jul-11 04:14 idownload/sources/pinterest.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-11 04:15 idownload-1.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1351 b- defN 23-Jul-11 04:15 idownload-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 04:15 idownload-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Jul-11 04:15 idownload-1.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-11 04:15 idownload-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      968 b- defN 23-Jul-11 04:15 idownload-1.2.0.dist-info/RECORD
+12 files, 9091 bytes uncompressed, 4017 bytes compressed:  55.8%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: idownload/sources/__init__.py
 Comment: 
 
 Filename: idownload/sources/pinterest.py
 Comment: 
 
-Filename: idownload-1.1.0.dist-info/LICENSE
+Filename: idownload-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: idownload-1.1.0.dist-info/METADATA
+Filename: idownload-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: idownload-1.1.0.dist-info/WHEEL
+Filename: idownload-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: idownload-1.1.0.dist-info/entry_points.txt
+Filename: idownload-1.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: idownload-1.1.0.dist-info/top_level.txt
+Filename: idownload-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: idownload-1.1.0.dist-info/RECORD
+Filename: idownload-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## idownload/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.0"
+__version__ = "1.2.0"
```

## idownload/cli.py

```diff
@@ -15,15 +15,15 @@
 def cli(**kwargs):
     pass
 
 
 for source in SOURCES:
 
     def command(**kwargs):
-        kwargs["progressbar"] = click.progressbar
+        kwargs["_progressbar"] = click.progressbar
         try:
             source.download(**kwargs)
         except SourceAccessException as e:
             click.echo(str(e), err=True)
 
     command.__name__ = source.COMMAND
     for arg in reversed(source.ARGS):
```

## idownload/sources/pinterest.py

```diff
@@ -31,31 +31,36 @@
 
 
 class PinterestSource:
     COMMAND = "pinterest"
     ARGS = ("username", "board", "dirpath")
 
     @classmethod
-    def download(cls, username, board, dirpath, progressbar=None, with_attr=False):
+    def download(cls, username, board, dirpath, with_attr=False, _progressbar=None):
         url = f"https://www.pinterest.com/{username}/{board}.rss"
         feed = feedparser.parse(url)
         if feed.status < 200 or feed.status > 299:
             raise SourceAccessException(
                 f"HTTP status {feed.status} while requesting feed {url}"
             )
 
-        if not progressbar:
+        if not _progressbar:
 
             @contextmanager
             def noop_progressbar(*args, **kwargs):
                 yield args[0]
 
-            progressbar = noop_progressbar
+            _progressbar = noop_progressbar
 
-        with progressbar(feed["items"], label="Downloading images") as bar:
+        try:
+            fnum_metadata = FnumMetadata.from_file(dirpath)
+        except FileNotFoundError:
+            fnum_metadata = None
+
+        with _progressbar(feed["items"], label="Downloading images") as bar:
             for item in bar:
                 source_name = item["title"]
                 if with_attr:
                     try:
                         source_name = nameattr.from_text(source_name)
                     except:
                         print(nameattr_err, end="")
@@ -83,23 +88,18 @@
 
                 suffixes = (".jpg", ".png")
                 dirpath = Path(dirpath)
                 possible_urls = list(f"{url_start}{suffix}" for suffix in suffixes)
 
                 if any((dirpath / Path(url).name).exists() for url in possible_urls):
                     continue
-                try:
-                    fnum_metadata = FnumMetadata.from_file(dirpath)
-                    if any(
-                        fnum_metadata.contains(str(Path(url).name))
-                        for url in possible_urls
-                    ):
-                        continue
-                except FileNotFoundError:
-                    pass
+                if fnum_metadata and any(
+                    fnum_metadata.contains(str(Path(url).name)) for url in possible_urls
+                ):
+                    continue
 
                 while possible_urls:
                     image_url = possible_urls.pop(0)
                     try:
                         request = urllib.request.Request(image_url)
                         data = urllib.request.urlopen(request).read()
                         break
@@ -107,7 +107,13 @@
                         if e.getcode() != 403 or not possible_urls:
                             raise ImageDownloadException(image_url, e)
 
                 filepath = dirpath / Path(image_url).name
                 filepath.write_bytes(data)
                 metadata["extension"] = filepath.suffix[1:]
                 ImageMetadata(metadata).to_image(str(filepath))
+                if fnum_metadata:
+                    fnum_metadata.order.append(filepath.name)
+                    fnum_metadata.originals[filepath.name] = filepath.name
+
+        if fnum_metadata:
+            fnum_metadata.to_file(dirpath)
```

## Comparing `idownload-1.1.0.dist-info/LICENSE` & `idownload-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `idownload-1.1.0.dist-info/METADATA` & `idownload-1.2.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idownload
-Version: 1.1.0
+Version: 1.2.0
 Summary: Downloads images and stores metadata about them in a JSON file
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/idownload
 Keywords: idownload,cli,utility,image,download,backup,archive,pinterest
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -20,15 +20,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8.0
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: feedparser (~=6.0)
 Requires-Dist: imeta (~=1.1)
-Requires-Dist: fnum (~=1.2)
+Requires-Dist: fnum (~=1.5)
 Provides-Extra: nameattr
 Requires-Dist: nameattr (~=1.0) ; extra == 'nameattr'
 Provides-Extra: tests
 Requires-Dist: pytest ; extra == 'tests'
 Requires-Dist: networktest ; extra == 'tests'
 Requires-Dist: nameattr (~=1.0) ; extra == 'tests'
```

