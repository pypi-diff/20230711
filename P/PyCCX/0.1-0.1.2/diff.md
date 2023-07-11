# Comparing `tmp/PyCCX-0.1.tar.gz` & `tmp/PyCCX-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyCCX-0.1.tar", last modified: Sat May  9 13:45:41 2020, max compression
+gzip compressed data, was "PyCCX-0.1.2.tar", last modified: Tue Jul 11 17:32:05 2023, max compression
```

## Comparing `PyCCX-0.1.tar` & `PyCCX-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,36 @@
-drwxrwxr-x   0 lparry    (1000) lparry    (1000)        0 2020-05-09 13:45:41.000000 PyCCX-0.1/
--rw-rw-r--   0 lparry    (1000) lparry    (1000)     1282 2020-04-13 13:52:14.000000 PyCCX-0.1/LICENSE
--rw-rw-r--   0 lparry    (1000) lparry    (1000)       16 2020-04-13 13:52:14.000000 PyCCX-0.1/MANIFEST.in
--rw-rw-r--   0 lparry    (1000) lparry    (1000)     9591 2020-05-09 13:45:41.000000 PyCCX-0.1/PKG-INFO
-drwxrwxr-x   0 lparry    (1000) lparry    (1000)        0 2020-05-09 13:45:41.000000 PyCCX-0.1/PyCCX.egg-info/
--rw-rw-r--   0 lparry    (1000) lparry    (1000)     9591 2020-05-09 13:45:41.000000 PyCCX-0.1/PyCCX.egg-info/PKG-INFO
--rw-rw-r--   0 lparry    (1000) lparry    (1000)      375 2020-05-09 13:45:41.000000 PyCCX-0.1/PyCCX.egg-info/SOURCES.txt
--rw-rw-r--   0 lparry    (1000) lparry    (1000)        1 2020-05-09 13:45:41.000000 PyCCX-0.1/PyCCX.egg-info/dependency_links.txt
--rw-rw-r--   0 lparry    (1000) lparry    (1000)      115 2020-05-09 13:45:41.000000 PyCCX-0.1/PyCCX.egg-info/requires.txt
--rw-rw-r--   0 lparry    (1000) lparry    (1000)        6 2020-05-09 13:45:41.000000 PyCCX-0.1/PyCCX.egg-info/top_level.txt
--rw-rw-r--   0 lparry    (1000) lparry    (1000)     7300 2020-05-09 13:45:32.000000 PyCCX-0.1/README.rst
-drwxrwxr-x   0 lparry    (1000) lparry    (1000)        0 2020-05-09 13:45:41.000000 PyCCX-0.1/pyccx/
--rw-rw-r--   0 lparry    (1000) lparry    (1000)      240 2020-04-13 13:52:14.000000 PyCCX-0.1/pyccx/__init__.py
--rw-rw-r--   0 lparry    (1000) lparry    (1000)    12538 2020-04-25 18:16:19.000000 PyCCX-0.1/pyccx/boundarycondition.py
--rw-rw-r--   0 lparry    (1000) lparry    (1000)    22836 2020-04-25 17:09:44.000000 PyCCX-0.1/pyccx/core.py
--rw-rw-r--   0 lparry    (1000) lparry    (1000)     8803 2020-04-25 17:17:52.000000 PyCCX-0.1/pyccx/loadcase.py
--rw-rw-r--   0 lparry    (1000) lparry    (1000)     9028 2020-04-17 14:14:29.000000 PyCCX-0.1/pyccx/material.py
-drwxrwxr-x   0 lparry    (1000) lparry    (1000)        0 2020-05-09 13:45:41.000000 PyCCX-0.1/pyccx/mesh/
--rw-rw-r--   0 lparry    (1000) lparry    (1000)       77 2020-04-16 19:53:08.000000 PyCCX-0.1/pyccx/mesh/__init__.py
--rw-rw-r--   0 lparry    (1000) lparry    (1000)     3884 2020-04-13 13:52:14.000000 PyCCX-0.1/pyccx/mesh/mesh.py
--rw-rw-r--   0 lparry    (1000) lparry    (1000)    34183 2020-04-21 19:05:51.000000 PyCCX-0.1/pyccx/mesh/mesher.py
--rw-rw-r--   0 lparry    (1000) lparry    (1000)    13922 2020-04-25 19:33:28.000000 PyCCX-0.1/pyccx/results.py
--rw-rw-r--   0 lparry    (1000) lparry    (1000)       21 2020-04-28 08:56:34.000000 PyCCX-0.1/pyccx/version.py
--rw-rw-r--   0 lparry    (1000) lparry    (1000)       38 2020-05-09 13:45:41.000000 PyCCX-0.1/setup.cfg
--rw-rw-r--   0 lparry    (1000) lparry    (1000)     2500 2020-05-09 13:32:04.000000 PyCCX-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:32:05.701904 PyCCX-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-11 17:31:56.000000 PyCCX-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 17:31:56.000000 PyCCX-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-11 17:32:05.701904 PyCCX-0.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:32:05.697904 PyCCX-0.1.2/PyCCX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-11 17:32:05.000000 PyCCX-0.1.2/PyCCX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-11 17:32:05.000000 PyCCX-0.1.2/PyCCX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:32:05.000000 PyCCX-0.1.2/PyCCX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 17:32:05.000000 PyCCX-0.1.2/PyCCX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 17:32:05.000000 PyCCX-0.1.2/PyCCX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-07-11 17:31:56.000000 PyCCX-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:32:05.697904 PyCCX-0.1.2/pyccx/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:32:05.697904 PyCCX-0.1.2/pyccx/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18913 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/analysis/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:32:05.697904 PyCCX-0.1.2/pyccx/bc/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/bc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/bc/boundarycondition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:32:05.697904 PyCCX-0.1.2/pyccx/loadcase/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/loadcase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/loadcase/loadcase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:32:05.697904 PyCCX-0.1.2/pyccx/material/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/material/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/material/material.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:32:05.701904 PyCCX-0.1.2/pyccx/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/mesh/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34182 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/mesh/mesher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:32:05.701904 PyCCX-0.1.2/pyccx/results/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/results/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 17:31:56.000000 PyCCX-0.1.2/pyccx/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:32:05.701904 PyCCX-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-11 17:31:56.000000 PyCCX-0.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyCCX-0.1/LICENSE` & `PyCCX-0.1.2/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020, Luke Parry
+Copyright (c) 2023, Luke Parry
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
```

### Comparing `PyCCX-0.1/PKG-INFO` & `PyCCX-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,191 +1,196 @@
 Metadata-Version: 2.1
 Name: PyCCX
-Version: 0.1
-Summary: Simulation FEA environment for Python built upon Calculix and GMSH
+Version: 0.1.2
+Summary: Simulation and FEA environment for Python built upon Calculix and GMSH
 Home-page: https://github.com/drlukeparry/pyccx
 Author: Luke Parry
 Author-email: dev@lukeparry.uk
-License: UNKNOWN
 Project-URL: Documentation, https://pyccx.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/drylukeparry/pyccx/pyccx/
 Project-URL: Tracker, https://github.com/drlukeparry/pyccx/issues
-Description: PyCCX - Python Library for Calculix
-        =======================================
-        
-        .. image:: https://github.com/drlukeparry/pyccx/workflows/Python%20application/badge.svg
-            :target: https://github.com/drlukeparry/pyccx/actions
-        .. image:: https://readthedocs.org/projects/pyccx/badge/?version=latest
-            :target: https://pyccx.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        .. image:: https://badges.gitter.im/pyccx/community.svg
-            :target: https://gitter.im/pyccx/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
-            :alt: Chat on Gitter
-        
-        Provides a library for creating and running 3D FEA simulations using the opensource Calculix FEA Package.
-        
-        The aims of this project was to provide a simple framework for implemented 3D FEA Analysis using the opensource `Calculix <http://www.calculix.de>`_ solver.
-        The analysis is complimented by use of the recent introduction of the
-        `GMSH-SDK <http://https://gitlab.onelab.info/gmsh/gmsh/api>`_ , an extension to `GMSH <http://gmsh.info/>`_  to provide API bindings for different programming languages
-        by the project authors to provide sophisticated 3D FEA mesh generation outside of the GUI implementation. This project aims to provide an integrated approach for generating full 3D FEA analysis
-        for use in research, development and prototyping in a Python environment. Along with setting up and processing the analysis,
-        convenience functions are included.
-        
-        The inception of this project was a result of finding no native Python/Matlab package available to perfom full non-linear FEA analysis
-        of 3D CAD models in order to prototype a concept related to 3D printing. The project aims to compliment the work of
-        the `PyCalculix project <https://github.com/spacether/pycalculix>`_, which currently is limited to providing capabilities
-        to generate 2D Meshes and FEA analysis for 2D planar structures. The potential in the future is to provide
-        a more generic extensible framework compatible with different opensource and commercial FEA solvers (e.g. Abaqus, Marc, Z88, Elmer).
-        
-        An interface that built upon GMSH was required to avoid the use of the GUI, and the domain specific .geo scripts.
-        `Learn more <http://lukeparry.uk/>`_.
-        
-        Structure
-        ##############
-        
-        PyCCX framework consists of classes for specifying common components on the pre-processing phase, including the following
-        common operations:
-        
-        * Mesh generation
-        * Creating and applying boundary conditions
-        * Creating load cases
-        * Creating and assigning material models
-        * Performing the simulation
-        
-        In addition, a meshing class provides an interface with GMSH for performing the meshing routines and for associating
-        boundary conditions with the elements/faces generated from geometrical CAD entities. The Simulation class assembles the
-        analysis and performs the execution to the Calculix Solver. Results obtained upon completion of the analysis can be processed.
-        Currently the analysis is unit-less, therefore the user should ensure that all constant, material paramters, and geometric
-        lengths are consistent - by default GMSH assumes 'mm' units.
-        
-        Current Features
-        ******************
-        
-        **Meshing:**
-        
-        * Integration with GMSH for generation 3D FEA Meshes (Tet4, Tet10 currently supported)
-        * Merging CAD assemblies using GMSH
-        * Attaching boundary conditions to Geometrical CAD entities
-        
-        **FEA Capabilities:**
-        
-        * **Boundary Conditions** (Acceleration, Convection, Fixed Displacements, Forces, Fluxes, Pressure, Radiation)
-        * **Loadcase Types** (Structural Static, Thermal, Coupled Thermo-Mechanical)
-        * **Materials** (Non-linear Elasto-Plastic Material)
-        
-        **Results Processing:**
-        
-        * Element and Nodal Results can be obtained across timesteps
-        
-        
-        Installation
-        *************
-        Installation is currently supported on Windows, all this further support will be added for
-        Linux environments. PyCCX can be installed along with dependencies for GMSH automatically using.
-        
-        .. code:: bash
-        
-            pip install pyccx
-        
-        
-        Depending on your environment, you will need to install the latest version of Calculix. This can be done through
-        the conda-forge `calculix package <https://anaconda.org/conda-forge/calculix>`_ in the Anaconda distribution,
-        
-        .. code:: bash
-        
-            conda install -c conda-forge calculix
-        
-        
-        or alternatively downloading the package directly. On Windows platforms the path of the executable needs to be initialised before use.
-        
-        .. code:: python
-        
-            from pyccx.core import Simulation
-        
-            # Set the path for Calculix in Windows
-            Simulation.setCalculixPath('Path')
-        
-        
-        Usage
-        ******
-        
-        The following code excerpt shows an example for creating and running a steady state thermal analysis of model using PyCCX
-        of an existing mesh generated using the pyccx.mesh.mesher class.
-        
-        .. code:: python
-        
-            from pyccx.core import DOF, ElementSet, NodeSet, SurfaceSet, Simulation
-            from pyccx.results import ElementResult, NodalResult, ResultProcessor
-            from pyccx.loadcase import  LoadCase, LoadCaseType
-            from pyccx.material import ElastoPlasticMaterial
-        
-            # Set the path for Calculix in Windows
-            Simulation.setCalculixPath('Path')
-        
-            # Create a thermal load case and set the timesettings
-            thermalLoadCase = LoadCase('Thermal Load Case')
-        
-            # Set the loadcase type to thermal - eventually this will be individual analysis classes with defaults
-            thermalLoadCase.setLoadCaseType(LoadCaseType.THERMAL)
-        
-            # Set the thermal analysis to be a steady state simulation
-            thermalLoadCase.isSteadyState = True
-        
-            # Attach the nodal and element result options to each loadcase
-            # Set the nodal and element variables to record in the results (.frd) file
-            nodeThermalPostResult = NodalResult('VolumeNodeSet')
-            nodeThermalPostResult.useNodalTemperatures = True
-        
-            elThermalPostResult = ElementResult('Volume1')
-            elThermalPostResult.useHeatFlux = True
-        
-            # Add the result configurations to the loadcase
-            thermalLoadCase.resultSet = [nodeThermalPostResult, elThermalPostResult]
-        
-            # Set thermal boundary conditions for the loadcase using specific NodeSets
-            thermalLoadCase.boundaryConditions.append(
-                {'type': 'fixed', 'nodes': 'surface6Nodes', 'dof': [DOF.T], 'value': [60]})
-        
-            thermalLoadCase.boundaryConditions.append(
-                {'type': 'fixed', 'nodes': 'surface1Nodes', 'dof': [DOF.T], 'value': [20]})
-        
-            # Material
-            # Add a elastic material and assign it to the volume.
-            # Note ensure that the units correctly correspond with the geometry length scales
-            steelMat = ElastoPlasticMaterial('Steel')
-            steelMat.density = 1.0    # Density
-            steelMat.cp =  1.0        # Specific Heat
-            steelMat.k = 1.0          # Thermal Conductivity
-        
-            analysis.materials.append(steelMat)
-        
-            # Assign the material the volume (use the part name set for geometry)
-            analysis.materialAssignments = [('PartA', 'Steel')]
-        
-            # Set the loadcases used in sequential order
-            analysis.loadCases = [thermalLoadCase]
-        
-            # Analysis Run #
-            # Run the analysis
-            analysis.run()
-        
-            # Open the results  file ('input') is currently the file that is generated by PyCCX
-            results = analysis.results()
-            results.load()
-        
-        
-        The basic usage is split between the meshing facilities provided by GMSH and analysing a problem using the Calculix Solver. Documented
-        examples are provided in `examples <https://github.com/drlukeparry/pyccx/tree/master/examples>`_ .
-        
 Keywords: FEA,Finite Element Analysis,Simulation,Calculix,GMSH
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 Provides-Extra: easy
 Provides-Extra: docs
+License-File: LICENSE
+
+PyCCX - Python Library for Calculix
+=======================================
+
+.. image:: https://github.com/drlukeparry/pyccx/workflows/Python%20application/badge.svg
+    :target: https://github.com/drlukeparry/pyccx/actions
+.. image:: https://readthedocs.org/projects/pyccx/badge/?version=latest
+    :target: https://pyccx.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+.. image:: https://badge.fury.io/py/PyCCX.svg
+    :target: https://badge.fury.io
+.. image:: https://badges.gitter.im/pyccx/community.svg
+    :target: https://gitter.im/pyccx/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
+    :alt: Chat on Gitter
+
+Provides a library for creating and running 3D FEA simulations using the opensource Calculix FEA Package.
+
+The aims of this project was to provide a simple framework for implemented 3D FEA Analysis using the opensource `Calculix <http://www.calculix.de>`_ solver.
+The analysis is complimented by use of the recent introduction of the
+`GMSH-SDK <http://https://gitlab.onelab.info/gmsh/gmsh/api>`_ , an extension to `GMSH <http://gmsh.info/>`_  to provide API bindings for different programming languages
+by the project authors to provide sophisticated 3D FEA mesh generation outside of the GUI implementation. This project aims to provide an integrated approach for generating full 3D FEA analysis
+for use in research, development and prototyping in a Python environment. Along with setting up and processing the analysis,
+convenience functions are included.
+
+The inception of this project was a result of finding no native Python/Matlab package available to perfom full non-linear FEA analysis
+of 3D CAD models in order to prototype a concept related to 3D printing. The project aims to compliment the work of
+the `PyCalculix project <https://github.com/spacether/pycalculix>`_, which currently is limited to providing capabilities
+to generate 2D Meshes and FEA analysis for 2D planar structures. The potential in the future is to provide
+a more generic extensible framework compatible with different opensource and commercial FEA solvers (e.g. Abaqus, Marc, Z88, Elmer).
+
+An interface that built upon GMSH was required to avoid the use of the GUI, and the domain specific .geo scripts.
+`Learn more <http://lukeparry.uk/>`_.
+
+Structure
+##############
+
+PyCCX framework consists of classes for specifying common components on the pre-processing phase, including the following
+common operations:
+
+* Mesh generation
+* Creating and applying boundary conditions
+* Creating load cases
+* Creating and assigning material models
+* Performing the simulation
+
+In addition, a meshing class provides an interface with GMSH for performing the meshing routines and for associating
+boundary conditions with the elements/faces generated from geometrical CAD entities. The Simulation class assembles the
+analysis and performs the execution to the Calculix Solver. Results obtained upon completion of the analysis can be processed.
+Currently the analysis is unit-less, therefore the user should ensure that all constant, material paramters, and geometric
+lengths are consistent - by default GMSH assumes 'mm' units.
+
+Current Features
+******************
+
+**Meshing:**
+
+* Integration with GMSH for generation 3D FEA Meshes (Tet4, Tet10 currently supported)
+* Merging CAD assemblies using GMSH
+* Attaching boundary conditions to Geometrical CAD entities
+
+**FEA Capabilities:**
+
+* **Boundary Conditions** (Acceleration, Convection, Fixed Displacements, Forces, Fluxes, Pressure, Radiation)
+* **Loadcase Types** (Structural Static, Thermal, Coupled Thermo-Mechanical)
+* **Materials** (Non-linear Elasto-Plastic Material)
+
+**Results Processing:**
+
+* Element and Nodal Results can be obtained across timesteps
+
+
+Installation
+*************
+Installation is currently supported on Windows, all this further support will be added for
+Linux environments. PyCCX can be installed along with dependencies for GMSH automatically using.
+
+.. code:: bash
+
+    pip install pyccx
+
+
+Depending on your environment, you will need to install the latest version of Calculix. This can be done through
+the conda-forge `calculix package <https://anaconda.org/conda-forge/calculix>`_ in the Anaconda distribution,
+
+.. code:: bash
+
+    conda install -c conda-forge calculix
+
+
+or alternatively downloading the package directly. On Windows platforms the path of the executable needs to be initialised before use.
+
+.. code:: python
+
+    from pyccx.core import Simulation
+
+    # Set the path for Calculix in Windows
+    Simulation.setCalculixPath('Path')
+
+
+Usage
+******
+
+The following code excerpt shows an example for creating and running a steady state thermal analysis of model using PyCCX
+of an existing mesh generated using the pyccx.mesh.mesher class.
+
+.. code:: python
+
+    from pyccx.core import DOF, ElementSet, NodeSet, SurfaceSet, Simulation
+    from pyccx.results import ElementResult, NodalResult, ResultProcessor
+    from pyccx.loadcase import  LoadCase, LoadCaseType
+    from pyccx.material import ElastoPlasticMaterial
+
+    # Set the path for Calculix in Windows
+    Simulation.setCalculixPath('Path')
+
+    # Create a thermal load case and set the timesettings
+    thermalLoadCase = LoadCase('Thermal Load Case')
+
+    # Set the loadcase type to thermal - eventually this will be individual analysis classes with defaults
+    thermalLoadCase.setLoadCaseType(LoadCaseType.THERMAL)
+
+    # Set the thermal analysis to be a steady state simulation
+    thermalLoadCase.isSteadyState = True
+
+    # Attach the nodal and element result options to each loadcase
+    # Set the nodal and element variables to record in the results (.frd) file
+    nodeThermalPostResult = NodalResult('VolumeNodeSet')
+    nodeThermalPostResult.useNodalTemperatures = True
+
+    elThermalPostResult = ElementResult('Volume1')
+    elThermalPostResult.useHeatFlux = True
+
+    # Add the result configurations to the loadcase
+    thermalLoadCase.resultSet = [nodeThermalPostResult, elThermalPostResult]
+
+    # Set thermal boundary conditions for the loadcase using specific NodeSets
+    thermalLoadCase.boundaryConditions.append(
+        {'type': 'fixed', 'nodes': 'surface6Nodes', 'dof': [DOF.T], 'value': [60]})
+
+    thermalLoadCase.boundaryConditions.append(
+        {'type': 'fixed', 'nodes': 'surface1Nodes', 'dof': [DOF.T], 'value': [20]})
+
+    # Material
+    # Add a elastic material and assign it to the volume.
+    # Note ensure that the units correctly correspond with the geometry length scales
+    steelMat = ElastoPlasticMaterial('Steel')
+    steelMat.density = 1.0    # Density
+    steelMat.cp =  1.0        # Specific Heat
+    steelMat.k = 1.0          # Thermal Conductivity
+
+    analysis.materials.append(steelMat)
+
+    # Assign the material the volume (use the part name set for geometry)
+    analysis.materialAssignments = [('PartA', 'Steel')]
+
+    # Set the loadcases used in sequential order
+    analysis.loadCases = [thermalLoadCase]
+
+    # Analysis Run #
+    # Run the analysis
+    analysis.run()
+
+    # Open the results  file ('input') is currently the file that is generated by PyCCX
+    results = analysis.results()
+    results.load()
+
+
+The basic usage is split between the meshing facilities provided by GMSH and analysing a problem using the Calculix Solver. Documented
+examples are provided in `examples <https://github.com/drlukeparry/pyccx/tree/master/examples>`_ .
```

### Comparing `PyCCX-0.1/PyCCX.egg-info/PKG-INFO` & `PyCCX-0.1.2/PyCCX.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,191 +1,196 @@
 Metadata-Version: 2.1
 Name: PyCCX
-Version: 0.1
-Summary: Simulation FEA environment for Python built upon Calculix and GMSH
+Version: 0.1.2
+Summary: Simulation and FEA environment for Python built upon Calculix and GMSH
 Home-page: https://github.com/drlukeparry/pyccx
 Author: Luke Parry
 Author-email: dev@lukeparry.uk
-License: UNKNOWN
 Project-URL: Documentation, https://pyccx.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/drylukeparry/pyccx/pyccx/
 Project-URL: Tracker, https://github.com/drlukeparry/pyccx/issues
-Description: PyCCX - Python Library for Calculix
-        =======================================
-        
-        .. image:: https://github.com/drlukeparry/pyccx/workflows/Python%20application/badge.svg
-            :target: https://github.com/drlukeparry/pyccx/actions
-        .. image:: https://readthedocs.org/projects/pyccx/badge/?version=latest
-            :target: https://pyccx.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        .. image:: https://badges.gitter.im/pyccx/community.svg
-            :target: https://gitter.im/pyccx/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
-            :alt: Chat on Gitter
-        
-        Provides a library for creating and running 3D FEA simulations using the opensource Calculix FEA Package.
-        
-        The aims of this project was to provide a simple framework for implemented 3D FEA Analysis using the opensource `Calculix <http://www.calculix.de>`_ solver.
-        The analysis is complimented by use of the recent introduction of the
-        `GMSH-SDK <http://https://gitlab.onelab.info/gmsh/gmsh/api>`_ , an extension to `GMSH <http://gmsh.info/>`_  to provide API bindings for different programming languages
-        by the project authors to provide sophisticated 3D FEA mesh generation outside of the GUI implementation. This project aims to provide an integrated approach for generating full 3D FEA analysis
-        for use in research, development and prototyping in a Python environment. Along with setting up and processing the analysis,
-        convenience functions are included.
-        
-        The inception of this project was a result of finding no native Python/Matlab package available to perfom full non-linear FEA analysis
-        of 3D CAD models in order to prototype a concept related to 3D printing. The project aims to compliment the work of
-        the `PyCalculix project <https://github.com/spacether/pycalculix>`_, which currently is limited to providing capabilities
-        to generate 2D Meshes and FEA analysis for 2D planar structures. The potential in the future is to provide
-        a more generic extensible framework compatible with different opensource and commercial FEA solvers (e.g. Abaqus, Marc, Z88, Elmer).
-        
-        An interface that built upon GMSH was required to avoid the use of the GUI, and the domain specific .geo scripts.
-        `Learn more <http://lukeparry.uk/>`_.
-        
-        Structure
-        ##############
-        
-        PyCCX framework consists of classes for specifying common components on the pre-processing phase, including the following
-        common operations:
-        
-        * Mesh generation
-        * Creating and applying boundary conditions
-        * Creating load cases
-        * Creating and assigning material models
-        * Performing the simulation
-        
-        In addition, a meshing class provides an interface with GMSH for performing the meshing routines and for associating
-        boundary conditions with the elements/faces generated from geometrical CAD entities. The Simulation class assembles the
-        analysis and performs the execution to the Calculix Solver. Results obtained upon completion of the analysis can be processed.
-        Currently the analysis is unit-less, therefore the user should ensure that all constant, material paramters, and geometric
-        lengths are consistent - by default GMSH assumes 'mm' units.
-        
-        Current Features
-        ******************
-        
-        **Meshing:**
-        
-        * Integration with GMSH for generation 3D FEA Meshes (Tet4, Tet10 currently supported)
-        * Merging CAD assemblies using GMSH
-        * Attaching boundary conditions to Geometrical CAD entities
-        
-        **FEA Capabilities:**
-        
-        * **Boundary Conditions** (Acceleration, Convection, Fixed Displacements, Forces, Fluxes, Pressure, Radiation)
-        * **Loadcase Types** (Structural Static, Thermal, Coupled Thermo-Mechanical)
-        * **Materials** (Non-linear Elasto-Plastic Material)
-        
-        **Results Processing:**
-        
-        * Element and Nodal Results can be obtained across timesteps
-        
-        
-        Installation
-        *************
-        Installation is currently supported on Windows, all this further support will be added for
-        Linux environments. PyCCX can be installed along with dependencies for GMSH automatically using.
-        
-        .. code:: bash
-        
-            pip install pyccx
-        
-        
-        Depending on your environment, you will need to install the latest version of Calculix. This can be done through
-        the conda-forge `calculix package <https://anaconda.org/conda-forge/calculix>`_ in the Anaconda distribution,
-        
-        .. code:: bash
-        
-            conda install -c conda-forge calculix
-        
-        
-        or alternatively downloading the package directly. On Windows platforms the path of the executable needs to be initialised before use.
-        
-        .. code:: python
-        
-            from pyccx.core import Simulation
-        
-            # Set the path for Calculix in Windows
-            Simulation.setCalculixPath('Path')
-        
-        
-        Usage
-        ******
-        
-        The following code excerpt shows an example for creating and running a steady state thermal analysis of model using PyCCX
-        of an existing mesh generated using the pyccx.mesh.mesher class.
-        
-        .. code:: python
-        
-            from pyccx.core import DOF, ElementSet, NodeSet, SurfaceSet, Simulation
-            from pyccx.results import ElementResult, NodalResult, ResultProcessor
-            from pyccx.loadcase import  LoadCase, LoadCaseType
-            from pyccx.material import ElastoPlasticMaterial
-        
-            # Set the path for Calculix in Windows
-            Simulation.setCalculixPath('Path')
-        
-            # Create a thermal load case and set the timesettings
-            thermalLoadCase = LoadCase('Thermal Load Case')
-        
-            # Set the loadcase type to thermal - eventually this will be individual analysis classes with defaults
-            thermalLoadCase.setLoadCaseType(LoadCaseType.THERMAL)
-        
-            # Set the thermal analysis to be a steady state simulation
-            thermalLoadCase.isSteadyState = True
-        
-            # Attach the nodal and element result options to each loadcase
-            # Set the nodal and element variables to record in the results (.frd) file
-            nodeThermalPostResult = NodalResult('VolumeNodeSet')
-            nodeThermalPostResult.useNodalTemperatures = True
-        
-            elThermalPostResult = ElementResult('Volume1')
-            elThermalPostResult.useHeatFlux = True
-        
-            # Add the result configurations to the loadcase
-            thermalLoadCase.resultSet = [nodeThermalPostResult, elThermalPostResult]
-        
-            # Set thermal boundary conditions for the loadcase using specific NodeSets
-            thermalLoadCase.boundaryConditions.append(
-                {'type': 'fixed', 'nodes': 'surface6Nodes', 'dof': [DOF.T], 'value': [60]})
-        
-            thermalLoadCase.boundaryConditions.append(
-                {'type': 'fixed', 'nodes': 'surface1Nodes', 'dof': [DOF.T], 'value': [20]})
-        
-            # Material
-            # Add a elastic material and assign it to the volume.
-            # Note ensure that the units correctly correspond with the geometry length scales
-            steelMat = ElastoPlasticMaterial('Steel')
-            steelMat.density = 1.0    # Density
-            steelMat.cp =  1.0        # Specific Heat
-            steelMat.k = 1.0          # Thermal Conductivity
-        
-            analysis.materials.append(steelMat)
-        
-            # Assign the material the volume (use the part name set for geometry)
-            analysis.materialAssignments = [('PartA', 'Steel')]
-        
-            # Set the loadcases used in sequential order
-            analysis.loadCases = [thermalLoadCase]
-        
-            # Analysis Run #
-            # Run the analysis
-            analysis.run()
-        
-            # Open the results  file ('input') is currently the file that is generated by PyCCX
-            results = analysis.results()
-            results.load()
-        
-        
-        The basic usage is split between the meshing facilities provided by GMSH and analysing a problem using the Calculix Solver. Documented
-        examples are provided in `examples <https://github.com/drlukeparry/pyccx/tree/master/examples>`_ .
-        
 Keywords: FEA,Finite Element Analysis,Simulation,Calculix,GMSH
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 Provides-Extra: easy
 Provides-Extra: docs
+License-File: LICENSE
+
+PyCCX - Python Library for Calculix
+=======================================
+
+.. image:: https://github.com/drlukeparry/pyccx/workflows/Python%20application/badge.svg
+    :target: https://github.com/drlukeparry/pyccx/actions
+.. image:: https://readthedocs.org/projects/pyccx/badge/?version=latest
+    :target: https://pyccx.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+.. image:: https://badge.fury.io/py/PyCCX.svg
+    :target: https://badge.fury.io
+.. image:: https://badges.gitter.im/pyccx/community.svg
+    :target: https://gitter.im/pyccx/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
+    :alt: Chat on Gitter
+
+Provides a library for creating and running 3D FEA simulations using the opensource Calculix FEA Package.
+
+The aims of this project was to provide a simple framework for implemented 3D FEA Analysis using the opensource `Calculix <http://www.calculix.de>`_ solver.
+The analysis is complimented by use of the recent introduction of the
+`GMSH-SDK <http://https://gitlab.onelab.info/gmsh/gmsh/api>`_ , an extension to `GMSH <http://gmsh.info/>`_  to provide API bindings for different programming languages
+by the project authors to provide sophisticated 3D FEA mesh generation outside of the GUI implementation. This project aims to provide an integrated approach for generating full 3D FEA analysis
+for use in research, development and prototyping in a Python environment. Along with setting up and processing the analysis,
+convenience functions are included.
+
+The inception of this project was a result of finding no native Python/Matlab package available to perfom full non-linear FEA analysis
+of 3D CAD models in order to prototype a concept related to 3D printing. The project aims to compliment the work of
+the `PyCalculix project <https://github.com/spacether/pycalculix>`_, which currently is limited to providing capabilities
+to generate 2D Meshes and FEA analysis for 2D planar structures. The potential in the future is to provide
+a more generic extensible framework compatible with different opensource and commercial FEA solvers (e.g. Abaqus, Marc, Z88, Elmer).
+
+An interface that built upon GMSH was required to avoid the use of the GUI, and the domain specific .geo scripts.
+`Learn more <http://lukeparry.uk/>`_.
+
+Structure
+##############
+
+PyCCX framework consists of classes for specifying common components on the pre-processing phase, including the following
+common operations:
+
+* Mesh generation
+* Creating and applying boundary conditions
+* Creating load cases
+* Creating and assigning material models
+* Performing the simulation
+
+In addition, a meshing class provides an interface with GMSH for performing the meshing routines and for associating
+boundary conditions with the elements/faces generated from geometrical CAD entities. The Simulation class assembles the
+analysis and performs the execution to the Calculix Solver. Results obtained upon completion of the analysis can be processed.
+Currently the analysis is unit-less, therefore the user should ensure that all constant, material paramters, and geometric
+lengths are consistent - by default GMSH assumes 'mm' units.
+
+Current Features
+******************
+
+**Meshing:**
+
+* Integration with GMSH for generation 3D FEA Meshes (Tet4, Tet10 currently supported)
+* Merging CAD assemblies using GMSH
+* Attaching boundary conditions to Geometrical CAD entities
+
+**FEA Capabilities:**
+
+* **Boundary Conditions** (Acceleration, Convection, Fixed Displacements, Forces, Fluxes, Pressure, Radiation)
+* **Loadcase Types** (Structural Static, Thermal, Coupled Thermo-Mechanical)
+* **Materials** (Non-linear Elasto-Plastic Material)
+
+**Results Processing:**
+
+* Element and Nodal Results can be obtained across timesteps
+
+
+Installation
+*************
+Installation is currently supported on Windows, all this further support will be added for
+Linux environments. PyCCX can be installed along with dependencies for GMSH automatically using.
+
+.. code:: bash
+
+    pip install pyccx
+
+
+Depending on your environment, you will need to install the latest version of Calculix. This can be done through
+the conda-forge `calculix package <https://anaconda.org/conda-forge/calculix>`_ in the Anaconda distribution,
+
+.. code:: bash
+
+    conda install -c conda-forge calculix
+
+
+or alternatively downloading the package directly. On Windows platforms the path of the executable needs to be initialised before use.
+
+.. code:: python
+
+    from pyccx.core import Simulation
+
+    # Set the path for Calculix in Windows
+    Simulation.setCalculixPath('Path')
+
+
+Usage
+******
+
+The following code excerpt shows an example for creating and running a steady state thermal analysis of model using PyCCX
+of an existing mesh generated using the pyccx.mesh.mesher class.
+
+.. code:: python
+
+    from pyccx.core import DOF, ElementSet, NodeSet, SurfaceSet, Simulation
+    from pyccx.results import ElementResult, NodalResult, ResultProcessor
+    from pyccx.loadcase import  LoadCase, LoadCaseType
+    from pyccx.material import ElastoPlasticMaterial
+
+    # Set the path for Calculix in Windows
+    Simulation.setCalculixPath('Path')
+
+    # Create a thermal load case and set the timesettings
+    thermalLoadCase = LoadCase('Thermal Load Case')
+
+    # Set the loadcase type to thermal - eventually this will be individual analysis classes with defaults
+    thermalLoadCase.setLoadCaseType(LoadCaseType.THERMAL)
+
+    # Set the thermal analysis to be a steady state simulation
+    thermalLoadCase.isSteadyState = True
+
+    # Attach the nodal and element result options to each loadcase
+    # Set the nodal and element variables to record in the results (.frd) file
+    nodeThermalPostResult = NodalResult('VolumeNodeSet')
+    nodeThermalPostResult.useNodalTemperatures = True
+
+    elThermalPostResult = ElementResult('Volume1')
+    elThermalPostResult.useHeatFlux = True
+
+    # Add the result configurations to the loadcase
+    thermalLoadCase.resultSet = [nodeThermalPostResult, elThermalPostResult]
+
+    # Set thermal boundary conditions for the loadcase using specific NodeSets
+    thermalLoadCase.boundaryConditions.append(
+        {'type': 'fixed', 'nodes': 'surface6Nodes', 'dof': [DOF.T], 'value': [60]})
+
+    thermalLoadCase.boundaryConditions.append(
+        {'type': 'fixed', 'nodes': 'surface1Nodes', 'dof': [DOF.T], 'value': [20]})
+
+    # Material
+    # Add a elastic material and assign it to the volume.
+    # Note ensure that the units correctly correspond with the geometry length scales
+    steelMat = ElastoPlasticMaterial('Steel')
+    steelMat.density = 1.0    # Density
+    steelMat.cp =  1.0        # Specific Heat
+    steelMat.k = 1.0          # Thermal Conductivity
+
+    analysis.materials.append(steelMat)
+
+    # Assign the material the volume (use the part name set for geometry)
+    analysis.materialAssignments = [('PartA', 'Steel')]
+
+    # Set the loadcases used in sequential order
+    analysis.loadCases = [thermalLoadCase]
+
+    # Analysis Run #
+    # Run the analysis
+    analysis.run()
+
+    # Open the results  file ('input') is currently the file that is generated by PyCCX
+    results = analysis.results()
+    results.load()
+
+
+The basic usage is split between the meshing facilities provided by GMSH and analysing a problem using the Calculix Solver. Documented
+examples are provided in `examples <https://github.com/drlukeparry/pyccx/tree/master/examples>`_ .
```

### Comparing `PyCCX-0.1/README.rst` & `PyCCX-0.1.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 =======================================
 
 .. image:: https://github.com/drlukeparry/pyccx/workflows/Python%20application/badge.svg
     :target: https://github.com/drlukeparry/pyccx/actions
 .. image:: https://readthedocs.org/projects/pyccx/badge/?version=latest
     :target: https://pyccx.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
+.. image:: https://badge.fury.io/py/PyCCX.svg
+    :target: https://badge.fury.io
 .. image:: https://badges.gitter.im/pyccx/community.svg
     :target: https://gitter.im/pyccx/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
     :alt: Chat on Gitter
 
 Provides a library for creating and running 3D FEA simulations using the opensource Calculix FEA Package.
 
 The aims of this project was to provide a simple framework for implemented 3D FEA Analysis using the opensource `Calculix <http://www.calculix.de>`_ solver.
```

### Comparing `PyCCX-0.1/pyccx/boundarycondition.py` & `PyCCX-0.1.2/pyccx/bc/boundarycondition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import abc
 from enum import Enum, Flag, auto
 from typing import Any, List, Tuple
 
 import numpy as np
 
-from .core import ElementSet, NodeSet, SurfaceSet, DOF
+from ..core import ElementSet, NodeSet, SurfaceSet, DOF
 
 
 class BoundaryConditionType(Flag):
     """
     Boundary condition type specifies which type of analyses the boundary condition may be applied to. Flags may be mixed
-    when coupled analyses are performed (e.g.  thermomechanical analysis: STRUCTURAL | THERMAL)
+    when coupled analyses are performed (e.g.  thermo-mechanical analysis: STRUCTURAL | THERMAL)
     """
 
     ANY = auto()
     """ Boundary condition can be used in any analysis"""
 
     STRUCTURAL = auto()
     """ Boundary condition can be used in a structural analysis"""
@@ -81,15 +81,15 @@
     """
 
     def __init__(self, target, h: float = 0.0, TAmbient: float = 0.0):
 
         self.h = h
         self.T_amb = TAmbient
 
-        if not isinstance(self.target, SurfaceSet):
+        if not isinstance(target, SurfaceSet):
             raise ValueError('A SurfaceSet must be used for a Film Boundary Condition')
 
         super().__init__(target)
 
     def type(self) -> BoundaryConditionType:
         return BoundaryConditionType.THERMAL
 
@@ -133,15 +133,15 @@
     coupled thermo-mechanical analyses.
     """
 
     def __init__(self, target, flux: float = 0.0):
 
         self._flux = flux
 
-        if not isinstance(self.target, SurfaceSet):
+        if not isinstance(target, SurfaceSet):
             raise ValueError('A SurfaceSet must be used for a Heat Flux Boundary Condition')
 
         super().__init__(target)
 
     def type(self) -> BoundaryConditionType:
         return BoundaryConditionType.THERMAL
 
@@ -168,24 +168,24 @@
 
 
 class Radiation(BoundaryCondition):
     """
     The radiation boundary condition applies Black-body radiation using the Stefan-Boltzmann Law,
     :math:`q_{rad} = \\epsilon \\sigma_b\\left(T-T_{amb}\\right)^4`, which is imposed on the faces of
     boundaries elements (correctly ordered according to Calculix's requirements). Ensure that the Stefan-Boltzmann constant :math:
-    `\\sigma_b`, has consistent units, which is set in the :attribute:`~pyccx.core.Simulation.SIGMAB`. This BC may be used in thermal and
+    `\\sigma_b`, has consistent units, which is set in the :attr:`~pyccx.analysis.Simulation.SIGMAB`. This BC may be used in thermal and
     coupled thermo-mechanical analyses.
     """
 
     def __init__(self, target, epsilon=1.0, TAmbient: float = 0.0):
 
         self.T_amb = TAmbient
         self._epsilon = epsilon
 
-        if not isinstance(self.target, SurfaceSet):
+        if not isinstance(target, SurfaceSet):
             raise ValueError('A SurfaceSet must be used for a Radiation Boundary Condition')
 
         super().__init__(target)
 
     def type(self) -> BoundaryConditionType:
         return BoundaryConditionType.THERMAL
 
@@ -230,17 +230,17 @@
     """
 
     def __init__(self, target: Any, dof: List[DOF] = [], values=None):
 
         if not isinstance(target, NodeSet):
             raise ValueError('The target for a Fixed Boundary Condition must be a NodeSet')
 
-        for d in dof:
-            if not d in DOF:
-                raise ValueError('Degree of freedom must be specified')
+        # for d in dof:
+        #     if not d in DOF:
+        #         raise ValueError('Degree of freedom must be specified')
 
         self._dof = dof
         self._values = values
 
         super().__init__(target)
 
     def type(self) -> BoundaryConditionType:
@@ -276,15 +276,15 @@
 
         if len(self.dof) != len(self._values):
             raise ValueError('DOF and Prescribed DOF must have a matching size')
 
         # 1-3 U, 4-6, rotational DOF, 11 = Temp
         for i in range(len(self._dof)):
             if self._values:
-                # inhomogenous boundary conditions
+                # Inhomogeneous boundary conditions
                 bCondStr += '{:s},{:d},, {:e}\n'.format(nodesetName, self._dof[i], self._values[i])
             else:
                 # Fixed boundary condition
                 bCondStr += '{:s},{:d}\n'.format(nodesetName, self._dof[i])
 
         return bCondStr
 
@@ -295,14 +295,17 @@
     analysis. This is provided as magnitude, direction of the acceleration on the body.
     """
 
     def __init__(self, target, dir=None, mag=1.0):
 
         self.mag = 1.0
 
+        if not isinstance(target, NodeSet) or not isinstance(target, ElementSet):
+            raise ValueError('The target for an Acceleration BC should be a node or element set.')
+
         if dir:
             self.dir = dir
         else:
             self.dir = np.array([0.0, 0.0, 1.0])
 
         super().__init__(target)
 
@@ -331,15 +334,15 @@
     def magnitude(self, magVal: float) -> None:
         from numpy import linalg
         self.mag = magVal
 
     @property
     def direction(self) -> np.ndarray:
         """
-        The acceleration direction (noramlised vector)
+        The acceleration direction (normalised vector)
         """
         return self.dir
 
     @direction.setter
     def direction(self, v: float) -> None:
         from numpy import linalg
         self.dir = v / linalg.norm(v)
@@ -356,15 +359,15 @@
     """
 
     def __init__(self, target, magnitude: float = 0.0):
 
         self.mag = magnitude
 
         if not isinstance(target, SurfaceSet):
-            raise ValueError('A surface set must be assigned to a Presure boundary condition.')
+            raise ValueError('A surface set must be assigned to a Pressure boundary condition.')
 
         super().__init__(target)
 
     def type(self) -> BoundaryConditionType:
         return BoundaryConditionType.STRUCTURAL
 
     @property
```

### Comparing `PyCCX-0.1/pyccx/core.py` & `PyCCX-0.1.2/pyccx/analysis/analysis.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-# -*- coding: utf-8 -*-
-
-
 import re  # used to get info from frd file
 import os
 import sys
 import subprocess  # used to check ccx version
 from enum import Enum, auto
 from typing import List, Tuple, Type
 import logging
 
-from .boundarycondition import BoundaryCondition
-from .loadcase import LoadCase
-from .material import Material
-from .mesh import Mesher
-from .results import ElementResult, NodalResult, ResultProcessor
-
-import numpy as np
+from ..bc import BoundaryCondition
+from ..core import MeshSet, ElementSet, SurfaceSet, NodeSet, Connector
+from ..loadcase import LoadCase
+from ..material import Material
+from ..mesh import Mesher
+from ..results import ElementResult, NodalResult, ResultProcessor
 
 
 class AnalysisError(Exception):
     """Exception raised for errors generated during the analysis
 
     Attributes:
         expression -- input expression in which the error occurred
@@ -28,179 +24,22 @@
 
     def __init__(self, expression, message):
         self.expression = expression
         self.message = message
 
 
 class AnalysisType(Enum):
+    """
+    The analysis types available for use.
+    """
     STRUCTURAL = auto()
     THERMAL = auto()
     FLUID = auto()
 
 
-class MeshSet:
-
-    def __init__(self, name):
-        self._name = name
-
-    @property
-    def name(self) -> str:
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        self._name = name
-
-
-class NodeSet(MeshSet):
-    """
-     An node set is basic entity for storing node set lists. The set remains constant without any dynamic referencing
-     to any underlying geometric entities.
-     """
-    def __init__(self, name, nodes):
-        super().__init__(name)
-        self._nodes = nodes
-
-    @property
-    def nodes(self):
-        """
-        Nodes contains the list of Node IDs
-        """
-        return self._nodes
-
-    @nodes.setter
-    def nodes(self, nodes):
-        self._nodes = nodes
-
-    def writeInput(self) -> str:
-        out = '*NSET,NSET={:s}\n'.format(self.name)
-        out += np.array2string(self.nodes, precision=2, separator=', ', threshold=9999999999)[1:-1]
-        return out
-
-
-class ElementSet(MeshSet):
-    """
-    An element set is basic entity for storing element set lists.The set remains constant without any dynamic referencing
-     to any underlying geometric entities.
-    """
-    def __init__(self, name, els):
-        super().__init__(name)
-        self._els = els
-
-    @property
-    def els(self):
-        """
-        Elements contains the list of Node IDs
-        """
-        return self._els
-
-    @els.setter
-    def els(self, elements):
-        self._els = elements
-
-    def writeInput(self) -> str:
-
-        out = '*ELSET,ELSET={:s\n}'.format(self.name)
-        out += np.array2string(self.els, precision=2, separator=', ', threshold=9999999999)[1:-1]
-        return out
-
-
-class SurfaceSet(MeshSet):
-    """
-    A surface-set set is basic entity for storing element face lists, typically for setting directional fluxes onto
-    surface elements based on the element ordering. The set remains constant without any dynamic referencing
-     to any underlying geometric entities.
-    """
-    def __init__(self, name, surfacePairs):
-
-        super().__init__(name)
-        self._elSurfacePairs = surfacePairs
-
-    @property
-    def surfacePairs(self):
-        """
-        Elements with the associated face orientations are specified as Nx2 numpy array, with the first column being
-        the element Id, and the second column the chosen face orientation
-        """
-        return self._elSurfacePairs
-
-    @surfacePairs.setter
-    def surfacePairs(self, surfacePairs):
-        self._elSurfacePairs = surfacePairs
-
-    def writeInput(self) -> str:
-
-        out = '*SURFACE,NAME={:s}\n'.format(self.name)
-
-        for i in range(self._elSurfacePairs.shape[0]):
-            out += '{:d},S{:d}\n'.format(self._elSurfacePairs[i,0], self._elSurfacePairs[i,1])
-
-        #out += np.array2string(self.els, precision=2, separator=', ', threshold=9999999999)[1:-1]
-        return out
-
-
-class Connector:
-    """
-     A Connector ir a rigid connector between a set of nodes and an (optional) reference node.
-     """
-    def __init__(self, name, nodes, refNode = None):
-        self.name = name
-        self._refNode = refNode
-        self._nodeset = None
-
-    @property
-    def refNode(self):
-        """
-        Reference Node ID
-        """
-        return self._refNode
-
-    @refNode.setter
-    def refNode(self, node):
-        self._refNode = node
-
-    @property
-    def nodeset(self):
-        """
-        Nodes contains the list of Node IDs
-        """
-        return self._nodeset
-
-    @nodeset.setter
-    def nodeset(self, nodes):
-
-        if isinstance(nodes, list) or isinstance(nodes,np.ndarray):
-            self._nodeset = NodeSet('Connecter_{:s}'.format(self.name), np.array(nodes))
-        elif isinstance(nodes,NodeSet):
-            self._nodeset = nodes
-        else:
-            raise ValueError('Invalid type for nodes passed to Connector()')
-
-    def writeInput(self) -> str:
-        # A nodeset is automatically created from the name of the connector
-        strOut = '*RIGIDBODY, NSET={:s}'.format(self.nodeset.name)
-
-        # A reference node is optional
-        if isinstance(self.refNode, int):
-            strOut += ',REF NODE={:d}\n'.format(self.refNode)
-        else:
-            strOut += '\n'
-
-        return strOut
-
-
-class DOF:
-    UX = 1
-    UY = 2
-    UZ = 3
-    RX = 4
-    RY = 5
-    RZ = 6
-    T = 11
-
 class Simulation:
     """
     Provides the base class for running a Calculix simulation
     """
 
     NUMTHREADS = 1
     """ Number of Threads used by the Calculix Solver """
@@ -283,66 +122,78 @@
         Sets if the output from Calculix should be verbose i.e. printed to the console
 
         :param state:
         """
 
         cls.VERBOSE_OUTPUT = state
 
-    def setWorkingDirectory(self, workDir):
+    def setWorkingDirectory(self, workDir) -> None:
+        """
+        Sets the working directory used during the analysis.
+
+        :param workDir: An accessible working directory path
+
+        """
         if os.path.isdir(workDir) and os.access(workDir, os.W_OK):
             self._workingDirectory = workDir
         else:
             raise ValueError('Working directory ({:s}) is not accessible or writable'.format(workDir))
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self._name
 
     def getBoundaryConditions(self) -> List[BoundaryCondition]:
         """
-        Collects all boundary conditions which are attached to loadcases in the analysis
+        Collects all :class:`~pyccx.boundarycondition.BoundaryCondition` which are attached to :class:`LoadCase` in
+        the analysis
+
+        :return:  All the boundary conditions in the analysis
         """
         bcs = []
         for loadcase in self._loadCases:
             bcs += loadcase.boundaryConditions
 
         return bcs
 
     @property
     def loadCases(self) -> List[LoadCase]:
         """
-        The Loadcases for the analysis
+        List of :class:`~pyccx.loadcase.LoadCase` used in the analysis
         """
         return self._loadCases
 
     @loadCases.setter
     def loadCases(self, loadCases: List[LoadCase]):
         self._loadCases = loadCases
 
     @property
     def connectors(self) -> List[Connector]:
         """
-        List of connectors used in the simulation
+        List of :class:`~pyccx.core.Connector` used in the analysis
         """
         return self._connectors
 
     @connectors.setter
-    def connectors(self, connectors):
+    def connectors(self, connectors: List[Connector]):
         self._connectors = connectors
 
     @property
     def mpcSets(self):
         return self._mpcSets
 
     @mpcSets.setter
     def mpcSets(self, value):
         self._mpcSets = value
 
     @property
     def materials(self) -> List[Material]:
+        """
+        User defined :class:`~pyccx.material.Material` used in the analysis
+        """
         return self._materials
 
     @materials.setter
     def materials(self, materials):
         self._materials = materials
 
     @property
@@ -356,15 +207,14 @@
     def materialAssignments(self, matAssignments):
         self._materialAssignments = matAssignments
 
     def _collectSets(self, setType: Type[MeshSet] = None):
         """
         Private function returns a unique set of Element, Nodal, Surface sets which are used by the analysis during writing.
         This reduces the need to explicitly attach them to an analysis.
-        :return:
         """
         elementSets = {}
         nodeSets = {}
         surfaceSets = {}
 
         # Iterate through all user defined sets
         for elSet in self._elementSets:
@@ -379,15 +229,15 @@
         # Iterate through all loadcases and boundary conditions.and find unique values. This is greedy so will override
         # any with same name.
         for loadcase in self.loadCases:
 
             # Collect result sets node and element sets automatically
             for resultSet in loadcase.resultSet:
                 if isinstance(resultSet, ElementResult):
-                    elementSets[resultSet.elSet.name] = resultSet.elSet
+                    elementSets[resultSet.elementSet.name] = resultSet.elementSet
                 elif isinstance(resultSet, NodalResult):
                     nodeSets[resultSet.nodeSet.name] = resultSet.nodeSet
 
             for bc in loadcase.boundaryConditions:
                 if isinstance(bc.target, ElementSet):
                     elementSets[bc.target.name] = bc.target
 
@@ -408,120 +258,107 @@
             return list(surfaceSets.values())
         else:
             return list(elementSets.values()), list(nodeSets.values()), list(surfaceSets.values())
 
     @property
     def elementSets(self) -> List[ElementSet]:
         """
-        User-defined element sets manually added to the analysis
+        User-defined :class:`~pyccx.core.ElementSet` manually added to the analysis
         """
         return self._elementSets
 
     @elementSets.setter
-    def elementSets(self, val = List[ElementSet]):
-        """
-        User-defined element sets manually added to the analysis
-        """
+    def elementSets(self, val: List[ElementSet]):
         self._elementSets = val
 
     @property
     def nodeSets(self) -> List[NodeSet]:
         """
-        User-defined node sets manually added to the analysis
+        User-defined :class:`~pyccx.core.NodeSet` manually added to the analysis
         """
         return self._nodeSets
 
     @nodeSets.setter
-    def nodeSets(self, val=List[NodeSet]):
-        """
-        User-defined element sets manually added to the analysis
-        """
+    def nodeSets(self, val: List[NodeSet]):
         nodeSets = val
 
     @property
     def surfaceSets(self) -> List[SurfaceSet]:
         """
-        User-defined element sets manually added to the analysis
+        User-defined :class:`pyccx.core.SurfaceSet`  manually added to the analysis
         """
         return self._nodeSets
 
     @surfaceSets.setter
     def surfaceSets(self, val=List[SurfaceSet]):
-        """
-        User-defined element sets manually added to the analysis
-        """
         surfaceSets = val
 
     def getElementSets(self) -> List[ElementSet]:
         """
-        Returns all the element sets used and generated in the analysis
+        Returns **all** the :class:`~pyccx.core.ElementSet` used and generated in the analysis
         """
         return self._collectSets(setType = ElementSet)
 
     def getNodeSets(self) -> List[NodeSet]:
         """
-        Returns all the element sets used and generated in the analysis
+        Returns **all** the :class:`pyccx.core.NodeSet` used and generated in the analysis
         """
         return self._collectSets(setType = NodeSet)
 
     def getSurfaceSets(self) -> List[SurfaceSet]:
         """
-        Returns all the element sets used and generated in the analysis
+        Returns **all** the :class:`pyccx.core.SurfaceSet` used and generated in the analysis
         """
         return self._collectSets(setType=SurfaceSet)
 
-    def writeHeaders(self):
-
-        self._input += os.linesep
-        self._input += '{:*^125}\n'.format(' INCLUDES ')
-
-        for filename in self.includes:
-            self._input += '*include,input={:s}'.format(filename)
-
     def writeInput(self) -> str:
         """
         Writes the input deck for the simulation
         """
 
         self.init()
 
-        self.writeHeaders()
-        self.writeMesh()
-        self.writeNodeSets()
-        self.writeElementSets()
-        self.writeKinematicConnectors()
-        self.writeMPCs()
-        self.writeMaterials()
-        self.writeMaterialAssignments()
-        self.writeInitialConditions()
-        self.writeAnalysisConditions()
-        self.writeLoadSteps()
+        self._writeHeaders()
+        self._writeMesh()
+        self._writeNodeSets()
+        self._writeElementSets()
+        self._writeKinematicConnectors()
+        self._writeMPCs()
+        self._writeMaterials()
+        self._writeMaterialAssignments()
+        self._writeInitialConditions()
+        self._writeAnalysisConditions()
+        self._writeLoadSteps()
 
         return self._input
 
+    def _writeHeaders(self):
 
-    def writeElementSets(self):
-        """
-        Functions writes element sets
-        """
+        self._input += os.linesep
+        self._input += '{:*^125}\n'.format(' INCLUDES ')
+
+        for filename in self.includes:
+            self._input += '*include,input={:s}'.format(filename)
+
+    def _writeElementSets(self):
 
         # Collect all sets
         elementSets = self._collectSets(setType = ElementSet)
 
         if len(elementSets) == 0:
             return
 
         self._input += os.linesep
         self._input += '{:*^125}\n'.format(' ELEMENT SETS ')
 
-        for elSet in self.elementSets:
+        for elSet in elementSets:
             self._input += os.linesep
             self._input += elSet.writeInput()
 
-    def writeNodeSets(self):
+    def _writeNodeSets(self):
 
         # Collect all sets
         nodeSets = self._collectSets(setType=NodeSet)
 
         if len(nodeSets) == 0:
             return
 
@@ -531,28 +368,28 @@
         for nodeSet in nodeSets:
             self._input += os.linesep
             self._input += nodeSet.writeInput()
             #self._input += '*NSET,NSET={:s}\n'.format(nodeSet['name'])
             #self._input += '*NSET,NSET={:s}\n'.format(nodeSet['name'])
             #self._input += np.array2string(nodeSet['nodes'], precision=2, separator=', ', threshold=9999999999)[1:-1]
 
-    def writeKinematicConnectors(self):
+    def _writeKinematicConnectors(self):
 
         if len(self.connectors) < 1:
             return
 
         self._input += os.linesep
         self._input += '{:*^125}\n'.format(' KINEMATIC CONNECTORS ')
 
         for connector in self.connectors:
 
             # A nodeset is automatically created from the name of the connector
             self._input += connector.writeInput()
 
-    def writeMPCs(self):
+    def _writeMPCs(self):
 
         if len(self.mpcSets) < 1:
             return
 
         self._input += os.linesep
         self._input += '{:*^125}\n'.format(' MPCS ')
 
@@ -565,56 +402,56 @@
 
                 self._input += os.linesep
 
     #        *EQUATION
     #        2 # number of terms in equation # typically two
     #        28,2,1.,22,2,-1. # node a id, dof, node b id, dof b
 
-    def writeMaterialAssignments(self):
+    def _writeMaterialAssignments(self):
         self._input += os.linesep
         self._input += '{:*^125}\n'.format(' MATERIAL ASSIGNMENTS ')
 
         for matAssignment in self.materialAssignments:
             self._input += '*solid section, elset={:s}, material={:s}\n'.format(matAssignment[0], matAssignment[1])
 
-    def writeMaterials(self):
+    def _writeMaterials(self):
         self._input += os.linesep
         self._input += '{:*^125}\n'.format(' MATERIALS ')
         for material in self.materials:
             self._input += material.writeInput()
 
-    def writeInitialConditions(self):
+    def _writeInitialConditions(self):
         self._input += os.linesep
         self._input += '{:*^125}\n'.format(' INITIAL CONDITIONS ')
 
         for initCond in self.initialConditions:
             self._input += '*INITIAL CONDITIONS,TYPE={:s}\n'.format(initCond['type'].upper())
             self._input += '{:s},{:e}\n'.format(initCond['set'], initCond['value'])
             self._input += os.linesep
 
         # Write the Physical Constants
         self._input += '*PHYSICAL CONSTANTS,ABSOLUTE ZERO={:e},STEFAN BOLTZMANN={:e}\n'.format(self.TZERO, self.SIGMAB)
 
-    def writeAnalysisConditions(self):
+    def _writeAnalysisConditions(self):
 
         self._input += os.linesep
         self._input += '{:*^125}\n'.format(' ANALYSIS CONDITIONS ')
 
         # Write the Initial Timestep
         self._input += '{:.3f}, {:.3f}\n'.format(self.initialTimeStep, self.defaultTimeStep)
 
-    def writeLoadSteps(self):
+    def _writeLoadSteps(self):
 
         self._input += os.linesep
         self._input += '{:*^125}\n'.format(' LOAD STEPS ')
 
         for loadCase in self.loadCases:
             self._input += loadCase.writeInput()
 
-    def writeMesh(self):
+    def _writeMesh(self):
 
         # TODO make a unique auto-generated name for the mesh
         meshFilename = 'mesh.inp'
         meshPath= os.path.join(self._workingDirectory, meshFilename)
 
         self.model.writeMesh(meshPath)
         self._input += '*include,input={:s}'.format(meshFilename)
@@ -652,28 +489,31 @@
             version = re.search(r"(\d+).(\d+)", stdout)
             return int(version.group(1)), int(version.group(2))
 
         else:
             raise NotImplemented(' Platform is not currently supported')
 
     def results(self) -> ResultProcessor:
-        """ Returns the results obtained after running an analysis """
+        """
+        The results obtained after running an analysis
+         """
         if self.isAnalysisCompleted():
             return ResultProcessor('input')
         else:
             raise ValueError('Results were not available')
 
     def isAnalysisCompleted(self) -> bool:
-        """ Returns if the analysis was completed successfully. """
+        """ Returns if the analysis was completed successfully """
         return self._analysisCompleted
 
-    def clearAnalysis(self, includeResults:bool = False) -> None:
-        """ Clears any files generated from the analysis
+    def clearAnalysis(self, includeResults: bool = False) -> None:
+        """
+        Clears any previous files generated from the analysis
 
-        :param includeResults:  If set True will also delete the result files generated from the analysis
+        :param includeResults:  If set `True` will also delete the result files generated from the analysis
         """
 
         filename = 'input' # Base filename for the analysis
 
         files = [filename + '.inp',
                  filename + '.cvg',
                  filename + '.sta']
@@ -727,15 +567,15 @@
                     print(stdout_line, end='')
 
             popen.stdout.close()
             return_code = popen.wait()
             if return_code:
                 raise subprocess.CalledProcessError(return_code, cmd)
 
-            # Analysis was completed successfully
+            # A        :return:nalysis was completed successfully
             self._analysisCompleted = True
 
         elif sys.platform == 'linux':
 
             filename = 'input'
 
             cmdSt = ['ccx', '-i', filename]
```

### Comparing `PyCCX-0.1/pyccx/loadcase.py` & `PyCCX-0.1.2/pyccx/loadcase/loadcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import numpy as np
 import abc
 import os
 
-from .boundarycondition import BoundaryCondition, BoundaryConditionType
-from .results import Result
 from enum import Enum, auto
 from typing import List, Tuple, Type
 
+from ..bc import BoundaryCondition, BoundaryConditionType
+from ..results import Result
+
 
 class LoadCaseType(Enum):
     """
     Enum Class specifies the Load Case Type
     """
+
     STATIC = auto()
     """Linear Static structural analysis"""
     THERMAL = auto()
     """Thermal analysis for performing heat transfer studies"""
     UNCOUPLEDTHERMOMECHANICAL = auto()
     """Coupled thermo-mechanical analysis"""
     BUCKLE = auto()
@@ -26,16 +28,16 @@
     """Dynamic analysis of a structure"""
 
 
 class LoadCase:
     """
     A unique Load case defines a set of simulation analysis conditions and a set of boundary conditions to apply to the domain.
     The default and initial timestep provide an estimate for the solver should be specified  along with the total duration
-    of the load case using :meth:`pyccx.loadcase.LoadCase.setTimeStep`. The analysis type for the loadcase should be
-    specified using :meth:`pyccx.loadcase.Loadcase.setLoadCaseType`. Depending on the analysis type the steady-state solution
+    of the load case using :meth:`setTimeStep`. The analysis type for the loadcase should be
+    specified using :meth:`setLoadCaseType`. Depending on the analysis type the steady-state solution
     may instead be calculated.
     """
     def __init__(self, loadCaseName, loadCaseType: LoadCaseType = None, resultSets = None):
 
         self._input = ''
         self._loadcaseName = loadCaseName
         self._loadCaseType = None
@@ -69,25 +71,25 @@
     @boundaryConditions.setter
     def boundaryConditions(self, bConds: List[BoundaryCondition]):
         self._boundaryConditions = bConds
 
     @property
     def resultSet(self) -> List[Result]:
         """
-        The result outputs (:class:`pyccx.results.ElementResult`, :class:`pyccx.results.NodalResult`) to generate the set
-        of results from this loadcase.
+        The result outputs (:class:`~pyccx.results.ElementResult`, :class:`~pyccx.results.NodeResult`) to generate
+        the set of results from this loadcase.
         """
         return self._resultSet
 
     @resultSet.setter
-    def resultSet(self, rSet: Type[Result]):
-        if not any(isinstance(rSet, Result)):
-            raise ValueError('Loadcase ResultSets must be of type Result')
+    def resultSet(self, rSets: Type[Result]):
+        if not any(isinstance(x, Result) for x in rSets):
+            raise ValueError('Loadcase ResultSets must be derived from a Result class')
         else:
-            self._resultSet = rSet
+            self._resultSet = rSets
 
     @property
     def name(self) -> str:
         return self._loadcaseName
 
     @name.setter
     def name(self, loadCaseName):
@@ -118,37 +120,38 @@
 
         if initialIimeStep is not None:
             self.initialTimeStep = initialIimeStep
 
         if totalTime is not None:
             self.totalTime = totalTime
 
-    def setLoadCaseType(self, loadCaseType) -> None:
+    def setLoadCaseType(self, loadCaseType: LoadCaseType) -> None:
         """
-        Set the loadcase type based on the analysis types available in :class:`pyccx.loadcase.LoadCasetype`.
+        Set the loadcase type based on the analysis types available in :class:`~pyccx.loadcase.LoadCaseType`.
 
-        :param loadCaseType: Set the loadcase type using the enum :class:`pyccx.loadcase.LoadCasetype`
+        :param loadCaseType: Set the loadcase type using the enum :class:`~pyccx.loadcase.LoadCaseType`
         """
 
-        if isinstance(loadCaseType):
+        if isinstance(loadCaseType, LoadCaseType):
             self._loadCaseType = loadCaseType
         else:
             raise ValueError('Load case type is not supported')
 
     def writeBoundaryCondition(self) -> str:
         """
-        Generates the string for Boundary Conditions in self.boundaryConditions containing all the attached boundary conditions.
-        Calculix cannot share existing boundary conditions and therefore has to be explicitly created per load case.
+        Generates the string for Boundary Conditions in self.boundaryConditions containing all the attached boundary
+        conditions. Calculix cannot share existing boundary conditions and therefore has to be explicitly
+        created per load case.
 
         :return: outStr
         """
         bcondStr = ''
 
         for bcond in self.boundaryConditions:
-            bcondStr += bcond
+            bcondStr += bcond.writeInput()
 
         if False:
             for bcond in self.boundaryConditions:
 
                 if bcond['type'] == 'film':
 
                     bcondStr += '*FILM\n'
```

### Comparing `PyCCX-0.1/pyccx/mesh/mesh.py` & `PyCCX-0.1.2/pyccx/mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `PyCCX-0.1/pyccx/mesh/mesher.py` & `PyCCX-0.1.2/pyccx/mesh/mesher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import os
 import numpy as np
 import gmsh
 from enum import Enum
-from typing import List, Tuple
+from typing import List, Optional, Tuple
+
 
 class MeshingAlgorithm(Enum):
     DELAUNAY = 1
     FRONTAL = 4
     FRONTAL_DELAUNAY = 5
     FRONTAL_HEX = 6
     MMG3D = 7
@@ -17,15 +18,15 @@
 
 class ElementType:
     """
     Element types information used via GMSH and Calculix
     """
 
     class NODE:
-        """ A single node element s"""
+        """ A single node element"""
         id = 15
         name = 'Node'
         nodes = 1
         faces = None
 
     class TET4:
         """ 1st order linear Tet Element (C3D4) """
@@ -91,15 +92,15 @@
     """
 
     # Static class variables for meshing operations
 
     ElementOrder = 1
     NumThreads = 4
     OptimiseNetgen = True
-    Units = 'mm'
+    Units = ''
     Initialised = False
 
     # Instance methods
     def __init__(self, modelName: str):
         """
         :param modelName: str: A model name is required for GMSH
         """
@@ -121,51 +122,52 @@
 
         # Set the model name for this instance
         gmsh.model.add(self._modelName)
 
     @classmethod
     def showGui(cls):
         """
-        Opens up the native GMSH gui to inspect the geometry in the model and the mesh. This will block the Python script
+        Opens up the native GMSH Gui to inspect the geometry in the model and the mesh. This will block the Python script
         until the GUI is exited.
         """
         if cls.Initialised:
             gmsh.fltk.run()
 
     def maxPhysicalGroupId(self, dim: int) -> int:
         """
         Returns the highest physical group id in the GMSH model
+
         :param dim: int: The chosen dimension
         :return: int: The highest group id used
         """
         self.setAsCurrentModel()
         return np.max([x[1] for x in gmsh.model.getPhysicalGroups(dim)])
 
     def getVolumeName(self, volId: int) -> str:
         """
         Gets the volume name (if assigned)
 
         :param volId: int: Volume id of a region
         """
         self.setAsCurrentModel()
-        return gmsh.model.getPhysicalName(3,volId)
+        return gmsh.model.getEntityName(3,volId)
 
     def getEntityName(self, id: Tuple[int, int]) -> str:
         """
         Returns the name of an entity given an id (if assigned)
 
         :param id: Dimension, Entity Id
 
         """
         self.setAsCurrentModel()
-        return gmsh.model.getPhysicalName(id[0],id[1])
+        return gmsh.model.getEntityName(id[0],id[1])
 
-    def setEntityName(self, id: Tuple[int, int], name:str) -> None:
+    def setEntityName(self, id: Tuple[int, int], name: str) -> None:
         """
-        Set the geometrical entity name - useful only as reference when vieiwing in the GMSH GUI
+        Set the geometrical entity name - useful only as reference when viewing in the GMSH GUI
 
         :param id: Entity Dimension and Entity Id
         :param name: The entity name
 
         """
         self.setAsCurrentModel()
         gmsh.model.setEntityName(id[0], id[1], name)
@@ -224,15 +226,15 @@
         Any changes to GMSH model should call this to prevent inconsistency in a generated model
 
         :param state:  Force the model to be shown as generated
         """
 
         self._isDirty = state
 
-    def addGeometry(self, filename: str, name: str, meshFactor: float = 0.03):
+    def addGeometry(self, filename: str, name: str, meshFactor: Optional[float] = 0.03):
         """
         Adds CAD geometry into the GMSH kernel. The filename of compatiable model files along with the mesh factor
         should be used to specify a target mesh size.
 
         :param filename:
         :param name: Name to assign to the geometries imported
         :param meshFactor: Initialise the target element size to a proportion of the average bounding box dimensions
@@ -247,26 +249,26 @@
         # Additional geometry will be merged into the current  model
         gmsh.merge(filename)
         self.geoms.append({'name': name, 'filename': filename, 'meshSize': None, 'meshFactor': meshFactor})
 
         # Set the name of the volume
         # This automatically done to ensure that are all exported. This may change to parse through all volumes following
         # merged and be recreated
-        print(len(self.geoms))
+
         gmsh.model.setEntityName(3, len(self.geoms), name)
         gmsh.model.addPhysicalGroup(3, [len(self.geoms)], len(self.geoms))
         gmsh.model.setPhysicalName(3, len(self.geoms), name)
 
         # set the mesh size for this geometry
         bbox = self.getGeomBoundingBoxById(len(self.geoms))
         extents = bbox[1, :] - bbox[0, :]
         avgDim = np.mean(extents)
         meshSize = avgDim * meshFactor
 
-        print('Avg dim', avgDim, ' mesh size: ', meshSize)
+        print('GMSH: Avg dim', avgDim, ' mesh size: ', meshSize)
         geomPoints = self.getPointsFromVolume(len(self.geoms))
 
         # Set the geometry volume size
         self.geoms[-1]['meshSize'] = meshSize
 
         self.setMeshSize(geomPoints, meshSize)
 
@@ -436,34 +438,31 @@
 
     @classmethod
     def finalize(cls):
         gmsh.finalize()
         cls.Initialised = False
 
     @classmethod
-    def initialise(cls):
+    def initialise(cls) -> None:
         """
         Initialises the GMSH runtime and sets default options. This is called automatically once.
-        :return:
         """
 
-        print(cls.Initialised)
-
         if cls.Initialised:
             return
 
-        print('\033[1;34;47m Initialising GMSH \n')
+        print('Initialising GMSH \n')
 
         gmsh.initialize()
 
         # Mesh.Algorithm3D
         # 3D mesh algorithm (1: Delaunay, 4: Frontal, 5: Frontal Delaunay, 6: Frontal Hex, 7: MMG3D, 9: R-tree, 10: HXT)
         # Default value: 1#
 
-        gmsh.option.setNumber("Mesh.Algorithm", 5);
+        gmsh.option.setNumber("Mesh.Algorithm", MeshingAlgorithm.FRONTAL_DELAUNAY.value);
         #        gmsh.option.setNumber("Mesh.Algorithm3D", 10);
 
         gmsh.option.setNumber("Mesh.ElementOrder", Mesher.ElementOrder)
         #        gmsh.option.setNumber("Mesh.OptimizeNetgen",1)
         gmsh.option.setNumber("Mesh.MaxNumThreads3D", Mesher.NumThreads)
 
         # gmsh.option.setNumber("Mesh.SaveGroupsOfNodes", 1);
@@ -537,49 +536,49 @@
         """
         From a Volume Id, obtain all Point Ids associated with this volume - note may include shared points.
 
         :param id: Volume ID
         :return: list(int) - List of Point Ids
         """
         self.setAsCurrentModel()
-        pnts = gmsh.model.getBoundary((3, id), recursive=True)
+        pnts = gmsh.model.getBoundary([(3, id)], recursive=True)
         return [x[1] for x in pnts]
 
     def getPointsFromEntity(self, id: Tuple[int,int]) -> List[int]:
         """
         From an Id, obtain all Point Ids associated with this volume - note may include shared points.
 
         :param id: Dimension and Entity ID
         :return: List of Point Ids
         """
         self.setAsCurrentModel()
-        pnts = gmsh.model.getBoundary(id, recursive=True)
+        pnts = gmsh.model.getBoundary([id], recursive=True)
         return [x[1] for x in pnts]
 
     def getChildrenFromEntities(self, id: Tuple[int,int]) -> List[int]:
         """
         From a Entity, obtain all children associated with this volume - note may include shared entities.
 
         :param id:  Dimension, Entity Id
         :return: List of Ids
         """
         self.setAsCurrentModel()
-        entities = gmsh.model.getBoundary(id, recursive=False)
+        entities = gmsh.model.getBoundary([id], recursive=False)
         return [x[1] for x in entities]
 
     def getSurfacesFromVolume(self, id: int) -> List[int]:
         """
         From a Volume Id, obtain all Surface Ids associated with this volume - note may include shared boundary surfaces.
 
         :param id:  Volume Id
         :return: List of surface Ids
         """
-        raise NotImplementedError()
+
         self.setAsCurrentModel()
-        surfs = gmsh.model.getBoundary((3, id), recursive=False)
+        surfs = gmsh.model.getBoundary( [(3, id)], recursive=False)
         return [x[1] for x in surfs]
 
     def getPointsFromVolumeByName(self, volumeName: str):
         """
         Returns all geometric points from a given volume domain by its name (if assigned)
         :param volumeName: volumeName
         :return:
@@ -629,24 +628,26 @@
         self.setAsCurrentModel()
 
         if not self._isMeshGenerated:
             raise ValueError('Mesh is not generated')
 
         if entityId:
             # return all the elements for the entity
-            return gmsh.model.mesh.getElements(entityId[0], entityId[1])[0]
+            result =  gmsh.model.mesh.getElements(entityId[0], entityId[1])
+            return np.hstack(result[1])
         else:
             # Return all the elements in the model
-            return gmsh.model.mesh.getElements()[0]
+            result =  gmsh.model.mesh.getElements()
+            return np.hstack(result[1])
 
 
     def getElementsByType(self, elType) -> np.ndarray:
         """
         Returns all elements of type (elType) from the GMSH model, within class ElementTypes. Note: the element ids are returned with
-        an index starting from 0 - internally GMSH uses an index starting from 1, like most FEA pre-processors
+        an index starting from 1 - internally GMSH uses an index starting from 1, like most FEA pre-processors
 
         :return: List of element Ids.
         """
 
         self.setAsCurrentModel()
 
         if not self._isMeshGenerated:
@@ -870,23 +871,23 @@
         """
         self._isMeshGenerated = False
 
         self._setModelOptions()
 
         self.setAsCurrentModel()
 
-        print('\033[1;34;47m Generating GMSH \n')
+        print('Generating GMSH \n')
 
         gmsh.model.mesh.generate(1)
         gmsh.model.mesh.generate(2)
 
         try:
             gmsh.model.mesh.generate(3)
         except:
-            print('\033[1;34;47m Meshing Failed \n')
+            print('Meshing Failed \n')
 
         self._isMeshGenerated = True
         self._isDirty = False
 
     def isMeshGenerated(self) -> bool:
         """
         Returns if the mesh has been successfully generated by GMSH
```

### Comparing `PyCCX-0.1/pyccx/results.py` & `PyCCX-0.1.2/pyccx/results/results.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 import re
 import os
 
-from .core import ElementSet, NodeSet
+from ..core import ElementSet, NodeSet
 
 import numpy as np
 
 
 class Result(abc.ABC):
     """
     Base Class for all Calculix Results
@@ -68,16 +68,15 @@
             inputStr += 'RF\n'
 
         inputStr += self.writeElementInput()
 
         return inputStr
 
     def writeElementInput(self):
-        str = ''
-        str += '*EL FILE, NSET={:s}, FREQUENCY={:d}\n'.format(self.nodeSet, self.frequency)
+        str = '*EL FILE, NSET={:s}, FREQUENCY={:d}\n'.format(self._nodeSet.name, self.frequency)
 
         if self.useCauchyStress:
             str += 'S\n'
         if self.useNodalStrain:
             str += 'E\n'
 
         if self.usePlasticStrain:
@@ -88,15 +87,15 @@
 
         return str
 
 
 class ElementResult(Result):
     def __init__(self, elSet: ElementSet):
 
-        self.elSet = elSet
+        self._elSet = elSet
         self.useElasticStrain = False
         self.useCauchyStress = False
         self.useHeatFlux = False
         self.useESE = False
 
         super().__init__()
 
@@ -109,15 +108,15 @@
 
     @elementSet.setter
     def elementSet(self, elSet: ElementSet):
         self._elSet = elSet
 
     def writeInput(self):
         str = ''
-        str += '*EL PRINT, ELSET={:s}, FREQUENCY={:d}\n'.format(self.elSet, self.frequency)
+        str += '*EL PRINT, ELSET={:s}, FREQUENCY={:d}\n'.format(self._elSet.name, self.frequency)
 
         if self.useCauchyStress:
             str += 'S\n'
 
         if self.useElasticStrain:
             str += 'E\n'
 
@@ -151,22 +150,22 @@
         """
 
         idx = sorted(list(self.increments.keys()))[-1]
         return self.increments[idx]
 
     def findIncrementByTime(self, incTime) -> int:
 
-        for inc in self.increments:
-            if abs(inc['time'] - incTime) < 1e-9:
-                return inc
+        for inc, increment in self.increments.items():
+            if abs(increment['time'] - incTime) < 1e-9:
+                return inc, increment
         else:
             raise ValueError('Increment could not be found at time <{:.5f}>s'.format(incTime))
 
     @staticmethod
-    def __get_vals(fstr: str, line: str):
+    def _getVals(fstr: str, line: str):
         """
         Returns a list of typed items based on an input format string. Credit for
         the processing of the .dat file is based from the PyCalculix project.
         https://github.com/spacether/pycalculix
 
         :param fstr: C format string, commas separate fields
         :param line: str: line string to parse
@@ -228,74 +227,74 @@
         """
         while True:
             line = infile.readline()
             if line[:3] == ' -1':
                 return line
 
     def readNodeDisp(self, line, rfstr) -> tuple:
-        nid, ux, uy, uz = self.__get_vals(rfstr, line)[1:]
+        nid, ux, uy, uz = self._getVals(rfstr, line)[1:]
         return nid, ux, uy, uz
 
     def readNodeForce(self, line, rfstr):
-        nid, f_x, f_y, f_z = self.__get_vals(rfstr, line)[1:]
+        nid, f_x, f_y, f_z = self._getVals(rfstr, line)[1:]
         return nid, f_x, f_y, f_z
 
     def readNodeFlux(self, line, rfstr) -> tuple:
-        nid, f_x, f_y, f_z = self.__get_vals(rfstr, line)[1:]
+        nid, f_x, f_y, f_z = self._getVals(rfstr, line)[1:]
         return nid, f_x, f_y, f_z
 
     def readNodeTemp(self, line, rfstr) -> tuple:
-        nid, temp = self.__get_vals(rfstr, line)[1:]
+        nid, temp = self._getVals(rfstr, line)[1:]
         return nid, temp
 
     def readNodeStress(self, line, rfstr) -> tuple:
-        nid, sxx, syy, szz, sxy, syz, szx = self.__get_vals(rfstr, line)[1:]
+        nid, sxx, syy, szz, sxy, syz, szx = self._getVals(rfstr, line)[1:]
         return nid, sxx, syy, szz, sxy, syz, szx
 
     def readNodeStrain(self, line, rfstr) -> tuple:
-        nid, exx, eyy, ezz, exy, eyz, ezx = self.__get_vals(rfstr, line)[1:]
+        nid, exx, eyy, ezz, exy, eyz, ezx = self._getVals(rfstr, line)[1:]
         return nid, exx, eyy, ezz, exy, eyz, ezx
 
     def readElFlux(self, line, rfstr, time):
         """Saves element integration point stresses"""
+        elFlux = self._getVals(rfstr, line)[1:]
 
-        elId, intp, qx, qy, qz = self.__get_vals(rfstr, line)[1:]
+        elId, intp, qx, qy, qz = self._getVals(rfstr, line)
 
         return elId, intp, qx, qy, qz
 
     def readElStress(self, line, rfstr, time):
         """Saves element integration point stresses"""
 
-        elId, intp, sxx, syy, szz, sxy, syz, szx = self.__get_vals(rfstr, line)[1:]
+        elId, intp, sxx, syy, szz, sxy, syz, szx = self._getVals(rfstr, line)
 
         return elId, intp, sxx, syy, szz, sxy, syz, szx
 
 
     def readElResultBlock(self, infile, line):
 
         """Returns an array of line, mode, rfstr, time"""
         words = line.strip().split()
         # add time if not present
         time = float(words[-1])
 
         # set mode
         rfstr = "I10,2X,I2,6E14.2"
-        tmp = self.__get_vals(rfstr, line)
 
         mode = 'stress'
         infile.readline()
         line = infile.readline()
         return [line, mode, rfstr, time]
 
     def readNodalResultsBlock(self, infile):
 
         """Returns an array of line, mode, rfstr, time"""
         line = infile.readline()
         fstr = "1X,' 100','C',6A1,E12.5,I12,20A1,I2,I5,10A1,I2"
-        tmp = self.__get_vals(fstr, line)
+        tmp = self._getVals(fstr, line)
         # [key, code, setname, value, numnod, text, ictype, numstp, analys, format_]
         time, format_ = tmp[3], tmp[9]
 
         # set results format to short, long or binary
         # only short and long are parsed so far
         if format_ == 0:
             rfstr = "1X,I2,I5,6E12.5"
@@ -308,15 +307,15 @@
         # set the time
         # self.__store_time(time)
 
         # get the name to determine if stress or displ
         line = infile.readline()
         fstr = "1X,I2,2X,8A1,2I5"
         # [key, name, ncomps, irtype]
-        ar2 = self.__get_vals(fstr, line)
+        ar2 = self._getVals(fstr, line)
         name = ar2[1]
         iteration = tmp[7]
         line = self.__get_first_dataline(infile)
 
         return [line, name, rfstr, time, iteration]
 
     def read(self) -> None:
@@ -366,14 +365,16 @@
             elif mode == 'FORC':
                 self.increments[inc]['force'].append(self.readNodeForce(line, rfstr))
             elif mode == 'NDTEMP':
                 self.increments[inc]['temp'].append(self.readNodeTemp(line, rfstr))
 
         infile.close()
 
+        self.readDat()
+
         # Process the nodal blocks
         for inc in self.increments.values():
             inc['disp'] = self.orderNodes(np.array(inc['disp']))
             inc['stress'] = self.orderNodes(np.array(inc['stress']))
             inc['strain'] = self.orderNodes(np.array(inc['strain']))
             inc['force'] = self.orderNodes(np.array(inc['force']))
             inc['temp'] = self.orderNodes(np.array(inc['temp']))
@@ -405,41 +406,50 @@
 
         infile = open(fname, 'r')
         print('Loading element results from file: ' + fname)
 
         mode = None
         rfstr = ''
         incTime = 0.0
+        inc = -1
         while True:
             line = infile.readline()
+
             if not line:
                 break
 
+            if line.strip() == '':
+                mode = None
+
             # check for stress, we skip down to the line data when
             # we call __modearr_estrsresults
             if 'stress' in line:
                 arr = self.readElResultBlock(infile, line)
                 line, mode, rfstr, incTime = arr
 
                 # store stress results
-                inc = self.findIncrementByTime(incTime)
+                inc, increment = self.findIncrementByTime(incTime)
                 self.increments[inc]['elStress'].append(self.readElStress(line, rfstr, incTime))
             elif 'heat flux' in line:
                 arr = self.readElResultBlock(infile, line)
                 line, mode, rfstr, incTime = arr
 
-                # store stress results
-                inc = self.findIncrementByTime(incTime)
-                self.increments[inc]['elHeatFlux'].append(self.readElFlux(line, rfstr, incTime))
+                print(incTime)
+                print(self.increments)
+                # store the heatlufx results
+                inc, increment = self.findIncrementByTime(incTime)
 
+                mode = 'elHeatFlux'
+                self.increments[inc][mode] = []
 
-            # reset the read type if we hit a blank line
-            if line.strip() == '':
-                mode = None
-            if not mode:
-                continue
+            if mode and inc > -1:
+                self.increments[inc][mode].append(self.readElFlux(line, rfstr, incTime))
 
         for inc in self.increments.values():
-            inc['elStress'] = self.orderElements(np.array(inc['elStress']))
-            inc['elHeatFlux'] = self.orderElements(np.array(inc['elHeatFlux']))
+
+            if 'elStress' in inc:
+                inc['elStress'] = self.orderElements(np.array(inc['elStress']))
+
+            if 'elHeatFlux' in inc:
+                inc['elHeatFlux'] = self.orderElements(np.array(inc['elHeatFlux']))
 
         infile.close()
```

### Comparing `PyCCX-0.1/setup.py` & `PyCCX-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 import os
 from setuptools import setup, find_packages
 
 # load __version__ without importing anything
 version_file = os.path.join(
     os.path.dirname(__file__),
     'pyccx/version.py')
@@ -17,16 +15,16 @@
 if os.path.exists('README.rst'):
     with open('README.rst', 'r') as f:
         long_description = f.read()
 
 # minimal requirements for installing pyccx
 # note that `pip` requires setuptools itself
 requirements_default = set([
-    'numpy',     # all data structures
-    'gmsh-sdk',  # Required for meshing geometry
+    'numpy',      # all data structures
+    'gmsh',       # Required for meshing geometry
     'setuptools'  # used for packaging
 ])
 
 # "easy" requirements should install without compiling
 # anything on Windows, Linux, and Mac, for Python 2.7-3.4+
 requirements_easy = set([
     'setuptools',  # do setuptools stuff
@@ -46,28 +44,32 @@
 
 with open('LICENSE') as f:
     license = f.read()
 
 setup(
     name='PyCCX',
     version=__version__,
-    description='Simulation FEA environment for Python built upon Calculix and GMSH',
+    description='Simulation and FEA environment for Python built upon Calculix and GMSH',
     long_description=long_description,
     long_description_content_type = 'text/x-rst',
     author='Luke Parry',
     author_email='dev@lukeparry.uk',
     url='https://github.com/drlukeparry/pyccx',
     keywords='FEA, Finite Element Analysis, Simulation, Calculix, GMSH',
     python_requires='>=3.5',
     classifiers=[
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Natural Language :: English',
         'Topic :: Scientific/Engineering'],
     license="",
     packages=find_packages(exclude=('tests', 'docs')),
     install_requires=list(requirements_default),
     extras_require={'easy': list(requirements_easy),
                     'docs': list(requirements_docs)},
```

