# Comparing `tmp/tinyimagenet-0.3.tar.gz` & `tmp/tinyimagenet-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyimagenet-0.3.tar", last modified: Tue Jul 12 19:45:07 2022, max compression
+gzip compressed data, was "tinyimagenet-0.4.tar", last modified: Tue Jul 11 15:16:37 2023, max compression
```

## Comparing `tinyimagenet-0.3.tar` & `tinyimagenet-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2022-07-12 19:45:07.326281 tinyimagenet-0.3/
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1072 2022-07-11 23:44:40.000000 tinyimagenet-0.3/LICENSE
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1519 2022-07-12 19:45:07.326281 tinyimagenet-0.3/PKG-INFO
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      606 2022-07-12 00:04:33.000000 tinyimagenet-0.3/README.md
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       38 2022-07-12 19:45:07.326281 tinyimagenet-0.3/setup.cfg
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     2943 2022-07-12 19:44:52.000000 tinyimagenet-0.3/setup.py
-drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2022-07-12 19:45:07.326281 tinyimagenet-0.3/tinyimagenet.egg-info/
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1519 2022-07-12 19:45:07.000000 tinyimagenet-0.3/tinyimagenet.egg-info/PKG-INFO
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      252 2022-07-12 19:45:07.000000 tinyimagenet-0.3/tinyimagenet.egg-info/SOURCES.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2022-07-12 19:45:07.000000 tinyimagenet-0.3/tinyimagenet.egg-info/dependency_links.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       12 2022-07-12 19:45:07.000000 tinyimagenet-0.3/tinyimagenet.egg-info/requires.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       13 2022-07-12 19:45:07.000000 tinyimagenet-0.3/tinyimagenet.egg-info/top_level.txt
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2022-07-12 19:44:33.000000 tinyimagenet-0.3/tinyimagenet.egg-info/zip-safe
--rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     5694 2022-07-12 19:42:51.000000 tinyimagenet-0.3/tinyimagenet.py
+drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2023-07-11 15:16:37.284914 tinyimagenet-0.4/
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1072 2023-07-11 14:47:13.000000 tinyimagenet-0.4/LICENSE
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1650 2023-07-11 15:16:37.284914 tinyimagenet-0.4/PKG-INFO
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      774 2023-07-11 14:47:13.000000 tinyimagenet-0.4/README.md
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       38 2023-07-11 15:16:37.284914 tinyimagenet-0.4/setup.cfg
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     2943 2023-07-11 15:01:49.000000 tinyimagenet-0.4/setup.py
+drwxrwxr-x   0 facundoq  (1000) facundoq  (1000)        0 2023-07-11 15:16:37.284914 tinyimagenet-0.4/tinyimagenet.egg-info/
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     1650 2023-07-11 15:16:37.000000 tinyimagenet-0.4/tinyimagenet.egg-info/PKG-INFO
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)      252 2023-07-11 15:16:37.000000 tinyimagenet-0.4/tinyimagenet.egg-info/SOURCES.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2023-07-11 15:16:37.000000 tinyimagenet-0.4/tinyimagenet.egg-info/dependency_links.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       12 2023-07-11 15:16:37.000000 tinyimagenet-0.4/tinyimagenet.egg-info/requires.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)       13 2023-07-11 15:16:37.000000 tinyimagenet-0.4/tinyimagenet.egg-info/top_level.txt
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)        1 2023-07-11 15:16:03.000000 tinyimagenet-0.4/tinyimagenet.egg-info/zip-safe
+-rw-rw-r--   0 facundoq  (1000) facundoq  (1000)     5773 2023-07-11 15:10:17.000000 tinyimagenet-0.4/tinyimagenet.py
```

### Comparing `tinyimagenet-0.3/LICENSE` & `tinyimagenet-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyimagenet-0.3/PKG-INFO` & `tinyimagenet-0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: tinyimagenet
-Version: 0.3
+Version: 0.4
 Summary: Dataset class for PyTorch and the TinyImageNet dataset, with automated download and extraction.
 Home-page: https://github.com/facundoq/tinyimagenet
 Author: Facundo Manuel Quiroga
 Author-email: facundoq@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/facundoq/tinyimagenet/issues
 Project-URL: Documentation, https://github.com/facundoq/tinyimagenet
 Project-URL: Source Code, https://github.com/facundoq/tinyimagenet
 Keywords: TinyImageNet ImageNet Dataset PyTorch torch torchvision
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # torchvision-tinyimagenet
 Dataset class for PyTorch and the TinyImageNet dataset.
 
+# Installation
+
+``` pip install tinyimagenet ```
 
 # How to use
 ````
 from tinyimagenet import TinyImageNet
-import logging
 from pathlib import Path
 
 logging.basicConfig(level=logging.INFO)
 
 split ="val"
 dataset = TinyImageNet(Path("~/.torchvision/tinyimagenet/"),split=split)
 n = len(dataset)
@@ -38,7 +38,8 @@
 n_samples = 5
 print(f"Showing info of {n_samples} samples...")
 for i in range(0,n,n//n_samples):
     image,klass = dataset[i]
     print(f"Sample of class {klass:3d}, image {image}, words {dataset.idx_to_words[klass]}")
 ````
 
+You can also check the [quickstart notebook](https://colab.research.google.com/drive/1FCDsDJg86mCjyeAWOxDW9iF49goWCx4j?usp=sharing)
```

### Comparing `tinyimagenet-0.3/README.md` & `tinyimagenet-0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # torchvision-tinyimagenet
 Dataset class for PyTorch and the TinyImageNet dataset.
 
+# Installation
+
+``` pip install tinyimagenet ```
 
 # How to use
 ````
 from tinyimagenet import TinyImageNet
-import logging
 from pathlib import Path
 
 logging.basicConfig(level=logging.INFO)
 
 split ="val"
 dataset = TinyImageNet(Path("~/.torchvision/tinyimagenet/"),split=split)
 n = len(dataset)
 print(f"TinyImageNet, split {split}, has  {n} samples.")
 n_samples = 5
 print(f"Showing info of {n_samples} samples...")
 for i in range(0,n,n//n_samples):
     image,klass = dataset[i]
     print(f"Sample of class {klass:3d}, image {image}, words {dataset.idx_to_words[klass]}")
-````
+````
+
+You can also check the [quickstart notebook](https://colab.research.google.com/drive/1FCDsDJg86mCjyeAWOxDW9iF49goWCx4j?usp=sharing)
```

### Comparing `tinyimagenet-0.3/setup.py` & `tinyimagenet-0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 url="https://github.com/facundoq/tinyimagenet"
-VERSION="0.3"
+VERSION="0.4"
 
 class UploadCommand(Command):
     """Support setup.py upload."""
 
     description = 'Build and publish the package.'
     user_options = []
```

### Comparing `tinyimagenet-0.3/tinyimagenet.egg-info/PKG-INFO` & `tinyimagenet-0.4/tinyimagenet.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: tinyimagenet
-Version: 0.3
+Version: 0.4
 Summary: Dataset class for PyTorch and the TinyImageNet dataset, with automated download and extraction.
 Home-page: https://github.com/facundoq/tinyimagenet
 Author: Facundo Manuel Quiroga
 Author-email: facundoq@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/facundoq/tinyimagenet/issues
 Project-URL: Documentation, https://github.com/facundoq/tinyimagenet
 Project-URL: Source Code, https://github.com/facundoq/tinyimagenet
 Keywords: TinyImageNet ImageNet Dataset PyTorch torch torchvision
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # torchvision-tinyimagenet
 Dataset class for PyTorch and the TinyImageNet dataset.
 
+# Installation
+
+``` pip install tinyimagenet ```
 
 # How to use
 ````
 from tinyimagenet import TinyImageNet
-import logging
 from pathlib import Path
 
 logging.basicConfig(level=logging.INFO)
 
 split ="val"
 dataset = TinyImageNet(Path("~/.torchvision/tinyimagenet/"),split=split)
 n = len(dataset)
@@ -38,7 +38,8 @@
 n_samples = 5
 print(f"Showing info of {n_samples} samples...")
 for i in range(0,n,n//n_samples):
     image,klass = dataset[i]
     print(f"Sample of class {klass:3d}, image {image}, words {dataset.idx_to_words[klass]}")
 ````
 
+You can also check the [quickstart notebook](https://colab.research.google.com/drive/1FCDsDJg86mCjyeAWOxDW9iF49goWCx4j?usp=sharing)
```

### Comparing `tinyimagenet-0.3/tinyimagenet.py` & `tinyimagenet-0.4/tinyimagenet.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import List, Tuple
 from urllib.error import URLError
 
 from torchvision.datasets import ImageFolder
 from torchvision.datasets.utils import check_integrity, extract_archive, verify_str_arg,download_and_extract_archive
 import logging
 
-
+import imagenet1k
 
 mirrors = [
     "http://cs231n.stanford.edu/",
 ]
 
 resources = [
     ("tiny-imagenet-200.zip", "90528d7ca1a48142e341f4ef8d21d0de"),
@@ -102,14 +102,15 @@
 class TinyImageNet(ImageFolder):
     mean = [0.485, 0.456, 0.406]
     std = [0.229, 0.224, 0.225]
 
     def __init__(self, root: Path, split: str = "train",transform=None, target_transform=None) -> None:
         if isinstance(root,str):
             root = Path(root)
+        self.class_to_imagenet_idx = imagenet1k.class_to_idx 
         assert split in ["train","val","test"]
         root = root.expanduser()
         images_root = root/"tiny-imagenet-200/"
         if not images_root.exists():
             download_resources(root,mirrors,resources)        
         preprocess_val(images_root)
         super().__init__(images_root/split,transform=transform,target_transform=target_transform)
```

