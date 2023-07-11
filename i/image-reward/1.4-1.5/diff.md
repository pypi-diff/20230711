# Comparing `tmp/image-reward-1.4.tar.gz` & `tmp/image-reward-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image-reward-1.4.tar", last modified: Wed Jun 28 10:55:00 2023, max compression
+gzip compressed data, was "dist/image-reward-1.5.tar", last modified: Tue Jul 11 06:07:15 2023, max compression
```

## Comparing `image-reward-1.4.tar` & `image-reward-1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 10:55:00.000000 image-reward-1.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 10:55:00.000000 image-reward-1.4/ImageReward/
--rw-r--r--   0 root         (0) root         (0)     6969 2023-06-28 10:52:22.000000 image-reward-1.4/ImageReward/ImageReward.py
--rw-r--r--   0 root         (0) root         (0)    36541 2023-06-28 10:52:22.000000 image-reward-1.4/ImageReward/ReFL.py
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-28 10:52:22.000000 image-reward-1.4/ImageReward/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 10:55:00.000000 image-reward-1.4/ImageReward/models/
--rw-r--r--   0 root         (0) root         (0)     3167 2023-06-28 10:52:22.000000 image-reward-1.4/ImageReward/models/AestheticScore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 10:55:00.000000 image-reward-1.4/ImageReward/models/BLIP/
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-28 10:52:22.000000 image-reward-1.4/ImageReward/models/BLIP/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3125 2023-06-28 10:52:22.000000 image-reward-1.4/ImageReward/models/BLIP/blip.py
--rw-r--r--   0 root         (0) root         (0)     1502 2023-06-28 10:52:22.000000 image-reward-1.4/ImageReward/models/BLIP/blip_pretrain.py
--rw-r--r--   0 root         (0) root         (0)    41498 2023-06-28 10:52:23.000000 image-reward-1.4/ImageReward/models/BLIP/med.py
--rw-r--r--   0 root         (0) root         (0)    14061 2023-06-28 10:52:23.000000 image-reward-1.4/ImageReward/models/BLIP/vit.py
--rw-r--r--   0 root         (0) root         (0)     3840 2023-06-28 10:52:23.000000 image-reward-1.4/ImageReward/models/BLIPScore.py
--rw-r--r--   0 root         (0) root         (0)     2928 2023-06-28 10:52:23.000000 image-reward-1.4/ImageReward/models/CLIPScore.py
--rw-r--r--   0 root         (0) root         (0)       99 2023-06-28 10:52:23.000000 image-reward-1.4/ImageReward/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5923 2023-06-28 10:52:23.000000 image-reward-1.4/ImageReward/utils.py
--rw-r--r--   0 root         (0) root         (0)    11351 2023-06-28 10:52:23.000000 image-reward-1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11974 2023-06-28 10:55:00.000000 image-reward-1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11665 2023-06-28 10:52:23.000000 image-reward-1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 10:55:00.000000 image-reward-1.4/image_reward.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11974 2023-06-28 10:55:00.000000 image-reward-1.4/image_reward.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-28 10:55:00.000000 image-reward-1.4/image_reward.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-28 10:55:00.000000 image-reward-1.4/image_reward.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-28 10:55:00.000000 image-reward-1.4/image_reward.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-28 10:55:00.000000 image-reward-1.4/image_reward.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 10:55:00.000000 image-reward-1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1079 2023-06-28 10:53:55.000000 image-reward-1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 06:07:15.000000 image-reward-1.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 06:07:15.000000 image-reward-1.5/ImageReward/
+-rw-r--r--   0 root         (0) root         (0)     6969 2023-07-11 05:54:03.000000 image-reward-1.5/ImageReward/ImageReward.py
+-rw-r--r--   0 root         (0) root         (0)    36585 2023-07-11 05:55:09.000000 image-reward-1.5/ImageReward/ReFL.py
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-11 05:54:03.000000 image-reward-1.5/ImageReward/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 06:07:15.000000 image-reward-1.5/ImageReward/models/
+-rw-r--r--   0 root         (0) root         (0)     3167 2023-07-11 05:54:03.000000 image-reward-1.5/ImageReward/models/AestheticScore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 06:07:15.000000 image-reward-1.5/ImageReward/models/BLIP/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-11 05:54:03.000000 image-reward-1.5/ImageReward/models/BLIP/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-07-11 05:54:03.000000 image-reward-1.5/ImageReward/models/BLIP/blip.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2023-07-11 05:54:03.000000 image-reward-1.5/ImageReward/models/BLIP/blip_pretrain.py
+-rw-r--r--   0 root         (0) root         (0)    41498 2023-07-11 05:54:03.000000 image-reward-1.5/ImageReward/models/BLIP/med.py
+-rw-r--r--   0 root         (0) root         (0)    14061 2023-07-11 05:54:03.000000 image-reward-1.5/ImageReward/models/BLIP/vit.py
+-rw-r--r--   0 root         (0) root         (0)     3840 2023-07-11 05:54:03.000000 image-reward-1.5/ImageReward/models/BLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-07-11 05:54:03.000000 image-reward-1.5/ImageReward/models/CLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-07-11 05:54:03.000000 image-reward-1.5/ImageReward/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5923 2023-07-11 05:54:03.000000 image-reward-1.5/ImageReward/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11351 2023-07-11 05:54:03.000000 image-reward-1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11974 2023-07-11 06:07:15.000000 image-reward-1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11665 2023-07-11 05:54:03.000000 image-reward-1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 06:07:15.000000 image-reward-1.5/image_reward.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11974 2023-07-11 06:07:15.000000 image-reward-1.5/image_reward.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-11 06:07:15.000000 image-reward-1.5/image_reward.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-11 06:07:15.000000 image-reward-1.5/image_reward.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-11 06:07:15.000000 image-reward-1.5/image_reward.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-11 06:07:15.000000 image-reward-1.5/image_reward.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 06:07:15.000000 image-reward-1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-07-11 05:54:32.000000 image-reward-1.5/setup.py
```

### Comparing `image-reward-1.4/ImageReward/ImageReward.py` & `image-reward-1.5/ImageReward/ImageReward.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.4/ImageReward/ReFL.py` & `image-reward-1.5/ImageReward/ReFL.py`

 * *Files 1% similar despite different names*

```diff
@@ -724,21 +724,21 @@
                                 latent_model_input,
                                 t,
                                 encoder_hidden_states=encoder_hidden_states,
                             ).sample
                             latents = self.noise_scheduler.step(noise_pred, t, latents).prev_sample
                     
                     latent_model_input = latents
-                    latent_model_input = self.noise_scheduler.scale_model_input(latent_model_input, mid_timestep)
+                    latent_model_input = self.noise_scheduler.scale_model_input(latent_model_input, timesteps[mid_timestep])
                     noise_pred = self.unet(
                         latent_model_input,
-                        mid_timestep,
+                        timesteps[mid_timestep],
                         encoder_hidden_states=encoder_hidden_states,
                     ).sample
-                    pred_original_sample = self.noise_scheduler.step(noise_pred, t, latents).pred_original_sample.to(self.weight_dtype)
+                    pred_original_sample = self.noise_scheduler.step(noise_pred, timesteps[mid_timestep], latents).pred_original_sample.to(self.weight_dtype)
                     
                     pred_original_sample = 1 / self.vae.config.scaling_factor * pred_original_sample
                     image = self.vae.decode(pred_original_sample.to(self.weight_dtype)).sample
                     image = (image / 2 + 0.5).clamp(0, 1)
 
                     # image encode
                     def _transform():
```

### Comparing `image-reward-1.4/ImageReward/models/AestheticScore.py` & `image-reward-1.5/ImageReward/models/AestheticScore.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.4/ImageReward/models/BLIP/blip.py` & `image-reward-1.5/ImageReward/models/BLIP/blip.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.4/ImageReward/models/BLIP/blip_pretrain.py` & `image-reward-1.5/ImageReward/models/BLIP/blip_pretrain.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.4/ImageReward/models/BLIP/med.py` & `image-reward-1.5/ImageReward/models/BLIP/med.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.4/ImageReward/models/BLIP/vit.py` & `image-reward-1.5/ImageReward/models/BLIP/vit.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.4/ImageReward/models/BLIPScore.py` & `image-reward-1.5/ImageReward/models/BLIPScore.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.4/ImageReward/models/CLIPScore.py` & `image-reward-1.5/ImageReward/models/CLIPScore.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.4/ImageReward/utils.py` & `image-reward-1.5/ImageReward/utils.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.4/LICENSE` & `image-reward-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `image-reward-1.4/PKG-INFO` & `image-reward-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-reward
-Version: 1.4
+Version: 1.5
 Summary: ImageReward
 Home-page: https://github.com/THUDM/ImageReward
 Author: Jiazheng Xu, et al.
 Author-email: <xjz22@mails.tsinghua.edu.cn>
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: image-reward Version: 1.4 Summary: ImageReward
+Metadata-Version: 2.1 Name: image-reward Version: 1.5 Summary: ImageReward
 Home-page: https://github.com/THUDM/ImageReward Author: Jiazheng Xu, et al.
 Author-email:
 mails.tsinghua.edu.cn> License: Apache 2.0 license Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE # ImageReward
     ð¤ HF_Repo â¢ ð¦ Twitter â¢ ð Paper â¢ ð¼ Dataset â¢ ð
                                  ä¸­æåå®¢
 **ImageReward: Learning and Evaluating Human Preferences for Text-to-Image
```

### Comparing `image-reward-1.4/README.md` & `image-reward-1.5/README.md`

 * *Files identical despite different names*

### Comparing `image-reward-1.4/image_reward.egg-info/PKG-INFO` & `image-reward-1.5/image_reward.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-reward
-Version: 1.4
+Version: 1.5
 Summary: ImageReward
 Home-page: https://github.com/THUDM/ImageReward
 Author: Jiazheng Xu, et al.
 Author-email: <xjz22@mails.tsinghua.edu.cn>
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: image-reward Version: 1.4 Summary: ImageReward
+Metadata-Version: 2.1 Name: image-reward Version: 1.5 Summary: ImageReward
 Home-page: https://github.com/THUDM/ImageReward Author: Jiazheng Xu, et al.
 Author-email:
 mails.tsinghua.edu.cn> License: Apache 2.0 license Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE # ImageReward
     ð¤ HF_Repo â¢ ð¦ Twitter â¢ ð Paper â¢ ð¼ Dataset â¢ ð
                                  ä¸­æåå®¢
 **ImageReward: Learning and Evaluating Human Preferences for Text-to-Image
```

### Comparing `image-reward-1.4/image_reward.egg-info/SOURCES.txt` & `image-reward-1.5/image_reward.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image-reward-1.4/setup.py` & `image-reward-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (Path(__file__).parent / "README.md").read_text()
 DESCRIPTION = 'ImageReward'
 
 # 配置
 setup(
         name="image-reward", 
         py_modules = ["ImageReward"],
-        version="1.4",
+        version="1.5",
         author="Jiazheng Xu, et al.",
         author_email="<xjz22@mails.tsinghua.edu.cn>",
         url="https://github.com/THUDM/ImageReward",
         description=DESCRIPTION,
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=find_packages(exclude=["tests*"]),
```

