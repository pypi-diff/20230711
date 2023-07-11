# Comparing `tmp/pydra-mrtrix3-0.2.tar.gz` & `tmp/pydra-mrtrix3-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydra-mrtrix3-0.2.tar", last modified: Wed Sep 28 02:06:49 2022, max compression
+gzip compressed data, was "pydra-mrtrix3-0.2.1.tar", last modified: Tue Jul 11 00:16:19 2023, max compression
```

## Comparing `pydra-mrtrix3-0.2.tar` & `pydra-mrtrix3-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 02:06:49.888714 pydra-mrtrix3-0.2/
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-09-28 02:06:39.000000 pydra-mrtrix3-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-28 02:06:39.000000 pydra-mrtrix3-0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-09-28 02:06:49.888714 pydra-mrtrix3-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-09-28 02:06:39.000000 pydra-mrtrix3-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 02:06:49.884714 pydra-mrtrix3-0.2/pydra/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 02:06:49.884714 pydra-mrtrix3-0.2/pydra/tasks/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 02:06:49.888714 pydra-mrtrix3-0.2/pydra/tasks/mrtrix3/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-28 02:06:39.000000 pydra-mrtrix3-0.2/pydra/tasks/mrtrix3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-09-28 02:06:49.888714 pydra-mrtrix3-0.2/pydra/tasks/mrtrix3/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-09-28 02:06:39.000000 pydra-mrtrix3-0.2/pydra/tasks/mrtrix3/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-09-28 02:06:39.000000 pydra-mrtrix3-0.2/pydra/tasks/mrtrix3/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 02:06:49.888714 pydra-mrtrix3-0.2/pydra/tasks/mrtrix3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 02:06:39.000000 pydra-mrtrix3-0.2/pydra/tasks/mrtrix3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-09-28 02:06:39.000000 pydra-mrtrix3-0.2/pydra/tasks/mrtrix3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4939 2022-09-28 02:06:39.000000 pydra-mrtrix3-0.2/pydra/tasks/mrtrix3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 02:06:49.888714 pydra-mrtrix3-0.2/pydra_mrtrix3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-09-28 02:06:49.000000 pydra-mrtrix3-0.2/pydra_mrtrix3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-09-28 02:06:49.000000 pydra-mrtrix3-0.2/pydra_mrtrix3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-28 02:06:49.000000 pydra-mrtrix3-0.2/pydra_mrtrix3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-09-28 02:06:49.000000 pydra-mrtrix3-0.2/pydra_mrtrix3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-28 02:06:49.000000 pydra-mrtrix3-0.2/pydra_mrtrix3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-28 02:06:39.000000 pydra-mrtrix3-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-09-28 02:06:49.888714 pydra-mrtrix3-0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      668 2022-09-28 02:06:39.000000 pydra-mrtrix3-0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    70238 2022-09-28 02:06:39.000000 pydra-mrtrix3-0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:16:19.600684 pydra-mrtrix3-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-11 00:16:06.000000 pydra-mrtrix3-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-11 00:16:06.000000 pydra-mrtrix3-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-11 00:16:19.600684 pydra-mrtrix3-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-11 00:16:06.000000 pydra-mrtrix3-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:16:19.596684 pydra-mrtrix3-0.2.1/pydra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:16:19.596684 pydra-mrtrix3-0.2.1/pydra/tasks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:16:19.604684 pydra-mrtrix3-0.2.1/pydra/tasks/mrtrix3/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 00:16:06.000000 pydra-mrtrix3-0.2.1/pydra/tasks/mrtrix3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-11 00:16:19.604684 pydra-mrtrix3-0.2.1/pydra/tasks/mrtrix3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-11 00:16:06.000000 pydra-mrtrix3-0.2.1/pydra/tasks/mrtrix3/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-11 00:16:06.000000 pydra-mrtrix3-0.2.1/pydra/tasks/mrtrix3/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:16:19.600684 pydra-mrtrix3-0.2.1/pydra/tasks/mrtrix3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 00:16:06.000000 pydra-mrtrix3-0.2.1/pydra/tasks/mrtrix3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-11 00:16:06.000000 pydra-mrtrix3-0.2.1/pydra/tasks/mrtrix3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-11 00:16:06.000000 pydra-mrtrix3-0.2.1/pydra/tasks/mrtrix3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 00:16:19.600684 pydra-mrtrix3-0.2.1/pydra_mrtrix3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-11 00:16:19.000000 pydra-mrtrix3-0.2.1/pydra_mrtrix3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-11 00:16:19.000000 pydra-mrtrix3-0.2.1/pydra_mrtrix3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 00:16:19.000000 pydra-mrtrix3-0.2.1/pydra_mrtrix3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-11 00:16:19.000000 pydra-mrtrix3-0.2.1/pydra_mrtrix3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 00:16:19.000000 pydra-mrtrix3-0.2.1/pydra_mrtrix3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 00:16:06.000000 pydra-mrtrix3-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-11 00:16:19.604684 pydra-mrtrix3-0.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-07-11 00:16:06.000000 pydra-mrtrix3-0.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70238 2023-07-11 00:16:06.000000 pydra-mrtrix3-0.2.1/versioneer.py
```

### Comparing `pydra-mrtrix3-0.2/LICENSE` & `pydra-mrtrix3-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra-mrtrix3-0.2/PKG-INFO` & `pydra-mrtrix3-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydra-mrtrix3
-Version: 0.2
+Version: 0.2.1
 Summary: Pydra tasks for MRtrix3
 Author: Nipype developers
 Author-email: neuroimaging@python.org
 License: Apache License, 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pydra-mrtrix3-0.2/pydra/tasks/mrtrix3/base.py` & `pydra-mrtrix3-0.2.1/pydra/tasks/mrtrix3/base.py`

 * *Files identical despite different names*

### Comparing `pydra-mrtrix3-0.2/pydra/tasks/mrtrix3/conftest.py` & `pydra-mrtrix3-0.2.1/pydra/tasks/mrtrix3/conftest.py`

 * *Files identical despite different names*

### Comparing `pydra-mrtrix3-0.2/pydra/tasks/mrtrix3/tests/test_utils.py` & `pydra-mrtrix3-0.2.1/pydra/tasks/mrtrix3/tests/test_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from pathlib import Path
 import pytest
 from pydra.tasks.mrtrix3.utils import MRConvert
-from medimages4tests.dicom.mri.dwi.siemens.skyra.syngo_d13c import (
-    sample_image as sample_dwi_dicom,
+from medimages4tests.dummy.dicom.mri.dwi.siemens.skyra.syngo_d13c import (
+    get_image as get_dwi_dicom,
 )
-from medimages4tests.nifti import sample_image as sample_nifti
+from medimages4tests.dummy.nifti import get_image as get_nifti
 
 
 @pytest.fixture
 def dwi_dicom_dataset():
-    return sample_dwi_dicom()
+    return get_dwi_dicom()
 
 
 @pytest.fixture
 def nifti_dataset(work_dir):
-    return sample_nifti(work_dir / "nifti", compressed=True)
+    return get_nifti(work_dir / "nifti", compressed=True)
 
 
 def test_mrconvert_default_out_file(nifti_dataset):
 
     task = MRConvert(in_file=nifti_dataset, axes=[0, 1, 2, -1])
 
     result = task()
```

### Comparing `pydra-mrtrix3-0.2/pydra/tasks/mrtrix3/utils.py` & `pydra-mrtrix3-0.2.1/pydra/tasks/mrtrix3/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                     "output_file_template": "{in_file}_converted",
                 },
             ),
         ),
         (
             "coord",
             attr.ib(
-                type=ty.List[float],
+                type=ty.Tuple[int, ty.Union[int, str]],
                 metadata={
                     "sep": " ",
                     "argstr": "-coord",
                     "help_string": "extract data at the specific coordinatest",
                 },
             ),
         ),
```

### Comparing `pydra-mrtrix3-0.2/pydra_mrtrix3.egg-info/PKG-INFO` & `pydra-mrtrix3-0.2.1/pydra_mrtrix3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydra-mrtrix3
-Version: 0.2
+Version: 0.2.1
 Summary: Pydra tasks for MRtrix3
 Author: Nipype developers
 Author-email: neuroimaging@python.org
 License: Apache License, 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pydra-mrtrix3-0.2/pydra_mrtrix3.egg-info/requires.txt` & `pydra-mrtrix3-0.2.1/pydra_mrtrix3.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pydra-mrtrix3-0.2/setup.cfg` & `pydra-mrtrix3-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pydra-mrtrix3-0.2/setup.py` & `pydra-mrtrix3-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `pydra-mrtrix3-0.2/versioneer.py` & `pydra-mrtrix3-0.2.1/versioneer.py`

 * *Files identical despite different names*

