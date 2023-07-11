# Comparing `tmp/pilab-regis-0.0.2.tar.gz` & `tmp/pilab-regis-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilab-regis-0.0.2.tar", last modified: Thu Mar  9 14:47:54 2023, max compression
+gzip compressed data, was "pilab-regis-0.0.3.tar", last modified: Tue Jul 11 08:34:29 2023, max compression
```

## Comparing `pilab-regis-0.0.2.tar` & `pilab-regis-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 14:47:54.530000 pilab-regis-0.0.2/
--rw-rw-rw-   0        0        0     2350 2023-03-09 14:47:56.000000 pilab-regis-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2039 2023-03-09 14:32:46.000000 pilab-regis-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-09 14:47:54.530000 pilab-regis-0.0.2/pilab_regis.egg-info/
--rw-rw-rw-   0        0        0     2350 2023-03-09 14:47:56.000000 pilab-regis-0.0.2/pilab_regis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-03-09 14:47:56.000000 pilab-regis-0.0.2/pilab_regis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 14:47:56.000000 pilab-regis-0.0.2/pilab_regis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-03-09 14:47:56.000000 pilab-regis-0.0.2/pilab_regis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-09 14:47:56.000000 pilab-regis-0.0.2/pilab_regis.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-09 14:47:54.550000 pilab-regis-0.0.2/regis/
--rw-rw-rw-   0        0        0       70 2023-03-09 14:47:30.000000 pilab-regis-0.0.2/regis/__init__.py
--rw-rw-rw-   0        0        0     8421 2023-03-09 14:39:24.000000 pilab-regis-0.0.2/regis/core.py
--rw-rw-rw-   0        0        0       42 2023-03-09 14:47:56.000000 pilab-regis-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-03-02 09:42:46.000000 pilab-regis-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:29.330000 pilab-regis-0.0.3/
+-rw-rw-rw-   0        0        0     2350 2023-07-11 08:34:30.000000 pilab-regis-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2039 2023-03-09 14:32:46.000000 pilab-regis-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:29.340000 pilab-regis-0.0.3/pilab_regis.egg-info/
+-rw-rw-rw-   0        0        0     2350 2023-07-11 08:34:30.000000 pilab-regis-0.0.3/pilab_regis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-07-11 08:34:30.000000 pilab-regis-0.0.3/pilab_regis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 08:34:30.000000 pilab-regis-0.0.3/pilab_regis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-11 08:34:30.000000 pilab-regis-0.0.3/pilab_regis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-11 08:34:30.000000 pilab-regis-0.0.3/pilab_regis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:29.350000 pilab-regis-0.0.3/regis/
+-rw-rw-rw-   0        0        0       70 2023-07-11 08:33:34.000000 pilab-regis-0.0.3/regis/__init__.py
+-rw-rw-rw-   0        0        0     8611 2023-04-06 12:42:04.000000 pilab-regis-0.0.3/regis/core.py
+-rw-rw-rw-   0        0        0       42 2023-07-11 08:34:30.000000 pilab-regis-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-03-02 09:42:46.000000 pilab-regis-0.0.3/setup.py
```

### Comparing `pilab-regis-0.0.2/PKG-INFO` & `pilab-regis-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilab-regis
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/PiLAB-Medical-Imaging/registration
 Author: PiLAB
 Author-email: nicolas.delinte@uclouvain.be
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `pilab-regis-0.0.2/README.md` & `pilab-regis-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pilab-regis-0.0.2/pilab_regis.egg-info/PKG-INFO` & `pilab-regis-0.0.3/pilab_regis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilab-regis
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/PiLAB-Medical-Imaging/registration
 Author: PiLAB
 Author-email: nicolas.delinte@uclouvain.be
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `pilab-regis-0.0.2/regis/core.py` & `pilab-regis-0.0.3/regis/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,16 @@
 
 
 def apply_transform(moving_file: str, mapping, static_file: str = '',
                     output_path: str = '', binary: bool = False,
                     binary_thresh: float = 0.5, labels: bool = False,
                     inverse: bool = False, mask_file: str = ''):
     '''
-
+    Applies the transformation obtained from find_transform() in 'mapping' to a
+    moving file.
 
     Parameters
     ----------
     moving_file : str
         Moving file path.
     mapping : TYPE
         Deformation from moving to static.
@@ -191,16 +192,16 @@
     inverse : bool, optional
         If True, the inverse transformation is applied. The default is False.
     mask_file : str, optional
         If specified, applies a binary mask to moving file before mapping.
 
     Returns
     -------
-    transformed : TYPE
-        DESCRIPTION.
+    transformed : 3-D array of shape (x,y,z)
+        Transformed array.
 
     '''
 
     moving = nib.load(moving_file)
     moving_data = moving.get_fdata()
 
     if len(moving_data.shape) > 3:
@@ -221,14 +222,17 @@
     else:
         transformed = mapping.transform(moving_data,
                                         interpolation=interpolation)
 
     if binary:
         transformed = np.where(transformed > binary_thresh, 1, 0)
 
+    if labels:
+        transformed = transformed.astype(int)
+
     if len(output_path) > 0:
 
         static = nib.load(static_file)
 
         out = nib.Nifti1Image(transformed, static.affine, header=static.header)
         out.to_filename(output_path)
```

### Comparing `pilab-regis-0.0.2/setup.py` & `pilab-regis-0.0.3/setup.py`

 * *Files identical despite different names*

