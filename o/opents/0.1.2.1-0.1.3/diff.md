# Comparing `tmp/opents-0.1.2.1-py3-none-any.whl.zip` & `tmp/opents-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 7338 bytes, number of entries: 12
+Zip file size: 7216 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx       54 b- defN 23-Jun-20 07:42 opents/__init__.py
 -rw-rw-r--  2.0 unx       14 b- defN 23-Jun-20 07:42 opents/data/__init__.py
 -rw-rw-r--  2.0 unx     6306 b- defN 23-Jun-20 13:04 opents/data/generate_datasets.py
 -rw-rw-r--  2.0 unx       77 b- defN 23-Jul-10 08:32 opents/datasets/__init__.py
--rw-rw-r--  2.0 unx     9499 b- defN 23-Jul-11 07:17 opents/datasets/datasets.py
+-rw-rw-r--  2.0 unx    10072 b- defN 23-Jul-11 08:51 opents/datasets/datasets.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-28 15:32 opents/nn/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-28 15:32 opents/utils/__init__.py
 -rw-rw-r--  2.0 unx     3533 b- defN 23-Jul-11 06:11 opents/utils/data_utils.py
--rw-rw-r--  2.0 unx     2025 b- defN 23-Jul-11 07:20 opents-0.1.2.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 07:20 opents-0.1.2.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jul-11 07:20 opents-0.1.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      943 b- defN 23-Jul-11 07:20 opents-0.1.2.1.dist-info/RECORD
-12 files, 22550 bytes uncompressed, 5744 bytes compressed:  74.5%
+-rw-rw-r--  2.0 unx     2023 b- defN 23-Jul-11 08:57 opents-0.1.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 08:57 opents-0.1.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jul-11 08:57 opents-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      936 b- defN 23-Jul-11 08:57 opents-0.1.3.dist-info/RECORD
+12 files, 23114 bytes uncompressed, 5638 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: opents/utils/__init__.py
 Comment: 
 
 Filename: opents/utils/data_utils.py
 Comment: 
 
-Filename: opents-0.1.2.1.dist-info/METADATA
+Filename: opents-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: opents-0.1.2.1.dist-info/WHEEL
+Filename: opents-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: opents-0.1.2.1.dist-info/top_level.txt
+Filename: opents-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: opents-0.1.2.1.dist-info/RECORD
+Filename: opents-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opents/datasets/datasets.py

```diff
@@ -1,16 +1,13 @@
 # coding=utf-8
-import os
 
 import pandas as pd
 import torch
 import numpy as np
-from scipy.io import arff
 from opents.utils.data_utils import data_file_type, get_dataset_root_path
-from sklearn.preprocessing import LabelEncoder
 
 class Dataset:
     def __init__(
             self,
             dataset_name,
             dataset_root_path=None,
             datasets_root_name=None,
@@ -108,63 +105,83 @@
         """ The path to read the UCR or UEA file, including the path of the training file and the path of the testing file.
         Args:
             dataset(string):Define a variable 'dataset_name' for the name of each file, which can be used to locate the training and testing file paths for each function.
         Returns:
             for UCR:add an extra dimension to the train data and test data, then return the train data, new label of train data, test data, and new label of test data.
             for UEA:return the train data, new label of train data, test data, and new label of test data.
         """
-        # Define the paths for the training and testing sets.
-        train_file_path = os.path.join(self.dataset_root_path, self.dataset_name, self.dataset_name + "_TRAIN.tsv")
-        test_file_path = os.path.join(self.dataset_root_path, self.dataset_name, self.dataset_name + "_TEST.tsv")
-
-        # Read the data from each file in the training set and testing set using the pandas library, which is a library for data processing.
-        train_file_df = pd.read_csv(train_file_path, sep='\t', header=None)
-        test_file_df = pd.read_csv(test_file_path, sep='\t', header=None)
-        
-        # merge the train and test file into a full data
-        all_data_df = pd.concat([train_file_df, test_file_df], axis=0)
-        
-        # Create a two-dimensional tensor file from the data in the all files.
-        all_tensor = torch.tensor(all_data_df.values)
-        # train_array = np.array(train_file_df)
+        train_file_df, test_file_df = data_file_type(self.dataset_name, self.dataset_root_path, self.datasets_root_name) 
 
-        # Here, we extract the distinct labels from each dataset.
-        all_labels = torch.unique(all_tensor[:, 0])
+        if self.datasets_root_name.lower() == 'ucr': 
+            # merge the train and test file into a full data
+            all_data_df = pd.concat([train_file_df, test_file_df], axis=0)
         
-        # Store the labels in a dictionary, where the key is the original label and the value is the count of that label.
-        transform = {}
+            # Create a two-dimensional tensor file from the data in the all files.
+            all_tensor = torch.tensor(all_data_df.values)
+            # train_array = np.array(train_file_df)
+
+            # Here, we extract the distinct labels from each dataset.
+            all_labels = torch.unique(all_tensor[:, 0])
+            
+            # Store the labels in a dictionary, where the key is the original label and the value is the count of that label.
+            transform = {}
 
-        for i, l in enumerate(all_labels):
-            transform[l.item()] = i
+            for i, l in enumerate(all_labels):
+                transform[l.item()] = i
 
-        # Convert the data into a list.
-        all_array = all_tensor.tolist()
-        all_array = np.array(all_array)
+            # Convert the data into a list.
+            all_array = all_tensor.tolist()
+            all_array = np.array(all_array)
 
-        # Retrieve the time-series data, excluding the labels. 
-        all = all_array[:, 1:].astype(np.float64)
+            # Retrieve the time-series data, excluding the labels. 
+            all = all_array[:, 1:].astype(np.float64)
 
-        # Retrieve the values of all new labels and store them in 'train_label'.
-        all_label = np.vectorize(transform.get)(all_array[:, 0])
+            # Retrieve the values of all new labels and store them in 'train_label'.
+            y_all = np.vectorize(transform.get)(all_array[:, 0])
+            
+            # Add an extra dimension to the train data and test data, then return the train data, new label of train data, test data, and new label of test data.
+            x_all = all[..., np.newaxis]
 
-        # Add an extra dimension to the train data and test data, then return the train data, new label of train data, test data, and new label of test data.
-        return all[..., np.newaxis], all_label
+        elif self.datasets_root_name.lower() == 'uea':
+            
+            all_data_df = pd.concat([train_file_df, test_file_df], axis=0)
+
+            all_data_df = all_data_df.reset_index(drop=True)
+            all_dataset_name = self.dataset_name + "_TRAIN"
+
+            # Store the train data and test data in list, and extend its dimention to 3.
+            all_array = np.array(all_data_df[all_dataset_name].tolist())
+            x_all = all_array.view((np.float64, len(all_array.dtype.names)))
+            
+            # Here, we extract the distinct labels from each dataset.
+            all_labels = torch.tensor(pd.to_numeric(all_data_df['target'], errors='coerce'))
+            y_all = torch.unique(all_labels)
+            
+            transform = {}
+
+            for i, l in enumerate(y_all):
+                transform[l.item()] = i
+            
+            # Retrieve the values of all new labels and store them in 'train_label'.
+            y_all = np.vectorize(transform.get)(all_labels)
+
+        return x_all, y_all
     
 
 class TSDataset(Dataset):
     def __init__(self, dataset_name, dataset_root_path=None, datasets_name=None, split=True):
         super().__init__(dataset_name, dataset_root_path, datasets_name, split)
 
     def load(self):
         # Call the parent class's ucr_dataset method to get the data
-        train_data, train_labels, test_data, test_labels = self.ts_dataset()
+        x_train, y_train, x_test, y_test = self.ts_dataset()
 
         # Modify or add any additional processing specific to TSDataset here
 
-        return train_data, train_labels, test_data, test_labels
+        return x_train, y_train, x_test, y_test 
     
     
 class UCRDataset(TSDataset):
     def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UCR', split=True):
         super().__init__(dataset_name, dataset_root_path, datasets_name, split)
         self.datasets_name = datasets_name
 
@@ -177,19 +194,19 @@
 
 class OpenDataset(Dataset):
     def __init__(self, dataset_name, dataset_root_path=None, datasets_name=None, split=False):
         super().__init__(dataset_name, dataset_root_path, datasets_name, split)
 
     def load(self):
         # Call the parent class's open_ucr_dataset method to get the data
-        all_data, all_labels = self.opents_dataset()
+        x_all, y_all = self.opents_dataset()
 
         # Modify or add any additional processing specific to OpenDataset here
 
-        return all_data, all_labels
+        return x_all, y_all
     
 class OpenUCRDataset(OpenDataset):
     def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UCR', split=False):
         super().__init__(dataset_name, dataset_root_path, datasets_name, split)
         self.datasets_name = datasets_name
 
 class OpenUEADataset(OpenDataset):
```

## Comparing `opents-0.1.2.1.dist-info/METADATA` & `opents-0.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opents
-Version: 0.1.2.1
+Version: 0.1.3
 Summary: OpenTS is a friendly Python Library for time series analysis
 Home-page: https://github.com/PyOpenTS/PyOpenTS
 Author: hushuguo
 Author-email: husg8217@mails.jlu.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: torch
```

## Comparing `opents-0.1.2.1.dist-info/RECORD` & `opents-0.1.3.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 opents/__init__.py,sha256=xRL8tSUxNiTSIygSIrQ0Y2i_guxRW_SNhljbNkCKNP4,54
 opents/data/__init__.py,sha256=E_iP2Kb-in3dJvXIMmvTbcBz6OrHVHDGFEwC-Qakdj0,14
 opents/data/generate_datasets.py,sha256=vh1CbEDm-UlIBhFIVJMivpFInA4xqoKLzyJJx_FuHso,6306
 opents/datasets/__init__.py,sha256=WXQaoGYqPi4E5-RpvsYmd9IUiijwbAgF97aJgvv_Pu8,77
-opents/datasets/datasets.py,sha256=zwxFCdc511ZZuUoh1yuRMHu3dlPeJEAmweA2S0vZ-Pc,9499
+opents/datasets/datasets.py,sha256=o0R3QgGYJnfv4b0DiWpKJTnfdh63QZrvQykkOhbBhZc,10072
 opents/nn/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 opents/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 opents/utils/data_utils.py,sha256=exRODMKhAbvLFgnQuZtZwPAcZiG-41S4OuMGlui76yo,3533
-opents-0.1.2.1.dist-info/METADATA,sha256=uzUqL4bOg8aNUYTnb3MqmW8rXIkFJYDZfBtRSY8YhIs,2025
-opents-0.1.2.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-opents-0.1.2.1.dist-info/top_level.txt,sha256=VMPO4pjOtyRL1h-EZc31aY2v5787ZqAKkOzzbkgw300,7
-opents-0.1.2.1.dist-info/RECORD,,
+opents-0.1.3.dist-info/METADATA,sha256=8g6ADJTzgho9nzaRu7OsQ-wAkuB5MjcDNffKTMJBJpg,2023
+opents-0.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+opents-0.1.3.dist-info/top_level.txt,sha256=VMPO4pjOtyRL1h-EZc31aY2v5787ZqAKkOzzbkgw300,7
+opents-0.1.3.dist-info/RECORD,,
```

