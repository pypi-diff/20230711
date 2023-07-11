# Comparing `tmp/dbbkp-0.1.8.tar.gz` & `tmp/dbbkp-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbbkp-0.1.8.tar", last modified: Wed Dec 21 21:55:38 2022, max compression
+gzip compressed data, was "dbbkp-0.1.9.tar", last modified: Sat Dec 31 06:54:40 2022, max compression
```

## Comparing `dbbkp-0.1.8.tar` & `dbbkp-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 un5       (1000) un5       (1000)        0 2022-12-21 21:55:38.488948 dbbkp-0.1.8/
--rw-rw-r--   0 un5       (1000) un5       (1000)      136 2022-12-21 21:55:38.488948 dbbkp-0.1.8/PKG-INFO
-drwxrwxr-x   0 un5       (1000) un5       (1000)        0 2022-12-21 21:55:38.484948 dbbkp-0.1.8/dbbkp/
--rwxrwxr-x   0 un5       (1000) un5       (1000)      116 2022-12-11 01:11:57.000000 dbbkp-0.1.8/dbbkp/__init__.py
--rwxrwxr-x   0 un5       (1000) un5       (1000)       56 2022-12-11 01:07:49.000000 dbbkp-0.1.8/dbbkp/array.py
-drwxrwxr-x   0 un5       (1000) un5       (1000)        0 2022-12-21 21:55:38.488948 dbbkp-0.1.8/dbbkp/engines/
--rw-rw-r--   0 un5       (1000) un5       (1000)        0 2022-12-11 01:59:22.000000 dbbkp-0.1.8/dbbkp/engines/__init__.py
--rw-rw-r--   0 un5       (1000) un5       (1000)        0 2022-12-21 20:52:40.000000 dbbkp-0.1.8/dbbkp/engines/dsDefault.py
--rw-rw-r--   0 un5       (1000) un5       (1000)     1280 2022-12-11 01:07:49.000000 dbbkp-0.1.8/dbbkp/engines/formatter.py
--rw-rw-r--   0 un5       (1000) un5       (1000)     1485 2022-12-21 21:49:08.000000 dbbkp-0.1.8/dbbkp/engines/fsDefault.py
--rw-rw-r--   0 un5       (1000) un5       (1000)     1680 2022-12-20 19:03:41.000000 dbbkp-0.1.8/dbbkp/engines/mongoDocker.py
--rw-rw-r--   0 un5       (1000) un5       (1000)     2808 2022-12-11 02:06:18.000000 dbbkp-0.1.8/dbbkp/engines/mysqlDefault.py
--rw-rw-r--   0 un5       (1000) un5       (1000)     1792 2022-12-11 05:14:43.000000 dbbkp-0.1.8/dbbkp/engines/mysqlDocker.py
--rwxrwxr-x   0 un5       (1000) un5       (1000)     1991 2022-12-21 21:48:33.000000 dbbkp-0.1.8/dbbkp/engines/scripts.py
--rwxrwxr-x   0 un5       (1000) un5       (1000)     1078 2022-12-21 21:01:43.000000 dbbkp-0.1.8/dbbkp/main.py
-drwxrwxr-x   0 un5       (1000) un5       (1000)        0 2022-12-21 21:55:38.488948 dbbkp-0.1.8/dbbkp.egg-info/
--rw-rw-r--   0 un5       (1000) un5       (1000)      136 2022-12-21 21:55:38.000000 dbbkp-0.1.8/dbbkp.egg-info/PKG-INFO
--rw-rw-r--   0 un5       (1000) un5       (1000)      457 2022-12-21 21:55:38.000000 dbbkp-0.1.8/dbbkp.egg-info/SOURCES.txt
--rw-rw-r--   0 un5       (1000) un5       (1000)        1 2022-12-21 21:55:38.000000 dbbkp-0.1.8/dbbkp.egg-info/dependency_links.txt
--rw-rw-r--   0 un5       (1000) un5       (1000)        1 2022-12-11 04:57:22.000000 dbbkp-0.1.8/dbbkp.egg-info/not-zip-safe
--rw-rw-r--   0 un5       (1000) un5       (1000)       45 2022-12-21 21:55:38.000000 dbbkp-0.1.8/dbbkp.egg-info/requires.txt
--rw-rw-r--   0 un5       (1000) un5       (1000)       20 2022-12-21 21:55:38.000000 dbbkp-0.1.8/dbbkp.egg-info/top_level.txt
--rwxrwxr-x   0 un5       (1000) un5       (1000)       79 2022-12-21 21:55:38.488948 dbbkp-0.1.8/setup.cfg
--rwxrwxr-x   0 un5       (1000) un5       (1000)      290 2022-12-21 21:55:31.000000 dbbkp-0.1.8/setup.py
+drwxrwxr-x   0 un5       (1000) un5       (1000)        0 2022-12-31 06:54:40.718770 dbbkp-0.1.9/
+-rw-rw-r--   0 un5       (1000) un5       (1000)      136 2022-12-31 06:54:40.718770 dbbkp-0.1.9/PKG-INFO
+drwxrwxr-x   0 un5       (1000) un5       (1000)        0 2022-12-31 06:54:40.714770 dbbkp-0.1.9/dbbkp/
+-rwxrwxr-x   0 un5       (1000) un5       (1000)      116 2022-12-11 01:11:57.000000 dbbkp-0.1.9/dbbkp/__init__.py
+-rwxrwxr-x   0 un5       (1000) un5       (1000)       56 2022-12-11 01:07:49.000000 dbbkp-0.1.9/dbbkp/array.py
+drwxrwxr-x   0 un5       (1000) un5       (1000)        0 2022-12-31 06:54:40.718770 dbbkp-0.1.9/dbbkp/engines/
+-rw-rw-r--   0 un5       (1000) un5       (1000)        0 2022-12-11 01:59:22.000000 dbbkp-0.1.9/dbbkp/engines/__init__.py
+-rw-rw-r--   0 un5       (1000) un5       (1000)     2477 2022-12-31 06:54:11.000000 dbbkp-0.1.9/dbbkp/engines/dsDefault.py
+-rw-rw-r--   0 un5       (1000) un5       (1000)     1280 2022-12-11 01:07:49.000000 dbbkp-0.1.9/dbbkp/engines/formatter.py
+-rw-rw-r--   0 un5       (1000) un5       (1000)     1485 2022-12-21 21:49:08.000000 dbbkp-0.1.9/dbbkp/engines/fsDefault.py
+-rw-rw-r--   0 un5       (1000) un5       (1000)     1680 2022-12-20 19:03:41.000000 dbbkp-0.1.9/dbbkp/engines/mongoDocker.py
+-rw-rw-r--   0 un5       (1000) un5       (1000)     2808 2022-12-11 02:06:18.000000 dbbkp-0.1.9/dbbkp/engines/mysqlDefault.py
+-rw-rw-r--   0 un5       (1000) un5       (1000)     1792 2022-12-11 05:14:43.000000 dbbkp-0.1.9/dbbkp/engines/mysqlDocker.py
+-rwxrwxr-x   0 un5       (1000) un5       (1000)     2357 2022-12-31 05:52:44.000000 dbbkp-0.1.9/dbbkp/engines/scripts.py
+-rw-rw-r--   0 un5       (1000) un5       (1000)      746 2022-12-31 03:31:29.000000 dbbkp-0.1.9/dbbkp/engines/svrDefault.py
+-rwxrwxr-x   0 un5       (1000) un5       (1000)     1187 2022-12-31 03:23:29.000000 dbbkp-0.1.9/dbbkp/main.py
+drwxrwxr-x   0 un5       (1000) un5       (1000)        0 2022-12-31 06:54:40.714770 dbbkp-0.1.9/dbbkp.egg-info/
+-rw-rw-r--   0 un5       (1000) un5       (1000)      136 2022-12-31 06:54:40.000000 dbbkp-0.1.9/dbbkp.egg-info/PKG-INFO
+-rw-rw-r--   0 un5       (1000) un5       (1000)      485 2022-12-31 06:54:40.000000 dbbkp-0.1.9/dbbkp.egg-info/SOURCES.txt
+-rw-rw-r--   0 un5       (1000) un5       (1000)        1 2022-12-31 06:54:40.000000 dbbkp-0.1.9/dbbkp.egg-info/dependency_links.txt
+-rw-rw-r--   0 un5       (1000) un5       (1000)        1 2022-12-11 04:57:22.000000 dbbkp-0.1.9/dbbkp.egg-info/not-zip-safe
+-rw-rw-r--   0 un5       (1000) un5       (1000)       45 2022-12-31 06:54:40.000000 dbbkp-0.1.9/dbbkp.egg-info/requires.txt
+-rw-rw-r--   0 un5       (1000) un5       (1000)       20 2022-12-31 06:54:40.000000 dbbkp-0.1.9/dbbkp.egg-info/top_level.txt
+-rwxrwxr-x   0 un5       (1000) un5       (1000)       79 2022-12-31 06:54:40.718770 dbbkp-0.1.9/setup.cfg
+-rwxrwxr-x   0 un5       (1000) un5       (1000)      290 2022-12-31 05:31:59.000000 dbbkp-0.1.9/setup.py
```

### Comparing `dbbkp-0.1.8/dbbkp/engines/formatter.py` & `dbbkp-0.1.9/dbbkp/engines/formatter.py`

 * *Files identical despite different names*

### Comparing `dbbkp-0.1.8/dbbkp/engines/fsDefault.py` & `dbbkp-0.1.9/dbbkp/engines/fsDefault.py`

 * *Files identical despite different names*

### Comparing `dbbkp-0.1.8/dbbkp/engines/mongoDocker.py` & `dbbkp-0.1.9/dbbkp/engines/mongoDocker.py`

 * *Files identical despite different names*

### Comparing `dbbkp-0.1.8/dbbkp/engines/mysqlDefault.py` & `dbbkp-0.1.9/dbbkp/engines/mysqlDefault.py`

 * *Files identical despite different names*

### Comparing `dbbkp-0.1.8/dbbkp/engines/mysqlDocker.py` & `dbbkp-0.1.9/dbbkp/engines/mysqlDocker.py`

 * *Files identical despite different names*

### Comparing `dbbkp-0.1.8/dbbkp/engines/scripts.py` & `dbbkp-0.1.9/dbbkp/engines/scripts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 ################################################ -------------------------------################################################
-# [1/2] MySQL
+# [1/4] MySQL
 
 
 def showDatabases():
     return '''sudo mysql -u root -e 'show databases';'''
 
 
 def exportDatabase(dbName, dbPath):
@@ -26,15 +26,15 @@
     PASSWORD_PATH='{passwordFilePath}'
     PASSWORD=`cat $PASSWORD_PATH`
     docker exec {containerName} /usr/bin/mysqldump -u root --password=$PASSWORD {databaseName} > {outputPath} --skip-dump-date --extended-insert=FALSE;
     '''
 
 
 ################################################ -------------------------------################################################
-# [2/2] MongoDb
+# [2/4] MongoDb
 
 def createMongoDbBackup(containerName):
     return f'''
     docker exec {containerName} sh -c 'mongodump -o /backup'
     '''
 
 
@@ -47,19 +47,33 @@
 def copyMongoDbBackupFiles(containerName, repoPath):
     return f'''
     docker cp {containerName}:/backup/ {os.path.join(repoPath, 'dump')}
     '''
 
 
 ################################################ -------------------------------################################################
-# [3/3] Fs
+# [3/4] Fs
 
 def removeFsBackupFiles(repoPath):
     return f'''
     rm -rf {os.path.join(repoPath, 'dump')}
     '''
 
 
 def copyFsBackupFiles(srcPath, repoPath):
     return f'''
     cp -r {srcPath} {os.path.join(repoPath, 'dump')}
     '''
+
+################################################ -------------------------------################################################
+# [4/4] DS
+
+def removeDsBackupFiles(repoPath):
+    return f'''
+    rm -rf {os.path.join(repoPath, 'dump')}
+    '''
+
+
+def copyDsBackupFiles(srcPath, repoPath):
+    return f'''
+    cp -r {srcPath} {os.path.join(repoPath, 'dump')}
+    '''
```

### Comparing `dbbkp-0.1.8/dbbkp/main.py` & `dbbkp-0.1.9/dbbkp/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .engines import mysqlDefault
 from .engines import mysqlDocker
 from .engines import mongoDocker
 from .engines import fsDefault
 from .engines import dsDefault
+from .engines import svrDefault
 # Entry Function
 
 
 def start(config):
     DB_ENGINE = config.DB_ENGINE
     MsqModule = ''
 
@@ -16,14 +17,16 @@
         MsqModule = mysqlDocker
     elif (DB_ENGINE == 'mongoDocker'):
         MsqModule = mongoDocker
     elif (DB_ENGINE == 'fsDefault'):
         MsqModule = fsDefault
     elif (DB_ENGINE == 'dsDefault'):
         MsqModule = dsDefault
+    elif (DB_ENGINE == 'svrDefault'):
+        MsqModule = svrDefault        
     else:
         MsqModule = mysqlDefault
 
     MsqModule.start(config)
 
 
 # Example Call Below ***-----------***-----------***-----------***-----------***
```

