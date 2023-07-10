# Comparing `tmp/unibox-0.1.3.tar.gz` & `tmp/unibox-0.1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unibox-0.1.3.tar", max compression
+gzip compressed data, was "unibox-0.1.3.2.tar", max compression
```

## Comparing `unibox-0.1.3.tar` & `unibox-0.1.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-07-10 22:24:32.736801 unibox-0.1.3/LICENSE
--rw-r--r--   0        0        0      125 2023-07-10 22:24:32.736801 unibox-0.1.3/README.md
--rw-r--r--   0        0        0      442 2023-07-10 22:24:32.740802 unibox-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       76 2023-07-10 22:24:32.740802 unibox-0.1.3/unibox/__init__.py
--rw-r--r--   0        0        0     1317 2023-07-10 22:24:32.740802 unibox-0.1.3/unibox/cli.py
--rw-r--r--   0        0        0        0 2023-07-10 22:24:32.740802 unibox-0.1.3/unibox/processing/__init__.py
--rw-r--r--   0        0        0     4852 2023-07-10 22:24:32.740802 unibox-0.1.3/unibox/processing/image_resizer.py
--rw-r--r--   0        0        0        0 2023-07-10 22:24:32.740802 unibox-0.1.3/unibox/utils/__init__.py
--rw-r--r--   0        0        0     2743 2023-07-10 22:24:32.740802 unibox-0.1.3/unibox/utils/data_loader.py
--rw-r--r--   0        0        0     3423 2023-07-10 22:24:32.740802 unibox-0.1.3/unibox/utils/logger.py
--rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 unibox-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-10 22:56:58.595244 unibox-0.1.3.2/LICENSE
+-rw-r--r--   0        0        0      125 2023-07-10 22:56:58.595244 unibox-0.1.3.2/README.md
+-rw-r--r--   0        0        0      444 2023-07-10 22:56:58.595244 unibox-0.1.3.2/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-07-10 22:56:58.595244 unibox-0.1.3.2/unibox/__init__.py
+-rw-r--r--   0        0        0     1403 2023-07-10 22:56:58.595244 unibox-0.1.3.2/unibox/cli.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:56:58.595244 unibox-0.1.3.2/unibox/processing/__init__.py
+-rw-r--r--   0        0        0     5451 2023-07-10 22:56:58.595244 unibox-0.1.3.2/unibox/processing/image_resizer.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:56:58.595244 unibox-0.1.3.2/unibox/utils/__init__.py
+-rw-r--r--   0        0        0     2743 2023-07-10 22:56:58.595244 unibox-0.1.3.2/unibox/utils/data_loader.py
+-rw-r--r--   0        0        0     3423 2023-07-10 22:56:58.595244 unibox-0.1.3.2/unibox/utils/logger.py
+-rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 unibox-0.1.3.2/PKG-INFO
```

### Comparing `unibox-0.1.3/LICENSE` & `unibox-0.1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unibox-0.1.3/unibox/cli.py` & `unibox-0.1.3.2/unibox/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+import os
 import click
 
 from .processing import image_resizer
 
+
 @click.group()
 def cli():
     pass
 
+
 @click.group()
 def setup():
     pass
 
+
 @setup.command()
 def awscli():
     # install_awscli()
     print('Setting up awscli')
 
+
 @cli.command()
 @click.argument('src_dir')
 @click.option('--min_side', '-m', default=None, type=int, help='Minimum side length of the image.')
 @click.option('--dst_dir', '-d', default=None, help='Destination directory for the images.')
 @click.option('--format', '-f', default=None, help='Format of the image.')
 @click.option('--quality', '-q', default=None, type=int, help='Quality of the image.')
 def resize(src_dir, min_side, dst_dir, format, quality):
@@ -26,18 +31,20 @@
     print(f'Resizing directory: {src_dir}')
 
     if not min_side:
         min_side = click.prompt('- Minimum side length', type=int, default=768)
     if not format:
         format = click.prompt('- File format', default="webp")
     if not dst_dir:
-        dst_dir = click.prompt('- Destination', default=f"{src_dir}_{min_side}_{format}")
+        src_dir_name = os.path.basename(os.path.abspath(src_dir))
+        dst_dir = click.prompt('- Destination', default=f"{src_dir_name}_{min_side}_{format}")
     if not quality:
         quality = click.prompt('- Image quality', type=int, default=95)
 
     resizer = image_resizer.ImageResizer(src_dir, dst_dir, min_side, format=format, quality=quality)
     resizer.resize_images()
 
+
 cli.add_command(setup)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `unibox-0.1.3/unibox/processing/image_resizer.py` & `unibox-0.1.3.2/unibox/processing/image_resizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,37 +25,52 @@
         """
         self.src_dir = Path(src_dir)
         self.dst_dir = Path(dst_dir)
         self.min_side = min_side
         self.format = self._validate_format(format)
         self.quality = quality
 
-    def _validate_format(self, format: str) -> str:
+    def _resize_image(self, file_path: Path, relative_path: Path):
         """
-        Validate the provided image format.
+        Resize a single image and save the result.
         """
-        if format not in SUPPORTED_FORMATS:
-            raise ValueError(f"Unsupported image format '{format}'. Supported formats are {SUPPORTED_FORMATS}.")
-        return format
+        dst_path = self.dst_dir / relative_path.with_suffix(f".{self.format}")
+
+        # Ensure the destination directory exists
+        dst_path.parent.mkdir(parents=True, exist_ok=True)
+
+        if HAS_PYVIPS:
+            image = self._resize_with_pyvips(file_path)
+        else:
+            image = self._resize_with_pil(file_path)
+
+        # Image might not need resizing but still needs to be saved in new format
+        if image is None:
+            if HAS_PYVIPS:
+                image = pyvips.Image.new_from_file(str(file_path), access="sequential")
+            else:
+                image = Image.open(file_path)
+
+        self._save_image(image, dst_path)
 
     def _resize_with_pil(self, image_path: Path) -> Image:
         """
         Resize an image using PIL.
         """
         try:
             image = Image.open(image_path)
         except IOError:
             print(f"Error opening image {image_path}. Skipping...")
             return None
 
         width, height = image.size
         min_dim = min(width, height)
 
-        if min_dim < self.min_side:
-            return image
+        if min_dim <= self.min_side:
+            return None
 
         scale = self.min_side / min_dim
         new_width = round(width * scale)
         new_height = round(height * scale)
 
         return image.resize((new_width, new_height), Image.LANCZOS)
 
@@ -65,15 +80,20 @@
         """
         try:
             image = pyvips.Image.new_from_file(str(image_path), access="sequential")
         except pyvips.error.Error:
             print(f"Error opening image {image_path} with pyvips. Skipping...")
             return None
 
-        scale = self.min_side / min(image.width, image.height)
+        min_dim = min(image.width, image.height)
+
+        if min_dim <= self.min_side:
+            return None
+
+        scale = self.min_side / min_dim
         return image.resize(scale)
 
     def _save_image(self, image, dst_path: Path):
         """
         Save an image in the specified format.
         """
         save_methods = {
```

### Comparing `unibox-0.1.3/unibox/utils/data_loader.py` & `unibox-0.1.3.2/unibox/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `unibox-0.1.3/unibox/utils/logger.py` & `unibox-0.1.3.2/unibox/utils/logger.py`

 * *Files identical despite different names*

### Comparing `unibox-0.1.3/PKG-INFO` & `unibox-0.1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unibox
-Version: 0.1.3
+Version: 0.1.3.2
 Summary: one toolbox to rule'em all
 License: GPL-3.0
 Author: yada
 Author-email: trojblue@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

