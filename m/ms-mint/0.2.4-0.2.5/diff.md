# Comparing `tmp/ms-mint-0.2.4.tar.gz` & `tmp/ms-mint-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms-mint-0.2.4.tar", last modified: Tue May  9 16:42:49 2023, max compression
+gzip compressed data, was "ms-mint-0.2.5.tar", last modified: Tue Jul 11 19:38:41 2023, max compression
```

## Comparing `ms-mint-0.2.4.tar` & `ms-mint-0.2.5.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:42:49.036971 ms-mint-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-05-09 16:42:32.000000 ms-mint-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-09 16:42:32.000000 ms-mint-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-05-09 16:42:49.036971 ms-mint-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-05-09 16:42:32.000000 ms-mint-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:42:49.036971 ms-mint-0.2.4/ms_mint/
--rw-r--r--   0 runner    (1001) docker     (123)    15871 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/Mint.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 16:42:49.036971 ms-mint-0.2.4/ms_mint/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/chromatogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/matplotlib_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/plotly_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/standards.py
--rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:42:49.036971 ms-mint-0.2.4/ms_mint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-05-09 16:42:48.000000 ms-mint-0.2.4/ms_mint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-09 16:42:49.000000 ms-mint-0.2.4/ms_mint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:42:48.000000 ms-mint-0.2.4/ms_mint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-09 16:42:48.000000 ms-mint-0.2.4/ms_mint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 16:42:48.000000 ms-mint-0.2.4/ms_mint.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:42:49.036971 ms-mint-0.2.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-09 16:42:32.000000 ms-mint-0.2.4/scripts/ms-mint-convert.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-05-09 16:42:49.036971 ms-mint-0.2.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-05-09 16:42:32.000000 ms-mint-0.2.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68780 2023-05-09 16:42:33.000000 ms-mint-0.2.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:38:41.310567 ms-mint-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-07-11 19:38:29.000000 ms-mint-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-11 19:38:29.000000 ms-mint-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-11 19:38:41.310567 ms-mint-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-07-11 19:38:29.000000 ms-mint-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:38:41.314567 ms-mint-0.2.5/ms_mint/
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/Chromatogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18035 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/Mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/MintPlotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/TargetOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-11 19:38:41.314567 ms-mint-0.2.5/ms_mint/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/matplotlib_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/plotly_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:38:41.310567 ms-mint-0.2.5/ms_mint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-11 19:38:41.000000 ms-mint-0.2.5/ms_mint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-11 19:38:41.000000 ms-mint-0.2.5/ms_mint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:38:41.000000 ms-mint-0.2.5/ms_mint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-11 19:38:41.000000 ms-mint-0.2.5/ms_mint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 19:38:41.000000 ms-mint-0.2.5/ms_mint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:38:41.310567 ms-mint-0.2.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-11 19:38:29.000000 ms-mint-0.2.5/scripts/ms-mint-convert.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-07-11 19:38:41.314567 ms-mint-0.2.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-07-11 19:38:29.000000 ms-mint-0.2.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68780 2023-07-11 19:38:30.000000 ms-mint-0.2.5/versioneer.py
```

### Comparing `ms-mint-0.2.4/LICENSE` & `ms-mint-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.4/PKG-INFO` & `ms-mint-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint
-Version: 0.2.4
+Version: 0.2.5
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,36 +12,43 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Python package](https://github.com/LewisResearchGroup/ms-mint/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/LewisResearchGroup/ms-mint/actions/workflows/pythonpackage.yml)
 ![](https://github.com/LewisResearchGroup/ms-mint/blob/develop/images/coverage.svg)
 [![CodeQL](https://github.com/lewisresearchgroup/ms-mint/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/lewisresearchgroup/ms-mint/actions/workflows/codeql-analysis.yml)
 
-# Wecome to ms-mint 
+# Wecome to ms-mint
 
 ## A Python library for targeted metabolomics
 The `ms-mint` library is a tool designed to assist with targeted metabolomics studies, which involves the systematic analysis of small chemical compounds called metabolites that are present in biological samples. These metabolites can provide valuable information about the state of an organism, including indicators of disease or other physiological changes. In order to perform a targeted metabolomics study, researchers typically use liquid chromatography-mass spectrometry (LCMS) to identify and quantify specific metabolites of interest.
 
 The `ms-mint` library includes a range of functions for processing LCMS data from targeted metabolomics experiments, and it is particularly well-suited for handling large amounts of data (10,000+ files). To use `ms-mint`, you provide it with a target list of the specific metabolites you want to analyze, as well as the names of the mass spectrometry files containing the data. ms-mint then extracts peak intensities and other relevant information from the data, allowing you to gain insights into the concentrations and profiles of the metabolites in your samples. This information can be used to identify biomarkers, which are indicators of disease or other physiological changes that can be used in the development of diagnostic tests or other medical applications.
 
+## Installation
+
+    pip install ms-mint
+
+
 ## Documentation
 The code documentation can be accessed [here](https://lewisresearchgroup.github.io/ms-mint/readme.html).
 
 ## ms-mint application with graphical user iterface (GUI)
 MINT has been split into the Python library and the app. This repository contains the Python library. For the app follow [this link](https://github.com/LewisResearchGroup/ms-mint-app).
 
+## Publications that used ms-mint
+1. Brown K, Thomson CA, Wacker S, Drikic M, Groves R, Fan V, et al. [Microbiota alters the metabolome in an age- and sex- dependent manner in mice.](https://pubmed.ncbi.nlm.nih.gov/36906623/) Nat Commun. 2023;14: 1348.
+
+---
 ## Contributions
 All contributions, bug reports, code reviews, bug fixes, documentation improvements, enhancements, and ideas are welcome.
 Before you modify the code please reach out to us using the [issues](https://github.com/LewisResearchGroup/ms-mint/issues) page.
 
 ## Code standards
 The project follows PEP8 standard and uses Black and Flake8 to ensure a consistent code format throughout the project.
 
----
-
 ## Usage
 
 To use the main class of the ms-mint library, you can import it into your code with the following command:
 
     from ms_mint.Mint import Mint
 
 This will import a lightweight version of the class with the essential functionality. If you want to use the ms-mint tool interactively in a Jupyter Notebook or JupyterLab, you can import the class with the following command:
@@ -125,15 +132,15 @@
 
 ## Optimize retention times
 
 If you only have retention time (Rt) values for your targets, or if the Rt values you have are not accurate, you can use the `mint.opt.rt_min_max()` function from the ms-mint library to generate better values for the `rt_min` and `rt_max` parameters. These parameters define the range of retention times within which `ms-mint` will search for peaks corresponding to your targets. By optimizing these values, you can improve the accuracy and reliability of your results.
 
 To use the `mint.opt.rt_min_max()` function, you will need to provide it with a list of retention times for your targets and the names of the mass spectrometry files containing your data. The function will then search through the data to find the optimal `rt_min` and `rt_max` values, which you can use to refine your analysis. You can then use these optimized values in conjunction with the other functions and methods of the `Mint` class to process and analyze your data.
 
-![](notebooks/peak-shapes-before-opt.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/peak-shapes-before-opt.png)
 
 Now, we can run the peak optimization with:
 
     mint.opt.rt_min_max(
         fns=[...]
         peak_labels=['Xanthine', 'Succinate', 'Citrulline'],
         plot=True, rel_height=0.7, sigma=50, col_wrap=1, aspect=3,
@@ -142,34 +149,34 @@
 
 The `mint.opt.rt_min_max()` function in the ms-mint library allows you to optimize the `rt_min` and `rt_max` values for your analysis. These values define the range of retention times within which ms-mint will search for peaks corresponding to your targets. By optimizing these values, you can improve the accuracy and reliability of your results.
 
 If you do not provide a list of peak_labels to the `mint.opt.rt_min_max()` function, it will run the optimization for all metabolites. Similarly, if you do not provide a list of filenames for the fn parameter, the function will use all of the files currently loaded into mint.ms_files. It is generally recommended to use a maximum of 20-40 files for the optimization process. If you have run a set of standards along with your samples (which is highly recommended), you can use the standard files to perform the optimization.
 
 After running the optimization, it is a good idea to perform a manual fine-tuning of the `rt_min` and `rt_max` values, especially for complicated peaks (peaks with multiple components, noisy peaks, etc.). You can use the `mint.plot.peak_shapes()` function to visualize the peak shapes and identify any areas that may require further attention.
     
-![](notebooks/optimize-rt_min_max.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/optimize-rt_min_max.png)
 
 The black lines indicates the average intensity across all files used for the optimization. The orange dotted lines show the shape of the gaussian function used to weight the mean intensities for peak selection. The orange horizontal lines indicate the peak width and the blue `x`s show the identified peak maxima. The green shaded areas show the Rt ranges which were selected by the algorithm.
 
 Then we apply the changes and plot the new peak shapes:
 
     mint.run()
     mint.plot.peak_shapes(col_wrap=3)
 
-![](notebooks/peak-shapes-after-opt.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/peak-shapes-after-opt.png)
 
 As you can see, the shapes of Xanthine, Succinate, Citrulline look much better.
 
 ## Plotting and data exploration
 
 The `Mint` class has a few convenient methods to visualize and explore the processed data. The results can be viewed directly in JupyterLab or stored to files using `matplotlib` and `seaborn` syntax. The figures are matplotlib objects and can be easily customised. 
 
 ## Plot peak shapes
 
-![](notebooks/peak-shapes-after-opt.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/peak-shapes-after-opt.png)
 
     mint.plot.peak_shapes(col_wrap = 3)
 
 The method uses seaborn [sns.relplot()](https://seaborn.pydata.org/generated/seaborn.relplot.html) function and keyword arguments are passed on. 
 
 ## Hierarchical clustering
 Mint ca be used to cluster the extracted data. An agglomerative hierarchical clustering is a bottom-up clustering technique where each data point starts as its own cluster and then are merged with other clusters in a hierarchical manner based on their proximity or similarity until a single cluster is formed or a specified stopping criteria is met. The proximity is usually determined by a distance metric, such as Euclidean distance, and the similarity is usually determined by a linkage function, such as ward linkage or complete linkage. The result is a tree-like representation called a dendrogram, which can be used to determine the number of clusters and the cluster assignments of the data points.
@@ -196,29 +203,29 @@
         transform_filenames_func="basename",  # Transformation function to shorten filenames
         transposed=False,  # Transpose the plot     
         top_height=2,  # Height of the top-dendrogram
         left_width=2,  # Width of the left-dendrogram
         cmap=None  # Name of a matplotlib color map                
     )
 
-![](notebooks/hierarchical_clustering.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/hierarchical_clustering.png)
 
 ## Principal Components Analysis
 
 Principal Component Analysis (PCA) is a widely used statistical technique for dimensionality reduction. It transforms the original high-dimensional data into a new set of linearly uncorrelated variables, called Principal Components (PCs), that capture the maximum variance in the data. The first PC accounts for the largest variance in the data, the second PC for the second largest variance, and so on. PCA is commonly used for data visualization, data compression, and noise reduction. By reducing the number of dimensions in the data, PCA allows us to more easily identify patterns and relationships in the data.
 
 Before clustering the data can be transformed and scaled. By default log2p1(x) = log_2(x+1) is used to transform the data and the standard scaler (z-scores) is used to normalize the variables for each target.
 
     mint.pca.run(n_components=5)
     
 After running the PCA the results can be plotted with:    
     
     mint.pca.plot.pairplot(n_components=5, interactive=False)
     
-![](notebooks/pca-pairplot.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/pca-pairplot.png)
 
 ## FAQ
 ### What is a target list
 A target list is a pandas dataframe with specific columns. 
 
 -   **peak_label**: string, Label of the peak (must be unique).
 -   **mz_mean**: numeric value, theoretical m/z value of the target ion to extract.
```

### Comparing `ms-mint-0.2.4/README.md` & `ms-mint-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 [![Python package](https://github.com/LewisResearchGroup/ms-mint/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/LewisResearchGroup/ms-mint/actions/workflows/pythonpackage.yml)
 ![](https://github.com/LewisResearchGroup/ms-mint/blob/develop/images/coverage.svg)
 [![CodeQL](https://github.com/lewisresearchgroup/ms-mint/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/lewisresearchgroup/ms-mint/actions/workflows/codeql-analysis.yml)
 
-# Wecome to ms-mint 
+# Wecome to ms-mint
 
 ## A Python library for targeted metabolomics
 The `ms-mint` library is a tool designed to assist with targeted metabolomics studies, which involves the systematic analysis of small chemical compounds called metabolites that are present in biological samples. These metabolites can provide valuable information about the state of an organism, including indicators of disease or other physiological changes. In order to perform a targeted metabolomics study, researchers typically use liquid chromatography-mass spectrometry (LCMS) to identify and quantify specific metabolites of interest.
 
 The `ms-mint` library includes a range of functions for processing LCMS data from targeted metabolomics experiments, and it is particularly well-suited for handling large amounts of data (10,000+ files). To use `ms-mint`, you provide it with a target list of the specific metabolites you want to analyze, as well as the names of the mass spectrometry files containing the data. ms-mint then extracts peak intensities and other relevant information from the data, allowing you to gain insights into the concentrations and profiles of the metabolites in your samples. This information can be used to identify biomarkers, which are indicators of disease or other physiological changes that can be used in the development of diagnostic tests or other medical applications.
 
+## Installation
+
+    pip install ms-mint
+
+
 ## Documentation
 The code documentation can be accessed [here](https://lewisresearchgroup.github.io/ms-mint/readme.html).
 
 ## ms-mint application with graphical user iterface (GUI)
 MINT has been split into the Python library and the app. This repository contains the Python library. For the app follow [this link](https://github.com/LewisResearchGroup/ms-mint-app).
 
+## Publications that used ms-mint
+1. Brown K, Thomson CA, Wacker S, Drikic M, Groves R, Fan V, et al. [Microbiota alters the metabolome in an age- and sex- dependent manner in mice.](https://pubmed.ncbi.nlm.nih.gov/36906623/) Nat Commun. 2023;14: 1348.
+
+---
 ## Contributions
 All contributions, bug reports, code reviews, bug fixes, documentation improvements, enhancements, and ideas are welcome.
 Before you modify the code please reach out to us using the [issues](https://github.com/LewisResearchGroup/ms-mint/issues) page.
 
 ## Code standards
 The project follows PEP8 standard and uses Black and Flake8 to ensure a consistent code format throughout the project.
 
----
-
 ## Usage
 
 To use the main class of the ms-mint library, you can import it into your code with the following command:
 
     from ms_mint.Mint import Mint
 
 This will import a lightweight version of the class with the essential functionality. If you want to use the ms-mint tool interactively in a Jupyter Notebook or JupyterLab, you can import the class with the following command:
@@ -111,15 +118,15 @@
 
 ## Optimize retention times
 
 If you only have retention time (Rt) values for your targets, or if the Rt values you have are not accurate, you can use the `mint.opt.rt_min_max()` function from the ms-mint library to generate better values for the `rt_min` and `rt_max` parameters. These parameters define the range of retention times within which `ms-mint` will search for peaks corresponding to your targets. By optimizing these values, you can improve the accuracy and reliability of your results.
 
 To use the `mint.opt.rt_min_max()` function, you will need to provide it with a list of retention times for your targets and the names of the mass spectrometry files containing your data. The function will then search through the data to find the optimal `rt_min` and `rt_max` values, which you can use to refine your analysis. You can then use these optimized values in conjunction with the other functions and methods of the `Mint` class to process and analyze your data.
 
-![](notebooks/peak-shapes-before-opt.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/peak-shapes-before-opt.png)
 
 Now, we can run the peak optimization with:
 
     mint.opt.rt_min_max(
         fns=[...]
         peak_labels=['Xanthine', 'Succinate', 'Citrulline'],
         plot=True, rel_height=0.7, sigma=50, col_wrap=1, aspect=3,
@@ -128,34 +135,34 @@
 
 The `mint.opt.rt_min_max()` function in the ms-mint library allows you to optimize the `rt_min` and `rt_max` values for your analysis. These values define the range of retention times within which ms-mint will search for peaks corresponding to your targets. By optimizing these values, you can improve the accuracy and reliability of your results.
 
 If you do not provide a list of peak_labels to the `mint.opt.rt_min_max()` function, it will run the optimization for all metabolites. Similarly, if you do not provide a list of filenames for the fn parameter, the function will use all of the files currently loaded into mint.ms_files. It is generally recommended to use a maximum of 20-40 files for the optimization process. If you have run a set of standards along with your samples (which is highly recommended), you can use the standard files to perform the optimization.
 
 After running the optimization, it is a good idea to perform a manual fine-tuning of the `rt_min` and `rt_max` values, especially for complicated peaks (peaks with multiple components, noisy peaks, etc.). You can use the `mint.plot.peak_shapes()` function to visualize the peak shapes and identify any areas that may require further attention.
     
-![](notebooks/optimize-rt_min_max.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/optimize-rt_min_max.png)
 
 The black lines indicates the average intensity across all files used for the optimization. The orange dotted lines show the shape of the gaussian function used to weight the mean intensities for peak selection. The orange horizontal lines indicate the peak width and the blue `x`s show the identified peak maxima. The green shaded areas show the Rt ranges which were selected by the algorithm.
 
 Then we apply the changes and plot the new peak shapes:
 
     mint.run()
     mint.plot.peak_shapes(col_wrap=3)
 
-![](notebooks/peak-shapes-after-opt.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/peak-shapes-after-opt.png)
 
 As you can see, the shapes of Xanthine, Succinate, Citrulline look much better.
 
 ## Plotting and data exploration
 
 The `Mint` class has a few convenient methods to visualize and explore the processed data. The results can be viewed directly in JupyterLab or stored to files using `matplotlib` and `seaborn` syntax. The figures are matplotlib objects and can be easily customised. 
 
 ## Plot peak shapes
 
-![](notebooks/peak-shapes-after-opt.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/peak-shapes-after-opt.png)
 
     mint.plot.peak_shapes(col_wrap = 3)
 
 The method uses seaborn [sns.relplot()](https://seaborn.pydata.org/generated/seaborn.relplot.html) function and keyword arguments are passed on. 
 
 ## Hierarchical clustering
 Mint ca be used to cluster the extracted data. An agglomerative hierarchical clustering is a bottom-up clustering technique where each data point starts as its own cluster and then are merged with other clusters in a hierarchical manner based on their proximity or similarity until a single cluster is formed or a specified stopping criteria is met. The proximity is usually determined by a distance metric, such as Euclidean distance, and the similarity is usually determined by a linkage function, such as ward linkage or complete linkage. The result is a tree-like representation called a dendrogram, which can be used to determine the number of clusters and the cluster assignments of the data points.
@@ -182,29 +189,29 @@
         transform_filenames_func="basename",  # Transformation function to shorten filenames
         transposed=False,  # Transpose the plot     
         top_height=2,  # Height of the top-dendrogram
         left_width=2,  # Width of the left-dendrogram
         cmap=None  # Name of a matplotlib color map                
     )
 
-![](notebooks/hierarchical_clustering.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/hierarchical_clustering.png)
 
 ## Principal Components Analysis
 
 Principal Component Analysis (PCA) is a widely used statistical technique for dimensionality reduction. It transforms the original high-dimensional data into a new set of linearly uncorrelated variables, called Principal Components (PCs), that capture the maximum variance in the data. The first PC accounts for the largest variance in the data, the second PC for the second largest variance, and so on. PCA is commonly used for data visualization, data compression, and noise reduction. By reducing the number of dimensions in the data, PCA allows us to more easily identify patterns and relationships in the data.
 
 Before clustering the data can be transformed and scaled. By default log2p1(x) = log_2(x+1) is used to transform the data and the standard scaler (z-scores) is used to normalize the variables for each target.
 
     mint.pca.run(n_components=5)
     
 After running the PCA the results can be plotted with:    
     
     mint.pca.plot.pairplot(n_components=5, interactive=False)
     
-![](notebooks/pca-pairplot.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/pca-pairplot.png)
 
 ## FAQ
 ### What is a target list
 A target list is a pandas dataframe with specific columns. 
 
 -   **peak_label**: string, Label of the peak (must be unique).
 -   **mz_mean**: numeric value, theoretical m/z value of the target ion to extract.
```

### Comparing `ms-mint-0.2.4/ms_mint/Mint.py` & `ms-mint-0.2.5/ms_mint/Mint.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,66 +7,73 @@
 import logging
 
 from pathlib import Path as P
 from multiprocessing import Pool, Manager, cpu_count
 from glob import glob
 
 from .standards import MINT_RESULTS_COLUMNS, TARGETS_COLUMNS, DEPRECATED_LABELS
-from .processing import process_ms1_files_in_parallel
+from .processing import process_ms1_files_in_parallel, extract_chromatogram_from_ms1
 from .io import export_to_excel, ms_file_to_df
-from .targets import read_targets, check_targets, standardize_targets, TargetOptimizer
+from .TargetOptimizer import TargetOptimizer
+from .targets import read_targets, check_targets, standardize_targets
 from .tools import (
     is_ms_file,
     get_ms_files_from_results,
     get_targets_from_results,
     scale_dataframe,
+    init_metadata,
+    fn_to_label
 )
 from .pca import PrincipalComponentsAnalyser
-from .plotting import MintPlotter
-
-# from .filter import Resampler
-from .chromatogram import Chromatogram, extract_chromatogram_from_ms1
+from .MintPlotter import MintPlotter
+from .Chromatogram import Chromatogram
 
 import ms_mint
 
 from tqdm import tqdm
 
 from typing import Callable
 from functools import lru_cache
 
+METADATA_DEFAUT_FN = 'metadata.parquet'
 
 class Mint(object):
     """
     Main class of the ms_mint package, which processes metabolomics files.
 
     :param verbose: Sets verbosity of the instance.
     :type verbose: bool
 
     :param progress_callback: A callback for a progress bar.
     :type progress_callback: Callable[]
 
+    :parm wdir: Working directory
+    :type wdir: str
     """
 
     def __init__(
         self,
         verbose: bool = False,
         progress_callback: Callable = None,
         time_unit: str = "s",
+        wdir: str = None
     ):
         self.verbose = verbose
         self._version = ms_mint.__version__
+        print("Mint version:", self.version, "\n")
         self.progress_callback = progress_callback
         self.reset()
-        if self.verbose:
-            print("Mint Version:", self.version, "\n")
         self.plot = MintPlotter(mint=self)
         self.opt = TargetOptimizer(mint=self)
         self.pca = PrincipalComponentsAnalyser(self)
         self.tqdm = tqdm
-        self.meta = None
+
+        # Setup working directory as pathlib.Path
+        self.wdir = os.getcwd() if wdir is None else wdir
+        self.wdir = P(self.wdir)
 
     @property
     def version(self):
         """
         ms-mint version number.
 
         :return: Version string.
@@ -86,14 +93,15 @@
         self._targets = pd.DataFrame(columns=TARGETS_COLUMNS)
         self._results = pd.DataFrame({i: [] for i in MINT_RESULTS_COLUMNS})
         self._all_df = None
         self._progress = 0
         self.runtime = None
         self._status = "waiting"
         self._messages = []
+        self.meta = init_metadata()
         return self
 
     def clear_targets(self):
         """
         Reset target list.
         """
         self.targets = pd.DataFrame(columns=TARGETS_COLUMNS)
@@ -196,15 +204,14 @@
                 f"Runtime per peak ({len(self.targets)}): {self.runtime_per_peak:.2f}s\n"
             )
             print("Results:", self.results)
 
     def _run_parallel(
         self, nthreads=1, mode="standard", maxtasksperchild=None, fn=None
     ):
-        print(f"maxtasksperchild: {maxtasksperchild}")
         pool = Pool(processes=nthreads, maxtasksperchild=maxtasksperchild)
         m = Manager()
         q = m.Queue()
         args = []
 
         if fn is not None:
             # Prepare output file (only headers)
@@ -270,14 +277,15 @@
         list_of_files = [str(P(i)) for i in list_of_files if is_ms_file(i)]
         for f in list_of_files:
             if not os.path.isfile(f):
                 logging.warning(f"File not found ({f})")
         self._files = list_of_files
         if self.verbose:
             print("Set files to:\n" + "\n".join(self.ms_files) + "\n")
+        self.meta = self.meta.reindex([fn_to_label(fn) for fn in list_of_files])
 
     @property
     def n_files(self):
         """
         Number of currently stored ms filenames.
 
         :return: Number of files stored in self.ms_files
@@ -369,31 +377,42 @@
         """
         return self._results
 
     @results.setter
     def results(self, df):
         self._results = df
 
-    def crosstab(self, col_name="peak_max", apply=None, scaler=None):
+    def crosstab(self, values: str = "peak_max", index: str = None, column: str = None, aggfunc: str = 'mean', apply: Callable = None, scaler: Callable = None):
         """
         Create condensed representation of the results.
         More specifically, a cross-table with filenames as index and target labels.
         The values in the cells are determined by *col_name*.
 
         :param col_name: Name of the column from *mint.results* table that is used for the cell values.
         :type col_name: str
 
         cells of the returned table.
         """
+
+        df_meta = pd.merge(self.meta, self.results, left_index=True, right_on='ms_file_label')
+
+        if index is None:
+            index = 'ms_file_label'
+        if column is None:
+            column = 'peak_label'
+        if values is None:
+            values = 'peak_area_top3'
+
         df = pd.crosstab(
-            self.results.ms_file,
-            self.results.peak_label,
-            self.results[col_name],
-            aggfunc=sum,
+            df_meta[index],
+            df_meta[column],
+            df_meta[values],
+            aggfunc=aggfunc,
         ).astype(np.float64)
+
         if apply:
             df = df.apply(apply)
         if scaler:
             df = scale_dataframe(df, scaler=scaler)
         return df
 
     @property
@@ -458,53 +477,88 @@
                 results["peak_shape_int"] = results["peak_shape_int"].fillna("")
                 self.results = results
 
             elif fn.endswith(".parquet"):
                 results = pd.read_parquet(fn)
         else:
             results = pd.read_csv(fn)
+
+        # Add file labels if not present already    
+        if 'ms_file_label' not in results.columns:
+            results['ms_file_label'] = [fn_to_label(fn) for fn in results.ms_file]
+
         self.results = results.rename(columns=DEPRECATED_LABELS)
         self.digest_results()
         return self
 
     def digest_results(self):
         self.ms_files = get_ms_files_from_results(self.results)
         self.targets = get_targets_from_results(self.results)
 
-    @lru_cache(1)
-    def get_chromatograms(self, fns=None, peak_label=None, **kwargs):
+
+    def get_chromatograms(self, fns=None, peak_labels=None, filters=None, **kwargs):
         if fns is None:
             fns = self.ms_files
+        if peak_labels is None:
+            peak_labels = self.peak_labels
+        return self._get_chromatograms(fns=tuple(fns), peak_labels=tuple(peak_labels), 
+                                       filters=tuple(filters) if filters is not None else None, **kwargs)
+
+    @lru_cache(1)
+    def _get_chromatograms(self, fns=None, peak_labels=None, filters=None, **kwargs):
 
         if isinstance(fns, tuple):
-            fns = list(fns)
+            fns = list(fns)     
 
         if not isinstance(fns, list):
             fns = [fns]
 
-        if peak_label is None:
-            peak_label = self.peak_labels
+        labels = [fn_to_label(fn) for fn in fns]
+
+        # Need to get the actual file names with get_chromatogramsath
+        # in case only ms_file_labels are provided
+        fns = [fn for fn in self.ms_files if fn_to_label(fn) in labels]
 
         data = []
 
-        for fn in self.tqdm(fns):
+        for fn in self.tqdm(fns, desc="Loading chromatograms"):
             df = ms_file_to_df(fn)
-            for label in peak_label:
+            for label in peak_labels:
                 mz_mean, mz_width, rt_min, rt_max = self.get_target_params(label)
                 chrom_raw = extract_chromatogram_from_ms1(
                     df, mz_mean=mz_mean, mz_width=mz_width
                 ).to_frame()
                 if len(chrom_raw) == 0:
                     continue
-                chrom = Chromatogram(chrom_raw.index, chrom_raw.values)
-                chrom.apply_filter()
+                chrom = Chromatogram(chrom_raw.index, chrom_raw.values, filters=filters, **kwargs)
+                if filters is not None:
+                    chrom.apply_filters()
                 chrom_data = chrom.data
                 chrom_data["ms_file"] = fn
+                chrom_data["ms_file_label"] = fn_to_label(fn)
                 chrom_data["peak_label"] = label
                 chrom_data["rt_min"] = rt_min
                 chrom_data["rt_max"] = rt_max
                 data.append(chrom_data)
 
         data = pd.concat(data).reset_index()
 
         data["ms_file"] = data["ms_file"].apply(lambda x: P(x).with_suffix("").name)
         return data
+
+    def load_metadata(self, fn=None):
+        if fn is None:
+            fn = self.wdir/METADATA_DEFAUT_FN
+        if str(fn).endswith('.csv'):
+            self.meta = pd.read_csv(fn, index_col=0)
+        elif str(fn).endswith('.parquet'):
+            self.meta = pd.read_parquet(fn)
+        return self
+
+    def save_metadata(self, fn=None):
+        if fn is None:
+            fn = self.wdir/METADATA_DEFAUT_FN
+        if str(fn).endswith('.csv'):
+            self.meta.to_csv(fn, na_filter=False)
+        elif str(fn).endswith('.parquet'):
+            self.meta.to_parquet(fn)
+        return self
```

### Comparing `ms-mint-0.2.4/ms_mint/chromatogram.py` & `ms-mint-0.2.5/ms_mint/Chromatogram.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,39 +2,56 @@
 import pandas as pd
 import logging
 
 from matplotlib import pyplot as plt
 
 from .tools import find_peaks_in_timeseries, gaussian, mz_mean_width_to_min_max
 from .io import ms_file_to_df
-from .filters import Resampler, Smoother, GaussFilter
+from .filters import Filter, Resampler, Smoother, GaussFilter
 from .matplotlib_tools import plot_peaks
+from .processing import get_chromatogram_from_ms_file
+
+from typing import Optional, Union, List, Any
 
 
 class Chromatogram:
     def __init__(
-        self, scan_times=None, intensities=None, filters=None, expected_rt=None
+        self,
+        scan_times: Optional[Union[List[float], np.ndarray]] = None,
+        intensities: Optional[Union[List[float], np.ndarray]] = None,
+        filters: Optional[List[Filter]] = None,
+        expected_rt: Optional[float] = None
     ):
-        self.t = np.array([0])
-        self.x = np.array([0])
+        """
+        Initialize a Chromatogram object.
+
+        :param scan_times: Array-like object containing the scan times.
+        :param intensities: Array-like object containing the intensities.
+        :param filters: List of filters to be applied.
+        :param expected_rt: Expected retention time.
+        """
+        # Initialize empty arrays for scan_times and intensities
+        # Initialize scan_times and intensities as empty lists or arrays
+        self.t = np.array([]) if scan_times is None or 0 in scan_times else np.array([0])
+        self.x = np.array([]) if intensities is None or 0 in scan_times else np.array([0])
+
+        # Update scan_times and intensities if provided
         if scan_times is not None:
             self.t = np.append(self.t, scan_times)
         if intensities is not None:
             self.x = np.append(self.x, intensities)
-        self.noise_level = None
-        if filters is None:
-            self.filters = [Resampler(), GaussFilter(), Smoother()]
-        else:
-            self.filters = filters
-        self.peaks = None
-        self.selected_peak_ndxs = None
-        if expected_rt is None and scan_times is not None:
-            expected_rt = max(scan_times) // 2
+
+        # Initialize other attributes
+        self.noise_level: Optional[float] = None
+        self.filters: List[Any] = filters or [Resampler(), GaussFilter(), Smoother()]
+        self.peaks: Optional[pd.DataFrame] = None
+        self.selected_peak_ndxs: Optional[List[int]] = None
         self.expected_rt = expected_rt
-        self.weights = None
+        self.weights: Optional[Union[List[float], np.ndarray]] = None
+
 
     def from_file(self, fn, mz_mean, mz_width=10, expected_rt=None):
         chrom = get_chromatogram_from_ms_file(fn, mz_mean=mz_mean, mz_width=mz_width)
         self.t = np.append(self.t, chrom.index)
         self.x = np.append(self.x, chrom.values)
         if expected_rt is not None:
             self.expected_rt = expected_rt
@@ -43,22 +60,23 @@
         data = pd.Series(index=self.t, data=self.x)
         self.noise_level = data.rolling(window, center=True).std().median()
 
     def apply_filters(self):
         for filt in self.filters:
             self.t, self.x = filt.transform(self.t, self.x)
 
-    def find_peaks(self, prominence=None, rel_height=0.9):
+    def find_peaks(self, prominence=None, rel_height=0.9, **kwargs):
         self.estimate_noise_level()
         if prominence is None:
-            prominence = self.noise_level * 3
+            prominence = self.noise_level * 5
         self.peaks = find_peaks_in_timeseries(
             self.data.intensity,
             prominence=prominence,
             rel_height=rel_height,
+            **kwargs
         )
 
     def optimise_peak_times_with_diff(self, rolling_window=20, plot=False):
         peaks = self.peaks
         diff = (
             (self.data - self.data.shift(1))
             .rolling(rolling_window, center=True)
@@ -149,19 +167,7 @@
             highlight=selected_peak_ndxs,
             expected_rt=self.expected_rt,
             weights=weights,
             **kwargs
         )
         return fig
 
-
-def get_chromatogram_from_ms_file(ms_file, mz_mean, mz_width=10):
-    df = ms_file_to_df(ms_file)
-    chrom = extract_chromatogram_from_ms1(df, mz_mean, mz_width=mz_width)
-    return chrom
-
-
-def extract_chromatogram_from_ms1(ms1, mz_mean, mz_width=10):
-    mz_min, mz_max = mz_mean_width_to_min_max(mz_mean, mz_width)
-    chrom = ms1[(ms1["mz"] >= mz_min) & (ms1["mz"] <= mz_max)].copy()
-    chrom = chrom.groupby("scan_time", as_index=False).sum(numeric_only=True)
-    return chrom.set_index("scan_time")["intensity"]
```

### Comparing `ms-mint-0.2.4/ms_mint/filelock.py` & `ms-mint-0.2.5/ms_mint/filelock.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.4/ms_mint/filters.py` & `ms-mint-0.2.5/ms_mint/filters.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 import pandas as pd
 from scipy.ndimage import gaussian_filter1d
+from typing import List, Tuple
 
 
-class Resampler:
+
+class Filter:
+    def transform(self, t: List[float], x: List[float]) -> Tuple[List[float], List[float]]:
+        raise NotImplementedError
+    
+
+class Resampler(Filter):
     """
     Filter for time series that resamples the data in
     a certain frequency.
     """
 
     def __init__(self, tau="500ms", input_unit="seconds"):
         """
@@ -38,15 +45,15 @@
         # resampled = chrom.resample(self.tau).nearest()
         resampled = chrom.resample(self.tau).fillna("nearest", limit=10)
         new_t = resampled.index.seconds + (resampled.index.microseconds / 1e6)
         new_x = resampled.values
         return new_t, new_x
 
 
-class Smoother:
+class Smoother(Filter):
     """
     Filter for time series that smoothes the
     x values by running one or more rolling
     averages.
     """
 
     def __init__(self, windows=None):
@@ -78,15 +85,15 @@
         for window in self.windows:
             tranformed = transformed.rolling(window, center=True).mean().fillna(0)
         new_t = tranformed.index
         new_x = tranformed.values
         return new_t, new_x
 
 
-class GaussFilter:
+class GaussFilter(Filter):
     """
     Filter for time series that applies a Gaussian filter.
     """
 
     def __init__(self, sigma=5):
         """
         Filter for time series that applies a Gaussian filter.
```

### Comparing `ms-mint-0.2.4/ms_mint/io.py` & `ms-mint-0.2.5/ms_mint/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         slices = []
         # Loop through the spectra and extract the data
         for spectrum in reader:
             time_unit = spectrum['scanList']['scan'][0]['scan start time'].unit_info
             if read_only:
                 continue
             # Extract the scan ID, retention time, m/z values, and intensity values
-            scan_id = int(spectrum["id"].split("scan=")[-1])
+            scan_id = int(spectrum["id"].split("=")[-1])
             rt = spectrum["scanList"]["scan"][0]["scan start time"]
             if time_unit == 'minute':
                 rt = rt * 60.
             mz = np.array(spectrum["m/z array"], dtype=np.float64)
             intensity = np.array(spectrum["intensity array"], dtype=np.float64)
             if "positive scan" in spectrum.keys():
                 polarity = "+"
```

### Comparing `ms-mint-0.2.4/ms_mint/matplotlib_tools.py` & `ms-mint-0.2.5/ms_mint/matplotlib_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,15 @@
             expected_rt, expected_rt + 1, color="blue", alpha=1, label="Expected Rt"
         )
     if weights is not None:
         plt.plot(weights, linestyle="--", label="Gaussian weight")
     plt.ylabel("Intensity")
     plt.xlabel("Scan time [s]")
     ax.ticklabel_format(axis="y", style="sci", scilimits=(0, 0))
-    plt.ylim((0.1, None))
+    #plt.ylim((0.001, None))
     if not legend:
         ax.get_legend().remove()
     return plt.gcf()
 
 
 def plot_metabolomics_hist2d(
     df,
```

### Comparing `ms-mint-0.2.4/ms_mint/notebook.py` & `ms-mint-0.2.5/ms_mint/notebook.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.4/ms_mint/pca.py` & `ms-mint-0.2.5/ms_mint/pca.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import seaborn as sns
 import plotly.figure_factory as ff
+from plotly import express as px
 
 from sklearn.decomposition import PCA
 from .tools import scale_dataframe
 
 
 class PrincipalComponentsAnalyser:
     """
@@ -119,53 +120,78 @@
         plt.xlabel("Principal Component")
         plt.ylabel("Explained variance [%]")
         plt.title("Cumulative explained variance")
         plt.grid()
         plt.xticks(range(1, len(cum_expl_var) + 1))
         return fig
 
-    def _prepare_data(self, n_components=3, labels=None):
+    def _prepare_data(self, n_components=3, hue=None):
         df = self.pca.results["df_projected"].copy()
         cols = df.columns.to_list()[:n_components]
         df = df[cols]
-        if labels is not None:
-            group_name = "Label"
-            df[group_name] = labels
-            df[group_name] = df[group_name].astype(str)
+
+        df = pd.merge(df, self.pca.mint.meta.dropna(axis=1, how='all'), left_index=True, right_index=True)
+
+        if hue and (not isinstance(hue, str)):
+            df['Label'] = hue
+            df['Label'] = df['Label'].astype(str)
+
         return df
 
     def pairplot(
-        self, n_components=3, labels=None, fig_kws=None, interactive=False, **kwargs
+        self, n_components=3, hue=None, fig_kws=None, interactive=False, **kwargs
     ):
         """
         After running mint.pca() this function can be used to plot a scatter matrix of the
         principal components.
 
         :param n_components: Number of principal components to plot, defaults to 3.
         :type n_components: int, optional
-        :param labels: Labels used for hue.
-        :type labels: List[str], optional
+        :param hue: Labels used for hue. If string, the data will be taken from the mint.meta dataframe.
+        :type hue: List[str] or str, optional
         :return: Returns a matplotlib figure.
         :rtype: seaborn.axisgrid.PairGrid
         """
 
-        df = self._prepare_data(n_components=n_components, labels=labels)
+        df = self._prepare_data(n_components=n_components, hue=hue)
+
+        if isinstance(hue, list):
+            hue = 'Label'
 
         if interactive:
-            return self.pairplot_plotly(df, **kwargs)
+            return self.pairplot_plotly(df, color_col=hue, **kwargs)
         else:
-            return self.pairplot_sns(df, fig_kws=fig_kws, **kwargs)
+            return self.pairplot_sns(df, fig_kws=fig_kws, hue=hue, **kwargs)
 
     def pairplot_sns(self, df, fig_kws=None, **kwargs):
         if fig_kws is None:
             fig_kws = {}
         plt.figure(**fig_kws)
-        g = sns.pairplot(df, hue="Label" if "Label" in df.columns else None, **kwargs)
+        g = sns.pairplot(df, **kwargs)
         return g
 
-    def pairplot_plotly(self, df, **kwargs):
-        color_col = "Label" if "Label" in df.columns else None
-        fig = ff.create_scatterplotmatrix(df, index=color_col, **kwargs)
+    def pairplot_plotly(self, df, color_col=None, **kwargs):
+        columns = df.filter(regex=f'PC|^{color_col}$').columns
+        fig = ff.create_scatterplotmatrix(df[columns], index=color_col, hovertext=df.index, **kwargs)
         # set the legendgroup equal to the marker color
         for t in fig.data:
             t.legendgroup = t.marker.color
         return fig
+
+    def loadings(self, interactive=False, **kwargs):
+        if interactive:
+            return self.loadings_plotly(**kwargs)
+        else:    
+            return self.loadings_sns(**kwargs)
+
+    def loadings_sns(self, **kwargs):
+        if 'row' not in kwargs:
+            kwargs['row'] = 'PC'
+        g = sns.catplot(data=self.pca.results['feature_contributions'], x='peak_label', y='Coefficient', kind='bar', **kwargs)
+        plt.tight_layout()
+        return g
+    
+    def loadings_plotly(self, **kwargs):
+        if 'facet_row' not in kwargs:
+            kwargs['facet_row'] = 'PC'
+        fig = px.bar(self.pca.results['feature_contributions'], x='peak_label', y='Coefficient', barmode='group', **kwargs)
+        return  fig
```

### Comparing `ms-mint-0.2.4/ms_mint/plotly_tools.py` & `ms-mint-0.2.5/ms_mint/plotly_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 import plotly.figure_factory as ff
 import plotly.io as pio
 
 from pathlib import Path as P
 from collections.abc import Iterable
 from plotly.subplots import make_subplots
 
+from .tools import fn_to_label
+
+
 
 def set_template():
     """
     A function that sets a template for plotly figures.
     """
     pio.templates["draft"] = go.layout.Template(
         layout=dict(font={"size": 10}),
@@ -229,28 +232,29 @@
 ):
     """
     Returns a plotly multiplost of all peak_shapes in mint.results
     grouped by peak_label.
     """
     mint_results = mint_results.copy()
 
+
     if fns is not None:
-        fns = [P(fn).name for fn in fns]
-        mint_results = mint_results[mint_results.ms_file.isin(fns)]
+        fns = [fn_to_label(fn) for fn in fns]
+        mint_results = mint_results[mint_results.ms_file_label.isin(fns)]
 
     mint_results.ms_file = [P(fn).name for fn in mint_results.ms_file]
 
     logging.warning("TEST")
 
     res = mint_results[mint_results.peak_max > 0]
 
-    fns = list(res.ms_file.drop_duplicates())
-    labels = list(mint_results.peak_label.drop_duplicates())
+    fns = res.ms_file_label.unique()
+    labels = mint_results.peak_label.unique()
 
-    res = res.set_index(["peak_label", "ms_file"]).sort_index()
+    res = res.set_index(["peak_label", "ms_file_label"]).sort_index()
 
     if isinstance(peak_labels, str):
         peak_labels = [peak_labels]
 
     # Calculate neccessary number of rows
     n_rows = max(1, len(labels) // col_wrap)
     if n_rows * col_wrap < len(labels):
```

### Comparing `ms-mint-0.2.4/ms_mint/plotting.py` & `ms-mint-0.2.5/ms_mint/MintPlotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,15 @@
         )
 
         if not transposed:
             self.mint.clustered = data.iloc[ndx_x, ndx_y]
         else:
             self.mint.clustered = data.iloc[ndx_y, ndx_x]
         return fig
+    
 
     def peak_shapes(self, fns=None, peak_labels=None, interactive=False, **kwargs):
         """Plot peak shapes.
 
         :return: Figure with peak shapes.
         :rtype: seaborn.axisgrid.FacetGrid
         """
@@ -259,15 +260,15 @@
             )
         if peak_label is None:
             plt.title(f'{P(fn).with_suffix("").name}')
         else:
             plt.title(f'{P(fn).with_suffix("").name}\n{peak_label}')
         return fig
 
-    def chromatogram(self, fns=None, peak_labels=None, interactive=False, **kwargs):
+    def chromatogram(self, fns=None, peak_labels=None, interactive=False, filters=None, **kwargs):
         """Plot the chromatogram extracted from one or more files.
 
         :param fns: File names to extract chromatogram from.
         :type fns: str or List[str]
         :param peak_label: Target from Mint.targets.peak_label to take mz
         parameters, defaults to None. If None `mz_mean and mz_width are used`.
         :type peak_label: str, optional
@@ -290,26 +291,26 @@
 
         if peak_labels is None:
             peak_labels = self.mint.peak_labels
 
         if peak_labels is not None:
             peak_labels = tuple(peak_labels)
 
-        data = self.mint.get_chromatograms(fns=fns, peak_labels=peak_labels)
+        data = self.mint.get_chromatograms(fns=fns, peak_labels=peak_labels, filters=filters)
 
         if not interactive:
             params = dict(
                 x="scan_time",
                 y="intensity",
                 col="peak_label",
                 col_wrap=1,
                 col_order=peak_labels,
                 height=1.5,
                 aspect=5,
-                hue="ms_file",
+                hue="ms_file_label",
                 facet_kws=dict(sharey=False),
                 marker=".",
                 linewidth=0,
             )
             params.update(kwargs)
             g = sns.relplot(data=data, **params)
 
@@ -327,14 +328,14 @@
 
         else:
             g = px.line(
                 data_frame=data,
                 x="scan_time",
                 y="intensity",
                 facet_col="peak_label",
-                color="ms_file",
+                color="ms_file_label",
                 height=700,
                 facet_col_wrap=1,
             )
             g.update_xaxes(matches=None)
             g.update_yaxes(matches=None)
             return g
```

### Comparing `ms-mint-0.2.4/ms_mint/processing.py` & `ms-mint-0.2.5/ms_mint/processing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # ms_mint/processing.py
 
 import os
 import pandas as pd
 import numpy as np
 import logging
 
+from  pathlib import Path as P
+
 from .tools import lock, mz_mean_width_to_min_max
 
 from .io import ms_file_to_df
 
 from .standards import RESULTS_COLUMNS, MINT_RESULTS_COLUMNS
 
 
@@ -80,17 +82,17 @@
     :type targets: pandas.DataFrame
     :return: DataFrame with processd peak intensities.
     :rtype: pandas.DataFrame
     """
     df = ms_file_to_df(filename)
     results = process_ms1(df, targets)
     results["total_intensity"] = df["intensity"].sum()
-    results["ms_file"] = os.path.basename(filename)
-    results["ms_path"] = os.path.dirname(filename)
-    results["ms_file_size"] = os.path.getsize(filename) / 1024 / 1024
+    results["ms_file"] = filename
+    results["ms_file_label"] = P(filename).with_suffix('').name
+    results["ms_file_size_MB"] = os.path.getsize(filename) / 1024 / 1024
     results["peak_score"] = score_peaks(results)
     return results[MINT_RESULTS_COLUMNS]
 
 
 def process_ms1(df, targets):
     """
     Process MS-1 data with a target list.
@@ -316,7 +318,36 @@
     R = mint_results.copy()
     scores = (
         ((1 - R.peak_delta_int.apply(abs) / R.peak_max))
         * (np.tanh(R.peak_n_datapoints / 20))
         * (1 / (1 + abs(R.peak_rt_of_max - R[["rt_min", "rt_max"]].mean(axis=1))))
     )
     return scores
+
+
+def get_chromatogram_from_ms_file(ms_file: str, mz_mean: float, mz_width: float = 10) -> pd.DataFrame:
+    """
+    Get chromatogram data from an MS file.
+
+    :param ms_file: Path to the MS file.
+    :param mz_mean: Mean m/z value.
+    :param mz_width: Width around the mean m/z to extract.
+    :return: Chromatogram data as a DataFrame.
+    """
+    df = ms_file_to_df(ms_file)
+    chrom = extract_chromatogram_from_ms1(df, mz_mean, mz_width=mz_width)
+    return chrom
+
+
+def extract_chromatogram_from_ms1(ms1: pd.DataFrame, mz_mean: float, mz_width: float = 10) -> pd.DataFrame:
+    """
+    Extract chromatogram from MS1 data.
+
+    :param ms1: MS1 data as a DataFrame.
+    :param mz_mean: Mean m/z value.
+    :param mz_width: Width around the mean m/z to extract.
+    :return: Chromatogram data as a DataFrame.
+    """
+    mz_min, mz_max = mz_mean_width_to_min_max(mz_mean, mz_width)
+    chrom = ms1[(ms1["mz"] >= mz_min) & (ms1["mz"] <= mz_max)].copy()
+    chrom = chrom.groupby("scan_time", as_index=False).sum(numeric_only=True)
+    return chrom.set_index("scan_time")["intensity"]
```

### Comparing `ms-mint-0.2.4/ms_mint/standards.py` & `ms-mint-0.2.5/ms_mint/standards.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,28 +33,29 @@
     "peak_mass_diff_25pc",
     "peak_mass_diff_50pc",
     "peak_mass_diff_75pc",
     "peak_score",
 ]
 
 MINT_RESULTS_COLUMNS = (
-    ["ms_file"]
+    ["ms_file", "ms_file_label"]
     + TARGETS_COLUMNS
     + RESULTS_COLUMNS
-    + ["total_intensity", "ms_path", "ms_file_size"]
+    + ["total_intensity", "ms_file_size_MB"]
 )
 
 DEPRECATED_LABELS = {
     "peakLabel": "peak_label",
     "compound": "peak_label",
     "peakMz": "mz_mean",
     "medRt": "rt",
     "medMz": "mz_mean",
     "peakMzWidth[ppm]": "mz_width",
     "rtmin": "rt_min",
     "rtmax": "rt_max",
     "peaklist": "target_filename",
     "peaklist_name": "target_filename",
     "scan_time_min": "scan_time",
+    "ms_file_size": "ms_file_size_MB",
 }
 
 M_PROTON = 1.00782503223
```

### Comparing `ms-mint-0.2.4/ms_mint/tools.py` & `ms-mint-0.2.5/ms_mint/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -141,16 +141,20 @@
     Extract MS-filenames from Mint results.
 
     :param results: DataFrame in Mint fesults format
     :type results: pandas.DataFrame
     :return: List of filenames
     :rtype: list
     """
-    ms_files = results[["ms_path", "ms_file"]].drop_duplicates()
-    ms_files = [P(ms_path) / ms_file for ms_path, ms_file in ms_files.values]
+    # Old schema
+    if 'ms_path' in results.columns:
+        ms_files = results[["ms_path", "ms_file"]].drop_duplicates()
+        ms_files = [P(ms_path) / ms_file for ms_path, ms_file in ms_files.values]
+    else:
+        ms_files = results.ms_file.unique()
     return ms_files
 
 
 def get_targets_from_results(results):
     """Extract targets dataframe from ms-mint results table.
 
     :param results: Mint results table
@@ -159,29 +163,29 @@
     :rtype: pandas.DataFrame
     """
     return results[
         [col for col in TARGETS_COLUMNS if col in results.columns]
     ].drop_duplicates()
 
 
-def find_peaks_in_timeseries(series, prominence=None, plot=False, rel_height=0.9):
+def find_peaks_in_timeseries(series, prominence=None, plot=False, rel_height=0.9, **kwargs):
     """_summary_
 
     :param series: _description_
     :type series: _type_
     :param prominence: _description_, defaults to None
     :type prominence: _type_, optional
     :param plot: _description_, defaults to False
     :type plot: bool, optional
     :return: _description_
     :rtype: _type_
     """
     t = series.index
     x = series.values
-    peak_ndxs, _ = find_peaks(x, prominence=prominence)
+    peak_ndxs, _ = find_peaks(x, prominence=prominence, rel_height=rel_height, **kwargs)
     widths, heights, left_ips, right_ips = peak_widths(
         x, peak_ndxs, rel_height=rel_height
     )
     times = series.iloc[peak_ndxs].index
 
     t_start = _map_ndxs_to_time(left_ips, min(t), max(t), 0, len(t))
     t_end = _map_ndxs_to_time(right_ips, min(t), max(t), 0, len(t))
@@ -217,7 +221,25 @@
 
 
 def mz_mean_width_to_min_max(mz_mean, mz_width):
     delta_mass = mz_width * mz_mean * 1e-6
     mz_min = mz_mean - delta_mass
     mz_max = mz_mean + delta_mass
     return mz_min, mz_max
+
+def init_metadata():
+    cols = [
+        'ms_file_label',
+        'ms_file',
+        'label', 
+        'group', 
+        'type',
+        'run_order', 
+        'plate', 
+        'plate_row', 
+        'plate_col'
+    ]
+    return pd.DataFrame(columns=cols).set_index('ms_file_label')
+
+
+def fn_to_label(fn):
+    return P(fn).with_suffix('').name
```

### Comparing `ms-mint-0.2.4/ms_mint.egg-info/PKG-INFO` & `ms-mint-0.2.5/ms_mint.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint
-Version: 0.2.4
+Version: 0.2.5
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,36 +12,43 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Python package](https://github.com/LewisResearchGroup/ms-mint/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/LewisResearchGroup/ms-mint/actions/workflows/pythonpackage.yml)
 ![](https://github.com/LewisResearchGroup/ms-mint/blob/develop/images/coverage.svg)
 [![CodeQL](https://github.com/lewisresearchgroup/ms-mint/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/lewisresearchgroup/ms-mint/actions/workflows/codeql-analysis.yml)
 
-# Wecome to ms-mint 
+# Wecome to ms-mint
 
 ## A Python library for targeted metabolomics
 The `ms-mint` library is a tool designed to assist with targeted metabolomics studies, which involves the systematic analysis of small chemical compounds called metabolites that are present in biological samples. These metabolites can provide valuable information about the state of an organism, including indicators of disease or other physiological changes. In order to perform a targeted metabolomics study, researchers typically use liquid chromatography-mass spectrometry (LCMS) to identify and quantify specific metabolites of interest.
 
 The `ms-mint` library includes a range of functions for processing LCMS data from targeted metabolomics experiments, and it is particularly well-suited for handling large amounts of data (10,000+ files). To use `ms-mint`, you provide it with a target list of the specific metabolites you want to analyze, as well as the names of the mass spectrometry files containing the data. ms-mint then extracts peak intensities and other relevant information from the data, allowing you to gain insights into the concentrations and profiles of the metabolites in your samples. This information can be used to identify biomarkers, which are indicators of disease or other physiological changes that can be used in the development of diagnostic tests or other medical applications.
 
+## Installation
+
+    pip install ms-mint
+
+
 ## Documentation
 The code documentation can be accessed [here](https://lewisresearchgroup.github.io/ms-mint/readme.html).
 
 ## ms-mint application with graphical user iterface (GUI)
 MINT has been split into the Python library and the app. This repository contains the Python library. For the app follow [this link](https://github.com/LewisResearchGroup/ms-mint-app).
 
+## Publications that used ms-mint
+1. Brown K, Thomson CA, Wacker S, Drikic M, Groves R, Fan V, et al. [Microbiota alters the metabolome in an age- and sex- dependent manner in mice.](https://pubmed.ncbi.nlm.nih.gov/36906623/) Nat Commun. 2023;14: 1348.
+
+---
 ## Contributions
 All contributions, bug reports, code reviews, bug fixes, documentation improvements, enhancements, and ideas are welcome.
 Before you modify the code please reach out to us using the [issues](https://github.com/LewisResearchGroup/ms-mint/issues) page.
 
 ## Code standards
 The project follows PEP8 standard and uses Black and Flake8 to ensure a consistent code format throughout the project.
 
----
-
 ## Usage
 
 To use the main class of the ms-mint library, you can import it into your code with the following command:
 
     from ms_mint.Mint import Mint
 
 This will import a lightweight version of the class with the essential functionality. If you want to use the ms-mint tool interactively in a Jupyter Notebook or JupyterLab, you can import the class with the following command:
@@ -125,15 +132,15 @@
 
 ## Optimize retention times
 
 If you only have retention time (Rt) values for your targets, or if the Rt values you have are not accurate, you can use the `mint.opt.rt_min_max()` function from the ms-mint library to generate better values for the `rt_min` and `rt_max` parameters. These parameters define the range of retention times within which `ms-mint` will search for peaks corresponding to your targets. By optimizing these values, you can improve the accuracy and reliability of your results.
 
 To use the `mint.opt.rt_min_max()` function, you will need to provide it with a list of retention times for your targets and the names of the mass spectrometry files containing your data. The function will then search through the data to find the optimal `rt_min` and `rt_max` values, which you can use to refine your analysis. You can then use these optimized values in conjunction with the other functions and methods of the `Mint` class to process and analyze your data.
 
-![](notebooks/peak-shapes-before-opt.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/peak-shapes-before-opt.png)
 
 Now, we can run the peak optimization with:
 
     mint.opt.rt_min_max(
         fns=[...]
         peak_labels=['Xanthine', 'Succinate', 'Citrulline'],
         plot=True, rel_height=0.7, sigma=50, col_wrap=1, aspect=3,
@@ -142,34 +149,34 @@
 
 The `mint.opt.rt_min_max()` function in the ms-mint library allows you to optimize the `rt_min` and `rt_max` values for your analysis. These values define the range of retention times within which ms-mint will search for peaks corresponding to your targets. By optimizing these values, you can improve the accuracy and reliability of your results.
 
 If you do not provide a list of peak_labels to the `mint.opt.rt_min_max()` function, it will run the optimization for all metabolites. Similarly, if you do not provide a list of filenames for the fn parameter, the function will use all of the files currently loaded into mint.ms_files. It is generally recommended to use a maximum of 20-40 files for the optimization process. If you have run a set of standards along with your samples (which is highly recommended), you can use the standard files to perform the optimization.
 
 After running the optimization, it is a good idea to perform a manual fine-tuning of the `rt_min` and `rt_max` values, especially for complicated peaks (peaks with multiple components, noisy peaks, etc.). You can use the `mint.plot.peak_shapes()` function to visualize the peak shapes and identify any areas that may require further attention.
     
-![](notebooks/optimize-rt_min_max.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/optimize-rt_min_max.png)
 
 The black lines indicates the average intensity across all files used for the optimization. The orange dotted lines show the shape of the gaussian function used to weight the mean intensities for peak selection. The orange horizontal lines indicate the peak width and the blue `x`s show the identified peak maxima. The green shaded areas show the Rt ranges which were selected by the algorithm.
 
 Then we apply the changes and plot the new peak shapes:
 
     mint.run()
     mint.plot.peak_shapes(col_wrap=3)
 
-![](notebooks/peak-shapes-after-opt.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/peak-shapes-after-opt.png)
 
 As you can see, the shapes of Xanthine, Succinate, Citrulline look much better.
 
 ## Plotting and data exploration
 
 The `Mint` class has a few convenient methods to visualize and explore the processed data. The results can be viewed directly in JupyterLab or stored to files using `matplotlib` and `seaborn` syntax. The figures are matplotlib objects and can be easily customised. 
 
 ## Plot peak shapes
 
-![](notebooks/peak-shapes-after-opt.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/peak-shapes-after-opt.png)
 
     mint.plot.peak_shapes(col_wrap = 3)
 
 The method uses seaborn [sns.relplot()](https://seaborn.pydata.org/generated/seaborn.relplot.html) function and keyword arguments are passed on. 
 
 ## Hierarchical clustering
 Mint ca be used to cluster the extracted data. An agglomerative hierarchical clustering is a bottom-up clustering technique where each data point starts as its own cluster and then are merged with other clusters in a hierarchical manner based on their proximity or similarity until a single cluster is formed or a specified stopping criteria is met. The proximity is usually determined by a distance metric, such as Euclidean distance, and the similarity is usually determined by a linkage function, such as ward linkage or complete linkage. The result is a tree-like representation called a dendrogram, which can be used to determine the number of clusters and the cluster assignments of the data points.
@@ -196,29 +203,29 @@
         transform_filenames_func="basename",  # Transformation function to shorten filenames
         transposed=False,  # Transpose the plot     
         top_height=2,  # Height of the top-dendrogram
         left_width=2,  # Width of the left-dendrogram
         cmap=None  # Name of a matplotlib color map                
     )
 
-![](notebooks/hierarchical_clustering.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/hierarchical_clustering.png)
 
 ## Principal Components Analysis
 
 Principal Component Analysis (PCA) is a widely used statistical technique for dimensionality reduction. It transforms the original high-dimensional data into a new set of linearly uncorrelated variables, called Principal Components (PCs), that capture the maximum variance in the data. The first PC accounts for the largest variance in the data, the second PC for the second largest variance, and so on. PCA is commonly used for data visualization, data compression, and noise reduction. By reducing the number of dimensions in the data, PCA allows us to more easily identify patterns and relationships in the data.
 
 Before clustering the data can be transformed and scaled. By default log2p1(x) = log_2(x+1) is used to transform the data and the standard scaler (z-scores) is used to normalize the variables for each target.
 
     mint.pca.run(n_components=5)
     
 After running the PCA the results can be plotted with:    
     
     mint.pca.plot.pairplot(n_components=5, interactive=False)
     
-![](notebooks/pca-pairplot.png)
+![](https://raw.githubusercontent.com/LewisResearchGroup/ms-mint/develop/notebooks/pca-pairplot.png)
 
 ## FAQ
 ### What is a target list
 A target list is a pandas dataframe with specific columns. 
 
 -   **peak_label**: string, Label of the peak (must be unique).
 -   **mz_mean**: numeric value, theoretical m/z value of the target ion to extract.
```

### Comparing `ms-mint-0.2.4/ms_mint.egg-info/SOURCES.txt` & `ms-mint-0.2.5/ms_mint.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
+ms_mint/Chromatogram.py
 ms_mint/Mint.py
+ms_mint/MintPlotter.py
+ms_mint/TargetOptimizer.py
 ms_mint/__init__.py
 ms_mint/_version.py
-ms_mint/chromatogram.py
 ms_mint/filelock.py
 ms_mint/filters.py
 ms_mint/io.py
 ms_mint/matplotlib_tools.py
 ms_mint/notebook.py
 ms_mint/pca.py
 ms_mint/plotly_tools.py
```

### Comparing `ms-mint-0.2.4/scripts/ms-mint-convert.py` & `ms-mint-0.2.5/scripts/ms-mint-convert.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.4/setup.py` & `ms-mint-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.4/versioneer.py` & `ms-mint-0.2.5/versioneer.py`

 * *Files identical despite different names*

