# Comparing `tmp/foscat-2.0.7.tar.gz` & `tmp/foscat-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-pba4exkf/foscat-2.0.7.tar", last modified: Tue Jul 11 13:14:57 2023, max compression
+gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-0uexk0g6/foscat-2.1.0.tar", last modified: Tue Jul 11 15:11:14 2023, max compression
```

## Comparing `foscat-2.0.7.tar` & `foscat-2.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 13:14:57.000000 foscat-2.0.7/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-11 13:14:57.000000 foscat-2.0.7/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2023-07-11 08:17:35.000000 foscat-2.0.7/README.md
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-07-11 13:14:57.000000 foscat-2.0.7/setup.cfg
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-07-11 13:14:26.000000 foscat-2.0.7/setup.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 13:14:57.000000 foscat-2.0.7/src/
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 13:14:57.000000 foscat-2.0.7/src/foscat/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57626 2023-07-11 10:02:58.000000 foscat-2.0.7/src/foscat/FoCUS.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.0.7/src/foscat/GetGPUinfo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     3594 2023-06-23 10:27:41.000000 foscat-2.0.7/src/foscat/Rformat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    16435 2023-07-10 14:25:03.000000 foscat-2.0.7/src/foscat/Synthesis.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.0.7/src/foscat/__init__.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    13733 2023-06-10 06:53:35.000000 foscat-2.0.7/src/foscat/backend.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.0.7/src/foscat/build_demo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.0.7/src/foscat/demo2d.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    29274 2023-07-11 08:46:53.000000 foscat-2.0.7/src/foscat/scat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.0.7/src/foscat/scat_cov.old.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53642 2023-07-11 10:46:11.000000 foscat-2.0.7/src/foscat/scat_cov.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.0.7/src/foscat/scat_cov_new.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 13:14:57.000000 foscat-2.0.7/src/foscat.egg-info/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-11 13:14:57.000000 foscat-2.0.7/src/foscat.egg-info/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-07-11 13:14:57.000000 foscat-2.0.7/src/foscat.egg-info/SOURCES.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-07-11 13:14:57.000000 foscat-2.0.7/src/foscat.egg-info/dependency_links.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-07-11 13:14:57.000000 foscat-2.0.7/src/foscat.egg-info/requires.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-07-11 13:14:57.000000 foscat-2.0.7/src/foscat.egg-info/top_level.txt
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 15:11:14.000000 foscat-2.1.0/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-11 15:11:14.000000 foscat-2.1.0/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2023-07-11 08:17:35.000000 foscat-2.1.0/README.md
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-07-11 15:11:14.000000 foscat-2.1.0/setup.cfg
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-07-11 15:08:52.000000 foscat-2.1.0/setup.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 15:11:14.000000 foscat-2.1.0/src/
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 15:11:14.000000 foscat-2.1.0/src/foscat/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57613 2023-07-11 14:30:51.000000 foscat-2.1.0/src/foscat/FoCUS.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.1.0/src/foscat/GetGPUinfo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     3594 2023-06-23 10:27:41.000000 foscat-2.1.0/src/foscat/Rformat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    16435 2023-07-10 14:25:03.000000 foscat-2.1.0/src/foscat/Synthesis.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.1.0/src/foscat/__init__.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    13733 2023-06-10 06:53:35.000000 foscat-2.1.0/src/foscat/backend.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.1.0/src/foscat/build_demo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.1.0/src/foscat/demo2d.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    33367 2023-07-11 15:05:00.000000 foscat-2.1.0/src/foscat/scat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.1.0/src/foscat/scat_cov.old.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    54003 2023-07-11 15:05:12.000000 foscat-2.1.0/src/foscat/scat_cov.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.1.0/src/foscat/scat_cov_new.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 15:11:14.000000 foscat-2.1.0/src/foscat.egg-info/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-11 15:11:14.000000 foscat-2.1.0/src/foscat.egg-info/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-07-11 15:11:14.000000 foscat-2.1.0/src/foscat.egg-info/SOURCES.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-07-11 15:11:14.000000 foscat-2.1.0/src/foscat.egg-info/dependency_links.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-07-11 15:11:14.000000 foscat-2.1.0/src/foscat.egg-info/requires.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-07-11 15:11:14.000000 foscat-2.1.0/src/foscat.egg-info/top_level.txt
```

### Comparing `foscat-2.0.7/PKG-INFO` & `foscat-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.0.7
+Version: 2.1.0
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

### Comparing `foscat-2.0.7/README.md` & `foscat-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `foscat-2.0.7/setup.py` & `foscat-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='foscat',
-    version='2.0.7',
+    version='2.1.0',
     description='Generate synthetic Healpix or 2D data using Cross Scattering Transform' ,
     long_description='Utilize the Cross Scattering Transform (described in https://arxiv.org/abs/2207.12527) to synthesize Healpix or 2D data that is suitable for component separation purposes, such as denoising. \n A demo package for this process can be found at https://github.com/jmdelouis/FOSCAT_DEMO. \n\n List of developers : J.-M. Delouis, T. Foulquier, L. Mousset, E. Allys ' ,
     license='MIT',
     author='Jean-Marc DELOUIS',
     author_email='jean.marc.delouis@ifremer.fr',
     maintainer='Theo Foulquier',
     maintainer_email='theo.foulquier@ifremer.fr',
```

### Comparing `foscat-2.0.7/src/foscat/FoCUS.py` & `foscat-2.1.0/src/foscat/FoCUS.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 import healpy as hp
 import os, sys
 import foscat.backend as bk
 import foscat.Rformat as Rformat
 
-            
 class FoCUS:
     def __init__(self,
                  NORIENT=4,
                  LAMBDA=1.2,
                  KERNELSZ=3,
                  slope=1.0,
                  all_type='float64',
```

### Comparing `foscat-2.0.7/src/foscat/GetGPUinfo.py` & `foscat-2.1.0/src/foscat/GetGPUinfo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.7/src/foscat/Rformat.py` & `foscat-2.1.0/src/foscat/Rformat.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.7/src/foscat/Synthesis.py` & `foscat-2.1.0/src/foscat/Synthesis.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.7/src/foscat/backend.py` & `foscat-2.1.0/src/foscat/backend.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.7/src/foscat/build_demo.py` & `foscat-2.1.0/src/foscat/build_demo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.7/src/foscat/scat.py` & `foscat-2.1.0/src/foscat/scat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import foscat.FoCUS as FOC
 import numpy as np
 import foscat.Rformat as Rformat
 import tensorflow as tf
-import traceback
   
 def read(filename):
     thescat=scat(1,1,1,1,1)
     return thescat.read(filename)
     
 class scat:
     def __init__(self,p00,s0,s1,s2,s2l,cross=False,backend=None):
@@ -16,15 +15,15 @@
         self.S2=s2
         self.S2L=s2l
         self.cross=cross
         self.backend=backend
         
     def get_j_idx(self):
         shape=list(self.S1.shape)
-        nscale=shape[1]
+        nscale=shape[2]
         n=nscale*(nscale+1)//2
         j1=np.zeros([n],dtype='int')
         j2=np.zeros([n],dtype='int')
         n=0
         for i in range(nscale):
             for j in range(i+1):
                 j1[n]=j
@@ -240,54 +239,165 @@
 
         j1,j2=self.get_j_idx()
         
         if name is None:
             name=''
 
         if hold:
-            plt.figure(figsize=(8,8))
+            plt.figure(figsize=(16,8))
         
-        plt.subplot(2,2,1)
-        if legend:
-            plt.plot(abs(self.l1_abs(self.S1).flatten()),':',color=color,lw=lw)
-            plt.plot(self.l1_abs(self.S1).flatten(),color=color,label=r'%s $S_1$'%(name),lw=lw)
-        else:
-            plt.plot(abs(self.l1_abs(self.S1).flatten()),':',color=color,lw=lw)
-            plt.plot(self.l1_abs(self.S1).flatten(),color=color,lw=lw)
+        test=None
+        plt.subplot(2, 2, 1)
+        tmp=abs(self.get_np(self.S1))
+        for k in range(tmp.shape[3]):
+            for i1 in range(tmp.shape[0]):
+                for i2 in range(tmp.shape[0]):
+                    if test is None:
+                        test=1
+                        plt.plot(tmp[i1,i2,:,k],color=color, label=r'%s $S_{1}$' % (name), lw=lw)
+                    else:
+                        plt.plot(tmp[i1,i2,:,k],color=color, lw=lw)
         plt.yscale('log')
+        plt.ylabel('S1')
+        plt.xlabel(r'$j_{1}$')
         plt.legend()
-        plt.subplot(2,2,2)
-        if legend:
-            plt.plot(abs(self.l1_abs(self.P00).flatten()),':',color=color,lw=lw)
-            plt.plot(self.l1_abs(self.P00).flatten(),color=color,label=r'%s $P_{00}$'%(name),lw=lw)
-        else:
-            plt.plot(abs(self.l1_abs(self.P00).flatten()),':',color=color,lw=lw)
-            plt.plot(self.l1_abs(self.P00).flatten(),color=color,lw=lw)
+
+        test=None
+        plt.subplot(2, 2, 2)
+        tmp=abs(self.get_np(self.P00))
+        for k in range(tmp.shape[3]):
+            for i1 in range(tmp.shape[0]):
+                for i2 in range(tmp.shape[0]):
+                    if test is None:
+                        test=1
+                        plt.plot(tmp[i1,i2,:,k],color=color, label=r'%s $P_{00}$' % (name), lw=lw)
+                    else:
+                        plt.plot(tmp[i1,i2,:,k],color=color, lw=lw)
         plt.yscale('log')
+        plt.ylabel('P00')
+        plt.xlabel(r'$j_{1}$')
         plt.legend()
-        plt.subplot(2,2,3)
-        print(self.l1_abs(self.S2).shape,j1.shape)
-        if legend:
-            plt.plot(abs(self.l1_abs(self.S2).flatten()),':',color=color,lw=lw)
-            plt.plot(self.l1_abs(self.S2).flatten(),color=color,label=r'%s $S_2$ L1 norm'%(name),lw=lw)
-        else:
-            plt.plot(abs(self.l1_abs(self.S2).flatten()),':',color=color,lw=lw)
-            plt.plot(self.l1_abs(self.S2).flatten(),color=color,lw=lw)
+        
+        ax1=plt.subplot(2, 2, 3)
+        ax2 = ax1.twiny()
+        n=0
+        tmp=abs(self.get_np(self.S2))
+        lname=r'%s $S_{2}$' % (name)
+        ax1.set_ylabel(r'$S_{2}$ [L1 norm]')
+        test=None
+        tabx=[]
+        tabnx=[]
+        tab2x=[]
+        tab2nx=[]
+        for i0 in range(tmp.shape[0]):
+            for i1 in range(tmp.shape[1]):
+                for i2 in range(j1.max()+1):
+                    for i3 in range(tmp.shape[3]):
+                        for i4 in range(tmp.shape[4]):
+                            if j2[j1==i2].shape[0]==1:
+                                ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4],'.', \
+                                             color=color, lw=lw)
+                            else:
+                                if legend and test is None:
+                                    ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
+                                             color=color, label=lname, lw=lw)
+                                    test=1
+                                ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
+                                         color=color, lw=lw)
+                    tabnx=tabnx+[r'%d'%(k) for k in j2[j1==i2]]
+                    tabx=tabx+[k+n for k in j2[j1==i2]]
+                    tab2x=tab2x+[(j2[j1==i2]+n).mean()]
+                    tab2nx=tab2nx+['%d'%(i2)]
+                    ax1.axvline((j2[j1==i2]+n).max()+0.5,ls=':',color='gray') 
+                    n=n+j2[j1==i2].shape[0]-1
         plt.yscale('log')
-        plt.legend()
+        ax1.set_xlim(0,n+2)
+        ax1.set_xticks(tabx)
+        ax1.set_xticklabels(tabnx,fontsize=6)
+        ax1.set_xlabel(r"$j_{2}$ ",fontsize=6)
+        
+        # Move twinned axis ticks and label from top to bottom
+        ax2.xaxis.set_ticks_position("bottom")
+        ax2.xaxis.set_label_position("bottom")
+
+        # Offset the twin axis below the host
+        ax2.spines["bottom"].set_position(("axes", -0.15))
+
+        # Turn on the frame for the twin axis, but then hide all 
+        # but the bottom spine
+        ax2.set_frame_on(True)
+        ax2.patch.set_visible(False)
+
+        for sp in ax2.spines.values():
+            sp.set_visible(False)
+        ax2.spines["bottom"].set_visible(True)
+        ax2.set_xlim(0,n+2)
+        ax2.set_xticks(tab2x)
+        ax2.set_xticklabels(tab2nx,fontsize=6)
+        ax2.set_xlabel(r"$j_{1}$",fontsize=6)
+        ax1.legend(frameon=0)
         
-        plt.subplot(2,2,4)
-        if legend:
-            plt.plot(abs(self.l1_abs(self.S2L).flatten()),':',color=color,lw=lw)
-            plt.plot(self.l1_abs(self.S2L).flatten(),color=color,label=r'%s $S_2$ L2 norm'%(name),lw=lw)
-        else:
-            plt.plot(abs(self.l1_abs(self.S2L).flatten()),':',color=color,lw=lw)
-            plt.plot(self.l1_abs(self.S2L).flatten(),color=color,lw=lw)
+        ax1=plt.subplot(2, 2, 4)
+        ax2 = ax1.twiny()
+        n=0
+        tmp=abs(self.get_np(self.S2L))
+        lname=r'%s $S2_{2}$' % (name)
+        ax1.set_ylabel(r'$S_{2}$ [L2 norm]')
+        test=None
+        tabx=[]
+        tabnx=[]
+        tab2x=[]
+        tab2nx=[]
+        for i0 in range(tmp.shape[0]):
+            for i1 in range(tmp.shape[1]):
+                for i2 in range(j1.max()+1):
+                    for i3 in range(tmp.shape[3]):
+                        for i4 in range(tmp.shape[4]):
+                            if j2[j1==i2].shape[0]==1:
+                                ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4],'.', \
+                                             color=color, lw=lw)
+                            else:
+                                if legend and test is None:
+                                    ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
+                                             color=color, label=lname, lw=lw)
+                                    test=1
+                                ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
+                                         color=color, lw=lw)
+                    tabnx=tabnx+[r'%d'%(k) for k in j2[j1==i2]]
+                    tabx=tabx+[k+n for k in j2[j1==i2]]
+                    tab2x=tab2x+[(j2[j1==i2]+n).mean()]
+                    tab2nx=tab2nx+['%d'%(i2)]
+                    ax1.axvline((j2[j1==i2]+n).max()+0.5,ls=':',color='gray') 
+                    n=n+j2[j1==i2].shape[0]-1
         plt.yscale('log')
-        plt.legend()
+        ax1.set_xlim(-1,n+3)
+        ax1.set_xticks(tabx)
+        ax1.set_xticklabels(tabnx,fontsize=6)
+        ax1.set_xlabel(r"$j_{2}$",fontsize=6)
+        
+        # Move twinned axis ticks and label from top to bottom
+        ax2.xaxis.set_ticks_position("bottom")
+        ax2.xaxis.set_label_position("bottom")
+
+        # Offset the twin axis below the host
+        ax2.spines["bottom"].set_position(("axes", -0.15))
+
+        # Turn on the frame for the twin axis, but then hide all 
+        # but the bottom spine
+        ax2.set_frame_on(True)
+        ax2.patch.set_visible(False)
+
+        for sp in ax2.spines.values():
+            sp.set_visible(False)
+        ax2.spines["bottom"].set_visible(True)
+        ax2.set_xlim(0,n+3)
+        ax2.set_xticks(tab2x)
+        ax2.set_xticklabels(tab2nx,fontsize=6)
+        ax2.set_xlabel(r"$j_{1}$",fontsize=6)
+        ax1.legend(frameon=0)
         
     def save(self,filename):
         np.save('%s_s0.npy'%(filename), self.get_S0().numpy())
         np.save('%s_s1.npy'%(filename), self.get_S1().numpy())
         np.save('%s_s2.npy'%(filename), self.get_S2().numpy())
         np.save('%s_s2l.npy'%(filename), self.get_S2L().numpy())
         np.save('%s_p0.npy'%(filename), self.get_P00().numpy())
@@ -431,21 +541,19 @@
     
     def eval(self, image1, image2=None,mask=None,Auto=True,s0_off=1E-6):
         # Check input consistency
         if not isinstance(image1,Rformat.Rformat):
             if image2 is not None and not isinstance(image2,Rformat.Rformat):
                 if list(image1.shape)!=list(image2.shape):
                     print('The two input image should have the same size to eval Scattering')
-                    traceback.print_exc()
                     
                     exit(0)
             if mask is not None:
                 if list(image1.shape)!=list(mask.shape)[1:]:
                     print('The mask should have the same size than the input image to eval Scattering')
-                    traceback.print_exc()
                     exit(0)
             
         ### AUTO OR CROSS
         cross = False
         if image2 is not None:
             cross = True
             all_cross=not Auto
```

### Comparing `foscat-2.0.7/src/foscat/scat_cov.old.py` & `foscat-2.1.0/src/foscat/scat_cov.old.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.7/src/foscat/scat_cov.py` & `foscat-2.1.0/src/foscat/scat_cov.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import foscat.FoCUS as FOC
 import numpy as np
 import foscat.backend as bk
 import foscat.Rformat as Rformat
-import traceback
 
 def read(filename):
     thescat = scat_cov(1, 1, 1)
     return thescat.read(filename)
 
 testwarn=0
 
@@ -440,31 +439,43 @@
         j1,j2=self.get_j_idx()
         
         if hold:
             plt.figure(figsize=(16, 8))
 
         if self.S1 is not None:
             plt.subplot(2, 2, 1)
-            if legend:
-                plt.plot(abs(self.get_np(self.S1)).flatten(), color=color, label=r'%s $S_1$' % (name), lw=lw)
-            else:
-                plt.plot(abs(self.get_np(self.S1)).flatten(), color=color, lw=lw)
+            tmp=abs(self.get_np(self.S1))
+            test=None
+            for k in range(tmp.shape[3]):
+                for i1 in range(tmp.shape[0]):
+                    for i2 in range(tmp.shape[0]):
+                        if test is None:
+                            test=1
+                            plt.plot(tmp[i1,i2,:,k],color=color, label=r'%s $S_1$' % (name), lw=lw)
+                        else:
+                            plt.plot(tmp[i1,i2,:,k],color=color, lw=lw)
             plt.yscale('log')
             plt.legend()
             plt.ylabel('S1')
             plt.xlabel(r'$j_{1},\Theta_{1}$')
 
+        test=None
         plt.subplot(2, 2, 2)
-        if legend:
-            plt.plot(abs(self.get_np(self.P00)).flatten(), color=color, label=r'%s $P_{00}$' % (name), lw=lw)
-        else:
-            plt.plot(abs(self.get_np(self.P00)).flatten(), color=color, lw=lw)
+        tmp=abs(self.get_np(self.P00))
+        for k in range(tmp.shape[3]):
+            for i1 in range(tmp.shape[0]):
+                for i2 in range(tmp.shape[0]):
+                    if test is None:
+                        test=1
+                        plt.plot(tmp[i1,i2,:,k],color=color, label=r'%s $P_{00}$' % (name), lw=lw)
+                    else:
+                        plt.plot(tmp[i1,i2,:,k],color=color, lw=lw)
         plt.yscale('log')
         plt.ylabel('P00')
-        plt.xlabel(r'$j_{1},\Theta_{1}$')
+        plt.xlabel(r'$j_{1}$')
         plt.legend()
 
         ax1=plt.subplot(2, 2, 3)
         ax2 = ax1.twiny()
         n=0
         tmp=abs(self.get_np(self.C01))
         lname=r'%s $C_{01}$' % (name)
@@ -856,20 +867,18 @@
         S1, P00, C01, C11 normalized
         """
         # Check input consistency
         if not isinstance(image1,Rformat.Rformat):
             if image2 is not None and not isinstance(image2,Rformat.Rformat):
                 if list(image1.shape)!=list(image2.shape):
                     print('The two input image should have the same size to eval Scattering Covariance')
-                    traceback.print_exc()
                     exit(0)
             if mask is not None:
                 if list(image1.shape)!=list(mask.shape)[1:]:
                     print('The mask should have the same size than the input image to eval Scattering Covariance')
-                    traceback.print_exc()
                     exit(0)
 
         ### AUTO OR CROSS
         cross = False
         if image2 is not None:
             cross = True
             all_cross=Auto
```

### Comparing `foscat-2.0.7/src/foscat/scat_cov_new.py` & `foscat-2.1.0/src/foscat/scat_cov_new.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.7/src/foscat.egg-info/PKG-INFO` & `foscat-2.1.0/src/foscat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.0.7
+Version: 2.1.0
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

