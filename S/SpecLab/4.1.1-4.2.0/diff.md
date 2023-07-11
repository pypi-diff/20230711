# Comparing `tmp/SpecLab-4.1.1.tar.gz` & `tmp/SpecLab-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpecLab-4.1.1.tar", last modified: Thu Jun 29 00:35:05 2023, max compression
+gzip compressed data, was "SpecLab-4.2.0.tar", last modified: Tue Jul 11 15:56:28 2023, max compression
```

## Comparing `SpecLab-4.1.1.tar` & `SpecLab-4.2.0.tar`

### file list

```diff
@@ -1,30 +1,38 @@
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/SpecLab/
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/SpecLab/imXam/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-05-30 23:51:42.000000 SpecLab-4.1.1/SpecLab/imXam/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    48692 2023-06-29 00:34:32.000000 SpecLab-4.1.1/SpecLab/imXam/imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/SpecLab/cfg/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2025 2023-06-14 20:25:01.000000 SpecLab-4.1.1/SpecLab/cfg/SpecLab_config.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-06-15 15:54:47.000000 SpecLab-4.1.1/SpecLab/cfg/epar_imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/SpecLab/gen/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53081 2023-06-28 23:09:48.000000 SpecLab-4.1.1/SpecLab/gen/SpecLabFunctions.py
--rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-06-02 18:44:11.000000 SpecLab-4.1.1/SpecLab/gen/globals.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:30.000000 SpecLab-4.1.1/SpecLab/gen/__init__.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-06-14 19:40:28.000000 SpecLab-4.1.1/SpecLab/gen/myfunc.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-01 23:14:48.000000 SpecLab-4.1.1/SpecLab/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/SpecLab/aux/
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/SpecLab/aux/param_files/
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-06-26 18:07:15.000000 SpecLab-4.1.1/SpecLab/aux/param_files/imXam_param.default.dat
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:07.000000 SpecLab-4.1.1/SpecLab/aux/param_files/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-06-26 18:06:59.000000 SpecLab-4.1.1/SpecLab/aux/param_files/imXam_param_ARCES.dat
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-06-26 18:06:44.000000 SpecLab-4.1.1/SpecLab/aux/param_files/imXam_param.dat
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:21:46.000000 SpecLab-4.1.1/SpecLab/aux/__init__.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)   619019 2023-06-29 00:31:34.000000 SpecLab-4.1.1/SpecLab/aux/pyqtgraph10_speclab.tar.gz
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/SpecLab/doc/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:19.000000 SpecLab-4.1.1/SpecLab/doc/__init__.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      592 2023-06-29 00:34:03.000000 SpecLab-4.1.1/SpecLab/doc/CHANGELOG.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     4715 2023-06-29 00:32:54.000000 SpecLab-4.1.1/SpecLab/doc/README.md
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1073 2023-06-29 00:33:05.000000 SpecLab-4.1.1/SpecLab/doc/KNOWN_ISSUES.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-06-14 15:39:40.000000 SpecLab-4.1.1/SpecLab/doc/LICENSE.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     6496 2023-06-29 00:35:05.000000 SpecLab-4.1.1/PKG-INFO
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1389 2023-06-29 00:34:54.000000 SpecLab-4.1.1/setup.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5081 2023-07-11 15:56:28.575577 SpecLab-4.2.0/PKG-INFO
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     4827 2023-07-11 15:47:12.000000 SpecLab-4.2.0/README.md
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab/aux/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/aux/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab/aux/param_files/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/aux/param_files/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/aux/param_files/imXam_param.dat
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/aux/param_files/imXam_param.default.dat
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/aux/param_files/imXam_param_ARCES.dat
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    36728 2023-07-11 15:31:38.000000 SpecLab-4.2.0/SpecLab/aux/pyqtgraph_modifications.tar.gz
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab/cfg/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2166 2023-07-11 15:37:55.000000 SpecLab-4.2.0/SpecLab/cfg/SpecLab_config.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/cfg/epar_imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab/doc/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      689 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/doc/CHANGELOG.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1073 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/doc/KNOWN_ISSUES.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/doc/LICENSE.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     4827 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/doc/README.md
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/doc/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab/gen/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53081 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/gen/SpecLabFunctions.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/gen/__init__.py
+-rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/gen/globals.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/gen/myfunc.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab/imXam/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.0/SpecLab/imXam/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    49771 2023-07-11 15:40:44.000000 SpecLab-4.2.0/SpecLab/imXam/imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-11 15:56:28.575577 SpecLab-4.2.0/SpecLab.egg-info/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5081 2023-07-11 15:56:28.000000 SpecLab-4.2.0/SpecLab.egg-info/PKG-INFO
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      760 2023-07-11 15:56:28.000000 SpecLab-4.2.0/SpecLab.egg-info/SOURCES.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        1 2023-07-11 15:56:28.000000 SpecLab-4.2.0/SpecLab.egg-info/dependency_links.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      138 2023-07-11 15:56:28.000000 SpecLab-4.2.0/SpecLab.egg-info/requires.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        8 2023-07-11 15:56:28.000000 SpecLab-4.2.0/SpecLab.egg-info/top_level.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)       38 2023-07-11 15:56:28.575577 SpecLab-4.2.0/setup.cfg
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1476 2023-07-11 15:56:25.000000 SpecLab-4.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `SpecLab-4.1.1/SpecLab/imXam/imXam.py` & `SpecLab-4.2.0/SpecLab/imXam/imXam.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 #!/usr/bin/env python
 
+# export QT_QPA_PLATFORM=offscreen
+#  https://stackoverflow.com/questions/68036484/qt6-qt-qpa-plugin-could-not-load-the-qt-platform-plugin-xcb-in-even-thou/68058308#68058308
+
 import numpy as np
-from pyqtgraph10_speclab.Qt import QtCore, QtGui
-import pyqtgraph10_speclab as pg
-from pyqtgraph10_speclab import PlotWidget, plot
-from pyqtgraph10_speclab.Point import Point
+from pyqtgraph.Qt import QtCore, QtGui, QtWidgets
+import pyqtgraph as pg
+from pyqtgraph import PlotWidget, plot
+from pyqtgraph.Point import Point
 from astropy.io import fits
 import astropy.io.ascii as ascii
 from scipy.interpolate import RegularGridInterpolator
 import matplotlib
 import matplotlib.pyplot as plt
-from PyQt5 import QtWidgets
-from PyQt5.QtCore import pyqtRemoveInputHook
-from PyQt5.QtCore import QCoreApplication
 from photutils.aperture import CircularAperture, CircularAnnulus
 from photutils.aperture import aperture_photometry
 from matplotlib.backend_bases import key_press_handler
 from photutils.centroids import centroid_2dg
 import sys
 import scipy, scipy.optimize
 import matplotlib.pyplot as plt
 import os
 from matplotlib.patches import Circle
 import plotly.graph_objects as go
+#os.environ['QT_QPA_PLATFORM'] = 'offscreen'
+
+#export QT_DEBUG_PLUGINS=1
 
 # updates 2023 (v4.0.5)
 ##  renamed from imxam.py to imXam.py so as to not interfere with astropys dist
 ##  replaced mpld3 with plotly
 ##  cubic spline added
 ##  g, x, t keys all work for KOSMOS spectra as long as -dispax 2 is set
 ##  cube_val should have a value with a single .fits is read in and there is a datacube.
@@ -36,15 +39,15 @@
 ##  Changed l2 to irisras, and irisras now takes a value corresponding to the image to plot starting from 0, same for value following -cube
 ##  Added keyword scube so now can subtract a preflare image if -cube is used.  Check 'threshold' key 'T' ...
 ##  Added such that lastheader.txt is automatically opened from 'H' key use.  
 ##  Many more things:  ....
 
 ## see KNOWN_ISSUES file 
 
-# 5/30/23:  SpecLab_config.py, this now uses pyqtgraph10_speclab/ in site-packages.
+# 7/11/23:  SpecLab_config.py, this copies over several routines in PyQtGraph so that they work with imXam functionality.
 # ======================
 
 import site
 
 your_site_packages_location = site.getsitepackages()
 
 imexam_path = your_site_packages_location[0]+'/SpecLab/aux/param_files/' # this is default location of default imXam_param.dat
@@ -83,15 +86,15 @@
     z2_zscale = imclean[midpoint] + (coeffsz[0] / 1.0) * (npoints - midpoint)
     return z1_zscale, z2_zscale
 
 
 
 print('======================================================')
 print('======================================================')
-print('imXam: adam f kowalski, v4.1.1: June 28, 2023')
+print('imXam: v4.2.0 (July 11, 2023)')
 print(' To shut down gui, type q into terminal, type h for interactive commands, use middle mouse wheel to zoom in and out')
 print(' You may have to click on gui with left mouse button in order to use interactive commands')
 print(' To get a list of command-line options, type imXam.py -h from a terminal.')
 print('======================================================')
 print('imXam.py located in ',your_site_packages_location[0]+'/SpecLab/imXam/')
 print(' and .../anaconda3/envs/<your_env_name>/bin/')
 print('Default param files located in ',your_site_packages_location[0]+'/SpecLab/aux/param_files/')
@@ -157,15 +160,15 @@
 boxy1=[]
 box_mean =[]
 box_med = []
 box_max = []
 box_min = []
 box_std = []
 
-pyqtRemoveInputHook()
+QtCore.pyqtRemoveInputHook()
 
 args = parser.parse_args()
 
 ifile = args.filename
 
 param_file = args.param
 
@@ -186,26 +189,27 @@
 #                   'N_Contours':uparm[5][2],  'Apspec_upper':uparm[6][2], 'Apspec_lower':uparm[7][2], 'Aptrace_radius':uparm[10][2], 'Sat_Limit':uparm[11][2]}
 colid = np.array((uparm[0][:]))
 colparm = np.array(uparm[1][:])
 colval = (uparm[2][:])
 col_desc = (uparm[3][:])
 
 
-app = QtGui.QApplication([])
-
+#app = QtGui.QGuiApplication([])
+app = pg.mkQApp()
 ## Create window with two ImageView widgets
-win = QtGui.QMainWindow()
+win = QtWidgets.QMainWindow()
 
 win.statusbar = QtWidgets.QStatusBar()
 win.setStatusBar(win.statusbar)
 win.resize(1024,1024)
 win.setWindowTitle('imXam')
-cw = QtGui.QWidget()
+cw = QtWidgets.QWidget()
 win.setCentralWidget(cw)
-l = QtGui.QGridLayout()
+l = QtWidgets.QGridLayout()
+#l = QtGui.QGridLayout()
 cw.setLayout(l)
 imv1 = pg.ImageView(view=pg.PlotItem())
 imv2 = pg.PlotWidget()
 imv3 = pg.PlotWidget()
 imv4 = pg.PlotWidget()
 
 l.addWidget(imv4, 0,0,3,4)
@@ -438,83 +442,104 @@
 
         if val == 'e':
             parm_2_edit =  input('Enter integer corresponding to first column in imXam_param.dat (note: will not be saved upon quitting imXam): ')
             parm_new = input('Enter its new value: ')
             colval[int(parm_2_edit)] = parm_new
 
 
-    test = int(np.argwhere(colparm == 'Window'))
-    imw = int(colval[test])
-
-    test = int(np.argwhere(colparm == 'Statsec'))
-    mrad = int(colval[test])
+    test = np.argwhere(colparm == 'Window')
+    sqz = np.squeeze(colval[test][0])
+    imw = int( sqz )
+
+    test = np.argwhere(colparm == 'Statsec')
+    sqz = np.squeeze(colval[test][0])
+    mrad = int( sqz )
     
-    test = int(np.argwhere(colparm == 'Apphot_Radius'))
-    apr = int(colval[test])
-
-    test = int(np.argwhere(colparm == 'Back_1'))
-    urin = int(colval[test])
-
-    test = int(np.argwhere(colparm == 'Back_2'))
-    urout = int(colval[test])
+    test = np.argwhere(colparm == 'Apphot_Radius')
+    sqz = np.squeeze(colval[test][0])
+    apr = int( sqz )
     
-    test = int(np.argwhere(colparm == 'Color'))
-    user_map = colval[test]
-
-    test = int(np.argwhere(colparm == 'RMax'))
-    Rplot = int(colval[test])
-
-    test = int(np.argwhere(colparm == 'N_Contours'))
-    Ncontours = int(colval[test])
-
-    test = int(np.argwhere(colparm == 'Apspec_Upper'))
-    apspec_radius_u = float(colval[test])
-
-    test = int(np.argwhere(colparm == 'Apspec_Lower'))
-    apspec_radius_l = float(colval[test])
-
-    test = int(np.argwhere(colparm == 'Window_Search'))
-    aptrace_window = int(colval[test])
-
-    test = int(np.argwhere(colparm == 'TSum'))
-    TSum = int(colval[test])
-
-    test = int(np.argwhere(colparm == 'NTrace'))
-    NTrace = int(colval[test])
-
-    test = int(np.argwhere(colparm == 'OTrace'))
-    OTrace = int(colval[test])
-
-    test = int(np.argwhere(colparm == 'Window_Show'))
-    imc = int(colval[test])
-
-    test = int(np.argwhere(colparm == 'Zmax'))
-    zmax = int(colval[test])
 
-    test = int(np.argwhere(colparm == 'Zmin'))
-    zmin = int(colval[test])
-
-    test = int(np.argwhere(colparm == 'Undo'))
-    undo = int(colval[test])
+    test = np.argwhere(colparm == 'Back_1')
+    sqz = np.squeeze(colval[test][0])
+    urin = int( sqz )
     
-    test = int(np.argwhere(colparm == 'FTrace'))
-    trace_func = colval[test]
-
-    test = int(np.argwhere(colparm == 'ITrace'))
-    trace_iter = int(colval[test])
-               
+    test = np.argwhere(colparm == 'Back_2')
+    sqz = np.squeeze(colval[test][0])
+    urout = int( sqz )
+    
+    test = np.argwhere(colparm == 'Color')
+    sqz = np.squeeze(colval[test][0])
+    user_map = sqz
+    
+    test = np.argwhere(colparm == 'RMax')
+    sqz = np.squeeze(colval[test][0])
+    Rplot = int( sqz )
+
+    test = np.argwhere(colparm == 'N_Contours')
+    sqz = np.squeeze(colval[test][0])
+    Ncontours = int( sqz )
+
+    test = np.argwhere(colparm == 'Apspec_Upper')
+    sqz = np.squeeze(colval[test][0])
+    apspec_radius_u = int( sqz )
+    
+    test = np.argwhere(colparm == 'Apspec_Lower')
+    sqz = np.squeeze(colval[test][0])
+    apspec_radius_l = int( sqz )
+    
+    test = np.argwhere(colparm == 'Window_Search')
+    sqz = np.squeeze(colval[test][0])
+    aptrace_window = int( sqz )
+    
+    test = np.argwhere(colparm == 'TSum')
+    sqz = np.squeeze(colval[test][0])
+    TSum = int( sqz )
+    
+    test = np.argwhere(colparm == 'NTrace')
+    sqz = np.squeeze(colval[test][0])
+    NTrace = int( sqz )
+    
+    test = np.argwhere(colparm == 'OTrace')
+    sqz = np.squeeze(colval[test][0])
+    OTrace = int( sqz )
+    
+    test = np.argwhere(colparm == 'Window_Show')
+    sqz = np.squeeze(colval[test][0])
+    imc = int( sqz )
+    
+    test = np.argwhere(colparm == 'Zmax')
+    sqz = np.squeeze(colval[test][0])
+    zmax = int( sqz )
+
+    test = np.argwhere(colparm == 'Zmin')
+    sqz = np.squeeze(colval[test][0])
+    zmin = int( sqz )
+
+    test = np.argwhere(colparm == 'Undo')
+    sqz = np.squeeze(colval[test][0])
+    undo = int( sqz )
+    
+    test = np.argwhere(colparm == 'FTrace')
+    sqz = np.squeeze(colval[test][0])
+    trace_func = sqz
+    
+    test = np.argwhere(colparm == 'ITrace')
+    sqz = np.squeeze(colval[test][0])
+    trace_iter = int( sqz )
+                   
     if zmin < 0 and zmax < 0:
         Vmax = v1
         Vmin = v0
         
     else:
         Vmax = zmax
         Vmin = zmin
     
-    QCoreApplication.processEvents()
+    QtCore.QCoreApplication.processEvents()
 
 
     if val == '1':  # lower left
         boxx0.append(user_x)
         boxy0.append(user_y)
 
     if val == '2': # upper right
@@ -566,15 +591,15 @@
         fig.update_xaxes(title='Wavelength pixel')
         fig.show()
         print('Trace parameters:  xstart = ', user_x, '  tsum = ',TSum, '   ntrace = ',NTrace, '   t_func =', trace_func, ' otrace = ', OTrace, '  N_iter = ', trace_iter)
         
         if val == 's':
             np.save('tmp.x1d', ap_extract)
 
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
         
     if val == 'g':
         fit_succ = 1
         if dispaxis == 1:
             b_data = (np.transpose(data[user_x , user_y-urout:user_y-urin]) + np.transpose(data[user_x , user_y+urin:user_y+urout]) ) / 2.0
             t_data = np.transpose(data[user_x , user_y-int(apspec_radius_l*2):user_y+int(apspec_radius_u*2)])
             b_data = np.nanmedian(b_data)
@@ -609,47 +634,47 @@
             fig = go.Figure(data=[go.Scatter(x=pix_1d-mu1, y=t_data, marker_color="#000000", name="Data",line_shape="hvh"), go.Scatter(x=pix_1d-mu1, y=fitprof, marker_color=BR_red_col_HEX, name="Gaussian fit", mode="markers+lines")])
             print('Gaussian FWHM = {0:8.3f} pixels'.format(FWHM))
         fig.update_layout(font_family='Times New Roman',font_size=15,title=ifile+"<br>Gaussian FWHM (pix) = {0:8.3f}".format(FWHM))
         fig.update_xaxes(title='Spatial pixel - Centroid',nticks=10)
         fig.update_yaxes(title='Counts per pixel')
         fig.show()
                 
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
            
     if val == 'c':
         yarr_1d = np.arange(0,len(data[user_x,:]),1)
         fig = go.Figure(data=[go.Scatter(x=yarr_1d, y=data[user_x, :], marker_color="#000000",line_shape="hvh")])
         fig.update_layout(font_family='Times New Roman',font_size=15)
         fig.update_yaxes(title='Counts per pixel',nticks=10)
         fig.update_xaxes(title='y pixel')
         fig.show()
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
         
     if val == 'l':
         
         f, ax = plt.subplots()
         xarr_1d = np.arange(0,len(data[:,user_y]),1) # starts at 0
         fig = go.Figure(data=[go.Scatter(x=xarr_1d, y=data[:,user_y], marker_color="#000000",line_shape="hvh")])
         fig.update_layout(font_family='Times New Roman',font_size=15)
         fig.update_yaxes(title='Counts per pixel',nticks=10)
         fig.update_xaxes(title='x pixel')
         fig.show()
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
 
     if val == 'm':
         t_data = np.transpose(data[user_x-mrad:user_x+mrad, user_y-mrad:user_y+mrad])
         print('     ')
         print('Stats in box of side ',  mrad*2, 'pixels')
         print('Max = {:8.2f}'.format(np.max(t_data)))
         print('Mean = {:8.2f}'.format(np.mean(t_data)))
         print('Median = {:8.2f}'.format(np.median(t_data)))
         print('Std Dev = {:8.2f}'.format(np.std(t_data)))
         print('     ')
 
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
 
             
             
     if val == 'r' or val == 'a' or val == 'z':
         t_data = np.transpose(data[user_x-aptrace_window:user_x+aptrace_window, user_y-aptrace_window:user_y+aptrace_window]) # just for centroidin
         t_data_all = np.transpose(data)
         dy = float( urout + 5 - aptrace_window)
@@ -689,15 +714,15 @@
                     scaleratio = 1,
                 )
                 fig.update_layout(font_family='Times New Roman',font_size=15)
                 fig.update_yaxes(title='y pixel')
                 fig.update_xaxes(title='x pixel')
                 fig.show()
     
-                QCoreApplication.processEvents()
+                QtCore.QCoreApplication.processEvents()
 
 
 
             
             if val == 'r' or val == 'a':
                 aper = CircularAperture([xcen0, ycen0], r=float(apr))
                 annulus_aperture = CircularAnnulus([xcen0, ycen0], r_in =  urin, r_out = urout)
@@ -776,15 +801,15 @@
                 
             
           #      https://pyqtgraph.readthedocs.io/en/latest/graphicsItems/axisitem.html
         #        http://www.silx.org/doc/silx/0.2.0/modules/gui/plot/plotwidget.html
     
         #https://www.learnpyqt.com/courses/graphics-plotting/plotting-pyqtgraph/
 
-                    QCoreApplication.processEvents()
+                    QtCore.QCoreApplication.processEvents()
         except:
             print('Failed to get centroid with centroid_2dg')
 
     if val == 'o':
         t_data = np.transpose(data[user_x-imc:user_x+imc, user_y-imc:user_y+imc])
         data_ap = data[user_x-imc:user_x+imc, user_y-imc:user_y+imc]
         aper = CircularAperture([user_x, user_y], r=float(apr))
@@ -815,15 +840,15 @@
                     scaleratio = 1,
                 )
         fig.update_layout(font_family='Times New Roman',font_size=15)
         fig.update_yaxes(title='y pixel')
         fig.update_xaxes(title='x pixel')
         fig.show()
 
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
 
     if val == 't':  # trace a spectrum and show trace with plotly 
         if dispaxis == 1:
             t_data = np.transpose(data)
             xtrace, ytrace, bsubtrace, xvalsfitted, yvalsfitted = SpecLab.trace_1d(t_data, yguess=user_y, xstrt=user_x, search_win = aptrace_window, tsum=TSum, ntrace=NTrace,otrace=OTrace, bmin=urin, bmax=urout, N_iter=trace_iter, t_func = trace_func)
             print('Trace parameters:  xstart = ', user_x, '  tsum = ',TSum, '   ntrace = ',NTrace, '   t_func =', trace_func, ' otrace = ', OTrace, '  N_iter = ', trace_iter)
             winup = int(np.max(ytrace))
@@ -889,15 +914,15 @@
 
         fig.update_layout(font_family='Times New Roman',font_size=15)
         fig.update_yaxes(title='y pixel')
         fig.update_xaxes(title='x pixel')
         fig.show()
     
 
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
 
     if val == 'T':  # Find and show pixels above a threshold.
         thressh =  input('Enter threshold value: ')
         thresh = float(thressh)
         t_data = np.transpose(data)
 
         sat_pixels = (t_data >= thresh)
@@ -926,15 +951,15 @@
 
         if inds2d.shape[0] == 0:
             print('  ')
             print('No pixels found above ', thresh)
             print('  ')
         else:
             print('Number of pixels found above threshold = ', thresh, ' is ',inds2d.shape[0])
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
 
     if val == 'H':
         try:
             hdr = fits.getheader(ifile)
             hdr.totextfile('lastheader.txt',overwrite=True)
             hdr.totextfile(ifile+'.header.txt',overwrite=True)
             print('Printed header to lastheader.txt and '+ifile+'.header.txt')
@@ -943,15 +968,15 @@
                 print('DATE-OBS = ',hdr['DATE-OBS'])
                 print('EXPTIME = ',hdr['EXPTIME'])
             except:
                 print('Could not find DATE-OBS and EXPTIME in header.')
         except:
             print('Could not print header.')
     if val == 'q':
-        QCoreApplication.exit()
+        QtCore.QCoreApplication.exit()
     if val == 'h' or val == '?' or  val == 'help' or val == 'Help':
         print('           ')
         print('************************************************************')
         print('q:  quit imXam.')
         print('r:  plot radial profile, print fwhm, and print aperture photometry w/ sky annulus subtraction centered at cursor location; plot x-range can be set with RMax.')
         print('x:  trace and extract spectrum with sky subtraction, at cursor location (can change params in imXam_param.dat).')
         print('g:  fits a Gaussian to the spatial profile (uniform weighting in fit) of a spectrum at cursor location. An estimate of a constant background level (e.g., bias in a raw frame) is subtracted before the fit')
@@ -1089,18 +1114,19 @@
         imv3.setLabel('bottom', 'Pix along slice')
 
 
 roi_v.sigRegionChanged.connect(update_2)
 
 update_2()
 
-mouse_tooltip = QtGui.QLabel()
-mouse_tooltip.setFrameShape(QtGui.QFrame.StyledPanel)
-mouse_tooltip.setWindowFlags(QtCore.Qt.ToolTip)
-mouse_tooltip.setAttribute(QtCore.Qt.WA_TransparentForMouseEvents)
+mouse_tooltip = QtWidgets.QLabel()
+# Commented these out b/c they don't work with PyQtGraph 0.13.
+#mouse_tooltip.setFrameShape(QtWidgets.QFrame.StyledPanel)
+#mouse_tooltip.setWindowFlags(QtCore.Qt.ToolTip)
+#mouse_tooltip.setAttribute(QtCore.Qt.WA_TransparentForMouseEvents)
 mouse_tooltip.show()
 
 
 
 def single_gau_fix( x, c1,sigma1):
     res =   c1 * np.exp( - (x - 0.0)**2.0 / (2.0 * sigma1**2.0) ) 
     return res
@@ -1109,15 +1135,19 @@
     return res
 
 
 
 #https://stackoverflow.com/questions/60183177/issue-with-matplotlib-plotting
 #roi.scene().sigMouseClicked.connect(keyPressEvent)
 
-
-## Start Qt event loop unless running in interactive mode.
 if __name__ == '__main__':
-    import sys
-    if (sys.flags.interactive != 1) or not hasattr(QtCore, 'PYQT_VERSION'):
-        QtGui.QApplication.instance().exec_()
+    #import sys
+    #if (sys.flags.interactive != 1) or not hasattr(QtCore, 'PYQT_VERSION'):
+    pg.exec()
+#QtGui.QGuiApplication.instance()
+## Start Qt event loop unless running in interactive mode.
+#if __name__ == '__main__':
+    #import sys
+    #if (sys.flags.interactive != 1) or not hasattr(QtCore, 'PYQT_VERSION'):
+#    QtGui.QGuiApplication.instance().open()
```

### Comparing `SpecLab-4.1.1/SpecLab/cfg/SpecLab_config.py` & `SpecLab-4.2.0/SpecLab/cfg/SpecLab_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,46 +3,49 @@
 import os
 import site
 import tarfile
 
 
 try:
     your_site_packages_location = site.getsitepackages()
-    tar_fname = your_site_packages_location[0]+'/'+'SpecLab/aux/pyqtgraph10_speclab.tar.gz'
+    tar_fname = your_site_packages_location[0]+'/'+'SpecLab/aux/pyqtgraph_modifications.tar.gz'
     current_dir = os.getcwd()+'/'
 
-    if not os.path.exists(your_site_packages_location[0]+'/pyqtgraph10_speclab/'):
-        print('Extracting PyQTGraph v10 tarfile (pyqtgraph10_speclab.tar.gz) contents to ', your_site_packages_location[0]+'/pyqtgraph10_speclab/')
-        print('If uninstall SpecLab through pip (pip uninstall SpecLab), you may also want to rm -r pyqtgraph10_speclab/ from within your site-packages/ directory. ** Please be careful with the rm -r command **')
-        tarfgz = tarfile.open(tar_fname)
-        tarfgz.extractall(your_site_packages_location[0]+'/')
-        tarfgz.close()
-    else:
-        print('Did not unpack pyqtgraph10 because already exists in site-packages.')
-
-
-    print('pyqtgraph v10 is in ', your_site_packages_location[0]+'/pyqtgraph10_speclab/')
-    print('  ')
+ #   if not os.path.exists(your_site_packages_location[0]+'/pyqtgraph10_speclab/'):
+#        print('Extracting PyQTGraph v10 tarfile (pyqtgraph10_speclab.tar.gz) contents to ', your_site_packages_location[0]+'/pyqtgraph10_speclab/')
+ #       print('If uninstall SpecLab through pip (pip uninstall SpecLab), you may also want to rm -r pyqtgraph10_speclab/ from within your site-packages/ directory. ** Please be careful with the rm -r command **')
+
+        
+ 
+    tarfgz = tarfile.open(tar_fname)
+    tarfgz.extractall(your_site_packages_location[0]+'/')
+    tarfgz.close()
+    #else:
+    #    print('Could not unpack pyqtgraph modifications.')
+
+
+    print('PyQtGraph is in ', your_site_packages_location[0]+'/pyqtgraph/')
+    print('Several routines were overwritten with imXam modifications:  ')
+    print('pyqtgraph/imageview/ImageView.py')
+    print('pyqtgraph/GraphicsScene/GraphicsScene.py')
+    print('pyqtgraph/graphicsItems/ROI.py')
     print(' ********* ')
     print('  ')
-    print('Installation and configuration complete! ')
     print('  ')
-    print(' *********  ')
+    print('Installation and configuration complete! ')
     print('  ')
     print('Basic use (from anywhere on disk) in Unix command line: imXam.py -f <file.fits>')
     print('  ')
-    print(' *********  ')
     print('Notes:  Can put alias in .bash_profile:  alias imXam=<single quotes>imXam.py -f<single quotes>')
     print('If the command python imXam.py is not recognized (it should be in your anaconda3 environment bin/), the source is located here:  ', your_site_packages_location[0]+'/SpecLab/imXam/')
     print(' in which case, just put an alias to the command <single quotes>python .../site-packages/SpecLab/imXam/imXam.py -f<single quotes> in .bash_profile (or create a softlink through ln -s to a bin/ folder')
     print('  ')
-    print(' *********  ')
     print('  ')
     print('To uninstall:  pip uninstall SpecLab')
     print('  ')
     print(' *********  ')
     
 
 except:
-    print('Unable to install.')
+    print('Unable to complete configuration of PyQtGraph routines for imXam.')
```

### Comparing `SpecLab-4.1.1/SpecLab/gen/SpecLabFunctions.py` & `SpecLab-4.2.0/SpecLab/gen/SpecLabFunctions.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/gen/globals.py` & `SpecLab-4.2.0/SpecLab/gen/globals.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/gen/myfunc.py` & `SpecLab-4.2.0/SpecLab/gen/myfunc.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/aux/param_files/imXam_param.default.dat` & `SpecLab-4.2.0/SpecLab/aux/param_files/imXam_param.default.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/aux/param_files/imXam_param_ARCES.dat` & `SpecLab-4.2.0/SpecLab/aux/param_files/imXam_param_ARCES.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/aux/param_files/imXam_param.dat` & `SpecLab-4.2.0/SpecLab/aux/param_files/imXam_param.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/doc/CHANGELOG.txt` & `SpecLab-4.2.0/SpecLab/doc/CHANGELOG.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,8 +21,12 @@
 
 4.1.0
 
 - updates for python 3.6 and 3.7
 
 4.1.1 
 
-- updates to PyQtGraph, photutils module call for Python 3.8, Numpy 1.2
+- updates to PyQtGraph, photutils module call for Python 3.8, Numpy 1.
+
+4.1.2
+
+- removed dependency on separate installation of PyQt5 to address issues with M1/M2 chips
```

### Comparing `SpecLab-4.1.1/SpecLab/doc/README.md` & `SpecLab-4.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# imXam:  v4.1.1 (Latest)
+# imXam:  v4.1.2 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
-with the same GUI design (pyqtgraph10 + Plotly) in the future as these get finished.
+with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
 This uses [PyQTGraph](https://www.pyqtgraph.org/), but a customized version of v10 will be installed automatically with the commands below
 
 author: Adam F Kowalski (June 28, 2023)
 
 ## Installing imXam 
 
@@ -25,15 +25,15 @@
 To set up a fresh conda environment:
 
 From a terminal window:
 
 `conda create --name your_env_name python=3.8`
 
 (Note, imXam will work with Python 3.6, 3.7, and 3.8.  Note that Python 3.7 was unfortunately deprecated on 6/27/23!)
-
+imXam will be fully updated to work with Python 3.9+ and PyQtGraph(v.latest) by the time Python 3.8 is deprecated.
 
 `conda activate your_env_name`
 
 `pip install SpecLab`
 
 
 ### Step 3
```

### Comparing `SpecLab-4.1.1/SpecLab/doc/KNOWN_ISSUES.txt` & `SpecLab-4.2.0/SpecLab/doc/KNOWN_ISSUES.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/doc/LICENSE.txt` & `SpecLab-4.2.0/SpecLab/doc/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/setup.py` & `SpecLab-4.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,26 +6,26 @@
    import pypandoc
    long_desc = pypandoc.convert_file('SpecLab/doc/README.md', 'rst')
 except(IOError, ImportError):
    long_desc = open('SpecLab/doc/README.md').read()
 
 setup(
     name='SpecLab',
-    version='4.1.1',
+    version='4.2.0',
     author='A. F. Kowalski',
     author_email='adam.f.kowalski@colorado.edu',
     packages=['SpecLab','SpecLab.aux','SpecLab.aux.param_files','SpecLab.imXam','SpecLab.doc','SpecLab.gen',],
     package_data = {'':['*.tar.gz', '*.txt', '*.dat', '*.md', '*.rst'],},
    # include_package_data=True,
    # package_dir={"": ""},
     scripts=['SpecLab/cfg/SpecLab_config.py','SpecLab/imXam/imXam.py','SpecLab/cfg/epar_imXam.py',],
     url='http://pypi.python.org/pypi/SpecLab/',
-    description='IRAF imexam+DS9 replacement for Python',long_description_content_type='text/x-rst',
-    long_description=long_desc,
-    install_requires=['numpy', 'plotly>=5.2.1', 'pandas','astropy>=4.0.2','scipy','matplotlib','PyQt5>=5.15.6', 'photutils',]
+    description='IRAF imexam+DS9 replacement for Python',long_description_content_type='text/markdown',
+    long_description=open('SpecLab/doc/README.md').read(),
+    install_requires=['numpy>=1.25.0', 'plotly>=5.15.0', 'pandas>=2.0.3','astropy>=5.3.1','scipy>=1.11.1','matplotlib>=3.7.2','PyQt6==6.5.1', 'photutils>=1.8.0','pyqtgraph==0.13.3',]
 )
 
 # python setup.py sdist
 # python -m twine upload --repository testpypi dist/*
 # pip install -i https://test.pypi.org/simple/ speclab-imXam==3.1.2
 # pip uninstall speclab-imXam==3.1.2
 #  I neeeded to put the #! crap at the top of any of the scripts=
```

