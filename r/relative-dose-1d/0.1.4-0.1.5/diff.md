# Comparing `tmp/relative_dose_1d-0.1.4.tar.gz` & `tmp/relative_dose_1d-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relative_dose_1d-0.1.4.tar", last modified: Tue Jul  4 23:44:27 2023, max compression
+gzip compressed data, was "relative_dose_1d-0.1.5.tar", last modified: Tue Jul 11 03:32:38 2023, max compression
```

## Comparing `relative_dose_1d-0.1.4.tar` & `relative_dose_1d-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 23:44:27.349592 relative_dose_1d-0.1.4/
--rw-rw-rw-   0        0        0     1108 2023-04-05 01:02:18.000000 relative_dose_1d-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     4190 2023-07-04 23:44:27.344602 relative_dose_1d-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3092 2023-07-04 23:43:45.000000 relative_dose_1d-0.1.4/README.md
--rw-rw-rw-   0        0        0     1414 2023-07-04 23:42:21.000000 relative_dose_1d-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 23:44:27.349592 relative_dose_1d-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 23:44:27.257785 relative_dose_1d-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 23:44:27.293686 relative_dose_1d-0.1.4/src/relative_dose_1d/
--rw-rw-rw-   0        0        0     9352 2023-05-03 01:27:57.000000 relative_dose_1d-0.1.4/src/relative_dose_1d/GUI.py
--rw-rw-rw-   0        0        0        0 2023-04-05 01:08:12.000000 relative_dose_1d-0.1.4/src/relative_dose_1d/__init__.py
--rw-rw-rw-   0        0        0    10542 2023-07-04 23:35:01.000000 relative_dose_1d-0.1.4/src/relative_dose_1d/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-04 23:44:27.335081 relative_dose_1d-0.1.4/src/relative_dose_1d.egg-info/
--rw-rw-rw-   0        0        0     4190 2023-07-04 23:44:27.000000 relative_dose_1d-0.1.4/src/relative_dose_1d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-07-04 23:44:27.000000 relative_dose_1d-0.1.4/src/relative_dose_1d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 23:44:27.000000 relative_dose_1d-0.1.4/src/relative_dose_1d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-04 23:44:27.000000 relative_dose_1d-0.1.4/src/relative_dose_1d.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-04 23:44:27.000000 relative_dose_1d-0.1.4/src/relative_dose_1d.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 03:32:38.848834 relative_dose_1d-0.1.5/
+-rw-rw-rw-   0        0        0     1108 2023-04-05 01:02:18.000000 relative_dose_1d-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     4831 2023-07-11 03:32:38.842850 relative_dose_1d-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3743 2023-07-11 02:17:16.000000 relative_dose_1d-0.1.5/README.md
+-rw-rw-rw-   0        0        0     1404 2023-07-10 23:57:40.000000 relative_dose_1d-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 03:32:38.849833 relative_dose_1d-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 03:32:38.699762 relative_dose_1d-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 03:32:38.770866 relative_dose_1d-0.1.5/src/relative_dose_1d/
+-rw-rw-rw-   0        0        0     1410 2023-07-08 19:50:00.000000 relative_dose_1d-0.1.5/src/relative_dose_1d/GUI.py
+-rw-rw-rw-   0        0        0    13205 2023-07-11 00:52:51.000000 relative_dose_1d-0.1.5/src/relative_dose_1d/GUI_tool.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 01:08:12.000000 relative_dose_1d-0.1.5/src/relative_dose_1d/__init__.py
+-rw-rw-rw-   0        0        0      482 2023-07-11 02:57:11.000000 relative_dose_1d-0.1.5/src/relative_dose_1d/forTest.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:32:38.827210 relative_dose_1d-0.1.5/src/relative_dose_1d/test_data/
+-rw-rw-rw-   0        0        0      341 2023-07-10 23:57:40.000000 relative_dose_1d-0.1.5/src/relative_dose_1d/test_data/clean.py
+-rw-rw-rw-   0        0        0    10639 2023-07-10 03:51:03.000000 relative_dose_1d-0.1.5/src/relative_dose_1d/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:32:38.823219 relative_dose_1d-0.1.5/src/relative_dose_1d.egg-info/
+-rw-rw-rw-   0        0        0     4831 2023-07-11 03:32:38.000000 relative_dose_1d-0.1.5/src/relative_dose_1d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-07-11 03:32:38.000000 relative_dose_1d-0.1.5/src/relative_dose_1d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 03:32:38.000000 relative_dose_1d-0.1.5/src/relative_dose_1d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-11 03:32:38.000000 relative_dose_1d-0.1.5/src/relative_dose_1d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-11 03:32:38.000000 relative_dose_1d-0.1.5/src/relative_dose_1d.egg-info/top_level.txt
```

### Comparing `relative_dose_1d-0.1.4/LICENSE` & `relative_dose_1d-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.1.4/PKG-INFO` & `relative_dose_1d-0.1.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,29 @@
-Metadata-Version: 2.1
-Name: relative_dose_1d
-Version: 0.1.4
-Summary: Python package to read an 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
-Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
-Project-URL: homepage, https://relative-dose-1d.readthedocs.io/en/latest/intro.html
-Project-URL: repository, https://github.com/LuisOlivaresJ/relative_dose_1d
-Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/relative_dose_1d/issues
-Keywords: Radiotherapy,Relative dose distribution,gamma index,python,w2CAD,mcc
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Healthcare Industry
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Natural Language :: Spanish
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # relative_dose_1d
 
-Python package to read 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
+Python package to read 1-dimensional dose profile from text file to perform subtraction and gamma analysis.
 
-![image_gui](/docs/assets/GUI_v011.PNG)
+![image_gui](/docs/assets/GUI_v015.PNG)
 
 ## [Documentation](https://relative-dose-1d.readthedocs.io/en/latest/intro.html)
 
+## Features
+
+### For gamma analysis
+* Interpolation between points
+* Profile positions does not require to be equal
+```{note}
+* The gamma analysis algorithm is limited to absolute normalization  relative to the maximum dose.
+```
+
+### For data import
+* PTW (R) and Varian (R) data formats suported.
+
 ## Format specifications
-Data should be in M ​​rows by 2 columns, corresponding to positions and
+Data should be in a numpy array with two columns, corresponding to positions and
 dose values, respectively.
 
 The package has been tested with the following examples:
 
 * File in w2CAD format (used by the TPS Eclipse 16.1, from the Varian(R) company).
   In the algorithm, the start of the data is identified by the words: 'STOM' or 'STOD'
   Physical unit assumed to be in mm.
@@ -89,9 +80,13 @@
 
 May-2023 Version 0.1.2
   * New web page for documentation, following [PEP 287 – reStructuredText Docstring Format](https://peps.python.org/pep-0287/) and [napoleon extension](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html#module-sphinx.ext.napoleon)
 
 May-2023 Version 0.1.3
   * [Interpolation error](https://github.com/LuisOlivaresJ/relative_dose_1d/issues/1) solved.
 
-Jul-2023 Version 0.1.4
-  * A new function to create a an array with physical positions.
+Jul-2023 Version 0.1.4 - 0.1.5
+* Two new functions, [build_from_array_and_step](Tools_module_label) to add physical positions, and [plot](GUI_tool_module_label) to show a GUI. 
+* [New GUI_tool module](GUI_tool_module_label).
+* Now it is possible to change tolerance parameter for gamma evaluation.
+* Pass rate, total and evaluated points are now displayed on the GUI.
+* gamma_1d function returns the number of evaluated points.
```

### Comparing `relative_dose_1d-0.1.4/pyproject.toml` & `relative_dose_1d-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,19 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "relative_dose_1d"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Luis Alfonso Olivares Jimenez", email="alfonso.cucei.udg@gmail.com" },
 ]
-description = "Python package to read an 1-dimensional dose profile from text file and perform subtraction and gamma index comparison."
+description = "Python package to read 1-dimensional dose profile from a text file to perform subtraction and gamma analysis."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENCE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
```

### Comparing `relative_dose_1d-0.1.4/src/relative_dose_1d/GUI.py` & `relative_dose_1d-0.1.5/src/relative_dose_1d/GUI_tool.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,146 @@
 # -*- coding: utf-8 -*-
-"""
-Created Apr-2023
 
-@author: Luis Alfonso Olivares Jimenez
-
-GUI to load text data corresponding to dose profiles and PDD. 
+from matplotlib.figure import Figure
+from matplotlib.backends.backend_qtagg import FigureCanvas
+from PyQt6.QtWidgets import (QApplication, QWidget, QLabel, QLineEdit, QHBoxLayout,
+                             QPushButton, QMessageBox, QFileDialog, QVBoxLayout,
+                             QFormLayout, QInputDialog, QMainWindow)
+from PyQt6.QtCore import Qt
+import numpy as np
+from relative_dose_1d.tools import identify_format, get_data, gamma_1D, build_from_array_and_step
+import sys
+import os
+import copy
 
-The data should be in M ​​rows by 2 columns, corresponding to positions and
-dose values, respectively.
+class GUI(QWidget):
 
-The script has been tested with the following examples:
+    def __init__(self, D_ref = None, D_eval = None):
+        """Constructor for a graphical user interface (GUI). Data has to be in 2 columns, 
+        corresponding to positions and dose values, respectively.
 
-    * File in w2CAD format (format used by the TPS Eclipse 16.1, from the Varian(R) company).
-      In the algorithm, the start of the data is identified by the words: '$STOM' or '$STOD'
-      Physical unit assumed to be in mm.
+        Parameters
+        ----------
 
-    * File in mcc format (format used by Verisoft 7.1.0.199 software, from PTW(R) company).
-      In the algorithm, the beginning of the data is identified by the word: 'BEGIN_DATA'
-      Physical unit assumed to be in mm.
+        D_ref : ndarray,
+            Reference dose profile represented by a (M, 2) numpy array.  
 
-    * File in text format
-      The data must be distributed in M ​​rows by 2 columns and separated
-      for a blank space.
-      The script ask for a word to identify the beginning of the data in the text file, 
-      a number to add to the positions, and a factor for distance dimension conversion.
+        D_eva : ndarray,
+            Dose profile to be evaluated, represented by a (N, 2) numpy array.
 
-After two successful loaded data, gamma index and dose difference are automatically calculated.
+        Returns
+        -------
 
-"""
+        A PyQt widget to showing dose profiles, gamma analysis and dose difference.
 
-import sys
-import os
-import numpy as np
-from PyQt6.QtWidgets import (QApplication, QWidget, QLabel, QLineEdit, QHBoxLayout,
-                             QPushButton, QMessageBox, QFileDialog, QVBoxLayout,
-                             QFormLayout, QInputDialog, QMainWindow)
-from PyQt6.QtCore import Qt
-
-from matplotlib.figure import Figure
-from matplotlib.backends.backend_qtagg import FigureCanvas
-
-from relative_dose_1d.tools import identify_format, get_data, gamma_1D
-# For testing
-#from tools import identify_format, get_data, gamma_1D
+        """
+        super().__init__()
 
-class Main_Window(QWidget):
+        self.D_ref = D_ref
+        self.D_eval = D_eval
 
-    def __init__(self):
-        """Constructor for Empty Window Class"""
-        super().__init__()
-        self.loaded_data = []
         self.initializeUI()
 
     def initializeUI(self):
         """Set up the apllication"""
         "x, y, width, height"
         self.setGeometry(200,100,1000,400)
         self.setWindowTitle("Relative dose 1D")
 
-        self.set_up()
+        self.set_up_window()
+        self.set_up_data()
         self.show()
 
-    def set_up(self):
-        "Layouts definition"
-        self.main_box_layout = QVBoxLayout()
-
-        self.open_and_clear_layout = QVBoxLayout()
-        self.main_box_layout.addLayout(self.open_and_clear_layout)
+    def set_up_window(self):
 
-        self.h_box_layout = QHBoxLayout()
+        "Layouts definition"
+        self.main_box_layout = QHBoxLayout()
+   
+        self.v_box_layout = QVBoxLayout()
         self.settings_layout_v = QVBoxLayout()
-        self.h_box_layout.addLayout(self.settings_layout_v)
-        self.main_box_layout.addLayout(self.h_box_layout)
+        
+        self.Q_grafica = Q_Base_Figure() 
+
+        self.main_box_layout.addLayout(self.settings_layout_v)
+        self.main_box_layout.addLayout(self.v_box_layout)
 
         self.setLayout(self.main_box_layout)
 
         self.open_file_button = QPushButton("Load a text file", self)
         self.open_file_button.clicked.connect(self.open_file_button_clicked)
 
         self.clear_button = QPushButton("Clear", self)
         self.clear_button.clicked.connect(self.clear_data_and_plots)
         
         self.button_factor = QPushButton("Scale factor", self)
         self.button_factor.clicked.connect(self.factor_button_clicked)
-        self.button_factor.setFixedSize(75, 40)
+        self.button_factor.setFixedSize(80, 40)
         self.button_factor.setEnabled(False)
 
         self.button_origin = QPushButton("Move origin", self)
         self.button_origin.clicked.connect(self.move_button_clicked)
-        self.button_origin.setFixedSize(75, 40)
+        self.button_origin.setFixedSize(80, 40)
         self.button_origin.setEnabled(False)
+
+        axis_label = QLabel("Axis position")
+        #axis_label.setFont(QFont(Arial, 15))
+        self.settings_layout_v.addWidget(axis_label, alignment = Qt.AlignmentFlag.AlignHCenter)
         self.settings_layout_v.addWidget(self.button_factor)
         self.settings_layout_v.addWidget(self.button_origin)
+        self.settings_layout_v.addWidget(QLabel("Gamma", alignment = Qt.AlignmentFlag.AlignHCenter))
+
+        gammaLayout = QFormLayout()
+        self.dose_t_QLine = QLineEdit()
+        self.dose_t_QLine.setFixedWidth(40)
+        self.dose_t_QLine.setText("3.0")
+        self.DTA_t_QLine = QLineEdit()
+        self.DTA_t_QLine.setFixedWidth(40)
+        self.DTA_t_QLine.setText("2.0")
+        self.thres_QLine = QLineEdit()
+        self.thres_QLine.setFixedWidth(40)
+        self.thres_QLine.setText("0.0")
+        self.interp_QLine = QLineEdit()
+        self.interp_QLine.setFixedWidth(40)
+        self.interp_QLine.setText("1")
+        gammaLayout.addRow("Dose [%]:", self.dose_t_QLine)
+        gammaLayout.addRow("DTA [mm]:", self.DTA_t_QLine)
+        gammaLayout.addRow("Threshold [%]:", self.thres_QLine)
+        gammaLayout.addRow("Interp.:", self.interp_QLine)
+
+        self.gamma_button = QPushButton("Apply")
+        self.gamma_button.clicked.connect(self.calc_difference_and_gamma)
+        self.gamma_button.setFixedSize(120, 40)
+        #self.button_origin.setEnabled(False)
+
+        results_label = QLabel("Results", alignment = Qt.AlignmentFlag.AlignHCenter)
+        self.gamma_rate_label = QLabel("Pass rate: ")
+        self.total_points_label = QLabel("Total points: ")
+        self.evaluated_points_label = QLabel("Evaluated ponits: ")
+
+        self.settings_layout_v.addLayout(gammaLayout)
+        self.settings_layout_v.addWidget(self.gamma_button)
+        self.settings_layout_v.addWidget(results_label)
+        self.settings_layout_v.addWidget(self.gamma_rate_label)
+        self.settings_layout_v.addWidget(self.total_points_label)
+        self.settings_layout_v.addWidget(self.evaluated_points_label)
+
         self.settings_layout_v.addStretch()
-        self.Q_grafica = Q_Graphic_Block() 
-        self.h_box_layout.addWidget(self.Q_grafica.Qt_fig)
          
-        self.open_and_clear_layout.addWidget(self.open_file_button)
-        self.open_and_clear_layout.addWidget(self.clear_button)
+        self.v_box_layout.addWidget(self.open_file_button)
+        self.v_box_layout.addWidget(self.clear_button)
+        self.v_box_layout.addWidget(self.Q_grafica.Qt_fig)
         
+    def set_up_data(self):
+        if self.D_ref is None:
+            self.loaded_data = []
+        else:          
+            self.loaded_data = [self.D_ref, self.D_eval]
+            self.Q_grafica.plot_data(self.D_ref)
+            self.Q_grafica.plot_data(self.D_eval)
+            self.calc_difference_and_gamma()
 
     # Button's functions
 
     def open_file_button_clicked(self):
         self.last_file_name, _ = QFileDialog.getOpenFileName()
         _ , extension = os.path.splitext(self.last_file_name)
 
@@ -115,30 +153,33 @@
             if format == 'text_file':
                 self.show_new_window()  #New window for input user parameters.
 
             else:
                 data = get_data(self.last_file_name)
                 self.load_data(data)
 
-
     def clear_data_and_plots(self):
         self.Q_grafica.ax_perfil.clear()
         self.Q_grafica.ax_perfil_resta.clear()
         self.Q_grafica.ax_gamma.clear()
         self.Q_grafica.fig.canvas.draw()
         self.open_file_button.setEnabled(True)
         self.loaded_data = []
 
+    def clear_gamma(self):
+        self.Q_grafica.ax_perfil_resta.clear()
+        self.Q_grafica.ax_gamma.clear()
+
     def factor_button_clicked(self):
         scale_factor, ok = QInputDialog.getText(self, 'Scale factor', 'Scale factor:')
         try:
             scale_factor = float(scale_factor)
             if ok:
                 self.loaded_data[-1][:,0] = self.loaded_data[-1][:,0] * scale_factor
-                cache_data = self.loaded_data
+                cache_data = copy.deepcopy(self.loaded_data)
                 self.clear_data_and_plots()
 
                 for data in cache_data:
                     self.load_data(data)
 
         except ValueError:
             QMessageBox().critical(self, "Error", "Enter a number.")
@@ -146,15 +187,15 @@
 
     def move_button_clicked(self):
         delta, ok = QInputDialog.getText(self, 'Scale factor', 'Origin displacement:')
         try:
             delta = float(delta)
             if ok:
                 self.loaded_data[-1][:,0] = self.loaded_data[-1][:,0] + delta
-                cache_data = self.loaded_data
+                cache_data = copy.deepcopy(self.loaded_data)
                 self.clear_data_and_plots()
 
                 for data in cache_data:
                     self.load_data(data)
 
         except ValueError:
             QMessageBox().critical(self, "Error", "Enter a number.")
@@ -189,72 +230,138 @@
         data_B_from_A_positions = np.interp(data_A[:,0], data_B[:,0], data_B[:,1], left = np.nan)
     
         difference = data_A[:,1] - data_B_from_A_positions
 
         added_positions = np.array((data_A[:,0], difference))
         values = np.transpose(added_positions)
        
-        g, g_percent = gamma_1D(data_A, data_B)
+        g, g_percent, evaluated_points = gamma_1D(
+            data_A, 
+            data_B,
+            dose_t = float(self.dose_t_QLine.text()),
+            dist_t = float(self.DTA_t_QLine.text()),
+            dose_threshold = float(self.thres_QLine.text()),
+            interpol = int(self.interp_QLine.text()),
+            )
 
         self.Q_grafica.plot_resta(values)
+        self.Q_grafica.ax_gamma.clear()
+        #self.Q_grafica.ax_gamma = self.Q_grafica.ax_perfil_resta.twinx()
         self.Q_grafica.plot_gamma(g)
-        print(g_percent)
+        #self.Q_grafica.ax_gamma.set_ylabel('gamma')
+        self.gamma_rate_label.setText(f"Pass rate: {g_percent:0.1f}%")
+        self.total_points_label.setText(f"Total points: {data_A.shape[0]:0.1f}")
+        self.evaluated_points_label.setText(f"Evaluated ponits: {evaluated_points:0.1f}")
 
-    
-class Q_Graphic_Block:
+class Q_Base_Figure:
         
     def __init__(self):
-        self.fig = Figure(figsize=(4,3), tight_layout = True, facecolor = 'whitesmoke')
+        self.fig = Figure(figsize=(40,4), tight_layout = True, facecolor = 'whitesmoke')
         self.Qt_fig = FigureCanvas(self.fig)
 
         #   Axes para la imagen
         self.ax_perfil = self.fig.add_subplot(1, 2, 1)
-        #self.ax_perfil.set_title('Pro')
         self.ax_perfil.set_ylabel('Percentage [%]')
-        self.ax_perfil.set_xlabel('Distance')
+        self.ax_perfil.set_xlabel('Distance [mm]')
         self.ax_perfil.grid(alpha = 0.3)
 
         self.ax_perfil_resta =  self.fig.add_subplot(1, 2, 2)
-        #self.ax_perfil_resta.set_title('Resta')
         self.ax_perfil_resta.set_ylabel('Percentage [%]')
-        self.ax_perfil_resta.set_xlabel('Distance')
+        self.ax_perfil_resta.set_xlabel('Distance [mm]')
         self.ax_perfil_resta.grid(alpha = 0.3)
 
         self.ax_gamma = self.ax_perfil_resta.twinx()
         self.ax_gamma.set_ylabel('gamma')
         #self.ax_gamma.set_ylim((0, 2))
         
     def plot_data(self, data):
         x = data[:,0]
         y = data[:,1]
         self.ax_perfil.plot(x, y)
         self.ax_perfil.set_ylabel('Percentage [%]')
-        self.ax_perfil.set_xlabel('Distance')
+        self.ax_perfil.set_xlabel('Distance [mm]')
         self.ax_perfil.grid(alpha = 0.3)
+        #self.ax_perfil.legend()
         self.fig.canvas.draw()
         
     def plot_resta(self, data):
         x = data[:,0]
         y = data[:,1]
-        self.ax_perfil_resta.plot(x, y, color='r', label = 'Diferencia', alpha = 0.6)
-        self.ax_perfil_resta.set_ylabel('Diferencia')
-        self.ax_perfil_resta.set_xlabel('Distancia [mm]')
-        self.ax_perfil_resta.grid(alpha = 0.3)
+        self.ax_perfil_resta.plot(x, y, color='r', label = 'Difference', alpha = 0.7)
+        self.ax_perfil_resta.set_ylabel('Difference')
+        self.ax_perfil_resta.set_xlabel('Distance [mm]')
+        self.ax_perfil_resta.grid(alpha = 0.4)
         self.ax_perfil_resta.legend(loc = 'upper left')
 
         self.fig.canvas.draw()
 
     def plot_gamma(self, data):
         x = data[:,0]
         y = data[:,1]
 
         self.ax_gamma.plot(x, y, color='g', label = 'gamma', marker = '.')
+        self.ax_gamma.plot(x, np.ones(x.shape[0]), 'g--', alpha = 0.5, linewidth=2)
         self.ax_gamma.set_ylabel('gamma')
+        self.ax_gamma.yaxis.set_label_position("right")
         self.ax_gamma.legend(loc = 'upper right')
 
-        self.fig.canvas.draw()        
+        self.fig.canvas.draw()
 
-        
-app = QApplication(sys.argv)
-window = Main_Window()
-sys.exit(app.exec())
+def plot(D_ref, D_eval):
+    """
+    A function to show a graphical user interface (GUI) to showing 1D dose profiles, 
+    gamma analysis and dose difference. Data has to be in 2 columns, 
+    corresponding to positions and dose values, respectively.
+
+    Parameters
+    ----------
+
+    D_ref : ndarray,
+        Reference dose profile represented by a (M, 2) numpy array.  
+
+    D_eva : ndarray,
+        Dose profile to be evaluated, represented by a (N, 2) numpy array.
 
+    Returns
+    -------
+
+    A GUI showing dose profiles, gamma analysis and dose difference.
+
+    Examples
+    --------
+
+    >>> import relative_dose_1d.GUI_tool as rd
+
+    >>> a = np.array([0,1,2,3,4,5,6,7,8,9,10])
+    >>> b = a + np.random.random_sample((11,))
+
+    >>> A = build_from_array_and_step(a, 1)
+    >>> B = build_from_array_and_step(b, 1)
+    
+    >>> rd.plot(A,B)
+
+    """
+
+    app = QApplication(sys.argv)    
+    window = GUI(D_ref, D_eval)
+    sys.exit(app.exec())
+
+def run_demo():
+
+    a = np.array([0,1,2,3,4,5,6,7,8,9,10])
+    b = a + np.random.random_sample((11,))
+
+    A = build_from_array_and_step(a, 1)
+    B = build_from_array_and_step(b, 1)
+    
+    plot(A,B)
+
+if __name__ == '__main__':
+    
+    a = np.array([0,1,2,3,4,5,6,7,8,9,10])
+    b = a + np.random.random_sample((11,))
+    A = build_from_array_and_step(a, 1)
+    B = build_from_array_and_step(b, 1)
+    
+    app = QApplication(sys.argv)
+    window = GUI(A, B)
+    sys.exit(app.exec())
```

### Comparing `relative_dose_1d-0.1.4/src/relative_dose_1d/tools.py` & `relative_dose_1d-0.1.5/src/relative_dose_1d/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created on Mon Apr 24 2023
 
 @author: Luis Alfonso Olivares Jimenez
 
-Functions to read 1-dimensional dose profiles and perform gamma index comparison.
+Tools to read 1-dimensional dose profiles and perform gamma index comparison.
 
 The data should be in M ​​rows by 2 columns, corresponding to positions and
 dose values, respectively.
 
 The script has been tested with the following examples:
 
     * File in w2CAD format (format used by the TPS Eclipse 16.1, from the Varian(R) company).
@@ -190,32 +190,32 @@
         data_array[:,0] = data_array[:,0] + float(delta)
         
     
     return data_array
 
 
 def build_from_array_and_step(array, step):
-    """Create a new array with the same length but an additional axis. The first column represents the 
-    physical positions of the given values. The second column is a copy of the given array. 
+    """Create a new array with the same length but with an additional axis. The first column represents the 
+    physical positions of the given values. The second column is a normalization of the given array. 
     The positions are builded with evenly step spacing starting from zero.
 
     Parameters
     ----------
 
     array : ndarrya,
         Numpy 1D array with the profile values
 
-    resolution : float,
+    step : float,
         The spacing between samples
 
     Returns
     -------
 
     array, ndarray
-        A new array with shape (M,2), where M is the shape of array.
+        A new array with shape (M,2), where M is the shape of the array.
 
     Examples
     --------
 
     >>> y = np.array([2,4,6,8,10])
     >>> A = build_from_array_and_step(y, 0.5)
     [ 
@@ -239,20 +239,20 @@
     num = array.shape[0]
     start = 0
     stop = (num - 1) * step
 
     positions = np.linspace(start, stop, num = num, endpoint = True)
     profile = np.zeros((num, 2))
     profile[:,0] = positions
-    profile[:,1] = array
+    profile[:,1] = array / np.max(array) * 100
 
     return profile
     
 
-def gamma_1D(ref, eval, dose_t = 3, dist_t = 2, dose_tresh = 0, interpol = 1):
+def gamma_1D(ref, eval, dose_t = 3, dist_t = 2, dose_threshold = 0, interpol = 1):
     '''
     1-dimensional gamma index calculation.
     Dose profiles have to be normalized (0-100%).
 
     Parameters
     ----------
 
@@ -276,33 +276,34 @@
     interpol : float, default = 1
         Number of interpolated points to generate between each two consecutive points in "eval" data.
 
     Returns
     -------
 
     ndarray, float
-        gamma distribution and gamma percent
+        gamma distribution, gamma percent and number of evaluated points
         
     '''
 
-    # min_position and max_position to analize.
+    # min_position and max_position to analyze.
     min_position = np.max( (np.min(ref[:,0]), np.min([eval[:,0]])) )
     max_position = np.min( (np.max(ref[:,0]), np.max([eval[:,0]])) ) 
 
     num_of_points = eval.shape[0]
     interp_positions = np.linspace(ref[0,0], ref[-1,0], (interpol + 1)*(num_of_points - 1) + 1, endpoint=True)
     eval_from_interp_positions = np.interp(interp_positions, eval[:,0], eval[:,1], left = np.nan, right = np.nan) 
     add_positions = np.array((interp_positions, eval_from_interp_positions))
     eval_from_interp_positions = np.transpose(add_positions)
 
-    #   A variable to storage gamma calculations.
-    gamma = np.zeros( (num_of_points, 2) )
+    #   A variable to store gamma calculations.
+    gamma = np.zeros( (ref.shape[0], 2) )
+
     gamma[:,0] = ref[:,0]   #Add the same positions.
 
-    for i in range(num_of_points):
+    for i in range(ref.shape[0]):
 
         if (ref[i,0] < min_position) or (ref[i,0] > max_position):  
 
             gamma[i, 1] = np.nan
             continue
 
         Gamma_appended = np.array([])  #   Gamma calculation for each point in "ref" data.
@@ -314,43 +315,44 @@
             Gamma = np.sqrt(
                         (distance**2) / (dist_t**2)
                         + (dose_difference**2) / (dose_t**2))
                         
             Gamma_appended = np.append(Gamma_appended, Gamma)
 
         gamma[i,1] = np.min( Gamma_appended[ ~np.isnan(Gamma_appended) ] )
-        if ref[i,1] < dose_tresh:
+        if ref[i,1] < dose_threshold:
             gamma[i,1] = np.nan
 
     # Coordinates for gamma values <= 1.
     less_than_1_coordinate = np.where(gamma[:,1] <= 1)
     # Number of points where gamma <= 1.
     less_than_1 = np.shape(less_than_1_coordinate)[1]
     # Number evaluated points (!= nan)
-    total_points = np.shape(gamma)[0] - np.shape(np.where(np.isnan(gamma[:,1])))[1]
+    evaluated_points = np.shape(gamma)[0] - np.shape(np.where(np.isnan(gamma[:,1])))[1]
     
-    gamma_percent = float(less_than_1)/total_points*100
+    gamma_percent = float(less_than_1)/evaluated_points*100
 
-    return gamma, gamma_percent
+    return gamma, gamma_percent, evaluated_points
 
 
 if __name__ == '__main__':
-
+    """
     y = np.array([2,4,6,8,10])
     A = build_from_array_and_step(y, 0.5)
     print(A)
 
     y = np.arange(10)
     B = build_from_array_and_step(y, 3)
     print(B)
 
-    """Test files"""
-    #file_name = './test_data/test_ptw.mcc'
+    """
+    #Test files
+    file_name = './test_data/test_ptw.mcc'
     #file_name = './test_data/test_varian.data'
     #file_name = './test_data/test_txt.txt'
 
-    #file_name_eval = "./test_data/X06 OPEN 10X10 PDD WAT 221214 13'13'42.mcc"
+    file_name_eval = "./test_data/X06 OPEN 10X10 PDD WAT 221214 13'13'42.mcc"
     
-    #data_ref = get_data(file_name, start_word =  'Field 1')
-    #data_eval = get_data(file_name_eval)
-    #g, gp = gamma_1D(data_ref, data_eval)
-    #print(gp)
+    data_ref = get_data(file_name, start_word =  'Field 1')
+    data_eval = get_data(file_name_eval)
+    g, gp = gamma_1D(data_ref, data_eval)
+    print(gp)
```

### Comparing `relative_dose_1d-0.1.4/src/relative_dose_1d.egg-info/PKG-INFO` & `relative_dose_1d-0.1.5/src/relative_dose_1d.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: relative-dose-1d
-Version: 0.1.4
-Summary: Python package to read an 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
+Version: 0.1.5
+Summary: Python package to read 1-dimensional dose profile from a text file to perform subtraction and gamma analysis.
 Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
 Project-URL: homepage, https://relative-dose-1d.readthedocs.io/en/latest/intro.html
 Project-URL: repository, https://github.com/LuisOlivaresJ/relative_dose_1d
 Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/relative_dose_1d/issues
 Keywords: Radiotherapy,Relative dose distribution,gamma index,python,w2CAD,mcc
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -17,22 +17,34 @@
 Classifier: Natural Language :: Spanish
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # relative_dose_1d
 
-Python package to read 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
+Python package to read 1-dimensional dose profile from text file to perform subtraction and gamma analysis.
 
-![image_gui](/docs/assets/GUI_v011.PNG)
+![image_gui](/docs/assets/GUI_v015.PNG)
 
 ## [Documentation](https://relative-dose-1d.readthedocs.io/en/latest/intro.html)
 
+## Features
+
+### For gamma analysis
+* Interpolation between points
+* Profile positions does not require to be equal
+```{note}
+* The gamma analysis algorithm is limited to absolute normalization  relative to the maximum dose.
+```
+
+### For data import
+* PTW (R) and Varian (R) data formats suported.
+
 ## Format specifications
-Data should be in M ​​rows by 2 columns, corresponding to positions and
+Data should be in a numpy array with two columns, corresponding to positions and
 dose values, respectively.
 
 The package has been tested with the following examples:
 
 * File in w2CAD format (used by the TPS Eclipse 16.1, from the Varian(R) company).
   In the algorithm, the start of the data is identified by the words: 'STOM' or 'STOD'
   Physical unit assumed to be in mm.
@@ -89,9 +101,13 @@
 
 May-2023 Version 0.1.2
   * New web page for documentation, following [PEP 287 – reStructuredText Docstring Format](https://peps.python.org/pep-0287/) and [napoleon extension](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html#module-sphinx.ext.napoleon)
 
 May-2023 Version 0.1.3
   * [Interpolation error](https://github.com/LuisOlivaresJ/relative_dose_1d/issues/1) solved.
 
-Jul-2023 Version 0.1.4
-  * A new function to create a an array with physical positions.
+Jul-2023 Version 0.1.4 - 0.1.5
+* Two new functions, [build_from_array_and_step](Tools_module_label) to add physical positions, and [plot](GUI_tool_module_label) to show a GUI. 
+* [New GUI_tool module](GUI_tool_module_label).
+* Now it is possible to change tolerance parameter for gamma evaluation.
+* Pass rate, total and evaluated points are now displayed on the GUI.
+* gamma_1d function returns the number of evaluated points.
```

