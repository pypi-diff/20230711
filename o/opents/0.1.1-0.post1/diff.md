# Comparing `tmp/opents-0.1.1-py3-none-any.whl.zip` & `tmp/opents-0.post1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 7318 bytes, number of entries: 12
+Zip file size: 8701 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx       54 b- defN 23-Jun-20 07:42 opents/__init__.py
 -rw-rw-r--  2.0 unx       14 b- defN 23-Jun-20 07:42 opents/data/__init__.py
+-rw-rw-r--  2.0 unx     9063 b- defN 23-Jun-28 02:05 opents/data/datasets.py
 -rw-rw-r--  2.0 unx     6306 b- defN 23-Jun-20 13:04 opents/data/generate_datasets.py
--rw-rw-r--  2.0 unx       77 b- defN 23-Jul-10 08:32 opents/datasets/__init__.py
--rw-rw-r--  2.0 unx     9463 b- defN 23-Jul-10 14:03 opents/datasets/datasets.py
+-rw-rw-r--  2.0 unx     3658 b- defN 23-Jun-20 11:58 opents/data/new_ucr.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-28 15:32 opents/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3133 b- defN 23-Jun-20 09:11 opents/datasets/ucr.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-28 15:32 opents/nn/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-28 15:32 opents/utils/__init__.py
--rw-rw-r--  2.0 unx     3533 b- defN 23-Jul-11 06:11 opents/utils/data_utils.py
--rw-rw-r--  2.0 unx     2023 b- defN 23-Jul-11 06:15 opents-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 06:15 opents-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jul-11 06:15 opents-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      935 b- defN 23-Jul-11 06:15 opents-0.1.1.dist-info/RECORD
-12 files, 22504 bytes uncompressed, 5740 bytes compressed:  74.5%
+-rw-rw-r--  2.0 unx     1927 b- defN 23-Jun-28 04:29 opents-0.post1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-28 04:29 opents-0.post1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-28 04:29 opents-0.post1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1013 b- defN 23-Jun-28 04:29 opents-0.post1.dist-info/RECORD
+13 files, 25267 bytes uncompressed, 7003 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -1,37 +1,40 @@
 Filename: opents/__init__.py
 Comment: 
 
 Filename: opents/data/__init__.py
 Comment: 
 
+Filename: opents/data/datasets.py
+Comment: 
+
 Filename: opents/data/generate_datasets.py
 Comment: 
 
+Filename: opents/data/new_ucr.py
+Comment: 
+
 Filename: opents/datasets/__init__.py
 Comment: 
 
-Filename: opents/datasets/datasets.py
+Filename: opents/datasets/ucr.py
 Comment: 
 
 Filename: opents/nn/__init__.py
 Comment: 
 
 Filename: opents/utils/__init__.py
 Comment: 
 
-Filename: opents/utils/data_utils.py
-Comment: 
-
-Filename: opents-0.1.1.dist-info/METADATA
+Filename: opents-0.post1.dist-info/METADATA
 Comment: 
 
-Filename: opents-0.1.1.dist-info/WHEEL
+Filename: opents-0.post1.dist-info/WHEEL
 Comment: 
 
-Filename: opents-0.1.1.dist-info/top_level.txt
+Filename: opents-0.post1.dist-info/top_level.txt
 Comment: 
 
-Filename: opents-0.1.1.dist-info/RECORD
+Filename: opents-0.post1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opents/datasets/__init__.py

```diff
@@ -1,5 +0,0 @@
-00000000: 6672 6f6d 202e 6461 7461 7365 7473 2069  from .datasets i
-00000010: 6d70 6f72 7420 5543 5244 6174 6173 6574  mport UCRDataset
-00000020: 2c20 5545 4144 6174 6173 6574 2c20 4f70  , UEADataset, Op
-00000030: 656e 5543 5244 6174 6173 6574 2c20 4f70  enUCRDataset, Op
-00000040: 656e 5545 4144 6174 6173 6574 0a         enUEADataset.
```

## Comparing `opents/datasets/datasets.py` & `opents/data/datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,118 +1,127 @@
 # coding=utf-8
 import os
 
 import pandas as pd
 import torch
 import numpy as np
-from scipy.io import arff
-from opents.utils.data_utils import data_file_type, get_dataset_root_path
-from sklearn.preprocessing import LabelEncoder
+import requests
+import zipfile 
 
-class Dataset:
+DEFAULT_DATASETS_ROOT = "data"
+
+def download_url(url, datasets_name, datasets_root_path):
+    response = requests.get(url)
+    if response.status_code == 200:
+        with open(datasets_root_path, 'wb') as file:
+            file.write(response.content)
+        print(datasets_name + "is successfully downloaded")
+    else:
+        print(datasets_name + "is not successfully downloaded") 
+
+
+
+def get_dataset_root_path(dataset_root_path=None, dataset_name=None, datasets_name=None,
+                          datasets_root_path=DEFAULT_DATASETS_ROOT):
+    if dataset_root_path is None:
+        dataset_root_path = os.path.join(datasets_root_path, dataset_name)
+    dataset_root_path = os.path.abspath(dataset_root_path)
+    
+    ucr_url = 'https://www.timeseriesclassification.com/ClassificationDownloads/Archives/Univariate2018_ts.zip'
+    ucr_password = "someone"
+
+    uea_url = "https://www.timeseriesclassification.com/ClassificationDownloads/Archives/Multivariate2018_ts.zip"
+
+    if os.path.exists(dataset_root_path) is False:
+        os.makedirs(dataset_root_path, exist_ok=True)
+        if datasets_name == "UCR":
+            download_url(ucr_url, "UCR", datasets_root_path)
+
+            with zipfile.ZipFile(datasets_root_path + "UCR_TS_Archive_2018.zip", 'r') as zf:
+                if zf.setpassword(bytes(ucr_password, 'utf-8')):
+                    zf.extractall()
+                    print("The ZIP file has been successfully extracted. UCR 2018 zip is successfully unzip.")
+
+        if datasets_name == "UEA":
+            download_url(uea_url, "UEA", datasets_root_path)
+
+            with zipfile.ZipFile(datasets_root_path + "Multivariate2018_ts.zip", 'r') as zf:
+                zf.extractall()
+                print("The ZIP file has been successfully extracted. UEA 2018 zip is successfully unzip.")
+    else:
+        print("unzip password is worng, please change the unzip password")
+    return dataset_root_path
+
+
+class Dataset(object):
     def __init__(
             self,
             dataset_name,
             dataset_root_path=None,
-            datasets_root_name=None,
+            datasets_name=None,
             split=False
             ):
-        """_summary_
-
-        Args:
-            dataset_name (_type_): _description_
-            dataset_root_path (_type_, optional): _description_. Defaults to None.
-            datasets_root_name (_type_, optional): _description_. Defaults to None.
-            split (bool, optional): _description_. Defaults to False.
-        """
         self.dataset_name = dataset_name
-        self.dataset_root_path = get_dataset_root_path(dataset_root_path, dataset_name, datasets_root_name)
-        self.datasets_root_name = datasets_root_name
+        self.dataset_root_path = get_dataset_root_path(dataset_root_path, dataset_name, datasets_name)
         self.split = split
 
     
     def ts_dataset(self):
-        """ The path to read the UCR or UEA file, including the path of the training file and the path of the testing file.
+        """ The path to read the UCR file, including the path of the training file and the path of the testing file.
         Args:
             dataset(string):Define a variable 'dataset_name' for the name of each file, which can be used to locate the training and testing file paths for each function.
         Returns:
-            for UCR:add an extra dimension to the train data and test data, then return the train data, new label of train data, test data, and new label of test data.
-            for UEA:return the train data, new label of train data, test data, and new label of test data.
+            Add an extra dimension to the train data and test data, then return the train data, new label of train data, test data, and new label of test data.
         """
-        train_file_df, test_file_df = data_file_type(self.dataset_name, self.dataset_root_path, self.datasets_root_name)
-        
-        if self.datasets_root_name.lower() == 'ucr':
-            # Create a two-dimensional tensor file from the data in the training set and testing set files.
-            train_tensor = torch.tensor(train_file_df.values)
-            test_tensor = torch.tensor(test_file_df.values)
-
-            # Here, we extract the distinct labels from each dataset.
-            train_labels = torch.unique(train_tensor[:, 0])
-            test_labels = torch.unique       
-            
-            # Convert the data into a list.
-            train_array = train_tensor.tolist()
-            train_array = np.array(train_array)
-            test_array = test_tensor.tolist()
-            test_array = np.array(test_array)
-
-            # Retrieve the time-series data, excluding the labels. 
-            x_train = train_array[:, 1:].astype(np.float64)
-            x_test = test_array[:, 1:].astype(np.float64)
-            # Store the labels in a dictionary, where the key is the original label and the value is the count of that label.
-            transform = {}
-
-            for i, l in enumerate(train_labels):
-                transform[l.item()] = i
-            # Retrieve the values of all new labels and store them in 'train_label'.
-            y_train = np.vectorize(transform.get)(train_array[:, 0])
-
-            # Retrieve all label values from the test set and store them in 'test_label'.
-            y_test = np.vectorize(transform.get)(test_array[:, 0])
-            # if dataset's dimention is 2, we change the dimention to 3
-            if x_train.shape == 2 and x_test.shape == 2:
-                x_train = x_train[..., np.newaxis]
-                x_test = x_test[..., np.newaxis]           
-
-        elif self.datasets_root_name.lower() == 'uea':
-            train_dataset_name = self.dataset_name + "_TRAIN"
-            test_dataset_name = self.dataset_name + "_TEST"
-
-            # Store the train data and test data in list, and extend its dimention to 3.
-            train_array = np.array(train_file_df[train_dataset_name].tolist())
-            x_train = train_array.view((np.float64, len(train_array.dtype.names)))
-
-            test_array = np.array(test_file_df[train_dataset_name].tolist())
-            x_test = test_array.view((np.float64, len(test_array.dtype.names)))
-
-            # Here, we extract the distinct labels from each dataset.
-            train_labels = torch.unique(torch.tensor(pd.to_numeric(train_file_df['target'], errors='coerce')))
-            test_labels = torch.unique(torch.tensor(pd.to_numeric(test_file_df['target'], errors='coerce')))
-            transform = {}
-
-            for i, l in enumerate(train_labels):
-                transform[l.item()] = i
-            
-            # Retrieve the values of all new labels and store them in 'train_label'.
-            y_train = np.vectorize(transform.get)(train_labels)
+        # Define the paths for the training and testing sets.
+        train_file_path = os.path.join(self.dataset_root_path, self.dataset_name, self.dataset_name + "_TRAIN.tsv")
+        test_file_path = os.path.join(self.dataset_root_path, self.dataset_name, self.dataset_name + "_TEST.tsv")
 
-            # Retrieve all label values from the test set and store them in 'test_label'.
-            y_test = np.vectorize(transform.get)(test_labels) 
+        # Read the data from each file in the training set and testing set using the pandas library, which is a library for data processing.
+        train_file_df = pd.read_csv(train_file_path, sep='\t', header=None)
+        test_file_df = pd.read_csv(test_file_path, sep='\t', header=None)
+
+        # Create a two-dimensional tensor file from the data in the training set and testing set files.
+        train_tensor = torch.tensor(train_file_df.values)
+        test_tensor = torch.tensor(test_file_df.values)
+
+        # Here, we extract the distinct labels from each dataset.
+        train_labels = torch.unique(train_tensor[:, 0])
+        test_labels = torch.unique(test_tensor[:, 0])
+        # Store the labels in a dictionary, where the key is the original label and the value is the count of that label.
+        transform = {}
+
+        for i, l in enumerate(train_labels):
+            transform[l.item()] = i
 
+        # Convert the data into a list.
+        train_array = train_tensor.tolist()
+        train_array = np.array(train_array)
+        test_array = test_tensor.tolist()
+        test_array = np.array(test_array)
+
+        # Retrieve the time-series data, excluding the labels. 
+        train = train_array[:, 1:].astype(np.float64)
+        test = test_array[:, 1:].astype(np.float64)
+
+        # Retrieve the values of all new labels and store them in 'train_label'.
+        train_label = np.vectorize(transform.get)(train_array[:, 0])
+
+        # Retrieve all label values from the test set and store them in 'test_label'.
+        test_label = np.vectorize(transform.get)(test_array[:, 0])
 
         # Add an extra dimension to the train data and test data, then return the train data, new label of train data, test data, and new label of test data.
-        return x_train, y_train, x_test, y_test
+        return train[..., np.newaxis], train_label, test[..., np.newaxis], test_label
 
     def opents_dataset(self):
-        """ The path to read the UCR or UEA file, including the path of the training file and the path of the testing file.
+        """ The path to read the UCR file, including the path of the training file and the path of the testing file.
         Args:
             dataset(string):Define a variable 'dataset_name' for the name of each file, which can be used to locate the training and testing file paths for each function.
         Returns:
-            for UCR:add an extra dimension to the train data and test data, then return the train data, new label of train data, test data, and new label of test data.
-            for UEA:return the train data, new label of train data, test data, and new label of test data.
+            Add an extra dimension to the train data and test data, then return the train data, new label of train data, test data, and new label of test data.
         """
         # Define the paths for the training and testing sets.
         train_file_path = os.path.join(self.dataset_root_path, self.dataset_name, self.dataset_name + "_TRAIN.tsv")
         test_file_path = os.path.join(self.dataset_root_path, self.dataset_name, self.dataset_name + "_TEST.tsv")
 
         # Read the data from each file in the training set and testing set using the pandas library, which is a library for data processing.
         train_file_df = pd.read_csv(train_file_path, sep='\t', header=None)
@@ -145,52 +154,46 @@
         all_label = np.vectorize(transform.get)(all_array[:, 0])
 
         # Add an extra dimension to the train data and test data, then return the train data, new label of train data, test data, and new label of test data.
         return all[..., np.newaxis], all_label
     
 
 class TSDataset(Dataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name=None, split=True):
-        super().__init__(dataset_name, dataset_root_path, datasets_name, split)
+    def __init__(self, dataset_name, dataset_root_path=None, split=True):
+        super().__init__(dataset_name, dataset_root_path, split)
 
     def load(self):
         # Call the parent class's ucr_dataset method to get the data
         train_data, train_labels, test_data, test_labels = self.ts_dataset()
 
         # Modify or add any additional processing specific to TSDataset here
 
         return train_data, train_labels, test_data, test_labels
     
     
 class UCRDataset(TSDataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UCR', split=True):
-        super().__init__(dataset_name, dataset_root_path, datasets_name, split)
-        self.datasets_name = datasets_name
+    def __init__(self, dataset_name, dataset_root_path=None, split=True):
+        super().__init__(dataset_name, dataset_root_path, split)
 
 class UEADataset(TSDataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UEA', split=True):
-        super().__init__(dataset_name, dataset_root_path, datasets_name, split)
-        self.datasets_name = datasets_name
-
-
+    def __init__(self, dataset_name, dataset_root_path=None, split=True):
+        super().__init__(dataset_name, dataset_root_path, split)
 
 class OpenDataset(Dataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name=None, split=False):
-        super().__init__(dataset_name, dataset_root_path, datasets_name, split)
+    def __init__(self, dataset_name, dataset_root_path=None, split=False):
+        super().__init__(dataset_name, dataset_root_path, split)
 
     def load(self):
         # Call the parent class's open_ucr_dataset method to get the data
         all_data, all_labels = self.opents_dataset()
 
         # Modify or add any additional processing specific to OpenDataset here
 
         return all_data, all_labels
     
 class OpenUCRDataset(OpenDataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UCR', split=False):
-        super().__init__(dataset_name, dataset_root_path, datasets_name, split)
-        self.datasets_name = datasets_name
+    def __init__(self, dataset_name, dataset_root_path=None, split=False):
+        super().__init__(dataset_name, dataset_root_path, split)
 
 class OpenUEADataset(OpenDataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UEA', split=False):
-        super().__init__(dataset_name, dataset_root_path, datasets_name, split)
-        self.datasets_name = datasets_name
+    def __init__(self, dataset_name, dataset_root_path=None, split=False):
+        super().__init__(dataset_name, dataset_root_path, split)
```

## Comparing `opents-0.1.1.dist-info/METADATA` & `opents-0.post1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,39 @@
 Metadata-Version: 2.1
 Name: opents
-Version: 0.1.1
+Version: 0-1
 Summary: OpenTS is a friendly Python Library for time series analysis
 Home-page: https://github.com/PyOpenTS/PyOpenTS
 Author: hushuguo
 Author-email: husg8217@mails.jlu.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: tqdm
 
 # PyOpenTS
-
 PyOpenTS is a library specifically designed to integrate methods and modules for time series. Its purpose is to allow users of this library to call and modify time series modules in a simpler and more convenient way. By using PyOpenTS, you can simplify the time series code process and reliably provide time series related module functions.  
 
 ## Our Goal
-
 Our goal is to simplify the process of handling time series code so that users can more easily tackle various time series problems. Whether you are a data scientist, an engineer, a researcher, or someone interested in time series, PyOpenTS will be a powerful tool for you.  
 
 ## Features
-
 * A clean API for quickly calling and modifying time series modules
 * Provides a range of methods and models for time series analysis, including but not limited to forecasting, clustering, classification, etc. 
-* Continuous updates and improvements to meet user needs
-
-## Installation
+* Continuous updates and improvements to meet user needs  
 
-Use the following commands below:
+## example 
 
-```cmd
-pip install -u opents
 ```
-
-## example
-
-```python
 from opents.data import datasets
 
 # load ucr and generate dataloader
 ucr_dataset = datasets.UCRDataset(dataset_name="Chinatown",dataset_root_path='UCR')
 train, train_label, test, test_label = ucr_dataset.load()
 ```
 
 ## Future Plans
-
 We will continue to update and improve PyOpenTS and gradually add some demo usage methods to show how to use this library. Please stay tuned for our updates.
 
 ## How to Get Help
-
 If you encounter any problems during use, feel free to submit them to Issues. We also welcome your suggestions for improving PyOpenTS. We hope that PyOpenTS can become a powerful assistant for you in dealing with time series problems.
```

