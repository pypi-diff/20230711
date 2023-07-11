# Comparing `tmp/prodiapy-3.3.tar.gz` & `tmp/prodiapy-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodiapy-3.3.tar", last modified: Thu Jun 29 19:00:12 2023, max compression
+gzip compressed data, was "prodiapy-3.4.tar", last modified: Tue Jul 11 10:59:15 2023, max compression
```

## Comparing `prodiapy-3.3.tar` & `prodiapy-3.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 19:00:12.221973 prodiapy-3.3/
--rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodiapy-3.3/LICENSE
--rw-rw-rw-   0        0        0     1041 2023-06-29 19:00:12.220683 prodiapy-3.3/PKG-INFO
--rw-rw-rw-   0        0        0      824 2023-06-29 18:59:44.000000 prodiapy-3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 19:00:12.208530 prodiapy-3.3/prodia/
--rw-rw-rw-   0        0        0      155 2023-06-29 15:03:14.000000 prodiapy-3.3/prodia/__init__.py
--rw-rw-rw-   0        0        0    17337 2023-06-29 15:09:24.000000 prodiapy-3.3/prodia/async_prodia.py
--rw-rw-rw-   0        0        0     3809 2023-06-29 13:54:34.000000 prodiapy-3.3/prodia/constants.py
--rw-rw-rw-   0        0        0      340 2023-06-29 12:58:05.000000 prodiapy-3.3/prodia/exceptions.py
--rw-rw-rw-   0        0        0    17271 2023-06-29 15:10:51.000000 prodiapy-3.3/prodia/sync_prodia.py
--rw-rw-rw-   0        0        0     2645 2023-06-29 18:12:53.000000 prodiapy-3.3/prodia/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-29 19:00:12.220683 prodiapy-3.3/prodiapy.egg-info/
--rw-rw-rw-   0        0        0     1041 2023-06-29 19:00:12.000000 prodiapy-3.3/prodiapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-29 19:00:12.000000 prodiapy-3.3/prodiapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 19:00:12.000000 prodiapy-3.3/prodiapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-29 19:00:12.000000 prodiapy-3.3/prodiapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 19:00:12.000000 prodiapy-3.3/prodiapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 19:00:12.221973 prodiapy-3.3/setup.cfg
--rw-rw-rw-   0        0        0      414 2023-06-29 18:59:16.000000 prodiapy-3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:59:15.430193 prodiapy-3.4/
+-rw-rw-rw-   0        0        0    11558 2023-07-11 07:13:20.000000 prodiapy-3.4/LICENSE
+-rw-rw-rw-   0        0        0     1671 2023-07-11 10:59:15.429186 prodiapy-3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1454 2023-07-11 10:56:25.000000 prodiapy-3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 10:59:15.412528 prodiapy-3.4/prodia/
+-rw-rw-rw-   0        0        0      141 2023-07-11 10:54:17.000000 prodiapy-3.4/prodia/__init__.py
+-rw-rw-rw-   0        0        0    14642 2023-07-11 10:45:12.000000 prodiapy-3.4/prodia/async_prodia.py
+-rw-rw-rw-   0        0        0     3809 2023-07-11 09:19:46.000000 prodiapy-3.4/prodia/constants.py
+-rw-rw-rw-   0        0        0      340 2023-07-11 07:13:20.000000 prodiapy-3.4/prodia/exceptions.py
+-rw-rw-rw-   0        0        0    13150 2023-07-11 10:54:17.000000 prodiapy-3.4/prodia/sync_prodia.py
+-rw-rw-rw-   0        0        0      332 2023-07-11 09:31:48.000000 prodiapy-3.4/prodia/templates.py
+-rw-rw-rw-   0        0        0     2637 2023-07-11 09:34:16.000000 prodiapy-3.4/prodia/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:59:15.428170 prodiapy-3.4/prodiapy.egg-info/
+-rw-rw-rw-   0        0        0     1671 2023-07-11 10:59:15.000000 prodiapy-3.4/prodiapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-07-11 10:59:15.000000 prodiapy-3.4/prodiapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 10:59:15.000000 prodiapy-3.4/prodiapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-11 10:59:15.000000 prodiapy-3.4/prodiapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-11 10:59:15.000000 prodiapy-3.4/prodiapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 10:59:15.430193 prodiapy-3.4/setup.cfg
+-rw-rw-rw-   0        0        0      425 2023-07-11 10:54:17.000000 prodiapy-3.4/setup.py
```

### Comparing `prodiapy-3.3/LICENSE` & `prodiapy-3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prodiapy-3.3/prodia/async_prodia.py` & `prodiapy-3.4/prodia/async_prodia.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,131 +1,45 @@
 from .constants import *
 from .utils import *
 from .exceptions import *
-import requests
+from .templates import *
+import aiohttp
 import asyncio
-import json
+import time
 
 
 class AsyncClient:
-    def __init__(self, api_key: str = None):
+    def __init__(self, api_key: str = None, delay: int = 1):
         if api_key is None:
-            raise ClientError("\n\n\nNo API key provided, please get API key from https://app.prodia.com/ and try again\nExample of usage:\n\nclient = prodia.Client(api_key='xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx')")
+            raise ClientError(
+                "\n\n\nNo API key provided, please get API key from https://app.prodia.com/ and try again\nExample of usage:\n\nclient = prodia.Client(api_key='xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx')")
         self.key = api_key
         self.base = Endpoint.base
+        self.delay = delay
 
-    async def retrieve(self, job_id:str=None):
-        if job_id is None:
-            error("job_id is required!")
-            return
-        headers_retrieve = {
-            "accept": "application/json",
-            "X-Prodia-Key": self.key
-        }
-        response_retrieve = requests.get(self.base + f"/job/{job_id}", headers=headers_retrieve)
-        return response_retrieve.json()
-
-    async def create(self, endpoint, imageUrl:str=None, model:str=Model.REALISTICVS_V14.value[0], controlnet_model:str=Control.CANNY.value[0],
-                     prompt:str="Cats in clouds", denoising_strength:float=0.5, negative_prompt:str="badly drawn, blurry, low quality",
-                      steps:int=30, cfg_scale:float=9.5, seed:int=-1, upscale:bool=False, sampler:str="DDIM", aspect_ratio:str="square"):
-        warn("Validators are turned off in create() method")
-        if endpoint == "job":
-            payload = {
-                "prompt": prompt,
-                "model": model,
-                "sampler": sampler,
-                "negative_prompt": negative_prompt,
-                "steps": steps,
-                "cfg_scale": cfg_scale,
-                "seed": seed,
-                "upscale": upscale,
-                "aspect_ratio": aspect_ratio
-            }
-            headers_create = {
-                "accept": "application/json",
-                "content-type": "application/json",
-                "X-Prodia-Key": self.key
-            }
-            print(f"job created:\n{payload}")
-            response = requests.post(self.base + "/job", json=payload, headers=headers_create)
-            return response.json()
-        elif endpoint == "transform":
-            payload = {
-                "imageUrl": imageUrl,
-                "prompt": prompt,
-                "model": model,
-                "sampler": sampler,
-                "negative_prompt": negative_prompt,
-                "steps": steps,
-                "cfg_scale": cfg_scale,
-                "seed": seed,
-                "upscale": upscale,
-                "denoising_strength": denoising_strength
-            }
-            headers_create = {
-                "accept": "application/json",
-                "content-type": "application/json",
-                "X-Prodia-Key": self.key
-            }
-            print(f"job created:\n{payload}")
-            response = requests.post(self.base + "/transform", json=payload, headers=headers_create)
-            return response.json()
-        elif endpoint == "controlnet":
-            payload = {
-                "imageUrl": imageUrl,
-                "prompt": prompt,
-                "model": model,
-                "controlnet_model": controlnet_model,
-                "sampler": sampler,
-                "negative_prompt": negative_prompt,
-                "steps": steps,
-                "cfg_scale": cfg_scale,
-                "seed": seed,
-                "upscale": upscale,
-                "denoising_strength": denoising_strength
-            }
-            headers_create = {
-                "accept": "application/json",
-                "content-type": "application/json",
-                "X-Prodia-Key": self.key
-            }
-            print(f"job created:\n{payload}")
-            response = requests.post(self.base + "/controlnet", json=payload, headers=headers_create)
-            return response.json()
-
-
-
-    async def txt2img(self, model: Model = Model.REALISTICVS_V14, prompt:str=None, negative_prompt:str="badly drawn, blurry, low quality",
-                      steps:int=30, cfg_scale:float=9.5, seed:int=-1, upscale:bool=False, sampler: Sampler = Sampler.DDIM, aspect_ratio: Ratio = Ratio.SQUARE):
+    async def txt2img(self, model: str = Model.SD_V15.value[0], prompt: str = None,
+                      negative_prompt: str = "badly drawn, blurry, low quality",
+                      steps: int = 30, cfg_scale: float = 9.5, seed: int = -1, upscale: bool = False,
+                      sampler: str = "DDIM", aspect_ratio: str = "square"):
         if is_empty_or_whitespace(prompt):
             raise InvalidParameter("\n\n\nPrompt cannot be empty or whitespace")
         if validate_ratio(aspect_ratio):
-            raise InvalidParameter(f"\n\n\nEntered aspect_ratio isnt valid\nvalid ratios:\n['square', 'portrait', 'landscape'] or [Ratio.SQUARE, Ratio.PORTRAIT, 'Ratio.LANDSCAPE']\nYou provided: {aspect_ratio}")
+            raise InvalidParameter(
+                f"\n\n\nEntered aspect_ratio isnt valid\nvalid ratios:\n['square', 'portrait', 'landscape']\nYou provided: {aspect_ratio}")
         if validate_sampler(sampler):
-            warn(f"The sampler you used probably does not exist\nYour sampler: {sampler}\nAvailable: {[v.value[0] for v in Sampler]}")
+            warn(
+                f"The sampler you used probably does not exist\nYour sampler: {sampler}\nAvailable: {[v.value[0] for v in Sampler]}")
         if validate_model(model):
             warn(f"The model you used probably does not exist\nYour model: {model}")
         if validate_steps(steps):
-            raise InvalidParameter(f"\n\n\nSteps must be between 1 and 50\nYour value: {steps}")
+            raise InvalidParameter(f"\n\n\nsteps must be between 1 and 50\nYour value: {steps}")
         if validate_cfg(cfg_scale):
-            raise InvalidParameter(f"\n\n\nCFG scale must be between 1.0 and 20.0\nYour value: {steps}")
+            raise InvalidParameter(f"\n\n\ncfg_scale must be between 1.0 and 20.0\nYour value: {cfg_scale}")
         if "bool" not in str(type(upscale)):
-            raise InvalidParameter("\n\n\nUpscale value must be boolean:\nTrue, False")
-        try:
-            model = model.value[0]
-        except:
-            model = model
-        try:
-            sampler = sampler.value[0]
-        except:
-            sampler = sampler
-        try:
-            aspect_ratio = aspect_ratio.value[0]
-        except:
-            aspect_ratio = aspect_ratio
+            raise InvalidParameter("\n\n\nupscale value must be boolean:\nTrue, False")
         payload = {
             "prompt": prompt,
             "model": model,
             "sampler": sampler,
             "negative_prompt": negative_prompt,
             "steps": steps,
             "cfg_scale": cfg_scale,
@@ -138,82 +52,77 @@
             "content-type": "application/json",
             "X-Prodia-Key": self.key
         }
         headers_retrieve = {
             "accept": "application/json",
             "X-Prodia-Key": self.key
         }
-        print(f"txt2img with params:\n{payload}")
-        response = requests.post(self.base + "/job", json=payload, headers=headers_create)
-        try:
-            job_id = response.json()['job']
-        except Exception as e:
-            if response.text == "Invalid Generation Parameters":
-                raise InvalidParameter(f"\n\n\nProdia API raise Invalid Generation Parameters error, check payload for None or invalid parameters\n\nResponse:\n\n{response.text}")
-            else:
-                raise UnknownError(f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response.text}")
-        await asyncio.sleep(3)
-
-        working = True
-        while working is True:
-            response_retrieve = requests.get(self.base +f"/job/{job_id}", headers=headers_retrieve)
-            try:
-                status = response_retrieve.json()['status']
-            except Exception as e:
-                if response_retrieve.text == "Invalid Generation Parameters":
-                    raise InvalidParameter(
-                        f"\n\n\nProdia API raise Invalid Generation Parameters error, check payload for None or invalid parameters\n\nResponse:\n\n{response_retrieve.text}")
-                else:
-                    raise UnknownError(f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response_retrieve.text}")
-            if status == "succeeded":
-                print(f"Image {job_id} generated!")
-                image_url = response_retrieve.json()['imageUrl']
-                class prodia_response:
-                    url = image_url
-                    seed = get_seed(image_url)
-                    pnginfo = get_pnginfo(image_url)
-                return prodia_response
-            elif status == "queued":
-                print("Still working...")
-                await asyncio.sleep(2)
-            elif status == "generating":
-                print("Still working...")
-                await asyncio.sleep(2)
-            else:
-                failed(f"Generation of {job_id} failed or another error occurred: {status}")
-                return status
-    async def img2img(self, imageUrl:str=None, model: Model = Model.REALISTICVS_V14, prompt:str=None, negative_prompt:str="badly drawn, blurry, low quality",
-                      steps:int=30, denoising_strength:float=0.5, cfg_scale:float=9.5, seed:int=-1, upscale:bool=False, sampler: Sampler = Sampler.DDIM):
+        start_time = time.time()
+        print(f"txt2img with params: {payload}")
+
+        async with aiohttp.ClientSession() as session:
+            async with session.post(self.base+"/job", json=payload, headers=headers_create) as response:
+                try:
+                    response_json = await response.json()
+                    job_id = response_json['job']
+                except Exception as e:
+                    if response.status == 400:
+                        raise InvalidParameter(
+                            f"\n\n\nProdia API raised Invalid Generation Parameters error(400), check payload for None or invalid parameters\n\nResponse:\n\n{response.text}")
+                    else:
+                        raise UnknownError(
+                            f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response.text}")
+
+                await asyncio.sleep(self.delay)
+
+                while True:
+                    elapsed_time = time.time() - start_time
+                    print(f"txt2img time elapsed: {elapsed_time:.2f}", end="\r")
+                    async with session.get(self.base + f"/job/{job_id}", headers=headers_retrieve) as response_retrieve:
+                        try:
+                            response_retrieve_json = await response_retrieve.json()
+                            status = response_retrieve_json['status']
+                        except Exception as e:
+                            if response_retrieve.text == "Invalid Generation Parameters":
+                                raise InvalidParameter(
+                                    f"\n\n\nProdia API raise Invalid Generation Parameters error, check payload for None or invalid parameters\n\nResponse:\n\n{response_retrieve.text}")
+                            else:
+                                raise UnknownError(f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response_retrieve.text}")
+                        if status == "succeeded":
+                            print(f"\nImage {job_id} generated!")
+                            image_url = response_retrieve_json['imageUrl']
+                            return ProdiaResponse(image_url, payload, response_retrieve_json)
+                        elif status == "queued":
+                            await asyncio.sleep(self.delay)
+                        elif status == "generating":
+                            await asyncio.sleep(self.delay)
+                        else:
+                            failed(f"\nGeneration of {job_id} failed or another error occurred: {status}")
+                            return status
+    async def img2img(self, imageUrl:str=None, model: str = Model.SD_V15.value[0], prompt:str=None, negative_prompt:str="badly drawn, blurry, low quality",
+                      steps:int=30, denoising_strength:float=0.5, cfg_scale:float=9.5, seed:int=-1, upscale:bool=False, sampler: str = "DDIM"):
         if is_empty_or_whitespace(prompt):
             raise InvalidParameter("\n\n\nPrompt cannot be empty or whitespace")
         if imageUrl is None:
             error("imageUrl not specified")
             return
         if validate_sampler(sampler):
             warn(f"The sampler you used probably does not exist\nYour sampler: {sampler}\nAvailable: {[v.value[0] for v in Sampler]}")
         if validate_model(model):
             warn(f"The model you used probably does not exist\nYour model: {model}")
         if validate_steps(steps):
             raise InvalidParameter(f"\n\n\nSteps must be between 1 and 50\nYour value: {steps}")
         if validate_cfg(cfg_scale):
-            raise InvalidParameter(f"\n\n\nCFG scale must be between 1.0 and 20.0\nYour value: {steps}")
+            raise InvalidParameter(f"\n\n\nCFG scale must be between 1.0 and 20.0\nYour value: {cfg_scale}")
         if validate_denoise(denoising_strength):
-            raise InvalidParameter(f"\n\n\nCFG scale must be between 0.1 and 0.9\nYour value: {steps}")
+            raise InvalidParameter(f"\n\n\nDenoising Strength must be between 0.1 and 0.9\nYour value: {denoising_strength}")
         if "bool" not in str(type(upscale)):
             raise InvalidParameter("\n\n\nUpscale value must be boolean:\nTrue, False")
-        try:
-            model = model.value[0]
-        except:
-            model = model
-        try:
-            sampler = sampler.value[0]
-        except:
-            sampler = sampler
         payload = {
-            "imageUrl":imageUrl,
+            "imageUrl": imageUrl,
             "prompt": prompt,
             "model": model,
             "sampler": sampler,
             "negative_prompt": negative_prompt,
             "steps": steps,
             "cfg_scale": cfg_scale,
             "seed": seed,
@@ -225,53 +134,60 @@
             "content-type": "application/json",
             "X-Prodia-Key": self.key
         }
         headers_retrieve = {
             "accept": "application/json",
             "X-Prodia-Key": self.key
         }
+        start_time = time.time()
         print(f"img2img with params:\n{payload}")
-        response = requests.post(self.base + "/transform", json=payload, headers=headers_create)
-        try:
-            job_id = response.json()['job']
-        except Exception as e:
-            if response.text == "Invalid Generation Parameters":
-                raise InvalidParameter(f"\n\n\nProdia API raise Invalid Generation Parameters error, check payload for None or invalid parameters\n\nResponse:\n\n{response.text}")
-            else:
-                raise UnknownError(f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response.text}")
-        await asyncio.sleep(3)
-
-        working = True
-        while working is True:
-            response_retrieve = requests.get(self.base +f"/job/{job_id}", headers=headers_retrieve)
-            try:
-                status = response_retrieve.json()['status']
-            except Exception as e:
-                if response_retrieve.text == "Invalid Generation Parameters":
-                    raise InvalidParameter(
-                        f"\n\n\nProdia API raise Invalid Generation Parameters error, check payload for None or invalid parameters\n\nResponse:\n\n{response_retrieve.text}")
-                else:
-                    raise UnknownError(f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response_retrieve.text}")
-            if status == "succeeded":
-                print(f"Image {job_id} generated!")
-                image_url = response_retrieve.json()['imageUrl']
-                class prodia_response:
-                    url = image_url
-                    seed = get_seed(image_url)
-                    pnginfo = get_pnginfo(image_url)
-                return prodia_response
-            elif status == "queued":
-                print("Still working...")
-                await asyncio.sleep(2)
-            elif status == "generating":
-                print("Still working...")
-                await asyncio.sleep(2)
-            else:
-                failed(f"Generation of {job_id} failed or another error occurred: {status}")
-                return status
+
+        async with aiohttp.ClientSession() as session:
+            async with session.post(self.base+"/transform", json=payload, headers=headers_create) as response:
+                try:
+                    response_json = await response.json()
+                    job_id = response_json['job']
+                except Exception as e:
+                    if response.status == 400:
+                        raise InvalidParameter(
+                            f"\n\n\nProdia API raised Invalid Generation Parameters error(400), check payload for None or invalid parameters\n\nResponse:\n\n{response.text}")
+                    else:
+                        raise UnknownError(
+                            f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response.text}")
+
+                await asyncio.sleep(self.delay)
+
+                while True:
+                    elapsed_time = time.time() - start_time
+                    print(f"img2img time elapsed: {elapsed_time:.2f}", end="\r")
+                    async with session.get(self.base + f"/job/{job_id}", headers=headers_retrieve) as response_retrieve:
+                        try:
+                            response_retrieve_json = await response_retrieve.json()
+                            status = response_retrieve_json['status']
+                        except Exception as e:
+                            if response_retrieve.text == "Invalid Generation Parameters":
+                                raise InvalidParameter(
+                                    f"\n\n\nProdia API raise Invalid Generation Parameters error, check payload for None or invalid parameters\n\nResponse:\n\n{response_retrieve.text}")
+                            else:
+                                raise UnknownError(
+                                    f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response_retrieve.text}")
+                        if status == "succeeded":
+                            print(f"\nImage {job_id} generated!")
+                            image_url = response_retrieve_json['imageUrl']
+                            return ProdiaResponse(image_url, payload, response_retrieve_json)
+                        elif status == "queued":
+                            await asyncio.sleep(self.delay)
+                        elif status == "generating":
+                            await asyncio.sleep(self.delay)
+                        else:
+                            failed(f"\nGeneration of {job_id} failed or another error occurred: {status}")
+                            return status
+
+
+        ###DEPRECATED###
 
     async def controlnet(self, imageUrl:str=None, model: Model = Model.REALISTICVS_V14, controlnet_model: Control = Control.CANNY, prompt:str=None, negative_prompt:str="badly drawn, blurry, low quality",
                       steps:int=30, cfg_scale:float=9.5, seed:int=-1, sampler: Sampler = Sampler.DDIM):
         warn("THIS METHOD IS BETA AND UNSTABLE! USE IT AT YOUR OWN RISK")
         warn("Make sure that you used right url")
         if imageUrl is None:
             error("imageUrl not specified")
```

### Comparing `prodiapy-3.3/prodia/constants.py` & `prodiapy-3.4/prodia/constants.py`

 * *Files identical despite different names*

### Comparing `prodiapy-3.3/prodia/sync_prodia.py` & `prodiapy-3.4/prodia/sync_prodia.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,131 +1,37 @@
 from .constants import *
-from .utils import *
 from .exceptions import *
+from .templates import *
 import requests
 import time
-import json
 
-free_api_key = "89c5ea85-407c-4d57-b410-908f1a5e135c"
 class Client:
-    def __init__(self, api_key: str = None):
+    def __init__(self, api_key: str = None, delay:int=1):
         if api_key is None:
             raise ClientError("\n\n\nNo API key provided, please get API key from https://app.prodia.com/ and try again\nExample of usage:\n\nclient = prodia.Client(api_key='xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx')")
         self.key = api_key
         self.base = Endpoint.base
+        self.delay = delay
 
-    def retrieve(self, job_id:str=None):
-        if job_id is None:
-            error("job_id is required!")
-            return
-        headers_retrieve = {
-            "accept": "application/json",
-            "X-Prodia-Key": self.key
-        }
-        response_retrieve = requests.get(self.base + f"/job/{job_id}", headers=headers_retrieve)
-        return response_retrieve.json()
-
-    def create(self, endpoint, imageUrl:str=None, model:str=Model.REALISTICVS_V14.value[0], controlnet_model:str=Control.CANNY.value[0],
-                     prompt:str="Cats in clouds", denoising_strength:float=0.5, negative_prompt:str="badly drawn, blurry, low quality",
-                      steps:int=30, cfg_scale:float=9.5, seed:int=-1, upscale:bool=False, sampler:str="DDIM", aspect_ratio:str="square"):
-        warn("Validators are turned off in create() method")
-        if endpoint == "job":
-            payload = {
-                "prompt": prompt,
-                "model": model,
-                "sampler": sampler,
-                "negative_prompt": negative_prompt,
-                "steps": steps,
-                "cfg_scale": cfg_scale,
-                "seed": seed,
-                "upscale": upscale,
-                "aspect_ratio": aspect_ratio
-            }
-            headers_create = {
-                "accept": "application/json",
-                "content-type": "application/json",
-                "X-Prodia-Key": self.key
-            }
-            print(f"job created:\n{payload}")
-            response = requests.post(self.base + "/job", json=payload, headers=headers_create)
-            return response.json()
-        elif endpoint == "transform":
-            payload = {
-                "imageUrl": imageUrl,
-                "prompt": prompt,
-                "model": model,
-                "sampler": sampler,
-                "negative_prompt": negative_prompt,
-                "steps": steps,
-                "cfg_scale": cfg_scale,
-                "seed": seed,
-                "upscale": upscale,
-                "denoising_strength": denoising_strength
-            }
-            headers_create = {
-                "accept": "application/json",
-                "content-type": "application/json",
-                "X-Prodia-Key": self.key
-            }
-            print(f"job created:\n{payload}")
-            response = requests.post(self.base + "/transform", json=payload, headers=headers_create)
-            return response.json()
-        elif endpoint == "controlnet":
-            payload = {
-                "imageUrl": imageUrl,
-                "prompt": prompt,
-                "model": model,
-                "controlnet_model": controlnet_model,
-                "sampler": sampler,
-                "negative_prompt": negative_prompt,
-                "steps": steps,
-                "cfg_scale": cfg_scale,
-                "seed": seed,
-                "upscale": upscale,
-                "denoising_strength": denoising_strength
-            }
-            headers_create = {
-                "accept": "application/json",
-                "content-type": "application/json",
-                "X-Prodia-Key": self.key
-            }
-            print(f"job created:\n{payload}")
-            response = requests.post(self.base + "/controlnet", json=payload, headers=headers_create)
-            return response.json()
-
-
-
-    def txt2img(self, model: Model = Model.REALISTICVS_V14, prompt:str=None, negative_prompt:str="badly drawn, blurry, low quality",
-                      steps:int=30, cfg_scale:float=9.5, seed:int=-1, upscale:bool=False, sampler: Sampler = Sampler.DDIM, aspect_ratio: Ratio = Ratio.SQUARE):
+    def txt2img(self, model:str = Model.SD_V15.value[0], prompt:str=None, negative_prompt:str="badly drawn, blurry, low quality",
+                      steps:int=30, cfg_scale:float=9.5, seed:int=-1, upscale:bool=False, sampler:str = "DDIM", aspect_ratio:str = "square"):
         if is_empty_or_whitespace(prompt):
             raise InvalidParameter("\n\n\nPrompt cannot be empty or whitespace")
         if validate_ratio(aspect_ratio):
-            raise InvalidParameter(f"\n\n\nEntered aspect_ratio isnt valid\nvalid ratios:\n['square', 'portrait', 'landscape'] or [Ratio.SQUARE, Ratio.PORTRAIT, 'Ratio.LANDSCAPE']\nYou provided: {aspect_ratio}")
+            raise InvalidParameter(f"\n\n\nEntered aspect_ratio isnt valid\nvalid ratios:\n['square', 'portrait', 'landscape']\nYou provided: {aspect_ratio}")
         if validate_sampler(sampler):
             warn(f"The sampler you used probably does not exist\nYour sampler: {sampler}\nAvailable: {[v.value[0] for v in Sampler]}")
         if validate_model(model):
             warn(f"The model you used probably does not exist\nYour model: {model}")
         if validate_steps(steps):
-            raise InvalidParameter(f"\n\n\nSteps must be between 1 and 50\nYour value: {steps}")
+            raise InvalidParameter(f"\n\n\nsteps must be between 1 and 50\nYour value: {steps}")
         if validate_cfg(cfg_scale):
-            raise InvalidParameter(f"\n\n\nCFG scale must be between 1.0 and 20.0\nYour value: {steps}")
+            raise InvalidParameter(f"\n\n\ncfg_scale must be between 1.0 and 20.0\nYour value: {cfg_scale}")
         if "bool" not in str(type(upscale)):
-            raise InvalidParameter("\n\n\nUpscale value must be boolean:\nTrue, False")
-        try:
-            model = model.value[0]
-        except:
-            model = model
-        try:
-            sampler = sampler.value[0]
-        except:
-            sampler = sampler
-        try:
-            aspect_ratio = aspect_ratio.value[0]
-        except:
-            aspect_ratio = aspect_ratio
+            raise InvalidParameter("\n\n\nupscale value must be boolean:\nTrue, False")
         payload = {
             "prompt": prompt,
             "model": model,
             "sampler": sampler,
             "negative_prompt": negative_prompt,
             "steps": steps,
             "cfg_scale": cfg_scale,
@@ -138,80 +44,69 @@
             "content-type": "application/json",
             "X-Prodia-Key": self.key
         }
         headers_retrieve = {
             "accept": "application/json",
             "X-Prodia-Key": self.key
         }
-        print(f"txt2img with params:\n{payload}")
-        response = requests.post(self.base + "/job", json=payload, headers=headers_create)
+        start_time = time.time()
+        print(f"txt2img with params: {payload}")
+        response = requests.post(self.base+"/job", json=payload, headers=headers_create)
         try:
             job_id = response.json()['job']
         except Exception as e:
-            if response.text == "Invalid Generation Parameters":
-                raise InvalidParameter(f"\n\n\nProdia API raise Invalid Generation Parameters error, check payload for None or invalid parameters\n\nResponse:\n\n{response.text}")
+            if response.status_code == 400:
+                raise InvalidParameter(f"\n\n\nProdia API raised Invalid Generation Parameters error(400), check payload for None or invalid parameters\n\nResponse:\n\n{response.text}")
             else:
                 raise UnknownError(f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response.text}")
-        time.sleep(3)
 
-        working = True
-        while working is True:
-            response_retrieve = requests.get(self.base +f"/job/{job_id}", headers=headers_retrieve)
+        time.sleep(self.delay)
+
+        while True:
+            elapsed_time = time.time() - start_time
+            print(f"txt2img time elapsed: {elapsed_time:.2f}", end="\r")
+            response_retrieve = requests.get(self.base+f"/job/{job_id}", headers=headers_retrieve)
             try:
                 status = response_retrieve.json()['status']
             except Exception as e:
                 if response_retrieve.text == "Invalid Generation Parameters":
                     raise InvalidParameter(
                         f"\n\n\nProdia API raise Invalid Generation Parameters error, check payload for None or invalid parameters\n\nResponse:\n\n{response_retrieve.text}")
                 else:
                     raise UnknownError(f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response_retrieve.text}")
             if status == "succeeded":
-                print(f"Image {job_id} generated!")
+                print(f"\nImage {job_id} generated!")
                 image_url = response_retrieve.json()['imageUrl']
-                class prodia_response:
-                    url = image_url
-                    seed = get_seed(image_url)
-                    pnginfo = get_pnginfo(image_url)
-                return prodia_response
+                return ProdiaResponse(image_url, payload, response_retrieve.json())
             elif status == "queued":
-                print("Still working...")
-                time.sleep(2)
+                time.sleep(self.delay)
             elif status == "generating":
-                print("Still working...")
-                time.sleep(2)
+                time.sleep(self.delay)
             else:
-                failed(f"Generation of {job_id} failed or another error occurred: {status}")
+                failed(f"\nGeneration of {job_id} failed or another error occurred: {status}")
                 return status
-    def img2img(self, imageUrl:str=None, model: Model = Model.REALISTICVS_V14, prompt:str=None, negative_prompt:str="badly drawn, blurry, low quality",
-                      steps:int=30, denoising_strength:float=0.5, cfg_scale:float=9.5, seed:int=-1, upscale:bool=False, sampler: Sampler = Sampler.DDIM):
+    def img2img(self, imageUrl:str=None, model:str = Model.REALISTICVS_V14.value[0], prompt:str=None, negative_prompt:str="badly drawn, blurry, low quality",
+                      steps:int=30, denoising_strength:float=0.5, cfg_scale:float=9.5, seed:int=-1, upscale:bool=False, sampler:str = "DDIM"):
         if is_empty_or_whitespace(prompt):
             raise InvalidParameter("\n\n\nPrompt cannot be empty or whitespace")
         if imageUrl is None:
             error("imageUrl not specified")
             return
         if validate_sampler(sampler):
             warn(f"The sampler you used probably does not exist\nYour sampler: {sampler}\nAvailable: {[v.value[0] for v in Sampler]}")
         if validate_model(model):
             warn(f"The model you used probably does not exist\nYour model: {model}")
         if validate_steps(steps):
-            raise InvalidParameter(f"\n\n\nSteps must be between 1 and 50\nYour value: {steps}")
+            raise InvalidParameter(f"\n\n\nsteps must be between 1 and 50\nYour value: {steps}")
         if validate_cfg(cfg_scale):
-            raise InvalidParameter(f"\n\n\nCFG scale must be between 1.0 and 20.0\nYour value: {steps}")
+            raise InvalidParameter(f"\n\n\ncfg_scale must be between 1.0 and 20.0\nYour value: {steps}")
         if validate_denoise(denoising_strength):
-            raise InvalidParameter(f"\n\n\nCFG scale must be between 0.1 and 0.9\nYour value: {steps}")
+            raise InvalidParameter(f"\n\n\ndenoising_strength must be between 0.1 and 0.9\nYour value: {steps}")
         if "bool" not in str(type(upscale)):
-            raise InvalidParameter("\n\n\nUpscale value must be boolean:\nTrue, False")
-        try:
-            model = model.value[0]
-        except:
-            model = model
-        try:
-            sampler = sampler.value[0]
-        except:
-            sampler = sampler
+            raise InvalidParameter("\n\n\nupscale value must be boolean:\nTrue, False")
         payload = {
             "imageUrl":imageUrl,
             "prompt": prompt,
             "model": model,
             "sampler": sampler,
             "negative_prompt": negative_prompt,
             "steps": steps,
@@ -225,54 +120,55 @@
             "content-type": "application/json",
             "X-Prodia-Key": self.key
         }
         headers_retrieve = {
             "accept": "application/json",
             "X-Prodia-Key": self.key
         }
+        start_time = time.time()
         print(f"img2img with params:\n{payload}")
-        response = requests.post(self.base + "/transform", json=payload, headers=headers_create)
+        response = requests.post(self.base+"/transform", json=payload, headers=headers_create)
         try:
             job_id = response.json()['job']
         except Exception as e:
-            if response.text == "Invalid Generation Parameters":
+            if response.status_code == 400:
                 raise InvalidParameter(f"\n\n\nProdia API raise Invalid Generation Parameters error, check payload for None or invalid parameters\n\nResponse:\n\n{response.text}")
             else:
                 raise UnknownError(f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response.text}")
-        time.sleep(3)
 
-        working = True
-        while working is True:
+        time.sleep(self.delay)
+
+        while True:
+            elapsed_time = time.time() - start_time
+            print(f"txt2img time elapsed: {elapsed_time:.2f}", end="\r")
             response_retrieve = requests.get(self.base +f"/job/{job_id}", headers=headers_retrieve)
             try:
                 status = response_retrieve.json()['status']
             except Exception as e:
                 if response_retrieve.text == "Invalid Generation Parameters":
                     raise InvalidParameter(
                         f"\n\n\nProdia API raise Invalid Generation Parameters error, check payload for None or invalid parameters\n\nResponse:\n\n{response_retrieve.text}")
                 else:
                     raise UnknownError(f"\n\n\nProdia API returned unknown error: {e}\n\nResponse:\n\n{response_retrieve.text}")
             if status == "succeeded":
                 print(f"Image {job_id} generated!")
                 image_url = response_retrieve.json()['imageUrl']
-                class prodia_response:
-                    url = image_url
-                    seed = get_seed(image_url)
-                    pnginfo = get_pnginfo(image_url)
-                return prodia_response
+                return ProdiaResponse(image_url, payload, response_retrieve.json())
             elif status == "queued":
-                print("Still working...")
-                time.sleep(2)
+                time.sleep(self.delay)
             elif status == "generating":
                 print("Still working...")
-                time.sleep(2)
+                time.sleep(self.delay)
             else:
                 failed(f"Generation of {job_id} failed or another error occurred: {status}")
                 return status
 
+
+    ###DEPRECATED###
+
     def controlnet(self, imageUrl:str=None, model: Model = Model.REALISTICVS_V14, controlnet_model: Control = Control.CANNY, prompt:str=None, negative_prompt:str="badly drawn, blurry, low quality",
                       steps:int=30, cfg_scale:float=9.5, seed:int=-1, sampler: Sampler = Sampler.DDIM):
         warn("THIS METHOD IS BETA AND UNSTABLE! USE IT AT YOUR OWN RISK")
         warn("Make sure that you used right url")
         if imageUrl is None:
             error("imageUrl not specified")
             return
```

### Comparing `prodiapy-3.3/prodia/utils.py` & `prodiapy-3.4/prodia/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import re
 import requests
 from PIL import Image
 from io import BytesIO
 from colorama import Fore, init, Style
-from .constants import *
+from .constants import * #######
 
 def get_pnginfo(imageurl):
     response = requests.get(imageurl)
     targetImage = Image.open(BytesIO(response.content))
     try:
         metadata = targetImage.text
-        data = "\n".join([f"{key}: {value}" for key, value in metadata.items()])
+        data = {key: value for key, value in metadata.items()}
     except AttributeError:
         data = "Sorry, there is no pnginfo in this image"
     return data
 
 def get_seed(image_url):
     string = requests.get(image_url)
     pattern = r'Seed: (\d+)'
@@ -93,7 +93,8 @@
 def controlnet_models():
     for model in Control:
         print(f"{model.value[0]} - {model.value[1]} - {model.value[2]}")
 
 def samplers():
     for sampler in Sampler:
         print(f"{sampler.value[0]} - {sampler.value[1]}")
+
```

