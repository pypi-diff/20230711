# Comparing `tmp/matgl-0.7.0.tar.gz` & `tmp/matgl-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.7.0.tar", last modified: Sun Jun 25 23:04:09 2023, max compression
+gzip compressed data, was "matgl-0.7.1.tar", last modified: Tue Jul 11 18:55:56 2023, max compression
```

## Comparing `matgl-0.7.0.tar` & `matgl-0.7.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.145969 matgl-0.7.0/
--rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-04-22 15:15:07.000000 matgl-0.7.0/LICENSE
--rw-r--r--   0 shyue      (501) staff       (20)    13724 2023-06-25 23:04:09.145716 matgl-0.7.0/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)    12555 2023-06-25 22:56:34.000000 matgl-0.7.0/README.md
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.140653 matgl-0.7.0/matgl/
--rw-r--r--   0 shyue      (501) staff       (20)      394 2023-06-13 20:15:14.000000 matgl-0.7.0/matgl/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.141721 matgl-0.7.0/matgl/apps/
--rw-r--r--   0 shyue      (501) staff       (20)      180 2023-06-13 20:15:14.000000 matgl-0.7.0/matgl/apps/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4221 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/apps/pes.py
--rw-r--r--   0 shyue      (501) staff       (20)     4777 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/cli.py
--rw-r--r--   0 shyue      (501) staff       (20)     1996 2023-06-15 14:38:52.000000 matgl-0.7.0/matgl/config.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.141961 matgl-0.7.0/matgl/data/
--rw-r--r--   0 shyue      (501) staff       (20)       55 2023-06-13 20:15:14.000000 matgl-0.7.0/matgl/data/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2542 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/data/transformer.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.142309 matgl-0.7.0/matgl/ext/
--rw-r--r--   0 shyue      (501) staff       (20)      118 2023-06-13 20:15:14.000000 matgl-0.7.0/matgl/ext/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    15658 2023-06-25 22:58:13.000000 matgl-0.7.0/matgl/ext/ase.py
--rw-r--r--   0 shyue      (501) staff       (20)     4875 2023-06-25 22:58:47.000000 matgl-0.7.0/matgl/ext/pymatgen.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.142736 matgl-0.7.0/matgl/graph/
--rw-r--r--   0 shyue      (501) staff       (20)       52 2023-06-13 20:15:14.000000 matgl-0.7.0/matgl/graph/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     5188 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/graph/compute.py
--rw-r--r--   0 shyue      (501) staff       (20)     2232 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/graph/converters.py
--rw-r--r--   0 shyue      (501) staff       (20)    11720 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/graph/data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.143806 matgl-0.7.0/matgl/layers/
--rw-r--r--   0 shyue      (501) staff       (20)      716 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/layers/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2037 2023-06-21 20:31:41.000000 matgl-0.7.0/matgl/layers/_activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     2996 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/layers/_atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)    12641 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/layers/_basis.py
--rw-r--r--   0 shyue      (501) staff       (20)     2231 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/layers/_bond.py
--rw-r--r--   0 shyue      (501) staff       (20)     6029 2023-06-20 18:49:06.000000 matgl-0.7.0/matgl/layers/_core.py
--rw-r--r--   0 shyue      (501) staff       (20)     3578 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/layers/_embedding.py
--rw-r--r--   0 shyue      (501) staff       (20)    16602 2023-06-20 18:49:06.000000 matgl-0.7.0/matgl/layers/_graph_convolution.py
--rw-r--r--   0 shyue      (501) staff       (20)     3935 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/layers/_readout.py
--rw-r--r--   0 shyue      (501) staff       (20)     4053 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/layers/_three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.144202 matgl-0.7.0/matgl/models/
--rw-r--r--   0 shyue      (501) staff       (20)      187 2023-06-13 20:15:14.000000 matgl-0.7.0/matgl/models/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    11949 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/models/_m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     9153 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/models/_megnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     2255 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/models/_wrappers.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.145199 matgl-0.7.0/matgl/utils/
--rw-r--r--   0 shyue      (501) staff       (20)       61 2023-06-13 20:15:14.000000 matgl-0.7.0/matgl/utils/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1372 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/utils/cutoff.py
--rw-r--r--   0 shyue      (501) staff       (20)    10549 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/utils/io.py
--rw-r--r--   0 shyue      (501) staff       (20)     7129 2023-06-20 18:49:06.000000 matgl-0.7.0/matgl/utils/maths.py
--rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-04-22 15:15:07.000000 matgl-0.7.0/matgl/utils/sb_roots.npy
--rw-r--r--   0 shyue      (501) staff       (20)    13462 2023-06-25 22:56:34.000000 matgl-0.7.0/matgl/utils/training.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.141498 matgl-0.7.0/matgl.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)    13724 2023-06-25 23:04:09.000000 matgl-0.7.0/matgl.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     1024 2023-06-25 23:04:09.000000 matgl-0.7.0/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-25 23:04:09.000000 matgl-0.7.0/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       39 2023-06-25 23:04:09.000000 matgl-0.7.0/matgl.egg-info/entry_points.txt
--rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-25 23:04:09.000000 matgl-0.7.0/matgl.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-25 23:04:09.000000 matgl-0.7.0/matgl.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)     2530 2023-06-25 22:56:34.000000 matgl-0.7.0/pyproject.toml
--rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-25 23:04:09.146019 matgl-0.7.0/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     2014 2023-06-25 23:01:46.000000 matgl-0.7.0/setup.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-25 23:04:09.145310 matgl-0.7.0/tests/
--rw-r--r--   0 shyue      (501) staff       (20)      194 2023-06-15 15:33:33.000000 matgl-0.7.0/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.332251 matgl-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-11 18:55:44.000000 matgl-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-07-11 18:55:56.328251 matgl-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-07-11 18:55:44.000000 matgl-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.324252 matgl-0.7.1/matgl/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.324252 matgl-0.7.1/matgl/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/apps/pes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.324252 matgl-0.7.1/matgl/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/data/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.324252 matgl-0.7.1/matgl/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15546 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/ext/ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/ext/pymatgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.324252 matgl-0.7.1/matgl/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/graph/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/graph/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12742 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/graph/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.328251 matgl-0.7.1/matgl/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_atom_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12725 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_graph_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/layers/_three_body.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.328251 matgl-0.7.1/matgl/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/models/_m3gnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/models/_megnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/models/_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.328251 matgl-0.7.1/matgl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/utils/cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/utils/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131200 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/utils/sb_roots.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    13697 2023-07-11 18:55:44.000000 matgl-0.7.1/matgl/utils/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.324252 matgl-0.7.1/matgl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-07-11 18:55:56.000000 matgl-0.7.1/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-11 18:55:56.000000 matgl-0.7.1/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:55:56.000000 matgl-0.7.1/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 18:55:56.000000 matgl-0.7.1/matgl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 18:55:56.000000 matgl-0.7.1/matgl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 18:55:56.000000 matgl-0.7.1/matgl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-11 18:55:44.000000 matgl-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:55:56.332251 matgl-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-11 18:55:44.000000 matgl-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:55:56.328251 matgl-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-11 18:55:44.000000 matgl-0.7.1/tests/test_config.py
```

### Comparing `matgl-0.7.0/LICENSE` & `matgl-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/PKG-INFO` & `matgl-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.7.0
+Version: 0.7.1
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `matgl-0.7.0/README.md` & `matgl-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/apps/pes.py` & `matgl-0.7.1/matgl/apps/pes.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,9 +114,8 @@
                         / g.ndata["volume"][count_node + num_nodes]
                     )
                 )
                 count_edge = count_edge + num_edges
                 num_nodes = g.batch_num_nodes()[graph_id]
                 count_node = count_node + num_nodes
             stresses = torch.cat(sts)
-
         return total_energies, forces, stresses, hessian
```

### Comparing `matgl-0.7.0/matgl/cli.py` & `matgl-0.7.1/matgl/cli.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/config.py` & `matgl-0.7.1/matgl/config.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/data/transformer.py` & `matgl-0.7.1/matgl/data/transformer.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/ext/ase.py` & `matgl-0.7.1/matgl/ext/ase.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
         Returns:
             g: DGL graph
             state_attr: state features
         """
         numerical_tol = 1.0e-8
         pbc = np.array([1, 1, 1], dtype=int)
         element_types = self.element_types
-        Z = np.array([np.eye(len(element_types))[element_types.index(i.symbol)] for i in atoms])
         lattice_matrix = np.ascontiguousarray(np.array(atoms.get_cell()), dtype=float)
         volume = atoms.get_volume()
         cart_coords = np.ascontiguousarray(np.array(atoms.get_positions()), dtype=float)
         src_id, dst_id, images, bond_dist = find_points_in_spheres(
             cart_coords,
             cart_coords,
             r=self.cutoff,
@@ -98,15 +97,14 @@
         )
         g, state_attr = super().get_graph_from_processed_structure(
             AseAtomsAdaptor().get_structure(atoms),
             src_id,
             dst_id,
             images,
             [lattice_matrix],
-            Z,
             element_types,
             cart_coords,
         )
         g.ndata["volume"] = torch.tensor([volume] * g.num_nodes())
         return g, state_attr
```

### Comparing `matgl-0.7.0/matgl/ext/pymatgen.py` & `matgl-0.7.1/matgl/ext/pymatgen.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,30 +52,28 @@
 
         :param mol: pymatgen molecule object
         :return: (dgl graph, state features)
         """
         natoms = len(mol)
         R = mol.cart_coords
         element_types = self.element_types
-        Z = np.array([np.eye(len(element_types))[element_types.index(site.specie.symbol)] for site in mol])
         np.array([site.specie.Z for site in mol])
         weight = mol.composition.weight / len(mol)
         dist = np.linalg.norm(R[:, None, :] - R[None, :, :], axis=-1)
         dists = mol.distance_matrix.flatten()
         nbonds = (np.count_nonzero(dists <= self.cutoff) - natoms) / 2
         nbonds /= natoms
         adj = sp.csr_matrix(dist <= self.cutoff) - sp.eye(natoms, dtype=np.bool_)
         adj = adj.tocoo()
         g, _ = super().get_graph_from_processed_structure(
             structure=mol,
             src_id=adj.row,
             dst_id=adj.col,
             images=torch.zeros(len(adj.row), 3),
             lattice_matrix=torch.zeros(1, 3, 3),
-            Z=Z,
             element_types=element_types,
             cart_coords=R,
         )
         state_attr = [weight, nbonds]
         return g, state_attr
 
 
@@ -103,15 +101,14 @@
         :return:
             g: DGL graph
             state_attr: state features
         """
         numerical_tol = 1.0e-8
         pbc = np.array([1, 1, 1], dtype=int)
         element_types = self.element_types
-        Z = np.array([np.eye(len(element_types))[element_types.index(site.specie.symbol)] for site in structure])
         lattice_matrix = np.ascontiguousarray(np.array(structure.lattice.matrix), dtype=float)
         volume = structure.volume
         cart_coords = np.ascontiguousarray(np.array(structure.cart_coords), dtype=float)
         src_id, dst_id, images, bond_dist = find_points_in_spheres(
             cart_coords,
             cart_coords,
             r=self.cutoff,
@@ -128,13 +125,12 @@
         )
         g, state_attr = super().get_graph_from_processed_structure(
             structure,
             src_id,
             dst_id,
             images,
             [lattice_matrix],
-            Z,
             element_types,
             cart_coords,
         )
         g.ndata["volume"] = torch.tensor([volume] * g.num_nodes())
         return g, state_attr
```

### Comparing `matgl-0.7.0/matgl/graph/compute.py` & `matgl-0.7.1/matgl/graph/compute.py`

 * *Files 21% similar despite different names*

```diff
@@ -56,16 +56,16 @@
     for n in n_atoms:
         j = i + n
         n_triple_s.append(torch.sum(n_triple_i[i:j]))
         i = j
 
     src_id, dst_id = (triple_bond_indices[:, 0], triple_bond_indices[:, 1])
     l_g = dgl.graph((src_id, dst_id))
-    three_body_id = np.unique(triple_bond_indices)
-    max_three_body_id = max(np.concatenate([three_body_id + 1, [0]]))
+    three_body_id = torch.unique(triple_bond_indices)
+    max_three_body_id = max(torch.cat([three_body_id + 1, torch.tensor([0])]))
     l_g.ndata["bond_dist"] = g.edata["bond_dist"][:max_three_body_id]
     l_g.ndata["bond_vec"] = g.edata["bond_vec"][:max_three_body_id]
     l_g.ndata["pbc_offset"] = g.edata["pbc_offset"][:max_three_body_id]
     l_g.ndata["n_triple_ij"] = n_triple_ij[:max_three_body_id]
     n_triple_s = torch.tensor(n_triple_s, dtype=torch.int64)  # type: ignore
     return l_g, triple_bond_indices, n_triple_ij, n_triple_i, n_triple_s
 
@@ -99,41 +99,55 @@
     edges: DGL graph edges
 
     Returns:
     cos_theta: torch.Tensor
     phi: torch.Tensor
     triple_bond_lengths (torch.tensor):
     """
+    angles = compute_theta(edges, cosine=True)
+    angles.update(
+        {
+            "phi": torch.zeros_like(angles["cos_theta"]),
+        }
+    )
+    return angles
+
+
+def compute_theta(edges: dgl.udf.EdgeBatch, cosine: bool = False) -> dict[str, torch.Tensor]:
+    """User defined dgl function to calculate bond angles from edges in a graph.
+
+    Args:
+        edges: DGL graph edges
+        cosine: Whether to return the cosine of the angle or the angle itself
+
+    Returns:
+        dict[str, torch.Tensor]: Dictionary containing bond angles and distances
+    """
     vec1 = edges.src["bond_vec"]
     vec2 = edges.dst["bond_vec"]
-    cosine_theta = torch.sum(vec1 * vec2, dim=1) / (torch.norm(vec1, dim=1) * torch.norm(vec2, dim=1))
-    return {
-        "cos_theta": cosine_theta,
-        "phi": torch.zeros_like(cosine_theta),
-        "triple_bond_lengths": edges.dst["bond_dist"],
-    }
+    key = "cos_theta" if cosine else "theta"
+    val = torch.sum(vec1 * vec2, dim=1) / (torch.norm(vec1, dim=1) * torch.norm(vec2, dim=1))
+    if not cosine:
+        val = torch.acos(val)
+    return {key: val, "triple_bond_lengths": edges.dst["bond_dist"]}
 
 
-def create_line_graph(g_batched: dgl.DGLGraph, threebody_cutoff: float):
-    """Calculate the three body indices from pair atom indices.
+def create_line_graph(g: dgl.DGLGraph, threebody_cutoff: float):
+    """
+    Calculate the three body indices from pair atom indices.
 
     Args:
-        g_batched: Batched DGL graph
+        g: DGL graph
         threebody_cutoff (float): cutoff for three-body interactions
 
     Returns:
         l_g: DGL graph containing three body information from graph
     """
-    g_unbatched = dgl.unbatch(g_batched)
-    l_g_unbatched = []
-    for g in g_unbatched:
-        valid_three_body = g.edata["bond_dist"] <= threebody_cutoff
-        src_id_with_three_body = g.edges()[0][valid_three_body]
-        dst_id_with_three_body = g.edges()[1][valid_three_body]
-        graph_with_three_body = dgl.graph((src_id_with_three_body, dst_id_with_three_body))
-        graph_with_three_body.edata["bond_dist"] = g.edata["bond_dist"][valid_three_body]
-        graph_with_three_body.edata["bond_vec"] = g.edata["bond_vec"][valid_three_body]
-        graph_with_three_body.edata["pbc_offset"] = g.edata["pbc_offset"][valid_three_body]
-        l_g, triple_bond_indices, n_triple_ij, n_triple_i, n_triple_s = compute_3body(graph_with_three_body)
-        l_g_unbatched.append(l_g)
-    l_g_batched = dgl.batch(l_g_unbatched)
-    return l_g_batched
+    valid_three_body = g.edata["bond_dist"] <= threebody_cutoff
+    src_id_with_three_body = g.edges()[0][valid_three_body]
+    dst_id_with_three_body = g.edges()[1][valid_three_body]
+    graph_with_three_body = dgl.graph((src_id_with_three_body, dst_id_with_three_body))
+    graph_with_three_body.edata["bond_dist"] = g.edata["bond_dist"][valid_three_body]
+    graph_with_three_body.edata["bond_vec"] = g.edata["bond_vec"][valid_three_body]
+    graph_with_three_body.edata["pbc_offset"] = g.edata["pbc_offset"][valid_three_body]
+    l_g, triple_bond_indices, n_triple_ij, n_triple_i, n_triple_s = compute_3body(graph_with_three_body)
+    return l_g
```

### Comparing `matgl-0.7.0/matgl/graph/converters.py` & `matgl-0.7.1/matgl/graph/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,39 +24,36 @@
     def get_graph_from_processed_structure(
         self,
         structure,
         src_id,
         dst_id,
         images,
         lattice_matrix,
-        Z,
         element_types,
         cart_coords,
     ) -> tuple[dgl.DGLGraph, list]:
         """Construct a dgl graph from processed structure and bond information.
 
         Args:
             structure: Input crystals or molecule of pymatgen structure or molecule types.
             src_id: site indices for starting point of bonds.
             dst_id: site indices for destination point of bonds.
             images: the periodic image offsets for the bonds.
             lattice_matrix: lattice information of the structure.
-            Z: Atomic number information of all atoms in the structure.
             element_types: Element symbols of all atoms in the structure.
             cart_coords: Cartisian coordinates of all atoms in the structure.
 
         Returns:
             DGLGraph object, state_attr
 
         """
         u, v = tensor(src_id), tensor(dst_id)
         g = dgl.graph((u, v))
         n_missing_node = len(structure) - g.num_nodes()  # isolated atoms without bonds
         g.add_nodes(n_missing_node)
         g.edata["pbc_offset"] = torch.tensor(images)
         g.edata["lattice"] = tensor(np.repeat(lattice_matrix, g.num_edges(), axis=0))
-        g.ndata["attr"] = tensor(Z)
         g.ndata["node_type"] = tensor(np.hstack([[element_types.index(site.specie.symbol)] for site in structure]))
         g.ndata["pos"] = tensor(cart_coords)
         state_attr = [0.0, 0.0]
         g.edata["pbc_offshift"] = torch.matmul(tensor(images), tensor(lattice_matrix[0]))
         return g, state_attr
```

### Comparing `matgl-0.7.0/matgl/graph/data.py` & `matgl-0.7.1/matgl/graph/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,20 +16,26 @@
 from matgl.graph.compute import compute_pair_vector_and_distance, create_line_graph
 from matgl.layers import BondExpansion
 
 if TYPE_CHECKING:
     from matgl.graph.converters import GraphConverter
 
 
-def collate_fn(batch):
+def collate_fn(batch, include_line_graph: bool = False):
     """Merge a list of dgl graphs to form a batch."""
-    graphs, labels, state_attr = map(list, zip(*batch))
+    if include_line_graph:
+        graphs, line_graphs, state_attr, labels = map(list, zip(*batch))
+    else:
+        graphs, state_attr, labels = map(list, zip(*batch))
     g = dgl.batch(graphs)
     labels = torch.tensor(labels, dtype=torch.float32)
     state_attr = torch.stack(state_attr)
+    if include_line_graph:
+        l_g = dgl.batch(line_graphs)
+        return g, l_g, state_attr, labels
     return g, labels, state_attr
 
 
 def collate_fn_efs(batch):
     """Merge a list of dgl graphs to form a batch."""
     graphs, line_graphs, state_attr, energies, forces, stresses = map(list, zip(*batch))
     g = dgl.batch(graphs)
@@ -149,34 +155,35 @@
         Returns: True if file exists.
         """
         return os.path.exists(filename)
 
     def process(self) -> tuple:
         """Convert Pymatgen structure into dgl graphs."""
         num_graphs = self.labels.shape[0]
-        self.graphs = []
-        self.state_attr = []
+        graphs = []
+        state_attrs = []
         bond_expansion = BondExpansion(
             rbf_type="Gaussian", initial=self.initial, final=self.final, num_centers=self.num_centers, width=self.width
         )
         for idx in trange(num_graphs):
             structure = self.structures[idx]
             graph, state_attr = self.converter.get_graph(structure)
             bond_vec, bond_dist = compute_pair_vector_and_distance(graph)
             graph.edata["edge_attr"] = bond_expansion(bond_dist)
-            self.graphs.append(graph)
-            self.state_attr.append(state_attr)
+            graphs.append(graph)
+            state_attrs.append(state_attr)
         if self.graph_labels is not None:
             if np.array(self.graph_labels).dtype == "int64":
-                self.state_attr = torch.tensor(self.graph_labels).long()  # type: ignore
+                state_attrs = torch.tensor(self.graph_labels).long()  # type: ignore
             else:
-                self.state_attr = torch.tensor(self.graph_labels)  # type: ignore
+                state_attrs = torch.tensor(self.graph_labels)  # type: ignore
         else:
-            self.state_attr = torch.tensor(self.state_attr)  # type: ignore
-
+            state_attrs = torch.tensor(state_attrs)  # type: ignore
+        self.graphs = graphs
+        self.state_attr = state_attrs
         return self.graphs, self.state_attr
 
     def save(self, filename: str = "dgl_graph.bin", filename_state_attr: str = "state_attr.pt"):
         """Save dgl graphs
         Args:
         :filename: Name of file storing dgl graphs
         :filename_state_attr: Name of file storing graph attrs.
@@ -193,101 +200,113 @@
         """
         self.graphs, label_dict = load_graphs(filename)
         self.label = torch.stack([label_dict[key] for key in self.label_keys], dim=1)
         self.state_attr = torch.load("state_attr.pt")
 
     def __getitem__(self, idx: int):
         """Get graph and label with idx."""
-        return self.graphs[idx], self.labels[idx], self.state_attr[idx]
+        return self.graphs[idx], self.state_attr[idx], self.labels[idx]
 
     def __len__(self):
         """Get size of dataset."""
         return len(self.graphs)
 
 
 class M3GNetDataset(DGLDataset):
     """Create a dataset including dgl graphs."""
 
     def __init__(
         self,
-        structures: list,
-        energies: list,
-        forces: list,
-        stresses: None | list,
         converter: GraphConverter,
         threebody_cutoff: float,
+        structures: list,
+        energies: list | None = None,
+        forces: list | None = None,
+        stresses: list | None = None,
+        labels: list | None = None,
         name="M3GNETDataset",
+        label_name: str | None = None,
         graph_labels: list | None = None,
     ):
         """
         Args:
+            converter: dgl graph converter
+            threebody_cutoff: cutoff for three body
             structures: Pymatgen structure
             energies: Target energies
             forces: Target forces
             stresses: Target stresses
-            converter: dgl graph converter
-            threebody_cutoff: cutoff for three body
+            labels: target properties
             name: name of dataset
+            label_name: name of target properties
             graph_labels: state attributes.
         """
         self.converter = converter
         self.structures = structures
         self.energies = energies
         self.forces = forces
+        self.labels = labels
+        self.label_name = label_name
         self.threebody_cutoff = threebody_cutoff
-        self.stresses = np.zeros(len(self.energies)) if stresses is None else stresses
+        self.stresses = np.zeros(len(self.structures)) if stresses is None else stresses
         self.graph_labels = graph_labels
         super().__init__(name=name)
 
     def has_cache(self, filename: str = "dgl_graph.bin") -> bool:
         """Check if the dgl_graph.bin exists or not
         Args:
             :filename: Name of file storing dgl graphs
         Returns: True if file exists.
         """
         return os.path.exists(filename)
 
     def process(self) -> tuple:
         """Convert Pymatgen structure into dgl graphs."""
-        num_graphs = len(self.energies)
-        self.graphs = []
-        self.line_graphs = []
-        self.state_attr = []
+        num_graphs = len(self.structures)
+        graphs = []
+        line_graphs = []
+        state_attrs = []
         for idx in trange(num_graphs):
             structure = self.structures[idx]
             graph, state_attr = self.converter.get_graph(structure)
-            self.graphs.append(graph)
-            self.state_attr.append(state_attr)
+            graphs.append(graph)
+            state_attrs.append(state_attr)
             bond_vec, bond_dist = compute_pair_vector_and_distance(graph)
             graph.edata["bond_vec"] = bond_vec
             graph.edata["bond_dist"] = bond_dist
             line_graph = create_line_graph(graph, self.threebody_cutoff)
-            line_graph.ndata.pop("bond_vec")
-            line_graph.ndata.pop("bond_dist")
-            line_graph.ndata.pop("pbc_offset")
-            self.line_graphs.append(line_graph)
+            for name in ["bond_vec", "bond_dist", "pbc_offset"]:
+                line_graph.ndata.pop(name)
+            line_graphs.append(line_graph)
         if self.graph_labels is not None:
-            self.state_attr = torch.tensor(self.graph_labels).long()  # type: ignore
+            state_attrs = torch.tensor(self.graph_labels).long()  # type: ignore
         else:
-            self.state_attr = torch.tensor(self.state_attr)  # type: ignore
+            state_attrs = torch.tensor(state_attrs)  # type: ignore
+
+        self.graphs = graphs
+        self.line_graphs = line_graphs
+        self.state_attr = state_attrs
 
         return self.graphs, self.line_graphs, self.state_attr
 
     def save(
         self,
         filename: str = "dgl_graph.bin",
         filename_line_graph: str = "dgl_line_graph.bin",
         filename_state_attr: str = "state_attr.pt",
     ):
         """Save dgl graphs
         Args:
         :filename: Name of file storing dgl graphs
         :filename_state_attr: Name of file storing graph attrs.
         """
-        labels_with_key = {"energies": self.energies, "forces": self.forces, "stresses": self.stresses}
+        if self.labels is None:
+            labels_with_key = {"energies": self.energies, "forces": self.forces, "stresses": self.stresses}
+        else:
+            labels_with_key = {self.label_name: self.labels}  # type: ignore
         save_graphs(filename, self.graphs)
         save_graphs(filename_line_graph, self.line_graphs)
         torch.save(self.state_attr, filename_state_attr)
         with open("labels.json", "w") as file:
             file.write("".join(str(labels_with_key).split("\n")))
 
     def load(
@@ -304,26 +323,31 @@
             filename_line_graph: Name of file storing dgl line graphs
             filename_state_attr: Name of file storing state attrs.
         """
         self.graphs = load_graphs(filename)
         self.line_graphs = load_graphs(filename_line_graph)
         with open("labels.json") as file:
             labels: dict = json.load(file)
-        self.energies = labels["energies"]
-        self.forces = labels["forces"]
-        self.stresses = labels["stresses"]
-        self.state_attr = torch.load("state_attr.pt")
+        if self.labels is None:
+            self.energies = labels["energies"]
+            self.forces = labels["forces"]
+            self.stresses = labels["stresses"]
+            self.state_attr = torch.load("state_attr.pt")
+        else:
+            self.labels = labels  # type: ignore
 
     def __getitem__(self, idx: int):
         """Get graph and label with idx."""
-        return (
-            self.graphs[idx],
-            self.line_graphs[idx],
-            self.state_attr[idx],
-            self.energies[idx],
-            torch.tensor(self.forces[idx]).float(),
-            torch.tensor(self.stresses[idx]).float(),  # type: ignore
-        )
+        if self.labels is None:
+            return (
+                self.graphs[idx],
+                self.line_graphs[idx],
+                self.state_attr[idx],
+                self.energies[idx],  # type: ignore
+                torch.tensor(self.forces[idx]).float(),  # type: ignore
+                torch.tensor(self.stresses[idx]).float(),  # type: ignore
+            )
+        return (self.graphs[idx], self.line_graphs[idx], self.state_attr[idx], self.labels[idx])
 
     def __len__(self):
         """Get size of dataset."""
         return len(self.graphs)
```

### Comparing `matgl-0.7.0/matgl/layers/__init__.py` & `matgl-0.7.1/matgl/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/layers/_activations.py` & `matgl-0.7.1/matgl/layers/_activations.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/layers/_atom_ref.py` & `matgl-0.7.1/matgl/layers/_atom_ref.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 
         Returns:
             features (np.array): a matrix (num_structures, num_elements)
         """
         n = len(graphs)
         features = np.zeros(shape=(n, self.max_z))
         for i, s in enumerate(graphs):
-            one_hot_vecs = s.ndata["attr"]
-            atomic_numbers = ((one_hot_vecs == 1).nonzero(as_tuple=True)[0]).tolist()
+            atomic_numbers = s.ndata["node_type"].cpu().numpy().tolist()
             features[i] = np.bincount(atomic_numbers, minlength=self.max_z)
         return features
 
     def fit(self, graphs: list, properties: np.typing.NDArray) -> None:
         """Fit the elemental reference values for the properties.
 
         Args:
@@ -56,22 +55,26 @@
         Args:
             g: a batch of dgl graphs
             state_attr: state attributes
 
         Returns:
             offset_per_graph
         """
+        num_elements = (
+            self.property_offset.size(dim=1) if self.property_offset.ndim > 1 else self.property_offset.size(dim=0)
+        )
+        one_hot = torch.eye(num_elements)[g.ndata["node_type"]]
         if self.property_offset.ndim > 1:
             offset_batched_with_state = []
             for i in range(0, self.property_offset.size(dim=0)):
                 property_offset_batched = self.property_offset[i].repeat(g.num_nodes(), 1)
-                offset = property_offset_batched * g.ndata["attr"]
+                offset = property_offset_batched * one_hot
                 g.ndata["atomic_offset"] = torch.sum(offset, 1)
                 offset_batched = dgl.readout_nodes(g, "atomic_offset")
                 offset_batched_with_state.append(offset_batched)
             offset_batched_with_state = torch.stack(offset_batched_with_state)  # type: ignore
             return offset_batched_with_state[state_attr]  # type: ignore
         property_offset_batched = self.property_offset.repeat(g.num_nodes(), 1)
-        offset = property_offset_batched * g.ndata["attr"]
+        offset = property_offset_batched * one_hot
         g.ndata["atomic_offset"] = torch.sum(offset, 1)
         offset_batched = dgl.readout_nodes(g, "atomic_offset")
         return offset_batched
```

### Comparing `matgl-0.7.0/matgl/layers/_basis.py` & `matgl-0.7.1/matgl/layers/_basis.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         max_l: int, max order (excluding l)
         max_n: int, max number of roots used in each l
         cutoff: float, cutoff radius
         smooth: Whether to smooth the function.
         """
         self.max_l = max_l
         self.max_n = max_n
-        self.cutoff = cutoff
+        self.cutoff = torch.tensor(cutoff)
         self.smooth = smooth
         if smooth:
             self.funcs = self._calculate_smooth_symbolic_funcs()
         else:
             self.funcs = self._calculate_symbolic_funcs()
 
     @lru_cache(maxsize=128)
@@ -110,15 +110,15 @@
         r_c = r.clone()
         r_c[r_c > self.cutoff] = self.cutoff
         roots = SPHERICAL_BESSEL_ROOTS[: self.max_l, : self.max_n]
 
         results = []
         factor = torch.tensor(sqrt(2.0 / self.cutoff**3))
         for i in range(self.max_l):
-            root = roots[i]
+            root = torch.tensor(roots[i])
             func = self.funcs[i]
             func_add1 = self.funcs[i + 1]
             results.append(
                 func(r_c[:, None] * root[None, :] / self.cutoff) * factor / torch.abs(func_add1(root[None, :]))
             )
         return torch.cat(results, axis=1)
 
@@ -144,15 +144,15 @@
     """Zeroth order bessel function of the first kind.
 
     Implements the proposed 1D radial basis function in terms of zeroth order bessel function of the first kind with
     increasing number of roots and a given cutoff.
 
     Details are given in: https://arxiv.org/abs/2003.03123
 
-    This is equivalent to SphericalBesselFunction class with max_l=1, i.e. only l=0 bessel fucntions), but with
+    This is equivalent to SphericalBesselFunction class with max_l=1, i.e. only l=0 bessel functions), but with
     optional learnable frequencies.
     """
 
     def __init__(self, max_n: int, cutoff: float, learnable: bool = False):
         """
         Args:
             max_n: int, max number of roots (including max_n)
@@ -305,19 +305,21 @@
         * (n + 2)
         / torch.sqrt(2 * n**2 + 6 * n + 5)
         * (_sinc(r * (n + 1) * pi / cutoff) + _sinc(r * (n + 2) * pi / cutoff))
     )
     en = n**2 * (n + 2) ** 2 / (4 * (n + 1) ** 4 + 1)
     dn = [torch.tensor(1.0)]
     for i in range(1, max_n):
-        dn.append(1 - en[0, i] / dn[-1])
+        dn_value = 1 - en[0, i] / dn[-1]
+        dn.append(dn_value)
     dn = torch.stack(dn)  # type: ignore
     gn = [fnr[:, 0]]
     for i in range(1, max_n):
-        gn.append(1 / torch.sqrt(dn[i]) * (fnr[:, i] + torch.sqrt(en[0, i] / dn[i - 1]) * gn[-1]))
+        gn_value = 1 / torch.sqrt(dn[i]) * (fnr[:, i] + torch.sqrt(en[0, i] / dn[i - 1]) * gn[-1])
+        gn.append(gn_value)
 
     return torch.t(torch.stack(gn))
 
 
 def _sinc(x):
     return torch.sin(x) / x
```

### Comparing `matgl-0.7.0/matgl/layers/_bond.py` & `matgl-0.7.1/matgl/layers/_bond.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/layers/_core.py` & `matgl-0.7.1/matgl/layers/_core.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/layers/_embedding.py` & `matgl-0.7.1/matgl/layers/_embedding.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/layers/_graph_convolution.py` & `matgl-0.7.1/matgl/layers/_graph_convolution.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/layers/_readout.py` & `matgl-0.7.1/matgl/layers/_readout.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/layers/_three_body.py` & `matgl-0.7.1/matgl/layers/_three_body.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/models/_m3gnet.py` & `matgl-0.7.1/matgl/models/_m3gnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 """
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
 import dgl
-import numpy as np
 import torch
 from torch import nn
 
 from matgl.config import DEFAULT_ELEMENT_TYPES
 from matgl.graph.compute import (
     compute_pair_vector_and_distance,
     compute_theta_and_phi,
@@ -54,15 +53,15 @@
 
     def __init__(
         self,
         element_types: tuple[str],
         dim_node_embedding: int = 64,
         dim_edge_embedding: int = 64,
         dim_state_embedding: int | None = None,
-        dim_state_types: int | None = None,
+        ntypes_state: int | None = None,
         dim_state_feats: int | None = None,
         max_n: int = 3,
         max_l: int = 3,
         nblocks: int = 3,
         rbf_type="SphericalBessel",
         is_intensive: bool = True,
         readout_type: str = "weighted_atom",
@@ -83,15 +82,15 @@
         """
         Args:
             element_types (tuple): list of elements appearing in the dataset
             dim_node_embedding (int): number of embedded atomic features
             dim_edge_embedding (int): number of edge features
             dim_state_embedding (int): number of hidden neurons in state embedding
             dim_state_feats (int): number of state features after linear layer
-            dim_state_types (int): number of state labels
+            ntypes_state (int): number of state labels
             max_n (int): number of radial basis expansion
             max_l (int): number of angular expansion
             nblocks (int): number of convolution blocks
             rbf_type (str): radial basis function. choose from 'Gaussian' or 'SphericalBessel'
             is_intensive (bool): whether the prediction is intensive
             readout_type (str): the readout function type. choose from `set2set`,
             `weighted_atom` and `reduce_atom`, default to `weighted_atom`
@@ -139,14 +138,15 @@
         degree_rbf = max_n if use_smooth else max_n * max_l
 
         self.embedding = EmbeddingBlock(
             degree_rbf=degree_rbf,
             dim_node_embedding=dim_node_embedding,
             dim_edge_embedding=dim_edge_embedding,
             ntypes_node=len(element_types),
+            ntypes_state=ntypes_state,
             dim_state_feats=dim_state_feats,
             include_state=include_state,
             dim_state_embedding=dim_state_embedding,
             activation=activation,
         )
 
         self.basis_expansion = SphericalBesselWithHarmonics(
@@ -166,14 +166,17 @@
                     ),
                     update_network_bond=GatedMLP(in_feats=degree, dims=[dim_edge_embedding], use_bias=False),
                 )
                 for _ in range(nblocks)
             }
         )
 
+        if dim_state_feats is None:
+            dim_state_feats = dim_state_embedding
+
         self.graph_layers = nn.ModuleList(
             {
                 M3GNetBlock(
                     degree=degree_rbf,
                     activation=activation,
                     conv_hiddens=[units, units],
                     num_node_feats=dim_node_embedding,
@@ -229,48 +232,52 @@
             l_g : DGLGraph for a batch of line graphs.
 
         Returns:
             output: Output property for a batch of graphs
         """
         node_types = g.ndata["node_type"]
         bond_vec, bond_dist = compute_pair_vector_and_distance(g)
-        g.edata["bond_vec"] = bond_vec
-        g.edata["bond_dist"] = bond_dist
+        g.edata["bond_vec"] = bond_vec.to(g.device)
+        g.edata["bond_dist"] = bond_dist.to(g.device)
 
         expanded_dists = self.bond_expansion(g.edata["bond_dist"])
         if l_g is None:
             l_g = create_line_graph(g, self.threebody_cutoff)
         else:
-            three_body_id = np.unique(np.concatenate(l_g.edges()))
-            max_three_body_id = max(np.concatenate([three_body_id + 1, [0]]))
-            l_g.ndata["bond_vec"] = g.edata["bond_vec"][:max_three_body_id]
-            l_g.ndata["bond_dist"] = g.edata["bond_dist"][:max_three_body_id]
-            l_g.ndata["pbc_offset"] = g.edata["pbc_offset"][:max_three_body_id]
+            if l_g.num_nodes() == g.num_edges():
+                valid_three_body = g.edata["bond_dist"] <= self.threebody_cutoff
+                l_g.ndata["bond_vec"] = g.edata["bond_vec"][valid_three_body]
+                l_g.ndata["bond_dist"] = g.edata["bond_dist"][valid_three_body]
+                l_g.ndata["pbc_offset"] = g.edata["pbc_offset"][valid_three_body]
+            else:
+                three_body_id = torch.unique(torch.concatenate(l_g.edges()))
+                max_three_body_id = max(torch.cat([three_body_id + 1, torch.tensor([0])]))
+                l_g.ndata["bond_vec"] = g.edata["bond_vec"][:max_three_body_id]
+                l_g.ndata["bond_dist"] = g.edata["bond_dist"][:max_three_body_id]
+                l_g.ndata["pbc_offset"] = g.edata["pbc_offset"][:max_three_body_id]
         l_g.apply_edges(compute_theta_and_phi)
         g.edata["rbf"] = expanded_dists
         three_body_basis = self.basis_expansion(l_g)
         three_body_cutoff = polynomial_cutoff(g.edata["bond_dist"], self.threebody_cutoff)
-        num_node_feats, num_edge_feats, num_state_feats = self.embedding(node_types, g.edata["rbf"], state_attr)
+        node_feat, edge_feat, state_feat = self.embedding(node_types, g.edata["rbf"], state_attr)
         for i in range(self.n_blocks):
-            num_edge_feats = self.three_body_interactions[i](
+            edge_feat = self.three_body_interactions[i](
                 g,
                 l_g,
                 three_body_basis,
                 three_body_cutoff,
-                num_node_feats,
-                num_edge_feats,
-            )
-            num_edge_feats, num_node_feats, num_state_feats = self.graph_layers[i](
-                g, num_edge_feats, num_node_feats, num_state_feats
+                node_feat,
+                edge_feat,
             )
-        g.ndata["node_feat"] = num_node_feats
-        g.edata["edge_feat"] = num_edge_feats
+            edge_feat, node_feat, state_feat = self.graph_layers[i](g, edge_feat, node_feat, state_feat)
+        g.ndata["node_feat"] = node_feat
+        g.edata["edge_feat"] = edge_feat
         if self.is_intensive:
             node_vec = self.readout(g)
-            vec = torch.hstack([node_vec, state_attr]) if self.include_states else node_vec  # type: ignore
+            vec = torch.hstack([node_vec, state_feat]) if self.include_states else node_vec  # type: ignore
             output = self.final_layer(vec)
             if self.task_type == "classification":
                 output = self.sigmoid(output)
         else:
             g.ndata["atomic_properties"] = self.final_layer(g)
             output = dgl.readout_nodes(g, "atomic_properties", op="sum")
         return torch.squeeze(output)
```

### Comparing `matgl-0.7.0/matgl/models/_megnet.py` & `matgl-0.7.1/matgl/models/_megnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,18 +129,19 @@
         block_args = {
             "conv_hiddens": hidden_layer_sizes_conv,
             "dropout": dropout,
             "act": activation,
             "skip": True,
         }
         # first block
-        blocks = [MEGNetBlock(dims=[dim_blocks_in], **block_args)]  # type: ignore
-        # other blocks
-        for _ in range(nblocks - 1):
-            blocks.append(MEGNetBlock(dims=[dim_blocks_out, *hidden_layer_sizes_input], **block_args))  # type: ignore
+        blocks = [MEGNetBlock(dims=[dim_blocks_in], **block_args)] + [  # type: ignore
+            MEGNetBlock(dims=[dim_blocks_out, *hidden_layer_sizes_input], **block_args)  # type: ignore
+            for _ in range(nblocks - 1)
+        ]
+
         self.blocks = nn.ModuleList(blocks)
 
         s2s_kwargs = {"n_iters": niters_set2set, "n_layers": nlayers_set2set}
         self.edge_s2s = EdgeSet2Set(dim_blocks_out, **s2s_kwargs)
         self.node_s2s = Set2Set(dim_blocks_out, **s2s_kwargs)
 
         self.output_proj = MLP(
@@ -194,15 +195,15 @@
         if self.dropout:
             vec = self.dropout(vec)  # pylint: disable=E1102
 
         output = self.output_proj(vec)
         if self.is_classification:
             output = torch.sigmoid(output)
 
-        return output
+        return torch.squeeze(output)
 
     def predict_structure(
         self,
         structure,
         state_feats: torch.Tensor | None = None,
         graph_converter: GraphConverter | None = None,
     ):
```

### Comparing `matgl-0.7.0/matgl/models/_wrappers.py` & `matgl-0.7.1/matgl/models/_wrappers.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/utils/cutoff.py` & `matgl-0.7.1/matgl/utils/cutoff.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/utils/io.py` & `matgl-0.7.1/matgl/utils/io.py`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/utils/maths.py` & `matgl-0.7.1/matgl/utils/maths.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Implementations of math functions."""
 
 from __future__ import annotations
 
 import os
 from functools import lru_cache
-from math import pi
+from math import pi, sqrt
 
 import numpy as np
 import sympy
 import torch
 from scipy.optimize import brentq
 from scipy.special import spherical_jn
 
@@ -52,48 +52,46 @@
     indices = []
     start = 0
 
     for i, b in enumerate(block_size):
         indices.append(torch.tile(col_index[start : start + b], [repeats[i]]))
         start += b
     indices = torch.cat(indices, axis=0)
-    return torch.index_select(array, 1, indices)
+    return torch.index_select(array, 1, indices.to(array.device))
 
 
 @lru_cache(maxsize=128)
 def _get_lambda_func(max_n, cutoff: float = 5.0):
     r = sympy.symbols("r")
-    d0 = 1.0
-    en = []
-    for i in range(max_n):
-        en.append(i**2 * (i + 2) ** 2 / (4 * (i + 1) ** 4 + 1))
+    en = [i**2 * (i + 2) ** 2 / (4 * (i + 1) ** 4 + 1) for i in range(max_n)]
 
-    dn = [d0]
+    dn = [1.0]
     for i in range(1, max_n):
-        dn.append(1 - en[i] / dn[-1])
+        dn_value = 1 - en[i] / dn[-1]
+        dn.append(dn_value)
 
-    fnr = []
-    for i in range(max_n):
-        fnr.append(
-            (-1) ** i
-            * sympy.sqrt(2.0)
-            * sympy.pi
-            / cutoff**1.5
-            * (i + 1)
-            * (i + 2)
-            / sympy.sqrt(1.0 * (i + 1) ** 2 + (i + 2) ** 2)
-            * (
-                sympy.sin(r * (i + 1) * sympy.pi / cutoff) / (r * (i + 1) * sympy.pi / cutoff)
-                + sympy.sin(r * (i + 2) * sympy.pi / cutoff) / (r * (i + 2) * sympy.pi / cutoff)
-            )
+    fnr = [
+        (-1) ** i
+        * sqrt(2.0)
+        * pi
+        / cutoff**1.5
+        * (i + 1)
+        * (i + 2)
+        / sympy.sqrt(1.0 * (i + 1) ** 2 + (i + 2) ** 2)
+        * (
+            sympy.sin(r * (i + 1) * pi / cutoff) / (r * (i + 1) * pi / cutoff)
+            + sympy.sin(r * (i + 2) * pi / cutoff) / (r * (i + 2) * pi / cutoff)
         )
+        for i in range(max_n)
+    ]
 
     gnr = [fnr[0]]
     for i in range(1, max_n):
-        gnr.append(1 / sympy.sqrt(dn[i]) * (fnr[i] + sympy.sqrt(en[i] / dn[i - 1]) * gnr[-1]))
+        gnr_value = 1 / sympy.sqrt(dn[i]) * (fnr[i] + sympy.sqrt(en[i] / dn[i - 1]) * gnr[-1])
+        gnr.append(gnr_value)
     return [sympy.lambdify([r], sympy.simplify(i), torch) for i in gnr]
 
 
 def get_segment_indices_from_n(ns):
     """Get segment indices from number array. For example if
     ns = [2, 3], then the function will return [0, 0, 1, 1, 1].
 
@@ -101,16 +99,17 @@
         ns: torch.Tensor, the number of atoms/bonds array
 
     Returns:
         object:
 
     Returns: segment indices tensor
     """
-    a = torch.arange(ns.size(dim=0))
-    return a.repeat_interleave(ns, dim=0)
+    B = ns
+    A = torch.arange(B.size(dim=0)).to(B.device)
+    return A.repeat_interleave(B, dim=0)
 
 
 def get_range_indices_from_n(ns):
     """Give ns = [2, 3], return [0, 1, 0, 1, 2].
 
     Args:
         ns: torch.Tensor, the number of atoms/bonds array
@@ -184,15 +183,15 @@
     """
     segment_ids = broadcast(segment_ids, input_tensor, dim)
     size = list(input_tensor.size())
     if segment_ids.numel() == 0:
         size[dim] = 0
     else:
         size[dim] = num_segments
-    output = torch.zeros(size, dtype=input_tensor.dtype)
+    output = torch.zeros(size, dtype=input_tensor.dtype, device=input_tensor.device)
     return output.scatter_add_(dim, segment_ids, input_tensor)
 
 
 def unsorted_segment_fraction(data: torch.Tensor, segment_ids: torch.Tensor, num_segments: int):
     """Segment fraction
     Args:
         data (torch.tensor): original data
```

### Comparing `matgl-0.7.0/matgl/utils/sb_roots.npy` & `matgl-0.7.1/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/matgl/utils/training.py` & `matgl-0.7.1/matgl/utils/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,16 +208,20 @@
     def step(self, batch: tuple):
         """Args:
             batch: Batch of training data.
 
         Returns:
             results, batch_size
         """
-        g, labels, state_attr = batch
-        preds = self(g=g, state_attr=state_attr)
+        if isinstance(self.model, M3GNet):
+            g, l_g, state_attr, labels = batch
+            preds = self(g=g, l_g=l_g, state_attr=state_attr)
+        else:
+            g, labels, state_attr = batch
+            preds = self(g=g, state_attr=state_attr)
         results = self.loss_fn(loss=self.loss, preds=preds, labels=labels)  # type: ignore
         batch_size = preds.numel()
         return results, batch_size
 
     def loss_fn(self, loss: nn.Module, labels: torch.Tensor, preds: torch.Tensor):
         """Args:
             loss: Loss function.
@@ -277,30 +281,31 @@
             lr: learning rate for training
             decay_steps: number of steps for decaying learning rate
             decay_alpha: parameter determines the minimum learning rate.
             **kwargs: Passthrough to parent init.
         """
         super().__init__(**kwargs)
 
-        self.model = Potential(model=model, element_refs=element_refs, calc_stresses=calc_stress)
-
         self.mae = torchmetrics.MeanAbsoluteError()
         self.rmse = torchmetrics.MeanSquaredError(squared=False)
         if data_mean is None:
             data_mean = torch.zeros(1)
         if data_std is None:
             data_std = torch.ones(1)
         self.data_mean = data_mean
         self.data_std = data_std
         self.energy_weight = energy_weight
         self.force_weight = force_weight
         self.stress_weight = stress_weight
         self.lr = lr
         self.decay_steps = decay_steps
         self.decay_alpha = decay_alpha
+        self.model = Potential(
+            model=model, element_refs=element_refs, calc_stresses=calc_stress, data_std=data_std, data_mean=data_mean
+        )
         if loss == "mse_loss":
             self.loss = F.mse_loss
         else:
             self.loss = F.l1_loss
         self.optimizer = optimizer
         self.scheduler = scheduler
         self.save_hyperparameters()
```

### Comparing `matgl-0.7.0/matgl.egg-info/PKG-INFO` & `matgl-0.7.1/matgl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.7.0
+Version: 0.7.1
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `matgl-0.7.0/matgl.egg-info/SOURCES.txt` & `matgl-0.7.1/matgl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matgl-0.7.0/pyproject.toml` & `matgl-0.7.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [build-system]
 requires = [
   # pin NumPy version used in the build
   "oldest-supported-numpy",
   "setuptools>=58.0.3",
 ]
 build-backend = "setuptools.build_meta"
-numpy = "1.24.2"
 
 [tool.black]
 line-length = 120
 target-version = ['py39']
 include = '\.pyi?$'
 exclude = '''
 (
@@ -74,14 +73,15 @@
 ]
 pydocstyle.convention = "google"
 isort.required-imports = ["from __future__ import annotations"]
 extend-exclude = ["tests"]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
+"maths.py" = ["PERF"]
 "setup.py" = ["D"]
 "tasks.py" = ["D"]
 "tests/**/*" = ["D"]
 "docs/**/*" = ["D"]
 "examples/**/*" = ["D"]
 
 [tool.pytest.ini_options]
```

### Comparing `matgl-0.7.0/setup.py` & `matgl-0.7.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from __future__ import annotations
 
 import os
 
-import numpy as np
 from setuptools import find_packages, setup
 
 this_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(this_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="matgl",
-    version="0.7.0",
+    version="0.7.1",
     author="Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong",
     author_email="t1ko@ucsd.edu, ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
     maintainer_email="ongsp@ucsd.edu",
     description="MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -53,14 +52,13 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Chemistry",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Scientific/Engineering :: Physics",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    include_dirs=[np.get_include()],
     entry_points={
         "console_scripts": [
             "mgl = matgl.cli:main",
         ]
     },
 )
```

