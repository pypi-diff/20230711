# Comparing `tmp/SC2Spa-1.1.9.tar.gz` & `tmp/SC2Spa-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SC2Spa-1.1.9.tar", last modified: Wed May 31 14:12:29 2023, max compression
+gzip compressed data, was "SC2Spa-1.2.0.tar", last modified: Tue Jul 11 14:12:51 2023, max compression
```

## Comparing `SC2Spa-1.1.9.tar` & `SC2Spa-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 14:12:29.716720 SC2Spa-1.1.9/
--rwxrwxrwx   0 root         (0) root         (0)     1525 2022-11-18 16:54:51.000000 SC2Spa-1.1.9/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1359 2023-05-31 14:12:29.716263 SC2Spa-1.1.9/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      806 2023-01-09 13:31:30.000000 SC2Spa-1.1.9/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 14:12:29.712256 SC2Spa-1.1.9/SC2Spa/
--rwxrwxrwx   0 root         (0) root         (0)    12963 2023-02-13 15:19:44.000000 SC2Spa-1.1.9/SC2Spa/BM.py
--rwxrwxrwx   0 root         (0) root         (0)     8248 2022-12-06 20:19:48.000000 SC2Spa-1.1.9/SC2Spa/ME.py
--rwxrwxrwx   0 root         (0) root         (0)     3062 2022-07-12 15:41:45.000000 SC2Spa-1.1.9/SC2Spa/PP.py
--rwxrwxrwx   0 root         (0) root         (0)    50542 2023-05-31 14:09:58.000000 SC2Spa-1.1.9/SC2Spa/SI.py
--rwxrwxrwx   0 root         (0) root         (0)     4381 2023-01-08 16:28:45.000000 SC2Spa-1.1.9/SC2Spa/SVA.py
--rwxrwxrwx   0 root         (0) root         (0)    21739 2023-05-30 12:11:12.000000 SC2Spa-1.1.9/SC2Spa/Vis.py
--rwxrwxrwx   0 root         (0) root         (0)      211 2023-03-14 16:25:06.000000 SC2Spa-1.1.9/SC2Spa/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      460 2023-03-14 16:25:06.000000 SC2Spa-1.1.9/SC2Spa/__metadata__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 14:12:29.715349 SC2Spa-1.1.9/SC2Spa.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1359 2023-05-31 14:12:29.000000 SC2Spa-1.1.9/SC2Spa.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      274 2023-05-31 14:12:29.000000 SC2Spa-1.1.9/SC2Spa.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-31 14:12:29.000000 SC2Spa-1.1.9/SC2Spa.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-05-31 14:12:29.000000 SC2Spa-1.1.9/SC2Spa.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      691 2023-05-31 14:12:04.000000 SC2Spa-1.1.9/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-31 14:12:29.716895 SC2Spa-1.1.9/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 14:12:51.272389 SC2Spa-1.2.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1525 2022-11-18 16:54:51.000000 SC2Spa-1.2.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-11 14:12:51.271961 SC2Spa-1.2.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      806 2023-01-09 13:31:30.000000 SC2Spa-1.2.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 14:12:51.268163 SC2Spa-1.2.0/SC2Spa/
+-rwxrwxrwx   0 root         (0) root         (0)    16137 2023-07-11 13:31:56.000000 SC2Spa-1.2.0/SC2Spa/BM.py
+-rwxrwxrwx   0 root         (0) root         (0)     8248 2022-12-06 20:19:48.000000 SC2Spa-1.2.0/SC2Spa/ME.py
+-rwxrwxrwx   0 root         (0) root         (0)     3062 2022-07-12 15:41:45.000000 SC2Spa-1.2.0/SC2Spa/PP.py
+-rwxrwxrwx   0 root         (0) root         (0)    50744 2023-07-11 14:10:24.000000 SC2Spa-1.2.0/SC2Spa/SI.py
+-rwxrwxrwx   0 root         (0) root         (0)     4381 2023-01-08 16:28:45.000000 SC2Spa-1.2.0/SC2Spa/SVA.py
+-rwxrwxrwx   0 root         (0) root         (0)    23359 2023-07-03 11:43:39.000000 SC2Spa-1.2.0/SC2Spa/Vis.py
+-rwxrwxrwx   0 root         (0) root         (0)      211 2023-03-14 16:25:06.000000 SC2Spa-1.2.0/SC2Spa/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      460 2023-07-11 14:12:07.000000 SC2Spa-1.2.0/SC2Spa/__metadata__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 14:12:51.271101 SC2Spa-1.2.0/SC2Spa.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-11 14:12:51.000000 SC2Spa-1.2.0/SC2Spa.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      274 2023-07-11 14:12:51.000000 SC2Spa-1.2.0/SC2Spa.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-11 14:12:51.000000 SC2Spa-1.2.0/SC2Spa.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-07-11 14:12:51.000000 SC2Spa-1.2.0/SC2Spa.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      691 2023-07-11 14:11:48.000000 SC2Spa-1.2.0/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-11 14:12:51.272566 SC2Spa-1.2.0/setup.cfg
```

### Comparing `SC2Spa-1.1.9/LICENSE` & `SC2Spa-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.9/PKG-INFO` & `SC2Spa-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.1.9
+Version: 1.2.0
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `SC2Spa-1.1.9/README.md` & `SC2Spa-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.9/SC2Spa/BM.py` & `SC2Spa-1.2.0/SC2Spa/BM.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import anndata
 from scipy import stats
 from sklearn.metrics import r2_score
+from sklearn.neighbors import NearestNeighbors
+from functools import reduce
 import numpy as np
 import pandas as pd
 import os
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 
 from scipy.stats import bootstrap
 
-from matplotlib import rc
-rc('font', **{'family':'sans-serif','sans-serif':['Helvetica']})
+from . import PP
+
+#from matplotlib import rc
+#rc('font', **{'family':'sans-serif','sans-serif':['Helvetica']})
+
+import seaborn as sns
+cmap = sns.cubehelix_palette(n_colors = 32,start = 2, rot=1.5, as_cmap = True)
 
 #Number of columes for the prediction
 #Global variable
 n_col = 2
 
 def my_pearsonr(Y_pred, Y_true):
     '''
@@ -154,35 +161,76 @@
      and Coefficient of Determination
     '''
 
     pearsonr = []
     for i in range(Y_true.shape[1]):
         t = stats.pearsonr(Y_true[:, i], Y_pred[:, i])[0]
         pearsonr.append(t)
+
+    #N = reduce(lambda x, y: x*y, Y_true.shape)
+
     rmse = np.sqrt(np.square(Y_true - Y_pred).sum() / Y_true.shape[0])
     r2 = r2_score(Y_true, Y_pred, multioutput='variance_weighted')
     out = [np.array(pearsonr).mean(), rmse, r2]
 
     return out
 
-def eval_cv(preds: list, YNorm: np.array, test_indices: list, CI_BS = False, n_resamples=200):
+
+def obtain_PDs(indices, CP, Y_Norm_all, Y_pred):
+    Original_PC1 = Y_Norm_all[CP[:, 0].astype(int)]
+    Original_PC2 = Y_Norm_all[CP[:, 1].astype(int)]
+    PD_true = ((Original_PC2 - Original_PC1) ** 2).sum(axis=1) ** 0.5
+
+    pred = pd.DataFrame(Y_pred, index=indices)
+    pred_PC1 = pred.loc[CP[:, 0].astype(int)].values
+    pred_PC2 = pred.loc[CP[:, 1].astype(int)].values
+    PD_pred = ((pred_PC2 - pred_PC1) ** 2).sum(axis=1) ** 0.5
+
+    return PD_pred, PD_true
+
+
+def PD_rmse(PD_pred, PD_true):
+    out = ((PD_pred - PD_true) ** 2).mean() ** 0.5
+
+    return out
+
+
+def eval_PD_rmse(YNorm, test_indices, preds, CPs):
+    PDRMSEs = []
+    PD_Pearsons = []
+
+    for i in range(len(test_indices)):
+        PD_pred, PD_true = obtain_PDs(indices=test_indices[i], CP=CPs[i],
+                                      Y_Norm_all=YNorm, Y_pred=preds[i])
+        PDRMSE = PD_rmse(PD_pred, PD_true)
+        PD_Pearson = stats.pearsonr(PD_pred, PD_true)[0]
+
+        PDRMSEs.append(PDRMSE)
+        PD_Pearsons.append(PD_Pearson)
+
+    return PDRMSEs, PD_Pearsons
+
+def eval_cv(preds: list, YNorm: np.array, test_indices: list, CPs: np.array,
+            CI_BS = False, n_resamples=200):
     '''
     Caculaate the Pearson Correlation Coefficient, Root Mean Square Error
      and Coefficient of Determination between the predicted locations
       and the original locations for the test beads in Cross-Validation.
     Corresponding confidence intervals will be calculated if `CI_BS` is True.
 
     Parameters
     ---------
     preds
-        The predicted locations for the test beads in cross-validation
+        The predicted min-max normalized locations for the test beads in cross-validation
     YNorm
-        The min-max normalized original locations of all beads
+        The original min-max normalized locations of all beads
     test_indices
         The indices of test beads in cross-validation
+    CPs
+        Cell pairs in the format of numpy array
     CI_BS
         Calculate confidence interval using bootstrap if True
     n_resamples
         The number of resamples performed to form the bootstrap distribution of the statistic
 
     Returns
     -------
@@ -206,14 +254,18 @@
         for i in range(len(preds)):
             performance = evaluate(Y_pred = preds[i],
                                    Y_true = YNorm[test_indices[i]])
             performances.append(performance)
 
         statistics = pd.DataFrame(performances,
                                   columns = ['pearsonr', 'RMSE', 'R2'])
+        PDRMSEs, PD_Pearsons = eval_PD_rmse(YNorm = YNorm, test_indices = test_indices, preds = preds,
+                                 CPs = CPs)
+        statistics['PD_RMSE'] = PDRMSEs
+        statistics['PD_Pearson'] = PD_Pearsons
 
         return statistics
 
     
 def Visualize_SSV2(adata:anndata.AnnData, coord:np.array, out_prefix = 'Benchmarking/MH1/',
 		           ctname = 'MCT', anchor = (1, 0.9), s = 3,
 	               xlim = [650, 5750], ylim = [650, 5750], lim = False,
@@ -303,15 +355,66 @@
     ###################
     # Create legend
     plt.legend(handles=scatter.legend_elements()[0],
                labels=list(t.obs[ctname].unique()))
     # Get current axes object and turn off axis
     plt.gca().set_axis_off()
     plt.savefig(out_prefix + 'legend.png', bbox_inches='tight')
-    
+
+
+def Vis_Euclidean(coord_ref: np.array, coord_pred: np.array, max_value: float,
+         out_prefix='BM_figures_2/MH1/', figsize=(8, 6), s=3, xlim=[650, 5750],
+         ylim=[650, 5750], cmap=cmap, lim=False, save='SC2Spa'):
+    '''
+    Show the euclidean distance of the original and predicted locations of beads.
+    Beads are colored by the distance.
+
+    Parameters
+    ---------
+    adata
+        A AnnData object. Cell type information is stored in adata.obs[ctname].
+    coord_ref
+        True coordinates of beads
+    coord_pred
+        Predicted coordinates of beads
+    s
+        size of beads in the figure
+    save
+        save the figure in `out_prefix` + `save` + '.png' if save is not None
+
+    Returns
+    -------
+    None
+
+    '''
+
+    if not os.path.exists(out_prefix):
+        os.makedirs(out_prefix)
+
+    dis = ((coord_pred - coord_ref) ** 2).sum(axis=1) ** 0.5
+
+    plt.figure(figsize=figsize)
+    plt.scatter(coord_ref[:, 0], coord_ref[:, 1],
+                s=s, c=dis, cmap=cmap, vmax = max_value)
+    plt.grid(False)
+    plt.tick_params(axis='both',
+                    which='both',
+                    bottom=False,
+                    labelbottom=False,
+                    left=False,
+                    labelleft=False)
+    plt.colorbar()
+    if (lim):
+        plt.xlim(xlim)
+        plt.ylim(ylim)
+    if (save != None):
+        plt.savefig(out_prefix + save + '.png', bbox_inches='tight')
+    plt.show()
+
+
 def Barplot(BMs:list, BMs_std = None, fontsize = 12, legend = False, save_root = 'Benchmarking/',
 	        colors = ['C3', 'C5', 'C4', 'C1', 'C0'], fill = True):
     '''
     Benchmark multiple tools on multiple datasets.
     A figure will be saved to `'Benchmarking/'+column+'_no_legend.png'`
     The legend of the figure will be saved to `'Benchmarking/barplot_legend.png'`
```

### Comparing `SC2Spa-1.1.9/SC2Spa/ME.py` & `SC2Spa-1.2.0/SC2Spa/ME.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.9/SC2Spa/PP.py` & `SC2Spa-1.2.0/SC2Spa/PP.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.9/SC2Spa/SI.py` & `SC2Spa-1.2.0/SC2Spa/SI.py`

 * *Files 1% similar despite different names*

```diff
@@ -696,16 +696,17 @@
     #Label closest ST beads of single cells
     adata_query.obs['ClosestBead_order'] = neighbors_sc[range(neighbors_sc.shape[0]),
                                                         dis_sc.argmin(axis=1)]
     adata_query.obs['ClosestBead_name'] = adata_query.obs['ClosestBead_order'].apply(lambda x: adata_ref.obs_names[x] if x < n_ST else 'NA')
 
     #Label closest single cells of ST beads
     # ClosestSC_list = adata_query.groupby('ClosestBead_name', as_index = False)['Dis2ClosestBead'].idxmin()['Dis2ClosestBead'].tolist()
+    index_name = adata_query.obs.reset_index().columns[0]
     ClosestSC_list = adata_query.obs.reset_index().groupby('ClosestBead_name', as_index=False).agg(
-        {'Dis2ClosestBead': 'min', 'index': 'first'})['index'].tolist()
+        {'Dis2ClosestBead': 'min', index_name: 'first'})[index_name].tolist()
     adata_query.obs['ClosestSC'] = False
     adata_query.obs.loc[ClosestSC_list, 'ClosestSC'] = True
 
     adata_query.obs['Recon_scST'] = False
     adata_query.obs['Recon_scST_layer'] = -1
     for layer, n_cell in enumerate(n_layer_cell):
 
@@ -888,15 +889,15 @@
     neighbors_st[dis_st > dis_cutoff] = -1
     ST_mask2 = (neighbors_st >= n_ST).sum(axis=1) > 0
     dis_st = dis_st[ST_mask2]
     neighbors_st = neighbors_st[ST_mask2]
 
     return neighbors_st, dis_st
 
-def NRD_weight(neighbors, dis, adata_ref, adata_query, ct_name='simp_name', weight_constant = 1):
+def NRD_weight(neighbors, dis, adata_ref, adata_query, ct_name=None, weight_constant = 1):
 
     '''
     Calculate the weights of nearby single cells for ST beads based on the fine mapping result
 
     Parameters
     ---------
     neighbors
@@ -929,15 +930,16 @@
                                   dis[:, 1:].flatten().reshape((-1, 1))], axis=1)
     df_neighbor = pd.DataFrame(df_neighbor, columns=['center', 'neighbor', 'dis'])
     # Select single cell neighbors for ST beads
     # Remove cell pairs whose distance are more than the cutoff distance
     ##(ID was labelled as -1 in the fine mapping step)
     df_neighbor = df_neighbor[df_neighbor['neighbor'] >= n_ST].reset_index(drop=True)
     df_neighbor[['center', 'neighbor']] = df_neighbor[['center', 'neighbor']].astype(int)
-    df_neighbor['SCT'] = adata_query.obs.iloc[df_neighbor['neighbor'] - n_ST][ct_name].tolist()
+    if(ct_name!=None):
+        df_neighbor['SCT'] = adata_query.obs.iloc[df_neighbor['neighbor'] - n_ST][ct_name].tolist()
 
     df_neighbor['weight'] = 1 / (df_neighbor['dis'] + weight_constant)
 
     return df_neighbor
 
 
 def NRD_CT(neighbors, dis, adata_ref, adata_query, ct_name='simp_name', weight_constant = 1,
@@ -975,15 +977,15 @@
 
     '''
 
     df_neighbor = NRD_weight(neighbors, dis, adata_ref, adata_query,
                              ct_name=ct_name, weight_constant=weight_constant)
 
     # Exclude CTs
-    if(exclude_CTs != None):
+    if((exclude_CTs != None)&(ct_name!=None)):
         select = df_neighbor['SCT'].apply(lambda x: x not in exclude_CTs)
         df_neighbor = df_neighbor[select]
 
     # Calculate normalized reciprocal distance for each cell type
     CT_NRD = df_neighbor[['center', 'SCT', 'weight']].groupby(['center', 'SCT']).max()
     CT_NRD = CT_NRD / CT_NRD.groupby(['center']).sum()
 
@@ -1005,15 +1007,15 @@
     ref_CT_NRD_ind = np.where(adata_ref.obs.columns == 'CT_NRD')[0][0]
     adata_ref.obs.iloc[CT_NRD_df.index, ref_CT_NRD_ind] = True
 
     CT_NRD_df.index = adata_ref.obs.index[CT_NRD_df.index]
     adata_ref.obs = adata_ref.obs.merge(CT_NRD_df, how='left', left_index=True, right_index=True)
 
 
-def NRD_impute(neighbors, dis, adata_ref, adata_query, ct_name='simp_name',
+def NRD_impute(neighbors, dis, adata_ref, adata_query, ct_name=None,
                weight_constant = 1, exclude_CTs=None):
 
     '''
     Reconstruct the gene expression profile of ST beads based on the NRD_weight output
     Predicted cell type proportion will be saved in adata_ref.obs.
 
     Parameters
@@ -1039,15 +1041,15 @@
     adata_impute
         An Anndata object that stores the reconstructed gene expression profile of ST beads
 
     '''
     df_neighbor = NRD_weight(neighbors, dis, adata_ref, adata_query,
                              ct_name=ct_name, weight_constant = weight_constant)
 
-    if (exclude_CTs != None):
+    if((exclude_CTs != None)&(ct_name!=None)):
         select = df_neighbor['SCT'].apply(lambda x: x not in exclude_CTs)
         df_neighbor = df_neighbor[select]
 
     CT_NRD = df_neighbor[['center', 'neighbor', 'weight']].groupby(['center', 'neighbor']).sum()
     CT_NRD = CT_NRD / CT_NRD.groupby(['center']).sum()
 
     n_ST = adata_ref.shape[0]
@@ -1299,34 +1301,36 @@
             pickle.dump(history, handle)
 
         with open('log/training_log_' + name + '.pickle', 'rb') as handle:
             history = pickle.load(handle)
             
         print(history.history['val_mse'][-1])
         
-def CheckAccuracy(name:str):
+def CheckAccuracy(name:str, item_name = 'rmse'):
     '''
      Read the FCNN or LR training histories saved in 'log/training_log_' + name + '.pickle'
      and Output accuracies and mean accuracy of cross-validation
 
      Parameters
      ----------
      name
+     item_name
+        loss name saved in the history files
 
      Returns
      -------
      None
 
      '''
     with open('log/training_log_' + name + '.pickle', 'rb') as handle:
         histories = pickle.load(handle)
 
         accuracy = []
 
         for history in histories:
-            accuracy.append(history['val_accuracy'][-1])
+            accuracy.append(history['val_' + item_name][-1])
 
         print(name)
-        print('Validation Accuracy')
+        print('Validation', item_name)
         print(accuracy)
         print(np.mean(accuracy))
```

### Comparing `SC2Spa-1.1.9/SC2Spa/SVA.py` & `SC2Spa-1.2.0/SC2Spa/SVA.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.9/SC2Spa/Vis.py` & `SC2Spa-1.2.0/SC2Spa/Vis.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,70 @@
                bbox_to_anchor=(1, 0.9))
     if(doub):
         out = 'doub_' + str(out)
     plt.savefig(root + 'train_overall_' + str(out) + '.pdf', bbox_inches='tight')
     plt.show()
 
 
+def VisCustomize2(adata: anndata.AnnData, coords_name,
+                  preds, ct_name, root, out, sta, end):
+    '''
+    Customized function for the paper
+
+    Parameters
+    ---------
+    adata
+    Coordinate Information should be stored in `adata.obsm[coords_name]`
+    Predicted Coordinate Information should be stored in `adata.obsm[preds_name]`
+
+    Returns
+    -------
+    None
+    '''
+    CTs = adata.obs[ct_name].value_counts()
+
+    SelectedCTs = CTs.index.tolist()[sta:end]
+
+    t = adata
+    Select1 = t.obs[ct_name].apply(lambda x: x in SelectedCTs)
+    Select = Select1
+    t = t[Select]
+    preds = preds[Select]
+
+    color_dic = {}
+    for i, ct in enumerate(t.obs[ct_name].unique()):
+        color_dic[ct] = i
+
+    color = list(map(lambda x: color_dic[x], t.obs[ct_name]))
+
+    fig, axes = plt.subplots(1, 2, figsize=(13, 5))
+
+    axes[0].scatter(t.obsm[coords_name][:, 0],
+                    t.obsm[coords_name][:, 1],
+                    s=3, c=color,
+                    cmap=plt.get_cmap('Paired'))
+
+    scatter = axes[1].scatter(preds[:, 0], preds[:, 1],
+                              s=3, c=color,
+                              cmap=plt.get_cmap('Paired'))
+
+    # plt.axis('off')
+
+    axes[0].title.set_text('raw')
+    axes[1].title.set_text('pred')
+
+    plt.legend(handles=scatter.legend_elements()[0],
+               labels=list(t.obs[ct_name].unique()),
+               bbox_to_anchor=(1, 0.9))
+
+    if not os.path.exists(root):
+        os.makedirs(root)
+    plt.savefig(root + 'Compare_' + str(out) + '.pdf', bbox_inches='tight')
+    plt.show()
+
 def DrawSVG(adata:anndata.AnnData, GeneList:pd.DataFrame, target_field: str, coords_name='spatial',
             n_genes = 9, s = 2, lim = False, alpha = 0.8, xlim = [650, 5750], ylim = [650, 5750],
             cmap = cmap, FM = True, scST = False, root = 'figures/SVG/', fontsize=40, CT_name = 'MCT',
             CT = '', Sparse = True, Bottom = False, output = None):
 
     '''
     Show the expression of location predictive genes (or spatially variable genes)
@@ -650,15 +706,15 @@
 
     Returns
     -------
     None
 
     '''
     from matplotlib import rc
-    rc('font', **{'family':'sans-serif','sans-serif':['Helvetica']})
+    rc('font', **{'family':'Arial','sans-serif':['Arial']})
     plt.rcParams['font.size'] = size
 
     a = np.array([[0,1]])
     pl.figure(figsize=figsize)
     img = pl.imshow(a, cmap=cmap)
     pl.gca().set_visible(False)
     cax = pl.axes([0, 0, 0.02, 1.6])
```

### Comparing `SC2Spa-1.1.9/SC2Spa.egg-info/PKG-INFO` & `SC2Spa-1.2.0/SC2Spa.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.1.9
+Version: 1.2.0
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `SC2Spa-1.1.9/pyproject.toml` & `SC2Spa-1.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SC2Spa"
-version = "1.1.9"
+version = "1.2.0"
 authors = [
   { name="Linbu Liao, Won Lab", email="linbu.liao@gmail.com" },
 ]
 description = "SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

