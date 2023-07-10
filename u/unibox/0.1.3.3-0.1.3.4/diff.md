# Comparing `tmp/unibox-0.1.3.3.tar.gz` & `tmp/unibox-0.1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unibox-0.1.3.3.tar", max compression
+gzip compressed data, was "unibox-0.1.3.4.tar", max compression
```

## Comparing `unibox-0.1.3.3.tar` & `unibox-0.1.3.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-07-10 23:04:27.849640 unibox-0.1.3.3/LICENSE
--rw-r--r--   0        0        0      125 2023-07-10 23:04:27.849640 unibox-0.1.3.3/README.md
--rw-r--r--   0        0        0      444 2023-07-10 23:04:27.849640 unibox-0.1.3.3/pyproject.toml
--rw-r--r--   0        0        0       76 2023-07-10 23:04:27.849640 unibox-0.1.3.3/unibox/__init__.py
--rw-r--r--   0        0        0     1403 2023-07-10 23:04:27.849640 unibox-0.1.3.3/unibox/cli.py
--rw-r--r--   0        0        0        0 2023-07-10 23:04:27.849640 unibox-0.1.3.3/unibox/processing/__init__.py
--rw-r--r--   0        0        0     5195 2023-07-10 23:04:27.849640 unibox-0.1.3.3/unibox/processing/image_resizer.py
--rw-r--r--   0        0        0        0 2023-07-10 23:04:27.849640 unibox-0.1.3.3/unibox/utils/__init__.py
--rw-r--r--   0        0        0     2743 2023-07-10 23:04:27.849640 unibox-0.1.3.3/unibox/utils/data_loader.py
--rw-r--r--   0        0        0     3423 2023-07-10 23:04:27.849640 unibox-0.1.3.3/unibox/utils/logger.py
--rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 unibox-0.1.3.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-10 23:45:04.957926 unibox-0.1.3.4/LICENSE
+-rw-r--r--   0        0        0      546 2023-07-10 23:45:04.957926 unibox-0.1.3.4/README.md
+-rw-r--r--   0        0        0      444 2023-07-10 23:45:04.957926 unibox-0.1.3.4/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-07-10 23:45:04.957926 unibox-0.1.3.4/unibox/__init__.py
+-rw-r--r--   0        0        0     1586 2023-07-10 23:45:04.957926 unibox-0.1.3.4/unibox/cli.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:45:04.957926 unibox-0.1.3.4/unibox/processing/__init__.py
+-rw-r--r--   0        0        0     5896 2023-07-10 23:45:04.957926 unibox-0.1.3.4/unibox/processing/image_resizer.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:45:04.957926 unibox-0.1.3.4/unibox/utils/__init__.py
+-rw-r--r--   0        0        0     2743 2023-07-10 23:45:04.957926 unibox-0.1.3.4/unibox/utils/data_loader.py
+-rw-r--r--   0        0        0     3423 2023-07-10 23:45:04.957926 unibox-0.1.3.4/unibox/utils/logger.py
+-rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 unibox-0.1.3.4/PKG-INFO
```

### Comparing `unibox-0.1.3.3/LICENSE` & `unibox-0.1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unibox-0.1.3.3/unibox/cli.py` & `unibox-0.1.3.4/unibox/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,15 +36,20 @@
         format = click.prompt('- File format', default="webp")
     if not dst_dir:
         src_dir_name = os.path.basename(os.path.abspath(src_dir))
         dst_dir = click.prompt('- Destination', default=f"{src_dir_name}_{min_side}_{format}")
     if not quality:
         quality = click.prompt('- Image quality', type=int, default=95)
 
+    # Printing the command
+    print("\nRunning Command:\n")
+    print(f"unibox resize {src_dir} --min_side {min_side} --dst_dir {dst_dir} --format {format} --quality {quality}\n")
+
     resizer = image_resizer.ImageResizer(src_dir, dst_dir, min_side, format=format, quality=quality)
     resizer.resize_images()
 
 
+
 cli.add_command(setup)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `unibox-0.1.3.3/unibox/processing/image_resizer.py` & `unibox-0.1.3.4/unibox/processing/image_resizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import concurrent.futures
+import multiprocessing
 import os
 from pathlib import Path
 from PIL import Image
 from tqdm.auto import tqdm
 
+
 try:
     import pyvips
 
     # Try to create a small image using libvips to check if it's working.
     pyvips.Image.black(1, 1)
     HAS_PYVIPS = True
 except ImportError:
@@ -24,14 +26,15 @@
         Initialize an instance of ImageResizer.
         """
         self.src_dir = Path(src_dir)
         self.dst_dir = Path(dst_dir)
         self.min_side = min_side
         self.format = self._validate_format(format)
         self.quality = quality
+        self.num_processes = multiprocessing.cpu_count()
 
     def _validate_format(self, format: str) -> str:
         """
         Validate the provided image format.
         """
         if format not in SUPPORTED_FORMATS:
             raise ValueError(f"Unsupported image format '{format}'. Supported formats are {SUPPORTED_FORMATS}.")
@@ -96,14 +99,16 @@
 
         if min_dim <= self.min_side:
             return None
 
         scale = self.min_side / min_dim
         return image.resize(scale)
 
+    def _task(self, file_path, relative_path):
+        self._resize_image(file_path, relative_path)
     def _save_image(self, image, dst_path: Path):
         """
         Save an image in the specified format.
         """
         save_methods = {
             "jpg": {"pil": "JPEG", "pyvips": "jpegsave", "params": {"Q": self.quality}},
             "webp": {"pil": "WEBP", "pyvips": "webpsave", "params": {"Q": self.quality}},
@@ -115,37 +120,51 @@
             if HAS_PYVIPS:
                 getattr(image, method_map["pyvips"])(str(dst_path), **method_map["params"])
             else:
                 image.save(dst_path, method_map["pil"], **method_map["params"])
         except Exception as e:
             print(f"Error saving image {dst_path}. Skipping...\n{str(e)}")
 
+
     def _execute_resize(self, tasks):
         """
-        Execute tasks using ThreadPoolExecutor
+        Execute tasks using ProcessPoolExecutor
         """
-        with concurrent.futures.ThreadPoolExecutor() as executor:
-            list(tqdm(executor.map(lambda task: task(), tasks), total=len(tasks),
+        with concurrent.futures.ProcessPoolExecutor(max_workers=self.num_processes) as executor:
+            futures = [executor.submit(task, *args) for task, *args in tasks]
+            list(tqdm(concurrent.futures.as_completed(futures), total=len(tasks),
                       desc=f"Resizing images to min_side={self.min_side}"))
 
     def resize_images(self):
         """
         Resize all supported images in the source directory.
         """
         tasks = []
 
+        self._print_debug_string()
+
         for file_path in self.src_dir.rglob("*"):
             if file_path.is_file() and file_path.suffix[1:].lower() in SUPPORTED_FORMATS:
                 relative_path = file_path.relative_to(self.src_dir)
-                tasks.append(
-                    (lambda _image: lambda: self._resize_image(_image, _image.relative_to(self.src_dir)))(file_path))
+                tasks.append((self._task, file_path, relative_path))
 
         self._execute_resize(tasks)
 
-        return f"Resized {len(tasks)} images to min_side={self.min_side}"
+    def _print_debug_string(self):
+        """
+        prints debug message once resize_images is called
+        """
+        debug_string = ""
+        if HAS_PYVIPS:
+            debug_string += "Resizing with libvips: "
+        else:
+            debug_string += "Resizing with PIL: "
+        debug_string += f"num_processes = {self.num_processes}, src_dir={self.src_dir}, dst_dir={self.dst_dir}, " \
+                        f"min_side={self.min_side}, format={self.format}, quality={self.quality}"
+        print(debug_string)
 
 
 if __name__ == "__main__":
     # Define the source and destination directories and the minimum side length for resizing
     src_dir = input("dir path:")
 
     dst_dir = f"{src_dir}_768webp"
```

### Comparing `unibox-0.1.3.3/unibox/utils/data_loader.py` & `unibox-0.1.3.4/unibox/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `unibox-0.1.3.3/unibox/utils/logger.py` & `unibox-0.1.3.4/unibox/utils/logger.py`

 * *Files identical despite different names*

