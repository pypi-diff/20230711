# Comparing `tmp/unibox-0.1.21.tar.gz` & `tmp/unibox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unibox-0.1.21.tar", max compression
+gzip compressed data, was "unibox-0.1.3.tar", max compression
```

## Comparing `unibox-0.1.21.tar` & `unibox-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-07-06 15:44:18.735710 unibox-0.1.21/LICENSE
--rw-r--r--   0        0        0      125 2023-07-06 15:44:18.735710 unibox-0.1.21/README.md
--rw-r--r--   0        0        0      426 2023-07-06 15:44:18.735710 unibox-0.1.21/pyproject.toml
--rw-r--r--   0        0        0       84 2023-07-06 15:44:18.735710 unibox-0.1.21/unibox/__init__.py
--rw-r--r--   0        0        0      672 2023-07-06 15:44:18.735710 unibox-0.1.21/unibox/cli.py
--rw-r--r--   0        0        0       21 2023-07-06 15:44:18.735710 unibox-0.1.21/unibox/setup/__init__.py
--rw-r--r--   0        0        0     1170 2023-07-06 15:44:18.735710 unibox-0.1.21/unibox/setup/setups.py
--rw-r--r--   0        0        0        0 2023-07-06 15:44:18.735710 unibox-0.1.21/unibox/uni_class/__init__.py
--rw-r--r--   0        0        0     2747 2023-07-06 15:44:18.735710 unibox-0.1.21/unibox/uni_class/data_loader.py
--rw-r--r--   0        0        0     3435 2023-07-06 15:44:18.735710 unibox-0.1.21/unibox/uni_class/logger.py
--rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 unibox-0.1.21/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-10 22:24:32.736801 unibox-0.1.3/LICENSE
+-rw-r--r--   0        0        0      125 2023-07-10 22:24:32.736801 unibox-0.1.3/README.md
+-rw-r--r--   0        0        0      442 2023-07-10 22:24:32.740802 unibox-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-07-10 22:24:32.740802 unibox-0.1.3/unibox/__init__.py
+-rw-r--r--   0        0        0     1317 2023-07-10 22:24:32.740802 unibox-0.1.3/unibox/cli.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:24:32.740802 unibox-0.1.3/unibox/processing/__init__.py
+-rw-r--r--   0        0        0     4852 2023-07-10 22:24:32.740802 unibox-0.1.3/unibox/processing/image_resizer.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:24:32.740802 unibox-0.1.3/unibox/utils/__init__.py
+-rw-r--r--   0        0        0     2743 2023-07-10 22:24:32.740802 unibox-0.1.3/unibox/utils/data_loader.py
+-rw-r--r--   0        0        0     3423 2023-07-10 22:24:32.740802 unibox-0.1.3/unibox/utils/logger.py
+-rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 unibox-0.1.3/PKG-INFO
```

### Comparing `unibox-0.1.21/LICENSE` & `unibox-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unibox-0.1.21/unibox/uni_class/data_loader.py` & `unibox-0.1.3/unibox/utils/data_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import tomli
 from omegaconf import OmegaConf
 from pathlib import Path
 from .logger import UniLogger
 
 
 class UniLoader:
-    """简单的loader uni_class, 用于原样加载json, txt, csv, image等数据;
+    """简单的loader utils, 用于原样加载json, txt, csv, image等数据;
     数据cleaning写在具体使用的class里
     """
 
     def __init__(self, logger=None):
         if not logger:
             self.logger = UniLogger(file_suffix="UniLoader")
         else:
```

### Comparing `unibox-0.1.21/unibox/uni_class/logger.py` & `unibox-0.1.3/unibox/utils/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import inspect
 from datetime import datetime
 
 NOTICE = 25  # Value between WARNING (30) and INFO (20)
 
 
 class UniLogger:
-    """包含时间和 caller frame的 logger uni_class
+    """包含时间和 caller frame的 logger utils
 
     VERSION: 2023.06.11 (JUNE)
 
     >>> logger = UniLogger("test", logger_name=__name__)
     >>> logger.info("test")
 
 
-    (Use in a uni_class:)
+    (Use in a utils:)
 
     if logger is not None:
         self.logger = logger
     else:
         logging.basicConfig(level=logging.INFO,
                             format='%(asctime)s [%(levelname)s] %(message)s',
                             datefmt='%Y-%m-%d %H:%M:%S')
@@ -72,15 +72,15 @@
     def log(self, log_level: str, message: str):
         level = getattr(logging, log_level.upper(), logging.INFO)
 
         # Get the caller function information
         caller_frame = inspect.currentframe().f_back.f_back  # Skip 'log' function frame
         caller_func_name = caller_frame.f_code.co_name
 
-        # Check if called from a uni_class
+        # Check if called from a utils
         if "self" in caller_frame.f_locals:
             caller_class_name = caller_frame.f_locals["self"].__class__.__name__
         else:
             caller_class_name = None
 
         # Include the caller function name in the message
         if caller_class_name:
```

### Comparing `unibox-0.1.21/PKG-INFO` & `unibox-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: unibox
-Version: 0.1.21
+Version: 0.1.3
 Summary: one toolbox to rule'em all
 License: GPL-3.0
 Author: yada
 Author-email: trojblue@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: click (>=8.1.4,<9.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # unibox
 
 unibox is a tool that aims to provide a unified interface for various common daily operations.
 
 ## Work in progress
```

