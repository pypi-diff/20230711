# Comparing `tmp/foscat-2.0.6.tar.gz` & `tmp/foscat-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-wu5frbmz/foscat-2.0.6.tar", last modified: Tue Jul 11 08:18:10 2023, max compression
+gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-pba4exkf/foscat-2.0.7.tar", last modified: Tue Jul 11 13:14:57 2023, max compression
```

## Comparing `foscat-2.0.6.tar` & `foscat-2.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 08:18:10.000000 foscat-2.0.6/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-11 08:18:10.000000 foscat-2.0.6/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2023-07-11 08:17:35.000000 foscat-2.0.6/README.md
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-07-11 08:18:10.000000 foscat-2.0.6/setup.cfg
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-07-11 08:17:47.000000 foscat-2.0.6/setup.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 08:18:10.000000 foscat-2.0.6/src/
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 08:18:10.000000 foscat-2.0.6/src/foscat/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57132 2023-06-10 06:53:35.000000 foscat-2.0.6/src/foscat/FoCUS.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.0.6/src/foscat/GetGPUinfo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     3594 2023-06-23 10:27:41.000000 foscat-2.0.6/src/foscat/Rformat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    16435 2023-07-10 14:25:03.000000 foscat-2.0.6/src/foscat/Synthesis.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.0.6/src/foscat/__init__.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    13733 2023-06-10 06:53:35.000000 foscat-2.0.6/src/foscat/backend.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.0.6/src/foscat/build_demo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.0.6/src/foscat/demo2d.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    29191 2023-07-11 07:38:44.000000 foscat-2.0.6/src/foscat/scat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.0.6/src/foscat/scat_cov.old.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    48501 2023-07-11 07:42:05.000000 foscat-2.0.6/src/foscat/scat_cov.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.0.6/src/foscat/scat_cov_new.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 08:18:10.000000 foscat-2.0.6/src/foscat.egg-info/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-11 08:18:10.000000 foscat-2.0.6/src/foscat.egg-info/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-07-11 08:18:10.000000 foscat-2.0.6/src/foscat.egg-info/SOURCES.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-07-11 08:18:10.000000 foscat-2.0.6/src/foscat.egg-info/dependency_links.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-07-11 08:18:10.000000 foscat-2.0.6/src/foscat.egg-info/requires.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-07-11 08:18:10.000000 foscat-2.0.6/src/foscat.egg-info/top_level.txt
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 13:14:57.000000 foscat-2.0.7/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-11 13:14:57.000000 foscat-2.0.7/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2023-07-11 08:17:35.000000 foscat-2.0.7/README.md
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-07-11 13:14:57.000000 foscat-2.0.7/setup.cfg
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-07-11 13:14:26.000000 foscat-2.0.7/setup.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 13:14:57.000000 foscat-2.0.7/src/
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 13:14:57.000000 foscat-2.0.7/src/foscat/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57626 2023-07-11 10:02:58.000000 foscat-2.0.7/src/foscat/FoCUS.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.0.7/src/foscat/GetGPUinfo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     3594 2023-06-23 10:27:41.000000 foscat-2.0.7/src/foscat/Rformat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    16435 2023-07-10 14:25:03.000000 foscat-2.0.7/src/foscat/Synthesis.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.0.7/src/foscat/__init__.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    13733 2023-06-10 06:53:35.000000 foscat-2.0.7/src/foscat/backend.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.0.7/src/foscat/build_demo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.0.7/src/foscat/demo2d.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    29274 2023-07-11 08:46:53.000000 foscat-2.0.7/src/foscat/scat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.0.7/src/foscat/scat_cov.old.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53642 2023-07-11 10:46:11.000000 foscat-2.0.7/src/foscat/scat_cov.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.0.7/src/foscat/scat_cov_new.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-11 13:14:57.000000 foscat-2.0.7/src/foscat.egg-info/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-11 13:14:57.000000 foscat-2.0.7/src/foscat.egg-info/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-07-11 13:14:57.000000 foscat-2.0.7/src/foscat.egg-info/SOURCES.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-07-11 13:14:57.000000 foscat-2.0.7/src/foscat.egg-info/dependency_links.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-07-11 13:14:57.000000 foscat-2.0.7/src/foscat.egg-info/requires.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-07-11 13:14:57.000000 foscat-2.0.7/src/foscat.egg-info/top_level.txt
```

### Comparing `foscat-2.0.6/PKG-INFO` & `foscat-2.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.0.6
+Version: 2.0.7
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

### Comparing `foscat-2.0.6/README.md` & `foscat-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `foscat-2.0.6/setup.py` & `foscat-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='foscat',
-    version='2.0.6',
+    version='2.0.7',
     description='Generate synthetic Healpix or 2D data using Cross Scattering Transform' ,
     long_description='Utilize the Cross Scattering Transform (described in https://arxiv.org/abs/2207.12527) to synthesize Healpix or 2D data that is suitable for component separation purposes, such as denoising. \n A demo package for this process can be found at https://github.com/jmdelouis/FOSCAT_DEMO. \n\n List of developers : J.-M. Delouis, T. Foulquier, L. Mousset, E. Allys ' ,
     license='MIT',
     author='Jean-Marc DELOUIS',
     author_email='jean.marc.delouis@ifremer.fr',
     maintainer='Theo Foulquier',
     maintainer_email='theo.foulquier@ifremer.fr',
```

### Comparing `foscat-2.0.6/src/foscat/FoCUS.py` & `foscat-2.0.7/src/foscat/FoCUS.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,21 +11,22 @@
                  LAMBDA=1.2,
                  KERNELSZ=3,
                  slope=1.0,
                  all_type='float64',
                  nstep_max=16,
                  padding='SAME',
                  gpupos=0,
-                 healpix=True,
                  OSTEP=0,
                  isMPI=False,
                  TEMPLATE_PATH='data',
                  BACKEND='tensorflow',
                  use_R_format=True,
                  chans=12,
+                 Healpix=True,
+                 JmaxDelta=0,
                  DODIV=False,
                  mpi_size=1,
                  mpi_rank=0):
 
         # P00 coeff for normalization for scat_cov
         self.P1_dic = None
         self.P2_dic = None
@@ -51,21 +52,37 @@
                 
         self.number_of_loss=0
 
         self.history=np.zeros([10])
         self.nlog=0
         
         self.padding=padding
-        self.healpix=healpix
-        if OSTEP<-1:
-            print('Warning : OSTEP can not be smaller than -1')
+            
+        if OSTEP!=0:
+            print('OPTION option is deprecated after version 2.0.6. Please use Jmax option')
+            JmaxDelta=OSTEP
+        else:
+            OSTEP=JmaxDelta
+            
+        if JmaxDelta<-1:
+            print('Warning : Jmax can not be smaller than -1')
             exit(0)
             
-        self.OSTEP=OSTEP
+        self.OSTEP=JmaxDelta
         self.use_R_format=use_R_format
+        
+        if chans!=12:
+            print('chans option is deprecated after version 2.0.6. Please use Healpix option')
+            if chans==1:
+                Healpix=False
+        if Healpix==False:
+            chans=1
+        else:
+            chans=12
+            
         self.chans=chans
         
         if isMPI:
             from mpi4py import MPI
 
             self.comm= MPI.COMM_WORLD
             if all_type=='float32':
```

### Comparing `foscat-2.0.6/src/foscat/GetGPUinfo.py` & `foscat-2.0.7/src/foscat/GetGPUinfo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.6/src/foscat/Rformat.py` & `foscat-2.0.7/src/foscat/Rformat.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.6/src/foscat/Synthesis.py` & `foscat-2.0.7/src/foscat/Synthesis.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.6/src/foscat/backend.py` & `foscat-2.0.7/src/foscat/backend.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.6/src/foscat/build_demo.py` & `foscat-2.0.7/src/foscat/build_demo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.6/src/foscat/scat.py` & `foscat-2.0.7/src/foscat/scat.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,14 +233,16 @@
             y=tmp
         
         return(y)
     
     def plot(self,name=None,hold=True,color='blue',lw=1,legend=True):
 
         import matplotlib.pyplot as plt
+
+        j1,j2=self.get_j_idx()
         
         if name is None:
             name=''
 
         if hold:
             plt.figure(figsize=(8,8))
         
@@ -259,14 +261,15 @@
             plt.plot(self.l1_abs(self.P00).flatten(),color=color,label=r'%s $P_{00}$'%(name),lw=lw)
         else:
             plt.plot(abs(self.l1_abs(self.P00).flatten()),':',color=color,lw=lw)
             plt.plot(self.l1_abs(self.P00).flatten(),color=color,lw=lw)
         plt.yscale('log')
         plt.legend()
         plt.subplot(2,2,3)
+        print(self.l1_abs(self.S2).shape,j1.shape)
         if legend:
             plt.plot(abs(self.l1_abs(self.S2).flatten()),':',color=color,lw=lw)
             plt.plot(self.l1_abs(self.S2).flatten(),color=color,label=r'%s $S_2$ L1 norm'%(name),lw=lw)
         else:
             plt.plot(abs(self.l1_abs(self.S2).flatten()),':',color=color,lw=lw)
             plt.plot(self.l1_abs(self.S2).flatten(),color=color,lw=lw)
         plt.yscale('log')
```

### Comparing `foscat-2.0.6/src/foscat/scat_cov.old.py` & `foscat-2.0.7/src/foscat/scat_cov.old.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.6/src/foscat/scat_cov.py` & `foscat-2.0.7/src/foscat/scat_cov.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import foscat.Rformat as Rformat
 import traceback
 
 def read(filename):
     thescat = scat_cov(1, 1, 1)
     return thescat.read(filename)
 
-
 testwarn=0
 
 class scat_cov:
     def __init__(self, p00, c01, c11, s1=None, c10=None,backend=None):
         self.P00     = p00
         self.C01     = c01
         self.C11     = c11
@@ -63,14 +62,31 @@
         for i in range(nscale):
             for j in range(i):
                 j1[n]=j
                 j2[n]=i
                 n=n+1
         return(j1,j2)
     
+    def get_jc11_idx(self):
+        shape=list(self.P00.shape)
+        nscale=shape[2]
+        n=nscale*(nscale-1)*(nscale-2)
+        j1=np.zeros([n*2],dtype='int')
+        j2=np.zeros([n*2],dtype='int')
+        j3=np.zeros([n*2],dtype='int')
+        n=0
+        for i in range(nscale):
+            for j in range(i):
+                for k in range(j):
+                    j1[n]=k
+                    j2[n]=j
+                    j3[n]=i
+                    n=n+1
+        return(j1[0:n],j2[0:n],j3[0:n])
+    
     def __add__(self, other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
                isinstance(other, bool) or isinstance(other, scat_cov)
 
         if self.S1 is None:
             s1 = None
         else:
@@ -417,53 +433,166 @@
     def plot(self, name=None, hold=True, color='blue', lw=1, legend=True):
 
         import matplotlib.pyplot as plt
 
         if name is None:
             name = ''
 
+        j1,j2=self.get_j_idx()
+        
         if hold:
-            plt.figure(figsize=(8, 8))
+            plt.figure(figsize=(16, 8))
 
         if self.S1 is not None:
             plt.subplot(2, 2, 1)
             if legend:
                 plt.plot(abs(self.get_np(self.S1)).flatten(), color=color, label=r'%s $S_1$' % (name), lw=lw)
             else:
                 plt.plot(abs(self.get_np(self.S1)).flatten(), color=color, lw=lw)
             plt.yscale('log')
             plt.legend()
+            plt.ylabel('S1')
+            plt.xlabel(r'$j_{1},\Theta_{1}$')
 
         plt.subplot(2, 2, 2)
         if legend:
             plt.plot(abs(self.get_np(self.P00)).flatten(), color=color, label=r'%s $P_{00}$' % (name), lw=lw)
         else:
             plt.plot(abs(self.get_np(self.P00)).flatten(), color=color, lw=lw)
         plt.yscale('log')
+        plt.ylabel('P00')
+        plt.xlabel(r'$j_{1},\Theta_{1}$')
         plt.legend()
 
-        plt.subplot(2, 2, 3)
-        if legend:
-            plt.plot(abs(self.get_np(self.C01)).flatten(), color=color, label=r'%s $C_{01}$' % (name), lw=lw)
-            if self.C10 is not None:
-                plt.plot(abs(self.get_np(self.C10)).flatten(), color=color, label=r'%s $C_{10}$' % (name), lw=lw)
-        else:
-            plt.plot(abs(self.get_np(self.C01)).flatten(), color=color, lw=lw)
-            if self.C10 is not None:
-                plt.plot(abs(self.get_np(self.C10)).flatten(), color=color, lw=lw)
+        ax1=plt.subplot(2, 2, 3)
+        ax2 = ax1.twiny()
+        n=0
+        tmp=abs(self.get_np(self.C01))
+        lname=r'%s $C_{01}$' % (name)
+        ax1.set_ylabel(r'$C_{01}$')
+        if self.C10 is not None:
+            tmp=abs(self.get_np(self.C01))
+            lname=r'%s $C_{10}$' % (name)
+            ax1.set_ylabel(r'$C_{10}$')
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
-
-        plt.subplot(2, 2, 4)
-        if legend:
-            plt.plot(abs(self.get_np(self.C11)).flatten(), color=color, label=r'%s $C_{11}$' % (name), lw=lw)
-        else:
-            plt.plot(abs(self.get_np(self.C11)).flatten(), color=color, lw=lw)
+        ax1.set_xlim(0,n+2)
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
+        ax2.set_xlim(0,n+2)
+        ax2.set_xticks(tab2x)
+        ax2.set_xticklabels(tab2nx,fontsize=6)
+        ax2.set_xlabel(r"$j_{1}$",fontsize=6)
+        ax1.legend(frameon=0)
+
+        ax1=plt.subplot(2, 2, 4)
+        j1,j2,j3=self.get_jc11_idx()
+        ax2 = ax1.twiny()
+        n=1
+        tmp=abs(self.get_np(self.C11))
+        lname=r'%s $C_{11}$' % (name)
+        test=None
+        tabx=[]
+        tabnx=[]
+        tab2x=[]
+        tab2nx=[]
+        for i0 in range(tmp.shape[0]):
+            for i1 in range(tmp.shape[1]):
+                for i2 in range(j1.max()+1):
+                    nprev=n
+                    for i2b in range(j2[j1==i2].max()+1):
+                        idx=np.where((j1==i2)*(j2==i2b))[0]
+                        for i3 in range(tmp.shape[3]):
+                            for i4 in range(tmp.shape[4]):
+                                for i5 in range(tmp.shape[5]):
+                                    if len(idx)==1:
+                                        ax1.plot(np.arange(len(idx))+n,tmp[i0,i1,idx,i3,i4,i5],'.', \
+                                                 color=color, lw=lw)
+                                    else:
+                                        if legend and test is None:
+                                            ax1.plot(np.arange(len(idx))+n,tmp[i0,i1,idx,i3,i4,i5], \
+                                                     color=color, label=lname, lw=lw)
+                                            test=1
+                                        ax1.plot(np.arange(len(idx))+n,tmp[i0,i1,idx,i3,i4,i5], \
+                                                 color=color, lw=lw)
+                        tabnx=tabnx+[r'%d,%d'%(j2[k],j3[k]) for k in idx]
+                        tabx=tabx+[k+n for k in range(len(idx))]
+                        n=n+idx.shape[0]
+                    tab2x=tab2x+[(n+nprev-1)/2]
+                    tab2nx=tab2nx+['%d'%(i2)]
+                    ax1.axvline(n-0.5,ls=':',color='gray') 
         plt.yscale('log')
-        plt.legend()
+        ax1.set_ylabel(r'$C_{11}$')
+        ax1.set_xticks(tabx)
+        ax1.set_xticklabels(tabnx,fontsize=6)
+        ax1.set_xlabel(r"$j_{2},j_{3}$",fontsize=6)
+        ax1.set_xlim(0,n)
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
+        ax2.set_xlim(0,n)
+        ax2.set_xticks(tab2x)
+        ax2.set_xticklabels(tab2nx,fontsize=6)
+        ax2.set_xlabel(r"$j_{1}$",fontsize=6)
+        ax1.legend(frameon=0)
 
     def get_np(self, x):
         if x is not None:
             if isinstance(x, np.ndarray):
                 return x
             else:
                 return x.numpy()
```

### Comparing `foscat-2.0.6/src/foscat/scat_cov_new.py` & `foscat-2.0.7/src/foscat/scat_cov_new.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.6/src/foscat.egg-info/PKG-INFO` & `foscat-2.0.7/src/foscat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.0.6
+Version: 2.0.7
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

