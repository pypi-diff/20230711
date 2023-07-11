# Comparing `tmp/mlbi_at_dku_lib-0.2.2.tar.gz` & `tmp/mlbi_at_dku_lib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.2.2.tar", last modified: Sun Jul  2 07:03:14 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.2.3.tar", last modified: Tue Jul 11 08:05:18 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.2.2.tar` & `mlbi_at_dku_lib-0.2.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-02 07:03:14.537073 mlbi_at_dku_lib-0.2.2/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.2/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      102 2023-07-02 06:59:42.000000 mlbi_at_dku_lib-0.2.2/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-02 07:03:14.533073 mlbi_at_dku_lib-0.2.2/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.2/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      827 2023-07-02 07:02:55.000000 mlbi_at_dku_lib-0.2.2/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-02 07:03:14.537073 mlbi_at_dku_lib-0.2.2/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-02 05:17:52.000000 mlbi_at_dku_lib-0.2.2/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-02 07:03:14.473074 mlbi_at_dku_lib-0.2.2/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-02 07:03:14.473074 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-02 07:03:14.521073 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/data/
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/data/GTmap_hg19.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/data/GTmap_hg38.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/data/GTmap_mm10.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     6012 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    36548 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37762 2023-07-02 06:36:14.000000 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-02 07:03:14.473074 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-02 07:03:14.000000 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      606 2023-07-02 07:03:14.000000 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-02 07:03:14.000000 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-02 07:03:14.000000 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-02 07:03:14.000000 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       16 2023-07-02 07:03:14.000000 mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 08:05:18.921107 mlbi_at_dku_lib-0.2.3/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.3/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      102 2023-07-02 06:59:42.000000 mlbi_at_dku_lib-0.2.3/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-11 08:05:18.921107 mlbi_at_dku_lib-0.2.3/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.3/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      827 2023-07-11 08:03:41.000000 mlbi_at_dku_lib-0.2.3/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-11 08:05:18.921107 mlbi_at_dku_lib-0.2.3/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-02 05:17:52.000000 mlbi_at_dku_lib-0.2.3/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 08:05:18.605115 mlbi_at_dku_lib-0.2.3/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 08:05:18.637114 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 08:05:18.861108 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/data/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/data/GTmap_hg19.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/data/GTmap_hg38.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/data/GTmap_mm10.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     5206 2023-07-11 04:59:49.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     6033 2023-07-11 04:52:53.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    36548 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    40645 2023-07-11 04:48:23.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 08:05:18.637114 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-11 08:05:18.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      633 2023-07-11 08:05:18.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-11 08:05:18.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-11 08:05:18.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-11 08:05:18.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       16 2023-07-11 08:05:18.000000 mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib.egg-info/top_level.txt
```

### Comparing `mlbi_at_dku_lib-0.2.2/LICENSE` & `mlbi_at_dku_lib-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.2/PKG-INFO` & `mlbi_at_dku_lib-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi_at_dku_lib
-Version: 0.2.2
+Version: 0.2.3
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `mlbi_at_dku_lib-0.2.2/pyproject.toml` & `mlbi_at_dku_lib-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlbi_at_dku_lib"
-version = "0.2.2"
+version = "0.2.3"
 description = "Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/cpdb.py` & `mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/cpdb.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/data/GTmap_hg19.csv` & `mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/data/GTmap_hg19.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/data/GTmap_hg38.csv` & `mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/data/GTmap_hg38.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/data/GTmap_mm10.csv` & `mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/data/GTmap_mm10.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/deiso.py` & `mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/deiso.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,17 +181,16 @@
                 b = df_res_all[key]['pval'] <= pv_cutoff
                 df_res_all[key].loc[b,:].to_excel(writer, sheet_name = key)
         cnt += 1
 
     return
 
 
-def load_excel(file):
+def load_excel(file, index_col = 0):
     
     xls = pd.ExcelFile(file)
     lst = xls.sheet_names
     df_res_all = {}
     for s in lst:
-        df_res_all[s] = pd.read_excel(xls, s, index_col = 0) 
+        df_res_all[s] = pd.read_excel(xls, s, index_col = index_col) 
         
-    return df_res_all
-
+    return df_res_all
```

### Comparing `mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/icnv.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,22 +182,27 @@
     
     if len(sort_by) > 0:
         df_celltype_pct.sort_values(by = sort_by, inplace = True)
 
     return df_celltype_cnt, df_celltype_pct
 
 
-def plot_population(df_celltype_pct, title = None, title_fs = 12, 
+def plot_population(df_pct, title = None, title_fs = 12, 
                     label_fs = 11, tick_fs = 10, tick_rot = 45,
                     legend_fs = 10, legend_loc = 'upper left', bbox_to_anchor = (1,1), 
-                    figsize=(5, 3), return_fig = False):    
+                    legend_ncol = 1, cmap_name = None, figsize=(5, 3), return_fig = False):    
 
-    ax = df_celltype_pct.plot.bar(stacked = True, rot = tick_rot, figsize = figsize)
-    ax.legend( df_celltype_pct.columns.values, bbox_to_anchor=bbox_to_anchor, 
-               loc = legend_loc, fontsize = legend_fs )
+    if cmap_name is None:
+        cmap_name = 'Spectral'
+    cmap = plt.get_cmap(cmap_name)
+    color = cmap(np.arange(df_pct.shape[1])/df_pct.shape[1])
+    
+    ax = df_pct.plot.bar(stacked = True, rot = tick_rot, figsize = figsize, color = color)
+    ax.legend( list(df_pct.columns.values), bbox_to_anchor=bbox_to_anchor, 
+               loc = legend_loc, fontsize = legend_fs, ncol = legend_ncol )
     plt.xticks(fontsize=tick_fs)
     plt.yticks(fontsize=tick_fs)
     plt.ylabel('Percentage [%]', fontsize = label_fs)
     plt.title(title, fontsize = title_fs)
     if return_fig:
         return ax
     else:
@@ -205,15 +210,20 @@
         return
     return
 
 
 def plot_population_g(df_pct, sg_map, sort_by = [], title = None, title_y = 1.05, title_fs = 14, 
                     title_fs2 = 12, label_fs = 11, tick_fs = 10, tick_rot = 45,
                     legend_fs = 10, legend_loc = 'upper left', bbox_to_anchor = (1,1), 
-                    figsize=(5, 3), return_fig = False):    
+                    legend_ncol = 1, cmap_name = None, figsize=(5, 3), return_fig = False):    
+
+    if cmap_name is None:
+        cmap_name = 'Spectral'
+    cmap = plt.get_cmap(cmap_name)
+    color = cmap(np.arange(df_pct.shape[1])/df_pct.shape[1])
     
     df = df_pct.copy(deep = True)
 
     items = list(df.columns.values)
 
     df['Group'] = list(df.index.values)
     df['Group'].replace(sg_map, inplace = True)
@@ -238,34 +248,39 @@
     cnt = 0
     for j, g in enumerate(glst):
         b = df['Group'] == g
         dft = df.loc[b,:]
         if len(sort_by) > 0:
             dft = dft.sort_values(sort_by)
         ax = dft.plot.bar(width = 0.75, stacked = True, ax = axes[j+cnt], 
-                          figsize = figsize, legend = None)
+                          figsize = figsize, legend = None, color = color)
         ax.set_title('%s' % (g), fontsize = title_fs2)
-        if j == 2: 
-            plt.legend(loc = 'upper left', bbox_to_anchor = (1,1), fontsize = legend_fs)  
-        else:
-            pass
         if j != 0:
             ax.set_yticks([])
         else:
             ax.set_ylabel('Proportion', fontsize = label_fs)
 
         ax.tick_params(axis='x', labelsize=tick_fs, rotation = tick_rot)
         ax.tick_params(axis='y', labelsize=tick_fs)
             
+        if g == glst[-1]: 
+            ax.legend(dft.columns.values, loc = legend_loc, bbox_to_anchor = bbox_to_anchor, 
+                       fontsize = legend_fs, ncol = legend_ncol)  
+        else:
+            pass
     plt.show()
     
     return
 
 
 def get_sample_to_group_dict( samples, conditions ):
+    
+    samples = np.array(samples)
+    conditions = np.array(conditions)
+    
     slst = list(set(list(samples)))
     slst.sort()
     glst = []
     for s in slst:
         b = samples == s
         g = conditions[b][0]
         glst.append(g)
@@ -273,14 +288,73 @@
     dct = dict(zip(slst, glst))
     return dct
 
 
 def plot_pct_box(df_pct, sg_map, nr_nc, figsize = None, dpi = 100,
                  title = None, title_y = 1.05, title_fs = 14, 
                  title_fs2 = 12, label_fs = 11, tick_fs = 10, tick_rot = 0, 
+                 annot_ref = None, annot_fmt = 'simple', annot_fs = 10, 
+                 ws_hs = (0.3, 0.3)):
+    
+    df = df_pct.copy(deep = True)
+    nr, nc = nr_nc
+    ws, hs = ws_hs
+    fig, axes = plt.subplots(figsize=figsize, dpi=dpi, nrows=nr, ncols=nc, constrained_layout=True)
+    fig.tight_layout() # Or equivalently,  "plt.tight_layout()"
+    if title is not None:
+        fig.suptitle('%s' % title, x = 0.5, y = title_y, fontsize = title_fs, ha = 'center')
+    plt.subplots_adjust(left=None, bottom=None, right=None, top=None, wspace=ws, hspace=hs)
+
+    items = list(df.columns.values)
+
+    df['Group'] = list(df.index.values)
+    df['Group'].replace(sg_map, inplace = True)
+
+    lst = df['Group'].unique()
+    lst_pair = []
+    if annot_ref in lst:
+        for k, l1 in enumerate(lst):
+            if l1 != annot_ref:
+                lst_pair.append((annot_ref, l1))
+    else:
+        for k, l1 in enumerate(lst):
+            for j, l2 in enumerate(lst):
+                if j >  k:
+                    lst_pair.append((l1, l2))
+
+    for k, item in enumerate(items):
+        plt.subplot(nr,nc,k+1)
+        ax = sns.boxplot(data = df, x = 'Group', y = item) #, order=['HC', 'CC', 'AC'])
+        if k%nc == 0: plt.ylabel('Percentage', fontsize = label_fs)
+        else: plt.ylabel(None)
+        if k >= nc*(nr-1): plt.xlabel('Condition', fontsize = label_fs)
+        else: plt.xlabel(None)
+        plt.title(item, fontsize = title_fs2)
+        if k < (nr*nc - nc):
+            plt.xticks([])
+            plt.yticks(fontsize = tick_fs)
+        else:
+            plt.xticks(rotation = tick_rot, ha = 'center', fontsize = tick_fs)
+            plt.yticks(fontsize = tick_fs)
+        
+        add_stat_annotation(ax, data=df, x = 'Group', y = item, 
+                        box_pairs=lst_pair, loc='inside', fontsize = annot_fs,
+                        test='t-test_ind', text_format=annot_fmt, verbose=0)
+        #'''
+    if (len(items) < (nr*nc)) & (nr > 1):
+        for k in range(nr*nc - len(items)):
+            axes[nr-1][len(items)%nc + k].axis("off")
+        
+    plt.show()
+    return 
+
+
+def plot_pct_box_old(df_pct, sg_map, nr_nc, figsize = None, dpi = 100,
+                 title = None, title_y = 1.05, title_fs = 14, 
+                 title_fs2 = 12, label_fs = 11, tick_fs = 10, tick_rot = 0, 
                  annot_fs = 10, ws_hs = (0.3, 0.3)):
     
     df = df_pct.copy(deep = True)
     nr, nc = nr_nc
     ws, hs = ws_hs
     fig, axes = plt.subplots(figsize=figsize, dpi=dpi, nrows=nr, ncols=nc, constrained_layout=True)
     fig.tight_layout() # Or equivalently,  "plt.tight_layout()"
```

### Comparing `mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib.egg-info/PKG-INFO` & `mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi-at-dku-lib
-Version: 0.2.2
+Version: 0.2.3
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `mlbi_at_dku_lib-0.2.2/src/mlbi_at_dku_lib.egg-info/SOURCES.txt` & `mlbi_at_dku_lib-0.2.3/src/mlbi_at_dku_lib.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/mlbi_at_dku_lib/__init__.py
 src/mlbi_at_dku_lib/cpdb.py
+src/mlbi_at_dku_lib/deg.py
 src/mlbi_at_dku_lib/deiso.py
 src/mlbi_at_dku_lib/gsea.py
 src/mlbi_at_dku_lib/icnv.py
 src/mlbi_at_dku_lib/misc.py
 src/mlbi_at_dku_lib.egg-info/PKG-INFO
 src/mlbi_at_dku_lib.egg-info/SOURCES.txt
 src/mlbi_at_dku_lib.egg-info/dependency_links.txt
```

