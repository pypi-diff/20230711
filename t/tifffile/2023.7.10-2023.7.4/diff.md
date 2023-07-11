# Comparing `tmp/tifffile-2023.7.10.tar.gz` & `tmp/tifffile-2023.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tifffile-2023.7.10.tar", last modified: Mon Jul 10 23:26:08 2023, max compression
+gzip compressed data, was "tifffile-2023.7.4.tar", last modified: Tue Jul  4 23:29:08 2023, max compression
```

## Comparing `tifffile-2023.7.10.tar` & `tifffile-2023.7.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 23:26:08.159172 tifffile-2023.7.10/
--rw-rw-rw-   0        0        0      324 2019-07-10 16:43:27.000000 tifffile-2023.7.10/ACKNOWLEDGEMENTS.rst
--rw-rw-rw-   0        0        0    36069 2023-07-10 23:26:02.000000 tifffile-2023.7.10/CHANGES.rst
--rw-rw-rw-   0        0        0     1559 2023-07-10 23:26:02.000000 tifffile-2023.7.10/LICENSE
--rw-rw-rw-   0        0        0      540 2023-01-23 07:24:27.000000 tifffile-2023.7.10/MANIFEST.in
--rw-rw-rw-   0        0        0    31710 2023-07-10 23:26:08.143567 tifffile-2023.7.10/PKG-INFO
--rw-rw-rw-   0        0        0    30744 2023-07-10 23:26:02.000000 tifffile-2023.7.10/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-10 23:26:08.112280 tifffile-2023.7.10/docs/
-drwxrwxrwx   0        0        0        0 2023-07-10 23:26:08.112280 tifffile-2023.7.10/docs/_static/
--rw-rw-rw-   0        0        0      127 2022-05-28 19:33:31.000000 tifffile-2023.7.10/docs/_static/custom.css
--rw-rw-rw-   0        0        0     1098 2023-01-12 21:14:58.000000 tifffile-2023.7.10/docs/conf.py
--rw-rw-rw-   0        0        0     3629 2023-03-04 01:54:58.000000 tifffile-2023.7.10/docs/make.py
-drwxrwxrwx   0        0        0        0 2023-07-10 23:26:08.127899 tifffile-2023.7.10/examples/
--rw-rw-rw-   0        0        0    15098 2023-07-04 23:25:39.000000 tifffile-2023.7.10/examples/earthbigdata.py
--rw-rw-rw-   0        0        0     2557 2023-06-27 16:33:23.000000 tifffile-2023.7.10/examples/issue125.py
--rw-rw-rw-   0        0        0       42 2023-07-10 23:26:08.159172 tifffile-2023.7.10/setup.cfg
--rw-rw-rw-   0        0        0     3870 2023-07-10 22:54:55.000000 tifffile-2023.7.10/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 23:26:08.127899 tifffile-2023.7.10/tests/
--rw-rw-rw-   0        0        0     1601 2023-03-14 03:16:25.000000 tifffile-2023.7.10/tests/conftest.py
--rw-rw-rw-   0        0        0   705922 2023-07-10 23:24:28.000000 tifffile-2023.7.10/tests/test_tifffile.py
-drwxrwxrwx   0        0        0        0 2023-07-10 23:26:08.143567 tifffile-2023.7.10/tifffile/
--rw-rw-rw-   0        0        0      110 2020-01-01 02:31:34.000000 tifffile-2023.7.10/tifffile/__init__.py
--rw-rw-rw-   0        0        0      135 2020-01-01 02:31:36.000000 tifffile-2023.7.10/tifffile/__main__.py
--rw-rw-rw-   0        0        0    11855 2023-07-03 00:18:30.000000 tifffile-2023.7.10/tifffile/_imagecodecs.py
--rw-rw-rw-   0        0        0    61794 2023-07-03 00:17:39.000000 tifffile-2023.7.10/tifffile/geodb.py
--rw-rw-rw-   0        0        0      680 2023-07-03 00:17:47.000000 tifffile-2023.7.10/tifffile/lsm2bin.py
--rw-rw-rw-   0        0        0     5906 2023-07-03 00:17:55.000000 tifffile-2023.7.10/tifffile/numcodecs.py
--rw-rw-rw-   0        0        0     2410 2023-07-03 00:18:03.000000 tifffile-2023.7.10/tifffile/tiff2fsspec.py
--rw-rw-rw-   0        0        0     1437 2023-07-03 00:18:11.000000 tifffile-2023.7.10/tifffile/tiffcomment.py
--rw-rw-rw-   0        0        0   864515 2023-07-10 22:56:11.000000 tifffile-2023.7.10/tifffile/tifffile.py
-drwxrwxrwx   0        0        0        0 2023-07-10 23:26:08.143567 tifffile-2023.7.10/tifffile.egg-info/
--rw-rw-rw-   0        0        0    31710 2023-07-10 23:26:06.000000 tifffile-2023.7.10/tifffile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2023-07-10 23:26:07.000000 tifffile-2023.7.10/tifffile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 23:26:06.000000 tifffile-2023.7.10/tifffile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-07-10 23:26:06.000000 tifffile-2023.7.10/tifffile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2023-07-10 23:26:06.000000 tifffile-2023.7.10/tifffile.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-10 23:26:06.000000 tifffile-2023.7.10/tifffile.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 23:29:08.172341 tifffile-2023.7.4/
+-rw-rw-rw-   0        0        0      324 2019-07-10 16:43:27.000000 tifffile-2023.7.4/ACKNOWLEDGEMENTS.rst
+-rw-rw-rw-   0        0        0    35933 2023-07-04 23:29:02.000000 tifffile-2023.7.4/CHANGES.rst
+-rw-rw-rw-   0        0        0     1559 2023-07-04 23:29:02.000000 tifffile-2023.7.4/LICENSE
+-rw-rw-rw-   0        0        0      540 2023-01-23 07:24:27.000000 tifffile-2023.7.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    31571 2023-07-04 23:29:08.172341 tifffile-2023.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0    30606 2023-07-04 23:29:02.000000 tifffile-2023.7.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-04 23:29:08.141076 tifffile-2023.7.4/docs/
+drwxrwxrwx   0        0        0        0 2023-07-04 23:29:08.141076 tifffile-2023.7.4/docs/_static/
+-rw-rw-rw-   0        0        0      127 2022-05-28 19:33:31.000000 tifffile-2023.7.4/docs/_static/custom.css
+-rw-rw-rw-   0        0        0     1098 2023-01-12 21:14:58.000000 tifffile-2023.7.4/docs/conf.py
+-rw-rw-rw-   0        0        0     3629 2023-03-04 01:54:58.000000 tifffile-2023.7.4/docs/make.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:29:08.141076 tifffile-2023.7.4/examples/
+-rw-rw-rw-   0        0        0    15098 2023-07-04 23:25:39.000000 tifffile-2023.7.4/examples/earthbigdata.py
+-rw-rw-rw-   0        0        0     2557 2023-06-27 16:33:23.000000 tifffile-2023.7.4/examples/issue125.py
+-rw-rw-rw-   0        0        0       42 2023-07-04 23:29:08.172341 tifffile-2023.7.4/setup.cfg
+-rw-rw-rw-   0        0        0     3869 2023-07-03 00:03:17.000000 tifffile-2023.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:29:08.141076 tifffile-2023.7.4/tests/
+-rw-rw-rw-   0        0        0     1601 2023-03-14 03:16:25.000000 tifffile-2023.7.4/tests/conftest.py
+-rw-rw-rw-   0        0        0   705766 2023-07-04 21:19:00.000000 tifffile-2023.7.4/tests/test_tifffile.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:29:08.156716 tifffile-2023.7.4/tifffile/
+-rw-rw-rw-   0        0        0      110 2020-01-01 02:31:34.000000 tifffile-2023.7.4/tifffile/__init__.py
+-rw-rw-rw-   0        0        0      135 2020-01-01 02:31:36.000000 tifffile-2023.7.4/tifffile/__main__.py
+-rw-rw-rw-   0        0        0    11855 2023-07-03 00:18:30.000000 tifffile-2023.7.4/tifffile/_imagecodecs.py
+-rw-rw-rw-   0        0        0    61794 2023-07-03 00:17:39.000000 tifffile-2023.7.4/tifffile/geodb.py
+-rw-rw-rw-   0        0        0      680 2023-07-03 00:17:47.000000 tifffile-2023.7.4/tifffile/lsm2bin.py
+-rw-rw-rw-   0        0        0     5906 2023-07-03 00:17:55.000000 tifffile-2023.7.4/tifffile/numcodecs.py
+-rw-rw-rw-   0        0        0     2410 2023-07-03 00:18:03.000000 tifffile-2023.7.4/tifffile/tiff2fsspec.py
+-rw-rw-rw-   0        0        0     1437 2023-07-03 00:18:11.000000 tifffile-2023.7.4/tifffile/tiffcomment.py
+-rw-rw-rw-   0        0        0   864300 2023-07-04 02:52:04.000000 tifffile-2023.7.4/tifffile/tifffile.py
+drwxrwxrwx   0        0        0        0 2023-07-04 23:29:08.172341 tifffile-2023.7.4/tifffile.egg-info/
+-rw-rw-rw-   0        0        0    31571 2023-07-04 23:29:06.000000 tifffile-2023.7.4/tifffile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      599 2023-07-04 23:29:07.000000 tifffile-2023.7.4/tifffile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 23:29:06.000000 tifffile-2023.7.4/tifffile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-07-04 23:29:06.000000 tifffile-2023.7.4/tifffile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2023-07-04 23:29:06.000000 tifffile-2023.7.4/tifffile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 23:29:06.000000 tifffile-2023.7.4/tifffile.egg-info/top_level.txt
```

### Comparing `tifffile-2023.7.10/CHANGES.rst` & `tifffile-2023.7.4/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 Revisions
 ---------
 
-2023.7.10
-
-- Increase default strip size to 256 KB when writing with compression.
-- Fix ZarrTiffStore with non-default chunkmode.
-
 2023.7.4
 
 - Pass 4992 tests.
 - Add option to return selection from imread (#200).
 - Fix reading OME series with missing trailing frames (#199).
 - Fix fsspec reference for WebP compressed segments missing alpha channel.
 - Fix linting issues.
```

### Comparing `tifffile-2023.7.10/LICENSE` & `tifffile-2023.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tifffile-2023.7.10/MANIFEST.in` & `tifffile-2023.7.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tifffile-2023.7.10/PKG-INFO` & `tifffile-2023.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifffile
-Version: 2023.7.10
+Version: 2023.7.4
 Summary: Read and write TIFF files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/tifffile/issues
 Project-URL: Source Code, https://github.com/cgohlke/tifffile
@@ -52,15 +52,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.7.10
+:Version: 2023.7.4
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -90,33 +90,28 @@
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
 - `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b3, 64-bit
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.25.0
-- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.7.10
+- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.7.4
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.2
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
-- `Lxml <https://pypi.org/project/lxml/>`_ 4.9.3
+- `Lxml <https://pypi.org/project/lxml/>`_ 4.9.2
   (required only for validating and printing XML)
 - `Zarr <https://pypi.org/project/zarr/>`_ 2.15.0
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.6.0
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
-2023.7.10
-
-- Increase default strip size to 256 KB when writing with compression.
-- Fix ZarrTiffStore with non-default chunkmode.
-
 2023.7.4
 
 - Pass 4992 tests.
 - Add option to return selection from imread (#200).
 - Fix reading OME series with missing trailing frames (#199).
 - Fix fsspec reference for WebP compressed segments missing alpha channel.
 - Fix linting issues.
```

### Comparing `tifffile-2023.7.10/README.rst` & `tifffile-2023.7.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.7.10
+:Version: 2023.7.4
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -64,33 +64,28 @@
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
 - `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b3, 64-bit
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.25.0
-- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.7.10
+- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.7.4
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.2
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
-- `Lxml <https://pypi.org/project/lxml/>`_ 4.9.3
+- `Lxml <https://pypi.org/project/lxml/>`_ 4.9.2
   (required only for validating and printing XML)
 - `Zarr <https://pypi.org/project/zarr/>`_ 2.15.0
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.6.0
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
-2023.7.10
-
-- Increase default strip size to 256 KB when writing with compression.
-- Fix ZarrTiffStore with non-default chunkmode.
-
 2023.7.4
 
 - Pass 4992 tests.
 - Add option to return selection from imread (#200).
 - Fix reading OME series with missing trailing frames (#199).
 - Fix fsspec reference for WebP compressed segments missing alpha channel.
 - Fix linting issues.
```

### Comparing `tifffile-2023.7.10/docs/conf.py` & `tifffile-2023.7.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.7.10/docs/make.py` & `tifffile-2023.7.4/docs/make.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.7.10/examples/earthbigdata.py` & `tifffile-2023.7.4/examples/earthbigdata.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.7.10/examples/issue125.py` & `tifffile-2023.7.4/examples/issue125.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.7.10/setup.py` & `tifffile-2023.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         raise ValueError(f'{pattern!r} not found')
     return match.groups()[0]
 
 
 with open('tifffile/tifffile.py', encoding='utf-8') as fh:
     code = fh.read().replace('\r\n', '\n').replace('\r', '\n')
 
-version = search(r"__version__ = '(.*?)'", code).replace('.x.x', '.dev0')
+version = search(r"__version__ = '(.*?)'", code).replace('.x.x', '.dev')
 version += ('.' + buildnumber) if buildnumber else ''
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
 
 readme = search(
     r'(?:\r\n|\r|\n){2}r"""(.*)"""(?:\r\n|\r|\n){2}from __future__',
     code,
```

### Comparing `tifffile-2023.7.10/tests/conftest.py` & `tifffile-2023.7.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.7.10/tests/test_tifffile.py` & `tifffile-2023.7.4/tests/test_tifffile.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # mypy: check-untyped-defs=False
 
 """Unittests for the tifffile package.
 
 Public data files can be requested from the author.
 Private data files are not available due to size and copyright restrictions.
 
-:Version: 2023.7.10
+:Version: 2023.7.4
 
 """
 
 import binascii
 import datetime
 import glob
 import json
@@ -14127,26 +14127,22 @@
 def test_write_compression_args(args):
     """Test compression parameter."""
     i = args[0]
     compressionargs = args[1:]
     compressed = compressionargs[0] not in {0, 1, NONE}
     if len(compressionargs) == 1:
         compressionargs = compressionargs[0]
-    rowsperstrip = 100 if compressed else None
 
     data = WRITE_DATA
     with TempFileName(f'compression_args_{i}') as fname:
-        # TODO: if i > 4: with pytest.warns(DeprecationWarning):
-        imwrite(
-            fname,
-            data,
-            compression=compressionargs,
-            photometric=RGB,
-            rowsperstrip=rowsperstrip,
-        )
+        if i > 4:
+            # TODO: with pytest.warns(DeprecationWarning):
+            imwrite(fname, data, compression=compressionargs, photometric=RGB)
+        else:
+            imwrite(fname, data, compression=compressionargs, photometric=RGB)
         assert_valid_tiff(fname)
         with TiffFile(fname) as tif:
             assert len(tif.pages) == 1
             page = tif.pages.first
             assert page.compression == (ADOBE_DEFLATE if compressed else NONE)
             assert page.planarconfig == SEPARATE
             assert page.photometric == RGB
@@ -14251,15 +14247,14 @@
     with TempFileName('compression_deflate') as fname:
         imwrite(
             fname,
             data,
             compression=DEFLATE,
             compressionargs={'level': 6},
             photometric=RGB,
-            rowsperstrip=108,
         )
         assert_valid_tiff(fname)
         with TiffFile(fname) as tif:
             assert len(tif.pages) == 1
             page = tif.pages.first
             assert not page.is_contiguous
             assert page.compression == DEFLATE
@@ -14304,17 +14299,15 @@
             assert__str__(tif)
 
 
 def test_write_compression_lzma():
     """Test write LZMA compression."""
     data = WRITE_DATA
     with TempFileName('compression_lzma') as fname:
-        imwrite(
-            fname, data, compression=LZMA, photometric=RGB, rowsperstrip=108
-        )
+        imwrite(fname, data, compression=LZMA, photometric=RGB)
         assert_valid_tiff(fname)
         with TiffFile(fname) as tif:
             assert len(tif.pages) == 1
             page = tif.pages.first
             assert not page.is_contiguous
             assert page.compression == LZMA
             assert page.planarconfig == SEPARATE
@@ -14331,17 +14324,15 @@
 
 
 @pytest.mark.skipif(SKIP_CODECS or not imagecodecs.ZSTD, reason=REASON)
 def test_write_compression_zstd():
     """Test write ZSTD compression."""
     data = WRITE_DATA
     with TempFileName('compression_zstd') as fname:
-        imwrite(
-            fname, data, compression=ZSTD, photometric=RGB, rowsperstrip=108
-        )
+        imwrite(fname, data, compression=ZSTD, photometric=RGB)
         assert_valid_tiff(fname)
         with TiffFile(fname) as tif:
             assert len(tif.pages) == 1
             page = tif.pages.first
             assert not page.is_contiguous
             assert page.compression == ZSTD
             assert page.planarconfig == SEPARATE
```

### Comparing `tifffile-2023.7.10/tifffile/_imagecodecs.py` & `tifffile-2023.7.4/tifffile/_imagecodecs.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.7.10/tifffile/geodb.py` & `tifffile-2023.7.4/tifffile/geodb.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.7.10/tifffile/lsm2bin.py` & `tifffile-2023.7.4/tifffile/lsm2bin.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.7.10/tifffile/numcodecs.py` & `tifffile-2023.7.4/tifffile/numcodecs.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.7.10/tifffile/tiff2fsspec.py` & `tifffile-2023.7.4/tifffile/tiff2fsspec.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.7.10/tifffile/tiffcomment.py` & `tifffile-2023.7.4/tifffile/tiffcomment.py`

 * *Files identical despite different names*

### Comparing `tifffile-2023.7.10/tifffile/tifffile.py` & `tifffile-2023.7.4/tifffile/tifffile.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.7.10
+:Version: 2023.7.4
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -94,33 +94,28 @@
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
 - `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b3, 64-bit
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.25.0
-- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.7.10
+- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.7.4
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.2
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
-- `Lxml <https://pypi.org/project/lxml/>`_ 4.9.3
+- `Lxml <https://pypi.org/project/lxml/>`_ 4.9.2
   (required only for validating and printing XML)
 - `Zarr <https://pypi.org/project/zarr/>`_ 2.15.0
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.6.0
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
-2023.7.10
-
-- Increase default strip size to 256 KB when writing with compression.
-- Fix ZarrTiffStore with non-default chunkmode.
-
 2023.7.4
 
 - Pass 4992 tests.
 - Add option to return selection from imread (#200).
 - Fix reading OME series with missing trailing frames (#199).
 - Fix fsspec reference for WebP compressed segments missing alpha channel.
 - Fix linting issues.
@@ -822,15 +817,15 @@
 
     $ python -m tifffile temp.ome.tif
 
 """
 
 from __future__ import annotations
 
-__version__ = '2023.7.10'
+__version__ = '2023.7.4'
 
 __all__ = [
     'TiffFile',
     'TiffFileError',
     'TiffFrame',
     'TiffPage',
     'TiffPages',
@@ -1740,15 +1735,15 @@
                 tags are used to write volumetric data.
                 Tiles cannot be used to write contiguous series, except if
                 the tile shape matches the data shape.
                 The values are written to the TileWidth, TileLength, and
                 TileDepth tags.
             rowsperstrip:
                 Number of rows per strip.
-                By default, strips are about 256 KB if `compression` is
+                By default, strips are about 64 KB if `compression` is
                 enabled, else rowsperstrip is set to the image length.
                 The value is written to the RowsPerStrip tag.
             bitspersample:
                 Number of bits per sample.
                 The default is the number of bits of the data's dtype.
                 Different values per samples are not supported.
                 Unsigned integer data are packed into bytes as tightly as
@@ -2982,18 +2977,18 @@
                 * storedshape.contig_samples
                 * datadtype.itemsize
             )
             if compressiontag == 48124:
                 # Jetraw works on whole camera frame
                 rowsperstrip = storedshape.length
             if rowsperstrip is None:
-                # compress ~256 KB chunks by default
+                # compress ~64 KB chunks by default
                 # TIFF-EP requires <= 64 KB
                 if compression:
-                    rowsperstrip = 262144 // rowsize
+                    rowsperstrip = 65536 // rowsize
                 else:
                     rowsperstrip = storedshape.length
             if rowsperstrip < 1:
                 rowsperstrip = maxsampling
             elif rowsperstrip > storedshape.length:
                 rowsperstrip = storedshape.length
             elif subsampling and rowsperstrip % maxsampling:
@@ -12826,16 +12821,14 @@
 
     def _contains(self, key: str, /) -> bool:
         """Return if key is in store."""
         try:
             _, page, _, offset, bytecount = self._parse_key(key)
         except KeyError:
             return False
-        if self._chunkmode and offset is None:
-            return True
         return (
             page is not None
             and offset is not None
             and bytecount is not None
             and offset > 0
             and bytecount > 0
         )
```

### Comparing `tifffile-2023.7.10/tifffile.egg-info/PKG-INFO` & `tifffile-2023.7.4/tifffile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifffile
-Version: 2023.7.10
+Version: 2023.7.4
 Summary: Read and write TIFF files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/tifffile/issues
 Project-URL: Source Code, https://github.com/cgohlke/tifffile
@@ -52,15 +52,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.7.10
+:Version: 2023.7.4
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -90,33 +90,28 @@
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
 - `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b3, 64-bit
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.25.0
-- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.7.10
+- `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2023.7.4
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.2
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
   (required for plotting)
-- `Lxml <https://pypi.org/project/lxml/>`_ 4.9.3
+- `Lxml <https://pypi.org/project/lxml/>`_ 4.9.2
   (required only for validating and printing XML)
 - `Zarr <https://pypi.org/project/zarr/>`_ 2.15.0
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2023.6.0
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
-2023.7.10
-
-- Increase default strip size to 256 KB when writing with compression.
-- Fix ZarrTiffStore with non-default chunkmode.
-
 2023.7.4
 
 - Pass 4992 tests.
 - Add option to return selection from imread (#200).
 - Fix reading OME series with missing trailing frames (#199).
 - Fix fsspec reference for WebP compressed segments missing alpha channel.
 - Fix linting issues.
```

### Comparing `tifffile-2023.7.10/tifffile.egg-info/SOURCES.txt` & `tifffile-2023.7.4/tifffile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

