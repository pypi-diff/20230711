# Comparing `tmp/pydra-dcm2niix-1.2.0.tar.gz` & `tmp/pydra-dcm2niix-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydra-dcm2niix-1.2.0.tar", last modified: Mon Sep 26 23:18:49 2022, max compression
+gzip compressed data, was "pydra-dcm2niix-1.2.1.tar", last modified: Tue Jul 11 01:10:34 2023, max compression
```

## Comparing `pydra-dcm2niix-1.2.0.tar` & `pydra-dcm2niix-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-09-26 23:18:49.955765 pydra-dcm2niix-1.2.0/
--rw-r--r--   0 tclose     (501) staff       (20)      588 2021-06-09 06:42:05.000000 pydra-dcm2niix-1.2.0/LICENSE
--rw-r--r--   0 tclose     (501) staff       (20)       63 2021-06-11 03:56:18.000000 pydra-dcm2niix-1.2.0/MANIFEST.in
--rw-r--r--   0 tclose     (501) staff       (20)     2418 2022-09-26 23:18:49.956035 pydra-dcm2niix-1.2.0/PKG-INFO
--rw-r--r--   0 tclose     (501) staff       (20)     1090 2021-07-27 07:09:41.000000 pydra-dcm2niix-1.2.0/README.md
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-09-26 23:18:49.947618 pydra-dcm2niix-1.2.0/pydra/
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-09-26 23:18:49.947720 pydra-dcm2niix-1.2.0/pydra/tasks/
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-09-26 23:18:49.957608 pydra-dcm2niix-1.2.0/pydra/tasks/dcm2niix/
--rw-r--r--   0 tclose     (501) staff       (20)      287 2021-06-16 00:51:30.000000 pydra-dcm2niix-1.2.0/pydra/tasks/dcm2niix/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)      497 2022-09-26 23:18:49.957707 pydra-dcm2niix-1.2.0/pydra/tasks/dcm2niix/_version.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-09-26 23:18:49.953095 pydra-dcm2niix-1.2.0/pydra/tasks/dcm2niix/tests/
--rw-r--r--   0 tclose     (501) staff       (20)        0 2021-06-09 07:57:34.000000 pydra-dcm2niix-1.2.0/pydra/tasks/dcm2niix/tests/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)      317 2022-07-27 01:08:33.000000 pydra-dcm2niix-1.2.0/pydra/tasks/dcm2niix/tests/test_utils.py
--rw-r--r--   0 tclose     (501) staff       (20)    11978 2022-09-26 23:01:26.000000 pydra-dcm2niix-1.2.0/pydra/tasks/dcm2niix/utils.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-09-26 23:18:49.955477 pydra-dcm2niix-1.2.0/pydra_dcm2niix.egg-info/
--rw-r--r--   0 tclose     (501) staff       (20)     2418 2022-09-26 23:18:49.000000 pydra-dcm2niix-1.2.0/pydra_dcm2niix.egg-info/PKG-INFO
--rw-r--r--   0 tclose     (501) staff       (20)      442 2022-09-26 23:18:49.000000 pydra-dcm2niix-1.2.0/pydra_dcm2niix.egg-info/SOURCES.txt
--rw-r--r--   0 tclose     (501) staff       (20)        1 2022-09-26 23:18:49.000000 pydra-dcm2niix-1.2.0/pydra_dcm2niix.egg-info/dependency_links.txt
--rw-r--r--   0 tclose     (501) staff       (20)      755 2022-09-26 23:18:49.000000 pydra-dcm2niix-1.2.0/pydra_dcm2niix.egg-info/requires.txt
--rw-r--r--   0 tclose     (501) staff       (20)        6 2022-09-26 23:18:49.000000 pydra-dcm2niix-1.2.0/pydra_dcm2niix.egg-info/top_level.txt
--rw-r--r--   0 tclose     (501) staff       (20)       54 2022-09-26 23:01:26.000000 pydra-dcm2niix-1.2.0/pyproject.toml
--rw-r--r--   0 tclose     (501) staff       (20)     1789 2022-09-26 23:18:49.957207 pydra-dcm2niix-1.2.0/setup.cfg
--rwxr-xr-x   0 tclose     (501) staff       (20)      828 2021-11-03 05:42:41.000000 pydra-dcm2niix-1.2.0/setup.py
--rw-r--r--   0 tclose     (501) staff       (20)    70238 2021-06-09 06:42:05.000000 pydra-dcm2niix-1.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:10:34.248033 pydra-dcm2niix-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-11 01:10:21.000000 pydra-dcm2niix-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-11 01:10:21.000000 pydra-dcm2niix-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-11 01:10:34.248033 pydra-dcm2niix-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-11 01:10:21.000000 pydra-dcm2niix-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:10:34.244033 pydra-dcm2niix-1.2.1/pydra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:10:34.244033 pydra-dcm2niix-1.2.1/pydra/tasks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:10:34.252033 pydra-dcm2niix-1.2.1/pydra/tasks/dcm2niix/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-11 01:10:21.000000 pydra-dcm2niix-1.2.1/pydra/tasks/dcm2niix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-11 01:10:34.252033 pydra-dcm2niix-1.2.1/pydra/tasks/dcm2niix/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:10:34.248033 pydra-dcm2niix-1.2.1/pydra/tasks/dcm2niix/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 01:10:21.000000 pydra-dcm2niix-1.2.1/pydra/tasks/dcm2niix/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-11 01:10:21.000000 pydra-dcm2niix-1.2.1/pydra/tasks/dcm2niix/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-07-11 01:10:21.000000 pydra-dcm2niix-1.2.1/pydra/tasks/dcm2niix/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:10:34.248033 pydra-dcm2niix-1.2.1/pydra_dcm2niix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-11 01:10:34.000000 pydra-dcm2niix-1.2.1/pydra_dcm2niix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-11 01:10:34.000000 pydra-dcm2niix-1.2.1/pydra_dcm2niix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 01:10:34.000000 pydra-dcm2niix-1.2.1/pydra_dcm2niix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-11 01:10:34.000000 pydra-dcm2niix-1.2.1/pydra_dcm2niix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 01:10:34.000000 pydra-dcm2niix-1.2.1/pydra_dcm2niix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 01:10:21.000000 pydra-dcm2niix-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-11 01:10:34.248033 pydra-dcm2niix-1.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      828 2023-07-11 01:10:21.000000 pydra-dcm2niix-1.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70238 2023-07-11 01:10:21.000000 pydra-dcm2niix-1.2.1/versioneer.py
```

### Comparing `pydra-dcm2niix-1.2.0/LICENSE` & `pydra-dcm2niix-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra-dcm2niix-1.2.0/PKG-INFO` & `pydra-dcm2niix-1.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,14 @@
 Metadata-Version: 2.1
 Name: pydra-dcm2niix
-Version: 1.2.0
+Version: 1.2.1
 Summary: Provides a task interface for the popular dcm2niix DICOM to NIfTI converter
-Home-page: UNKNOWN
 Author: Thomas G. Close
 Author-email: tom.g.close@gmail.com
 License: Apache License, 2.0
-Description: # Pydra Dcm2Niix Task
-        
-        This repository contains Pydra task interface for the `dcm2niix`
-        DICOM to NIfTI converter tool (https://github.com/rordenlab/dcm2niix).
-        
-        Part of this effort is to establish a (mostly) declarative language for describing tasks that
-        potentially have intricate rules for determining the availability and names from the choice of
-        inputs.
-        
-        ## Installation
-        ```
-        pip install /path/to/pydra-dcm2niix/
-        ```
-        
-        ### Installation for developers
-        ```
-        pip install -e /path/to/pydra-dcm2niix/[dev]
-        ```
-        
-        ## Basic Use
-        
-        To run the `dcm2niix` task
-        
-        ```
-        from pydra.tasks.dcm2niix import Dcm2Niix
-        
-        task = Dcm2Niix(in_dir='/path/to/dicom/dir', out_dir='/path/to/create/nifti/output')
-        result = task()
-        ```
-        
-        However, the converter task interface will typically be used as the first step within larger Pydra workflows
-        
-        ```
-        from pydra import Workflow
-        from pydra.tasks.dcm2niix import Dcm2Niix
-        
-        my_workflow = Workflow(name='my_workflow', input_spec=['in_dicom'])
-        
-        my_workflow.add(
-            Dcm2Niix(name='converter', in_dir=my_workflow.lzin.in_dicom, out_dir='.'))
-        my_workflow.add(...)
-        
-        my_workflow()
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
@@ -66,7 +19,53 @@
 Description-Content-Type: text/markdown; variant=CommonMark
 Provides-Extra: doc
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: tests
 Provides-Extra: dev
 Provides-Extra: all
+License-File: LICENSE
+
+# Pydra Dcm2Niix Task
+
+This repository contains Pydra task interface for the `dcm2niix`
+DICOM to NIfTI converter tool (https://github.com/rordenlab/dcm2niix).
+
+Part of this effort is to establish a (mostly) declarative language for describing tasks that
+potentially have intricate rules for determining the availability and names from the choice of
+inputs.
+
+## Installation
+```
+pip install /path/to/pydra-dcm2niix/
+```
+
+### Installation for developers
+```
+pip install -e /path/to/pydra-dcm2niix/[dev]
+```
+
+## Basic Use
+
+To run the `dcm2niix` task
+
+```
+from pydra.tasks.dcm2niix import Dcm2Niix
+
+task = Dcm2Niix(in_dir='/path/to/dicom/dir', out_dir='/path/to/create/nifti/output')
+result = task()
+```
+
+However, the converter task interface will typically be used as the first step within larger Pydra workflows
+
+```
+from pydra import Workflow
+from pydra.tasks.dcm2niix import Dcm2Niix
+
+my_workflow = Workflow(name='my_workflow', input_spec=['in_dicom'])
+
+my_workflow.add(
+    Dcm2Niix(name='converter', in_dir=my_workflow.lzin.in_dicom, out_dir='.'))
+my_workflow.add(...)
+
+my_workflow()
+```
```

### Comparing `pydra-dcm2niix-1.2.0/README.md` & `pydra-dcm2niix-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pydra-dcm2niix-1.2.0/pydra/tasks/dcm2niix/utils.py` & `pydra-dcm2niix-1.2.1/pydra/tasks/dcm2niix/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,31 +14,33 @@
 
     # Check to see if multiple echos exist in the DICOM dataset
     if not fpath.exists():
         if file_postfix is not None:  # NB: doesn't match attrs.NOTHING
             neighbours = [
                 str(p) for p in fpath.parent.iterdir() if p.name.endswith(ext)
             ]
-            raise ValueError(
-                f"\nDid not find expected file '{fpath}' (file_postfix={file_postfix}) "
-                "after DICOM -> NIfTI conversion, please see "
-                "https://github.com/rordenlab/dcm2niix/blob/master/FILENAMING.md for the "
-                "list of postfixes that dcm2niix produces and provide an appropriate "
-                "postfix, or set postfix to None to ignore matching a single file and use "
-                "the list returned in 'out_files' instead. Found the following files "
-                "with matching extensions:\n" + "\n".join(neighbours)
-            )
+            if len(neighbours) == 1 and file_postfix is attrs.NOTHING:
+                fpath = neighbours[0]
+            else:
+                raise ValueError(
+                    f"\nDid not find expected file '{fpath}' (file_postfix={file_postfix}) "
+                    "after DICOM -> NIfTI conversion, please see "
+                    "https://github.com/rordenlab/dcm2niix/blob/master/FILENAMING.md for the "
+                    "list of postfixes that dcm2niix produces and provide an appropriate "
+                    "postfix, or set postfix to None to ignore matching a single file and use "
+                    "the list returned in 'out_files' instead. Found the following files "
+                    "with matching extensions:\n" + "\n".join(neighbours)
+                )
         else:
             fpath = attrs.NOTHING  # Did not find output path and
 
     return fpath
 
 
 def dcm2niix_out_file(out_dir, filename, file_postfix, compress):
-
     ext = ".nii"
     # If compressed, append the zip extension
     if compress in ("y", "o", "i"):
         ext += ".gz"
 
     return out_file_path(out_dir, filename, file_postfix, ext)
 
@@ -69,15 +71,15 @@
             "position": -1,
             "help_string": ("The directory containing the DICOMs to be converted"),
             "mandatory": True,
         },
     ),
     (
         "out_dir",
-        Directory,
+        Path,
         {
             "argstr": "-o '{out_dir}'",
             "help_string": "output directory",
             "mandatory": True,
         },
     ),
     (
```

### Comparing `pydra-dcm2niix-1.2.0/pydra_dcm2niix.egg-info/PKG-INFO` & `pydra-dcm2niix-1.2.1/pydra_dcm2niix.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,14 @@
 Metadata-Version: 2.1
 Name: pydra-dcm2niix
-Version: 1.2.0
+Version: 1.2.1
 Summary: Provides a task interface for the popular dcm2niix DICOM to NIfTI converter
-Home-page: UNKNOWN
 Author: Thomas G. Close
 Author-email: tom.g.close@gmail.com
 License: Apache License, 2.0
-Description: # Pydra Dcm2Niix Task
-        
-        This repository contains Pydra task interface for the `dcm2niix`
-        DICOM to NIfTI converter tool (https://github.com/rordenlab/dcm2niix).
-        
-        Part of this effort is to establish a (mostly) declarative language for describing tasks that
-        potentially have intricate rules for determining the availability and names from the choice of
-        inputs.
-        
-        ## Installation
-        ```
-        pip install /path/to/pydra-dcm2niix/
-        ```
-        
-        ### Installation for developers
-        ```
-        pip install -e /path/to/pydra-dcm2niix/[dev]
-        ```
-        
-        ## Basic Use
-        
-        To run the `dcm2niix` task
-        
-        ```
-        from pydra.tasks.dcm2niix import Dcm2Niix
-        
-        task = Dcm2Niix(in_dir='/path/to/dicom/dir', out_dir='/path/to/create/nifti/output')
-        result = task()
-        ```
-        
-        However, the converter task interface will typically be used as the first step within larger Pydra workflows
-        
-        ```
-        from pydra import Workflow
-        from pydra.tasks.dcm2niix import Dcm2Niix
-        
-        my_workflow = Workflow(name='my_workflow', input_spec=['in_dicom'])
-        
-        my_workflow.add(
-            Dcm2Niix(name='converter', in_dir=my_workflow.lzin.in_dicom, out_dir='.'))
-        my_workflow.add(...)
-        
-        my_workflow()
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
@@ -66,7 +19,53 @@
 Description-Content-Type: text/markdown; variant=CommonMark
 Provides-Extra: doc
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: tests
 Provides-Extra: dev
 Provides-Extra: all
+License-File: LICENSE
+
+# Pydra Dcm2Niix Task
+
+This repository contains Pydra task interface for the `dcm2niix`
+DICOM to NIfTI converter tool (https://github.com/rordenlab/dcm2niix).
+
+Part of this effort is to establish a (mostly) declarative language for describing tasks that
+potentially have intricate rules for determining the availability and names from the choice of
+inputs.
+
+## Installation
+```
+pip install /path/to/pydra-dcm2niix/
+```
+
+### Installation for developers
+```
+pip install -e /path/to/pydra-dcm2niix/[dev]
+```
+
+## Basic Use
+
+To run the `dcm2niix` task
+
+```
+from pydra.tasks.dcm2niix import Dcm2Niix
+
+task = Dcm2Niix(in_dir='/path/to/dicom/dir', out_dir='/path/to/create/nifti/output')
+result = task()
+```
+
+However, the converter task interface will typically be used as the first step within larger Pydra workflows
+
+```
+from pydra import Workflow
+from pydra.tasks.dcm2niix import Dcm2Niix
+
+my_workflow = Workflow(name='my_workflow', input_spec=['in_dicom'])
+
+my_workflow.add(
+    Dcm2Niix(name='converter', in_dir=my_workflow.lzin.in_dicom, out_dir='.'))
+my_workflow.add(...)
+
+my_workflow()
+```
```

### Comparing `pydra-dcm2niix-1.2.0/pydra_dcm2niix.egg-info/requires.txt` & `pydra-dcm2niix-1.2.1/pydra_dcm2niix.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pydra-dcm2niix-1.2.0/setup.cfg` & `pydra-dcm2niix-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 	black
 	pre-commit
 all = 
 	%(doc)s
 	%(dev)s
 
 [versioneer]
-vcs = git
+VCS = git
 style = pep440
 versionfile_source = pydra/tasks/dcm2niix/_version.py
 versionfile_build = pydra/tasks/dcm2niix/_version.py
 tag_prefix = 
 parentdir_prefix = 
 
 [tool:pytest]
```

### Comparing `pydra-dcm2niix-1.2.0/setup.py` & `pydra-dcm2niix-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `pydra-dcm2niix-1.2.0/versioneer.py` & `pydra-dcm2niix-1.2.1/versioneer.py`

 * *Files identical despite different names*

