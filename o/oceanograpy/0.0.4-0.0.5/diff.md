# Comparing `tmp/oceanograpy-0.0.4.tar.gz` & `tmp/oceanograpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanograpy-0.0.4.tar", last modified: Tue Jul 11 14:40:40 2023, max compression
+gzip compressed data, was "oceanograpy-0.0.5.tar", last modified: Tue Jul 11 20:38:44 2023, max compression
```

## Comparing `oceanograpy-0.0.4.tar` & `oceanograpy-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 14:40:40.961719 oceanograpy-0.0.4/
--rw-rw-rw-   0        0        0    35823 2023-07-07 18:08:28.000000 oceanograpy-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      782 2023-07-11 14:40:40.961719 oceanograpy-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-07-08 03:43:29.000000 oceanograpy-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 14:40:40.938737 oceanograpy-0.0.4/oceanograpy/
--rw-rw-rw-   0        0        0      215 2023-07-09 03:11:06.000000 oceanograpy-0.0.4/oceanograpy/__init__.py
--rw-rw-rw-   0        0        0    24745 2023-07-11 00:32:09.000000 oceanograpy-0.0.4/oceanograpy/adcp_plot_tools.py
--rw-rw-rw-   0        0        0     2166 2023-07-11 00:30:41.000000 oceanograpy-0.0.4/oceanograpy/example.py
--rw-rw-rw-   0        0        0     2797 2023-07-09 03:07:43.000000 oceanograpy-0.0.4/oceanograpy/frma.py
--rw-rw-rw-   0        0        0     5339 2023-07-10 23:50:52.000000 oceanograpy-0.0.4/oceanograpy/matplotlib_dhi.py
--rw-rw-rw-   0        0        0     4375 2023-07-08 03:16:35.000000 oceanograpy-0.0.4/oceanograpy/processing_tools.py
--rw-rw-rw-   0        0        0    24857 2023-07-08 03:22:23.000000 oceanograpy-0.0.4/oceanograpy/seabird_ctd.py
--rw-rw-rw-   0        0        0    67612 2023-07-08 17:53:37.000000 oceanograpy-0.0.4/oceanograpy/workhorse_adcp.py
-drwxrwxrwx   0        0        0        0 2023-07-11 14:40:40.959720 oceanograpy-0.0.4/oceanograpy.egg-info/
--rw-rw-rw-   0        0        0      782 2023-07-11 14:40:40.000000 oceanograpy-0.0.4/oceanograpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-07-11 14:40:40.000000 oceanograpy-0.0.4/oceanograpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 14:40:40.000000 oceanograpy-0.0.4/oceanograpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-11 14:40:40.000000 oceanograpy-0.0.4/oceanograpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      102 2023-07-08 00:06:28.000000 oceanograpy-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 14:40:40.961719 oceanograpy-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      591 2023-07-11 14:35:48.000000 oceanograpy-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:38:44.199522 oceanograpy-0.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-07-07 18:08:28.000000 oceanograpy-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      782 2023-07-11 20:38:44.199522 oceanograpy-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-08 03:43:29.000000 oceanograpy-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 20:38:44.190522 oceanograpy-0.0.5/oceanograpy/
+-rw-rw-rw-   0        0        0      198 2023-07-11 20:37:15.000000 oceanograpy-0.0.5/oceanograpy/__init__.py
+-rw-rw-rw-   0        0        0    24735 2023-07-11 18:15:27.000000 oceanograpy-0.0.5/oceanograpy/adcp_plot_tools.py
+-rw-rw-rw-   0        0        0     2434 2023-07-11 20:22:37.000000 oceanograpy-0.0.5/oceanograpy/example.py
+-rw-rw-rw-   0        0        0     2797 2023-07-09 03:07:43.000000 oceanograpy-0.0.5/oceanograpy/frma.py
+-rw-rw-rw-   0        0        0     5339 2023-07-10 23:50:52.000000 oceanograpy-0.0.5/oceanograpy/matplotlib_dhi.py
+-rw-rw-rw-   0        0        0     4375 2023-07-08 03:16:35.000000 oceanograpy-0.0.5/oceanograpy/processing_tools.py
+-rw-rw-rw-   0        0        0    24857 2023-07-08 03:22:23.000000 oceanograpy-0.0.5/oceanograpy/seabird_ctd.py
+-rw-rw-rw-   0        0        0    67612 2023-07-08 17:53:37.000000 oceanograpy-0.0.5/oceanograpy/workhorse_adcp.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:38:44.197521 oceanograpy-0.0.5/oceanograpy.egg-info/
+-rw-rw-rw-   0        0        0      782 2023-07-11 20:38:44.000000 oceanograpy-0.0.5/oceanograpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-07-11 20:38:44.000000 oceanograpy-0.0.5/oceanograpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 20:38:44.000000 oceanograpy-0.0.5/oceanograpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-11 20:38:44.000000 oceanograpy-0.0.5/oceanograpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      102 2023-07-08 00:06:28.000000 oceanograpy-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 20:38:44.199522 oceanograpy-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-07-11 20:38:32.000000 oceanograpy-0.0.5/setup.py
```

### Comparing `oceanograpy-0.0.4/LICENSE` & `oceanograpy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.4/PKG-INFO` & `oceanograpy-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanograpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Toolbox for importing and plotting ADCP and CTD data
 Home-page:  
 Author: Andy Banks
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oceanograpy-0.0.4/oceanograpy/adcp_plot_tools.py` & `oceanograpy-0.0.5/oceanograpy/adcp_plot_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,16 +360,16 @@
         else:
             X = np.flipud(X)
             extent = [xlims[0],xlims[-1],ylims[1],ylims[0]]
         return X,extent
         
     
     cmaps = {'PERCENT GOOD': plt.cm.bone,
-             'ECHO INTENSITY': plt.cm.Spectral_r,
-             'CORRELATION MAGNITUDE': plt.cm.twilight_shifted}
+             'ECHO INTENSITY': plt.cm.turbo,
+             'CORRELATION MAGNITUDE': plt.cm.nipy_spectral}
     cmap = cmaps[field]
     
     
     vmin = np.nanmin([x1,x2,x3,x4])
     vmax = np.nanmax([x1,x2,x3,x4])
     print(vmin)
     
@@ -508,18 +508,19 @@
         extent = [xlims[0],xlims[-1],ylims[0],ylims[1]]
     else:
         x = np.flipud(x)
         extent = [xlims[0],xlims[-1],ylims[1],ylims[0]]
         
         
     cmaps = {'PERCENT GOOD': plt.cm.bone,
-             'ECHO INTENSITY': plt.cm.Spectral_r,
-             'CORRELATION MAGNITUDE': plt.cm.twilight_shifted}
+             'ECHO INTENSITY': plt.cm.turbo,
+             'CORRELATION MAGNITUDE': plt.cm.nipy_spectral}
     cmap = cmaps[field]
     
+    
     im = ax.imshow(x, origin = 'lower', extent = extent, cmap = cmap, aspect = 'auto')
     cbar = fig.colorbar(im, ax=ax,orientation="vertical",location = 'right',fraction=0.046)
     
     if beam == 0:
         cbar_label = f'{field}\n BEAM AVERAGE' 
     else:
         cbar_label = f'{field}\n BEAM {beam}'
```

### Comparing `oceanograpy-0.0.4/oceanograpy/example.py` & `oceanograpy-0.0.5/oceanograpy/example.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import processing_tools as ptools 
 from matplotlib_dhi import subplots 
 import adcp_plot_tools
 
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 
-pt3_filepath = r'\\USDEN1-STOR.DHI.DK\Projects\41806287\41806287 NORI-D Data\Data\ROV\Island Pride HD14\ADCP\Config\ROV_ADCP_20161_PT3.txt'
-adcp_filepath = r'\\USDEN1-STOR.DHI.DK\Projects\41806287\41806287 NORI-D Data\Data\ROV\Island Pride HD14\ADCP\Raw\ADCP_24142_600kHz\ROV_ADCP_12102022\_RDI_005.000'
+# pt3_filepath = r'\\USDEN1-STOR.DHI.DK\Projects\41806287\41806287 NORI-D Data\Data\ROV\Island Pride HD14\ADCP\Config\ROV_ADCP_20161_PT3.txt'
+# adcp_filepath = r'\\USDEN1-STOR.DHI.DK\Projects\41806287\41806287 NORI-D Data\Data\ROV\Island Pride HD14\ADCP\Raw\ADCP_24142_600kHz\ROV_ADCP_12102022\_RDI_005.000'
 
 
 
 pt3_filepath = r'\\USDEN1-STOR.DHI.DK\Projects\41806287\41806287 NORI-D Data\Data\Fixed Stations\02_Fixed_Bottom_Current_Turbidity\02_FBCT2\01_ADCP_600kHz-24144\Config_File\FBCT02_P3_TEST_17112022.txt'
 adcp_filepath = r'\\USDEN1-STOR.DHI.DK\Projects\41806287\41806287 NORI-D Data\Data\Fixed Stations\02_Fixed_Bottom_Current_Turbidity\02_FBCT2\01_ADCP_600kHz-24144\Raw\FBCT2_Full_Download_17112022\FBCT2000.000'
 
 
@@ -28,47 +28,48 @@
 
 
 #%%
 
 import adcp_plot_tools
 import processing_tools as ptools
 from matplotlib_dhi import subplots
-
 import os
 
 
 adcp_plot_tools.progressive_vector_plot(adcp_data)#, color_by , start_bin, end_bin, start_ensemble, end_ensemble, title)
 fig,ax = adcp_plot_tools.error_velocity_plot(adcp_data)
 
 fig,ax = adcp_plot_tools.four_beam_flood_plot(adcp_data,field = 'ECHO INTENSITY')
 fig,ax = adcp_plot_tools.four_beam_flood_plot(adcp_data,field = 'CORRELATION MAGNITUDE')
 fig,ax = adcp_plot_tools.four_beam_flood_plot(adcp_data,field = 'PERCENT GOOD')
 
 fig,ax = adcp_plot_tools.single_beam_flood_plot(adcp_data,field = 'ECHO INTENSITY')
 fig,ax = adcp_plot_tools.single_beam_flood_plot(adcp_data,field = 'CORRELATION MAGNITUDE')
 fig,ax = adcp_plot_tools.single_beam_flood_plot(adcp_data,field = 'PERCENT GOOD')
-#fig,ax = adcp_plot_tools.metadata_table(adcp_data)
-
-
-
+fig,ax = adcp_plot_tools.metadata_table(adcp_data)
 
+#%% Add position data 
+import pandas as pd 
 
+adcp_file = adcp_data 
+IP_ROV_Pos = pd.read_csv(r'\\USDEN1-STOR.DHI.DK\Projects\41806287\41806287 NORI-D Data\Data\ROV\Island Pride HD14\Position\Processed\01 Merge\USBL_data_all_dives_cleaned.csv', index_col = [0])
 
+IP_ROV.dropna()
 
-#%% correlation magnitude plots 
 
 
 
 #%% Auto QAQC
 
 
 
 
+#%% lump together ADCP data into single files 
+
 
 
 
 
-#%% Add position data
```

### Comparing `oceanograpy-0.0.4/oceanograpy/frma.py` & `oceanograpy-0.0.5/oceanograpy/frma.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.4/oceanograpy/matplotlib_dhi.py` & `oceanograpy-0.0.5/oceanograpy/matplotlib_dhi.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.4/oceanograpy/processing_tools.py` & `oceanograpy-0.0.5/oceanograpy/processing_tools.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.4/oceanograpy/seabird_ctd.py` & `oceanograpy-0.0.5/oceanograpy/seabird_ctd.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.4/oceanograpy/workhorse_adcp.py` & `oceanograpy-0.0.5/oceanograpy/workhorse_adcp.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.4/oceanograpy.egg-info/PKG-INFO` & `oceanograpy-0.0.5/oceanograpy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanograpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Toolbox for importing and plotting ADCP and CTD data
 Home-page:  
 Author: Andy Banks
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oceanograpy-0.0.4/setup.py` & `oceanograpy-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="oceanograpy",
-    version="0.0.4",
+    version="0.0.5",
     author="Andy Banks",
     author_email="",
     description="Toolbox for importing and plotting ADCP and CTD data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=" ",
     packages=["oceanograpy"],
```

