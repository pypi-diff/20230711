# Comparing `tmp/pypeec-0.0.2.tar.gz` & `tmp/pypeec-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypeec-0.0.2.tar", last modified: Fri Jun 23 23:03:04 2023, max compression
+gzip compressed data, was "pypeec-0.0.3.tar", last modified: Mon Jul 10 23:01:03 2023, max compression
```

## Comparing `pypeec-0.0.2.tar` & `pypeec-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2023-06-23 23:03:04.320638 pypeec-0.0.2/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      530 2023-05-06 19:25:22.000000 pypeec-0.0.2/LICENSE.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1082 2023-06-23 23:03:04.320638 pypeec-0.0.2/PKG-INFO
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      843 2023-06-23 22:40:59.000000 pypeec-0.0.2/README.md
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2023-06-23 23:03:04.320638 pypeec-0.0.2/pypeec/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     5111 2023-05-06 19:25:22.000000 pypeec-0.0.2/pypeec/gerber_png.py
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2023-06-23 23:03:04.320638 pypeec-0.0.2/pypeec.egg-info/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1082 2023-06-23 23:03:04.000000 pypeec-0.0.2/pypeec.egg-info/PKG-INFO
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      216 2023-06-23 23:03:04.000000 pypeec-0.0.2/pypeec.egg-info/SOURCES.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        1 2023-06-23 23:03:04.000000 pypeec-0.0.2/pypeec.egg-info/dependency_links.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       47 2023-06-23 23:03:04.000000 pypeec-0.0.2/pypeec.egg-info/requires.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        7 2023-06-23 23:03:04.000000 pypeec-0.0.2/pypeec.egg-info/top_level.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       94 2023-06-23 22:44:40.000000 pypeec-0.0.2/pyproject.toml
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      402 2023-06-23 23:03:04.320638 pypeec-0.0.2/setup.cfg
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2023-07-10 23:01:03.065753 pypeec-0.0.3/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      530 2023-05-06 19:25:22.000000 pypeec-0.0.3/LICENSE.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1105 2023-07-10 23:01:03.065753 pypeec-0.0.3/PKG-INFO
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      866 2023-07-10 22:55:29.000000 pypeec-0.0.3/README.md
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2023-07-10 23:01:03.061753 pypeec-0.0.3/pypeec/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     5111 2023-05-06 19:25:22.000000 pypeec-0.0.3/pypeec/gerber_png.py
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2023-07-10 23:01:03.065753 pypeec-0.0.3/pypeec.egg-info/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1105 2023-07-10 23:01:03.000000 pypeec-0.0.3/pypeec.egg-info/PKG-INFO
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      216 2023-07-10 23:01:03.000000 pypeec-0.0.3/pypeec.egg-info/SOURCES.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        1 2023-07-10 23:01:03.000000 pypeec-0.0.3/pypeec.egg-info/dependency_links.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       47 2023-07-10 23:01:03.000000 pypeec-0.0.3/pypeec.egg-info/requires.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        7 2023-07-10 23:01:03.000000 pypeec-0.0.3/pypeec.egg-info/top_level.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       94 2023-06-23 22:44:40.000000 pypeec-0.0.3/pyproject.toml
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      402 2023-07-10 23:01:03.065753 pypeec-0.0.3/setup.cfg
```

### Comparing `pypeec-0.0.2/LICENSE.txt` & `pypeec-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypeec-0.0.2/PKG-INFO` & `pypeec-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: pypeec
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyPEEC
 Author: Thomas Guillod
 Author-email: guillod@otvam.ch
 License: All rights reserved
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # PyPEEC
 
+![banner](banner.png)
+
 ## Author
 
 * **Thomas Guillod**, Dartmouth College, NH, USA
 * Email: [guillod@otvam.ch](mailto:guillod@otvam.ch)
 * Personal website: [https://otvam.ch](https://otvam.ch)
 * Lab website: [https://pmic.engineering.dartmouth.edu](https://pmic.engineering.dartmouth.edu)
```

### Comparing `pypeec-0.0.2/README.md` & `pypeec-0.0.3/pypeec.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,22 @@
+Metadata-Version: 2.1
+Name: pypeec
+Version: 0.0.3
+Summary: PyPEEC
+Author: Thomas Guillod
+Author-email: guillod@otvam.ch
+License: All rights reserved
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # PyPEEC
 
+![banner](banner.png)
+
 ## Author
 
 * **Thomas Guillod**, Dartmouth College, NH, USA
 * Email: [guillod@otvam.ch](mailto:guillod@otvam.ch)
 * Personal website: [https://otvam.ch](https://otvam.ch)
 * Lab website: [https://pmic.engineering.dartmouth.edu](https://pmic.engineering.dartmouth.edu)
```

### Comparing `pypeec-0.0.2/pypeec/gerber_png.py` & `pypeec-0.0.3/pypeec/gerber_png.py`

 * *Files identical despite different names*

### Comparing `pypeec-0.0.2/pypeec.egg-info/PKG-INFO` & `pypeec-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,11 @@
-Metadata-Version: 2.1
-Name: pypeec
-Version: 0.0.2
-Summary: PyPEEC
-Author: Thomas Guillod
-Author-email: guillod@otvam.ch
-License: All rights reserved
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # PyPEEC
 
+![banner](banner.png)
+
 ## Author
 
 * **Thomas Guillod**, Dartmouth College, NH, USA
 * Email: [guillod@otvam.ch](mailto:guillod@otvam.ch)
 * Personal website: [https://otvam.ch](https://otvam.ch)
 * Lab website: [https://pmic.engineering.dartmouth.edu](https://pmic.engineering.dartmouth.edu)
```

