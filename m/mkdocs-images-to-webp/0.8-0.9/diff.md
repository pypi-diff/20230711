# Comparing `tmp/mkdocs-images-to-webp-0.8.tar.gz` & `tmp/mkdocs-images-to-webp-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-images-to-webp-0.8.tar", last modified: Wed Jul  5 10:45:14 2023, max compression
+gzip compressed data, was "mkdocs-images-to-webp-0.9.tar", last modified: Wed Jul  5 10:55:34 2023, max compression
```

## Comparing `mkdocs-images-to-webp-0.8.tar` & `mkdocs-images-to-webp-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 10:45:14.133000 mkdocs-images-to-webp-0.8/
--rw-rw-r--   0 user      (1000) user      (1000)     1068 2023-01-25 09:31:29.000000 mkdocs-images-to-webp-0.8/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)      407 2023-07-05 10:45:14.133000 mkdocs-images-to-webp-0.8/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      648 2023-02-07 12:01:18.000000 mkdocs-images-to-webp-0.8/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 10:45:14.133000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-30 06:39:53.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1841 2023-07-05 10:40:35.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp/plugin.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 10:45:14.133000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      407 2023-07-05 10:45:14.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      389 2023-07-05 10:45:14.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-05 10:45:14.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       89 2023-07-05 10:45:14.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)      114 2023-07-05 10:45:14.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       22 2023-07-05 10:45:14.000000 mkdocs-images-to-webp-0.8/mkdocs_images_to_webp.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      430 2023-07-05 10:45:03.000000 mkdocs-images-to-webp-0.8/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)      380 2023-07-05 10:45:14.133000 mkdocs-images-to-webp-0.8/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      597 2023-07-05 10:44:59.000000 mkdocs-images-to-webp-0.8/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 10:55:34.396089 mkdocs-images-to-webp-0.9/
+-rw-rw-r--   0 user      (1000) user      (1000)     1068 2023-01-25 09:31:29.000000 mkdocs-images-to-webp-0.9/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)      407 2023-07-05 10:55:34.396089 mkdocs-images-to-webp-0.9/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      648 2023-02-07 12:01:18.000000 mkdocs-images-to-webp-0.9/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 10:55:34.396089 mkdocs-images-to-webp-0.9/mkdocs_images_to_webp/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-30 06:39:53.000000 mkdocs-images-to-webp-0.9/mkdocs_images_to_webp/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1770 2023-07-05 10:52:24.000000 mkdocs-images-to-webp-0.9/mkdocs_images_to_webp/plugin.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-05 10:55:34.396089 mkdocs-images-to-webp-0.9/mkdocs_images_to_webp.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      407 2023-07-05 10:55:34.000000 mkdocs-images-to-webp-0.9/mkdocs_images_to_webp.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      389 2023-07-05 10:55:34.000000 mkdocs-images-to-webp-0.9/mkdocs_images_to_webp.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-05 10:55:34.000000 mkdocs-images-to-webp-0.9/mkdocs_images_to_webp.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       89 2023-07-05 10:55:34.000000 mkdocs-images-to-webp-0.9/mkdocs_images_to_webp.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      114 2023-07-05 10:55:34.000000 mkdocs-images-to-webp-0.9/mkdocs_images_to_webp.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       22 2023-07-05 10:55:34.000000 mkdocs-images-to-webp-0.9/mkdocs_images_to_webp.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      430 2023-07-05 10:55:21.000000 mkdocs-images-to-webp-0.9/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)      380 2023-07-05 10:55:34.396089 mkdocs-images-to-webp-0.9/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      597 2023-07-05 10:55:24.000000 mkdocs-images-to-webp-0.9/setup.py
```

### Comparing `mkdocs-images-to-webp-0.8/LICENSE` & `mkdocs-images-to-webp-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-images-to-webp-0.8/README.md` & `mkdocs-images-to-webp-0.9/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-images-to-webp-0.8/mkdocs_images_to_webp/plugin.py` & `mkdocs-images-to-webp-0.9/mkdocs_images_to_webp/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 
     def on_files(self, files, config):
         extensions_local = list([extension for extension in self.config.extensions])
         for file in files:
             for extension in extensions_local:
                 if file.abs_src_path.endswith(extension):
                     image = Image.open(file.abs_src_path)
-                    file.abs_src_path = file.abs_src_path[:len(file.abs_src_path) - 4] + ".webp"
+                    file.abs_src_path = file.abs_src_path + ".webp"
                     image.save(file.abs_src_path, format='webp')
-                    file.abs_dest_path = file.abs_dest_path[:len(file.abs_src_path) - 4] + ".webp"
+                    file.abs_dest_path = file.abs_dest_path + ".webp"
                     break
         print("INFO     -  [images-to-webp] Formats", ', '.join(extensions_local), 'successfully changed to webp')
         return files
 
     def on_page_content(self, html, page, config, files):
         extensions_local = list([extension for extension in self.config.extensions])
         for extension in extensions_local:
-            html = html.replace(extension, extension + ".webp")
+            html = html.replace(extension, "webp")
         return html
 
     # def on_post_build(self, config):
     #     target_dir = self.config.img_dir
     #     self.clean(target_dir)
```

### Comparing `mkdocs-images-to-webp-0.8/setup.py` & `mkdocs-images-to-webp-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='mkdocs-images-to-webp',
-    version='0.8',
+    version='0.9',
     install_requires=[
         'mkdocs == 1.4.2',
         'pillow',
         'importlib-metadata; python_version == "3.8"',
     ],
     author='mur4d1n',
     author_email='mur4d1n@yandex.ru',
```

