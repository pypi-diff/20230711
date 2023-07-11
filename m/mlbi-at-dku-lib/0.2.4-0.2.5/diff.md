# Comparing `tmp/mlbi_at_dku_lib-0.2.4.tar.gz` & `tmp/mlbi_at_dku_lib-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.2.4.tar", last modified: Tue Jul 11 09:25:56 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.2.5.tar", last modified: Tue Jul 11 10:40:10 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.2.4.tar` & `mlbi_at_dku_lib-0.2.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 09:25:56.848965 mlbi_at_dku_lib-0.2.4/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.4/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      102 2023-07-02 06:59:42.000000 mlbi_at_dku_lib-0.2.4/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-11 09:25:56.844965 mlbi_at_dku_lib-0.2.4/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.4/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      827 2023-07-11 09:25:34.000000 mlbi_at_dku_lib-0.2.4/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-11 09:25:56.848965 mlbi_at_dku_lib-0.2.4/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-02 05:17:52.000000 mlbi_at_dku_lib-0.2.4/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 09:25:56.784966 mlbi_at_dku_lib-0.2.4/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 09:25:56.784966 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 09:25:56.832965 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/data/
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/data/GTmap_hg19.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/data/GTmap_hg38.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/data/GTmap_mm10.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     5206 2023-07-11 04:59:49.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     6033 2023-07-11 04:52:53.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    36548 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    40645 2023-07-11 04:48:23.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 09:25:56.784966 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-11 09:25:56.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      633 2023-07-11 09:25:56.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-11 09:25:56.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-11 09:25:56.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-11 09:25:56.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       16 2023-07-11 09:25:56.000000 mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 10:40:10.772814 mlbi_at_dku_lib-0.2.5/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.5/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      102 2023-07-02 06:59:42.000000 mlbi_at_dku_lib-0.2.5/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-11 10:40:10.772814 mlbi_at_dku_lib-0.2.5/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.5/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      827 2023-07-11 10:39:56.000000 mlbi_at_dku_lib-0.2.5/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-11 10:40:10.772814 mlbi_at_dku_lib-0.2.5/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-02 05:17:52.000000 mlbi_at_dku_lib-0.2.5/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 10:40:10.708816 mlbi_at_dku_lib-0.2.5/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 10:40:10.712816 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 10:40:10.760815 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/data/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/data/GTmap_hg19.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/data/GTmap_hg38.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/data/GTmap_mm10.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     5206 2023-07-11 04:59:49.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     6033 2023-07-11 04:52:53.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    36550 2023-07-11 10:36:34.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    40645 2023-07-11 04:48:23.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 10:40:10.712816 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-11 10:40:10.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      633 2023-07-11 10:40:10.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-11 10:40:10.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-11 10:40:10.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-11 10:40:10.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       16 2023-07-11 10:40:10.000000 mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/top_level.txt
```

### Comparing `mlbi_at_dku_lib-0.2.4/LICENSE` & `mlbi_at_dku_lib-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.4/PKG-INFO` & `mlbi_at_dku_lib-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi_at_dku_lib
-Version: 0.2.4
+Version: 0.2.5
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `mlbi_at_dku_lib-0.2.4/pyproject.toml` & `mlbi_at_dku_lib-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlbi_at_dku_lib"
-version = "0.2.4"
+version = "0.2.5"
 description = "Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/cpdb.py` & `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/cpdb.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/data/GTmap_hg19.csv` & `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/data/GTmap_hg19.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/data/GTmap_hg38.csv` & `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/data/GTmap_hg38.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/data/GTmap_mm10.csv` & `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/data/GTmap_mm10.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/deg.py` & `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/deg.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/deiso.py` & `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/deiso.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/icnv.py`

 * *Files 0% similar despite different names*

```diff
@@ -912,15 +912,15 @@
         warnings.simplefilter("ignore")
     
         ## Normalize and log-transform
         sc.pp.normalize_total(adata, target_sum=1e4)
         sc.pp.log1p(adata)
 
         sc.pp.highly_variable_genes(adata, n_top_genes = 2000) # , flavor = 'seurat_v3')
-        sc.tl.score_genes_cell_cycle(adata, cell_cycle_genes_s, cell_cycle_genes_g2m)
+        # sc.tl.score_genes_cell_cycle(adata, cell_cycle_genes_s, cell_cycle_genes_g2m)
 
         cnv.io.genomic_position_from_gtf(gtf_file, adata, gtf_gene_id='gene_name', adata_gene_id=None, inplace=True)
         cnv.tl.infercnv(adata, reference_key = ref_key, reference_cat=ref_types, window_size=100)
 
         if pca_umap:
             print('PCA .. ', end = '')
             cnv.tl.pca(adata, svd_solver='arpack', n_comps = N_pca)
```

### Comparing `mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib/misc.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib.egg-info/PKG-INFO` & `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi-at-dku-lib
-Version: 0.2.4
+Version: 0.2.5
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `mlbi_at_dku_lib-0.2.4/src/mlbi_at_dku_lib.egg-info/SOURCES.txt` & `mlbi_at_dku_lib-0.2.5/src/mlbi_at_dku_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

