# Comparing `tmp/dendromatics-0.2.0.tar.gz` & `tmp/dendromatics-0.2.1.tar.gz`

## Comparing `dendromatics-0.2.0.tar` & `dendromatics-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 dendromatics-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 dendromatics-0.2.0/readthedocs.yaml
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dendromatics-0.2.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 dendromatics-0.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/Makefile
--rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/algorithm.rst
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/cc_plugin.rst
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/conf.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/dendromatics.rst
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/examples.rst
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/executable.rst
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/index.rst
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/installation.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/make.bat
--rw-r--r--   0        0        0   252269 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/_static/3dfin_logo.png
--rw-r--r--   0        0        0   270012 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/_static/dendromatics_logo.png
--rw-r--r--   0        0        0   113056 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/_static/height-normalization.jpg
--rw-r--r--   0        0        0    45823 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/_static/individualized_trees.jpg
--rw-r--r--   0        0        0   109342 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/_static/sections_and_axes.jpg
--rw-r--r--   0        0        0   210688 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/_static/stripe_and_groups.jpg
--rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 dendromatics-0.2.0/docs/_static/tree_height.jpg
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 dendromatics-0.2.0/examples/example.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/__about__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/__init__.py
--rw-r--r--   0        0        0    13686 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/draw.py
--rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/ground.py
--rw-r--r--   0        0        0    18686 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/individualize.py
--rw-r--r--   0        0        0    42900 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/sections.py
--rw-r--r--   0        0        0     8424 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/stripe.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/voxel/__init__.py
--rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 dendromatics-0.2.0/src/dendromatics/voxel/voxel.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 dendromatics-0.2.0/tests/test_ground.py
--rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 dendromatics-0.2.0/tests/test_voxel.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 dendromatics-0.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 dendromatics-0.2.0/LICENSE
--rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 dendromatics-0.2.0/README.rst
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 dendromatics-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7675 2020-02-02 00:00:00.000000 dendromatics-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dendromatics-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 dendromatics-0.2.1/readthedocs.yaml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dendromatics-0.2.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 dendromatics-0.2.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/Makefile
+-rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/algorithm.rst
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/cc_plugin.rst
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/conf.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/dendromatics.rst
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/examples.rst
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/executable.rst
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/index.rst
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/installation.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/make.bat
+-rw-r--r--   0        0        0   252269 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/_static/3dfin_logo.png
+-rw-r--r--   0        0        0   270012 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/_static/dendromatics_logo.png
+-rw-r--r--   0        0        0   113056 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/_static/height-normalization.jpg
+-rw-r--r--   0        0        0    45823 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/_static/individualized_trees.jpg
+-rw-r--r--   0        0        0   109342 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/_static/sections_and_axes.jpg
+-rw-r--r--   0        0        0   210688 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/_static/stripe_and_groups.jpg
+-rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 dendromatics-0.2.1/docs/_static/tree_height.jpg
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 dendromatics-0.2.1/examples/example.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dendromatics-0.2.1/src/dendromatics/__about__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 dendromatics-0.2.1/src/dendromatics/__init__.py
+-rw-r--r--   0        0        0    13686 2020-02-02 00:00:00.000000 dendromatics-0.2.1/src/dendromatics/draw.py
+-rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 dendromatics-0.2.1/src/dendromatics/ground.py
+-rw-r--r--   0        0        0    18686 2020-02-02 00:00:00.000000 dendromatics-0.2.1/src/dendromatics/individualize.py
+-rw-r--r--   0        0        0    42900 2020-02-02 00:00:00.000000 dendromatics-0.2.1/src/dendromatics/sections.py
+-rw-r--r--   0        0        0     8424 2020-02-02 00:00:00.000000 dendromatics-0.2.1/src/dendromatics/stripe.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dendromatics-0.2.1/src/dendromatics/voxel/__init__.py
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 dendromatics-0.2.1/src/dendromatics/voxel/voxel.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 dendromatics-0.2.1/tests/test_ground.py
+-rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 dendromatics-0.2.1/tests/test_voxel.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 dendromatics-0.2.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 dendromatics-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 dendromatics-0.2.1/README.rst
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 dendromatics-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7675 2020-02-02 00:00:00.000000 dendromatics-0.2.1/PKG-INFO
```

### Comparing `dendromatics-0.2.0/CHANGELOG.md` & `dendromatics-0.2.1/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.2.1] - 2023-07-10
+
+### Fixed
+
+- Fixed a bug in clean_ground(). It caused that, during denoising step before dtm computation, the removed points (noise) were independent of the voxel resolution used.
+
 ## [0.2.0] - 2023-06-02
 
 ### Added
 
 - This CHANGELOG file.
 - Documentation is now live at `ReadTheDocs.io`.
 - A `process_hook` in order to replace the current embedded progress logging.
```

### Comparing `dendromatics-0.2.0/readthedocs.yaml` & `dendromatics-0.2.1/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/.github/workflows/build.yml` & `dendromatics-0.2.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/.github/workflows/test.yml` & `dendromatics-0.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/docs/Makefile` & `dendromatics-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/docs/algorithm.rst` & `dendromatics-0.2.1/docs/algorithm.rst`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/docs/conf.py` & `dendromatics-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/docs/dendromatics.rst` & `dendromatics-0.2.1/docs/dendromatics.rst`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/docs/examples.rst` & `dendromatics-0.2.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/docs/executable.rst` & `dendromatics-0.2.1/docs/executable.rst`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/docs/index.rst` & `dendromatics-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/docs/make.bat` & `dendromatics-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/docs/_static/3dfin_logo.png` & `dendromatics-0.2.1/docs/_static/3dfin_logo.png`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/docs/_static/dendromatics_logo.png` & `dendromatics-0.2.1/docs/_static/dendromatics_logo.png`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/docs/_static/height-normalization.jpg` & `dendromatics-0.2.1/docs/_static/height-normalization.jpg`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/docs/_static/individualized_trees.jpg` & `dendromatics-0.2.1/docs/_static/individualized_trees.jpg`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/docs/_static/sections_and_axes.jpg` & `dendromatics-0.2.1/docs/_static/sections_and_axes.jpg`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/docs/_static/stripe_and_groups.jpg` & `dendromatics-0.2.1/docs/_static/stripe_and_groups.jpg`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/docs/_static/tree_height.jpg` & `dendromatics-0.2.1/docs/_static/tree_height.jpg`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/examples/example.py` & `dendromatics-0.2.1/examples/example.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/src/dendromatics/draw.py` & `dendromatics-0.2.1/src/dendromatics/draw.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/src/dendromatics/ground.py` & `dendromatics-0.2.1/src/dendromatics/ground.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,16 @@
     """
 
     vox_cloud, vox_to_cloud_ind, cloud_to_vox_ind = voxelate(
         cloud, res_ground, res_ground, with_n_points=False
     )
     # Cluster labels are appended to the FILTERED cloud. They map each point to
     # the cluster they belong to, according to the clustering algorithm.
-    clustering = DBSCAN(eps=0.3, min_samples=min_points).fit(vox_cloud)
+    eps = res_ground * 1.75
+    clustering = DBSCAN(eps=eps, min_samples=min_points).fit(vox_cloud)
 
     cloud_labs = np.append(
         cloud, np.expand_dims(clustering.labels_[vox_to_cloud_ind], axis=1), axis=1
     )
 
     # Set of all cluster labels and their cardinality: cluster_id = {1,...,K},
     # K = 'number of points'.
```

### Comparing `dendromatics-0.2.0/src/dendromatics/individualize.py` & `dendromatics-0.2.1/src/dendromatics/individualize.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/src/dendromatics/sections.py` & `dendromatics-0.2.1/src/dendromatics/sections.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/src/dendromatics/stripe.py` & `dendromatics-0.2.1/src/dendromatics/stripe.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/src/dendromatics/voxel/voxel.py` & `dendromatics-0.2.1/src/dendromatics/voxel/voxel.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/tests/test_ground.py` & `dendromatics-0.2.1/tests/test_ground.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/tests/test_voxel.py` & `dendromatics-0.2.1/tests/test_voxel.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/.gitignore` & `dendromatics-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/LICENSE` & `dendromatics-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/README.rst` & `dendromatics-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/pyproject.toml` & `dendromatics-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dendromatics-0.2.0/PKG-INFO` & `dendromatics-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dendromatics
-Version: 0.2.0
+Version: 0.2.1
 Summary: Automatic dendrometry and forest inventory for terrestrial point clouds
 Project-URL: Source, https://github.com/3DFin/dendromatics
 Project-URL: Documentation, https://dendromatics.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/3DFin/dendromatics/issues
 Author-email: Carlos Cabo <carloscabo@uniovi.es>, Diego Laino <diegolainor@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
```

