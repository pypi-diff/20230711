# Comparing `tmp/PyHive-0.7.0.dev0.tar.gz` & `tmp/PyHive-0.7.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHive-0.7.0.dev0.tar", last modified: Wed May 17 19:03:25 2023, max compression
+gzip compressed data, was "PyHive-0.7.1.dev0.tar", last modified: Tue Jul 11 08:35:28 2023, max compression
```

## Comparing `PyHive-0.7.0.dev0.tar` & `PyHive-0.7.1.dev0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 bogdankyryliuk   (501) staff       (20)        0 2023-05-17 19:03:25.969788 PyHive-0.7.0.dev0/
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      558 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/LICENSE
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)       16 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/MANIFEST.in
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     6474 2023-05-17 19:03:25.969849 PyHive-0.7.0.dev0/PKG-INFO
-drwxr-xr-x   0 bogdankyryliuk   (501) staff       (20)        0 2023-05-17 19:03:25.966211 PyHive-0.7.0.dev0/PyHive.egg-info/
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     6474 2023-05-17 19:03:25.000000 PyHive-0.7.0.dev0/PyHive.egg-info/PKG-INFO
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      508 2023-05-17 19:03:25.000000 PyHive-0.7.0.dev0/PyHive.egg-info/SOURCES.txt
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)        1 2023-05-17 19:03:25.000000 PyHive-0.7.0.dev0/PyHive.egg-info/dependency_links.txt
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      268 2023-05-17 19:03:25.000000 PyHive-0.7.0.dev0/PyHive.egg-info/entry_points.txt
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      198 2023-05-17 19:03:25.000000 PyHive-0.7.0.dev0/PyHive.egg-info/requires.txt
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)       19 2023-05-17 19:03:25.000000 PyHive-0.7.0.dev0/PyHive.egg-info/top_level.txt
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     5915 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/README.rst
-drwxr-xr-x   0 bogdankyryliuk   (501) staff       (20)        0 2023-05-17 19:03:25.967517 PyHive-0.7.0.dev0/TCLIService/
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)   131364 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/TCLIService/TCLIService.py
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)       49 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/TCLIService/__init__.py
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     1087 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/TCLIService/constants.py
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)   263044 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/TCLIService/ttypes.py
-drwxr-xr-x   0 bogdankyryliuk   (501) staff       (20)        0 2023-05-17 19:03:25.969609 PyHive-0.7.0.dev0/pyhive/
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      101 2023-05-17 17:02:25.000000 PyHive-0.7.0.dev0/pyhive/__init__.py
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     9340 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/common.py
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     2196 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/exc.py
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)    22401 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/hive.py
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)    15379 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/presto.py
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)    13017 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/sqlalchemy_hive.py
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     7388 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/sqlalchemy_presto.py
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     1926 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/sqlalchemy_trino.py
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     4833 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/pyhive/trino.py
--rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      881 2023-05-17 19:03:25.970459 PyHive-0.7.0.dev0/setup.cfg
--rwxr-xr-x   0 bogdankyryliuk   (501) staff       (20)     2149 2023-05-17 16:58:56.000000 PyHive-0.7.0.dev0/setup.py
+drwxr-xr-x   0 bogdankyryliuk   (501) staff       (20)        0 2023-07-11 08:35:28.707529 PyHive-0.7.1.dev0/
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      558 2023-05-17 16:58:56.000000 PyHive-0.7.1.dev0/LICENSE
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)       16 2023-05-17 16:58:56.000000 PyHive-0.7.1.dev0/MANIFEST.in
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     7157 2023-07-11 08:35:28.707608 PyHive-0.7.1.dev0/PKG-INFO
+drwxr-xr-x   0 bogdankyryliuk   (501) staff       (20)        0 2023-07-11 08:35:28.703340 PyHive-0.7.1.dev0/PyHive.egg-info/
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     7157 2023-07-11 08:35:28.000000 PyHive-0.7.1.dev0/PyHive.egg-info/PKG-INFO
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      530 2023-07-11 08:35:28.000000 PyHive-0.7.1.dev0/PyHive.egg-info/SOURCES.txt
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)        1 2023-07-11 08:35:28.000000 PyHive-0.7.1.dev0/PyHive.egg-info/dependency_links.txt
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      268 2023-07-11 08:35:28.000000 PyHive-0.7.1.dev0/PyHive.egg-info/entry_points.txt
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      267 2023-07-11 08:35:28.000000 PyHive-0.7.1.dev0/PyHive.egg-info/requires.txt
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)       19 2023-07-11 08:35:28.000000 PyHive-0.7.1.dev0/PyHive.egg-info/top_level.txt
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     6567 2023-07-11 07:29:32.000000 PyHive-0.7.1.dev0/README.rst
+drwxr-xr-x   0 bogdankyryliuk   (501) staff       (20)        0 2023-07-11 08:35:28.704943 PyHive-0.7.1.dev0/TCLIService/
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)   131364 2023-05-17 16:58:56.000000 PyHive-0.7.1.dev0/TCLIService/TCLIService.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)       49 2023-05-17 16:58:56.000000 PyHive-0.7.1.dev0/TCLIService/__init__.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     1087 2023-05-17 16:58:56.000000 PyHive-0.7.1.dev0/TCLIService/constants.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)   263044 2023-05-17 16:58:56.000000 PyHive-0.7.1.dev0/TCLIService/ttypes.py
+drwxr-xr-x   0 bogdankyryliuk   (501) staff       (20)        0 2023-07-11 08:35:28.707283 PyHive-0.7.1.dev0/pyhive/
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      101 2023-07-11 08:34:40.000000 PyHive-0.7.1.dev0/pyhive/__init__.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     9340 2023-05-17 16:58:56.000000 PyHive-0.7.1.dev0/pyhive/common.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     2196 2023-05-17 16:58:56.000000 PyHive-0.7.1.dev0/pyhive/exc.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)    23308 2023-07-06 10:11:55.000000 PyHive-0.7.1.dev0/pyhive/hive.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)    15379 2023-05-17 16:58:56.000000 PyHive-0.7.1.dev0/pyhive/presto.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     1992 2023-07-06 10:11:55.000000 PyHive-0.7.1.dev0/pyhive/sasl_compat.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)    13484 2023-07-11 07:29:33.000000 PyHive-0.7.1.dev0/pyhive/sqlalchemy_hive.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     7939 2023-07-11 07:29:33.000000 PyHive-0.7.1.dev0/pyhive/sqlalchemy_presto.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     2234 2023-07-11 07:29:33.000000 PyHive-0.7.1.dev0/pyhive/sqlalchemy_trino.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)     4833 2023-05-17 16:58:56.000000 PyHive-0.7.1.dev0/pyhive/trino.py
+-rw-r--r--   0 bogdankyryliuk   (501) staff       (20)      881 2023-07-11 08:35:28.707911 PyHive-0.7.1.dev0/setup.cfg
+-rwxr-xr-x   0 bogdankyryliuk   (501) staff       (20)     2292 2023-07-06 10:11:55.000000 PyHive-0.7.1.dev0/setup.py
```

### Comparing `PyHive-0.7.0.dev0/LICENSE` & `PyHive-0.7.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyHive-0.7.0.dev0/PKG-INFO` & `PyHive-0.7.1.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: PyHive
-Version: 0.7.0.dev0
+Version: 0.7.1.dev0
 Summary: Python interface to Hive
 Home-page: https://github.com/dropbox/PyHive
 Author: Jing Wang
 Author-email: jing@dropbox.com
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database :: Front-Ends
 Provides-Extra: presto
 Provides-Extra: trino
 Provides-Extra: hive
+Provides-Extra: hive_pure_sasl
 Provides-Extra: sqlalchemy
 Provides-Extra: kerberos
 License-File: LICENSE
 
 ================================
 Project is currently unsupported
 ================================
@@ -86,25 +87,41 @@
 
     from sqlalchemy import *
     from sqlalchemy.engine import create_engine
     from sqlalchemy.schema import *
     # Presto
     engine = create_engine('presto://localhost:8080/hive/default')
     # Trino
-    engine = create_engine('trino://localhost:8080/hive/default')
+    engine = create_engine('trino+pyhive://localhost:8080/hive/default')
     # Hive
     engine = create_engine('hive://localhost:10000/default')
+
+    # SQLAlchemy < 2.0
     logs = Table('my_awesome_data', MetaData(bind=engine), autoload=True)
     print select([func.count('*')], from_obj=logs).scalar()
 
     # Hive + HTTPS + LDAP or basic Auth
     engine = create_engine('hive+https://username:password@localhost:10000/')
     logs = Table('my_awesome_data', MetaData(bind=engine), autoload=True)
     print select([func.count('*')], from_obj=logs).scalar()
 
+    # SQLAlchemy >= 2.0
+    metadata_obj = MetaData()
+    books = Table("books", metadata_obj, Column("id", Integer), Column("title", String), Column("primary_author", String))
+    metadata_obj.create_all(engine)
+    inspector = inspect(engine)
+    inspector.get_columns('books')
+
+    with engine.connect() as con:
+        data = [{ "id": 1, "title": "The Hobbit", "primary_author": "Tolkien" }, 
+                { "id": 2, "title": "The Silmarillion", "primary_author": "Tolkien" }]
+        con.execute(books.insert(), data[0])
+        result = con.execute(text("select * from books"))
+        print(result.fetchall())
+
 Note: query generation functionality is not exhaustive or fully tested, but there should be no
 problem with raw SQL.
 
 Passing session configuration
 -----------------------------
 
 .. code-block:: python
```

### Comparing `PyHive-0.7.0.dev0/PyHive.egg-info/PKG-INFO` & `PyHive-0.7.1.dev0/PyHive.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: PyHive
-Version: 0.7.0.dev0
+Version: 0.7.1.dev0
 Summary: Python interface to Hive
 Home-page: https://github.com/dropbox/PyHive
 Author: Jing Wang
 Author-email: jing@dropbox.com
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database :: Front-Ends
 Provides-Extra: presto
 Provides-Extra: trino
 Provides-Extra: hive
+Provides-Extra: hive_pure_sasl
 Provides-Extra: sqlalchemy
 Provides-Extra: kerberos
 License-File: LICENSE
 
 ================================
 Project is currently unsupported
 ================================
@@ -86,25 +87,41 @@
 
     from sqlalchemy import *
     from sqlalchemy.engine import create_engine
     from sqlalchemy.schema import *
     # Presto
     engine = create_engine('presto://localhost:8080/hive/default')
     # Trino
-    engine = create_engine('trino://localhost:8080/hive/default')
+    engine = create_engine('trino+pyhive://localhost:8080/hive/default')
     # Hive
     engine = create_engine('hive://localhost:10000/default')
+
+    # SQLAlchemy < 2.0
     logs = Table('my_awesome_data', MetaData(bind=engine), autoload=True)
     print select([func.count('*')], from_obj=logs).scalar()
 
     # Hive + HTTPS + LDAP or basic Auth
     engine = create_engine('hive+https://username:password@localhost:10000/')
     logs = Table('my_awesome_data', MetaData(bind=engine), autoload=True)
     print select([func.count('*')], from_obj=logs).scalar()
 
+    # SQLAlchemy >= 2.0
+    metadata_obj = MetaData()
+    books = Table("books", metadata_obj, Column("id", Integer), Column("title", String), Column("primary_author", String))
+    metadata_obj.create_all(engine)
+    inspector = inspect(engine)
+    inspector.get_columns('books')
+
+    with engine.connect() as con:
+        data = [{ "id": 1, "title": "The Hobbit", "primary_author": "Tolkien" }, 
+                { "id": 2, "title": "The Silmarillion", "primary_author": "Tolkien" }]
+        con.execute(books.insert(), data[0])
+        result = con.execute(text("select * from books"))
+        print(result.fetchall())
+
 Note: query generation functionality is not exhaustive or fully tested, but there should be no
 problem with raw SQL.
 
 Passing session configuration
 -----------------------------
 
 .. code-block:: python
```

### Comparing `PyHive-0.7.0.dev0/README.rst` & `PyHive-0.7.1.dev0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -67,25 +67,41 @@
 
     from sqlalchemy import *
     from sqlalchemy.engine import create_engine
     from sqlalchemy.schema import *
     # Presto
     engine = create_engine('presto://localhost:8080/hive/default')
     # Trino
-    engine = create_engine('trino://localhost:8080/hive/default')
+    engine = create_engine('trino+pyhive://localhost:8080/hive/default')
     # Hive
     engine = create_engine('hive://localhost:10000/default')
+
+    # SQLAlchemy < 2.0
     logs = Table('my_awesome_data', MetaData(bind=engine), autoload=True)
     print select([func.count('*')], from_obj=logs).scalar()
 
     # Hive + HTTPS + LDAP or basic Auth
     engine = create_engine('hive+https://username:password@localhost:10000/')
     logs = Table('my_awesome_data', MetaData(bind=engine), autoload=True)
     print select([func.count('*')], from_obj=logs).scalar()
 
+    # SQLAlchemy >= 2.0
+    metadata_obj = MetaData()
+    books = Table("books", metadata_obj, Column("id", Integer), Column("title", String), Column("primary_author", String))
+    metadata_obj.create_all(engine)
+    inspector = inspect(engine)
+    inspector.get_columns('books')
+
+    with engine.connect() as con:
+        data = [{ "id": 1, "title": "The Hobbit", "primary_author": "Tolkien" }, 
+                { "id": 2, "title": "The Silmarillion", "primary_author": "Tolkien" }]
+        con.execute(books.insert(), data[0])
+        result = con.execute(text("select * from books"))
+        print(result.fetchall())
+
 Note: query generation functionality is not exhaustive or fully tested, but there should be no
 problem with raw SQL.
 
 Passing session configuration
 -----------------------------
 
 .. code-block:: python
```

### Comparing `PyHive-0.7.0.dev0/TCLIService/TCLIService.py` & `PyHive-0.7.1.dev0/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.7.0.dev0/TCLIService/constants.py` & `PyHive-0.7.1.dev0/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.7.0.dev0/TCLIService/ttypes.py` & `PyHive-0.7.1.dev0/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.7.0.dev0/pyhive/common.py` & `PyHive-0.7.1.dev0/pyhive/common.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.7.0.dev0/pyhive/exc.py` & `PyHive-0.7.1.dev0/pyhive/exc.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.7.0.dev0/pyhive/hive.py` & `PyHive-0.7.1.dev0/pyhive/hive.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,53 @@
 ssl_cert_parameter_map = {
     "none": CERT_NONE,
     "optional": CERT_OPTIONAL,
     "required": CERT_REQUIRED,
 }
 
 
+def get_sasl_client(host, sasl_auth, service=None, username=None, password=None):
+    import sasl
+    sasl_client = sasl.Client()
+    sasl_client.setAttr('host', host)
+
+    if sasl_auth == 'GSSAPI':
+        sasl_client.setAttr('service', service)
+    elif sasl_auth == 'PLAIN':
+        sasl_client.setAttr('username', username)
+        sasl_client.setAttr('password', password)
+    else:
+        raise ValueError("sasl_auth only supports GSSAPI and PLAIN")
+
+    sasl_client.init()
+    return sasl_client
+
+
+def get_pure_sasl_client(host, sasl_auth, service=None, username=None, password=None):
+    from pyhive.sasl_compat import PureSASLClient
+
+    if sasl_auth == 'GSSAPI':
+        sasl_kwargs = {'service': service}
+    elif sasl_auth == 'PLAIN':
+        sasl_kwargs = {'username': username, 'password': password}
+    else:
+        raise ValueError("sasl_auth only supports GSSAPI and PLAIN")
+
+    return PureSASLClient(host=host, **sasl_kwargs)
+
+
+def get_installed_sasl(host, sasl_auth, service=None, username=None, password=None):
+    try:
+        return get_sasl_client(host=host, sasl_auth=sasl_auth, service=service, username=username, password=password)
+        # The sasl library is available
+    except ImportError:
+        # Fallback to pure-sasl library
+        return get_pure_sasl_client(host=host, sasl_auth=sasl_auth, service=service, username=username, password=password)
+    
+
 def _parse_timestamp(value):
     if value:
         match = _TIMESTAMP_PATTERN.match(value)
         if match:
             if match.group(2):
                 format = '%Y-%m-%d %H:%M:%S.%f'
                 # use the pattern to truncate the value
@@ -196,39 +235,26 @@
                 auth = 'NONE'
             socket = thrift.transport.TSocket.TSocket(host, port)
             if auth == 'NOSASL':
                 # NOSASL corresponds to hive.server2.authentication=NOSASL in hive-site.xml
                 self._transport = thrift.transport.TTransport.TBufferedTransport(socket)
             elif auth in ('LDAP', 'KERBEROS', 'NONE', 'CUSTOM'):
                 # Defer import so package dependency is optional
-                import sasl
                 import thrift_sasl
 
                 if auth == 'KERBEROS':
                     # KERBEROS mode in hive.server2.authentication is GSSAPI in sasl library
                     sasl_auth = 'GSSAPI'
                 else:
                     sasl_auth = 'PLAIN'
                     if password is None:
                         # Password doesn't matter in NONE mode, just needs to be nonempty.
                         password = 'x'
-
-                def sasl_factory():
-                    sasl_client = sasl.Client()
-                    sasl_client.setAttr('host', host)
-                    if sasl_auth == 'GSSAPI':
-                        sasl_client.setAttr('service', kerberos_service_name)
-                    elif sasl_auth == 'PLAIN':
-                        sasl_client.setAttr('username', username)
-                        sasl_client.setAttr('password', password)
-                    else:
-                        raise AssertionError
-                    sasl_client.init()
-                    return sasl_client
-                self._transport = thrift_sasl.TSaslClientTransport(sasl_factory, sasl_auth, socket)
+                
+                self._transport = thrift_sasl.TSaslClientTransport(lambda: get_installed_sasl(host=host, sasl_auth=sasl_auth, service=kerberos_service_name, username=username, password=password), sasl_auth, socket)
             else:
                 # All HS2 config options:
                 # https://cwiki.apache.org/confluence/display/Hive/Setting+Up+HiveServer2#SettingUpHiveServer2-Configuration
                 # PAM currently left to end user via thrift_transport option.
                 raise NotImplementedError(
                     "Only NONE, NOSASL, LDAP, KERBEROS, CUSTOM "
                     "authentication are supported, got {}".format(auth))
```

### Comparing `PyHive-0.7.0.dev0/pyhive/presto.py` & `PyHive-0.7.1.dev0/pyhive/presto.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.7.0.dev0/pyhive/sqlalchemy_hive.py` & `PyHive-0.7.1.dev0/pyhive/sqlalchemy_hive.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,30 @@
 from __future__ import unicode_literals
 
 import datetime
 import decimal
 
 import re
 from sqlalchemy import exc
-from sqlalchemy import processors
+from sqlalchemy.sql import text
+try:
+    from sqlalchemy import processors
+except ImportError:
+    # Required for SQLAlchemy>=2.0
+    from sqlalchemy.engine import processors
 from sqlalchemy import types
 from sqlalchemy import util
 # TODO shouldn't use mysql type
-from sqlalchemy.databases import mysql
+try:
+    from sqlalchemy.databases import mysql
+    mysql_tinyinteger = mysql.MSTinyInteger
+except ImportError:
+    # Required for SQLAlchemy>2.0
+    from sqlalchemy.dialects import mysql
+    mysql_tinyinteger = mysql.base.MSTinyInteger
 from sqlalchemy.engine import default
 from sqlalchemy.sql import compiler
 from sqlalchemy.sql.compiler import SQLCompiler
 
 from pyhive import hive
 from pyhive.common import UniversalSet
 
@@ -117,15 +128,15 @@
             dialect,
             initial_quote='`',
         )
 
 
 _type_map = {
     'boolean': types.Boolean,
-    'tinyint': mysql.MSTinyInteger,
+    'tinyint': mysql_tinyinteger,
     'smallint': types.SmallInteger,
     'int': types.Integer,
     'bigint': types.BigInteger,
     'float': types.Float,
     'double': types.Float,
     'string': types.String,
     'varchar': types.String,
@@ -243,48 +254,53 @@
     supports_unicode_statements = True
     supports_unicode_binds = True
     returns_unicode_strings = True
     description_encoding = None
     supports_multivalues_insert = True
     type_compiler = HiveTypeCompiler
     supports_sane_rowcount = False
+    supports_statement_cache = False
 
     @classmethod
     def dbapi(cls):
         return hive
+    
+    @classmethod
+    def import_dbapi(cls):
+        return hive
 
     def create_connect_args(self, url):
         kwargs = {
             'host': url.host,
             'port': url.port or 10000,
             'username': url.username,
             'password': url.password,
             'database': url.database or 'default',
         }
         kwargs.update(url.query)
         return [], kwargs
 
     def get_schema_names(self, connection, **kw):
         # Equivalent to SHOW DATABASES
-        return [row[0] for row in connection.execute('SHOW SCHEMAS')]
+        return [row[0] for row in connection.execute(text('SHOW SCHEMAS'))]
 
     def get_view_names(self, connection, schema=None, **kw):
         # Hive does not provide functionality to query tableType
         # This allows reflection to not crash at the cost of being inaccurate
         return self.get_table_names(connection, schema, **kw)
 
     def _get_table_columns(self, connection, table_name, schema):
         full_table = table_name
         if schema:
             full_table = schema + '.' + table_name
         # TODO using TGetColumnsReq hangs after sending TFetchResultsReq.
         # Using DESCRIBE works but is uglier.
         try:
             # This needs the table name to be unescaped (no backticks).
-            rows = connection.execute('DESCRIBE {}'.format(full_table)).fetchall()
+            rows = connection.execute(text('DESCRIBE {}'.format(full_table))).fetchall()
         except exc.OperationalError as e:
             # Does the table exist?
             regex_fmt = r'TExecuteStatementResp.*SemanticException.*Table not found {}'
             regex = regex_fmt.format(re.escape(full_table))
             if re.search(regex, e.args[0]):
                 raise exc.NoSuchTableError(full_table)
             else:
@@ -292,15 +308,15 @@
         else:
             # Hive is stupid: this is what I get from DESCRIBE some_schema.does_not_exist
             regex = r'Table .* does not exist'
             if len(rows) == 1 and re.match(regex, rows[0].col_name):
                 raise exc.NoSuchTableError(full_table)
             return rows
 
-    def has_table(self, connection, table_name, schema=None):
+    def has_table(self, connection, table_name, schema=None, **kw):
         try:
             self._get_table_columns(connection, table_name, schema)
             return True
         except exc.NoSuchTableError:
             return False
 
     def get_columns(self, connection, table_name, schema=None, **kw):
@@ -357,15 +373,15 @@
         else:
             return []
 
     def get_table_names(self, connection, schema=None, **kw):
         query = 'SHOW TABLES'
         if schema:
             query += ' IN ' + self.identifier_preparer.quote_identifier(schema)
-        return [row[0] for row in connection.execute(query)]
+        return [row[0] for row in connection.execute(text(query))]
 
     def do_rollback(self, dbapi_connection):
         # No transactions for Hive
         pass
 
     def _check_unicode_returns(self, connection, additional_tests=None):
         # We decode everything as UTF-8
```

### Comparing `PyHive-0.7.0.dev0/pyhive/sqlalchemy_presto.py` & `PyHive-0.7.1.dev0/pyhive/sqlalchemy_presto.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,35 +5,44 @@
 which is released under the MIT license.
 """
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
 
 import re
+import sqlalchemy
 from sqlalchemy import exc
 from sqlalchemy import types
 from sqlalchemy import util
 # TODO shouldn't use mysql type
-from sqlalchemy.databases import mysql
+from sqlalchemy.sql import text
+try:
+    from sqlalchemy.databases import mysql
+    mysql_tinyinteger = mysql.MSTinyInteger
+except ImportError:
+    # Required for SQLAlchemy>=2.0
+    from sqlalchemy.dialects import mysql
+    mysql_tinyinteger = mysql.base.MSTinyInteger
 from sqlalchemy.engine import default
 from sqlalchemy.sql import compiler
 from sqlalchemy.sql.compiler import SQLCompiler
 
 from pyhive import presto
 from pyhive.common import UniversalSet
 
+sqlalchemy_version = float(re.search(r"^([\d]+\.[\d]+)\..+", sqlalchemy.__version__).group(1))
 
 class PrestoIdentifierPreparer(compiler.IdentifierPreparer):
     # Just quote everything to make things simpler / easier to upgrade
     reserved_words = UniversalSet()
 
 
 _type_map = {
     'boolean': types.Boolean,
-    'tinyint': mysql.MSTinyInteger,
+    'tinyint': mysql_tinyinteger,
     'smallint': types.SmallInteger,
     'integer': types.Integer,
     'bigint': types.BigInteger,
     'real': types.Float,
     'double': types.Float,
     'varchar': types.String,
     'timestamp': types.TIMESTAMP,
@@ -76,22 +85,27 @@
     supports_alter = False
     supports_pk_autoincrement = False
     supports_default_values = False
     supports_empty_insert = False
     supports_multivalues_insert = True
     supports_unicode_statements = True
     supports_unicode_binds = True
+    supports_statement_cache = False
     returns_unicode_strings = True
     description_encoding = None
     supports_native_boolean = True
     type_compiler = PrestoTypeCompiler
 
     @classmethod
     def dbapi(cls):
         return presto
+    
+    @classmethod
+    def import_dbapi(cls):
+        return presto
 
     def create_connect_args(self, url):
         db_parts = (url.database or 'hive').split('/')
         kwargs = {
             'host': url.host,
             'port': url.port or 8080,
             'username': url.username,
@@ -104,22 +118,22 @@
             kwargs['catalog'] = db_parts[0]
             kwargs['schema'] = db_parts[1]
         else:
             raise ValueError("Unexpected database format {}".format(url.database))
         return [], kwargs
 
     def get_schema_names(self, connection, **kw):
-        return [row.Schema for row in connection.execute('SHOW SCHEMAS')]
+        return [row.Schema for row in connection.execute(text('SHOW SCHEMAS'))]
 
     def _get_table_columns(self, connection, table_name, schema):
         full_table = self.identifier_preparer.quote_identifier(table_name)
         if schema:
             full_table = self.identifier_preparer.quote_identifier(schema) + '.' + full_table
         try:
-            return connection.execute('SHOW COLUMNS FROM {}'.format(full_table))
+            return connection.execute(text('SHOW COLUMNS FROM {}'.format(full_table)))
         except (presto.DatabaseError, exc.DatabaseError) as e:
             # Normally SQLAlchemy should wrap this exception in sqlalchemy.exc.DatabaseError, which
             # it successfully does in the Hive version. The difference with Presto is that this
             # error is raised when fetching the cursor's description rather than the initial execute
             # call. SQLAlchemy doesn't handle this. Thus, we catch the unwrapped
             # presto.DatabaseError here.
             # Does the table exist?
@@ -130,15 +144,15 @@
             )
             regex = r"Table\ \'.*{}\'\ does\ not\ exist".format(re.escape(table_name))
             if msg and re.search(regex, msg):
                 raise exc.NoSuchTableError(table_name)
             else:
                 raise
 
-    def has_table(self, connection, table_name, schema=None):
+    def has_table(self, connection, table_name, schema=None, **kw):
         try:
             self._get_table_columns(connection, table_name, schema)
             return True
         except exc.NoSuchTableError:
             return False
 
     def get_columns(self, connection, table_name, schema=None, **kw):
@@ -172,14 +186,16 @@
         col_names = []
         for row in rows:
             part_key = 'Partition Key'
             # Presto puts this information in one of 3 places depending on version
             # - a boolean column named "Partition Key"
             # - a string in the "Comment" column
             # - a string in the "Extra" column
+            if sqlalchemy_version >= 1.4:
+                row = row._mapping
             is_partition_key = (
                 (part_key in row and row[part_key])
                 or row['Comment'].startswith(part_key)
                 or ('Extra' in row and 'partition key' in row['Extra'])
             )
             if is_partition_key:
                 col_names.append(row['Column'])
@@ -188,15 +204,15 @@
         else:
             return []
 
     def get_table_names(self, connection, schema=None, **kw):
         query = 'SHOW TABLES'
         if schema:
             query += ' FROM ' + self.identifier_preparer.quote_identifier(schema)
-        return [row.Table for row in connection.execute(query)]
+        return [row.Table for row in connection.execute(text(query))]
 
     def do_rollback(self, dbapi_connection):
         # No transactions for Presto
         pass
 
     def _check_unicode_returns(self, connection, additional_tests=None):
         # requests gives back Unicode strings
```

### Comparing `PyHive-0.7.0.dev0/pyhive/sqlalchemy_trino.py` & `PyHive-0.7.1.dev0/pyhive/sqlalchemy_trino.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,30 +9,36 @@
 from __future__ import unicode_literals
 
 import re
 from sqlalchemy import exc
 from sqlalchemy import types
 from sqlalchemy import util
 # TODO shouldn't use mysql type
-from sqlalchemy.databases import mysql
+try:
+    from sqlalchemy.databases import mysql
+    mysql_tinyinteger = mysql.MSTinyInteger
+except ImportError:
+    # Required for SQLAlchemy>=2.0
+    from sqlalchemy.dialects import mysql
+    mysql_tinyinteger = mysql.base.MSTinyInteger
 from sqlalchemy.engine import default
 from sqlalchemy.sql import compiler
 from sqlalchemy.sql.compiler import SQLCompiler
 
 from pyhive import trino
 from pyhive.common import UniversalSet
 from pyhive.sqlalchemy_presto import PrestoDialect, PrestoCompiler, PrestoIdentifierPreparer
 
 class TrinoIdentifierPreparer(PrestoIdentifierPreparer):
     pass
 
 
 _type_map = {
     'boolean': types.Boolean,
-    'tinyint': mysql.MSTinyInteger,
+    'tinyint': mysql_tinyinteger,
     'smallint': types.SmallInteger,
     'integer': types.Integer,
     'bigint': types.BigInteger,
     'real': types.Float,
     'double': types.Float,
     'varchar': types.String,
     'timestamp': types.TIMESTAMP,
@@ -63,11 +69,16 @@
             return 'VARCHAR({:d})'.format(type_.length)
         else:
             return 'VARCHAR'
 
 
 class TrinoDialect(PrestoDialect):
     name = 'trino'
+    supports_statement_cache = False
 
     @classmethod
     def dbapi(cls):
         return trino
+    
+    @classmethod
+    def import_dbapi(cls):
+        return trino
```

### Comparing `PyHive-0.7.0.dev0/pyhive/trino.py` & `PyHive-0.7.1.dev0/pyhive/trino.py`

 * *Files identical despite different names*

### Comparing `PyHive-0.7.0.dev0/setup.cfg` & `PyHive-0.7.1.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyHive-0.7.0.dev0/setup.py` & `PyHive-0.7.1.dev0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,24 +42,27 @@
         'future',
         'python-dateutil',
     ],
     extras_require={
         'presto': ['requests>=1.0.0'],
         'trino': ['requests>=1.0.0'],
         'hive': ['sasl>=0.2.1', 'thrift>=0.10.0', 'thrift_sasl>=0.1.0'],
+        'hive_pure_sasl': ['pure-sasl>=0.6.2', 'thrift>=0.10.0', 'thrift_sasl>=0.1.0'],
         'sqlalchemy': ['sqlalchemy>=1.3.0'],
         'kerberos': ['requests_kerberos>=0.12.0'],
     },
     tests_require=[
         'mock>=1.0.0',
         'pytest',
         'pytest-cov',
         'requests>=1.0.0',
         'requests_kerberos>=0.12.0',
         'sasl>=0.2.1',
+        'pure-sasl>=0.6.2',
+        'kerberos>=1.3.0',
         'sqlalchemy>=1.3.0',
         'thrift>=0.10.0',
     ],
     cmdclass={'test': PyTest},
     package_data={
         '': ['*.rst'],
     },
```

