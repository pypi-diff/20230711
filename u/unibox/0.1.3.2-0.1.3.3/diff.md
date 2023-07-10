# Comparing `tmp/unibox-0.1.3.2.tar.gz` & `tmp/unibox-0.1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unibox-0.1.3.2.tar", max compression
+gzip compressed data, was "unibox-0.1.3.3.tar", max compression
```

## Comparing `unibox-0.1.3.2.tar` & `unibox-0.1.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-07-10 22:56:58.595244 unibox-0.1.3.2/LICENSE
--rw-r--r--   0        0        0      125 2023-07-10 22:56:58.595244 unibox-0.1.3.2/README.md
--rw-r--r--   0        0        0      444 2023-07-10 22:56:58.595244 unibox-0.1.3.2/pyproject.toml
--rw-r--r--   0        0        0       76 2023-07-10 22:56:58.595244 unibox-0.1.3.2/unibox/__init__.py
--rw-r--r--   0        0        0     1403 2023-07-10 22:56:58.595244 unibox-0.1.3.2/unibox/cli.py
--rw-r--r--   0        0        0        0 2023-07-10 22:56:58.595244 unibox-0.1.3.2/unibox/processing/__init__.py
--rw-r--r--   0        0        0     5451 2023-07-10 22:56:58.595244 unibox-0.1.3.2/unibox/processing/image_resizer.py
--rw-r--r--   0        0        0        0 2023-07-10 22:56:58.595244 unibox-0.1.3.2/unibox/utils/__init__.py
--rw-r--r--   0        0        0     2743 2023-07-10 22:56:58.595244 unibox-0.1.3.2/unibox/utils/data_loader.py
--rw-r--r--   0        0        0     3423 2023-07-10 22:56:58.595244 unibox-0.1.3.2/unibox/utils/logger.py
--rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 unibox-0.1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-10 23:04:27.849640 unibox-0.1.3.3/LICENSE
+-rw-r--r--   0        0        0      125 2023-07-10 23:04:27.849640 unibox-0.1.3.3/README.md
+-rw-r--r--   0        0        0      444 2023-07-10 23:04:27.849640 unibox-0.1.3.3/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-07-10 23:04:27.849640 unibox-0.1.3.3/unibox/__init__.py
+-rw-r--r--   0        0        0     1403 2023-07-10 23:04:27.849640 unibox-0.1.3.3/unibox/cli.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:04:27.849640 unibox-0.1.3.3/unibox/processing/__init__.py
+-rw-r--r--   0        0        0     5195 2023-07-10 23:04:27.849640 unibox-0.1.3.3/unibox/processing/image_resizer.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:04:27.849640 unibox-0.1.3.3/unibox/utils/__init__.py
+-rw-r--r--   0        0        0     2743 2023-07-10 23:04:27.849640 unibox-0.1.3.3/unibox/utils/data_loader.py
+-rw-r--r--   0        0        0     3423 2023-07-10 23:04:27.849640 unibox-0.1.3.3/unibox/utils/logger.py
+-rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 unibox-0.1.3.3/PKG-INFO
```

### Comparing `unibox-0.1.3.2/LICENSE` & `unibox-0.1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unibox-0.1.3.2/unibox/cli.py` & `unibox-0.1.3.3/unibox/cli.py`

 * *Files identical despite different names*

### Comparing `unibox-0.1.3.2/unibox/processing/image_resizer.py` & `unibox-0.1.3.3/unibox/processing/image_resizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,22 @@
         """
         self.src_dir = Path(src_dir)
         self.dst_dir = Path(dst_dir)
         self.min_side = min_side
         self.format = self._validate_format(format)
         self.quality = quality
 
+    def _validate_format(self, format: str) -> str:
+        """
+        Validate the provided image format.
+        """
+        if format not in SUPPORTED_FORMATS:
+            raise ValueError(f"Unsupported image format '{format}'. Supported formats are {SUPPORTED_FORMATS}.")
+        return format
+
     def _resize_image(self, file_path: Path, relative_path: Path):
         """
         Resize a single image and save the result.
         """
         dst_path = self.dst_dir / relative_path.with_suffix(f".{self.format}")
 
         # Ensure the destination directory exists
@@ -107,31 +115,14 @@
             if HAS_PYVIPS:
                 getattr(image, method_map["pyvips"])(str(dst_path), **method_map["params"])
             else:
                 image.save(dst_path, method_map["pil"], **method_map["params"])
         except Exception as e:
             print(f"Error saving image {dst_path}. Skipping...\n{str(e)}")
 
-    def _resize_image(self, file_path: Path, relative_path: Path):
-        """
-        Resize a single image and save the result.
-        """
-        dst_path = self.dst_dir / relative_path.with_suffix(f".{self.format}")
-
-        # Ensure the destination directory exists
-        dst_path.parent.mkdir(parents=True, exist_ok=True)
-
-        if HAS_PYVIPS:
-            image = self._resize_with_pyvips(file_path)
-        else:
-            image = self._resize_with_pil(file_path)
-
-        if image is not None:
-            self._save_image(image, dst_path)
-
     def _execute_resize(self, tasks):
         """
         Execute tasks using ThreadPoolExecutor
         """
         with concurrent.futures.ThreadPoolExecutor() as executor:
             list(tqdm(executor.map(lambda task: task(), tasks), total=len(tasks),
                       desc=f"Resizing images to min_side={self.min_side}"))
```

### Comparing `unibox-0.1.3.2/unibox/utils/data_loader.py` & `unibox-0.1.3.3/unibox/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `unibox-0.1.3.2/unibox/utils/logger.py` & `unibox-0.1.3.3/unibox/utils/logger.py`

 * *Files identical despite different names*

### Comparing `unibox-0.1.3.2/PKG-INFO` & `unibox-0.1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unibox
-Version: 0.1.3.2
+Version: 0.1.3.3
 Summary: one toolbox to rule'em all
 License: GPL-3.0
 Author: yada
 Author-email: trojblue@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

