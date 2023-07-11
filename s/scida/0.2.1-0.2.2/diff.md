# Comparing `tmp/scida-0.2.1.tar.gz` & `tmp/scida-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scida-0.2.1.tar", max compression
+gzip compressed data, was "scida-0.2.2.tar", max compression
```

## Comparing `scida-0.2.1.tar` & `scida-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,47 @@
--rw-r--r--   0        0        0     1069 2023-06-29 21:39:54.909294 scida-0.2.1/LICENSE
--rw-r--r--   0        0        0     1473 2023-06-29 21:39:54.909294 scida-0.2.1/README.md
--rw-r--r--   0        0        0     1546 2023-06-29 21:39:54.917294 scida-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      391 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/__init__.py
--rw-r--r--   0        0        0     5752 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/config.py
--rw-r--r--   0        0        0        0 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/__init__.py
--rw-r--r--   0        0        0      953 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/config.yaml
--rw-r--r--   0        0        0     3198 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/simulations.yaml
--rw-r--r--   0        0        0        0 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/units/__init__.py
--rw-r--r--   0        0        0     3144 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/units/eagle.yaml
--rw-r--r--   0        0        0      662 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/units/gaia.yaml
--rw-r--r--   0        0        0       30 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/units/general.yaml
--rw-r--r--   0        0        0     1319 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/units/gizmo.yaml
--rw-r--r--   0        0        0     6118 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/configfiles/units/illustris.yaml
--rw-r--r--   0        0        0    11409 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/convenience.py
--rw-r--r--   0        0        0        0 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/customs/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/customs/arepo/__init__.py
--rw-r--r--   0        0        0    35081 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/customs/arepo/dataset.py
--rw-r--r--   0        0        0     2204 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/customs/arepo/series.py
--rw-r--r--   0        0        0      480 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/customs/gizmo/series.py
--rw-r--r--   0        0        0     1366 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/customs/rockstar/dataset.py
--rw-r--r--   0        0        0     3628 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/discovertypes.py
--rw-r--r--   0        0        0    12114 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/fields.py
--rw-r--r--   0        0        0     9055 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/helpers_hdf5.py
--rw-r--r--   0        0        0     2356 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/helpers_misc.py
--rw-r--r--   0        0        0    12540 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/interface.py
--rw-r--r--   0        0        0     5803 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/interfaces/gadgetstyle.py
--rw-r--r--   0        0        0      307 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/interfaces/mixins/__init__.py
--rw-r--r--   0        0        0       22 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/interfaces/mixins/base.py
--rw-r--r--   0        0        0     2419 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/interfaces/mixins/cosmology.py
--rw-r--r--   0        0        0     2360 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/interfaces/mixins/spatial.py
--rw-r--r--   0        0        0    15238 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/interfaces/mixins/units.py
--rw-r--r--   0        0        0    13618 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/io.py
--rw-r--r--   0        0        0     6144 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/misc.py
--rw-r--r--   0        0        0      221 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/registries.py
--rw-r--r--   0        0        0     9772 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/series.py
--rw-r--r--   0        0        0      314 2023-06-29 21:39:54.917294 scida-0.2.1/src/scida/utilities.py
--rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 scida-0.2.1/setup.py
--rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 scida-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-11 10:43:08.191682 scida-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1473 2023-07-11 10:43:08.191682 scida-0.2.2/README.md
+-rw-r--r--   0        0        0     1546 2023-07-11 10:43:08.203683 scida-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      712 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/__init__.py
+-rw-r--r--   0        0        0     5752 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/config.py
+-rw-r--r--   0        0        0        0 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/configfiles/__init__.py
+-rw-r--r--   0        0        0      953 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/configfiles/config.yaml
+-rw-r--r--   0        0        0     3274 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/configfiles/simulations.yaml
+-rw-r--r--   0        0        0        0 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/configfiles/units/__init__.py
+-rw-r--r--   0        0        0     3144 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/configfiles/units/eagle.yaml
+-rw-r--r--   0        0        0      662 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/configfiles/units/gaia.yaml
+-rw-r--r--   0        0        0       30 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/configfiles/units/general.yaml
+-rw-r--r--   0        0        0     1327 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/configfiles/units/gizmo.yaml
+-rw-r--r--   0        0        0     6120 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/configfiles/units/illustris.yaml
+-rw-r--r--   0        0        0     1970 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/configfiles/units/rockstar.yaml
+-rw-r--r--   0        0        0    10794 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/convenience.py
+-rw-r--r--   0        0        0        0 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/customs/__init__.py
+-rw-r--r--   0        0        0       31 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/customs/arepo/MTNG/__init__.py
+-rw-r--r--   0        0        0     3742 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/customs/arepo/MTNG/dataset.py
+-rw-r--r--   0        0        0      105 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/customs/arepo/TNGcluster/__init__.py
+-rw-r--r--   0        0        0     5167 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/customs/arepo/TNGcluster/dataset.py
+-rw-r--r--   0        0        0        0 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/customs/arepo/__init__.py
+-rw-r--r--   0        0        0    35544 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/customs/arepo/dataset.py
+-rw-r--r--   0        0        0     1336 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/customs/arepo/series.py
+-rw-r--r--   0        0        0        0 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/customs/gadgetstyle/__init__.py
+-rw-r--r--   0        0        0     6317 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/customs/gadgetstyle/dataset.py
+-rw-r--r--   0        0        0     2671 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/customs/gadgetstyle/series.py
+-rw-r--r--   0        0        0     2173 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/customs/gizmo/dataset.py
+-rw-r--r--   0        0        0     1222 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/customs/gizmo/series.py
+-rw-r--r--   0        0        0     1313 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/customs/rockstar/dataset.py
+-rw-r--r--   0        0        0     5420 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/discovertypes.py
+-rw-r--r--   0        0        0    12745 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/fields.py
+-rw-r--r--   0        0        0    10238 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/helpers_hdf5.py
+-rw-r--r--   0        0        0     3036 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/helpers_misc.py
+-rw-r--r--   0        0        0    12622 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/interface.py
+-rw-r--r--   0        0        0      307 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/interfaces/mixins/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/interfaces/mixins/base.py
+-rw-r--r--   0        0        0     2863 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/interfaces/mixins/cosmology.py
+-rw-r--r--   0        0        0     2360 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/interfaces/mixins/spatial.py
+-rw-r--r--   0        0        0    15373 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/interfaces/mixins/units.py
+-rw-r--r--   0        0        0    13955 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/io.py
+-rw-r--r--   0        0        0     6288 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/misc.py
+-rw-r--r--   0        0        0      221 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/registries.py
+-rw-r--r--   0        0        0     9772 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/series.py
+-rw-r--r--   0        0        0      314 2023-07-11 10:43:08.203683 scida-0.2.2/src/scida/utilities.py
+-rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 scida-0.2.2/setup.py
+-rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 scida-0.2.2/PKG-INFO
```

### Comparing `scida-0.2.1/LICENSE` & `scida-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scida-0.2.1/README.md` & `scida-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `scida-0.2.1/pyproject.toml` & `scida-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scida"
-version = "0.2.1"
+version = "0.2.2"
 description = "Convenience wrapper around large scientific datasets to process with dask."
 authors = ["Chris Byrohl"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.21"
```

### Comparing `scida-0.2.1/src/scida/config.py` & `scida-0.2.2/src/scida/config.py`

 * *Files identical despite different names*

### Comparing `scida-0.2.1/src/scida/configfiles/config.yaml` & `scida-0.2.2/src/scida/configfiles/config.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.2.1/src/scida/configfiles/simulations.yaml` & `scida-0.2.2/src/scida/configfiles/simulations.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -99,13 +99,15 @@
           RunLabel: "\"Eagle"
       unitfile: units/eagle.yaml
 
   gaia-dr3:
       identifiers:
         name_contains: "gaia"
 
-
   FIRE2:
     unitfile: units/gizmo.yaml
     identifiers:
       Header:
         ReadMe: "This snapshot is part of the Feedback in Realistic Environments (FIRE) project -- Use, modification, or distribution only permitted with approval of the PI and the FIRE team -- No warranty, use at your own risk -- compactify_hdf5 (c) RF 2018"
+    dataset_type:
+      series: GizmoSimulation
+      dataset: GizmoSnapshot
```

### Comparing `scida-0.2.1/src/scida/configfiles/units/eagle.yaml` & `scida-0.2.2/src/scida/configfiles/units/eagle.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.2.1/src/scida/configfiles/units/gaia.yaml` & `scida-0.2.2/src/scida/configfiles/units/gaia.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.2.1/src/scida/configfiles/units/gizmo.yaml` & `scida-0.2.2/src/scida/configfiles/units/gizmo.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   code_energy: (code_velocity)^2
   code_density: code_mass / code_length^3
   code_magnetic: gauss
   code_divdamp: code_magnetic * code_velocity
 fields:
   _all:
     Coordinates: code_length
-    Velocities: code_velocity
+    Velocities: a^0.5 * code_velocity
     ParticleIDs:
     ParticleChildIDsNumber:
     ParticleIDGenerationNumber:
     Masses: code_mass
     Potential: (km / s)^2  # TODO: not in GIZMO manual, taken from https://bitbucket.org/awetzel/gizmo_analysis/src/master/gizmo_io.py
   PartType0:
     InternalEnergy: code_energy
```

### Comparing `scida-0.2.1/src/scida/configfiles/units/illustris.yaml` & `scida-0.2.2/src/scida/configfiles/units/illustris.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
       override: true  # set this to override potential disagreeing units from metadata
     GFM_CoolingRate: erg * cm^3 / s
     GFM_Metallicity:
     GFM_Metals:
     GFM_MetalsTagged:
     GFM_WindDMVelDisp: km / s
     GFM_WindHostHaloMass: code_mass
-    InternalEnergy: (km / s)^2
+    InternalEnergy: (km / s) ^ 2
     InternalEnergyOld: (km / s)^2
     Machnumber:
     MagneticField: (h / a^2) * (code_pressure)^(1/2)
     MagneticFieldDivergence: (h^3 / a^2) * code_mass^(1/2) * (km/s) * (ckpc)^(-5/2)
     NeutralHydrogenAbundance:
     # TODO: Pressure?
     SmoothingLength: code_length
```

### Comparing `scida-0.2.1/src/scida/convenience.py` & `scida-0.2.2/src/scida/convenience.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 import sys
 import tarfile
 import time
 from typing import Optional, Union
 
 import requests
 
-from scida.config import get_config, get_simulationconfig
-from scida.discovertypes import _determine_mixins, _determine_type
-from scida.interface import Dataset
+from scida.config import get_config
+from scida.discovertypes import (
+    _determine_mixins,
+    _determine_type,
+    _determine_type_from_simconfig,
+)
 from scida.interfaces.mixins import UnitMixin
 from scida.io import load_metadata
-from scida.misc import check_config_for_dataset
 from scida.registries import dataseries_type_registry, dataset_type_registry
 from scida.series import DatasetSeries
 
 log = logging.getLogger(__name__)
 
 
 def download_and_extract(
@@ -218,67 +220,53 @@
 
     path = os.path.realpath(path)
     cls = _determine_type(path, **kwargs)[1][0]
 
     msg = "Dataset is identified as '%s' via _determine_type." % cls
     log.debug(msg)
 
+    # any identifying metadata?
+    classtype = "dataset"
+    if issubclass(cls, DatasetSeries):
+        classtype = "series"
+    cls_simconf = _determine_type_from_simconfig(path, classtype=classtype, reg=reg)
+
+    if cls_simconf and not issubclass(cls, cls_simconf):
+        oldcls = cls
+        cls = cls_simconf
+        if oldcls != cls:
+            msg = "Dataset is identified as '%s' via the simulation config replacing prior candidate '%s'."
+            log.debug(msg % (cls, oldcls))
+        else:
+            msg = "Dataset is identified as '%s' via the simulation config, identical to prior candidate."
+            log.debug(msg % cls)
+
+    if force_class is not None:
+        cls = force_class
+
     # determine additional mixins not set by class
     mixins = []
+    if hasattr(cls, "_unitfile"):
+        unitfile = cls._unitfile
     if unitfile:
         if not units:
             units = True
         kwargs["unitfile"] = unitfile
 
     if units:
         mixins.append(UnitMixin)
         kwargs["units"] = units
 
     kwargs["overwritecache"] = overwrite
 
-    # any identifying metadata?
+    # we append since unit mixin is added outside of this func right now
     metadata_raw = dict()
-    if issubclass(cls, Dataset):
+    if classtype == "dataset":
         metadata_raw = load_metadata(path, fileprefix=None)
-    candidates = check_config_for_dataset(metadata_raw, path=path)
-    assert len(candidates) <= 1
-    if len(candidates) == 1:
-        simconf = get_simulationconfig()
-        dstype = simconf.get("data", {}).get(candidates[0]).get("dataset_type", None)
-        oldcls = cls
-        if isinstance(dstype, dict):
-            # series or dataset based on past candidate
-            if issubclass(cls, DatasetSeries):
-                cls = reg[dstype["series"]]
-            elif issubclass(cls, Dataset):
-                cls = reg[dstype["dataset"]]
-            else:
-                raise ValueError("Unknown type of dataset '%s'." % cls.__name__)
-        elif isinstance(dstype, str):
-            cls = reg[dstype]
-        elif dstype is None:
-            pass  # simply no dataset_type specified
-        else:
-            raise ValueError(
-                "Unknown type of dataset config variable. content: '%s'" % dstype
-            )
-
-        msg = "Dataset is identified as '%s' via the simulation config replacing prior candidate '%s'."
-        if dstype is not None:
-            log.debug(msg % (dstype, oldcls))
-
-    if force_class is not None:
-        cls = force_class
-
-    p = path
-    if metadata_raw is not None:
-        p = None  # if we have metadata, do not pass path (unnecessary IO)
-
-    # we append since unit mixin is added outside of this func right now
-    other_mixins = _determine_mixins(path=p, metadata_raw=metadata_raw)
+    other_mixins = _determine_mixins(path=path, metadata_raw=metadata_raw)
     mixins += other_mixins
 
     log.debug("Adding mixins '%s' to dataset." % mixins)
     if hasattr(cls, "_mixins"):
         cls_mixins = cls._mixins
         for m in cls_mixins:
             # remove duplicates
```

### Comparing `scida-0.2.1/src/scida/customs/arepo/dataset.py` & `scida-0.2.2/src/scida/customs/arepo/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,33 @@
 import logging
 import os
 import warnings
 from typing import Dict, List, Optional, Union
 
 import dask
 import numpy as np
+import pint
 from dask import array as da
 from dask import delayed
 from numba import jit
 from numpy.typing import NDArray
 
-from scida.discovertypes import _determine_mixins
+from scida.customs.gadgetstyle.dataset import GadgetStyleSnapshot
+from scida.discovertypes import CandidateStatus, _determine_mixins
 from scida.fields import FieldContainer
-from scida.helpers_misc import computedecorator, get_args, get_kwargs, parse_humansize
+from scida.helpers_misc import (
+    computedecorator,
+    get_args,
+    get_kwargs,
+    map_blocks,
+    parse_humansize,
+)
 from scida.interface import Selector, create_MixinDataset
-from scida.interfaces.gadgetstyle import GadgetStyleSnapshot
 from scida.interfaces.mixins import SpatialCartesian3DMixin, UnitMixin
+from scida.io import load_metadata
 
 log = logging.getLogger(__name__)
 
 
 class ArepoSelector(Selector):
     def __init__(self) -> None:
         super().__init__()
@@ -67,71 +75,15 @@
         if not self.iscatalog:
             if self.catalog is None:
                 self.discover_catalog()
                 # try to discover group catalog in parent directories.
             if self.catalog == "none":
                 pass  # this string can be set to explicitly disable catalog
             elif self.catalog is not None:
-                virtualcache = False  # copy catalog for better performance
-                catalog_kwargs = kwargs.get("catalog_kwargs", {})
-                catalog_kwargs["overwritecache"] = kwargs.get("overwritecache", False)
-                # fileprefix = catalog_kwargs.get("fileprefix", self._fileprefix_catalog)
-                prfx = self._get_fileprefix(self.catalog)
-
-                # explicitly need to create unitaware class for catalog as needed
-                # TODO: should just be determined from mixins of parent?
-                cls = ArepoCatalog
-                withunits = kwargs.get("units", False)
-                mixins = []
-                if withunits:
-                    mixins += [UnitMixin]
-
-                other_mixins = _determine_mixins(path=path)
-                mixins += other_mixins
-                cls = create_MixinDataset(cls, mixins)
-
-                ureg = None
-                if hasattr(self, "ureg"):
-                    ureg = self.ureg
-
-                self.catalog = cls(
-                    self.catalog,
-                    virtualcache=virtualcache,
-                    fileprefix=prfx,
-                    units=self.withunits,
-                    ureg=ureg,
-                )
-                if "Redshift" in self.catalog.header and "Redshift" in self.header:
-                    z_catalog = self.catalog.header["Redshift"]
-                    z_snap = self.header["Redshift"]
-                    if not np.isclose(z_catalog, z_snap):
-                        raise ValueError(
-                            "Redshift mismatch between snapshot and catalog: "
-                            f"{z_snap:.2f} vs {z_catalog:.2f}"
-                        )
-                for k in self.catalog.data:
-                    if k not in self.data:
-                        self.data[k] = self.catalog.data[k]
-                    self.catalog.data.fieldrecipes_kwargs["snap"] = self
-                if (
-                    len(self.catalog.data["Group"].keys()) > 0
-                ):  # starting snapshots often dont have groups
-                    self.add_catalogIDs()
-
-                # merge hints from snap and catalog
-                for h in self.catalog.hints:
-                    if h not in self.hints:
-                        self.hints[h] = self.catalog.hints[h]
-                    elif isinstance(self.hints[h], dict):
-                        # merge dicts
-                        for k in self.catalog.hints[h]:
-                            if k not in self.hints[h]:
-                                self.hints[h][k] = self.catalog.hints[h][k]
-                    else:
-                        pass  # nothing to do; we do not overwrite with catalog props
+                self.load_catalog(kwargs)
 
         # add aliases
         aliases = dict(
             PartType0=["gas", "baryons"],
             PartType1=["dm", "dark matter"],
             PartType2=["lowres", "lowres dm"],
             PartType3=["tracer", "tracers"],
@@ -146,24 +98,92 @@
 
         # set metadata
         self._set_metadata()
 
         # add some default fields
         self.data.merge(fielddefs)
 
+    def load_catalog(self, kwargs):
+        virtualcache = False  # copy catalog for better performance
+        catalog_kwargs = kwargs.get("catalog_kwargs", {})
+        catalog_kwargs["overwritecache"] = kwargs.get("overwritecache", False)
+        # fileprefix = catalog_kwargs.get("fileprefix", self._fileprefix_catalog)
+        prfx = self._get_fileprefix(self.catalog)
+
+        # explicitly need to create unitaware class for catalog as needed
+        # TODO: should just be determined from mixins of parent?
+        cls = ArepoCatalog
+        withunits = kwargs.get("units", False)
+        mixins = []
+        if withunits:
+            mixins += [UnitMixin]
+
+        other_mixins = _determine_mixins(path=self.path)
+        mixins += other_mixins
+        cls = create_MixinDataset(cls, mixins)
+
+        ureg = None
+        if hasattr(self, "ureg"):
+            ureg = self.ureg
+
+        self.catalog = cls(
+            self.catalog,
+            virtualcache=virtualcache,
+            fileprefix=prfx,
+            units=self.withunits,
+            ureg=ureg,
+        )
+        if "Redshift" in self.catalog.header and "Redshift" in self.header:
+            z_catalog = self.catalog.header["Redshift"]
+            z_snap = self.header["Redshift"]
+            if not np.isclose(z_catalog, z_snap):
+                raise ValueError(
+                    "Redshift mismatch between snapshot and catalog: "
+                    f"{z_snap:.2f} vs {z_catalog:.2f}"
+                )
+
+        # merge data
+        self.merge_data(self.catalog)
+
+        # first snapshots often do not have groups
+        if "Group" in self.catalog.data:
+            ngkeys = self.catalog.data["Group"].keys()
+            if len(ngkeys) > 0:
+                self.add_catalogIDs()
+
+        # merge hints from snap and catalog
+        self.merge_hints(self.catalog)
+
     def _set_metadata(self):
         """
         Set metadata from header and config.
         """
         md = self._clean_metadata_from_raw(self._metadata_raw)
         self.metadata = md
 
     @classmethod
-    def validate_path(cls, path: Union[str, os.PathLike], *args, **kwargs) -> bool:
+    def validate_path(
+        cls, path: Union[str, os.PathLike], *args, **kwargs
+    ) -> CandidateStatus:
         valid = super().validate_path(path, *args, **kwargs)
+        if valid.value > CandidateStatus.MAYBE.value:
+            valid = CandidateStatus.MAYBE
+        else:
+            return valid
+        # Arepo has no dedicated attribute to identify such runs.
+        # lets just query a bunch of attributes that are present for arepo runs
+        metadata_raw = load_metadata(path, **kwargs)
+        matchingattrs = True
+        matchingattrs &= "Git_commit" in metadata_raw["/Header"]
+        # not existent for any arepo run?
+        matchingattrs &= "Compactify_Version" not in metadata_raw["/Header"]
+
+        if matchingattrs:
+            valid = CandidateStatus.MAYBE
+
         return valid
 
     @classmethod
     def _clean_metadata_from_raw(cls, rawmetadata):
         """
         Set metadata from raw metadata.
         """
@@ -193,20 +213,21 @@
     def discover_catalog(self):
         """
         Discover the group catalog given the current path
         Returns
         -------
 
         """
+        p = str(self.path)
         # order of candidates matters. For Illustris "groups" must precede "fof_subhalo_tab"
         candidates = [
-            self.path.replace("snapshot", "group"),
-            self.path.replace("snapshot", "groups"),
-            self.path.replace("snapdir", "groups").replace("snap", "groups"),
-            self.path.replace("snapdir", "groups").replace("snap", "fof_subhalo_tab"),
+            p.replace("snapshot", "group"),
+            p.replace("snapshot", "groups"),
+            p.replace("snapdir", "groups").replace("snap", "groups"),
+            p.replace("snapdir", "groups").replace("snap", "fof_subhalo_tab"),
         ]
         for candidate in candidates:
             if not os.path.exists(candidate):
                 continue
             if candidate == self.path:
                 continue
             self.catalog = candidate
@@ -292,15 +313,23 @@
                 if not (key.startswith("PartType")):
                     continue
                 self.data[key]["SubhaloID"] = -1 * da.ones_like(
                     da[key]["uid"], dtype=np.int64
                 )
             return
 
-        subhalogrnr = self.data["Subhalo"]["SubhaloGrNr"]
+        shnr_attr = "SubhaloGrNr"
+        if shnr_attr not in self.data["Subhalo"]:
+            shnr_attr = "SubhaloGroupNr"  # what MTNG does
+        if shnr_attr not in self.data["Subhalo"]:
+            raise ValueError(
+                f"Could not find 'SubhaloGrNr' or 'SubhaloGroupNr' in {self.catalog}"
+            )
+
+        subhalogrnr = self.data["Subhalo"][shnr_attr]
         subhalocellcounts = self.data["Subhalo"]["SubhaloLenType"]
 
         # remove "units" for numba funcs
         if hasattr(subhalogrnr, "magnitude"):
             subhalogrnr = subhalogrnr.magnitude
         if hasattr(subhalocellcounts, "magnitude"):
             subhalocellcounts = subhalocellcounts.magnitude
@@ -374,14 +403,16 @@
         self.data[parttype][name] = hquantity
 
     def get_grouplengths(self, parttype="PartType0"):
         # todo: write/use PartType func always using integer rather than string?
         if parttype not in self._grouplengths:
             partnum = int(parttype[-1])
             lengths = self.data["Group"]["GroupLenType"][:, partnum].compute()
+            if isinstance(lengths, pint.Quantity):
+                lengths = lengths.magnitude
             self._grouplengths[parttype] = lengths
         return self._grouplengths[parttype]
 
     def grouped(
         self,
         fields: Union[str, da.Array, List[str], Dict[str, da.Array]] = "",
         parttype="PartType0",
@@ -389,41 +420,43 @@
         inputfields = None
         if isinstance(fields, str):
             if fields == "":  # if nothing is specified, we pass all we have.
                 arrdict = self.data[parttype]
             else:
                 arrdict = dict(field=self.data[parttype][fields])
                 inputfields = [fields]
-        elif isinstance(fields, da.Array):
+        elif isinstance(fields, da.Array) or isinstance(fields, pint.Quantity):
             arrdict = dict(daskarr=fields)
             inputfields = [fields.name]
         elif isinstance(fields, list):
             arrdict = {k: self.data[parttype][k] for k in fields}
             inputfields = fields
         elif isinstance(fields, dict):
             arrdict = {}
             arrdict.update(**fields)
             inputfields = list(arrdict.keys())
         else:
-            raise ValueError("Unknown input type.")
+            raise ValueError("Unknown input type '%s'." % type(fields))
         gop = GroupAwareOperation(
             self.get_grouplengths(parttype=parttype), arrdict, inputfields=inputfields
         )
         return gop
 
 
 class ArepoCatalog(ArepoSnapshot):
     def __init__(self, *args, **kwargs):
         kwargs["iscatalog"] = True
         if "fileprefix" not in kwargs:
             kwargs["fileprefix"] = "groups"
         super().__init__(*args, **kwargs)
 
     @classmethod
-    def validate_path(cls, path: Union[str, os.PathLike], *args, **kwargs) -> bool:
+    def validate_path(
+        cls, path: Union[str, os.PathLike], *args, **kwargs
+    ) -> CandidateStatus:
         kwargs["fileprefix"] = cls._get_fileprefix(path)
         valid = super().validate_path(path, *args, expect_grp=True, **kwargs)
         return valid
 
 
 class GroupAwareOperation:
     opfuncs = dict(min=np.min, max=np.max, sum=np.sum, half=lambda x: x[::2])
@@ -626,21 +659,23 @@
     return da.map_blocks(
         get_hidx_daskwrap, gidx, halocelloffsets, meta=np.array((), dtype=np.int64)
     )
 
 
 def compute_haloquantity(gidx, halocelloffsets, hvals, *args):
     """Computes a halo quantity for each particle with dask."""
-    return da.map_blocks(
+    res = map_blocks(
         get_haloquantity_daskwrap,
         gidx,
         halocelloffsets,
         hvals,
         meta=np.array((), dtype=hvals.dtype),
+        output_units=hvals.units,
     )
+    return res
 
 
 @jit(nopython=True)
 def get_shidx(
     gidx_start: int,
     gidx_count: int,
     celloffsets: NDArray[np.int64],
@@ -920,15 +955,15 @@
         entry_nbytes_out,
         cpucost_halo=cpucost_halo,
         Nmin=Nmin,
         chunksize_bytes=chunksize_bytes,
     )
 
     # TODO: Get rid of oindex; only here because have not adjusted code to map_halo_operation_get_chunkedges
-    totlength = offsets[-1]
+    totlength = int(offsets[-1])
     oindex = np.array(list(list_chunkedges[:, 0]) + [list_chunkedges[-1, -1]])
 
     new_axis = None
     chunks = np.diff(oindex)
     # TODO: Where does the next line come from? Does not make sense
     # chunks[-1] += lengths.shape[0]
     chunks = [tuple(chunks.tolist())]
```

### Comparing `scida-0.2.1/src/scida/customs/rockstar/dataset.py` & `scida-0.2.2/src/scida/customs/rockstar/dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import os
 from typing import Union
 
 from scida.interface import Dataset
+from scida.interfaces.mixins import CosmologyMixin
 from scida.io import load_metadata_all
 
 
-class RockstarCatalog(Dataset):
+class RockstarCatalog(CosmologyMixin, Dataset):
+    _unitfile = "units/rockstar.yaml"
+
     def __init__(self, path, **kwargs) -> None:
         super().__init__(path, **kwargs)
 
     @classmethod
     def validate_path(cls, path: Union[str, os.PathLike], *args, **kwargs) -> bool:
         """
         Check if path is valid for this interface.
@@ -29,19 +32,15 @@
         iszarr = path.rstrip("/").endswith(".zarr")
         if path.endswith(".hdf5") or iszarr:
             possibly_valid = True
 
         if possibly_valid:
             metadata_raw_all = load_metadata_all(path, **kwargs)
 
-            attrs = metadata_raw_all["attrs"]
-
-            # lets use the "feature" that rockstar adds no attributes (?) but uses scalar datasets
-            if len(attrs) != 0:
-                return False
+            # attrs = metadata_raw_all["attrs"]
 
             # usually rockstar has some cosmology parameters attached
             datasets = metadata_raw_all["datasets"]
             dsnames = [d[0] for d in datasets]
             if "/cosmology:omega_dm" not in dsnames:
                 return False
```

### Comparing `scida-0.2.1/src/scida/discovertypes.py` & `scida-0.2.2/src/scida/discovertypes.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 import os
 from collections import Counter
 from enum import Enum
 from functools import reduce
 from inspect import getmro
 from typing import List, Union
 
+from scida.config import get_simulationconfig
 from scida.interfaces.mixins import CosmologyMixin
 from scida.io import load_metadata
+from scida.misc import check_config_for_dataset
 from scida.registries import dataseries_type_registry, dataset_type_registry
 
 log = logging.getLogger(__name__)
 
 
 class CandidateStatus(Enum):
     NO = 0  # definitely not a candidate
@@ -26,14 +28,47 @@
         metadata_raw = load_metadata(path, fileprefix=None)
     z = metadata_raw.get("/Header", {}).get("Redshift", None)
     if z is not None:
         mixins.append(CosmologyMixin)
     return mixins
 
 
+def _determine_type_from_simconfig(path, classtype="dataset", reg=None):
+    if reg is None:
+        reg = dict()
+        reg.update(**dataset_type_registry)
+        reg.update(**dataseries_type_registry)
+    metadata_raw = dict()
+    if classtype == "dataset":
+        metadata_raw = load_metadata(path, fileprefix=None)
+    candidates = check_config_for_dataset(metadata_raw, path=path)
+    assert len(candidates) <= 1
+    cls = None
+    if len(candidates) == 1:
+        simconf = get_simulationconfig()
+        dstype = simconf.get("data", {}).get(candidates[0]).get("dataset_type", None)
+        if isinstance(dstype, dict):
+            # series or dataset based on past candidate
+            if classtype == "series":
+                cls = reg[dstype["series"]]
+            elif classtype == "dataset":
+                cls = reg[dstype["dataset"]]
+            else:
+                raise ValueError("Unknown class type '%s'." % classtype)
+        elif isinstance(dstype, str):
+            cls = reg[dstype]  # not split into series and dataset
+        elif dstype is None:
+            pass  # simply no dataset_type specified
+        else:
+            raise ValueError(
+                "Unknown type of dataset config variable. content: '%s'" % dstype
+            )
+    return cls
+
+
 def _determine_type(
     path: Union[str, os.PathLike],
     test_datasets: bool = True,
     test_dataseries: bool = True,
     strict: bool = False,
     catch_exception: bool = True,
     **kwargs
@@ -71,25 +106,32 @@
         if valid != CandidateStatus.NO:
             available_dtypes.append(k)
             dtypes_status.append(valid)  # will be YES or MAYBE
 
     if len(available_dtypes) == 0:
         raise ValueError("Unknown data type.")
     if len(available_dtypes) > 1:
-        good_matches = [
-            k
-            for k, v in zip(available_dtypes, dtypes_status)
-            if v == CandidateStatus.YES
-        ]
-        if len(good_matches) >= 1:
-            available_dtypes = (
-                good_matches  # discard all MAYBEs as we have better options
-            )
+        # TODO: Rethink how tu use MAYBE/YES information.
+        # below lines not suitable for this.
+        # good_matches = [
+        #     k
+        #     for k, v in zip(available_dtypes, dtypes_status)
+        #     if v == CandidateStatus.YES
+        # ]
+        # if len(good_matches) >= 1:
+        #     available_dtypes = (
+        #         good_matches  # discard all MAYBEs as we have better options
+        #     )
         # reduce candidates by looking at most specific ones.
         inheritancecounters = [Counter(getmro(reg[k])) for k in reg.keys()]
+        mros = [getmro(reg[k]) for k in reg.keys()]
+        lens = [len([m for m in mro if "Mixin" not in m.__name__]) for mro in mros]
+        zp = zip(available_dtypes, lens, dtypes_status)
+        lst = sorted(zp, key=lambda x: x[2].value)
+        lst = sorted(lst, key=lambda x: x[1])
         # try to find candidate that shows up only once across all inheritance trees.
         # => this will be the most specific candidate(s).
         count = reduce(lambda x, y: x + y, inheritancecounters)
         countdict = {k: count[reg[k]] for k in available_dtypes}
         mincount = min(countdict.values())
         available_dtypes = [k for k in available_dtypes if count[reg[k]] == mincount]
         if len(available_dtypes) > 1:
```

### Comparing `scida-0.2.1/src/scida/fields.py` & `scida-0.2.2/src/scida/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,15 @@
             fieldrecipes_kwargs = {}
         self.aliases = aliases
         self.name = kwargs.pop("name", None)
         self._fields: Dict[str, da.Array] = {}
         self._fields.update(*args, **kwargs)
         self._recipes = "bla"
         self._fieldrecipes = {}
+        self._fieldlength = None
         self.fieldrecipes_kwargs = fieldrecipes_kwargs
         self.withunits = withunits
         self._containers: Dict[
             str, FieldContainer
         ] = dict()  # other containers as subgroups
         if containers is not None:
             for k in containers:
@@ -100,17 +101,15 @@
 
     def merge(self, collection, overwrite=True):
         if not isinstance(collection, FieldContainer):
             raise TypeError("Can only merge FieldContainers.")
         # TODO: support nested containers
         for k in collection._containers:
             if k not in self._containers:
-                self._containers[k] = FieldContainer(
-                    fieldrecipes_kwargs=self.fieldrecipes_kwargs
-                )
+                continue
             if overwrite:
                 c1 = self._containers[k]
                 c2 = collection._containers[k]
             else:
                 c1 = collection._containers[k]
                 c2 = self._containers[k]
             c1._fields.update(**c2._fields)
@@ -121,20 +120,31 @@
         rcps = set(self._fieldrecipes)
         flds = set([k for k in self._fields if k not in self.internals])
         ntot = len(rcps | flds)
         return ntot
 
     @property
     def fieldlength(self):
-        itr = iter(self._fields.values())
-        if len(self._fields) == 0:
-            return None
-        first = next(itr)
+        if self._fieldlength is not None:
+            return self._fieldlength
+        fvals = self._fields.values()
+        itr = iter(fvals)
+        if len(fvals) == 0:
+            # can we infer from recipes?
+            if len(self._fieldrecipes) > 0:
+                # get first recipe
+                name = next(iter(self._fieldrecipes.keys()))
+                first = self._getitem(name, evaluate_recipe=True)
+            else:
+                return None
+        else:
+            first = next(itr)
         if all(first.shape[0] == v.shape[0] for v in self._fields.values()):
-            return first.shape[0]
+            self._fieldlength = first.shape[0]
+            return self._fieldlength
         else:
             return None
 
     def keys(
         self, withgroups=True, withrecipes=True, withinternal=False, withfields=True
     ):
         fieldkeys = []
@@ -149,18 +159,18 @@
                 fieldkeys = list(set(fieldkeys) | set(recipekeys))
         if withgroups:
             groupkeys = self._containers.keys()
             fieldkeys = list(set(fieldkeys) | set(groupkeys))
         return sorted(fieldkeys)
 
     def items(self):
-        return ((k, self._getitem(k, evaluate_recipe=False)) for k in self.keys())
+        return ((k, self._getitem(k, evaluate_recipe=True)) for k in self.keys())
 
     def values(self):
-        return (self._getitem(k, evaluate_recipe=False) for k in self.keys())
+        return (self._getitem(k, evaluate_recipe=True) for k in self.keys())
 
     def register_field(
         self,
         containernames=None,
         name: Optional[str] = None,
         description="",
         units=None,
@@ -259,19 +269,22 @@
         ddf = dd.concat(dfs, axis=1)
         return ddf
 
     def add_alias(self, alias, name):
         self.aliases[alias] = name
 
     def add_container(self, key, **kwargs):
+        tkwargs = dict(**kwargs)
+        if "name" not in tkwargs:
+            tkwargs["name"] = key
         self._containers[key] = FieldContainer(
             fieldrecipes_kwargs=self.fieldrecipes_kwargs,
             withunits=self.withunits,
             parent=self,
-            **kwargs,
+            **tkwargs,
         )
 
     def _getitem(
         self, key, force_derived=False, update_dict=True, evaluate_recipe=True
     ):
         if key in self.aliases:
             key = self.aliases[key]
@@ -314,15 +327,20 @@
                 return field
             else:
                 raise KeyError("Unknown field '%s'" % key)
 
     def __delitem__(self, key):
         if key in self._fieldrecipes:
             del self._fieldrecipes[key]
-        del self._fields[key]
+        if key in self._containers:
+            del self._containers[key]
+        elif key in self._fields:
+            del self._fields[key]
+        else:
+            raise KeyError("Unknown key '%s'" % key)
 
     def __len__(self):
         return len(self.keys())
 
     def get(self, key, value=None, allow_derived=True, force_derived=False):
         if key in self._fieldrecipes and not allow_derived:
             raise KeyError("Field '%s' is derived (allow_derived=False)" % key)
```

### Comparing `scida-0.2.1/src/scida/helpers_hdf5.py` & `scida-0.2.2/src/scida/helpers_hdf5.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,45 @@
 import h5py
 import numpy as np
 import zarr
 
 log = logging.getLogger(__name__)
 
 
-def walk_group(obj, tree, get_attrs=False):
+def get_dtype(obj):
+    if isinstance(obj, h5py.Dataset):
+        try:
+            dtype = obj.dtype
+        except TypeError as e:
+            msg = "data type '<u6' not understood"
+            if msg == e.__str__():
+                # MTNG defines 6 byte unsigned integers, which are not supported by h5py
+                # could not figure out how to query type in h5py other than the reporting error.
+                # (any call to .dtype will try to resolve "<u6" to a numpy dtype, which fails)
+                # we just handle this as 64 bit unsigned integer
+                dtype = np.uint64
+            else:
+                raise e
+        return dtype
+    elif isinstance(obj, zarr.Array):
+        return obj.dtype
+    else:
+        return None
+
+
+def walk_group(obj, tree, get_attrs=False, scalar_to_attr=True):
     if len(tree) == 0:
         tree.update(**dict(attrs={}, groups=[], datasets=[]))
     if get_attrs and len(obj.attrs) > 0:
         tree["attrs"][obj.name] = dict(obj.attrs)
     if isinstance(obj, (h5py.Dataset, zarr.Array)):
-        tree["datasets"].append([obj.name, obj.shape, obj.dtype])
+        dtype = get_dtype(obj)
+        tree["datasets"].append([obj.name, obj.shape, dtype])
+        if scalar_to_attr and len(obj.shape) == 0:
+            tree["attrs"][obj.name] = obj[()]
     elif isinstance(obj, (h5py.Group, zarr.Group)):
         tree["groups"].append(obj.name)  # continue the walk
         for k, o in obj.items():
             walk_group(o, tree, get_attrs=get_attrs)
 
 
 def walk_zarrfile(fn, tree, get_attrs=True):
@@ -213,17 +237,22 @@
                 attrval0 = attrvallist[0]
                 if isinstance(attrval0, np.ndarray):
                     if not (np.all([np.array_equal(attrval0, v) for v in attrvallist])):
                         log.debug("%s: %s has different values." % (apath, k))
                         attrs_differ[apath][k] = np.stack(attrvallist)
                         continue
                 else:
-                    if not len(set(attrvallist)) == 1:
+                    same = len(set(attrvallist)) == 1
+                    if isinstance(attrval0, np.floating):
+                        # for floats we do not require binary equality
+                        # (we had some incident...)
+                        same = np.allclose(attrval0, attrvallist)
+                    if not same:
                         log.debug("%s: %s has different values." % (apath, k))
-                        attrs_differ[apath][k] = np.array(attrval0)
+                        attrs_differ[apath][k] = np.array(attrvallist)
                         continue
                 attrs_same[apath][k] = attrval0
         for apath in attrspaths_all:
             for k, v in attrs_same.get(apath, {}).items():
                 hf[apath].attrs[k] = v
             for k, v in attrs_differ.get(apath, {}).items():
                 hf[apath].attrs[k] = v
```

### Comparing `scida-0.2.1/src/scida/helpers_misc.py` & `scida-0.2.2/src/scida/helpers_misc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import hashlib
 import inspect
 import io
 import re
 import types
 
+import dask.array as da
 import numpy as np
 
 
 def hash_path(path):
     sha = hashlib.sha256()
     sha.update(str(path).strip("/ ").encode())
     return sha.hexdigest()[:16]
@@ -84,7 +85,44 @@
 def sprint(*args, end="\n", **kwargs):
     """print to string"""
     output = io.StringIO()
     print(*args, file=output, end=end, **kwargs)
     contents = output.getvalue()
     output.close()
     return contents
+
+
+def map_blocks(
+    func,
+    *args,
+    name=None,
+    token=None,
+    dtype=None,
+    chunks=None,
+    drop_axis=None,
+    new_axis=None,
+    enforce_ndim=False,
+    meta=None,
+    output_units=None,
+    **kwargs,
+):
+    """map_blocks with units"""
+    da_kwargs = dict(
+        name=name,
+        token=token,
+        dtype=dtype,
+        chunks=chunks,
+        drop_axis=drop_axis,
+        new_axis=new_axis,
+        enforce_ndim=enforce_ndim,
+        meta=meta,
+    )
+    res = da.map_blocks(
+        func,
+        *args,
+        **da_kwargs,
+        **kwargs,
+    )
+    if output_units is not None:
+        res = res * output_units
+
+    return res
```

### Comparing `scida-0.2.1/src/scida/interface.py` & `scida-0.2.2/src/scida/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,22 +366,24 @@
 
 
 class Selector(object):
     """Base Class for data selection decorator factory"""
 
     def __init__(self):
         self.keys = None  # the keys we check for.
-        self.data_backup = {}  # holds a copy of the species' fields
-        self.data = {}  # holds the species' fields we operate on
+        self.data_backup = FieldContainer()  # holds a copy of the species' fields
+        self.data: FieldContainer = (
+            FieldContainer()
+        )  # holds the species' fields we operate on
 
     def __call__(self, fn, *args, **kwargs):
         def newfn(*args, **kwargs):
             # TODO: Add graceful exit/restore after exception in self.prepare
             self.data_backup = args[0].data
-            self.data = {}
+            self.data = FieldContainer()
             deepdictkeycopy(self.data_backup, self.data)
 
             self.prepare(*args, **kwargs)
             if self.keys is None:
                 raise NotImplementedError(
                     "Subclass implementation needed for self.keys!"
                 )
```

### Comparing `scida-0.2.1/src/scida/interfaces/gadgetstyle.py` & `scida-0.2.2/src/scida/customs/gadgetstyle/dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 import re
-from typing import Union
+from typing import Optional, Union
 
 import numpy as np
 
+from scida.discovertypes import CandidateStatus
 from scida.interface import Dataset
 from scida.io import load_metadata
 
 log = logging.getLogger(__name__)
 
 
 class GadgetStyleSnapshot(Dataset):
@@ -63,41 +64,41 @@
         if set(prfxs) == {"groups", "fof_subhalo_tab"}:
             return "groups"  # "groups" over "fof_subhalo_tab"
         return prfxs[0]
 
     @classmethod
     def validate_path(
         cls, path: Union[str, os.PathLike], *args, expect_grp=False, **kwargs
-    ) -> bool:
+    ) -> CandidateStatus:
         """
         Check if path is valid for this interface.
         Parameters
         ----------
         path: str, os.PathLike
             path to check
         args
         kwargs
 
         Returns
         -------
         bool
         """
         path = str(path)
-        possibly_valid = False
+        possibly_valid = CandidateStatus.NO
         iszarr = path.rstrip("/").endswith(".zarr")
         if path.endswith(".hdf5") or iszarr:
-            possibly_valid = True
+            possibly_valid = CandidateStatus.MAYBE
         if os.path.isdir(path):
             files = os.listdir(path)
             sufxs = [f.split(".")[-1] for f in files]
             if not iszarr and len(set(sufxs)) > 1:
-                possibly_valid = False
+                possibly_valid = CandidateStatus.NO
             if sufxs[0] == "hdf5":
-                possibly_valid = True
-        if possibly_valid:
+                possibly_valid = CandidateStatus.MAYBE
+        if possibly_valid != CandidateStatus.NO:
             metadata_raw = load_metadata(path, **kwargs)
             # need some silly combination of attributes to be sure
             if all([k in metadata_raw for k in ["/Header"]]):
                 # identifying snapshot or group catalog
                 is_snap = all(
                     [
                         k in metadata_raw["/Header"]
@@ -107,23 +108,52 @@
                 is_grp = all(
                     [
                         k in metadata_raw["/Header"]
                         for k in ["Ngroups_ThisFile", "Ngroups_Total"]
                     ]
                 )
                 if is_grp:
-                    return True
+                    return CandidateStatus.YES
                 if is_snap and not expect_grp:
-                    return True
-        return False
+                    return CandidateStatus.YES
+        return CandidateStatus.NO
 
     def register_field(self, parttype, name=None, description=""):
         res = self.data.register_field(parttype, name=name, description=description)
         return res
 
+    def merge_data(
+        self, secondobj, fieldname_suffix="", root_group: Optional[str] = None
+    ):
+        data = self.data
+        if root_group is not None:
+            if root_group not in data._containers:
+                data.add_container(root_group)
+            data = self.data[root_group]
+        for k in secondobj.data:
+            key = k + fieldname_suffix
+            if key not in data:
+                data[key] = secondobj.data[k]
+            else:
+                log.debug("Not overwriting field '%s' during merge_data." % key)
+            secondobj.data.fieldrecipes_kwargs["snap"] = self
+
+    def merge_hints(self, secondobj):
+        # merge hints from snap and catalog
+        for h in secondobj.hints:
+            if h not in self.hints:
+                self.hints[h] = secondobj.hints[h]
+            elif isinstance(self.hints[h], dict):
+                # merge dicts
+                for k in secondobj.hints[h]:
+                    if k not in self.hints[h]:
+                        self.hints[h][k] = secondobj.hints[h][k]
+            else:
+                pass  # nothing to do; we do not overwrite with catalog props
+
 
 class SwiftSnapshot(GadgetStyleSnapshot):
     def __init__(self, path, chunksize="auto", virtualcache=True, **kwargs) -> None:
         super().__init__(path, chunksize=chunksize, virtualcache=virtualcache, **kwargs)
 
     @classmethod
     def validate_path(cls, path: Union[str, os.PathLike], *args, **kwargs) -> bool:
@@ -132,24 +162,8 @@
             return False
         metadata_raw = load_metadata(path, **kwargs)
         comparestr = metadata_raw.get("/Code", {}).get("Code", b"").decode()
         valid = "SWIFT" in comparestr
         return valid
 
 
-class GizmoSnapshot(GadgetStyleSnapshot):
-    def __init__(self, path, chunksize="auto", virtualcache=True, **kwargs) -> None:
-        super().__init__(path, chunksize=chunksize, virtualcache=virtualcache, **kwargs)
-
-    @classmethod
-    def validate_path(cls, path: Union[str, os.PathLike], *args, **kwargs) -> bool:
-        valid = super().validate_path(path, *args, **kwargs)
-        if not valid:
-            return False
-        # there does not seem to be identifying metadata for Gizmo (? see SIMBA snap),
-        # so we just return False for now (i.e. falling back onto GadgetStyleSnapshot on auto-detection)
-        # TODO: split routine into "validate" and "identify"? One accessing whether we *could* read the data,
-        # the other checking whether we *should* primarily read the data this way?
-        return False
-
-
 # right now ArepoSnapshot is defined in separate file
```

### Comparing `scida-0.2.1/src/scida/interfaces/mixins/cosmology.py` & `scida-0.2.2/src/scida/interfaces/mixins/cosmology.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,23 +43,32 @@
     return z
 
 
 def get_cosmology_from_rawmetadata(metadata_raw):
     import astropy.units as u
     from astropy.cosmology import FlatLambdaCDM
 
+    # gadgetstyle
     aliasdict = dict(h=["HubbleParam"], om0=["Omega0"], ob0=["OmegaBaryon"])
     cparams = dict(h=None, om0=None, ob0=None)
     for grp in ["Parameters", "Header"]:
         for p, v in cparams.items():
             if v is not None:
                 continue  # already acquired some value for this item.
             for alias in aliasdict[p]:
                 cparams[p] = metadata_raw.get("/" + grp, {}).get(alias, cparams[p])
 
+    # rockstar
+    if cparams["h"] is None and "/cosmology:hubble" in metadata_raw:
+        cparams["h"] = metadata_raw["/cosmology:hubble"]
+    if cparams["om0"] is None and "/cosmology:omega_matter" in metadata_raw:
+        cparams["om0"] = metadata_raw["/cosmology:omega_matter"]
+    if cparams["ob0"] is None and "/cosmology:omega_baryon" in metadata_raw:
+        cparams["ob0"] = metadata_raw["/cosmology:omega_baryon"]
+
     h, om0, ob0 = cparams["h"], cparams["om0"], cparams["ob0"]
     if None in [h, om0]:
         log.info("Cannot infer cosmology.")
         return None
     elif ob0 is None:
         log.info(
             "No Omega baryon given, we will assume a value of '0.0486' for the cosmology."
```

### Comparing `scida-0.2.1/src/scida/interfaces/mixins/spatial.py` & `scida-0.2.2/src/scida/interfaces/mixins/spatial.py`

 * *Files identical despite different names*

### Comparing `scida-0.2.1/src/scida/interfaces/mixins/units.py` & `scida-0.2.2/src/scida/interfaces/mixins/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,16 @@
         has_convfactor = len(cgskey) > 0
         if has_convfactor:
             cgskey = cgskey[0]
             cgsfactor = attrs[cgskey]
     # get dimensions
     unit = cgsfactor
     if isinstance(unit, np.ndarray):
-        assert len(unit) == 1
+        if len(unit) != 1:
+            log.debug("Unexpected shape (%s) of unit factor." % unit.shape)
         unit = unit[0]
     if unit == 0.0:
         unit = ureg.Quantity(1.0)  # zero makes no sense.
     # TODO: Missing a scaling?
     # TODO: Missing h scaling?
     ukeys = ["length", "mass", "velocity", "time", "h", "a"]
     if any([k + "_scaling" in attrs.keys() for k in ukeys]):  # like TNG
@@ -180,16 +181,17 @@
 
 class UnitMixin(Mixin):
     def __init__(self, *args, **kwargs):
         self.units = {}
         self.data = {}
         self._metadata_raw = {}
 
-        ureg = UnitRegistry(autoconvert_offset_to_baseunit=True)
-        ureg = kwargs.pop("ureg", ureg)
+        ureg = kwargs.pop("ureg", None)
+        if ureg is None:
+            ureg = UnitRegistry(autoconvert_offset_to_baseunit=True)
         self.ureg = self.unitregistry = ureg
 
         super().__init__(*args, **kwargs)
 
         # get unit hints
         unithints = {}
         unitfile = ""
@@ -197,15 +199,15 @@
         missing_units = userconf.get("missing_units", "warn")
         assert missing_units in ["warn", "raise", "ignore"]
         if "dsname" in self.hints:
             c = get_simulationconfig()
             dsprops = c["data"][self.hints["dsname"]]
             missing_units = dsprops.get("missing_units", missing_units)
             unitfile = dsprops.get("unitfile", "")
-        unitfile = kwargs.pop("unitfile", unitfile)
+        unitfile = kwargs.pop("unitfile", unitfile)  # passed kwarg takes precedence
         unitdefs = get_config_fromfile("units/general.yaml").get("units", {})
         if unitfile != "":
             unithints = get_config_fromfile(unitfile)
             unitdefs.update(unithints.get("units", {}))
 
         units = kwargs.pop("units")
         if isinstance(units, bool):
```

### Comparing `scida-0.2.1/src/scida/io.py` & `scida-0.2.2/src/scida/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     def __init__(self, path):
         super().__init__(path)
         self.tempfile = ""
         self.location = ""
 
     def load_metadata(self, fileprefix="", **kwargs):
         """Take a quick glance at the metadata."""
-        cachefp = return_hdf5cachepath(self.path)
+        cachefp = return_hdf5cachepath(self.path, fileprefix=fileprefix)
         if cachefp is not None and os.path.isfile(cachefp):
             path = cachefp
         else:
             # get data from first file in list
             paths = self.get_chunkedfiles(fileprefix)
             if len(paths) == 0:
                 raise ValueError("No files for prefix '%s' found." % fileprefix)
@@ -132,29 +132,34 @@
         overwrite=False,
         fileprefix="",
         token="",
         chunksize="auto",
         virtualcache=False,
         **kwargs
     ):
-        cachefp = return_hdf5cachepath(self.path)
+        cachefp = return_hdf5cachepath(self.path, fileprefix=fileprefix)
         # three cases we need to cache:
         create = False
         if cachefp is None:
             # 1. no cachepath given
             create = True
         elif not os.path.isfile(cachefp):
             # 2. no cachefile exists
             create = True
         elif overwrite:
             # 3. cachefile exists, but overwrite=True
             create = True
 
         if create:
-            self.create_cachefile(fileprefix=fileprefix, virtualcache=virtualcache)
+            print_cachefile_creation = kwargs.get("print_cachefile_creation", True)
+            self.create_cachefile(
+                fileprefix=fileprefix,
+                virtualcache=virtualcache,
+                verbose=print_cachefile_creation,
+            )
 
         try:
             datadict = self.load_cachefile(
                 cachefp, token=token, chunksize=chunksize, **kwargs
             )
         except InvalidCacheError:
             # if we get an error, we try to create a new cache file (once)
@@ -202,20 +207,22 @@
             )
             raise ValueError(msg)
         nmbrs = [int(f.split(".")[-2]) for f in files]
         sortidx = np.argsort(nmbrs)
         files = files[sortidx]
         return files
 
-    def create_cachefile(self, fileprefix="", virtualcache=False):
+    def create_cachefile(self, fileprefix="", virtualcache=False, verbose=None):
         config = get_config()
-        print_msg = config.get("print_cachefile_creation", True)
+        print_msg = verbose
+        if verbose is None:
+            print_msg = config.get("print_cachefile_creation", True)
         if print_msg:
             print("Creating cache file, this may take a while...")
-        cachefp = return_hdf5cachepath(self.path)
+        cachefp = return_hdf5cachepath(self.path, fileprefix=fileprefix)
         files = self.get_chunkedfiles(fileprefix)
 
         self.location = cachefp
         if cachefp is None:
             # no filepath available
             self.tempfile = tempfile.NamedTemporaryFile("wb", suffix=".hdf5")
             self.location = self.tempfile.name
@@ -304,14 +311,17 @@
     # Make each datadict entry a FieldContainer
     for group in datagroups:
         get_container_from_path(group, rootcontainer, create_missing=True)
 
     # datasets
     for i, dataset in enumerate(tree["datasets"]):
         # fpath is the path to the group containing given field
+        # ignore if scalar
+        if len(dataset[1]) == 0:
+            continue
         fpath = "/".join(dataset[0].split("/")[:-1])
         toload = fpath == "" or fpath in datagroups
         if not toload:
             continue
 
         container = get_container_from_path(fpath, rootcontainer)
         # TODO: still change for nesting
@@ -390,16 +400,14 @@
             # TODO: as we do not load any fields any more we do not have a reference for the dask chunking.
             container["uid"] = da.arange(nparts)
         else:
             print("no uid created for %s" % container.name)
 
     walk_container(data, handler_group=create_uids)
 
-    # walk_container(data, handler_field=lambda x, y: print(x, y))
-
     # attrs
     metadata = tree["attrs"]
     return data, metadata
 
 
 def determine_loader(path):
     if os.path.isdir(path):
```

### Comparing `scida-0.2.1/src/scida/misc.py` & `scida-0.2.2/src/scida/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,22 +26,26 @@
             if not create_missing:
                 raise ValueError("Container '%s' not found in '%s'" % (key, rv))
             rv.add_container(key, name=key)
         rv = rv._containers[key]
     return rv
 
 
-def return_hdf5cachepath(path_original) -> str:
-    fp = return_cachefile_path(os.path.join(hash_path(path_original), "data.hdf5"))
+def return_hdf5cachepath(path_original, fileprefix=None) -> str:
+    path = path_original
+    if fileprefix is not None:
+        path = os.path.join(path, fileprefix)
+    hsh = hash_path(path)
+    fp = return_cachefile_path(os.path.join(hsh, "data.hdf5"))
     return fp
 
 
-def path_hdf5cachefile_exists(path) -> bool:
+def path_hdf5cachefile_exists(path, **kwargs) -> bool:
     """Checks whether a cache file exists for given path."""
-    fp = return_hdf5cachepath(path)
+    fp = return_hdf5cachepath(path, **kwargs)
     if os.path.isfile(fp):
         return True
     return False
 
 
 def return_cachefile_path(fname: str) -> Optional[str]:
     """If path cannot be generated, return None"""
```

### Comparing `scida-0.2.1/src/scida/series.py` & `scida-0.2.2/src/scida/series.py`

 * *Files identical despite different names*

### Comparing `scida-0.2.1/setup.py` & `scida-0.2.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 
 packages = \
 ['scida',
  'scida.configfiles',
  'scida.configfiles.units',
  'scida.customs',
  'scida.customs.arepo',
+ 'scida.customs.arepo.MTNG',
+ 'scida.customs.arepo.TNGcluster',
+ 'scida.customs.gadgetstyle',
  'scida.customs.gizmo',
  'scida.customs.rockstar',
- 'scida.interfaces',
  'scida.interfaces.mixins']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['astropy>=5.0,<6.0',
@@ -30,15 +32,15 @@
  'pyyaml>=5.3.1',
  'requests>=2.31.0,<3.0.0',
  'tqdm>=4.64.1,<5.0.0',
  'zarr>=v2.10.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'scida',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Convenience wrapper around large scientific datasets to process with dask.',
     'long_description': '# scida\n\n![test status](https://github.com/cbyrohl/scida/actions/workflows/tests.yml/badge.svg)\n\nscida is an out-of-the-box analysis tool for large scientific datasets. It primarily supports the astrophysics community, focusing on cosmological and galaxy formation simulations using particles or unstructured meshes, as well as large observational datasets.\nThis tool uses dask, allowing analysis to scale up from your personal computer to HPC resources and the cloud.\n\n## Features\n\n- Unified, high-level interface to load and analyze large datasets from a variety of sources.\n- Parallel, task-based data processing with dask arrays.\n- Physical unit support via pint.\n- Easily extensible architecture.\n\n## Requirements\n\n- Python >= 3.9\n\n\n## Documentation\nThe documentation can be found [here](https://cbyrohl.github.io/scida/).\n\n## Install\n\n```\npip install scida\n```\n\n## First Steps\nAfter installing scida, follow the [tutorial](https://cbyrohl.github.io/scida/tutorial/).\n\n## License\n\nDistributed under the terms of the [MIT license](LICENSE),\n_scida_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue](https://github.com/cbyrohl/scida/issues/new) along with a detailed description.\n\n## Acknowledgements\n\nThe project structure was adapted from [Wolt](https://github.com/woltapp/wolt-python-package-cookiecutter) and [Hypermodern Python](https://github.com/cjolowicz/cookiecutter-hypermodern-python) cookiecutter templates.\n',
     'author': 'Chris Byrohl',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scida-0.2.1/PKG-INFO` & `scida-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scida
-Version: 0.2.1
+Version: 0.2.2
 Summary: Convenience wrapper around large scientific datasets to process with dask.
 Author: Chris Byrohl
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

