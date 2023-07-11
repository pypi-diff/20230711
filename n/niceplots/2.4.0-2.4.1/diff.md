# Comparing `tmp/niceplots-2.4.0-py3-none-any.whl.zip` & `tmp/niceplots-2.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 17416 bytes, number of entries: 11
--rw-r--r--  2.0 unx       66 b- defN 23-Jun-09 15:52 niceplots/__init__.py
--rw-r--r--  2.0 unx     3452 b- defN 23-Jun-09 15:52 niceplots/parula.py
--rw-r--r--  2.0 unx    37149 b- defN 23-Jun-09 15:52 niceplots/utils.py
--rw-r--r--  2.0 unx     1146 b- defN 23-Jun-09 15:52 niceplots/styles/doumont-dark.mplstyle
--rw-r--r--  2.0 unx     1112 b- defN 23-Jun-09 15:52 niceplots/styles/doumont-light.mplstyle
--rw-r--r--  2.0 unx      909 b- defN 23-Jun-09 15:52 niceplots/styles/james-dark.mplstyle
--rw-r--r--  2.0 unx      904 b- defN 23-Jun-09 15:52 niceplots/styles/james-light.mplstyle
--rw-r--r--  2.0 unx     4491 b- defN 23-Jun-09 15:52 niceplots-2.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 15:52 niceplots-2.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-09 15:52 niceplots-2.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      910 b- defN 23-Jun-09 15:52 niceplots-2.4.0.dist-info/RECORD
-11 files, 50241 bytes uncompressed, 15870 bytes compressed:  68.4%
+Zip file size: 17424 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       66 b- defN 23-Jul-11 21:03 niceplots/__init__.py
+-rw-r--r--  2.0 unx     3452 b- defN 23-Jul-11 21:03 niceplots/parula.py
+-rw-r--r--  2.0 unx    37165 b- defN 23-Jul-11 21:03 niceplots/utils.py
+-rw-r--r--  2.0 unx     1146 b- defN 23-Jul-11 21:03 niceplots/styles/doumont-dark.mplstyle
+-rw-r--r--  2.0 unx     1112 b- defN 23-Jul-11 21:03 niceplots/styles/doumont-light.mplstyle
+-rw-r--r--  2.0 unx      909 b- defN 23-Jul-11 21:03 niceplots/styles/james-dark.mplstyle
+-rw-r--r--  2.0 unx      904 b- defN 23-Jul-11 21:03 niceplots/styles/james-light.mplstyle
+-rw-r--r--  2.0 unx     4491 b- defN 23-Jul-11 21:03 niceplots-2.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 21:03 niceplots-2.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-11 21:03 niceplots-2.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      910 b- defN 23-Jul-11 21:03 niceplots-2.4.1.dist-info/RECORD
+11 files, 50257 bytes uncompressed, 15878 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: niceplots/styles/james-dark.mplstyle
 Comment: 
 
 Filename: niceplots/styles/james-light.mplstyle
 Comment: 
 
-Filename: niceplots-2.4.0.dist-info/METADATA
+Filename: niceplots-2.4.1.dist-info/METADATA
 Comment: 
 
-Filename: niceplots-2.4.0.dist-info/WHEEL
+Filename: niceplots-2.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: niceplots-2.4.0.dist-info/top_level.txt
+Filename: niceplots-2.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: niceplots-2.4.0.dist-info/RECORD
+Filename: niceplots-2.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## niceplots/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = "2.4.0"
+__version__ = "2.4.1"
 
 from .utils import *
 from .parula import *
```

## niceplots/utils.py

```diff
@@ -335,16 +335,16 @@
     color : str
         hexcode for the color of the scatter points used
 
     Returns
     -------
     fig: matplotlib Figure
         Figure created
-    ax: matplotlib Axes
-        Axes on which data is plotted
+    axes: array of matplotlib Axes
+        The subplot axes, one for each bar
     """
 
     # Use the first color if none is specified
     if color is None:
         color = get_colors_list()[0]
     style_colors = get_colors()
     line_color = style_colors["Axis"]
@@ -352,25 +352,25 @@
     # Obtain parameters to size the chart correctly
     num = len(times)
     width = size[0]
     height = size[1] * num
     t_max = max(times)
 
     # Create the corresponding number of subplots for each individual timing
-    fig, axarr = plt.subplots(num, 1, figsize=[width, height])
+    fig, axes = plt.subplots(num, 1, figsize=[width, height])
 
     # Loop over each time and get the max number of digits
     t_max_digits = 0
     for t in times:
         tm = len(str(int(t)))
         if tm > t_max_digits:
             t_max_digits = tm
 
     # Actual loop that draws each bar
-    for j, (l, t, ax) in enumerate(zip(labels, times, axarr)):
+    for j, (l, t, ax) in enumerate(zip(labels, times, axes)):
         # Draw the gray line and singular yellow dot
         ax.axhline(y=1, c=line_color, lw=3, zorder=0, alpha=0.5)
         ax.scatter([t], [1], c=color, lw=0, s=100, zorder=1, clip_on=False)
 
         # Set chart properties
         ax.set_ylim(0.99, 1.01)
         ax.set_xlim(0, t_max * 1.05)
@@ -401,15 +401,15 @@
         )
 
         # Create the top bar line
         if j == 0:
             ax.text(0, 1.02, header[0], ha="right", fontweight="bold", fontsize="large")
             ax.text(t_max, 1.02, header[1], ha="left", fontweight="bold", fontsize="large")
 
-    return fig, ax
+    return fig, axes
 
 
 def stacked_plots(
     xlabel,
     xdata,
     data_dict_list,
     figsize=(12, 10),
```

## Comparing `niceplots-2.4.0.dist-info/METADATA` & `niceplots-2.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niceplots
-Version: 2.4.0
+Version: 2.4.1
 Summary: Plotting utilities for matplotlib in python
 Home-page: https://github.com/mdolab/niceplots
 Author: 
 Author-email: 
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `niceplots-2.4.0.dist-info/RECORD` & `niceplots-2.4.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-niceplots/__init__.py,sha256=Dg11PWdNO-v99L9OX7PyMQyd5gUefeQlS7Mzit4UbVo,66
+niceplots/__init__.py,sha256=pkSSaTvvs-E2zEb_ygJgSVmrS7ftSkDCQ0aMuU1G3CM,66
 niceplots/parula.py,sha256=by5EIIIjnxZalrrgXHkcT5PeIiT7rv6bn-W3rg3VaOU,3452
-niceplots/utils.py,sha256=I2GykuvCLeamqrWbx9VXRdrAIqPCaSlLni1mDQjc5hw,37149
+niceplots/utils.py,sha256=JnELeZ8EM2tIgNnpdsVoIxiYdDCU0jP3Bca7q3x0Yn4,37165
 niceplots/styles/doumont-dark.mplstyle,sha256=8S0wCuAk7YYTWmY4wZ5mgDoyYAsS6yx5Uv5oNdNXIKc,1146
 niceplots/styles/doumont-light.mplstyle,sha256=cxNC2Au1VLDVizB7pQXcAZZbCCrVVLab_fNsChmsURE,1112
 niceplots/styles/james-dark.mplstyle,sha256=xoIEscAkdxItnivxgBLQ1RZ2-t9lTDsctebEdNlcIlk,909
 niceplots/styles/james-light.mplstyle,sha256=OYy_nIw0GDbKhJmN2LX8zzqeW6IfO7pHv_1i-0eeddI,904
-niceplots-2.4.0.dist-info/METADATA,sha256=_AAuZAEroLumLG67yHLUMN-4cb7FJMWTCQQf-poL1Bg,4491
-niceplots-2.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-niceplots-2.4.0.dist-info/top_level.txt,sha256=AXPTUh13A4r5iKtvXz0ZzOPnkrYIDczBiw3z9IyS4uI,10
-niceplots-2.4.0.dist-info/RECORD,,
+niceplots-2.4.1.dist-info/METADATA,sha256=8dJitEIkZI4bVF76mFiCkfDBf8uJBxBfYRfGltzwkcQ,4491
+niceplots-2.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+niceplots-2.4.1.dist-info/top_level.txt,sha256=AXPTUh13A4r5iKtvXz0ZzOPnkrYIDczBiw3z9IyS4uI,10
+niceplots-2.4.1.dist-info/RECORD,,
```

