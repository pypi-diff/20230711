# Comparing `tmp/pudu-0.3.0.tar.gz` & `tmp/pudu-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pudu-0.3.0.tar", last modified: Mon Jul 10 09:00:19 2023, max compression
+gzip compressed data, was "pudu-0.3.1.tar", last modified: Tue Jul 11 10:01:04 2023, max compression
```

## Comparing `pudu-0.3.0.tar` & `pudu-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 09:00:19.942481 pudu-0.3.0/
--rw-rw-rw-   0        0        0     1124 2023-07-10 07:31:04.000000 pudu-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      129 2022-11-04 23:37:34.000000 pudu-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4517 2023-07-10 09:00:19.943478 pudu-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3681 2023-05-17 09:45:31.000000 pudu-0.3.0/README.md
--rw-rw-rw-   0        0        0     3721 2023-05-17 09:45:54.000000 pudu-0.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-10 09:00:19.918546 pudu-0.3.0/pudu/
--rw-rw-rw-   0        0        0      137 2023-07-10 07:31:20.000000 pudu-0.3.0/pudu/__init__.py
--rw-rw-rw-   0        0        0     4461 2023-07-08 13:16:56.000000 pudu-0.3.0/pudu/error_handler.py
--rw-rw-rw-   0        0        0     2616 2023-07-09 10:38:07.000000 pudu-0.3.0/pudu/masks.py
--rw-rw-rw-   0        0        0    12316 2023-07-08 15:34:18.000000 pudu-0.3.0/pudu/perturbation.py
--rw-rw-rw-   0        0        0    13365 2023-07-04 13:45:49.000000 pudu-0.3.0/pudu/plots.py
--rw-rw-rw-   0        0        0    28362 2023-07-10 07:29:05.000000 pudu-0.3.0/pudu/pudu.py
--rw-rw-rw-   0        0        0     2941 2023-07-08 14:00:15.000000 pudu-0.3.0/pudu/standards.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:00:19.942481 pudu-0.3.0/pudu.egg-info/
--rw-rw-rw-   0        0        0     4517 2023-07-10 09:00:19.000000 pudu-0.3.0/pudu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-07-10 09:00:19.000000 pudu-0.3.0/pudu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       62 2023-07-10 09:00:19.000000 pudu-0.3.0/pudu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-11-22 10:14:32.000000 pudu-0.3.0/pudu.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       62 2023-07-10 09:00:19.000000 pudu-0.3.0/pudu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-10 09:00:19.000000 pudu-0.3.0/pudu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      164 2022-02-13 18:34:42.000000 pudu-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       66 2023-06-28 13:59:09.000000 pudu-0.3.0/requirements.txt
--rw-rw-rw-   0        0        0      449 2023-07-10 09:00:19.945473 pudu-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1844 2023-07-10 07:30:25.000000 pudu-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:01:04.959476 pudu-0.3.1/
+-rw-rw-rw-   0        0        0     1124 2023-07-10 07:31:04.000000 pudu-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      129 2022-11-04 23:37:34.000000 pudu-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4517 2023-07-11 10:01:04.959476 pudu-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3681 2023-05-17 09:45:31.000000 pudu-0.3.1/README.md
+-rw-rw-rw-   0        0        0     3721 2023-05-17 09:45:54.000000 pudu-0.3.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-11 10:01:04.907753 pudu-0.3.1/pudu/
+-rw-rw-rw-   0        0        0      137 2023-07-11 09:56:27.000000 pudu-0.3.1/pudu/__init__.py
+-rw-rw-rw-   0        0        0     4461 2023-07-08 13:16:56.000000 pudu-0.3.1/pudu/error_handler.py
+-rw-rw-rw-   0        0        0     2616 2023-07-09 10:38:07.000000 pudu-0.3.1/pudu/masks.py
+-rw-rw-rw-   0        0        0    12316 2023-07-08 15:34:18.000000 pudu-0.3.1/pudu/perturbation.py
+-rw-rw-rw-   0        0        0    13835 2023-07-11 09:47:35.000000 pudu-0.3.1/pudu/plots.py
+-rw-rw-rw-   0        0        0    28395 2023-07-11 09:54:31.000000 pudu-0.3.1/pudu/pudu.py
+-rw-rw-rw-   0        0        0     2941 2023-07-08 14:00:15.000000 pudu-0.3.1/pudu/standards.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:01:04.957664 pudu-0.3.1/pudu.egg-info/
+-rw-rw-rw-   0        0        0     4517 2023-07-11 10:01:04.000000 pudu-0.3.1/pudu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-07-11 10:01:04.000000 pudu-0.3.1/pudu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       62 2023-07-11 10:01:04.000000 pudu-0.3.1/pudu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-11-22 10:14:32.000000 pudu-0.3.1/pudu.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       62 2023-07-11 10:01:04.000000 pudu-0.3.1/pudu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-11 10:01:04.000000 pudu-0.3.1/pudu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      164 2022-02-13 18:34:42.000000 pudu-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       66 2023-06-28 13:59:09.000000 pudu-0.3.1/requirements.txt
+-rw-rw-rw-   0        0        0      449 2023-07-11 10:01:04.959476 pudu-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1844 2023-07-11 09:56:02.000000 pudu-0.3.1/setup.py
```

### Comparing `pudu-0.3.0/LICENSE` & `pudu-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pudu-0.3.0/PKG-INFO` & `pudu-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pudu
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python library for explainability of machine learinng algorithms in an agnostic, deterministic, and simple way.
 Home-page: https://github.com/pudu-py/pudu
 Author: pudu
 Author-email: puduhola@gmail.com
 License: MIT license
 Keywords: pudu
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pudu-0.3.0/README.md` & `pudu-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pudu-0.3.0/README.rst` & `pudu-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `pudu-0.3.0/pudu/error_handler.py` & `pudu-0.3.1/pudu/error_handler.py`

 * *Files identical despite different names*

### Comparing `pudu-0.3.0/pudu/masks.py` & `pudu-0.3.1/pudu/masks.py`

 * *Files identical despite different names*

### Comparing `pudu-0.3.0/pudu/perturbation.py` & `pudu-0.3.1/pudu/perturbation.py`

 * *Files identical despite different names*

### Comparing `pudu-0.3.0/pudu/plots.py` & `pudu-0.3.1/pudu/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import matplotlib.pyplot as plt
+from matplotlib import ticker
 import matplotlib as mpl
 import numpy as np
 
 def plot(feature, image, axis=None, show_data=True, title='Importance', 
         xlabel='Feature', ylabel='Intensity', xticks=None, yticks=[], cmap='Greens',
-        font_size=15, figsize=(14, 4)):
+        font_size=15, figsize=(14, 4), padding=(0, 0, 1, 1), cbar_pad=0.05, vmin=None,
+        vmax=None):
     """
     Easy plot function for `importance`, `speed`, or `synergy`. It shows the analyzed
         feature `feature` with a colormap overlay indicating the result along with
         a colorbar. Works for both vectors and images.
 
     :type feature: list
     :param feature: feature analyzed or any that the user whant to plot against.
@@ -49,45 +51,55 @@
     :param figsize: Size of the figure. Default is `(14, 4)`.
     """
 
     dims = np.array(image).shape
 
     image = np.array(image)[0,:,:,0]
     feature = np.array(feature)[0,:,:,0]
-    
+
+    if vmin is None:
+        vmin = np.min(image)
+        
+    if vmax is None:
+        vmax = np.max(image)
+
     if dims[1] > 1:
         rows, cols = dims[1], dims[2]
         ext = [0, cols, 0, rows]
     else:
         rows, cols = 1, len(image)
                 
         if axis is None:
             axis = [i for i in range(len(feature[0]))]
             ext = [0, len(feature[0]), min(feature[0]), max(feature[0])]
         else:
             ext = [min(axis), max(axis), min(feature[0]), max(feature[0])]
     
     plt.rc('font', size=font_size)
+    plt.subplots_adjust(left=padding[0], bottom=padding[1], right=padding[2], top=padding[3])
     plt.figure(figsize=figsize)
     if dims[1] > 1 and show_data:
         plt.imshow(feature, cmap='binary', aspect="auto", 
-                    interpolation='nearest', extent=ext, alpha=1)
+                    interpolation='nearest', extent=ext, alpha=1,
+                    vmin=vmin, vmax=vmax)
     elif dims[1] == 1 and show_data:
         plt.plot(axis, feature[0], 'k')
     plt.imshow(image, cmap=cmap, aspect="auto", 
-                interpolation='nearest', extent=ext, alpha=0.5)
+                interpolation='nearest', extent=ext, alpha=0.5,
+                vmin=vmin, vmax=vmax)
     plt.title(title) 
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
     plt.yticks(yticks)
-
+  
     if xticks:
         plt.xticks(axis, xticks, rotation='vertical')
-
-    plt.colorbar()
+    
+    plt.tight_layout()
+    plt.colorbar(pad=cbar_pad, ticks=ticker.LinearLocator(numticks=5))
     plt.show()  
 
 
 def feature_report(aso, plot=True, print_report=False, sort=True, title='Feature Report', 
                     ylabel='Counts', xlabel='Feature', fig_size=(7,5), rot_ticks=45, 
                     bar_width=0.9, background_color='thistle', bar_color='purple', 
                     x_lims=(-0.5, -0.61), borders=True, font_size=14,
```

### Comparing `pudu-0.3.0/pudu/pudu.py` & `pudu-0.3.1/pudu/pudu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections import defaultdict, Counter
+import matplotlib.pyplot as plt
 from keras.models import Model
 import numpy as np
 import copy
 
 from . import error_handler, standards
 from . import masks as msk
 from . import perturbation as ptn
```

### Comparing `pudu-0.3.0/pudu/standards.py` & `pudu-0.3.1/pudu/standards.py`

 * *Files identical despite different names*

### Comparing `pudu-0.3.0/pudu.egg-info/PKG-INFO` & `pudu-0.3.1/pudu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pudu
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python library for explainability of machine learinng algorithms in an agnostic, deterministic, and simple way.
 Home-page: https://github.com/pudu-py/pudu
 Author: pudu
 Author-email: puduhola@gmail.com
 License: MIT license
 Keywords: pudu
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pudu-0.3.0/setup.py` & `pudu-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='pudu',
     name='pudu',
     packages=find_packages(include=['pudu', 'pudu.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/pudu-py/pudu',
-    version='0.3.0',
+    version='0.3.1',
     zip_safe=False,
 )
```

