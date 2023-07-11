# Comparing `tmp/rubberduckie-2023.5.1-py3-none-any.whl.zip` & `tmp/rubberduckie-2023.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,18 @@
-Zip file size: 4502 bytes, number of entries: 13
--rw-r--r--  2.0 unx      181 b- defN 23-May-22 10:41 rubberduckie/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 09:48 rubberduckie/db/__init__.py
--rw-r--r--  2.0 unx     2956 b- defN 23-May-22 10:19 rubberduckie/db/hadoop.py
+Zip file size: 7085 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      346 b- defN 23-Jul-11 05:21 rubberduckie/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-22 09:48 rubberduckie/cdsw/__init__.py
+-rw-r--r--  2.0 unx     2956 b- defN 23-May-22 10:19 rubberduckie/cdsw/hadoop.py
+-rw-r--r--  2.0 unx     3400 b- defN 23-Jul-11 05:19 rubberduckie/cdsw/import_fix.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 05:14 rubberduckie/da/__init__.py
+-rw-r--r--  2.0 unx     2439 b- defN 23-Jul-11 05:20 rubberduckie/da/pilot.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-22 11:00 rubberduckie/dl/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-22 04:32 rubberduckie/ml/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-22 04:32 rubberduckie/plot/__init__.py
 -rw-r--r--  2.0 unx     1835 b- defN 23-May-22 10:38 rubberduckie/plot/evaluation.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-22 04:32 rubberduckie/xai/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 11:21 rubberduckie-2023.5.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      420 b- defN 23-May-22 11:21 rubberduckie-2023.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 11:21 rubberduckie-2023.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-May-22 11:21 rubberduckie-2023.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1084 b- defN 23-May-22 11:21 rubberduckie-2023.5.1.dist-info/RECORD
-13 files, 6581 bytes uncompressed, 2650 bytes compressed:  59.7%
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 05:27 rubberduckie-2023.7.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      420 b- defN 23-Jul-11 05:27 rubberduckie-2023.7.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 05:27 rubberduckie-2023.7.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Jul-11 05:27 rubberduckie-2023.7.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1338 b- defN 23-Jul-11 05:27 rubberduckie-2023.7.1.dist-info/RECORD
+16 files, 12839 bytes uncompressed, 4833 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -1,14 +1,23 @@
 Filename: rubberduckie/__init__.py
 Comment: 
 
-Filename: rubberduckie/db/__init__.py
+Filename: rubberduckie/cdsw/__init__.py
 Comment: 
 
-Filename: rubberduckie/db/hadoop.py
+Filename: rubberduckie/cdsw/hadoop.py
+Comment: 
+
+Filename: rubberduckie/cdsw/import_fix.py
+Comment: 
+
+Filename: rubberduckie/da/__init__.py
+Comment: 
+
+Filename: rubberduckie/da/pilot.py
 Comment: 
 
 Filename: rubberduckie/dl/__init__.py
 Comment: 
 
 Filename: rubberduckie/ml/__init__.py
 Comment: 
@@ -18,23 +27,23 @@
 
 Filename: rubberduckie/plot/evaluation.py
 Comment: 
 
 Filename: rubberduckie/xai/__init__.py
 Comment: 
 
-Filename: rubberduckie-2023.5.1.dist-info/LICENSE.txt
+Filename: rubberduckie-2023.7.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: rubberduckie-2023.5.1.dist-info/METADATA
+Filename: rubberduckie-2023.7.1.dist-info/METADATA
 Comment: 
 
-Filename: rubberduckie-2023.5.1.dist-info/WHEEL
+Filename: rubberduckie-2023.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: rubberduckie-2023.5.1.dist-info/top_level.txt
+Filename: rubberduckie-2023.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rubberduckie-2023.5.1.dist-info/RECORD
+Filename: rubberduckie-2023.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rubberduckie/__init__.py

```diff
@@ -1,8 +1,18 @@
-from rubberduckie.db.hadoop import (
+from rubberduckie.cdsw.hadoop import (
     prepare_connection,
     execute_db_query,
     extract_db_data,
 )
+
+from rubberduckie.cdsw.import_fix import (
+    fix_cdsw_import_error,
+)
+
 from rubberduckie.plot.evaluation import (
     prepare_confusion_matrix,
 )
+
+from rubberduckie.da.pilot import (
+    calc_weeks_between,
+    prepare_dev_triangle,
+)
```

## Comparing `rubberduckie/db/hadoop.py` & `rubberduckie/cdsw/hadoop.py`

 * *Files identical despite different names*

## Comparing `rubberduckie-2023.5.1.dist-info/RECORD` & `rubberduckie-2023.7.1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-rubberduckie/__init__.py,sha256=P32lOv8vmAIMA8-y3wbH7XOWDRMKA8ClWpj1prWau5g,181
-rubberduckie/db/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rubberduckie/db/hadoop.py,sha256=upDJewzqbCDwCpB7SoUytxYUe143VQcEyleyha0CUEU,2956
+rubberduckie/__init__.py,sha256=NOHg64NlglW-sWLjuS_r53NC_lL1F-KbmDMkBziPlxA,346
+rubberduckie/cdsw/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+rubberduckie/cdsw/hadoop.py,sha256=upDJewzqbCDwCpB7SoUytxYUe143VQcEyleyha0CUEU,2956
+rubberduckie/cdsw/import_fix.py,sha256=vFb7-KpvfcqOzCJ9wTRm5EZmOgebWwlowZ4IafIaMME,3400
+rubberduckie/da/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+rubberduckie/da/pilot.py,sha256=Cs5S7_8d-6ZAtLc74NEdFAc49bmxGE_XlYHTqUnu498,2439
 rubberduckie/dl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rubberduckie/ml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rubberduckie/plot/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rubberduckie/plot/evaluation.py,sha256=tzB_TrCYyMRaC0I-5RLJxPbjbPVtgByFTmZuWDmAma0,1835
 rubberduckie/xai/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rubberduckie-2023.5.1.dist-info/LICENSE.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rubberduckie-2023.5.1.dist-info/METADATA,sha256=3kU3dFLXIiwKGY0fALE_roVZN13eCA--bFuR5jTaDl0,420
-rubberduckie-2023.5.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rubberduckie-2023.5.1.dist-info/top_level.txt,sha256=10EHDBDRla6FQ9v_RwhUA08sGKU1P499ZlDoj2XQXqc,13
-rubberduckie-2023.5.1.dist-info/RECORD,,
+rubberduckie-2023.7.1.dist-info/LICENSE.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+rubberduckie-2023.7.1.dist-info/METADATA,sha256=biXi6-pTpgxgzxqfXgyZzbVrbOH0W7g-FP28k-CdGXs,420
+rubberduckie-2023.7.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rubberduckie-2023.7.1.dist-info/top_level.txt,sha256=10EHDBDRla6FQ9v_RwhUA08sGKU1P499ZlDoj2XQXqc,13
+rubberduckie-2023.7.1.dist-info/RECORD,,
```

