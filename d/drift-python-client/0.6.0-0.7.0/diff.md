# Comparing `tmp/drift_python_client-0.6.0-py3-none-any.whl.zip` & `tmp/drift_python_client-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 23598 bytes, number of entries: 13
--rw-r--r--  2.0 unx      140 b- defN 23-Jun-16 15:04 drift_client/__init__.py
--rw-r--r--  2.0 unx    11878 b- defN 23-Jun-16 15:04 drift_client/drift_client.py
--rw-r--r--  2.0 unx     3419 b- defN 23-Jun-16 15:04 drift_client/drift_data_package.py
--rw-r--r--  2.0 unx      100 b- defN 23-Jun-16 15:04 drift_client/error.py
--rw-r--r--  2.0 unx     2644 b- defN 23-Jun-16 15:04 drift_client/influxdb_client.py
--rw-r--r--  2.0 unx     1908 b- defN 23-Jun-16 15:04 drift_client/minio_client.py
--rw-r--r--  2.0 unx     4047 b- defN 23-Jun-16 15:04 drift_client/mqtt_client.py
--rw-r--r--  2.0 unx     4420 b- defN 23-Jun-16 15:04 drift_client/reduct_client.py
--rw-r--r--  2.0 unx    16725 b- defN 23-Jun-16 15:05 drift_python_client-0.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    23644 b- defN 23-Jun-16 15:05 drift_python_client-0.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 15:05 drift_python_client-0.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-16 15:05 drift_python_client-0.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1125 b- defN 23-Jun-16 15:05 drift_python_client-0.6.0.dist-info/RECORD
-13 files, 70155 bytes uncompressed, 21706 bytes compressed:  69.1%
+Zip file size: 23671 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      140 b- defN 23-Jul-11 07:41 drift_client/__init__.py
+-rw-r--r--  2.0 unx    11878 b- defN 23-Jul-11 07:41 drift_client/drift_client.py
+-rw-r--r--  2.0 unx     3635 b- defN 23-Jul-11 07:41 drift_client/drift_data_package.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Jul-11 07:41 drift_client/error.py
+-rw-r--r--  2.0 unx     2644 b- defN 23-Jul-11 07:41 drift_client/influxdb_client.py
+-rw-r--r--  2.0 unx     1908 b- defN 23-Jul-11 07:41 drift_client/minio_client.py
+-rw-r--r--  2.0 unx     4047 b- defN 23-Jul-11 07:41 drift_client/mqtt_client.py
+-rw-r--r--  2.0 unx     4420 b- defN 23-Jul-11 07:41 drift_client/reduct_client.py
+-rw-r--r--  2.0 unx    16725 b- defN 23-Jul-11 07:41 drift_python_client-0.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    23644 b- defN 23-Jul-11 07:41 drift_python_client-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 07:41 drift_python_client-0.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Jul-11 07:41 drift_python_client-0.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1125 b- defN 23-Jul-11 07:41 drift_python_client-0.7.0.dist-info/RECORD
+13 files, 70371 bytes uncompressed, 21779 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: drift_client/mqtt_client.py
 Comment: 
 
 Filename: drift_client/reduct_client.py
 Comment: 
 
-Filename: drift_python_client-0.6.0.dist-info/LICENSE
+Filename: drift_python_client-0.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: drift_python_client-0.6.0.dist-info/METADATA
+Filename: drift_python_client-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: drift_python_client-0.6.0.dist-info/WHEEL
+Filename: drift_python_client-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: drift_python_client-0.6.0.dist-info/top_level.txt
+Filename: drift_python_client-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: drift_python_client-0.6.0.dist-info/RECORD
+Filename: drift_python_client-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## drift_client/drift_data_package.py

```diff
@@ -1,9 +1,9 @@
 """Wrapper around DriftPackage"""
-from typing import Optional
+from typing import Optional, Dict
 
 from wavelet_buffer import WaveletBuffer  # pylint: disable=no-name-in-module
 from drift_protocol.common import DataPayload, DriftPackage, StatusCode
 from drift_protocol.meta import MetaInfo
 
 import numpy as np
 
@@ -126,7 +126,16 @@
 
         Args:
             scale_factor: Wavelet composition factor, defaults to 0
         Returns:
             Data payload as NumPy Array
         """
         return self.as_buffer().compose(scale_factor)
+
+    @property
+    def labels(self) -> Dict[str, str]:
+        """Labels as dict"""
+        labels = {}
+        for label in self._pkg.labels:
+            labels[label.key] = label.value
+
+        return labels
```

## Comparing `drift_python_client-0.6.0.dist-info/LICENSE` & `drift_python_client-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `drift_python_client-0.6.0.dist-info/METADATA` & `drift_python_client-0.7.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drift-python-client
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python Client to access data of PANDA|Drift
 Author-email: "PANDA, GmbH" <info@panda.technology>
 Maintainer-email: "PANDA, GmbH" <info@panda.technology>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
@@ -392,19 +392,19 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: influxdb-client (<2.0.0,>=1.36.1)
 Requires-Dist: drift-protocol (<1.0.0,>=0.5.0)
-Requires-Dist: wavelet-buffer (<1.0.0,>=0.6.0)
+Requires-Dist: wavelet-buffer (<1.0.0,>=0.7.0)
 Requires-Dist: paho-mqtt (<2.0.0,>=1.6.1)
 Requires-Dist: numpy (<2.0.0,>=1.24.3)
 Requires-Dist: deprecation (==2.1.0)
-Requires-Dist: reduct-py (<2.0.0,>=1.4)
+Requires-Dist: reduct-py (<2.0.0,>=1.5)
 Requires-Dist: minio (==7.1.10)
 Provides-Extra: docs
 Requires-Dist: mkdocs (<2.0.0,>=1.4.3) ; extra == 'docs'
 Requires-Dist: mkdocs-material (<10.0.0,>=9.1.16) ; extra == 'docs'
 Requires-Dist: plantuml-markdown (<4.0.0,>=3.9.1) ; extra == 'docs'
 Requires-Dist: mkdocstrings[python] (~=0.22) ; extra == 'docs'
 Requires-Dist: mkdocs-jupyter (~=0.24) ; extra == 'docs'
```

## Comparing `drift_python_client-0.6.0.dist-info/RECORD` & `drift_python_client-0.7.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 drift_client/__init__.py,sha256=pV24wjUn9l6ohjXcTeIX16m62YTrJjxt_jCwIIJX-Gk,140
 drift_client/drift_client.py,sha256=Z8yQvqW_zd63mykj8-mFxB6_fBFAmvUz0a2HMhtZ54c,11878
-drift_client/drift_data_package.py,sha256=-v8Wbhv7PU3WlpfWIAO6aVkhciD0Pox8onKOCBTrkL0,3419
+drift_client/drift_data_package.py,sha256=HLJUURTxWeHKFQqLncD3lltScCzqvCWd2pp4xwxwPmI,3635
 drift_client/error.py,sha256=VSSWHJiakIsRjtGx8sHyJ0nqS0uYavrc9TCFIuD7atA,100
 drift_client/influxdb_client.py,sha256=n_7rNPOI_h3r7Ry0uBgZV59ECDk2mSaJaW5lMhLYZDM,2644
 drift_client/minio_client.py,sha256=LqPBOIwtdOLY05YPVZpmb9eHsvJeqFxwn81bXHyG4xg,1908
 drift_client/mqtt_client.py,sha256=4-r4ZomTrw7YHqLZ6SU-PLmhxuw8CGqeMxzANFxz2wk,4047
 drift_client/reduct_client.py,sha256=4PFXX2XIjBZPszCLrPWjt3qXncunV1hIpWKctBDTMag,4420
-drift_python_client-0.6.0.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-drift_python_client-0.6.0.dist-info/METADATA,sha256=f1UhbeWUuZuUDifl-o4hrzb7k5ReTWd4wcwypF95UPM,23644
-drift_python_client-0.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-drift_python_client-0.6.0.dist-info/top_level.txt,sha256=g36GfF0WcMjKkwPW7zawUU5n5XsLJT-4oLxcVgeobno,13
-drift_python_client-0.6.0.dist-info/RECORD,,
+drift_python_client-0.7.0.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+drift_python_client-0.7.0.dist-info/METADATA,sha256=sng7JcyMEjI4gXhHbi5ZIldSyrZa3sov5UKHvU6FPaE,23644
+drift_python_client-0.7.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+drift_python_client-0.7.0.dist-info/top_level.txt,sha256=g36GfF0WcMjKkwPW7zawUU5n5XsLJT-4oLxcVgeobno,13
+drift_python_client-0.7.0.dist-info/RECORD,,
```

