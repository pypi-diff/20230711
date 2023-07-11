# Comparing `tmp/MRItaxonomy-0.1.0.tar.gz` & `tmp/MRItaxonomy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MRItaxonomy-0.1.0.tar", last modified: Thu May 18 13:25:19 2023, max compression
+gzip compressed data, was "MRItaxonomy-0.1.1.tar", last modified: Tue Jul 11 13:56:19 2023, max compression
```

## Comparing `MRItaxonomy-0.1.0.tar` & `MRItaxonomy-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 colinprice  (1000) colinprice  (1000)        0 2023-05-18 13:25:19.951879 MRItaxonomy-0.1.0/
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)    35129 2023-05-17 17:53:31.000000 MRItaxonomy-0.1.0/LICENSE.txt
-drwxrwxr-x   0 colinprice  (1000) colinprice  (1000)        0 2023-05-18 13:25:19.951879 MRItaxonomy-0.1.0/MRItaxonomy/
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     6299 2023-05-18 13:21:27.000000 MRItaxonomy-0.1.0/MRItaxonomy/NCBI_fetch.py
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)      360 2023-05-17 18:46:27.000000 MRItaxonomy-0.1.0/MRItaxonomy/__init__.py
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     1514 2023-05-17 21:04:11.000000 MRItaxonomy-0.1.0/MRItaxonomy/accession2taxid.py
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     1425 2023-05-17 19:07:45.000000 MRItaxonomy-0.1.0/MRItaxonomy/nnID.py
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     4091 2023-05-17 18:51:47.000000 MRItaxonomy-0.1.0/MRItaxonomy/nucDL.py
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     1486 2023-05-17 21:07:41.000000 MRItaxonomy-0.1.0/MRItaxonomy/protacc2taxid.py
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     1811 2023-05-17 17:53:31.000000 MRItaxonomy-0.1.0/MRItaxonomy/slidingwindow.py
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     2395 2023-05-17 18:51:42.000000 MRItaxonomy-0.1.0/MRItaxonomy/taxid.py
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     2219 2023-05-17 21:06:46.000000 MRItaxonomy-0.1.0/MRItaxonomy/taxid2name.py
-drwxrwxr-x   0 colinprice  (1000) colinprice  (1000)        0 2023-05-18 13:25:19.951879 MRItaxonomy-0.1.0/MRItaxonomy.egg-info/
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)      718 2023-05-18 13:25:19.000000 MRItaxonomy-0.1.0/MRItaxonomy.egg-info/PKG-INFO
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)      431 2023-05-18 13:25:19.000000 MRItaxonomy-0.1.0/MRItaxonomy.egg-info/SOURCES.txt
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)        1 2023-05-18 13:25:19.000000 MRItaxonomy-0.1.0/MRItaxonomy.egg-info/dependency_links.txt
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)       40 2023-05-18 13:25:19.000000 MRItaxonomy-0.1.0/MRItaxonomy.egg-info/requires.txt
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)       12 2023-05-18 13:25:19.000000 MRItaxonomy-0.1.0/MRItaxonomy.egg-info/top_level.txt
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)      718 2023-05-18 13:25:19.951879 MRItaxonomy-0.1.0/PKG-INFO
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)      122 2023-05-17 17:53:31.000000 MRItaxonomy-0.1.0/README.md
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)       38 2023-05-18 13:25:19.951879 MRItaxonomy-0.1.0/setup.cfg
--rw-rw-r--   0 colinprice  (1000) colinprice  (1000)      897 2023-05-17 17:53:31.000000 MRItaxonomy-0.1.0/setup.py
+drwxrwxr-x   0 colinprice  (1000) colinprice  (1000)        0 2023-07-11 13:56:19.282721 MRItaxonomy-0.1.1/
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)    35129 2023-05-18 14:10:35.000000 MRItaxonomy-0.1.1/LICENSE.txt
+drwxrwxr-x   0 colinprice  (1000) colinprice  (1000)        0 2023-07-11 13:56:19.282721 MRItaxonomy-0.1.1/MRItaxonomy/
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     6299 2023-05-18 14:10:35.000000 MRItaxonomy-0.1.1/MRItaxonomy/NCBI_fetch.py
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)      360 2023-05-18 14:10:35.000000 MRItaxonomy-0.1.1/MRItaxonomy/__init__.py
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     1514 2023-05-18 14:10:35.000000 MRItaxonomy-0.1.1/MRItaxonomy/accession2taxid.py
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     1425 2023-05-18 14:10:35.000000 MRItaxonomy-0.1.1/MRItaxonomy/nnID.py
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     4091 2023-05-18 14:10:35.000000 MRItaxonomy-0.1.1/MRItaxonomy/nucDL.py
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     1486 2023-05-18 14:10:35.000000 MRItaxonomy-0.1.1/MRItaxonomy/protacc2taxid.py
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     1811 2023-05-18 14:10:35.000000 MRItaxonomy-0.1.1/MRItaxonomy/slidingwindow.py
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     2395 2023-05-18 14:10:35.000000 MRItaxonomy-0.1.1/MRItaxonomy/taxid.py
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)     2221 2023-07-11 13:30:53.000000 MRItaxonomy-0.1.1/MRItaxonomy/taxid2name.py
+drwxrwxr-x   0 colinprice  (1000) colinprice  (1000)        0 2023-07-11 13:56:19.282721 MRItaxonomy-0.1.1/MRItaxonomy.egg-info/
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)      754 2023-07-11 13:56:19.000000 MRItaxonomy-0.1.1/MRItaxonomy.egg-info/PKG-INFO
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)      431 2023-07-11 13:56:19.000000 MRItaxonomy-0.1.1/MRItaxonomy.egg-info/SOURCES.txt
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)        1 2023-07-11 13:56:19.000000 MRItaxonomy-0.1.1/MRItaxonomy.egg-info/dependency_links.txt
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)       40 2023-07-11 13:56:19.000000 MRItaxonomy-0.1.1/MRItaxonomy.egg-info/requires.txt
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)       12 2023-07-11 13:56:19.000000 MRItaxonomy-0.1.1/MRItaxonomy.egg-info/top_level.txt
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)      754 2023-07-11 13:56:19.282721 MRItaxonomy-0.1.1/PKG-INFO
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)      122 2023-05-18 14:10:35.000000 MRItaxonomy-0.1.1/README.md
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)       38 2023-07-11 13:56:19.282721 MRItaxonomy-0.1.1/setup.cfg
+-rw-rw-r--   0 colinprice  (1000) colinprice  (1000)      914 2023-07-11 13:48:47.000000 MRItaxonomy-0.1.1/setup.py
```

### Comparing `MRItaxonomy-0.1.0/LICENSE.txt` & `MRItaxonomy-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MRItaxonomy-0.1.0/MRItaxonomy/NCBI_fetch.py` & `MRItaxonomy-0.1.1/MRItaxonomy/NCBI_fetch.py`

 * *Files identical despite different names*

### Comparing `MRItaxonomy-0.1.0/MRItaxonomy/accession2taxid.py` & `MRItaxonomy-0.1.1/MRItaxonomy/accession2taxid.py`

 * *Files identical despite different names*

### Comparing `MRItaxonomy-0.1.0/MRItaxonomy/nnID.py` & `MRItaxonomy-0.1.1/MRItaxonomy/nnID.py`

 * *Files identical despite different names*

### Comparing `MRItaxonomy-0.1.0/MRItaxonomy/nucDL.py` & `MRItaxonomy-0.1.1/MRItaxonomy/nucDL.py`

 * *Files identical despite different names*

### Comparing `MRItaxonomy-0.1.0/MRItaxonomy/protacc2taxid.py` & `MRItaxonomy-0.1.1/MRItaxonomy/protacc2taxid.py`

 * *Files identical despite different names*

### Comparing `MRItaxonomy-0.1.0/MRItaxonomy/slidingwindow.py` & `MRItaxonomy-0.1.1/MRItaxonomy/slidingwindow.py`

 * *Files identical despite different names*

### Comparing `MRItaxonomy-0.1.0/MRItaxonomy/taxid.py` & `MRItaxonomy-0.1.1/MRItaxonomy/taxid.py`

 * *Files identical despite different names*

### Comparing `MRItaxonomy-0.1.0/MRItaxonomy/taxid2name.py` & `MRItaxonomy-0.1.1/MRItaxonomy/taxid2name.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,10 +53,10 @@
             return TAXID2NAME_df2.loc[tid]['merged']
         else:
             return 0
     else:
 	    return tid
 	
 def get_name(tax):
-    TAXID2NAME_df, = load_dataframe()
+    TAXID2NAME_df, _ = load_dataframe()
     tax = get_merge(tax)
     return TAXID2NAME_df.loc[tax]['name']
```

### Comparing `MRItaxonomy-0.1.0/MRItaxonomy.egg-info/PKG-INFO` & `MRItaxonomy-0.1.1/MRItaxonomy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: MRItaxonomy
-Version: 0.1.0
+Version: 0.1.1
 Summary: MRIGlobal's taxonomy related operators
 Home-page: https://github.com/mriglobal/MRItaxonomy
-Author: Colin Price
-Author-email: cprice@mriglobal.org
+Author: MRIGlobal Bioinformatics Team
+Author-email: biofx@mriglobal.org
 License: MIT
 Keywords: mriglobal taxonomy ncbi
+Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # MRItaxonomy - MRIGlobals Taxonomy Library
 
 A compendium of convenient taxonomic related operations interfacing with NCBI
+
```

### Comparing `MRItaxonomy-0.1.0/PKG-INFO` & `MRItaxonomy-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: MRItaxonomy
-Version: 0.1.0
+Version: 0.1.1
 Summary: MRIGlobal's taxonomy related operators
 Home-page: https://github.com/mriglobal/MRItaxonomy
-Author: Colin Price
-Author-email: cprice@mriglobal.org
+Author: MRIGlobal Bioinformatics Team
+Author-email: biofx@mriglobal.org
 License: MIT
 Keywords: mriglobal taxonomy ncbi
+Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # MRItaxonomy - MRIGlobals Taxonomy Library
 
 A compendium of convenient taxonomic related operations interfacing with NCBI
+
```

### Comparing `MRItaxonomy-0.1.0/setup.py` & `MRItaxonomy-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MRItaxonomy",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=['pandas>=0.19.0',
                       'biopython>=1.7',
                       'wget>=3.2'],
-    author="Colin Price",
-    author_email="cprice@mriglobal.org",
+    author="MRIGlobal Bioinformatics Team",
+    author_email="biofx@mriglobal.org",
     keywords="mriglobal taxonomy ncbi",
     description="MRIGlobal's taxonomy related operators",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="MIT", # or the license you chose
     url="https://github.com/mriglobal/MRItaxonomy",
     classifiers=[
```

