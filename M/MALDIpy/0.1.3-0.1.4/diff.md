# Comparing `tmp/MALDIpy-0.1.3.tar.gz` & `tmp/MALDIpy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MALDIpy-0.1.3.tar", last modified: Mon Jun 12 22:20:46 2023, max compression
+gzip compressed data, was "MALDIpy-0.1.4.tar", last modified: Mon Jul 10 22:15:56 2023, max compression
```

## Comparing `MALDIpy-0.1.3.tar` & `MALDIpy-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:20:46.208704 MALDIpy-0.1.3/
--rw-r--r--   0 hli       (1002) labmem    (1001)     1062 2023-04-04 21:12:06.000000 MALDIpy-0.1.3/LICENSE
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:20:46.208704 MALDIpy-0.1.3/MALDIpy/
--rw-r--r--   0 hli       (1002) labmem    (1001)      187 2023-06-12 22:20:25.000000 MALDIpy-0.1.3/MALDIpy/__init__.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     7607 2023-06-12 22:20:09.000000 MALDIpy-0.1.3/MALDIpy/featureplot.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     6599 2023-04-06 16:02:36.000000 MALDIpy-0.1.3/MALDIpy/msi_data.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     3084 2023-04-06 18:34:41.000000 MALDIpy-0.1.3/MALDIpy/multi_sample.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     6619 2023-06-10 01:50:57.000000 MALDIpy-0.1.3/MALDIpy/projection.py
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:20:46.208704 MALDIpy-0.1.3/MALDIpy/shell/
--rw-r--r--   0 hli       (1002) labmem    (1001)       61 2023-04-04 21:15:37.000000 MALDIpy-0.1.3/MALDIpy/shell/__init__.py
--rw-r--r--   0 hli       (1002) labmem    (1001)      196 2023-04-04 21:15:37.000000 MALDIpy-0.1.3/MALDIpy/shell/usage.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     1690 2023-04-06 13:55:22.000000 MALDIpy-0.1.3/MALDIpy/single_cell.py
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:20:46.208704 MALDIpy-0.1.3/MALDIpy/src/
--rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.1.3/MALDIpy/src/temp.txt
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:20:46.208704 MALDIpy-0.1.3/MALDIpy.egg-info/
--rw-r--r--   0 hli       (1002) labmem    (1001)      575 2023-06-12 22:20:46.000000 MALDIpy-0.1.3/MALDIpy.egg-info/PKG-INFO
--rw-r--r--   0 hli       (1002) labmem    (1001)      441 2023-06-12 22:20:46.000000 MALDIpy-0.1.3/MALDIpy.egg-info/SOURCES.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-06-12 22:20:46.000000 MALDIpy-0.1.3/MALDIpy.egg-info/dependency_links.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)       47 2023-06-12 22:20:46.000000 MALDIpy-0.1.3/MALDIpy.egg-info/entry_points.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        8 2023-06-12 22:20:46.000000 MALDIpy-0.1.3/MALDIpy.egg-info/top_level.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-04-04 21:25:43.000000 MALDIpy-0.1.3/MALDIpy.egg-info/zip-safe
--rw-r--r--   0 hli       (1002) labmem    (1001)      176 2023-04-04 21:15:37.000000 MALDIpy-0.1.3/MANIFEST.in
--rw-r--r--   0 hli       (1002) labmem    (1001)      575 2023-06-12 22:20:46.208704 MALDIpy-0.1.3/PKG-INFO
--rw-r--r--   0 hli       (1002) labmem    (1001)      139 2023-06-12 22:20:32.000000 MALDIpy-0.1.3/README.md
--rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.1.3/requirements.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)       38 2023-06-12 22:20:46.208704 MALDIpy-0.1.3/setup.cfg
--rw-r--r--   0 hli       (1002) labmem    (1001)     1922 2023-06-10 02:02:43.000000 MALDIpy-0.1.3/setup.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-07-10 22:15:56.483955 MALDIpy-0.1.4/
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1062 2023-04-04 21:12:06.000000 MALDIpy-0.1.4/LICENSE
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-07-10 22:15:56.471955 MALDIpy-0.1.4/MALDIpy/
+-rw-r--r--   0 hli       (1002) labmem    (1001)      187 2023-07-10 22:08:55.000000 MALDIpy-0.1.4/MALDIpy/__init__.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     7607 2023-06-12 22:20:09.000000 MALDIpy-0.1.4/MALDIpy/featureplot.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     6599 2023-04-06 16:02:36.000000 MALDIpy-0.1.4/MALDIpy/msi_data.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     3084 2023-04-06 18:34:41.000000 MALDIpy-0.1.4/MALDIpy/multi_sample.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     8178 2023-07-10 22:12:08.000000 MALDIpy-0.1.4/MALDIpy/projection.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-07-10 22:15:56.483955 MALDIpy-0.1.4/MALDIpy/shell/
+-rw-r--r--   0 hli       (1002) labmem    (1001)       61 2023-04-04 21:15:37.000000 MALDIpy-0.1.4/MALDIpy/shell/__init__.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)      196 2023-04-04 21:15:37.000000 MALDIpy-0.1.4/MALDIpy/shell/usage.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1690 2023-04-06 13:55:22.000000 MALDIpy-0.1.4/MALDIpy/single_cell.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-07-10 22:15:56.483955 MALDIpy-0.1.4/MALDIpy/src/
+-rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.1.4/MALDIpy/src/temp.txt
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-07-10 22:15:56.483955 MALDIpy-0.1.4/MALDIpy.egg-info/
+-rw-r--r--   0 hli       (1002) labmem    (1001)      855 2023-07-10 22:15:56.000000 MALDIpy-0.1.4/MALDIpy.egg-info/PKG-INFO
+-rw-r--r--   0 hli       (1002) labmem    (1001)      441 2023-07-10 22:15:56.000000 MALDIpy-0.1.4/MALDIpy.egg-info/SOURCES.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-07-10 22:15:56.000000 MALDIpy-0.1.4/MALDIpy.egg-info/dependency_links.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)       47 2023-07-10 22:15:56.000000 MALDIpy-0.1.4/MALDIpy.egg-info/entry_points.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        8 2023-07-10 22:15:56.000000 MALDIpy-0.1.4/MALDIpy.egg-info/top_level.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-04-04 21:25:43.000000 MALDIpy-0.1.4/MALDIpy.egg-info/zip-safe
+-rw-r--r--   0 hli       (1002) labmem    (1001)      176 2023-04-04 21:15:37.000000 MALDIpy-0.1.4/MANIFEST.in
+-rw-r--r--   0 hli       (1002) labmem    (1001)      855 2023-07-10 22:15:56.483955 MALDIpy-0.1.4/PKG-INFO
+-rw-r--r--   0 hli       (1002) labmem    (1001)      328 2023-07-10 22:12:43.000000 MALDIpy-0.1.4/README.md
+-rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.1.4/requirements.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)       38 2023-07-10 22:15:56.483955 MALDIpy-0.1.4/setup.cfg
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1989 2023-07-10 22:14:10.000000 MALDIpy-0.1.4/setup.py
```

### Comparing `MALDIpy-0.1.3/LICENSE` & `MALDIpy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.1.3/MALDIpy/featureplot.py` & `MALDIpy-0.1.4/MALDIpy/featureplot.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.1.3/MALDIpy/msi_data.py` & `MALDIpy-0.1.4/MALDIpy/msi_data.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.1.3/MALDIpy/multi_sample.py` & `MALDIpy-0.1.4/MALDIpy/multi_sample.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.1.3/MALDIpy/projection.py` & `MALDIpy-0.1.4/MALDIpy/projection.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 sc.settings.verbosity = 3
 sc.settings.set_figure_params(dpi=100, facecolor='white',fontsize=12)
 import matplotlib.pyplot as plt
 import seaborn as sns
 from mpl_toolkits.axes_grid1.anchored_artists import AnchoredSizeBar
 import matplotlib.font_manager
 import matplotlib.font_manager as fm
+import anndata
 
 def create_loc(meta_df):
     df = pd.DataFrame(0,index=range(1),columns=range(len(meta_df.iloc[:,5:].columns)))
     df.columns = pd.MultiIndex.from_tuples(meta_df.iloc[:,5:].columns.str.split('_').map(tuple))
     df = df.stack()
     df = df.reset_index()
     df.index = df["level_1"]
@@ -150,8 +151,50 @@
         scalebar1 = AnchoredSizeBar(ax1.transData,30, '300 µm', 'lower right',frameon=False,size_vertical=2,sep=5,
                                    fontproperties=fm.FontProperties(size=10))
         scalebar2 = AnchoredSizeBar(ax2.transData, 30, '300 µm', 'lower right',frameon=False,size_vertical=2,sep=5,
                                    fontproperties=fm.FontProperties(size=10))
         scalebar3 = AnchoredSizeBar(ax3.transData, 30, '300 µm', 'lower right',frameon=False,size_vertical=2,sep=5,
                                    fontproperties=fm.FontProperties(size=10))
         ax1.add_artist(scalebar1);ax2.add_artist(scalebar2);ax3.add_artist(scalebar3)
-    plt.show()
+    plt.show()
+    
+def add_coords(adata):
+    x_coords=[]
+    y_coords=[]
+    for i in adata.obs.index:
+        x1=i.split('_')[0].split('x')[1]
+        y1=i.split('_')[1].split('y')[1]
+        x_coords.append(int(x1))
+        y_coords.append(int(y1))
+    adata.obs['x_coords']=x_coords
+    adata.obs['y_coords']=y_coords
+    return adata
+
+def project_cluster_in_groups(adata, cluster_id, cluster_obs_name, group_list, group_obs_name, cmap='Greys'):
+    
+    print("Cluster: ", cluster_id)
+    fig, axes = plt.subplots(1, len(group_list), figsize = (5*len(group_list),5), dpi = 300)
+    df_dict = {}
+    for g in group_list:
+        sub_ad = adata[(adata.obs[group_obs_name] == g) & (adata.obs[cluster_obs_name] == str(cluster_id))]
+        loc_df = sub_ad.obs[["x_coords","y_coords"]].copy()
+        M = loc_df["y_coords"].max() + 1
+        N = loc_df["x_coords"].max() + 1
+        loc_df["values"] = 1
+        loc_df.set_index(["y_coords", "x_coords"], inplace=True)
+        index = pd.MultiIndex.from_product([range(M), range(N)], names=['y_coords', 'x_coords'])
+        df_zero = loc_df.reindex(index, fill_value=-1)['values'].unstack()
+        df_zero.rename_axis(index=None, columns=None, inplace=True)
+        df_dict[g] = df_zero
+    
+    axes = axes.flatten()
+    
+    for idx, g in enumerate(group):
+        plt_df = df_dict[g]
+        sns.heatmap(plt_df, cmap=cmap, ax=axes[idx], cbar=False)
+        axes[idx].set_xticks([])
+        axes[idx].set_yticks([])
+        axes[idx].set_facecolor("white")
+    
+    plt.tight_layout()
+    
+    return fig
```

### Comparing `MALDIpy-0.1.3/MALDIpy/single_cell.py` & `MALDIpy-0.1.4/MALDIpy/single_cell.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.1.3/setup.py` & `MALDIpy-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 NAME = "MALDIpy"
-AUTHOR = "Haikuo Li; Dian Li; Qiao Xuanyuan; Benjamin Humphreys"
+AUTHOR = "Haikuo Li; Qiao Xuanyuan; Dian Li; Benjamin Humphreys"
 EMAIL = "haikuolibio@gmail.com"
 URL = "https://github.com/TheHumphreysLab"
 #LICENSE = "your license"
-DESCRIPTION = "MALDI-MS data analysis at the single-cell level"
+DESCRIPTION = "MALDI-MS data analysis at the single-cell level (Tutorials available at https://github.com/TheHumphreysLab/MALDIpy"
 
 if sys.version_info < (3, 6, 0):
     raise RuntimeError(f"{NAME} requires Python >=3.6.0, but yours is {sys.version}!")
 
 try:
     lib_py = os.path.join(NAME, "__init__.py")
     with open(lib_py, "r", encoding="utf8") as f_v:
```

