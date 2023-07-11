# Comparing `tmp/textnets-0.9.2.tar.gz` & `tmp/textnets-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textnets-0.9.2.tar", max compression
+gzip compressed data, was "textnets-0.9.3.tar", max compression
```

## Comparing `textnets-0.9.2.tar` & `textnets-0.9.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      264 2023-06-28 14:05:40.319017 textnets-0.9.2/AUTHORS.rst
--rw-r--r--   0        0        0     3868 2023-06-28 14:05:40.319017 textnets-0.9.2/CONTRIBUTING.rst
--rw-r--r--   0        0        0    13834 2023-06-28 14:05:40.319017 textnets-0.9.2/HISTORY.rst
--rw-r--r--   0        0        0    35149 2023-06-28 14:05:40.319017 textnets-0.9.2/LICENSE
--rw-r--r--   0        0        0     4474 2023-06-28 14:05:40.319017 textnets-0.9.2/README.rst
--rw-r--r--   0        0        0      296 2023-06-28 14:05:40.319017 textnets-0.9.2/build.py
--rw-r--r--   0        0        0  1210458 2023-06-28 14:05:40.323017 textnets-0.9.2/docs/_static/impeachment-statements.svg
--rw-r--r--   0        0        0     5739 2023-06-28 14:05:40.323017 textnets-0.9.2/docs/_static/textnets-logo.svg
--rw-r--r--   0        0        0     7854 2023-06-28 14:05:40.323017 textnets-0.9.2/docs/advanced.rst
--rw-r--r--   0        0        0       28 2023-06-28 14:05:40.323017 textnets-0.9.2/docs/authors.rst
--rw-r--r--   0        0        0       78 2023-06-28 14:05:40.323017 textnets-0.9.2/docs/bibliography.rst
--rwxr-xr-x   0        0        0     5433 2023-06-28 14:05:40.323017 textnets-0.9.2/docs/conf.py
--rw-r--r--   0        0        0       33 2023-06-28 14:05:40.323017 textnets-0.9.2/docs/contributing.rst
--rw-r--r--   0        0        0       28 2023-06-28 14:05:40.323017 textnets-0.9.2/docs/history.rst
--rw-r--r--   0        0        0      290 2023-06-28 14:05:40.327017 textnets-0.9.2/docs/index.rst
--rw-r--r--   0        0        0     3826 2023-06-28 14:05:40.327017 textnets-0.9.2/docs/installation.rst
--rw-r--r--   0        0        0      102 2023-06-28 14:05:40.327017 textnets-0.9.2/docs/license.rst
--rw-r--r--   0        0        0      105 2023-06-28 14:05:40.327017 textnets-0.9.2/docs/reference.rst
--rw-r--r--   0        0        0     4423 2023-06-28 14:05:40.327017 textnets-0.9.2/docs/refs.bib
--rw-r--r--   0        0        0     5625 2023-06-28 14:05:40.327017 textnets-0.9.2/docs/textnets-logo-sm.svg
--rw-r--r--   0        0        0    15533 2023-06-28 14:05:40.327017 textnets-0.9.2/docs/tutorial.rst
--rw-r--r--   0        0        0     2828 2023-06-28 14:05:40.327017 textnets-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       38 2023-06-28 14:05:40.327017 textnets-0.9.2/tests/__init__.py
--rw-r--r--   0        0        0      291 2023-06-28 14:05:40.327017 textnets-0.9.2/tests/conftest.py
--rw-r--r--   0        0        0    11722 2023-06-28 14:05:40.327017 textnets-0.9.2/tests/test_textnets.py
--rw-r--r--   0        0        0     1771 2023-06-28 14:05:40.327017 textnets-0.9.2/textnets/__init__.py
--rw-r--r--   0        0        0       47 2023-06-28 14:05:40.327017 textnets-0.9.2/textnets/_ext.pxd
--rw-r--r--   0        0        0      215 2023-06-28 14:05:40.327017 textnets-0.9.2/textnets/_ext.pyx
--rw-r--r--   0        0        0     2488 2023-06-28 14:05:40.327017 textnets-0.9.2/textnets/_util.py
--rw-r--r--   0        0        0     3999 2023-06-28 14:05:40.327017 textnets-0.9.2/textnets/config.py
--rw-r--r--   0        0        0    22166 2023-06-28 14:05:40.327017 textnets-0.9.2/textnets/corpus.py
--rw-r--r--   0        0        0     6093 2023-06-28 14:05:40.327017 textnets-0.9.2/textnets/examples.py
--rw-r--r--   0        0        0     1367 2023-06-28 14:05:40.327017 textnets-0.9.2/textnets/fca.py
--rw-r--r--   0        0        0    34740 2023-06-28 14:05:40.327017 textnets-0.9.2/textnets/network.py
--rw-r--r--   0        0        0     8954 2023-06-28 14:05:40.327017 textnets-0.9.2/textnets/viz.py
--rw-r--r--   0        0        0     5740 1970-01-01 00:00:00.000000 textnets-0.9.2/setup.py
--rw-r--r--   0        0        0     6548 1970-01-01 00:00:00.000000 textnets-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-07-11 10:11:23.220004 textnets-0.9.3/AUTHORS.rst
+-rw-r--r--   0        0        0     3868 2023-07-11 10:11:23.220004 textnets-0.9.3/CONTRIBUTING.rst
+-rw-r--r--   0        0        0    14088 2023-07-11 10:11:23.224004 textnets-0.9.3/HISTORY.rst
+-rw-r--r--   0        0        0    35149 2023-07-11 10:11:23.224004 textnets-0.9.3/LICENSE
+-rw-r--r--   0        0        0     4474 2023-07-11 10:11:23.224004 textnets-0.9.3/README.rst
+-rw-r--r--   0        0        0      296 2023-07-11 10:11:23.224004 textnets-0.9.3/build.py
+-rw-r--r--   0        0        0  1210458 2023-07-11 10:11:23.228004 textnets-0.9.3/docs/_static/impeachment-statements.svg
+-rw-r--r--   0        0        0     5739 2023-07-11 10:11:23.228004 textnets-0.9.3/docs/_static/textnets-logo.svg
+-rw-r--r--   0        0        0     7854 2023-07-11 10:11:23.228004 textnets-0.9.3/docs/advanced.rst
+-rw-r--r--   0        0        0       28 2023-07-11 10:11:23.228004 textnets-0.9.3/docs/authors.rst
+-rw-r--r--   0        0        0       78 2023-07-11 10:11:23.228004 textnets-0.9.3/docs/bibliography.rst
+-rwxr-xr-x   0        0        0     5433 2023-07-11 10:11:23.228004 textnets-0.9.3/docs/conf.py
+-rw-r--r--   0        0        0       33 2023-07-11 10:11:23.228004 textnets-0.9.3/docs/contributing.rst
+-rw-r--r--   0        0        0       28 2023-07-11 10:11:23.228004 textnets-0.9.3/docs/history.rst
+-rw-r--r--   0        0        0      290 2023-07-11 10:11:23.228004 textnets-0.9.3/docs/index.rst
+-rw-r--r--   0        0        0     3826 2023-07-11 10:11:23.228004 textnets-0.9.3/docs/installation.rst
+-rw-r--r--   0        0        0      102 2023-07-11 10:11:23.228004 textnets-0.9.3/docs/license.rst
+-rw-r--r--   0        0        0      105 2023-07-11 10:11:23.228004 textnets-0.9.3/docs/reference.rst
+-rw-r--r--   0        0        0     4423 2023-07-11 10:11:23.228004 textnets-0.9.3/docs/refs.bib
+-rw-r--r--   0        0        0     5625 2023-07-11 10:11:23.228004 textnets-0.9.3/docs/textnets-logo-sm.svg
+-rw-r--r--   0        0        0    15533 2023-07-11 10:11:23.228004 textnets-0.9.3/docs/tutorial.rst
+-rw-r--r--   0        0        0     2939 2023-07-11 10:11:23.228004 textnets-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-07-11 10:11:23.228004 textnets-0.9.3/tests/__init__.py
+-rw-r--r--   0        0        0      291 2023-07-11 10:11:23.228004 textnets-0.9.3/tests/conftest.py
+-rw-r--r--   0        0        0    11722 2023-07-11 10:11:23.228004 textnets-0.9.3/tests/test_textnets.py
+-rw-r--r--   0        0        0     1771 2023-07-11 10:11:23.232004 textnets-0.9.3/textnets/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-11 10:11:23.232004 textnets-0.9.3/textnets/_ext.pxd
+-rw-r--r--   0        0        0      215 2023-07-11 10:11:23.232004 textnets-0.9.3/textnets/_ext.pyx
+-rw-r--r--   0        0        0     2488 2023-07-11 10:11:23.232004 textnets-0.9.3/textnets/_util.py
+-rw-r--r--   0        0        0     3999 2023-07-11 10:11:23.232004 textnets-0.9.3/textnets/config.py
+-rw-r--r--   0        0        0    22208 2023-07-11 10:11:23.232004 textnets-0.9.3/textnets/corpus.py
+-rw-r--r--   0        0        0     6093 2023-07-11 10:11:23.232004 textnets-0.9.3/textnets/examples.py
+-rw-r--r--   0        0        0     1367 2023-07-11 10:11:23.232004 textnets-0.9.3/textnets/fca.py
+-rw-r--r--   0        0        0    34740 2023-07-11 10:11:23.232004 textnets-0.9.3/textnets/network.py
+-rw-r--r--   0        0        0     8954 2023-07-11 10:11:23.232004 textnets-0.9.3/textnets/viz.py
+-rw-r--r--   0        0        0     5777 1970-01-01 00:00:00.000000 textnets-0.9.3/setup.py
+-rw-r--r--   0        0        0     6599 1970-01-01 00:00:00.000000 textnets-0.9.3/PKG-INFO
```

### Comparing `textnets-0.9.2/CONTRIBUTING.rst` & `textnets-0.9.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/HISTORY.rst` & `textnets-0.9.3/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =======
 History
 =======
 
+=======
+0.9.3 (unreleased)
+------------------
+* Updates to igraph 0.10.5.
+* Updates to spaCy 3.6.0, bringing support for Slovenian.
+* Add dependency on ``spacy-lookups-data`` for better support of languages
+  without pre-trained models (e.g., Turkish).
+
 0.9.2 (2023-06-28)
 ------------------
 * Improves documentation.
 * Updates to scipy 1.10.
 * Fixes how the compiled extension is built.
 
 0.9.1 (2023-06-16)
```

### Comparing `textnets-0.9.2/LICENSE` & `textnets-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/README.rst` & `textnets-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/docs/_static/impeachment-statements.svg` & `textnets-0.9.3/docs/_static/impeachment-statements.svg`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/docs/_static/textnets-logo.svg` & `textnets-0.9.3/docs/_static/textnets-logo.svg`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/docs/advanced.rst` & `textnets-0.9.3/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/docs/conf.py` & `textnets-0.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/docs/installation.rst` & `textnets-0.9.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/docs/refs.bib` & `textnets-0.9.3/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/docs/textnets-logo-sm.svg` & `textnets-0.9.3/docs/textnets-logo-sm.svg`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/docs/tutorial.rst` & `textnets-0.9.3/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/pyproject.toml` & `textnets-0.9.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "textnets"
-version = "0.9.2"
+version = "0.9.3"
 description = "Automated text analysis with networks"
 license = "GNU General Public License v3"
 keywords = [
     "computational social science",
     "network analysis",
     "nlp",
     "text analysis",
@@ -29,50 +29,49 @@
     "Topic :: Sociology"
 ]
 homepage = "https://textnets.readthedocs.io"
 repository = "https://github.com/jboynyc/textnets"
 authors = ["John D. Boy <jboy@bius.moe>"]
 readme = "README.rst"
 include = [
-    "docs/*.rst",
+    { path = "textnets/_ext*.so", format = "wheel" },
     "docs/*.py",
     "docs/refs.bib",
-    "docs/*.svg",
+    "docs/*.rst",
     "docs/_static",
+    "docs/*.svg",
     "LICENSE",
     "*.rst",
-    "tests/*.py"
-]
-exclude = [
-    "textnets/_ext.c"
+    "tests/*.py",
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/jboynyc/textnets/issues"
 "Changelog" = "https://textnets.readthedocs.io/en/stable/history.html"
 "Documentation" = "https://textnets.readthedocs.io"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 setuptools = ">=41"
 Cython = "^0.29.24"
-igraph = "^0.10.4"
-leidenalg = "^0.9.0"
-pandas = "^2.0.1"
 cairocffi = {version = "^1.4.0", markers = "sys_platform=='linux' or sys_platform=='darwin'"}
 pycairo = {version = "^1.22.0", markers = "sys_platform=='win32'"}
+igraph = "^0.10.5"
+leidenalg = "^0.9.0"
+pandas = "^2.0.1"
 scipy = "^1.10.0"
-spacy = "^3.5.3"
+spacy = "^3.6.0"
+spacy-lookups-data = "^1.0.3"
 toolz = "^0.12.0"
 tqdm = "^4.64.1"
 wasabi = ">=0.10.1"
 concepts = {version = "^0.9.2", optional = true}
 
 [tool.poetry.group.doc.dependencies]
-en-core-web-sm = {url = "https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.5.0/en_core_web_sm-3.5.0.tar.gz"}
+en-core-web-sm = {url = "https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.6.0/en_core_web_sm-3.6.0-py3-none-any.whl"}
 ipykernel = "^6.22.0"
 jupyter-sphinx = "^0.4.0"
 shibuya = {version = "^2023.6.25", allow-prereleases = true}
 sphinx = "^7.0.0"
 sphinxcontrib-bibtex = "^2.3.0"
 
 [tool.poetry.group.dev.dependencies]
@@ -100,7 +99,12 @@
 
 [tool.mypy]
 files = "textnets"
 warn_unused_ignores = true
 warn_unreachable = true
 ignore_missing_imports = true
 pretty = true
+
+[tool.ufmt]
+excludes = [
+    "textnets/_ext*.so"
+]
```

### Comparing `textnets-0.9.2/tests/test_textnets.py` & `textnets-0.9.3/tests/test_textnets.py`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/textnets/__init__.py` & `textnets-0.9.3/textnets/__init__.py`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/textnets/_util.py` & `textnets-0.9.3/textnets/_util.py`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/textnets/config.py` & `textnets-0.9.3/textnets/config.py`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/textnets/corpus.py` & `textnets-0.9.3/textnets/corpus.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     "mk": "mk_core_news_sm",  # Macedonian
     "nb": "nb_core_news_sm",  # Norwegian
     "nl": "nl_core_news_sm",  # Dutch
     "pl": "pl_core_news_sm",  # Polish
     "pt": "pt_core_news_sm",  # Portuguese
     "ro": "ro_core_news_sm",  # Romanian
     "ru": "ru_core_news_sm",  # Russian
+    "sl": "sl_core_news_sm",  # Slovenian
     "sv": "sv_core_news_sm",  # Swedish
     "uk": "uk_core_news_sm",  # Ukrainian
     "zh": "zh_core_web_sm",  # Chinese
 }
 
 #: Custom type for objects resembling documents (token sequences).
 DocLike = Union[Doc, Sequence[Token]]
```

### Comparing `textnets-0.9.2/textnets/examples.py` & `textnets-0.9.3/textnets/examples.py`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/textnets/fca.py` & `textnets-0.9.3/textnets/fca.py`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/textnets/network.py` & `textnets-0.9.3/textnets/network.py`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/textnets/viz.py` & `textnets-0.9.3/textnets/viz.py`

 * *Files identical despite different names*

### Comparing `textnets-0.9.2/setup.py` & `textnets-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 ['textnets']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Cython>=0.29.24,<0.30.0',
- 'igraph>=0.10.4,<0.11.0',
+ 'igraph>=0.10.5,<0.11.0',
  'leidenalg>=0.9.0,<0.10.0',
  'pandas>=2.0.1,<3.0.0',
  'scipy>=1.10.0,<2.0.0',
  'setuptools>=41',
- 'spacy>=3.5.3,<4.0.0',
+ 'spacy-lookups-data>=1.0.3,<2.0.0',
+ 'spacy>=3.6.0,<4.0.0',
  'toolz>=0.12.0,<0.13.0',
  'tqdm>=4.64.1,<5.0.0',
  'wasabi>=0.10.1']
 
 extras_require = \
 {':sys_platform == "linux" or sys_platform == "darwin"': ['cairocffi>=1.4.0,<2.0.0'],
  ':sys_platform == "win32"': ['pycairo>=1.22.0,<2.0.0'],
  'fca': ['concepts>=0.9.2,<0.10.0']}
 
 setup_kwargs = {
     'name': 'textnets',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'Automated text analysis with networks',
     'long_description': '=====================================\nTextnets: text analysis with networks\n=====================================\n\n.. image:: https://mybinder.org/badge_logo.svg\n   :target: https://mybinder.org/v2/gh/jboynyc/textnets-binder/trunk?filepath=Tutorial.ipynb\n   :alt: Launch on Binder\n\n.. image:: https://github.com/jboynyc/textnets/actions/workflows/ci.yml/badge.svg\n   :target: https://github.com/jboynyc/textnets/actions/workflows/ci.yml\n   :alt: CI status\n\n.. image:: https://readthedocs.org/projects/textnets/badge/?version=stable\n   :target: https://textnets.readthedocs.io/en/stable/?badge=stable\n   :alt: Documentation Status\n\n.. image:: https://anaconda.org/conda-forge/textnets/badges/version.svg\n   :target: https://anaconda.org/conda-forge/textnets\n   :alt: Install with conda\n\n.. image:: https://joss.theoj.org/papers/10.21105/joss.02594/status.svg\n   :target: https://doi.org/10.21105/joss.02594\n   :alt: Published in Journal of Open Source Software\n\n**textnets** represents collections of texts as networks of documents and\nwords. This provides novel possibilities for the visualization and analysis of\ntexts.\n\n.. figure:: https://textnets.readthedocs.io/en/dev/_static/impeachment-statements.svg\n   :alt: Bipartite network graph\n\n   Network of U.S. Senators and words used in their official statements\n   following the acquittal vote in the 2020 Senate impeachment trial (`source\n   <https://www.jboy.space/blog/enemies-foreign-and-partisan.html>`_).\n\n**textnets** is free software under the terms of the GNU General Public License\nv3.\n\nThe ideas underlying **textnets** are presented in this paper:\n\n  Christopher A. Bail, "`Combining natural language processing and network\n  analysis to examine how advocacy organizations stimulate conversation on social\n  media`__," *Proceedings of the National Academy of Sciences of the United States\n  of America* 113, no. 42 (2016), 11823–11828, doi:10.1073/pnas.1607151113.\n\n__ https://doi.org/10.1073/pnas.1607151113\n\nInitially begun as a Python implementation of `Chris Bail\'s textnets package\nfor R`_, **textnets** now comprises several unique features for term extraction\nand weighing, visualization, and analysis.\n\n.. _`Chris Bail\'s textnets package for R`: https://github.com/cbail/textnets/\n\nFeatures\n--------\n\n**textnets** builds on `spaCy`_, a state-of-the-art library for\nnatural-language processing, and `igraph`_ for network analysis. It uses the\n`Leiden algorithm`_ for community detection, which is able to perform community\ndetection on the bipartite (word–group) network.\n\n.. _`igraph`: http://igraph.org/python/\n.. _`Leiden algorithm`: https://doi.org/10.1038/s41598-019-41695-z\n.. _`spaCy`: https://spacy.io/\n\n**textnets** is installable using the ``conda``, ``pip`` and ``nix`` package\nmanagers. It requires Python 3.8 or higher.\n\n**textnets** integrates seamlessly with Python\'s excellent `scientific stack`_.\nThat means that you can use **textnets** to analyze and visualize your data in\nJupyter notebooks!\n\n.. _`scientific stack`: https://scientific-python.org\n\nRead `the documentation <https://textnets.readthedocs.io>`_ to learn more about\nthe package\'s features.\n\nCitation\n--------\n\nUsing **textnets** in a scholarly publication? Please cite this paper:\n\n.. code-block:: bibtex\n\n   @article{Boy2020,\n     author   = {John D. Boy},\n     title    = {textnets},\n     subtitle = {A {P}ython Package for Text Analysis with Networks},\n     journal  = {Journal of Open Source Software},\n     volume   = {5},\n     number   = {54},\n     pages    = {2594},\n     year     = {2020},\n     doi      = {10.21105/joss.02594},\n   }\n\nLearn More\n----------\n\n==================  =============================================\n**Documentation**   https://textnets.readthedocs.io/\n**Repository**      https://github.com/jboynyc/textnets\n**Issues & Ideas**  https://github.com/jboynyc/textnets/issues\n**Conda-Forge**     https://anaconda.org/conda-forge/textnets\n**PyPI**            https://pypi.org/project/textnets/\n**FOSDEM ’22**      https://fosdem.org/2022/schedule/event/open_research_textnets/\n**DOI**             `10.21105/joss.02594 <https://doi.org/10.21105/joss.02594>`_\n**Archive**         `10.5281/zenodo.3866676 <https://doi.org/10.5281/zenodo.3866676>`_\n==================  =============================================\n\n.. image:: https://textnets.readthedocs.io/en/dev/_static/textnets-logo.svg\n   :alt: textnets logo\n   :target: https://textnets.readthedocs.io\n   :align: center\n   :width: 140\n',
     'author': 'John D. Boy',
     'author_email': 'jboy@bius.moe',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://textnets.readthedocs.io',
```

### Comparing `textnets-0.9.2/PKG-INFO` & `textnets-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textnets
-Version: 0.9.2
+Version: 0.9.3
 Summary: Automated text analysis with networks
 Home-page: https://textnets.readthedocs.io
 License: GNU General Public License v3
 Keywords: computational social science,network analysis,nlp,text analysis,visualization
 Author: John D. Boy
 Author-email: jboy@bius.moe
 Requires-Python: >=3.8.1,<3.12
@@ -24,21 +24,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Sociology
 Provides-Extra: fca
 Requires-Dist: Cython (>=0.29.24,<0.30.0)
 Requires-Dist: cairocffi (>=1.4.0,<2.0.0) ; sys_platform == "linux" or sys_platform == "darwin"
 Requires-Dist: concepts (>=0.9.2,<0.10.0) ; extra == "fca"
-Requires-Dist: igraph (>=0.10.4,<0.11.0)
+Requires-Dist: igraph (>=0.10.5,<0.11.0)
 Requires-Dist: leidenalg (>=0.9.0,<0.10.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pycairo (>=1.22.0,<2.0.0) ; sys_platform == "win32"
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Requires-Dist: setuptools (>=41)
-Requires-Dist: spacy (>=3.5.3,<4.0.0)
+Requires-Dist: spacy (>=3.6.0,<4.0.0)
+Requires-Dist: spacy-lookups-data (>=1.0.3,<2.0.0)
 Requires-Dist: toolz (>=0.12.0,<0.13.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: wasabi (>=0.10.1)
 Project-URL: Bug Tracker, https://github.com/jboynyc/textnets/issues
 Project-URL: Changelog, https://textnets.readthedocs.io/en/stable/history.html
 Project-URL: Documentation, https://textnets.readthedocs.io
 Project-URL: Repository, https://github.com/jboynyc/textnets
```

