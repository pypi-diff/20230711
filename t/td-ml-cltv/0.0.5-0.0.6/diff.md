# Comparing `tmp/td_ml_cltv-0.0.5.tar.gz` & `tmp/td_ml_cltv-0.0.6.tar.gz`

## Comparing `td_ml_cltv-0.0.5.tar` & `td_ml_cltv-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.5/.DS_Store
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.5/src/td_ml_cltv/__init__.py
--rw-r--r--   0        0        0    12626 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.5/src/td_ml_cltv/cltv_helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.5/LICENSE
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.5/README.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.6/.DS_Store
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.6/src/td_ml_cltv/__init__.py
+-rw-r--r--   0        0        0    10738 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.6/src/td_ml_cltv/cltv_helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.6/LICENSE
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.6/README.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.6/PKG-INFO
```

### Comparing `td_ml_cltv-0.0.5/.DS_Store` & `td_ml_cltv-0.0.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `td_ml_cltv-0.0.5/src/td_ml_cltv/cltv_helpers.py` & `td_ml_cltv-0.0.6/src/td_ml_cltv/cltv_helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,61 +21,34 @@
 from sklearn.cluster import KMeans
 from sklearn.impute import SimpleImputer
 from scipy.sparse import issparse
 from shap.utils._legacy import DenseData
 import warnings
 warnings.filterwarnings("ignore")
 
-#Read data from TD using new optimized query     
-@profile
-def new_query(database, query_syntax, td_api_key, td_api_server):
-
-    #set dictonaries where you will store column name-datatype pairs
-    dtype_list = [('object', np.object_),('float16', np.float16) , ('float32', np.float32), ('uint8', np.uint8), 
-                  ('uint16', np.uint16), ('uint32', np.uint32)]
-    object_dict = {}
-
-    #query db.table in TD and save job.results() as np.array
-    with tdclient.Client(apikey=td_api_key, endpoint=td_api_server) as td:
-            job = td.query(database, query_syntax, type='presto')
-            job.wait()
-            raw_array = np.array(list(job.result()))
-            columns = [f[0] for f in job.result_schema]
-            
-            #take a small slice of the job.results object and create a small sample DF
-            sliced = islice(job.result(), 10)
-            sample_df = pd.DataFrame(sliced, columns=columns)
-            
-            #apply reducer to sample_df to exctract the optimal datatypes for each column
-            test_df = Reducer(use_null_int=False, n_jobs = 1).reduce(sample_df, verbose=False)
-            
-            #below stores a list of column names, index positions in DF and converted datatypes after reducer was applied
-            for data_type in dtype_list:
-                cols_idxs = [(col, test_df.columns.get_loc(col)) for col in test_df.columns if test_df[col].dtype.name == data_type[0]]
-                if len(cols_idxs):
-                    object_dict[data_type[0]] = cols_idxs
-            
-            #Generate a base array by extracting all Object dtypes using indexes on the job_results array
-            object_arr =  np.take(raw_array, [item[1] for item in object_dict['object']], axis = 1)
-            object_arr = object_arr.astype(np.object_)
-            base_df = pd.DataFrame(object_arr, columns = [item[0] for item in object_dict['object']])
-            
-            #Loop through list of all other datatypes, create temporary DFs for each and concat to base_df 
-            for tup in dtype_list[1:]:
-                if tup[0] in list(object_dict.keys()):
-                    new_arr = np.take(raw_array, [item[1] for item in object_dict[tup[0]]], axis = 1)
-                    new_arr = new_arr.astype(np.float32).astype(tup[1])
-                    names = [item[0] for item in object_dict[tup[0]]]
-                    new_df = pd.DataFrame(new_arr, columns = names)
-                    base_df = pd.concat([base_df, new_df], axis = 1)
-                    
-                    #delete temp df after concating to base_df, to free space
-                    del new_df
-                    
-    return base_df
+
+def get_table(table, db, apikey, td_api_server):
+    """Retrieve table from TD account.
+
+    Args:
+        table (str): Table to retrieve data from. may also include additional SQL clauses; anything after the FROM in a query.
+        db (str): Database to retrieve table from.
+        apikey (str): Master API key from TD account, must have query permissions.
+        td_api_server (str): TD API server.
+
+    Returns:
+        Pandas DataFrame: query result.
+    """
+    with tdclient.Client(apikey=apikey, endpoint=td_api_server) as td:
+        job = td.query(db, f"SELECT * FROM {table}", type='presto')
+        job.wait()
+        data = job.result()
+        columns = [f[0] for f in job.result_schema]
+        df = pd.DataFrame(data, columns=columns)
+    return df
 
 
 # Function below replaces outliers with desired percentile of data. It also allows to change the 1.5 coeff
 def replace_outliers(target, q_up = 0.98, q_low = 0.02, coeff = 1):
     Q1 = target.quantile(0.25)
     Q3 = target.quantile(0.75)
     IQR = Q3 - Q1
@@ -84,43 +57,41 @@
     #these can also be controled using q_up and q_low coeffs
     target = target.where(target < (Q3 + coeff * IQR), target.quantile(q_up))
     target = target.where(target > (Q1 - coeff * IQR), target.quantile(q_low))
     
     return target
 
 
-def query_data_splits(database, input_table, num_splits = 1):
+def query_data_splits(database, input_table, apikey, td_api_server, num_splits=1):
 
     #create split ratio based on how many times you want to split original table
     split = 1.0 / num_splits
     
     #empty list to store temporary DFs
     df_list = []
     
     #Loop through count of splits and query original table in TD in smaller chunks and reduce each chunk
     for i in list(range(num_splits)):
         query_syntax = f'select * from {input_table} where rnd > {i*split} AND rnd <= {(i+1)*split}'
         print(query_syntax)
         
-        temp_df = new_query(database, query_syntax)
+        temp_df = get_table(f'{input_table} where rnd > {i*split} AND rnd <= {(i+1)*split}', database, 
+                            apikey, td_api_server)
         temp_df = Reducer(use_null_int=False, n_jobs = 1).reduce(temp_df, verbose=False)
         df_list.append(temp_df)
         del temp_df
         
     #Concactenate all reduced chunk into a final DF and reduce one last time
     df_final= pd.concat(df_list, ignore_index = True)
-    # df_final= Reducer(use_null_int=False, n_jobs = 1).reduce(df_final, verbose=False)
     
     return df_final
 
 
-
    
 # Function for getting importances via coefficients
-@profile
 def impt_coef(model, x_data):
     try:
         importances = model.coef_
     except:
         importances = model.feature_importances_
 
     features = x_data.columns
```

### Comparing `td_ml_cltv-0.0.5/pyproject.toml` & `td_ml_cltv-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "td_ml_cltv"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Yish Lim", email="yish.lim@treasure-data.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

