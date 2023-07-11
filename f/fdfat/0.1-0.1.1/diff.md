# Comparing `tmp/fdfat-0.1.tar.gz` & `tmp/fdfat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdfat-0.1.tar", last modified: Tue Jul 11 11:21:15 2023, max compression
+gzip compressed data, was "fdfat-0.1.1.tar", last modified: Tue Jul 11 13:34:53 2023, max compression
```

## Comparing `fdfat-0.1.tar` & `fdfat-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 11:21:15.488623 fdfat-0.1/
--rw-r--r--   0 ryan       (501) staff       (20)     2536 2023-07-11 11:21:15.488452 fdfat-0.1/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     1257 2023-07-07 04:23:18.000000 fdfat-0.1/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 11:21:15.480243 fdfat-0.1/fdfat/
--rw-r--r--   0 ryan       (501) staff       (20)      238 2023-07-05 04:46:00.000000 fdfat-0.1/fdfat/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 11:21:15.482095 fdfat-0.1/fdfat/cfg/
--rw-r--r--   0 ryan       (501) staff       (20)     4668 2023-07-11 11:08:58.000000 fdfat-0.1/fdfat/cfg/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1/fdfat/cfg/yaml_utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 11:21:15.482541 fdfat-0.1/fdfat/cli/
--rw-r--r--   0 ryan       (501) staff       (20)      433 2023-07-11 11:08:58.000000 fdfat-0.1/fdfat/cli/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 11:21:15.482902 fdfat-0.1/fdfat/data/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1/fdfat/data/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     4202 2023-07-11 11:08:58.000000 fdfat-0.1/fdfat/data/dataloader.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 11:21:15.484028 fdfat-0.1/fdfat/engine/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 07:53:43.000000 fdfat-0.1/fdfat/engine/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     1925 2023-07-11 11:08:58.000000 fdfat-0.1/fdfat/engine/tester.py
--rw-r--r--   0 ryan       (501) staff       (20)     2705 2023-07-11 11:08:58.000000 fdfat-0.1/fdfat/engine/trainer.py
--rw-r--r--   0 ryan       (501) staff       (20)     2116 2023-07-11 11:08:58.000000 fdfat-0.1/fdfat/engine/validator.py
--rw-r--r--   0 ryan       (501) staff       (20)     6121 2023-07-11 11:08:58.000000 fdfat-0.1/fdfat/main.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 11:21:15.484375 fdfat-0.1/fdfat/metric/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1/fdfat/metric/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-09 04:19:57.000000 fdfat-0.1/fdfat/metric/metric.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 11:21:15.486242 fdfat-0.1/fdfat/nn/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1/fdfat/nn/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     3643 2023-07-10 01:40:50.000000 fdfat-0.1/fdfat/nn/conv.py
--rw-r--r--   0 ryan       (501) staff       (20)     6047 2023-07-10 01:40:40.000000 fdfat-0.1/fdfat/nn/model.py
--rw-r--r--   0 ryan       (501) staff       (20)     4920 2023-07-09 05:55:54.000000 fdfat-0.1/fdfat/nn/module.py
--rw-r--r--   0 ryan       (501) staff       (20)     4925 2023-07-09 05:19:14.000000 fdfat-0.1/fdfat/nn/module2.py
--rw-r--r--   0 ryan       (501) staff       (20)     4925 2023-07-10 01:41:37.000000 fdfat-0.1/fdfat/nn/module3.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 11:21:15.487946 fdfat-0.1/fdfat/utils/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1/fdfat/utils/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     4016 2023-07-02 02:03:14.000000 fdfat-0.1/fdfat/utils/logger.py
--rw-r--r--   0 ryan       (501) staff       (20)     7031 2023-07-11 11:08:58.000000 fdfat-0.1/fdfat/utils/model_utils.py
--rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-07 05:05:30.000000 fdfat-0.1/fdfat/utils/pose_estimation.py
--rw-r--r--   0 ryan       (501) staff       (20)     4857 2023-07-10 09:42:57.000000 fdfat-0.1/fdfat/utils/utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 11:21:15.481646 fdfat-0.1/fdfat.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     2536 2023-07-11 11:21:15.000000 fdfat-0.1/fdfat.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      728 2023-07-11 11:21:15.000000 fdfat-0.1/fdfat.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-11 11:21:15.000000 fdfat-0.1/fdfat.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-11 11:21:15.000000 fdfat-0.1/fdfat.egg-info/entry_points.txt
--rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-11 11:21:15.000000 fdfat-0.1/fdfat.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-11 11:21:15.000000 fdfat-0.1/fdfat.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-11 11:21:15.488677 fdfat-0.1/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-11 11:16:04.000000 fdfat-0.1/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.985430 fdfat-0.1.1/
+-rw-r--r--   0 ryan       (501) staff       (20)     2625 2023-07-11 13:34:53.985297 fdfat-0.1.1/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     1344 2023-07-11 11:22:59.000000 fdfat-0.1.1/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.978545 fdfat-0.1.1/fdfat/
+-rw-r--r--   0 ryan       (501) staff       (20)      240 2023-07-11 13:34:26.000000 fdfat-0.1.1/fdfat/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.979502 fdfat-0.1.1/fdfat/cfg/
+-rw-r--r--   0 ryan       (501) staff       (20)     4678 2023-07-11 12:42:35.000000 fdfat-0.1.1/fdfat/cfg/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1.1/fdfat/cfg/yaml_utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.979864 fdfat-0.1.1/fdfat/cli/
+-rw-r--r--   0 ryan       (501) staff       (20)      433 2023-07-11 11:08:58.000000 fdfat-0.1.1/fdfat/cli/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.980306 fdfat-0.1.1/fdfat/data/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1.1/fdfat/data/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4202 2023-07-11 11:08:58.000000 fdfat-0.1.1/fdfat/data/dataloader.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.981238 fdfat-0.1.1/fdfat/engine/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 07:53:43.000000 fdfat-0.1.1/fdfat/engine/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1922 2023-07-11 13:22:27.000000 fdfat-0.1.1/fdfat/engine/tester.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2702 2023-07-11 13:22:27.000000 fdfat-0.1.1/fdfat/engine/trainer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2113 2023-07-11 13:22:27.000000 fdfat-0.1.1/fdfat/engine/validator.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6862 2023-07-11 13:34:19.000000 fdfat-0.1.1/fdfat/main.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.981601 fdfat-0.1.1/fdfat/metric/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1.1/fdfat/metric/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-09 04:19:57.000000 fdfat-0.1.1/fdfat/metric/metric.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.983549 fdfat-0.1.1/fdfat/nn/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1.1/fdfat/nn/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3643 2023-07-10 01:40:50.000000 fdfat-0.1.1/fdfat/nn/conv.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6047 2023-07-10 01:40:40.000000 fdfat-0.1.1/fdfat/nn/model.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4920 2023-07-09 05:55:54.000000 fdfat-0.1.1/fdfat/nn/module.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4925 2023-07-09 05:19:14.000000 fdfat-0.1.1/fdfat/nn/module2.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4925 2023-07-10 01:41:37.000000 fdfat-0.1.1/fdfat/nn/module3.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.984934 fdfat-0.1.1/fdfat/utils/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1.1/fdfat/utils/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4013 2023-07-11 13:22:27.000000 fdfat-0.1.1/fdfat/utils/logger.py
+-rw-r--r--   0 ryan       (501) staff       (20)     7031 2023-07-11 11:08:58.000000 fdfat-0.1.1/fdfat/utils/model_utils.py
+-rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-07 05:05:30.000000 fdfat-0.1.1/fdfat/utils/pose_estimation.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4857 2023-07-10 09:42:57.000000 fdfat-0.1.1/fdfat/utils/utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-11 13:34:53.979268 fdfat-0.1.1/fdfat.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     2625 2023-07-11 13:34:53.000000 fdfat-0.1.1/fdfat.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      728 2023-07-11 13:34:53.000000 fdfat-0.1.1/fdfat.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-11 13:34:53.000000 fdfat-0.1.1/fdfat.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-11 13:34:53.000000 fdfat-0.1.1/fdfat.egg-info/entry_points.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-11 13:34:53.000000 fdfat-0.1.1/fdfat.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-11 13:34:53.000000 fdfat-0.1.1/fdfat.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-11 13:34:53.985477 fdfat-0.1.1/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-11 11:16:04.000000 fdfat-0.1.1/setup.py
```

### Comparing `fdfat-0.1/PKG-INFO` & `fdfat-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdfat
-Version: 0.1
+Version: 0.1.1
 Summary: Fast 6DoF Face Alignment and Tracking
 Home-page: https://github.com/RyanDam/Fast-6DoF-Face-Alignment-and-Tracking
 Author: RyanDam
 License: GPL-3.0
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -24,14 +24,16 @@
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
+[![PyPI version](https://badge.fury.io/py/fdfat.svg)](https://badge.fury.io/py/fdfat)
+
 Working in progess...
 
 # Fast 6DoF Face Alignment and Tracking
 
 This project purpose is to implement Ultra lightweight 6 DoF Face Alignment and Tracking. This project is capable of realtime tracking face for mobile device.
 
 ## Installation
```

### Comparing `fdfat-0.1/README.md` & `fdfat-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![PyPI version](https://badge.fury.io/py/fdfat.svg)](https://badge.fury.io/py/fdfat)
+
 Working in progess...
 
 # Fast 6DoF Face Alignment and Tracking
 
 This project purpose is to implement Ultra lightweight 6 DoF Face Alignment and Tracking. This project is capable of realtime tracking face for mobile device.
 
 ## Installation
```

### Comparing `fdfat-0.1/fdfat/cfg/__init__.py` & `fdfat-0.1.1/fdfat/cfg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict, Union
 
 from fdfat.cfg.yaml_utils import yaml_load, yaml_save, yaml_print, DEFAULT_CFG_DICT, DEFAULT_CFG_DATA, IterableSimpleNamespace
 
 CFG_INT_KEYS= 'seed', 'workers', 'imgsz', 'epoch', 'batch_size', 'dump_batch', 'patience', 'warmup'
 CFG_FRACTION_KEYS = ('lr', 'lr0_factor', 'lr_factor', 'aux_pose_weight')
 CFG_FLOAT_KEYS = ("aug", 'muliplier', 'w_jaw', 'w_leyeb', 'w_reyeb', 'w_nose', 'w_nosetip', 'w_leye', 'w_reye', 'w_mount', 'w_purpil')
-CFG_BOOL_KEYS = ("save", "override", "pin_memory", "aux_pose", "lossw_enabled")
+CFG_BOOL_KEYS = ("save", "override", "pin_memory", "aux_pose", "lossw_enabled", "resume")
 
 def cfg2dict(cfg):
     """
     Convert a configuration object to a dictionary, whether it is a file path, a string, or a SimpleNamespace object.
 
     Inputs:
         cfg (str) or (Path) or (SimpleNamespace): Configuration object to be converted to a dictionary.
```

### Comparing `fdfat-0.1/fdfat/cfg/yaml_utils.py` & `fdfat-0.1.1/fdfat/cfg/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1/fdfat/data/dataloader.py` & `fdfat-0.1.1/fdfat/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1/fdfat/engine/tester.py` & `fdfat-0.1.1/fdfat/engine/tester.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tqdm
 import torch
 from collections import defaultdict
 
 from fdfat.utils.utils import LMK_PARTS, LMK_PART_NAMES, render_batch
-from landmark import TQDM_BAR_FORMAT
+from fdfat import TQDM_BAR_FORMAT
 from fdfat.metric.metric import nme
 
 def test_loop(cfgs, dataloader, model, loss_fn, name="Test"):
 
     loss_dict = defaultdict(lambda: 0)
 
     num_batches = len(dataloader)
```

### Comparing `fdfat-0.1/fdfat/engine/trainer.py` & `fdfat-0.1.1/fdfat/engine/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tqdm
 from collections import defaultdict
 
 import torch
 
 from fdfat.utils.utils import LMK_PARTS, LMK_PART_NAMES, render_batch
-from landmark import TQDM_BAR_FORMAT
+from fdfat import TQDM_BAR_FORMAT
 from fdfat.metric.metric import nme
 
 def train_loop(cfgs, current_epoch, dataloader, model, loss_fn, optimizer, name="Train"):
     loss_dict = defaultdict(lambda: 0)
 
     if cfgs.lossw_enabled:
         loss_weight = torch.zeros((cfgs.batch_size, 70))
```

### Comparing `fdfat-0.1/fdfat/engine/validator.py` & `fdfat-0.1.1/fdfat/engine/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tqdm
 import torch
 from collections import defaultdict
 
 from fdfat.utils.utils import LMK_PARTS, LMK_PART_NAMES, render_batch
-from landmark import TQDM_BAR_FORMAT
+from fdfat import TQDM_BAR_FORMAT
 from fdfat.metric.metric import nme
 
 def val_loop(cfgs, current_epoch, dataloader, model, loss_fn, name="Valid"):
     loss_dict = defaultdict(lambda: 0)
 
     num_batches = len(dataloader)
     pbar = tqdm.tqdm(enumerate(dataloader), total=num_batches, bar_format=TQDM_BAR_FORMAT)
```

### Comparing `fdfat-0.1/fdfat/main.py` & `fdfat-0.1.1/fdfat/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import time
 from pathlib import Path
 from types import SimpleNamespace
 from typing import Dict, Union
+from datetime import datetime, timedelta
+from copy import deepcopy
 import matplotlib
 matplotlib.use('Agg')
 
 import torch
 import torchvision
 torchvision.disable_beta_transforms_warning()
 from torch import nn
 from torch.utils.data import DataLoader
 from torch.optim.lr_scheduler import ConstantLR, SequentialLR, LinearLR, ReduceLROnPlateau
 
+from . import __version__
+
 from fdfat.nn import model
 from fdfat.utils.logger import LOGGER
 from fdfat.data.dataloader import LandmarkDataset
 from fdfat.utils.utils import LMK_PART_NAMES, increment_path, generate_graph, read_file_list
 from fdfat.utils.model_utils import init_seeds, select_device, model_info
 from fdfat.cfg import get_cfg, get_cfg_data, yaml_save, cfg2dict, yaml_print
 
@@ -68,17 +72,22 @@
                                     pose_rotation=cfgs.aux_pose, 
                                     aug=False)
     test_dataloader = DataLoader(dataset_test, batch_size=cfgs.batch_size, shuffle=False,
                                     pin_memory=cfgs.pin_memory,
                                     num_workers=cfgs.workers,
                                     persistent_workers=True,
                                     multiprocessing_context="spawn")
-
+    start_epoch = 0
     LOGGER.info(f"Load Model: {cfgs.model}")
     net = getattr(model, cfgs.model)(imgz=cfgs.imgsz, muliplier=cfgs.muliplier, pose_rotation=cfgs.aux_pose).to(cfgs.device)
+    # if cfgs.resume:
+    #     checkpoint = torch.load(save_best)
+    #     net.load_state_dict(checkpoint)
+    #     start_epoch = checkpoint['epoch']
+
     _ = model_info(net, detailed=True, imgsz=cfgs.imgsz, device=cfgs.device)
 
     loss_fn = getattr(nn, cfgs.loss)(reduction='none')
     if cfgs.optimizer == "SGD":
         optimizer = getattr(torch.optim, cfgs.optimizer)(net.parameters(), lr=cfgs.lr, momentum=0.95, nesterov=True)
     else:
         optimizer = getattr(torch.optim, cfgs.optimizer)(net.parameters(), lr=cfgs.lr)
@@ -87,20 +96,32 @@
     best_epoch_no = 0
     start_train_time = time.time()
 
     scheduler_warmup = ConstantLR(optimizer, factor=cfgs.lr0_factor, total_iters=cfgs.warmup)
     scheduler_main = LinearLR(optimizer, start_factor=1, end_factor=0.1, total_iters=cfgs.epoch-cfgs.warmup)
     scheduler = SequentialLR(optimizer, schedulers=[scheduler_warmup, scheduler_main], milestones=[cfgs.warmup])
 
+    # if not cfgs.resume:
     with open(save_log_csv, "a") as f:
         fields = '\t'.join(LMK_PART_NAMES)
         fields_test = '\t'.join([f"test_{a}" for a in LMK_PART_NAMES])
         f.write(f"epoch\ttotal\tnme\t{fields}\tpose\ttest_total\ttest_nme\t{fields_test}\ttest_pose\n")
 
-    for current_epoch in range(cfgs.epoch):
+    def save_model(epoch, save_path):
+        ckpt = {
+            'epoch': epoch,
+            'model': deepcopy(net).half(),
+            'optimizer': optimizer.state_dict(),
+            'train_args': cfgs,
+            'date': datetime.now().isoformat(),
+            'version': __version__
+        }
+        torch.save(ckpt, save_path)
+
+    for current_epoch in range(start_epoch, cfgs.epoch):
         LOGGER.info(f"\n\nEPOCH {current_epoch+1}, lr: {scheduler.get_last_lr()[0]:>7f}")
         
         train_loss_dict = train_loop(cfgs, current_epoch, train_dataloader, net, loss_fn, optimizer)
         test_loss_dict = val_loop(cfgs, current_epoch, test_dataloader, net, loss_fn)
         scheduler.step()
 
         with open(save_log_csv, "a") as f:
@@ -117,19 +138,21 @@
                 f.write(f"\t{test_loss_dict[n]}")
             f.write(f"\t{test_loss_dict['pose']}")
             
             f.write(f"\n")
 
         generate_graph(save_log_csv, save_log_png)
 
-        torch.save(net.state_dict(), save_last)
+        save_model(current_epoch, save_last)
+        # torch.save(net.state_dict(), save_last)
         if test_loss_dict["total"] < best_epoch_loss:
             best_epoch_loss = test_loss_dict["total"]
             best_epoch_no = current_epoch
-            torch.save(net.state_dict(), save_best)
+            # torch.save(net.state_dict(), save_best)
+            save_model(current_epoch, save_best)
             LOGGER.info(f"---> Saved best: epoch: {current_epoch+1}, loss: {best_epoch_loss:>7f}")
         else:
             if current_epoch - best_epoch_no > cfgs.patience:
                 LOGGER.info(f"STOPPED in {int(time.time() - start_train_time)}s, due to no improvement after {current_epoch - best_epoch_no} epochs, best epoch: {best_epoch_no}, val loss: {best_epoch_loss:>7f}")
                 break
             
     LOGGER.info(f"DONE in {int(time.time() - start_train_time)}s, best epoch: {best_epoch_no}, val loss: {best_epoch_loss:>7f}")
```

### Comparing `fdfat-0.1/fdfat/metric/metric.py` & `fdfat-0.1.1/fdfat/metric/metric.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1/fdfat/nn/conv.py` & `fdfat-0.1.1/fdfat/nn/conv.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1/fdfat/nn/model.py` & `fdfat-0.1.1/fdfat/nn/model.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1/fdfat/nn/module.py` & `fdfat-0.1.1/fdfat/nn/module.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1/fdfat/nn/module2.py` & `fdfat-0.1.1/fdfat/nn/module2.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1/fdfat/nn/module3.py` & `fdfat-0.1.1/fdfat/nn/module3.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1/fdfat/utils/logger.py` & `fdfat-0.1.1/fdfat/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import logging.config
 import pkg_resources as pkg
 
-from landmark import LOGGING_NAME, VERBOSE, MACOS, LINUX, WINDOWS
+from fdfat import LOGGING_NAME, VERBOSE, MACOS, LINUX, WINDOWS
 
 def check_version(current: str = '0.0.0',
                   minimum: str = '0.0.0',
                   name: str = 'version ',
                   pinned: bool = False,
                   hard: bool = False,
                   verbose: bool = False) -> bool:
```

### Comparing `fdfat-0.1/fdfat/utils/model_utils.py` & `fdfat-0.1.1/fdfat/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1/fdfat/utils/pose_estimation.py` & `fdfat-0.1.1/fdfat/utils/pose_estimation.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1/fdfat/utils/utils.py` & `fdfat-0.1.1/fdfat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1/fdfat.egg-info/PKG-INFO` & `fdfat-0.1.1/fdfat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdfat
-Version: 0.1
+Version: 0.1.1
 Summary: Fast 6DoF Face Alignment and Tracking
 Home-page: https://github.com/RyanDam/Fast-6DoF-Face-Alignment-and-Tracking
 Author: RyanDam
 License: GPL-3.0
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -24,14 +24,16 @@
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
+[![PyPI version](https://badge.fury.io/py/fdfat.svg)](https://badge.fury.io/py/fdfat)
+
 Working in progess...
 
 # Fast 6DoF Face Alignment and Tracking
 
 This project purpose is to implement Ultra lightweight 6 DoF Face Alignment and Tracking. This project is capable of realtime tracking face for mobile device.
 
 ## Installation
```

### Comparing `fdfat-0.1/fdfat.egg-info/SOURCES.txt` & `fdfat-0.1.1/fdfat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdfat-0.1/setup.py` & `fdfat-0.1.1/setup.py`

 * *Files identical despite different names*

