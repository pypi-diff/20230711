# Comparing `tmp/icatcher-0.1.0.tar.gz` & `tmp/icatcher-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icatcher-0.1.0.tar", last modified: Fri Jun 23 23:08:01 2023, max compression
+gzip compressed data, was "icatcher-0.1.1.tar", last modified: Tue Jul 11 09:27:11 2023, max compression
```

## Comparing `icatcher-0.1.0.tar` & `icatcher-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:08:01.980412 icatcher-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 23:05:42.000000 icatcher-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    47847 2023-06-23 23:08:01.980412 icatcher-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-06-23 23:05:42.000000 icatcher-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-23 23:05:42.000000 icatcher-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 23:08:01.980412 icatcher-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:08:01.976412 icatcher-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:08:01.976412 icatcher-0.1.0/src/icatcher/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23510 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/face_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-06-23 23:05:42.000000 icatcher-0.1.0/src/icatcher/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:08:01.980412 icatcher-0.1.0/src/icatcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47847 2023-06-23 23:08:01.000000 icatcher-0.1.0/src/icatcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-23 23:08:01.000000 icatcher-0.1.0/src/icatcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 23:08:01.000000 icatcher-0.1.0/src/icatcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 23:08:01.000000 icatcher-0.1.0/src/icatcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-23 23:08:01.000000 icatcher-0.1.0/src/icatcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 23:08:01.000000 icatcher-0.1.0/src/icatcher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:08:01.980412 icatcher-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-23 23:05:42.000000 icatcher-0.1.0/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-23 23:05:42.000000 icatcher-0.1.0/tests/test_face_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:27:11.581190 icatcher-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 09:24:49.000000 icatcher-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    47847 2023-07-11 09:27:11.581190 icatcher-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-11 09:24:49.000000 icatcher-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-11 09:24:49.000000 icatcher-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 09:27:11.581190 icatcher-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:27:11.577190 icatcher-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:27:11.577190 icatcher-0.1.1/src/icatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-11 09:24:49.000000 icatcher-0.1.1/src/icatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23220 2023-07-11 09:24:49.000000 icatcher-0.1.1/src/icatcher/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-11 09:24:49.000000 icatcher-0.1.1/src/icatcher/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-11 09:24:49.000000 icatcher-0.1.1/src/icatcher/face_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-07-11 09:24:49.000000 icatcher-0.1.1/src/icatcher/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-07-11 09:24:49.000000 icatcher-0.1.1/src/icatcher/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-11 09:24:49.000000 icatcher-0.1.1/src/icatcher/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-11 09:24:49.000000 icatcher-0.1.1/src/icatcher/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:27:11.581190 icatcher-0.1.1/src/icatcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47847 2023-07-11 09:27:11.000000 icatcher-0.1.1/src/icatcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-11 09:27:11.000000 icatcher-0.1.1/src/icatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 09:27:11.000000 icatcher-0.1.1/src/icatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-11 09:27:11.000000 icatcher-0.1.1/src/icatcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-11 09:27:11.000000 icatcher-0.1.1/src/icatcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 09:27:11.000000 icatcher-0.1.1/src/icatcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:27:11.581190 icatcher-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-11 09:24:49.000000 icatcher-0.1.1/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-07-11 09:24:49.000000 icatcher-0.1.1/tests/test_face_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-11 09:24:49.000000 icatcher-0.1.1/tests/test_gaze_model.py
```

### Comparing `icatcher-0.1.0/LICENSE` & `icatcher-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `icatcher-0.1.0/PKG-INFO` & `icatcher-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icatcher
-Version: 0.1.0
+Version: 0.1.1
 Summary: iCatcher+: Robust and automated annotation of infant gaze from videos collected in laboratory, field, and online studies.
 Author-email: Yotam Erel <erelyotam@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `icatcher-0.1.0/README.md` & `icatcher-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `icatcher-0.1.0/pyproject.toml` & `icatcher-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icatcher"
-version = "0.1.0"
+version = "0.1.1"
 description = "iCatcher+: Robust and automated annotation of infant gaze from videos collected in laboratory, field, and online studies."
 readme = "README.md"
 authors = [{ name = "Yotam Erel", email = "erelyotam@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -35,15 +35,15 @@
 build = ["bumpver", "build", "twine"]
 dev = ["pytest"]
 
 [project.urls]
 Homepage = "https://github.com/yoterel/icatcher_plus"
 
 [tool.bumpver]
-current_version = "0.1.0"
+current_version = "0.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `icatcher-0.1.0/src/icatcher/cli.py` & `icatcher-0.1.1/src/icatcher/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,35 +146,29 @@
     # zip_content_file = GOODBOY.fetch("zip_content.txt")
     # with open(zip_content_file, "r") as f:
         # zip_content = [x.strip() for x in f]
     file_paths = GOODBOY.fetch("icatcher+_models.zip",
                                processor=pooch.Unzip(),
                                progressbar=True)
     file_names = [Path(x).name for x in file_paths]
-    if opt.fd_model == "retinaface":  # option for retina face vs. previous opencv dnn model
+    if opt.fd_model == "retinaface":
         face_detector_model_file = file_paths[file_names.index("Resnet50_Final.pth")]
         face_detector_model = RetinaFace(
             gpu_id=opt.gpu_id, model_path=face_detector_model_file, network="resnet50"
         )
     elif opt.fd_model == "opencv_dnn":
         face_detector_model_file = file_paths[file_names.index("face_model.caffemodel")]
         config_file = file_paths[file_names.index("config.prototxt")]
         face_detector_model = cv2.dnn.readNetFromCaffe(str(config_file), str(face_detector_model_file))
     else:
         raise NotImplementedError
-    path_to_gaze_model = file_paths[file_names.index("icatcher+_lookit.pth")]
-    if opt.model:
-        path_to_gaze_model = opt.model
-    path_to_fc_model = file_paths[file_names.index("face_classifier_lookit.pth")]
-    if opt.fc_model:
-        path_to_fc_model = opt.fc_model
-    # face_detector_model_file = Path("models", "face_model.caffemodel")
-    # config_file = Path("models", "config.prototxt")
-    # path_to_gaze_model = opt.model
-    gaze_model = models.GazeCodingModel(opt).to(opt.device)
+    path_to_gaze_model = Path(file_paths[file_names.index(opt.model)])
+    is_regnet = "regnet" in str(path_to_gaze_model.stem)
+    path_to_fc_model = file_paths[file_names.index(opt.fc_model)]
+    gaze_model = models.GazeCodingModel(opt, is_regnet=is_regnet).to(opt.device)
     if opt.device == 'cpu':
         state_dict = torch.load(str(path_to_gaze_model), map_location=torch.device(opt.device))
     else:
         state_dict = torch.load(str(path_to_gaze_model))
     try:
         gaze_model.load_state_dict(state_dict)
     except RuntimeError as e:  # hack to deal with models trained on distributed setup
@@ -183,15 +177,15 @@
         for k, v in state_dict.items():
             name = k[7:]  # remove `module.`
             new_state_dict[name] = v
         # load params
         gaze_model.load_state_dict(new_state_dict)
     gaze_model.eval()
 
-    if opt.fc_model or opt.use_fc_model:
+    if opt.use_fc_model:
         face_classifier_model, fc_input_size = models.init_face_classifier(opt.device,
                                                                            num_classes=2,
                                                                            resume_from=path_to_fc_model)
         face_classifier_model.eval()
         face_classifier_model.to(opt.device)
         face_classifier_data_transforms = models.get_fc_data_transforms(fc_input_size)
     else:
@@ -353,15 +347,15 @@
                 bbox_sequence.pop(0)
                 from_tracker.pop(0)
                 if not image_sequence[opt.sliding_window_size // 2][1]:  # if middle image is valid
                     to_predict = {"imgs": torch.tensor(np.array([x[0] for x in image_sequence[0::2]]), dtype=torch.float).squeeze().permute(0, 3, 1, 2).to(opt.device),
                                     "boxs": torch.tensor(np.array(box_sequence[::2]), dtype=torch.float).to(opt.device)
                                     }
                     with torch.set_grad_enabled(False):
-                        outputs = gaze_model(to_predict)  # actual gaze prediction
+                        outputs = gaze_model(to_predict).detach()  # actual gaze prediction
                         probs = torch.nn.functional.softmax(outputs, dim=1)
                         _, prediction = torch.max(outputs, 1)
                         confidence, _ = torch.max(probs, 1)
                         float32_conf = confidence.cpu().numpy()[0]
                         int32_pred = prediction.cpu().numpy()[0]
                     answers[loc] = int32_pred  # update answers for the middle frame
                     confidences[loc] = float32_conf  # update confidences for the middle frame
```

### Comparing `icatcher-0.1.0/src/icatcher/draw.py` & `icatcher-0.1.1/src/icatcher/draw.py`

 * *Files identical despite different names*

### Comparing `icatcher-0.1.0/src/icatcher/face_detector.py` & `icatcher-0.1.1/src/icatcher/face_detector.py`

 * *Files identical despite different names*

### Comparing `icatcher-0.1.0/src/icatcher/models.py` & `icatcher-0.1.1/src/icatcher/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn.functional as F
 from torchvision.models.resnet import resnet18
-from torchvision.models import vgg16
+from torchvision.models import vgg16, regnet_y_16gf
 from torchvision import transforms
 
 
 def get_fc_data_transforms(input_size, dt_key=None):
     if dt_key is not None and dt_key != 'train':
         return {dt_key: transforms.Compose([
             transforms.ToTensor(),
@@ -99,20 +99,24 @@
         x = self.fc1(x)
         x = self.dropout(F.relu(self.bn(x)))
         x = self.fc2(x)
 
         return x
 
 class GazeCodingModel(torch.nn.Module):
-    def __init__(self, args, add_box=True):
+    def __init__(self, args, is_regnet=True, add_box=True):
         super().__init__()
         self.args = args
         self.n = (args.sliding_window_size + 1) // args.window_stride
         self.add_box = add_box
-        self.encoder_img = resnet18(num_classes=256).to(self.args.device)
+        if is_regnet:
+            # Use the RegNet network architecture
+            self.encoder_img = regnet_y_16gf(num_classes=256).to(self.args.device)
+        else:
+            self.encoder_img = resnet18(num_classes=256).to(self.args.device)
         self.encoder_box = Encoder_box().to(self.args.device)
         self.predictor = Predictor_fc(self.n, add_box).to(self.args.device)
 
     def forward(self, data):
         imgs = data['imgs']  # bs x n x 3 x 100 x 100
         boxs = data['boxs']  # bs x n x 5
         embedding = self.encoder_img(imgs.view(-1, 3, 100, 100)).view(-1, self.n, 256)
```

### Comparing `icatcher-0.1.0/src/icatcher/options.py` & `icatcher-0.1.1/src/icatcher/options.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,28 @@
     """
     parse command line arguments
     :param my_string: if provided, will parse this string instead of command line arguments
     :return: parsed arguments
     """
     parser = argparse.ArgumentParser(prog='icatcher')
     parser.add_argument("source", type=str, help="the source to use (path to video file, folder or webcam id)")
-    parser.add_argument("--model", type=str, help="path to model that will be used for predictions "
-                                                  "if not supplied will use model trained on the lookit dataset")
+    parser.add_argument("--model", type=str, default="icatcher+_lookit_regnet.pth", 
+                        choices=["icatcher+_lookit.pth",
+                                 "icatcher+_lookit_regnet.pth",
+                                 "icatcher+_bw-cali.pth",
+                                 "icatcher+_senegal.pth"],
+                        help="model file that will be used for gaze detection")
     parser.add_argument("--use_fc_model", action="store_true", help="if supplied, will use face classifier "
-                                                                              "to decide which crop to use from every frame.")
-    parser.add_argument("--fc_model", type=str, help="path to face classifier model that will be used for deciding "
-                                                     "which crop should we select from every frame. "
-                                                     "if not supplied but use_fc_model is true, will use the model trained on the lookit dataset.")
+                                                                    "to decide which crop to use from every frame.")
+    parser.add_argument("--fc_model", type=str, default="face_classifier_lookit.pth",
+                        choices=["face_classifier_lookit.pth",
+                                 "face_classifier_cali-bw.pth",
+                                  "face_classifier_senegal.pth"],
+                        help="face classifier model file that will be used for deciding "
+                                                     "which crop should we select from every frame. ")
     parser.add_argument("--source_type", type=str, default="file", choices=["file", "webcam"],
                         help="selects source of stream to use.")
     parser.add_argument("--crop_percent", type=int, default=0, help="A percent to crop video frames to prevent other people from appearing")
     parser.add_argument("--crop_mode", type=str, choices=["top", "left", "right"], nargs="+", default=["top"], help="where to crop video from, multi-choice.")
     parser.add_argument("--track_face", action="store_true", help="if detection is lost, will keep track of face using last known position.")
     parser.add_argument("--show_output", action="store_true", help="show results online in a separate window")
     parser.add_argument("--output_annotation", type=str, help="folder to output annotations to")
@@ -67,23 +74,19 @@
                         help="(cpu only) amount of frames to skip between each face detection. previous bbox will be used")
     parser.add_argument("--dont_buffer", action="store_true", default=False,
                         help="(cpu, retinaface only) frames will not be buffered, decreasing memory usage, but increasing processing time. Allows live stream of results.")
     if my_string is not None:
         args = parser.parse_args(my_string.split())
     else:
         args = parser.parse_args()
-    if args.model:
-        args.model = Path(args.model)
     if args.fd_confidence_threshold is None:  # set defaults outside argparse to avoid complication
         if args.fd_model == "retinaface":
             args.fd_confidence_threshold = 0.9
         elif args.fd_model == "opencv_dnn":
             args.fd_confidence_threshold = 0.7
-    # if not args.model.is_file():
-    #     raise FileNotFoundError("Model file not found")
     if args.crop_percent not in [x for x in range(100)]:
         raise ValueError("crop_video must be a percent between 0 - 99")
     if "left" in args.crop_mode and "right" in args.crop_mode:
         if args.crop_percent > 49:
             raise ValueError("crop_video must be a percent between 0 - 49 when cropping both sides")
     if args.video_filter:
         args.video_filter = Path(args.video_filter)
```

### Comparing `icatcher-0.1.0/src/icatcher/parsers.py` & `icatcher-0.1.1/src/icatcher/parsers.py`

 * *Files identical despite different names*

### Comparing `icatcher-0.1.0/src/icatcher/video.py` & `icatcher-0.1.1/src/icatcher/video.py`

 * *Files identical despite different names*

### Comparing `icatcher-0.1.0/src/icatcher.egg-info/PKG-INFO` & `icatcher-0.1.1/src/icatcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icatcher
-Version: 0.1.0
+Version: 0.1.1
 Summary: iCatcher+: Robust and automated annotation of infant gaze from videos collected in laboratory, field, and online studies.
 Author-email: Yotam Erel <erelyotam@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `icatcher-0.1.0/tests/test_basic.py` & `icatcher-0.1.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `icatcher-0.1.0/tests/test_face_detector.py` & `icatcher-0.1.1/tests/test_face_detector.py`

 * *Files identical despite different names*

