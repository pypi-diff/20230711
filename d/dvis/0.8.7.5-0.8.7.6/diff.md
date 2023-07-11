# Comparing `tmp/dvis-0.8.7.5-py3-none-any.whl.zip` & `tmp/dvis-0.8.7.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18591 bytes, number of entries: 11
+Zip file size: 18598 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx       35 b- defN 22-Aug-10 15:03 dvis/__init__.py
--rw-rw-r--  2.0 unx    38991 b- defN 23-Jul-11 09:52 dvis/dvis.py
+-rw-rw-r--  2.0 unx    39040 b- defN 23-Jul-11 10:21 dvis/dvis.py
 -rw-rw-r--  2.0 unx     1525 b- defN 23-Jan-04 10:29 dvis/dvis_cli.py
 -rw-rw-r--  2.0 unx     8263 b- defN 23-Jan-02 10:43 dvis/dvis_client.py
 -rw-rw-r--  2.0 unx     6060 b- defN 22-Aug-10 15:03 dvis/dvis_client_old.py
 -rw-rw-r--  2.0 unx     5510 b- defN 23-Jul-11 09:52 dvis/utils.py
--rw-rw-r--  2.0 unx     4228 b- defN 23-Jul-11 09:52 dvis-0.8.7.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 09:52 dvis-0.8.7.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 09:52 dvis-0.8.7.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        5 b- defN 23-Jul-11 09:52 dvis-0.8.7.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      827 b- defN 23-Jul-11 09:52 dvis-0.8.7.5.dist-info/RECORD
-11 files, 65628 bytes uncompressed, 17209 bytes compressed:  73.8%
+-rw-rw-r--  2.0 unx     4228 b- defN 23-Jul-11 10:21 dvis-0.8.7.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 10:21 dvis-0.8.7.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 10:21 dvis-0.8.7.6.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-11 10:21 dvis-0.8.7.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      827 b- defN 23-Jul-11 10:21 dvis-0.8.7.6.dist-info/RECORD
+11 files, 65677 bytes uncompressed, 17216 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: dvis/dvis_client_old.py
 Comment: 
 
 Filename: dvis/utils.py
 Comment: 
 
-Filename: dvis-0.8.7.5.dist-info/METADATA
+Filename: dvis-0.8.7.6.dist-info/METADATA
 Comment: 
 
-Filename: dvis-0.8.7.5.dist-info/WHEEL
+Filename: dvis-0.8.7.6.dist-info/WHEEL
 Comment: 
 
-Filename: dvis-0.8.7.5.dist-info/entry_points.txt
+Filename: dvis-0.8.7.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: dvis-0.8.7.5.dist-info/top_level.txt
+Filename: dvis-0.8.7.6.dist-info/top_level.txt
 Comment: 
 
-Filename: dvis-0.8.7.5.dist-info/RECORD
+Filename: dvis-0.8.7.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dvis/dvis.py

```diff
@@ -3,21 +3,21 @@
 
 Note:
     Requires DVIS server to run - sends data via websocket to localhost:5001 (3D visualizations) and localhost:4999 (using visdom for 2D visualization).
 """
 import shutil
 import numpy as np
 try:
-    import torch.Tensor, torch.float, torch.double
+    from torch import Tensor as torch_tensor
+    from torch import float as torch_float
+    from torch import double as torch_double
 except:
-    class Dummy():
-        Tensor = None
-        float = None
-        double = None
-    torch = Dummy()
+    torch_tensor = None
+    torch_float = None
+    torch_double = None
 from .dvis_client_old import (
     sendMesh2server,
     send_clear,
     send_config,
     sendTrack2server,
     send_camera,
     sendCmd2server,
@@ -48,15 +48,15 @@
     if type(data) == list:
         # convert to array
         return np.stack([convert_to_nd(x) for x in data])
     if type(data) == np.ndarray:
         return data
     if type(data) == list:
         return np.array(data)
-    if type(data) == torch.Tensor:
+    if type(data) == torch_tensor:
         return data.data.cpu().numpy()
     try:
         import imageio
         if type(data) == imageio.core.util.Array:
             return np.array(data)
     except:
         pass
@@ -297,15 +297,15 @@
 
 
 ##### refactoring
 
 
 def dvis_obj_kf(data, t, name):
     # sending object keyframe state
-    if isinstance(data, (np.ndarray, torch.Tensor)):
+    if isinstance(data, (np.ndarray, torch_tensor)):
         trs = data
         visible = True
         obj_name = name
         kf = t
     else:
         trs = data["trs"]
         visible = data.get("visible")
@@ -329,15 +329,15 @@
         text = data[0]
     elif isinstance(data, dict):
         pos = data.get("position", data.get("pos"))
         text = data.get("text", data.get("txt"))
     else:
         pos = data
         text = name
-    if isinstance(pos, (np.ndarray, torch.Tensor)):
+    if isinstance(pos, (np.ndarray, torch_tensor)):
         pos = pos.tolist()
     send2server(
         data={"position": pos, "text": text},
         data_format="text",
         size=vs,
         color=c,
         layers=l,
@@ -468,15 +468,15 @@
     send2server(None, "group", vs=1, c=1, t=0, l=[0], add=False, name=name, meta=meta)
 
 
 def dvis_points(data, fmt="points", s=1, c=0, l=[0], t=None, name=None, meta=None, ms=None, vis_conf=None, shape="b", cm=None, sub_format=None):
     """Display points
 
     Args:
-        data (np.ndarray, torch.Tensor): point cloud data
+        data (np.ndarray, torch_tensor): point cloud data
         fmt (str): points, xyzrgb, xyz, xyzc, xyzr
     """
     if name is None:
         name = "Points"
     data = convert_to_nd(data)
 
     if fmt == "points":
@@ -530,15 +530,15 @@
     send2server(data, fmt, s, c, l, t, name, meta, vis_conf, shape, sub_format=sub_format)
 
 
 def dvis_voxels(data, fmt="voxels", s=1, c=0, l=[0], t=None, name=None, meta=None, ms=None, vis_conf=None, shape="v", cm=None):
     """Display voxels
 
     Args:
-        data (np.ndarray, torch.Tensor): voxel grid data
+        data (np.ndarray, torch_tensor): voxel grid data
         fmt (str): voxels, cwhl, whlc, whl
     """
     if name is None:
         name = "Voxels"
 
     data = convert_to_nd(data)
     if fmt == "voxels":
@@ -574,15 +574,15 @@
     dvis_points(data, fmt, s, c, l, t, name, meta, vis_conf, ms, shape, cm=cm, sub_format=sub_format)
 
 
 def dvis_box(data, fmt="box", s=1, c=0, l=[0], t=None, name=None, meta=None, ms=None, vis_conf=None, shape="v"):
     """Display boxed annotation
 
     Args:
-        data (np.ndarray, torch.Tensor): Nxk box data
+        data (np.ndarray, torch_tensor): Nxk box data
         fmt (str): box, bbox, hbboxes, hbboxes_c, corners
 
     Formats:
         - bbox: Nx (x_min, y_min, z_min, x_max, y_max, z_max)
         - hbboxes: Nx (x, y, z, w, h, l, angle)
         - hbboxes_c: Nx (x, y, z, w, h, l, angle, c)
 
@@ -650,15 +650,15 @@
 
     return send2server(tm, compression, None, c, l, t, name, meta, vis_conf, None, compression)
 
 
 def dvis_vec(data, s=1, c=0, l=[0], t=0, name="vec", meta=None, vis_conf=None):
     """Display vector(s)
     Args:
-        data (tuple,list,torch.Tensor, np.ndarray): start_pos, end_pos of the vector(s)
+        data (tuple,list,torch_tensor, np.ndarray): start_pos, end_pos of the vector(s)
 
     For Nx3, start_pos is origin
     """
     if name is None:
         name = "vec"
     start_pos = np.zeros((1, 3))
     if isinstance(data, (tuple, list)):
@@ -666,29 +666,29 @@
         if len(data) > 2:
             # regard data as single vec
             end_pos = np.array([data])
 
         else:
             start_pos, end_pos = data
             start_pos, end_pos = np.expand_dims(start_pos, 0), np.expand_dims(end_pos, 0)
-    elif isinstance(data, (np.ndarray, torch.Tensor)):
+    elif isinstance(data, (np.ndarray, torch_tensor)):
         if len(data.shape) == 1:
             if data.shape[0] == 3:
                 end_pos = data[None, :]
             else:
                 start_pos, end_pos = np.expand_dims(data[:3], 0), np.expand_dims(data[3:6], 0)
         elif len(data.shape) == 2:
             if data.shape[1] == 3:
                 start_pos, end_pos = np.tile(start_pos, (data.shape[0], 1)), data
             else:
                 start_pos, end_pos = data[:, :3], data[:, 3:6]
 
-    if isinstance(end_pos, torch.Tensor):
+    if isinstance(end_pos, torch_tensor):
         end_pos = end_pos.cpu().numpy()
-    if isinstance(start_pos, torch.Tensor):
+    if isinstance(start_pos, torch_tensor):
         start_pos = start_pos.cpu().numpy()
     data = np.concatenate([start_pos, end_pos], 1)
     data_np = convert_to_nd(data)
     send2server(
         data=data_np,
         data_format="vec",
         size=s,
@@ -701,15 +701,15 @@
         compression="pkl",
     )
 
 
 def dvis_line(data, s=1, c=0, l=[0], t=0, name="line", meta=None, vis_conf=None):
     """Display vector
     Args:
-        data (torch.Tensor, np.ndarray): Nx3 array of line vertices
+        data (torch_tensor, np.ndarray): Nx3 array of line vertices
     """
     if name is None:
         name = "line"
     data_np = convert_to_nd(data)
     send2server(
         data=data_np,
         data_format="line",
@@ -723,15 +723,15 @@
         compression="pkl",
     )
 
 
 def dvis_arrow(data, s=1, c=0, l=[0], t=0, name="arrow", meta=None, vis_conf=None):
     """Display arrow
     Args:
-        data (torch.Tensor, np.ndarray): 3x3 or 4x4 transformation matrix
+        data (torch_tensor, np.ndarray): 3x3 or 4x4 transformation matrix
     """
     if name is None:
         name = "arrow"
     data_np = convert_to_nd(data)
     if data_np.shape[0] == 3 and data_np.shape[1] == 3:
         trans_fmt = np.eye(4)
         trans_fmt[:3, :3] = data_np
@@ -750,15 +750,15 @@
         compression="pkl",
     )
 
 
 def dvis_transform(data, s=1, c=0, l=[0], t=0, name="transform", meta=None, vis_conf=None):
     """Display transformation
     Args:
-        data (torch.Tensor, np.ndarray): 3x3 or 4x4 transformation matrix
+        data (torch_tensor, np.ndarray): 3x3 or 4x4 transformation matrix
     """
     if name is None:
         name = "transform"
     data_np = convert_to_nd(data)
     if data_np.shape[0] == 3 and data_np.shape[1] == 3:
         trans_fmt = np.eye(4)
         trans_fmt[:3, :3] = data_np
@@ -915,16 +915,16 @@
     if isinstance(data, np.ndarray):
         if data.dtype in [np.float32, np.float64]:
             # range type
             return 'xyr'
         else:
             # label type
             return 'xyl'
-    elif isinstance(data, torch.Tensor):
-        if data.dtype in [torch.float, torch.double]:
+    elif isinstance(data, torch_tensor):
+        if data.dtype in [torch_float, torch_double]:
             # range type
             return 'xyr'
         else:
             # label type
             return 'xyl'
     else:
         raise IOError("Unknown instance type")
```

## Comparing `dvis-0.8.7.5.dist-info/METADATA` & `dvis-0.8.7.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvis
-Version: 0.8.7.5
+Version: 0.8.7.6
 Summary: The best web-based visualizer
 Home-page: https://github.com/SirWyver/dvis
 Author: Norman Müller
 Author-email: norman.mueller@tum.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `dvis-0.8.7.5.dist-info/RECORD` & `dvis-0.8.7.6.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 dvis/__init__.py,sha256=bfwoJN9nz_CchjmbhA9LJ0RKF1sHsInHrU4y79KfKpg,35
-dvis/dvis.py,sha256=bMPtoBL7E5pnnn-DaljlZHxfQHrb9E5O4K4hHVsKxYA,38991
+dvis/dvis.py,sha256=i0KKL1ReHPpfcBJvM0DB__wYLrAnV_0pJlNDkQXVmrU,39040
 dvis/dvis_cli.py,sha256=ON6Hgf4fZLldr2kRYlcDszVr5aONASkJOv3fhW_B5cE,1525
 dvis/dvis_client.py,sha256=IuyqDe6B2K0pc9gJv0zCH3xUBKGuJTnPZRrJlFmmv-w,8263
 dvis/dvis_client_old.py,sha256=kJCMvv9fMB0o2xT1rXeFknTlYwxVipsmtR4XZD6jgHM,6060
 dvis/utils.py,sha256=HqiY7EByL6jGPmtFn01vrUOSYjqN9rGHwijWsr6uTJc,5510
-dvis-0.8.7.5.dist-info/METADATA,sha256=T5JUpTtgP_vvTaW22byz0mfvUiIqwGoI4r_VUHOtwuc,4228
-dvis-0.8.7.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dvis-0.8.7.5.dist-info/entry_points.txt,sha256=2MbvKd1b3fX4-mCWebjq9WV9WGvKphkaIWK1y9t8Rfw,92
-dvis-0.8.7.5.dist-info/top_level.txt,sha256=umqc2hmt_MBtmCWlbzVNRfIDt27Fp6CQmRB6dhDkcnk,5
-dvis-0.8.7.5.dist-info/RECORD,,
+dvis-0.8.7.6.dist-info/METADATA,sha256=tEJ4LH3OwqEniTRQqzLakvHpww4lavFoQMupZiXIaHo,4228
+dvis-0.8.7.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dvis-0.8.7.6.dist-info/entry_points.txt,sha256=2MbvKd1b3fX4-mCWebjq9WV9WGvKphkaIWK1y9t8Rfw,92
+dvis-0.8.7.6.dist-info/top_level.txt,sha256=umqc2hmt_MBtmCWlbzVNRfIDt27Fp6CQmRB6dhDkcnk,5
+dvis-0.8.7.6.dist-info/RECORD,,
```

