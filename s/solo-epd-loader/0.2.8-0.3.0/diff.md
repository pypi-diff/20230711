# Comparing `tmp/solo_epd_loader-0.2.8.tar.gz` & `tmp/solo_epd_loader-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-htd_kfzz/solo_epd_loader-0.2.8.tar", last modified: Wed Jun 21 10:41:23 2023, max compression
+gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-04rue_h5/solo_epd_loader-0.3.0.tar", last modified: Tue Jul 11 13:18:08 2023, max compression
```

## Comparing `solo_epd_loader-0.2.8.tar` & `solo_epd_loader-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-21 10:41:23.817713 solo_epd_loader-0.2.8/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.8/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.8/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-21 10:41:23.817713 solo_epd_loader-0.2.8/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15847 2023-06-19 08:20:58.000000 solo_epd_loader-0.2.8/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.8/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-21 10:41:23.813713 solo_epd_loader-0.2.8/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.8/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.8/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.8/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.8/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-21 10:41:23.813713 solo_epd_loader-0.2.8/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.8/examples/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.8/examples/ws2021_fig_2d.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.8/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.8/gh2021_fig_2a.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-21 10:41:23.817713 solo_epd_loader-0.2.8/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.8/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.8/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.8/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2306 2023-06-21 10:41:23.821713 solo_epd_loader-0.2.8/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.8/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-21 10:41:23.817713 solo_epd_loader-0.2.8/solo_epd_loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    55919 2023-06-21 10:39:08.000000 solo_epd_loader-0.2.8/solo_epd_loader/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-21 10:41:23.817713 solo_epd_loader-0.2.8/solo_epd_loader/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.8/solo_epd_loader/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-06-21 10:41:23.000000 solo_epd_loader-0.2.8/solo_epd_loader/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-21 10:41:23.817713 solo_epd_loader-0.2.8/solo_epd_loader.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-21 10:41:23.000000 solo_epd_loader-0.2.8/solo_epd_loader.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      611 2023-06-21 10:41:23.000000 solo_epd_loader-0.2.8/solo_epd_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-06-21 10:41:23.000000 solo_epd_loader-0.2.8/solo_epd_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.8/solo_epd_loader.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      192 2023-06-21 10:41:23.000000 solo_epd_loader-0.2.8/solo_epd_loader.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-06-21 10:41:23.000000 solo_epd_loader-0.2.8/solo_epd_loader.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.8/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-11 13:18:08.273784 solo_epd_loader-0.3.0/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.0/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.0/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16697 2023-07-11 13:18:08.273784 solo_epd_loader-0.3.0/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15749 2023-07-11 13:14:50.000000 solo_epd_loader-0.3.0/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.3.0/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-11 13:18:08.261785 solo_epd_loader-0.3.0/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.0/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.0/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.3.0/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.0/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-11 13:18:08.265785 solo_epd_loader-0.3.0/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.3.0/examples/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.3.0/examples/ws2021_fig_2d.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.3.0/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.3.0/gh2021_fig_2a.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-11 13:18:08.269784 solo_epd_loader-0.3.0/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.3.0/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2023-07-05 12:35:18.000000 solo_epd_loader-0.3.0/licenses/SUNPY_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.0/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.0/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2302 2023-07-11 13:18:08.273784 solo_epd_loader-0.3.0/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.3.0/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-11 13:18:08.269784 solo_epd_loader-0.3.0/solo_epd_loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    76151 2023-07-11 13:17:01.000000 solo_epd_loader-0.3.0/solo_epd_loader/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-11 13:18:08.273784 solo_epd_loader-0.3.0/solo_epd_loader/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.3.0/solo_epd_loader/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-07-11 13:18:08.000000 solo_epd_loader-0.3.0/solo_epd_loader/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-07-11 13:18:08.273784 solo_epd_loader-0.3.0/solo_epd_loader.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16697 2023-07-11 13:18:08.000000 solo_epd_loader-0.3.0/solo_epd_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      638 2023-07-11 13:18:08.000000 solo_epd_loader-0.3.0/solo_epd_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-07-11 13:18:08.000000 solo_epd_loader-0.3.0/solo_epd_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.3.0/solo_epd_loader.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      188 2023-07-11 13:18:08.000000 solo_epd_loader-0.3.0/solo_epd_loader.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-07-11 13:18:08.000000 solo_epd_loader-0.3.0/solo_epd_loader.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.3.0/tox.ini
```

### Comparing `solo_epd_loader-0.2.8/LICENSE.rst` & `solo_epd_loader-0.3.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.8/PKG-INFO` & `solo_epd_loader-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo_epd_loader
-Version: 0.2.8
+Version: 0.3.0
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -43,16 +43,16 @@
 - Electron Proton Telescope (EPT)
 - High Energy Telescope (HET)
 - SupraThermal Electrons and Protons (STEP)
 
 Current caveats:
 
 - Only the standard ``rates`` data products are supported (i.e., no ``burst`` or ``high cadence`` data).
-- Only electrons, protons and alpha particles are processed (i.e., for HET He3, He4, C, N, O, Fe are omitted at the moment).
-- For the old STEP data product (until Oct 22, 2021), the sectored data is not processed (i.e., only averaged data is supported) and electron data needs to be calculated manually.
+- For EPT and HET, only electrons, protons and alpha particles are processed (i.e., for HET He3, He4, C, N, O, Fe are omitted at the moment).
+- For STEP, electron data needs to be calculated manually.
 - The Suprathermal Ion Spectrograph (SIS) is not yet included. 
 
 Disclaimer
 ----------
 This software is provided "as is", with no guarantee. It is no official data source, and not officially endorsed by the corresponding instrument teams. **Please always refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
 
 Installation
@@ -266,15 +266,15 @@
    # plot selection of ept electron channels
    for channel in [0, 8, 16, 26]:
       df_electrons_ept['Electron_Flux'][f'Electron_Flux_{channel}'].resample(resample).mean().plot(
          ax = axs[0], logy=True, label='EPT '+energies_ept["Electron_Bins_Text"][channel][0])
 
    # plot selection of step ion channels
    for channel in [8, 17, 33]:
-      df_step['Magnet_Flux'][channel].resample(resample).mean().plot(
+      df_step[f'Magnet_Avg_Flux_{channel}'].resample(resample).mean().plot(
          ax = axs[1], logy=True, label='STEP '+energies_step["Bins_Text"][channel][0])
 
    # plot selection of ept ion channels
    for channel in [6, 22, 32, 48]:
       df_protons_ept['Ion_Flux'][f'Ion_Flux_{channel}'].resample(resample).mean().plot(
          ax = axs[1], logy=True, label='EPT '+energies_ept["Ion_Bins_Text"][channel][0])
```

### Comparing `solo_epd_loader-0.2.8/README.rst` & `solo_epd_loader-0.3.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 - Electron Proton Telescope (EPT)
 - High Energy Telescope (HET)
 - SupraThermal Electrons and Protons (STEP)
 
 Current caveats:
 
 - Only the standard ``rates`` data products are supported (i.e., no ``burst`` or ``high cadence`` data).
-- Only electrons, protons and alpha particles are processed (i.e., for HET He3, He4, C, N, O, Fe are omitted at the moment).
-- For the old STEP data product (until Oct 22, 2021), the sectored data is not processed (i.e., only averaged data is supported) and electron data needs to be calculated manually.
+- For EPT and HET, only electrons, protons and alpha particles are processed (i.e., for HET He3, He4, C, N, O, Fe are omitted at the moment).
+- For STEP, electron data needs to be calculated manually.
 - The Suprathermal Ion Spectrograph (SIS) is not yet included. 
 
 Disclaimer
 ----------
 This software is provided "as is", with no guarantee. It is no official data source, and not officially endorsed by the corresponding instrument teams. **Please always refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
 
 Installation
@@ -241,15 +241,15 @@
    # plot selection of ept electron channels
    for channel in [0, 8, 16, 26]:
       df_electrons_ept['Electron_Flux'][f'Electron_Flux_{channel}'].resample(resample).mean().plot(
          ax = axs[0], logy=True, label='EPT '+energies_ept["Electron_Bins_Text"][channel][0])
 
    # plot selection of step ion channels
    for channel in [8, 17, 33]:
-      df_step['Magnet_Flux'][channel].resample(resample).mean().plot(
+      df_step[f'Magnet_Avg_Flux_{channel}'].resample(resample).mean().plot(
          ax = axs[1], logy=True, label='STEP '+energies_step["Bins_Text"][channel][0])
 
    # plot selection of ept ion channels
    for channel in [6, 22, 32, 48]:
       df_protons_ept['Ion_Flux'][f'Ion_Flux_{channel}'].resample(resample).mean().plot(
          ax = axs[1], logy=True, label='EPT '+energies_ept["Ion_Bins_Text"][channel][0])
```

### Comparing `solo_epd_loader-0.2.8/code_of_conduct.md` & `solo_epd_loader-0.3.0/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.8/docs/Makefile` & `solo_epd_loader-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.8/docs/conf.py` & `solo_epd_loader-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.8/docs/make.bat` & `solo_epd_loader-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.8/examples/gh2021_fig_2.png` & `solo_epd_loader-0.3.0/examples/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.8/examples/ws2021_fig_2d.png` & `solo_epd_loader-0.3.0/examples/ws2021_fig_2d.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.8/gh2021_fig_2.png` & `solo_epd_loader-0.3.0/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.8/gh2021_fig_2a.png` & `solo_epd_loader-0.3.0/gh2021_fig_2a.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.8/licenses/LICENSE.rst` & `solo_epd_loader-0.3.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.8/licenses/TEMPLATE_LICENSE.rst` & `solo_epd_loader-0.3.0/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.8/setup.cfg` & `solo_epd_loader-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 packages = find:
 include_package_data = True
 python_requires = >=3.6
 setup_requires = setuptools_scm
 install_requires = 
 	astropy
 	bs4
-	cdflib<1.0
+	cdflib
 	datetime
 	drms
 	h5netcdf
 	lxml
 	matplotlib
 	numpy
 	pandas
```

### Comparing `solo_epd_loader-0.2.8/setup.py` & `solo_epd_loader-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.8/solo_epd_loader/__init__.py` & `solo_epd_loader-0.3.0/solo_epd_loader/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,38 +11,40 @@
 import glob
 import itertools
 import os
 import re
 import sunpy
 import urllib.request
 import warnings
+from packaging.version import Version
 from pathlib import Path
 
 import cdflib
 import numpy as np
 import pandas as pd
 from astropy.io.votable import parse_single_table
-if int(sunpy.__version__[0]) == 4:
-    from sunpy.io.cdf import read_cdf
-elif int(sunpy.__version__[0]) >= 5:
-    from sunpy.io._cdf import read_cdf
+
+if hasattr(sunpy, "__version__") and Version(sunpy.__version__) >= Version("5.0.0"):
+    from sunpy.io._cdf import read_cdf, _known_units
+else:
+    from sunpy.io.cdf import read_cdf, _known_units
 from sunpy.timeseries import TimeSeries
 
 # omit Pandas' PerformanceWarning
 warnings.simplefilter(action='ignore', category=pd.errors.PerformanceWarning)
 
 
 """
 Example code that loads low latency (ll) electron and proton (+alphas) fluxes
 (and errors) for 'ept' 'north' telescope from Apr 15 2021 to Apr 16 2021 into
 two Pandas dataframes (one for protons & alphas, one for electrons). In general
 available are 'sun', 'asun', 'north', and 'south' viewing directions for 'ept'
 and 'het' telescopes of SolO/EPD.
 
-from epd_loader import *
+from solo_epd_loader import *
 
 df_protons, df_electrons, energies = \
 _read_epd_cdf('ept', 'north', 'll', 20210415, 20210416,
 path='/home/userxyz/solo/data/')
 
 # plot protons and alphas
 ax = df_protons.plot(logy=True, subplots=True, figsize=(20,60))
@@ -139,16 +141,15 @@
         if verbose:
             print("Module tqdm not installed, won't show progress bar. To get rid of this: pip install tqdm")
         tqdm_available = False
         download_url = None
     return tqdm_available, download_url
 
 
-def _get_epd_filelist(sensor, level, startdate, enddate, path,
-                      filenames_only=False):
+def _get_epd_filelist(sensor, level, startdate, enddate, path, filenames_only=False):
     """
     INPUT:
         sensor: 'ept' or 'het'
         level: 'll', 'l2'
         startdate, enddate: YYYYMMDD
         path: directory in which the data is located;
               e.g. '/home/userxyz/uni/solo/data/l2/epd/ept/'
@@ -193,16 +194,15 @@
                 'asun': filelist_asun,
                 'north': filelist_north,
                 'south': filelist_south
                 }
     return filelist
 
 
-def _get_step_filelist(level, startdate, enddate, path,
-                       filenames_only=False):
+def _get_step_filelist(level, startdate, enddate, path, filenames_only=False):
     """
     INPUT:
         level: 'll', 'l2'
         startdate, enddate: YYYYMMDD
         path: directory in which the data is located;
               e.g. '/home/userxyz/uni/solo/data/l2/epd/step/'
         filenames_only: if True only give the filenames, not the full path
@@ -438,16 +438,15 @@
                                      viewing=tview)
             if level.lower() == 'l2':
                 _ = _epd_l2_download(date=tdate, path=path, sensor=sensor,
                                      viewing=tview)
     return
 
 
-def epd_load(sensor, startdate, enddate=None, level='l2', viewing=None, path=None,
-             autodownload=False, only_averages=False):
+def epd_load(sensor, startdate, enddate=None, level='l2', viewing=None, path=None, autodownload=False, only_averages=False, old_step_loading=False):
     """
     Load SolO/EPD data
 
     Load-in data for Solar Orbiter/EPD energetic charged particle sensors EPT,
     HET, and STEP. Supports level 2 and low latency data provided by ESA's
     Solar Orbiter Archive. Optionally downloads missing data directly. Returns
     data as Pandas dataframe.
@@ -479,14 +478,18 @@
     autodownload : bool, optional
         If True, will try to download missing data files from SOAR, by default
         False.
     only_averages : bool, optional
         If True, will for STEP only return the averaged fluxes, and not the data
         of each of the 15 Pixels. This will reduce the memory consumption. By
         default False.
+    old_step_loading : bool, optional
+        If True, will for old (i.e. before Oct 2021) STEP data loading use the
+        legacy code that provides a multi-index DataFrame as output. Otherwise
+        new loading functionality by sunpy will be used. By default True.
 
     Returns
     -------
     For EPT & HET:
         1. Pandas dataframe with proton fluxes and errors (for EPT also alpha particles) in 'particles / (s cm^2 sr MeV)'
         2. Pandas dataframe with electron fluxes and errors in 'particles / (s cm^2 sr MeV)'
         3. Dictionary with energy information for all particles:
@@ -536,32 +539,32 @@
     for d in [startdate, enddate]:
         if isinstance(d, int):
             if len(str(d)) != 8:
                 raise SystemExit(f"startdate & enddate must be (datetime objects or) integers of the form YYYYMMDD, not {d}!")
 
     if sensor.lower() == 'step':
         datadf, energies_dict = \
-            _read_step_cdf(level, startdate, enddate, path, autodownload, only_averages)
+            _read_step_cdf(level=level, startdate=startdate, enddate=enddate, path=path, autodownload=autodownload,
+                           only_averages=only_averages, old_loading=old_step_loading)
         return datadf, energies_dict
     if sensor.lower() == 'ept' or sensor.lower() == 'het':
         if viewing is None:
             raise Exception("EPT and HET need a telescope 'viewing' " +
                             "direction! No data read!")
             df_epd_p = []
             df_epd_e = []
             energies_dict = []
         else:
             df_epd_p, df_epd_e, energies_dict = \
-                _read_epd_cdf(sensor, viewing, level, startdate, enddate, path,
-                              autodownload)
+                _read_epd_cdf(sensor=sensor, viewing=viewing, level=level, startdate=startdate, enddate=enddate,
+                              path=path, autodownload=autodownload)
         return df_epd_p, df_epd_e, energies_dict
 
 
-def _read_epd_cdf(sensor, viewing, level, startdate, enddate=None, path=None,
-                  autodownload=False):
+def _read_epd_cdf(sensor, viewing, level, startdate, enddate=None, path=None, autodownload=False):
     """
     INPUT:
         sensor: 'ept' or 'het' (string)
         viewing: 'sun', 'asun', 'north', or 'south' (string)
         level: 'll' or 'l2' (string)
         startdate,
         enddate:    YYYYMMDD, e.g., 20210415 (integer)
@@ -649,67 +652,79 @@
                 df_p = pd.concat([df_p, t_df_p])
                 df_e = pd.concat([df_e, t_df_e])
 
         # directly open first cdf file with cdflib to access metadata used in the following
         t_cdf_file = cdflib.CDF(filelist[0])
 
         # p intensities:
-        flux_p_channels = \
-            [protons+f'_Flux_{i}' for i in
-             range(t_cdf_file.varinq(protons+'_Flux')['Dim_Sizes'][0])]
+        if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+            flux_p_channels = [protons+f'_Flux_{i}' for i in range(t_cdf_file.varinq(protons+'_Flux').Dim_Sizes[0])]
+        else:
+            flux_p_channels = [protons+f'_Flux_{i}' for i in range(t_cdf_file.varinq(protons+'_Flux')['Dim_Sizes'][0])]
         # p errors:
         if level.lower() == 'll':
-            flux_sigma_p_channels = \
-                [protons+f'_Flux_Sigma_{i}' for i in
-                 range(t_cdf_file.varinq(protons+'_Flux')['Dim_Sizes'][0])]
+            if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+                flux_sigma_p_channels = [protons+f'_Flux_Sigma_{i}' for i in range(t_cdf_file.varinq(protons+'_Flux').Dim_Sizes[0])]
+            else:
+                flux_sigma_p_channels = [protons+f'_Flux_Sigma_{i}' for i in range(t_cdf_file.varinq(protons+'_Flux')['Dim_Sizes'][0])]
         if level.lower() == 'l2':
-            flux_sigma_p_channels = \
-                [protons+f'_Uncertainty_{i}' for i in
-                 range(t_cdf_file.varinq(protons+'_Flux')['Dim_Sizes'][0])]
+            if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+                flux_sigma_p_channels = [protons+f'_Uncertainty_{i}' for i in range(t_cdf_file.varinq(protons+'_Flux').Dim_Sizes[0])]
+            else:
+                flux_sigma_p_channels = [protons+f'_Uncertainty_{i}' for i in range(t_cdf_file.varinq(protons+'_Flux')['Dim_Sizes'][0])]
             # p rates:
-            rate_p_channels = \
-                [protons+f'_Rate_{i}' for i in
-                 range(t_cdf_file.varinq(protons+'_Rate')['Dim_Sizes'][0])]
+            if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+                rate_p_channels = [protons+f'_Rate_{i}' for i in range(t_cdf_file.varinq(protons+'_Rate').Dim_Sizes[0])]
+            else:
+                rate_p_channels = [protons+f'_Rate_{i}' for i in range(t_cdf_file.varinq(protons+'_Rate')['Dim_Sizes'][0])]
 
         if sensor.lower() == 'ept':
             # alpha intensities:
-            flux_a_channels = \
-                [f'Alpha_Flux_{i}' for i in
-                 range(t_cdf_file.varinq("Alpha_Flux")['Dim_Sizes'][0])]
+            if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+                flux_a_channels = [f'Alpha_Flux_{i}' for i in range(t_cdf_file.varinq("Alpha_Flux").Dim_Sizes[0])]
+            else:
+                flux_a_channels = [f'Alpha_Flux_{i}' for i in range(t_cdf_file.varinq("Alpha_Flux")['Dim_Sizes'][0])]
             # alpha errors:
             if level.lower() == 'll':
-                flux_sigma_a_channels = \
-                    [f'Alpha_Flux_Sigma_{i}' for i in
-                     range(t_cdf_file.varinq("Alpha_Flux")['Dim_Sizes'][0])]
+                if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+                    flux_sigma_a_channels = [f'Alpha_Flux_Sigma_{i}' for i in range(t_cdf_file.varinq("Alpha_Flux").Dim_Sizes[0])]
+                else:
+                    flux_sigma_a_channels = [f'Alpha_Flux_Sigma_{i}' for i in range(t_cdf_file.varinq("Alpha_Flux")['Dim_Sizes'][0])]
             if level.lower() == 'l2':
-                flux_sigma_a_channels = \
-                    [f'Alpha_Uncertainty_{i}' for i in
-                     range(t_cdf_file.varinq("Alpha_Flux")['Dim_Sizes'][0])]
+                if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+                    flux_sigma_a_channels = [f'Alpha_Uncertainty_{i}' for i in range(t_cdf_file.varinq("Alpha_Flux").Dim_Sizes[0])]
+                else:
+                    flux_sigma_a_channels = [f'Alpha_Uncertainty_{i}' for i in range(t_cdf_file.varinq("Alpha_Flux")['Dim_Sizes'][0])]
                 # alpha rates:
-                rate_a_channels = \
-                    [f'Alpha_Rate_{i}' for i in
-                     range(t_cdf_file.varinq("Alpha_Rate")['Dim_Sizes'][0])]
+                if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+                    rate_a_channels = [f'Alpha_Rate_{i}' for i in range(t_cdf_file.varinq("Alpha_Rate").Dim_Sizes[0])]
+                else:
+                    rate_a_channels = [f'Alpha_Rate_{i}' for i in range(t_cdf_file.varinq("Alpha_Rate")['Dim_Sizes'][0])]
 
         # e intensities:
-        flux_e_channels = \
-            [electrons+f'_Flux_{i}' for i in
-             range(t_cdf_file.varinq(electrons+'_Flux')['Dim_Sizes'][0])]
+        if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+            flux_e_channels = [electrons+f'_Flux_{i}' for i in range(t_cdf_file.varinq(electrons+'_Flux').Dim_Sizes[0])]
+        else:
+            flux_e_channels = [electrons+f'_Flux_{i}' for i in range(t_cdf_file.varinq(electrons+'_Flux')['Dim_Sizes'][0])]
         # e errors:
         if level.lower() == 'll':
-            flux_sigma_e_channels = \
-                [f'Ele_Flux_Sigma_{i}' for i in
-                 range(t_cdf_file.varinq(electrons+'_Flux')['Dim_Sizes'][0])]
+            if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+                flux_sigma_e_channels = [f'Ele_Flux_Sigma_{i}' for i in range(t_cdf_file.varinq(electrons+'_Flux').Dim_Sizes[0])]
+            else:
+                flux_sigma_e_channels = [f'Ele_Flux_Sigma_{i}' for i in range(t_cdf_file.varinq(electrons+'_Flux')['Dim_Sizes'][0])]
         if level.lower() == 'l2':
-            flux_sigma_e_channels = \
-                [f'Electron_Uncertainty_{i}' for i in
-                 range(t_cdf_file.varinq(electrons+'_Flux')['Dim_Sizes'][0])]
+            if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+                flux_sigma_e_channels = [f'Electron_Uncertainty_{i}' for i in range(t_cdf_file.varinq(electrons+'_Flux').Dim_Sizes[0])]
+            else:
+                flux_sigma_e_channels = [f'Electron_Uncertainty_{i}' for i in range(t_cdf_file.varinq(electrons+'_Flux')['Dim_Sizes'][0])]
             # e rates:
-            rate_e_channels = \
-                [electrons+f'_Rate_{i}' for i in
-                 range(t_cdf_file.varinq(electrons+'_Rate')['Dim_Sizes'][0])]
+            if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+                rate_e_channels = [electrons+f'_Rate_{i}' for i in range(t_cdf_file.varinq(electrons+'_Rate').Dim_Sizes[0])]
+            else:
+                rate_e_channels = [electrons+f'_Rate_{i}' for i in range(t_cdf_file.varinq(electrons+'_Rate')['Dim_Sizes'][0])]
 
         if level.lower() == 'l2':
             if sensor.lower() == 'het':
                 df_epd_p = pd.concat(
                     [df_p[flux_p_channels], df_p[flux_sigma_p_channels],
                      df_p[rate_p_channels], df_p['DELTA_EPOCH'],
                      df_p['QUALITY_FLAG'], df_p['QUALITY_BITMASK']],
@@ -820,16 +835,15 @@
     Careful if adding more species - they might have different EPOCH
     dependencies and cannot easily be put in the same dataframe!
     '''
 
     return df_epd_p, df_epd_e, energies_dict
 
 
-def _read_step_cdf(level, startdate, enddate=None, path=None, autodownload=False,
-                   only_averages=False):
+def _read_step_cdf(level, startdate, enddate=None, path=None, autodownload=False, only_averages=False, old_loading=False):
     """
     INPUT:
         level: 'll' or 'l2' (string)
         startdate,
         enddate:    YYYYMMDD, e.g., 20210415 (integer)
                     (if no enddate is given, 'enddate = startdate' will be set)
         path: directory in which Solar Orbiter data is/should be organized;
@@ -888,143 +902,187 @@
         filelist = _check_duplicates(filelist, verbose=True)
 
         if len(filelist) == 0:
             warnings.warn('WARNING: No corresponding data files found! Try different settings, path or autodownload.')
             datadf = []
             energies_dict = []
         elif product == 'rates':
-            all_cdf = []
-            for file in filelist:
-                all_cdf.append(cdflib.CDF(file))
-
-            if level == 'l2':
-                param_list = ['Integral_Flux', 'Magnet_Flux', 'Integral_Rate',
-                              'Magnet_Rate', 'Magnet_Uncertainty',
-                              'Integral_Uncertainty']
-                # set up the dictionary:
-                energies_dict = \
-                    {"Bins_Text": all_cdf[0].varget('Bins_Text'),
-                     "Bins_Low_Energy": all_cdf[0].varget('Bins_Low_Energy'),
-                     "Bins_Width": all_cdf[0].varget('Bins_Width'),
-                     "Sector_Bins_Text": all_cdf[0].varget('Sector_Bins_Text'),
-                     "Sector_Bins_Low_Energy": all_cdf[0].varget('Sector_Bins_Low_Energy'),
-                     "Sector_Bins_Width": all_cdf[0].varget('Sector_Bins_Width')
-                     }
-            if level == 'll':
-                param_list = ['Integral_Flux', 'Ion_Flux', 'Integral_Flux_Sigma',
-                              'Ion_Flux_Sigma']
-                # set up the dictionary:
-                energies_dict = \
-                    {"Integral_Bins_Text": all_cdf[0].varget('Integral_Bins_Text'),
-                     "Integral_Bins_Low_Energy": all_cdf[0].varget('Integral_Bins_Low_Energy'),
-                     "Integral_Bins_Width": all_cdf[0].varget('Integral_Bins_Width'),
-                     "Ion_Bins_Text": all_cdf[0].varget('Ion_Bins_Text'),
-                     "Ion_Bins_Low_Energy": all_cdf[0].varget('Ion_Bins_Low_Energy'),
-                     "Ion_Bins_Width": all_cdf[0].varget('Ion_Bins_Width')
-                     }
-
-            df_list = []
-            for cdffile in all_cdf:
-                col_list = []
-                for key in param_list:
-                    try:
-                        t_df = pd.DataFrame(cdffile[key], index=cdffile['EPOCH'])
-
-                        # Replace FILLVAL dynamically for each element of param_list
-                        fillval = cdffile.varattsget(key)["FILLVAL"]
-                        t_df = t_df.replace(fillval, np.nan)
-
-                        col_list.append(t_df)
-                    except TypeError:
-                        print(' ')
-                        print("WARNING: Gap in dataframe due to missing cdf file.")
-                        break
-                try:
-                    temp_df = pd.concat(col_list, axis=1, keys=param_list)
-                    df_list.append(temp_df)
-                except ValueError:
-                    continue
-            datadf = pd.concat(df_list)
-
-            # transform the index of the dataframe into pd_datetime
-            datetimes = cdflib.cdfepoch.encode(datadf.index.values)
-            datadf.index = pd.to_datetime(datetimes)
-
-            datadf.index.names = ['Time']
-
-            # if type(contamination_threshold) == int:
-            #     print("'contamination_threshold' not yet included for old STEP data (before Oct 22, 2021)!")
+            if old_loading:
+                all_cdf = []
+                for file in filelist:
+                    all_cdf.append(cdflib.CDF(file))
+
+                if level == 'l2':
+                    param_list = ['Integral_Flux', 'Magnet_Flux', 'Integral_Rate',
+                                  'Magnet_Rate', 'Magnet_Uncertainty',
+                                  'Integral_Uncertainty']
+                    # set up the dictionary:
+                    energies_dict = \
+                        {"Bins_Text": all_cdf[0].varget('Bins_Text'),
+                         "Bins_Low_Energy": all_cdf[0].varget('Bins_Low_Energy'),
+                         "Bins_Width": all_cdf[0].varget('Bins_Width'),
+                         "Sector_Bins_Text": all_cdf[0].varget('Sector_Bins_Text'),
+                         "Sector_Bins_Low_Energy": all_cdf[0].varget('Sector_Bins_Low_Energy'),
+                         "Sector_Bins_Width": all_cdf[0].varget('Sector_Bins_Width')
+                         }
+                if level == 'll':
+                    param_list = ['Integral_Flux', 'Ion_Flux', 'Integral_Flux_Sigma',
+                                  'Ion_Flux_Sigma']
+                    # set up the dictionary:
+                    energies_dict = \
+                        {"Integral_Bins_Text": all_cdf[0].varget('Integral_Bins_Text'),
+                         "Integral_Bins_Low_Energy": all_cdf[0].varget('Integral_Bins_Low_Energy'),
+                         "Integral_Bins_Width": all_cdf[0].varget('Integral_Bins_Width'),
+                         "Ion_Bins_Text": all_cdf[0].varget('Ion_Bins_Text'),
+                         "Ion_Bins_Low_Energy": all_cdf[0].varget('Ion_Bins_Low_Energy'),
+                         "Ion_Bins_Width": all_cdf[0].varget('Ion_Bins_Width')
+                         }
 
+                df_list = []
+                for cdffile in all_cdf:
+                    col_list = []
+                    for key in param_list:
+                        try:
+                            t_df = pd.DataFrame(cdffile[key], index=cdffile['EPOCH'])
+
+                            # Replace FILLVAL dynamically for each element of param_list
+                            fillval = cdffile.varattsget(key)["FILLVAL"]
+                            t_df = t_df.replace(fillval, np.nan)
+
+                            col_list.append(t_df)
+                        except TypeError:
+                            print(' ')
+                            print("WARNING: Gap in dataframe due to missing cdf file.")
+                            break
+                    try:
+                        temp_df = pd.concat(col_list, axis=1, keys=param_list)
+                        df_list.append(temp_df)
+                    except ValueError:
+                        continue
+                datadf = pd.concat(df_list)
+
+                # transform the index of the dataframe into pd_datetime
+                datetimes = cdflib.cdfepoch.encode(datadf.index.values)
+                datadf.index = pd.to_datetime(datetimes)
+
+                datadf.index.names = ['Time']
+
+                # if type(contamination_threshold) == int:
+                #     print("'contamination_threshold' not yet included for old STEP data (before Oct 22, 2021)!")
+            else:
+                datadf, energies_dict = _read_new_step_cdf(filelist, only_averages)
         elif product == 'main':
             datadf, energies_dict = _read_new_step_cdf(filelist, only_averages)
 
+    # rename index column (instead of e.g. 'EPOCH' or 'EPOCH_1')
+    datadf.index.names = ['Time']
+
     '''
     Careful if adding more species - they might have different EPOCH
     dependencies and cannot easily be put in the same dataframe!
     '''
 
     return datadf, energies_dict
 
 
 def _read_new_step_cdf(files, only_averages=False):
     """
-    Function that reads in new format (since Oct 2021) STEP CDF 'files'.
+    Function that reads in old & new format (since Oct 2021) STEP CDF 'files'.
     EPOCH_X dependent data is obtained as Pandas Dataframe via sunpy.
     Time-independent meta data is read in from the first cdf file via cdflib.
     """
+    all_columns = False  # if False, Rate data will be omitted
+
     # read electron correction factors and meta data via cdflib
     cdf = cdflib.CDF(files[0])
-    Electron_Flux_Mult = {'Electron_Avg_Flux_Mult': cdf['Electron_Avg_Flux_Mult']}
-    # if not only_averages:
-    for i in range(1, 16):
-        Electron_Flux_Mult['Electron_'+str(i).rjust(2, '0')+'_Flux_Mult'] = cdf['Electron_'+str(i).rjust(2, '0')+'_Flux_Mult']
-    # df_Electron_Flux_Mult = pd.DataFrame(Electron_Flux_Mult)  # get dataframe from dict - not needed atm.
+    cdf_info = cdf.cdf_info()
+    if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+        all_var_keys = cdf_info.rVariables + cdf_info.zVariables
+    else:
+        all_var_keys = cdf_info['rVariables'] + cdf_info['zVariables']
+    var_attrs = {key: cdf.varattsget(key) for key in all_var_keys}
+    support_var_keys = [var for var in var_attrs if 'DEPEND_0' not in var_attrs[var] and not var.startswith('EPOCH') and not var.endswith('_Flux_Mult')]
 
-    meta = {'Bins_Low_Energy': cdf['Bins_Low_Energy']}
-    for i in ['Bins_Width', 'Bins_Text', 'Electron_Bins_Low_Energy', 'Electron_Bins_Width', 'Electron_Bins_Text', 'XYZ', 'XYZ_Pixels', 'XYZ_Labels', 'RTN_Labels']:
+    meta = {support_var_keys[0]: cdf[support_var_keys.pop(0)]}
+    for i in support_var_keys:
         meta[i] = cdf[i]
 
-    meta['Electron_Flux_Mult'] = Electron_Flux_Mult
+    if 'Electron_Avg_Flux_Mult' in var_attrs:
+        Electron_Flux_Mult = {'Electron_Avg_Flux_Mult': cdf['Electron_Avg_Flux_Mult']}
+        # if not only_averages:
+        for i in range(1, 16):
+            Electron_Flux_Mult['Electron_'+str(i).rjust(2, '0')+'_Flux_Mult'] = cdf['Electron_'+str(i).rjust(2, '0')+'_Flux_Mult']
+        # df_Electron_Flux_Mult = pd.DataFrame(Electron_Flux_Mult)  # get dataframe from dict - not needed atm.
+
+        meta['Electron_Flux_Mult'] = Electron_Flux_Mult
 
     meta['df_rtn_desc'] = cdf.varattsget('RTN')['CATDESC']
-    # TODO: add to meta: 'Sector_Bins_Text', 'Sector_Bins_Low_Energy', 'Sector_Bins_Width' -- don't exist in new data product?
 
     del cdf
 
-    # use sunpy to get Pandas DataFrame of EPOCH_X-dependent variables
-    # data = TimeSeries(files, concatenate=True)
-    # df = data.to_dataframe()
-    # del(data)
-
     df = pd.DataFrame()
+    df_rtn = pd.DataFrame()
+    df_hci = pd.DataFrame()
     for f in files:
         print('Loading', f)
-        data = TimeSeries(f, concatenate=True)
-        tdf = data.to_dataframe()
-        all_columns = False
+        # data = TimeSeries(f, concatenate=True)
+        ignore_vars = []
+        if not all_columns:
+            # TODO: so far only for new STEP data
+            ignore_vars = ignore_vars + ['Integral_01_Rate', 'Integral_02_Rate', 'Integral_03_Rate', 'Integral_04_Rate', 'Integral_05_Rate', 'Integral_06_Rate',
+                                         'Integral_07_Rate', 'Integral_08_Rate', 'Integral_09_Rate', 'Integral_10_Rate', 'Integral_11_Rate', 'Integral_12_Rate',
+                                         'Integral_13_Rate', 'Integral_14_Rate', 'Integral_15_Rate', 'Magnet_01_Rate', 'Magnet_02_Rate', 'Magnet_03_Rate', 'Magnet_04_Rate',
+                                         'Magnet_05_Rate', 'Magnet_06_Rate', 'Magnet_07_Rate', 'Magnet_08_Rate', 'Magnet_09_Rate', 'Magnet_10_Rate', 'Magnet_11_Rate',
+                                         'Magnet_12_Rate', 'Magnet_13_Rate', 'Magnet_14_Rate', 'Magnet_15_Rate', 'Integral_00_Rate', 'Magnet_00_Rate']
+        if only_averages:
+            # TODO: so far only for new STEP data
+            ignore_vars = ignore_vars + ['Integral_01_Flux', 'Integral_01_Uncertainty', 'Integral_02_Flux', 'Integral_02_Uncertainty',
+                                         'Integral_03_Flux', 'Integral_03_Uncertainty', 'Integral_04_Flux', 'Integral_04_Uncertainty',
+                                         'Integral_05_Flux', 'Integral_05_Uncertainty', 'Integral_06_Flux', 'Integral_06_Uncertainty',
+                                         'Integral_07_Flux', 'Integral_07_Uncertainty', 'Integral_08_Flux', 'Integral_08_Uncertainty',
+                                         'Integral_09_Flux', 'Integral_09_Uncertainty', 'Integral_10_Flux', 'Integral_10_Uncertainty',
+                                         'Integral_11_Flux', 'Integral_11_Uncertainty', 'Integral_12_Flux', 'Integral_12_Uncertainty',
+                                         'Integral_13_Flux', 'Integral_13_Uncertainty', 'Integral_14_Flux', 'Integral_14_Uncertainty',
+                                         'Integral_15_Flux', 'Integral_15_Uncertainty', 'Magnet_01_Flux', 'Magnet_01_Uncertainty',
+                                         'Magnet_02_Flux', 'Magnet_02_Uncertainty', 'Magnet_03_Flux', 'Magnet_03_Uncertainty',
+                                         'Magnet_04_Flux', 'Magnet_04_Uncertainty', 'Magnet_05_Flux', 'Magnet_05_Uncertainty',
+                                         'Magnet_06_Flux', 'Magnet_06_Uncertainty', 'Magnet_07_Flux', 'Magnet_07_Uncertainty',
+                                         'Magnet_08_Flux', 'Magnet_08_Uncertainty', 'Magnet_09_Flux', 'Magnet_09_Uncertainty',
+                                         'Magnet_10_Flux', 'Magnet_10_Uncertainty', 'Magnet_11_Flux', 'Magnet_11_Uncertainty',
+                                         'Magnet_12_Flux', 'Magnet_12_Uncertainty', 'Magnet_13_Flux', 'Magnet_13_Uncertainty',
+                                         'Magnet_14_Flux', 'Magnet_14_Uncertainty', 'Magnet_15_Flux', 'Magnet_15_Uncertainty']
+        tss = _read_cdf_mod(f, ignore_vars=ignore_vars)
+        # data = tss.pop(0)
+        # for ts in tss:
+        #     data = data.concatenate(ts)
+        # tdf = data.to_dataframe()
+        tdf = tss[0].to_dataframe()
+        tdf_rtn = tss[1].to_dataframe()
+        tdf_hci = tss[2].to_dataframe()
         if not all_columns:
-            # print('dropping Rates from tdf')
+            # should be removed here; better use ignore_vars above to prohibit that the columns are loaded in the first place
             tdf.drop(columns=tdf.filter(like='Rate').columns, inplace=True)
         # drop per-Pixel data from tdf
         if only_averages:
-            # print('dropping Pixels from tdf')
             drop_cols = ['Integral_0', 'Integral_1', 'Magnet_0', 'Magnet_1']
             for col in drop_cols:
                 tdf.drop(columns=tdf.filter(like=col).columns, inplace=True)
-        # print('merge dataframes...')
+        # merge dataframes
         df = pd.concat([df, tdf])
-        del (data, tdf)
+        df_rtn = pd.concat([df_rtn, tdf_rtn])
+        df_hci = pd.concat([df_hci, tdf_hci])
+        del (tss, tdf, tdf_rtn, tdf_hci)
 
     # move RTN and HCI to different df's because they have different time indices
     # print('move RTN')
-    df_rtn = df[['RTN_0', 'RTN_1', 'RTN_2']].dropna(how='all')
-    df = df.drop(columns=['RTN_0', 'RTN_1', 'RTN_2']).dropna(how='all')  # remove lines only containing NaN's (all)
+    # df_rtn = df[['RTN_0', 'RTN_1', 'RTN_2']].dropna(how='all')
+    # df = df.drop(columns=['RTN_0', 'RTN_1', 'RTN_2']).dropna(how='all')  # remove lines only containing NaN's (all)
     # print('move HCI')
-    df_hci = df[['HCI_Lat', 'HCI_Lon', 'HCI_R']].dropna(how='all')
-    df = df.drop(columns=['HCI_Lat', 'HCI_Lon', 'HCI_R']).dropna(how='all')  # remove lines only containing NaN's (all)
+    # df_hci = df[['HCI_Lat', 'HCI_Lon', 'HCI_R']].dropna(how='all')
+    # df = df.drop(columns=['HCI_Lat', 'HCI_Lon', 'HCI_R']).dropna(how='all')  # remove lines only containing NaN's (all)
     meta['df_rtn'] = df_rtn
     del df_rtn
     meta['df_hci'] = df_hci
     del df_hci
 
     """
     # what to do with this? not read in by sunpy because of multi-dimensionality. skip for now
@@ -1034,19 +1092,66 @@
     meta['RTN_Pixels'] = 'CDF var RTN_Pixels (Particle flow direction (unit vector) in RTN coordinates for each pixel) left out as of now because it is multidimensional'
 
     """
     Electron_Flux calculation moved to own function that includes correct resampling. For Now, it should be called independently.
     df = calc_electrons(df, meta, contamination_threshold=contamination_threshold, only_averages=only_averages, resample=False)
     """
 
+    # define old STEP data electron multiplication factors
+    if 'Electron_Flux_Mult' not in meta.keys():
+        if df.index[0] <= pd.Timestamp(dt.date(2021, 10, 22)):  # old STEP data
+            meta['Electron_Flux_Mult'] = {'Electron_Avg_Flux_Mult': np.array([0.6, 0.61, 0.63, 0.68, 0.76, 0.81, 1.06, 1.32, 1.35, 1.35, 1.35,
+                                                                              1.34, 1.34, 1.35, 1.38, 1.36, 1.32, 1.32, 1.28, 1.26, 1.15, 1.15,
+                                                                              1.15, 1.15, 1.16, 1.16, 1.16, 1.17, 1.17, 1.16, 1.18, 1.17, 1.17,
+                                                                              1.16, 1.17, 1.15, 1.16, 1.17, 1.18, 1.17, 1.17, 1.17, 1.18, 1.18,
+                                                                              1.19, 1.18, 1.19, 1.2])}
+            for i in range(1, 16):
+                meta['Electron_Flux_Mult']['Electron_'+str(i).rjust(2, '0')+'_Flux_Mult'] = np.array([0.66, 1.22, 1.35, 1.36, 1.18, 1.17, 1.16, 1.18])
+
+    # define old STEP data electron energy values
+    if 'Electron_Bins_Low_Energy' not in meta.keys():
+        if 'Electron_Avg_Bins_Low_Energy' not in meta.keys():
+            if df.index[0] <= pd.Timestamp(dt.date(2021, 10, 22)):  # old STEP data
+                meta['Electron_Avg_Bins_Low_Energy'] = np.array([4.09, 4.37, 4.56, 4.83, 5.17, 5.4, 5.65, 5.96, 6.42,
+                                                                 6.7, 7.05, 9.06, 9.81, 10.25, 10.69, 11.71, 12.21, 12.73,
+                                                                 13.87, 14.45, 15.09, 16.43, 17.19, 18.72, 19.5, 20.4, 22.32,
+                                                                 23.34, 24.32, 26.54, 27.65, 28.83, 31.35, 32.77, 35.88, 37.4,
+                                                                 38.92, 42.55, 44.6, 46.65, 50.7, 53.04, 55.34, 60.21, 62.73,
+                                                                 68.55, 71.66, 74.84])
+                meta['Electron_Avg_Bins_High_Energy'] = np.array([4.57, 4.79, 4.97, 5.31, 5.55, 5.78, 6.03, 6.48, 6.78,
+                                                                  7.07, 9.06, 9.81, 10.25, 10.69, 11.71, 12.21, 12.73, 13.87,
+                                                                  14.45, 15.09, 16.43, 17.19, 18.72, 19.5, 20.4, 22.32, 23.34,
+                                                                  24.32, 26.54, 27.65, 28.83, 31.35, 32.77, 35.88, 37.4, 38.92,
+                                                                  42.55, 44.6, 46.65, 50.7, 53.04, 55.34, 60.21, 62.73, 68.55,
+                                                                  71.66, 74.84, 81.36])
+                meta['Electron_Avg_Bins_Text'] = np.array([[f"{meta['Electron_Avg_Bins_Low_Energy'][i]} - {meta['Electron_Avg_Bins_High_Energy'][i]} keV"] for i in range(len(meta['Electron_Avg_Bins_High_Energy']))])
+                meta['Electron_Avg_Bins_Low_Energy'] = meta['Electron_Avg_Bins_Low_Energy']/1000  # convert from keV to MeV for consistency with new STEP data
+                meta['Electron_Avg_Bins_High_Energy'] = meta['Electron_Avg_Bins_High_Energy']/1000  # convert from keV to MeV for consistency with new STEP data
+                meta['Electron_Avg_Bins_Width'] = meta['Electron_Avg_Bins_High_Energy'] - meta['Electron_Avg_Bins_Low_Energy']
+
+                meta['Electron_Sectors_Bins_Low_Energy'] = np.array([4.19, 5.50, 7.04, 9.06, 13.88, 21.29, 32.77, 53.05])
+                meta['Electron_Sectors_Bins_High_Energy'] = np.array([5.50, 7.04, 9.06, 13.88, 21.29, 32.77, 53.05, 81.38])
+                meta['Electron_Sectors_Bins_Text'] = np.array([[f"{meta['Electron_Sectors_Bins_Low_Energy'][i]} - {meta['Electron_Sectors_Bins_High_Energy'][i]} keV"] for i in range(len(meta['Electron_Sectors_Bins_High_Energy']))])
+                meta['Electron_Sectors_Bins_Low_Energy'] = meta['Electron_Sectors_Bins_Low_Energy']/1000  # convert from keV to MeV for consistency with new STEP data
+                meta['Electron_Sectors_Bins_High_Energy'] = meta['Electron_Sectors_Bins_High_Energy']/1000  # convert from keV to MeV for consistency with new STEP data
+                meta['Electron_Sectors_Bins_Width'] = meta['Electron_Sectors_Bins_High_Energy'] - meta['Electron_Sectors_Bins_Low_Energy']
+
+    # add 'Avg' to old STEP data product's corresponding columns (Magnet_Flux_0 => Magnet_Avg_Flux_0) in order to be consistent with new data product
+    avg_dict = {}
+    for col in df.columns.to_list():
+        if col.startswith('Integral_Rate_') or col.startswith('Integral_Flux_') or col.startswith('Integral_Uncertainty_') or \
+           col.startswith('Magnet_Rate_') or col.startswith('Magnet_Flux_') or col.startswith('Magnet_Uncertainty_'):
+            avg_dict[col] = col.replace(col.split('_')[0], col.split('_')[0]+'_Avg')
+    df.rename(columns=avg_dict, inplace=True)
+
     # TODO: replace all negative values in dataframe with np.nan (applies for electron fluxes that get negative in their calculation)
     # ==> not needed any more after masking above?
     # df = df.mask(df < 0)
 
-    # TODO: multi-index (or rather multi-column) dataframe like previous product?
+    # TODO: multi-index (or rather multi-column) dataframe like previous product? => create_multiindex(df)
 
     # df3['QUALITY_FLAG'] = df['QUALITY_FLAG']
     # df3['QUALITY_BITMASK'] = df['QUALITY_BITMASK']
     # df3['SMALL_PIXELS_FLAG'] = df['SMALL_PIXELS_FLAG']
 
     return df, meta
 
@@ -1122,42 +1227,60 @@
     # create list of electron fluxes to be calculated: only average or average + all individual pixels:
     if only_averages:
         pix_list = ['Avg']
     else:
         pix_list = ['Avg']+[str(n).rjust(2, '0') for n in range(1, 16)]
 
     # calculate electron fluxes from Magnet and Integral Fluxes using correction factors
-    for i in range(len(Electron_Flux_Mult['Electron_Avg_Flux_Mult'])):  # 32 energy channels
-        for pix in pix_list:  # Avg, pixel 01 - 15 (00 is background pixel)
-            df[f'Electron_{pix}_Flux_{i}'] = Electron_Flux_Mult[f'Electron_{pix}_Flux_Mult'][i] * (df[f'Integral_{pix}_Flux_{i}'] - df[f'Magnet_{pix}_Flux_{i}'])
-            df[f'Electron_{pix}_Uncertainty_{i}'] = \
-                Electron_Flux_Mult[f'Electron_{pix}_Flux_Mult'][i] * np.sqrt(df[f'Integral_{pix}_Uncertainty_{i}']**2 + df[f'Magnet_{pix}_Uncertainty_{i}']**2)
-
-            if type(contamination_threshold) == int:
-                if contamination_threshold != 0:
-                    clean = (df[f'Integral_{pix}_Flux_{i}'] - df[f'Magnet_{pix}_Flux_{i}']) > contamination_threshold*df[f'Integral_{pix}_Uncertainty_{i}']
-                    # clean = (df[f'Integral_{pix}_Rate_{i}'] - df[f'Magnet_{pix}_Rate_{i}']) > contamination_threshold*np.sqrt(df[f'Integral_{pix}_Rate_{i}'])/np.sqrt(df['DELTA_EPOCH'])
-                    # clean = (df[f'Integral_{pix}_Rate_{i}'] - df[f'Magnet_{pix}_Rate_{i}']) > contamination_threshold*np.sqrt(df[f'Integral_{pix}_Counts_{i}'])/df['DELTA_EPOCH']
-
-                    # mask non-clean data
-                    df[f'Electron_{pix}_Flux_{i}'] = df[f'Electron_{pix}_Flux_{i}'].mask(~clean)
-                    df[f'Electron_{pix}_Uncertainty_{i}'] = df[f'Electron_{pix}_Uncertainty_{i}'].mask(~clean)
+    # for old data, calculation needs to be separated for Avg and pixels bc. of different amount of energy channels (48 vs 8):
+    if not only_averages and len(Electron_Flux_Mult['Electron_Avg_Flux_Mult']) != len(Electron_Flux_Mult['Electron_01_Flux_Mult']):
+        # Avg only:
+        pix = pix_list.pop(0)
+        for i in range(len(Electron_Flux_Mult['Electron_Avg_Flux_Mult'])):  # 48 energy channels for old data (for Avg)
+            df = _calc_electrons_per_pixel_and_channel(df, Electron_Flux_Mult, pix, contamination_threshold, i)
+        # all pixels, without Avg:
+        for i in range(len(Electron_Flux_Mult['Electron_01_Flux_Mult'])):  # 8 energy channels for old data (per pixel)
+            for pix in pix_list:  # pixel 01 - 15 (00 is background pixel)
+                df = _calc_electrons_per_pixel_and_channel(df, Electron_Flux_Mult, pix, contamination_threshold, i)
+    else:  # classic approach:
+        for i in range(len(Electron_Flux_Mult['Electron_Avg_Flux_Mult'])):  # 32 energy channels for new data, 48 for old data (Avg)
+            for pix in pix_list:  # Avg, pixel 01 - 15 (00 is background pixel)
+                df = _calc_electrons_per_pixel_and_channel(df, Electron_Flux_Mult, pix, contamination_threshold, i)
 
     if contamination_threshold == 0:
         print("contamination_threshold has been set to 0. Ignoring the contamination_threshold (i.e., NOT calculating it for 0)!")
 
     if type(contamination_threshold) != int:
         print("Info: contamination_threshold will only be applied if it is an integer. Otherwise only negative fluxes are removed.")
 
     # remove negative fluxes (probably not needed for masked data, but for contamination_threshold=None)
     df = df.mask(df < 0)
 
     return df
 
 
+def _calc_electrons_per_pixel_and_channel(df, Electron_Flux_Mult, pixel, contamination_threshold, energy_channel):
+    pix = pixel
+    i = energy_channel
+    df[f'Electron_{pix}_Flux_{i}'] = Electron_Flux_Mult[f'Electron_{pix}_Flux_Mult'][i] * (df[f'Integral_{pix}_Flux_{i}'] - df[f'Magnet_{pix}_Flux_{i}'])
+    df[f'Electron_{pix}_Uncertainty_{i}'] = \
+        Electron_Flux_Mult[f'Electron_{pix}_Flux_Mult'][i] * np.sqrt(df[f'Integral_{pix}_Uncertainty_{i}']**2 + df[f'Magnet_{pix}_Uncertainty_{i}']**2)
+
+    if type(contamination_threshold) == int:
+        if contamination_threshold != 0:
+            clean = (df[f'Integral_{pix}_Flux_{i}'] - df[f'Magnet_{pix}_Flux_{i}']) > contamination_threshold*df[f'Integral_{pix}_Uncertainty_{i}']
+            # clean = (df[f'Integral_{pix}_Rate_{i}'] - df[f'Magnet_{pix}_Rate_{i}']) > contamination_threshold*np.sqrt(df[f'Integral_{pix}_Rate_{i}'])/np.sqrt(df['DELTA_EPOCH'])
+            # clean = (df[f'Integral_{pix}_Rate_{i}'] - df[f'Magnet_{pix}_Rate_{i}']) > contamination_threshold*np.sqrt(df[f'Integral_{pix}_Counts_{i}'])/df['DELTA_EPOCH']
+
+            # mask non-clean data
+            df[f'Electron_{pix}_Flux_{i}'] = df[f'Electron_{pix}_Flux_{i}'].mask(~clean)
+            df[f'Electron_{pix}_Uncertainty_{i}'] = df[f'Electron_{pix}_Uncertainty_{i}'].mask(~clean)
+    return df
+
+
 def _calc_electrons_rates(df, meta, contamination_threshold=2, only_averages=False, resample=False):
     """
     Outdated version of calc_electrons() that used rates to calculate counts, which are then used to calculate resampled uncertainties
     """
     df = df.copy()
 
     Electron_Flux_Mult = meta['Electron_Flux_Mult']
@@ -1292,7 +1415,171 @@
             df.index = df.index + pd.tseries.frequencies.to_offset(pd.Timedelta(resample)/2)
         # if pos_timestamp == 'stop' or pos_timestamp == 'end':
         #     df.index = df.index + pd.tseries.frequencies.to_offset(pd.Timedelta(resample))
     except ValueError:
         raise ValueError(f"Your 'resample' option of [{resample}] doesn't seem to be a proper Pandas frequency!")
 
     return df
+
+
+def create_multiindex(df):
+    """
+    Create a multiindex dataframe from a standard dataframe. The input standard
+    dataframe is expected to be provided by SunPy read_cdf() or TimeSeries() for
+    multidimensional data. That is, the dataframe columns are named 'VAR_0',
+    'VAR_1', 'VAR_2' and so on. Multiindex dataframe will then have a column
+    named 'VAR' with sub-columns 'VAR_0', 'VAR_1', 'VAR_2'.
+    """
+    cols = df.columns.to_list()
+    arrays = [np.copy(cols), np.copy(cols)]
+    for i, item in enumerate(cols):
+        if item[-1].isnumeric():
+            arrays[0][i] = "_".join(item.split("_")[:-1])
+
+    # https://pandas.pydata.org/pandas-docs/stable/user_guide/advanced.html
+    tuples = list(zip(*arrays))
+    index = pd.MultiIndex.from_tuples(tuples)
+
+    df = pd.DataFrame(df.values, index=df.index, columns=index)
+    #  df.index.names = ['Time']
+    return df
+
+
+"""
+Modification of sunpy's read_cdf function to allow skipping of reading variables from a cdf file.
+This function is copied from sunpy under the terms of the BSD 2-Clause licence. See licenses/SUNPY_LICENSE.rst
+"""
+
+
+def _read_cdf_mod(fname, ignore_vars=[]):
+    """
+    Read a CDF file that follows the ISTP/IACG guidelines.
+
+    Parameters
+    ----------
+    fname : path-like
+        Location of single CDF file to read.
+
+    Returns
+    -------
+    list[GenericTimeSeries]
+        A list of time series objects, one for each unique time index within
+        the CDF file.
+
+    References
+    ----------
+    Space Physics Guidelines for CDF https://spdf.gsfc.nasa.gov/sp_use_of_cdf.html
+    """
+    import astropy.units as u
+    from cdflib.epochs import CDFepoch
+    from sunpy import log
+    from sunpy.timeseries import GenericTimeSeries
+    from sunpy.util.exceptions import warn_user
+    cdf = cdflib.CDF(str(fname))
+    # Extract the time varying variables
+    cdf_info = cdf.cdf_info()
+    meta = cdf.globalattsget()
+    if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+        all_var_keys = cdf_info.rVariables + cdf_info.zVariables
+    else:
+        all_var_keys = cdf_info['rVariables'] + cdf_info['zVariables']
+    var_attrs = {key: cdf.varattsget(key) for key in all_var_keys}
+    # Get keys that depend on time
+    var_keys = [var for var in var_attrs if 'DEPEND_0' in var_attrs[var] and var_attrs[var]['DEPEND_0'] is not None]
+
+    # Get unique time index keys
+    time_index_keys = sorted(set([var_attrs[var]['DEPEND_0'] for var in var_keys]))
+
+    all_ts = []
+    # For each time index, construct a GenericTimeSeries
+    for index_key in time_index_keys:
+        try:
+            index = cdf.varget(index_key)
+        except ValueError:
+            # Empty index for cdflib >= 0.3.20
+            continue
+        # TODO: use to_astropy_time() instead here when we drop pandas in timeseries
+        index = CDFepoch.to_datetime(index)
+        df = pd.DataFrame(index=pd.DatetimeIndex(name=index_key, data=index))
+        units = {}
+
+        for var_key in sorted(var_keys):
+            if var_key in ignore_vars:
+                continue  # leave for-loop, skipping var_key
+
+            attrs = var_attrs[var_key]
+            # If this variable doesn't depend on this index, continue
+            if attrs['DEPEND_0'] != index_key:
+                continue
+
+            # Get data
+            if hasattr(cdflib, "__version__") and Version(cdflib.__version__) >= Version("1.0.0"):
+                var_last_rec = cdf.varinq(var_key).Last_Rec
+            else:
+                var_last_rec = cdf.varinq(var_key)['Last_Rec']
+            if var_last_rec == -1:
+                log.debug(f'Skipping {var_key} in {fname} as it has zero elements')
+                continue
+
+            data = cdf.varget(var_key)
+
+            # Set fillval values to NaN
+            # It would be nice to properley mask these values to work with
+            # non-floating point (ie. int) dtypes, but this is not possible with pandas
+            if np.issubdtype(data.dtype, np.floating):
+                data[data == attrs['FILLVAL']] = np.nan
+
+            # Get units
+            if 'UNITS' in attrs:
+                unit_str = attrs['UNITS']
+                try:
+                    unit = u.Unit(unit_str)
+                except ValueError:
+                    if unit_str in _known_units:
+                        unit = _known_units[unit_str]
+                    else:
+                        warn_user(f'astropy did not recognize units of "{unit_str}". '
+                                  'Assigning dimensionless units. '
+                                  'If you think this unit should not be dimensionless, '
+                                  'please raise an issue at https://github.com/sunpy/sunpy/issues')
+                        unit = u.dimensionless_unscaled
+            else:
+                warn_user(f'No units provided for variable "{var_key}". '
+                          'Assigning dimensionless units.')
+                unit = u.dimensionless_unscaled
+
+            if data.ndim > 3:
+                # Skip data with dimensions >= 3 and give user warning
+                warn_user(f'The variable "{var_key}" has been skipped because it has more than 3 dimensions, which is unsupported.')
+            elif data.ndim == 3:
+                # Multiple columns, give each column a unique label.
+                # Numbering hard-corded to SolO/EPD/STEP (old) data!
+                if var_key.startswith('Sector_'):
+                    for j in range(data.T.shape[0]):
+                        for i, col in enumerate(data.T[j, :, :]):
+                            var_key_mod = var_key.removeprefix('Sector_')
+                            var_key_mod = var_key_mod.replace('_', '_'+str(j+1).rjust(2, '0')+'_')  # j+1: numbering hard-corded to SolO/EPD/STEP (old) data!
+                            df[var_key_mod + f'_{i}'] = col
+                            units[var_key_mod + f'_{i}'] = unit
+                elif var_key == 'RTN_Sectors' or var_key == 'RTN_Pixels':
+                    for j in range(data.T.shape[1]):
+                        for i, col in enumerate(data.T[:, j, :]):
+                            var_key_mod = var_key+'_'+str(j+1).rjust(2, '0')  # j+1: numbering hard-corded to SolO/EPD/STEP (old) data!
+                            df[var_key_mod + f'_{i}'] = col
+                            units[var_key_mod + f'_{i}'] = unit
+                else:
+                    warn_user(f'The variable "{var_key}" has been skipped because it is unsupported.')
+            elif data.ndim == 2:
+                # Multiple columns, give each column a unique label
+                for i, col in enumerate(data.T):
+                    df[var_key + f'_{i}'] = col
+                    units[var_key + f'_{i}'] = unit
+            else:
+                # Single column
+                df[var_key] = data
+                units[var_key] = unit
+
+        all_ts.append(GenericTimeSeries(data=df, units=units, meta=meta))
+
+    if not len(all_ts):
+        log.debug(f'No data found in file {fname}')
+    return all_ts
```

### Comparing `solo_epd_loader-0.2.8/solo_epd_loader.egg-info/PKG-INFO` & `solo_epd_loader-0.3.0/solo_epd_loader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo-epd-loader
-Version: 0.2.8
+Version: 0.3.0
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -43,16 +43,16 @@
 - Electron Proton Telescope (EPT)
 - High Energy Telescope (HET)
 - SupraThermal Electrons and Protons (STEP)
 
 Current caveats:
 
 - Only the standard ``rates`` data products are supported (i.e., no ``burst`` or ``high cadence`` data).
-- Only electrons, protons and alpha particles are processed (i.e., for HET He3, He4, C, N, O, Fe are omitted at the moment).
-- For the old STEP data product (until Oct 22, 2021), the sectored data is not processed (i.e., only averaged data is supported) and electron data needs to be calculated manually.
+- For EPT and HET, only electrons, protons and alpha particles are processed (i.e., for HET He3, He4, C, N, O, Fe are omitted at the moment).
+- For STEP, electron data needs to be calculated manually.
 - The Suprathermal Ion Spectrograph (SIS) is not yet included. 
 
 Disclaimer
 ----------
 This software is provided "as is", with no guarantee. It is no official data source, and not officially endorsed by the corresponding instrument teams. **Please always refer to the** `official EPD data description <http://espada.uah.es/epd/EPD_data.php>`_ **before using the data!**
 
 Installation
@@ -266,15 +266,15 @@
    # plot selection of ept electron channels
    for channel in [0, 8, 16, 26]:
       df_electrons_ept['Electron_Flux'][f'Electron_Flux_{channel}'].resample(resample).mean().plot(
          ax = axs[0], logy=True, label='EPT '+energies_ept["Electron_Bins_Text"][channel][0])
 
    # plot selection of step ion channels
    for channel in [8, 17, 33]:
-      df_step['Magnet_Flux'][channel].resample(resample).mean().plot(
+      df_step[f'Magnet_Avg_Flux_{channel}'].resample(resample).mean().plot(
          ax = axs[1], logy=True, label='STEP '+energies_step["Bins_Text"][channel][0])
 
    # plot selection of ept ion channels
    for channel in [6, 22, 32, 48]:
       df_protons_ept['Ion_Flux'][f'Ion_Flux_{channel}'].resample(resample).mean().plot(
          ax = axs[1], logy=True, label='EPT '+energies_ept["Ion_Bins_Text"][channel][0])
```

### Comparing `solo_epd_loader-0.2.8/solo_epd_loader.egg-info/SOURCES.txt` & `solo_epd_loader-0.3.0/solo_epd_loader.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 examples/gh2021_fig_2.png
 examples/ws2021_fig_2d.png
 licenses/LICENSE.rst
+licenses/SUNPY_LICENSE.rst
 licenses/TEMPLATE_LICENSE.rst
 solo_epd_loader/__init__.py
 solo_epd_loader/version.py
 solo_epd_loader.egg-info/PKG-INFO
 solo_epd_loader.egg-info/SOURCES.txt
 solo_epd_loader.egg-info/dependency_links.txt
 solo_epd_loader.egg-info/not-zip-safe
```

### Comparing `solo_epd_loader-0.2.8/tox.ini` & `solo_epd_loader-0.3.0/tox.ini`

 * *Files identical despite different names*

