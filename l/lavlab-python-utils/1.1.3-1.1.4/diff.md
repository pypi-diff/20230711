# Comparing `tmp/lavlab-python-utils-1.1.3.tar.gz` & `tmp/lavlab-python-utils-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavlab-python-utils-1.1.3.tar", last modified: Tue Jul 11 14:49:03 2023, max compression
+gzip compressed data, was "lavlab-python-utils-1.1.4.tar", last modified: Tue Jul 11 16:09:15 2023, max compression
```

## Comparing `lavlab-python-utils-1.1.3.tar` & `lavlab-python-utils-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:03.221859 lavlab-python-utils-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-11 14:49:03.217859 lavlab-python-utils-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:49:03.221859 lavlab-python-utils-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:03.217859 lavlab-python-utils-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:03.217859 lavlab-python-utils-1.1.3/src/lavlab/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/src/lavlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/src/lavlab/omero_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    27587 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/src/lavlab/omero_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/src/lavlab/python_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:03.217859 lavlab-python-utils-1.1.3/src/lavlab_python_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-11 14:49:03.000000 lavlab-python-utils-1.1.3/src/lavlab_python_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-11 14:49:03.000000 lavlab-python-utils-1.1.3/src/lavlab_python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:49:03.000000 lavlab-python-utils-1.1.3/src/lavlab_python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 14:49:03.000000 lavlab-python-utils-1.1.3/src/lavlab_python_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 14:49:03.000000 lavlab-python-utils-1.1.3/src/lavlab_python_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:03.217859 lavlab-python-utils-1.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/test/test_omero_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-11 14:48:50.000000 lavlab-python-utils-1.1.3/test/test_python_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:09:15.492064 lavlab-python-utils-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-11 16:09:15.492064 lavlab-python-utils-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:09:15.492064 lavlab-python-utils-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:09:15.492064 lavlab-python-utils-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:09:15.492064 lavlab-python-utils-1.1.4/src/lavlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/src/lavlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/src/lavlab/omero_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/src/lavlab/omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/src/lavlab/python_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:09:15.492064 lavlab-python-utils-1.1.4/src/lavlab_python_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-11 16:09:15.000000 lavlab-python-utils-1.1.4/src/lavlab_python_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-11 16:09:15.000000 lavlab-python-utils-1.1.4/src/lavlab_python_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:09:15.000000 lavlab-python-utils-1.1.4/src/lavlab_python_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 16:09:15.000000 lavlab-python-utils-1.1.4/src/lavlab_python_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 16:09:15.000000 lavlab-python-utils-1.1.4/src/lavlab_python_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:09:15.492064 lavlab-python-utils-1.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/test/test_omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/test/test_python_utils.py
```

### Comparing `lavlab-python-utils-1.1.3/PKG-INFO` & `lavlab-python-utils-1.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.1.3
+Version: 1.1.4
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lavlab-python-utils-1.1.3/pyproject.toml` & `lavlab-python-utils-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "lavlab-python-utils"
 description = "LaViolette Lab utility package"
-version = "1.1.3"
+version = "1.1.4"
 
 authors = [
   { name="Michael Barrett", email="mjbarrett@mcw.edu" },
 ]
 
 readme = "README.rst"
 classifiers = [
```

### Comparing `lavlab-python-utils-1.1.3/src/lavlab/omero_asyncio.py` & `lavlab-python-utils-1.1.4/src/lavlab/omero_asyncio.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.1.3/src/lavlab/omero_util.py` & `lavlab-python-utils-1.1.4/src/lavlab/omero_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         # create and init rps for this group
         rps = await session.createRawPixelsStore()
         await rps.setPixelsId(id,rps_bypass)
 
         # set res and get default res level if necessary
         if resLvl is None:
             resLvl = await rps.getResolutionLevels()
-        await rps.setResolutionLevel(resLvl)
+        await rps.setResolutionLevel(resLvl-1)
 
         # request and return tiles
         i=1
         tile_len=len(tiles)
         for z,c,t,tile in tiles:
             rv = np.frombuffer(await rps.getTile(z,c,t,*tile), dtype=np.uint8)
             rv.shape=tile[3],tile[2]
@@ -148,15 +148,15 @@
 
 
     # force async client
     session =  omero_asyncio.AsyncSession(img._conn.c.sf)
 
     # create parallel raw pixels stores
     jobs=[]
-    for chunk in chunkify(tiles, PARALLEL_STORE_COUNT):
+    for chunk in chunkify(tiles, int(len(tiles)/PARALLEL_STORE_COUNT)):
         jobs.append(work(img.getPrimaryPixels().getId(), chunk, resLvl))
     return merge_async_iters(*jobs)
 
 def getDownsampledXYDimensions(img: ImageWrapper, downsample_factor: int) -> tuple[int,int]:
     """
 Returns XY (rows,columns) dimensions of given image at the downsample.
```

### Comparing `lavlab-python-utils-1.1.3/src/lavlab/python_util.py` & `lavlab-python-utils-1.1.4/src/lavlab/python_util.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.1.3/src/lavlab_python_utils.egg-info/PKG-INFO` & `lavlab-python-utils-1.1.4/src/lavlab_python_utils.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.1.3
+Version: 1.1.4
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lavlab-python-utils-1.1.3/test/test_omero_util.py` & `lavlab-python-utils-1.1.4/test/test_omero_util.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.1.3/test/test_python_utils.py` & `lavlab-python-utils-1.1.4/test/test_python_utils.py`

 * *Files identical despite different names*

