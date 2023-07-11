# Comparing `tmp/foscat-2.0.5.tar.gz` & `tmp/foscat-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-js6yoa5p/foscat-2.0.5.tar", last modified: Wed Jul  5 10:04:06 2023, max compression
+gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-wu5frbmz/foscat-2.0.6.tar", last modified: Tue Jul 11 08:18:10 2023, max compression
```

## Comparing `foscat-2.0.5.tar` & `foscat-2.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 10:04:06.000000 foscat-2.0.5/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-05 10:04:06.000000 foscat-2.0.5/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2022-12-13 16:07:53.000000 foscat-2.0.5/README.md
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-07-05 10:04:06.000000 foscat-2.0.5/setup.cfg
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-07-05 10:02:36.000000 foscat-2.0.5/setup.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 10:04:06.000000 foscat-2.0.5/src/
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 10:04:06.000000 foscat-2.0.5/src/foscat/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57132 2023-06-10 06:53:35.000000 foscat-2.0.5/src/foscat/FoCUS.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.0.5/src/foscat/GetGPUinfo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     3594 2023-06-23 10:27:41.000000 foscat-2.0.5/src/foscat/Rformat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    16207 2023-07-05 10:03:34.000000 foscat-2.0.5/src/foscat/Synthesis.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.0.5/src/foscat/__init__.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    13733 2023-06-10 06:53:35.000000 foscat-2.0.5/src/foscat/backend.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.0.5/src/foscat/build_demo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.0.5/src/foscat/demo2d.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    29024 2023-07-05 08:23:52.000000 foscat-2.0.5/src/foscat/scat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.0.5/src/foscat/scat_cov.old.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    48336 2023-07-05 08:21:43.000000 foscat-2.0.5/src/foscat/scat_cov.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.0.5/src/foscat/scat_cov_new.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 10:04:06.000000 foscat-2.0.5/src/foscat.egg-info/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-05 10:04:06.000000 foscat-2.0.5/src/foscat.egg-info/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-07-05 10:04:06.000000 foscat-2.0.5/src/foscat.egg-info/SOURCES.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-07-05 10:04:06.000000 foscat-2.0.5/src/foscat.egg-info/dependency_links.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-07-05 10:04:06.000000 foscat-2.0.5/src/foscat.egg-info/requires.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-07-05 10:04:06.000000 foscat-2.0.5/src/foscat.egg-info/top_level.txt
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 08:18:10.000000 foscat-2.0.6/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-11 08:18:10.000000 foscat-2.0.6/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2023-07-11 08:17:35.000000 foscat-2.0.6/README.md
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-07-11 08:18:10.000000 foscat-2.0.6/setup.cfg
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-07-11 08:17:47.000000 foscat-2.0.6/setup.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 08:18:10.000000 foscat-2.0.6/src/
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 08:18:10.000000 foscat-2.0.6/src/foscat/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57132 2023-06-10 06:53:35.000000 foscat-2.0.6/src/foscat/FoCUS.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.0.6/src/foscat/GetGPUinfo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     3594 2023-06-23 10:27:41.000000 foscat-2.0.6/src/foscat/Rformat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    16435 2023-07-10 14:25:03.000000 foscat-2.0.6/src/foscat/Synthesis.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.0.6/src/foscat/__init__.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    13733 2023-06-10 06:53:35.000000 foscat-2.0.6/src/foscat/backend.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.0.6/src/foscat/build_demo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.0.6/src/foscat/demo2d.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    29191 2023-07-11 07:38:44.000000 foscat-2.0.6/src/foscat/scat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.0.6/src/foscat/scat_cov.old.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    48501 2023-07-11 07:42:05.000000 foscat-2.0.6/src/foscat/scat_cov.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.0.6/src/foscat/scat_cov_new.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 08:18:10.000000 foscat-2.0.6/src/foscat.egg-info/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-11 08:18:10.000000 foscat-2.0.6/src/foscat.egg-info/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-07-11 08:18:10.000000 foscat-2.0.6/src/foscat.egg-info/SOURCES.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-07-11 08:18:10.000000 foscat-2.0.6/src/foscat.egg-info/dependency_links.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-07-11 08:18:10.000000 foscat-2.0.6/src/foscat.egg-info/requires.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-07-11 08:18:10.000000 foscat-2.0.6/src/foscat.egg-info/top_level.txt
```

### Comparing `foscat-2.0.5/PKG-INFO` & `foscat-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.0.5
+Version: 2.0.6
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

### Comparing `foscat-2.0.5/README.md` & `foscat-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `foscat-2.0.5/setup.py` & `foscat-2.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='foscat',
-    version='2.0.5',
+    version='2.0.6',
     description='Generate synthetic Healpix or 2D data using Cross Scattering Transform' ,
     long_description='Utilize the Cross Scattering Transform (described in https://arxiv.org/abs/2207.12527) to synthesize Healpix or 2D data that is suitable for component separation purposes, such as denoising. \n A demo package for this process can be found at https://github.com/jmdelouis/FOSCAT_DEMO. \n\n List of developers : J.-M. Delouis, T. Foulquier, L. Mousset, E. Allys ' ,
     license='MIT',
     author='Jean-Marc DELOUIS',
     author_email='jean.marc.delouis@ifremer.fr',
     maintainer='Theo Foulquier',
     maintainer_email='theo.foulquier@ifremer.fr',
```

### Comparing `foscat-2.0.5/src/foscat/FoCUS.py` & `foscat-2.0.6/src/foscat/FoCUS.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.5/src/foscat/GetGPUinfo.py` & `foscat-2.0.6/src/foscat/GetGPUinfo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.5/src/foscat/Rformat.py` & `foscat-2.0.6/src/foscat/Rformat.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.5/src/foscat/Synthesis.py` & `foscat-2.0.6/src/foscat/Synthesis.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,14 +291,15 @@
             
         if self.nlog==self.history.shape[0]:
             new_log=np.zeros([self.history.shape[0]*2])
             new_log[0:self.nlog]=self.history
             self.history=new_log
 
         l_tot=self.ltot[self.ltot!=-1].mean()
+        
         self.history[self.nlog]=l_tot
 
         g_tot=grad.flatten()
 
         if g_tot.dtype=='complex64' or g_tot.dtype=='complex128':
             return l_tot.astype('float64'),g_tot
         
@@ -312,15 +313,18 @@
         if operation.get_use_R():
             if axis==0:
                 l_x=operation.to_R(x,only_border=True,chans=self.operation.chans)
                 x=operation.from_R(l_x)
             else:
                 l_x=operation.to_R(x[0],only_border=True,chans=self.operation.chans)
                 tmp_x=operation.from_R(l_x)
-                out_x=np.zeros([x.shape[0],tmp_x.shape[0]])
+                if self.operation.chans!=1:
+                    out_x=np.zeros([self.in_x_nshape,tmp_x.shape[0]])
+                else:
+                    out_x=np.zeros([self.in_x_nshape,tmp_x.shape[0],tmp_x.shape[1]])
                 out_x[0]=tmp_x
                 del tmp_x
                 for i in range(1,self.in_x_nshape):
                     l_x=operation.to_R(x[i],only_border=True,chans=self.operation.chans)
                     out_x[i]=operation.from_R(l_x)
                 x=out_x
         
@@ -361,14 +365,15 @@
         if do_lbfgs and (in_x.dtype=='complex64' or in_x.dtype=='complex128'):
             print('L_BFGS minimisation not yet implemented for acomplex array, use default FOSCAT minimizer or convert your problem to float32 or float64')
             exit(0)
             
         np.random.seed(self.mpi_rank*7+1234)
             
         if self.operation.get_use_R():
+            # TO DO : detect acis error, is it possible ?
             if axis==0:
                 x=self.operation.to_R_center(self.operation.backend.bk_cast(in_x),chans=self.operation.chans)
             else:
                 tmp_x=self.operation.to_R_center(self.operation.backend.bk_cast(in_x[0]),chans=self.operation.chans)
                 x=np.zeros([in_x.shape[0],tmp_x.shape[0]],dtype=self.operation.all_type)
                 x[0]=tmp_x
                 del tmp_x
```

### Comparing `foscat-2.0.5/src/foscat/backend.py` & `foscat-2.0.6/src/foscat/backend.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.5/src/foscat/build_demo.py` & `foscat-2.0.6/src/foscat/build_demo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.5/src/foscat/scat.py` & `foscat-2.0.6/src/foscat/scat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import foscat.FoCUS as FOC
 import numpy as np
 import foscat.Rformat as Rformat
 import tensorflow as tf
-
+import traceback
+  
 def read(filename):
     thescat=scat(1,1,1,1,1)
     return thescat.read(filename)
     
 class scat:
     def __init__(self,p00,s0,s1,s2,s2l,cross=False,backend=None):
         self.P00=p00
@@ -424,21 +425,24 @@
         
     
 class funct(FOC.FoCUS):
     
     def eval(self, image1, image2=None,mask=None,Auto=True,s0_off=1E-6):
         # Check input consistency
         if not isinstance(image1,Rformat.Rformat):
-            if image2 is not None:
+            if image2 is not None and not isinstance(image2,Rformat.Rformat):
                 if list(image1.shape)!=list(image2.shape):
                     print('The two input image should have the same size to eval Scattering')
+                    traceback.print_exc()
+                    
                     exit(0)
             if mask is not None:
                 if list(image1.shape)!=list(mask.shape)[1:]:
                     print('The mask should have the same size than the input image to eval Scattering')
+                    traceback.print_exc()
                     exit(0)
             
         ### AUTO OR CROSS
         cross = False
         if image2 is not None:
             cross = True
             all_cross=not Auto
```

### Comparing `foscat-2.0.5/src/foscat/scat_cov.old.py` & `foscat-2.0.6/src/foscat/scat_cov.old.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.5/src/foscat/scat_cov.py` & `foscat-2.0.6/src/foscat/scat_cov.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import foscat.FoCUS as FOC
 import numpy as np
 import foscat.backend as bk
 import foscat.Rformat as Rformat
-
+import traceback
 
 def read(filename):
     thescat = scat_cov(1, 1, 1)
     return thescat.read(filename)
 
 
 testwarn=0
@@ -724,21 +724,23 @@
             If True return only the terms computable in the auto case.
         Returns
         -------
         S1, P00, C01, C11 normalized
         """
         # Check input consistency
         if not isinstance(image1,Rformat.Rformat):
-            if image2 is not None:
+            if image2 is not None and not isinstance(image2,Rformat.Rformat):
                 if list(image1.shape)!=list(image2.shape):
-                    print('The two input image should have the same size to eval Scattering')
+                    print('The two input image should have the same size to eval Scattering Covariance')
+                    traceback.print_exc()
                     exit(0)
             if mask is not None:
                 if list(image1.shape)!=list(mask.shape)[1:]:
-                    print('The mask should have the same size than the input image to eval Scattering')
+                    print('The mask should have the same size than the input image to eval Scattering Covariance')
+                    traceback.print_exc()
                     exit(0)
 
         ### AUTO OR CROSS
         cross = False
         if image2 is not None:
             cross = True
             all_cross=Auto
```

### Comparing `foscat-2.0.5/src/foscat/scat_cov_new.py` & `foscat-2.0.6/src/foscat/scat_cov_new.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.5/src/foscat.egg-info/PKG-INFO` & `foscat-2.0.6/src/foscat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.0.5
+Version: 2.0.6
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

