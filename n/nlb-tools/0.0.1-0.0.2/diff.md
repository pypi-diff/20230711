# Comparing `tmp/nlb_tools-0.0.1.tar.gz` & `tmp/nlb_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlb_tools-0.0.1.tar", max compression
+gzip compressed data, was "nlb_tools-0.0.2.tar", max compression
```

## Comparing `nlb_tools-0.0.1.tar` & `nlb_tools-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-03-22 23:47:20.940707 nlb_tools-0.0.1/LICENSE
--rw-r--r--   0        0        0     2820 2023-03-23 21:30:59.026384 nlb_tools-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-03-22 23:47:20.979706 nlb_tools-0.0.1/nlb_tools/__init__.py
--rw-r--r--   0        0        0    15656 2023-03-22 23:47:20.980706 nlb_tools-0.0.1/nlb_tools/chop.py
--rw-r--r--   0        0        0    17376 2023-03-22 23:47:20.982706 nlb_tools-0.0.1/nlb_tools/evaluation.py
--rw-r--r--   0        0        0    61047 2023-03-22 23:47:20.983706 nlb_tools-0.0.1/nlb_tools/make_tensors.py
--rw-r--r--   0        0        0    36815 2023-03-23 21:02:56.903626 nlb_tools-0.0.1/nlb_tools/nwb_interface.py
--rw-r--r--   0        0        0      876 2023-03-22 23:48:00.359227 nlb_tools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 nlb_tools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-03-22 23:47:20.940707 nlb_tools-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2820 2023-07-10 20:50:18.617518 nlb_tools-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-03-22 23:47:20.979706 nlb_tools-0.0.2/nlb_tools/__init__.py
+-rw-r--r--   0        0        0    15656 2023-03-22 23:47:20.980706 nlb_tools-0.0.2/nlb_tools/chop.py
+-rw-r--r--   0        0        0    17376 2023-03-22 23:47:20.982706 nlb_tools-0.0.2/nlb_tools/evaluation.py
+-rw-r--r--   0        0        0    61667 2023-07-11 00:05:58.169964 nlb_tools-0.0.2/nlb_tools/make_tensors.py
+-rw-r--r--   0        0        0    36815 2023-07-10 20:50:18.630518 nlb_tools-0.0.2/nlb_tools/nwb_interface.py
+-rw-r--r--   0        0        0      876 2023-07-11 00:05:58.171964 nlb_tools-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 nlb_tools-0.0.2/PKG-INFO
```

### Comparing `nlb_tools-0.0.1/LICENSE` & `nlb_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nlb_tools-0.0.1/README.md` & `nlb_tools-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 * `nlb_tools/` has code to load and preprocess our dataset files, format data for modeling, and locally evaluate results
 * `examples/tutorials/` contains tutorial notebooks demonstrating basic usage of `nlb_tools`
 * `examples/baselines/` holds the code we used to run our baseline methods. They may serve as helpful references on more extensive usage of `nlb_tools`
 
 ## Installation
 The package can be installed with the following command:
 ```
-pip install nlb_tools
+pip install nlb-tools
 ```
 However, to run the tutorial notebooks locally or make any modifications to the code, you should clone the repo. The package can then be installed with the following commands:
 ```
 git clone https://github.com/neurallatents/nlb_tools.git
 cd nlb_tools
 pip install -e .
 ```
```

### Comparing `nlb_tools-0.0.1/nlb_tools/chop.py` & `nlb_tools-0.0.2/nlb_tools/chop.py`

 * *Files identical despite different names*

### Comparing `nlb_tools-0.0.1/nlb_tools/evaluation.py` & `nlb_tools-0.0.2/nlb_tools/evaluation.py`

 * *Files identical despite different names*

### Comparing `nlb_tools-0.0.1/nlb_tools/make_tensors.py` & `nlb_tools-0.0.2/nlb_tools/make_tensors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1266,15 +1266,15 @@
     train_ids_list = np.array(train_ids_list, dtype='object')
     eval_ids_list = np.array(eval_ids_list, dtype='object')
 
     return (train_ids_list, eval_ids_list), psth, good_comb
 
 
 ''' Tensor saving functions '''
-def save_to_h5(data_dict, save_path, overwrite=False, dlen=32):
+def save_to_h5(data_dict, save_path, overwrite=False, dlen=32, compression="gzip"):
     """Function that saves dict as .h5 file while preserving
     nested dict structure
 
     Parameters
     ----------
     data_dict : dict
         Dict containing data to be saved in HDF5 format
@@ -1283,21 +1283,23 @@
     overwrite : bool, optional
         Whether to overwrite duplicate data found 
         at `save_path` if file already exists, by
         default False
     dlen : int, optional
         Byte length of data format to save numerical data,
         by default 32.
+    compression : str, optional
+        Compression to use when writing to HDF5, default "gzip"
     """
     h5file = h5py.File(save_path, 'a')
     good, dup_list = _check_h5_r(data_dict, h5file, overwrite)
     if good:
         if len(dup_list) > 0:
             logger.warning(f"{dup_list} already found in {save_path}. Overwriting...")
-        _save_h5_r(data_dict, h5file, dlen)
+        _save_h5_r(data_dict, h5file, dlen, compression)
         logger.info(f"Saved data to {save_path}")
     else:
         logger.warning(f"{dup_list} already found in {save_path}. Save to file canceled. " \
             "Please set `overwrite=True` or specify a different file path.")
     h5file.close()
 
 def _check_h5_r(data_dict, h5obj, overwrite):
@@ -1332,38 +1334,50 @@
                 dup_list.append(key)
                 if overwrite:
                     del h5obj[key]
                 else:
                     good = False
     return good, dup_list
 
-def _save_h5_r(data_dict, h5obj, dlen):
+def _save_h5_r(data_dict, h5obj, dlen, compression="gzip"):
     """Recursive function that adds all the items in a dict to an h5py.File or h5py.Group object
 
     Parameters
     ----------
     data_dict : dict
         Dict containing data to be saved in HDF5 format
     h5obj : h5py.File or h5py.Group
         h5py object to save data to
     dlen : int, optional
         Byte length of data format to save numerical data,
         by default 32.
+    compression : str, optional
+        Compression to use when writing to HDF5, default "gzip"
     """
     for key, val in data_dict.items():
         if isinstance(val, dict):
             h5group = h5obj[key] if key in h5obj.keys() else h5obj.create_group(key)
             _save_h5_r(val, h5group, dlen)
         else:
             if val.dtype == 'object':
-                sub_dtype = f'float{dlen}' if val[0].dtype == np.float else f'int{dlen}' if val[0].dtype == np.int else val[0].dtype
+                sub_dtype = val[0].dtype
+                if dlen is not None:
+                    if np.issubdtype(sub_dtype, np.floating):
+                        sub_dtype = f'float{dlen}'
+                    elif np.issubdtype(sub_dtype, np.integer):
+                        sub_dtype = f'int{dlen}'                    
                 dtype = h5py.vlen_dtype(sub_dtype)
             else:
-                dtype = f'float{dlen}' if val.dtype == np.float else f'int{dlen}' if val.dtype == np.int else val.dtype
-            h5obj.create_dataset(key, data=val, dtype=dtype)
+                dtype = val.dtype
+                if dlen is not None:
+                    if np.issubdtype(dtype, np.floating):
+                        dtype = f'float{dlen}'
+                    elif np.issubdtype(dtype, np.integer):
+                        dtype = f'int{dlen}'
+            h5obj.create_dataset(key, data=val, dtype=dtype, compression=compression)
             
 def h5_to_dict(h5obj):
     """Recursive function that reads HDF5 file to dict
 
     Parameters
     ----------
     h5obj : h5py.File or h5py.Group
```

### Comparing `nlb_tools-0.0.1/nlb_tools/nwb_interface.py` & `nlb_tools-0.0.2/nlb_tools/nwb_interface.py`

 * *Files identical despite different names*

### Comparing `nlb_tools-0.0.1/pyproject.toml` & `nlb_tools-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nlb_tools"
-version = "0.0.1"
+version = "0.0.2"
 license = "MIT"
 description = "Python tools for participating in Neural Latents Benchmark '21"
 authors = [
     "Felix Pei <felp8484@gmail.com>"
 ]
 packages = [
     {include = "nlb_tools"}
```

### Comparing `nlb_tools-0.0.1/PKG-INFO` & `nlb_tools-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlb-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python tools for participating in Neural Latents Benchmark '21
 Home-page: https://github.com/neurallatents/nlb_tools
 License: MIT
 Author: Felix Pei
 Author-email: felp8484@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Science/Research
@@ -39,15 +39,15 @@
 * `nlb_tools/` has code to load and preprocess our dataset files, format data for modeling, and locally evaluate results
 * `examples/tutorials/` contains tutorial notebooks demonstrating basic usage of `nlb_tools`
 * `examples/baselines/` holds the code we used to run our baseline methods. They may serve as helpful references on more extensive usage of `nlb_tools`
 
 ## Installation
 The package can be installed with the following command:
 ```
-pip install nlb_tools
+pip install nlb-tools
 ```
 However, to run the tutorial notebooks locally or make any modifications to the code, you should clone the repo. The package can then be installed with the following commands:
 ```
 git clone https://github.com/neurallatents/nlb_tools.git
 cd nlb_tools
 pip install -e .
 ```
```

