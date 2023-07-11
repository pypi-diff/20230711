# Comparing `tmp/polycleaver-0.0.2.tar.gz` & `tmp/polycleaver-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polycleaver-0.0.2.tar", last modified: Mon Jul 10 20:15:36 2023, max compression
+gzip compressed data, was "polycleaver-0.0.3.tar", last modified: Tue Jul 11 14:32:32 2023, max compression
```

## Comparing `polycleaver-0.0.2.tar` & `polycleaver-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-10 20:15:36.499253 polycleaver-0.0.2/
--rw-r--r--   0 eric       (501) staff       (20)    35149 2023-06-13 15:55:31.000000 polycleaver-0.0.2/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)      607 2023-07-10 20:15:36.498981 polycleaver-0.0.2/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     3614 2023-06-13 15:55:31.000000 polycleaver-0.0.2/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-10 20:15:36.494564 polycleaver-0.0.2/polycleaver/
--rw-r--r--   0 eric       (501) staff       (20)        0 2023-06-13 15:55:31.000000 polycleaver-0.0.2/polycleaver/__init__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-10 20:15:36.496229 polycleaver-0.0.2/polycleaver/core/
--rw-r--r--   0 eric       (501) staff       (20)        0 2023-06-13 15:55:31.000000 polycleaver-0.0.2/polycleaver/core/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      269 2023-06-13 15:55:31.000000 polycleaver-0.0.2/polycleaver/core/miscellaneous.py
--rw-r--r--   0 eric       (501) staff       (20)    18667 2023-07-10 15:50:14.000000 polycleaver-0.0.2/polycleaver/core/mnx.py
--rw-r--r--   0 eric       (501) staff       (20)     1853 2023-06-14 14:18:51.000000 polycleaver-0.0.2/polycleaver/core/mx.py
--rw-r--r--   0 eric       (501) staff       (20)     5294 2023-06-19 10:50:28.000000 polycleaver-0.0.2/polycleaver/core/tools.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-10 20:15:36.495180 polycleaver-0.0.2/polycleaver.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)      607 2023-07-10 20:15:36.000000 polycleaver-0.0.2/polycleaver.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      360 2023-07-10 20:15:36.000000 polycleaver-0.0.2/polycleaver.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-07-10 20:15:36.000000 polycleaver-0.0.2/polycleaver.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)        9 2023-07-10 20:15:36.000000 polycleaver-0.0.2/polycleaver.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       12 2023-07-10 20:15:36.000000 polycleaver-0.0.2/polycleaver.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-07-10 20:15:36.499338 polycleaver-0.0.2/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)      962 2023-07-10 20:15:24.000000 polycleaver-0.0.2/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-11 14:32:32.305164 polycleaver-0.0.3/
+-rw-r--r--   0 eric       (501) staff       (20)    35149 2023-06-13 15:55:31.000000 polycleaver-0.0.3/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)      607 2023-07-11 14:32:32.305004 polycleaver-0.0.3/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     3614 2023-06-13 15:55:31.000000 polycleaver-0.0.3/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-11 14:32:32.303009 polycleaver-0.0.3/polycleaver/
+-rw-r--r--   0 eric       (501) staff       (20)        0 2023-06-13 15:55:31.000000 polycleaver-0.0.3/polycleaver/__init__.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-11 14:32:32.304677 polycleaver-0.0.3/polycleaver/core/
+-rw-r--r--   0 eric       (501) staff       (20)        0 2023-06-13 15:55:31.000000 polycleaver-0.0.3/polycleaver/core/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      269 2023-06-13 15:55:31.000000 polycleaver-0.0.3/polycleaver/core/miscellaneous.py
+-rw-r--r--   0 eric       (501) staff       (20)    18560 2023-07-11 14:29:33.000000 polycleaver-0.0.3/polycleaver/core/mnx.py
+-rw-r--r--   0 eric       (501) staff       (20)     1853 2023-06-14 14:18:51.000000 polycleaver-0.0.3/polycleaver/core/mx.py
+-rw-r--r--   0 eric       (501) staff       (20)     5294 2023-06-19 10:50:28.000000 polycleaver-0.0.3/polycleaver/core/tools.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-11 14:32:32.303617 polycleaver-0.0.3/polycleaver.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)      607 2023-07-11 14:32:32.000000 polycleaver-0.0.3/polycleaver.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)      360 2023-07-11 14:32:32.000000 polycleaver-0.0.3/polycleaver.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-07-11 14:32:32.000000 polycleaver-0.0.3/polycleaver.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)        9 2023-07-11 14:32:32.000000 polycleaver-0.0.3/polycleaver.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       12 2023-07-11 14:32:32.000000 polycleaver-0.0.3/polycleaver.egg-info/top_level.txt
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-07-11 14:32:32.305209 polycleaver-0.0.3/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)      962 2023-07-11 14:32:24.000000 polycleaver-0.0.3/setup.py
```

### Comparing `polycleaver-0.0.2/LICENSE` & `polycleaver-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polycleaver-0.0.2/PKG-INFO` & `polycleaver-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polycleaver
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for the generation of non-polar and stoichiometric surfaces from ionic structures.
 Author: Eric Mates-Torres
 Author-email: <eric.mates@uab.cat>
 Keywords: python,slab,surface,miller,ionic,mineral
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `polycleaver-0.0.2/README.md` & `polycleaver-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `polycleaver-0.0.2/polycleaver/core/mnx.py` & `polycleaver-0.0.3/polycleaver/core/mnx.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,36 +368,35 @@
     bulk = tools.read_bulk(bulk_str)
     bulk.add_oxidation_state_by_guess()
     bulk_obj = BulkUnit(bulk)
     initial_slabs = tools.get_initial_slabs(bulk, hkl, thickness, vacuum)
 
     final_slabs = []
     for index, slab in enumerate(initial_slabs):
-        if index > 16:
-            load_bar(index, len(initial_slabs))
-            initial_slab = slab.get_orthogonal_c_slab()
-            scaffold = SlabUnit(initial_slab.copy(), bulk_obj)
-            while len(np.append(scaffold.clusters_to_remove, scaffold.lone_anions)):
-                scaffold.remove_sites(np.append(scaffold.clusters_to_remove, np.array(scaffold.lone_anions, dtype=object)))
-                if center_str not in scaffold.atoms.formula:
-                    continue
-            scaffold.remove_element(cations_strs)
-            topbot = scaffold.depolarize_anions()
-            reconstruction = SlabUnit(initial_slab.copy(), bulk_obj)
-            reconstruction.remove_sites([site for site in reconstruction.atoms
-                                            if site not in scaffold.atoms
-                                            and site.element not in cations_strs])
-            reconstruction.depolarize_cations(topbot)
-            reconstruction.stoichiometrize()
-            tools.set_site_attributes(reconstruction.atoms)
-            if (not reconstruction.atoms.is_polar(tol_dipole_per_unit_area=0.01) and
-                reconstruction.there_are_cations() and
-                reconstruction.undercoordinated_sites(reconstruction.centers).size == 0):
-                final_slabs.append(reconstruction)
-            sys.stdout.flush()
+        load_bar(index, len(initial_slabs))
+        initial_slab = slab.get_orthogonal_c_slab()
+        scaffold = SlabUnit(initial_slab.copy(), bulk_obj)
+        while len(np.append(scaffold.clusters_to_remove, scaffold.lone_anions)):
+            scaffold.remove_sites(np.append(scaffold.clusters_to_remove, np.array(scaffold.lone_anions, dtype=object)))
+            if center_str not in scaffold.atoms.formula:
+                continue
+        scaffold.remove_element(cations_strs)
+        topbot = scaffold.depolarize_anions()
+        reconstruction = SlabUnit(initial_slab.copy(), bulk_obj)
+        reconstruction.remove_sites([site for site in reconstruction.atoms
+                                        if site not in scaffold.atoms
+                                        and site.element not in cations_strs])
+        reconstruction.depolarize_cations(topbot)
+        reconstruction.stoichiometrize()
+        tools.set_site_attributes(reconstruction.atoms)
+        if (not reconstruction.atoms.is_polar(tol_dipole_per_unit_area=0.01) and
+            reconstruction.there_are_cations() and
+            reconstruction.undercoordinated_sites(reconstruction.centers).size == 0):
+            final_slabs.append(reconstruction)
+        sys.stdout.flush()
 
     print('\nRemoving equivalent slabs...')
     tools.remove_equivalent_slabs(final_slabs)
 
     print(f'{len(final_slabs)} non-polar, stoichiometric slabs generated.')
 
     if save:
```

### Comparing `polycleaver-0.0.2/polycleaver/core/mx.py` & `polycleaver-0.0.3/polycleaver/core/mx.py`

 * *Files identical despite different names*

### Comparing `polycleaver-0.0.2/polycleaver/core/tools.py` & `polycleaver-0.0.3/polycleaver/core/tools.py`

 * *Files identical despite different names*

### Comparing `polycleaver-0.0.2/polycleaver.egg-info/PKG-INFO` & `polycleaver-0.0.3/polycleaver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polycleaver
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for the generation of non-polar and stoichiometric surfaces from ionic structures.
 Author: Eric Mates-Torres
 Author-email: <eric.mates@uab.cat>
 Keywords: python,slab,surface,miller,ionic,mineral
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `polycleaver-0.0.2/setup.py` & `polycleaver-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Package for the generation of non-polar and stoichiometric surfaces from ionic structures.'
 LONG_DESCRIPTION = 'Package for the generation of non-polar and stoichiometric surfaces from ionic structures.'
 
 # Setting up
 setup(
     name="polycleaver",
     version=VERSION,
```

