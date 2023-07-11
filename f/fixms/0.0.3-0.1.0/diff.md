# Comparing `tmp/fixms-0.0.3.tar.gz` & `tmp/fixms-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixms-0.0.3.tar", max compression
+gzip compressed data, was "fixms-0.1.0.tar", max compression
```

## Comparing `fixms-0.0.3.tar` & `fixms-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-09 12:05:08.417412 fixms-0.0.3/LICENSE
--rw-r--r--   0        0        0     3097 2023-07-09 12:05:08.417412 fixms-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-07-09 12:05:08.417412 fixms-0.0.3/fixms/__init__.py
--rw-r--r--   0        0        0    12266 2023-07-09 12:05:08.417412 fixms-0.0.3/fixms/fix_ms_corrs.py
--rw-r--r--   0        0        0    12469 2023-07-09 12:05:08.417412 fixms-0.0.3/fixms/fix_ms_dir.py
--rw-r--r--   0        0        0      729 2023-07-09 12:05:08.417412 fixms-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3742 1970-01-01 00:00:00.000000 fixms-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-11 09:04:59.115948 fixms-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3920 2023-07-11 09:04:59.115948 fixms-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 09:04:59.115948 fixms-0.1.0/fixms/__init__.py
+-rw-r--r--   0        0        0     1478 2023-07-11 09:04:59.115948 fixms-0.1.0/fixms/fix_ms.py
+-rw-r--r--   0        0        0    13572 2023-07-11 09:04:59.119949 fixms-0.1.0/fixms/fix_ms_corrs.py
+-rw-r--r--   0        0        0    12469 2023-07-11 09:04:59.119949 fixms-0.1.0/fixms/fix_ms_dir.py
+-rw-r--r--   0        0        0      757 2023-07-11 09:04:59.119949 fixms-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4565 1970-01-01 00:00:00.000000 fixms-0.1.0/PKG-INFO
```

### Comparing `fixms-0.0.3/LICENSE` & `fixms-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fixms-0.0.3/README.md` & `fixms-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 ASKAP MSs are produced in a way that breaks compatibility with most other imagers (e.g. CASA, WSclean). Here we provide two modules (with CLI hooks) that perform the fixes that need to be applied in order to produce astronomically correct imagers with non-YandaSoft imagers:
 
 1. `fix_ms_dir` : ASKAP MeasurementSets are phased towards the centre of field, but not the centre of its given beam. This utility reads the appropriate offsets to the beam centre from the `BEAM_OFFSET` and updates the `FIELD` table, as well as the phase and delay reference columns.
 
 2. `fix_ms_corrs` : ASKAP MeasurementSets, as calibrated by the obervatory, provide correlations in the instrument frame. ASKAP has a unique 'roll' axis which means, in principle, the instrument frame can be at any arbitrary rotation on the sky. This utility applies the appropriate rotation matrix to the visibilities such the 'X' is aligned North-South and 'Y' is aligned East-West (IAU convention). Further, ASKAPsoft defines Stokes I as $I=XX+YY$, whereas most other telescopes use $I=\frac{1}{2}(XX+YY)$ (note this also applies to all other Stokes paramters). This factor is also corrected for here at the same time as the rotation.
 
+For convenience, we also provide `fix_ms` which does both of the above!
+
 Full documentation on [Read The Docs](https://fixms.readthedocs.io/en/latest/).
 
 ## Installation
 
 Obtain and install Python 3 (I recommend [Miniforge](https://github.com/conda-forge/miniforge) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html)).
 
 Install the Python scripts:
@@ -27,31 +29,51 @@
 ```
 pip install FixMS
 ```
 
 ## Usage
 
 ```
+❯ fix_ms -h
+usage: fix_ms [-h] [--chunksize CHUNKSIZE] [--data-column DATA_COLUMN] [--corrected-data-column CORRECTED_DATA_COLUMN] [ms]
+
+Utility to correct the ASKAP beam positions and apply a rotation to apply a change of the reference frame of the visibilities
+
+positional arguments:
+  ms                    Measurement set to update (default: None)
+
+options:
+  -h, --help            show this help message and exit
+  --chunksize CHUNKSIZE
+                        The chunksize to use when reading the MS (default: 1000)
+  --data-column DATA_COLUMN
+                        The column to fix (default: DATA)
+  --corrected-data-column CORRECTED_DATA_COLUMN
+                        The column to write the corrected data to (default: CORRECTED_DATA)
+```
+
+```
 ❯ fix_ms_corrs -h
 usage: fix_ms_corrs [-h] [--chunksize CHUNKSIZE] [--data-column DATA_COLUMN] [--corrected-data-column CORRECTED_DATA_COLUMN] ms
 
 Fix the correlation rotation of ASKAP MSs. Converts the ASKAP standard correlations to the 'standard' correlations This will make them compatible with most imagers (e.g. wsclean, CASA) The new correlations are placed in a new column called 'CORRECTED_DATA'
 
 positional arguments:
   ms                    The MS to fix
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --chunksize CHUNKSIZE
                         The chunksize to use when reading the MS (default: 1000)
   --data-column DATA_COLUMN
                         The column to fix (default: DATA)
   --corrected-data-column CORRECTED_DATA_COLUMN
                         The column to write the corrected data to (default: CORRECTED_DATA)
 ```
+
 ```
 ❯ fix_ms_dir -h
 usage: fix_ms_dir [-h] [ms]
 
 ASKAP utility - update the pointing centre of a beam in an MS. - Allows imaging by CASA or wsclean.
 
 positional arguments:
```

### Comparing `fixms-0.0.3/fixms/fix_ms_corrs.py` & `fixms-0.1.0/fixms/fix_ms_corrs.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,44 +7,55 @@
 This will make them compatible with most imagers (e.g. wsclean, CASA)
 
 The new correlations are placed in a new column called 'CORRECTED_DATA'
 """
 __author__ = ["Alec Thomson"]
 import logging
 from pathlib import Path
-from typing import Iterator
+from typing import Iterator, Optional
 
 import astropy.units as u
 import numpy as np
 from casacore.tables import makecoldesc, table
 from tqdm import tqdm
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 
-def get_pol_axis(ms: Path) -> u.Quantity:
+def get_pol_axis(ms: Path, feed_idx: Optional[int] = None) -> u.Quantity:
     """Get the polarization axis from the ASKAP MS. Checks are performed
     to ensure this polarisation axis angle is constant throughout the observation.
 
 
     Args:
         ms (Path): The path to the measurement set that will be inspected
+        feed_idx (Optional[int], optional): Specify the entery in the FEED
+        table of `ms` to return. This might be required when a subset of a
+        measurement set has been extracted from an observation with a varying
+        orientation.
 
     Returns:
         astropy.units.Quantity: The rotation of the PAF throughout the observing.
     """
     with table((ms / "FEED").as_posix(), readonly=True, ack=False) as tf:
         ms_feed = tf.getcol("RECEPTOR_ANGLE") * u.rad
         pol_axes = -(ms_feed - 45.0 * u.deg)
 
-    assert (ms_feed[:, 0] == ms_feed[0, 0]).all() & (
-        ms_feed[:, 1] == ms_feed[0, 1]
-    ).all(), "The RECEPTOR_ANGLE changes with time, please check the MS"
-    return pol_axes[0, 0].to(u.deg)
+    if feed_idx is None:
+        assert (ms_feed[:, 0] == ms_feed[0, 0]).all() & (
+            ms_feed[:, 1] == ms_feed[0, 1]
+        ).all(), "The RECEPTOR_ANGLE changes with time, please check the MS"
+
+        pol_ang = pol_axes[0, 0].to(u.deg)
+    else:
+        logger.debug(f"Extracting the third-axis orientation for {feed_idx=}")
+        pol_ang = pol_axes[feed_idx, 0].to(u.deg)
+
+    return pol_ang
 
 
 def convert_correlations(correlations: np.ndarray, pol_axis: u.Quantity) -> np.ndarray:
     """
     Convert ASKAP standard correlations to the 'standard' correlations
 
     Args:
@@ -157,40 +168,40 @@
         ]
     )
     # This is a matrix multiplication broadcasted along the time and channel axes
     return np.einsum("ij,...j->...i", correction_matrix, correlations)
 
 
 def get_data_chunk(
-    ms: Path, chunksize: int, data_column: str = "DATA_ASKAP"
+    ms: Path, chunksize: int, data_column: str = "DATA"
 ) -> Iterator[np.ndarray]:
     """Generator function that will yield a chunk of data from the `ms` data table.
 
     Args:
         ms (Path): Measurement set whose data will be iterated over
         chunksize (int): The number of rows to process per chunk
-        data_column (str, optional): The column name of the data to iterate. Defaults to "DATA_ASKAP".
+        data_column (str, optional): The column name of the data to iterate. Defaults to "DATA".
 
     Yields:
         Iterator[np.ndarray]: Chunk of datta to process
     """
     with table(ms.as_posix(), readonly=True, ack=False) as tab:
         data = tab.__getattr__(data_column)
         for i in range(0, len(data), chunksize):
             yield np.array(data[i : i + chunksize])
 
 
-def get_nchunks(ms: Path, chunksize: int, data_column: str = "DATA_ASKAP") -> int:
+def get_nchunks(ms: Path, chunksize: int, data_column: str = "DATA") -> int:
     """Returns the number of chunks that are needed to iterator over the datacolumsn
     using a specified `chunksize`.
 
     Args:
         ms (Path): Measurement sett thatt will be iterated over
         chunksize (int): Size of a single chunk
-        data_column (str, optional): Name of the datacolumn that will be iterated over. Defaults to "DATA_ASKAP".
+        data_column (str, optional): Name of the datacolumn that will be iterated over. Defaults to "DATA".
 
     Returns:
         int: Number of chunks in a measurement set
     """
     with table(ms.as_posix(), readonly=True, ack=False) as tab:
         return int(np.ceil(len(tab.__getattr__(data_column)) / chunksize))
 
@@ -199,19 +210,20 @@
     ms: Path,
     chunksize: int = 10_000,
     data_column: str = "DATA",
     corrected_data_column: str = "CORRECTED_DATA",
 ) -> None:
     """Apply corrections to the ASKAP visibilities to bring them inline with
     what is expectede from other imagers, including CASA and WSClean. The
-    original data in `data_column` are copied to `DATA_ASKAP`. The corrected
-    datsa are placed back into `data_column`.
+    original data in `data_column` are copied to `corrected_data_column` before
+    the correction is applied. This is done to ensure that the original data
+    are not lost.
 
-    If `CORRECTED_DATA` is detected as an existing column then the correction
-    will not be applied.
+    If 'corrected_data_column' is detected as an existing column then the
+    correction will not be applied.
 
     Args:
         ms (Path): Path of the ASKAP measurement set tto correct.
         chunksize (int, optional): Size of chunked data to correct. Defaults to 10_000.
         data_column (str, optional): The name of the data column to correct. Defaults to "DATA".
         corrected_data_column (str, optional): The name of the corrected data column. Defaults to "CORRECTED_DATA".
     """
@@ -227,16 +239,32 @@
         # Check if 'corrected_data_column' exists
         if corrected_data_column in cols:
             logger.critical(
                 f"Column {corrected_data_column} already exists in {ms}! Exiting..."
             )
             return
 
+        feed1 = np.unique(tab.getcol("FEED1"))
+        feed2 = np.unique(tab.getcol("FEED2"))
+
+        # For some ASKAP observations the orientation of the third-axis changes
+        # throughout the observation. For example, bandpass observations vary
+        # this direction as each beam cycles in the footprint cycles over the
+        # calibrator source.
+        assert len(feed1) == 1 and len(feed2) == 1, "Found more than one feed orientation!"
+        assert (
+            feed1[0] == feed2[0]
+        ), f"The unique feed enteries available in the data table differ, {feed1=} {feed2=}"
+
+        # The two assertions above should enfore enough constraint
+        # to make sure the rotation matix constructed is correct
+        feed_idx = feed1[0]
+
     # Get the polarization axis
-    pol_axis = get_pol_axis(ms)
+    pol_axis = get_pol_axis(ms, feed_idx=feed_idx)
     logger.info(f"Polarization axis is {pol_axis}")
 
     # Get the data chunk by chunk and convert the correlations
     # then write them back to the MS in the 'data_column' column
     data_chunks = get_data_chunk(ms, chunksize, data_column=data_column)
     nchunks = get_nchunks(ms, chunksize, data_column=data_column)
     start_row = 0
```

### Comparing `fixms-0.0.3/fixms/fix_ms_dir.py` & `fixms-0.1.0/fixms/fix_ms_dir.py`

 * *Files identical despite different names*

### Comparing `fixms-0.0.3/pyproject.toml` & `fixms-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fixms"
-version = "0.0.3"
+version = "0.1.0"
 description = ""
 authors = ["Alec Thomson (S&A, Kensington WA) <alec.thomson@csiro.au>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -28,8 +28,9 @@
 
 [tool.poetry.extras]
 dev = ["isort", "black", "sphinx", "numpydoc", "myst_parser", "autoapi", "sphinx-autoapi"]
 
 
 [tool.poetry.scripts]
 fix_ms_corrs = "fixms.fix_ms_corrs:cli"
-fix_ms_dir = "fixms.fix_ms_dir:cli"
+fix_ms_dir = "fixms.fix_ms_dir:cli"
+fix_ms = "fixms.fix_ms:cli"
```

### Comparing `fixms-0.0.3/PKG-INFO` & `fixms-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixms
-Version: 0.0.3
+Version: 0.1.0
 Summary: 
 License: MIT
 Author: Alec Thomson (S&A, Kensington WA)
 Author-email: alec.thomson@csiro.au
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -27,14 +27,16 @@
 
 ASKAP MSs are produced in a way that breaks compatibility with most other imagers (e.g. CASA, WSclean). Here we provide two modules (with CLI hooks) that perform the fixes that need to be applied in order to produce astronomically correct imagers with non-YandaSoft imagers:
 
 1. `fix_ms_dir` : ASKAP MeasurementSets are phased towards the centre of field, but not the centre of its given beam. This utility reads the appropriate offsets to the beam centre from the `BEAM_OFFSET` and updates the `FIELD` table, as well as the phase and delay reference columns.
 
 2. `fix_ms_corrs` : ASKAP MeasurementSets, as calibrated by the obervatory, provide correlations in the instrument frame. ASKAP has a unique 'roll' axis which means, in principle, the instrument frame can be at any arbitrary rotation on the sky. This utility applies the appropriate rotation matrix to the visibilities such the 'X' is aligned North-South and 'Y' is aligned East-West (IAU convention). Further, ASKAPsoft defines Stokes I as $I=XX+YY$, whereas most other telescopes use $I=\frac{1}{2}(XX+YY)$ (note this also applies to all other Stokes paramters). This factor is also corrected for here at the same time as the rotation.
 
+For convenience, we also provide `fix_ms` which does both of the above!
+
 Full documentation on [Read The Docs](https://fixms.readthedocs.io/en/latest/).
 
 ## Installation
 
 Obtain and install Python 3 (I recommend [Miniforge](https://github.com/conda-forge/miniforge) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html)).
 
 Install the Python scripts:
@@ -48,31 +50,51 @@
 ```
 pip install FixMS
 ```
 
 ## Usage
 
 ```
+❯ fix_ms -h
+usage: fix_ms [-h] [--chunksize CHUNKSIZE] [--data-column DATA_COLUMN] [--corrected-data-column CORRECTED_DATA_COLUMN] [ms]
+
+Utility to correct the ASKAP beam positions and apply a rotation to apply a change of the reference frame of the visibilities
+
+positional arguments:
+  ms                    Measurement set to update (default: None)
+
+options:
+  -h, --help            show this help message and exit
+  --chunksize CHUNKSIZE
+                        The chunksize to use when reading the MS (default: 1000)
+  --data-column DATA_COLUMN
+                        The column to fix (default: DATA)
+  --corrected-data-column CORRECTED_DATA_COLUMN
+                        The column to write the corrected data to (default: CORRECTED_DATA)
+```
+
+```
 ❯ fix_ms_corrs -h
 usage: fix_ms_corrs [-h] [--chunksize CHUNKSIZE] [--data-column DATA_COLUMN] [--corrected-data-column CORRECTED_DATA_COLUMN] ms
 
 Fix the correlation rotation of ASKAP MSs. Converts the ASKAP standard correlations to the 'standard' correlations This will make them compatible with most imagers (e.g. wsclean, CASA) The new correlations are placed in a new column called 'CORRECTED_DATA'
 
 positional arguments:
   ms                    The MS to fix
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --chunksize CHUNKSIZE
                         The chunksize to use when reading the MS (default: 1000)
   --data-column DATA_COLUMN
                         The column to fix (default: DATA)
   --corrected-data-column CORRECTED_DATA_COLUMN
                         The column to write the corrected data to (default: CORRECTED_DATA)
 ```
+
 ```
 ❯ fix_ms_dir -h
 usage: fix_ms_dir [-h] [ms]
 
 ASKAP utility - update the pointing centre of a beam in an MS. - Allows imaging by CASA or wsclean.
 
 positional arguments:
```

