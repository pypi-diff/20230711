# Comparing `tmp/WqUtils-0.1.4-py3-none-any.whl.zip` & `tmp/WqUtils-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9492 bytes, number of entries: 10
+Zip file size: 9593 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     5333 b- defN 23-Jun-19 08:15 WqUtils/Utils.py
 -rw-r--r--  2.0 unx      334 b- defN 23-Jun-21 05:54 WqUtils/__init__.py
--rw-r--r--  2.0 unx     7635 b- defN 23-Jun-21 05:40 WqUtils/DB_Utils/ExecPgSql.py
+-rw-r--r--  2.0 unx     8390 b- defN 23-Jul-11 06:15 WqUtils/DB_Utils/ExecPgSql.py
 -rw-r--r--  2.0 unx     6557 b- defN 23-Jun-19 16:59 WqUtils/DB_Utils/SqlServer_DB.py
 -rw-r--r--  2.0 unx      267 b- defN 23-Jun-19 06:58 WqUtils/DB_Utils/__init__.py
--rw-r--r--  2.0 unx      457 b- defN 23-Jun-21 02:48 WqUtils/DB_Utils/db_config.toml
--rw-r--r--  2.0 unx      208 b- defN 23-Jun-21 05:55 WqUtils-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 05:55 WqUtils-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-21 05:55 WqUtils-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      790 b- defN 23-Jun-21 05:55 WqUtils-0.1.4.dist-info/RECORD
-10 files, 21681 bytes uncompressed, 8144 bytes compressed:  62.4%
+-rw-r--r--  2.0 unx      435 b- defN 23-Jul-10 12:53 WqUtils/DB_Utils/db_config.toml
+-rw-r--r--  2.0 unx      208 b- defN 23-Jul-11 06:21 WqUtils-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 06:21 WqUtils-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-11 06:21 WqUtils-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      790 b- defN 23-Jul-11 06:21 WqUtils-0.1.5.dist-info/RECORD
+10 files, 22414 bytes uncompressed, 8245 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: WqUtils/DB_Utils/__init__.py
 Comment: 
 
 Filename: WqUtils/DB_Utils/db_config.toml
 Comment: 
 
-Filename: WqUtils-0.1.4.dist-info/METADATA
+Filename: WqUtils-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: WqUtils-0.1.4.dist-info/WHEEL
+Filename: WqUtils-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: WqUtils-0.1.4.dist-info/top_level.txt
+Filename: WqUtils-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: WqUtils-0.1.4.dist-info/RECORD
+Filename: WqUtils-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## WqUtils/DB_Utils/ExecPgSql.py

```diff
@@ -71,14 +71,15 @@
         self.pymssql_config = TomlConfig('db_config.toml').read()
         self.sql_conf = self._get_sql_conf()
         self.host = self.sql_conf['HOST']
         self.port = self.sql_conf['PORT']
         self.user = self.sql_conf['USERNAME']
         self.pwd = self.sql_conf['PASSWORD']
         self.test_db = self.sql_conf['DB']
+        self.options = self.sql_conf['OPTIONS']
 
 
     def load_config(self):
         # 读取环境变量数据库信息如果有|直接使用，如果没有再读取本地配置文件
         if os.getenv("MSSQL_HOST", None):
             config = {"HOST": os.getenv("PG_HOST"), "PORT": int(os.getenv(
                 "PG_PORT")), "USERNAME":
@@ -147,47 +148,56 @@
             self.conn.commit()
             self.cursor.close()
             self.conn.close()
             return result
         except Exception as e:
             print("sql类型或sql错误：{0}".format(e))
 
-    def _create_table(self, table_name=None, fields_lst=None):
-        confirm_fields = " varchar(1000),".join(map(str, fields_lst)).strip(',') + " " \
-                                                                                  "varchar(1000)"
-        confirm_fields = "create_time TIMESTAMP DEFAULT current_timestamp,update_time " \
-                         "TIMESTAMP DEFAULT current_timestamp," + confirm_fields
-        table_template = """create table IF NOT EXISTS {0} ({1});""".format(table_name, confirm_fields)
+    def _create_table(self, table_name=None, fields_lst=None, table_id=None):
+        if table_id:
+            confirm_fields = " varchar,".join(map(str, fields_lst)).strip(',') + " " \
+                                                                                 "varchar"
+            confirm_fields = "t_id integer GENERATED ALWAYS AS IDENTITY PRIMARY KEY," \
+                             "create_time TIMESTAMP DEFAULT current_timestamp," \
+                             "update_time " \
+                             "TIMESTAMP DEFAULT current_timestamp," + confirm_fields
+        else:
+            confirm_fields = " varchar,".join(map(str, fields_lst)).strip(',') + " " \
+                                    "varchar"
+            confirm_fields = "create_time TIMESTAMP DEFAULT current_timestamp,update_time " \
+                             "TIMESTAMP DEFAULT current_timestamp," + confirm_fields
+        table_template = """create table IF NOT EXISTS {0} ({1});""".format(table_name,
+                                                                            confirm_fields)
 
         self.exec_sql("insert", table_template)
 
-    def _df_trans_sql(self, table_name=None, df_data=None):
+    def _df_trans_sql(self, table_name=None, df_data=None, table_id=None):
         df_data = df_data.fillna('')
         columns = df_data.columns.tolist()  # 表字段
         columns = [f'"{i}"' for i in columns]
         values = df_data.values.tolist()  # 表字段对应的值
-        table_name = f'"{self.test_db}".dbo."{table_name}"'
-        self._create_table(table_name, columns)
+        table_name = f'"{self.test_db}".{self.options}."{table_name}"'
+        self._create_table(table_name, columns, table_id)
 
         tmp = []
         for v in values:
             value = [str(s).replace("'", "''") for s in v]
             tmp.append("('" + "','".join(value) + "')")
         SQL = '''INSERT INTO {0}({1}) VALUES {2};'''.format(table_name, ','.join(columns),
                                                             ','.join(tmp))
         SQL = SQL.replace('%', '%%')  # 特殊字符转换
         return SQL
 
-    def _copy_from(self, table_name=None, df_data=None):
+    def _copy_from(self, table_name=None, df_data=None, table_id=None):
         df_data = df_data.fillna('')
         columns = df_data.columns.tolist()  # 表字段
         columns = [f'"{i}"' for i in columns]
         values = df_data.values.tolist()  # 表字段对应的值
-        table_name = f'"{self.test_db}".dbo."{table_name}"'
-        self._create_table(table_name, columns)
+        table_name = f'"{self.test_db}".{self.options}."{table_name}"'
+        self._create_table(table_name, columns, table_id)
         values_column = ['\t'.join(map(str, column)) for column in values]
         values_row = '\n'.join(values_column)
 
         self.connect_db()
         cursor = self.get_cursor()
         try:
             cursor.copy_from(StringIO(values_row), table_name.split('.')[-1].strip('"'),
@@ -197,27 +207,29 @@
         except Exception as e:
             print(e)
             self.conn.rollback()
         finally:
             cursor.close()
             self.conn.close()
 
-    def df_insert(self, table_name=None, df_data=None, batch_size=10000, copy_from=False):
+    def df_insert(self, table_name=None, df_data=None, batch_size=10000,
+                  copy_from=False, id_flag=False):
         total_len = len(df_data)
         epochs = math.ceil(total_len / batch_size)
         for idx in range(epochs):
             batch_df = df_data[idx * batch_size: min((idx + 1) * batch_size, total_len)]
             if copy_from:
-                self._copy_from(table_name, batch_df)
+                self._copy_from(table_name, batch_df, id_flag)
             else:
-                batch_sql = self._df_trans_sql(table_name, batch_df)
+                batch_sql = self._df_trans_sql(table_name, batch_df, id_flag)
                 self.exec_sql("insert", batch_sql)
 
 
 if __name__ == "__main__":
     pass
-    # pg_instance = ExecPgSql()
-    # sql_temp = """select * from category_test0531 limit 10;"""
-    # a = pg_instance.exec_sql("select", sql_temp)
-    #
-    # df1 = pd.read_excel("../../UnitTest/5月份规则接口输出品类检查.xlsx")[:3]
-    # pg_instance.df_insert(table_name="pg_test_wq", df_data=df1, copy_from=False)
+    pg_instance = ExecPgSql()
+    sql_temp = """select * from category_test0531 limit 10;"""
+    a = pg_instance.exec_sql("select", sql_temp)
+
+    df1 = pd.read_excel("../../UnitTest/5月份规则接口输出品类检查.xlsx")[:3]
+    pg_instance.df_insert(table_name="pg_test_wq", df_data=df1, copy_from=False,
+                          id_flag=True)
```

## WqUtils/DB_Utils/db_config.toml

```diff
@@ -13,8 +13,8 @@
 
 [pg_database]
 HOST = "gp-uf6xpccjt4kem37d4o-master.gpdb.rds.aliyuncs.com"
 PORT = "5432"
 USERNAME = "colourdata"
 PASSWORD = "Colourdata110!"
 DB = "CD_Research_DB"
-options = "-c search_path=dbo,public"
+OPTIONS = "dbo"
```

## Comparing `WqUtils-0.1.4.dist-info/RECORD` & `WqUtils-0.1.5.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 WqUtils/Utils.py,sha256=5rCtSyMBSETtUzG1qdK5rBzylKmMFIvq7M2AXhbwubY,5333
 WqUtils/__init__.py,sha256=xjLvC1XO31tSqFeyhyDDWC4_L9pxf0x-1pv2mdcVKek,334
-WqUtils/DB_Utils/ExecPgSql.py,sha256=O80RCop_ck8_0tTCzT2FM1Z3hzcZaqZvCR1DxxvLy1s,7635
+WqUtils/DB_Utils/ExecPgSql.py,sha256=ahHQ91Yt3HPaUL1bi1lnZT4G72vqfCPQ1fLUoUhFLQA,8390
 WqUtils/DB_Utils/SqlServer_DB.py,sha256=QlSCVxMEogmk7STQpCHhiFEI9SFnvCXViMdJ5jdZ5f0,6557
 WqUtils/DB_Utils/__init__.py,sha256=U1spx2Yz0uxJA1A_7-Yb-ZKoy47wJM1VZEuZ4vIB00M,267
-WqUtils/DB_Utils/db_config.toml,sha256=aSE9uvCRtZvIPsCCmJGI-f2dUsrQUmOV-hbGGuCoEJQ,457
-WqUtils-0.1.4.dist-info/METADATA,sha256=et-bVSOhDXROAut5pOtJhZ2FN2W1DWpEy_6PuMkvX04,208
-WqUtils-0.1.4.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-WqUtils-0.1.4.dist-info/top_level.txt,sha256=XpUtbHzxrhqE5cOFUxWQrZAlMz2b2ww_pX2dKJrr9cs,8
-WqUtils-0.1.4.dist-info/RECORD,,
+WqUtils/DB_Utils/db_config.toml,sha256=JFCcA2WrqSQ4f47TIvNVsJA2gJXsElU6-RXXRs77zBY,435
+WqUtils-0.1.5.dist-info/METADATA,sha256=sMAmmjL5mNj40Ipc_2hn5TaRqOAowdmt66zmQxbA4KY,208
+WqUtils-0.1.5.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+WqUtils-0.1.5.dist-info/top_level.txt,sha256=XpUtbHzxrhqE5cOFUxWQrZAlMz2b2ww_pX2dKJrr9cs,8
+WqUtils-0.1.5.dist-info/RECORD,,
```

