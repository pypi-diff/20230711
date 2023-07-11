# Comparing `tmp/Alpha_Rabbit-1.4.6.tar.gz` & `tmp/Alpha_Rabbit-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Alpha_Rabbit-1.4.6.tar", last modified: Mon Jul 10 10:04:14 2023, max compression
+gzip compressed data, was "Alpha_Rabbit-1.4.7.tar", last modified: Tue Jul 11 09:21:18 2023, max compression
```

## Comparing `Alpha_Rabbit-1.4.6.tar` & `Alpha_Rabbit-1.4.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 10:04:14.193369 Alpha_Rabbit-1.4.6/
-drwxrwxrwx   0        0        0        0 2023-07-10 10:04:13.916326 Alpha_Rabbit-1.4.6/Alpha_Rabbit/
--rw-rw-rw-   0        0        0    42540 2023-07-10 10:03:27.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit/Alpha_Rabbit.py
--rw-rw-rw-   0        0        0    13979 2023-07-10 08:16:58.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit/Factor_Calculator.py
--rw-rw-rw-   0        0        0    22658 2023-06-05 07:41:31.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit/Factor_Def_and_Get_Method.py
--rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit/trade_strategy.py
-drwxrwxrwx   0        0        0        0 2023-07-10 10:04:13.984567 Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/
--rw-rw-rw-   0        0        0      787 2023-07-10 10:04:13.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-07-10 10:04:13.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 10:04:13.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-10 10:04:13.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-10 10:04:13.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.6/LICENSE.txt
--rw-rw-rw-   0        0        0      787 2023-07-10 10:04:14.193369 Alpha_Rabbit-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.6/README.md
--rw-rw-rw-   0        0        0       85 2023-07-10 10:04:14.196368 Alpha_Rabbit-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1229 2023-07-10 10:03:58.000000 Alpha_Rabbit-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:21:18.011242 Alpha_Rabbit-1.4.7/
+drwxrwxrwx   0        0        0        0 2023-07-11 09:21:17.384434 Alpha_Rabbit-1.4.7/Alpha_Rabbit/
+-rw-rw-rw-   0        0        0    43319 2023-07-11 09:19:02.000000 Alpha_Rabbit-1.4.7/Alpha_Rabbit/Alpha_Rabbit.py
+-rw-rw-rw-   0        0        0    13979 2023-07-10 08:16:58.000000 Alpha_Rabbit-1.4.7/Alpha_Rabbit/Factor_Calculator.py
+-rw-rw-rw-   0        0        0    22658 2023-06-05 07:41:31.000000 Alpha_Rabbit-1.4.7/Alpha_Rabbit/Factor_Def_and_Get_Method.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.7/Alpha_Rabbit/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.7/Alpha_Rabbit/trade_strategy.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:21:18.009158 Alpha_Rabbit-1.4.7/Alpha_Rabbit.egg-info/
+-rw-rw-rw-   0        0        0      787 2023-07-11 09:21:16.000000 Alpha_Rabbit-1.4.7/Alpha_Rabbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-07-11 09:21:16.000000 Alpha_Rabbit-1.4.7/Alpha_Rabbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 09:21:16.000000 Alpha_Rabbit-1.4.7/Alpha_Rabbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-11 09:21:16.000000 Alpha_Rabbit-1.4.7/Alpha_Rabbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-11 09:21:16.000000 Alpha_Rabbit-1.4.7/Alpha_Rabbit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.7/Alpha_Rabbit.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      787 2023-07-11 09:21:18.011749 Alpha_Rabbit-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.7/README.md
+-rw-rw-rw-   0        0        0       85 2023-07-11 09:21:18.012749 Alpha_Rabbit-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2023-07-11 09:20:59.000000 Alpha_Rabbit-1.4.7/setup.py
```

### Comparing `Alpha_Rabbit-1.4.6/Alpha_Rabbit/Alpha_Rabbit.py` & `Alpha_Rabbit-1.4.7/Alpha_Rabbit/Alpha_Rabbit.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,19 +44,23 @@
     def one_factor_return(self,df,factorname,ndays,return_col,w_method,demean = False): # 计算分组收益
         if w_method =='average':
             qreturn = df.groupby(level = 'date', group_keys = True).apply(lambda x: x.groupby(factorname+'_quantile')[[return_col]].mean()/ndays).unstack()
             qreturn.columns = [i[1] for i in list(qreturn)]
             
         if w_method == 'factor_weighted':
             tmpdf = df.copy()
-            tmpdf[tmpdf[factorname]<0][return_col]*=-1
+            tmpdf['rwf'] = tmpdf[return_col]*tmpdf[factorname]
+            tmpdf.dropna(subset = ['rwf'],inplace = True)
             qreturn = tmpdf.groupby(level = 'date', group_keys = True).\
                 apply(lambda x: x.groupby(factorname+'_quantile').\
-                      apply(lambda x: (x[return_col]*x[factorname]).sum()/x[factorname].sum())/ndays)       
-
+                      apply(lambda x: x['rwf'].sum()/x[factorname].sum() if x[factorname].sum()>0 else 0)/ndays)       
+            # qreturn = tmpdf.groupby(level = 'date', group_keys = True).\
+            #     apply(lambda x: x.groupby(factorname+'_quantile').\
+            #           apply(lambda x: (x[return_col]*x[factorname]).sum()/x[factorname].sum())/ndays)      
+            
         if w_method =='cap_weighted':
             qreturn = df.groupby(level = 'date', group_keys = True).\
                 apply(lambda x: x.groupby(factorname+'_quantile').\
                       apply(lambda x: (x[return_col]*x['cap']).sum()/x['cap'].sum())/ndays)
 
         if demean:
             qreturn = qreturn.apply(lambda x: x-x.mean(),axis = 1)
@@ -97,14 +101,18 @@
         clean_factor[str(days)+'D'] = fwr[str(days)+'D']
         clean_factor = clean_factor.reset_index()
         clean_factor['date'] = clean_factor['date'].astype(str)
         clean_factor = clean_factor.set_index(['date','asset']).dropna()
         if index_price is not None:
             clean_factor = mate_al.trans_ex_return(clean_factor,index_price,ret_col=[str(days)+'D'])
         qreturn = self.one_factor_return(clean_factor,fcname,days,str(days)+'D',w_method = weight_method,demean=demean)
+        if len(qreturn.index.names)==1:
+            pass
+        else:
+            qreturn= qreturn.unstack().fillna(0)
         plottools.factor_plt(qreturn,to,fcname,savedir)
         return qreturn,clean_factor
     
     def judge_material(self,qreturn,fc):
         quantiles = max(qreturn.columns)
         lsret = qreturn[quantiles] - qreturn[1]
         groupmean = qreturn.mean(axis = 0)
@@ -656,35 +664,42 @@
         self.weighted_method = weighted_method
         pass
 
     def AutoMatic_DirCheck(self,path):
         if not os.path.exists(path):
             os.makedirs(path)
 
-    def AutoMatic_Direc_Adjust(self,neu_factors,dir_):
+    def AutoMatic_Direc_Adjust(self,factors,dir_):
+        neu_factors = factors.copy()
         direction_dict = {}
         self.AutoMatic_DirCheck(dir_+'direction/')
         for fc in list(neu_factors):
             res_df = self.sst.factor_prepare(neu_factors,fc,self.quantiles,self.qcut)
             if self.weighted_method == 'cap_weighted':
                 res_df['cap'] = self.cap
             qreturn = self.sst.factor_ret_test_sheet(self.weighted_method,self.base_index,fc,res_df,self.Price,self.days,dir_+'/direction/',self.demean)[0]
             if qreturn[list(qreturn)[0]].sum()<= qreturn[self.quantiles].sum():
                 print(fc+'是正向因子')
                 direction_dict[fc] = 1
             if qreturn[list(qreturn)[0]].sum() > qreturn[self.quantiles].sum():
                 print(fc+'是负向因子')
+                neu_factors = neu_factors.copy()
                 neu_factors[fc]*=-1
                 direction_dict[fc] = -1
         self.AutoMatic_DirCheck(dir_+'direction/redirection/')
         neu_factors = self.mft.mat_normlize(neu_factors)
+        best_perf_sr = 0
         for fc in list(neu_factors):
             res_df = self.sst.factor_prepare(neu_factors,fc,self.quantiles,self.qcut)
             qreturn = self.sst.factor_ret_test_sheet(self.weighted_method,self.base_index,fc,res_df,self.Price,self.days,dir_+'direction/redirection/',self.demean)[0]
-        return neu_factors,direction_dict
+            perf_sr = self.AutoMatic_Compare_Indicator(qreturn,False)
+            if perf_sr > best_perf_sr:
+                best_perf_sr = perf_sr
+                selected_fc = fc
+        return neu_factors,direction_dict,selected_fc
     
     def AutoMatic_Factor_Merge_Ret(self,neu_factors,base_factors,mergename,dir_):
         base_f = pd.DataFrame(neu_factors[base_factors].sum(axis = 1),columns = [mergename])
         res_df = self.sst.factor_prepare(base_f,mergename,self.quantiles,self.qcut)
         self.AutoMatic_DirCheck(dir_)
         if self.weighted_method == 'cap_weighted':
             res_df['cap'] = self.cap
```

### Comparing `Alpha_Rabbit-1.4.6/Alpha_Rabbit/Factor_Calculator.py` & `Alpha_Rabbit-1.4.7/Alpha_Rabbit/Factor_Calculator.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.6/Alpha_Rabbit/Factor_Def_and_Get_Method.py` & `Alpha_Rabbit-1.4.7/Alpha_Rabbit/Factor_Def_and_Get_Method.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.6/Alpha_Rabbit/trade_strategy.py` & `Alpha_Rabbit-1.4.7/Alpha_Rabbit/trade_strategy.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.6/Alpha_Rabbit.egg-info/PKG-INFO` & `Alpha_Rabbit-1.4.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Alpha-Rabbit
-Version: 1.4.6
+Name: Alpha_Rabbit
+Version: 1.4.7
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.4.6/LICENSE.txt` & `Alpha_Rabbit-1.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.6/PKG-INFO` & `Alpha_Rabbit-1.4.7/Alpha_Rabbit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Alpha_Rabbit
-Version: 1.4.6
+Name: Alpha-Rabbit
+Version: 1.4.7
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.4.6/setup.py` & `Alpha_Rabbit-1.4.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Alpha_Rabbit",
-    version="1.4.6",
+    version="1.4.7",
     author="lijiongting",
     author_email="448986334@qq.com",
     description="Alpha_Rabbit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="",
```

