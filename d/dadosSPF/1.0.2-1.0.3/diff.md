# Comparing `tmp/dadosSPF-1.0.2.tar.gz` & `tmp/dadosSPF-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dadosSPF-1.0.2.tar", last modified: Mon Jun 19 14:29:51 2023, max compression
+gzip compressed data, was "dist/dadosSPF-1.0.3.tar", last modified: Tue Jul 11 19:33:40 2023, max compression
```

## Comparing `dadosSPF-1.0.2.tar` & `dadosSPF-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-19 14:29:51.000000 dadosSPF-1.0.2/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1309 2023-06-19 14:29:51.000000 dadosSPF-1.0.2/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      781 2023-06-13 13:23:21.000000 dadosSPF-1.0.2/README.md
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-19 14:29:51.000000 dadosSPF-1.0.2/dadosSPF/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-06-13 13:21:19.000000 dadosSPF-1.0.2/dadosSPF/__init__.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)    37018 2023-06-19 14:26:52.000000 dadosSPF-1.0.2/dadosSPF/dadosSPF.py
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-19 14:29:51.000000 dadosSPF-1.0.2/dadosSPF.egg-info/
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-19 14:29:51.000000 dadosSPF-1.0.2/dadosSPF.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1328 2023-06-13 13:22:55.000000 dadosSPF-1.0.2/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      219 2023-06-13 13:21:19.000000 dadosSPF-1.0.2/dadosSPF.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-06-13 13:23:37.000000 dadosSPF-1.0.2/dadosSPF.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-06-13 13:22:59.000000 dadosSPF-1.0.2/dadosSPF.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-06-13 13:21:19.000000 dadosSPF-1.0.2/dadosSPF.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1309 2023-06-19 14:29:50.000000 dadosSPF-1.0.2/dadosSPF.egg-info/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      528 2023-06-19 14:29:50.000000 dadosSPF-1.0.2/dadosSPF.egg-info/SOURCES.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-06-19 14:29:50.000000 dadosSPF-1.0.2/dadosSPF.egg-info/dependency_links.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-06-19 14:29:50.000000 dadosSPF-1.0.2/dadosSPF.egg-info/requires.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-06-19 14:29:50.000000 dadosSPF-1.0.2/dadosSPF.egg-info/top_level.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2023-06-19 14:29:51.000000 dadosSPF-1.0.2/setup.cfg
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      545 2023-06-19 14:27:45.000000 dadosSPF-1.0.2/setup.py
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-11 19:33:40.000000 dadosSPF-1.0.3/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1309 2023-07-11 19:33:40.000000 dadosSPF-1.0.3/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      781 2023-06-13 13:23:21.000000 dadosSPF-1.0.3/README.md
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-11 19:33:39.000000 dadosSPF-1.0.3/dadosSPF/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-06-13 13:21:19.000000 dadosSPF-1.0.3/dadosSPF/__init__.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)    40912 2023-07-11 19:33:12.000000 dadosSPF-1.0.3/dadosSPF/dadosSPF.py
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-11 19:33:40.000000 dadosSPF-1.0.3/dadosSPF.egg-info/
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-11 19:33:40.000000 dadosSPF-1.0.3/dadosSPF.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1328 2023-06-13 13:22:55.000000 dadosSPF-1.0.3/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      219 2023-06-13 13:21:19.000000 dadosSPF-1.0.3/dadosSPF.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-06-13 13:23:37.000000 dadosSPF-1.0.3/dadosSPF.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-06-13 13:22:59.000000 dadosSPF-1.0.3/dadosSPF.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-06-13 13:21:19.000000 dadosSPF-1.0.3/dadosSPF.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1309 2023-07-11 19:33:38.000000 dadosSPF-1.0.3/dadosSPF.egg-info/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      528 2023-07-11 19:33:39.000000 dadosSPF-1.0.3/dadosSPF.egg-info/SOURCES.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-07-11 19:33:38.000000 dadosSPF-1.0.3/dadosSPF.egg-info/dependency_links.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-07-11 19:33:38.000000 dadosSPF-1.0.3/dadosSPF.egg-info/requires.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-07-11 19:33:38.000000 dadosSPF-1.0.3/dadosSPF.egg-info/top_level.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2023-07-11 19:33:40.000000 dadosSPF-1.0.3/setup.cfg
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      545 2023-07-11 19:17:28.000000 dadosSPF-1.0.3/setup.py
```

### Comparing `dadosSPF-1.0.2/PKG-INFO` & `dadosSPF-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dadosSPF
-Version: 1.0.2
+Version: 1.0.3
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.com.br/dadosSPF
 Author: Carlos Piveta
 Author-email: cepo496@gmail.com
 License: MIT License
 Description: # dadosSPF
```

### Comparing `dadosSPF-1.0.2/README.md` & `dadosSPF-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dadosSPF-1.0.2/dadosSPF/dadosSPF.py` & `dadosSPF-1.0.3/dadosSPF/dadosSPF.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ =     "CARLOS PIVETA"
 __collaborators__ = "CARLOS PIVETA"
 __license__ =    "DADOS"
-__version__ =    "1.0.2"
+__version__ =    "1.0.3"
 __maintainer__ = "CARLOS PIVETA"
 __status__ =     "Production"
 
 import os
 import re
 import sys
 import glob
@@ -302,28 +302,31 @@
             impala.execute(strQuery)
             df = as_pandas(impala)
             return df
         except Exception as e:
             print('ERRO!!! ')
             print(e) 
             
-    def getLastPartition(self,strSchema,strTable,exportDataframe = False,intLimit = None):
+    def getLastPartition(self,strSchema,strTable,exportDataframe = False,intLimit = None,dPrint = True):
         """
-        [dtPartition] = getLastPartition(strSchema = 'abc',strTable ='tabela',[exportDataframe = True], [intLimit = 1000])
+        [dtPartition] = getLastPartition(strSchema = 'abc',strTable ='tabela',[exportDataframe = True], [intLimit = 1000],dPrint = True)
         Função para pegar a ultima partição caso exista 
         Parameters
         ----------
         strSchema: str
             Nome do database aonde a tabela esta localizada
         strTable : str
             Nome da tabela a ser deletada do ambiente sandbox
         exportDataframe: bol
             marcação [True/False] se o retorno será em dataframe ou string
         intLimit: int
             limitação de linhas de retorno
+        dPrint: bol
+            Define se será impresso a menssagem de retorno
+            
         
         Returns
         -------
         (exportDataframe = False) str
             valor da ultima partição da tabela
         
         (exportDataframe = True) dataframe
@@ -334,27 +337,27 @@
         if self.tpConn == None:
             self.getConn()
             
         strLimit  = '' if intLimit == None else ' limit '+str(intLimit)
         try:
             partition = self.tpConn.sql("SHOW PARTITIONS {}.{}".format(strSchema,strTable)).agg({"partition": "max"}).collect()[0][0].split('/')[0].split('=')
             if exportDataframe == False:
-                    print('ultima partição {} = {}'.format(partition[0],partition[1]))
+                    if dPrint == True: print('ultima partição {} = {}'.format(partition[0],partition[1]))
                     return partition[1]
             else:
                 try:
-                    print('ultima partição {} = {}'.format(partition[0],partition[1]))
+                    if dPrint == True: print('ultima partição {} = {}'.format(partition[0],partition[1]))
                     strsql = "select * from {}.{} where {}='{}' {}".format(strSchema,strTable,str(partition[0]),str(partition[1]),strLimit)
                     df = self.tpConn.sql(strsql)
                     return df
                 except Exception as e:
                     df = self.tpConn.sql('select * from {}.{} {}'.format(strSchema,strTable,strLimit))
                     return df
         except Exception as e:
-            print('Tabela {} não possui partição'.format(strTable))
+            if dPrint == True: print('Tabela {} não possui partição'.format(strTable))
             print(e)
             
     def toSandBox(self,strSchema,strTable,ultimaParticao = False,intLimit = None,CampoDocumento = None,tpDocumento = None):
         """
         toSandBox(strSchema = 'abc',strTable = 'tabela',[ultimaParticao = False],[intLimit = 100],[CampoDocumento = None],[tpDocumento = None])
         Função para salvar uma tabela do ambiente produtivo no ambiente sandbox com id unico caso seja necessário
         Parameters
@@ -634,51 +637,51 @@
             else:
                 raise ValueError("ERRO! Formato NÃO suportado !!!")
             print("csv {} salvo !!!".format(nomeArquivo))   
         except Exception as e:
             print("ERRO! csv {} NÃO salvo !!!".format(nomeArquivo))
             print(e)
     
-#     def replaceTbQuery(self,vQuery,vTabelas,limit_dev = 'limit 100'):
-#         list_tables = vTabelas.upper().split(",")
-#         for tb in list_tables:
-#             nmTb = tb.split(".")[1]
-#             if (self.environment == "DEV"):
-#                 tbName = self.sandbox+"."+tb.split(".")[1];
-#             else:
-#                 tbName=tb;
-#             vQuery = vQuery.replace(nmTb,nmTb.lower());
-#             vQuery = vQuery.replace(tb.lower(),tbName);  
-#             vQuery = vQuery.replace(tb.lower(),tbName.lower());  
-#             vQuery = vQuery.replace(tb,tbName);
-#         if(vQuery.lower().find("select")>=0):
-#             vQuery = vQuery+" "+limit_dev
-#         return vQuery;
-    
-#     def SaveFileProces(self,DF_INSERT,vTable,vEtapa,paths3):
-#         """
-#         Função utilizada pelo time de CRM
-#         """
-#         pos = len(vTable.split("_"))-1
-#         contexto = vTable.split("_")[pos]
-#         etapa = "0"+vEtapa+"_"+contexto.upper()
-#         pathFile ="{0}_{1}/parquet_tmp/{2}/".format(paths3,contexto,etapa)
-#         DF_INSERT\
-#          .write\
-#          .format("parquet")\
-#          .mode("overwrite")\
-#          .save(pathFile)
-#         print(f"Arquivo salvo em: {pathFile}");
-    
-#     def CheckPoint(self,df,table,paths3):
-#         pathTable = "{0}/temp/{1}/".format(paths3,table)
-#         self.spark.sparkContext.setCheckpointDir(pathTable)
-#         df = df.checkpoint()
-#         df.createOrReplaceTempView(table)
-#         return df
+    def replaceTbQuery(self,vQuery,vTabelas,limit_dev = 'limit 100'):
+        list_tables = vTabelas.upper().split(",")
+        for tb in list_tables:
+            nmTb = tb.split(".")[1]
+            if (self.environment == "DEV"):
+                tbName = self.sandbox+"."+tb.split(".")[1];
+            else:
+                tbName=tb;
+            vQuery = vQuery.replace(nmTb,nmTb.lower());
+            vQuery = vQuery.replace(tb.lower(),tbName);  
+            vQuery = vQuery.replace(tb.lower(),tbName.lower());  
+            vQuery = vQuery.replace(tb,tbName);
+        if(vQuery.lower().find("select")>=0):
+            vQuery = vQuery+" "+limit_dev
+        return vQuery;
+    
+    def SaveFileProces(self,DF_INSERT,vTable,vEtapa,paths3):
+        """
+        Função utilizada pelo time de CRM
+        """
+        pos = len(vTable.split("_"))-1
+        contexto = vTable.split("_")[pos]
+        etapa = "0"+vEtapa+"_"+contexto.upper()
+        pathFile ="{0}_{1}/parquet_tmp/{2}/".format(paths3,contexto,etapa)
+        DF_INSERT\
+         .write\
+         .format("parquet")\
+         .mode("overwrite")\
+         .save(pathFile)
+        print(f"Arquivo salvo em: {pathFile}");
+    
+    def CheckPoint(self,df,table,paths3):
+        pathTable = "{0}/temp/{1}/".format(paths3,table)
+        self.spark.sparkContext.setCheckpointDir(pathTable)
+        df = df.checkpoint()
+        df.createOrReplaceTempView(table)
+        return df
     
     def SetNullToString(self,df):
         """
         df2 = sc.SetNullToString(df)
 
         Função para alterar os valores Null para a string ''
 
@@ -760,14 +763,78 @@
                     print('ERRO!!! Arquivo {} NÃO carregado'.format(file))
                     move = False
                     print(e)
                 if move == True:
                     shutil.move(file, pasta+'carregados/'+arq)
         else:
             print('Sem arquivos para serem carregados')
+    
+def procImpalaSBX(self,strPasta = 'queries', strProc = 'MACRO', variaveis = {"strMes": "202302","strFim":'2023-07-31',"sandbox": self.sandbox}):
+    try:    
+        debugPrint = True
+        path = strPasta
+        files = os.listdir(strPasta)
+        str_where = {}
+        str_where = {**str_where, **variaveis}
+
+        if strProc != None:
+                file = strProc
+                file = file if file[-4:].lower() == '.txt' else file+'.txt'
+                resp = filter(lambda x: x == file, files)
+                resp = list(resp)
+
+                if resp != []:
+                    files = resp
+
+        files = sorted(files)
+        for fls in range(len(files)):
+            if files[fls].endswith(".txt"):
+                proc = files[fls].replace('.txt','')
+                with open(path+r'/'+files[fls], 'r') as file:
+                    query = file.read()
+                    try:
+                        query = query.format(**str_where)
+                    except Exception as e:
+                        print(e)
+                    table = files[fls].replace('.txt','')
+                    tmpTxt = query.replace(';','')
+                    arquivo = files[fls].replace('.txt','')
+                    tmptables = re.findall(r'FROM(.*?)(\S+)',tmpTxt.upper())
+                    tmptables = tmptables+re.findall(r'JOIN(.*?)(\S+)',tmpTxt.upper())
+                    tmptables = tmptables+re.findall(r'JOIN(.*?)(\S+)',tmpTxt.upper())
+                    tables = list(set(tmptables))
+                    tmpTxt = None
+
+            for tt in range(len(tables)):
+                if tables[tt][1].replace('(','').replace(')','') == '':
+                    pass
+                else:
+                    schema = tables[tt][1].lower().split('.')[0]
+                    tabela = tables[tt][1].lower().split('.')[1]
+                    s.getSpark()
+                    lp = self.getLastPartition(schema,tabela,dPrint = False)
+                    if lp != None:
+                        str_where[tables[tt][1].lower().split('.')[1]] = "" + "'" + lp +"'"
+
+            executionPlan = query.format(**str_where).split(';')
+
+            impala = s.getImpala()
+            for i in range(len(executionPlan)):
+                try:
+                    val = executionPlan[i].replace('\n',' ')
+                    print(f'Executando : {val}')
+                    impala.execute(executionPlan[i])
+                    print(f'-----FINALIZADO -----')
+                except Exception as e:
+                    print(f'-----!!! ERRO !!!-----')
+                    print(e)   
+                    pass
+        
+    except Exception as e:
+        print(e)
             
 # -------------------------------------------------------------------------------------------------------------------------------
 # | CLASS TOOLS
 # -------------------------------------------------------------------------------------------------------------------------------
 
 class tool():
     """
@@ -833,14 +900,40 @@
             por padrão essa data é hoje
         strFormat str
             formatação da tada a ser retornada
             
         """
         return datetime.strptime(strDate, strFormat).date()
     
+    def setNumAnoMes(self,meses = -5,dt_ref = str(date.today()),dm1=True) -> str:
+        """
+        setNumAnoMes(self,meses = -5,dt_ref = str(date.today()),dm1=True)
+        Função que retorna ANOMES (202307) alem de poder mover os meses para frente ou para trás
+        
+        Parameters
+        ----------
+        meses int
+            quantidade de meses a serem movimentados
+        dt_ref str
+            Variavel com a data que deseja deslocar o NUMANOMES
+            por padrão essa data é hoje            
+        """
+        dt_ref = self.dateStringToDate(dt_ref)
+        if meses <0:
+            meses = meses*-1
+            if dm1==True:
+                return (date.today() - relativedelta(months=meses) - relativedelta(day=1)).strftime('%Y%m')
+            else:
+                return (date.today() - relativedelta(months=meses)).strftime('%Y%m')
+        else:
+            if dm1==True:
+                return (date.today() + relativedelta(months=meses) - relativedelta(day=1)).strftime('%Y%m')
+            else:
+                return (date.today() + relativedelta(months=meses)).strftime('%Y%m')
+    
     def dropcol(self,df01,df02):
         """
         DFB = dropcol(df01 = DFA,df02 = DFB)
         Função para igualar as colunas entre 2 dataframes
         excluido as colunas do df02 que existem a mais do que o df01
         
         Parameters
```

### Comparing `dadosSPF-1.0.2/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `dadosSPF-1.0.3/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files identical despite different names*

### Comparing `dadosSPF-1.0.2/dadosSPF.egg-info/PKG-INFO` & `dadosSPF-1.0.3/dadosSPF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dadosSPF
-Version: 1.0.2
+Version: 1.0.3
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.com.br/dadosSPF
 Author: Carlos Piveta
 Author-email: cepo496@gmail.com
 License: MIT License
 Description: # dadosSPF
```

### Comparing `dadosSPF-1.0.2/dadosSPF.egg-info/SOURCES.txt` & `dadosSPF-1.0.3/dadosSPF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dadosSPF-1.0.2/setup.py` & `dadosSPF-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(
     name='dadosSPF',
-    version='1.0.2',
+    version='1.0.3',
     url='https://gitlab.com.br/dadosSPF',
     license='MIT License',
     author='Carlos Piveta',
 	long_description=readme,
     long_description_content_type="text/markdown",
     author_email='cepo496@gmail.com',
     keywords='Pacote',
```

