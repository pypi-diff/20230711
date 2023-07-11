# Comparing `tmp/metalmaps-1.0.0.tar.gz` & `tmp/metalmaps-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalmaps-1.0.0.tar", last modified: Sun Jul  9 20:43:39 2023, max compression
+gzip compressed data, was "metalmaps-2.0.0.tar", last modified: Tue Jul 11 18:11:05 2023, max compression
```

## Comparing `metalmaps-1.0.0.tar` & `metalmaps-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:43:39.004961 metalmaps-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-09 20:43:28.000000 metalmaps-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-09 20:43:28.000000 metalmaps-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-07-09 20:43:39.004961 metalmaps-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-07-09 20:43:28.000000 metalmaps-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:43:39.004961 metalmaps-1.0.0/metalmaps/
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-07-09 20:43:28.000000 metalmaps-1.0.0/metalmaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 20:43:28.000000 metalmaps-1.0.0/metalmaps/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-09 20:43:28.000000 metalmaps-1.0.0/metalmaps/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-09 20:43:28.000000 metalmaps-1.0.0/metalmaps/make_cmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:43:39.004961 metalmaps-1.0.0/metalmaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-07-09 20:43:38.000000 metalmaps-1.0.0/metalmaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-09 20:43:39.000000 metalmaps-1.0.0/metalmaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:43:38.000000 metalmaps-1.0.0/metalmaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 20:43:38.000000 metalmaps-1.0.0/metalmaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 20:43:38.000000 metalmaps-1.0.0/metalmaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-09 20:43:28.000000 metalmaps-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 20:43:39.008961 metalmaps-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:11:05.254760 metalmaps-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-11 18:10:55.000000 metalmaps-2.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 18:10:55.000000 metalmaps-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15629 2023-07-11 18:11:05.254760 metalmaps-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-11 18:10:55.000000 metalmaps-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:11:05.254760 metalmaps-2.0.0/metalmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-11 18:10:55.000000 metalmaps-2.0.0/metalmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 18:10:55.000000 metalmaps-2.0.0/metalmaps/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-11 18:10:55.000000 metalmaps-2.0.0/metalmaps/colorcycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-07-11 18:10:55.000000 metalmaps-2.0.0/metalmaps/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-11 18:10:55.000000 metalmaps-2.0.0/metalmaps/make_cmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:11:05.254760 metalmaps-2.0.0/metalmaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15629 2023-07-11 18:11:05.000000 metalmaps-2.0.0/metalmaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-11 18:11:05.000000 metalmaps-2.0.0/metalmaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:11:05.000000 metalmaps-2.0.0/metalmaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 18:11:05.000000 metalmaps-2.0.0/metalmaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 18:11:05.000000 metalmaps-2.0.0/metalmaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-11 18:10:55.000000 metalmaps-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:11:05.254760 metalmaps-2.0.0/setup.cfg
```

### Comparing `metalmaps-1.0.0/LICENSE.txt` & `metalmaps-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `metalmaps-1.0.0/PKG-INFO` & `metalmaps-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalmaps
-Version: 1.0.0
+Version: 2.0.0
 Summary: Metal and rock inspired Matplotlib colormaps.
 Author-email: Mladen Ivkovic <mladen.ivkovic@hotmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -174,27 +174,34 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-## Metalmaps - Heavy Metal and Classic Rock Album Art Inspired Matplotlib Colormaps
+Metalmaps - Heavy Metal and Classic Rock Album Art Inspired Matplotlib Colormaps
+----------------------------------------------------------------------------------
 
 Ever wanted to make your python plots more metal? Fear not, now you can! `metalmaps`
 delivers heavy metal and classic rock album art inspired `matplotlib` colormaps!
 
-All of this was inspired by (and shamelessly copied from) Josh Borrow's 
-[swiftascmaps](https://github.com/jborrow/swiftascmaps).
+Visit the [gallery](https://mladenivkovic.github.io/metalmaps/metalmaps.html) for a
+comprehensive picture.
 
-License: LGPLv3
 
-Authors: Mladen Ivkovic, Josh Borrow
 
+Contents
+------------------
 
++ [Installation](#installation)
++ [Usage](#usage)
++ [Examples](#examples)
++ [Note](#note)
++ [Contributing](#contributing)
++ [Authors, License, Credits](#authors-license-credits)
 
 
 Installation
 ------------------
 
 Install this package via pip:
 
@@ -202,15 +209,15 @@
 pip install metalmaps
 ```
 
 Alternatively, grab the source from [github](https://github.com/mladenivkovic/metalmaps).
 
 
 Usage
------
+-------
 
 To use these, you can import them and use them
 with matplotlib as you would with any other color map.
 
 ```python
 from metalmaps import black_sabbath
 from matplotlib.pyplot import imshow
@@ -225,14 +232,64 @@
 ```python
 import metalmaps
 
 imshow(random.rand(128, 128), cmap="metalmaps.red")
 ```
 
 
+### Using a colormap as default line colors in plots
+
+It's possible to replace the default matplotlib color cycle with one
+provided by this package. To achieve this, call the provided
+`metalmaps.set_color_cycle()` function, and pass the colormap you 
+want as the argument, e.g:
+
+```python
+import metalmaps
+metalmaps.set_color_cycle(metalmaps.reign_in_blood)
+```
+
+For example, this code
+
+```python
+from matplotlib import pyplot as plt
+import numpy as np
+
+import metalmaps
+metalmaps.set_color_cycle(metalmaps.reign_in_blood)
+
+x = np.linspace(0, 1.4, 200)
+def y(x, phi):
+    return np.sin(1.2 * np.pi * (x + 0.25) - 0.1 * phi)
+
+plt.figure()
+
+for i in range(10):
+    labelname = label="C"+str(i)
+    plt.plot(x, y(x, i), linewidth=5, label=labelname)
+
+plt.legend(ncols=2)
+plt.tight_layout()
+plt.savefig("my_figure.png")
+
+```
+
+results in the following figure:
+
+![](images/lineplot.png)
+
+where we didn't have to specify the different colors each time we
+called ``plot()``.
+
+
+
+
+
+
+
 
 Examples
 --------
 
 This package currently includes 30 colormaps: 
 
 
@@ -347,13 +404,30 @@
 + add your addition to the album lists in `README.md` and `__init__.py`
 + submit your merge request
 + ???
 + profit!
 
 
 
-Image Credits
--------------
+Authors, License, Credits
+---------------------------
+
+### Credits
+
+All of this was inspired by (and shamelessly copied from) Josh Borrow's 
+[swiftascmaps](https://github.com/jborrow/swiftascmaps).
+
+Image credits:
 
 + The "Kelvin-Helmholtz" data used in the plots below were generated using [mesh-hydro](https://github.com/mladenivkovic/mesh-hydro).
 + The "EAGLE" data used in the plots below were obtained from the [swiftsim](https://github.com/SWIFTSIM/SWIFT) repository.
 + The "NGC" data used in the plots below were originally obtained from [flickr](https://www.flickr.com/photos/geckzilla/52040747525/), credits to [Judy Schmidt](https://www.flickr.com/people/geckzilla/). I modified the image later to normalize the pixel values to be able to demonstrate the colormaps as above.
+
+
+### License
+
+License: LGPLv3
+
+
+### Authors and Contributors
+Mladen Ivkovic, Josh Borrow
+
```

### Comparing `metalmaps-1.0.0/README.md` & `metalmaps-2.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-## Metalmaps - Heavy Metal and Classic Rock Album Art Inspired Matplotlib Colormaps
+Metalmaps - Heavy Metal and Classic Rock Album Art Inspired Matplotlib Colormaps
+----------------------------------------------------------------------------------
 
 Ever wanted to make your python plots more metal? Fear not, now you can! `metalmaps`
 delivers heavy metal and classic rock album art inspired `matplotlib` colormaps!
 
-All of this was inspired by (and shamelessly copied from) Josh Borrow's 
-[swiftascmaps](https://github.com/jborrow/swiftascmaps).
+Visit the [gallery](https://mladenivkovic.github.io/metalmaps/metalmaps.html) for a
+comprehensive picture.
 
-License: LGPLv3
 
-Authors: Mladen Ivkovic, Josh Borrow
 
+Contents
+------------------
 
++ [Installation](#installation)
++ [Usage](#usage)
++ [Examples](#examples)
++ [Note](#note)
++ [Contributing](#contributing)
++ [Authors, License, Credits](#authors-license-credits)
 
 
 Installation
 ------------------
 
 Install this package via pip:
 
@@ -22,15 +29,15 @@
 pip install metalmaps
 ```
 
 Alternatively, grab the source from [github](https://github.com/mladenivkovic/metalmaps).
 
 
 Usage
------
+-------
 
 To use these, you can import them and use them
 with matplotlib as you would with any other color map.
 
 ```python
 from metalmaps import black_sabbath
 from matplotlib.pyplot import imshow
@@ -45,14 +52,64 @@
 ```python
 import metalmaps
 
 imshow(random.rand(128, 128), cmap="metalmaps.red")
 ```
 
 
+### Using a colormap as default line colors in plots
+
+It's possible to replace the default matplotlib color cycle with one
+provided by this package. To achieve this, call the provided
+`metalmaps.set_color_cycle()` function, and pass the colormap you 
+want as the argument, e.g:
+
+```python
+import metalmaps
+metalmaps.set_color_cycle(metalmaps.reign_in_blood)
+```
+
+For example, this code
+
+```python
+from matplotlib import pyplot as plt
+import numpy as np
+
+import metalmaps
+metalmaps.set_color_cycle(metalmaps.reign_in_blood)
+
+x = np.linspace(0, 1.4, 200)
+def y(x, phi):
+    return np.sin(1.2 * np.pi * (x + 0.25) - 0.1 * phi)
+
+plt.figure()
+
+for i in range(10):
+    labelname = label="C"+str(i)
+    plt.plot(x, y(x, i), linewidth=5, label=labelname)
+
+plt.legend(ncols=2)
+plt.tight_layout()
+plt.savefig("my_figure.png")
+
+```
+
+results in the following figure:
+
+![](images/lineplot.png)
+
+where we didn't have to specify the different colors each time we
+called ``plot()``.
+
+
+
+
+
+
+
 
 Examples
 --------
 
 This package currently includes 30 colormaps: 
 
 
@@ -167,13 +224,30 @@
 + add your addition to the album lists in `README.md` and `__init__.py`
 + submit your merge request
 + ???
 + profit!
 
 
 
-Image Credits
--------------
+Authors, License, Credits
+---------------------------
+
+### Credits
+
+All of this was inspired by (and shamelessly copied from) Josh Borrow's 
+[swiftascmaps](https://github.com/jborrow/swiftascmaps).
+
+Image credits:
 
 + The "Kelvin-Helmholtz" data used in the plots below were generated using [mesh-hydro](https://github.com/mladenivkovic/mesh-hydro).
 + The "EAGLE" data used in the plots below were obtained from the [swiftsim](https://github.com/SWIFTSIM/SWIFT) repository.
 + The "NGC" data used in the plots below were originally obtained from [flickr](https://www.flickr.com/photos/geckzilla/52040747525/), credits to [Judy Schmidt](https://www.flickr.com/people/geckzilla/). I modified the image later to normalize the pixel values to be able to demonstrate the colormaps as above.
+
+
+### License
+
+License: LGPLv3
+
+
+### Authors and Contributors
+Mladen Ivkovic, Josh Borrow
+
```

### Comparing `metalmaps-1.0.0/metalmaps/__init__.py` & `metalmaps-2.0.0/metalmaps/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
     imshow(random.rand(128, 128), cmap=black_sabbath)
 
 """
 
 import metalmaps.colors as colors
 from metalmaps.make_cmap import make_custom_cmap
+from metalmaps.colorcycle import set_color_cycle
 from metalmaps.__version__ import __version__
 
 apostasy, apostasy_r = make_custom_cmap("apostasy", colors.apostasy)
 ashes_of_the_wake, ashes_of_the_wake_r = make_custom_cmap(
     "ashes_of_the_wake", colors.ashes_of_the_wake
 )
 blues_brothers, blues_brothers_r = make_custom_cmap(
```

### Comparing `metalmaps-1.0.0/metalmaps/colors.py` & `metalmaps-2.0.0/metalmaps/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         "#F4F3F1",
         "#26180C",
         "#000000",
     ]
 )
 
 london_calling = hex_to_rgb(
-    ["#130b0a", "#2e2724", "#1b9045", "c8c0b0", "#989989", "#6b625a", "d86a7d"]
+    ["#130b0a", "#2e2724", "#1b9045", "#c8c0b0", "#989989", "#6b625a", "#d86a7d"]
 )
 
 master_of_puppets = hex_to_rgb(
     [
         "#160907",
         "#2D0509",
         "#4C2415",
@@ -230,18 +230,18 @@
     [
         "#12090a",
         "#323a47",
         "#33386a",
         "#475383",
         "#506c8e",
         "#9382af",
-        "b3b1c6",
-        "dcdde3",
-        "e1bf30",
-        "e13421",
+        "#b3b1c6",
+        "#dcdde3",
+        "#e1bf30",
+        "#e13421",
     ]
 )
 
 obzen = hex_to_rgb(
     [
         "#0A0908",
         "#242324",
```

### Comparing `metalmaps-1.0.0/metalmaps/make_cmap.py` & `metalmaps-2.0.0/metalmaps/make_cmap.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Wrapper function for making color maps from lists
 of colors.
 """
 
 from matplotlib.cm import register_cmap
-from matplotlib.colors import LinearSegmentedColormap
+from matplotlib.colors import LinearSegmentedColormap, to_rgb
 from typing import List, Tuple
 
 
 def hex_to_rgb(colors: List[str]) -> List[List[int]]:
     """
     Converts colors from hex codes to 8-bit integer RGB values.
 
@@ -23,24 +23,21 @@
 
     rgb_colors: List[List[int]]
         List of colors formatted as rgb [[0, 0, 0]]
     """
 
     rgb_colors = []
 
-    # clean up formatting without leading '#'
-    cleaned_colors = []
     for color in colors:
-        if color.startswith("#"):
-            cleaned_colors.append(color)
-        else:
-            cleaned_colors.append("#" + color)
+        # clean up formatting without leading '#'
+        if not color.startswith("#"):
+            color = "#" + color
 
-    for color in cleaned_colors:
-        rgb_colors.append(list(int(color[1:][i : i + 2], 16) for i in (0, 2, 4)))
+        #  rgb_colors.append(list(int(color[1:][i : i + 2], 16) for i in (0, 2, 4)))
+        rgb_colors.append([int(rgb * 256) for rgb in to_rgb(color)])
 
     return rgb_colors
 
 
 def make_custom_cmap(name: str, colors: List) -> Tuple[LinearSegmentedColormap]:
     """
     Makes a custom color map from your set of colors, and returns
```

### Comparing `metalmaps-1.0.0/metalmaps.egg-info/PKG-INFO` & `metalmaps-2.0.0/metalmaps.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalmaps
-Version: 1.0.0
+Version: 2.0.0
 Summary: Metal and rock inspired Matplotlib colormaps.
 Author-email: Mladen Ivkovic <mladen.ivkovic@hotmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -174,27 +174,34 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-## Metalmaps - Heavy Metal and Classic Rock Album Art Inspired Matplotlib Colormaps
+Metalmaps - Heavy Metal and Classic Rock Album Art Inspired Matplotlib Colormaps
+----------------------------------------------------------------------------------
 
 Ever wanted to make your python plots more metal? Fear not, now you can! `metalmaps`
 delivers heavy metal and classic rock album art inspired `matplotlib` colormaps!
 
-All of this was inspired by (and shamelessly copied from) Josh Borrow's 
-[swiftascmaps](https://github.com/jborrow/swiftascmaps).
+Visit the [gallery](https://mladenivkovic.github.io/metalmaps/metalmaps.html) for a
+comprehensive picture.
 
-License: LGPLv3
 
-Authors: Mladen Ivkovic, Josh Borrow
 
+Contents
+------------------
 
++ [Installation](#installation)
++ [Usage](#usage)
++ [Examples](#examples)
++ [Note](#note)
++ [Contributing](#contributing)
++ [Authors, License, Credits](#authors-license-credits)
 
 
 Installation
 ------------------
 
 Install this package via pip:
 
@@ -202,15 +209,15 @@
 pip install metalmaps
 ```
 
 Alternatively, grab the source from [github](https://github.com/mladenivkovic/metalmaps).
 
 
 Usage
------
+-------
 
 To use these, you can import them and use them
 with matplotlib as you would with any other color map.
 
 ```python
 from metalmaps import black_sabbath
 from matplotlib.pyplot import imshow
@@ -225,14 +232,64 @@
 ```python
 import metalmaps
 
 imshow(random.rand(128, 128), cmap="metalmaps.red")
 ```
 
 
+### Using a colormap as default line colors in plots
+
+It's possible to replace the default matplotlib color cycle with one
+provided by this package. To achieve this, call the provided
+`metalmaps.set_color_cycle()` function, and pass the colormap you 
+want as the argument, e.g:
+
+```python
+import metalmaps
+metalmaps.set_color_cycle(metalmaps.reign_in_blood)
+```
+
+For example, this code
+
+```python
+from matplotlib import pyplot as plt
+import numpy as np
+
+import metalmaps
+metalmaps.set_color_cycle(metalmaps.reign_in_blood)
+
+x = np.linspace(0, 1.4, 200)
+def y(x, phi):
+    return np.sin(1.2 * np.pi * (x + 0.25) - 0.1 * phi)
+
+plt.figure()
+
+for i in range(10):
+    labelname = label="C"+str(i)
+    plt.plot(x, y(x, i), linewidth=5, label=labelname)
+
+plt.legend(ncols=2)
+plt.tight_layout()
+plt.savefig("my_figure.png")
+
+```
+
+results in the following figure:
+
+![](images/lineplot.png)
+
+where we didn't have to specify the different colors each time we
+called ``plot()``.
+
+
+
+
+
+
+
 
 Examples
 --------
 
 This package currently includes 30 colormaps: 
 
 
@@ -347,13 +404,30 @@
 + add your addition to the album lists in `README.md` and `__init__.py`
 + submit your merge request
 + ???
 + profit!
 
 
 
-Image Credits
--------------
+Authors, License, Credits
+---------------------------
+
+### Credits
+
+All of this was inspired by (and shamelessly copied from) Josh Borrow's 
+[swiftascmaps](https://github.com/jborrow/swiftascmaps).
+
+Image credits:
 
 + The "Kelvin-Helmholtz" data used in the plots below were generated using [mesh-hydro](https://github.com/mladenivkovic/mesh-hydro).
 + The "EAGLE" data used in the plots below were obtained from the [swiftsim](https://github.com/SWIFTSIM/SWIFT) repository.
 + The "NGC" data used in the plots below were originally obtained from [flickr](https://www.flickr.com/photos/geckzilla/52040747525/), credits to [Judy Schmidt](https://www.flickr.com/people/geckzilla/). I modified the image later to normalize the pixel values to be able to demonstrate the colormaps as above.
+
+
+### License
+
+License: LGPLv3
+
+
+### Authors and Contributors
+Mladen Ivkovic, Josh Borrow
+
```

### Comparing `metalmaps-1.0.0/pyproject.toml` & `metalmaps-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 [tool.setuptools]
 packages = ["metalmaps"]
 
 [project]
 name = "metalmaps"
 description="Metal and rock inspired Matplotlib colormaps."
 readme = "README.md"
-version = "1.0.0"
+version = "2.0.0"
 authors= [
     { name = "Mladen Ivkovic", email="mladen.ivkovic@hotmail.com"},
     ]
 license = { file = "LICENSE.txt" }
 classifiers=[
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Operating System :: OS Independent"
 ]
 keywords = [ "metal", "rock", "colormap", "matplotlib" ]
-dependencies=[ "matplotlib" ]
+dependencies=[ "matplotlib", "cycler" ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/mladenivkovic/metalmaps"
 "Gallery" = "https://mladenivkovic.github.io/metalmaps/metalmaps.html"
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "2.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

