# Comparing `tmp/tinyimagenet-0.4.tar.gz` & `tmp/tinyimagenet-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyimagenet-0.4.tar", last modified: Tue Jul 11 15:16:37 2023, max compression
+gzip compressed data, was "tinyimagenet-0.5.tar", last modified: Tue Jul 11 15:27:28 2023, max compression
```

## Comparing `tinyimagenet-0.4.tar` & `tinyimagenet-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2023-07-11 15:16:37.284914 tinyimagenet-0.4/
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1072 2023-07-11 14:47:13.000000 tinyimagenet-0.4/LICENSE
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1650 2023-07-11 15:16:37.284914 tinyimagenet-0.4/PKG-INFO
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      774 2023-07-11 14:47:13.000000 tinyimagenet-0.4/README.md
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       38 2023-07-11 15:16:37.284914 tinyimagenet-0.4/setup.cfg
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     2943 2023-07-11 15:01:49.000000 tinyimagenet-0.4/setup.py
-drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2023-07-11 15:16:37.284914 tinyimagenet-0.4/tinyimagenet.egg-info/
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1650 2023-07-11 15:16:37.000000 tinyimagenet-0.4/tinyimagenet.egg-info/PKG-INFO
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      252 2023-07-11 15:16:37.000000 tinyimagenet-0.4/tinyimagenet.egg-info/SOURCES.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2023-07-11 15:16:37.000000 tinyimagenet-0.4/tinyimagenet.egg-info/dependency_links.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       12 2023-07-11 15:16:37.000000 tinyimagenet-0.4/tinyimagenet.egg-info/requires.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       13 2023-07-11 15:16:37.000000 tinyimagenet-0.4/tinyimagenet.egg-info/top_level.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2023-07-11 15:16:03.000000 tinyimagenet-0.4/tinyimagenet.egg-info/zip-safe
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     5773 2023-07-11 15:10:17.000000 tinyimagenet-0.4/tinyimagenet.py
+drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2023-07-11 15:27:28.845934 tinyimagenet-0.5/
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1072 2023-07-11 14:47:13.000000 tinyimagenet-0.5/LICENSE
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1665 2023-07-11 15:27:28.841934 tinyimagenet-0.5/PKG-INFO
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      789 2023-07-11 15:17:51.000000 tinyimagenet-0.5/README.md
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       38 2023-07-11 15:27:28.845934 tinyimagenet-0.5/setup.cfg
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     2943 2023-07-11 15:27:16.000000 tinyimagenet-0.5/setup.py
+drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2023-07-11 15:27:28.841934 tinyimagenet-0.5/tinyimagenet.egg-info/
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1665 2023-07-11 15:27:28.000000 tinyimagenet-0.5/tinyimagenet.egg-info/PKG-INFO
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      252 2023-07-11 15:27:28.000000 tinyimagenet-0.5/tinyimagenet.egg-info/SOURCES.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2023-07-11 15:27:28.000000 tinyimagenet-0.5/tinyimagenet.egg-info/dependency_links.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       12 2023-07-11 15:27:28.000000 tinyimagenet-0.5/tinyimagenet.egg-info/requires.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       13 2023-07-11 15:27:28.000000 tinyimagenet-0.5/tinyimagenet.egg-info/top_level.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2023-07-11 15:16:03.000000 tinyimagenet-0.5/tinyimagenet.egg-info/zip-safe
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     6235 2023-07-11 15:24:55.000000 tinyimagenet-0.5/tinyimagenet.py
```

### Comparing `tinyimagenet-0.4/LICENSE` & `tinyimagenet-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyimagenet-0.4/PKG-INFO` & `tinyimagenet-0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyimagenet
-Version: 0.4
+Version: 0.5
 Summary: Dataset class for PyTorch and the TinyImageNet dataset, with automated download and extraction.
 Home-page: https://github.com/facundoq/tinyimagenet
 Author: Facundo Manuel Quiroga
 Author-email: facundoq@gmail.com
 Project-URL: Bug Tracker, https://github.com/facundoq/tinyimagenet/issues
 Project-URL: Documentation, https://github.com/facundoq/tinyimagenet
 Project-URL: Source Code, https://github.com/facundoq/tinyimagenet
@@ -24,14 +24,15 @@
 
 ``` pip install tinyimagenet ```
 
 # How to use
 ````
 from tinyimagenet import TinyImageNet
 from pathlib import Path
+import logging
 
 logging.basicConfig(level=logging.INFO)
 
 split ="val"
 dataset = TinyImageNet(Path("~/.torchvision/tinyimagenet/"),split=split)
 n = len(dataset)
 print(f"TinyImageNet, split {split}, has  {n} samples.")
```

### Comparing `tinyimagenet-0.4/README.md` & `tinyimagenet-0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 ``` pip install tinyimagenet ```
 
 # How to use
 ````
 from tinyimagenet import TinyImageNet
 from pathlib import Path
+import logging
 
 logging.basicConfig(level=logging.INFO)
 
 split ="val"
 dataset = TinyImageNet(Path("~/.torchvision/tinyimagenet/"),split=split)
 n = len(dataset)
 print(f"TinyImageNet, split {split}, has  {n} samples.")
```

### Comparing `tinyimagenet-0.4/setup.py` & `tinyimagenet-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 url="https://github.com/facundoq/tinyimagenet"
-VERSION="0.4"
+VERSION="0.5"
 
 class UploadCommand(Command):
     """Support setup.py upload."""
 
     description = 'Build and publish the package.'
     user_options = []
```

### Comparing `tinyimagenet-0.4/tinyimagenet.egg-info/PKG-INFO` & `tinyimagenet-0.5/tinyimagenet.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyimagenet
-Version: 0.4
+Version: 0.5
 Summary: Dataset class for PyTorch and the TinyImageNet dataset, with automated download and extraction.
 Home-page: https://github.com/facundoq/tinyimagenet
 Author: Facundo Manuel Quiroga
 Author-email: facundoq@gmail.com
 Project-URL: Bug Tracker, https://github.com/facundoq/tinyimagenet/issues
 Project-URL: Documentation, https://github.com/facundoq/tinyimagenet
 Project-URL: Source Code, https://github.com/facundoq/tinyimagenet
@@ -24,14 +24,15 @@
 
 ``` pip install tinyimagenet ```
 
 # How to use
 ````
 from tinyimagenet import TinyImageNet
 from pathlib import Path
+import logging
 
 logging.basicConfig(level=logging.INFO)
 
 split ="val"
 dataset = TinyImageNet(Path("~/.torchvision/tinyimagenet/"),split=split)
 n = len(dataset)
 print(f"TinyImageNet, split {split}, has  {n} samples.")
```

### Comparing `tinyimagenet-0.4/tinyimagenet.py` & `tinyimagenet-0.5/tinyimagenet.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,28 +95,42 @@
                 writer = csv.writer(f,delimiter=delimiter)
                 for row in files:
                     writer.writerow(row)
         logging.warning(f"About to delete {images_root}")
         images_root.rmdir()
 
 
+
+    
+
 class TinyImageNet(ImageFolder):
     mean = [0.485, 0.456, 0.406]
     std = [0.229, 0.224, 0.225]
+    
+    def target_transform_imagenet_idx(self,tinyimagenet_idx):
+        print(tinyimagenet_idx)
+        klass = self.idx_to_class[tinyimagenet_idx]
+        imagenet_idx = imagenet1k.class_to_idx[klass]
+        return imagenet_idx
 
-    def __init__(self, root: Path, split: str = "train",transform=None, target_transform=None) -> None:
+    def __init__(self, root: Path, split: str = "train",transform=None, target_transform=None,imagenet_idx=False) -> None:
         if isinstance(root,str):
             root = Path(root)
         self.class_to_imagenet_idx = imagenet1k.class_to_idx 
         assert split in ["train","val","test"]
         root = root.expanduser()
         images_root = root/"tiny-imagenet-200/"
         if not images_root.exists():
             download_resources(root,mirrors,resources)        
         preprocess_val(images_root)
+        if target_transform is None:
+            target_transform = lambda x: x
+        if imagenet_idx:
+            target_transform = lambda x: target_transform(self.target_transform_imagenet_idx(x))
+
         super().__init__(images_root/split,transform=transform,target_transform=target_transform)
         self.idx_to_words,self.idx_to_class = self.load_words_classes(images_root)
     
     def load_words_classes(self,root:Path):
         tiny_classes = open(root/"wnids.txt", 'r').read().splitlines()
         with open(root/"words.txt") as f:
             words = {}
```

