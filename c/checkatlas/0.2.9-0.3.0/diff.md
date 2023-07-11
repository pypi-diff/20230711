# Comparing `tmp/checkatlas-0.2.9.tar.gz` & `tmp/checkatlas-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkatlas-0.2.9.tar", max compression
+gzip compressed data, was "checkatlas-0.3.0.tar", max compression
```

## Comparing `checkatlas-0.2.9.tar` & `checkatlas-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,36 @@
--rw-r--r--   0        0        0     1211 2023-07-07 21:13:51.160490 checkatlas-0.2.9/LICENSE
--rw-r--r--   0        0        0     4238 2023-07-07 21:13:51.164491 checkatlas-0.2.9/README.md
--rw-r--r--   0        0        0      117 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/__init__.py
--rw-r--r--   0        0        0    21675 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/atlas.py
--rw-r--r--   0        0        0    17277 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/atlas_seurat.py
--rw-r--r--   0        0        0     6631 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/checkatlas.py
--rw-r--r--   0        0        0     1905 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/folders.py
--rw-r--r--   0        0        0        0 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/__init__.py
--rw-r--r--   0        0        0      192 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/annot/__init__.py
--rw-r--r--   0        0        0      242 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/annot/adj_mutual_info.py
--rw-r--r--   0        0        0      153 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/annot/dunn_index.py
--rw-r--r--   0        0        0      232 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/annot/fowlkes_mallow.py
--rw-r--r--   0        0        0      228 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/annot/rand_index.py
--rw-r--r--   0        0        0      220 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/annot/vmeasure.py
--rw-r--r--   0        0        0      125 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/cluster/__init__.py
--rw-r--r--   0        0        0      225 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/cluster/calinski_harabasz.py
--rw-r--r--   0        0        0      219 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/cluster/davies_bouldin.py
--rw-r--r--   0        0        0      211 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/cluster/silhouette.py
--rw-r--r--   0        0        0       89 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/dimred/__init__.py
--rw-r--r--   0        0        0      602 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/dimred/kruskal_stress.py
--rw-r--r--   0        0        0      162 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/dimred/spearman_rho.py
--rw-r--r--   0        0        0     4103 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/metrics.py
--rw-r--r--   0        0        0        0 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/specificity/__init__.py
--rw-r--r--   0        0        0     6278 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/specificity/analysis.py
--rw-r--r--   0        0        0     8417 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/specificity/compute.py
--rw-r--r--   0        0        0     4107 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/specificity/get_data.py
--rw-r--r--   0        0        0     9993 2023-07-07 21:13:51.164491 checkatlas-0.2.9/checkatlas/metrics/specificity/plot.py
--rw-r--r--   0        0        0     1266 2023-07-07 21:13:51.364509 checkatlas-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     5378 1970-01-01 00:00:00.000000 checkatlas-0.2.9/setup.py
--rw-r--r--   0        0        0     5187 1970-01-01 00:00:00.000000 checkatlas-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1506 2023-07-11 21:43:46.215059 checkatlas-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4452 2023-07-11 21:43:46.215059 checkatlas-0.3.0/README.md
+-rw-r--r--   0        0        0      111 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/__init__.py
+-rw-r--r--   0        0        0     4648 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/__main__.py
+-rw-r--r--   0        0        0    24191 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/atlas.py
+-rw-r--r--   0        0        0     4715 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/cellranger.py
+-rw-r--r--   0        0        0     4236 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/checkatlas.py
+-rw-r--r--   0        0        0       45 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/annot/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/annot/adj_mutual_info.py
+-rw-r--r--   0        0        0      153 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/annot/dunn_index.py
+-rw-r--r--   0        0        0      232 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/annot/fowlkes_mallow.py
+-rw-r--r--   0        0        0      228 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/annot/rand_index.py
+-rw-r--r--   0        0        0      220 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/annot/vmeasure.py
+-rw-r--r--   0        0        0      125 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/cluster/__init__.py
+-rw-r--r--   0        0        0      225 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/cluster/calinski_harabasz.py
+-rw-r--r--   0        0        0      219 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/cluster/davies_bouldin.py
+-rw-r--r--   0        0        0      211 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/cluster/silhouette.py
+-rw-r--r--   0        0        0       89 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/dimred/__init__.py
+-rw-r--r--   0        0        0      602 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/dimred/kruskal_stress.py
+-rw-r--r--   0        0        0      162 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/dimred/spearman_rho.py
+-rw-r--r--   0        0        0     4108 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/metrics.py
+-rw-r--r--   0        0        0        0 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/specificity/__init__.py
+-rw-r--r--   0        0        0     6278 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/specificity/analysis.py
+-rw-r--r--   0        0        0     8417 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/specificity/compute.py
+-rw-r--r--   0        0        0     4107 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/specificity/get_data.py
+-rw-r--r--   0        0        0     9993 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/specificity/plot.py
+-rw-r--r--   0        0        0    20167 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/seurat.py
+-rw-r--r--   0        0        0      107 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/utils/__init__.py
+-rw-r--r--   0        0        0     4544 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/utils/checkatlas_arguments.py
+-rw-r--r--   0        0        0     2230 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/utils/files.py
+-rw-r--r--   0        0        0     1960 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/utils/folders.py
+-rw-r--r--   0        0        0     6267 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/utils/obsolete_arguments.py
+-rw-r--r--   0        0        0     1350 2023-07-11 21:43:46.399061 checkatlas-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5726 1970-01-01 00:00:00.000000 checkatlas-0.3.0/setup.py
+-rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 checkatlas-0.3.0/PKG-INFO
```

### Comparing `checkatlas-0.2.9/README.md` & `checkatlas-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 ![Conda](https://img.shields.io/conda/pn/bioconda/checkatlas)
 
 [![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)
 [![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)
 [![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)
 
+![Static Badge](https://img.shields.io/badge/Packaging-Poetry-blue)
+![Static Badge](https://img.shields.io/badge/Docs-Mkdocs-red)
+![Static Badge](https://img.shields.io/badge/Linting-flake8%20black%20mypy-yellow)
+
 CheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the
 quality control tables and figures which can be then processed by multiqc. CheckAtlas is able to load Scanpy, Seurat,
 and CellRanger files.
 
 
 ## Summary
```

### Comparing `checkatlas-0.2.9/checkatlas/atlas.py` & `checkatlas-0.3.0/checkatlas/atlas.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,39 @@
+import argparse
 import logging
 import os
 import re
+import warnings
 
-import anndata
 import numpy as np
 import pandas as pd
 import scanpy as sc
+from anndata import AnnData
+from anndata import _io as _io
 
-from . import checkatlas, folders
+from . import cellranger, checkatlas
 from .metrics import metrics
-
-# try:
-#     from .metrics.cluster import clust_compute
-# except ImportError:
-#     from metrics.cluster import clust_compute
-# try:
-#     from .metrics.dim_red import dr_compute
-# except ImportError:
-#     from metrics.dim_red import dr_compute
-#
-# try:
-#     from . import checkatlas, folders
-# except ImportError:
-#     import folders
-#     import checkatlas
-
+from .utils import files, folders
 
 """
-Atlas module
+Atlas module for AnnData (Scanpy)
 All the function to screen the atlases
 """
 
+ANNDATA_TYPE = "AnnData"
+ANNDATA_EXTENSION = ".h5ad"
+
 OBS_CLUSTERS = [
     "cell_type",
     "CellType",
     "celltype",
     "ann_finest_level",
     "cellranger_graphclust",
     "seurat_clusters",
+    "RNA_snn_res.0.5",
     "louvain",
     "leiden",
     "orig.ident",
 ]
 
 OBSM_DIMRED = [
     "X_umap",
@@ -72,71 +64,97 @@
     "pct_counts_ribo",
 ]
 
 CELLINDEX_HEADER = "cell_index"
 
 logger = logging.getLogger("checkatlas")
 
+warnings.simplefilter(action="ignore", category=FutureWarning)
+warnings.simplefilter(action="ignore", category=UserWarning)
+sc.settings.verbosity = 0
+
 
-def read_atlas(atlas_path, atlas_info):
-    logger.info(f"Load {atlas_info[0]} in {atlas_info[-1]}")
+def detect_scanpy(atlas_path: str) -> dict:
+    if atlas_path.endswith(ANNDATA_EXTENSION):
+        atlas_info = dict()
+        atlas_info[checkatlas.ATLAS_NAME_KEY] = os.path.splitext(
+            os.path.basename(atlas_path)
+        )[0]
+        atlas_info[checkatlas.ATLAS_TYPE_KEY] = ANNDATA_TYPE
+        atlas_info[checkatlas.ATLAS_EXTENSION_KEY] = ANNDATA_EXTENSION
+        atlas_info[checkatlas.ATLAS_PATH_KEY] = atlas_path
+        return atlas_info
+    else:
+        return dict()
+
+
+def read_atlas(atlas_info: dict) -> AnnData:
+    """
+    Read Scanpy or Cellranger data : .h5ad or .h5
+
+    Args:
+        atlas_path (dict): info about the atlas
+
+    Returns:
+        AnnData: scanpy object from .h5ad
+    """
+    logger.info(
+        f"Load {atlas_info[checkatlas.ATLAS_NAME_KEY]} "
+        f"in {atlas_info[checkatlas.ATLAS_PATH_KEY]}"
+    )
     try:
-        if atlas_path.endswith(".h5"):
-            logger.debug(f"Read Cellranger results {atlas_path}")
-            adata = read_cellranger(atlas_path)
+        if (
+            atlas_info[checkatlas.ATLAS_TYPE_KEY]
+            == cellranger.CELLRANGER_TYPE_CURRENT
+        ):
+            logger.debug(
+                "Read Cellranger results "
+                f"{atlas_info[checkatlas.ATLAS_PATH_KEY]}"
+            )
+            adata = cellranger.read_cellranger_current(atlas_info)
+        elif (
+            atlas_info[checkatlas.ATLAS_TYPE_KEY]
+            == cellranger.CELLRANGER_TYPE_OBSOLETE
+        ):
+            logger.debug(
+                "Read Cellranger results "
+                f"{atlas_info[checkatlas.ATLAS_PATH_KEY]}"
+            )
+            adata = cellranger.read_cellranger_obsolete(atlas_info)
         else:
-            logger.debug(f"Read Scanpy file {atlas_path}")
-            adata = sc.read_h5ad(atlas_path)
+            logger.debug(
+                f"Read Scanpy file {atlas_info[checkatlas.ATLAS_PATH_KEY]}"
+            )
+            adata = sc.read_h5ad(atlas_info[checkatlas.ATLAS_PATH_KEY])
         return adata
-    except anndata._io.utils.AnnDataReadError:
-        logger.warning(f"AnnDataReadError, cannot read: {atlas_info[0]}")
-        return None
-
-
-def read_cellranger(atlas_path):
-    cellranger_path = atlas_path.replace(checkatlas.CELLRANGER_FILE, "")
-    cellranger_path = os.path.join(cellranger_path, "outs")
-    clust_path = os.path.join(
-        cellranger_path, "analysis", "clustering", "graphclust", "clusters.csv"
-    )
-    rna_umap = os.path.join(
-        cellranger_path, "analysis", "umap", "2_components", "projection.csv"
-    )
-    rna_tsne = os.path.join(
-        cellranger_path, "analysis", "tsne", "2_components", "projection.csv"
-    )
-    rna_pca = os.path.join(
-        cellranger_path, "analysis", "pca", "10_components", "projection.csv"
-    )
-    adata = sc.read_10x_h5(atlas_path)
-    adata.var_names_make_unique()
-    # Add cluster
-    if os.path.exists(clust_path):
-        df_cluster = pd.read_csv(clust_path, index_col=0)
-        adata.obs["cellranger_graphclust"] = df_cluster["Cluster"]
-    # Add reduction
-    if os.path.exists(rna_umap):
-        df_umap = pd.read_csv(rna_umap, index_col=0)
-        adata.obsm["X_umap"] = df_umap
-    if os.path.exists(rna_tsne):
-        df_tsne = pd.read_csv(rna_tsne, index_col=0)
-        adata.obsm["X_tsne"] = df_tsne
-    if os.path.exists(rna_pca):
-        df_pca = pd.read_csv(rna_pca, index_col=0)
-        adata.obsm["X_pca"] = df_pca
-    return adata
+    except _io.utils.AnnDataReadError:
+        logger.warning(
+            "AnnDataReadError, cannot read: "
+            f"{atlas_info[checkatlas.ATLAS_PATH_KEY]}"
+        )
+        return dict()
 
 
-def clean_scanpy_atlas(adata, atlas_info) -> bool:
+def clean_scanpy_atlas(adata: AnnData, atlas_info: dict) -> AnnData:
     """
     Clean the Scanpy object to be sure to get all information out of it
-    :param adata:
-    :return:
+
+    - Make var names unique
+    - Make var unique for Raw matrix
+    - If OBS_CLUSTERS are present and in int32 -> be sure to
+    transform them in categorical
+
+    Args:
+        adata (AnnData): atlas to analyse
+        atlas_info (dict): info on the atlas
+
+    Returns:
+        AnnData: cleaned atlas
     """
-    logger.debug(f"Clean scanpy: {atlas_info[0]}")
+    logger.debug(f"Clean scanpy: {atlas_info[checkatlas.ATLAS_NAME_KEY]}")
     # Make var names unique
     list_var = adata.var_names
     if len(set(list_var)) == len(list_var):
         logger.debug("Var names unique")
     else:
         logger.debug(
             "Var names not unique, ran : adata.var_names_make_unique()"
@@ -190,35 +208,45 @@
                     adata.obs[obs_key].dtype == np.int32
                     or adata.obs[obs_key].dtype == np.int64
                 ):
                     adata.obs[obs_key] = pd.Categorical(adata.obs[obs_key])
     return adata
 
 
-def get_viable_obs_qc(adata, args):
+def get_viable_obs_qc(adata: AnnData, args: argparse.Namespace) -> list:
     """
     Search in obs_keys a match to OBS_QC values
     Extract sorted obs_keys in same order then OBS_QC
-    :param adata:
-    :return:
+
+    Args:
+        adata (AnnData): atlas to analyse
+        args (argparse.Namespace): list of arguments from checkatlas workflow
+
+    Returns:
+        list: obs_keys
     """
     obs_keys = list()
     for obs_key in adata.obs_keys():
         if obs_key in args.qc_display:
             obs_keys.append(obs_key)
     return obs_keys
 
 
-def get_viable_obs_annot(adata, args):
+def get_viable_obs_annot(adata: AnnData, args: argparse.Namespace) -> list:
     """
     Search in obs_keys a match to OBS_CLUSTERS values
     ! Remove obs_key with only one category !
     Extract sorted obs_keys in same order then OBS_CLUSTERS
-    :param adata:
-    :return:
+
+    Args:
+        adata (AnnData): atlas to analyse
+        args (argparse.Namespace): list of arguments from checkatlas workflow
+
+    Returns:
+        list: obs_keys
     """
     obs_keys = list()
     # Get keys from OBS_CLUSTERS
     for obs_key in adata.obs_keys():
         for obs_key_celltype in args.obs_cluster:
             if obs_key_celltype in obs_key:
                 if type(adata.obs[obs_key].dtype) == pd.CategoricalDtype:
@@ -236,81 +264,90 @@
         # Add obs_key with more than one category (with Nan removed)
         if len(categories) != 1:
             logger.debug(f"Add obs_key {obs_key} with cat {categories_temp}")
             obs_keys_final.append(obs_key)
     return sorted(obs_keys_final)
 
 
-def get_viable_obsm(adata, args):
+def get_viable_obsm(adata: AnnData, args: argparse.Namespace) -> list:
     """
+    TO DO
     Search viable obsm for dimensionality reduction metric
     calc.
     ! No filter on osbm is appled for now !
-    :param adata:
-    :param args:
-    :return:
+    Args:
+        adata (AnnData): atlas to analyse
+        args (argparse.Namespace): list of arguments from checkatlas workflow
+
+    Returns:
+        list: obsm_keys
     """
     obsm_keys = list()
     # for obsm_key in adata.obsm_keys():
     #   if obsm_key in args.obsm_dimred:
     obsm_keys = adata.obsm_keys()
     logger.debug(f"Add obsm {obsm_keys}")
     return obsm_keys
 
 
-def create_summary_table(adata, atlas_path, atlas_info, args) -> None:
+def create_summary_table(
+    adata: AnnData, atlas_info: dict, args: argparse.Namespace
+) -> None:
     """
-    Create a table with all interesting variables
-    :param adata:
-    :param atlas_name:
-    :param csv_path:
-    :return:
-    """
-    atlas_name = atlas_info[0]
+    Create a table with all summarizing variables
+
+    Args:
+        adata (AnnData): atlas to analyse
+        atlas_path (str): path of the atlas
+        args (argparse.Namespace): list of arguments from checkatlas workflow
+    """
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
+    atlas_type = atlas_info[checkatlas.ATLAS_TYPE_KEY]
+    atlas_path = atlas_info[checkatlas.ATLAS_PATH_KEY]
     logger.debug(f"Create Summary table for {atlas_name}")
-    atlas_file_type = atlas_info[1]
-    atlas_extension = atlas_info[2]
-    csv_path = os.path.join(
-        folders.get_folder(args.path, folders.SUMMARY),
-        atlas_name + checkatlas.SUMMARY_EXTENSION,
+    csv_path = files.get_file_path(
+        atlas_name, folders.SUMMARY, checkatlas.SUMMARY_EXTENSION, args.path
     )
     # Create summary table
     header = [
         "AtlasFileType",
         "NbCells",
         "NbGenes",
         "AnnData.raw",
         "AnnData.X",
         "File_extension",
         "File_path",
     ]
     df_summary = pd.DataFrame(index=[atlas_name], columns=header)
-    df_summary["AtlasFileType"][atlas_name] = atlas_file_type
+    df_summary["AtlasFileType"][atlas_name] = atlas_type
     df_summary["NbCells"][atlas_name] = adata.n_obs
     df_summary["NbGenes"][atlas_name] = adata.n_vars
     df_summary["AnnData.raw"][atlas_name] = adata.raw is not None
     df_summary["AnnData.X"][atlas_name] = adata.X is not None
-    df_summary["File_extension"][atlas_name] = atlas_extension
-    df_summary["File_path"][atlas_name] = atlas_path.replace(args.path, "")
+    df_summary["File_extension"][atlas_name] = atlas_name
+    df_summary["File_path"][atlas_name] = atlas_path
     df_summary.to_csv(csv_path, index=False, sep="\t")
 
 
-def create_anndata_table(adata, atlas_path, atlas_info, args) -> None:
+def create_anndata_table(
+    adata: AnnData, atlas_info: dict, args: argparse.Namespace
+) -> None:
     """
-    Create a table with all AnnData arguments
-    :param adata:
-    :param atlas_name:
-    :param atlas_path:
-    :return:
+    Create an html table with all AnnData arguments
+    The html code will make all elements of the table visible in MultiQC
+    Args:
+        adata (AnnData): atlas to analyse
+        atlas_info (dict): info on the atlas
+        args (argparse.Namespace): list of arguments from checkatlas workflow
     """
-    atlas_name = atlas_info[0]
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
+
     logger.debug(f"Create Adata table for {atlas_name}")
-    csv_path = os.path.join(
-        folders.get_folder(args.path, folders.ANNDATA),
-        atlas_name + checkatlas.ADATA_EXTENSION,
+    csv_path = files.get_file_path(
+        atlas_name, folders.ANNDATA, checkatlas.ADATA_EXTENSION, args.path
     )
     # Create AnnData table
     header = ["obs", "obsm", "var", "varm", "uns"]
     df_summary = pd.DataFrame(index=[atlas_name], columns=header)
     # html_element = "<span class=\"label label-primary\">"
     # new_line = ''
     # for value in list(adata.obs.columns):
@@ -336,29 +373,30 @@
     )
     df_summary["uns"][atlas_name] = (
         "<code>" + "</code><br><code>".join(list(adata.uns_keys())) + "</code>"
     )
     df_summary.to_csv(csv_path, index=False, quoting=False, sep="\t")
 
 
-def create_qc_tables(adata, atlas_path, atlas_info, args) -> None:
+def create_qc_tables(
+    adata: AnnData, atlas_info: dict, args: argparse.Namespace
+) -> None:
     """
-    Display the atlas QC
+    Display the atlas QC table
     Search for the OBS variable which correspond to the toal_RNA, total_UMI,
      MT_ratio, RT_ratio
-    :param path:
-    :param adata:
-    :param atlas_name:
-    :param atlas_path:
-    :return:
-    """
-    atlas_name = atlas_info[0]
-    qc_path = os.path.join(
-        folders.get_folder(args.path, folders.QC),
-        atlas_name + checkatlas.QC_EXTENSION,
+
+    Args:
+        adata (AnnData): atlas to analyse
+        atlas_info (dict): info on the atlas
+        args (argparse.Namespace): list of arguments from checkatlas workflow
+    """
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
+    qc_path = files.get_file_path(
+        atlas_name, folders.QC, checkatlas.QC_EXTENSION, args.path
     )
     logger.debug(f"Create QC tables for {atlas_name}")
     qc_genes = []
     # mitochondrial genes
     adata.var["mt"] = adata.var_names.str.startswith("MT-")
     if len(adata.var[adata.var["mt"]]) != 0:
         qc_genes.append("mt")
@@ -390,26 +428,28 @@
 
     # Sample QC table when more cells than args.plot_celllimit are present
     df_annot = atlas_sampling(df_annot, "QC", args)
     df_annot.loc[:, [CELLINDEX_HEADER]] = range(1, len(df_annot) + 1)
     df_annot.to_csv(qc_path, index=False, quoting=False, sep="\t")
 
 
-def create_qc_plots(adata, atlas_path, atlas_info, args) -> None:
+def create_qc_plots(
+    adata: AnnData, atlas_info: dict, args: argparse.Namespace
+) -> None:
     """
-    Display the atlas QC
+    Display the atlas QC plot
     Search for the OBS variable which correspond to the toal_RNA, total_UMI,
      MT_ratio, RT_ratio
-    :param path:
-    :param adata:
-    :param atlas_name:
-    :param atlas_path:
-    :return:
+
+    Args:
+        adata (AnnData): atlas to analyse
+        atlas_info (dict): info on the atlas
+        args (argparse.Namespace): list of arguments from checkatlas workflow
     """
-    atlas_name = atlas_info[0]
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     sc.settings.figdir = folders.get_workingdir(args.path)
     sc.set_figure_params(dpi_save=80)
     qc_path = os.sep + atlas_name + checkatlas.QC_FIG_EXTENSION
     logger.debug(f"Create QC violin plot for {atlas_name}")
     # mitochondrial genes
     adata.var["mt"] = adata.var_names.str.startswith("MT-")
     # ribosomal genes
@@ -432,25 +472,27 @@
         jitter=0.4,
         multi_panel=True,
         show=False,
         save=qc_path,
     )
 
 
-def create_umap_fig(adata, atlas_path, atlas_info, args) -> None:
+def create_umap_fig(
+    adata: AnnData, atlas_info: dict, args: argparse.Namespace
+) -> None:
     """
     Display the UMAP of celltypes
     Search for the OBS variable which correspond to the celltype annotation
-    :param path:
-    :param adata:
-    :param atlas_name:
-    :param atlas_path:
-    :return:
+
+    Args:
+        adata (AnnData): atlas to analyse
+        atlas_info (dict): info on the atlas
+        args (argparse.Namespace): list of arguments from checkatlas workflow
     """
-    atlas_name = atlas_info[0]
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     sc.set_figure_params(dpi_save=150)
     # Search if umap reduction exists
     obsm_keys = get_viable_obsm(adata, args)
     r = re.compile(".*umap*.")
     obsm_umap_keys = list(filter(r.match, obsm_keys))
     if len(obsm_umap_keys) > 0:
         obsm_umap = obsm_umap_keys[0]
@@ -470,25 +512,27 @@
         obs_keys = get_viable_obs_annot(adata, args)
         if len(obs_keys) != 0:
             sc.pl.umap(adata, color=obs_keys[0], show=False, save=umap_path)
         else:
             sc.pl.umap(adata, show=False, save=umap_path)
 
 
-def create_tsne_fig(adata, atlas_path, atlas_info, args) -> None:
+def create_tsne_fig(
+    adata: AnnData, atlas_info: dict, args: argparse.Namespace
+) -> None:
     """
     Display the TSNE of celltypes
     Search for the OBS variable which correspond to the celltype annotation
-    :param path:
-    :param adata:
-    :param atlas_name:
-    :param atlas_path:
-    :return:
+
+    Args:
+        adata (AnnData): atlas to analyse
+        atlas_info (dict): info on the atlas
+        args (argparse.Namespace): list of arguments from checkatlas workflow
     """
-    atlas_name = atlas_info[0]
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     sc.set_figure_params(dpi_save=150)
     # Search if tsne reduction exists
     obsm_keys = get_viable_obsm(adata, args)
     r = re.compile(".*tsne*.")
     obsm_tsne_keys = list(filter(r.match, obsm_keys))
     if len(obsm_tsne_keys) > 0:
         obsm_tsne = obsm_tsne_keys[0]
@@ -510,32 +554,37 @@
         obs_keys = get_viable_obs_annot(adata, args)
         if len(obs_keys) != 0:
             sc.pl.tsne(adata, color=obs_keys[0], show=False, save=tsne_path)
         else:
             sc.pl.tsne(adata, show=False, save=tsne_path)
 
 
-def metric_cluster(adata, atlas_path, atlas_info, args) -> None:
+def create_metric_cluster(
+    adata: AnnData, atlas_info: dict, args: argparse.Namespace
+) -> None:
     """
     Calc clustering metrics
-    :param adata:
-    :param atlas_path:
-    :param atlas_info:
-    :param args:
-    :return:
-    """
-    atlas_name = atlas_info[0]
-    csv_path = os.path.join(
-        folders.get_folder(args.path, folders.CLUSTER),
-        atlas_name + checkatlas.METRIC_CLUSTER_EXTENSION,
+
+    Args:
+        adata (AnnData): atlas to analyse
+        atlas_info (dict): path of the atlas
+        args (argparse.Namespace): list of arguments from checkatlas workflow
+    """
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
+    csv_path = files.get_file_path(
+        atlas_name,
+        folders.CLUSTER,
+        checkatlas.METRIC_CLUSTER_EXTENSION,
+        args.path,
     )
     header = ["Sample", "obs"] + args.metric_cluster
     df_cluster = pd.DataFrame(columns=header)
     obs_keys = get_viable_obs_annot(adata, args)
     obsm_key_representation = "X_umap"
+
     if len(obs_keys) > 0:
         logger.debug(f"Calc clustering metrics for {atlas_name}")
         for obs_key in obs_keys:
             dict_line = {
                 "Sample": [atlas_name + "_" + obs_key],
                 "obs": [obs_key],
             }
@@ -553,27 +602,31 @@
                 [df_cluster, df_line], ignore_index=True, axis=0
             )
         df_cluster.to_csv(csv_path, index=False, sep="\t")
     else:
         logger.debug(f"No viable obs_key was found for {atlas_name}")
 
 
-def metric_annot(adata, atlas_path, atlas_info, args) -> None:
+def create_metric_annot(
+    adata: AnnData, atlas_info: dict, args: argparse.Namespace
+) -> None:
     """
     Calc annotation metrics
-    :param adata:
-    :param atlas_path:
-    :param atlas_info:
-    :param args:
-    :return:
-    """
-    atlas_name = atlas_info[0]
-    csv_path = os.path.join(
-        folders.get_folder(args.path, folders.ANNOTATION),
-        atlas_name + checkatlas.METRIC_ANNOTATION_EXTENSION,
+
+    Args:
+        adata (AnnData): atlas to analyse
+        atlas_path (dict): path of the atlas
+        args (argparse.Namespace): list of arguments from checkatlas workflow
+    """
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
+    csv_path = files.get_file_path(
+        atlas_name,
+        folders.ANNOTATION,
+        checkatlas.METRIC_ANNOTATION_EXTENSION,
+        args.path,
     )
     header = ["Sample", "Reference", "obs"] + args.metric_annot
     df_annot = pd.DataFrame(columns=header)
     obs_keys = get_viable_obs_annot(adata, args)
     if len(obs_keys) > 1:
         logger.debug(f"Calc annotation metrics for {atlas_name}")
         ref_obs = obs_keys[0]
@@ -598,27 +651,31 @@
                 [df_annot, df_line], ignore_index=True, axis=0
             )
         df_annot.to_csv(csv_path, index=False, sep="\t")
     else:
         logger.debug(f"No viable obs_key was found for {atlas_name}")
 
 
-def metric_dimred(adata, atlas_path, atlas_info, args) -> None:
+def create_metric_dimred(
+    adata: AnnData, atlas_info: dict, args: argparse.Namespace
+) -> None:
     """
     Calc dimensionality reduction metrics
-    :param adata:
-    :param atlas_path:
-    :param atlas_info:
-    :param args:
-    :return:
-    """
-    atlas_name = atlas_info[0]
-    csv_path = os.path.join(
-        folders.get_folder(args.path, folders.DIMRED),
-        atlas_name + checkatlas.METRIC_DIMRED_EXTENSION,
+
+    Args:
+        adata (AnnData): atlas to analyse
+        atlas_info (dict): path of the atlas
+        args (argparse.Namespace): list of arguments from checkatlas workflow
+    """
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
+    csv_path = files.get_file_path(
+        atlas_name,
+        folders.DIMRED,
+        checkatlas.METRIC_DIMRED_EXTENSION,
+        args.path,
     )
     header = ["Sample", "obsm"] + args.metric_dimred
     df_dimred = pd.DataFrame(columns=header)
     obsm_keys = get_viable_obsm(adata, args)
     if len(obsm_keys) > 0:
         logger.debug(f"Calc dim red metrics for {atlas_name}")
         for obsm_key in obsm_keys:
@@ -639,22 +696,27 @@
                 [df_dimred, df_line], ignore_index=True, axis=0
             )
         df_dimred.to_csv(csv_path, index=False, sep="\t")
     else:
         logger.debug(f"No viable obsm_key was found for {atlas_name}")
 
 
-def atlas_sampling(df_annot, type_df, args):
-    """_summary_
+def atlas_sampling(
+    df_annot: pd.DataFrame, type_df: str, args: argparse.Namespace
+) -> pd.DataFrame:
+    """
+    If args.plot_celllimit != 0 and args.plot_celllimit < len(df_annot)
+    The atlas qC table will be sampled for MultiQC
 
     Args:
-        df_annot (_type_): _description_
-        args (_type_): _description_
+        df_annot (pd.DataFrame): Table to sample
+        type_df (str): type of table
+        args (argparse.Namespace): arguments of checkatlas workflow
 
     Returns:
-        _type_: _description_
+        pd.DataFrame: Sampled QC table
     """
     if args.plot_celllimit != 0 and args.plot_celllimit < len(df_annot):
         logger.debug(f"Sample {type_df} table with {len(df_annot)} cells")
         df_annot = df_annot.sample(args.plot_celllimit)
         logger.debug(f"{type_df} table sampled to {len(df_annot)} cells")
     return df_annot
```

### Comparing `checkatlas-0.2.9/checkatlas/atlas_seurat.py` & `checkatlas-0.3.0/checkatlas/seurat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,44 @@
+import argparse
 import logging
 import os
 import re
+import warnings
 
 import pandas as pd
 import rpy2.robjects as ro
 import rpy2.robjects as robjects
+import rpy2.robjects.packages as rpackages
 from rpy2.rinterface_lib.sexp import NULLType
 from rpy2.robjects import pandas2ri
-from rpy2.robjects.conversion import localconverter
+from rpy2.robjects.methods import RS4
 from rpy2.robjects.packages import importr
-from rpy2.robjects.vectors import FactorVector
+from rpy2.robjects.vectors import FactorVector, StrVector
 
-from . import checkatlas, folders
-from .metrics import metrics
+from checkatlas import atlas, checkatlas
+from checkatlas.metrics import metrics
+from checkatlas.utils import folders
 
 """
 Module for management of Atlas n Seurat format
 
 - Adata and summary tables are created from seuratà
 - QC are created using Seurat
 - UMAP, t-SNE are created using Seurat
 - For creating metrics tables, obs tables are
   first converted from R to python and then
   scikitlearn is used.
 """
 
 logger = logging.getLogger("checkatlas")
+warnings.filterwarnings(action="ignore", message="R[write to console]")
+
+SEURAT_TYPE = "Seurat"
+SEURAT_EXTENSION = ".rds"
+
 
 SCANPY_TO_SEURAT_OBS = {
     "total_counts": "nCount_RNA",
     "n_genes_by_counts": "nFeature_RNA",
     "pct_counts_mt": "percent.mito",
     "pct_counts_ribo": "percent.ribo",
     "violin_plot": "violin_plot",
@@ -39,70 +48,108 @@
     "nCount_RNA": "total_counts",
     "nFeature_RNA": "n_genes_by_counts",
     "percent.mito": "pct_counts_mt",
     "percent.ribo": "pct_counts_ribo",
 }
 
 
-def check_seurat_install():
-    """
-    Check if Seurat is installed, run installation if not
-    :return:
-    """
-    r_script = """install.packages(setdiff(c(\'Seurat\',\'SeuratObject\'),
-                rownames(installed.packages())))"""
-    robjects.r(r_script)
+def detect_seurat(atlas_path: str) -> dict:
+    if atlas_path.endswith(SEURAT_EXTENSION):
+        atlas_info = dict()
+        atlas_info[checkatlas.ATLAS_NAME_KEY] = os.path.splitext(
+            os.path.basename(atlas_path)
+        )[0]
+        atlas_info[checkatlas.ATLAS_TYPE_KEY] = SEURAT_TYPE
+        atlas_info[checkatlas.ATLAS_EXTENSION_KEY] = SEURAT_EXTENSION
+        atlas_info[checkatlas.ATLAS_PATH_KEY] = atlas_path
+        return atlas_info
+    else:
+        return dict()
 
 
-def read_atlas(atlas_path, atlas_info):
-    """
-    Read Seurat object in python using rpy2
-    :param atlas_path:
-    :param atlas_info:
-    :return:
-    """
-    importr("Seurat")
-    importr("SeuratObject")
-    logger.info(f"Load {atlas_info[0]} in {atlas_info[-1]}")
+def check_seurat_install() -> None:
+    """Check if Seurat is installed, run installation if not"""
+    # import R's utility package
+    utils = rpackages.importr("utils")
+    # select a mirror for R packages
+    utils.chooseCRANmirror(ind=1)  # select the first mirror in the list
+    # R package names
+    packnames = ("Seurat", "SeuratObject")
+    # Selectively install what needs to be install.
+    # We are fancy, just because we can.
+    names_to_install = [x for x in packnames if not rpackages.isinstalled(x)]
+    if len(names_to_install) > 0:
+        # create personal library
+        rcode = """dir.create(Sys.getenv("R_LIBS_USER"), recursive = TRUE)"""
+        robjects.r(rcode)
+        # add to the path
+        rcode = """.libPaths(Sys.getenv("R_LIBS_USER"))"""
+        robjects.r(rcode)
+        logger.debug(f"Set Rlibpaths: {robjects.r(rcode)}")
+        utils.install_packages(StrVector(names_to_install))
+
+
+def read_atlas(atlas_info: dict) -> RS4:
+    """Read Seurat object in python using rpy2
+
+    Args:
+        atlas_path (str): _description_
+
+    Returns:
+        RS4: _description_
+    """
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
+    atlas_path = atlas_info[checkatlas.ATLAS_PATH_KEY]
+    logger.info(f"Load {atlas_name} in " f"{atlas_path}")
     rcode = f'readRDS("{atlas_path}")'
     seurat = robjects.r(rcode)
     rclass = robjects.r["class"]
     if rclass(seurat)[0] == "Seurat":
         importr("Seurat")
         return seurat
     else:
-        logger.info(f"{atlas_info[0]} is not a Seurat object")
+        logger.info(f"{atlas_name} is not a Seurat object")
         return None
 
 
-def get_viable_obs_qc(seurat, args):
+def get_viable_obs_qc(seurat: RS4, args: argparse.Namespace) -> list:
     """
     Search in obs_keys a match to OBS_QC values
     Extract sorted obs_keys in same order then OBS_QC
-    :param adata:
-    :return:
+
+    Args:
+        seurat (RS4): _description_
+        args (argparse.Namespace): _description_
+
+    Returns:
+        list: _description_
     """
     r_obs = robjects.r(
         "obs <- function(seurat){ return(colnames(seurat@meta.data))}"
     )
     obs_keys = list()
     for obs_qc in args.qc_display:
         obs_qc = SCANPY_TO_SEURAT_OBS[obs_qc]
         if obs_qc in r_obs(seurat):
             obs_keys.append(obs_qc)
     return obs_keys
 
 
-def get_viable_obs_annot(seurat, args):
+def get_viable_obs_annot(seurat: RS4, args: argparse.Namespace) -> list:
     """
     Search in obs_keys a match to OBS_CLUSTERS values
     ! Remove obs_key with only one category !
     Extract sorted obs_keys in same order then OBS_CLUSTERS
-    :param adata:
-    :return:
+
+    Args:
+        seurat (RS4): _description_
+        args (argparse.Namespace): _description_
+
+    Returns:
+        list: _description_
     """
     obs_keys = list()
     r_obs = robjects.r(
         "obs <- function(seurat){ return(colnames(seurat@meta.data))}"
     )
     obs_key_seurat = r_obs(seurat)
     r_annot = robjects.r(
@@ -138,31 +185,35 @@
     """
     obsm_keys = list()
     # for obsm_key in adata.obsm_keys():
     #   if obsm_key in args.obsm_dimred:
     r_obsm = robjects.r(
         "f<-function(seurat){return(names(seurat@reductions))}"
     )
-    obsm_keys = r_obsm(seurat)
+    obsm_keys_r = r_obsm(seurat)
+    obsm_keys = list()
+    for obsm_key in obsm_keys_r:
+        print(obsm_key)
+        obsm_keys.append(obsm_key)
     logger.debug(f"Add obsm {obsm_keys}")
     return obsm_keys
 
 
-def create_summary_table(seurat, atlas_path, atlas_info, args) -> None:
+def create_summary_table(
+    seurat: RS4, atlas_info: dict, args=argparse.Namespace
+) -> None:
     """
     Create a table with all interesting variables
     :param seurat:
     :param atlas_name:
     :param csv_path:
     :return:
     """
-    atlas_name = atlas_info[0]
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     logger.debug(f"Create Summary table for {atlas_name}")
-    atlas_file_type = atlas_info[1]
-    atlas_extension = atlas_info[2]
     csv_path = os.path.join(
         folders.get_folder(args.path, folders.SUMMARY),
         atlas_name + checkatlas.SUMMARY_EXTENSION,
     )
     # Create summary table
     header = [
         "AtlasFileType",
@@ -176,33 +227,39 @@
     r_nrow = robjects.r["nrow"]
     r_ncol = robjects.r["ncol"]
     ncells = r_ncol(seurat)[0]
     ngenes = r_nrow(seurat)[0]
     x_raw = False
     x_norm = True
     df_summary = pd.DataFrame(index=[atlas_name], columns=header)
-    df_summary["AtlasFileType"][atlas_name] = atlas_file_type
+    df_summary["AtlasFileType"][atlas_name] = atlas_info[
+        checkatlas.ATLAS_TYPE_KEY
+    ]
     df_summary["NbCells"][atlas_name] = ncells
     df_summary["NbGenes"][atlas_name] = ngenes
     df_summary["AnnData.raw"][atlas_name] = x_raw
     df_summary["AnnData.X"][atlas_name] = x_norm
-    df_summary["File_extension"][atlas_name] = atlas_extension
-    df_summary["File_path"][atlas_name] = atlas_path.replace(args.path, "")
+    df_summary["File_extension"][atlas_name] = atlas_info[
+        checkatlas.ATLAS_EXTENSION_KEY
+    ]
+    df_summary["File_path"][atlas_name] = atlas_info[checkatlas.ATLAS_PATH_KEY]
     df_summary.to_csv(csv_path, index=False, sep="\t")
 
 
-def create_anndata_table(seurat, atlas_path, atlas_info, args) -> None:
+def create_anndata_table(
+    seurat: RS4, atlas_info: dict, args=argparse.Namespace
+) -> None:
     """
     Create a table with all AnnData-like arguments in Seurat object
     :param seurat:
     :param atlas_name:
     :param atlas_path:
     :return:
     """
-    atlas_name = atlas_info[0]
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     logger.debug(f"Create Adata table for {atlas_name}")
     csv_path = os.path.join(
         folders.get_folder(args.path, folders.ANNDATA),
         atlas_name + checkatlas.ADATA_EXTENSION,
     )
     # Create AnnData table
     header = ["obs", "obsm", "var", "varm", "uns"]
@@ -214,14 +271,15 @@
     )
     r_obsm = robjects.r(
         "f<-function(seurat){return(names(seurat@reductions))}"
     )
     r_uns = robjects.r(
         "uns <- function(seurat){ return(colnames(seurat@misc))}"
     )
+
     obs_list = r_obs(seurat)
     obsm_list = r_obsm(seurat)
     var_list = [""]
     varm_list = [""]
     uns_list = [""]
     if not isinstance(r_uns(seurat), NULLType):
         uns_list = r_uns(seurat)
@@ -240,57 +298,72 @@
     )
     df_summary["uns"][atlas_name] = (
         "<code>" + "</code><br><code>".join(uns_list) + "</code>"
     )
     df_summary.to_csv(csv_path, index=False, quoting=False, sep="\t")
 
 
-def create_qc_tables(seurat, atlas_path, atlas_info, args) -> None:
+def create_qc_tables(
+    seurat: RS4, atlas_info: dict, args=argparse.Namespace
+) -> None:
     """
     Display the atlas QC of seurat
     Search for the metadata variable which correspond
     to the total_RNA, total_UMI, MT_ratio, RT_ratio
     :param path:
     :param adata:
     :param atlas_name:
     :param atlas_path:
     :return:
     """
-    atlas_name = atlas_info[0]
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     qc_path = os.path.join(
         folders.get_folder(args.path, folders.QC),
         atlas_name + checkatlas.QC_EXTENSION,
     )
     logger.debug(f"Create QC tables for {atlas_name}")
     obs_keys = get_viable_obs_qc(seurat, args)
     r_meta = robjects.r("obs <- function(seurat){ return(seurat@meta.data)}")
     r_metadata = r_meta(seurat)
-    with localconverter(ro.default_converter + pandas2ri.converter):
-        df_metadata = ro.conversion.rpy2py(r_metadata)
+    with (ro.default_converter + pandas2ri.converter).context():
+        df_metadata = ro.conversion.get_conversion().rpy2py(r_metadata)
         df_annot = df_metadata[obs_keys]
         # rename columns with scanpy names
         new_columns = list()
         for column in df_annot.columns:
             new_columns.append(SEURAT_TO_SCANPY_OBS[column])
         df_annot.columns = new_columns
+
+        # Rank cell by qc metric
+        for header in df_annot.columns:
+            if header != atlas.CELLINDEX_HEADER:
+                new_header = f"cellrank_{header}"
+                df_annot = df_annot.sort_values(header, ascending=False)
+                df_annot.loc[:, [new_header]] = range(1, len(df_annot) + 1)
+
+        # Sample QC table when more cells than args.plot_celllimit are present
+        df_annot = atlas.atlas_sampling(df_annot, "QC", args)
+        df_annot.loc[:, [atlas.CELLINDEX_HEADER]] = range(1, len(df_annot) + 1)
         df_annot.to_csv(qc_path, index=False, quoting=False, sep="\t")
 
 
-def create_qc_plots(seurat, atlas_path, atlas_info, args) -> None:
+def create_qc_plots(
+    seurat: RS4, atlas_info: dict, args=argparse.Namespace
+) -> None:
     """
     Display the atlas QC
     Search for the OBS variable which correspond to the toal_RNA, total_UMI,
      MT_ratio, RT_ratio
     :param path:
     :param adata:
     :param atlas_name:
     :param atlas_path:
     :return:
     """
-    atlas_name = atlas_info[0]
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     qc_path = os.path.join(
         folders.get_folder(args.path, folders.QC_FIG),
         atlas_name + checkatlas.QC_FIG_EXTENSION,
     )
     logger.debug(f"Create QC violin plot for {atlas_name}")
     importr("ggplot2")
     r_cmd = (
@@ -301,25 +374,27 @@
     )
     r_violin = robjects.r(r_cmd)
     obs_keys = list(SEURAT_TO_SCANPY_OBS.keys())
     r_obs = robjects.StrVector(obs_keys)
     r_violin(seurat, r_obs, qc_path)
 
 
-def create_umap_fig(seurat, atlas_path, atlas_info, args) -> None:
+def create_umap_fig(
+    seurat: RS4, atlas_info: dict, args=argparse.Namespace
+) -> None:
     """
     Display the UMAP of celltypes
     Search for the OBS variable which correspond to the celltype annotation
     :param path:
     :param adata:
     :param atlas_name:
     :param atlas_path:
     :return:
     """
-    atlas_name = atlas_info[0]
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     # Search if tsne reduction exists
     r = re.compile(".*umap*.")
     r_names = robjects.r["names"]
     obsm_list = r_names(seurat)
     importr("ggplot2")
     if len(list(filter(r.match, obsm_list))) > 0:
         logger.debug(f"Create UMAP figure for {atlas_name}")
@@ -337,25 +412,27 @@
             "ggsave(umap_path, umap_plot, width = 10, "
             "height = 6, dpi = 76)}"
         )
         r_umap = robjects.r(r_cmd)
         r_umap(seurat, obs_keys[0], umap_path)
 
 
-def create_tsne_fig(seurat, atlas_path, atlas_info, args) -> None:
+def create_tsne_fig(
+    seurat: RS4, atlas_info: dict, args=argparse.Namespace
+) -> None:
     """
     Display the TSNE of celltypes
     Search for the OBS variable which correspond to the celltype annotation
     :param path:
     :param adata:
     :param atlas_name:
     :param atlas_path:
     :return:
     """
-    atlas_name = atlas_info[0]
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     # Search if tsne reduction exists
     r = re.compile(".*tsne*.")
     r_names = robjects.r["names"]
     obsm_list = r_names(seurat)
     importr("ggplot2")
     if len(list(filter(r.match, obsm_list))) > 0:
         logger.debug(f"Create t-SNE figure for {atlas_name}")
@@ -373,24 +450,26 @@
             "ggsave(tsne_path, tsne_plot, width = 10, "
             "height = 6, dpi = 76)}"
         )
         r_tsne = robjects.r(r_cmd)
         r_tsne(seurat, obs_keys[0], tsne_path)
 
 
-def metric_cluster(seurat, atlas_path, atlas_info, args) -> None:
+def create_metric_cluster(
+    seurat: RS4, atlas_info: dict, args=argparse.Namespace
+) -> None:
     """
     Calc clustering metrics
     :param seurat:
     :param atlas_path:
     :param atlas_info:
     :param args:
     :return:
     """
-    atlas_name = atlas_info[0]
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     csv_path = os.path.join(
         folders.get_folder(args.path, folders.CLUSTER),
         atlas_name + checkatlas.METRIC_CLUSTER_EXTENSION,
     )
     header = ["Sample", "obs"] + args.metric_cluster
     df_cluster = pd.DataFrame(columns=header)
     obs_keys = get_viable_obs_annot(seurat, args)
@@ -416,24 +495,26 @@
                 [df_cluster, df_line], ignore_index=True, axis=0
             )
         df_cluster.to_csv(csv_path, index=False, sep="\t")
     else:
         logger.debug(f"No viable obs_key was found for {atlas_name}")
 
 
-def metric_annot(seurat, atlas_path, atlas_info, args) -> None:
+def create_metric_annot(
+    seurat: RS4, atlas_info: dict, args=argparse.Namespace
+) -> None:
     """
     Calc annotation metrics
     :param adata:
     :param atlas_path:
     :param atlas_info:
     :param args:
     :return:
     """
-    atlas_name = atlas_info[0]
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     csv_path = os.path.join(
         folders.get_folder(args.path, folders.ANNOTATION),
         atlas_name + checkatlas.METRIC_ANNOTATION_EXTENSION,
     )
     header = ["Sample", "Reference", "obs"] + args.metric_annot
     df_annot = pd.DataFrame(columns=header)
     obs_keys = get_viable_obs_annot(seurat, args)
@@ -462,24 +543,26 @@
                     [df_annot, df_line], ignore_index=True, axis=0
                 )
             df_annot.to_csv(csv_path, index=False, sep="\t")
     else:
         logger.debug(f"No viable obs_key was found for {atlas_name}")
 
 
-def metric_dimred(seurat, atlas_path, atlas_info, args) -> None:
+def create_metric_dimred(
+    seurat: RS4, atlas_info: dict, args=argparse.Namespace
+) -> None:
     """
     Calc dimensionality reduction metrics
     :param adata:
     :param atlas_path:
     :param atlas_info:
     :param args:
     :return:
     """
-    atlas_name = atlas_info[0]
+    atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     csv_path = os.path.join(
         folders.get_folder(args.path, folders.DIMRED),
         atlas_name + checkatlas.METRIC_DIMRED_EXTENSION,
     )
     header = ["Sample", "obsm"] + args.metric_dimred
     df_dimred = pd.DataFrame(columns=header)
     # r_reduction = robjects.r(
```

### Comparing `checkatlas-0.2.9/checkatlas/folders.py` & `checkatlas-0.3.0/checkatlas/utils/folders.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 
-working_dir = "checkatlas_files"
+WORKING_DIR = "checkatlas_files"
 SUMMARY = "summary"
 ANNDATA = "adata"
 QC = "qc"
 QC_FIG = "violin"
 UMAP = "umap"
 TSNE = "tsne"
 CLUSTER = "cluster"
@@ -29,50 +29,51 @@
     TEMP: TEMP,
     NEXTFLOW: NEXTFLOW,
 }
 
 logger = logging.getLogger("checkatlas")
 
 
-def get_workingdir(path):
-    """
-    Return the working_dir = path of search
+def get_workingdir(path: str) -> str:
+    """Return the working_dir = path of search
     + working_dir
     with working_dir = checkatlas_files/
+
     Args:
-        path: Search path for atlas given by user
+        path (str): Search path for atlas given by user
+
     Returns:
         str: os.path.join(path, working_dir)
     """
-    return os.path.join(path, working_dir)
+    return os.path.join(path, WORKING_DIR)
 
 
-def get_folder(path, key_folder):
-    """
-    Get the folder path giving the search path and
+def get_folder(path: str, key_folder: str) -> str:
+    """Get the folder path giving the search path and
     the folder key in DICT_FOLDER
+
     Args:
-        path: Search path for atlas given by user
-        key_folder: key folder in the DICT_FOLDER
+        path (str): Search path for atlas given by user
+        key_folder (str): key folder in the DICT_FOLDER
             example: ANNDATA, SUMMARY, UMAP
 
     Returns:
         str: the folder path
-
     """
     return os.path.join(get_workingdir(path), DICT_FOLDER[key_folder])
 
 
-def checkatlas_folders(path):
-    """
-    Check in path if the different checkatlas folders exists.<br>
+def checkatlas_folders(path: str) -> None:
+    """Check in path if the different checkatlas folders exists.<br>
     Create them if needed.
     All folders are given by DICT_FOLDER
+
     Args:
-        path: Search path for atlas given by user
+        path (str): Search path for atlas given by user
+
     Returns:
         None: None
     """
     global_path = get_workingdir(path)
     if not os.path.exists(global_path):
         os.mkdir(global_path)
```

### Comparing `checkatlas-0.2.9/checkatlas/metrics/dimred/kruskal_stress.py` & `checkatlas-0.3.0/checkatlas/metrics/dimred/kruskal_stress.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.9/checkatlas/metrics/metrics.py` & `checkatlas-0.3.0/checkatlas/metrics/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,17 +81,17 @@
 
 
 def calc_metric_annot_seurat(metric, seurat, obs_key, ref_obs):
     if metric in METRICS_ANNOT:
         metric_module = getattr(annot, metric)
         annotation = ro.conversion.rpy2py(R_ANNOT(seurat, obs_key))
         ref_annotation = ro.conversion.rpy2py(R_ANNOT(seurat, ref_obs))
-        annotation, ref_annotation = annotation_to_num(
-            annotation, ref_annotation
-        )
+        # annotation, ref_annotation = annotation_to_num(
+        #    annotation, ref_annotation
+        # )
         return metric_module.run(annotation, ref_annotation)
     else:
         logger.warning(
             f"{metric} is not a recognized annotation metric."
             f"\nList of annotation metrics: {METRICS_ANNOT}"
         )
         return -1
```

### Comparing `checkatlas-0.2.9/checkatlas/metrics/specificity/analysis.py` & `checkatlas-0.3.0/checkatlas/metrics/specificity/analysis.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.9/checkatlas/metrics/specificity/compute.py` & `checkatlas-0.3.0/checkatlas/metrics/specificity/compute.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.9/checkatlas/metrics/specificity/get_data.py` & `checkatlas-0.3.0/checkatlas/metrics/specificity/get_data.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.9/checkatlas/metrics/specificity/plot.py` & `checkatlas-0.3.0/checkatlas/metrics/specificity/plot.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.2.9/pyproject.toml` & `checkatlas-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkatlas"
-version = "0.2.9"
+version = "0.3.0"
 description="One liner tool to check the quality of your single-cell atlases."
 authors = ["becavin-lab"]
 readme = "README.md"
 license = "BSD 3-Clause"
 packages = [{include = "checkatlas"}]
 include = ["checkatlas/checkatlas_workflow.nf"]
 exclude = ["tests/", ".github", "*dask-worker-space*"]
@@ -12,21 +12,21 @@
 repository = "https://github.com/becavin-lab/checkatlas/"
 documentation = "https://checkatlas.readthedocs.io/"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 scikit-learn = "^1.2.1"
-rpy2 = "^3.5.8"
 llvmlite = "^0.39.1"
 numba = "^0.56.4"
 types-pyyaml = "^6.0.12.6"
 scanpy = "^1.9.1"
 numpy = "^1.23.5"
 poetry = "^1.5.1"
+rpy2 = "3.5.10"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "^67.3.2"
 gitchangelog = "^3.0.4"
@@ -34,14 +34,15 @@
 flake8 = "^6.0.0"
 codecov = "^2.1.12"
 pytest-cov = "^4.0.0"
 isort = "^5.12.0"
 mypy = "^1.0.0"
 jupyter-black = "^0.3.3"
 no-implicit-optional = "^1.3"
+leidenalg = "^0.10.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocstrings-python-legacy = "^0.2.3"
@@ -49,7 +50,9 @@
 [tool.mypy]
 no_implicit_optional = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.poetry.scripts]
+checkatlas = 'checkatlas.__main__:main'
```

### Comparing `checkatlas-0.2.9/setup.py` & `checkatlas-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,40 +3,45 @@
 
 packages = \
 ['checkatlas',
  'checkatlas.metrics',
  'checkatlas.metrics.annot',
  'checkatlas.metrics.cluster',
  'checkatlas.metrics.dimred',
- 'checkatlas.metrics.specificity']
+ 'checkatlas.metrics.specificity',
+ 'checkatlas.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['llvmlite>=0.39.1,<0.40.0',
  'numba>=0.56.4,<0.57.0',
  'numpy>=1.23.5,<2.0.0',
  'poetry>=1.5.1,<2.0.0',
- 'rpy2>=3.5.8,<4.0.0',
+ 'rpy2==3.5.10',
  'scanpy>=1.9.1,<2.0.0',
  'scikit-learn>=1.2.1,<2.0.0',
  'types-pyyaml>=6.0.12.6,<7.0.0.0']
 
+entry_points = \
+{'console_scripts': ['checkatlas = checkatlas.__main__:main']}
+
 setup_kwargs = {
     'name': 'checkatlas',
-    'version': '0.2.9',
+    'version': '0.3.0',
     'description': 'One liner tool to check the quality of your single-cell atlases.',
-    'long_description': "# ![CheckAtlas](docs/images/checkatlas_logo.png) \n\n\n![PyPI](https://img.shields.io/pypi/v/checkatlas)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/checkatlas)\n![PyPI - License](https://img.shields.io/pypi/l/checkatlas)\n![Conda](https://img.shields.io/conda/pn/bioconda/checkatlas)\n\n[![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)\n[![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)\n[![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)\n\nCheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the\nquality control tables and figures which can be then processed by multiqc. CheckAtlas is able to load Scanpy, Seurat,\nand CellRanger files.\n\n\n## Summary\n\n### Parse Scanpy, Seurat and CellRanger objects\n\nThe checkatlas pipeline start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.\n\n\n### Create checkatlas summary files\n\nGo through all atlas files and produce summary information:\n\n- All basic QC (nRNA, nFeature, ratio_mito)\n- General information (nbcells, nbgenes, nblayers)\n- All elements in atlas files (obs, obsm, uns, var, varm)\n- Reductions (pca, umap, tsne)\n- All metrics (clustering, annotation, dimreduction, specificity)\n\n### Parse checkatlas files in MultiQC\n\n   Update MultiQC project to add checkatlas parsing. Dev project in: https://github.com/becavin-lab/MultiQC/tree/checkatlas\n\nhttps://checkatlas.readthedocs.io/en/latest/\n\n## Examples\n\n1. Evaluate and compare different atlases: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Atlas_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_1/CheckAtlas_example_1.html\n\n2. Evaluate different version of your atlas: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Version_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_2/CheckAtlas_example_2.html\n\n3. Explore Scanpy, Seurat and CellRanger objects in your folder: https://github.com/becavin-lab/checkatlas/blob/main/examples/AtlasType_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_3/CheckAtlas_example_3.html\n\n## Installation\n\nCheckAtlas can be downloaded from PyPI. However, the project is in an early development phase. We strongly recommend to use the developmental version.\n\n### Install checkatlas development version\n\n```bash\ngit clone git@github.com:becavin-lab/checkatlas.git\npip install checkatlas/.\n```\n\nInstall MultiQC with checkatlas file management. This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.\n\n```bash\ngit clone git@github.com:becavin-lab/MultiQC.git\ncd MultiQC/\ngit checkout checkatlas\npip install .\n```\n\n### Install it from PyPI\n\n```bash\npip install checkatlas\n```\n\n### Install Seurat\n\nTo be able to manage seurat file, rpy2 should have Seurat installed. The easiest way is to put all checkatlas requirements in a conda environment and add r-seurat.\n\n```bash\nconda create -n checkatlas python=3.9\npip install checkatlas\nconda install -c bioconda r-seurat\n```\n\nOr, open R in checkatlas environment (the one where you ran 'pip install') and install Seurat.\n\n```bash\n% R\n> install.packages('Seurat')\n> library(Seurat)\n```\n\n\n## Usage\n\nThe one liner way to run checkatlas is the following: \n\n```bash\n$ cd your_search_folder/\n$ python -m checkatlas .\n#or\n$ checkatlas .\n```\n\nOr run it inside your python workflow.\n\n```py\nfrom checkatlas import checkatlas\ncheckatlas.run(path, atlas_list, multithread, n_cpus)\n```\n\n\n## Development\n\nRead the [CONTRIBUTING.md](docs/contributing.md) file.\n\nProject developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)\n\n",
+    'long_description': "# ![CheckAtlas](docs/images/checkatlas_logo.png) \n\n\n![PyPI](https://img.shields.io/pypi/v/checkatlas)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/checkatlas)\n![PyPI - License](https://img.shields.io/pypi/l/checkatlas)\n![Conda](https://img.shields.io/conda/pn/bioconda/checkatlas)\n\n[![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)\n[![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)\n[![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)\n\n![Static Badge](https://img.shields.io/badge/Packaging-Poetry-blue)\n![Static Badge](https://img.shields.io/badge/Docs-Mkdocs-red)\n![Static Badge](https://img.shields.io/badge/Linting-flake8%20black%20mypy-yellow)\n\nCheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the\nquality control tables and figures which can be then processed by multiqc. CheckAtlas is able to load Scanpy, Seurat,\nand CellRanger files.\n\n\n## Summary\n\n### Parse Scanpy, Seurat and CellRanger objects\n\nThe checkatlas pipeline start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.\n\n\n### Create checkatlas summary files\n\nGo through all atlas files and produce summary information:\n\n- All basic QC (nRNA, nFeature, ratio_mito)\n- General information (nbcells, nbgenes, nblayers)\n- All elements in atlas files (obs, obsm, uns, var, varm)\n- Reductions (pca, umap, tsne)\n- All metrics (clustering, annotation, dimreduction, specificity)\n\n### Parse checkatlas files in MultiQC\n\n   Update MultiQC project to add checkatlas parsing. Dev project in: https://github.com/becavin-lab/MultiQC/tree/checkatlas\n\nhttps://checkatlas.readthedocs.io/en/latest/\n\n## Examples\n\n1. Evaluate and compare different atlases: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Atlas_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_1/CheckAtlas_example_1.html\n\n2. Evaluate different version of your atlas: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Version_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_2/CheckAtlas_example_2.html\n\n3. Explore Scanpy, Seurat and CellRanger objects in your folder: https://github.com/becavin-lab/checkatlas/blob/main/examples/AtlasType_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_3/CheckAtlas_example_3.html\n\n## Installation\n\nCheckAtlas can be downloaded from PyPI. However, the project is in an early development phase. We strongly recommend to use the developmental version.\n\n### Install checkatlas development version\n\n```bash\ngit clone git@github.com:becavin-lab/checkatlas.git\npip install checkatlas/.\n```\n\nInstall MultiQC with checkatlas file management. This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.\n\n```bash\ngit clone git@github.com:becavin-lab/MultiQC.git\ncd MultiQC/\ngit checkout checkatlas\npip install .\n```\n\n### Install it from PyPI\n\n```bash\npip install checkatlas\n```\n\n### Install Seurat\n\nTo be able to manage seurat file, rpy2 should have Seurat installed. The easiest way is to put all checkatlas requirements in a conda environment and add r-seurat.\n\n```bash\nconda create -n checkatlas python=3.9\npip install checkatlas\nconda install -c bioconda r-seurat\n```\n\nOr, open R in checkatlas environment (the one where you ran 'pip install') and install Seurat.\n\n```bash\n% R\n> install.packages('Seurat')\n> library(Seurat)\n```\n\n\n## Usage\n\nThe one liner way to run checkatlas is the following: \n\n```bash\n$ cd your_search_folder/\n$ python -m checkatlas .\n#or\n$ checkatlas .\n```\n\nOr run it inside your python workflow.\n\n```py\nfrom checkatlas import checkatlas\ncheckatlas.run(path, atlas_list, multithread, n_cpus)\n```\n\n\n## Development\n\nRead the [CONTRIBUTING.md](docs/contributing.md) file.\n\nProject developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)\n\n",
     'author': 'becavin-lab',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://checkatlas.readthedocs.io/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `checkatlas-0.2.9/PKG-INFO` & `checkatlas-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: checkatlas
-Version: 0.2.9
+Version: 0.3.0
 Summary: One liner tool to check the quality of your single-cell atlases.
 Home-page: https://checkatlas.readthedocs.io/
 License: BSD 3-Clause
 Author: becavin-lab
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: llvmlite (>=0.39.1,<0.40.0)
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: poetry (>=1.5.1,<2.0.0)
-Requires-Dist: rpy2 (>=3.5.8,<4.0.0)
+Requires-Dist: rpy2 (==3.5.10)
 Requires-Dist: scanpy (>=1.9.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
 Requires-Dist: types-pyyaml (>=6.0.12.6,<7.0.0.0)
 Project-URL: Documentation, https://checkatlas.readthedocs.io/
 Project-URL: Repository, https://github.com/becavin-lab/checkatlas/
 Description-Content-Type: text/markdown
 
@@ -31,14 +31,18 @@
 ![Conda](https://img.shields.io/conda/pn/bioconda/checkatlas)
 
 [![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)
 [![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)
 [![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)
 
+![Static Badge](https://img.shields.io/badge/Packaging-Poetry-blue)
+![Static Badge](https://img.shields.io/badge/Docs-Mkdocs-red)
+![Static Badge](https://img.shields.io/badge/Linting-flake8%20black%20mypy-yellow)
+
 CheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the
 quality control tables and figures which can be then processed by multiqc. CheckAtlas is able to load Scanpy, Seurat,
 and CellRanger files.
 
 
 ## Summary
```

