# Comparing `tmp/point-cloud-utils-0.29.5.tar.gz` & `tmp/point-cloud-utils-0.29.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "point-cloud-utils-0.29.5.tar", last modified: Wed Apr 19 13:31:43 2023, max compression
+gzip compressed data, was "point-cloud-utils-0.29.6.tar", last modified: Mon Jul 10 20:58:24 2023, max compression
```

## Comparing `point-cloud-utils-0.29.5.tar` & `point-cloud-utils-0.29.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:31:43.473127 point-cloud-utils-0.29.5/
--rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-04-19 13:31:26.000000 point-cloud-utils-0.29.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36230 2023-04-19 13:31:43.469127 point-cloud-utils-0.29.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35746 2023-04-19 13:31:26.000000 point-cloud-utils-0.29.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:31:43.469127 point-cloud-utils-0.29.5/point_cloud_utils/
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/_mesh_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/_point_cloud_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/_pointcloud_normals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/_ray_mesh_intersector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/_ray_point_cloud_intersector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/_sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/point_cloud_utils/_voxels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:31:43.469127 point-cloud-utils-0.29.5/point_cloud_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36230 2023-04-19 13:31:43.000000 point-cloud-utils-0.29.5/point_cloud_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-19 13:31:43.000000 point-cloud-utils-0.29.5/point_cloud_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:31:43.000000 point-cloud-utils-0.29.5/point_cloud_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:31:43.000000 point-cloud-utils-0.29.5/point_cloud_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 13:31:43.000000 point-cloud-utils-0.29.5/point_cloud_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 13:31:43.000000 point-cloud-utils-0.29.5/point_cloud_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:31:43.473127 point-cloud-utils-0.29.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:31:43.469127 point-cloud-utils-0.29.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    32125 2023-04-19 13:31:27.000000 point-cloud-utils-0.29.5/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:58:24.550897 point-cloud-utils-0.29.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-07-10 20:58:07.000000 point-cloud-utils-0.29.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36230 2023-07-10 20:58:24.550897 point-cloud-utils-0.29.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35746 2023-07-10 20:58:07.000000 point-cloud-utils-0.29.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:58:24.550897 point-cloud-utils-0.29.6/point_cloud_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-07-10 20:58:08.000000 point-cloud-utils-0.29.6/point_cloud_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-07-10 20:58:08.000000 point-cloud-utils-0.29.6/point_cloud_utils/_mesh_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-10 20:58:08.000000 point-cloud-utils-0.29.6/point_cloud_utils/_point_cloud_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-10 20:58:08.000000 point-cloud-utils-0.29.6/point_cloud_utils/_pointcloud_normals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-10 20:58:08.000000 point-cloud-utils-0.29.6/point_cloud_utils/_ray_mesh_intersector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-10 20:58:08.000000 point-cloud-utils-0.29.6/point_cloud_utils/_ray_point_cloud_intersector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-07-10 20:58:08.000000 point-cloud-utils-0.29.6/point_cloud_utils/_sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-10 20:58:08.000000 point-cloud-utils-0.29.6/point_cloud_utils/_voxels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:58:24.550897 point-cloud-utils-0.29.6/point_cloud_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36230 2023-07-10 20:58:24.000000 point-cloud-utils-0.29.6/point_cloud_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-10 20:58:24.000000 point-cloud-utils-0.29.6/point_cloud_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:58:24.000000 point-cloud-utils-0.29.6/point_cloud_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:58:24.000000 point-cloud-utils-0.29.6/point_cloud_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 20:58:24.000000 point-cloud-utils-0.29.6/point_cloud_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 20:58:24.000000 point-cloud-utils-0.29.6/point_cloud_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-10 20:58:08.000000 point-cloud-utils-0.29.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 20:58:24.550897 point-cloud-utils-0.29.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-10 20:58:08.000000 point-cloud-utils-0.29.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:58:24.550897 point-cloud-utils-0.29.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    32125 2023-07-10 20:58:08.000000 point-cloud-utils-0.29.6/tests/test_examples.py
```

### Comparing `point-cloud-utils-0.29.5/LICENSE` & `point-cloud-utils-0.29.6/LICENSE`

 * *Files identical despite different names*

### Comparing `point-cloud-utils-0.29.5/PKG-INFO` & `point-cloud-utils-0.29.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: point-cloud-utils
-Version: 0.29.5
+Version: 0.29.6
 Summary: A Python library for common tasks on 3D point clouds and meshes
 Home-page: https://github.com/fwilliams/point-cloud-utils
 Author: Francis Williams
 Author-email: francis@fwilliams.info
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -885,9 +885,9 @@
 voxel_origin = [0.0, 0.0, 0.0]  # The position of the bottom-back-left corner of the (0, 0, 0) voxel
 
 gap_fraction = 0.01  # Generate an optional small gap between voxels which can look nice -- this is a fraction of the voxel size
 
 ijk = np.random.randint(-100, 100, size=(128, 3))  # Generate 128 random voxels in [-100, 100]^3
 
 # vox_v, vox_f are vertices/faces of mesh for voxel grid
-vox_v, vox_f = pcu.voxel_grid_geoemtry(ijk, v, gap_fraction=gap_fraction, voxel_size=voxel_size, voxel_origin=voxel_origin)
+vox_v, vox_f = pcu.voxel_grid_geoemtry(ijk, v, voxel_size=voxel_size, voxel_origin=voxel_origin, gap_fraction=gap_fraction)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: point-cloud-utils Version: 0.29.5 Summary: A Python
+Metadata-Version: 2.1 Name: point-cloud-utils Version: 0.29.6 Summary: A Python
 library for common tasks on 3D point clouds and meshes Home-page: https://
 github.com/fwilliams/point-cloud-utils Author: Francis Williams Author-email:
 francis@fwilliams.info Classifier: Programming Language :: C++ Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v3 (GPLv3) Description-Content-Type: text/markdown
 License-File: LICENSE ![Point Cloud Utils Logo](docs/docs/imgs/logo_crop.png) !
 [Point Cloud Utils Teaser](docs/docs/imgs/pcu_teaser_3.png)
@@ -457,9 +457,9 @@
 `voxel_grid_geometry` function as follows ```python import point_cloud_utils as
 pcu voxel_size = 1.0 / 200.0 # Size of each voxel voxel_origin = [0.0, 0.0,
 0.0] # The position of the bottom-back-left corner of the (0, 0, 0) voxel
 gap_fraction = 0.01 # Generate an optional small gap between voxels which can
 look nice -- this is a fraction of the voxel size ijk = np.random.randint(-100,
 100, size=(128, 3)) # Generate 128 random voxels in [-100, 100]^3 # vox_v,
 vox_f are vertices/faces of mesh for voxel grid vox_v, vox_f =
-pcu.voxel_grid_geoemtry(ijk, v, gap_fraction=gap_fraction,
-voxel_size=voxel_size, voxel_origin=voxel_origin) ```
+pcu.voxel_grid_geoemtry(ijk, v, voxel_size=voxel_size,
+voxel_origin=voxel_origin, gap_fraction=gap_fraction) ```
```

### Comparing `point-cloud-utils-0.29.5/README.md` & `point-cloud-utils-0.29.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -872,9 +872,9 @@
 voxel_origin = [0.0, 0.0, 0.0]  # The position of the bottom-back-left corner of the (0, 0, 0) voxel
 
 gap_fraction = 0.01  # Generate an optional small gap between voxels which can look nice -- this is a fraction of the voxel size
 
 ijk = np.random.randint(-100, 100, size=(128, 3))  # Generate 128 random voxels in [-100, 100]^3
 
 # vox_v, vox_f are vertices/faces of mesh for voxel grid
-vox_v, vox_f = pcu.voxel_grid_geoemtry(ijk, v, gap_fraction=gap_fraction, voxel_size=voxel_size, voxel_origin=voxel_origin)
+vox_v, vox_f = pcu.voxel_grid_geoemtry(ijk, v, voxel_size=voxel_size, voxel_origin=voxel_origin, gap_fraction=gap_fraction)
 ```
```

#### html2text {}

```diff
@@ -451,9 +451,9 @@
 `voxel_grid_geometry` function as follows ```python import point_cloud_utils as
 pcu voxel_size = 1.0 / 200.0 # Size of each voxel voxel_origin = [0.0, 0.0,
 0.0] # The position of the bottom-back-left corner of the (0, 0, 0) voxel
 gap_fraction = 0.01 # Generate an optional small gap between voxels which can
 look nice -- this is a fraction of the voxel size ijk = np.random.randint(-100,
 100, size=(128, 3)) # Generate 128 random voxels in [-100, 100]^3 # vox_v,
 vox_f are vertices/faces of mesh for voxel grid vox_v, vox_f =
-pcu.voxel_grid_geoemtry(ijk, v, gap_fraction=gap_fraction,
-voxel_size=voxel_size, voxel_origin=voxel_origin) ```
+pcu.voxel_grid_geoemtry(ijk, v, voxel_size=voxel_size,
+voxel_origin=voxel_origin, gap_fraction=gap_fraction) ```
```

### Comparing `point-cloud-utils-0.29.5/point_cloud_utils/__init__.py` & `point-cloud-utils-0.29.6/point_cloud_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `point-cloud-utils-0.29.5/point_cloud_utils/_mesh_io.py` & `point-cloud-utils-0.29.6/point_cloud_utils/_mesh_io.py`

 * *Files identical despite different names*

### Comparing `point-cloud-utils-0.29.5/point_cloud_utils/_point_cloud_geometry.py` & `point-cloud-utils-0.29.6/point_cloud_utils/_point_cloud_geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,26 +38,26 @@
 
     if len(r.shape) != 1:
         raise ValueError("Invalid shape for argument r, must have shape (N,) or (N, 1)")
 
     return r
 
 
-def voxel_grid_geometry(ijk, gap_fraction=0.0, voxel_size=np.array((1., 1., 1.)), voxel_origin=np.array((0., 0., 0.))):
+def voxel_grid_geometry(ijk, voxel_size=np.array((1., 1., 1.)), voxel_origin=np.array((0., 0., 0.)), gap_fraction=0.0):
     """
     Generate a triangle mesh of cubes for voxel coordinates ijk. The [0, 0, 0] voxel has its
     bottom-back-left corner at voxel_origin and each voxel has voxel_size.
 
     Args:
         ijk np.ndarray: [num_voxels, 3] array of integer voxel coordinates
-        gap_fraction: scalar between [0, 1) indicating how much of a gap to leave between voxels
         voxel_size: Float or triple representing the size of each voxel.
                     Defaults to np.array((1., 1., 1.)).
         voxel_origin: Bottom-back-left coordinate of the [0, 0, 0] voxel.
                       Defaults to np.array((0., 0., 0.)).
+        gap_fraction: Fraction of a voxel to leave as a gap between voxels (default 0.0)
 
     Returns:
         v: Numpy array of vertices for the cube mesh
         f: Numpy array of faces for the cube mesh
     """
     return _voxel_mesh_internal(ijk, gap_fraction,
                                 _coord3d_to_array(voxel_origin, dtype=np.float64),
```

### Comparing `point-cloud-utils-0.29.5/point_cloud_utils/_pointcloud_normals.py` & `point-cloud-utils-0.29.6/point_cloud_utils/_pointcloud_normals.py`

 * *Files identical despite different names*

### Comparing `point-cloud-utils-0.29.5/point_cloud_utils/_ray_mesh_intersector.py` & `point-cloud-utils-0.29.6/point_cloud_utils/_ray_mesh_intersector.py`

 * *Files identical despite different names*

### Comparing `point-cloud-utils-0.29.5/point_cloud_utils/_ray_point_cloud_intersector.py` & `point-cloud-utils-0.29.6/point_cloud_utils/_ray_point_cloud_intersector.py`

 * *Files identical despite different names*

### Comparing `point-cloud-utils-0.29.5/point_cloud_utils/_sinkhorn.py` & `point-cloud-utils-0.29.6/point_cloud_utils/_sinkhorn.py`

 * *Files identical despite different names*

### Comparing `point-cloud-utils-0.29.5/point_cloud_utils/_voxels.py` & `point-cloud-utils-0.29.6/point_cloud_utils/_voxels.py`

 * *Files identical despite different names*

### Comparing `point-cloud-utils-0.29.5/point_cloud_utils.egg-info/PKG-INFO` & `point-cloud-utils-0.29.6/point_cloud_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: point-cloud-utils
-Version: 0.29.5
+Version: 0.29.6
 Summary: A Python library for common tasks on 3D point clouds and meshes
 Home-page: https://github.com/fwilliams/point-cloud-utils
 Author: Francis Williams
 Author-email: francis@fwilliams.info
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -885,9 +885,9 @@
 voxel_origin = [0.0, 0.0, 0.0]  # The position of the bottom-back-left corner of the (0, 0, 0) voxel
 
 gap_fraction = 0.01  # Generate an optional small gap between voxels which can look nice -- this is a fraction of the voxel size
 
 ijk = np.random.randint(-100, 100, size=(128, 3))  # Generate 128 random voxels in [-100, 100]^3
 
 # vox_v, vox_f are vertices/faces of mesh for voxel grid
-vox_v, vox_f = pcu.voxel_grid_geoemtry(ijk, v, gap_fraction=gap_fraction, voxel_size=voxel_size, voxel_origin=voxel_origin)
+vox_v, vox_f = pcu.voxel_grid_geoemtry(ijk, v, voxel_size=voxel_size, voxel_origin=voxel_origin, gap_fraction=gap_fraction)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: point-cloud-utils Version: 0.29.5 Summary: A Python
+Metadata-Version: 2.1 Name: point-cloud-utils Version: 0.29.6 Summary: A Python
 library for common tasks on 3D point clouds and meshes Home-page: https://
 github.com/fwilliams/point-cloud-utils Author: Francis Williams Author-email:
 francis@fwilliams.info Classifier: Programming Language :: C++ Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v3 (GPLv3) Description-Content-Type: text/markdown
 License-File: LICENSE ![Point Cloud Utils Logo](docs/docs/imgs/logo_crop.png) !
 [Point Cloud Utils Teaser](docs/docs/imgs/pcu_teaser_3.png)
@@ -457,9 +457,9 @@
 `voxel_grid_geometry` function as follows ```python import point_cloud_utils as
 pcu voxel_size = 1.0 / 200.0 # Size of each voxel voxel_origin = [0.0, 0.0,
 0.0] # The position of the bottom-back-left corner of the (0, 0, 0) voxel
 gap_fraction = 0.01 # Generate an optional small gap between voxels which can
 look nice -- this is a fraction of the voxel size ijk = np.random.randint(-100,
 100, size=(128, 3)) # Generate 128 random voxels in [-100, 100]^3 # vox_v,
 vox_f are vertices/faces of mesh for voxel grid vox_v, vox_f =
-pcu.voxel_grid_geoemtry(ijk, v, gap_fraction=gap_fraction,
-voxel_size=voxel_size, voxel_origin=voxel_origin) ```
+pcu.voxel_grid_geoemtry(ijk, v, voxel_size=voxel_size,
+voxel_origin=voxel_origin, gap_fraction=gap_fraction) ```
```

### Comparing `point-cloud-utils-0.29.5/point_cloud_utils.egg-info/SOURCES.txt` & `point-cloud-utils-0.29.6/point_cloud_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `point-cloud-utils-0.29.5/setup.py` & `point-cloud-utils-0.29.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         sys.argv.remove('--use-mkl')
     if 'EXCLUDE_ARCH' in os.environ or '--exclude-arch' in sys.argv:
         exclude_arch = True
         sys.argv.remove('--exclude-arch')
 
     setuptools.setup(
         name="point-cloud-utils",
-        version="0.29.5",
+        version="0.29.6",
         author="Francis Williams",
         author_email="francis@fwilliams.info",
         description="A Python library for common tasks on 3D point clouds and meshes",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/fwilliams/point-cloud-utils",
         packages=setuptools.find_packages(exclude=["tests"]),
```

### Comparing `point-cloud-utils-0.29.5/tests/test_examples.py` & `point-cloud-utils-0.29.6/tests/test_examples.py`

 * *Files identical despite different names*

