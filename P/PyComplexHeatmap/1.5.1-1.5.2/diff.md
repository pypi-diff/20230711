# Comparing `tmp/PyComplexHeatmap-1.5.1.tar.gz` & `tmp/PyComplexHeatmap-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComplexHeatmap-1.5.1.tar", last modified: Fri Jun 16 19:01:38 2023, max compression
+gzip compressed data, was "PyComplexHeatmap-1.5.2.tar", last modified: Tue Jul 11 17:11:53 2023, max compression
```

## Comparing `PyComplexHeatmap-1.5.1.tar` & `PyComplexHeatmap-1.5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-06-16 19:01:38.429423 PyComplexHeatmap-1.5.1/
--rw-r--r--   0 wding      (503) staff       (20)     1067 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.1/LICENSE
--rw-r--r--   0 wding      (503) staff       (20)      105 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.1/MANIFEST.in
--rw-r--r--   0 wding      (503) staff       (20)    11894 2023-06-16 19:01:38.428834 PyComplexHeatmap-1.5.1/PKG-INFO
-drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-06-16 19:01:38.425075 PyComplexHeatmap-1.5.1/PyComplexHeatmap/
--rw-r--r--   0 wding      (503) staff       (20)      387 2023-06-16 18:59:50.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/__init__.py
--rw-r--r--   0 wding      (503) staff       (20)    66619 2023-06-16 18:42:57.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/annotations.py
--rw-r--r--   0 wding      (503) staff       (20)    75826 2023-06-16 18:44:04.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/clustermap.py
--rw-r--r--   0 wding      (503) staff       (20)     5430 2023-05-15 19:27:29.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/colors.py
--rw-r--r--   0 wding      (503) staff       (20)    21257 2023-06-09 16:20:57.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/dotHeatmap.py
--rw-r--r--   0 wding      (503) staff       (20)     6766 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/example.py
--rw-r--r--   0 wding      (503) staff       (20)    17872 2023-06-09 16:23:11.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/oncoPrint.py
--rw-r--r--   0 wding      (503) staff       (20)     6788 2023-06-09 16:21:38.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/tools.py
--rw-r--r--   0 wding      (503) staff       (20)    28836 2023-06-16 17:06:16.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/utils.py
-drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-06-16 19:01:38.428084 PyComplexHeatmap-1.5.1/PyComplexHeatmap.egg-info/
--rw-r--r--   0 wding      (503) staff       (20)    11894 2023-06-16 19:01:38.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap.egg-info/PKG-INFO
--rw-r--r--   0 wding      (503) staff       (20)      473 2023-06-16 19:01:38.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap.egg-info/SOURCES.txt
--rw-r--r--   0 wding      (503) staff       (20)        1 2023-06-16 19:01:38.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap.egg-info/dependency_links.txt
--rw-r--r--   0 wding      (503) staff       (20)       17 2023-06-16 19:01:38.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap.egg-info/top_level.txt
--rw-r--r--   0 wding      (503) staff       (20)    11285 2023-06-09 04:09:45.000000 PyComplexHeatmap-1.5.1/README.md
--rw-r--r--   0 wding      (503) staff       (20)      686 2023-06-16 18:59:11.000000 PyComplexHeatmap-1.5.1/pyproject.toml
--rw-r--r--   0 wding      (503) staff       (20)       38 2023-06-16 19:01:38.429647 PyComplexHeatmap-1.5.1/setup.cfg
--rw-r--r--   0 wding      (503) staff       (20)     1044 2023-06-16 18:59:26.000000 PyComplexHeatmap-1.5.1/setup.py
+drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-07-11 17:11:53.108732 PyComplexHeatmap-1.5.2/
+-rw-r--r--   0 wding      (503) staff       (20)     1067 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.2/LICENSE
+-rw-r--r--   0 wding      (503) staff       (20)      105 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.2/MANIFEST.in
+-rw-r--r--   0 wding      (503) staff       (20)    11925 2023-07-11 17:11:53.108010 PyComplexHeatmap-1.5.2/PKG-INFO
+drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-07-11 17:11:53.104495 PyComplexHeatmap-1.5.2/PyComplexHeatmap/
+-rw-r--r--   0 wding      (503) staff       (20)      387 2023-07-11 17:10:14.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/__init__.py
+-rw-r--r--   0 wding      (503) staff       (20)    66678 2023-07-11 17:05:35.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/annotations.py
+-rw-r--r--   0 wding      (503) staff       (20)    75906 2023-07-10 17:29:22.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/clustermap.py
+-rw-r--r--   0 wding      (503) staff       (20)     5430 2023-05-15 19:27:29.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/colors.py
+-rw-r--r--   0 wding      (503) staff       (20)    21257 2023-06-09 16:20:57.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/dotHeatmap.py
+-rw-r--r--   0 wding      (503) staff       (20)     6766 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/example.py
+-rw-r--r--   0 wding      (503) staff       (20)    17872 2023-06-09 16:23:11.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/oncoPrint.py
+-rw-r--r--   0 wding      (503) staff       (20)     6788 2023-06-09 16:21:38.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/tools.py
+-rw-r--r--   0 wding      (503) staff       (20)    28838 2023-07-11 17:10:03.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/utils.py
+drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-07-11 17:11:53.107260 PyComplexHeatmap-1.5.2/PyComplexHeatmap.egg-info/
+-rw-r--r--   0 wding      (503) staff       (20)    11925 2023-07-11 17:11:52.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap.egg-info/PKG-INFO
+-rw-r--r--   0 wding      (503) staff       (20)      473 2023-07-11 17:11:52.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 wding      (503) staff       (20)        1 2023-07-11 17:11:52.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 wding      (503) staff       (20)       17 2023-07-11 17:11:52.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap.egg-info/top_level.txt
+-rw-r--r--   0 wding      (503) staff       (20)    11316 2023-06-19 21:12:13.000000 PyComplexHeatmap-1.5.2/README.md
+-rw-r--r--   0 wding      (503) staff       (20)      686 2023-07-11 17:08:37.000000 PyComplexHeatmap-1.5.2/pyproject.toml
+-rw-r--r--   0 wding      (503) staff       (20)       38 2023-07-11 17:11:53.108937 PyComplexHeatmap-1.5.2/setup.cfg
+-rw-r--r--   0 wding      (503) staff       (20)     1044 2023-07-11 17:09:17.000000 PyComplexHeatmap-1.5.2/setup.py
```

### Comparing `PyComplexHeatmap-1.5.1/LICENSE` & `PyComplexHeatmap-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.5.1/PKG-INFO` & `PyComplexHeatmap-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.5.1
+Version: 1.5.2
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
@@ -41,14 +41,16 @@
 ```
 pip install --ignore-install matplotlib==3.5.1 numpy==1.20.3 pandas==1.4.1
 pip install seaborn #only needed when call functions in tools.py
 ```
 
 ## Citation
 Ding, W., Goldberg, D. and Zhou, W. (2023), PyComplexHeatmap: A Python package to visualize multimodal genomics data. iMeta e115. https://doi.org/10.1002/imt2.115
+<br>
+**DOI**: 10.1002/imt2.115
 
 ## **Installation**
 ----------------------
 1. **Install using pip**:
 ```shell
 pip install PyComplexHeatmap
```

### Comparing `PyComplexHeatmap-1.5.1/PyComplexHeatmap/annotations.py` & `PyComplexHeatmap-1.5.2/PyComplexHeatmap/annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,23 +180,23 @@
             assert len(colors) == self.df.iloc[:, 0].nunique()
             colors = {label: color for label, color in zip(self.df.iloc[:, 0].unique(), colors)}
         if not isinstance(colors, dict):
             raise TypeError("colors must be a dict!")
         if len(colors) >= self.df.iloc[:, 0].nunique():
             self.colors = colors
         else:
-            raise TypeError("Unknown type of colors")
+            raise TypeError("The length of `colors` is not consistent with the shape of the input data")
 
     def _calculate_cmap(self):
         self.color_dict = self.colors
         col = self.df.columns.tolist()[0]
         cc_list = list(self.color_dict.keys())  # column values
         self.df[col] = self.df[col].map({v: cc_list.index(v) for v in cc_list})
         self.cmap = matplotlib.colors.ListedColormap([self.color_dict[k] for k in cc_list])
-        self.plot_kws.setdefault('vmax', plt.colormaps.get(self.cmap).N)
+        self.plot_kws.setdefault('vmax', plt.colormaps.get(self.cmap).N-1)
         self.plot_kws.setdefault('vmin', 0)
 
     def _type_specific_params(self):
         pass
 
     def reorder(self, idx):  # Before plotting, df needs to be reordered according to the new clustered order.
         """
@@ -273,19 +273,19 @@
         cc_list = list(self.color_dict.keys())  # column values
         self.cc_list = cc_list
         self.cmap = matplotlib.colors.ListedColormap([self.color_dict[k] for k in cc_list])
 
     def plot(self, ax=None, axis=1, subplot_spec=None, label_kws={},
              ticklabels_kws={}):  # add self.gs,self.fig,self.ax,self.axes
         if hasattr(self.cmap,'N'):
-            vmax=self.cmap.N
+            vmax=self.cmap.N-1
         elif type(self.cmap)==str:
-            vmax=plt.colormaps.get(self.cmap).N
+            vmax=plt.colormaps.get(self.cmap).N-1
         else:
-            vmax=len(self.color_dict)
+            vmax=len(self.color_dict)-1
         self.plot_kws.setdefault('vmax',vmax)  # plt.colormaps.get(self.cmap).N
         self.plot_kws.setdefault('vmin', 0)
         if self.cc_list:
             mat = self.plot_data.iloc[:, 0].map({v: self.cc_list.index(v) for v in self.cc_list}).values
         else:
             mat = self.plot_data.values
         matrix = mat.reshape(1, -1) if axis == 1 else mat.reshape(-1, 1)
@@ -376,15 +376,15 @@
         self.luminance = luminance
         self.extend = extend
         self.frac = frac
         self.relpos = relpos
         self.annotated_texts = []
 
     def _height(self, height):
-        return 5 if height is None else height
+        return 4 if height is None else height
 
     def set_side(self, side):
         self.side = side
 
     def set_plot_kws(self, axis):
         shrink = 1  # 1 * mm2inch * 72  # 1mm -> points
         if axis == 1:  # columns
```

### Comparing `PyComplexHeatmap-1.5.1/PyComplexHeatmap/clustermap.py` & `PyComplexHeatmap-1.5.2/PyComplexHeatmap/clustermap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1133,21 +1133,22 @@
             #index=self.dendrogram_row.dendrogram['ivl']).to_frame(name='cluster')
 
         elif isinstance(self.row_split, (pd.Series, pd.DataFrame)):
             if isinstance(self.row_split, pd.Series):
                 self.row_split = self.row_split.to_frame(name=self.row_split.name)
             cols = self.row_split.columns.tolist()
             row_clusters = self.row_split.groupby(cols).apply(lambda x: x.index.tolist())
-            if len(cols)==1 and self.row_split_order is None:
-                # calculate row_split_order using the mean across all samples in this group of
-                # values of mean values across all samples
-                self.row_split_order = row_clusters.apply(lambda x: self.data2d.loc[x].mean(axis=1).mean())\
-                    .sort_values(ascending=False).index.tolist()
-            else:
-                self.row_split_order=row_clusters.sort_index().index.tolist()
+            if self.row_split_order is None:
+                if len(cols)==1:
+                    # calculate row_split_order using the mean across all samples in this group of
+                    # values of mean values across all samples
+                    self.row_split_order = row_clusters.apply(lambda x: self.data2d.loc[x].mean(axis=1).mean())\
+                        .sort_values(ascending=False).index.tolist()
+                else:
+                    self.row_split_order=row_clusters.sort_index().index.tolist()
             self.row_clusters = row_clusters.loc[self.row_split_order].to_dict()
         elif not self.row_cluster:
             self.row_order = [self.data2d.index.tolist()]
             return None
         else:
             raise TypeError("row_split must be integar or dataframe or series")
 
@@ -1182,21 +1183,22 @@
             #index=self.dendrogram_col.dendrogram['ivl']).to_frame(name='cluster')
 
         elif isinstance(self.col_split, (pd.Series, pd.DataFrame)):
             if isinstance(self.col_split, pd.Series):
                 self.col_split = self.col_split.to_frame(name=self.col_split.name)
             cols = self.col_split.columns.tolist()
             col_clusters = self.col_split.groupby(cols).apply(lambda x: x.index.tolist())
-            if len(cols)==1 and self.col_split_order is None:
-                # calculate col_split_order using the mean across all samples in this group of
-                # values of mean values across all samples
-                self.col_split_order = col_clusters.apply(lambda x: self.data2d.loc[:,x].mean().mean())\
-                    .sort_values(ascending=False).index.tolist()
-            else:
-                self.col_split_order=col_clusters.sort_index().index.tolist()
+            if self.col_split_order is None:
+                if len(cols)==1:
+                    # calculate col_split_order using the mean across all samples in this group of
+                    # values of mean values across all samples
+                    self.col_split_order = col_clusters.apply(lambda x: self.data2d.loc[:,x].mean().mean())\
+                        .sort_values(ascending=False).index.tolist()
+                else:
+                    self.col_split_order=col_clusters.sort_index().index.tolist()
             self.col_clusters = col_clusters.loc[self.col_split_order].to_dict()
         elif not self.col_cluster:
             self.col_order = [self.data2d.columns.tolist()]
             return None
         else:
             raise TypeError("row_split must be integar or dataframe or series")
```

### Comparing `PyComplexHeatmap-1.5.1/PyComplexHeatmap/colors.py` & `PyComplexHeatmap-1.5.2/PyComplexHeatmap/colors.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.5.1/PyComplexHeatmap/dotHeatmap.py` & `PyComplexHeatmap-1.5.2/PyComplexHeatmap/dotHeatmap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.5.1/PyComplexHeatmap/example.py` & `PyComplexHeatmap-1.5.2/PyComplexHeatmap/example.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.5.1/PyComplexHeatmap/oncoPrint.py` & `PyComplexHeatmap-1.5.2/PyComplexHeatmap/oncoPrint.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.5.1/PyComplexHeatmap/tools.py` & `PyComplexHeatmap-1.5.2/PyComplexHeatmap/tools.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.5.1/PyComplexHeatmap/utils.py` & `PyComplexHeatmap-1.5.2/PyComplexHeatmap/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -595,15 +595,15 @@
         left=ax.get_position().x0+ax.yaxis.labelpad*2/ax.figure.get_window_extent().width if delta_x is None else ax.get_position().x0+delta_x
     else:
         #labelpad: Spacing in points, pad is the fraction relative to x1.
         pad = (space+ax.yaxis.labelpad*1.2*ax.figure.dpi / 72) / ax.figure.get_window_extent().width if delta_x is None else delta_x #labelpad unit is points
         left=ax.get_position().x1 + pad
     if legend_width is None:
         legend_width=cal_legend_width(legend_list) + 2.5 #base width for color rectangle is set to 2.5 mm
-        print(f"Estimated legend width: {legend_width} mm")
+        # print(f"Estimated legend width: {legend_width} mm")
     legend_width=legend_width*mm2inch*ax.figure.dpi / ax.figure.get_window_extent().width #mm to px to fraction
     cmap_width = cmap_width * mm2inch * ax.figure.dpi / ax.figure.get_window_extent().width  # mm to px to fraction
     if legend_side=='right':
         ax_legend=ax.figure.add_axes([left,ax.get_position().y0,legend_width,ax.get_position().height]) #left, bottom, width, height
     legend_axes=[ax_legend]
     cbars=[]
     leg_pos = ax_legend.get_position() #left bototm: x0,y0; top right: x1,y1
```

### Comparing `PyComplexHeatmap-1.5.1/PyComplexHeatmap.egg-info/PKG-INFO` & `PyComplexHeatmap-1.5.2/PyComplexHeatmap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.5.1
+Version: 1.5.2
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
@@ -41,14 +41,16 @@
 ```
 pip install --ignore-install matplotlib==3.5.1 numpy==1.20.3 pandas==1.4.1
 pip install seaborn #only needed when call functions in tools.py
 ```
 
 ## Citation
 Ding, W., Goldberg, D. and Zhou, W. (2023), PyComplexHeatmap: A Python package to visualize multimodal genomics data. iMeta e115. https://doi.org/10.1002/imt2.115
+<br>
+**DOI**: 10.1002/imt2.115
 
 ## **Installation**
 ----------------------
 1. **Install using pip**:
 ```shell
 pip install PyComplexHeatmap
```

### Comparing `PyComplexHeatmap-1.5.1/README.md` & `PyComplexHeatmap-1.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 ```
 pip install --ignore-install matplotlib==3.5.1 numpy==1.20.3 pandas==1.4.1
 pip install seaborn #only needed when call functions in tools.py
 ```
 
 ## Citation
 Ding, W., Goldberg, D. and Zhou, W. (2023), PyComplexHeatmap: A Python package to visualize multimodal genomics data. iMeta e115. https://doi.org/10.1002/imt2.115
+<br>
+**DOI**: 10.1002/imt2.115
 
 ## **Installation**
 ----------------------
 1. **Install using pip**:
 ```shell
 pip install PyComplexHeatmap
```

### Comparing `PyComplexHeatmap-1.5.1/pyproject.toml` & `PyComplexHeatmap-1.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0","matplotlib>=3.5.1","numpy>=1.20.3","pandas>=1.4.1", "scipy","fastcluster"]
+requires = ["setuptools>=61.0","matplotlib>=3.5.1","numpy>=1.20.3","pandas>=1.3.5", "scipy","fastcluster"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyComplexHeatmap"
-version = "1.5.1"
+version = "1.5.2"
 authors = [
   { name="Wubin Ding", email="ding.wu.bin.gm@gmail.com" },
 ]
 description = "A python package to plot complex heatmap"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `PyComplexHeatmap-1.5.1/setup.py` & `PyComplexHeatmap-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 # print(long_description)
 
 #release new version
 setup(
    name='PyComplexHeatmap',
-   version='1.5.1',
+   version='1.5.2',
    description='A Python package to plot complex heatmap',
    # long_description="#PyComplexHeatmap\n##Documentation:https://dingwb.github.io/PyComplexHeatmap/build/html/index.html",
    # long_description_content_type='text/markdown',
    author='Wubin Ding',
    author_email='ding.wu.bin.gm@gmail.com',
    url="https://github.com/DingWB/PyComplexHeatmap",
    packages=['PyComplexHeatmap'], #src
```

