# Comparing `tmp/spyndex-0.4.0.tar.gz` & `tmp/spyndex-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyndex-0.4.0.tar", last modified: Mon Mar 13 09:51:43 2023, max compression
+gzip compressed data, was "spyndex-0.5.0.tar", last modified: Tue Jul 11 08:03:21 2023, max compression
```

## Comparing `spyndex-0.4.0.tar` & `spyndex-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-03-13 09:51:43.793411 spyndex-0.4.0/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2021-09-03 21:24:15.000000 spyndex-0.4.0/LICENSE
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)    17941 2023-03-13 09:51:43.793411 spyndex-0.4.0/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)    17285 2022-03-11 15:13:15.000000 spyndex-0.4.0/README.md
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-03-13 09:51:43.793411 spyndex-0.4.0/setup.cfg
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1393 2023-03-13 09:21:12.000000 spyndex-0.4.0/setup.py
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-03-13 09:51:43.776744 spyndex-0.4.0/spyndex/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      243 2023-03-13 09:33:12.000000 spyndex-0.4.0/spyndex/__init__.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)    14436 2023-03-13 09:17:05.000000 spyndex-0.4.0/spyndex/axioms.py
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-03-13 09:51:43.790078 spyndex-0.4.0/spyndex/data/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)  6284146 2021-09-06 18:53:31.000000 spyndex-0.4.0/spyndex/data/S2_10m.json
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)    23999 2023-03-13 09:17:05.000000 spyndex-0.4.0/spyndex/data/bands.json
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2817 2022-10-08 12:10:18.000000 spyndex-0.4.0/spyndex/data/constants.json
--rwxr-xr-x   0 dmontero  (1001) dmontero  (1001)   155222 2023-03-13 09:17:05.000000 spyndex-0.4.0/spyndex/data/spectral-indices-dict.json
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)    16684 2021-09-11 12:19:14.000000 spyndex-0.4.0/spyndex/data/spectral.json
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1743 2021-10-07 15:49:12.000000 spyndex-0.4.0/spyndex/datasets.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1785 2021-09-13 11:48:08.000000 spyndex-0.4.0/spyndex/plot.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)    13418 2022-01-17 22:12:10.000000 spyndex-0.4.0/spyndex/spyndex.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1721 2022-06-02 13:19:12.000000 spyndex-0.4.0/spyndex/utils.py
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-03-13 09:51:43.776744 spyndex-0.4.0/spyndex.egg-info/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)    17941 2023-03-13 09:51:43.000000 spyndex-0.4.0/spyndex.egg-info/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      434 2023-03-13 09:51:43.000000 spyndex-0.4.0/spyndex.egg-info/SOURCES.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-03-13 09:51:43.000000 spyndex-0.4.0/spyndex.egg-info/dependency_links.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      109 2023-03-13 09:51:43.000000 spyndex-0.4.0/spyndex.egg-info/requires.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        8 2023-03-13 09:51:43.000000 spyndex-0.4.0/spyndex.egg-info/top_level.txt
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-11 08:03:21.220546 spyndex-0.5.0/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2021-09-03 21:24:15.000000 spyndex-0.5.0/LICENSE
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)    18042 2023-07-11 08:03:21.220546 spyndex-0.5.0/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)    17386 2023-07-10 11:17:33.000000 spyndex-0.5.0/README.md
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-07-11 08:03:21.220546 spyndex-0.5.0/setup.cfg
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1366 2023-07-11 07:51:15.000000 spyndex-0.5.0/setup.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-11 08:03:21.207213 spyndex-0.5.0/spyndex/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      243 2023-07-11 07:51:20.000000 spyndex-0.5.0/spyndex/__init__.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)    14436 2023-03-13 09:17:05.000000 spyndex-0.5.0/spyndex/axioms.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-11 08:03:21.220546 spyndex-0.5.0/spyndex/data/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)  6284146 2021-09-06 18:53:31.000000 spyndex-0.5.0/spyndex/data/S2_10m.json
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)    23999 2023-03-13 09:17:05.000000 spyndex-0.5.0/spyndex/data/bands.json
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2954 2023-07-10 11:17:33.000000 spyndex-0.5.0/spyndex/data/constants.json
+-rwxr-xr-x   0 dmontero  (1001) dmontero  (1001)   156701 2023-07-10 11:17:33.000000 spyndex-0.5.0/spyndex/data/spectral-indices-dict.json
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)    16684 2021-09-11 12:19:14.000000 spyndex-0.5.0/spyndex/data/spectral.json
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1743 2021-10-07 15:49:12.000000 spyndex-0.5.0/spyndex/datasets.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2040 2023-07-10 13:58:03.000000 spyndex-0.5.0/spyndex/plot.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)    13418 2022-01-17 22:12:10.000000 spyndex-0.5.0/spyndex/spyndex.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1721 2022-06-02 13:19:12.000000 spyndex-0.5.0/spyndex/utils.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-11 08:03:21.207213 spyndex-0.5.0/spyndex.egg-info/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)    18042 2023-07-11 08:03:21.000000 spyndex-0.5.0/spyndex.egg-info/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      434 2023-07-11 08:03:21.000000 spyndex-0.5.0/spyndex.egg-info/SOURCES.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-07-11 08:03:21.000000 spyndex-0.5.0/spyndex.egg-info/dependency_links.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      104 2023-07-11 08:03:21.000000 spyndex-0.5.0/spyndex.egg-info/requires.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        8 2023-07-11 08:03:21.000000 spyndex-0.5.0/spyndex.egg-info/top_level.txt
```

### Comparing `spyndex-0.4.0/LICENSE` & `spyndex-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spyndex-0.4.0/PKG-INFO` & `spyndex-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyndex
-Version: 0.4.0
+Version: 0.5.0
 Summary: Awesome Spectral Indices in Python
 Home-page: https://github.com/awesome-spectral-indices/spyndex
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -75,14 +75,16 @@
 
 ---
 
 **GitHub**: [https://github.com/davemlz/spyndex](https://github.com/davemlz/spyndex)
 
 **Documentation**: [https://spyndex.readthedocs.io/](https://spyndex.readthedocs.io/)
 
+**Paper**: [https://doi.org/10.1038/s41597-023-02096-0](https://doi.org/10.1038/s41597-023-02096-0)
+
 **PyPI**: [https://pypi.org/project/spyndex/](https://pypi.org/project/spyndex/)
 
 **Conda-forge**: [https://anaconda.org/conda-forge/spyndex](https://anaconda.org/conda-forge/spyndex)
 
 **Tutorials**: [https://spyndex.readthedocs.io/en/latest/tutorials.html](https://spyndex.readthedocs.io/en/latest/tutorials.html)
 
 ---
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spyndex Version: 0.4.0 Summary: Awesome Spectral
+Metadata-Version: 2.1 Name: spyndex Version: 0.5.0 Summary: Awesome Spectral
 Indices in Python Home-page: https://github.com/awesome-spectral-indices/
 spyndex Author: David Montero Loaiza Author-email: dml.mont@gmail.com License:
 MIT Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Description-
@@ -10,19 +10,20 @@
                                    [spyndex]
                       Awesome_Spectral_Indices in Python:
 Numpy | Pandas | GeoPandas | Xarray | Earth_Engine | Planetary_Computer | Dask
 [PyPI] [conda-forge] [Documentation_Status] [Tests] [Awesome_Spectral_Indices]
 [License] [GitHub_Sponsors] [Buy_me_a_coffee] [Ko-fi] [Twitter] [Black] [isort]
 --- **GitHub**: [https://github.com/davemlz/spyndex](https://github.com/
 davemlz/spyndex) **Documentation**: [https://spyndex.readthedocs.io/](https://
-spyndex.readthedocs.io/) **PyPI**: [https://pypi.org/project/spyndex/](https://
-pypi.org/project/spyndex/) **Conda-forge**: [https://anaconda.org/conda-forge/
-spyndex](https://anaconda.org/conda-forge/spyndex) **Tutorials**: [https://
-spyndex.readthedocs.io/en/latest/tutorials.html](https://
-spyndex.readthedocs.io/en/latest/tutorials.html) --- ## Overview The [Awesome
+spyndex.readthedocs.io/) **Paper**: [https://doi.org/10.1038/s41597-023-02096-
+0](https://doi.org/10.1038/s41597-023-02096-0) **PyPI**: [https://pypi.org/
+project/spyndex/](https://pypi.org/project/spyndex/) **Conda-forge**: [https://
+anaconda.org/conda-forge/spyndex](https://anaconda.org/conda-forge/spyndex)
+**Tutorials**: [https://spyndex.readthedocs.io/en/latest/tutorials.html](https:
+//spyndex.readthedocs.io/en/latest/tutorials.html) --- ## Overview The [Awesome
 Spectral Indices](https://github.com/davemlz/awesome-spectral-indices) is a
 standardized ready-to-use curated list of spectral indices that can be used as
 expressions for computing spectral indices in remote sensing applications. The
 list was born initially to supply spectral indices for [Google Earth Engine]
 (https://earthengine.google.com/) through [eemont](https://github.com/davemlz/
 eemont) and [spectral](https://github.com/davemlz/spectral), but given the
 necessity to compute spectral indices for other object classes outside the
```

### Comparing `spyndex-0.4.0/README.md` & `spyndex-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 
 ---
 
 **GitHub**: [https://github.com/davemlz/spyndex](https://github.com/davemlz/spyndex)
 
 **Documentation**: [https://spyndex.readthedocs.io/](https://spyndex.readthedocs.io/)
 
+**Paper**: [https://doi.org/10.1038/s41597-023-02096-0](https://doi.org/10.1038/s41597-023-02096-0)
+
 **PyPI**: [https://pypi.org/project/spyndex/](https://pypi.org/project/spyndex/)
 
 **Conda-forge**: [https://anaconda.org/conda-forge/spyndex](https://anaconda.org/conda-forge/spyndex)
 
 **Tutorials**: [https://spyndex.readthedocs.io/en/latest/tutorials.html](https://spyndex.readthedocs.io/en/latest/tutorials.html)
 
 ---
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
                                    [spyndex]
                       Awesome_Spectral_Indices in Python:
 Numpy | Pandas | GeoPandas | Xarray | Earth_Engine | Planetary_Computer | Dask
 [PyPI] [conda-forge] [Documentation_Status] [Tests] [Awesome_Spectral_Indices]
 [License] [GitHub_Sponsors] [Buy_me_a_coffee] [Ko-fi] [Twitter] [Black] [isort]
 --- **GitHub**: [https://github.com/davemlz/spyndex](https://github.com/
 davemlz/spyndex) **Documentation**: [https://spyndex.readthedocs.io/](https://
-spyndex.readthedocs.io/) **PyPI**: [https://pypi.org/project/spyndex/](https://
-pypi.org/project/spyndex/) **Conda-forge**: [https://anaconda.org/conda-forge/
-spyndex](https://anaconda.org/conda-forge/spyndex) **Tutorials**: [https://
-spyndex.readthedocs.io/en/latest/tutorials.html](https://
-spyndex.readthedocs.io/en/latest/tutorials.html) --- ## Overview The [Awesome
+spyndex.readthedocs.io/) **Paper**: [https://doi.org/10.1038/s41597-023-02096-
+0](https://doi.org/10.1038/s41597-023-02096-0) **PyPI**: [https://pypi.org/
+project/spyndex/](https://pypi.org/project/spyndex/) **Conda-forge**: [https://
+anaconda.org/conda-forge/spyndex](https://anaconda.org/conda-forge/spyndex)
+**Tutorials**: [https://spyndex.readthedocs.io/en/latest/tutorials.html](https:
+//spyndex.readthedocs.io/en/latest/tutorials.html) --- ## Overview The [Awesome
 Spectral Indices](https://github.com/davemlz/awesome-spectral-indices) is a
 standardized ready-to-use curated list of spectral indices that can be used as
 expressions for computing spectral indices in remote sensing applications. The
 list was born initially to supply spectral indices for [Google Earth Engine]
 (https://earthengine.google.com/) through [eemont](https://github.com/davemlz/
 eemont) and [spectral](https://github.com/davemlz/spectral), but given the
 necessity to compute spectral indices for other object classes outside the
```

### Comparing `spyndex-0.4.0/setup.py` & `spyndex-0.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,35 +10,33 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
     name="spyndex",
-    version="0.4.0",
+    version="0.5.0",
     url="https://github.com/awesome-spectral-indices/spyndex",
     license="MIT",
     author="David Montero Loaiza",
     author_email="dml.mont@gmail.com",
     description="Awesome Spectral Indices in Python",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=("tests",)),
     package_data={"spyndex": ["data/*.json"]},
     install_requires=[
-        "dask>=2021.9.1",
-        "earthengine-api",
+        "dask>=2023.7.0",
         "eemont>=0.3.6",
         "matplotlib",
-        "numpy",
-        "pandas",
+        "pandas>=2.0.3",
         "python-box>=6.0",
         "requests",
         "seaborn",
-        "xarray",
+        "xarray>=2023.6.0",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

### Comparing `spyndex-0.4.0/spyndex/axioms.py` & `spyndex-0.5.0/spyndex/axioms.py`

 * *Files identical despite different names*

### Comparing `spyndex-0.4.0/spyndex/data/S2_10m.json` & `spyndex-0.5.0/spyndex/data/S2_10m.json`

 * *Files identical despite different names*

### Comparing `spyndex-0.4.0/spyndex/data/bands.json` & `spyndex-0.5.0/spyndex/data/bands.json`

 * *Files identical despite different names*

### Comparing `spyndex-0.4.0/spyndex/data/constants.json` & `spyndex-0.5.0/spyndex/data/constants.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'epsilon'": "OrderedDict([('default', 1), ('description', 'Adjustment constant used for EBI'), "*

 * *              "('short_name', 'epsilon')])"}*

```diff
@@ -35,14 +35,19 @@
         "short_name": "c"
     },
     "cexp": {
         "default": 1.16,
         "description": "Exponent used for OCVI",
         "short_name": "cexp"
     },
+    "epsilon": {
+        "default": 1,
+        "description": "Adjustment constant used for EBI",
+        "short_name": "epsilon"
+    },
     "fdelta": {
         "default": 0.581,
         "description": "Adjustment factor used for SEVI",
         "short_name": "fdelta"
     },
     "g": {
         "default": 2.5,
```

### Comparing `spyndex-0.4.0/spyndex/data/spectral-indices-dict.json` & `spyndex-0.5.0/spyndex/data/spectral-indices-dict.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9957081545064378%*

 * *Differences: {"'SpectralIndices'": "{'EBI': OrderedDict([('application_domain', 'vegetation'), ('bands', ['R', "*

 * *                      "'G', 'B', 'epsilon']), ('contributor', 'https://github.com/geoSanjeeb'), "*

 * *                      "('date_of_addition', '2023-07-03'), ('formula', '(R + G + B)/((G/B) * (R - "*

 * *                      "B + epsilon))'), ('long_name', 'Enhanced Bloom Index'), ('platforms', "*

 * *                      "['Sentinel-2', 'Landsat-OLI', 'Landsat-TM', 'Landsat-ETM+', 'MODIS', "*

 * *                      "'P […]*

```diff
@@ -846,14 +846,37 @@
             "platforms": [
                 "Landsat-TM",
                 "Landsat-ETM+"
             ],
             "reference": "https://doi.org/10.3390/rs4102957",
             "short_name": "EBBI"
         },
+        "EBI": {
+            "application_domain": "vegetation",
+            "bands": [
+                "R",
+                "G",
+                "B",
+                "epsilon"
+            ],
+            "contributor": "https://github.com/geoSanjeeb",
+            "date_of_addition": "2023-07-03",
+            "formula": "(R + G + B)/((G/B) * (R - B + epsilon))",
+            "long_name": "Enhanced Bloom Index",
+            "platforms": [
+                "Sentinel-2",
+                "Landsat-OLI",
+                "Landsat-TM",
+                "Landsat-ETM+",
+                "MODIS",
+                "Planet-Fusion"
+            ],
+            "reference": "https://doi.org/10.1016/j.isprsjprs.2019.08.006",
+            "short_name": "EBI"
+        },
         "EMBI": {
             "application_domain": "soil",
             "bands": [
                 "S1",
                 "S2",
                 "N",
                 "G"
@@ -3665,14 +3688,35 @@
             "platforms": [
                 "Sentinel-2",
                 "Landsat-OLI"
             ],
             "reference": "https://eurekamag.com/research/009/395/009395053.php",
             "short_name": "SIPI"
         },
+        "SLAVI": {
+            "application_domain": "vegetation",
+            "bands": [
+                "N",
+                "R",
+                "S2"
+            ],
+            "contributor": "https://github.com/geoSanjeeb",
+            "date_of_addition": "2023-07-03",
+            "formula": "N/(R + S2)",
+            "long_name": "Specific Leaf Area Vegetation Index",
+            "platforms": [
+                "Sentinel-2",
+                "Landsat-OLI",
+                "Landsat-TM",
+                "Landsat-ETM+",
+                "MODIS"
+            ],
+            "reference": "https://www.asprs.org/wp-content/uploads/pers/2000journal/february/2000_feb_183-191.pdf",
+            "short_name": "SLAVI"
+        },
         "SR": {
             "application_domain": "vegetation",
             "bands": [
                 "N",
                 "R"
             ],
             "contributor": "https://github.com/davemlz",
```

### Comparing `spyndex-0.4.0/spyndex/data/spectral.json` & `spyndex-0.5.0/spyndex/data/spectral.json`

 * *Files identical despite different names*

### Comparing `spyndex-0.4.0/spyndex/datasets.py` & `spyndex-0.5.0/spyndex/datasets.py`

 * *Files identical despite different names*

### Comparing `spyndex-0.4.0/spyndex/plot.py` & `spyndex-0.5.0/spyndex/plot.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,31 @@
 import seaborn as sns
 
 import spyndex
 
 from .utils import _check_params, _get_indices
 
 
-def heatmap(index: str, x: str, y: str, params: Optional[dict] = None, **kwargs):
+def heatmap(index: str, x: str, y: str, params: Optional[dict] = None, online: bool = False, **kwargs):
     """Plot all posible index values as a color-encoded matrix.
 
     Parameters
     ----------
     index : str
         Index to plot.
     x : str
         Band to plot in the x-axis.
     y : str
         Band to plot in the y-axis.
     params: dict
         Parameters for all remaining bands that are not used in :code:`x` nor :code:`y`.
         This dictionary must store just float values.
+    online : bool, default = False
+        Whether to retrieve the most recent list of indices directly from the GitHub
+        repository and not from the local copy.
     **kwargs : Keyword arguments
         Keyword arguments that can be passed to :code:`seaborn.heatmap()`.
 
     Returns
     -------
     Matplotlib Axes
         Axes object with the index heatmap.
@@ -60,17 +63,18 @@
     )
 
     if params is not None:
         params = {**params, x: df[x], y: df[y]}
     else:
         params = {x: df[x], y: df[y]}
 
-    _check_params(index, params)
+    indices = _get_indices(online)
+    _check_params(index, params, indices)
 
     df[index] = spyndex.computeIndex(index=index, params=params)
 
-    df = df.pivot(y, x, index)
+    df = df.pivot(index=y, columns=x, values=index)
 
     h = sns.heatmap(df, **kwargs)
     h.invert_yaxis()
 
     return h
```

### Comparing `spyndex-0.4.0/spyndex/spyndex.py` & `spyndex-0.5.0/spyndex/spyndex.py`

 * *Files identical despite different names*

### Comparing `spyndex-0.4.0/spyndex/utils.py` & `spyndex-0.5.0/spyndex/utils.py`

 * *Files identical despite different names*

### Comparing `spyndex-0.4.0/spyndex.egg-info/PKG-INFO` & `spyndex-0.5.0/spyndex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyndex
-Version: 0.4.0
+Version: 0.5.0
 Summary: Awesome Spectral Indices in Python
 Home-page: https://github.com/awesome-spectral-indices/spyndex
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -75,14 +75,16 @@
 
 ---
 
 **GitHub**: [https://github.com/davemlz/spyndex](https://github.com/davemlz/spyndex)
 
 **Documentation**: [https://spyndex.readthedocs.io/](https://spyndex.readthedocs.io/)
 
+**Paper**: [https://doi.org/10.1038/s41597-023-02096-0](https://doi.org/10.1038/s41597-023-02096-0)
+
 **PyPI**: [https://pypi.org/project/spyndex/](https://pypi.org/project/spyndex/)
 
 **Conda-forge**: [https://anaconda.org/conda-forge/spyndex](https://anaconda.org/conda-forge/spyndex)
 
 **Tutorials**: [https://spyndex.readthedocs.io/en/latest/tutorials.html](https://spyndex.readthedocs.io/en/latest/tutorials.html)
 
 ---
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spyndex Version: 0.4.0 Summary: Awesome Spectral
+Metadata-Version: 2.1 Name: spyndex Version: 0.5.0 Summary: Awesome Spectral
 Indices in Python Home-page: https://github.com/awesome-spectral-indices/
 spyndex Author: David Montero Loaiza Author-email: dml.mont@gmail.com License:
 MIT Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Description-
@@ -10,19 +10,20 @@
                                    [spyndex]
                       Awesome_Spectral_Indices in Python:
 Numpy | Pandas | GeoPandas | Xarray | Earth_Engine | Planetary_Computer | Dask
 [PyPI] [conda-forge] [Documentation_Status] [Tests] [Awesome_Spectral_Indices]
 [License] [GitHub_Sponsors] [Buy_me_a_coffee] [Ko-fi] [Twitter] [Black] [isort]
 --- **GitHub**: [https://github.com/davemlz/spyndex](https://github.com/
 davemlz/spyndex) **Documentation**: [https://spyndex.readthedocs.io/](https://
-spyndex.readthedocs.io/) **PyPI**: [https://pypi.org/project/spyndex/](https://
-pypi.org/project/spyndex/) **Conda-forge**: [https://anaconda.org/conda-forge/
-spyndex](https://anaconda.org/conda-forge/spyndex) **Tutorials**: [https://
-spyndex.readthedocs.io/en/latest/tutorials.html](https://
-spyndex.readthedocs.io/en/latest/tutorials.html) --- ## Overview The [Awesome
+spyndex.readthedocs.io/) **Paper**: [https://doi.org/10.1038/s41597-023-02096-
+0](https://doi.org/10.1038/s41597-023-02096-0) **PyPI**: [https://pypi.org/
+project/spyndex/](https://pypi.org/project/spyndex/) **Conda-forge**: [https://
+anaconda.org/conda-forge/spyndex](https://anaconda.org/conda-forge/spyndex)
+**Tutorials**: [https://spyndex.readthedocs.io/en/latest/tutorials.html](https:
+//spyndex.readthedocs.io/en/latest/tutorials.html) --- ## Overview The [Awesome
 Spectral Indices](https://github.com/davemlz/awesome-spectral-indices) is a
 standardized ready-to-use curated list of spectral indices that can be used as
 expressions for computing spectral indices in remote sensing applications. The
 list was born initially to supply spectral indices for [Google Earth Engine]
 (https://earthengine.google.com/) through [eemont](https://github.com/davemlz/
 eemont) and [spectral](https://github.com/davemlz/spectral), but given the
 necessity to compute spectral indices for other object classes outside the
```

