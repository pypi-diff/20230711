# Comparing `tmp/SPACEL-1.0.1.tar.gz` & `tmp/SPACEL-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPACEL-1.0.1.tar", last modified: Tue Apr  4 10:32:12 2023, max compression
+gzip compressed data, was "SPACEL-1.1.1.tar", last modified: Tue Jul 11 12:51:44 2023, max compression
```

## Comparing `SPACEL-1.0.1.tar` & `SPACEL-1.1.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-04-04 10:32:12.137915 SPACEL-1.0.1/
--rw-r--r--   0 xuhao      (501) staff       (20)     3149 2023-04-04 10:32:12.137543 SPACEL-1.0.1/PKG-INFO
--rw-r--r--   0 xuhao      (501) staff       (20)     2848 2023-03-17 10:58:24.000000 SPACEL-1.0.1/README.md
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-04-04 10:32:12.126745 SPACEL-1.0.1/SPACEL/
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-04-04 10:32:12.130575 SPACEL-1.0.1/SPACEL/Scube/
--rw-r--r--   0 xuhao      (501) staff       (20)      151 2023-03-17 08:40:55.000000 SPACEL-1.0.1/SPACEL/Scube/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)    12457 2023-03-17 08:40:55.000000 SPACEL-1.0.1/SPACEL/Scube/alignment.py
--rw-r--r--   0 xuhao      (501) staff       (20)    14330 2023-03-17 08:40:55.000000 SPACEL-1.0.1/SPACEL/Scube/gpr.py
--rw-r-----   0 xuhao      (501) staff       (20)     6191 2023-03-17 08:40:52.000000 SPACEL-1.0.1/SPACEL/Scube/plot.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4381 2023-03-17 08:40:52.000000 SPACEL-1.0.1/SPACEL/Scube/utils_3d.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-04-04 10:32:12.132773 SPACEL-1.0.1/SPACEL/Splane/
--rw-r--r--   0 xuhao      (501) staff       (20)      149 2023-03-17 08:41:02.000000 SPACEL-1.0.1/SPACEL/Splane/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)     1937 2023-03-17 08:40:55.000000 SPACEL-1.0.1/SPACEL/Splane/graph.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-04-04 10:32:12.133828 SPACEL-1.0.1/SPACEL/Splane/kegra/
--rw-r--r--   0 xuhao      (501) staff       (20)        0 2023-03-17 08:41:02.000000 SPACEL-1.0.1/SPACEL/Splane/kegra/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4662 2023-03-17 08:41:03.000000 SPACEL-1.0.1/SPACEL/Splane/kegra/gnn.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4658 2023-03-17 08:41:03.000000 SPACEL-1.0.1/SPACEL/Splane/kegra/gnn_utils.py
--rw-r--r--   0 xuhao      (501) staff       (20)    17210 2023-04-04 10:26:13.000000 SPACEL-1.0.1/SPACEL/Splane/model.py
--rw-r--r--   0 xuhao      (501) staff       (20)     2050 2023-03-17 08:41:03.000000 SPACEL-1.0.1/SPACEL/Splane/pygcn_utils.py
--rw-r--r--   0 xuhao      (501) staff       (20)     2576 2023-04-04 10:26:12.000000 SPACEL-1.0.1/SPACEL/Splane/utils.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-04-04 10:32:12.137078 SPACEL-1.0.1/SPACEL/Spoint/
--rw-r--r--   0 xuhao      (501) staff       (20)      138 2023-03-17 08:41:04.000000 SPACEL-1.0.1/SPACEL/Spoint/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)    27903 2023-04-04 10:07:37.000000 SPACEL-1.0.1/SPACEL/Spoint/base_model.py
--rw-r--r--   0 xuhao      (501) staff       (20)     1332 2023-03-17 08:41:04.000000 SPACEL-1.0.1/SPACEL/Spoint/data_augmentation.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4007 2023-03-17 08:41:04.000000 SPACEL-1.0.1/SPACEL/Spoint/data_downsample.py
--rw-r--r--   0 xuhao      (501) staff       (20)     6551 2023-03-17 08:41:04.000000 SPACEL-1.0.1/SPACEL/Spoint/data_utils.py
--rw-r--r--   0 xuhao      (501) staff       (20)     1017 2023-03-17 08:41:04.000000 SPACEL-1.0.1/SPACEL/Spoint/metrics.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4655 2023-04-04 10:26:13.000000 SPACEL-1.0.1/SPACEL/Spoint/model.py
--rw-r--r--   0 xuhao      (501) staff       (20)    16273 2023-03-17 08:41:05.000000 SPACEL-1.0.1/SPACEL/Spoint/spatial_simulation.py
--rw-r--r--   0 xuhao      (501) staff       (20)      745 2023-03-17 08:48:32.000000 SPACEL-1.0.1/SPACEL/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)       33 2023-04-04 10:31:51.000000 SPACEL-1.0.1/SPACEL/_version.py
--rw-r--r--   0 xuhao      (501) staff       (20)      719 2023-03-17 08:41:07.000000 SPACEL-1.0.1/SPACEL/setting.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-04-04 10:32:12.128554 SPACEL-1.0.1/SPACEL.egg-info/
--rw-r--r--   0 xuhao      (501) staff       (20)     3149 2023-04-04 10:32:11.000000 SPACEL-1.0.1/SPACEL.egg-info/PKG-INFO
--rw-r--r--   0 xuhao      (501) staff       (20)      790 2023-04-04 10:32:11.000000 SPACEL-1.0.1/SPACEL.egg-info/SOURCES.txt
--rw-r--r--   0 xuhao      (501) staff       (20)        1 2023-04-04 10:32:11.000000 SPACEL-1.0.1/SPACEL.egg-info/dependency_links.txt
--rw-r--r--   0 xuhao      (501) staff       (20)      108 2023-04-04 10:32:11.000000 SPACEL-1.0.1/SPACEL.egg-info/requires.txt
--rw-r--r--   0 xuhao      (501) staff       (20)        7 2023-04-04 10:32:11.000000 SPACEL-1.0.1/SPACEL.egg-info/top_level.txt
--rw-r--r--   0 xuhao      (501) staff       (20)       38 2023-04-04 10:32:12.138008 SPACEL-1.0.1/setup.cfg
--rw-r--r--   0 xuhao      (501) staff       (20)      885 2023-03-17 10:55:32.000000 SPACEL-1.0.1/setup.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-11 12:51:44.027290 SPACEL-1.1.1/
+-rw-r--r--   0 xuhao      (501) staff       (20)     3655 2023-07-11 12:51:44.026958 SPACEL-1.1.1/PKG-INFO
+-rw-r--r--   0 xuhao      (501) staff       (20)     3354 2023-07-11 12:50:36.000000 SPACEL-1.1.1/README.md
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-11 12:51:43.938820 SPACEL-1.1.1/SPACEL/
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-11 12:51:43.958498 SPACEL-1.1.1/SPACEL/Scube/
+-rw-r--r--   0 xuhao      (501) staff       (20)      151 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Scube/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    13309 2023-07-11 12:14:50.000000 SPACEL-1.1.1/SPACEL/Scube/alignment.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    14330 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Scube/gpr.py
+-rw-r-----   0 xuhao      (501) staff       (20)     6191 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Scube/plot.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4381 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Scube/utils_3d.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-11 12:51:43.996974 SPACEL-1.1.1/SPACEL/Splane/
+-rw-r--r--   0 xuhao      (501) staff       (20)      149 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Splane/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    15183 2023-07-11 12:20:57.000000 SPACEL-1.1.1/SPACEL/Splane/base_model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     1627 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Splane/graph.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-11 12:51:44.011126 SPACEL-1.1.1/SPACEL/Splane/kegra/
+-rw-r--r--   0 xuhao      (501) staff       (20)        0 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Splane/kegra/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4662 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Splane/kegra/gnn.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4658 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Splane/kegra/gnn_utils.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     3688 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Splane/model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     2050 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Splane/pygcn_utils.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4225 2023-07-11 09:00:10.000000 SPACEL-1.1.1/SPACEL/Splane/utils.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-11 12:51:44.026063 SPACEL-1.1.1/SPACEL/Spoint/
+-rw-r--r--   0 xuhao      (501) staff       (20)      138 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Spoint/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    27194 2023-07-11 09:03:42.000000 SPACEL-1.1.1/SPACEL/Spoint/base_model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     1332 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Spoint/data_augmentation.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4007 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Spoint/data_downsample.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     6788 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Spoint/data_utils.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     1017 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Spoint/metrics.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4998 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Spoint/model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    20829 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Spoint/spatial_simulation.py
+-rw-r--r--   0 xuhao      (501) staff       (20)      745 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)       32 2023-07-11 12:50:36.000000 SPACEL-1.1.1/SPACEL/_version.py
+-rw-r--r--   0 xuhao      (501) staff       (20)      719 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/setting.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-11 12:51:43.941235 SPACEL-1.1.1/SPACEL.egg-info/
+-rw-r--r--   0 xuhao      (501) staff       (20)     3655 2023-07-11 12:51:43.000000 SPACEL-1.1.1/SPACEL.egg-info/PKG-INFO
+-rw-r--r--   0 xuhao      (501) staff       (20)      818 2023-07-11 12:51:43.000000 SPACEL-1.1.1/SPACEL.egg-info/SOURCES.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)        1 2023-07-11 12:51:43.000000 SPACEL-1.1.1/SPACEL.egg-info/dependency_links.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)      120 2023-07-11 12:51:43.000000 SPACEL-1.1.1/SPACEL.egg-info/requires.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)        7 2023-07-11 12:51:43.000000 SPACEL-1.1.1/SPACEL.egg-info/top_level.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)       38 2023-07-11 12:51:44.027378 SPACEL-1.1.1/setup.cfg
+-rw-r--r--   0 xuhao      (501) staff       (20)      908 2023-07-11 12:48:07.000000 SPACEL-1.1.1/setup.py
```

### Comparing `SPACEL-1.0.1/PKG-INFO` & `SPACEL-1.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-Metadata-Version: 2.1
-Name: SPACEL
-Version: 1.0.1
-Summary: SPACEL: characterizing spatial transcriptome architectures by deep-learning
-Home-page: https://github.com/QuKunLab/SPACEL
-Author: Hao Xu
-Author-email: xuhaoustc@mail.ustc.edu.cn
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 [![Documentation Status](https://readthedocs.org/projects/spacel/badge/?version=latest)](https://spacel.readthedocs.io/en/latest/?badge=latest)
+![PyPI](https://img.shields.io/pypi/v/SPACEL)
 
 # SPACEL: characterizing spatial transcriptome architectures by deep-learning
 
 ![](docs/_static/img/figure1.png "Overview")
 SPACEL (**SP**atial **A**rchitecture **C**haracterization by d**E**ep **L**earning) is a Python package of deep-learning-based methods for ST data analysis. SPACEL consists of three modules: 
 * Spoint embedded a multiple-layer perceptron with a probabilistic model to deconvolute cell type composition for each spot on single ST slice.
 * Splane employs a graph convolutional network approach and an adversarial learning algorithm to identify uniform spatial domains that are transcriptomically and spatially coherent across multiple ST slices.
 * Scube automatically transforms the spatial coordinate systems of consecutive slices and stacks them together to construct a three-dimensional (3D) alignment of the tissue.
 
 ## Getting started
 * [Requirements](#Requirements)
 * [Installation](#Installation)
 * Tutorials
-    * [Spoint tutorial: Deconvolution of cell types distribution of spatial transcriptomics](docs/tutorials/deconvolution_of_cell_types_distribution.ipynb)
-    * [Splane tutorial: Identify uniform spatial domain in multiple slices](docs/tutorials/identification_of_uniform_spatial_domain.ipynb)
-    * [Scube tutorial: Alignment of multiple spatial transcriptomic slices](docs/tutorials/alignment_of_multiple_slices.ipynb)
+    * [Spoint tutorial: Deconvolution of cell types compostion on human brain Visium dataset](docs/tutorials/deconvolution_of_cell_types_distribution.ipynb)
+    * [Splane tutorial: Identify uniform spatial domain on human breast cancer Visium dataset](docs/tutorials/identification_of_uniform_spatial_domain.ipynb)
+    * [Scube tutorial: Alignment of consecutive ST slices on human brain MERFISH dataset](docs/tutorials/alignment_of_multiple_slices.ipynb)
     * [Scube tutorial: 3D expression modeling with gaussian process regression](docs/tutorials/3D_expression_modeling.ipynb)
 
 Read the [documentation](https://spacel.readthedocs.io) for more information.
+
+## Latest updates
+### Version 1.1.1 2023-07-11
+#### Features
+* All code based on `Tensorflow` have been mirated to `PyTorch`, it does not have `Tensorflow` as dependency anymore.
+* The `Splane.utils.add_cell_type_composition` function has been implemented to facilitate the cell type composition predicted by deconvolution methods into Splane.
+* Spoint and Splane now support tqdm type output for improved progress tracking.
     
 ## Requirements
 
 To install `SPACEL`, you need to install [PyTorch](https://pytorch.org) with GPU support first. If you don't need GPU acceleration, you can just skip the installation for `cudnn` and `cudatoolkit`.
 * Create conda environment for `SPACEL`:
 ```
 conda env create -f environment.yml
```

### Comparing `SPACEL-1.0.1/README.md` & `SPACEL-1.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,45 @@
+Metadata-Version: 2.1
+Name: SPACEL
+Version: 1.1.1
+Summary: SPACEL: characterizing spatial transcriptome architectures by deep-learning
+Home-page: https://github.com/QuKunLab/SPACEL
+Author: Hao Xu
+Author-email: xuhaoustc@mail.ustc.edu.cn
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 [![Documentation Status](https://readthedocs.org/projects/spacel/badge/?version=latest)](https://spacel.readthedocs.io/en/latest/?badge=latest)
+![PyPI](https://img.shields.io/pypi/v/SPACEL)
 
 # SPACEL: characterizing spatial transcriptome architectures by deep-learning
 
 ![](docs/_static/img/figure1.png "Overview")
 SPACEL (**SP**atial **A**rchitecture **C**haracterization by d**E**ep **L**earning) is a Python package of deep-learning-based methods for ST data analysis. SPACEL consists of three modules: 
 * Spoint embedded a multiple-layer perceptron with a probabilistic model to deconvolute cell type composition for each spot on single ST slice.
 * Splane employs a graph convolutional network approach and an adversarial learning algorithm to identify uniform spatial domains that are transcriptomically and spatially coherent across multiple ST slices.
 * Scube automatically transforms the spatial coordinate systems of consecutive slices and stacks them together to construct a three-dimensional (3D) alignment of the tissue.
 
 ## Getting started
 * [Requirements](#Requirements)
 * [Installation](#Installation)
 * Tutorials
-    * [Spoint tutorial: Deconvolution of cell types distribution of spatial transcriptomics](docs/tutorials/deconvolution_of_cell_types_distribution.ipynb)
-    * [Splane tutorial: Identify uniform spatial domain in multiple slices](docs/tutorials/identification_of_uniform_spatial_domain.ipynb)
-    * [Scube tutorial: Alignment of multiple spatial transcriptomic slices](docs/tutorials/alignment_of_multiple_slices.ipynb)
+    * [Spoint tutorial: Deconvolution of cell types compostion on human brain Visium dataset](docs/tutorials/deconvolution_of_cell_types_distribution.ipynb)
+    * [Splane tutorial: Identify uniform spatial domain on human breast cancer Visium dataset](docs/tutorials/identification_of_uniform_spatial_domain.ipynb)
+    * [Scube tutorial: Alignment of consecutive ST slices on human brain MERFISH dataset](docs/tutorials/alignment_of_multiple_slices.ipynb)
     * [Scube tutorial: 3D expression modeling with gaussian process regression](docs/tutorials/3D_expression_modeling.ipynb)
 
 Read the [documentation](https://spacel.readthedocs.io) for more information.
+
+## Latest updates
+### Version 1.1.1 2023-07-11
+#### Features
+* All code based on `Tensorflow` have been mirated to `PyTorch`, it does not have `Tensorflow` as dependency anymore.
+* The `Splane.utils.add_cell_type_composition` function has been implemented to facilitate the cell type composition predicted by deconvolution methods into Splane.
+* Spoint and Splane now support tqdm type output for improved progress tracking.
     
 ## Requirements
 
 To install `SPACEL`, you need to install [PyTorch](https://pytorch.org) with GPU support first. If you don't need GPU acceleration, you can just skip the installation for `cudnn` and `cudatoolkit`.
 * Create conda environment for `SPACEL`:
 ```
 conda env create -f environment.yml
```

### Comparing `SPACEL-1.0.1/SPACEL/Scube/alignment.py` & `SPACEL-1.1.1/SPACEL/Scube/alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,34 +83,42 @@
 def score(warp_param, target_loc, source_loc, target_cluster, source_cluster,k,knn_exclude_cutoff,p,a):
     new_source_loc = []
     x0 = 0
     y0 = 0
     for x,y in source_loc:
         new_source_loc.append(rotate_loc(x,y,x0,y0,warp_param[0]))
     new_source_loc = np.array(new_source_loc)
-    new_source_loc[:,0] += warp_param[1]  #x方向平移
-    new_source_loc[:,1] += warp_param[2]  #y方向平移
+    new_source_loc[:,0] += warp_param[1]
+    new_source_loc[:,1] += warp_param[2]
     return -neighbor_simi_fast(new_source_loc, target_loc, source_cluster, target_cluster, k, knn_exclude_cutoff,p,a)
 
 def optimize(target_loc, source_loc, target_cluster, source_cluster, n_neighbors, knn_exclude_cutoff ,p,a, bound_alpha,n_threads,*args,**kwargs): 
 
     source_loc_flip = deepcopy(source_loc)
     source_loc_flip[:,0] = -source_loc_flip[:,0]
     func1 = partial(score, target_loc=target_loc, source_loc=source_loc, target_cluster=target_cluster, source_cluster=source_cluster,k=n_neighbors,knn_exclude_cutoff=knn_exclude_cutoff,p=p,a=a)
-    opm1 = differential_evolution(func1, bounds=((0, 360), (target_loc.min(0)[0]*bound_alpha, target_loc.max(0)[0]*bound_alpha), (target_loc.min(0)[1]*bound_alpha, target_loc.max(0)[1]*bound_alpha)),workers=n_threads,*args,**kwargs)
+    opm1 = differential_evolution(func1, 
+                                  bounds=((0, 360), (target_loc.min(0)[0]*bound_alpha, target_loc.max(0)[0]*bound_alpha), (target_loc.min(0)[1]*bound_alpha, target_loc.max(0)[1]*bound_alpha)),
+                                  workers=n_threads,
+                                  updating='immediate' if n_threads == 1 else 'deferred',
+                                  *args,
+                                  **kwargs)
     score1 = -opm1.fun
     result1 = opm1.x
     
     func2 = partial(score, target_loc=target_loc, source_loc=source_loc_flip, target_cluster=target_cluster, source_cluster=source_cluster,k=n_neighbors,knn_exclude_cutoff=knn_exclude_cutoff,p=p,a=a)
-    opm2 = differential_evolution(func2,bounds=((0, 360), (target_loc.min(0)[0]*bound_alpha, target_loc.max(0)[0]*bound_alpha), (target_loc.min(0)[1]*bound_alpha, target_loc.max(0)[1]*bound_alpha)),workers=n_threads,*args,**kwargs)
+    opm2 = differential_evolution(func2,
+                                  bounds=((0, 360), (target_loc.min(0)[0]*bound_alpha, target_loc.max(0)[0]*bound_alpha), (target_loc.min(0)[1]*bound_alpha, target_loc.max(0)[1]*bound_alpha)),
+                                  workers=n_threads,
+                                  updating='immediate' if n_threads == 1 else 'deferred',
+                                  *args,
+                                  **kwargs)
     score2 = -opm2.fun
     result2 = opm2.x
 
-    print(f'Optimal score: flip = {score1}, not flip = {score2}')
-
     if score1 > score2:
         return 0, result1, score1, 1, result2, score2
     else:
         return 1, result2, score2, 0, result1, score1
 
 def align_pairwise(param, n_neighbors, knn_exclude_cutoff,p,a,bound_alpha,n_threads,*args,**kwargs):
     i, target_loc,source_loc,target_cluster,source_cluster = param
@@ -119,38 +127,38 @@
 
 def align(
     ad_list,
     cluster_key='spatial_domain',
     output_path=None,
     raw_loc_key='spatial',
     aligned_loc_key='spatial_aligned',
-    n_neighbors=5,
-    knn_exclude_cutoff=1,
+    n_neighbors=15,
+    knn_exclude_cutoff=None,
     p=2,
     a=1,
     bound_alpha=1,
     write_loc_path=None,
     n_threads=1,
     seed=42,
     subset_prop=None,
     *args,
     **kwargs
 ):
     """Pairwise alignment.
     
     Pairwise align the slices in ad_list. The aligned coordinates are saved in ``.obsm[aligned_loc_key]`` in each slices of ``ad_list``.
-
+    
     Args:
         ad_list: A list containing all slice data in AnnData object.
         cluster_key: A string representing one column of ``obs`` in AnnData object, containing the spatial domain information used for alignment.
         output_path: A string representing the path directory where the alignment parameters are saved. If ``None``, it will be 'Scube_outputs'.
-        raw_loc_key: A string representing one key of ``obsm`` in AnnData object of each slices in ``ad_list``, containing the raw coordinates.
-        aligned_loc_key: A string written to a key of ``obsm`` in AnnData object of each slices in ``ad_list``, containing the aligned coordinates.
+        raw_loc_key: A string representing one key of ``obsm`` in AnnData object of each slice in ``ad_list``, containing the raw coordinates.
+        aligned_loc_key: A string written to a key of ``obsm`` in AnnData object of each slice in ``ad_list``, containing the aligned coordinates.
         n_neighbors: A number of neighbors in target slices considered by each spot/cell in source slices.
-        knn_exclude_cutoff: A number used to filter the neighbors in KNN. The neighbor will be exclude when the distance of neighbors larger than the median of neareast ``n_neighbors + knn_exclude_cutoff`` neighbors distance in all spot/cell in target slice.
+        knn_exclude_cutoff: A number used to filter the neighbors in MNN. The neighbor will be exclude when the distance of neighbors larger than the median of neareast ``n_neighbors + knn_exclude_cutoff`` neighbors distance in all spots/cells in target slice. If ``None``, it will automatically default to ``n_neighbors``.
         p: Degree of the penalty function.
         a: Coefficient of the penalty function.
         bound_alpha: For the optimized boundary, the multiplier based on the maximum and minimum values of the slice coordinates.
         write_loc_path: A string representing the path directory where the aligned coordinates of all slices are saved. If ``None``, it won't be saved.
         n_threads: The number of parallel threads for the optimization algorithm.
         seed: Seed for the optimization algorithm.
         subset_prop: The downsampling ratio for cells in each slice.
@@ -167,36 +175,44 @@
         os.makedirs(output_path)
     
     # centering X, Y coordinate
     for i in range(len(ad_list)):
         raw_loc = np.asarray(ad_list[i].obsm[raw_loc_key], dtype=np.float32)
         raw_loc[:,:2] = raw_loc[:,:2] - np.median(raw_loc[:,:2],axis=0)
         ad_list[i].obsm['spatial_pair'] = raw_loc
+        
+    if knn_exclude_cutoff is None:
+        knn_exclude_cutoff = n_neighbors
     
     start = time.time()
     print('Start alignment...')
     res = []
     for i in range(1,len(ad_list)):
         print(f'Alignment slice {i} to {i-1}')
         target_ind = i-1
         source_ind = i
         target_xy = ad_list[target_ind].obsm['spatial_pair'][:,:2]
         source_xy = ad_list[source_ind].obsm['spatial_pair'][:,:2]
         target_cluster = np.asarray(ad_list[target_ind].obs[cluster_key])
         source_cluster = np.asarray(ad_list[source_ind].obs[cluster_key])
+        cluster_name = np.unique(np.concatenate([target_cluster,source_cluster]))
+        cluster_index = np.arange(len(cluster_name))
+        cluster_name = dict(zip(cluster_name, cluster_index))
+        target_cluster = np.array(pd.Series(target_cluster).replace(cluster_name))
+        source_cluster = np.array(pd.Series(source_cluster).replace(cluster_name))
+        
         param = [i, target_xy, source_xy, target_cluster, source_cluster]
         r = align_pairwise(param, n_neighbors=n_neighbors, knn_exclude_cutoff=knn_exclude_cutoff,p=p,a=a,bound_alpha=bound_alpha, n_threads=n_threads,seed=seed)
         res.append(r)
     
     warp_info=np.array(res,dtype=np.float32)
     np.save(os.path.join(output_path,'warp_info.npy'),warp_info)
     
     warp_info = warp_info[:,:6]
     score = warp_info[:,5]
-    print('All score:', str(score))
     print('Runtime: ' + str(time.time() - start),'s')
 
     ad_list[0].obsm[aligned_loc_key] = ad_list[0].obsm['spatial_pair']
     for i in range(1,len(ad_list)):
         target_ind = i-1
         source_ind = i
         target_loc = ad_list[target_ind].obsm['spatial_pair']
@@ -232,8 +248,8 @@
         ad_list[i].obsm[aligned_loc_key] = aligned_loc
     
     if write_loc_path is not None:
         coo = pd.DataFrame()
         for i in range(len(ad_list)):
             loc = ad_list[i].obsm[aligned_loc_key]
             coo = pd.concat([coo,loc],axis=0)
-        coo.to_csv(write_loc_path)
+        coo.to_csv(write_loc_path)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `SPACEL-1.0.1/SPACEL/Scube/gpr.py` & `SPACEL-1.1.1/SPACEL/Scube/gpr.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.0.1/SPACEL/Scube/plot.py` & `SPACEL-1.1.1/SPACEL/Scube/plot.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.0.1/SPACEL/Scube/utils_3d.py` & `SPACEL-1.1.1/SPACEL/Scube/utils_3d.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.0.1/SPACEL/Splane/graph.py` & `SPACEL-1.1.1/SPACEL/Splane/graph.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 import numpy as np
-from scipy.sparse import coo_matrix
+from scipy.sparse import coo_matrix, block_diag
 import torch
 import torch.nn.functional as F
 from .pygcn_utils import *
 
 def get_graph_inputs(celltype_ad_list):
     print('Generating GNN inputs...')
     A_list = []
     X_list = []
     for celltype_ad in celltype_ad_list:
         X_tmp = np.matrix(celltype_ad.X,dtype='float32')
         X_list.append(X_tmp)
         A_list.append(coo_matrix(celltype_ad.obsp['spatial_distances'],dtype='float32'))
 
     X_raw = np.concatenate(X_list)
-    element_num = 0
-    for A_tmp in A_list:
-        element_num += A_tmp.shape[0]
-    A = np.zeros((element_num,element_num),dtype='float32')
-    loc_index = 0
     class_index = 0
     slice_class = []
     for A_tmp in A_list:
-        A[loc_index:loc_index+A_tmp.shape[0],loc_index:loc_index+A_tmp.shape[0]] = A_tmp.toarray()
         slice_class = slice_class + [class_index]*A_tmp.shape[0]
-        loc_index += A_tmp.shape[0]
         class_index += 1
-    A = coo_matrix(A,dtype='float32')
-    nb_mask = np.array(np.where((A>0).todense()))
+    A = block_diag(A_list)
+    nb_mask = np.argwhere(A > 0).T
     slice_class_onehot = F.one_hot(torch.tensor(slice_class)).float()
     return X_raw,A,nb_mask,slice_class_onehot
 
 def get_graph_kernel(features,adj,k=2):
     features_scaled = (features-features.mean(0))/features.std(0)
     features_scaled = torch.tensor(features_scaled)
     SYM_NORM = False  # symmetric (True) vs. left-only (False) normalization
```

### Comparing `SPACEL-1.0.1/SPACEL/Splane/kegra/gnn.py` & `SPACEL-1.1.1/SPACEL/Splane/kegra/gnn.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.0.1/SPACEL/Splane/kegra/gnn_utils.py` & `SPACEL-1.1.1/SPACEL/Splane/kegra/gnn_utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.0.1/SPACEL/Splane/model.py` & `SPACEL-1.1.1/SPACEL/Splane/base_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 import random
 import os 
 import matplotlib
 from sklearn.cluster import KMeans
 from sklearn.metrics import davies_bouldin_score
 import seaborn as sns
 import squidpy as sq
-from .graph import get_graph_inputs,get_graph_kernel,split_train_test_idx
-from .utils import generate_celltype_ad_list,cal_celltype_weight,clustering
+from .utils import clustering
 import math
 import time
 import numpy as np
 from tqdm import tqdm
+from time import strftime, localtime
+import tempfile
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.optim as optim
 from torch.nn.parameter import Parameter
 from torch.nn.modules.module import Module
@@ -237,37 +238,56 @@
         g_loss = torch.sum(self.celltype_weights*F.cosine_similarity(x_mask, decoded_mask,dim=0))+torch.sum(self.celltype_weights*self.kl_divergence(x_mask, decoded_mask, dim=0)) + simi_l*simi_loss
         total_loss = g_loss - d_l*d_loss
         db_loss = clustering(self.Cluster, encoded.cpu().detach().numpy())
         return total_loss, g_loss, d_loss, accuarcy, simi_loss, db_loss, encoded, decoded
     
     def train(
         self,
-        max_epochs=1000,
+        max_epochs=300,
         convergence=0.0001,
         db_convergence=0,
         early_stop_epochs=10,
-        d_l=0.2,
+        d_l=0.5,
         simi_l=None,
         g_step = 1,
         d_step = 1,
         plot_step=5,
-        save_path = 'Splane_models',
+        save_path=None,
         prefix=None
     ):
+        """Training Splane model.
+
+        Training Splane model for identification of uniform spatial domains in multiple slics.
+
+        Args:
+            max_steps: The max step of training. The training process will be stop when achive max step.
+            convergence: The total loss threshold for early stop.
+            db_convergence: The DBS threshold for early stop.
+            early_stop_epochs: The max epochs of loss difference less than convergence.
+            d_l: The weight of discriminator loss.
+            simi_l: The weight of similarity loss.
+            plot_step: The interval steps of training.
+            save_path: A string representing the path directory where the model is saved.
+            prefix: A string added to the prefix of file name of saved model.
+
+        Returns:
+            ``None``
+        """
         best_loss = np.inf
         best_db_loss = np.inf
         best_simi_loss = np.inf
         simi_l = 1/np.mean(self.morans_mean)
-
+        
+        if save_path is None:
+            save_path = os.path.join(tempfile.gettempdir() ,'Splane_models_'+strftime("%Y%m%d%H%M%S",localtime()))
         if not os.path.exists(save_path):
             os.makedirs(save_path)
         early_stop_count = 0
         pbar = tqdm(range(max_epochs))
         for epoch in pbar:
-
             for _ in range(g_step):
                 train_total_loss = self.train_model_g(d_l=d_l, simi_l=simi_l)
             for _ in range(d_step):
                 self.train_model_d()
 
             if epoch % plot_step == 0:
                 test_total_loss, test_g_loss, test_d_loss, test_acc, simi_loss, db_loss, encoded, decoded = self.test_model(d_l=d_l, simi_l=simi_l)
@@ -294,15 +314,26 @@
                 
 
                 # print("Epoch {} train g loss={} g loss={} d loss={} acc={} simi loss={} db loss={}".format(epoch, test_total_loss, test_g_loss, test_d_loss, test_acc, simi_loss, db_loss))
                 if early_stop_count > early_stop_epochs:
                     print('Stop trainning because of loss convergence')
                     break
     
-    def identify_spatial_domain(self,colors=None,key=None):
+    def identify_spatial_domain(self,key=None,colors=None):
+        """Identify Spaital domains.
+
+        Identification of uniform spatial domains in multiple slics.
+
+        Args:
+            key: A column name to be saved in  the `.obs` attribute of AnnData object of the ST data, representing the spatial domains. If not provided, the spatial domain will be saved as 'spatial_domain' in the `.obs` attribute.
+            colors: A list of colors assigned to each spatial domain.
+            
+        Returns:
+            ``None``
+        """
         if colors is None:
             if self.n_clusters > 10:
                 colors = [matplotlib.colors.to_hex(c) for c in sns.color_palette('tab20',n_colors=self.n_clusters)]
             else:
                 colors = [matplotlib.colors.to_hex(c) for c in sns.color_palette('tab10',n_colors=self.n_clusters)]
             color_map = pd.DataFrame(colors,index=np.arange(self.n_clusters),columns=['color'])
         if key is None:
@@ -316,105 +347,7 @@
         for i in range(len(self.expr_ad_list)):
             if key in self.expr_ad_list[i].obs.columns:
                 self.expr_ad_list[i].obs = self.expr_ad_list[i].obs.drop(columns=key)
             self.expr_ad_list[i].obs[key] = clusters[loc_index:loc_index+self.expr_ad_list[i].shape[0]]
             self.expr_ad_list[i].obs[key] = pd.Categorical(self.expr_ad_list[i].obs[key])
             self.expr_ad_list[i].uns[f'{key}_colors'] = [color_map.loc[c,'color'] for c in self.expr_ad_list[i].obs['spatial_domain'].cat.categories]
             loc_index += self.expr_ad_list[i].shape[0]
-
-def init_model(
-    expr_ad_list:list,
-    n_clusters:int,
-    k:int=2,
-    use_weight=True,
-    train_prop:float=0.5,
-    n_neighbors=6,
-    min_prop=0.01,
-    lr:float=3e-3,
-    l1:float=0.01,
-    l2:float=0.01,
-    latent_dim:int=16,
-    hidden_dims:int=64,
-    gnn_dropout:float=0.8,
-    simi_neighbor=1,
-    use_gpu=None,
-    seed=42
-)->SplaneModel:
-    """Initialize Splane model.
-    
-    Build the model then set the data and paratemters. 
-    
-    Args:
-        expr_ad_list: A list of AnnData object of spatial transcriptomic data as the model input.
-        n_clusters: The number of cluster of the model ouput. 
-        k: The order of neighbors of a spot for graph construction.
-        use_weight: If True, the cell type proportion of Moran was used as the weight of the loss.
-        train_prop: The proportion of training set.
-        n_neighbors: The number of neighbors for graph construction.
-        lr: Learning rate of training.
-        latent_dim: The dimension of latent features. It equal to the number of nodes of bottleneck layer.
-        hidden_dims: The number of nodes of hidden layers.
-        gnn_dropout: The dropout rate of GNN model.
-        simi_neighbor: The order of neighbors used for similarity loss. If is None, It equal to the order used for constructed graph.
-        seed: Random number seed.
-    Returns:
-        A ``DataFrame`` contained deconvoluted results. Each row representing a spot, and each column representing a cell type.
-    """
-    
-    print('Setting global seed:', seed)
-    random.seed(seed)
-    np.random.seed(seed)
-    torch.manual_seed(seed)
-    torch.cuda.manual_seed(seed)
-    torch.backends.cudnn.deterministic = True
-    torch.backends.cudnn.benchmark = False
-    
-    if use_gpu is None:
-        if torch.cuda.is_available():
-            use_gpu = True
-        else:
-            use_gpu = False
-    
-    for expr_ad in expr_ad_list:
-        if 'spatial_connectivities' not in expr_ad.obsp.keys():
-            sq.gr.spatial_neighbors(expr_ad,coord_type='grid',n_neighs=n_neighbors)
-    celltype_ad_list = generate_celltype_ad_list(expr_ad_list,min_prop=min_prop)
-    celltype_weights,morans_mean = cal_celltype_weight(celltype_ad_list)
-    kept_ind = celltype_weights > 0
-    if not use_weight:
-        celltype_weights = np.ones(len(celltype_weights))/len(celltype_weights)
-    X,A,nb_mask,slice_class_onehot = get_graph_inputs(celltype_ad_list)
-    X_filtered, graph, support = get_graph_kernel(X[:,kept_ind],A,k=k)
-    celltype_weights = celltype_weights[kept_ind]
-    morans_mean = morans_mean[kept_ind]
-    if simi_neighbor == 1:
-        nb_mask = nb_mask
-    elif simi_neighbor == None:
-        nb_mask = np.array(np.where(graph[-1].to_dense())!=0)
-        nb_mask = nb_mask[:,nb_mask[0] != nb_mask[1]]
-    else:
-        raise ValueError('simi_neighbor must be 1 or None.')
-    train_idx,test_idx = split_train_test_idx(X,train_prop=0.5)
-    if use_gpu:
-        for i in range(len(graph)):
-            graph[i] = graph[i].cuda()
-        slice_class_onehot = slice_class_onehot.cuda()
-    return SplaneModel(
-        expr_ad_list,
-        n_clusters,
-        X_filtered,
-        graph,
-        support,
-        slice_class_onehot,
-        nb_mask,
-        train_idx,
-        test_idx,
-        celltype_weights,
-        morans_mean,
-        lr,
-        l1,
-        l2,
-        latent_dim,
-        hidden_dims,
-        gnn_dropout,
-        use_gpu
-    )
```

### Comparing `SPACEL-1.0.1/SPACEL/Splane/pygcn_utils.py` & `SPACEL-1.1.1/SPACEL/Splane/pygcn_utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.0.1/SPACEL/Spoint/base_model.py` & `SPACEL-1.1.1/SPACEL/Spoint/base_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pandas as pd
 import scanpy as sc
 import scvi
 import anndata
 from . import metrics
 import matplotlib.pyplot as plt
 import os
+import tempfile
 from copy import deepcopy
 import logging
 import itertools
 from functools import partial
 from tqdm import tqdm
 from time import strftime, localtime
 from scipy.sparse import issparse
@@ -22,126 +23,85 @@
 import torch.nn.functional as F
 import torch.optim as optim
 from torch.utils.data import TensorDataset, DataLoader, RandomSampler, BatchSampler
 from torch.nn.parameter import Parameter
 from torch.nn.modules.module import Module
 from torch.utils.data.dataloader import default_collate
 
-def guassian_kernel(source, target):
-    n_samples = int(source.shape[0])+int(target.shape[0])
-    total = np.concatenate((source, target), axis=0)
-    total0 = np.expand_dims(total,axis=0)
-    total0= np.broadcast_to(total0,[int(total.shape[0]), int(total.shape[0]), int(total.shape[1])])
-    total1 = np.expand_dims(total,axis=1)
-    total1=np.broadcast_to(total1,[int(total.shape[0]), int(total.shape[0]), int(total.shape[1])])
-    L2_distance_square = np.cumsum(np.square(total0-total1),axis=2)
-    bandwidth = np.sum(L2_distance_square) / (n_samples**2-n_samples)
-    kernel_val = np.exp(-L2_distance_square / bandwidth)
-    return kernel_val
-
-def MMD(source, target):
-    batch_size = int(source.shape[0])
-    kernels = guassian_kernel(source, target)
-    loss = 0
-    for i in range(batch_size):
-        s1, s2 = i, (i + 1) % batch_size
-        t1, t2 = s1 + batch_size, s2 + batch_size
-        loss += kernels[s1, s2] + kernels[t1, t2]
-        loss -= kernels[s1, t2] + kernels[s2, t1]
-    n_loss= loss / float(batch_size)
-    return np.mean(n_loss)
-
 def compute_kernel(x, y):
     x_size = x.size(0)
     y_size = y.size(0)
     dim = x.size(1)
-    tiled_x = torch.tile(torch.reshape(x, (x_size, 1, dim)), (1, y_size, 1))
-    tiled_y = torch.tile(torch.reshape(y, (1, y_size, dim)), (x_size, 1, 1))
-    return torch.exp(-torch.square(tiled_x - tiled_y).mean(2) / dim)
+
+    tiled_x = x.unsqueeze(1).expand(x_size, y_size, dim)
+    tiled_y = y.unsqueeze(0).expand(x_size, y_size, dim)
+
+    kernel = torch.exp(-torch.square(tiled_x - tiled_y).mean(dim=2) / dim)
+    return kernel
 
 def compute_mmd(x, y):
     x_kernel = compute_kernel(x, x)
     y_kernel = compute_kernel(y, y)
     xy_kernel = compute_kernel(x, y)
-    return x_kernel.mean() + y_kernel.mean() - 2 * xy_kernel.mean()
+
+    mmd = x_kernel.mean() + y_kernel.mean() - 2 * xy_kernel.mean()
+    return mmd
 
 class PredictionModel(nn.Module):
     def __init__(
-        self, 
+        self,
         input_dims,
         latent_dims,
         hidden_dims,
         celltype_dims,
         dropout
     ):
         super(PredictionModel, self).__init__()
         
         self.encoder = nn.Sequential(
             nn.Linear(input_dims, hidden_dims),
             nn.LeakyReLU(),
-            nn.BatchNorm1d(hidden_dims),
-            nn.Linear(hidden_dims, hidden_dims),
-            nn.LeakyReLU(),
-            nn.BatchNorm1d(hidden_dims),
-            nn.Linear(hidden_dims, hidden_dims),
-            nn.LeakyReLU(),
-            nn.BatchNorm1d(hidden_dims),
+            nn.LayerNorm(hidden_dims),
             nn.Dropout(dropout),
-            nn.Linear(hidden_dims, latent_dims)
+            nn.Linear(hidden_dims, latent_dims),
         )
         self.decoder = nn.Sequential(
-            nn.Linear(latent_dims, hidden_dims),
+            nn.Linear(celltype_dims, hidden_dims),
             nn.LeakyReLU(),
-            nn.BatchNorm1d(hidden_dims),
+            nn.LayerNorm(hidden_dims),
             nn.Linear(hidden_dims, hidden_dims),
             nn.LeakyReLU(),
-            nn.BatchNorm1d(hidden_dims),
+            nn.LayerNorm(hidden_dims),
             nn.Linear(hidden_dims, hidden_dims),
             nn.LeakyReLU(),
-            nn.BatchNorm1d(hidden_dims),
-            nn.Dropout(dropout),
+            nn.LayerNorm(hidden_dims),
             nn.Linear(hidden_dims, input_dims)
         )
         self.pred = nn.Sequential(
             nn.Linear(latent_dims, hidden_dims),
             nn.LeakyReLU(),
+            nn.LayerNorm(hidden_dims),
+            nn.Dropout(dropout),
             nn.Linear(hidden_dims, celltype_dims),
             nn.Softmax(dim=1),
         )
                 
         nn.init.kaiming_normal_(self.encoder[0].weight)
-        nn.init.kaiming_normal_(self.encoder[3].weight)
-        nn.init.kaiming_normal_(self.encoder[6].weight)
-        nn.init.xavier_uniform_(self.encoder[-1].weight)
-        
+        nn.init.kaiming_normal_(self.encoder[4].weight)
         nn.init.kaiming_normal_(self.decoder[0].weight)
         nn.init.kaiming_normal_(self.decoder[3].weight)
         nn.init.kaiming_normal_(self.decoder[6].weight)
         nn.init.xavier_uniform_(self.decoder[-1].weight)
-
         nn.init.kaiming_normal_(self.pred[0].weight)
-        nn.init.xavier_uniform_(self.pred[2].weight)
-        
-    @staticmethod
-    def l2_activate(x,dim):
-        
-        def scale(z):
-            zmax = z.max(1, keepdims=True).values
-            zmin = z.min(1, keepdims=True).values
-            z_std = torch.nan_to_num(torch.div(z - zmin,(zmax - zmin)),0)
-            return z_std
-        
-        x = scale(x)
-        x = F.normalize(x, p=2, dim=1)
-        return x
+        nn.init.xavier_uniform_(self.pred[4].weight)
 
     def forward(self, x):
-        z = self.l2_activate(self.encoder(x),dim=1)
+        z = self.encoder(x)
         pred = self.pred(z)
-        decoded = self.decoder(z)
+        decoded = self.decoder(pred)
         return z, pred, decoded
 
 class SpointModel():
     def __init__(
         self, 
         st_ad, 
         sm_ad, 
@@ -152,18 +112,19 @@
         st_batch_key=None,
         scvi_layers=2,
         scvi_latent=64,
         scvi_gene_likelihood='zinb',
         scvi_dispersion='gene-batch',
         latent_dims=32, 
         hidden_dims=512,
+        infer_losses=['kl','cos'],
         l1=0.01,
         l2=0.01,
         sm_lr=3e-4,
-        st_lr=3e-4,
+        st_lr=3e-5,
         use_gpu=None,
         seed=42
     ):
         if ((use_gpu is None) or (use_gpu is True)) and (torch.cuda.is_available()):
             self.device = 'cuda'
         else:
             self.device = 'cpu'
@@ -176,57 +137,75 @@
         self.used_genes = used_genes
         self.clusters = clusters
         self.st_batch_key = st_batch_key
         self.scvi_layers = scvi_layers
         self.scvi_latent = scvi_latent
         self.scvi_gene_likelihood = scvi_gene_likelihood
         self.scvi_dispersion = scvi_dispersion
-        self.mse_loss_func = F.mse_loss
         self.kl_infer_loss_func = partial(self.kl_divergence, dim=1)
-        self.kl_rec_loss_func = partial(self.kl_divergence, dim=0)
+        self.kl_rec_loss_func = partial(self.kl_divergence, dim=1)
         self.cosine_infer_loss_func = partial(F.cosine_similarity, dim=1)
-        self.cosine_rec_loss_func = partial(F.cosine_similarity, dim=0)
+        self.cosine_rec_loss_func = partial(F.cosine_similarity, dim=1)
+        self.rmse_loss_func = self.rmse
+        self.infer_losses = infer_losses
+        self.mmd_loss = compute_mmd
         self.l1 = l1
         self.l2 = l2
         self.use_rep = use_rep
         if use_rep == 'scvi':
-            feature_dims = scvi_latent
+            self.feature_dims = scvi_latent
         elif use_rep == 'X':
-            feature_dims = st_ad.shape[1]
+            self.feature_dims = st_ad.shape[1]
         elif use_rep == 'pca':
-            feature_dims = 50
+            self.feature_dims = 50
         else:
             raise ValueError('use_rep must be one of scvi, pca and X.')
-        self.model = PredictionModel(feature_dims,latent_dims,hidden_dims,len(clusters),0.5).to(self.device)
-        self.sm_optimizer = optim.Adam(self.model.parameters(),lr=sm_lr)
-        self.st_optimizer = optim.Adam(list(self.model.encoder.parameters())+list(self.model.decoder.parameters()),lr=st_lr)
+        self.latent_dims = latent_dims
+        self.hidden_dims = hidden_dims
+        self.sm_lr = sm_lr
+        self.st_lr = st_lr
+        self.init_model()
+        self.st_data = None
+        self.sm_data = None
+        self.sm_labels = None
         self.best_path = None
-        self.history = pd.DataFrame(columns = ['sm_train_rec_loss','sm_train_infer_loss','sm_train_total_loss','sm_test_rec_loss','sm_test_infer_loss','sm_test_total_loss','st_train_rec_loss','st_test_rec_loss','is_best'])
+        self.history = pd.DataFrame(columns = ['sm_train_rec_loss','sm_train_infer_loss','sm_test_rec_loss','sm_test_infer_loss','st_train_rec_loss','st_test_rec_loss','st_train_mmd_loss','st_test_mmd_loss','is_best'])
         self.batch_size = None
         self.seed = seed
+
+    @staticmethod
+    def rmse(y_true, y_pred):
+        mse = F.mse_loss(y_pred, y_true)
+        rmse = torch.sqrt(mse)
+        return rmse
         
     @staticmethod
     def kl_divergence(y_true, y_pred, dim=0):
         y_pred = torch.clip(y_pred, torch.finfo(torch.float32).eps)
         y_true = y_true.to(y_pred.dtype)
         y_true = torch.nan_to_num(torch.div(y_true, y_true.sum(dim, keepdims=True)),0)
         y_pred = torch.nan_to_num(torch.div(y_pred, y_pred.sum(dim, keepdims=True)),0)
         y_true = torch.clip(y_true, torch.finfo(torch.float32).eps, 1)
         y_pred = torch.clip(y_pred, torch.finfo(torch.float32).eps, 1)
         return torch.mul(y_true, torch.log(torch.nan_to_num(torch.div(y_true, y_pred)))).mean(dim)
+    
+    def init_model(self):
+        self.model = PredictionModel(self.feature_dims,self.latent_dims,self.hidden_dims,len(self.clusters),0.8).to(self.device)
+        self.sm_optimizer = optim.Adam(list(self.model.encoder.parameters())+list(self.model.pred.parameters()),lr=self.sm_lr)
+        self.st_optimizer = optim.Adam(list(self.model.encoder.parameters())+list(self.model.decoder.parameters()),lr=self.st_lr)
         
     def get_scvi_latent(
         self,
-        n_layers,
-        n_latent,
-        gene_likelihood,
-        dispersion,
-        max_epochs,
-        early_stopping,
-        batch_size,
+        n_layers=None,
+        n_latent=None,
+        gene_likelihood=None,
+        dispersion=None,
+        max_epochs=100,
+        early_stopping=True,
+        batch_size=4096,
     ):
         if self.st_batch_key is not None:
             if 'simulated' in self.st_ad.obs[self.st_batch_key]:
                 raise ValueError(f'obs[{self.st_batch_key}] cannot include "real".')
             self.st_ad.obs["batch"] = self.st_ad.obs[self.st_batch_key].astype(str)
             self.sm_ad.obs["batch"] = 'simulated'
         else:
@@ -237,15 +216,22 @@
         adata.layers["counts"] = adata.X.copy()
 
         scvi.model.SCVI.setup_anndata(
             adata,
             layer="counts",
             batch_key="batch"
         )
-
+        if n_layers is None:
+            n_layers = self.scvi_layers
+        if n_latent is None:
+            n_latent = self.scvi_latent
+        if gene_likelihood is None:
+            gene_likelihood = self.scvi_gene_likelihood
+        if dispersion is None:
+            dispersion = self.scvi_dispersion
         vae = scvi.model.SCVI(adata, n_layers=n_layers, n_latent=n_latent, gene_likelihood=gene_likelihood,dispersion=dispersion)
         vae.train(max_epochs=max_epochs,early_stopping=early_stopping,batch_size=batch_size,use_gpu=self.use_gpu)
         adata.obsm["X_scVI"] = vae.get_latent_representation()
 
         st_scvi_ad = anndata.AnnData(adata[adata.obs['batch'] != 'simulated'].obsm["X_scVI"])
         sm_scvi_ad = anndata.AnnData(adata[adata.obs['batch'] == 'simulated'].obsm["X_scVI"])
 
@@ -261,15 +247,17 @@
         self.sm_data = sm_scvi_ad.X
         self.sm_labels = sm_scvi_ad.obsm['label'].values
         self.st_data = st_scvi_ad.X
         
         return sm_scvi_ad,st_scvi_ad
 
     
-    def build_dataset(self, batch_size, device):
+    def build_dataset(self, batch_size, device=None):
+        if device is None:
+            device = self.device
         x_train,y_train,x_test,y_test = data_utils.split_shuffle_data(np.array(self.sm_data,dtype=np.float32),np.array(self.sm_labels,dtype=np.float32))
         
         x_train = torch.tensor(x_train).to(device)
         y_train = torch.tensor(y_train).to(device)
         x_test = torch.tensor(x_test).to(device)
         y_test = torch.tensor(y_test).to(device)
         st_data = torch.tensor(self.st_data).to(device)
@@ -284,91 +272,85 @@
         
         g = torch.Generator()
         g.manual_seed(self.seed)
         self.sm_train_sampler = BatchSampler(RandomSampler(self.sm_train_ds, generator=g), batch_size=self.sm_train_batch_size, drop_last=True)
         self.sm_test_sampler = BatchSampler(RandomSampler(self.sm_test_ds, generator=g), batch_size=self.sm_test_batch_size, drop_last=True)
         self.st_sampler = BatchSampler(RandomSampler(self.st_ds, generator=g), batch_size=self.st_batch_size, drop_last=True)
     
-    def train_sm(self, data, labels, rec_w=0.5, infer_w=1):
+    def train_st(self, sm_data, st_data, rec_w=1, m_w=1):
         self.model.train()
-        self.sm_optimizer.zero_grad()
-        latent, predictions, rec_data = self.model(data)
-        rec_loss = self.kl_rec_loss_func(data, rec_data).mean() - self.cosine_rec_loss_func(data,rec_data).mean()
-        infer_loss = self.kl_infer_loss_func(labels,predictions).mean() - self.cosine_infer_loss_func(labels,predictions).mean()
-
-        regularization_params = torch.cat([
-            torch.cat([x.view(-1) for x in self.model.encoder[0].parameters()]),
-            torch.cat([x.view(-1) for x in self.model.encoder[3].parameters()]),
-            torch.cat([x.view(-1) for x in self.model.encoder[6].parameters()]),
-            torch.cat([x.view(-1) for x in self.model.decoder[0].parameters()]),
-            torch.cat([x.view(-1) for x in self.model.decoder[3].parameters()]),
-            torch.cat([x.view(-1) for x in self.model.decoder[6].parameters()]),
-            torch.cat([x.view(-1) for x in self.model.pred[0].parameters()]),
-        ])
-        l1_regularization = self.l1 * torch.norm(regularization_params, 1)
-        l2_regularization = self.l2 * torch.norm(regularization_params, 2)
-        l1_l2_loss = l1_regularization + l2_regularization
-        
-        loss = rec_w*rec_loss + infer_w*infer_loss # + l1_l2_loss
+        self.st_optimizer.zero_grad()
+        sm_latent, sm_predictions, sm_rec_data = self.model(sm_data)
+        st_latent, _, st_rec_data = self.model(st_data)
+        sm_rec_loss = self.kl_rec_loss_func(sm_data, sm_rec_data).mean() - self.cosine_rec_loss_func(sm_data, sm_rec_data).mean()
+        st_rec_loss = self.kl_rec_loss_func(st_data, st_rec_data).mean() - self.cosine_rec_loss_func(st_data, st_rec_data).mean()
+        mmd_loss = self.mmd_loss(sm_latent, st_latent)
+        loss = rec_w*sm_rec_loss + rec_w*st_rec_loss + m_w*mmd_loss
         loss.backward()
-        self.sm_optimizer.step()
-        return latent , loss, rec_loss, infer_loss
+        self.st_optimizer.step()
+        return loss, sm_rec_loss, st_rec_loss, mmd_loss
 
-    def train_st(self, data):
+    def train_sm(self, sm_data, sm_labels, infer_w=1):
         self.model.train()
-        self.st_optimizer.zero_grad()
-        latent, predictions, rec_data = self.model(data)
-        rec_loss = self.kl_rec_loss_func(data,rec_data).mean() - self.cosine_rec_loss_func(data,rec_data).mean()
-        regularization_params = torch.cat([
-            torch.cat([x.view(-1) for x in self.model.encoder[0].parameters()]),
-            torch.cat([x.view(-1) for x in self.model.encoder[3].parameters()]),
-            torch.cat([x.view(-1) for x in self.model.encoder[6].parameters()]),
-            torch.cat([x.view(-1) for x in self.model.decoder[0].parameters()]),
-            torch.cat([x.view(-1) for x in self.model.decoder[3].parameters()]),
-            torch.cat([x.view(-1) for x in self.model.decoder[6].parameters()]),
-            torch.cat([x.view(-1) for x in self.model.pred[0].parameters()]),
-        ])
-        l1_regularization = self.l1 * torch.norm(regularization_params, 1)
-        l2_regularization = self.l2 * torch.norm(regularization_params, 2)
-        l1_l2_loss = l1_regularization + l2_regularization
-        loss = rec_loss # + l1_l2_loss
+        self.sm_optimizer.zero_grad()
+        sm_latent, sm_predictions, sm_rec_data = self.model(sm_data)
+        infer_loss = 0
+        for loss in self.infer_losses:
+            if loss == 'kl':
+                infer_loss += self.kl_infer_loss_func(sm_labels, sm_predictions).mean()
+            elif loss == 'cos':
+                infer_loss -= self.cosine_infer_loss_func(sm_labels, sm_predictions).mean()
+            elif loss == 'rmse':
+                infer_loss += self.rmse_loss_func(sm_labels, sm_predictions)
+        loss = infer_w*infer_loss
         loss.backward()
-        self.st_optimizer.step()
-        return latent , rec_loss
+        self.sm_optimizer.step()
+        return loss, infer_loss
         
-    def test_sm(self, data, labels, rec_w=0.5, infer_w=1):
+    def test_st(self, sm_data, st_data, rec_w=1, m_w=1):
         self.model.eval()
-        latent, predictions, rec_data = self.model(data)
-        rec_loss = rec_w*(self.kl_rec_loss_func(data,rec_data).mean() - self.cosine_rec_loss_func(data,rec_data).mean())
-        infer_loss = infer_w*(self.kl_infer_loss_func(labels,predictions).mean() - self.cosine_infer_loss_func(labels,predictions).mean())
-        loss = rec_loss + infer_loss
-        return latent, loss, rec_loss, infer_loss
+        sm_latent, sm_predictions, sm_rec_data = self.model(sm_data)
+        st_latent, _, st_rec_data = self.model(st_data)
+        sm_rec_loss = self.kl_rec_loss_func(sm_data, sm_rec_data).mean() - self.cosine_rec_loss_func(sm_data, sm_rec_data).mean()
+        st_rec_loss = self.kl_rec_loss_func(st_data, st_rec_data).mean() - self.cosine_rec_loss_func(st_data, st_rec_data).mean()
+        mmd_loss = self.mmd_loss(sm_latent, st_latent)
+        loss = rec_w*sm_rec_loss + rec_w*st_rec_loss + m_w*mmd_loss
+        return loss, sm_rec_loss, st_rec_loss, mmd_loss
         
-    def test_st(self, data):
+    def test_sm(self, sm_data, sm_labels, infer_w=1):
         self.model.eval()
-        latent, predictions, rec_data = self.model(data)
-        rec_loss = self.kl_rec_loss_func(data,rec_data).mean() - self.cosine_rec_loss_func(data,rec_data).mean()
-        return latent , rec_loss
+        sm_latent, sm_predictions, sm_rec_data = self.model(sm_data)
+        infer_loss = 0
+        for loss in self.infer_losses:
+            if loss == 'kl':
+                infer_loss += self.kl_infer_loss_func(sm_labels, sm_predictions).mean()
+            elif loss == 'cos':
+                infer_loss -= self.cosine_infer_loss_func(sm_labels, sm_predictions).mean()
+            elif loss == 'rmse':
+                infer_loss += self.rmse_loss_func(sm_labels, sm_predictions)
+        loss = infer_w*infer_loss
+        return loss, infer_loss
     
     def train_model_by_step(
         self,
         max_steps=5000,
-        save_mode='best',
+        save_mode='all',
         save_path=None,
         prefix=None,
-        sm_step=4,
-        st_step=1,
-        test_step_gap=10,
+        sm_step=10,
+        st_step=10,
+        test_step_gap=1,
         convergence=0.001,
         early_stop=True,
-        early_stop_max=20,
+        early_stop_max=2000,
         sm_lr=None,
         st_lr=None,
-        rec_w=0.5, 
+        rec_w=1, 
         infer_w=1,
+        m_w=1,
     ):
         if len(self.history) > 0:
             best_ind = np.where(self.history['is_best'] == 'True')[0][-1]
             best_loss = self.history['sm_test_infer_loss'][best_ind]
             best_rec_loss = self.history['st_test_rec_loss'][best_ind]
         else:
             best_loss = np.inf
@@ -378,41 +360,40 @@
             for g in self.sm_optimizer.param_groups:
                 g['lr'] = sm_lr
         if st_lr is not None:
             for g in self.st_optimizer.param_groups:
                 g['lr'] = st_lr
 
         pbar = tqdm(range(max_steps))
-        mmd_loss = 0
         sm_trainr_iter = itertools.cycle(self.sm_train_sampler)
+        sm_test_iter = itertools.cycle(self.sm_test_sampler)
         st_iter = itertools.cycle(self.st_sampler)
-        sm_shuffle_step = max(int(len(self.sm_train_ds)/(self.sm_train_batch_size*sm_step)),1)
+        sm_train_shuffle_step = max(int(len(self.sm_train_ds)/(self.sm_train_batch_size*sm_step)),1)
+        sm_test_shuffle_step = max(int(len(self.sm_test_ds)/(self.sm_test_batch_size*sm_step)),1)
         st_shuffle_step = max(int(len(self.st_ds)/(self.st_batch_size*st_step)),1)
         for step in pbar:
-            if step % sm_shuffle_step == 0:
+            if step % sm_train_shuffle_step == 0:
                 sm_train_iter = itertools.cycle(self.sm_train_sampler)
+            if step % sm_test_shuffle_step == 0:
+                sm_test_iter = itertools.cycle(self.sm_test_sampler)
             if step % st_shuffle_step == 0:
                 st_iter = itertools.cycle(self.st_sampler)
+
+            st_exp = self.st_ds[next(st_iter)][0]
+            sm_exp, sm_proportion = self.sm_train_ds[next(sm_train_iter)]
             for i in range(st_step):
-                exp = self.st_ds[next(st_iter)][0]
-                st_latent, st_train_rec_loss = self.train_st(exp)
+                st_train_total_loss, sm_train_rec_loss, st_train_rec_loss, st_train_mmd_loss = self.train_st(sm_exp, st_exp, rec_w=rec_w, m_w=m_w)
             for i in range(sm_step):
-                exp, proportion = self.sm_train_ds[next(sm_train_iter)]
-                sm_latent, sm_train_total_loss, sm_train_rec_loss, sm_train_infer_loss = self.train_sm(exp, proportion, rec_w=rec_w, infer_w=infer_w)
-            # mmd_loss = compute_mmd(st_latent,sm_latent)*m_w
-
+                sm_train_total_loss, sm_train_infer_loss = self.train_sm(sm_exp, sm_proportion, infer_w=infer_w)
+            
             if step % test_step_gap == 0:
-                for ind in self.st_sampler:
-                    exp = self.st_ds[ind][0]
-                    st_latent, st_test_rec_loss = self.test_st(exp)
-                for ind in self.sm_test_sampler:
-                    exp, proportion = self.sm_test_ds[ind]
-                    sm_latent, sm_test_total_loss, sm_test_rec_loss, sm_test_infer_loss = self.test_sm(exp,proportion, rec_w=rec_w, infer_w=infer_w)
-                # mmd_loss = compute_mmd(st_latent,sm_latent)*m_w
-
+                sm_test_exp, sm_test_proportion = self.sm_test_ds[next(sm_test_iter)]
+                st_test_total_loss, sm_test_rec_loss, st_test_rec_loss, st_test_mmd_loss = self.test_st(sm_test_exp, st_exp, rec_w=rec_w, m_w=m_w)
+                sm_test_total_loss, sm_test_infer_loss = self.test_sm(sm_test_exp, sm_test_proportion, infer_w=infer_w)
+                
                 current_infer_loss = sm_test_infer_loss.item()
 
                 best_flag='False'
                 if best_loss - current_infer_loss > convergence:
                     if best_loss > current_infer_loss:
                         best_loss = current_infer_loss
                     best_flag='True'
@@ -428,142 +409,169 @@
                             if os.path.exists(old_best_path):
                                 os.remove(old_best_path)
                         torch.save(self.model.state_dict(), self.best_path)
                 else:
                     early_stop_count += 1
                     
                 if save_mode == 'all':
-                    if prefix != '':
+                    if prefix is not None:
                         self.best_path = os.path.join(save_path,prefix+'_'+f'celleagle_weights_step{step}.h5')
                     else:
                         self.best_path = os.path.join(save_path,f'celleagle_weights_step{step}.h5')
                     torch.save(self.model.state_dict(), self.best_path)
-                    
-                self.history = self.history.append({
-                    'sm_train_rec_loss':sm_train_rec_loss.item(),
-                    'sm_train_infer_loss':sm_train_infer_loss.item(),
-                    'sm_train_total_loss':sm_train_total_loss.item(),
-                    'sm_test_rec_loss':sm_test_rec_loss.item(),
-                    'sm_test_infer_loss':sm_test_infer_loss.item(),
-                    'sm_test_total_loss':sm_test_total_loss.item(),
-                    'st_train_rec_loss':st_train_rec_loss.item(),
-                    'st_test_rec_loss':st_test_rec_loss.item(),
-                    'is_best':best_flag
-                }, ignore_index=True)
+                
+                self.history = pd.concat([
+                    self.history,
+                    pd.DataFrame({
+                        'sm_train_infer_loss':sm_train_infer_loss.item(),
+                        'sm_train_rec_loss':sm_train_infer_loss.item(),
+                        'sm_test_rec_loss':sm_test_rec_loss.item(),
+                        'sm_test_infer_loss':sm_test_infer_loss.item(),
+                        'st_train_rec_loss':st_train_rec_loss.item(),
+                        'st_test_rec_loss':st_test_rec_loss.item(),
+                        'st_train_mmd_loss':st_train_rec_loss.item(),
+                        'st_test_mmd_loss':st_test_rec_loss.item(),
+                        'is_best':best_flag
+                    },index=[0])
+                ]).reset_index(drop=True)
 
-                pbar.set_description(f"Step {step + 1}: test inf loss={sm_test_infer_loss.item():.3f}, train inf loss={sm_train_infer_loss.item():.3f}, test rec loss={sm_test_rec_loss.item():.3f}, train rec loss={sm_train_rec_loss.item():.3f}, st test rec loss={st_test_rec_loss.item():.3f}",refresh=True)
+                pbar.set_description(f"Step {step + 1}: Test inference loss={sm_test_infer_loss.item():.3f}",refresh=True)
                 
                 if (early_stop_count > early_stop_max) and early_stop:
                     print('Stop trainning because of loss convergence')
                     break
-            
+    
+    def train_model(
+        self,
+        max_steps=5000,
+        save_mode='all',
+        save_path=None,
+        prefix=None,
+        sm_step=10,
+        st_step=10,
+        test_step_gap=1,
+        convergence=0.001,
+        early_stop=False,
+        early_stop_max=2000,
+        sm_lr=None,
+        st_lr=None,
+        batch_size=1024,
+        rec_w=1, 
+        infer_w=1,
+        m_w=1,
+    ):
+        """Training Spoint model.
+        
+        Training Spoint model.
+
+        Args:
+            max_steps: The max step of training. The training process will be stop when achive max step.
+            save_mode: A string determinates how the model is saved. It must be one of 'best' and 'all'.
+            save_path: A string representing the path directory where the model is saved.
+            prefix: A string added to the prefix of file name of saved model.
+            convergence: The threshold of early stop.
+            early_stop: If True, turn on early stop.
+            early_stop_max: The max steps of loss difference less than convergence.
+            sm_lr: Learning rate for simulated data.
+            st_lr: Learning rate for spatial transcriptomic data.
+            disc_lr: Learning rate of discriminator.
+            batch_size: Batch size of the data be feeded in model once.
+            rec_w: The weight of reconstruction loss.
+            infer_w: The weig ht of inference loss.
+            m_w: The weight of MMD loss.
+        
+        Returns:
+            ``None``
+        """
+        self.init_model()
+        self.train_model_by_step(
+            max_steps=max_steps,
+            save_mode=save_mode,
+            save_path=save_path,
+            prefix=prefix,
+            sm_step=sm_step,
+            st_step=st_step,
+            test_step_gap=test_step_gap,
+            convergence=convergence,
+            early_stop=early_stop,
+            early_stop_max=early_stop_max,
+            sm_lr=sm_lr,
+            st_lr=st_lr,
+            rec_w=rec_w, 
+            infer_w=infer_w,
+            m_w=m_w
+        )
+                        
     def train(
         self,
-        max_steps=20000,
-        save_mode='best',
+        max_steps=5000,
+        save_mode='all',
         save_path=None,
         prefix=None,
-        sm_step=4,
-        st_step=1,
-        test_step_gap=10,
+        sm_step=10,
+        st_step=10,
+        test_step_gap=1,
         convergence=0.001,
-        early_stop=True,
-        early_stop_max=200,
+        early_stop=False,
+        early_stop_max=2000,
         sm_lr=None,
         st_lr=None,
-        batch_size=4096,
-        rec_w=0.5, 
+        batch_size=1024,
+        rec_w=1, 
         infer_w=1,
+        m_w=1,
         scvi_max_epochs=100,
         scvi_early_stopping=True,
         scvi_batch_size=4096,
     ):
         """Training Spoint model.
         
-        Obtain latent feature from scVI then feed in Spoint model for training until loss convengence.
+        Obtain latent feature from scVI then feed in Spoint model for training.
 
         Args:
             max_steps: The max step of training. The training process will be stop when achive max step.
             save_mode: A string determinates how the model is saved. It must be one of 'best' and 'all'.
             save_path: A string representing the path directory where the model is saved.
             prefix: A string added to the prefix of file name of saved model.
             convergence: The threshold of early stop.
             early_stop: If True, turn on early stop.
             early_stop_max: The max steps of loss difference less than convergence.
             sm_lr: Learning rate for simulated data.
             st_lr: Learning rate for spatial transcriptomic data.
-            disc_lr: Learning rate of discriminator.
             batch_size: Batch size of the data be feeded in model once.
             rec_w: The weight of reconstruction loss.
             infer_w: The weig ht of inference loss.
             m_w: The weight of MMD loss.
             scvi_max_epochs: The max epoch of scVI.
             scvi_batch_size: The batch size of scVI.
-        
         Returns:
             ``None``
         """
-        if self.use_rep == 'scvi':
-            self.get_scvi_latent(
-                n_layers=self.scvi_layers,
-                n_latent=self.scvi_latent,
-                gene_likelihood=self.scvi_gene_likelihood,
-                dispersion=self.scvi_dispersion,
-                max_epochs=scvi_max_epochs,
-                early_stopping=scvi_early_stopping,
-                batch_size=scvi_batch_size,
-            )
-        elif self.use_rep == 'X':
-            if issparse(self.sm_ad.X):
-                self.sm_data = self.sm_ad.X.toarray()
-            else:
-                self.sm_data = self.sm_ad.X
-            self.sm_labels = self.sm_ad.obsm['label'].values
-            if issparse(self.st_ad.X):
-                self.st_data = self.st_ad.X.toarray()
-            else:
-                self.st_data = self.st_ad.X            
-        elif self.use_rep == 'pca':
-            if issparse(self.sm_ad.X):
-                self.sm_data = self.sm_ad.X.toarray()
-            else:
-                self.sm_data = self.sm_ad.X
-            self.sm_labels = self.sm_ad.obsm['label'].values
-            if issparse(self.st_ad.X):
-                self.st_data = self.st_ad.X.toarray()
-            else:
-                self.st_data = self.st_ad.X
-            
-            pca_data = np.concatenate([self.st_data,self.sm_data],axis=0)
-            pca = PCA(n_components=50)
-            pca.fit(pca_data)
-            pca_data = pca.transform(pca_data)
-            self.st_data = pca_data[:self.st_data.shape[0],:]
-            self.sm_data = pca_data[self.st_data.shape[0]:,:]
-
-        self.build_dataset(batch_size, self.device)
         if save_path is None:
-            save_path = 'Spoint_models_'+strftime("%Y%m%d%H%M%S",localtime())
+            save_path = os.path.join(tempfile.gettempdir() ,'Spoint_models_'+strftime("%Y%m%d%H%M%S",localtime()))
         if not os.path.exists(save_path):
             os.makedirs(save_path)
-        self.train_model_by_step(
+        self.get_scvi_latent(max_epochs=scvi_max_epochs, early_stopping=scvi_early_stopping, batch_size=scvi_batch_size)
+        self.build_dataset(batch_size)
+        self.train_model(
             max_steps=max_steps,
             save_mode=save_mode,
             save_path=save_path,
             prefix=prefix,
             sm_step=sm_step,
             st_step=st_step,
             test_step_gap=test_step_gap,
             convergence=convergence,
             early_stop=early_stop,
             early_stop_max=early_stop_max,
             sm_lr=sm_lr,
             st_lr=st_lr,
             rec_w=rec_w, 
             infer_w=infer_w,
+            m_w=m_w
         )
     
     def eval_model(self,model_path=None,use_best_model=True,batch_size=4096,metric='pcc'):
         if metric=='pcc':
             metric_name = 'PCC'
             func = metrics.pcc
         if metric=='spcc':
```

### Comparing `SPACEL-1.0.1/SPACEL/Spoint/data_augmentation.py` & `SPACEL-1.1.1/SPACEL/Spoint/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.0.1/SPACEL/Spoint/data_downsample.py` & `SPACEL-1.1.1/SPACEL/Spoint/data_downsample.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.0.1/SPACEL/Spoint/data_utils.py` & `SPACEL-1.1.1/SPACEL/Spoint/data_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,16 +109,16 @@
 def check_data_type(ad):
     if issparse(ad.X):
         ad.X = ad.X.toarray()
     if ad.X.dtype != np.float32:
         ad.X =ad.X.astype(np.float32)
     return ad
 
-def generate_sm_adata(sc_ad,num_sample,celltype_key,n_threads,cell_counts,clusters_mean,cells_mean,cells_min,cells_max):
-    sm_data,sm_labels = spatial_simulation.generate_simulation_data(sc_ad,num_sample=num_sample,celltype_key=celltype_key,downsample_fraction=None,data_augmentation=False,n_cpus=n_threads,cell_counts=cell_counts,clusters_mean=clusters_mean,cells_mean=cells_mean,cells_min=cells_min,cells_max=cells_max)
+def generate_sm_adata(sc_ad,num_sample,celltype_key,n_threads,cell_counts,clusters_mean,cells_mean,cells_min,cells_max,cell_sample_counts,cluster_sample_counts,ncell_sample_list,cluster_sample_list):
+    sm_data,sm_labels = spatial_simulation.generate_simulation_data(sc_ad,num_sample=num_sample,celltype_key=celltype_key,downsample_fraction=None,data_augmentation=False,n_cpus=n_threads,cell_counts=cell_counts,clusters_mean=clusters_mean,cells_mean=cells_mean,cells_min=cells_min,cells_max=cells_max,cell_sample_counts=cell_sample_counts,cluster_sample_counts=cluster_sample_counts,ncell_sample_list=ncell_sample_list,cluster_sample_list=cluster_sample_list)
     sm_data_mtx = csr_matrix(sm_data)
     sm_ad = anndata.AnnData(sm_data_mtx)
     sm_ad.var.index = sc_ad.var_names
     sm_labels = (sm_labels.T/sm_labels.sum(axis=1)).T
     sm_ad.obsm['label'] = pd.DataFrame(sm_labels,columns=np.array(sc_ad.obs[celltype_key].value_counts().index.values),index=sm_ad.obs_names)
     return sm_ad
```

### Comparing `SPACEL-1.0.1/SPACEL/Spoint/metrics.py` & `SPACEL-1.1.1/SPACEL/Spoint/metrics.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.0.1/SPACEL/Spoint/model.py` & `SPACEL-1.1.1/SPACEL/Spoint/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,32 +20,37 @@
     celltype_key,
     sc_genes=None,
     st_genes=None,
     used_genes=None,
     deg_method:str='wilcoxon',
     n_top_markers:int=200,
     n_top_hvg:int=None,
-    log2fc_min=0.5, 
-    pval_cutoff=0.01, 
+    log2fc_min=0.5,
+    pval_cutoff=0.01,
     pct_diff=None, 
     pct_min=0.1,
     use_rep='scvi',
     st_batch_key=None,
     sm_size:int=500000,
     cell_counts=None,
     clusters_mean=None,
     cells_mean=10,
     cells_min=1,
     cells_max=20,
+    cell_sample_counts=None,
+    cluster_sample_counts=None,
+    ncell_sample_list=None,
+    cluster_sample_list=None,
     scvi_layers=2,
-    scvi_latent=64,
+    scvi_latent=128,
     scvi_gene_likelihood='zinb',
     scvi_dispersion='gene-batch',
-    latent_dims=32, 
+    latent_dims=128, 
     hidden_dims=512,
+    infer_losses=['kl','cos'],
     n_threads=4,
     seed=42,
     use_gpu=None
 ):
     """Initialize Spoint model.
     
     Given specific data and parameters to initialize Spoint model.
@@ -96,15 +101,15 @@
         sc_genes=sc_genes,
         st_genes=st_genes,
         log2fc_min=log2fc_min, 
         pval_cutoff=pval_cutoff, 
         pct_diff=pct_diff, 
         pct_min=pct_min
     )
-    sm_ad = data_utils.generate_sm_adata(sc_ad,num_sample=sm_size,celltype_key=celltype_key,n_threads=n_threads,cell_counts=cell_counts,clusters_mean=clusters_mean,cells_mean=cells_mean,cells_min=cells_min,cells_max=cells_max)
+    sm_ad = data_utils.generate_sm_adata(sc_ad,num_sample=sm_size,celltype_key=celltype_key,n_threads=n_threads,cell_counts=cell_counts,clusters_mean=clusters_mean,cells_mean=cells_mean,cells_min=cells_min,cells_max=cells_max,cell_sample_counts=cell_sample_counts,cluster_sample_counts=cluster_sample_counts,ncell_sample_list=ncell_sample_list,cluster_sample_list=cluster_sample_list)
     data_utils.downsample_sm_spot_counts(sm_ad,st_ad,n_threads=n_threads)
 
     model = base_model.SpointModel(
         st_ad,
         sm_ad,
         clusters = np.array(sm_ad.obsm['label'].columns),
         spot_names = np.array(st_ad.obs_names),
@@ -113,11 +118,12 @@
         st_batch_key=st_batch_key,
         scvi_layers=scvi_layers,
         scvi_latent=scvi_latent,
         scvi_gene_likelihood=scvi_gene_likelihood,
         scvi_dispersion=scvi_dispersion,
         latent_dims=latent_dims, 
         hidden_dims=hidden_dims,
+        infer_losses=infer_losses,
         use_gpu=use_gpu,
         seed=seed
     )
     return model
```

### Comparing `SPACEL-1.0.1/SPACEL/Spoint/spatial_simulation.py` & `SPACEL-1.1.1/SPACEL/Spoint/spatial_simulation.py`

 * *Files 22% similar despite different names*

```diff
@@ -65,15 +65,41 @@
     density = np.empty((len(param_list), sample_cluster.shape[1]),dtype=np.float32)
 
     for i in nb.prange(len(param_list)):
         params = param_list[i]
         num_cell = params[0]
         num_cluster = params[1]
         used_clusters = clusters[np.searchsorted(np.cumsum(cluster_p), np.random.rand(num_cluster), side="right")]
-        cluster_mask=np.array([False]*len(cluster_id))
+        cluster_mask = np.array([False]*len(cluster_id))
+        for c in used_clusters:
+            cluster_mask = (cluster_id==c)|(cluster_mask)
+        # print('cluster_mask',cluster_mask)
+        # print('used_clusters',used_clusters)
+        used_cell_ind = np.where(cluster_mask)[0]
+        used_cell_p = cell_p_balanced[cluster_mask]
+        used_cell_p = used_cell_p/used_cell_p.sum()
+        sampled_cells = used_cell_ind[np.searchsorted(np.cumsum(used_cell_p), np.random.rand(num_cell), side="right")]
+        combined_exp = np_sum(sample_exp[sampled_cells,:],axis=0).astype(np.float32)
+        if data_augmentation:
+            combined_exp = random_augmentation_cell(combined_exp,max_rate=max_rate,max_val=max_val,kth=kth)
+        if downsample_fraction is not None:
+            combined_exp = downsample_cell(combined_exp, downsample_fraction)
+        combined_clusters = np_sum(sample_cluster[cluster_id[sampled_cells]],axis=0).astype(np.float32)
+        exp[i,:] = combined_exp
+        density[i,:] = combined_clusters
+    return exp,density
+
+@jit(nopython=True,parallel=True)
+def sample_cell_from_clusters(cluster_sample_list,ncell_sample_list,cluster_id,sample_exp,sample_cluster,cell_p_balanced,downsample_fraction=None,data_augmentation=True,max_rate=0.8,max_val=0.8,kth=0.2):
+    exp = np.empty((len(cluster_sample_list), sample_exp.shape[1]),dtype=np.float32)
+    density = np.empty((len(cluster_sample_list), sample_cluster.shape[1]),dtype=np.float32)
+    for i in nb.prange(len(cluster_sample_list)):
+        used_clusters = np.where(cluster_sample_list[i] == 1)[0]
+        num_cell = ncell_sample_list[i]
+        cluster_mask = np.array([False]*len(cluster_id))
         for c in used_clusters:
             cluster_mask = (cluster_id==c)|(cluster_mask)
         used_cell_ind = np.where(cluster_mask)[0]
         used_cell_p = cell_p_balanced[cluster_mask]
         used_cell_p = used_cell_p/used_cell_p.sum()
         sampled_cells = used_cell_ind[np.searchsorted(np.cumsum(used_cell_p), np.random.rand(num_cell), side="right")]
         combined_exp = np_sum(sample_exp[sampled_cells,:],axis=0).astype(np.float32)
@@ -186,98 +212,140 @@
     downsample_fraction=None,
     data_augmentation=True,
     max_rate=0.8,max_val=0.8,kth=0.2,
     cells_min=1,cells_max=20,
     cells_mean=10,cells_std=5,
     clusters_mean=None,clusters_std=None,
     clusters_min=None,clusters_max=None,
+    cell_sample_counts=None,cluster_sample_counts=None,
+    ncell_sample_list=None,
+    cluster_sample_list=None,
     n_cpus=None
 ):
     if not 'cluster_p_unbalance' in sc_ad.uns:
         sc_ad = init_sample_prob(sc_ad,celltype_key)
     num_sample_per_mode = num_sample//len(balance_mode)
     cluster_ordered = np.array(sc_ad.obs['celltype_num'].value_counts().index)
-#     print(cluster_ordered)
     cluster_num = len(cluster_ordered)
-#     print(cluster_num)
     cluster_id = sc_ad.obs['celltype_num'].values
-#     print(cluster_id)
     cluster_mask = np.eye(cluster_num)
-#     print(cluster_mask)
-    
-    if cell_counts is not None:
-        cells_mean = np.mean(np.sort(cell_counts)[int(len(cell_counts)*0.05):int(len(cell_counts)*0.95)])
-        cells_std = np.std(np.sort(cell_counts)[int(len(cell_counts)*0.05):int(len(cell_counts)*0.95)])
-        cells_min = int(np.min(np.sort(cell_counts)[int(len(cell_counts)*0.05):int(len(cell_counts)*0.95)]))
-        cells_max = int(np.max(np.sort(cell_counts)[int(len(cell_counts)*0.05):int(len(cell_counts)*0.95)]))
-    if clusters_mean is None:
-        clusters_mean = cells_mean/2
-    if clusters_std is None:
-        clusters_std = cells_std/2
-    if clusters_min is None:
-        clusters_min = cells_min
-    if clusters_max is None:
-        clusters_max = np.min((cells_max//2,cluster_num))
-            
-    if cell_counts is not None:
-        cell_counts, cluster_count = get_param_from_cell_counts(num_sample_per_mode,cell_counts,cluster_sample_method,cells_mean=cells_mean,cells_std=cells_std,cells_max=cells_max,cells_min=cells_min,clusters_mean=clusters_mean,clusters_std=clusters_std,clusters_min=clusters_min,clusters_max=clusters_max)
-    elif cell_sample_method == 'gaussian':
-        cell_counts, cluster_count = get_param_from_gaussian(num_sample_per_mode,cells_mean=cells_mean,cells_std=cells_std,cells_max=cells_max,cells_min=cells_min,clusters_mean=clusters_mean,clusters_std=clusters_std)
-    elif cell_sample_method == 'uniform':
-        cell_counts, cluster_count = get_param_from_uniform(num_sample_per_mode,cells_max=cells_max,cells_min=cells_min,clusters_min=clusters_min,clusters_max=clusters_max)
-    else:
-        raise TypeError('Not correct sample method.')
-    params = np.array(list(zip(cell_counts, cluster_count)))
-
-    sample_data_list = []
-    sample_labels_list = []
-    for b in balance_mode:
-        print(f'### Genetating simulated spatial data using scRNA data with mode: {b}')
-        cluster_p = get_cluster_sample_prob(sc_ad,b)
-        if downsample_fraction is not None:
-            if downsample_fraction > 0.035:
+    if (cell_sample_counts is None) or (cluster_sample_counts is None):
+        if cell_counts is not None:
+            cells_mean = np.mean(np.sort(cell_counts)[int(len(cell_counts)*0.05):int(len(cell_counts)*0.95)])
+            cells_std = np.std(np.sort(cell_counts)[int(len(cell_counts)*0.05):int(len(cell_counts)*0.95)])
+            cells_min = int(np.min(np.sort(cell_counts)[int(len(cell_counts)*0.05):int(len(cell_counts)*0.95)]))
+            cells_max = int(np.max(np.sort(cell_counts)[int(len(cell_counts)*0.05):int(len(cell_counts)*0.95)]))
+        if clusters_mean is None:
+            clusters_mean = cells_mean/2
+        if clusters_std is None:
+            clusters_std = cells_std/2
+        if clusters_min is None:
+            clusters_min = cells_min
+        if clusters_max is None:
+            clusters_max = np.min((cells_max//2,cluster_num))
+
+        if cell_counts is not None:
+            cell_sample_counts, cluster_sample_counts = get_param_from_cell_counts(num_sample_per_mode,cell_counts,cluster_sample_method,cells_mean=cells_mean,cells_std=cells_std,cells_max=cells_max,cells_min=cells_min,clusters_mean=clusters_mean,clusters_std=clusters_std,clusters_min=clusters_min,clusters_max=clusters_max)
+        elif cell_sample_method == 'gaussian':
+            cell_sample_counts, cluster_sample_counts = get_param_from_gaussian(num_sample_per_mode,cells_mean=cells_mean,cells_std=cells_std,cells_max=cells_max,cells_min=cells_min,clusters_mean=clusters_mean,clusters_std=clusters_std)
+        elif cell_sample_method == 'uniform':
+            cell_sample_counts, cluster_sample_counts = get_param_from_uniform(num_sample_per_mode,cells_max=cells_max,cells_min=cells_min,clusters_min=clusters_min,clusters_max=clusters_max)
+        else:
+            raise TypeError('Not correct sample method.')
+    if cluster_sample_list is None or ncell_sample_list is None:
+        params = np.array(list(zip(cell_sample_counts, cluster_sample_counts)))
+
+        sample_data_list = []
+        sample_labels_list = []
+        for b in balance_mode:
+            print(f'### Genetating simulated spatial data using scRNA data with mode: {b}')
+            cluster_p = get_cluster_sample_prob(sc_ad,b)
+            if downsample_fraction is not None:
+                if downsample_fraction > 0.035:
+                    sample_data,sample_labels = sample_cell(
+                        param_list=params,
+                        cluster_p=cluster_p,
+                        clusters=cluster_ordered,
+                        cluster_id=cluster_id,
+                        sample_exp=generate_sample_array(sc_ad,used_genes),
+                        sample_cluster=cluster_mask,
+                        cell_p_balanced=sc_ad.obs['cell_p_balanced'].values,
+                        downsample_fraction=downsample_fraction,
+                        data_augmentation=data_augmentation,max_rate=max_rate,max_val=max_val,kth=kth,
+                    )
+                else:
+                    sample_data,sample_labels = sample_cell(
+                        param_list=params,
+                        cluster_p=cluster_p,
+                        clusters=cluster_ordered,
+                        cluster_id=cluster_id,
+                        sample_exp=generate_sample_array(sc_ad,used_genes),
+                        sample_cluster=cluster_mask,
+                        cell_p_balanced=sc_ad.obs['cell_p_balanced'].values,
+                        data_augmentation=data_augmentation,max_rate=max_rate,max_val=max_val,kth=kth,
+                    )
+                    # logging.warning('### Downsample data with python backend')
+                    sample_data = downsample_matrix_by_cell(sample_data, downsample_fraction, n_cpus=n_cpus, numba_end=False)
+            else:
                 sample_data,sample_labels = sample_cell(
                     param_list=params,
                     cluster_p=cluster_p,
                     clusters=cluster_ordered,
                     cluster_id=cluster_id,
                     sample_exp=generate_sample_array(sc_ad,used_genes),
                     sample_cluster=cluster_mask,
                     cell_p_balanced=sc_ad.obs['cell_p_balanced'].values,
-                    downsample_fraction=downsample_fraction,
                     data_augmentation=data_augmentation,max_rate=max_rate,max_val=max_val,kth=kth,
                 )
+    #         if data_augmentation:
+    #             sample_data = random_augment(sample_data)
+            sample_data_list.append(sample_data)
+            sample_labels_list.append(sample_labels)
+    else:
+        sample_data_list = []
+        sample_labels_list = []
+        for b in balance_mode:
+            print(f'### Genetating simulated spatial data using scRNA data with mode: {b}')
+            cluster_p = get_cluster_sample_prob(sc_ad,b)
+            if downsample_fraction is not None:
+                if downsample_fraction > 0.035:
+                    sample_data,sample_labels = sample_cell_from_clusters(
+                        cluster_sample_list=cluster_sample_list,
+                        ncell_sample_list=ncell_sample_list,
+                        cluster_id=cluster_id,
+                        sample_exp=generate_sample_array(sc_ad,used_genes),
+                        sample_cluster=cluster_mask,
+                        cell_p_balanced=sc_ad.obs['cell_p_balanced'].values,
+                        downsample_fraction=downsample_fraction,
+                        data_augmentation=data_augmentation,max_rate=max_rate,max_val=max_val,kth=kth,
+                    )
+                else:
+                    sample_data,sample_labels = sample_cell_from_clusters(
+                        cluster_sample_list=cluster_sample_list,
+                        ncell_sample_list=ncell_sample_list,
+                        cluster_id=cluster_id,
+                        sample_exp=generate_sample_array(sc_ad,used_genes),
+                        sample_cluster=cluster_mask,
+                        cell_p_balanced=sc_ad.obs['cell_p_balanced'].values,
+                        data_augmentation=data_augmentation,max_rate=max_rate,max_val=max_val,kth=kth,
+                    )
+                    # logging.warning('### Downsample data with python backend')
+                    sample_data = downsample_matrix_by_cell(sample_data, downsample_fraction, n_cpus=n_cpus, numba_end=False)
             else:
-                sample_data,sample_labels = sample_cell(
-                    param_list=params,
-                    cluster_p=cluster_p,
-                    clusters=cluster_ordered,
+                sample_data,sample_labels = sample_cell_from_clusters(
+                    cluster_sample_list=cluster_sample_list,
+                    ncell_sample_list=ncell_sample_list,
                     cluster_id=cluster_id,
                     sample_exp=generate_sample_array(sc_ad,used_genes),
                     sample_cluster=cluster_mask,
                     cell_p_balanced=sc_ad.obs['cell_p_balanced'].values,
                     data_augmentation=data_augmentation,max_rate=max_rate,max_val=max_val,kth=kth,
                 )
-                # logging.warning('### Downsample data with python backend')
-                sample_data = downsample_matrix_by_cell(sample_data, downsample_fraction, n_cpus=n_cpus, numba_end=False)
-        else:
-            sample_data,sample_labels = sample_cell(
-                param_list=params,
-                cluster_p=cluster_p,
-                clusters=cluster_ordered,
-                cluster_id=cluster_id,
-                sample_exp=generate_sample_array(sc_ad,used_genes),
-                sample_cluster=cluster_mask,
-                cell_p_balanced=sc_ad.obs['cell_p_balanced'].values,
-                data_augmentation=data_augmentation,max_rate=max_rate,max_val=max_val,kth=kth,
-            )
-#         if data_augmentation:
-#             sample_data = random_augment(sample_data)
-        sample_data_list.append(sample_data)
-        sample_labels_list.append(sample_labels)
+            sample_data_list.append(sample_data)
+            sample_labels_list.append(sample_labels)
     return np.concatenate(sample_data_list), np.concatenate(sample_labels_list)
 
 @jit(nopython=True,parallel=True)
 def sample_cell_exp(cell_counts,sample_exp,cell_p,downsample_fraction=None,data_augmentation=True,max_rate=0.8,max_val=0.8,kth=0.2):
     exp = np.empty((len(cell_counts), sample_exp.shape[1]),dtype=np.float32)
     ind = np.zeros((len(cell_counts), np.max(cell_counts)),dtype=np.int32)
     cell_ind = np.arange(sample_exp.shape[0])
```

### Comparing `SPACEL-1.0.1/SPACEL/__init__.py` & `SPACEL-1.1.1/SPACEL/__init__.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.0.1/SPACEL/setting.py` & `SPACEL-1.1.1/SPACEL/setting.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.0.1/SPACEL.egg-info/PKG-INFO` & `SPACEL-1.1.1/SPACEL.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 Metadata-Version: 2.1
 Name: SPACEL
-Version: 1.0.1
+Version: 1.1.1
 Summary: SPACEL: characterizing spatial transcriptome architectures by deep-learning
 Home-page: https://github.com/QuKunLab/SPACEL
 Author: Hao Xu
 Author-email: xuhaoustc@mail.ustc.edu.cn
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/spacel/badge/?version=latest)](https://spacel.readthedocs.io/en/latest/?badge=latest)
+![PyPI](https://img.shields.io/pypi/v/SPACEL)
 
 # SPACEL: characterizing spatial transcriptome architectures by deep-learning
 
 ![](docs/_static/img/figure1.png "Overview")
 SPACEL (**SP**atial **A**rchitecture **C**haracterization by d**E**ep **L**earning) is a Python package of deep-learning-based methods for ST data analysis. SPACEL consists of three modules: 
 * Spoint embedded a multiple-layer perceptron with a probabilistic model to deconvolute cell type composition for each spot on single ST slice.
 * Splane employs a graph convolutional network approach and an adversarial learning algorithm to identify uniform spatial domains that are transcriptomically and spatially coherent across multiple ST slices.
 * Scube automatically transforms the spatial coordinate systems of consecutive slices and stacks them together to construct a three-dimensional (3D) alignment of the tissue.
 
 ## Getting started
 * [Requirements](#Requirements)
 * [Installation](#Installation)
 * Tutorials
-    * [Spoint tutorial: Deconvolution of cell types distribution of spatial transcriptomics](docs/tutorials/deconvolution_of_cell_types_distribution.ipynb)
-    * [Splane tutorial: Identify uniform spatial domain in multiple slices](docs/tutorials/identification_of_uniform_spatial_domain.ipynb)
-    * [Scube tutorial: Alignment of multiple spatial transcriptomic slices](docs/tutorials/alignment_of_multiple_slices.ipynb)
+    * [Spoint tutorial: Deconvolution of cell types compostion on human brain Visium dataset](docs/tutorials/deconvolution_of_cell_types_distribution.ipynb)
+    * [Splane tutorial: Identify uniform spatial domain on human breast cancer Visium dataset](docs/tutorials/identification_of_uniform_spatial_domain.ipynb)
+    * [Scube tutorial: Alignment of consecutive ST slices on human brain MERFISH dataset](docs/tutorials/alignment_of_multiple_slices.ipynb)
     * [Scube tutorial: 3D expression modeling with gaussian process regression](docs/tutorials/3D_expression_modeling.ipynb)
 
 Read the [documentation](https://spacel.readthedocs.io) for more information.
+
+## Latest updates
+### Version 1.1.1 2023-07-11
+#### Features
+* All code based on `Tensorflow` have been mirated to `PyTorch`, it does not have `Tensorflow` as dependency anymore.
+* The `Splane.utils.add_cell_type_composition` function has been implemented to facilitate the cell type composition predicted by deconvolution methods into Splane.
+* Spoint and Splane now support tqdm type output for improved progress tracking.
     
 ## Requirements
 
 To install `SPACEL`, you need to install [PyTorch](https://pytorch.org) with GPU support first. If you don't need GPU acceleration, you can just skip the installation for `cudnn` and `cudatoolkit`.
 * Create conda environment for `SPACEL`:
 ```
 conda env create -f environment.yml
```

### Comparing `SPACEL-1.0.1/SPACEL.egg-info/SOURCES.txt` & `SPACEL-1.1.1/SPACEL.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 SPACEL.egg-info/top_level.txt
 SPACEL/Scube/__init__.py
 SPACEL/Scube/alignment.py
 SPACEL/Scube/gpr.py
 SPACEL/Scube/plot.py
 SPACEL/Scube/utils_3d.py
 SPACEL/Splane/__init__.py
+SPACEL/Splane/base_model.py
 SPACEL/Splane/graph.py
 SPACEL/Splane/model.py
 SPACEL/Splane/pygcn_utils.py
 SPACEL/Splane/utils.py
 SPACEL/Splane/kegra/__init__.py
 SPACEL/Splane/kegra/gnn.py
 SPACEL/Splane/kegra/gnn_utils.py
```

### Comparing `SPACEL-1.0.1/setup.py` & `SPACEL-1.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,11 +25,12 @@
         "scvi-tools",
         "scipy",
         "scikit-learn",
         "matplotlib",
         "seaborn",
         "scanpy",
         "numba",
+        "torch<=1.13",
         "gpytorch",
         "torchmetrics",
     ],
 )
```

