# Comparing `tmp/pybiopax-0.1.3.tar.gz` & `tmp/pybiopax-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybiopax-0.1.3.tar", last modified: Thu Feb  9 04:20:18 2023, max compression
+gzip compressed data, was "pybiopax-0.1.4.tar", last modified: Tue Jul 11 21:29:06 2023, max compression
```

## Comparing `pybiopax-0.1.3.tar` & `pybiopax-0.1.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-02-09 04:20:18.210564 pybiopax-0.1.3/
--rw-r--r--   0 ben        (503) staff       (20)     1346 2022-03-06 12:43:07.000000 pybiopax-0.1.3/LICENSE
--rw-r--r--   0 ben        (503) staff       (20)      160 2023-02-09 04:17:55.000000 pybiopax-0.1.3/MANIFEST.in
--rw-r--r--   0 ben        (503) staff       (20)     4634 2023-02-09 04:20:18.210425 pybiopax-0.1.3/PKG-INFO
--rw-r--r--   0 ben        (503) staff       (20)     3972 2022-09-06 22:49:47.000000 pybiopax-0.1.3/README.md
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-02-09 04:20:18.204625 pybiopax-0.1.3/doc/
--rw-r--r--   0 ben        (503) staff       (20)      634 2022-03-06 12:43:07.000000 pybiopax-0.1.3/doc/Makefile
--rw-r--r--   0 ben        (503) staff       (20)     2377 2022-09-06 22:49:47.000000 pybiopax-0.1.3/doc/conf.py
--rw-r--r--   0 ben        (503) staff       (20)      447 2022-09-06 22:49:47.000000 pybiopax-0.1.3/doc/index.rst
--rw-r--r--   0 ben        (503) staff       (20)      795 2022-03-06 12:43:07.000000 pybiopax-0.1.3/doc/make.bat
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-02-09 04:20:18.205328 pybiopax-0.1.3/doc/modules/
--rw-r--r--   0 ben        (503) staff       (20)       93 2022-03-06 12:43:07.000000 pybiopax-0.1.3/doc/modules/api.rst
--rw-r--r--   0 ben        (503) staff       (20)      772 2022-09-06 22:49:47.000000 pybiopax-0.1.3/doc/modules/biopax.rst
--rw-r--r--   0 ben        (503) staff       (20)       95 2022-03-06 12:43:07.000000 pybiopax-0.1.3/doc/modules/paths.rst
--rw-r--r--   0 ben        (503) staff       (20)      119 2022-03-06 12:43:07.000000 pybiopax-0.1.3/doc/modules/pc_client.rst
--rw-r--r--   0 ben        (503) staff       (20)      130 2022-03-06 12:43:07.000000 pybiopax-0.1.3/doc/modules/xml_util.rst
--rw-r--r--   0 ben        (503) staff       (20)       82 2022-03-06 12:43:07.000000 pybiopax-0.1.3/doc/requirements.txt
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-02-09 04:20:18.206274 pybiopax-0.1.3/pybiopax/
--rw-r--r--   0 ben        (503) staff       (20)       42 2023-02-09 04:19:28.000000 pybiopax-0.1.3/pybiopax/__init__.py
--rw-r--r--   0 ben        (503) staff       (20)    10040 2023-02-09 04:17:55.000000 pybiopax-0.1.3/pybiopax/api.py
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-02-09 04:20:18.207789 pybiopax-0.1.3/pybiopax/biopax/
--rw-r--r--   0 ben        (503) staff       (20)      281 2023-02-09 04:17:55.000000 pybiopax-0.1.3/pybiopax/biopax/__init__.py
--rw-r--r--   0 ben        (503) staff       (20)     7537 2022-09-06 22:49:47.000000 pybiopax-0.1.3/pybiopax/biopax/base.py
--rw-r--r--   0 ben        (503) staff       (20)     5544 2022-09-06 22:49:47.000000 pybiopax-0.1.3/pybiopax/biopax/interaction.py
--rw-r--r--   0 ben        (503) staff       (20)     5492 2023-02-09 04:17:55.000000 pybiopax-0.1.3/pybiopax/biopax/model.py
--rw-r--r--   0 ben        (503) staff       (20)     3166 2022-09-06 22:49:47.000000 pybiopax-0.1.3/pybiopax/biopax/physical_entity.py
--rw-r--r--   0 ben        (503) staff       (20)    18108 2022-09-06 22:49:47.000000 pybiopax-0.1.3/pybiopax/biopax/util.py
--rw-r--r--   0 ben        (503) staff       (20)     3363 2022-03-06 12:43:07.000000 pybiopax-0.1.3/pybiopax/paths.py
--rw-r--r--   0 ben        (503) staff       (20)     3017 2022-03-06 12:43:07.000000 pybiopax-0.1.3/pybiopax/pc_client.py
--rw-r--r--   0 ben        (503) staff       (20)        0 2023-02-09 04:17:55.000000 pybiopax-0.1.3/pybiopax/py.typed
--rw-r--r--   0 ben        (503) staff       (20)     1409 2022-09-06 22:49:47.000000 pybiopax-0.1.3/pybiopax/references.py
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-02-09 04:20:18.210231 pybiopax-0.1.3/pybiopax/tests/
--rw-r--r--   0 ben        (503) staff       (20)        0 2022-03-06 12:43:07.000000 pybiopax-0.1.3/pybiopax/tests/__init__.py
--rw-r--r--   0 ben        (503) staff       (20)  3623423 2022-03-06 12:43:07.000000 pybiopax-0.1.3/pybiopax/tests/biopax_test.owl.gz
--rw-r--r--   0 ben        (503) staff       (20)     3244 2022-09-06 22:49:47.000000 pybiopax-0.1.3/pybiopax/tests/test_biopax.py
--rw-r--r--   0 ben        (503) staff       (20)     2718 2022-03-06 12:43:07.000000 pybiopax-0.1.3/pybiopax/tests/test_paths.py
--rw-r--r--   0 ben        (503) staff       (20)      470 2023-02-09 04:17:55.000000 pybiopax-0.1.3/pybiopax/tests/test_serialization.py
--rw-r--r--   0 ben        (503) staff       (20)     3995 2022-03-06 12:43:07.000000 pybiopax-0.1.3/pybiopax/xml_util.py
-drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-02-09 04:20:18.206973 pybiopax-0.1.3/pybiopax.egg-info/
--rw-r--r--   0 ben        (503) staff       (20)     4634 2023-02-09 04:20:18.000000 pybiopax-0.1.3/pybiopax.egg-info/PKG-INFO
--rw-r--r--   0 ben        (503) staff       (20)      864 2023-02-09 04:20:18.000000 pybiopax-0.1.3/pybiopax.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (503) staff       (20)        1 2023-02-09 04:20:18.000000 pybiopax-0.1.3/pybiopax.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (503) staff       (20)       19 2023-02-09 04:20:18.000000 pybiopax-0.1.3/pybiopax.egg-info/requires.txt
--rw-r--r--   0 ben        (503) staff       (20)        9 2023-02-09 04:20:18.000000 pybiopax-0.1.3/pybiopax.egg-info/top_level.txt
--rw-r--r--   0 ben        (503) staff       (20)      189 2022-03-06 12:43:07.000000 pybiopax-0.1.3/pyproject.toml
--rw-r--r--   0 ben        (503) staff       (20)       38 2023-02-09 04:20:18.210609 pybiopax-0.1.3/setup.cfg
--rw-r--r--   0 ben        (503) staff       (20)     1474 2022-03-06 12:43:07.000000 pybiopax-0.1.3/setup.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-07-11 21:29:06.977102 pybiopax-0.1.4/
+-rw-r--r--   0 ben        (503) staff       (20)     1346 2022-03-06 12:43:07.000000 pybiopax-0.1.4/LICENSE
+-rw-r--r--   0 ben        (503) staff       (20)      160 2023-02-09 04:17:55.000000 pybiopax-0.1.4/MANIFEST.in
+-rw-r--r--   0 ben        (503) staff       (20)     4634 2023-07-11 21:29:06.976962 pybiopax-0.1.4/PKG-INFO
+-rw-r--r--   0 ben        (503) staff       (20)     3972 2022-09-06 22:49:47.000000 pybiopax-0.1.4/README.md
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-07-11 21:29:06.962265 pybiopax-0.1.4/doc/
+-rw-r--r--   0 ben        (503) staff       (20)      634 2022-03-06 12:43:07.000000 pybiopax-0.1.4/doc/Makefile
+-rw-r--r--   0 ben        (503) staff       (20)     2377 2022-09-06 22:49:47.000000 pybiopax-0.1.4/doc/conf.py
+-rw-r--r--   0 ben        (503) staff       (20)      447 2022-09-06 22:49:47.000000 pybiopax-0.1.4/doc/index.rst
+-rw-r--r--   0 ben        (503) staff       (20)      795 2022-03-06 12:43:07.000000 pybiopax-0.1.4/doc/make.bat
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-07-11 21:29:06.963179 pybiopax-0.1.4/doc/modules/
+-rw-r--r--   0 ben        (503) staff       (20)       93 2022-03-06 12:43:07.000000 pybiopax-0.1.4/doc/modules/api.rst
+-rw-r--r--   0 ben        (503) staff       (20)      772 2022-09-06 22:49:47.000000 pybiopax-0.1.4/doc/modules/biopax.rst
+-rw-r--r--   0 ben        (503) staff       (20)       95 2022-03-06 12:43:07.000000 pybiopax-0.1.4/doc/modules/paths.rst
+-rw-r--r--   0 ben        (503) staff       (20)      119 2022-03-06 12:43:07.000000 pybiopax-0.1.4/doc/modules/pc_client.rst
+-rw-r--r--   0 ben        (503) staff       (20)      130 2022-03-06 12:43:07.000000 pybiopax-0.1.4/doc/modules/xml_util.rst
+-rw-r--r--   0 ben        (503) staff       (20)       82 2022-03-06 12:43:07.000000 pybiopax-0.1.4/doc/requirements.txt
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-07-11 21:29:06.964500 pybiopax-0.1.4/pybiopax/
+-rw-r--r--   0 ben        (503) staff       (20)       42 2023-07-11 21:28:45.000000 pybiopax-0.1.4/pybiopax/__init__.py
+-rw-r--r--   0 ben        (503) staff       (20)    10040 2023-02-09 04:17:55.000000 pybiopax-0.1.4/pybiopax/api.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-07-11 21:29:06.966373 pybiopax-0.1.4/pybiopax/biopax/
+-rw-r--r--   0 ben        (503) staff       (20)      281 2023-02-09 04:17:55.000000 pybiopax-0.1.4/pybiopax/biopax/__init__.py
+-rw-r--r--   0 ben        (503) staff       (20)     7579 2023-07-11 21:28:45.000000 pybiopax-0.1.4/pybiopax/biopax/base.py
+-rw-r--r--   0 ben        (503) staff       (20)     5544 2022-09-06 22:49:47.000000 pybiopax-0.1.4/pybiopax/biopax/interaction.py
+-rw-r--r--   0 ben        (503) staff       (20)     5492 2023-02-09 04:17:55.000000 pybiopax-0.1.4/pybiopax/biopax/model.py
+-rw-r--r--   0 ben        (503) staff       (20)     3166 2022-09-06 22:49:47.000000 pybiopax-0.1.4/pybiopax/biopax/physical_entity.py
+-rw-r--r--   0 ben        (503) staff       (20)    18908 2023-07-11 21:28:45.000000 pybiopax-0.1.4/pybiopax/biopax/util.py
+-rw-r--r--   0 ben        (503) staff       (20)     3363 2022-03-06 12:43:07.000000 pybiopax-0.1.4/pybiopax/paths.py
+-rw-r--r--   0 ben        (503) staff       (20)     3017 2022-03-06 12:43:07.000000 pybiopax-0.1.4/pybiopax/pc_client.py
+-rw-r--r--   0 ben        (503) staff       (20)        0 2023-02-09 04:17:55.000000 pybiopax-0.1.4/pybiopax/py.typed
+-rw-r--r--   0 ben        (503) staff       (20)     1409 2022-09-06 22:49:47.000000 pybiopax-0.1.4/pybiopax/references.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-07-11 21:29:06.976665 pybiopax-0.1.4/pybiopax/tests/
+-rw-r--r--   0 ben        (503) staff       (20)        0 2022-03-06 12:43:07.000000 pybiopax-0.1.4/pybiopax/tests/__init__.py
+-rw-r--r--   0 ben        (503) staff       (20)  3623423 2022-03-06 12:43:07.000000 pybiopax-0.1.4/pybiopax/tests/biopax_test.owl.gz
+-rw-r--r--   0 ben        (503) staff       (20)     3244 2022-09-06 22:49:47.000000 pybiopax-0.1.4/pybiopax/tests/test_biopax.py
+-rw-r--r--   0 ben        (503) staff       (20)     2718 2022-03-06 12:43:07.000000 pybiopax-0.1.4/pybiopax/tests/test_paths.py
+-rw-r--r--   0 ben        (503) staff       (20)      470 2023-02-09 04:17:55.000000 pybiopax-0.1.4/pybiopax/tests/test_serialization.py
+-rw-r--r--   0 ben        (503) staff       (20)     3995 2022-03-06 12:43:07.000000 pybiopax-0.1.4/pybiopax/xml_util.py
+drwxr-xr-x   0 ben        (503) staff       (20)        0 2023-07-11 21:29:06.965168 pybiopax-0.1.4/pybiopax.egg-info/
+-rw-r--r--   0 ben        (503) staff       (20)     4634 2023-07-11 21:29:06.000000 pybiopax-0.1.4/pybiopax.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (503) staff       (20)      864 2023-07-11 21:29:06.000000 pybiopax-0.1.4/pybiopax.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (503) staff       (20)        1 2023-07-11 21:29:06.000000 pybiopax-0.1.4/pybiopax.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (503) staff       (20)       19 2023-07-11 21:29:06.000000 pybiopax-0.1.4/pybiopax.egg-info/requires.txt
+-rw-r--r--   0 ben        (503) staff       (20)        9 2023-07-11 21:29:06.000000 pybiopax-0.1.4/pybiopax.egg-info/top_level.txt
+-rw-r--r--   0 ben        (503) staff       (20)      189 2022-03-06 12:43:07.000000 pybiopax-0.1.4/pyproject.toml
+-rw-r--r--   0 ben        (503) staff       (20)       38 2023-07-11 21:29:06.977136 pybiopax-0.1.4/setup.cfg
+-rw-r--r--   0 ben        (503) staff       (20)     1474 2022-03-06 12:43:07.000000 pybiopax-0.1.4/setup.py
```

### Comparing `pybiopax-0.1.3/LICENSE` & `pybiopax-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/PKG-INFO` & `pybiopax-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybiopax
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python implementation of the BioPAX object model, and parts of PaxTools.
 Home-page: https://github.com/indralab/pybiopax
 Author: Benjamin M. Gyori, Harvard Medical School
 Author-email: benjamin_gyori@hms.harvard.edu
 Keywords: biology,pathway
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pybiopax-0.1.3/README.md` & `pybiopax-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/doc/Makefile` & `pybiopax-0.1.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/doc/conf.py` & `pybiopax-0.1.4/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/doc/make.bat` & `pybiopax-0.1.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/doc/modules/biopax.rst` & `pybiopax-0.1.4/doc/modules/biopax.rst`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/pybiopax/api.py` & `pybiopax-0.1.4/pybiopax/api.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/pybiopax/biopax/base.py` & `pybiopax-0.1.4/pybiopax/biopax/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -215,24 +215,24 @@
     @property
     def controller_of(self):
         return self._controller_of
 
 
 class Pathway(Entity, Controller):
     """BioPAX Pathway."""
-    list_types = Entity.list_types + ['pathway_component']
+    list_types = Entity.list_types + ['pathway_component', 'pathway_order']
 
     def __init__(self,
                  pathway_component=None,
                  pathway_order=None,
                  organism=None,
                  **kwargs):
         super().__init__(**kwargs)
         self.pathway_component = pathway_component if pathway_component else []
-        self.pathway_order = pathway_order
+        self.pathway_order = pathway_order if pathway_order else []
         self.organism = organism
 
 
 # These are necessary to have the objects in the global
 # scope, required for some modes of deserialization
 from .interaction import *
 from .physical_entity import *
```

### Comparing `pybiopax-0.1.3/pybiopax/biopax/interaction.py` & `pybiopax-0.1.4/pybiopax/biopax/interaction.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/pybiopax/biopax/model.py` & `pybiopax-0.1.4/pybiopax/biopax/model.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/pybiopax/biopax/physical_entity.py` & `pybiopax-0.1.4/pybiopax/biopax/physical_entity.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/pybiopax/biopax/util.py` & `pybiopax-0.1.4/pybiopax/biopax/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -335,23 +335,23 @@
     """BioPAX PathwayStep.
 
     Attributes
     ----------
     step_process : List[Process]
     next_step : List[Process]
     """
-    list_types = UtilityClass.list_types + Observable.list_types
+    list_types = UtilityClass.list_types + Observable.list_types + ['step_process', 'next_step']
 
     def __init__(self,
                  step_process=None,
                  next_step=None,
                  **kwargs):
         super().__init__(**kwargs)
-        self.step_process = step_process
-        self.next_step = next_step
+        self.step_process = step_process  if step_process else []
+        self.next_step = next_step  if next_step else []
         self._next_step_of = set()
         self._pathway_order_of = set()
 
     @property
     def next_step_of(self):
         return self._next_step_of
 
@@ -525,27 +525,51 @@
                  **kwargs):
         super().__init__(**kwargs)
         self.organism = organism
         self.sequence = sequence
 
 
 class NucleicAcidReference(SequenceEntityReference):
-    """BioPAX NucleicAcidReference"""
-    pass
+    """BioPAX NucleicAcidReference
+
+    Attributes
+    ----------
+    sub_region : List[NucleicAcidRegionReference]
+    """
+    list_types = SequenceEntityReference.list_types + ['sub_region']
+
+    def __init__(self,
+                 sub_region=None,
+                 **kwargs):
+        super().__init__(**kwargs)
+        self.sub_region = sub_region if sub_region else []
 
 
 class NucleicAcidRegionReference(NucleicAcidReference):
-    """BioPAX NucleicAcidRegionReference"""
-    def __init__(self, **kwargs):
+    """BioPAX NucleicAcidRegionReference
+
+    Attributes
+    ----------
+    absolute_region : SequenceLocation
+    region_type : List[SequenceRegionVocabulary]
+    """
+    list_types = NucleicAcidReference.list_types + ['region_type']
+
+    def __init__(self,
+                 absolute_region=None,
+                 region_type=None,
+                 **kwargs):
         super().__init__(**kwargs)
-        self._subregion_of = set()
+        self.absolute_region = absolute_region
+        self.region_type = region_type if region_type else []
+        self._sub_region_of = set()
 
     @property
-    def subregion_of(self):
-        return self._subregion_of
+    def sub_region_of(self):
+        return self._sub_region_of
 
 
 class RnaReference(NucleicAcidReference):
     """BioPAX RnaReference."""
     pass
```

### Comparing `pybiopax-0.1.3/pybiopax/paths.py` & `pybiopax-0.1.4/pybiopax/paths.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/pybiopax/pc_client.py` & `pybiopax-0.1.4/pybiopax/pc_client.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/pybiopax/references.py` & `pybiopax-0.1.4/pybiopax/references.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/pybiopax/tests/biopax_test.owl.gz` & `pybiopax-0.1.4/pybiopax/tests/biopax_test.owl.gz`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/pybiopax/tests/test_biopax.py` & `pybiopax-0.1.4/pybiopax/tests/test_biopax.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/pybiopax/tests/test_paths.py` & `pybiopax-0.1.4/pybiopax/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/pybiopax/xml_util.py` & `pybiopax-0.1.4/pybiopax/xml_util.py`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/pybiopax.egg-info/PKG-INFO` & `pybiopax-0.1.4/pybiopax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybiopax
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python implementation of the BioPAX object model, and parts of PaxTools.
 Home-page: https://github.com/indralab/pybiopax
 Author: Benjamin M. Gyori, Harvard Medical School
 Author-email: benjamin_gyori@hms.harvard.edu
 Keywords: biology,pathway
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pybiopax-0.1.3/pybiopax.egg-info/SOURCES.txt` & `pybiopax-0.1.4/pybiopax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybiopax-0.1.3/setup.py` & `pybiopax-0.1.4/setup.py`

 * *Files identical despite different names*

