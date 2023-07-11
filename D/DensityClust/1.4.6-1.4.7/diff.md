# Comparing `tmp/DensityClust-1.4.6.tar.gz` & `tmp/DensityClust-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DensityClust-1.4.6.tar", last modified: Tue Jun 27 13:38:55 2023, max compression
+gzip compressed data, was "DensityClust-1.4.7.tar", last modified: Tue Jul 11 07:43:16 2023, max compression
```

## Comparing `DensityClust-1.4.6.tar` & `DensityClust-1.4.7.tar`

### file list

```diff
@@ -1,39 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 13:38:55.490597 DensityClust-1.4.6/
-drwxrwxrwx   0        0        0        0 2023-06-27 13:38:55.468654 DensityClust-1.4.6/DensityClust/
--rw-rw-rw-   0        0        0     7105 2023-06-23 10:21:24.000000 DensityClust-1.4.6/DensityClust/LocalDensityClustering_main.py
--rw-rw-rw-   0        0        0        0 2023-06-23 11:05:30.000000 DensityClust-1.4.6/DensityClust/__init__.py
--rw-rw-rw-   0        0        0    29426 2023-06-23 04:03:04.000000 DensityClust-1.4.6/DensityClust/clustring_subfunc.py
--rw-rw-rw-   0        0        0    51177 2023-06-27 12:06:09.000000 DensityClust-1.4.6/DensityClust/localDenClust2.py
--rw-rw-rw-   0        0        0    11964 2023-06-23 04:03:04.000000 DensityClust-1.4.6/DensityClust/split_cube.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:38:55.475637 DensityClust-1.4.6/DensityClust.egg-info/
--rw-rw-rw-   0        0        0      377 2023-06-27 13:38:55.000000 DensityClust-1.4.6/DensityClust.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      778 2023-06-27 13:38:55.000000 DensityClust-1.4.6/DensityClust.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 13:38:55.000000 DensityClust-1.4.6/DensityClust.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-06-27 13:38:55.000000 DensityClust-1.4.6/DensityClust.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 13:38:55.478628 DensityClust-1.4.6/Generate/
--rw-rw-rw-   0        0        0     3381 2023-06-23 04:03:04.000000 DensityClust-1.4.6/Generate/fits_header.py
--rw-rw-rw-   0        0        0    15795 2023-06-23 04:03:04.000000 DensityClust-1.4.6/Generate/generate.py
--rw-rw-rw-   0        0        0    13320 2023-06-23 04:03:04.000000 DensityClust-1.4.6/Generate/synthetic_data.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:38:55.480623 DensityClust-1.4.6/LDC_MGM_main/
--rw-rw-rw-   0        0        0     7159 2023-06-23 11:10:39.000000 DensityClust-1.4.6/LDC_MGM_main/LDC_MGM_main.py
--rw-rw-rw-   0        0        0     1329 2023-06-23 11:10:39.000000 DensityClust-1.4.6/LDC_MGM_main/LDC_mian.py
--rw-rw-rw-   0        0        0        0 2023-06-23 04:03:04.000000 DensityClust-1.4.6/LDC_MGM_main/__init__.py
--rw-rw-rw-   0        0        0      377 2023-06-27 13:38:55.489599 DensityClust-1.4.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 13:38:55.483615 DensityClust-1.4.6/fit_clump_function/
--rw-rw-rw-   0        0        0        0 2023-06-23 04:03:04.000000 DensityClust-1.4.6/fit_clump_function/__init__.py
--rw-rw-rw-   0        0        0     9322 2023-06-23 04:03:04.000000 DensityClust-1.4.6/fit_clump_function/main_fit_gauss_3d.py
--rw-rw-rw-   0        0        0    26027 2023-06-27 13:27:49.000000 DensityClust-1.4.6/fit_clump_function/multi_gauss_fitting_new.py
--rw-rw-rw-   0        0        0    11936 2023-06-23 04:03:04.000000 DensityClust-1.4.6/fit_clump_function/touch_clump.py
--rw-rw-rw-   0        0        0       42 2023-06-27 13:38:55.490597 DensityClust-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0      507 2023-06-27 13:38:51.000000 DensityClust-1.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:38:55.484612 DensityClust-1.4.6/t_match/
-drwxrwxrwx   0        0        0        0 2023-06-27 13:38:55.485610 DensityClust-1.4.6/t_match/.idea/
--rw-rw-rw-   0        0        0      291 2023-06-23 04:03:04.000000 DensityClust-1.4.6/t_match/.idea/t_match.iml
--rw-rw-rw-   0        0        0        0 2023-06-23 04:03:04.000000 DensityClust-1.4.6/t_match/__init__.py
--rw-rw-rw-   0        0        0    24986 2023-06-23 04:03:04.000000 DensityClust-1.4.6/t_match/match_6_.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:38:55.489599 DensityClust-1.4.6/tools/
--rw-rw-rw-   0        0        0        0 2023-06-23 04:03:04.000000 DensityClust-1.4.6/tools/__init__.py
--rw-rw-rw-   0        0        0     7193 2023-06-23 04:03:04.000000 DensityClust-1.4.6/tools/data_merge.py
--rw-rw-rw-   0        0        0     8962 2023-06-23 04:03:04.000000 DensityClust-1.4.6/tools/make_plot.py
--rw-rw-rw-   0        0        0    14792 2023-06-23 04:03:04.000000 DensityClust-1.4.6/tools/show_clumps.py
--rw-rw-rw-   0        0        0    12625 2023-06-23 04:03:04.000000 DensityClust-1.4.6/tools/ultil_lxy.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:43:16.687481 DensityClust-1.4.7/
+drwxrwxrwx   0        0        0        0 2023-07-11 07:43:16.075513 DensityClust-1.4.7/DensityClust/
+-rw-rw-rw-   0        0        0     7130 2023-07-11 03:19:44.000000 DensityClust-1.4.7/DensityClust/LocalDensityClustering_main.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 11:05:30.000000 DensityClust-1.4.7/DensityClust/__init__.py
+-rw-rw-rw-   0        0        0    29426 2023-06-23 04:03:04.000000 DensityClust-1.4.7/DensityClust/clustring_subfunc.py
+-rw-rw-rw-   0        0        0    51046 2023-07-11 03:19:44.000000 DensityClust-1.4.7/DensityClust/localDenClust2.py
+-rw-rw-rw-   0        0        0    11996 2023-07-11 03:19:44.000000 DensityClust-1.4.7/DensityClust/split_cube.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:43:16.156750 DensityClust-1.4.7/DensityClust.egg-info/
+-rw-rw-rw-   0        0        0      377 2023-07-11 07:43:15.000000 DensityClust-1.4.7/DensityClust.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1609 2023-07-11 07:43:15.000000 DensityClust-1.4.7/DensityClust.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 07:43:15.000000 DensityClust-1.4.7/DensityClust.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-07-11 07:43:15.000000 DensityClust-1.4.7/DensityClust.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 07:43:16.206462 DensityClust-1.4.7/Generate/
+-rw-rw-rw-   0        0        0     4843 2023-06-23 04:03:04.000000 DensityClust-1.4.7/Generate/README.md
+-rw-rw-rw-   0        0        0        0 2023-07-11 07:02:25.000000 DensityClust-1.4.7/Generate/__init__.py
+-rw-rw-rw-   0        0        0     3381 2023-06-23 04:03:04.000000 DensityClust-1.4.7/Generate/fits_header.py
+-rw-rw-rw-   0        0        0   282240 2023-06-23 04:03:04.000000 DensityClust-1.4.7/Generate/gauss_outcat_m16_13_ellipse.FIT
+-rw-rw-rw-   0        0        0    15795 2023-06-23 04:03:04.000000 DensityClust-1.4.7/Generate/generate.py
+-rw-rw-rw-   0        0        0   871433 2023-06-23 04:03:04.000000 DensityClust-1.4.7/Generate/sample_data.txt
+-rw-rw-rw-   0        0        0    13320 2023-06-23 04:03:04.000000 DensityClust-1.4.7/Generate/synthetic_data.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:43:16.340222 DensityClust-1.4.7/LDC_MGM_main/
+-rw-rw-rw-   0        0        0     7207 2023-07-11 03:19:45.000000 DensityClust-1.4.7/LDC_MGM_main/LDC_MGM_main.py
+-rw-rw-rw-   0        0        0     1337 2023-07-11 03:19:45.000000 DensityClust-1.4.7/LDC_MGM_main/LDC_mian.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 04:03:04.000000 DensityClust-1.4.7/LDC_MGM_main/__init__.py
+-rw-rw-rw-   0        0        0     2457 2023-06-23 04:03:04.000000 DensityClust-1.4.7/LDC_MGM_main/readme.md
+-rw-rw-rw-   0        0        0      377 2023-07-11 07:43:16.681953 DensityClust-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-11 03:19:11.000000 DensityClust-1.4.7/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:43:16.435822 DensityClust-1.4.7/fit_clump_function/
+-rw-rw-rw-   0        0        0     1351 2023-06-23 04:03:04.000000 DensityClust-1.4.7/fit_clump_function/README.md
+-rw-rw-rw-   0        0        0        0 2023-06-23 04:03:04.000000 DensityClust-1.4.7/fit_clump_function/__init__.py
+-rw-rw-rw-   0        0        0     9386 2023-07-11 03:19:44.000000 DensityClust-1.4.7/fit_clump_function/main_fit_gauss_3d.py
+-rw-rw-rw-   0        0        0    26027 2023-06-27 13:27:49.000000 DensityClust-1.4.7/fit_clump_function/multi_gauss_fitting_new.py
+-rw-rw-rw-   0        0        0    11936 2023-06-23 04:03:04.000000 DensityClust-1.4.7/fit_clump_function/touch_clump.py
+-rw-rw-rw-   0        0        0  1043012 2023-06-23 04:03:04.000000 DensityClust-1.4.7/fit_clump_function/参数还原实验记录.pdf
+-rw-rw-rw-   0        0        0       42 2023-07-11 07:43:16.688480 DensityClust-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-07-11 03:22:41.000000 DensityClust-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:43:16.452345 DensityClust-1.4.7/t_match/
+drwxrwxrwx   0        0        0        0 2023-07-11 07:43:16.547079 DensityClust-1.4.7/t_match/.idea/
+-rw-rw-rw-   0        0        0       50 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/.idea/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-11 07:43:16.573316 DensityClust-1.4.7/t_match/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      179 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      197 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/.idea/misc.xml
+-rw-rw-rw-   0        0        0      273 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/.idea/modules.xml
+-rw-rw-rw-   0        0        0      291 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/.idea/t_match.iml
+-rw-rw-rw-   0        0        0        0 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:43:16.613088 DensityClust-1.4.7/t_match/data/
+-rw-rw-rw-   0        0        0    15067 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/data/detected_outcat.txt
+-rw-rw-rw-   0        0        0    43200 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/data/gaussclumps_outcat_000.FIT
+-rw-rw-rw-   0        0        0    57600 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/data/gaussclumps_outcat_099.FIT
+-rw-rw-rw-   0        0        0    40320 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/data/s_outcat_000.FIT
+-rw-rw-rw-   0        0        0    57600 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/data/s_outcat_099.FIT
+-rw-rw-rw-   0        0        0    29033 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/data/simulated_outcat_000.txt
+-rw-rw-rw-   0        0        0    24986 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/match_6_.py
+drwxrwxrwx   0        0        0        0 2023-07-11 07:43:16.625160 DensityClust-1.4.7/t_match/match_result/
+-rw-rw-rw-   0        0        0     1671 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/match_result/False_0000.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 07:43:16.633681 DensityClust-1.4.7/t_match/match_result/False_table/
+-rw-rw-rw-   0        0        0     1671 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/match_result/False_table/False_000.txt
+-rw-rw-rw-   0        0        0    30927 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/match_result/Match_0000.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 07:43:16.638709 DensityClust-1.4.7/t_match/match_result/Match_table/
+-rw-rw-rw-   0        0        0    30927 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/match_result/Match_table/Match_000.txt
+-rw-rw-rw-   0        0        0     4986 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/match_result/Miss_0000.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 07:43:16.648292 DensityClust-1.4.7/t_match/match_result/Miss_table/
+-rw-rw-rw-   0        0        0     4986 2023-06-23 04:03:04.000000 DensityClust-1.4.7/t_match/match_result/Miss_table/Miss_000.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 07:43:16.677959 DensityClust-1.4.7/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-23 04:03:04.000000 DensityClust-1.4.7/tools/__init__.py
+-rw-rw-rw-   0        0        0     7193 2023-06-23 04:03:04.000000 DensityClust-1.4.7/tools/data_merge.py
+-rw-rw-rw-   0        0        0    15344 2023-07-11 06:57:58.000000 DensityClust-1.4.7/tools/identify_plot_711.py
+-rw-rw-rw-   0        0        0     8946 2023-07-11 03:19:45.000000 DensityClust-1.4.7/tools/make_plot.py
+-rw-rw-rw-   0        0        0    14857 2023-07-11 06:06:11.000000 DensityClust-1.4.7/tools/show_clumps.py
+-rw-rw-rw-   0        0        0    12641 2023-07-11 03:19:45.000000 DensityClust-1.4.7/tools/ultil_lxy.py
```

### Comparing `DensityClust-1.4.6/DensityClust/LocalDensityClustering_main.py` & `DensityClust-1.4.7/DensityClust/LocalDensityClustering_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import shutil
 import pandas as pd
-from DensityClust.localDenClust2 import LocalDensityCluster as LDC
-from DensityClust import split_cube
-from tools.show_clumps import make_plot_wcs_1
-from DensityClust.localDenClust2 import Data, Param
+from distrib.DensityClust.localDenClust2 import LocalDensityCluster as LDC
+from distrib.DensityClust import split_cube
+from distrib.tools.show_clumps import make_plot_wcs_1
+from distrib.DensityClust.localDenClust2 import Data
 
 
 def localDenCluster(data_name, para, save_folder):
     """
     LDC algorithm
 
     :param data_name: 待检测数据的路径(str)，fits文件
```

### Comparing `DensityClust-1.4.6/DensityClust/clustring_subfunc.py` & `DensityClust-1.4.7/DensityClust/clustring_subfunc.py`

 * *Files identical despite different names*

### Comparing `DensityClust-1.4.6/DensityClust/localDenClust2.py` & `DensityClust-1.4.7/DensityClust/localDenClust2.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from skimage import filters, measure
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import time
 import tqdm
 
-from DensityClust.clustring_subfunc import get_xyz, my_print, get_area_v_len, get_clump_angle
-from DensityClust.clustring_subfunc import assignation, divide_boundary_by_grad
+from distrib.DensityClust.clustring_subfunc import get_xyz, my_print, get_area_v_len, get_clump_angle
+from distrib.DensityClust.clustring_subfunc import assignation, divide_boundary_by_grad
 from Generate.fits_header import Header
 
 
 """
 1.4.0 2022/11/04
 """
 
@@ -872,15 +872,15 @@
             LDC_outcat = np.column_stack((id_clumps, clump_Peak123.T[:, ::-1], clump_Cen.T, clump_Size.T, clump_Peak.T,
                                           clump_Sum.T, clump_Volume.T, clump_Angle.T))
 
             LDC_outcat = pd.DataFrame(LDC_outcat, columns=table_title)
             self.result.detect_num[0] = LDC_outcat.shape[0]
             if self.para.rm_touch_edge:
                 LDC_outcat, label_data_all = self.touch_edge(LDC_outcat, label_data_all)
-                self.result.detect_num[1] = LDC_outcat.shape[0]
+            self.result.detect_num[1] = LDC_outcat.shape[0]
 
             if self.para.save_loc:
                 loc_LDC_outcat = self.get_outcat_local(LDC_outcat)
                 self.result.detect_num[2] = loc_LDC_outcat.shape[0]
                 self.result.loc_outcat = loc_LDC_outcat
                 self.result.loc_outcat_wcs = self.change_pix2world(loc_LDC_outcat, id_prefix=self.para.id_prefix)
 
@@ -968,18 +968,15 @@
 
     def touch_edge(self, outcat, label_data_all):
         """
         判断云核是否到达边界
         :param outcat:
         :return:
         """
-        # data_name = r'F:\DensityClust_distribution_class\DensityClust\m16_denoised.fits'
-        # outcat_name = r'F:\DensityClust_distribution_class\DensityClust\m16_denoised\LDC_outcat.txt'
-        # data = fits.getdata(data_name)
-        # outcat_record = pd.read_csv(outcat_name, sep='\t')
+
         if self.data.n_dim == 3:
             [size_x, size_y, size_v] = self.data.data_cube.shape
             indx = []
 
             # condition 1: 峰值到达边界-->接触边界
             for item_peak, item_size in zip(['Peak1', 'Peak2', 'Peak3'], [size_v, size_y, size_x]):
                 indx.append(np.where(outcat[item_peak] == item_size)[0])
@@ -989,17 +986,17 @@
             for item_cen, item_size in zip([['Cen1', 'Size1'], ['Cen2', 'Size2'], ['Cen3', 'Size3']],
                                            [size_v, size_y, size_x]):
                 indx.append(np.where((outcat[item_cen[0]] + 2 / 2.3548 * outcat[item_cen[1]]) > item_size)[0])
                 indx.append(np.where((outcat[item_cen[0]] - 2 / 2.3548 * outcat[item_cen[1]]) < 1)[0])
 
             inde_all = []
             for item_ in indx:
-                [inde_all.append(item) for item in item_]
+                [inde_all.append(item) for item in item_]   # 索引是从0开始的，outcat 中的ID是从1开始的
 
-            inde_all = np.array(list(set(inde_all)))
+            inde_all = np.array(list(set(inde_all)))  # 去除重复
             label_data_all_ = label_data_all.copy()
         else:
             [size_x, size_y] = self.data.data_cube.shape
             indx = []
 
             for item_peak, item_size in zip(['Peak1', 'Peak2'], [size_y, size_x]):
                 indx.append(np.where(outcat[item_peak] == item_size)[0])
@@ -1013,18 +1010,19 @@
             inde_all = []
             for item_ in indx:
                 [inde_all.append(item) for item in item_]
 
             inde_all = np.array(list(set(inde_all)))
             label_data_all_ = label_data_all.copy()
         if inde_all.shape[0] > 0:
+            # TODO 这个地方可能会有问题
             for item_i in outcat.index[inde_all]:
-                label_data_all_[label_data_all == item_i] = 0
+                label_data_all_[label_data_all == (item_i + 1)] = 0
+                break
             outcat = outcat.drop(outcat.index[inde_all])
-
         else:
             outcat = outcat
         return outcat, label_data_all_
 
     def get_outcat_local(self, outcat, cen1_edge=None, cen2_edge=None, cen3_edge=None):
         """
         返回局部区域的检测结果：
```

### Comparing `DensityClust-1.4.6/DensityClust/split_cube.py` & `DensityClust-1.4.7/DensityClust/split_cube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
-from tools.show_clumps import make_plot_wcs_1
+from distrib.tools.show_clumps import make_plot_wcs_1
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from spectral_cube import SpectralCube
-from DensityClust.localDenClust2 import LocalDensityCluster as LDC
-from DensityClust.localDenClust2 import Data
-from t_match.match_6_ import match_simu_detect_new
+from distrib.DensityClust.localDenClust2 import LocalDensityCluster as LDC
+from distrib.DensityClust.localDenClust2 import Data
+from distrib.t_match.match_6_ import match_simu_detect_new
 
 
 split_list = [[0, 150, 0, 150], [0, 150, 90, 271], [0, 150, 210, 361],
               [90, 241, 0, 150], [90, 241, 90, 271], [90, 241, 210, 361]]
 
 
 def split_cube_lxy(data_path, save_folder_all):
```

### Comparing `DensityClust-1.4.6/Generate/fits_header.py` & `DensityClust-1.4.7/Generate/fits_header.py`

 * *Files identical despite different names*

### Comparing `DensityClust-1.4.6/Generate/generate.py` & `DensityClust-1.4.7/Generate/generate.py`

 * *Files identical despite different names*

### Comparing `DensityClust-1.4.6/Generate/synthetic_data.py` & `DensityClust-1.4.7/Generate/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `DensityClust-1.4.6/LDC_MGM_main/LDC_MGM_main.py` & `DensityClust-1.4.7/LDC_MGM_main/LDC_MGM_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import shutil
 import pandas as pd
-from DensityClust.localDenClust2 import LocalDensityCluster as LDC
-from DensityClust import split_cube
-from tools import show_clumps
-from DensityClust.localDenClust2 import Data, Param
-from DensityClust.LocalDensityClustering_main import localDenCluster
-from fit_clump_function import main_fit_gauss_3d as mgm
+from distrib.DensityClust.localDenClust2 import LocalDensityCluster as LDC
+from distrib.DensityClust import split_cube
+from distrib.tools import show_clumps
+from distrib.DensityClust.localDenClust2 import Data, Param
+from distrib.DensityClust.LocalDensityClustering_main import localDenCluster
+from distrib.fit_clump_function import main_fit_gauss_3d as mgm
 
 
 def LDC_MGM_split_mode(data_name, para, save_folder_all, save_mgm_png):
     """
     LDC algorithm
     :param data_name: 待检测数据的路径(str)，fits文件
     :param para: 算法参数，dict
```

### Comparing `DensityClust-1.4.6/LDC_MGM_main/LDC_mian.py` & `DensityClust-1.4.7/LDC_MGM_main/LDC_mian.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from DensityClust.LocalDensityClustering_main import localDenCluster
+from distrib.DensityClust.LocalDensityClustering_main import localDenCluster
 
 
 def LDC_main(data_name, para, save_folder=None):
     """
         LDC algorithm
         :param data_name: 待检测数据的路径(str)，fits文件
         :param para: 算法参数, dict
```

### Comparing `DensityClust-1.4.6/fit_clump_function/main_fit_gauss_3d.py` & `DensityClust-1.4.7/fit_clump_function/main_fit_gauss_3d.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import numpy as np
 import os
 import time
 import pandas as pd
 from tqdm import tqdm
 import threading
-from fit_clump_function import multi_gauss_fitting_new, touch_clump
-from tools.ultil_lxy import create_folder, get_points_by_clumps_id, move_csv_png, restruct_fitting_outcat,\
+from distrib.fit_clump_function import multi_gauss_fitting_new
+from distrib.fit_clump_function import touch_clump
+from distrib.tools.ultil_lxy import create_folder, get_points_by_clumps_id, move_csv_png, restruct_fitting_outcat,\
     get_save_clumps_xyv
-from tools import show_clumps
-from DensityClust.localDenClust2 import Data, Param
+from distrib.tools import show_clumps
+from distrib.DensityClust.localDenClust2 import Data
 
 
 def fitting_LDC_clumps(points_path, outcat_name, data_rms, thresh_num, save_png=False, ldc_mgm_path=None,
                        fitting_outcat_path=None):
     """
     对LDC的检测结果进行3维高斯拟合，保存分子云核的参数
     拟合核表 DataFrame格式
```

### Comparing `DensityClust-1.4.6/fit_clump_function/multi_gauss_fitting_new.py` & `DensityClust-1.4.7/fit_clump_function/multi_gauss_fitting_new.py`

 * *Files identical despite different names*

### Comparing `DensityClust-1.4.6/fit_clump_function/touch_clump.py` & `DensityClust-1.4.7/fit_clump_function/touch_clump.py`

 * *Files identical despite different names*

### Comparing `DensityClust-1.4.6/t_match/match_6_.py` & `DensityClust-1.4.7/t_match/match_6_.py`

 * *Files identical despite different names*

### Comparing `DensityClust-1.4.6/tools/data_merge.py` & `DensityClust-1.4.7/tools/data_merge.py`

 * *Files identical despite different names*

### Comparing `DensityClust-1.4.6/tools/make_plot.py` & `DensityClust-1.4.7/tools/make_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from matplotlib import pyplot as plt
-import pandas as pd
 from astropy.coordinates import SkyCoord
-import os
-from DensityClust.clustring_subfunc import *
-from DensityClust.clustring_subfunc import get_wcs
+from distrib.DensityClust.clustring_subfunc import *
+from distrib.DensityClust.clustring_subfunc import get_wcs
 
 
 plt.rcParams['xtick.direction'] = 'in'
 plt.rcParams['ytick.direction'] = 'in'
 plt.rcParams['xtick.top'] = 'True'
 plt.rcParams['ytick.right'] = 'True'
 plt.rcParams['xtick.color'] = 'red'
```

### Comparing `DensityClust-1.4.6/tools/show_clumps.py` & `DensityClust-1.4.7/tools/show_clumps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import astropy.io.fits as fits
 import pandas as pd
 import matplotlib.pyplot as plt
-from astropy import wcs
+from astropy.wcs import WCS
 import os
 import numpy as np
 from astropy.coordinates import SkyCoord
-from tools.ultil_lxy import get_data_points
+from distrib.tools.ultil_lxy import get_data_points
 
 
 plt.rcParams['xtick.direction'] = 'in'
 plt.rcParams['ytick.direction'] = 'in'
 plt.rcParams['xtick.color'] = 'red'
 plt.rcParams['ytick.color'] = 'red'
 
@@ -20,17 +20,21 @@
     :param data_name: fits文件
     :return:
     data_wcs
     """
     data_header = fits.getheader(data_name)
     keys = data_header.keys()
     key = [k for k in keys if k.endswith('4')]
-    [data_header.remove(k) for k in key]
-    data_header.remove('VELREF')
-    data_wcs = wcs.WCS(data_header)
+    try:
+        [data_header.remove(k) for k in key]
+        data_header.remove('VELREF')
+    except KeyError:
+        pass
+    data_wcs = WCS(data_header)
+
     return data_wcs
 
 
 def make_plot_11(data_mask_plot, spectrum_max, spectrum_mean, Cen3, Peak3, title_name, save_path):
 
     bottom_123 = 0.66
     pad = 0.005
@@ -307,15 +311,15 @@
         path_outcat_wcs = os.path.join(path_detect, 'LDC_outcat_wcs.csv')
 
     path_mask = os.path.join(path_detect, 'LDC_mask.fits')
     detect_log = os.path.join(path_detect, 'LDC_detect_log.txt')
     f = open(detect_log)
     file_name = [item for item in f.readlines() if item.count('fits')]
     f.close()
-    file_name = file_name[0].split(' ')[-1][:-1]
+    file_name = file_name[0].split(': ')[-1][:-1]
     path_data = file_name
     deal_data(path_outcat, path_outcat_wcs, path_mask, path_data, path_save_fig, v_len=30)
 
 
 def plot_average_spectr(data):
     '''
     平均谱SpectralCube read data
```

### Comparing `DensityClust-1.4.6/tools/ultil_lxy.py` & `DensityClust-1.4.7/tools/ultil_lxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from astropy.io import fits
 from astropy.coordinates import SkyCoord
 import pandas as pd
 import matplotlib.pyplot as plt
 import shutil
 import threading
 
-from DensityClust.localDenClust2 import Data
-from DensityClust.localDenClust2 import LocalDensityCluster as LDC
+from distrib.DensityClust.localDenClust2 import Data
+from distrib.DensityClust.localDenClust2 import LocalDensityCluster as LDC
 
 
 def make_plot_wcs_1(outcat_wcs, data_wcs, data_cube):
     """
     在积分图上绘制检测结果
     当没有检测到云核时，只画积分图
     """
```

