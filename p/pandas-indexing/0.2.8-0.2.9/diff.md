# Comparing `tmp/pandas-indexing-0.2.8.tar.gz` & `tmp/pandas-indexing-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-indexing-0.2.8.tar", last modified: Sat Jun 24 12:01:24 2023, max compression
+gzip compressed data, was "pandas-indexing-0.2.9.tar", last modified: Tue Jul 11 12:33:58 2023, max compression
```

## Comparing `pandas-indexing-0.2.8.tar` & `pandas-indexing-0.2.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.918776 pandas-indexing-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-24 12:01:24.918776 pandas-indexing-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.914776 pandas-indexing-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/AUTHORS.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.914776 pandas-indexing-0.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.914776 pandas-indexing-0.2.8/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   362710 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/notebooks/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 12:01:24.918776 pandas-indexing-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.914776 pandas-indexing-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.918776 pandas-indexing-0.2.8/src/pandas_indexing/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.918776 pandas-indexing-0.2.8/src/pandas_indexing/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/datasets/remindhighre_power.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-24 12:01:02.000000 pandas-indexing-0.2.8/src/pandas_indexing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:01:24.918776 pandas-indexing-0.2.8/src/pandas_indexing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-24 12:01:24.000000 pandas-indexing-0.2.8/src/pandas_indexing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-24 12:01:24.000000 pandas-indexing-0.2.8/src/pandas_indexing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 12:01:24.000000 pandas-indexing-0.2.8/src/pandas_indexing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-24 12:01:24.000000 pandas-indexing-0.2.8/src/pandas_indexing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-24 12:01:24.000000 pandas-indexing-0.2.8/src/pandas_indexing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:33:58.543812 pandas-indexing-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-11 12:33:58.543812 pandas-indexing-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:33:58.539812 pandas-indexing-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/docs/AUTHORS.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:33:58.539812 pandas-indexing-0.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:33:58.539812 pandas-indexing-0.2.9/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   362710 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/docs/notebooks/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 12:33:58.543812 pandas-indexing-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:33:58.539812 pandas-indexing-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:33:58.543812 pandas-indexing-0.2.9/src/pandas_indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/src/pandas_indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/src/pandas_indexing/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/src/pandas_indexing/arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21351 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/src/pandas_indexing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:33:58.543812 pandas-indexing-0.2.9/src/pandas_indexing/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/src/pandas_indexing/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/src/pandas_indexing/datasets/remindhighre_power.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/src/pandas_indexing/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/src/pandas_indexing/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/src/pandas_indexing/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-11 12:33:39.000000 pandas-indexing-0.2.9/src/pandas_indexing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:33:58.543812 pandas-indexing-0.2.9/src/pandas_indexing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-11 12:33:58.000000 pandas-indexing-0.2.9/src/pandas_indexing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-11 12:33:58.000000 pandas-indexing-0.2.9/src/pandas_indexing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:33:58.000000 pandas-indexing-0.2.9/src/pandas_indexing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-11 12:33:58.000000 pandas-indexing-0.2.9/src/pandas_indexing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 12:33:58.000000 pandas-indexing-0.2.9/src/pandas_indexing.egg-info/top_level.txt
```

### Comparing `pandas-indexing-0.2.8/CHANGELOG.rst` & `pandas-indexing-0.2.9/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 .. currentmodule:: pandas_indexing
 
 Changelog
 =========
 
+v0.2.9 (2023-07-11)
+------------------------------------------------------------
+* Rename pandas accessor to ``.pix`` (``.idx`` is as of now deprecated, but available
+  for the time being) in :pull:`27`.
+* Fix :func:`~core.projectlevel` on columns of a ``DataFrame`` :pull:`28`
+
 v0.2.8 (2023-06-24)
 ------------------------------------------------------------
 * Units can be converted with :func:`~units.convert_unit`, like f.ex.
   ``convert_unit(df, "km / h")`` or with ``convert_unit(df, {"m / s": "km / h"})``
   to convert only data with the ``m / s`` unit
-* If the openscm-units registry is registered as pint application registry then emission conversion between gas species are possible under the correct contexts:
+* If the openscm-units registry is registered as pint application registry then emission
+  conversion between gas species are possible under the correct contexts:
 
 .. code-block:: python
 
     from pandas_indexing import set_openscm_registry_as_default, convert_unit
 
     ur = set_openscm_registry_as_default()
     with ur.context("AR6GWP100"):
         df = convert_unit(df, "Mt CO2e/yr")  # or df = df.idx.convert_unit("Mt CO2e/yr")
 
 * To use unit conversion, you should install with ``pip install "pandas-indexing[units]"``
   to pull in the optional ``pint`` and ``openscm-units`` dependencies
-* For more information about unit handling, refer to :py:mod:`~pandas_indexing.units` or check the code
-  added in :pull:`17`
+* For more information about unit handling, refer to
+  :py:mod:`~pandas_indexing.units` or check the code added in :pull:`17`
 * Documentation fixes: MyST notebook rendering from :pull:`20` and new docs for
   :func:`~core.extractlevel` in :pull:`21`.
 * Bug fixes: :func:`~core.semijoin`, :func:`~core.concat` and :func:`~selectors.ismatch`
   are working again as advertised :pull:`21` and :pull:`24`.
 
 v0.2.7 (2023-05-26)
 ------------------------------------------------------------
```

### Comparing `pandas-indexing-0.2.8/CODE_OF_CONDUCT.md` & `pandas-indexing-0.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.8/CONTRIBUTING.rst` & `pandas-indexing-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.8/LICENSE` & `pandas-indexing-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.8/PKG-INFO` & `pandas-indexing-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.8
+Version: 0.2.9
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
```

### Comparing `pandas-indexing-0.2.8/README.rst` & `pandas-indexing-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.8/docs/api.rst` & `pandas-indexing-0.2.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.8/docs/conf.py` & `pandas-indexing-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.8/docs/notebooks/introduction.ipynb` & `pandas-indexing-0.2.9/docs/notebooks/introduction.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995002876042566%*

 * *Differences: {"'cells'": '{4: {\'source\': {insert: [(14, \'   df.pix.assign(unit="Mt CO2e/yr)\\n\')], delete: '*

 * *            '[14]}}, 14: {\'source\': {insert: [(3, \'# or: df.pix.extract(variable="Secondary '*

 * *            'Energy|{carrier}|{fuel}")\\n\')], delete: [3]}}, 16: {\'source\': {insert: [(1, \'# '*

 * *            'or: df.pix.format(variable="Secondary Energy|{carrier}|{fuel}")\')], delete: [1]}}, '*

 * *            "33: {'source': {insert: [(4, ')  # or: fossil_series.pix.semijoin(idx, "*

 * *            'how="right")\')],  […]*

```diff
@@ -368,15 +368,15 @@
                 "   from pandas_indexing import assignlevel\n",
                 "   assignlevel(df, unit=\"Mt CO2e/yr\")\n",
                 "   ```\n",
                 "2. convenience accessors that are hooking into pandas as extensions, like\n",
                 "   \n",
                 "   ```python\n",
                 "   import pandas_indexing.accessors\n",
-                "   df.idx.assign(unit=\"Mt CO2e/yr)\n",
+                "   df.pix.assign(unit=\"Mt CO2e/yr)\n",
                 "   ```\n",
                 "\n",
                 "Most of the functionality is available with both styles under slightly different names. I'll present the functional style here first (and add the alternative as comments)"
             ]
         },
         {
             "cell_type": "code",
@@ -1515,15 +1515,15 @@
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from pandas_indexing import extractlevel, formatlevel\n",
                 "\n",
                 "splitdf = extractlevel(df, variable=\"Secondary Energy|{carrier}|{fuel}\", drop=True)\n",
-                "# or: df.idx.extract(variable=\"Secondary Energy|{carrier}|{fuel}\")\n",
+                "# or: df.pix.extract(variable=\"Secondary Energy|{carrier}|{fuel}\")\n",
                 "splitdf"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "405720c7",
@@ -2016,15 +2016,15 @@
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "formatlevel(splitdf, variable=\"Secondary Energy|{carrier}|{fuel}\", drop=True)\n",
-                "# or: df.idx.format(variable=\"Secondary Energy|{carrier}|{fuel}\")"
+                "# or: df.pix.format(variable=\"Secondary Energy|{carrier}|{fuel}\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "e78ace7d",
             "metadata": {},
@@ -2710,15 +2710,15 @@
                 }
             ],
             "source": [
                 "from pandas_indexing import semijoin\n",
                 "\n",
                 "semijoin(\n",
                 "    fossil_series, idx, how=\"right\"\n",
-                ")  # or: fossil_series.idx.semijoin(idx, how=\"right\")"
+                ")  # or: fossil_series.pix.semijoin(idx, how=\"right\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "cbaa73b0",
             "metadata": {},
@@ -2792,15 +2792,15 @@
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from pandas_indexing import projectlevel\n",
                 "\n",
                 "simple_fossil_series = projectlevel(fossil_series, [\"variable\", \"year\"])\n",
-                "# or: fossil_series.idx.project([\"variable\", \"year\"])\n",
+                "# or: fossil_series.pix.project([\"variable\", \"year\"])\n",
                 "simple_fossil_series"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "715fe070",
@@ -3711,15 +3711,15 @@
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from pandas_indexing import assignlevel\n",
                 "\n",
                 "assignlevel(df, variable=\"Updated|\" + projectlevel(df.index, \"variable\"), unit=\"bla\")\n",
-                "# or: df.idx.assign(variable=df.index.idx.project(\"variable\"), unit=\"bla\")"
+                "# or: df.pix.assign(variable=df.index.pix.project(\"variable\"), unit=\"bla\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "1349c89d",
             "metadata": {},
@@ -4582,15 +4582,15 @@
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from pandas_indexing import formatlevel\n",
                 "\n",
                 "formatlevel(df, variable=\"Updated|{variable}\", unit=\"bla\")\n",
-                "# or: df.idx.format(variable=...)"
+                "# or: df.pix.format(variable=...)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "a8416465",
             "metadata": {},
@@ -5515,15 +5515,15 @@
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from pandas_indexing import uniquelevel\n",
                 "\n",
                 "uniquelevel(df, \"variable\")\n",
-                "# or: df.idx.unique(\"variable\")\n",
+                "# or: df.pix.unique(\"variable\")\n",
                 "# or in vanilla pandas: df.index.unique(\"variable\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 28,
             "id": "23378320",
```

### Comparing `pandas-indexing-0.2.8/pyproject.toml` & `pandas-indexing-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.8/src/pandas_indexing/__init__.py` & `pandas-indexing-0.2.9/src/pandas_indexing/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.8/src/pandas_indexing/accessors.py` & `pandas-indexing-0.2.9/src/pandas_indexing/accessors.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-"""Registers convenience accessors into the ``idx`` namespace of each pandas
+"""Registers convenience accessors into the ``pix`` namespace of each pandas
 object.
 
 Examples
 --------
->>> df.idx.project(["model", "scenario"])
+>>> df.pix.project(["model", "scenario"])
 
->>> df.index.idx.assign(unit="Mt CO2")
+>>> df.index.pix.assign(unit="Mt CO2")
 
->>> df.idx.multiply(other, how="left")
+>>> df.pix.multiply(other, how="left")
 """
 
 from typing import Any, Callable, Literal, Mapping, Optional, Sequence, Union
 
 import pandas as pd
+from deprecated.sphinx import deprecated
 from pandas import DataFrame, Index, MultiIndex, Series
 
 from . import arithmetics
 from .core import (
     assignlevel,
     describelevel,
     dropnalevel,
     extractlevel,
+    fixindexna,
     formatlevel,
     isna,
     notna,
     projectlevel,
     semijoin,
     uniquelevel,
 )
 from .types import Axis, Data
 from .units import convert_unit, dequantify, quantify
 from .utils import doc
 
 
-class _IdxAccessor:
+class _PixAccessor:
     """
     Convenience accessor for accessing `pandas-indexing` functions.
     """
 
     def __init__(self, pandas_obj):
         self._obj = pandas_obj
 
@@ -105,16 +107,23 @@
         self,
         subset: Optional[Sequence[str]] = None,
         how: Literal["any", "all"] = "any",
         axis: Axis = 0,
     ) -> Union[DataFrame, Series, Index]:
         return dropnalevel(self._obj, subset=subset, how=how, axis=axis)
 
+    @doc(fixindexna, index_or_data="")
+    def fixna(
+        self,
+        axis: Axis = 0,
+    ) -> Union[DataFrame, Series, Index]:
+        return fixindexna(self._obj, axis=axis)
+
 
-class _DataIdxAccessor(_IdxAccessor):
+class _DataPixAccessor(_PixAccessor):
     @doc(semijoin, frame_or_series="")
     def semijoin(
         self,
         other: Index,
         *,
         how: Literal["left", "right", "inner", "outer"] = "left",
         level: Union[str, int, None] = None,
@@ -131,15 +140,15 @@
 
     def add(self, other, **align_kwds):
         return arithmetics.add(self._obj, other, **align_kwds)
 
     def subtract(self, other, **align_kwds):
         return arithmetics.subtract(self._obj, other, **align_kwds)
 
-    @doc(quantify, data="", example_call="s.idx.quantify()")
+    @doc(quantify, data="", example_call="s.pix.quantify()")
     def quantify(
         self,
         level: str = "unit",
         unit: Optional[str] = None,
         axis: Axis = 0,
         copy: bool = False,
     ):
@@ -147,32 +156,55 @@
 
     def dequantify(self, level: str = "unit", axis: Axis = 0, copy: bool = False):
         return dequantify(self._obj, level=level, axis=axis, copy=copy)
 
     @doc(
         convert_unit,
         data="",
-        convert_unit_s_km='s.idx.convert_unit("km")',
-        convert_unit_s_m_to_km='s.idx.convert_unit({"m": "km"})',
+        convert_unit_s_km='s.pix.convert_unit("km")',
+        convert_unit_s_m_to_km='s.pix.convert_unit({"m": "km"})',
     )
     def convert_unit(
         self,
         unit: Union[str, Mapping[str, str], Callable[[str], str]],
         level: Optional[str] = "unit",
         axis: Axis = 0,
     ):
         return convert_unit(self._obj, unit=unit, level=level, axis=axis)
 
 
+@pd.api.extensions.register_dataframe_accessor("pix")
+class DataFramePixAccessor(_DataPixAccessor):
+    pass
+
+
+@pd.api.extensions.register_series_accessor("pix")
+class SeriesPixAccessor(_DataPixAccessor):
+    pass
+
+
+@pd.api.extensions.register_index_accessor("pix")
+class IndexPixAccessor(_PixAccessor):
+    pass
+
+
+use_pix_instead = deprecated(
+    reason="Use the new name ``df.pix`` of the accessor", version="0.2.9"
+)
+
+
 @pd.api.extensions.register_dataframe_accessor("idx")
-class DataFrameIdxAccessor(_DataIdxAccessor):
+@use_pix_instead
+class DataFrameIdxAccessor(_DataPixAccessor):
     pass
 
 
 @pd.api.extensions.register_series_accessor("idx")
-class SeriesIdxAccessor(_DataIdxAccessor):
+@use_pix_instead
+class SeriesIdxAccessor(_DataPixAccessor):
     pass
 
 
 @pd.api.extensions.register_index_accessor("idx")
-class IndexIdxAccessor(_IdxAccessor):
+@use_pix_instead
+class IndexIdxAccessor(_PixAccessor):
     pass
```

### Comparing `pandas-indexing-0.2.8/src/pandas_indexing/arithmetics.py` & `pandas-indexing-0.2.9/src/pandas_indexing/arithmetics.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.8/src/pandas_indexing/core.py` & `pandas-indexing-0.2.9/src/pandas_indexing/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     pandas.MultiIndex.droplevel
     pandas.Series.droplevel
     pandas.DataFrame.droplevel
     """
     if isinstance(index_or_data, Index):
         return _projectlevel(index_or_data, levels)
 
-    index = get_axis(index_or_data.index, axis)
+    index = get_axis(index_or_data, axis)
     return index_or_data.set_axis(_projectlevel(index, levels), axis=axis)
 
 
 def concat(
     objs: Union[Iterable[S], Mapping[str, S]],
     order: Optional[Sequence[str]] = None,
     axis: Axis = 0,
@@ -740,7 +740,39 @@
         If ``templates`` refer to non-existant levels
     """
     if isinstance(index_or_data, Index):
         return _formatlevel(index_or_data, drop, **templates)
 
     index = get_axis(index_or_data, axis)
     return index_or_data.set_axis(_formatlevel(index, drop, **templates), axis=axis)
+
+
+def _fixindexna(index: Index):
+    return index.set_codes(index.codes)
+
+
+@doc(
+    index_or_data="""
+    index_or_data : Index, Series or DataFrame
+        Datdropnalevel(self._obj, subset=subset, how=how, axis=axis)a
+    """
+)
+def fixindexna(index_or_data: T, axis: Axis = 0) -> T:
+    """Fix broken MultiIndex NA representation from .groupby(..., dropna=False)
+
+    Refer to https://github.com/coroa/pandas-indexing/issues/25 for details
+
+    Parameters
+    ----------\
+    {index_or_data}
+    axis : Axis, optional
+        Axis to fix, by default 0
+
+    Returns
+    -------
+    index_or_data
+    """
+    if isinstance(index_or_data, Index):
+        return _fixindexna(index_or_data)
+
+    new_index = _fixindexna(get_axis(index_or_data, axis))
+    return index_or_data.set_axis(new_index, axis=axis)
```

### Comparing `pandas-indexing-0.2.8/src/pandas_indexing/datasets/__init__.py` & `pandas-indexing-0.2.9/src/pandas_indexing/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.8/src/pandas_indexing/datasets/remindhighre_power.csv` & `pandas-indexing-0.2.9/src/pandas_indexing/datasets/remindhighre_power.csv`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.8/src/pandas_indexing/selectors.py` & `pandas-indexing-0.2.9/src/pandas_indexing/selectors.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.8/src/pandas_indexing/units.py` & `pandas-indexing-0.2.9/src/pandas_indexing/units.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.2.8/src/pandas_indexing/utils.py` & `pandas-indexing-0.2.9/src/pandas_indexing/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,19 @@
         .replace("$", r"\$")
     )
 
 
 def print_list(x, n):
     """Return a printable string of a list shortened to n characters.
 
-    Copied from pyam.utils.print_list by Daniel Huppmann, licensed under Apache 2.0.
+    Copied from pyam.utils.print_list by Daniel Huppmann, licensed under
+    Apache 2.0.
 
-    https://github.com/IAMconsortium/pyam/blob/449b77cb1c625b455e3675801477f19e99b30e64/pyam/utils.py#L599-L638 .
+    https://github.com/IAMconsortium/pyam/blob/449b77cb1c625b455e3675801477f19e99b30e64/pyam/utils.py#L599-L638
+    .
     """
     # if list is empty, only write count
     if len(x) == 0:
         return "(0)"
 
     # write number of elements, subtract count added at end from line width
     x = [i if i != "" else "''" for i in map(str, x)]
```

### Comparing `pandas-indexing-0.2.8/src/pandas_indexing.egg-info/PKG-INFO` & `pandas-indexing-0.2.9/src/pandas_indexing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.2.8
+Version: 0.2.9
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
```

### Comparing `pandas-indexing-0.2.8/src/pandas_indexing.egg-info/SOURCES.txt` & `pandas-indexing-0.2.9/src/pandas_indexing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

