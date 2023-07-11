# Comparing `tmp/tidynamics-1.0.0.tar.gz` & `tmp/tidynamics-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tidynamics-1.0.0.tar", last modified: Tue Aug 21 12:44:52 2018, max compression
+gzip compressed data, was "tidynamics-1.1.2.tar", last modified: Tue Jul 11 12:37:46 2023, max compression
```

## Comparing `tidynamics-1.0.0.tar` & `tidynamics-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,65 @@
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2018-08-21 12:44:52.000000 tidynamics-1.0.0/
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2018-08-21 12:44:52.000000 tidynamics-1.0.0/tidynamics.egg-info/
--rw-r--r--   0 pierre    (1000) pierre    (1000)      306 2018-08-21 12:44:52.000000 tidynamics-1.0.0/tidynamics.egg-info/SOURCES.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        6 2018-08-21 12:44:52.000000 tidynamics-1.0.0/tidynamics.egg-info/requires.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2018-08-21 12:44:52.000000 tidynamics-1.0.0/tidynamics.egg-info/dependency_links.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       11 2018-08-21 12:44:52.000000 tidynamics-1.0.0/tidynamics.egg-info/top_level.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4313 2018-08-21 12:44:52.000000 tidynamics-1.0.0/tidynamics.egg-info/PKG-INFO
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2018-08-21 12:44:52.000000 tidynamics-1.0.0/tidynamics/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4174 2018-08-20 18:45:24.000000 tidynamics-1.0.0/tidynamics/_correlation.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)        6 2018-08-21 12:18:09.000000 tidynamics-1.0.0/tidynamics/VERSION
--rw-r--r--   0 pierre    (1000) pierre    (1000)      625 2018-08-21 11:51:48.000000 tidynamics-1.0.0/tidynamics/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1796 2018-06-29 12:19:36.000000 tidynamics-1.0.0/tidynamics/core.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      825 2018-08-14 13:26:11.000000 tidynamics-1.0.0/setup.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)       16 2018-08-14 12:41:41.000000 tidynamics-1.0.0/MANIFEST.in
--rw-r--r--   0 pierre    (1000) pierre    (1000)       67 2018-08-21 12:44:52.000000 tidynamics-1.0.0/setup.cfg
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3133 2018-08-21 11:54:03.000000 tidynamics-1.0.0/README.rst
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1468 2018-06-07 07:59:53.000000 tidynamics-1.0.0/LICENSE
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4313 2018-08-21 12:44:52.000000 tidynamics-1.0.0/PKG-INFO
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-11 12:37:46.021011 tidynamics-1.1.2/
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-11 12:37:46.005012 tidynamics-1.1.2/.binder/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       96 2023-07-11 12:24:53.000000 tidynamics-1.1.2/.binder/README.txt
+-rwxr-xr-x   0 pierre    (1000) pierre    (1000)       36 2023-07-11 12:24:53.000000 tidynamics-1.1.2/.binder/postBuild
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       17 2023-07-11 12:24:53.000000 tidynamics-1.1.2/.binder/requirements.txt
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-11 12:37:45.997012 tidynamics-1.1.2/.github/
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-11 12:37:46.005012 tidynamics-1.1.2/.github/workflows/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      589 2023-07-11 12:24:53.000000 tidynamics-1.1.2/.github/workflows/test.yml
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       71 2017-12-09 20:54:54.000000 tidynamics-1.1.2/.gitignore
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      954 2020-01-14 10:37:07.000000 tidynamics-1.1.2/.travis.yml
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      765 2019-10-16 13:31:29.000000 tidynamics-1.1.2/CITATION
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       40 2019-10-16 13:31:29.000000 tidynamics-1.1.2/CONTRIBUTORS
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1473 2023-07-11 12:24:53.000000 tidynamics-1.1.2/LICENSE
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       16 2018-08-14 12:41:41.000000 tidynamics-1.1.2/MANIFEST.in
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3693 2023-07-11 12:37:46.021011 tidynamics-1.1.2/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3309 2023-07-11 12:34:39.000000 tidynamics-1.1.2/README.rst
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-11 12:37:46.009012 tidynamics-1.1.2/doc/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       29 2017-12-11 13:47:46.000000 tidynamics-1.1.2/doc/.gitignore
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      845 2018-02-08 22:53:51.000000 tidynamics-1.1.2/doc/Makefile
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2637 2023-07-11 08:31:09.000000 tidynamics-1.1.2/doc/algorithms.rst
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1805 2018-08-13 16:27:22.000000 tidynamics-1.1.2/doc/bibtex.bib
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     5650 2023-07-11 12:24:53.000000 tidynamics-1.1.2/doc/conf.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      384 2018-06-30 12:50:04.000000 tidynamics-1.1.2/doc/contents.rst
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       82 2018-06-30 12:50:24.000000 tidynamics-1.1.2/doc/contributors.rst
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      201 2019-10-16 13:31:29.000000 tidynamics-1.1.2/doc/correlation.rst
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1412 2018-08-16 10:27:04.000000 tidynamics-1.1.2/doc/data_format.rst
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3455 2018-08-20 18:49:19.000000 tidynamics-1.1.2/doc/index.ipynb
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3768 2023-07-11 12:34:55.000000 tidynamics-1.1.2/doc/index.rst
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       76 2018-08-14 09:38:23.000000 tidynamics-1.1.2/doc/zbibliography.rst
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-11 12:37:46.013012 tidynamics-1.1.2/examples/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      974 2018-08-13 14:06:18.000000 tidynamics-1.1.2/examples/README.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1823 2019-05-21 09:02:19.000000 tidynamics-1.1.2/examples/plot_acf_1.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2248 2019-05-21 09:02:19.000000 tidynamics-1.1.2/examples/plot_msd_1.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1679 2023-07-11 12:24:53.000000 tidynamics-1.1.2/examples/plot_nlogn_scaling.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2461 2018-08-13 13:05:06.000000 tidynamics-1.1.2/examples/random_steps_sample_0.txt.gz
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     6938 2018-08-13 13:04:58.000000 tidynamics-1.1.2/examples/random_walk_sample_0.txt.gz
+-rwxr-xr-x   0 pierre    (1000) pierre    (1000)     1326 2023-07-11 12:24:53.000000 tidynamics-1.1.2/examples/tidynamics_tool.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-11 12:37:46.013012 tidynamics-1.1.2/paper/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    15901 2019-10-16 13:31:29.000000 tidynamics-1.1.2/paper/msd_example.pdf
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3764 2019-10-16 13:31:29.000000 tidynamics-1.1.2/paper/paper.bib
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4218 2019-10-16 13:31:29.000000 tidynamics-1.1.2/paper/paper.md
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    15303 2019-10-16 13:31:29.000000 tidynamics-1.1.2/paper/scaling.pdf
+-rw-r--r--   0 pierre    (1000) pierre    (1000)    17290 2019-10-16 13:31:29.000000 tidynamics-1.1.2/paper/vacf_example.pdf
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      673 2023-07-11 12:24:53.000000 tidynamics-1.1.2/pyproject.toml
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       38 2023-07-11 12:37:46.021011 tidynamics-1.1.2/setup.cfg
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-11 12:37:46.017012 tidynamics-1.1.2/tests/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      427 2017-12-08 08:32:31.000000 tidynamics-1.1.2/tests/test_acf_1.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      448 2020-02-13 13:17:51.000000 tidynamics-1.1.2/tests/test_acf_2.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      556 2018-06-18 15:25:01.000000 tidynamics-1.1.2/tests/test_correlation_1.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      511 2018-06-18 15:25:35.000000 tidynamics-1.1.2/tests/test_correlation_1d.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      274 2018-01-17 09:21:01.000000 tidynamics-1.1.2/tests/test_cross_msd_1.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      404 2020-02-13 13:23:03.000000 tidynamics-1.1.2/tests/test_msd_1.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1007 2020-02-13 13:21:49.000000 tidynamics-1.1.2/tests/test_msd_2.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      621 2020-02-13 13:25:03.000000 tidynamics-1.1.2/tests/test_msd_3.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-11 12:37:46.021011 tidynamics-1.1.2/tidynamics/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        6 2023-07-11 12:35:29.000000 tidynamics-1.1.2/tidynamics/VERSION
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      625 2019-10-16 13:31:29.000000 tidynamics-1.1.2/tidynamics/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4213 2023-07-11 12:24:53.000000 tidynamics-1.1.2/tidynamics/_correlation.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1764 2023-07-11 12:24:53.000000 tidynamics-1.1.2/tidynamics/core.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-07-11 12:37:46.021011 tidynamics-1.1.2/tidynamics.egg-info/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3693 2023-07-11 12:37:45.000000 tidynamics-1.1.2/tidynamics.egg-info/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1117 2023-07-11 12:37:45.000000 tidynamics-1.1.2/tidynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-07-11 12:37:45.000000 tidynamics-1.1.2/tidynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       21 2023-07-11 12:37:45.000000 tidynamics-1.1.2/tidynamics.egg-info/requires.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       11 2023-07-11 12:37:45.000000 tidynamics-1.1.2/tidynamics.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tidynamics-1.0.0/tidynamics.egg-info/PKG-INFO` & `tidynamics-1.1.2/doc/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,116 @@
-Metadata-Version: 2.1
-Name: tidynamics
-Version: 1.0.0
-Summary: Tiny package to compute dynamics correlations
-Home-page: https://pypi.org/project/tidynamics/
-Author: Pierre de Buyl
-Author-email: pdebuyl@pdebuyl.be
-License: BSD
-Description: tidynamics
-        ==========
-        
-        .. image:: http://joss.theoj.org/papers/10.21105/joss.00877/status.svg
-           :target: https://doi.org/10.21105/joss.00877
-           :alt: DOI link to JOSS article
-        
-        .. image:: https://travis-ci.org/pdebuyl-lab/tidynamics.svg?branch=master
-           :target: https://travis-ci.org/pdebuyl-lab/tidynamics
-           :alt: Test status
-        
-        .. image:: https://anaconda.org/conda-forge/tidynamics/badges/version.svg
-           :target: https://anaconda.org/conda-forge/tidynamics
-           :alt: Link to conda-forge page
-        
-        .. image:: https://mybinder.org/badge.svg
-           :target: https://mybinder.org/v2/gh/pdebuyl-lab/tidynamics/master?filepath=doc%2Findex.ipynb
-           :alt: Link to binder example notebook
-        
-        A tiny package to compute the dynamics of stochastic and molecular simulations.
-        
-        :License: BSD 3-clause
-        :Author: Pierre de Buyl
-        :Website: http://lab.pdebuyl.be/tidynamics/
-        
-        tidynamics
-        
-        - performs the computation of mean-square displacements and correlation functions.
-        - accepts as input NumPy arrays storing the positions and velocities of particles.
-        - implements the so-called Fast Correlation Algorithm proposed by Kneller and others for the
-          `nMOLDYN <http://dirac.cnrs-orleans.fr/plone/software/nmoldyn/>`_ analysis program.
-        - depends only `Python <https://www.python.org/>`_ and `NumPy <http://www.numpy.org/>`_.
-        
-        For a quick jump into tidynamics, have a look at the examples.
-        
-        Goals and plans:
-        
-        - Minimal dependencies.
-        - Serve as a reference implementation for common algorithms that are useful for molecular
-          and stochastic simulations.
-        - Provide later a bit more flexibility to handle cross correlations and many-body systems.
-        
-        
-        Installation
-        ------------
-        
-        It is necessary to have Python and NumPy to install and use tidynamics.
-        
-        tidynamics can be installed with pip::
-        
-            pip install --user tidynamics
-        
-        or with conda (via conda-forge)::
-        
-            conda install -c conda-forge tidynamics
-        
-        It is also possible to download the source code and execute the setup.py file.
-        
-        I ran the tests with Python 2.7, 3.5 and 3.6 and NumPy 1.11 and 1.13. If you encounter any
-        issue, let me know (see Contact below).
-        
-        
-        Citation
-        --------
-        
-        When using tidynamics in a publication, please cite the following paper:
-        
-        Pierre de Buyl (2018), *tidynamics: A tiny package to compute the dynamics of
-        stochastic and molecular simulations*, The Journal of Open Source
-        Software https://doi.org/10.21105/joss.00877
-        
-        
-        Testing
-        -------
-        
-        We use `pytest <https://pypi.python.org/pypi/pytest/>`_ for testing::
-        
-            python -m pytest
-        
-        Installing tidynamics does not install the tests. It is necessary to download tidynamics'
-        source and to install pytest to run the tests.
-        
-        Contact, support, and contribution information
-        ----------------------------------------------
-        
-        To contact the author about tidynamics, you can either write an email to `Pierre de Buyl
-        <https://www.kuleuven.be/wieiswie/nl/person/00092351>`_ or use the `issue tracker
-        <https://github.com/pdebuyl-lab/tidynamics/issues>`_ of the GitHub project.
-        Existing contributors are listed in the file CONTRIBUTORS.
-        
-        Bug reports are welcome. If you consider proposing a feature, please keep in mind the goals
-        and plans exposed above.
-        
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/x-rst
+.. tidynamics documentation master file, created by
+   sphinx-quickstart on Sat Dec  9 22:10:27 2017.
+   You can adapt this file completely to your liking, but it should at least
+   contain the root `toctree` directive.
+
+tidynamics
+==========
+
+.. only:: html
+
+   .. image:: http://joss.theoj.org/papers/10.21105/joss.00877/status.svg
+      :target: https://doi.org/10.21105/joss.00877
+      :alt: DOI link to JOSS article
+
+   .. image:: https://github.com/pdebuyl-lab/tidynamics/actions/workflows/test.yml/badge.svg
+      :target: https://github.com/pdebuyl-lab/tidynamics/actions/workflows/test.yml
+      :alt: Test status
+
+   .. image:: https://anaconda.org/conda-forge/tidynamics/badges/version.svg
+      :target: https://anaconda.org/conda-forge/tidynamics
+      :alt: Link to conda-forge page
+
+   .. image:: https://mybinder.org/badge.svg
+      :target: https://mybinder.org/v2/gh/pdebuyl-lab/tidynamics/master?filepath=doc%2Findex.ipynb
+      :alt: Link to binder example notebook
+
+   .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.1401184.svg
+      :target: https://doi.org/10.5281/zenodo.1401184
+      :alt: Link Zenodo archive
+
+
+.. only:: latex
+
+    Introduction
+    ------------
+
+
+A tiny package to compute the dynamics of stochastic and molecular simulations.
+
+:License: BSD 3-clause
+:Author: Pierre de Buyl
+:Website: http://lab.pdebuyl.be/tidynamics/
+:Version: |release|
+
+tidynamics
+
+- performs the computation of mean-square displacements and correlation functions.
+- accepts as input NumPy arrays storing the positions and velocities of particles.
+- implements the so-called Fast Correlation Algorithm proposed by Kneller and others
+  :cite:`nmoldyn_1995` for the `nMOLDYN
+  <http://dirac.cnrs-orleans.fr/nMOLDYN.html>`_ analysis program.
+- depends only `Python <https://www.python.org/>`_ and `NumPy <http://www.numpy.org/>`_.
+
+For a quick jump into tidynamics, have a look at the examples.
+
+Goals and plans:
+
+- Minimal dependencies.
+- Serve as a reference implementation for common algorithms that are useful for molecular
+  and stochastic simulations.
+- Provide later a bit more flexibility to handle cross correlations and many-body systems.
+
+
+Installation
+------------
+
+It is necessary to have Python and NumPy to install and use tidynamics.
+
+tidynamics can be installed with pip::
+
+    pip install --user tidynamics
+
+or with conda (via conda-forge)::
+
+    conda install -c conda-forge tidynamics
+
+It is also possible to download the source code and execute pip locally.
+
+Tests are run with Python 3.7 to 3.11. Python 2 is not supported anymore.  If
+you encounter any issue, let me know (see :ref:`Contact` below).
+
+
+Citation
+--------
+
+When using tidynamics in a publication, please cite the following paper:
+
+Pierre de Buyl (2018), *tidynamics: A tiny package to compute the dynamics of
+stochastic and molecular simulations*, The Journal of Open Source
+Software https://doi.org/10.21105/joss.00877
+
+The BibTeX entry can be found in :download:`CITATION <../CITATION>`.
+
+Testing
+-------
+
+We use `pytest <https://pypi.python.org/pypi/pytest/>`_ for testing::
+
+    python -m pytest
+
+Installing tidynamics does not install the tests. It is necessary to download tidynamics'
+source and to install pytest to run the tests.
+
+.. _contact:
+
+Contact, support, and contribution information
+----------------------------------------------
+
+To contact the author about tidynamics, you can either write an email to `Pierre de Buyl
+<https://www.kuleuven.be/wieiswie/nl/person/00092351>`_ or use the `issue tracker
+<https://github.com/pdebuyl-lab/tidynamics/issues>`_ of the GitHub project.
+
+Bug reports are welcome. If you consider proposing a feature, please keep in mind the goals
+and plans exposed above.
+
+Contributors are listed in :ref:`contributors`.
```

### Comparing `tidynamics-1.0.0/tidynamics/_correlation.py` & `tidynamics-1.1.2/tidynamics/_correlation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import division
 import numpy as np
 from .core import autocorrelation_1d, correlation_1d
 import itertools
 
 def acf(data):
     """Autocorrelation of the input data using the Fast Correlation Algorithm.
 
@@ -44,14 +43,16 @@
     Returns:
         : ndarray of shape (N,) with the MSD for successive linearly spaced time
         delays.
 
     """
 
     pos = np.asarray(pos)
+    if pos.shape[0] == 0:
+        return np.array([], dtype=pos.dtype)
     if pos.ndim==1:
         pos = pos.reshape((-1,1))
     N = len(pos)
     rsq = np.sum(pos**2, axis=1)
     MSD = np.zeros(N, dtype=float)
 
     SAB = autocorrelation_1d(pos[:,0])
```

### Comparing `tidynamics-1.0.0/tidynamics/__init__.py` & `tidynamics-1.1.2/tidynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `tidynamics-1.0.0/tidynamics/core.py` & `tidynamics-1.1.2/tidynamics/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import division
 import numpy as np
 
 def select_power_of_two(n):
     """
     Select the closest i such that n<=2**i
     """
     current_exp = int(np.ceil(np.log2(n+1)))
```

### Comparing `tidynamics-1.0.0/README.rst` & `tidynamics-1.1.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 tidynamics
 ==========
 
 .. image:: http://joss.theoj.org/papers/10.21105/joss.00877/status.svg
    :target: https://doi.org/10.21105/joss.00877
    :alt: DOI link to JOSS article
 
-.. image:: https://travis-ci.org/pdebuyl-lab/tidynamics.svg?branch=master
-   :target: https://travis-ci.org/pdebuyl-lab/tidynamics
+.. image:: https://github.com/pdebuyl-lab/tidynamics/actions/workflows/test.yml/badge.svg
+   :target: https://github.com/pdebuyl-lab/tidynamics/actions/workflows/test.yml
    :alt: Test status
 
 .. image:: https://anaconda.org/conda-forge/tidynamics/badges/version.svg
    :target: https://anaconda.org/conda-forge/tidynamics
    :alt: Link to conda-forge page
 
 .. image:: https://mybinder.org/badge.svg
    :target: https://mybinder.org/v2/gh/pdebuyl-lab/tidynamics/master?filepath=doc%2Findex.ipynb
    :alt: Link to binder example notebook
 
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.1401184.svg
+   :target: https://doi.org/10.5281/zenodo.1401184
+   :alt: Link Zenodo archive
+
 A tiny package to compute the dynamics of stochastic and molecular simulations.
 
 :License: BSD 3-clause
 :Author: Pierre de Buyl
 :Website: http://lab.pdebuyl.be/tidynamics/
 
 tidynamics
 
 - performs the computation of mean-square displacements and correlation functions.
 - accepts as input NumPy arrays storing the positions and velocities of particles.
 - implements the so-called Fast Correlation Algorithm proposed by Kneller and others for the
-  `nMOLDYN <http://dirac.cnrs-orleans.fr/plone/software/nmoldyn/>`_ analysis program.
+  `nMOLDYN <http://dirac.cnrs-orleans.fr/nMOLDYN.html>`_ analysis program.
 - depends only `Python <https://www.python.org/>`_ and `NumPy <http://www.numpy.org/>`_.
 
 For a quick jump into tidynamics, have a look at the examples.
 
 Goals and plans:
 
 - Minimal dependencies.
@@ -50,19 +54,18 @@
 
     pip install --user tidynamics
 
 or with conda (via conda-forge)::
 
     conda install -c conda-forge tidynamics
 
-It is also possible to download the source code and execute the setup.py file.
-
-I ran the tests with Python 2.7, 3.5 and 3.6 and NumPy 1.11 and 1.13. If you encounter any
-issue, let me know (see Contact below).
-
+It is also possible to download the source code and execute pip locally.
+ 
+Tests are run with Python 3.7 to 3.11. Python 2 is not supported anymore.  If
+you encounter any issue, let me know (see Contact below).
 
 Citation
 --------
 
 When using tidynamics in a publication, please cite the following paper:
 
 Pierre de Buyl (2018), *tidynamics: A tiny package to compute the dynamics of
```

### Comparing `tidynamics-1.0.0/LICENSE` & `tidynamics-1.1.2/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2017,2018 Pierre de Buyl
+Copyright (c) 2017,2018,2023 Pierre de Buyl
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
 1. Redistributions of source code must retain the above copyright
 notice, this list of conditions and the following disclaimer.
```

