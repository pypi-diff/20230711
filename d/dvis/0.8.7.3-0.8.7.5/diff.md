# Comparing `tmp/dvis-0.8.7.3-py3-none-any.whl.zip` & `tmp/dvis-0.8.7.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18348 bytes, number of entries: 11
+Zip file size: 18591 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx       35 b- defN 22-Aug-10 15:03 dvis/__init__.py
--rw-rw-r--  2.0 unx    38101 b- defN 23-Jan-02 11:02 dvis/dvis.py
+-rw-rw-r--  2.0 unx    38991 b- defN 23-Jul-11 09:52 dvis/dvis.py
 -rw-rw-r--  2.0 unx     1525 b- defN 23-Jan-04 10:29 dvis/dvis_cli.py
 -rw-rw-r--  2.0 unx     8263 b- defN 23-Jan-02 10:43 dvis/dvis_client.py
 -rw-rw-r--  2.0 unx     6060 b- defN 22-Aug-10 15:03 dvis/dvis_client_old.py
--rw-rw-r--  2.0 unx     5519 b- defN 23-Feb-23 09:32 dvis/utils.py
--rw-rw-r--  2.0 unx     4228 b- defN 23-Apr-19 14:34 dvis-0.8.7.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 14:34 dvis-0.8.7.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-19 14:34 dvis-0.8.7.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        5 b- defN 23-Apr-19 14:34 dvis-0.8.7.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      827 b- defN 23-Apr-19 14:34 dvis-0.8.7.3.dist-info/RECORD
-11 files, 64747 bytes uncompressed, 16966 bytes compressed:  73.8%
+-rw-rw-r--  2.0 unx     5510 b- defN 23-Jul-11 09:52 dvis/utils.py
+-rw-rw-r--  2.0 unx     4228 b- defN 23-Jul-11 09:52 dvis-0.8.7.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 09:52 dvis-0.8.7.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 09:52 dvis-0.8.7.5.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-11 09:52 dvis-0.8.7.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      827 b- defN 23-Jul-11 09:52 dvis-0.8.7.5.dist-info/RECORD
+11 files, 65628 bytes uncompressed, 17209 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: dvis/dvis_client_old.py
 Comment: 
 
 Filename: dvis/utils.py
 Comment: 
 
-Filename: dvis-0.8.7.3.dist-info/METADATA
+Filename: dvis-0.8.7.5.dist-info/METADATA
 Comment: 
 
-Filename: dvis-0.8.7.3.dist-info/WHEEL
+Filename: dvis-0.8.7.5.dist-info/WHEEL
 Comment: 
 
-Filename: dvis-0.8.7.3.dist-info/entry_points.txt
+Filename: dvis-0.8.7.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: dvis-0.8.7.3.dist-info/top_level.txt
+Filename: dvis-0.8.7.5.dist-info/top_level.txt
 Comment: 
 
-Filename: dvis-0.8.7.3.dist-info/RECORD
+Filename: dvis-0.8.7.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dvis/dvis.py

```diff
@@ -2,15 +2,22 @@
 Client side bridge to send various type of 2D and 3D to the server.
 
 Note:
     Requires DVIS server to run - sends data via websocket to localhost:5001 (3D visualizations) and localhost:4999 (using visdom for 2D visualization).
 """
 import shutil
 import numpy as np
-import torch
+try:
+    import torch.Tensor, torch.float, torch.double
+except:
+    class Dummy():
+        Tensor = None
+        float = None
+        double = None
+    torch = Dummy()
 from .dvis_client_old import (
     sendMesh2server,
     send_clear,
     send_config,
     sendTrack2server,
     send_camera,
     sendCmd2server,
@@ -80,15 +87,15 @@
         else:
             ref_color = get_color(c, cm) if c > 0 else 1
             return (
                 np.concatenate([data_np[:, :3], ref_color * np.stack((data_np[:, 3], data_np[:, 3], data_np[:, 3]), -1)], 1),
                 "xyzrgb",
             )
     elif fmt == "xyzrgb":
-        if np.any(data_np[:, 3:6] > 1) and np.all(data_np[:, 3:6] == data_np[:, 3:6].astype(np.int)):
+        if np.any(data_np[:, 3:6] > 1) and np.all(data_np[:, 3:6] == data_np[:, 3:6].astype(int)):
             ## color as uint 8
             data_np[:, 3:6] /= 255
             return data_np, fmt
         else:
             return data_np, fmt
     elif fmt == "xyz" or fmt == "bbox" or fmt == "corners" or fmt == "line" or fmt == "hbboxes" or fmt == "hbboxes_c":
         return data_np, fmt
@@ -100,15 +107,15 @@
             return fmtted, fmt
         return data_np, fmt
     elif fmt == "uv" or fmt == "uvrgb":
         if bounds is None:
             bounds = np.min(data_np[:, :2], 0), np.max(data_np[:, :2], 0)
         if len(bounds) == 2:
             if isinstance(bounds[0], (int, float)):
-                bounds = np.zeros(2, dtype=np.int), np.array(bounds)
+                bounds = np.zeros(2, dtype=int), np.array(bounds)
             elif isinstance(bounds[0], (tuple, list)):
                 bounds = np.array(bounds[0]), np.array(bounds[1])
         img = np.zeros((*(bounds[1] - bounds[0]), 3))
         valid_pixel = np.all(data_np[:, :2] >= bounds[0], 1) & np.all(data_np[:, :2] < bounds[1], 1)
         if data_np.shape[1] == 2:
 
             img[tuple((data_np[valid_pixel, :2] - bounds[0]).astype(int).T)] = 255
@@ -365,16 +372,28 @@
         name=name,
         meta_data=meta,
         compression="pkl",
         vis_conf=vis_conf,
         shape=shape,
     )
 
+def _image_size(img, s, is_bool=False):
+    if s!=1:
+        if isinstance(s, (int,float)):
+            if s < 10:
+                # rescaling
+                new_size = (int(img.height*s), int(img.width*s))
+            else:
+                new_size = (s, int(img.width/img.height*s))
+        else:
+            new_size = (int(s[0]), int(s[1]))
+        img = img.resize((new_size[1], new_size[0]), Image.Resampling.NEAREST if is_bool else Image.Resampling.LANCZOS)
+    return img
 
-def dvis_img(data, vs=1, c=0, l=[0], t=None, name=None, meta=None, vis_conf=None, cm='default', fmt='img', mi=None, ma=None):
+def dvis_img(data, vs=1, c=0, l=[0], t=None, name=None, meta=None, vis_conf=None, cm='default', fmt='img', mi=None, ma=None, s=1):
     if isinstance(data, (ImageFile.ImageFile)):
         data = np.array(data)
     if isinstance(data, str):
         fn = data
         if data.endswith(".gif"):
             # load image as base64 for visdom
             data = open(data, "rb").read()
@@ -384,58 +403,68 @@
             )
             return
         else:
             if ":" in fn:
                 # remote path
                 from fabric import Connection
                 hostname, remote_path, suffix = fn.split(":")[0], fn.split(":")[1], fn.split('.')[-1]
-                fn =f"tmp.{suffix}" 
+                fn =f"tmp.{suffix}"
                 Connection(hostname).get(remote_path,fn)
-                data = np.array(Image.open(fn))
+                img = Image.open(fn)
+                data = np.array(_image_size(img))
                 os.remove(fn)
             else:
-                data = np.array(Image.open(fn))
+                img = Image.open(fn)
+                data = np.array(_image_size(img))
         if meta is None:
             meta = {}
         meta["obj_path"] = fn
     try:
         if isinstance(data, matplotlib.axes.Axes):
             data = data.figure
         if isinstance(data, matplotlib.figure.Figure):
             data = np.array(matplot2PIL(data))
     except:
         pass
+    is_bool = data.dtype == bool
     data = convert_to_nd(data)
     sub_format = None
     if len(data.shape) == 3 and data.shape[0] in [3,4]:  # C,W,H
         data = np.transpose(data, [1, 2, 0])
     if fmt == 'xyl':
         # label image
-        data = visualize_label(data, cm=cm) 
+        data = visualize_label(data, cm=cm)
         sub_format = 'xyl'
     elif fmt == 'xyr':
-        # range image with 
+        # range image with
         # remap default to jet
         data = visualize_range(data, cm=("jet" if cm=='default' else cm), mi=mi, ma=ma)
         sub_format = 'xyr'
-            
+
     if data.max() <= 255:
         if (data.min() >= -1) and (data.min() < 0) and data.max() <= 1:
             data = data * 0.5 + 0.5
         if data.max() <= 1:
             data = data * 255
         data = data.astype(np.uint8)
     else:
         raise IOError("Image values cannot be interpreted")
     if data.shape[-1] == 4:
         #rgba
         data = data/255
         alpha_mask = data[...,3:]
         data[...,:3] = data[...,:3] * alpha_mask + (1.0 - c) * (1-alpha_mask)
         data = (data[...,:3]*255).astype(np.uint8)
+    if s!=1:
+        img = Image.fromarray(data)
+        img = _image_size(img,s, is_bool=is_bool)
+        data = np.array(img)
+        if is_bool:
+            data = data.astype(np.uint8)
+
     send2server(data=data, data_format="img", size=vs, color=c, layers=l, t=t, name=name, meta_data=meta, vis_conf=vis_conf, sub_format=sub_format)
 
 
 def dvis_group(name, meta):
     send2server(None, "group", vs=1, c=1, t=0, l=[0], add=False, name=name, meta=meta)
 
 
@@ -467,15 +496,15 @@
                     fmt = "xyzrgb"
             elif data.shape[1] == 7:
                 fmt = "xyzrgba"
             elif data.shape[1] == 3:
                 # xyz
                 fmt = "xyz"
             elif data.shape[1] == 4:
-                if np.abs(data[:,3].astype(np.int) -  data[:,3]).max()<1e-3:
+                if np.abs(data[:,3].astype(int) -  data[:,3]).max()<1e-3:
                     # xyzl
                     fmt = "xyzl"
                 else:
                     # xyzr
                     fmt = "xyzr"
         else:
             raise IOError(f"Points format {data.shape} not understood")
@@ -485,15 +514,15 @@
         data, fmt = np.concatenate([data[:, :3],label_colors], 1), "xyzrgb"
 
     if fmt == "xyzr":
         range_colors = visualize_range(data[:,3],cm=cm if cm is not None else "jet")[:,0]
         data, fmt = np.concatenate([data[:, :3],range_colors, data[:,3:4]], 1), "xyzrgba"
 
     if fmt in ["xyzrgb", "xyzrgba"]:
-        if np.any(data[:, 3:6] > 1) and np.all(data[:, 3:6] == data[:, 3:6].astype(np.int)):
+        if np.any(data[:, 3:6] > 1) and np.all(data[:, 3:6] == data[:, 3:6].astype(int)):
             ## color as uint 8
             data = data.astype(np.float32)
             data[:, 3:6] /= 255
 
     ## downsample
     if ms is not None and len(data) > ms:
         data = data[np.random.choice(len(data), ms, replace=False)]
@@ -754,24 +783,24 @@
     if len(data.shape)==3 or data.shape[-1] == 1:
         sub_format = _resolve_sub_type(data)
         # range or label sequence
         if sub_format == 'xyl':
             # label image
             data = np.stack(visualize_label(data[i], cm=cm) for i in range(data.shape[0]))
         elif sub_format == 'xyr':
-            # range image with 
+            # range image with
             # remap default to jet
             data = np.stack(visualize_range(data[i], cm=("jet" if cm=='default' else cm), mi=mi, ma=ma) for i in range(data.shape[0]))
     if data.shape[-1] in [3,4]: # T H W C
         data = data.transpose(0,3,1,2)
     if name is None:
         import time
         # unique name
         name = str(time.time())
-            
+
     if data.max() <= 255:
         if (data.min() >= -1) and (data.min() < 0) and data.max() <= 1:
             data = data * 0.5 + 0.5
         if data.max() <= 1:
             data = data * 255
         data = data.astype(np.uint8)
     else:
@@ -782,15 +811,15 @@
         #rgba
         data = data.transpose(0,2,3,1)
         data = data/255
         alpha_mask = data[...,3:]
         data[...,:3] = data[...,:3] * alpha_mask + (1.0 - c) * (1-alpha_mask)
         data = (data[...,:3]*255).astype(np.uint8)
         data = data.transpose(0,3,1,2)
-        
+
     send2server(data=data, data_format="seq", size=vs, color=c, layers=l, t=t, name=name, meta_data=meta, vis_conf=vis_conf, sub_format=sub_format)
 
 
 
 def _infer_format(data):
     if isinstance(data, (trimesh.Trimesh, trimesh.Scene)):
         fmt = "mesh"
@@ -895,15 +924,15 @@
             # range type
             return 'xyr'
         else:
             # label type
             return 'xyl'
     else:
         raise IOError("Unknown instance type")
-    return 
+    return
 
 def dvis_cam(data, name="RenderCam"):
     """Adds a new camera
     Args:
         data (dict): camera description as intrinsics or fov
         name (str): camera name
 
@@ -993,19 +1022,19 @@
         ma (float): Maximum bin
         layout (dict): Layout for plolty (https://plotly.com/python/reference/layout)
     """
 
     data = convert_to_nd(data)
 
     converted_layout = _convert_to_plotly_layout(name=name,c=c)
-    
+
     if layout is None:
         layout = dict()
     layout.update(converted_layout)
-    
+
     data_payload = {
         "type": "histogram",
         "x" : data.flatten().tolist(),
         "nbinsx": nbins,
     }
     xbins={}
     if mi is not None:
@@ -1123,15 +1152,15 @@
     elif fmt in ["config", "conf", "cfg"]:
         dvis_cfg(data)
     elif fmt == "mesh_pc":
         dvis_mesh_pc(data, vs, c, l, t, name, meta, ms, vis_conf, shape)
     elif fmt == "group":
         dvis_group(name, meta)
     elif fmt in ["img", 'xyl', 'xyr']:
-        dvis_img(data, vs, c, l, t, name, meta, vis_conf, fmt=fmt, cm=kwargs.get("cm",'default'), mi=kwargs.get('mi'), ma=kwargs.get('ma'))
+        dvis_img(data, vs, c, l, t, name, meta, vis_conf, fmt=fmt, cm=kwargs.get("cm",'default'), mi=kwargs.get('mi'), ma=kwargs.get('ma'), s=s)
     elif fmt == "hist":
         dvis_histogram(data, nbins=kwargs.get('nbins'), mi=kwargs.get('mi'), ma=kwargs.get('ma'), layout=kwargs.get("layout"), name=name, c=c)
     else:
         print("Format unknown")
     """
     if new is not None:
         if isinstance(new, bool):
```

## dvis/utils.py

```diff
@@ -2,15 +2,15 @@
 import cv2
 
 
 def rgb2hex(rgb):
     if rgb.max()<1:
         return '#%02x%02x%02x' % tuple(x for x in (255*rgb).astype(np.uint8))
     return '#%02x%02x%02x' %  tuple(x for x in rgb)
-    
+
 
 def str2cmap(cm: str):
     return cv2.__dict__[f"COLORMAP_{cm.upper()}"]
 
 
 def get_color(color_code, cm=None):
     if cm is None:
@@ -25,15 +25,15 @@
         return cv2.applyColorMap(np.array(int(255*color_code), dtype=np.uint8), str2cmap(cm)).flatten()
 
 
 def get_color_batched(col_vals, cm=None):
     colored_batch = np.zeros((len(col_vals), 3))
     if cm is None or cm == 'default':
         # use default color palette
-        col_vals = col_vals.astype(np.int32)
+        col_vals = col_vals.astype(int)
         unique_cvals = np.unique(col_vals)
         for uq_cval in unique_cvals:
             if uq_cval >= 0:
                 colored_batch[col_vals == uq_cval] = color_palette[uq_cval % len(
                     color_palette)]
             else:
                 colored_batch[col_vals == uq_cval] = special_color_palette[(
```

## Comparing `dvis-0.8.7.3.dist-info/METADATA` & `dvis-0.8.7.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvis
-Version: 0.8.7.3
+Version: 0.8.7.5
 Summary: The best web-based visualizer
 Home-page: https://github.com/SirWyver/dvis
 Author: Norman Müller
 Author-email: norman.mueller@tum.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `dvis-0.8.7.3.dist-info/RECORD` & `dvis-0.8.7.5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 dvis/__init__.py,sha256=bfwoJN9nz_CchjmbhA9LJ0RKF1sHsInHrU4y79KfKpg,35
-dvis/dvis.py,sha256=C_yURtfDco7HbU-fUU7Cbe9B4oj-RcWd0TiISLhFHdo,38101
+dvis/dvis.py,sha256=bMPtoBL7E5pnnn-DaljlZHxfQHrb9E5O4K4hHVsKxYA,38991
 dvis/dvis_cli.py,sha256=ON6Hgf4fZLldr2kRYlcDszVr5aONASkJOv3fhW_B5cE,1525
 dvis/dvis_client.py,sha256=IuyqDe6B2K0pc9gJv0zCH3xUBKGuJTnPZRrJlFmmv-w,8263
 dvis/dvis_client_old.py,sha256=kJCMvv9fMB0o2xT1rXeFknTlYwxVipsmtR4XZD6jgHM,6060
-dvis/utils.py,sha256=s2q78zNtycRXMCSyk14_iALqUAnRoX6BvamKuIuVJMQ,5519
-dvis-0.8.7.3.dist-info/METADATA,sha256=DxSCFJr_JLPhE62RndkVztxG4dI9cEbcAl3jMurqa7s,4228
-dvis-0.8.7.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dvis-0.8.7.3.dist-info/entry_points.txt,sha256=2MbvKd1b3fX4-mCWebjq9WV9WGvKphkaIWK1y9t8Rfw,92
-dvis-0.8.7.3.dist-info/top_level.txt,sha256=umqc2hmt_MBtmCWlbzVNRfIDt27Fp6CQmRB6dhDkcnk,5
-dvis-0.8.7.3.dist-info/RECORD,,
+dvis/utils.py,sha256=HqiY7EByL6jGPmtFn01vrUOSYjqN9rGHwijWsr6uTJc,5510
+dvis-0.8.7.5.dist-info/METADATA,sha256=T5JUpTtgP_vvTaW22byz0mfvUiIqwGoI4r_VUHOtwuc,4228
+dvis-0.8.7.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dvis-0.8.7.5.dist-info/entry_points.txt,sha256=2MbvKd1b3fX4-mCWebjq9WV9WGvKphkaIWK1y9t8Rfw,92
+dvis-0.8.7.5.dist-info/top_level.txt,sha256=umqc2hmt_MBtmCWlbzVNRfIDt27Fp6CQmRB6dhDkcnk,5
+dvis-0.8.7.5.dist-info/RECORD,,
```

