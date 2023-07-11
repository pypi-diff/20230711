# Comparing `tmp/cPredictor-0.1.3-py3-none-any.whl.zip` & `tmp/cPredictor-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 17393 bytes, number of entries: 11
--rw-r--r--  2.0 unx    31485 b- defN 23-Jul-07 16:35 cPredictor/SVM_prediction.py
--rw-r--r--  2.0 unx      354 b- defN 23-Jul-07 16:35 cPredictor/__init__.py
--rw-r--r--  2.0 unx     6315 b- defN 23-Jul-07 16:35 cPredictor/tests/SVM_prediction_test.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 16:35 cPredictor/tests/__init__.py
--rw-r--r--  2.0 unx     2351 b- defN 23-Jul-07 16:35 cPredictor/tests/cPredictor_test_model.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-07 16:39 cPredictor-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1666 b- defN 23-Jul-07 16:39 cPredictor-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 16:39 cPredictor-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx      227 b- defN 23-Jul-07 16:39 cPredictor-0.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-07 16:39 cPredictor-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      941 b- defN 23-Jul-07 16:39 cPredictor-0.1.3.dist-info/RECORD
-11 files, 54799 bytes uncompressed, 15785 bytes compressed:  71.2%
+Zip file size: 17505 bytes, number of entries: 11
+-rw-r--r--  2.0 unx    31691 b- defN 23-Jul-11 12:15 cPredictor/SVM_prediction.py
+-rw-r--r--  2.0 unx      354 b- defN 23-Jul-11 12:15 cPredictor/__init__.py
+-rw-r--r--  2.0 unx     6296 b- defN 23-Jul-11 12:15 cPredictor/tests/SVM_prediction_test.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 12:15 cPredictor/tests/__init__.py
+-rw-r--r--  2.0 unx     2398 b- defN 23-Jul-11 12:15 cPredictor/tests/cPredictor_test_model.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-11 12:18 cPredictor-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1666 b- defN 23-Jul-11 12:18 cPredictor-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 12:18 cPredictor-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      227 b- defN 23-Jul-11 12:18 cPredictor-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-11 12:18 cPredictor-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      941 b- defN 23-Jul-11 12:18 cPredictor-0.2.0.dist-info/RECORD
+11 files, 55033 bytes uncompressed, 15897 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: cPredictor/tests/__init__.py
 Comment: 
 
 Filename: cPredictor/tests/cPredictor_test_model.py
 Comment: 
 
-Filename: cPredictor-0.1.3.dist-info/LICENSE
+Filename: cPredictor-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: cPredictor-0.1.3.dist-info/METADATA
+Filename: cPredictor-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: cPredictor-0.1.3.dist-info/WHEEL
+Filename: cPredictor-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: cPredictor-0.1.3.dist-info/entry_points.txt
+Filename: cPredictor-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cPredictor-0.1.3.dist-info/top_level.txt
+Filename: cPredictor-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cPredictor-0.1.3.dist-info/RECORD
+Filename: cPredictor-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cPredictor/SVM_prediction.py

```diff
@@ -8,14 +8,15 @@
 import matplotlib
 import matplotlib.pyplot as plt
 from sklearn.svm import LinearSVC
 from sklearn.calibration import CalibratedClassifierCV
 from sklearn.metrics import confusion_matrix
 from sklearn.model_selection import KFold
 from sklearn.preprocessing import LabelEncoder
+from sklearn.preprocessing import MinMaxScaler
 from sklearn.metrics import f1_score
 from sklearn.metrics import accuracy_score
 from sklearn.metrics import precision_score
 from scanpy import read_h5ad
 from importlib.resources import files
 import re
 from statistics import mean
@@ -45,15 +46,22 @@
         training=read_h5ad(reference_H5AD) 
     if meta_atlas is True:
         meta_dir='data/cma_meta_atlas.h5ad'
         training=read_h5ad(meta_dir) 
 
     # Load in the test data
     testing=read_h5ad(query_H5AD)
- 
+
+    # Checks if the test data contains a raw data slot and sets it as the count value
+    try:
+        testing=testing.raw.to_adata()
+    except AttributeError:
+        print("Query object does not contain raw data, using sparce matrix from adata.X")
+        print("Please manually check if this sparce matrix contains actual raw counts")
+
     print("Generating training and testing matrices from the H5AD objects")
     
     # training data
     matrix_train = pd.DataFrame.sparse.from_spmatrix(training.X, index=list(training.obs.index.values), columns=list(training.var.features.values))
 
     # testing data
     try: 
@@ -99,28 +107,33 @@
         Threshold = Threshold_rej
 
     print("Log normalizing the training and testing data")
     
     # normalise data
     data_train = np.log1p(data_train)
     data_test = np.log1p(data_test)  
-        
+
+    print("Scaling the training and testing data")
+    scaler = MinMaxScaler()
+    data_train = scaler.fit_transform(data_train)
+    data_test = scaler.fit_transform(data_test)
+    
     Classifier = LinearSVC()
     pred = []
     
     if rejected is True:
         print("Running SVMrejection")
         kf = KFold(n_splits=3)
         clf = CalibratedClassifierCV(Classifier, cv=kf)
         probability = [] 
         clf.fit(data_train, labels_train.values.ravel())
         predicted = clf.predict(data_test)
         prob = np.max(clf.predict_proba(data_test), axis = 1)
         unlabeled = np.where(prob < Threshold)
-        predicted[unlabeled] = 'Unknown'
+        predicted[unlabeled] = 'Unlabeled'
         pred.extend(predicted)
         probability.extend(prob)
         pred = pd.DataFrame(pred)
         probability = pd.DataFrame(probability)
         
         # Save the labels and probability
         pred.to_csv(str(OutputDir) + "SVMrej_Pred_Labels.csv", index = False)
@@ -157,39 +170,32 @@
 
     # Load in the object and add the predicted labels
     print("Adding predictions to query data")
     for file in os.listdir(OutputDir):
         if file.endswith('.csv'):
             if 'rej' not in file:
                 filedir= OutputDir+file
-                #print(filedir)
-                influence_data= pd.read_csv(filedir,sep=',',index_col=0)
-                #print(influence_data)
-                influence_data=influence_data.index.tolist()
-                adata.obs["SVM_predicted"]=influence_data
+                SVM_output_dir= pd.read_csv(filedir,sep=',',index_col=0)
+                SVM_output_dir=SVM_output_dir.index.tolist()
+                adata.obs["SVM_predicted"]=SVM_output_dir
             if 'rej_Pred' in file:
                 filedir= OutputDir+file
-                #print(filedir)
-                influence_data= pd.read_csv(filedir,sep=',',index_col=0)
-                #print(influence_data)
-                influence_data=influence_data.index.tolist()
-                adata.obs["SVMrej_predicted"]=influence_data
+                SVM_output_dir= pd.read_csv(filedir,sep=',',index_col=0)
+                SVM_output_dir=SVM_output_dir.index.tolist()
+                adata.obs["SVMrej_predicted"]=SVM_output_dir
             if 'rej_Prob' in file:
                 filedir= OutputDir+file
-                #print(filedir)
-                influence_data= pd.read_csv(filedir,sep=',',index_col=0)
-                #print(influence_data)
-                influence_data=influence_data.index.tolist()
-                adata.obs["SVMrej_predicted_prob"]=influence_data
+                SVM_output_dir= pd.read_csv(filedir,sep=',',index_col=0)
+                SVM_output_dir=SVM_output_dir.index.tolist()
+                adata.obs["SVMrej_predicted_prob"]=SVM_output_dir
 
     # Set category colors:
     if meta_atlas is True and colord is not None:
         df_category_colors=pd.read_csv(colord, header=None,index_col=False, sep='\t')
         category_colors = dict(zip(df_category_colors.iloc[:,0], df_category_colors.iloc[:,1]))
-        print(category_colors)
         if SVM_key == "SVMrej_predicted":
           category_colors["Unlabeled"]= "#808080"
                     
     if meta_atlas is False or colord is None:
     
       # Load a large color palette
       palette_name = "tab20"
@@ -236,24 +242,22 @@
 
         if meta_atlas is True and colord is not None:
             palette=category_colors
             if SVM_type == 'SVM' :
               ord_list = [key for key in palette]
               
             if SVM_type == 'SVMrej':
-              colordkeys_list = [key for key in palette]
-              ord_list=colordkeys_list.append("Unlabeled")
+              ord_list = [key for key in palette]
             
             # Sorts the df on the longer ordered list
             def sort_small_list(long_list, small_list):
               sorted_list = sorted(small_list, key=lambda x: long_list.index(x))
               return sorted_list
             
             sorter = sort_small_list(ord_list, df.columns.tolist())
-            #sorter=sorted(df.columns, key=ord_list.get)
             
             # Retrieve the color codes from the sorted list
             lstval = [palette[key] for key in sorter]
             
             try:
               df=df[sorter]
             except KeyError:
@@ -292,15 +296,14 @@
 
         # Set labels and title
         plt.xlabel('SVM Certainty Scores')
         plt.ylabel('Density')
         plt.title('Stacked Density Plots of Prediction Certainty Scores by Cell State')
 
         # Add a legend
-        #fig.legend(loc=7,title="Cell states and median predictions scores")
         plt.legend(bbox_to_anchor=(1.04, 1), loc="upper left")
 
         # Saving the density plot
         fig.savefig("figures/Density_prediction_scores.pdf", bbox_inches='tight')
         plt.close(fig)
     else:
         None
@@ -331,14 +334,18 @@
     print("Normalising the data")
     data = data.to_numpy(dtype="float16")
     np.log1p(data,out=data)
 
     X = data
     del data
 
+    print("Scaling the data")
+    scaler = MinMaxScaler()
+    X = scaler.fit_transform(X)
+    
     label_encoder = LabelEncoder()
     
     y = label_encoder.fit_transform(labels.iloc[:,0].tolist())
 
     # Generate a dictionary to map values to strings
     res = dict(zip(label_encoder.inverse_transform(y),y))
     res['Unlabeled'] = 999999
@@ -350,23 +357,19 @@
 
     train_indices = []
     test_indices = []
 
     # Iterate over each fold and split the data
     print("Generate indices for train and test")
     for train_index, test_index in kfold.split(X):
-        #X_train, X_test = X[train_index], X[test_index]
         y_train, y_test = y[train_index], y[test_index]
 
         # Store the indices of the training and test sets for each fold
         train_indices.append(list(train_index))
         test_indices.append(list(test_index))
-        
-    #train_indices = list(train_indices)
-    #test_indices = list(test_indices)
 
     # Run the SVM model
     test_ind=test_indices
     train_ind=train_indices
     Classifier = LinearSVC()
 
     if SVM_type == "SVMrej":
@@ -493,27 +496,30 @@
     # Reading in the Labels_1 for the replicates
     # First tries to read in Labels_1 as a path
     try:
       label_data=pd.read_csv(Labels_1,sep=',',index_col=0)
       label_data=label_data.index.tolist()
       cond_1.obs["meta_atlas"]=label_data
       cond_1_label="meta_atlas"
+
     # Then tries to read in Labels_1 as a string in obs
     except (TypeError, FileNotFoundError) as error:
       try:
         cond_1_label=str(Labels_1)
         cond_1.obs[cond_1_label]
+
     # If no key if found a valid key must be entered
       except KeyError:
         raise ValueError('Please provide a valid name for labels in Labels_1')
       
     print("Constructing condition for condition 1")
     cond_1.obs["condition"]="cond1"
 
     print("Constructing batches for condition 1")
+
     # Add extra index to the ref object:
     cond_1.obs["batch"] = cond_1.obs[condition_1_batch]
 
     # Convert the 'Category' column to numeric labels
     cond_1.obs["batch"] = pd.factorize(cond_1.obs["batch"])[0] + 1
 
     cond_1.obs["merged"]=cond_1.obs[cond_1_label]+"."+cond_1.obs["condition"]
@@ -545,15 +551,15 @@
             cond_name="cond2"
 
         # Construct the sample.tsv file    
         cond.obs["assembly"]="hg38"
 
         adata = cond.copy()
 
-        # extract names of genes
+        # Extract names of genes
         try:
             adata.var_names=adata.var["_index"].tolist()
         except KeyError:
             adata.var_names=adata.var.index
 
 
         for cluster_id in ["merged_batch","full_batch"]:
@@ -708,30 +714,30 @@
 
 def importpars():
 
     parser = argparse.ArgumentParser(description="Imports predicted results back to H5AD file")
     parser.add_argument("--query_H5AD", type=str, help="Path to query H5AD file")
     parser.add_argument("--OutputDir", type=str, help="Output directory path")
     parser.add_argument("--SVM_type", type=str, help="Type of SVM prediction (SVM or SVMrej)")
-    parser.add_argument("--colord", type=str, help=".tsv file with meta-atlas order and colors")
     parser.add_argument("--replicates", type=str, help="Replicates")
+    parser.add_argument("--colord", type=str, help=".tsv file with meta-atlas order and colors")
     parser.add_argument("--meta-atlas", dest="meta_atlas", action="store_true", help="Use meta-atlas data")
+    parser.add_argument("--show_bar", dest="show_bar", action="store_true", help="Plot barplot with SVM labels over specified replicates")
 
     args = parser.parse_args()
 
     SVM_import(
         args.query_H5AD,
         args.OutputDir,
         args.SVM_type,
-        args.colord,
         args.replicates,
+        args.colord,
         args.meta_atlas,
         args.show_bar)
-
-# ADD 
+    
 
 def pseudopars():
 
     parser = argparse.ArgumentParser(description="Performs individual and joined pseudobulk on two H5AD objects")
     parser.add_argument("--condition_1", type=str, help="Path to meta-atlas or other H5AD file")
     parser.add_argument("--condition_1_batch", type=str, help="Technical, biological or other replicate column in condition_1.obs")
     parser.add_argument("--condition_2", type=str, help="Path to H5AD file with SVM predictions")
```

## cPredictor/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.3"
+__version__ = "0.2.0"
 
 from .SVM_prediction import SVM_predict
 from .SVM_prediction import SVM_import
 from .SVM_prediction import SVM_performance
 from .SVM_prediction import SVM_pseudobulk
 from .SVM_prediction import predpars
 from .SVM_prediction import importpars
```

## cPredictor/tests/SVM_prediction_test.py

```diff
@@ -5,22 +5,21 @@
 import pandas as pd
 import scanpy as sc
 import time as tm
 import seaborn as sns
 from sklearn.svm import LinearSVC
 from sklearn.calibration import CalibratedClassifierCV
 from sklearn.metrics import confusion_matrix
+from sklearn.preprocessing import MinMaxScaler
 from scanpy import read_h5ad
 from importlib_resources import files
 import subprocess
 import re
 import matplotlib.pyplot as plt
 from statistics import mean
-from scipy.stats import pearsonr
-from scipy.stats import spearmanr
 
 # Import standalone functions for unit tests
 from cPredictor.SVM_prediction import SVM_predict
 from cPredictor.SVM_prediction import SVM_import
 from cPredictor.SVM_prediction import SVM_pseudobulk
 from cPredictor.SVM_prediction import SVM_performance
 from cPredictor.SVM_prediction import predpars
@@ -174,8 +173,8 @@
                               '--condition_2', str("SVM_predicted.h5ad"),
                               '--condition_2_batch', str("batch"),
                               '--Labels_1', str(labels)]
 
     subprocess.run(command_to_be_executed, shell=False, timeout=None,
                    text=True)
     assert os.path.exists("pseudobulk_output/full_batch_samples.tsv") == 1
-    assert os.path.exists("pseudobulk_output/merged_batch_samples.tsv") == 1
+    assert os.path.exists("pseudobulk_output/merged_batch_samples.tsv") == 1
```

## cPredictor/tests/cPredictor_test_model.py

```diff
@@ -9,29 +9,30 @@
 import matplotlib
 import matplotlib.pyplot as plt
 from sklearn.svm import LinearSVC
 from sklearn.calibration import CalibratedClassifierCV
 from sklearn.metrics import confusion_matrix
 from sklearn.model_selection import KFold
 from sklearn.preprocessing import LabelEncoder
+from sklearn.preprocessing import MinMaxScaler
 from sklearn.metrics import f1_score
 from sklearn.metrics import accuracy_score
 from sklearn.metrics import precision_score
 from scanpy import read_h5ad
 from importlib.resources import files
 
 print("Import performance function")
 from cPredictor.SVM_prediction import SVM_performance
 os.environ["GIT_PYTHON_REFRESH"] = "quiet"
 import git
 
 reference = "data/cma_meta_atlas.h5ad"
 labels = "data/training_labels_meta.csv"
 outdir = "test_output/"
-cPredictor_version = "0.1.3"
+cPredictor_version = "0.2.0"
 
 metrics = SVM_performance(reference_H5AD=reference,LabelsPath=labels,OutputDir=outdir)
 
 print("Setup tokens")
 # Set environments and passwords
 DAGSHUB_USER_NAME = 'Arts-of-coding'
 DAGSHUB_TOKEN =  os.environ['DH_key']
```

## Comparing `cPredictor-0.1.3.dist-info/LICENSE` & `cPredictor-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cPredictor-0.1.3.dist-info/METADATA` & `cPredictor-0.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cPredictor
-Version: 0.1.3
+Version: 0.2.0
 Summary: Cell command line predictor
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools (<=57.5.0)
 Requires-Dist: wheel
 Requires-Dist: python-build
 Requires-Dist: pytest-cov
```

## Comparing `cPredictor-0.1.3.dist-info/RECORD` & `cPredictor-0.2.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-cPredictor/SVM_prediction.py,sha256=ELe7jNHNEMfxIqNIYh68DrUBz1DkUJJSGKYzq3kYCF0,31485
-cPredictor/__init__.py,sha256=PjBteb1KRYocvJh79pgVH6z1tLyXbW6SEeiAlEbpgos,354
-cPredictor/tests/SVM_prediction_test.py,sha256=Jhog2SlFpTe1maaXKpPyZxEo0kwXVyhjd42Kk1W8btY,6315
+cPredictor/SVM_prediction.py,sha256=tBhhE198yfBmBouig5XwEEE1dlh8Oro_4NU6Q4DmSHI,31691
+cPredictor/__init__.py,sha256=BPB6whyP8RMW2Pt_92ymT9NglnPP8dRuLQxdsa3_nZg,354
+cPredictor/tests/SVM_prediction_test.py,sha256=GmDC5ncB_v5LQGeDvm2CSBqTSxz9g77wEQFvTBubux0,6296
 cPredictor/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cPredictor/tests/cPredictor_test_model.py,sha256=kQswXDldAYX0qZdjkDfghWd2VPrzzmV4yDDQI2YXYek,2351
-cPredictor-0.1.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-cPredictor-0.1.3.dist-info/METADATA,sha256=bcg9_BzrdOmU2GZ22U9E-wDHmvVseu3NNU7Dyk8AL8k,1666
-cPredictor-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cPredictor-0.1.3.dist-info/entry_points.txt,sha256=jWviDlyXk8UTuVRVDXW5ihbZ7xWbKSt3uKRwjx2pvJw,227
-cPredictor-0.1.3.dist-info/top_level.txt,sha256=NXWRMFJ_ywM9zoRGffXs1j38bnAtf-odfECMfsNtJV4,11
-cPredictor-0.1.3.dist-info/RECORD,,
+cPredictor/tests/cPredictor_test_model.py,sha256=sQGbWo1QC3qSOgM0n64KdJdyLAW9Em-MupufqinYcrU,2398
+cPredictor-0.2.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+cPredictor-0.2.0.dist-info/METADATA,sha256=WqLS6atfXf3-3jydllORZisJ8jBi0q9XffaxMYYEbU0,1666
+cPredictor-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cPredictor-0.2.0.dist-info/entry_points.txt,sha256=jWviDlyXk8UTuVRVDXW5ihbZ7xWbKSt3uKRwjx2pvJw,227
+cPredictor-0.2.0.dist-info/top_level.txt,sha256=NXWRMFJ_ywM9zoRGffXs1j38bnAtf-odfECMfsNtJV4,11
+cPredictor-0.2.0.dist-info/RECORD,,
```

