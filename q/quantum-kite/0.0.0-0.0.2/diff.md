# Comparing `tmp/quantum-kite-0.0.0.tar.gz` & `tmp/quantum-kite-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantum-kite-0.0.0.tar", last modified: Sun Jul  2 09:38:21 2023, max compression
+gzip compressed data, was "quantum-kite-0.0.2.tar", last modified: Tue Jul 11 16:44:34 2023, max compression
```

## Comparing `quantum-kite-0.0.0.tar` & `quantum-kite-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:38:21.631488 quantum-kite-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-02 09:38:21.631488 quantum-kite-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:38:21.627488 quantum-kite-0.0.0/kite/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/kite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/kite/calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)    49077 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/kite/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/kite/disorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/kite/execute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:38:21.627488 quantum-kite-0.0.0/kite/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/kite/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/kite/modification.py
--rw-r--r--   0 runner    (1001) docker     (123)    42946 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/kite/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:38:21.631488 quantum-kite-0.0.0/kite/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/kite/tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3121 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/kite/tools/process_arpes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4421 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/kite/tools/process_new.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1309 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/kite/tools/process_single_shot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:38:21.631488 quantum-kite-0.0.0/kite/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/kite/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/kite/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/kite/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:38:21.631488 quantum-kite-0.0.0/quantum_kite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-02 09:38:21.000000 quantum-kite-0.0.0/quantum_kite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-02 09:38:21.000000 quantum-kite-0.0.0/quantum_kite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:38:21.000000 quantum-kite-0.0.0/quantum_kite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-02 09:38:21.000000 quantum-kite-0.0.0/quantum_kite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 09:38:21.000000 quantum-kite-0.0.0/quantum_kite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 09:38:21.631488 quantum-kite-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:38:21.631488 quantum-kite-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-02 09:37:56.000000 quantum-kite-0.0.0/tests/test_dos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:44:34.668230 quantum-kite-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-07-11 16:44:34.668230 quantum-kite-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:44:34.668230 quantum-kite-0.0.2/kite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/kite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/kite/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49077 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/kite/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/kite/disorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/kite/execute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:44:34.668230 quantum-kite-0.0.2/kite/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/kite/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/kite/modification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43120 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/kite/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:44:34.668230 quantum-kite-0.0.2/kite/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/kite/tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3121 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/kite/tools/process_arpes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4421 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/kite/tools/process_new.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1309 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/kite/tools/process_single_shot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:44:34.668230 quantum-kite-0.0.2/kite/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/kite/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/kite/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/kite/utils/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:44:34.668230 quantum-kite-0.0.2/quantum_kite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-07-11 16:44:34.000000 quantum-kite-0.0.2/quantum_kite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-11 16:44:34.000000 quantum-kite-0.0.2/quantum_kite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:44:34.000000 quantum-kite-0.0.2/quantum_kite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-11 16:44:34.000000 quantum-kite-0.0.2/quantum_kite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 16:44:34.000000 quantum-kite-0.0.2/quantum_kite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 16:44:34.668230 quantum-kite-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:44:34.668230 quantum-kite-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/tests/local.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-11 16:44:06.000000 quantum-kite-0.0.2/tests/test_dos.py
```

### Comparing `quantum-kite-0.0.0/LICENSE.md` & `quantum-kite-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quantum-kite-0.0.0/PKG-INFO` & `quantum-kite-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: quantum-kite
-Version: 0.0.0
+Version: 0.0.2
 Summary: KITE: Real-space quantum transport simulator. (c) 2018-2023, Quantum-Kite team
-Author: Simão M. João, João M.V.P Lopes, Tatiana G. Rappoport, Misa Andelkovic, Lucian Covaci, Aires Ferreira, João P.S. Pires, Bert Jorissen, Emile Aerts, Robin Smeyers, David T.S. Perkins
+Author: Simão M. João, João M.V.P Lopes, Tatiana G. Rappoport, Misa Andelkovic, Lucian Covaci, Aires Ferreira, João P.S. Pires, Bert Jorissen, Emile Aerts, Robin Smeyers
+Maintainer-email: Bert Jorissen <info@bertjorissen.be>
 License: 
                            GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -177,22 +178,20 @@
 Keywords: pybinding,tight-binding,solid-state physics,physics,cmt,quantum,transport,graphene,TMD,KPM,CPGF
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 <img src=https://user-images.githubusercontent.com/39924384/41094707-9e4ead6e-6a25-11e8-9e16-070a3236c8da.png width="100">
 
 **KITE** is an open-source Python/C++ software suite for efficient real-space tight-binding (TB) simulations of electronic structure and bulk quantum transport properties of disordered systems scalable to multi billions of atomic orbitals.
```

### Comparing `quantum-kite-0.0.0/README.md` & `quantum-kite-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `quantum-kite-0.0.0/kite/__init__.py` & `quantum-kite-0.0.2/kite/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum-kite-0.0.0/kite/calculation.py` & `quantum-kite-0.0.2/kite/calculation.py`

 * *Files identical despite different names*

### Comparing `quantum-kite-0.0.0/kite/configuration.py` & `quantum-kite-0.0.2/kite/configuration.py`

 * *Files identical despite different names*

### Comparing `quantum-kite-0.0.0/kite/disorder.py` & `quantum-kite-0.0.2/kite/disorder.py`

 * *Files identical despite different names*

### Comparing `quantum-kite-0.0.0/kite/execute.py` & `quantum-kite-0.0.2/kite/execute.py`

 * *Files identical despite different names*

### Comparing `quantum-kite-0.0.0/kite/modification.py` & `quantum-kite-0.0.2/kite/modification.py`

 * *Files identical despite different names*

### Comparing `quantum-kite-0.0.0/kite/system.py` & `quantum-kite-0.0.2/kite/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """Functions to create a HDF5 file"""
 
 import numpy as np
 import h5py as hp
 import pybinding as pb
+import pybinding
 from scipy.sparse import coo_matrix
+
+import kite
+from typing import Optional
 from .modification import Modification
 from .utils.model import estimate_bounds
 __all__ = ['config_system']
 
 
-def config_system(lattice, config, calculation, modification=None, **kwargs):
+def config_system(lattice: pybinding.Lattice, config: kite.Configuration, calculation: kite.Calculation,
+                  modification: Optional[kite.Modification] = None, **kwargs):
     """Export the lattice and related parameters to the *.h5 file
 
     Parameters
     ----------
-    lattice : pb.Lattice
-        Pybinding lattice object that carries the info about the unit cell vectors, unit cell cites, hopping terms and
-        onsite energies.
-    config : Configuration
+    lattice
+        pb.Lattice: Pybinding lattice object that carries the info about the unit cell vectors, unit cell cites, hopping terms and
+        onsite energies. :class:`pybinding.Lattice`
+    config
         Configuration object, basic parameters defining size, precision, energy scale and number of decomposition parts
         in the calculation.
     calculation : Calculation
         Calculation object that defines the requested functions for the calculation.
     modification : Modification = None
         If specified modification object, has the magnetic field selection, either in terms of field, or in the number
         of flux quantum through the selected system.
```

### Comparing `quantum-kite-0.0.0/kite/tools/process_arpes.py` & `quantum-kite-0.0.2/kite/tools/process_arpes.py`

 * *Files identical despite different names*

### Comparing `quantum-kite-0.0.0/kite/tools/process_new.py` & `quantum-kite-0.0.2/kite/tools/process_new.py`

 * *Files identical despite different names*

### Comparing `quantum-kite-0.0.0/kite/tools/process_single_shot.py` & `quantum-kite-0.0.2/kite/tools/process_single_shot.py`

 * *Files identical despite different names*

### Comparing `quantum-kite-0.0.0/kite/utils/model.py` & `quantum-kite-0.0.2/kite/utils/model.py`

 * *Files identical despite different names*

### Comparing `quantum-kite-0.0.0/pyproject.toml` & `quantum-kite-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 [project]
 name = "quantum-kite"
-version = "0.0.0"
+version = "0.0.2"
 authors = [
     {name="Simão M. João"},
     {name="João M.V.P Lopes"},
     {name="Tatiana G. Rappoport"},
     {name="Misa Andelkovic"},
     {name="Lucian Covaci"},
     {name="Aires Ferreira"},
     {name="João P.S. Pires"},
     {name="Bert Jorissen"},
     {name="Emile Aerts"},
-    {name="Robin Smeyers"},
-    {name="David T.S. Perkins"}
+    {name="Robin Smeyers"}
+]
+maintainers = [
+    { name="Bert Jorissen", email="info@bertjorissen.be"}
 ]
 description = "KITE: Real-space quantum transport simulator. (c) 2018-2023, Quantum-Kite team"
 readme = "README.md"
 dependencies = [
     "numpy>=1.12",
     "scipy>=0.19",
-    "matplotlib>=2.0",
+    "matplotlib>=3.5",
     "h5py==3.8.0",
     "pytest>=5.0",
     "pybinding>=0.9.5"
 ]
-requires-python = ">=3.6"
+requires-python = ">=3.8"
 license = {file = "LICENSE.md"}
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Science/Research',
     'Topic :: Scientific/Engineering :: Physics',
     'License :: OSI Approved :: BSD License',
     'Programming Language :: C++',
     'Programming Language :: Python :: 3 :: Only',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: Implementation :: CPython',
 ]
 keywords = [
```

### Comparing `quantum-kite-0.0.0/quantum_kite.egg-info/PKG-INFO` & `quantum-kite-0.0.2/quantum_kite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: quantum-kite
-Version: 0.0.0
+Version: 0.0.2
 Summary: KITE: Real-space quantum transport simulator. (c) 2018-2023, Quantum-Kite team
-Author: Simão M. João, João M.V.P Lopes, Tatiana G. Rappoport, Misa Andelkovic, Lucian Covaci, Aires Ferreira, João P.S. Pires, Bert Jorissen, Emile Aerts, Robin Smeyers, David T.S. Perkins
+Author: Simão M. João, João M.V.P Lopes, Tatiana G. Rappoport, Misa Andelkovic, Lucian Covaci, Aires Ferreira, João P.S. Pires, Bert Jorissen, Emile Aerts, Robin Smeyers
+Maintainer-email: Bert Jorissen <info@bertjorissen.be>
 License: 
                            GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -177,22 +178,20 @@
 Keywords: pybinding,tight-binding,solid-state physics,physics,cmt,quantum,transport,graphene,TMD,KPM,CPGF
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 <img src=https://user-images.githubusercontent.com/39924384/41094707-9e4ead6e-6a25-11e8-9e16-070a3236c8da.png width="100">
 
 **KITE** is an open-source Python/C++ software suite for efficient real-space tight-binding (TB) simulations of electronic structure and bulk quantum transport properties of disordered systems scalable to multi billions of atomic orbitals.
```

### Comparing `quantum-kite-0.0.0/quantum_kite.egg-info/SOURCES.txt` & `quantum-kite-0.0.2/quantum_kite.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.md
 README.md
 pyproject.toml
+setup.cfg
 setup.py
 kite/__init__.py
 kite/calculation.py
 kite/configuration.py
 kite/disorder.py
 kite/execute.py
 kite/modification.py
@@ -19,8 +20,9 @@
 kite/utils/warnings.py
 quantum_kite.egg-info/PKG-INFO
 quantum_kite.egg-info/SOURCES.txt
 quantum_kite.egg-info/dependency_links.txt
 quantum_kite.egg-info/requires.txt
 quantum_kite.egg-info/top_level.txt
 tests/__init__.py
+tests/local.cfg
 tests/test_dos.py
```

### Comparing `quantum-kite-0.0.0/setup.py` & `quantum-kite-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,53 +21,59 @@
         for ext in self.extensions:
             self.build_extension(ext)
 
     def build_extension(self, ext):
         extdir = os.path.abspath(os.path.dirname(self.get_ext_fullpath(ext.name)))
         if not extdir.endswith(os.path.sep):
             extdir += os.path.sep
-        cmake_args = ["-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=" + extdir + "kite/lib",
+        cmake_args = ["-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=" + extdir + "kite" + os.path.sep + "lib",
                       "-DPYTHON_EXECUTABLE=" + sys.executable]
-        cmake_args += ["-DQK_NATIVE_HDF5=" + os.environ.get("QK_NATIVE_HDF5", "OFF"),
-                       "-DQK_NATIVE_EIGEN=" + os.environ.get("QK_NATIVE_EIGEN", "OFF")]
 
-        cfg = "Release" #os.environ.get("KITE_BUILD_TYPE", "Release")
+        cmake_args += ["-DQK_NATIVE_HDF5=" + os.environ.get("QK_NATIVE_HDF5", "OFF"),
+                       "-DQK_NATIVE_EIGEN=" + os.environ.get("QK_NATIVE_EIGEN", "OFF"),
+                       "-DQK_CCACHE=" + os.environ.get("QK_CCACHE", "OFF"),
+                       "-DQK_CMAKE_PREFIX_PATH=" + os.environ.get("QK_CMAKE_PREFIX_PATH", "")]
+        try:
+            import h5py
+            cmake_args += ["-DHDF5_DOWNLOAD_VERSION=" + os.environ.get("HDF5_DOWNLOAD_VERSION", h5py.version.hdf5_version)]
+        except ImportError:
+            cmake_args += []
+        cfg = os.environ.get("QK_BUILD_TYPE", "Release")
         build_args = ["--config", cfg]
 
         if platform.system() == "Windows":
             cmake_args += ["-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_{}={}".format(cfg.upper(), extdir + "kite/lib")]
             cmake_args += ["-A", "x64" if sys.maxsize > 2**32 else "Win32"]
             build_args += ["--", "/v:m", "/m"]
         else:
             cmake_args += ["-DCMAKE_BUILD_TYPE=" + cfg]
             if "-j" not in os.environ.get("MAKEFLAGS", ""):
-                parallel_jobs = 2 if not os.environ.get("READTHEDOCS") else int(os.cpu_count() - 1)
+                parallel_jobs = int(os.cpu_count() - 1) if not os.environ.get("READTHEDOCS") else 1
                 build_args += ["--", "-j{}".format(parallel_jobs)]
 
         env = os.environ.copy()
         env["CXXFLAGS"] = '{} -DCPB_VERSION=\\"{}\\"'.format(env.get("CXXFLAGS", ""),
                                                              self.distribution.get_version())
 
         def build():
             os.makedirs(self.build_temp, exist_ok=True)
             check_call(["cmake", ext.sourcedir] + cmake_args, cwd=self.build_temp, env=env)
-            check_call(["cmake", "--build", "."] + build_args, cwd=self.build_temp)
+            check_call(["cmake", "--build", ".", "--target", "kitecore"] + build_args, cwd=self.build_temp)
 
         try:
             build()
         except CalledProcessError:  # possible CMake error if the build cache has been copied
             shutil.rmtree(self.build_temp)  # delete build cache and try again
             build()
 
 
-# manifest_maker.template = "MANIFEST.in"
 setup(
     packages=find_packages(exclude=['cppcore', 'cppmodule', 'test*']) + ['kite.tests', 'kite.lib'],
     package_dir={'kite.tests': 'tests', 'kite.lib': 'kite/lib'},
     include_package_data=True,
     ext_modules=[CMakeExtension('kitecore')],
-    package_data={'kite.lib': [
-        'libhdf5.so', 'libhdf5_cpp.so', 'libhdf5.so.200',
-        'libhdf5_cpp.so.200', 'libhdf5.so.200.2.0', 'libhdf5_cpp.so.200.2.0'
-    ]},
+    package_data={
+        'kite.lib': ['*'],
+        'kite.tests': ["*"]
+    },
     cmdclass=dict(build_ext=CMakeBuild)
 )
```

### Comparing `quantum-kite-0.0.0/tests/test_dos.py` & `quantum-kite-0.0.2/tests/test_dos.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Test the DOS calculation of KITE"""
 import numpy as np
 import pybinding as pb
 import kite
-import os
 import pathlib
+import os
+import sys
+from contextlib import contextmanager
+os.environ["SEED"] = "3"
 
 
-def square(a: float=1., t: float=1.) -> pb.Lattice:
+def square(a: float = 1., t: float = 1.) -> pb.Lattice:
     """Make a square lattice to test the DOS.
 
     Parameters
     ----------
     a : float
         The unit vector length of the square lattice [nm].
     t : float
@@ -28,31 +31,25 @@
     lat.add_hoppings(
         ([0, 1], 'A', 'A', t),
         ([1, 0], 'A', 'A', t)
     )
     return lat
 
 
-from contextlib import contextmanager
-import os
-import sys
-
-
 @contextmanager
 def block_output():
     with open(os.devnull, 'w') as output:
         init_output = os.dup(sys.stdout.fileno())
         os.dup2(output.fileno(), sys.stdout.fileno())
         try:
             yield
         finally:
             os.dup2(init_output, sys.stdout.fileno())
 
 
-os.environ["SEED"] = "3"
 def test_square(tmp_path: pathlib.Path):
     """Do the tests for the square lattice."""
     if isinstance(tmp_path, str):
         file = tmp_path
     else:
         file = str((tmp_path / "config").with_suffix(".h5"))
     # construct the lattice
@@ -74,20 +71,62 @@
     calculation.dos(
         num_points=1000,
         num_moments=m,
         num_random=1,
         num_disorder=1)
 
     # make the input file
-
     if os.path.exists(file):
         os.remove(file)
     kite.config_system(lattice, configuration, calculation, filename=file)
-    # do the calculation, with the right random values
-    # os.system("./cmake-build-debug/cppcore/kitex/KITEx {0}".format(file))
     kite.execute.kitex(file)
     # check the contents for the file
     from tests.kitex.compare import compare
     hdf5_internal_dest = "/Calculation/dos/MU"
     ref_file = "tests/kitex/large000_KITEx_sq_dos/configREF.h5"
     assert compare([file, hdf5_internal_dest, ref_file, hdf5_internal_dest])[0] < 1e-8,\
         "The desired accuracy wasn't achieved."
+
+
+def test_magnetic(tmp_path: pathlib.Path):
+    """Do the tests for the square lattice."""
+    if isinstance(tmp_path, str):
+        file = tmp_path
+    else:
+        file = str((tmp_path / "config").with_suffix(".h5"))
+    # construct the lattice
+    lattice = square()
+
+    # set the parameters for the calculation with KITEx
+    nx = ny = 2
+    lx = ly = 512
+    m = 4192
+    configuration = kite.Configuration(
+        divisions=[nx, ny],
+        length=[lx, ly],
+        boundaries=["periodic", "periodic"],
+        is_complex=True,
+        precision=1,
+        spectrum_range=[-4.1, 4.1]
+    )
+    calculation = kite.Calculation(configuration)
+    mod = kite.Modification(magnetic_field=9)
+    calculation.dos(
+        num_points=4096,
+        num_moments=m,
+        num_random=1,
+        num_disorder=1)
+
+    # make the input file
+    if os.path.exists(file):
+        os.remove(file)
+    kite.config_system(lattice, configuration, calculation,  modification=mod, filename=file)
+    kite.execute.kitex(file)
+    # check the contents for the file
+    from tests.kitex.compare import compare, compare_txt
+    hdf5_internal_dest = "/Calculation/dos/MU"
+    ref_file = "tests/kitex/large001_magdos2d/configREF.h5"
+    assert compare([file, hdf5_internal_dest, ref_file, hdf5_internal_dest], set_abs=True)[0] < 1e-8, \
+        "The desired accuracy wasn't achieved."
+    kite.execute.kitetools(file)
+    file3, file4 = "tests/kitex/large001_magdos2d/dos.dat", "tests/kitex/large001_magdos2d/dosREF.dat"
+    assert compare_txt([file3, file4], set_abs=True)[0] < 1e-8, "The desired accuracy wasn't achieved, {0}".format(compare_txt([file3, file4], set_abs=True)[0])
```

