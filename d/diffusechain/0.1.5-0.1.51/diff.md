# Comparing `tmp/diffusechain-0.1.5.tar.gz` & `tmp/diffusechain-0.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffusechain-0.1.5.tar", max compression
+gzip compressed data, was "diffusechain-0.1.51.tar", max compression
```

## Comparing `diffusechain-0.1.5.tar` & `diffusechain-0.1.51.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      233 2023-07-09 12:50:06.797797 diffusechain-0.1.5/diffusechain/__init__.py
--rw-r--r--   0        0        0    15749 2023-07-09 13:15:20.723018 diffusechain-0.1.5/diffusechain/Automatic1111.py
--rw-r--r--   0        0        0        0 2023-07-09 12:48:39.750318 diffusechain-0.1.5/diffusechain/chains/__init__.py
--rw-r--r--   0        0        0       73 2023-07-09 12:53:17.902435 diffusechain-0.1.5/diffusechain/chains/consistentFaceChain.py
--rw-r--r--   0        0        0       63 2023-07-09 12:14:22.417256 diffusechain-0.1.5/diffusechain/Diffusers.py
--rw-r--r--   0        0        0      414 2023-07-09 13:18:58.459920 diffusechain-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       15 2023-07-06 19:14:58.750868 diffusechain-0.1.5/README.md
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 diffusechain-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      233 2023-07-09 12:50:06.797797 diffusechain-0.1.51/diffusechain/__init__.py
+-rw-r--r--   0        0        0    20316 2023-07-11 18:27:04.668791 diffusechain-0.1.51/diffusechain/Automatic1111.py
+-rw-r--r--   0        0        0        0 2023-07-09 12:48:39.750318 diffusechain-0.1.51/diffusechain/chains/__init__.py
+-rw-r--r--   0        0        0       73 2023-07-09 12:53:17.902435 diffusechain-0.1.51/diffusechain/chains/consistentFaceChain.py
+-rw-r--r--   0        0        0       63 2023-07-09 12:14:22.417256 diffusechain-0.1.51/diffusechain/Diffusers.py
+-rw-r--r--   0        0        0      415 2023-07-11 18:27:52.587045 diffusechain-0.1.51/pyproject.toml
+-rw-r--r--   0        0        0       15 2023-07-06 19:14:58.750868 diffusechain-0.1.51/README.md
+-rw-r--r--   0        0        0      584 1970-01-01 00:00:00.000000 diffusechain-0.1.51/PKG-INFO
```

### Comparing `diffusechain-0.1.5/diffusechain/Automatic1111.py` & `diffusechain-0.1.51/diffusechain/Automatic1111.py`

 * *Files 14% similar despite different names*

```diff
@@ -365,15 +365,138 @@
         import aiohttp
 
         async with aiohttp.ClientSession() as session:
             auth = aiohttp.BasicAuth(self.session.auth[0], self.session.auth[1]) if self.session.auth else None
             async with session.post(url, json=json, auth=auth) as response:
                 return await self._to_api_result_async(response)
 
-    
+    def img2img(
+        self,
+        images=[],  # list of PIL Image
+        resize_mode=0,
+        denoising_strength=0.75,
+        image_cfg_scale=1.5,
+        mask_image=None,  # PIL Image mask
+        mask_blur=4,
+        inpainting_fill=0,
+        inpaint_full_res=True,
+        inpaint_full_res_padding=0,
+        inpainting_mask_invert=0,
+        initial_noise_multiplier=1,
+        prompt="",
+        styles=[],
+        seed=-1,
+        subseed=-1,
+        subseed_strength=0,
+        seed_resize_from_h=0,
+        seed_resize_from_w=0,
+        sampler_name=None,  # use this instead of sampler_index
+        batch_size=1,
+        n_iter=1,
+        steps=None,
+        cfg_scale=7.0,
+        width=512,
+        height=512,
+        restore_faces=False,
+        tiling=False,
+        do_not_save_samples=False,
+        do_not_save_grid=False,
+        negative_prompt="",
+        eta=1.0,
+        s_churn=0,
+        s_tmax=0,
+        s_tmin=0,
+        s_noise=1,
+        override_settings={},
+        override_settings_restore_afterwards=True,
+        script_args=None,  # List of arguments for the script "script_name"
+        sampler_index=None,  # deprecated: use sampler_name
+        include_init_images=False,
+        script_name=None,
+        send_images=True,
+        save_images=False,
+        alwayson_scripts={},
+        controlnet_units: List[ControlNetUnit] = [],
+        use_deprecated_controlnet=False,
+        use_async=False,
+    ):
+        if sampler_name is None:
+            sampler_name = self.default_sampler
+        if sampler_index is None:
+            sampler_index = self.default_sampler
+        if steps is None:
+            steps = self.default_steps
+        if script_args is None:
+            script_args = []
+
+        payload = {
+            "init_images": [b64_img(x) for x in images],
+            "resize_mode": resize_mode,
+            "denoising_strength": denoising_strength,
+            "mask_blur": mask_blur,
+            "inpainting_fill": inpainting_fill,
+            "inpaint_full_res": inpaint_full_res,
+            "inpaint_full_res_padding": inpaint_full_res_padding,
+            "inpainting_mask_invert": inpainting_mask_invert,
+            "initial_noise_multiplier": initial_noise_multiplier,
+            "prompt": prompt,
+            "styles": styles,
+            "seed": seed,
+            "subseed": subseed,
+            "subseed_strength": subseed_strength,
+            "seed_resize_from_h": seed_resize_from_h,
+            "seed_resize_from_w": seed_resize_from_w,
+            "batch_size": batch_size,
+            "n_iter": n_iter,
+            "steps": steps,
+            "cfg_scale": cfg_scale,
+            "image_cfg_scale": image_cfg_scale,
+            "width": width,
+            "height": height,
+            "restore_faces": restore_faces,
+            "tiling": tiling,
+            "do_not_save_samples": do_not_save_samples,
+            "do_not_save_grid": do_not_save_grid,
+            "negative_prompt": negative_prompt,
+            "eta": eta,
+            "s_churn": s_churn,
+            "s_tmax": s_tmax,
+            "s_tmin": s_tmin,
+            "s_noise": s_noise,
+            "override_settings": override_settings,
+            "override_settings_restore_afterwards": override_settings_restore_afterwards,
+            "sampler_name": sampler_name,
+            "sampler_index": sampler_index,
+            "include_init_images": include_init_images,
+            "script_name": script_name,
+            "script_args": script_args,
+            "send_images": send_images,
+            "save_images": save_images,
+            "alwayson_scripts": alwayson_scripts,
+        }
+        if mask_image is not None:
+            payload["mask"] = b64_img(mask_image)
+
+        if use_deprecated_controlnet and controlnet_units and len(controlnet_units) > 0:
+            payload["controlnet_units"] = [x.to_dict() for x in controlnet_units]
+            return self.custom_post(
+                "controlnet/img2img", payload=payload, use_async=use_async
+            )
+
+        if controlnet_units and len(controlnet_units) > 0:
+            payload["alwayson_scripts"]["ControlNet"] = {
+                "args": [x.to_dict() for x in controlnet_units]
+            }
+        elif self.has_controlnet:
+            payload["alwayson_scripts"]["ControlNet"] = {"args": []}
+
+        return self.post_and_get_api_result(
+            f"{self.baseurl}/img2img", payload, use_async
+        )
+
 
     def extra_single_image(
         self,
         image,  # PIL Image
         resize_mode=0,
         show_extras_results=True,
         gfpgan_visibility=0,
@@ -465,8 +588,10 @@
     def png_info(self, image):
         payload = {
             "image": b64_img(image),
         }
 
         response = self.session.post(url=f"{self.baseurl}/png-info", json=payload)
         return self._to_api_result(response)
+    
+
```

### Comparing `diffusechain-0.1.5/PKG-INFO` & `diffusechain-0.1.51/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffusechain
-Version: 0.1.5
+Version: 0.1.51
 Summary: 
 Author: Adithya S K
 Author-email: adithyaskolavi@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

