# Comparing `tmp/pyl3dmd-0.1.0.tar.gz` & `tmp/pyl3dmd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyl3dmd-0.1.0.tar", last modified: Sat Apr 22 16:45:19 2023, max compression
+gzip compressed data, was "pyl3dmd-0.1.1.tar", last modified: Tue Jul 11 04:02:58 2023, max compression
```

## Comparing `pyl3dmd-0.1.0.tar` & `pyl3dmd-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 16:45:19.382943 pyl3dmd-0.1.0/
--rw-rw-rw-   0        0        0      753 2023-04-22 16:45:19.381948 pyl3dmd-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-22 16:45:19.373968 pyl3dmd-0.1.0/pyl3dmd/
--rw-rw-rw-   0        0        0      908 2023-02-08 02:47:17.000000 pyl3dmd-0.1.0/pyl3dmd/__init__.py
--rw-rw-rw-   0        0        0     7700 2023-02-14 04:41:39.000000 pyl3dmd-0.1.0/pyl3dmd/cpsa.py
--rw-rw-rw-   0        0        0    19226 2023-04-22 16:38:51.000000 pyl3dmd-0.1.0/pyl3dmd/descriptors1set.py
--rw-rw-rw-   0        0        0    27100 2023-04-22 16:37:16.000000 pyl3dmd-0.1.0/pyl3dmd/descriptors2set.py
--rw-rw-rw-   0        0        0    11685 2023-04-22 16:40:28.000000 pyl3dmd-0.1.0/pyl3dmd/descriptors3set.py
--rw-rw-rw-   0        0        0     7700 2023-02-17 11:13:14.000000 pyl3dmd-0.1.0/pyl3dmd/descriptors4set.py
--rw-rw-rw-   0        0        0     3086 2023-02-17 11:13:14.000000 pyl3dmd-0.1.0/pyl3dmd/descriptors5set.py
--rw-rw-rw-   0        0        0     4278 2023-02-17 11:13:14.000000 pyl3dmd-0.1.0/pyl3dmd/descriptors6set.py
--rw-rw-rw-   0        0        0     2966 2023-02-14 04:42:15.000000 pyl3dmd-0.1.0/pyl3dmd/distancedistancematrixdescriptors.py
--rw-rw-rw-   0        0        0     2573 2023-02-14 04:42:09.000000 pyl3dmd-0.1.0/pyl3dmd/geary.py
--rw-rw-rw-   0        0        0    24925 2023-02-14 04:42:04.000000 pyl3dmd-0.1.0/pyl3dmd/geometricdescriptors.py
--rw-rw-rw-   0        0        0     5432 2023-04-22 16:37:44.000000 pyl3dmd-0.1.0/pyl3dmd/getadjacencyanddistancematrices.py
--rw-rw-rw-   0        0        0     8781 2023-02-17 06:58:03.000000 pyl3dmd-0.1.0/pyl3dmd/getatomicproperties.py
--rw-rw-rw-   0        0        0    11133 2023-02-14 04:42:26.000000 pyl3dmd-0.1.0/pyl3dmd/getaway.py
--rw-rw-rw-   0        0        0    10918 2023-04-21 19:20:13.000000 pyl3dmd-0.1.0/pyl3dmd/getinfofromlammpsdatafile.py
--rw-rw-rw-   0        0        0    11194 2023-02-08 02:50:57.000000 pyl3dmd-0.1.0/pyl3dmd/getinfofromlammpstrajfile.py
--rw-rw-rw-   0        0        0     2607 2023-02-14 04:42:53.000000 pyl3dmd-0.1.0/pyl3dmd/moran.py
--rw-rw-rw-   0        0        0     2283 2023-02-14 04:42:48.000000 pyl3dmd-0.1.0/pyl3dmd/moreaubroto.py
--rw-rw-rw-   0        0        0     2413 2023-02-14 04:42:43.000000 pyl3dmd-0.1.0/pyl3dmd/morse.py
--rw-rw-rw-   0        0        0     9558 2023-02-13 17:27:02.000000 pyl3dmd-0.1.0/pyl3dmd/pyl3dmd.py
--rw-rw-rw-   0        0        0     2438 2023-02-14 04:43:08.000000 pyl3dmd-0.1.0/pyl3dmd/rdf.py
--rw-rw-rw-   0        0        0     5408 2023-04-22 16:44:14.000000 pyl3dmd-0.1.0/pyl3dmd/removehydrogenfrommolecule.py
--rw-rw-rw-   0        0        0    15383 2023-02-14 04:43:20.000000 pyl3dmd-0.1.0/pyl3dmd/topologyconnectivity3Ddescriptors.py
--rw-rw-rw-   0        0        0     3082 2023-02-14 04:43:37.000000 pyl3dmd-0.1.0/pyl3dmd/whim.py
-drwxrwxrwx   0        0        0        0 2023-04-22 16:45:19.380949 pyl3dmd-0.1.0/pyl3dmd.egg-info/
--rw-rw-rw-   0        0        0      753 2023-04-22 16:45:19.000000 pyl3dmd-0.1.0/pyl3dmd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      781 2023-04-22 16:45:19.000000 pyl3dmd-0.1.0/pyl3dmd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 16:45:19.000000 pyl3dmd-0.1.0/pyl3dmd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-22 16:45:19.000000 pyl3dmd-0.1.0/pyl3dmd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 16:45:19.383940 pyl3dmd-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2272 2023-04-22 16:42:36.000000 pyl3dmd-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 04:02:58.024189 pyl3dmd-0.1.1/
+-rw-rw-rw-   0        0        0      753 2023-07-11 04:02:58.024189 pyl3dmd-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-11 04:02:58.015211 pyl3dmd-0.1.1/pyl3dmd/
+-rw-rw-rw-   0        0        0      908 2023-02-08 02:47:17.000000 pyl3dmd-0.1.1/pyl3dmd/__init__.py
+-rw-rw-rw-   0        0        0     7700 2023-02-14 04:41:39.000000 pyl3dmd-0.1.1/pyl3dmd/cpsa.py
+-rw-rw-rw-   0        0        0    19226 2023-04-22 16:38:51.000000 pyl3dmd-0.1.1/pyl3dmd/descriptors1set.py
+-rw-rw-rw-   0        0        0    27100 2023-04-22 16:37:16.000000 pyl3dmd-0.1.1/pyl3dmd/descriptors2set.py
+-rw-rw-rw-   0        0        0    11685 2023-04-22 16:40:28.000000 pyl3dmd-0.1.1/pyl3dmd/descriptors3set.py
+-rw-rw-rw-   0        0        0     7656 2023-07-05 01:48:34.000000 pyl3dmd-0.1.1/pyl3dmd/descriptors4set.py
+-rw-rw-rw-   0        0        0     3166 2023-06-21 22:14:34.000000 pyl3dmd-0.1.1/pyl3dmd/descriptors5set.py
+-rw-rw-rw-   0        0        0     4278 2023-02-17 11:13:14.000000 pyl3dmd-0.1.1/pyl3dmd/descriptors6set.py
+-rw-rw-rw-   0        0        0     2966 2023-02-14 04:42:15.000000 pyl3dmd-0.1.1/pyl3dmd/distancedistancematrixdescriptors.py
+-rw-rw-rw-   0        0        0     2573 2023-02-14 04:42:09.000000 pyl3dmd-0.1.1/pyl3dmd/geary.py
+-rw-rw-rw-   0        0        0    24925 2023-02-14 04:42:04.000000 pyl3dmd-0.1.1/pyl3dmd/geometricdescriptors.py
+-rw-rw-rw-   0        0        0     5432 2023-04-22 16:37:44.000000 pyl3dmd-0.1.1/pyl3dmd/getadjacencyanddistancematrices.py
+-rw-rw-rw-   0        0        0     8781 2023-02-17 06:58:03.000000 pyl3dmd-0.1.1/pyl3dmd/getatomicproperties.py
+-rw-rw-rw-   0        0        0    11133 2023-02-14 04:42:26.000000 pyl3dmd-0.1.1/pyl3dmd/getaway.py
+-rw-rw-rw-   0        0        0    10918 2023-04-21 19:20:13.000000 pyl3dmd-0.1.1/pyl3dmd/getinfofromlammpsdatafile.py
+-rw-rw-rw-   0        0        0    11194 2023-02-08 02:50:57.000000 pyl3dmd-0.1.1/pyl3dmd/getinfofromlammpstrajfile.py
+-rw-rw-rw-   0        0        0     2607 2023-02-14 04:42:53.000000 pyl3dmd-0.1.1/pyl3dmd/moran.py
+-rw-rw-rw-   0        0        0     2283 2023-02-14 04:42:48.000000 pyl3dmd-0.1.1/pyl3dmd/moreaubroto.py
+-rw-rw-rw-   0        0        0     2413 2023-02-14 04:42:43.000000 pyl3dmd-0.1.1/pyl3dmd/morse.py
+-rw-rw-rw-   0        0        0     9748 2023-07-11 04:00:13.000000 pyl3dmd-0.1.1/pyl3dmd/pyl3dmd.py
+-rw-rw-rw-   0        0        0     2438 2023-02-14 04:43:08.000000 pyl3dmd-0.1.1/pyl3dmd/rdf.py
+-rw-rw-rw-   0        0        0     5408 2023-04-22 16:44:14.000000 pyl3dmd-0.1.1/pyl3dmd/removehydrogenfrommolecule.py
+-rw-rw-rw-   0        0        0    15383 2023-02-14 04:43:20.000000 pyl3dmd-0.1.1/pyl3dmd/topologyconnectivity3Ddescriptors.py
+-rw-rw-rw-   0        0        0     3082 2023-02-14 04:43:37.000000 pyl3dmd-0.1.1/pyl3dmd/whim.py
+drwxrwxrwx   0        0        0        0 2023-07-11 04:02:58.022194 pyl3dmd-0.1.1/pyl3dmd.egg-info/
+-rw-rw-rw-   0        0        0      753 2023-07-11 04:02:57.000000 pyl3dmd-0.1.1/pyl3dmd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      781 2023-07-11 04:02:57.000000 pyl3dmd-0.1.1/pyl3dmd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 04:02:57.000000 pyl3dmd-0.1.1/pyl3dmd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 04:02:57.000000 pyl3dmd-0.1.1/pyl3dmd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 04:02:58.025184 pyl3dmd-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2272 2023-07-11 04:01:15.000000 pyl3dmd-0.1.1/setup.py
```

### Comparing `pyl3dmd-0.1.0/PKG-INFO` & `pyl3dmd-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyl3dmd
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python LAMMPS 3-Dimensional Molecular Dynamics/Descriptors
 Author: Pawan Panwar, Quanpeng Yang, Ashlie Martini
 Author-email: panwarp@msoe.edu
 Keywords: Python,LAMMPS,Molecular Dynamics Simulations,Molecular Descriptors,Machine Learning,MD Simulations,3-Dimensional
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pyl3dmd-0.1.0/pyl3dmd/__init__.py` & `pyl3dmd-0.1.1/pyl3dmd/__init__.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/cpsa.py` & `pyl3dmd-0.1.1/pyl3dmd/cpsa.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/descriptors1set.py` & `pyl3dmd-0.1.1/pyl3dmd/descriptors1set.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/descriptors2set.py` & `pyl3dmd-0.1.1/pyl3dmd/descriptors2set.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/descriptors3set.py` & `pyl3dmd-0.1.1/pyl3dmd/descriptors3set.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/descriptors4set.py` & `pyl3dmd-0.1.1/pyl3dmd/descriptors4set.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,203 +1,207 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu December 10 11:41:02 2022
-
-@author: Pawan Panwar, Quanpeng Yang, Ashlie Martini
-
-
-PyL3dMD: Python LAMMPS 3D Molecular Dynamics/Descriptors
-Copyright (C) 2022  Pawan Panwar, Quanpeng Yang, Ashlie Martini
-
-This file is part of PyL3dMD.
-
-PyL3dMD is free software: you can redistribute it and/or modify 
-it under the terms of the GNU General Public License as published 
-by the Free Software Foundation, either version 3 of the License, 
-or (at your option) any later version.
-
-PyL3dMD is distributed in the hope that it will be useful, but 
-WITHOUT ANY WARRANTY; without even the implied warranty of 
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. 
-See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
- along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
-"""
-
-"""
-This algorithm uses the dot density technique found in:
-
-Shrake, A., and J. A. Rupley. "Environment and Exposure to Solvent
-of Protein Atoms. Lysozyme and Insulin." JMB (1973) 79:351-371.
-
-
-The same approach was used in the Dr. Cao's chemopy package:
-Cao, D. S., Xu, Q. S., Hu, Q. N., & Liang, Y. Z. (2013). ChemoPy: freely
-available python package for computational biology and chemoinformatics. 
-Bioinformatics, 29(8), 1092-1094.
-"""
-
-from math import pi, sqrt
-import numpy as np
-
-inc = pi * (3 - sqrt(5))
-
-def generate_sphere_points(n):
-    """
-    3D coordinates of n points on a sphere using the Golden Section Spiral algorithm
-    """
-    offset = 2.0 / n
-
-    i = np.arange(n, dtype=float)
-
-    phi = i * inc
-    y = i * offset - 1.0 + (offset / 2.0)
-    temp = np.sqrt(1 - y * y)
-    x = np.cos(phi) * temp
-    z = np.sin(phi) * temp
-    points = np.array([x, y, z]).T
-    return points
-
-
-def find_neighbor_indices(xyz, Rc, RadiusProbe, k):
-    """
-    Indices of atoms within probe distance to atom k
-    """
-    dist = np.linalg.norm(xyz - xyz[k], axis=1)
-    temp = Rc[k] + Rc + 2 * RadiusProbe
-    indices = np.arange(xyz.shape[0], dtype=int)
-    return indices[(indices != k) & (dist < temp)]
-
-
-def calculate_asa(xyz, Rc, RadiusProbe, n_sphere_point):
-    """
-    Partial accessible surface areas of the atoms, using the probe and atom radius 
-    which were used todefine the surface
-    """
-    areas = []
-    radius = RadiusProbe + Rc
-    constant = 4.0*pi/n_sphere_point
-    sphere_points = generate_sphere_points(n_sphere_point)
-    areas = np.zeros(xyz.shape[0])
-    for i in range(len(xyz)):
-        neighbor_indices = find_neighbor_indices(xyz, Rc, RadiusProbe, i)
-        r = Rc[neighbor_indices] + RadiusProbe
-        testpoint = sphere_points*radius[i] + xyz[i,:]
-        n_accessible_point = sum([1.0 if np.all(np.linalg.norm(xyz[neighbor_indices] - testpoint[ii], axis=1)>=r) 
-                                  else 0.0 for ii in range(n_sphere_point)])
-        areas[i] = constant * (radius[i]**2) * n_accessible_point 
-    return areas
-
-
-def getcpsadescriptors(xyz, charge, apRc):
-    """
-    Get 3D CPSA descriptors
-        ASA = solvent-accessible surface area
-        MSA = molecular surface area
-        PNSA1 = partial negative area
-        PNSA2 = total charge wighted negative surface area
-        PNSA3 = atom charge weighted negative surface area
-        PPSA1 = partial positive area
-        PPSA2 = total charge wighted positive surface area
-        PPSA3 = atom charge weighted positive surface area
-        DPSA1 = difference in charged partial surface area
-        DPSA2 = total charge wighted difference in charged partial surface area
-        DPSA3 = atom charge weighted difference in charged partial surface area
-        FNSA1 = fractional charged partial negative surface area
-        FNSA2 = total charge wighted fractional charged partial negative surface area
-        FNSA3 = atom charge weighted fractional charged partial negative surface area
-        FPSA1 = fractional charged partial positive surface area
-        FPSA2 = total charge wighted fractional charged partial positive surface area
-        FPSA3 = atom charge weighted fractional charged partial positive surface area
-        WNSA1 = surface weighted charged partial negative surface area 1
-        WNSA2 = surface weighted charged partial negative surface area 2
-        WNSA3 = surface weighted charged partial negative surface area 3
-        WPSA1 = surface weighted charged partial positive surface area 1
-        WPSA2 = surface weighted charged partial positive surface area 2
-        WPSA3 = surface weighted charged partial positive surface area 3
-        TASA = total hydrophobic surface area
-        TPSA = total polar surface area
-        FrTATP = TASA/TPSA
-        RASA = relative hydrophobic surface area
-        RPSA = relative polar surface area
-        RNCS = relative negative charge surface area
-        RPCS = relative positive charge surface area
-    """
-    Rc = apRc * 1.75
-    CPSA = {}
-
-    # molecular surface areas (MSA)
-    RadiusProbe = 0.0
-    n_sphere_point = 500
-    SA = calculate_asa(xyz, Rc, RadiusProbe, n_sphere_point)
-    CPSA['MSA'] = sum(SA)
-
-    # solvent-accessible surface areas (ASA)
-    RadiusProbe = 1.5
-    n_sphere_point = 1500
-    SA = calculate_asa(xyz, Rc, RadiusProbe, n_sphere_point)
-    CPSA['ASA'] = sum(SA)
-
-    # Find indexes of the atoms with negative charge 
-    idxNeg = np.where(charge < 0.0)
-
-    # Find indexes of the atoms with positive charge 
-    idxPos = np.where(charge > 0.0)
-
-    # Find indexes of the atoms with absolute charge < 0.2 and >= 0.2
-    idx1 = np.where(abs(charge) <  0.2)
-    idx2 = np.where(abs(charge) >= 0.2)
-
-    CPSA['PNSA1'] = sum(SA[idxNeg])
-    CPSA['PPSA1'] = sum(SA[idxPos])
-
-    CPSA['PNSA2'] = sum(charge[idxNeg]) * sum(SA[idxNeg])
-    CPSA['PPSA2'] = sum(charge[idxPos]) * sum(SA[idxPos])
-
-    CPSA['PNSA3'] = sum(charge[idxNeg] * SA[idxNeg])
-    CPSA['PPSA3'] = sum(charge[idxPos] * SA[idxPos])
-
-    # difference in charged partial surface areas
-    CPSA['DPSA1'] = CPSA['PPSA1'] - CPSA['PNSA1']
-    CPSA['DPSA2'] = CPSA['PPSA2'] - CPSA['PNSA2']
-    CPSA['DPSA3'] = CPSA['PPSA3'] - CPSA['PNSA3']
-
-    # fractional charged partial surface areas
-    temp = sum(SA)
-    CPSA['FNSA1'] = CPSA['PNSA1'] / temp
-    CPSA['FNSA2'] = CPSA['PNSA2'] / temp
-    CPSA['FNSA3'] = CPSA['PNSA3'] / temp
-    CPSA['FPSA1'] = CPSA['PPSA1'] / temp
-    CPSA['FPSA2'] = CPSA['PPSA2'] / temp
-    CPSA['FPSA3'] = CPSA['PPSA3'] / temp
-
-    # surface weighted charged partial surface areas
-    CPSA['WNSA1'] = CPSA['PNSA1'] * temp / 1000
-    CPSA['WNSA2'] = CPSA['PNSA2'] * temp / 1000
-    CPSA['WNSA3'] = CPSA['PNSA3'] * temp / 1000
-    CPSA['WPSA1'] = CPSA['PPSA1'] * temp / 1000
-    CPSA['WPSA2'] = CPSA['PPSA2'] * temp / 1000
-    CPSA['WPSA3'] = CPSA['PPSA3'] * temp / 1000
-
-    # total hydrophobic (TASA) and polar surface areas (TPSA)
-    CPSA['TASA'] = sum(SA[idx1])
-    CPSA['TPSA'] = sum(SA[idx2])
-
-    # fraction between TASA and TPSA
-    if CPSA['TPSA'] == 0:
-        CPSA['FrTATP'] = 0.0
-    else:
-        CPSA['FrTATP'] = CPSA['TASA'] / CPSA['TPSA']
-
-    # relative hydrophobic surface and polar surface areas
-    CPSA['RASA'] = CPSA['TASA'] / temp
-    CPSA['RPSA'] = CPSA['TPSA'] / temp
-
-    # relative negative and positive charge surface areas
-    idxmincharge = np.where(charge == min(charge))
-    RNCG = min(charge) / sum(charge[idxNeg])
-    RPCG = max(charge) / sum(charge[idxPos])
-    CPSA['RNCS'] = np.mean(SA[idxmincharge]) / RNCG
-    CPSA['RPCS'] = np.mean(SA[idxmincharge]) / RPCG
-
-    return CPSA
+# -*- coding: utf-8 -*-
+"""
+Created on Thu December 10 11:41:02 2022
+
+@author: Pawan Panwar, Quanpeng Yang, Ashlie Martini
+
+
+PyL3dMD: Python LAMMPS 3D Molecular Dynamics/Descriptors
+Copyright (C) 2022  Pawan Panwar, Quanpeng Yang, Ashlie Martini
+
+This file is part of PyL3dMD.
+
+PyL3dMD is free software: you can redistribute it and/or modify 
+it under the terms of the GNU General Public License as published 
+by the Free Software Foundation, either version 3 of the License, 
+or (at your option) any later version.
+
+PyL3dMD is distributed in the hope that it will be useful, but 
+WITHOUT ANY WARRANTY; without even the implied warranty of 
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. 
+See the GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+ along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+"""
+This algorithm uses the dot density technique found in:
+
+Shrake, A., and J. A. Rupley. "Environment and Exposure to Solvent
+of Protein Atoms. Lysozyme and Insulin." JMB (1973) 79:351-371.
+
+
+The same approach was used in the Dr. Cao's chemopy package:
+Cao, D. S., Xu, Q. S., Hu, Q. N., & Liang, Y. Z. (2013). ChemoPy: freely
+available python package for computational biology and chemoinformatics. 
+Bioinformatics, 29(8), 1092-1094.
+"""
+
+from math import pi, sqrt
+import numpy as np
+from numba import njit
+
+inc = pi * (3 - sqrt(5))
+
+@njit
+def generate_sphere_points(n):
+    """
+    3D coordinates of n points on a sphere using the Golden Section Spiral algorithm
+    """
+    offset = 2.0 / n
+    inc = np.pi * (3 - np.sqrt(5))
+    i = np.arange(n)
+    phi = i * inc
+    y = i * offset - 1.0 + (offset / 2.0)
+    temp = np.sqrt(1 - y * y)
+    x = np.cos(phi) * temp
+    z = np.sin(phi) * temp
+    points = np.empty((n, 3))  # Preallocate the array
+    points[:, 0] = x
+    points[:, 1] = y
+    points[:, 2] = z
+    return points
+
+@njit
+def find_neighbor_indices(xyz, Rc, RadiusProbe, k):
+    """
+    Indices of atoms within probe distance to atom k
+    """
+    dist = np.sqrt(np.sum((xyz - xyz[k])**2, axis=1))
+    temp = Rc[k] + Rc + 2 * RadiusProbe
+    indices = np.arange(xyz.shape[0], dtype=np.int64)
+    return indices[(indices != k) & (dist < temp)]
+
+@njit
+def calculate_asa(xyz, Rc, RadiusProbe, n_sphere_point):
+    """
+    Partial accessible surface areas of the atoms, using the probe and atom radius 
+    which were used todefine the surface
+    """
+    areas = []
+    radius = RadiusProbe + Rc
+    constant = 4.0*pi/n_sphere_point
+    sphere_points = generate_sphere_points(n_sphere_point)
+    areas = np.zeros(xyz.shape[0])
+    for i in range(len(xyz)):
+        neighbor_indices = find_neighbor_indices(xyz, Rc, RadiusProbe, i)
+        r = Rc[neighbor_indices] + RadiusProbe
+        testpoint = sphere_points*radius[i] + xyz[i,:]
+        n_accessible_point = sum([1.0 if np.all(np.sqrt(np.sum((xyz[neighbor_indices] - testpoint[ii])**2, axis=1))>=r) 
+                                  else 0.0 for ii in range(n_sphere_point)])
+        areas[i] = constant * (radius[i]**2) * n_accessible_point 
+    return areas
+
+
+def getcpsadescriptors(xyz, charge, apRc):
+    """
+    Get 3D CPSA descriptors
+        ASA = solvent-accessible surface area
+        MSA = molecular surface area
+        PNSA1 = partial negative area
+        PNSA2 = total charge wighted negative surface area
+        PNSA3 = atom charge weighted negative surface area
+        PPSA1 = partial positive area
+        PPSA2 = total charge wighted positive surface area
+        PPSA3 = atom charge weighted positive surface area
+        DPSA1 = difference in charged partial surface area
+        DPSA2 = total charge wighted difference in charged partial surface area
+        DPSA3 = atom charge weighted difference in charged partial surface area
+        FNSA1 = fractional charged partial negative surface area
+        FNSA2 = total charge wighted fractional charged partial negative surface area
+        FNSA3 = atom charge weighted fractional charged partial negative surface area
+        FPSA1 = fractional charged partial positive surface area
+        FPSA2 = total charge wighted fractional charged partial positive surface area
+        FPSA3 = atom charge weighted fractional charged partial positive surface area
+        WNSA1 = surface weighted charged partial negative surface area 1
+        WNSA2 = surface weighted charged partial negative surface area 2
+        WNSA3 = surface weighted charged partial negative surface area 3
+        WPSA1 = surface weighted charged partial positive surface area 1
+        WPSA2 = surface weighted charged partial positive surface area 2
+        WPSA3 = surface weighted charged partial positive surface area 3
+        TASA = total hydrophobic surface area
+        TPSA = total polar surface area
+        FrTATP = TASA/TPSA
+        RASA = relative hydrophobic surface area
+        RPSA = relative polar surface area
+        RNCS = relative negative charge surface area
+        RPCS = relative positive charge surface area
+    """
+    Rc = apRc * 1.75
+    CPSA = {}
+
+    # molecular surface areas (MSA)
+    RadiusProbe = 0.0
+    n_sphere_point = 500
+    SA = calculate_asa(xyz, Rc, RadiusProbe, n_sphere_point)
+    CPSA['MSA'] = sum(SA)
+
+    # solvent-accessible surface areas (ASA)
+    RadiusProbe = 1.5
+    n_sphere_point = 1500
+    SA = calculate_asa(xyz, Rc, RadiusProbe, n_sphere_point)
+    CPSA['ASA'] = sum(SA)
+
+    # Find indexes of the atoms with negative charge 
+    idxNeg = np.where(charge < 0.0)
+
+    # Find indexes of the atoms with positive charge 
+    idxPos = np.where(charge > 0.0)
+
+    # Find indexes of the atoms with absolute charge < 0.2 and >= 0.2
+    idx1 = np.where(abs(charge) <  0.2)
+    idx2 = np.where(abs(charge) >= 0.2)
+
+    CPSA['PNSA1'] = sum(SA[idxNeg])
+    CPSA['PPSA1'] = sum(SA[idxPos])
+
+    CPSA['PNSA2'] = sum(charge[idxNeg]) * sum(SA[idxNeg])
+    CPSA['PPSA2'] = sum(charge[idxPos]) * sum(SA[idxPos])
+
+    CPSA['PNSA3'] = sum(charge[idxNeg] * SA[idxNeg])
+    CPSA['PPSA3'] = sum(charge[idxPos] * SA[idxPos])
+
+    # difference in charged partial surface areas
+    CPSA['DPSA1'] = CPSA['PPSA1'] - CPSA['PNSA1']
+    CPSA['DPSA2'] = CPSA['PPSA2'] - CPSA['PNSA2']
+    CPSA['DPSA3'] = CPSA['PPSA3'] - CPSA['PNSA3']
+
+    # fractional charged partial surface areas
+    temp = sum(SA)
+    CPSA['FNSA1'] = CPSA['PNSA1'] / temp
+    CPSA['FNSA2'] = CPSA['PNSA2'] / temp
+    CPSA['FNSA3'] = CPSA['PNSA3'] / temp
+    CPSA['FPSA1'] = CPSA['PPSA1'] / temp
+    CPSA['FPSA2'] = CPSA['PPSA2'] / temp
+    CPSA['FPSA3'] = CPSA['PPSA3'] / temp
+
+    # surface weighted charged partial surface areas
+    CPSA['WNSA1'] = CPSA['PNSA1'] * temp / 1000
+    CPSA['WNSA2'] = CPSA['PNSA2'] * temp / 1000
+    CPSA['WNSA3'] = CPSA['PNSA3'] * temp / 1000
+    CPSA['WPSA1'] = CPSA['PPSA1'] * temp / 1000
+    CPSA['WPSA2'] = CPSA['PPSA2'] * temp / 1000
+    CPSA['WPSA3'] = CPSA['PPSA3'] * temp / 1000
+
+    # total hydrophobic (TASA) and polar surface areas (TPSA)
+    CPSA['TASA'] = sum(SA[idx1])
+    CPSA['TPSA'] = sum(SA[idx2])
+
+    # fraction between TASA and TPSA
+    if CPSA['TPSA'] == 0:
+        CPSA['FrTATP'] = 0.0
+    else:
+        CPSA['FrTATP'] = CPSA['TASA'] / CPSA['TPSA']
+
+    # relative hydrophobic surface and polar surface areas
+    CPSA['RASA'] = CPSA['TASA'] / temp
+    CPSA['RPSA'] = CPSA['TPSA'] / temp
+
+    # relative negative and positive charge surface areas
+    idxmincharge = np.where(charge == min(charge))
+    RNCG = min(charge) / sum(charge[idxNeg])
+    RPCG = max(charge) / sum(charge[idxPos])
+    CPSA['RNCS'] = np.mean(SA[idxmincharge]) / RNCG
+    CPSA['RPCS'] = np.mean(SA[idxmincharge]) / RPCG
+
+    return CPSA
```

### Comparing `pyl3dmd-0.1.0/pyl3dmd/descriptors5set.py` & `pyl3dmd-0.1.1/pyl3dmd/whim.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 WITHOUT ANY WARRANTY; without even the implied warranty of 
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. 
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
  along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
 """
-
-
 import numpy as np
 
 """
 Calculate Weighted WHIM descriptors
 """
 def calwhimdescriptors(xyz, propertyValue, propertyName):
     nA = xyz.shape[0]
```

### Comparing `pyl3dmd-0.1.0/pyl3dmd/descriptors6set.py` & `pyl3dmd-0.1.1/pyl3dmd/descriptors6set.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/distancedistancematrixdescriptors.py` & `pyl3dmd-0.1.1/pyl3dmd/distancedistancematrixdescriptors.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/geary.py` & `pyl3dmd-0.1.1/pyl3dmd/geary.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/geometricdescriptors.py` & `pyl3dmd-0.1.1/pyl3dmd/geometricdescriptors.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/getadjacencyanddistancematrices.py` & `pyl3dmd-0.1.1/pyl3dmd/getadjacencyanddistancematrices.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/getatomicproperties.py` & `pyl3dmd-0.1.1/pyl3dmd/getatomicproperties.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/getaway.py` & `pyl3dmd-0.1.1/pyl3dmd/getaway.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/getinfofromlammpsdatafile.py` & `pyl3dmd-0.1.1/pyl3dmd/getinfofromlammpsdatafile.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/getinfofromlammpstrajfile.py` & `pyl3dmd-0.1.1/pyl3dmd/getinfofromlammpstrajfile.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/moran.py` & `pyl3dmd-0.1.1/pyl3dmd/moran.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/moreaubroto.py` & `pyl3dmd-0.1.1/pyl3dmd/moreaubroto.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/morse.py` & `pyl3dmd-0.1.1/pyl3dmd/morse.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/pyl3dmd.py` & `pyl3dmd-0.1.1/pyl3dmd/pyl3dmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,39 +90,47 @@
         # GET ALL ATOMIC PROPERTIES
         _, _, _, _, self.eachMolsRc, self.eachMolsm, self.eachMolsV, self.eachMolsEn, self.eachMolsalapha, self.eachMolsIP, self.eachMolsEA = getatomicproperties.getatomicproperties(
             atomMasses, self.eachMolsIdx)
 
         # Get adjacency and distnace matrices
         self.eachMolsAdjMat, self.eachMolsDisMat = getadjacencyanddistancematrices.getadjANDdismatrices(self.eachMolsMass, self.eachMolsBonds)
 
+    # Create a function to save a group to a file
+    def savedata(self, i):
+        fildename = 'Molecule_' + str(i + 1) + '.csv'
+        self.splits[i][1].to_csv(fildename, index=False)
+
+
     def start(self):
         print(f"Started pool with {self.numberofcores} workers.")
         t1 = time.perf_counter()
-        items = []
+        items1 = []
+        items2 = []
         for i in range(self.numMols):
+            items2.append(i)
             for j in range(self.nframes):
-                items.append((i, j))
+                items1.append((i, j))
 
                 # create the process pool
         with mp.Pool(processes=self.numberofcores) as pool:
 
             ans = []
             # call the same function with different data in parallel
-            for result in pool.starmap(self.caldescriptors, items):
+            for result in pool.starmap(self.caldescriptors, items1):
                 # report the value to show progress
                 ans.append(result)
 
         # Convert to dataframe
         df = pd.DataFrame.from_dict(ans)
 
         # split dataframe using gropuby
-        splits = list(df.groupby("molecule"))
-        for i in range(self.numMols):
-            # Dump descriptors of a molecule for all time frames
-            splits[i][1].to_csv('Molecule_' + str(i + 1) + '.csv')
+        self.splits = list(df.groupby("molecule"))
+
+        with mp.Pool(processes=self.numberofcores) as pool:
+            pool.map(self.savedata, items2)
 
         t2 = time.perf_counter()
         print(f'Finished in {t2 - t1} seconds')
 
     def caldensity(self, massBox, volBox):
         """
         simulation calculated density of the fluid [g/cc]
```

### Comparing `pyl3dmd-0.1.0/pyl3dmd/rdf.py` & `pyl3dmd-0.1.1/pyl3dmd/rdf.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/removehydrogenfrommolecule.py` & `pyl3dmd-0.1.1/pyl3dmd/removehydrogenfrommolecule.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/topologyconnectivity3Ddescriptors.py` & `pyl3dmd-0.1.1/pyl3dmd/topologyconnectivity3Ddescriptors.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/pyl3dmd/whim.py` & `pyl3dmd-0.1.1/pyl3dmd/descriptors5set.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,106 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu December 10 11:41:02 2022
-
-@author: Pawan Panwar, Quanpeng Yang, Ashlie Martini
-
-
-PyL3dMD: Python LAMMPS 3D Molecular Dynamics/Descriptors
-Copyright (C) 2022  Pawan Panwar, Quanpeng Yang, Ashlie Martini
-
-This file is part of PyL3dMD.
-
-PyL3dMD is free software: you can redistribute it and/or modify 
-it under the terms of the GNU General Public License as published 
-by the Free Software Foundation, either version 3 of the License, 
-or (at your option) any later version.
-
-PyL3dMD is distributed in the hope that it will be useful, but 
-WITHOUT ANY WARRANTY; without even the implied warranty of 
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. 
-See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
- along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
-"""
-import numpy as np
-
-"""
-Calculate Weighted WHIM descriptors
-"""
-def calwhimdescriptors(xyz, propertyValue, propertyName):
-    nA = xyz.shape[0]
-
-    xyzNew = xyz-np.mean(xyz,axis=0)
-    if propertyName == 'u':
-        weight = np.matrix(np.eye(nA))
-    else:
-        weight = np.matrix(np.diag(propertyValue))
-        
-    temp = xyzNew.T*weight*xyzNew/sum(np.diag(weight))
-    u,s,v = np.linalg.svd(temp)
-
-    L1 = s[0] 
-    L2 = s[1]
-    L3 = s[2]
-    T = sum(s)
-    A = s[0]*s[1] + s[0]*s[2] + s[1]*s[2]    
-    V = A + T + s[0]*s[1]*s[2]
-    P1 = s[0] / sum(s)
-    P2 = s[1] / sum(s)
-    P3 = s[2] / sum(s)
-
-      
-    K = 3.0/4*sum(abs(s/sum(s) - 1/3.0))
-
-    E1 = np.power(s[0],2)*nA/sum(np.power(xyzNew*u[:,0],4)).item()
-    E2 = np.power(s[1],2)*nA/sum(np.power(xyzNew*u[:,1],4)).item()
-    E3 = np.power(s[2],2)*nA/sum(np.power(xyzNew*u[:,2],4)).item()
-    D = E1 + E2 + E3
-
-    WHIM = {}
-    WHIM['WHIM_L1'+propertyName] = L1
-    WHIM['WHIM_L2'+propertyName] = L2
-    WHIM['WHIM_L3'+propertyName] = L3
-    WHIM['WHIM_T'+propertyName] = T
-    WHIM['WHIM_A'+propertyName] = A
-    WHIM['WHIM_V'+propertyName] = V
-    WHIM['WHIM_P1'+propertyName] = P1
-    WHIM['WHIM_P2'+propertyName] = P2
-    WHIM['WHIM_P3'+propertyName] = P3
-    WHIM['WHIM_K'+propertyName] = K
-    WHIM['WHIM_E1'+propertyName] = E1
-    WHIM['WHIM_E2'+propertyName] = E2
-    WHIM['WHIM_E3'+propertyName] = E3
-    WHIM['WHIM_D'+propertyName] = D
-    return WHIM
-
-"""
-Get RDF descriptors for all atomic weights/properties
-"""
-def getwhimdescriptors(*args):
-    """ INPUTS
-    0 ; xyz coordinates of atoms
-    1 : atomic charge (c)
-    2 : atomic mass (m)
-    3 : van der Waals vloume (V)
-    4 : Sanderson electronegativity (En)
-    5 : atomic polarizability in 10e-24 cm3 (P)
-    6 : ionization potential in eV (IP)
-    7 : electron affinity in eV (EA)
-    """
-     
-    propertyNames = ['c','m','V','En','P','IP','EA']
-    
-    WHIM = {}
-    WHIM.update(calwhimdescriptors(args[0], 0, 'u'))
-    for i in range(len(propertyNames)):
-        WHIM.update(calwhimdescriptors(args[0], args[i+1], propertyNames[i]))
+# -*- coding: utf-8 -*-
+"""
+Created on Thu December 10 11:41:02 2022
+
+@author: Pawan Panwar, Quanpeng Yang, Ashlie Martini
+
+
+PyL3dMD: Python LAMMPS 3D Molecular Dynamics/Descriptors
+Copyright (C) 2022  Pawan Panwar, Quanpeng Yang, Ashlie Martini
+
+This file is part of PyL3dMD.
+
+PyL3dMD is free software: you can redistribute it and/or modify 
+it under the terms of the GNU General Public License as published 
+by the Free Software Foundation, either version 3 of the License, 
+or (at your option) any later version.
+
+PyL3dMD is distributed in the hope that it will be useful, but 
+WITHOUT ANY WARRANTY; without even the implied warranty of 
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. 
+See the GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+ along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
+"""
+
+
+import numpy as np
+
+"""
+Calculate Weighted WHIM descriptors
+"""
+def calwhimdescriptors(xyz, propertyValue, propertyName):
+    nA = xyz.shape[0]
+
+    xyzNew = xyz-np.mean(xyz,axis=0)
+    if propertyName == 'u':
+        weight = np.matrix(np.eye(nA))
+    else:
+        weight = np.matrix(np.diag(propertyValue))
+        
+    if sum(np.diag(weight)) == 0:
+        temp = xyzNew.T*weight*xyzNew/sum(np.diag(weight)+1.0)
+    else:
+        temp = xyzNew.T*weight*xyzNew/sum(np.diag(weight))
+    #print(propertyValue)
+    #print(propertyName)
+    #print(temp)
+    u, s, v = np.linalg.svd(temp)
+    L1 = s[0] 
+    L2 = s[1]
+    L3 = s[2]
+    T = sum(s)
+    A = s[0]*s[1] + s[0]*s[2] + s[1]*s[2]    
+    V = A + T + s[0]*s[1]*s[2]
+    P1 = s[0] / sum(s)
+    P2 = s[1] / sum(s)
+    P3 = s[2] / sum(s)
+
+      
+    K = 3.0/4*sum(abs(s/sum(s) - 1/3.0))
+
+    E1 = np.power(s[0],2)*nA/sum(np.power(xyzNew*u[:,0],4)).item()
+    E2 = np.power(s[1],2)*nA/sum(np.power(xyzNew*u[:,1],4)).item()
+    E3 = np.power(s[2],2)*nA/sum(np.power(xyzNew*u[:,2],4)).item()
+    D = E1 + E2 + E3
+
+    WHIM = {}
+    WHIM['WHIM_L1'+propertyName] = L1
+    WHIM['WHIM_L2'+propertyName] = L2
+    WHIM['WHIM_L3'+propertyName] = L3
+    WHIM['WHIM_T'+propertyName] = T
+    WHIM['WHIM_A'+propertyName] = A
+    WHIM['WHIM_V'+propertyName] = V
+    WHIM['WHIM_P1'+propertyName] = P1
+    WHIM['WHIM_P2'+propertyName] = P2
+    WHIM['WHIM_P3'+propertyName] = P3
+    WHIM['WHIM_K'+propertyName] = K
+    WHIM['WHIM_E1'+propertyName] = E1
+    WHIM['WHIM_E2'+propertyName] = E2
+    WHIM['WHIM_E3'+propertyName] = E3
+    WHIM['WHIM_D'+propertyName] = D
+    return WHIM
+
+"""
+Get RDF descriptors for all atomic weights/properties
+"""
+def getwhimdescriptors(*args):
+    """ INPUTS
+    0 ; xyz coordinates of atoms
+    1 : atomic charge (c)
+    2 : atomic mass (m)
+    3 : van der Waals vloume (V)
+    4 : Sanderson electronegativity (En)
+    5 : atomic polarizability in 10e-24 cm3 (P)
+    6 : ionization potential in eV (IP)
+    7 : electron affinity in eV (EA)
+    """
+     
+    propertyNames = ['c','m','V','En','P','IP','EA']
+    
+    WHIM = {}
+    WHIM.update(calwhimdescriptors(args[0], 0, 'u'))
+    for i in range(len(propertyNames)):
+        WHIM.update(calwhimdescriptors(args[0], args[i+1], propertyNames[i]))
     return WHIM
```

### Comparing `pyl3dmd-0.1.0/pyl3dmd.egg-info/PKG-INFO` & `pyl3dmd-0.1.1/pyl3dmd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyl3dmd
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python LAMMPS 3-Dimensional Molecular Dynamics/Descriptors
 Author: Pawan Panwar, Quanpeng Yang, Ashlie Martini
 Author-email: panwarp@msoe.edu
 Keywords: Python,LAMMPS,Molecular Dynamics Simulations,Molecular Descriptors,Machine Learning,MD Simulations,3-Dimensional
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pyl3dmd-0.1.0/pyl3dmd.egg-info/SOURCES.txt` & `pyl3dmd-0.1.1/pyl3dmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.1.0/setup.py` & `pyl3dmd-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
 """
 
 
 
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0' 
+VERSION = '0.1.1' 
 DESCRIPTION = 'Python LAMMPS 3-Dimensional Molecular Dynamics/Descriptors'
 LONG_DESCRIPTION = 'PyL3dMD stands for Python LAMMPS 3-Dimensional Molecular Dynamics/Descriptors, a python package for 3D descriptors calculation'
 
 # setup
 setup(
        # name has to be identical with the name of the folder where the package is
         name="pyl3dmd",
```

