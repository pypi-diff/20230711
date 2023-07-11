# Comparing `tmp/mlbi_at_dku_lib-0.2.5.tar.gz` & `tmp/mlbi_at_dku_lib-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.2.5.tar", last modified: Tue Jul 11 10:40:10 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.2.6.tar", last modified: Tue Jul 11 14:22:57 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.2.5.tar` & `mlbi_at_dku_lib-0.2.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 10:40:10.772814 mlbi_at_dku_lib-0.2.5/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.5/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      102 2023-07-02 06:59:42.000000 mlbi_at_dku_lib-0.2.5/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-11 10:40:10.772814 mlbi_at_dku_lib-0.2.5/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.5/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      827 2023-07-11 10:39:56.000000 mlbi_at_dku_lib-0.2.5/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-11 10:40:10.772814 mlbi_at_dku_lib-0.2.5/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-02 05:17:52.000000 mlbi_at_dku_lib-0.2.5/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 10:40:10.708816 mlbi_at_dku_lib-0.2.5/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 10:40:10.712816 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 10:40:10.760815 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/data/
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/data/GTmap_hg19.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/data/GTmap_hg38.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/data/GTmap_mm10.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     5206 2023-07-11 04:59:49.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     6033 2023-07-11 04:52:53.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    36550 2023-07-11 10:36:34.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    40645 2023-07-11 04:48:23.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 10:40:10.712816 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-11 10:40:10.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      633 2023-07-11 10:40:10.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-11 10:40:10.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-11 10:40:10.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-11 10:40:10.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       16 2023-07-11 10:40:10.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 14:22:57.203400 mlbi_at_dku_lib-0.2.6/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.6/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      102 2023-07-02 06:59:42.000000 mlbi_at_dku_lib-0.2.6/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-11 14:22:57.203400 mlbi_at_dku_lib-0.2.6/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.6/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      827 2023-07-11 14:21:48.000000 mlbi_at_dku_lib-0.2.6/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-11 14:22:57.203400 mlbi_at_dku_lib-0.2.6/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-02 05:17:52.000000 mlbi_at_dku_lib-0.2.6/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 14:22:57.139402 mlbi_at_dku_lib-0.2.6/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 14:22:57.139402 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 14:22:57.187401 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/data/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/data/GTmap_hg19.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/data/GTmap_hg38.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/data/GTmap_mm10.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    14644 2023-07-11 14:20:18.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     6033 2023-07-11 04:52:53.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    36550 2023-07-11 10:36:34.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    30776 2023-07-11 14:11:49.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 14:22:57.139402 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-11 14:22:57.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      633 2023-07-11 14:22:57.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-11 14:22:57.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-11 14:22:57.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-11 14:22:57.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       16 2023-07-11 14:22:57.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/top_level.txt
```

### Comparing `mlbi_at_dku_lib-0.2.5/LICENSE` & `mlbi_at_dku_lib-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.5/PKG-INFO` & `mlbi_at_dku_lib-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi_at_dku_lib
-Version: 0.2.5
+Version: 0.2.6
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `mlbi_at_dku_lib-0.2.5/pyproject.toml` & `mlbi_at_dku_lib-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlbi_at_dku_lib"
-version = "0.2.5"
+version = "0.2.6"
 description = "Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/cpdb.py` & `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/cpdb.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/data/GTmap_hg19.csv` & `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/data/GTmap_hg19.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/data/GTmap_hg38.csv` & `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/data/GTmap_hg38.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/data/GTmap_mm10.csv` & `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/data/GTmap_mm10.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/deg.py` & `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/deiso.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,156 +1,196 @@
 import time, os, sys, warnings
 import numpy as np
 import pandas as pd
 from scipy import stats
 
-MIN_VALUE = 1e-10
-MIN_VALUE_EF = 1e-10
+SKLEARN = True
+try:
+    from sklearn.decomposition import PCA
+except ImportError:
+    SKLEARN = False
+    print('DEiso ERROR: scikit-learn not installed.')
+
+    
+def DEiso_pca( dfs, n_comp = 2 ):
+
+    rownames = ['PC%i' % (i+1) for i in range(int(n_comp))]
+    pca_obj = PCA(n_components=int(n_comp))
+    X_pca = pca_obj.fit_transform(dfs.transpose()).transpose()  
+    df_pca = pd.DataFrame(X_pca, index = rownames, columns = dfs.columns.values)
+    return df_pca
+
+
+def get_mean_and_cov(dfx):
+    m = dfx.mean(axis = 1)
+    dfy = dfx.sub(m, axis = 0)
+    C = dfy.dot(dfy.transpose())/(dfy.shape[1]-1)    
+    return m, C 
+
+
+def DEiso_anal_per_gene( dfs_in, groups, gr, norm = False, log = False,
+                         n_pca_comp = 0, cn_th = 1e-10, ro = 0.1, nth = 0.8 ):
+    
+    dfs = dfs_in.copy(deep = True)
+    if norm:
+        dfs = dfs.div(dfs.sum(axis = 0), axis = 1)*100
+        if log:
+            dfs = np.log2(dfs + 1)
+            
+    if n_pca_comp > 0:
+        dfs = DEiso_pca( dfs, n_comp = min(n_pca_comp, dfs.shape[0]) )
+    
+    samples = np.array(list(dfs.columns.values))
+    glst = list(groups)
+    glst = list(set(glst))
+    glst.sort()
+    if gr in glst:
+        glst.remove(gr)
 
-def perform_deg( df_cbyg_in, groups, target_group, min_ef = 0.05, exp_only = False ):
-    
-    # b = groups == ref_group
-    b = groups != target_group
-    
-    b1 = (df_cbyg_in.loc[~b,:] > 0).mean(axis = 0) >= min_ef 
-    b2 = (df_cbyg_in.loc[b,:] > 0).mean(axis = 0) >= min_ef 
-    bx = b1 | b2
-    df_cbyg = (df_cbyg_in).loc[:,bx]
-    
-    g_mec_ref = (df_cbyg.loc[b,:] > 0).mean(axis = 0)
-    g_mec_test = (df_cbyg.loc[~b,:] > 0).mean(axis = 0)
+    cov = {}
+    mns = {}
     
-    eft = (g_mec_test)
-    efr = (g_mec_ref)
-    efc = (eft + MIN_VALUE_EF)/(efr + MIN_VALUE_EF)
+    b = np.array(groups) == gr
+    ssel = list(samples[b])
     
-    df = pd.DataFrame(index = df_cbyg.columns)
-    
-    df['EFC'] = list(efc)
-    df['log10_EFC'] = list(np.round(np.log10(efc), 3))
-    df['EF_test'] = list(eft)
-    df['EF_ref'] = list(efr)
-    # df['Score'] = df['log10_EFC']*(np.sum(~b)*eft + np.sum(b)*efr)
-        
-    #'''
-    g_mean_ref = df_cbyg.loc[b,:].mean(axis = 0)
-    g_mean_test = df_cbyg.loc[~b,:].mean(axis = 0)
-    g_std_ref = df_cbyg.loc[b,:].std(axis = 0)
-    g_std_test = df_cbyg.loc[~b,:].std(axis = 0)
-
-    if exp_only: 
-        g_mean_ref = g_mean_ref/(efr + MIN_VALUE)
-        g_mean_test = g_mean_test/(eft + MIN_VALUE)
-        g_std_ref = g_std_ref/np.sqrt(efr + MIN_VALUE)
-        g_std_test = g_std_test/np.sqrt(eft + MIN_VALUE)
-    
-    # fc = (g_mean_test + MIN_VALUE)/(g_mean_ref + MIN_VALUE)
-    fc = (np.expm1(g_mean_test) + MIN_VALUE)/(np.expm1(g_mean_ref) + MIN_VALUE)
-    stat = np.abs(g_mean_test - g_mean_ref)
-    
-    if exp_only: 
-        stat = stat/((g_std_ref/np.sqrt(np.sum(b)*efr + MIN_VALUE)) \
-                    + g_std_test/np.sqrt(np.sum(~b)*eft + MIN_VALUE))
-    else:
-        stat = stat/(g_std_ref/np.sqrt(np.sum(b) + MIN_VALUE) \
-                   + g_std_test/np.sqrt(np.sum(~b) + MIN_VALUE))
-        
-    df['mean_test'] = list(g_mean_test)
-    df['mean_ref'] = list(g_mean_ref)
-    df['log2_FC'] = list(np.round(np.log2(fc), 3))
-    
-    if exp_only:
-        pv = stats.t.sf(stat*np.sqrt(2), df = (np.sum(b)*efr + np.sum(~b)*eft)-2)*2
-    else:
-        pv = stats.t.sf(stat*np.sqrt(2), df = (np.sum(b)*efr + np.sum(~b)*eft)-2)*2
-        # pv = stats.t.sf(stat, df = np.sum(b)-2)*2
-    pv = pv 
+    bt = ((dfs[ssel] > 0).sum(axis = 0) > 0)
+    if bt.sum() < dfs[ssel].shape[1]*nth:
+        return None
+
+    # Cr = np.array( dfs[ssel].transpose().cov() )
+    # mr = np.array( dfs[ssel].mean(axis = 1) )
+    mr, Cr = get_mean_and_cov(dfs[ssel])
+    
+    res = {}
+    for i, g in enumerate(glst):
+        b = np.array(groups) == g
+        ssel = list(samples[b])
         
-    pv_adj = pv * df_cbyg.shape[1]
-    df['pval'] = list(pv)
-    df['pval_adj'] = list(pv_adj)
-    df['pval_adj'].clip(upper = 1, inplace = True)
-    #'''
-    df = df.sort_values(by = 'EFC', ascending = False)
+        bt = ((dfs[ssel] > 0).sum(axis = 0) > 0)
+        if bt.sum() >= dfs[ssel].shape[1]*nth:
         
-    return df
-
-
-def deg_multi( df_cbyg_in, groups_in, ref_group = None, samples_in = None,
-               min_ef = 0.05, exp_only = False, min_frac = 0.1 ):
-
-    glst = list(set(list(groups_in)))
-    glst.sort()
-    
-    if not isinstance(groups_in, pd.Series):
-        groups_in = pd.Series(groups_in, index = df_cbyg_in.index.values)
-
-    df_lst = {}
-    for g in glst:
-
-        if (ref_group is None):
-            groups = groups_in.copy(deep = True).astype(str)
-            ref_g = 'others'
-            b = groups != g
-            groups[b] = ref_group
-            df_cbyg = df_cbyg_in
-        else:
-            if ref_group == g:
-                groups = groups_in.copy(deep = True).astype(str)
-                ref_g = 'others'
-                b = groups != g
-                groups[b] = ref_g
-                df_cbyg = df_cbyg_in
+            # Ct = np.array( dfs[ssel].transpose().cov() )
+            # mt = np.array( dfs[ssel].mean(axis = 1) )
+            mt, Ct = get_mean_and_cov(dfs[ssel])
+            
+            m = mt - mr    
+
+            C = Cr + Ct
+            C = C + (np.diag(C).mean()*ro)*np.eye(C.shape[0])
+            if np.linalg.det(C) < cn_th:
+                c1 = 0
             else:
-                ref_g = ref_group
-                b = groups_in.isin([g, ref_group])
-                groups = groups_in[b]
-                df_cbyg = df_cbyg_in.loc[b,:]
-
-        df_deg = perform_deg( df_cbyg, groups, target_group = g, 
-                              min_ef = min_ef, exp_only = exp_only )
-        key = '%s_vs_%s' % (g, ref_g)
-        df_lst[key] = df_deg
-
-        if samples_in is not None:
-            if len(samples_in) == df_cbyg_in.shape[0]:
-                b = groups_in == g
-                dft = find_fraction_of_patients_for_vaild_marker_exp( df_lst[key], 
-                            df_cbyg_in.loc[b,:], pids = samples_in[b], min_frac = min_frac )
-                df_lst[key]['Rp'] = dft['Rp'] 
-        
-    return df_lst
+                C = np.linalg.inv(C)
+                c1 = m.dot(C.dot(m))
+                c1 = np.sqrt(c1)
 
+                p1 = stats.t.sf(c1, df = dfs.shape[1])*2
+                res['%s_vs_%s' % (g, gr)] = (c1, p1)
 
-def find_fraction_of_patients_for_vaild_marker_exp( df_deg, df_cbyg, pids, min_frac = 0.1 ):
+    return res    
     
-    dft = pd.DataFrame(index = df_deg.index) 
-    dft['Rp'] = 0
-    X = df_cbyg
 
-    glst = list(dft.index.values)
-    plst= list(set(list(pids)))
+def DEiso_anal( df, gene_names, groups, ref_group, norm = True, log = False, 
+                n_pca_comp = 0, rho = 0.1, nth = 0.8, verbose = True ):
     
-    for p in plst:
-        bp = pids == p
-        exp_frac = (X.loc[bp, glst] > 0).mean(axis = 0)
-
-        dft['Rp'] += list(exp_frac >= min_frac)
-
-    dft['Rp'] = np.round(dft['Rp']/len(plst), 3)
+    if not SKLEARN:
+        print('DEiso ERROR: scikit-learn not installed.', flush=True)
+        return None
     
-    return dft
-
-def get_fraction_of_samples_for_vaild_marker( df_lst, df_cbyg, groups, samples, min_frac = 0.1 ):
-
-    for key in df_lst.keys():
-
-        subtype = key.split('_')[0]
-        b = groups == subtype
-
-        ## For each markers, get percentage of patient who has the marker expressed 
-        dft = find_fraction_of_patients_for_vaild_marker_exp( df_lst[key], df_cbyg.loc[b,:], 
-                                                              pids = samples[b], min_frac = min_frac )
-        ## fraction of patient who has the corresponding marker expressed
-        df_lst[key]['Rp'] = dft['Rp'] 
+    gr = ref_group
+    glst = list(set(gene_names))
+    glst.sort()
+    idxs = {}
+    for g in glst:
+        idxs[g] = []
 
-    return df_lst
+    ilst = list(df.index.values)
+    nlst = list(gene_names)
+    for g, t in zip(nlst, ilst):
+        idxs[g].append(t)
+
+    start = time.time()
+
+    df_res = None
+    cnt = 0
+    for k, g in enumerate(glst):
+        idx = idxs[g]
+        if len(idx) >= 2:
+            dfs = df.loc[idx,:]
+            
+            bt = ((dfs > 0).sum(axis = 0) > 1)
+            if bt.sum() >= dfs.shape[1]: 
+                
+                # v = None
+                v = DEiso_anal_per_gene( dfs, groups, gr, norm = norm, log = log,
+                                        n_pca_comp = n_pca_comp, ro = rho, nth = nth )
+                if v is not None:
+                    if isinstance(v, dict):
+                        keys = v.keys()
+                        if cnt == 0:
+                            df_res = {}
+                            for key in keys:
+                                df_res[key] = pd.DataFrame(columns = ['stat', 'pval'])
+
+                        for key in keys:
+                            if key in list(df_res.keys()):
+                                df_res[key].loc[g, :] = list(v[key])
+                            else:
+                                df_res[key] = pd.DataFrame(columns = ['stat', 'pval'])
+
+                    else:
+                        if cnt == 0:
+                            df_res = pd.DataFrame(columns = ['stat', 'pval'])
+                        df_res.loc[g, :] = list(v)
+
+                    cnt += 1
+
+        if verbose: 
+            if k%100 == 0: 
+                print('DEiso Progress: %i/%i(%i)   ' % (k, len(glst), cnt), end = '\r', flush=True)
+
+    elapsed = time.time() - start
+    if verbose: print('DEiso done (%i) .. %i               ' % (elapsed, cnt), flush=True)
+
+    if df_res is not None:
+        if isinstance(df_res, dict):
+            for key in df_res.keys():
+                df_res[key]['pval_adj'] = df_res[key]['pval']*cnt
+                b = df_res[key]['pval_adj'] > 1
+                df_res[key].loc[b, 'pval_adj'] = 1
+                df_res[key] = df_res[key].sort_values(['stat'], ascending = False)
+        else:
+            df_res['pval_adj'] = df_res['pval']*cnt
+            b = df_res['pval_adj'] > 1
+            df_res.loc[b, 'pval_adj'] = 1
+            df_res = df_res.sort_values(['stat'], ascending = False)
+       
+    return df_res
+
+
+def save_to_excel(df_res_all, file_out, pv_cutoff = 0.1):
+
+    cnt = 0
+    for key in df_res_all.keys():
+
+        if cnt == 0: 
+            with pd.ExcelWriter(file_out, mode='w') as writer:
+                b = df_res_all[key]['pval'] <= pv_cutoff
+                df_res_all[key].loc[b,:].to_excel(writer, sheet_name = key)
+        else: 
+            with pd.ExcelWriter(file_out, mode='a', if_sheet_exists = 'replace') as writer:
+                b = df_res_all[key]['pval'] <= pv_cutoff
+                df_res_all[key].loc[b,:].to_excel(writer, sheet_name = key)
+        cnt += 1
+
+    return
+
+
+def load_excel(file, index_col = 0):
+    
+    xls = pd.ExcelFile(file)
+    lst = xls.sheet_names
+    df_res_all = {}
+    for s in lst:
+        df_res_all[s] = pd.read_excel(xls, s, index_col = index_col) 
+        
+    return df_res_all
```

### Comparing `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/icnv.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/misc.py`

 * *Files 18% similar despite different names*

```diff
@@ -150,291 +150,14 @@
                 # 'font': 12,
                 'xanchor': 'center',
                 'yanchor': 'top'})    
     fig.show()   
     return
 
 
-### Example 
-# df_cnt, df_pct= get_population( adata_s.obs['sid'], 
-#                                 adata_s.obs['minor'], sort_by = [] )
-# plot_population(df_pct, figsize=(6, 4), dpi = 80, return_fig = False)
-# df_cnt
-    
-def get_population( pids, cts, sort_by = [] ):
-    
-    pid_lst = list(set(list(pids)))
-    pid_lst.sort()
-    celltype_lst = list(set(list(cts)))
-    celltype_lst.sort()
-
-    df_celltype_cnt = pd.DataFrame(index = pid_lst, columns = celltype_lst)
-    df_celltype_cnt.loc[:,:] = 0
-
-    for pid in pid_lst:
-        b = np.array(pids) == pid
-        ct_sel = np.array(cts)[b]
-
-        for ct in celltype_lst:
-            bx = ct_sel == ct
-            df_celltype_cnt.loc[pid, ct] = np.sum(bx)
-
-    df_celltype_pct = (df_celltype_cnt.div(df_celltype_cnt.sum(axis = 1), axis = 0)*100).astype(float)
-    
-    if len(sort_by) > 0:
-        df_celltype_pct.sort_values(by = sort_by, inplace = True)
-
-    return df_celltype_cnt, df_celltype_pct
-
-
-def plot_population(df_pct, title = None, title_fs = 12, 
-                    label_fs = 11, tick_fs = 10, tick_rot = 45,
-                    legend_fs = 10, legend_loc = 'upper left', bbox_to_anchor = (1,1), 
-                    legend_ncol = 1, cmap_name = None, figsize=(5, 3), return_fig = False):    
-
-    if cmap_name is None:
-        cmap_name = 'Spectral'
-    cmap = plt.get_cmap(cmap_name)
-    color = cmap(np.arange(df_pct.shape[1])/df_pct.shape[1])
-    
-    ax = df_pct.plot.bar(stacked = True, rot = tick_rot, figsize = figsize, color = color)
-    ax.legend( list(df_pct.columns.values), bbox_to_anchor=bbox_to_anchor, 
-               loc = legend_loc, fontsize = legend_fs, ncol = legend_ncol )
-    plt.xticks(fontsize=tick_fs)
-    plt.yticks(fontsize=tick_fs)
-    plt.ylabel('Percentage [%]', fontsize = label_fs)
-    plt.title(title, fontsize = title_fs)
-    if return_fig:
-        return ax
-    else:
-        plt.show()
-        return
-    return
-
-
-def plot_population_g(df_pct, sg_map, sort_by = [], title = None, title_y = 1.05, title_fs = 14, 
-                    title_fs2 = 12, label_fs = 11, tick_fs = 10, tick_rot = 45,
-                    legend_fs = 10, legend_loc = 'upper left', bbox_to_anchor = (1,1), 
-                    legend_ncol = 1, cmap_name = None, figsize=(5, 3), return_fig = False):    
-
-    if cmap_name is None:
-        cmap_name = 'Spectral'
-    cmap = plt.get_cmap(cmap_name)
-    color = cmap(np.arange(df_pct.shape[1])/df_pct.shape[1])
-    
-    df = df_pct.copy(deep = True)
-
-    items = list(df.columns.values)
-
-    df['Group'] = list(df.index.values)
-    df['Group'].replace(sg_map, inplace = True)
-
-    num_p = []
-
-    glst = list(df['Group'].unique())
-    glst.sort()
-
-    cnt = df['Group'].value_counts()
-    for g in glst:
-        num_p.append(cnt.loc[g])
-
-    nr, nc = 1, len(glst)
-    fig, axes = plt.subplots(nrows=nr, ncols=nc, constrained_layout=True, 
-                             gridspec_kw={'width_ratios': num_p})
-    fig.tight_layout() 
-    if title is not None: 
-        fig.suptitle(title, x = 0.5, y = title_y, fontsize = title_fs, ha = 'center')
-    plt.subplots_adjust(left=None, bottom=None, right=None, top=None, wspace=0.06, hspace=0.25)
-
-    cnt = 0
-    for j, g in enumerate(glst):
-        b = df['Group'] == g
-        dft = df.loc[b,:]
-        if len(sort_by) > 0:
-            dft = dft.sort_values(sort_by)
-        ax = dft.plot.bar(width = 0.75, stacked = True, ax = axes[j+cnt], 
-                          figsize = figsize, legend = None, color = color)
-        ax.set_title('%s' % (g), fontsize = title_fs2)
-        if j != 0:
-            ax.set_yticks([])
-        else:
-            ax.set_ylabel('Proportion', fontsize = label_fs)
-
-        ax.tick_params(axis='x', labelsize=tick_fs, rotation = tick_rot)
-        ax.tick_params(axis='y', labelsize=tick_fs)
-            
-        if g == glst[-1]: 
-            ax.legend(dft.columns.values, loc = legend_loc, bbox_to_anchor = bbox_to_anchor, 
-                       fontsize = legend_fs, ncol = legend_ncol)  
-        else:
-            pass
-    plt.show()
-    
-    return
-
-
-def get_sample_to_group_dict( samples, conditions ):
-    
-    samples = np.array(samples)
-    conditions = np.array(conditions)
-    
-    slst = list(set(list(samples)))
-    slst.sort()
-    glst = []
-    for s in slst:
-        b = samples == s
-        g = conditions[b][0]
-        glst.append(g)
-        
-    dct = dict(zip(slst, glst))
-    return dct
-
-
-def plot_pct_box(df_pct, sg_map, nr_nc, figsize = None, dpi = 100,
-                 title = None, title_y = 1.05, title_fs = 14, 
-                 title_fs2 = 12, label_fs = 11, tick_fs = 10, tick_rot = 0, 
-                 annot_ref = None, annot_fmt = 'simple', annot_fs = 10, 
-                 ws_hs = (0.3, 0.3)):
-    
-    df = df_pct.copy(deep = True)
-    nr, nc = nr_nc
-    ws, hs = ws_hs
-    fig, axes = plt.subplots(figsize=figsize, dpi=dpi, nrows=nr, ncols=nc, constrained_layout=True)
-    fig.tight_layout() # Or equivalently,  "plt.tight_layout()"
-    if title is not None:
-        fig.suptitle('%s' % title, x = 0.5, y = title_y, fontsize = title_fs, ha = 'center')
-    plt.subplots_adjust(left=None, bottom=None, right=None, top=None, wspace=ws, hspace=hs)
-
-    items = list(df.columns.values)
-
-    df['Group'] = list(df.index.values)
-    df['Group'].replace(sg_map, inplace = True)
-
-    lst = df['Group'].unique()
-    lst_pair = []
-    if annot_ref in lst:
-        for k, l1 in enumerate(lst):
-            if l1 != annot_ref:
-                lst_pair.append((annot_ref, l1))
-    else:
-        for k, l1 in enumerate(lst):
-            for j, l2 in enumerate(lst):
-                if j >  k:
-                    lst_pair.append((l1, l2))
-
-    for k, item in enumerate(items):
-        plt.subplot(nr,nc,k+1)
-        ax = sns.boxplot(data = df, x = 'Group', y = item) #, order=['HC', 'CC', 'AC'])
-        if k%nc == 0: plt.ylabel('Percentage', fontsize = label_fs)
-        else: plt.ylabel(None)
-        if k >= nc*(nr-1): plt.xlabel('Condition', fontsize = label_fs)
-        else: plt.xlabel(None)
-        plt.title(item, fontsize = title_fs2)
-        if k < (nr*nc - nc):
-            plt.xticks([])
-            plt.yticks(fontsize = tick_fs)
-        else:
-            plt.xticks(rotation = tick_rot, ha = 'center', fontsize = tick_fs)
-            plt.yticks(fontsize = tick_fs)
-        
-        add_stat_annotation(ax, data=df, x = 'Group', y = item, 
-                        box_pairs=lst_pair, loc='inside', fontsize = annot_fs,
-                        test='t-test_ind', text_format=annot_fmt, verbose=0)
-        #'''
-    if (len(items) < (nr*nc)) & (nr > 1):
-        for k in range(nr*nc - len(items)):
-            axes[nr-1][len(items)%nc + k].axis("off")
-        
-    plt.show()
-    return 
-
-
-def plot_pct_box_old(df_pct, sg_map, nr_nc, figsize = None, dpi = 100,
-                 title = None, title_y = 1.05, title_fs = 14, 
-                 title_fs2 = 12, label_fs = 11, tick_fs = 10, tick_rot = 0, 
-                 annot_fs = 10, ws_hs = (0.3, 0.3)):
-    
-    df = df_pct.copy(deep = True)
-    nr, nc = nr_nc
-    ws, hs = ws_hs
-    fig, axes = plt.subplots(figsize=figsize, dpi=dpi, nrows=nr, ncols=nc, constrained_layout=True)
-    fig.tight_layout() # Or equivalently,  "plt.tight_layout()"
-    if title is not None:
-        fig.suptitle('%s' % title, x = 0.5, y = title_y, fontsize = title_fs, ha = 'center')
-    plt.subplots_adjust(left=None, bottom=None, right=None, top=None, wspace=ws, hspace=hs)
-
-    items = list(df.columns.values)
-
-    df['Group'] = list(df.index.values)
-    df['Group'].replace(sg_map, inplace = True)
-
-    lst = df['Group'].unique()
-    lst_pair = []
-    for k, l1 in enumerate(lst):
-        for j, l2 in enumerate(lst):
-            if j >  k:
-                lst_pair.append((l1, l2))
-
-    for k, item in enumerate(items):
-        plt.subplot(nr,nc,k+1)
-        ax = sns.boxplot(data = df, x = 'Group', y = item) #, order=['HC', 'CC', 'AC'])
-        if k%nc == 0: plt.ylabel('Percentage', fontsize = label_fs)
-        else: plt.ylabel(None)
-        if k >= nc*(nr-1): plt.xlabel('Condition', fontsize = label_fs)
-        else: plt.xlabel(None)
-        plt.title(item, fontsize = title_fs2)
-        if k < (nr*nc - nc):
-            plt.xticks([])
-            plt.yticks(fontsize = tick_fs)
-        else:
-            plt.xticks(rotation = 0, ha = 'center', fontsize = tick_fs)
-            plt.yticks(fontsize = tick_fs)
-
-        add_stat_annotation(ax, data=df, x = 'Group', y = item, # order=['HC', 'CC', 'AC'],
-                        box_pairs=lst_pair, loc='inside', fontsize = annot_fs,
-                        test='t-test_ind', text_format='simple', verbose=0)
-        #'''
-    if (len(items) < (nr*nc)) & (nr > 1):
-        for k in range(nr*nc - len(items)):
-            axes[nr-1][len(items)%nc + k].axis("off")
-        
-    plt.show()
-    return
-
-
-def plot_composition_bar( adata_t,  pid_field = 'pid', cell_type_field = 'cell_type_major_pred',
-                          sort_by = [] ):
-    
-    pid_lst = list(adata_t.obs[pid_field].unique())
-
-    ct_idx = cell_type_field
-    celltype_lst = list(adata_t.obs[ct_idx].unique())
-
-    df_celltype_cnt = pd.DataFrame(index = pid_lst, columns = celltype_lst)
-    df_celltype_cnt.loc[:,:] = 0
-
-    for pid in pid_lst:
-        b = adata_t.obs[pid_field] == pid
-        ct_sel = adata_t.obs.loc[b, ct_idx]
-
-        for ct in celltype_lst:
-            bx = ct_sel == ct
-            df_celltype_cnt.loc[pid, ct] = np.sum(bx)
-
-    df_celltype_pct = df_celltype_cnt.div(df_celltype_cnt.sum(axis = 1), axis = 0)*100
-    
-    if len(sort_by) > 0:
-        df_celltype_pct.sort_values(by = sort_by, inplace = True)
-
-    sc.settings.set_figure_params(figsize=(5, 3), dpi=80, facecolor='white')
-    ax = df_celltype_pct.plot.bar(stacked = True, rot = 90)
-    ax.legend( df_celltype_pct.columns.values, bbox_to_anchor=(1, 1) )
-    
-    return df_celltype_cnt
-
 
 '''
 ### DigitalCellSorter
 
 ## df_ann = cell_type_id_using_DCS( df, name = 'DCS_tmp', batch = None, mkr = 'CIBERSORT_LM22_7', n_clust = 30 )
 
 import urllib.request
```

### Comparing `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/PKG-INFO` & `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi-at-dku-lib
-Version: 0.2.5
+Version: 0.2.6
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/SOURCES.txt` & `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

