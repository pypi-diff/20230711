# Comparing `tmp/opents-0.1.2-py3-none-any.whl.zip` & `tmp/opents-0.1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 7298 bytes, number of entries: 12
+Zip file size: 7338 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx       54 b- defN 23-Jun-20 07:42 opents/__init__.py
 -rw-rw-r--  2.0 unx       14 b- defN 23-Jun-20 07:42 opents/data/__init__.py
 -rw-rw-r--  2.0 unx     6306 b- defN 23-Jun-20 13:04 opents/data/generate_datasets.py
 -rw-rw-r--  2.0 unx       77 b- defN 23-Jul-10 08:32 opents/datasets/__init__.py
--rw-rw-r--  2.0 unx     9398 b- defN 23-Jul-11 06:30 opents/datasets/datasets.py
+-rw-rw-r--  2.0 unx     9499 b- defN 23-Jul-11 07:17 opents/datasets/datasets.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-28 15:32 opents/nn/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-28 15:32 opents/utils/__init__.py
 -rw-rw-r--  2.0 unx     3533 b- defN 23-Jul-11 06:11 opents/utils/data_utils.py
--rw-rw-r--  2.0 unx     2023 b- defN 23-Jul-11 06:32 opents-0.1.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 06:32 opents-0.1.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jul-11 06:32 opents-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      935 b- defN 23-Jul-11 06:32 opents-0.1.2.dist-info/RECORD
-12 files, 22439 bytes uncompressed, 5720 bytes compressed:  74.5%
+-rw-rw-r--  2.0 unx     2025 b- defN 23-Jul-11 07:20 opents-0.1.2.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 07:20 opents-0.1.2.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jul-11 07:20 opents-0.1.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      943 b- defN 23-Jul-11 07:20 opents-0.1.2.1.dist-info/RECORD
+12 files, 22550 bytes uncompressed, 5744 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: opents/utils/__init__.py
 Comment: 
 
 Filename: opents/utils/data_utils.py
 Comment: 
 
-Filename: opents-0.1.2.dist-info/METADATA
+Filename: opents-0.1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: opents-0.1.2.dist-info/WHEEL
+Filename: opents-0.1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: opents-0.1.2.dist-info/top_level.txt
+Filename: opents-0.1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: opents-0.1.2.dist-info/RECORD
+Filename: opents-0.1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opents/datasets/datasets.py

```diff
@@ -43,15 +43,15 @@
         if self.datasets_root_name.lower() == 'ucr':
             # Create a two-dimensional tensor file from the data in the training set and testing set files.
             train_tensor = torch.tensor(train_file_df.values)
             test_tensor = torch.tensor(test_file_df.values)
 
             # Here, we extract the distinct labels from each dataset.
             train_labels = torch.unique(train_tensor[:, 0])
-            test_labels = torch.unique       
+            test_labels = torch.unique(test_tensor[:, 0]) 
             
             # Convert the data into a list.
             train_array = train_tensor.tolist()
             train_array = np.array(train_array)
             test_array = test_tensor.tolist()
             test_array = np.array(test_array)
 
@@ -70,29 +70,32 @@
             y_test = np.vectorize(transform.get)(test_array[:, 0])
             # if dataset's dimention is 2, we change the dimention to 3
             x_train = x_train[..., np.newaxis]
             x_test = x_test[..., np.newaxis]           
 
         elif self.datasets_root_name.lower() == 'uea':
             train_dataset_name = self.dataset_name + "_TRAIN"
-            test_dataset_name = self.dataset_name + "_TEST"
+            test_dataset_name = self.dataset_name + "_TRAIN"
 
             # Store the train data and test data in list, and extend its dimention to 3.
             train_array = np.array(train_file_df[train_dataset_name].tolist())
             x_train = train_array.view((np.float64, len(train_array.dtype.names)))
 
-            test_array = np.array(test_file_df[train_dataset_name].tolist())
+            test_array = np.array(test_file_df[test_dataset_name].tolist())
             x_test = test_array.view((np.float64, len(test_array.dtype.names)))
 
             # Here, we extract the distinct labels from each dataset.
-            train_labels = torch.unique(torch.tensor(pd.to_numeric(train_file_df['target'], errors='coerce')))
-            test_labels = torch.unique(torch.tensor(pd.to_numeric(test_file_df['target'], errors='coerce')))
+            train_labels = torch.tensor(pd.to_numeric(train_file_df['target'], errors='coerce'))
+            train_label = torch.unique(train_labels)
+            test_labels = torch.tensor(pd.to_numeric(test_file_df['target'], errors='coerce'))
+            test_label = torch.unique(test_labels)
+            
             transform = {}
 
-            for i, l in enumerate(train_labels):
+            for i, l in enumerate(train_label):
                 transform[l.item()] = i
             
             # Retrieve the values of all new labels and store them in 'train_label'.
             y_train = np.vectorize(transform.get)(train_labels)
 
             # Retrieve all label values from the test set and store them in 'test_label'.
             y_test = np.vectorize(transform.get)(test_labels)
```

## Comparing `opents-0.1.2.dist-info/METADATA` & `opents-0.1.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opents
-Version: 0.1.2
+Version: 0.1.2.1
 Summary: OpenTS is a friendly Python Library for time series analysis
 Home-page: https://github.com/PyOpenTS/PyOpenTS
 Author: hushuguo
 Author-email: husg8217@mails.jlu.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: torch
```

## Comparing `opents-0.1.2.dist-info/RECORD` & `opents-0.1.2.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 opents/__init__.py,sha256=xRL8tSUxNiTSIygSIrQ0Y2i_guxRW_SNhljbNkCKNP4,54
 opents/data/__init__.py,sha256=E_iP2Kb-in3dJvXIMmvTbcBz6OrHVHDGFEwC-Qakdj0,14
 opents/data/generate_datasets.py,sha256=vh1CbEDm-UlIBhFIVJMivpFInA4xqoKLzyJJx_FuHso,6306
 opents/datasets/__init__.py,sha256=WXQaoGYqPi4E5-RpvsYmd9IUiijwbAgF97aJgvv_Pu8,77
-opents/datasets/datasets.py,sha256=03eaub7u7qj7gzHZnSo9PKZMRgaxiA1LLxLbG6WBY2s,9398
+opents/datasets/datasets.py,sha256=zwxFCdc511ZZuUoh1yuRMHu3dlPeJEAmweA2S0vZ-Pc,9499
 opents/nn/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 opents/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 opents/utils/data_utils.py,sha256=exRODMKhAbvLFgnQuZtZwPAcZiG-41S4OuMGlui76yo,3533
-opents-0.1.2.dist-info/METADATA,sha256=IpfbP4j5lWHwXR4t1pao_98d98g4ATaCA9SGjhe-QSs,2023
-opents-0.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-opents-0.1.2.dist-info/top_level.txt,sha256=VMPO4pjOtyRL1h-EZc31aY2v5787ZqAKkOzzbkgw300,7
-opents-0.1.2.dist-info/RECORD,,
+opents-0.1.2.1.dist-info/METADATA,sha256=uzUqL4bOg8aNUYTnb3MqmW8rXIkFJYDZfBtRSY8YhIs,2025
+opents-0.1.2.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+opents-0.1.2.1.dist-info/top_level.txt,sha256=VMPO4pjOtyRL1h-EZc31aY2v5787ZqAKkOzzbkgw300,7
+opents-0.1.2.1.dist-info/RECORD,,
```

