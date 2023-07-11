# Comparing `tmp/cloud-sql-python-connector-1.2.4.tar.gz` & `tmp/cloud-sql-python-connector-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-sql-python-connector-1.2.4.tar", last modified: Tue Jun 13 15:54:32 2023, max compression
+gzip compressed data, was "cloud-sql-python-connector-1.3.0.tar", last modified: Tue Jul 11 16:16:41 2023, max compression
```

## Comparing `cloud-sql-python-connector-1.2.4.tar` & `cloud-sql-python-connector-1.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:54:32.378790 cloud-sql-python-connector-1.2.4/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/LICENSE
--rw-r--r--   0 root         (0)     1003    22470 2023-06-13 15:54:32.382790 cloud-sql-python-connector-1.2.4/PKG-INFO
--rw-rw-r--   0 root         (0)     1003    21323 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/README.md
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:54:32.378790 cloud-sql-python-connector-1.2.4/cloud_sql_python_connector.egg-info/
--rw-r--r--   0 root         (0)     1003    22470 2023-06-13 15:54:32.000000 cloud-sql-python-connector-1.2.4/cloud_sql_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      935 2023-06-13 15:54:32.000000 cloud-sql-python-connector-1.2.4/cloud_sql_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-13 15:54:32.000000 cloud-sql-python-connector-1.2.4/cloud_sql_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-06-13 15:54:32.000000 cloud-sql-python-connector-1.2.4/cloud_sql_python_connector.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-13 15:54:32.000000 cloud-sql-python-connector-1.2.4/cloud_sql_python_connector.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      156 2023-06-13 15:54:32.000000 cloud-sql-python-connector-1.2.4/cloud_sql_python_connector.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-13 15:54:32.000000 cloud-sql-python-connector-1.2.4/cloud_sql_python_connector.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:54:32.378790 cloud-sql-python-connector-1.2.4/google/
--rw-rw-r--   0 root         (0)     1003      746 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:54:32.378790 cloud-sql-python-connector-1.2.4/google/cloud/
--rw-rw-r--   0 root         (0)     1003      746 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:54:32.378790 cloud-sql-python-connector-1.2.4/google/cloud/sql/
--rw-rw-r--   0 root         (0)     1003        0 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/google/cloud/sql/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:54:32.378790 cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/
--rw-rw-r--   0 root         (0)     1003      876 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/__init__.py
--rw-rw-r--   0 root         (0)     1003     1838 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/asyncpg.py
--rwxrwxr-x   0 root         (0)     1003    13327 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/connector.py
--rw-rw-r--   0 root         (0)     1003     1454 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/exceptions.py
--rw-rw-r--   0 root         (0)     1003    17690 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/instance.py
--rw-rw-r--   0 root         (0)     1003     2031 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/pg8000.py
--rw-rw-r--   0 root         (0)     1003     2105 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/pymysql.py
--rw-rw-r--   0 root         (0)     1003     2452 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/pytds.py
--rw-rw-r--   0 root         (0)     1003     2954 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/rate_limiter.py
--rw-rw-r--   0 root         (0)     1003     9383 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/refresh_utils.py
--rwxrwxr-x   0 root         (0)     1003     4371 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/utils.py
--rw-rw-r--   0 root         (0)     1003      597 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/version.py
--rw-rw-r--   0 root         (0)     1003       67 2023-06-13 15:54:32.382790 cloud-sql-python-connector-1.2.4/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2871 2023-06-13 15:52:01.000000 cloud-sql-python-connector-1.2.4/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 16:16:41.591254 cloud-sql-python-connector-1.3.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/LICENSE
+-rw-r--r--   0 root         (0)     1003    23813 2023-07-11 16:16:41.591254 cloud-sql-python-connector-1.3.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003    22716 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/README.md
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 16:16:41.587253 cloud-sql-python-connector-1.3.0/cloud_sql_python_connector.egg-info/
+-rw-r--r--   0 root         (0)     1003    23813 2023-07-11 16:16:41.000000 cloud-sql-python-connector-1.3.0/cloud_sql_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      935 2023-07-11 16:16:41.000000 cloud-sql-python-connector-1.3.0/cloud_sql_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-11 16:16:41.000000 cloud-sql-python-connector-1.3.0/cloud_sql_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-11 16:16:41.000000 cloud-sql-python-connector-1.3.0/cloud_sql_python_connector.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-11 16:16:41.000000 cloud-sql-python-connector-1.3.0/cloud_sql_python_connector.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      156 2023-07-11 16:16:41.000000 cloud-sql-python-connector-1.3.0/cloud_sql_python_connector.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-11 16:16:41.000000 cloud-sql-python-connector-1.3.0/cloud_sql_python_connector.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 16:16:41.587253 cloud-sql-python-connector-1.3.0/google/
+-rw-rw-r--   0 root         (0)     1003      746 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 16:16:41.587253 cloud-sql-python-connector-1.3.0/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      746 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 16:16:41.587253 cloud-sql-python-connector-1.3.0/google/cloud/sql/
+-rw-rw-r--   0 root         (0)     1003        0 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/google/cloud/sql/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 16:16:41.591254 cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/
+-rw-rw-r--   0 root         (0)     1003      876 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1838 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/asyncpg.py
+-rwxrwxr-x   0 root         (0)     1003    14195 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/connector.py
+-rw-rw-r--   0 root         (0)     1003     1649 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/exceptions.py
+-rw-rw-r--   0 root         (0)     1003    17711 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/instance.py
+-rw-rw-r--   0 root         (0)     1003     2031 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/pg8000.py
+-rw-rw-r--   0 root         (0)     1003     2105 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/pymysql.py
+-rw-rw-r--   0 root         (0)     1003     2452 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/pytds.py
+-rw-rw-r--   0 root         (0)     1003     2954 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/rate_limiter.py
+-rw-rw-r--   0 root         (0)     1003     9565 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/refresh_utils.py
+-rwxrwxr-x   0 root         (0)     1003     4371 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/utils.py
+-rw-rw-r--   0 root         (0)     1003      597 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/version.py
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-11 16:16:41.591254 cloud-sql-python-connector-1.3.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2822 2023-07-11 16:14:01.000000 cloud-sql-python-connector-1.3.0/setup.py
```

### Comparing `cloud-sql-python-connector-1.2.4/LICENSE` & `cloud-sql-python-connector-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.4/PKG-INFO` & `cloud-sql-python-connector-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 636c 6f75  : 2.1.Name: clou
 00000020: 642d 7371 6c2d 7079 7468 6f6e 2d63 6f6e  d-sql-python-con
 00000030: 6e65 6374 6f72 0a56 6572 7369 6f6e 3a20  nector.Version: 
-00000040: 312e 322e 340a 5375 6d6d 6172 793a 2054  1.2.4.Summary: T
+00000040: 312e 332e 300a 5375 6d6d 6172 793a 2054  1.3.0.Summary: T
 00000050: 6865 2043 6c6f 7564 2053 514c 2050 7974  he Cloud SQL Pyt
 00000060: 686f 6e20 436f 6e6e 6563 746f 7220 6973  hon Connector is
 00000070: 2061 206c 6962 7261 7279 2074 6861 7420   a library that 
 00000080: 6361 6e20 6265 2075 7365 6420 616c 6f6e  can be used alon
 00000090: 6773 6964 6520 6120 6461 7461 6261 7365  gside a database
 000000a0: 2064 7269 7665 7220 746f 2061 6c6c 6f77   driver to allow
 000000b0: 2075 7365 7273 2077 6974 6820 7375 6666   users with suff
@@ -41,1365 +41,1449 @@
 00000280: 726f 7665 6420 3a3a 2041 7061 6368 6520  roved :: Apache 
 00000290: 536f 6674 7761 7265 204c 6963 656e 7365  Software License
 000002a0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
 000002b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 000002c0: 6520 3a3a 2050 7974 686f 6e0a 436c 6173  e :: Python.Clas
 000002d0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
 000002e0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000002f0: 5079 7468 6f6e 203a 3a20 332e 370a 436c  Python :: 3.7.Cl
+000002f0: 5079 7468 6f6e 203a 3a20 332e 380a 436c  Python :: 3.8.Cl
 00000300: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
 00000310: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000320: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
+00000320: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
 00000330: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
 00000340: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 00000350: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000360: 390a 436c 6173 7369 6669 6572 3a20 5072  9.Classifier: Pr
-00000370: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000380: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000390: 332e 3130 0a43 6c61 7373 6966 6965 723a  3.10.Classifier:
-000003a0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000003b0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000003c0: 3a3a 2033 2e31 310a 5265 7175 6972 6573  :: 3.11.Requires
-000003d0: 2d50 7974 686f 6e3a 203e 3d33 2e37 0a44  -Python: >=3.7.D
-000003e0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-000003f0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-00000400: 726b 646f 776e 0a50 726f 7669 6465 732d  rkdown.Provides-
-00000410: 4578 7472 613a 2070 796d 7973 716c 0a50  Extra: pymysql.P
-00000420: 726f 7669 6465 732d 4578 7472 613a 2070  rovides-Extra: p
-00000430: 6738 3030 300a 5072 6f76 6964 6573 2d45  g8000.Provides-E
-00000440: 7874 7261 3a20 7079 7464 730a 5072 6f76  xtra: pytds.Prov
-00000450: 6964 6573 2d45 7874 7261 3a20 6173 796e  ides-Extra: asyn
-00000460: 6370 670a 4c69 6365 6e73 652d 4669 6c65  cpg.License-File
-00000470: 3a20 4c49 4345 4e53 450a 0a3c 7020 616c  : LICENSE..<p al
-00000480: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
-00000490: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-000004a0: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
-000004b0: 636f 6d2f 626c 6f67 2f74 6f70 6963 732f  com/blog/topics/
-000004c0: 6465 7665 6c6f 7065 7273 2d70 7261 6374  developers-pract
-000004d0: 6974 696f 6e65 7273 2f68 6f77 2d63 6f6e  itioners/how-con
-000004e0: 6e65 6374 2d63 6c6f 7564 2d73 716c 2d75  nect-cloud-sql-u
-000004f0: 7369 6e67 2d70 7974 686f 6e2d 6561 7379  sing-python-easy
-00000500: 2d77 6179 223e 0a20 2020 2020 2020 203c  -way">.        <
-00000510: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000520: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00000530: 6f6e 7465 6e74 2e63 6f6d 2f47 6f6f 676c  ontent.com/Googl
-00000540: 6543 6c6f 7564 506c 6174 666f 726d 2f63  eCloudPlatform/c
-00000550: 6c6f 7564 2d73 716c 2d70 7974 686f 6e2d  loud-sql-python-
-00000560: 636f 6e6e 6563 746f 722f 6d61 696e 2f64  connector/main/d
-00000570: 6f63 732f 696d 6167 6573 2f63 6c6f 7564  ocs/images/cloud
-00000580: 2d73 716c 2d70 7974 686f 6e2d 636f 6e6e  -sql-python-conn
-00000590: 6563 746f 722e 706e 6722 2061 6c74 3d22  ector.png" alt="
-000005a0: 636c 6f75 642d 7371 6c2d 7079 7468 6f6e  cloud-sql-python
-000005b0: 2d63 6f6e 6e65 6374 6f72 2069 6d61 6765  -connector image
-000005c0: 223e 0a20 2020 203c 2f61 3e0a 3c2f 703e  ">.    </a>.</p>
-000005d0: 0a0a 3c68 3120 616c 6967 6e3d 2263 656e  ..<h1 align="cen
-000005e0: 7465 7222 3e43 6c6f 7564 2053 514c 2050  ter">Cloud SQL P
-000005f0: 7974 686f 6e20 436f 6e6e 6563 746f 723c  ython Connector<
-00000600: 2f68 313e 0a0a 5b21 5b4f 7065 6e20 496e  /h1>..[![Open In
-00000610: 2043 6f6c 6162 5d5b 636f 6c61 622d 6261   Colab][colab-ba
-00000620: 6467 655d 5d5b 636f 6c61 622d 6e6f 7465  dge]][colab-note
-00000630: 626f 6f6b 5d0a 5b21 5b43 495d 5b63 692d  book].[![CI][ci-
-00000640: 6261 6467 655d 5d5b 6369 2d62 7569 6c64  badge]][ci-build
-00000650: 5d0a 5b21 5b70 7970 695d 5b70 7970 692d  ].[![pypi][pypi-
-00000660: 6261 6467 655d 5d5b 7079 7069 2d64 6f63  badge]][pypi-doc
-00000670: 735d 0a5b 215b 5079 5049 2064 6f77 6e6c  s].[![PyPI downl
-00000680: 6f61 6420 6d6f 6e74 685d 5b70 7970 692d  oad month][pypi-
-00000690: 646f 776e 6c6f 6164 735d 5d5b 7079 7069  downloads]][pypi
-000006a0: 2d64 6f63 735d 0a5b 215b 7079 7468 6f6e  -docs].[![python
-000006b0: 5d5b 7079 7468 6f6e 2d76 6572 7369 6f6e  ][python-version
-000006c0: 735d 5d5b 7079 7069 2d64 6f63 735d 0a0a  s]][pypi-docs]..
-000006d0: 5b63 6f6c 6162 2d62 6164 6765 5d3a 2068  [colab-badge]: h
-000006e0: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
-000006f0: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
-00000700: 2f61 7373 6574 732f 636f 6c61 622d 6261  /assets/colab-ba
-00000710: 6467 652e 7376 670a 5b63 6f6c 6162 2d6e  dge.svg.[colab-n
-00000720: 6f74 6562 6f6f 6b5d 3a20 6874 7470 733a  otebook]: https:
-00000730: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-00000740: 2e67 6f6f 676c 652e 636f 6d2f 6769 7468  .google.com/gith
-00000750: 7562 2f47 6f6f 676c 6543 6c6f 7564 506c  ub/GoogleCloudPl
-00000760: 6174 666f 726d 2f63 6c6f 7564 2d73 716c  atform/cloud-sql
-00000770: 2d70 7974 686f 6e2d 636f 6e6e 6563 746f  -python-connecto
-00000780: 722f 626c 6f62 2f6d 6169 6e2f 7361 6d70  r/blob/main/samp
-00000790: 6c65 732f 6e6f 7465 626f 6f6b 732f 706f  les/notebooks/po
-000007a0: 7374 6772 6573 5f70 7974 686f 6e5f 636f  stgres_python_co
-000007b0: 6e6e 6563 746f 722e 6970 796e 620a 5b63  nnector.ipynb.[c
-000007c0: 692d 6261 6467 655d 3a20 6874 7470 733a  i-badge]: https:
-000007d0: 2f2f 6769 7468 7562 2e63 6f6d 2f47 6f6f  //github.com/Goo
-000007e0: 676c 6543 6c6f 7564 506c 6174 666f 726d  gleCloudPlatform
-000007f0: 2f63 6c6f 7564 2d73 716c 2d70 7974 686f  /cloud-sql-pytho
-00000800: 6e2d 636f 6e6e 6563 746f 722f 6163 7469  n-connector/acti
-00000810: 6f6e 732f 776f 726b 666c 6f77 732f 7465  ons/workflows/te
-00000820: 7374 732e 796d 6c2f 6261 6467 652e 7376  sts.yml/badge.sv
-00000830: 673f 6576 656e 743d 7075 7368 0a5b 6369  g?event=push.[ci
-00000840: 2d62 7569 6c64 5d3a 2068 7474 7073 3a2f  -build]: https:/
-00000850: 2f67 6974 6875 622e 636f 6d2f 476f 6f67  /github.com/Goog
-00000860: 6c65 436c 6f75 6450 6c61 7466 6f72 6d2f  leCloudPlatform/
-00000870: 636c 6f75 642d 7371 6c2d 7079 7468 6f6e  cloud-sql-python
-00000880: 2d63 6f6e 6e65 6374 6f72 2f61 6374 696f  -connector/actio
-00000890: 6e73 2f77 6f72 6b66 6c6f 7773 2f74 6573  ns/workflows/tes
-000008a0: 7473 2e79 6d6c 3f71 7565 7279 3d65 7665  ts.yml?query=eve
-000008b0: 6e74 2533 4170 7573 682b 6272 616e 6368  nt%3Apush+branch
-000008c0: 2533 416d 6169 6e0a 5b70 7970 692d 6261  %3Amain.[pypi-ba
-000008d0: 6467 655d 3a20 6874 7470 733a 2f2f 696d  dge]: https://im
-000008e0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-000008f0: 692f 762f 636c 6f75 642d 7371 6c2d 7079  i/v/cloud-sql-py
-00000900: 7468 6f6e 2d63 6f6e 6e65 6374 6f72 0a5b  thon-connector.[
-00000910: 7079 7069 2d64 6f63 735d 3a20 6874 7470  pypi-docs]: http
-00000920: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000930: 6a65 6374 2f63 6c6f 7564 2d73 716c 2d70  ject/cloud-sql-p
-00000940: 7974 686f 6e2d 636f 6e6e 6563 746f 720a  ython-connector.
-00000950: 5b70 7970 692d 646f 776e 6c6f 6164 735d  [pypi-downloads]
-00000960: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00000970: 6965 6c64 732e 696f 2f70 7970 692f 646d  ields.io/pypi/dm
-00000980: 2f63 6c6f 7564 2d73 716c 2d70 7974 686f  /cloud-sql-pytho
-00000990: 6e2d 636f 6e6e 6563 746f 722e 7376 670a  n-connector.svg.
-000009a0: 5b70 7974 686f 6e2d 7665 7273 696f 6e73  [python-versions
-000009b0: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
-000009c0: 6869 656c 6473 2e69 6f2f 7079 7069 2f70  hields.io/pypi/p
-000009d0: 7976 6572 7369 6f6e 732f 636c 6f75 642d  yversions/cloud-
-000009e0: 7371 6c2d 7079 7468 6f6e 2d63 6f6e 6e65  sql-python-conne
-000009f0: 6374 6f72 0a0a 5468 6520 5f43 6c6f 7564  ctor..The _Cloud
-00000a00: 2053 514c 2050 7974 686f 6e20 436f 6e6e   SQL Python Conn
-00000a10: 6563 746f 725f 2069 7320 6120 436c 6f75  ector_ is a Clou
-00000a20: 6420 5351 4c20 636f 6e6e 6563 746f 7220  d SQL connector 
-00000a30: 6465 7369 676e 6564 2066 6f72 2075 7365  designed for use
-00000a40: 2077 6974 6820 7468 650a 5079 7468 6f6e   with the.Python
-00000a50: 206c 616e 6775 6167 652e 2055 7369 6e67   language. Using
-00000a60: 2061 2043 6c6f 7564 2053 514c 2063 6f6e   a Cloud SQL con
-00000a70: 6e65 6374 6f72 2070 726f 7669 6465 7320  nector provides 
-00000a80: 7468 6520 666f 6c6c 6f77 696e 6720 6265  the following be
-00000a90: 6e65 6669 7473 3a0a 2a20 2a2a 4941 4d20  nefits:.* **IAM 
-00000aa0: 4175 7468 6f72 697a 6174 696f 6e3a 2a2a  Authorization:**
-00000ab0: 2075 7365 7320 4941 4d20 7065 726d 6973   uses IAM permis
-00000ac0: 7369 6f6e 7320 746f 2063 6f6e 7472 6f6c  sions to control
-00000ad0: 2077 686f 2f77 6861 7420 6361 6e20 636f   who/what can co
-00000ae0: 6e6e 6563 7420 746f 0a20 2079 6f75 7220  nnect to.  your 
-00000af0: 436c 6f75 6420 5351 4c20 696e 7374 616e  Cloud SQL instan
-00000b00: 6365 730a 2a20 2a2a 496d 7072 6f76 6564  ces.* **Improved
-00000b10: 2053 6563 7572 6974 793a 2a2a 2075 7365   Security:** use
-00000b20: 7320 726f 6275 7374 2c20 7570 6461 7465  s robust, update
-00000b30: 6420 544c 5320 312e 3320 656e 6372 7970  d TLS 1.3 encryp
-00000b40: 7469 6f6e 2061 6e64 0a20 2069 6465 6e74  tion and.  ident
-00000b50: 6974 7920 7665 7269 6669 6361 7469 6f6e  ity verification
-00000b60: 2062 6574 7765 656e 2074 6865 2063 6c69   between the cli
-00000b70: 656e 7420 636f 6e6e 6563 746f 7220 616e  ent connector an
-00000b80: 6420 7468 6520 7365 7276 6572 2d73 6964  d the server-sid
-00000b90: 6520 7072 6f78 792c 0a20 2069 6e64 6570  e proxy,.  indep
-00000ba0: 656e 6465 6e74 206f 6620 7468 6520 6461  endent of the da
-00000bb0: 7461 6261 7365 2070 726f 746f 636f 6c2e  tabase protocol.
-00000bc0: 0a2a 202a 2a43 6f6e 7665 6e69 656e 6365  .* **Convenience
-00000bd0: 3a2a 2a20 7265 6d6f 7665 7320 7468 6520  :** removes the 
-00000be0: 7265 7175 6972 656d 656e 7420 746f 2075  requirement to u
-00000bf0: 7365 2061 6e64 2064 6973 7472 6962 7574  se and distribut
-00000c00: 6520 5353 4c0a 2020 6365 7274 6966 6963  e SSL.  certific
-00000c10: 6174 6573 2c20 6173 2077 656c 6c20 6173  ates, as well as
-00000c20: 206d 616e 6167 6520 6669 7265 7761 6c6c   manage firewall
-00000c30: 7320 6f72 2073 6f75 7263 652f 6465 7374  s or source/dest
-00000c40: 696e 6174 696f 6e20 4950 2061 6464 7265  ination IP addre
-00000c50: 7373 6573 2e0a 2a20 286f 7074 696f 6e61  sses..* (optiona
-00000c60: 6c6c 7929 202a 2a49 414d 2044 4220 4175  lly) **IAM DB Au
-00000c70: 7468 656e 7469 6361 7469 6f6e 3a2a 2a20  thentication:** 
-00000c80: 7072 6f76 6964 6573 2073 7570 706f 7274  provides support
-00000c90: 2066 6f72 0a20 205b 436c 6f75 6420 5351   for.  [Cloud SQ
-00000ca0: 4ce2 8099 7320 6175 746f 6d61 7469 6320  L...s automatic 
-00000cb0: 4941 4d20 4442 2041 7574 684e 5d5b 6961  IAM DB AuthN][ia
-00000cc0: 6d2d 6462 2d61 7574 686e 5d20 6665 6174  m-db-authn] feat
-00000cd0: 7572 652e 0a0a 5b69 616d 2d64 622d 6175  ure...[iam-db-au
-00000ce0: 7468 6e5d 3a20 6874 7470 733a 2f2f 636c  thn]: https://cl
-00000cf0: 6f75 642e 676f 6f67 6c65 2e63 6f6d 2f73  oud.google.com/s
-00000d00: 716c 2f64 6f63 732f 706f 7374 6772 6573  ql/docs/postgres
-00000d10: 2f61 7574 6865 6e74 6963 6174 696f 6e0a  /authentication.
-00000d20: 0a54 6865 2043 6c6f 7564 2053 514c 2050  .The Cloud SQL P
-00000d30: 7974 686f 6e20 436f 6e6e 6563 746f 7220  ython Connector 
-00000d40: 6973 2061 2070 6163 6b61 6765 2074 6f20  is a package to 
-00000d50: 6265 2075 7365 6420 616c 6f6e 6773 6964  be used alongsid
-00000d60: 6520 6120 6461 7461 6261 7365 2064 7269  e a database dri
-00000d70: 7665 722e 0a43 7572 7265 6e74 6c79 2073  ver..Currently s
-00000d80: 7570 706f 7274 6564 2064 7269 7665 7273  upported drivers
-00000d90: 2061 7265 3a0a 202d 205b 6070 796d 7973   are:. - [`pymys
-00000da0: 716c 605d 2868 7474 7073 3a2f 2f67 6974  ql`](https://git
-00000db0: 6875 622e 636f 6d2f 5079 4d79 5351 4c2f  hub.com/PyMySQL/
-00000dc0: 5079 4d79 5351 4c29 2028 4d79 5351 4c29  PyMySQL) (MySQL)
-00000dd0: 0a20 2d20 5b60 7067 3830 3030 605d 2868  . - [`pg8000`](h
-00000de0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000df0: 6d2f 746c 6f63 6b65 2f70 6738 3030 3029  m/tlocke/pg8000)
-00000e00: 2028 506f 7374 6772 6553 514c 290a 202d   (PostgreSQL). -
-00000e10: 205b 6061 7379 6e63 7067 605d 2868 7474   [`asyncpg`](htt
-00000e20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000e30: 4d61 6769 6353 7461 636b 2f61 7379 6e63  MagicStack/async
-00000e40: 7067 2920 2850 6f73 7467 7265 5351 4c29  pg) (PostgreSQL)
-00000e50: 0a20 2d20 5b60 7079 7464 7360 5d28 6874  . - [`pytds`](ht
-00000e60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000e70: 2f64 656e 6973 656e 6b6f 6d2f 7079 7464  /denisenkom/pytd
-00000e80: 7329 2028 5351 4c20 5365 7276 6572 290a  s) (SQL Server).
-00000e90: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-00000ea0: 6e0a 0a59 6f75 2063 616e 2069 6e73 7461  n..You can insta
-00000eb0: 6c6c 2074 6869 7320 6c69 6272 6172 7920  ll this library 
-00000ec0: 7769 7468 2060 7069 7020 696e 7374 616c  with `pip instal
-00000ed0: 6c60 2c20 7370 6563 6966 7969 6e67 2074  l`, specifying t
-00000ee0: 6865 2064 7269 7665 720a 6261 7365 6420  he driver.based 
-00000ef0: 6f6e 2079 6f75 7220 6461 7461 6261 7365  on your database
-00000f00: 2064 6961 6c65 6374 2e0a 0a23 2323 204d   dialect...### M
-00000f10: 7953 514c 0a60 6060 0a70 6970 2069 6e73  ySQL.```.pip ins
-00000f20: 7461 6c6c 2022 636c 6f75 642d 7371 6c2d  tall "cloud-sql-
-00000f30: 7079 7468 6f6e 2d63 6f6e 6e65 6374 6f72  python-connector
-00000f40: 5b70 796d 7973 716c 5d22 0a60 6060 0a23  [pymysql]".```.#
-00000f50: 2323 2050 6f73 7467 7265 730a 5468 6572  ## Postgres.Ther
-00000f60: 6520 6172 6520 7477 6f20 6469 6666 6572  e are two differ
-00000f70: 656e 7420 6461 7461 6261 7365 2064 7269  ent database dri
-00000f80: 7665 7273 2074 6861 7420 6172 6520 7375  vers that are su
-00000f90: 7070 6f72 7465 6420 666f 7220 7468 6520  pported for the 
-00000fa0: 506f 7374 6772 6573 2064 6961 6c65 6374  Postgres dialect
-00000fb0: 3a0a 0a23 2323 2320 7067 3830 3030 0a60  :..#### pg8000.`
-00000fc0: 6060 0a70 6970 2069 6e73 7461 6c6c 2022  ``.pip install "
-00000fd0: 636c 6f75 642d 7371 6c2d 7079 7468 6f6e  cloud-sql-python
-00000fe0: 2d63 6f6e 6e65 6374 6f72 5b70 6738 3030  -connector[pg800
-00000ff0: 305d 220a 6060 600a 2323 2323 2061 7379  0]".```.#### asy
-00001000: 6e63 7067 0a60 6060 0a70 6970 2069 6e73  ncpg.```.pip ins
-00001010: 7461 6c6c 2022 636c 6f75 642d 7371 6c2d  tall "cloud-sql-
-00001020: 7079 7468 6f6e 2d63 6f6e 6e65 6374 6f72  python-connector
-00001030: 5b61 7379 6e63 7067 5d22 0a60 6060 0a23  [asyncpg]".```.#
-00001040: 2323 2053 514c 2053 6572 7665 720a 6060  ## SQL Server.``
-00001050: 600a 7069 7020 696e 7374 616c 6c20 2263  `.pip install "c
-00001060: 6c6f 7564 2d73 716c 2d70 7974 686f 6e2d  loud-sql-python-
-00001070: 636f 6e6e 6563 746f 725b 7079 7464 735d  connector[pytds]
-00001080: 220a 6060 600a 2323 2055 7361 6765 0a0a  ".```.## Usage..
-00001090: 5468 6973 2070 6163 6b61 6765 2070 726f  This package pro
-000010a0: 7669 6465 7320 7365 7665 7261 6c20 6675  vides several fu
-000010b0: 6e63 7469 6f6e 7320 666f 7220 6175 7468  nctions for auth
-000010c0: 6f72 697a 696e 6720 616e 6420 656e 6372  orizing and encr
-000010d0: 7970 7469 6e67 0a63 6f6e 6e65 6374 696f  ypting.connectio
-000010e0: 6e73 2e20 5468 6573 6520 6675 6e63 7469  ns. These functi
-000010f0: 6f6e 7320 6172 6520 7573 6564 2077 6974  ons are used wit
-00001100: 6820 796f 7572 2064 6174 6162 6173 6520  h your database 
-00001110: 6472 6976 6572 2074 6f20 636f 6e6e 6563  driver to connec
-00001120: 7420 746f 0a79 6f75 7220 436c 6f75 6420  t to.your Cloud 
-00001130: 5351 4c20 696e 7374 616e 6365 2e0a 0a54  SQL instance...T
-00001140: 6865 2069 6e73 7461 6e63 6520 636f 6e6e  he instance conn
-00001150: 6563 7469 6f6e 206e 616d 6520 666f 7220  ection name for 
-00001160: 796f 7572 2043 6c6f 7564 2053 514c 2069  your Cloud SQL i
-00001170: 6e73 7461 6e63 6520 6973 2061 6c77 6179  nstance is alway
-00001180: 7320 696e 2074 6865 0a66 6f72 6d61 7420  s in the.format 
-00001190: 2270 726f 6a65 6374 3a72 6567 696f 6e3a  "project:region:
-000011a0: 696e 7374 616e 6365 222e 0a0a 2323 2320  instance"...### 
-000011b0: 4150 4973 2061 6e64 2053 6572 7669 6365  APIs and Service
-000011c0: 730a 0a54 6869 7320 7061 636b 6167 6520  s..This package 
-000011d0: 7265 7175 6972 6573 2074 6865 2066 6f6c  requires the fol
-000011e0: 6c6f 7769 6e67 2074 6f20 7375 6363 6573  lowing to succes
-000011f0: 7366 756c 6c79 206d 616b 6520 436c 6f75  sfully make Clou
-00001200: 6420 5351 4c20 436f 6e6e 6563 7469 6f6e  d SQL Connection
-00001210: 733a 0a0a 2d20 4941 4d20 7072 696e 6369  s:..- IAM princi
-00001220: 7061 6c20 2875 7365 722c 2073 6572 7669  pal (user, servi
-00001230: 6365 2061 6363 6f75 6e74 2c20 6574 632e  ce account, etc.
-00001240: 2920 7769 7468 2074 6865 0a5b 436c 6f75  ) with the.[Clou
-00001250: 6420 5351 4c20 436c 6965 6e74 5d5b 636c  d SQL Client][cl
-00001260: 6965 6e74 2d72 6f6c 655d 2072 6f6c 652e  ient-role] role.
-00001270: 2054 6869 7320 4941 4d20 7072 696e 6369   This IAM princi
-00001280: 7061 6c20 7769 6c6c 2062 6520 7573 6564  pal will be used
-00001290: 2066 6f72 0a5b 6372 6564 656e 7469 616c   for.[credential
-000012a0: 735d 2823 6372 6564 656e 7469 616c 7329  s](#credentials)
-000012b0: 2e0a 2d20 5468 6520 5b43 6c6f 7564 2053  ..- The [Cloud S
-000012c0: 514c 2041 646d 696e 2041 5049 5d5b 6164  QL Admin API][ad
-000012d0: 6d69 6e2d 6170 695d 2074 6f20 6265 2065  min-api] to be e
-000012e0: 6e61 626c 6564 2077 6974 6869 6e20 796f  nabled within yo
-000012f0: 7572 2047 6f6f 676c 6520 436c 6f75 640a  ur Google Cloud.
-00001300: 5072 6f6a 6563 742e 2042 7920 6465 6661  Project. By defa
-00001310: 756c 742c 2074 6865 2041 5049 2077 696c  ult, the API wil
-00001320: 6c20 6265 2063 616c 6c65 6420 696e 2074  l be called in t
-00001330: 6865 2070 726f 6a65 6374 2061 7373 6f63  he project assoc
-00001340: 6961 7465 6420 7769 7468 0a74 6865 2049  iated with.the I
-00001350: 414d 2070 7269 6e63 6970 616c 2e0a 0a5b  AM principal...[
-00001360: 6164 6d69 6e2d 6170 695d 3a20 6874 7470  admin-api]: http
-00001370: 733a 2f2f 636f 6e73 6f6c 652e 636c 6f75  s://console.clou
-00001380: 642e 676f 6f67 6c65 2e63 6f6d 2f61 7069  d.google.com/api
-00001390: 732f 6170 692f 7371 6c61 646d 696e 2e67  s/api/sqladmin.g
-000013a0: 6f6f 676c 6561 7069 732e 636f 6d0a 5b63  oogleapis.com.[c
-000013b0: 6c69 656e 742d 726f 6c65 5d3a 2068 7474  lient-role]: htt
-000013c0: 7073 3a2f 2f63 6c6f 7564 2e67 6f6f 676c  ps://cloud.googl
-000013d0: 652e 636f 6d2f 7371 6c2f 646f 6373 2f6d  e.com/sql/docs/m
-000013e0: 7973 716c 2f72 6f6c 6573 2d61 6e64 2d70  ysql/roles-and-p
-000013f0: 6572 6d69 7373 696f 6e73 0a0a 2323 2320  ermissions..### 
-00001400: 4372 6564 656e 7469 616c 730a 0a54 6869  Credentials..Thi
-00001410: 7320 6c69 6272 6172 7920 7573 6573 2074  s library uses t
-00001420: 6865 205b 4170 706c 6963 6174 696f 6e20  he [Application 
-00001430: 4465 6661 756c 7420 4372 6564 656e 7469  Default Credenti
-00001440: 616c 7320 2841 4443 295d 5b61 6463 5d20  als (ADC)][adc] 
-00001450: 7374 7261 7465 6779 2066 6f72 0a72 6573  strategy for.res
-00001460: 6f6c 7669 6e67 2063 7265 6465 6e74 6961  olving credentia
-00001470: 6c73 2e20 506c 6561 7365 2073 6565 205b  ls. Please see [
-00001480: 7468 6573 6520 696e 7374 7275 6374 696f  these instructio
-00001490: 6e73 2066 6f72 2068 6f77 2074 6f20 7365  ns for how to se
-000014a0: 7420 796f 7572 2041 4443 5d5b 7365 742d  t your ADC][set-
-000014b0: 6164 635d 0a28 476f 6f67 6c65 2043 6c6f  adc].(Google Clo
-000014c0: 7564 2041 7070 6c69 6361 7469 6f6e 2076  ud Application v
-000014d0: 7320 4c6f 6361 6c20 4465 7665 6c6f 706d  s Local Developm
-000014e0: 656e 742c 2049 414d 2075 7365 7220 7673  ent, IAM user vs
-000014f0: 2073 6572 7669 6365 2061 6363 6f75 6e74   service account
-00001500: 2063 7265 6465 6e74 6961 6c73 292c 0a6f   credentials),.o
-00001510: 7220 636f 6e73 756c 7420 7468 6520 5b67  r consult the [g
-00001520: 6f6f 676c 652e 6175 7468 5d5b 676f 6f67  oogle.auth][goog
-00001530: 6c65 2d61 7574 685d 2070 6163 6b61 6765  le-auth] package
-00001540: 2e0a 0a54 6f20 6578 706c 6963 6974 6c79  ...To explicitly
-00001550: 2073 6574 2061 2073 7065 6369 6669 6320   set a specific 
-00001560: 736f 7572 6365 2066 6f72 2074 6865 2063  source for the c
-00001570: 7265 6465 6e74 6961 6c73 2c20 7365 650a  redentials, see.
-00001580: 5b43 6f6e 6669 6775 7269 6e67 2074 6865  [Configuring the
-00001590: 2043 6f6e 6e65 6374 6f72 5d28 2363 6f6e   Connector](#con
-000015a0: 6669 6775 7269 6e67 2d74 6865 2d63 6f6e  figuring-the-con
-000015b0: 6e65 6374 6f72 2920 6265 6c6f 772e 0a0a  nector) below...
-000015c0: 5b61 6463 5d3a 2068 7474 7073 3a2f 2f63  [adc]: https://c
-000015d0: 6c6f 7564 2e67 6f6f 676c 652e 636f 6d2f  loud.google.com/
-000015e0: 646f 6373 2f61 7574 6865 6e74 6963 6174  docs/authenticat
-000015f0: 696f 6e23 6164 630a 5b73 6574 2d61 6463  ion#adc.[set-adc
-00001600: 5d3a 2068 7474 7073 3a2f 2f63 6c6f 7564  ]: https://cloud
-00001610: 2e67 6f6f 676c 652e 636f 6d2f 646f 6373  .google.com/docs
-00001620: 2f61 7574 6865 6e74 6963 6174 696f 6e2f  /authentication/
-00001630: 7072 6f76 6964 652d 6372 6564 656e 7469  provide-credenti
-00001640: 616c 732d 6164 630a 5b67 6f6f 676c 652d  als-adc.[google-
-00001650: 6175 7468 5d3a 2068 7474 7073 3a2f 2f67  auth]: https://g
-00001660: 6f6f 676c 652d 6175 7468 2e72 6561 6474  oogle-auth.readt
-00001670: 6865 646f 6373 2e69 6f2f 656e 2f6d 6173  hedocs.io/en/mas
-00001680: 7465 722f 7265 6665 7265 6e63 652f 676f  ter/reference/go
-00001690: 6f67 6c65 2e61 7574 682e 6874 6d6c 0a0a  ogle.auth.html..
-000016a0: 2323 2320 486f 7720 746f 2075 7365 2074  ### How to use t
-000016b0: 6869 7320 436f 6e6e 6563 746f 720a 0a54  his Connector..T
-000016c0: 6f20 636f 6e6e 6563 7420 746f 2043 6c6f  o connect to Clo
-000016d0: 7564 2053 514c 2075 7369 6e67 2074 6865  ud SQL using the
-000016e0: 2063 6f6e 6e65 6374 6f72 2c20 696e 6974   connector, init
-000016f0: 6974 616c 697a 6520 6120 6043 6f6e 6e65  italize a `Conne
-00001700: 6374 6f72 600a 6f62 6a65 6374 2061 6e64  ctor`.object and
-00001710: 2063 616c 6c20 6974 2773 2060 636f 6e6e   call it's `conn
-00001720: 6563 7460 206d 6574 686f 6420 7769 7468  ect` method with
-00001730: 2074 6865 2070 726f 7065 7220 696e 7075   the proper inpu
-00001740: 7420 7061 7261 6d65 7465 7273 2e0a 0a54  t parameters...T
-00001750: 6865 2060 436f 6e6e 6563 746f 7260 2069  he `Connector` i
-00001760: 7473 656c 6620 6372 6561 7465 7320 636f  tself creates co
-00001770: 6e6e 6563 7469 6f6e 206f 626a 6563 7473  nnection objects
-00001780: 2062 7920 6361 6c6c 696e 6720 6974 7320   by calling its 
-00001790: 6063 6f6e 6e65 6374 6020 6d65 7468 6f64  `connect` method
-000017a0: 2062 7574 2064 6f65 7320 6e6f 7420 6d61   but does not ma
-000017b0: 6e61 6765 2064 6174 6162 6173 6520 636f  nage database co
-000017c0: 6e6e 6563 7469 6f6e 2070 6f6f 6c69 6e67  nnection pooling
-000017d0: 2e20 466f 7220 7468 6973 2072 6561 736f  . For this reaso
-000017e0: 6e2c 2069 7420 6973 2072 6563 6f6d 6d65  n, it is recomme
-000017f0: 6e64 6564 2074 6f20 7573 6520 7468 6520  nded to use the 
-00001800: 636f 6e6e 6563 746f 7220 616c 6f6e 6773  connector alongs
-00001810: 6964 6520 6120 6c69 6272 6172 7920 7468  ide a library th
-00001820: 6174 2063 616e 2063 7265 6174 6520 636f  at can create co
-00001830: 6e6e 6563 7469 6f6e 2070 6f6f 6c73 2c20  nnection pools, 
-00001840: 7375 6368 2061 7320 5b53 514c 416c 6368  such as [SQLAlch
-00001850: 656d 795d 2868 7474 7073 3a2f 2f77 7777  emy](https://www
-00001860: 2e73 716c 616c 6368 656d 792e 6f72 672f  .sqlalchemy.org/
-00001870: 292e 2054 6869 7320 7769 6c6c 2061 6c6c  ). This will all
-00001880: 6f77 2066 6f72 2063 6f6e 6e65 6374 696f  ow for connectio
-00001890: 6e73 2074 6f20 7265 6d61 696e 206f 7065  ns to remain ope
-000018a0: 6e20 616e 6420 6265 2072 6575 7365 642c  n and be reused,
-000018b0: 2072 6564 7563 696e 6720 636f 6e6e 6563   reducing connec
-000018c0: 7469 6f6e 206f 7665 7268 6561 6420 616e  tion overhead an
-000018d0: 6420 7468 6520 6e75 6d62 6572 206f 6620  d the number of 
-000018e0: 636f 6e6e 6563 7469 6f6e 7320 6e65 6564  connections need
-000018f0: 6564 2e0a 0a49 6e20 7468 6520 436f 6e6e  ed...In the Conn
-00001900: 6563 746f 7227 7320 6063 6f6e 6e65 6374  ector's `connect
-00001910: 6020 6d65 7468 6f64 2062 656c 6f77 2c20  ` method below, 
-00001920: 696e 7075 7420 796f 7572 2063 6f6e 6e65  input your conne
-00001930: 6374 696f 6e20 7374 7269 6e67 2061 7320  ction string as 
-00001940: 7468 6520 6669 7273 7420 706f 7369 7469  the first positi
-00001950: 6f6e 616c 2061 7267 756d 656e 7420 616e  onal argument an
-00001960: 6420 7468 6520 6e61 6d65 206f 6620 7468  d the name of th
-00001970: 6520 6461 7461 6261 7365 2064 7269 7665  e database drive
-00001980: 7220 666f 7220 7468 6520 7365 636f 6e64  r for the second
-00001990: 2070 6f73 6974 696f 6e61 6c20 6172 6775   positional argu
-000019a0: 6d65 6e74 2e20 496e 7365 7274 2074 6865  ment. Insert the
-000019b0: 2072 6573 7420 6f66 2079 6f75 7220 636f   rest of your co
-000019c0: 6e6e 6563 7469 6f6e 206b 6579 776f 7264  nnection keyword
-000019d0: 2061 7267 756d 656e 7473 206c 696b 6520   arguments like 
-000019e0: 7573 6572 2c20 7061 7373 776f 7264 2061  user, password a
-000019f0: 6e64 2064 6174 6162 6173 652e 2059 6f75  nd database. You
-00001a00: 2063 616e 2061 6c73 6f20 7365 7420 7468   can also set th
-00001a10: 6520 6f70 7469 6f6e 616c 2060 7469 6d65  e optional `time
-00001a20: 6f75 7460 206f 7220 6069 705f 7479 7065  out` or `ip_type
-00001a30: 6020 6b65 7977 6f72 6420 6172 6775 6d65  ` keyword argume
-00001a40: 6e74 732e 0a0a 546f 2075 7365 2074 6869  nts...To use thi
-00001a50: 7320 636f 6e6e 6563 746f 7220 7769 7468  s connector with
-00001a60: 2053 514c 416c 6368 656d 792c 2075 7365   SQLAlchemy, use
-00001a70: 2074 6865 2060 6372 6561 746f 7260 2061   the `creator` a
-00001a80: 7267 756d 656e 7420 666f 7220 6073 716c  rgument for `sql
-00001a90: 616c 6368 656d 792e 6372 6561 7465 5f65  alchemy.create_e
-00001aa0: 6e67 696e 6560 3a0a 0a60 6060 7079 7468  ngine`:..```pyth
-00001ab0: 6f6e 0a66 726f 6d20 676f 6f67 6c65 2e63  on.from google.c
-00001ac0: 6c6f 7564 2e73 716c 2e63 6f6e 6e65 6374  loud.sql.connect
-00001ad0: 6f72 2069 6d70 6f72 7420 436f 6e6e 6563  or import Connec
-00001ae0: 746f 720a 696d 706f 7274 2073 716c 616c  tor.import sqlal
-00001af0: 6368 656d 790a 0a23 2069 6e69 7469 616c  chemy..# initial
-00001b00: 697a 6520 436f 6e6e 6563 746f 7220 6f62  ize Connector ob
-00001b10: 6a65 6374 0a63 6f6e 6e65 6374 6f72 203d  ject.connector =
-00001b20: 2043 6f6e 6e65 6374 6f72 2829 0a0a 2320   Connector()..# 
-00001b30: 6675 6e63 7469 6f6e 2074 6f20 7265 7475  function to retu
-00001b40: 726e 2074 6865 2064 6174 6162 6173 6520  rn the database 
-00001b50: 636f 6e6e 6563 7469 6f6e 0a64 6566 2067  connection.def g
-00001b60: 6574 636f 6e6e 2829 202d 3e20 7079 6d79  etconn() -> pymy
-00001b70: 7371 6c2e 636f 6e6e 6563 7469 6f6e 732e  sql.connections.
-00001b80: 436f 6e6e 6563 7469 6f6e 3a0a 2020 2020  Connection:.    
-00001b90: 636f 6e6e 3a20 7079 6d79 7371 6c2e 636f  conn: pymysql.co
-00001ba0: 6e6e 6563 7469 6f6e 732e 436f 6e6e 6563  nnections.Connec
-00001bb0: 7469 6f6e 203d 2063 6f6e 6e65 6374 6f72  tion = connector
-00001bc0: 2e63 6f6e 6e65 6374 280a 2020 2020 2020  .connect(.      
-00001bd0: 2020 2270 726f 6a65 6374 3a72 6567 696f    "project:regio
-00001be0: 6e3a 696e 7374 616e 6365 222c 0a20 2020  n:instance",.   
-00001bf0: 2020 2020 2022 7079 6d79 7371 6c22 2c0a       "pymysql",.
-00001c00: 2020 2020 2020 2020 7573 6572 3d22 6d79          user="my
-00001c10: 2d75 7365 7222 2c0a 2020 2020 2020 2020  -user",.        
-00001c20: 7061 7373 776f 7264 3d22 6d79 2d70 6173  password="my-pas
-00001c30: 7377 6f72 6422 2c0a 2020 2020 2020 2020  sword",.        
-00001c40: 6462 3d22 6d79 2d64 622d 6e61 6d65 220a  db="my-db-name".
-00001c50: 2020 2020 290a 2020 2020 7265 7475 726e      ).    return
-00001c60: 2063 6f6e 6e0a 0a23 2063 7265 6174 6520   conn..# create 
-00001c70: 636f 6e6e 6563 7469 6f6e 2070 6f6f 6c0a  connection pool.
-00001c80: 706f 6f6c 203d 2073 716c 616c 6368 656d  pool = sqlalchem
-00001c90: 792e 6372 6561 7465 5f65 6e67 696e 6528  y.create_engine(
-00001ca0: 0a20 2020 2022 6d79 7371 6c2b 7079 6d79  .    "mysql+pymy
-00001cb0: 7371 6c3a 2f2f 222c 0a20 2020 2063 7265  sql://",.    cre
-00001cc0: 6174 6f72 3d67 6574 636f 6e6e 2c0a 290a  ator=getconn,.).
-00001cd0: 6060 600a 0a54 6865 2072 6574 7572 6e65  ```..The returne
-00001ce0: 6420 636f 6e6e 6563 7469 6f6e 2070 6f6f  d connection poo
-00001cf0: 6c20 656e 6769 6e65 2063 616e 2074 6865  l engine can the
-00001d00: 6e20 6265 2075 7365 6420 746f 2071 7565  n be used to que
-00001d10: 7279 2061 6e64 206d 6f64 6966 7920 7468  ry and modify th
-00001d20: 6520 6461 7461 6261 7365 2e0a 0a60 6060  e database...```
-00001d30: 7079 7468 6f6e 0a23 2069 6e73 6572 7420  python.# insert 
-00001d40: 7374 6174 656d 656e 740a 696e 7365 7274  statement.insert
-00001d50: 5f73 746d 7420 3d20 7371 6c61 6c63 6865  _stmt = sqlalche
-00001d60: 6d79 2e74 6578 7428 0a20 2020 2022 494e  my.text(.    "IN
-00001d70: 5345 5254 2049 4e54 4f20 6d79 5f74 6162  SERT INTO my_tab
-00001d80: 6c65 2028 6964 2c20 7469 746c 6529 2056  le (id, title) V
-00001d90: 414c 5545 5320 283a 6964 2c20 3a74 6974  ALUES (:id, :tit
-00001da0: 6c65 2922 2c0a 290a 0a77 6974 6820 706f  le)",.)..with po
-00001db0: 6f6c 2e63 6f6e 6e65 6374 2829 2061 7320  ol.connect() as 
-00001dc0: 6462 5f63 6f6e 6e3a 0a20 2020 2023 2069  db_conn:.    # i
-00001dd0: 6e73 6572 7420 696e 746f 2064 6174 6162  nsert into datab
-00001de0: 6173 650a 2020 2020 6462 5f63 6f6e 6e2e  ase.    db_conn.
-00001df0: 6578 6563 7574 6528 696e 7365 7274 5f73  execute(insert_s
-00001e00: 746d 742c 2070 6172 616d 6574 6572 733d  tmt, parameters=
-00001e10: 7b22 6964 223a 2022 626f 6f6b 3122 2c20  {"id": "book1", 
-00001e20: 2274 6974 6c65 223a 2022 426f 6f6b 204f  "title": "Book O
-00001e30: 6e65 227d 290a 0a20 2020 2023 2071 7565  ne"})..    # que
-00001e40: 7279 2064 6174 6162 6173 650a 2020 2020  ry database.    
-00001e50: 7265 7375 6c74 203d 2064 625f 636f 6e6e  result = db_conn
-00001e60: 2e65 7865 6375 7465 2873 716c 616c 6368  .execute(sqlalch
-00001e70: 656d 792e 7465 7874 2822 5345 4c45 4354  emy.text("SELECT
-00001e80: 202a 2066 726f 6d20 6d79 5f74 6162 6c65   * from my_table
-00001e90: 2229 292e 6665 7463 6861 6c6c 2829 0a0a  ")).fetchall()..
-00001ea0: 2020 2020 2320 636f 6d6d 6974 2074 7261      # commit tra
-00001eb0: 6e73 6163 7469 6f6e 2028 5351 4c41 6c63  nsaction (SQLAlc
-00001ec0: 6865 6d79 2076 322e 582e 5820 6973 2063  hemy v2.X.X is c
-00001ed0: 6f6d 6d69 7420 6173 2079 6f75 2067 6f29  ommit as you go)
-00001ee0: 0a20 2020 2064 625f 636f 6e6e 2e63 6f6d  .    db_conn.com
-00001ef0: 6d69 7428 290a 0a20 2020 2023 2044 6f20  mit()..    # Do 
-00001f00: 736f 6d65 7468 696e 6720 7769 7468 2074  something with t
-00001f10: 6865 2072 6573 756c 7473 0a20 2020 2066  he results.    f
-00001f20: 6f72 2072 6f77 2069 6e20 7265 7375 6c74  or row in result
-00001f30: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
-00001f40: 726f 7729 0a60 6060 0a0a 546f 2063 6c6f  row).```..To clo
-00001f50: 7365 2074 6865 2060 436f 6e6e 6563 746f  se the `Connecto
-00001f60: 7260 206f 626a 6563 7427 7320 6261 636b  r` object's back
-00001f70: 6772 6f75 6e64 2072 6573 6f75 7263 6573  ground resources
-00001f80: 2c20 6361 6c6c 2069 7427 7320 6063 6c6f  , call it's `clo
-00001f90: 7365 2829 6020 6d65 7468 6f64 2061 7320  se()` method as 
-00001fa0: 666f 6c6c 6f77 733a 0a0a 6060 6070 7974  follows:..```pyt
-00001fb0: 686f 6e0a 636f 6e6e 6563 746f 722e 636c  hon.connector.cl
-00001fc0: 6f73 6528 290a 6060 600a 0a2a 2a4e 6f74  ose().```..**Not
-00001fd0: 652a 2a3a 2046 6f72 206d 6f72 6520 6578  e**: For more ex
-00001fe0: 616d 706c 6573 206f 6620 7573 696e 6720  amples of using 
-00001ff0: 5351 4c41 6c63 6865 6d79 2074 6f20 6d61  SQLAlchemy to ma
-00002000: 6e61 6765 2063 6f6e 6e65 6374 696f 6e20  nage connection 
-00002010: 706f 6f6c 696e 6720 7769 7468 2074 6865  pooling with the
-00002020: 2063 6f6e 6e65 6374 6f72 2c20 706c 6561   connector, plea
-00002030: 7365 2073 6565 205b 436c 6f75 6420 5351  se see [Cloud SQ
-00002040: 4c20 5351 4c41 6c63 6865 6d79 2053 616d  L SQLAlchemy Sam
-00002050: 706c 6573 5d28 6874 7470 733a 2f2f 636c  ples](https://cl
-00002060: 6f75 642e 676f 6f67 6c65 2e63 6f6d 2f73  oud.google.com/s
-00002070: 716c 2f64 6f63 732f 706f 7374 6772 6573  ql/docs/postgres
-00002080: 2f63 6f6e 6e65 6374 2d63 6f6e 6e65 6374  /connect-connect
-00002090: 6f72 7323 7079 7468 6f6e 5f31 292e 0a0a  ors#python_1)...
-000020a0: 2a2a 4e6f 7465 2066 6f72 2053 514c 2053  **Note for SQL S
-000020b0: 6572 7665 7220 7573 6572 732a 2a3a 2049  erver users**: I
-000020c0: 6620 796f 7572 2053 514c 2053 6572 7665  f your SQL Serve
-000020d0: 7220 696e 7374 616e 6365 2072 6571 7569  r instance requi
-000020e0: 7265 7320 5353 4c2c 2079 6f75 206e 6565  res SSL, you nee
-000020f0: 6420 746f 2064 6f77 6e6c 6f61 6420 7468  d to download th
-00002100: 6520 4341 2063 6572 7469 6669 6361 7465  e CA certificate
-00002110: 2066 6f72 2079 6f75 7220 696e 7374 616e   for your instan
-00002120: 6365 2061 6e64 2069 6e63 6c75 6465 2060  ce and include `
-00002130: 6361 6669 6c65 3d7b 7061 7468 2074 6f20  cafile={path to 
-00002140: 646f 776e 6c6f 6164 6564 2063 6572 7469  downloaded certi
-00002150: 6669 6361 7465 7d60 2061 6e64 2060 7661  ficate}` and `va
-00002160: 6c69 6461 7465 5f68 6f73 743d 4661 6c73  lidate_host=Fals
-00002170: 6560 2e20 5468 6973 2069 7320 6120 776f  e`. This is a wo
-00002180: 726b 6172 6f75 6e64 2066 6f72 2061 205b  rkaround for a [
-00002190: 6b6e 6f77 6e20 6973 7375 655d 2868 7474  known issue](htt
-000021a0: 7073 3a2f 2f69 7373 7565 7472 6163 6b65  ps://issuetracke
-000021b0: 722e 676f 6f67 6c65 2e63 6f6d 2f31 3834  r.google.com/184
-000021c0: 3836 3731 3437 292e 0a0a 2323 2320 436f  867147)...### Co
-000021d0: 6e66 6967 7572 696e 6720 7468 6520 436f  nfiguring the Co
-000021e0: 6e6e 6563 746f 720a 0a49 6620 796f 7520  nnector..If you 
-000021f0: 6e65 6564 2074 6f20 6375 7374 6f6d 697a  need to customiz
-00002200: 6520 736f 6d65 7468 696e 6720 6162 6f75  e something abou
-00002210: 7420 7468 6520 636f 6e6e 6563 746f 722c  t the connector,
-00002220: 206f 7220 7761 6e74 2074 6f20 7370 6563   or want to spec
-00002230: 6966 790a 6465 6661 756c 7473 2066 6f72  ify.defaults for
-00002240: 2065 6163 6820 636f 6e6e 6563 7469 6f6e   each connection
-00002250: 2074 6f20 6d61 6b65 2c20 796f 7520 6361   to make, you ca
-00002260: 6e20 696e 6974 6961 6c69 7a65 2061 0a60  n initialize a.`
-00002270: 436f 6e6e 6563 746f 7260 206f 626a 6563  Connector` objec
-00002280: 7420 6173 2066 6f6c 6c6f 7773 3a0a 0a60  t as follows:..`
-00002290: 6060 7079 7468 6f6e 0a66 726f 6d20 676f  ``python.from go
-000022a0: 6f67 6c65 2e63 6c6f 7564 2e73 716c 2e63  ogle.cloud.sql.c
-000022b0: 6f6e 6e65 6374 6f72 2069 6d70 6f72 7420  onnector import 
-000022c0: 436f 6e6e 6563 746f 722c 2049 5054 7970  Connector, IPTyp
-000022d0: 6573 0a0a 2320 4e6f 7465 3a20 616c 6c20  es..# Note: all 
-000022e0: 7061 7261 6d65 7465 7273 2062 656c 6f77  parameters below
-000022f0: 2061 7265 206f 7074 696f 6e61 6c0a 636f   are optional.co
-00002300: 6e6e 6563 746f 7220 3d20 436f 6e6e 6563  nnector = Connec
-00002310: 746f 7228 0a20 2020 2069 705f 7479 7065  tor(.    ip_type
-00002320: 3d49 5054 7970 6573 2e50 5542 4c49 432c  =IPTypes.PUBLIC,
-00002330: 0a20 2020 2065 6e61 626c 655f 6961 6d5f  .    enable_iam_
-00002340: 6175 7468 3d46 616c 7365 2c0a 2020 2020  auth=False,.    
-00002350: 7469 6d65 6f75 743d 3330 2c0a 2020 2020  timeout=30,.    
-00002360: 6372 6564 656e 7469 616c 733d 6375 7374  credentials=cust
-00002370: 6f6d 5f63 7265 6473 2023 2067 6f6f 676c  om_creds # googl
-00002380: 652e 6175 7468 2e63 7265 6465 6e74 6961  e.auth.credentia
-00002390: 6c73 2e43 7265 6465 6e74 6961 6c73 0a29  ls.Credentials.)
-000023a0: 0a60 6060 0a0a 2323 2320 5573 696e 6720  .```..### Using 
-000023b0: 436f 6e6e 6563 746f 7220 6173 2061 2043  Connector as a C
-000023c0: 6f6e 7465 7874 204d 616e 6167 6572 0a0a  ontext Manager..
-000023d0: 5468 6520 6043 6f6e 6e65 6374 6f72 6020  The `Connector` 
-000023e0: 6f62 6a65 6374 2063 616e 2061 6c73 6f20  object can also 
-000023f0: 6265 2075 7365 6420 6173 2061 2063 6f6e  be used as a con
-00002400: 7465 7874 206d 616e 6167 6572 2069 6e20  text manager in 
-00002410: 6f72 6465 7220 746f 0a61 7574 6f6d 6174  order to.automat
-00002420: 6963 616c 6c79 2063 6c6f 7365 2061 6e64  ically close and
-00002430: 2063 6c65 616e 7570 2072 6573 6f75 7263   cleanup resourc
-00002440: 6573 2c20 7265 6d6f 7669 6e67 2074 6865  es, removing the
-00002450: 206e 6565 6420 666f 7220 6578 706c 6963   need for explic
-00002460: 6974 0a63 616c 6c73 2074 6f20 6063 6f6e  it.calls to `con
-00002470: 6e65 6374 6f72 2e63 6c6f 7365 2829 602e  nector.close()`.
-00002480: 0a0a 436f 6e6e 6563 746f 7220 6173 2061  ..Connector as a
-00002490: 2063 6f6e 7465 7874 206d 616e 6167 6572   context manager
-000024a0: 3a0a 0a60 6060 7079 7468 6f6e 0a66 726f  :..```python.fro
-000024b0: 6d20 676f 6f67 6c65 2e63 6c6f 7564 2e73  m google.cloud.s
-000024c0: 716c 2e63 6f6e 6e65 6374 6f72 2069 6d70  ql.connector imp
-000024d0: 6f72 7420 436f 6e6e 6563 746f 720a 696d  ort Connector.im
-000024e0: 706f 7274 2073 716c 616c 6368 656d 790a  port sqlalchemy.
-000024f0: 0a23 2062 7569 6c64 2063 6f6e 6e65 6374  .# build connect
-00002500: 696f 6e0a 6465 6620 6765 7463 6f6e 6e28  ion.def getconn(
-00002510: 2920 2d3e 2070 796d 7973 716c 2e63 6f6e  ) -> pymysql.con
-00002520: 6e65 6374 696f 6e73 2e43 6f6e 6e65 6374  nections.Connect
-00002530: 696f 6e3a 0a20 2020 2077 6974 6820 436f  ion:.    with Co
-00002540: 6e6e 6563 746f 7228 2920 6173 2063 6f6e  nnector() as con
-00002550: 6e65 6374 6f72 3a0a 2020 2020 2020 2020  nector:.        
-00002560: 636f 6e6e 203d 2063 6f6e 6e65 6374 6f72  conn = connector
-00002570: 2e63 6f6e 6e65 6374 280a 2020 2020 2020  .connect(.      
-00002580: 2020 2020 2020 2270 726f 6a65 6374 3a72        "project:r
-00002590: 6567 696f 6e3a 696e 7374 616e 6365 222c  egion:instance",
-000025a0: 0a20 2020 2020 2020 2020 2020 2022 7079  .            "py
-000025b0: 6d79 7371 6c22 2c0a 2020 2020 2020 2020  mysql",.        
-000025c0: 2020 2020 7573 6572 3d22 6d79 2d75 7365      user="my-use
-000025d0: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
-000025e0: 7061 7373 776f 7264 3d22 6d79 2d70 6173  password="my-pas
-000025f0: 7377 6f72 6422 2c0a 2020 2020 2020 2020  sword",.        
-00002600: 2020 2020 6462 3d22 6d79 2d64 622d 6e61      db="my-db-na
-00002610: 6d65 220a 2020 2020 2020 2020 290a 2020  me".        ).  
-00002620: 2020 7265 7475 726e 2063 6f6e 6e0a 0a23    return conn..#
-00002630: 2063 7265 6174 6520 636f 6e6e 6563 7469   create connecti
-00002640: 6f6e 2070 6f6f 6c0a 706f 6f6c 203d 2073  on pool.pool = s
-00002650: 716c 616c 6368 656d 792e 6372 6561 7465  qlalchemy.create
-00002660: 5f65 6e67 696e 6528 0a20 2020 2022 6d79  _engine(.    "my
-00002670: 7371 6c2b 7079 6d79 7371 6c3a 2f2f 222c  sql+pymysql://",
-00002680: 0a20 2020 2063 7265 6174 6f72 3d67 6574  .    creator=get
-00002690: 636f 6e6e 2c0a 290a 0a23 2069 6e73 6572  conn,.)..# inser
-000026a0: 7420 7374 6174 656d 656e 740a 696e 7365  t statement.inse
-000026b0: 7274 5f73 746d 7420 3d20 7371 6c61 6c63  rt_stmt = sqlalc
-000026c0: 6865 6d79 2e74 6578 7428 0a20 2020 2022  hemy.text(.    "
-000026d0: 494e 5345 5254 2049 4e54 4f20 6d79 5f74  INSERT INTO my_t
-000026e0: 6162 6c65 2028 6964 2c20 7469 746c 6529  able (id, title)
-000026f0: 2056 414c 5545 5320 283a 6964 2c20 3a74   VALUES (:id, :t
-00002700: 6974 6c65 2922 2c0a 290a 0a23 2069 6e74  itle)",.)..# int
-00002710: 6572 6163 7420 7769 7468 2043 6c6f 7564  eract with Cloud
-00002720: 2053 514c 2064 6174 6162 6173 6520 7573   SQL database us
-00002730: 696e 6720 636f 6e6e 6563 7469 6f6e 2070  ing connection p
-00002740: 6f6f 6c0a 7769 7468 2070 6f6f 6c2e 636f  ool.with pool.co
-00002750: 6e6e 6563 7428 2920 6173 2064 625f 636f  nnect() as db_co
-00002760: 6e6e 3a0a 2020 2020 2320 696e 7365 7274  nn:.    # insert
-00002770: 2069 6e74 6f20 6461 7461 6261 7365 0a20   into database. 
-00002780: 2020 2064 625f 636f 6e6e 2e65 7865 6375     db_conn.execu
-00002790: 7465 2869 6e73 6572 745f 7374 6d74 2c20  te(insert_stmt, 
-000027a0: 7061 7261 6d65 7465 7273 3d7b 2269 6422  parameters={"id"
-000027b0: 3a20 2262 6f6f 6b31 222c 2022 7469 746c  : "book1", "titl
-000027c0: 6522 3a20 2242 6f6f 6b20 4f6e 6522 7d29  e": "Book One"})
-000027d0: 0a0a 2020 2020 2320 636f 6d6d 6974 2074  ..    # commit t
-000027e0: 7261 6e73 6163 7469 6f6e 2028 5351 4c41  ransaction (SQLA
-000027f0: 6c63 6865 6d79 2076 322e 582e 5820 6973  lchemy v2.X.X is
-00002800: 2063 6f6d 6d69 7420 6173 2079 6f75 2067   commit as you g
-00002810: 6f29 0a20 2020 2064 625f 636f 6e6e 2e63  o).    db_conn.c
-00002820: 6f6d 6d69 7428 290a 0a20 2020 2023 2071  ommit()..    # q
-00002830: 7565 7279 2064 6174 6162 6173 650a 2020  uery database.  
-00002840: 2020 7265 7375 6c74 203d 2064 625f 636f    result = db_co
-00002850: 6e6e 2e65 7865 6375 7465 2873 716c 616c  nn.execute(sqlal
-00002860: 6368 656d 792e 7465 7874 2822 5345 4c45  chemy.text("SELE
-00002870: 4354 202a 2066 726f 6d20 6d79 5f74 6162  CT * from my_tab
-00002880: 6c65 2229 292e 6665 7463 6861 6c6c 2829  le")).fetchall()
-00002890: 0a0a 2020 2020 2320 446f 2073 6f6d 6574  ..    # Do somet
-000028a0: 6869 6e67 2077 6974 6820 7468 6520 7265  hing with the re
-000028b0: 7375 6c74 730a 2020 2020 666f 7220 726f  sults.    for ro
-000028c0: 7720 696e 2072 6573 756c 743a 0a20 2020  w in result:.   
-000028d0: 2020 2020 2070 7269 6e74 2872 6f77 290a       print(row).
-000028e0: 6060 600a 0a23 2323 2053 7065 6369 6679  ```..### Specify
-000028f0: 696e 6720 5075 626c 6963 206f 7220 5072  ing Public or Pr
-00002900: 6976 6174 6520 4950 0a0a 5468 6520 436c  ivate IP..The Cl
-00002910: 6f75 6420 5351 4c20 436f 6e6e 6563 746f  oud SQL Connecto
-00002920: 7220 666f 7220 5079 7468 6f6e 2063 616e  r for Python can
-00002930: 2062 6520 7573 6564 2074 6f20 636f 6e6e   be used to conn
-00002940: 6563 7420 746f 2043 6c6f 7564 2053 514c  ect to Cloud SQL
-00002950: 2069 6e73 7461 6e63 6573 2075 7369 6e67   instances using
-00002960: 2062 6f74 6820 7075 626c 6963 2061 6e64   both public and
-00002970: 2070 7269 7661 7465 2049 5020 6164 6472   private IP addr
-00002980: 6573 7365 732e 2054 6f20 7370 6563 6966  esses. To specif
-00002990: 7920 7768 6963 6820 4950 2061 6464 7265  y which IP addre
-000029a0: 7373 2074 6f20 7573 6520 746f 2063 6f6e  ss to use to con
-000029b0: 6e65 6374 2c20 7365 7420 7468 6520 6069  nect, set the `i
-000029c0: 705f 7479 7065 6020 6b65 7977 6f72 6420  p_type` keyword 
-000029d0: 6172 6775 6d65 6e74 2050 6f73 7369 626c  argument Possibl
-000029e0: 6520 7661 6c75 6573 2061 7265 2060 4950  e values are `IP
-000029f0: 5479 7065 732e 5055 424c 4943 6020 616e  Types.PUBLIC` an
-00002a00: 6420 6049 5054 7970 6573 2e50 5249 5641  d `IPTypes.PRIVA
-00002a10: 5445 602e 0a45 7861 6d70 6c65 3a0a 0a60  TE`..Example:..`
-00002a20: 6060 7079 7468 6f6e 0a66 726f 6d20 676f  ``python.from go
-00002a30: 6f67 6c65 2e63 6c6f 7564 2e73 716c 2e63  ogle.cloud.sql.c
-00002a40: 6f6e 6e65 6374 6f72 2069 6d70 6f72 7420  onnector import 
-00002a50: 4950 5479 7065 730a 0a63 6f6e 6e65 6374  IPTypes..connect
-00002a60: 6f72 2e63 6f6e 6e65 6374 280a 2020 2020  or.connect(.    
-00002a70: 2270 726f 6a65 6374 3a72 6567 696f 6e3a  "project:region:
-00002a80: 696e 7374 616e 6365 222c 0a20 2020 2022  instance",.    "
-00002a90: 7079 6d79 7371 6c22 2c0a 2020 2020 6970  pymysql",.    ip
-00002aa0: 5f74 7970 653d 4950 5479 7065 732e 5052  _type=IPTypes.PR
-00002ab0: 4956 4154 4520 2320 7573 6520 7072 6976  IVATE # use priv
-00002ac0: 6174 6520 4950 0a2e 2e2e 2069 6e73 6572  ate IP.... inser
-00002ad0: 7420 6f74 6865 7220 6b77 6172 6773 202e  t other kwargs .
-00002ae0: 2e2e 0a29 0a60 6060 0a0a 4e6f 7465 3a20  ...).```..Note: 
-00002af0: 4966 2073 7065 6369 6679 696e 6720 5072  If specifying Pr
-00002b00: 6976 6174 6520 4950 2c20 796f 7572 2061  ivate IP, your a
-00002b10: 7070 6c69 6361 7469 6f6e 206d 7573 7420  pplication must 
-00002b20: 616c 7265 6164 7920 6265 2069 6e20 7468  already be in th
-00002b30: 6520 7361 6d65 2056 5043 206e 6574 776f  e same VPC netwo
-00002b40: 726b 2061 7320 796f 7572 2043 6c6f 7564  rk as your Cloud
-00002b50: 2053 514c 2049 6e73 7461 6e63 652e 0a0a   SQL Instance...
-00002b60: 2323 2320 4941 4d20 4175 7468 656e 7469  ### IAM Authenti
-00002b70: 6361 7469 6f6e 0a0a 436f 6e6e 6563 7469  cation..Connecti
-00002b80: 6f6e 7320 7573 696e 6720 5b41 7574 6f6d  ons using [Autom
-00002b90: 6174 6963 2049 414d 2064 6174 6162 6173  atic IAM databas
-00002ba0: 6520 6175 7468 656e 7469 6361 7469 6f6e  e authentication
-00002bb0: 5d28 6874 7470 733a 2f2f 636c 6f75 642e  ](https://cloud.
-00002bc0: 676f 6f67 6c65 2e63 6f6d 2f73 716c 2f64  google.com/sql/d
-00002bd0: 6f63 732f 706f 7374 6772 6573 2f61 7574  ocs/postgres/aut
-00002be0: 6865 6e74 6963 6174 696f 6e23 6175 746f  hentication#auto
-00002bf0: 6d61 7469 6329 2061 7265 2073 7570 706f  matic) are suppo
-00002c00: 7274 6564 2077 6865 6e20 7573 696e 6720  rted when using 
-00002c10: 506f 7374 6772 6573 206f 7220 4d79 5351  Postgres or MySQ
-00002c20: 4c20 6472 6976 6572 732e 0a46 6972 7374  L drivers..First
-00002c30: 2c20 6d61 6b65 2073 7572 6520 746f 205b  , make sure to [
-00002c40: 636f 6e66 6967 7572 6520 796f 7572 2043  configure your C
-00002c50: 6c6f 7564 2053 514c 2049 6e73 7461 6e63  loud SQL Instanc
-00002c60: 6520 746f 2061 6c6c 6f77 2049 414d 2061  e to allow IAM a
-00002c70: 7574 6865 6e74 6963 6174 696f 6e5d 2868  uthentication](h
-00002c80: 7474 7073 3a2f 2f63 6c6f 7564 2e67 6f6f  ttps://cloud.goo
-00002c90: 676c 652e 636f 6d2f 7371 6c2f 646f 6373  gle.com/sql/docs
-00002ca0: 2f70 6f73 7467 7265 732f 6372 6561 7465  /postgres/create
-00002cb0: 2d65 6469 742d 6961 6d2d 696e 7374 616e  -edit-iam-instan
-00002cc0: 6365 7323 636f 6e66 6967 7572 652d 6961  ces#configure-ia
-00002cd0: 6d2d 6462 2d69 6e73 7461 6e63 6529 0a61  m-db-instance).a
-00002ce0: 6e64 205b 6164 6420 616e 2049 414d 2064  nd [add an IAM d
-00002cf0: 6174 6162 6173 6520 7573 6572 5d28 6874  atabase user](ht
-00002d00: 7470 733a 2f2f 636c 6f75 642e 676f 6f67  tps://cloud.goog
-00002d10: 6c65 2e63 6f6d 2f73 716c 2f64 6f63 732f  le.com/sql/docs/
-00002d20: 706f 7374 6772 6573 2f63 7265 6174 652d  postgres/create-
-00002d30: 6d61 6e61 6765 2d69 616d 2d75 7365 7273  manage-iam-users
-00002d40: 2363 7265 6174 696e 672d 612d 6461 7461  #creating-a-data
-00002d50: 6261 7365 2d75 7365 7229 2e0a 0a4e 6f77  base-user)...Now
-00002d60: 2c20 796f 7520 6361 6e20 636f 6e6e 6563  , you can connec
-00002d70: 7420 7573 696e 6720 7573 6572 206f 7220  t using user or 
-00002d80: 7365 7276 6963 6520 6163 636f 756e 7420  service account 
-00002d90: 6372 6564 656e 7469 616c 7320 696e 7374  credentials inst
-00002da0: 6561 6420 6f66 2061 2070 6173 7377 6f72  ead of a passwor
-00002db0: 642e 0a49 6e20 7468 6520 6361 6c6c 2074  d..In the call t
-00002dc0: 6f20 636f 6e6e 6563 742c 2073 6574 2074  o connect, set t
-00002dd0: 6865 2060 656e 6162 6c65 5f69 616d 5f61  he `enable_iam_a
-00002de0: 7574 6860 206b 6579 776f 7264 2061 7267  uth` keyword arg
-00002df0: 756d 656e 7420 746f 2074 7275 6520 616e  ument to true an
-00002e00: 6420 7468 6520 6075 7365 7260 2061 7267  d the `user` arg
-00002e10: 756d 656e 7420 746f 2074 6865 2061 7070  ument to the app
-00002e20: 726f 7072 6961 7465 6c79 2066 6f72 6d61  ropriately forma
-00002e30: 7474 6564 2049 414d 2070 7269 6e63 6970  tted IAM princip
-00002e40: 616c 2e0a 3e20 506f 7374 6772 6573 3a20  al..> Postgres: 
-00002e50: 466f 7220 616e 2049 414d 2075 7365 7220  For an IAM user 
-00002e60: 6163 636f 756e 742c 2074 6869 7320 6973  account, this is
-00002e70: 2074 6865 2075 7365 7227 7320 656d 6169   the user's emai
-00002e80: 6c20 6164 6472 6573 732e 2046 6f72 2061  l address. For a
-00002e90: 2073 6572 7669 6365 2061 6363 6f75 6e74   service account
-00002ea0: 2c20 6974 2069 7320 7468 6520 7365 7276  , it is the serv
-00002eb0: 6963 6520 6163 636f 756e 7427 7320 656d  ice account's em
-00002ec0: 6169 6c20 7769 7468 6f75 7420 7468 6520  ail without the 
-00002ed0: 602e 6773 6572 7669 6365 6163 636f 756e  `.gserviceaccoun
-00002ee0: 742e 636f 6d60 2064 6f6d 6169 6e20 7375  t.com` domain su
-00002ef0: 6666 6978 2e0a 0a3e 204d 7953 514c 3a20  ffix...> MySQL: 
-00002f00: 466f 7220 616e 2049 414d 2075 7365 7220  For an IAM user 
-00002f10: 6163 636f 756e 742c 2074 6869 7320 6973  account, this is
-00002f20: 2074 6865 2075 7365 7227 7320 656d 6169   the user's emai
-00002f30: 6c20 6164 6472 6573 732c 2077 6974 686f  l address, witho
-00002f40: 7574 2074 6865 2040 206f 7220 646f 6d61  ut the @ or doma
-00002f50: 696e 206e 616d 652e 2046 6f72 2065 7861  in name. For exa
-00002f60: 6d70 6c65 2c20 666f 7220 6074 6573 742d  mple, for `test-
-00002f70: 7573 6572 4067 6d61 696c 2e63 6f6d 602c  user@gmail.com`,
-00002f80: 2073 6574 2074 6865 2060 7573 6572 6020   set the `user` 
-00002f90: 6172 6775 6d65 6e74 2074 6f20 6074 6573  argument to `tes
-00002fa0: 742d 7573 6572 602e 2046 6f72 2061 2073  t-user`. For a s
-00002fb0: 6572 7669 6365 2061 6363 6f75 6e74 2c20  ervice account, 
-00002fc0: 7468 6973 2069 7320 7468 6520 7365 7276  this is the serv
-00002fd0: 6963 6520 6163 636f 756e 7427 7320 656d  ice account's em
-00002fe0: 6169 6c20 6164 6472 6573 7320 7769 7468  ail address with
-00002ff0: 6f75 7420 7468 6520 6040 7072 6f6a 6563  out the `@projec
-00003000: 742d 6964 2e69 616d 2e67 7365 7276 6963  t-id.iam.gservic
-00003010: 6561 6363 6f75 6e74 2e63 6f6d 6020 7375  eaccount.com` su
-00003020: 6666 6978 2e0a 0a45 7861 6d70 6c65 3a0a  ffix...Example:.
-00003030: 0a60 6060 7079 7468 6f6e 0a63 6f6e 6e65  .```python.conne
-00003040: 6374 6f72 2e63 6f6e 6e65 6374 280a 2020  ctor.connect(.  
-00003050: 2020 2022 7072 6f6a 6563 743a 7265 6769     "project:regi
-00003060: 6f6e 3a69 6e73 7461 6e63 6522 2c0a 2020  on:instance",.  
-00003070: 2020 2022 7067 3830 3030 222c 0a20 2020     "pg8000",.   
-00003080: 2020 7573 6572 3d22 706f 7374 6772 6573    user="postgres
-00003090: 2d69 616d 2d75 7365 7240 676d 6169 6c2e  -iam-user@gmail.
-000030a0: 636f 6d22 2c0a 2020 2020 2064 623d 226d  com",.     db="m
-000030b0: 792d 6462 2d6e 616d 6522 2c0a 2020 2020  y-db-name",.    
-000030c0: 2065 6e61 626c 655f 6961 6d5f 6175 7468   enable_iam_auth
-000030d0: 3d54 7275 652c 0a20 290a 6060 600a 0a23  =True,. ).```..#
-000030e0: 2323 2053 514c 2053 6572 7665 7220 4163  ## SQL Server Ac
-000030f0: 7469 7665 2044 6972 6563 746f 7279 2041  tive Directory A
-00003100: 7574 6865 6e74 6963 6174 696f 6e0a 0a41  uthentication..A
-00003110: 6374 6976 6520 4469 7265 6374 6f72 7920  ctive Directory 
-00003120: 6175 7468 656e 7469 6361 7469 6f6e 2066  authentication f
-00003130: 6f72 2053 514c 2053 6572 7665 7220 696e  or SQL Server in
-00003140: 7374 616e 6365 7320 6973 2063 7572 7265  stances is curre
-00003150: 6e74 6c79 206f 6e6c 7920 7375 7070 6f72  ntly only suppor
-00003160: 7465 6420 6f6e 2057 696e 646f 7773 2e20  ted on Windows. 
-00003170: 4669 7273 742c 206d 616b 6520 7375 7265  First, make sure
-00003180: 2074 6f20 666f 6c6c 6f77 205b 7468 6573   to follow [thes
-00003190: 6520 7374 6570 735d 2868 7474 7073 3a2f  e steps](https:/
-000031a0: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
-000031b0: 6d2f 626c 6f67 2f74 6f70 6963 732f 6465  m/blog/topics/de
-000031c0: 7665 6c6f 7065 7273 2d70 7261 6374 6974  velopers-practit
-000031d0: 696f 6e65 7273 2f63 7265 6174 696e 672d  ioners/creating-
-000031e0: 7371 6c2d 7365 7276 6572 2d69 6e73 7461  sql-server-insta
-000031f0: 6e63 652d 696e 7465 6772 6174 6564 2d61  nce-integrated-a
-00003200: 6374 6976 652d 6469 7265 6374 6f72 792d  ctive-directory-
-00003210: 7573 696e 672d 676f 6f67 6c65 2d63 6c6f  using-google-clo
-00003220: 7564 2d73 716c 2920 746f 2073 6574 2075  ud-sql) to set u
-00003230: 7020 6120 4d61 6e61 6765 6420 4144 2064  p a Managed AD d
-00003240: 6f6d 6169 6e20 616e 6420 6a6f 696e 2079  omain and join y
-00003250: 6f75 7220 436c 6f75 6420 5351 4c20 696e  our Cloud SQL in
-00003260: 7374 616e 6365 2074 6f20 7468 6520 646f  stance to the do
-00003270: 6d61 696e 2e20 5b53 6565 2068 6572 6520  main. [See here 
-00003280: 666f 7220 6d6f 7265 2069 6e66 6f20 6f6e  for more info on
-00003290: 2043 6c6f 7564 2053 514c 2041 6374 6976   Cloud SQL Activ
-000032a0: 6520 4469 7265 6374 6f72 7920 696e 7465  e Directory inte
-000032b0: 6772 6174 696f 6e5d 2868 7474 7073 3a2f  gration](https:/
-000032c0: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
-000032d0: 6d2f 7371 6c2f 646f 6373 2f73 716c 7365  m/sql/docs/sqlse
-000032e0: 7276 6572 2f61 6429 2e0a 0a4f 6e63 6520  rver/ad)...Once 
-000032f0: 796f 7520 6861 7665 2066 6f6c 6c6f 7765  you have followe
-00003300: 6420 7468 6520 7374 6570 7320 6c69 6e6b  d the steps link
-00003310: 6564 2061 626f 7665 2c20 796f 7520 6361  ed above, you ca
-00003320: 6e20 7275 6e20 7468 6520 666f 6c6c 6f77  n run the follow
-00003330: 696e 6720 636f 6465 2074 6f20 7265 7475  ing code to retu
-00003340: 726e 2061 2063 6f6e 6e65 6374 696f 6e20  rn a connection 
-00003350: 6f62 6a65 6374 3a0a 0a60 6060 7079 7468  object:..```pyth
-00003360: 6f6e 0a63 6f6e 6e65 6374 6f72 2e63 6f6e  on.connector.con
-00003370: 6e65 6374 280a 2020 2020 2270 726f 6a65  nect(.    "proje
-00003380: 6374 3a72 6567 696f 6e3a 696e 7374 616e  ct:region:instan
-00003390: 6365 222c 0a20 2020 2022 7079 7464 7322  ce",.    "pytds"
-000033a0: 2c0a 2020 2020 6462 3d22 6d79 2d64 622d  ,.    db="my-db-
-000033b0: 6e61 6d65 222c 0a20 2020 2061 6374 6976  name",.    activ
-000033c0: 655f 6469 7265 6374 6f72 795f 6175 7468  e_directory_auth
-000033d0: 3d54 7275 652c 0a20 2020 2073 6572 7665  =True,.    serve
-000033e0: 725f 6e61 6d65 3d22 7075 626c 6963 2e5b  r_name="public.[
-000033f0: 696e 7374 616e 6365 5d2e 5b6c 6f63 6174  instance].[locat
-00003400: 696f 6e5d 2e5b 7072 6f6a 6563 745d 2e63  ion].[project].c
-00003410: 6c6f 7564 7371 6c2e 5b64 6f6d 6169 6e5d  loudsql.[domain]
-00003420: 222c 0a29 0a60 6060 0a0a 4f72 2c20 6966  ",.).```..Or, if
-00003430: 2075 7369 6e67 2050 7269 7661 7465 2049   using Private I
-00003440: 503a 0a0a 6060 6070 7974 686f 6e0a 636f  P:..```python.co
-00003450: 6e6e 6563 746f 722e 636f 6e6e 6563 7428  nnector.connect(
-00003460: 0a20 2020 2022 7072 6f6a 6563 743a 7265  .    "project:re
-00003470: 6769 6f6e 3a69 6e73 7461 6e63 6522 2c0a  gion:instance",.
-00003480: 2020 2020 2270 7974 6473 222c 0a20 2020      "pytds",.   
-00003490: 2064 623d 226d 792d 6462 2d6e 616d 6522   db="my-db-name"
-000034a0: 2c0a 2020 2020 6163 7469 7665 5f64 6972  ,.    active_dir
-000034b0: 6563 746f 7279 5f61 7574 683d 5472 7565  ectory_auth=True
-000034c0: 2c0a 2020 2020 7365 7276 6572 5f6e 616d  ,.    server_nam
-000034d0: 653d 2270 7269 7661 7465 2e5b 696e 7374  e="private.[inst
-000034e0: 616e 6365 5d2e 5b6c 6f63 6174 696f 6e5d  ance].[location]
-000034f0: 2e5b 7072 6f6a 6563 745d 2e63 6c6f 7564  .[project].cloud
-00003500: 7371 6c2e 5b64 6f6d 6169 6e5d 222c 0a20  sql.[domain]",. 
-00003510: 2020 2069 705f 7479 7065 3d49 5054 7970     ip_type=IPTyp
-00003520: 6573 2e50 5249 5641 5445 0a29 0a60 6060  es.PRIVATE.).```
-00003530: 0a0a 2323 2320 5573 696e 6720 7468 6520  ..### Using the 
-00003540: 5079 7468 6f6e 2043 6f6e 6e65 6374 6f72  Python Connector
-00003550: 2077 6974 6820 5079 7468 6f6e 2057 6562   with Python Web
-00003560: 2046 7261 6d65 776f 726b 730a 0a54 6865   Frameworks..The
-00003570: 2050 7974 686f 6e20 436f 6e6e 6563 746f   Python Connecto
-00003580: 7220 6361 6e20 6265 2075 7365 6420 616c  r can be used al
-00003590: 6f6e 6773 6964 6520 706f 7075 6c61 7220  ongside popular 
-000035a0: 5079 7468 6f6e 2077 6562 2066 7261 6d65  Python web frame
-000035b0: 776f 726b 7320 7375 6368 0a61 7320 466c  works such.as Fl
-000035c0: 6173 6b2c 2046 6173 7441 5049 2c20 6574  ask, FastAPI, et
-000035d0: 632c 2074 6f20 696e 7465 6772 6174 6520  c, to integrate 
-000035e0: 436c 6f75 6420 5351 4c20 6461 7461 6261  Cloud SQL databa
-000035f0: 7365 7320 7769 7468 696e 2079 6f75 720a  ses within your.
-00003600: 7765 6220 6170 706c 6963 6174 696f 6e73  web applications
-00003610: 2e0a 0a23 2323 2320 466c 6173 6b2d 5351  ...#### Flask-SQ
-00003620: 4c41 6c63 6865 6d79 0a0a 5b46 6c61 736b  LAlchemy..[Flask
-00003630: 2d53 514c 416c 6368 656d 795d 2868 7474  -SQLAlchemy](htt
-00003640: 7073 3a2f 2f66 6c61 736b 2d73 716c 616c  ps://flask-sqlal
-00003650: 6368 656d 792e 7061 6c6c 6574 7370 726f  chemy.palletspro
-00003660: 6a65 6374 732e 636f 6d2f 656e 2f32 2e78  jects.com/en/2.x
-00003670: 2f29 0a69 7320 616e 2065 7874 656e 7369  /).is an extensi
-00003680: 6f6e 2066 6f72 205b 466c 6173 6b5d 2868  on for [Flask](h
-00003690: 7474 7073 3a2f 2f66 6c61 736b 2e70 616c  ttps://flask.pal
-000036a0: 6c65 7473 7072 6f6a 6563 7473 2e63 6f6d  letsprojects.com
-000036b0: 2f65 6e2f 322e 322e 782f 290a 7468 6174  /en/2.2.x/).that
-000036c0: 2061 6464 7320 7375 7070 6f72 7420 666f   adds support fo
-000036d0: 7220 5b53 514c 416c 6368 656d 795d 2868  r [SQLAlchemy](h
-000036e0: 7474 7073 3a2f 2f77 7777 2e73 716c 616c  ttps://www.sqlal
-000036f0: 6368 656d 792e 6f72 672f 2920 746f 2079  chemy.org/) to y
-00003700: 6f75 720a 6170 706c 6963 6174 696f 6e2e  our.application.
-00003710: 2049 7420 6169 6d73 2074 6f20 7369 6d70   It aims to simp
-00003720: 6c69 6679 2075 7369 6e67 2053 514c 416c  lify using SQLAl
-00003730: 6368 656d 7920 7769 7468 2046 6c61 736b  chemy with Flask
-00003740: 2062 7920 7072 6f76 6964 696e 670a 7573   by providing.us
-00003750: 6566 756c 2064 6566 6175 6c74 7320 616e  eful defaults an
-00003760: 6420 6578 7472 6120 6865 6c70 6572 7320  d extra helpers 
-00003770: 7468 6174 206d 616b 6520 6974 2065 6173  that make it eas
-00003780: 6965 7220 746f 2061 6363 6f6d 706c 6973  ier to accomplis
-00003790: 680a 636f 6d6d 6f6e 2074 6173 6b73 2e0a  h.common tasks..
-000037a0: 0a59 6f75 2063 616e 2063 6f6e 6669 6775  .You can configu
-000037b0: 7265 2046 6c61 736b 2d53 514c 416c 6368  re Flask-SQLAlch
-000037c0: 656d 7920 746f 2063 6f6e 6e65 6374 2074  emy to connect t
-000037d0: 6f20 6120 436c 6f75 6420 5351 4c20 6461  o a Cloud SQL da
-000037e0: 7461 6261 7365 2066 726f 6d0a 796f 7572  tabase from.your
-000037f0: 2077 6562 2061 7070 6c69 6361 7469 6f6e   web application
-00003800: 2074 6872 6f75 6768 2074 6865 2066 6f6c   through the fol
-00003810: 6c6f 7769 6e67 3a0a 0a60 6060 7079 7468  lowing:..```pyth
-00003820: 6f6e 0a66 726f 6d20 666c 6173 6b20 696d  on.from flask im
-00003830: 706f 7274 2046 6c61 736b 0a66 726f 6d20  port Flask.from 
-00003840: 666c 6173 6b5f 7371 6c61 6c63 6865 6d79  flask_sqlalchemy
-00003850: 2069 6d70 6f72 7420 5351 4c41 6c63 6865   import SQLAlche
-00003860: 6d79 0a66 726f 6d20 676f 6f67 6c65 2e63  my.from google.c
-00003870: 6c6f 7564 2e73 716c 2e63 6f6e 6e65 6374  loud.sql.connect
-00003880: 6f72 2069 6d70 6f72 7420 436f 6e6e 6563  or import Connec
-00003890: 746f 722c 2049 5054 7970 6573 0a0a 0a23  tor, IPTypes...#
-000038a0: 2050 7974 686f 6e20 436f 6e6e 6563 746f   Python Connecto
-000038b0: 7220 6461 7461 6261 7365 2063 6f6e 6e65  r database conne
-000038c0: 6374 696f 6e20 6675 6e63 7469 6f6e 0a64  ction function.d
-000038d0: 6566 2067 6574 636f 6e6e 2829 3a0a 2020  ef getconn():.  
-000038e0: 2020 7769 7468 2043 6f6e 6e65 6374 6f72    with Connector
-000038f0: 2829 2061 7320 636f 6e6e 6563 746f 723a  () as connector:
-00003900: 0a20 2020 2020 2020 2063 6f6e 6e20 3d20  .        conn = 
-00003910: 636f 6e6e 6563 746f 722e 636f 6e6e 6563  connector.connec
-00003920: 7428 0a20 2020 2020 2020 2020 2020 2022  t(.            "
-00003930: 7072 6f6a 6563 743a 7265 6769 6f6e 3a69  project:region:i
-00003940: 6e73 7461 6e63 652d 6e61 6d65 222c 2023  nstance-name", #
-00003950: 2043 6c6f 7564 2053 514c 2049 6e73 7461   Cloud SQL Insta
-00003960: 6e63 6520 436f 6e6e 6563 7469 6f6e 204e  nce Connection N
-00003970: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-00003980: 2270 6738 3030 3022 2c0a 2020 2020 2020  "pg8000",.      
-00003990: 2020 2020 2020 7573 6572 3d22 6d79 2d75        user="my-u
-000039a0: 7365 7222 2c0a 2020 2020 2020 2020 2020  ser",.          
-000039b0: 2020 7061 7373 776f 7264 3d22 6d79 2d70    password="my-p
-000039c0: 6173 7377 6f72 6422 2c0a 2020 2020 2020  assword",.      
-000039d0: 2020 2020 2020 6462 3d22 6d79 2d64 6174        db="my-dat
-000039e0: 6162 6173 6522 2c0a 2020 2020 2020 2020  abase",.        
-000039f0: 2020 2020 6970 5f74 7970 653d 2049 5054      ip_type= IPT
-00003a00: 7970 6573 2e50 5542 4c49 4320 2023 2049  ypes.PUBLIC  # I
-00003a10: 5054 7970 6573 2e50 5249 5641 5445 2066  PTypes.PRIVATE f
-00003a20: 6f72 2070 7269 7661 7465 2049 500a 2020  or private IP.  
-00003a30: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00003a40: 7265 7475 726e 2063 6f6e 6e0a 0a0a 6170  return conn...ap
-00003a50: 7020 3d20 466c 6173 6b28 5f5f 6e61 6d65  p = Flask(__name
-00003a60: 5f5f 290a 0a23 2063 6f6e 6669 6775 7265  __)..# configure
-00003a70: 2046 6c61 736b 2d53 514c 416c 6368 656d   Flask-SQLAlchem
-00003a80: 7920 746f 2075 7365 2050 7974 686f 6e20  y to use Python 
-00003a90: 436f 6e6e 6563 746f 720a 6170 702e 636f  Connector.app.co
-00003aa0: 6e66 6967 5b27 5351 4c41 4c43 4845 4d59  nfig['SQLALCHEMY
-00003ab0: 5f44 4154 4142 4153 455f 5552 4927 5d20  _DATABASE_URI'] 
-00003ac0: 3d20 2270 6f73 7467 7265 7371 6c2b 7067  = "postgresql+pg
-00003ad0: 3830 3030 3a2f 2f22 0a61 7070 2e63 6f6e  8000://".app.con
-00003ae0: 6669 675b 2753 514c 414c 4348 454d 595f  fig['SQLALCHEMY_
-00003af0: 454e 4749 4e45 5f4f 5054 494f 4e53 275d  ENGINE_OPTIONS']
-00003b00: 203d 207b 0a20 2020 2022 6372 6561 746f   = {.    "creato
-00003b10: 7222 3a20 6765 7463 6f6e 6e0a 7d0a 0a64  r": getconn.}..d
-00003b20: 6220 3d20 5351 4c41 6c63 6865 6d79 2861  b = SQLAlchemy(a
-00003b30: 7070 290a 6060 600a 0a46 6f72 206d 6f72  pp).```..For mor
-00003b40: 6520 6465 7461 696c 7320 6f6e 2068 6f77  e details on how
-00003b50: 2074 6f20 7573 6520 466c 6173 6b2d 5351   to use Flask-SQ
-00003b60: 4c41 6c63 6865 6d79 2c20 6368 6563 6b20  LAlchemy, check 
-00003b70: 6f75 7420 7468 650a 5b46 6c61 736b 2d53  out the.[Flask-S
-00003b80: 514c 416c 6368 656d 7920 5175 6963 6b73  QLAlchemy Quicks
-00003b90: 7461 7274 735d 2868 7474 7073 3a2f 2f66  tarts](https://f
-00003ba0: 6c61 736b 2d73 716c 616c 6368 656d 792e  lask-sqlalchemy.
-00003bb0: 7061 6c6c 6574 7370 726f 6a65 6374 732e  palletsprojects.
-00003bc0: 636f 6d2f 656e 2f32 2e78 2f71 7569 636b  com/en/2.x/quick
-00003bd0: 7374 6172 742f 2329 0a0a 2323 2323 2046  start/#)..#### F
-00003be0: 6173 7441 5049 0a0a 5b46 6173 7441 5049  astAPI..[FastAPI
-00003bf0: 5d28 6874 7470 733a 2f2f 6661 7374 6170  ](https://fastap
-00003c00: 692e 7469 616e 676f 6c6f 2e63 6f6d 2f29  i.tiangolo.com/)
-00003c10: 2069 7320 6120 6d6f 6465 726e 2c20 6661   is a modern, fa
-00003c20: 7374 2028 6869 6768 2d70 6572 666f 726d  st (high-perform
-00003c30: 616e 6365 292c 0a77 6562 2066 7261 6d65  ance),.web frame
-00003c40: 776f 726b 2066 6f72 2062 7569 6c64 696e  work for buildin
-00003c50: 6720 4150 4973 2077 6974 6820 5079 7468  g APIs with Pyth
-00003c60: 6f6e 2062 6173 6564 206f 6e20 7374 616e  on based on stan
-00003c70: 6461 7264 2050 7974 686f 6e20 7479 7065  dard Python type
-00003c80: 2068 696e 7473 2e0a 0a59 6f75 2063 616e   hints...You can
-00003c90: 2063 6f6e 6669 6775 7265 2046 6173 7441   configure FastA
-00003ca0: 5049 2074 6f20 636f 6e6e 6563 7420 746f  PI to connect to
-00003cb0: 2061 2043 6c6f 7564 2053 514c 2064 6174   a Cloud SQL dat
-00003cc0: 6162 6173 6520 6672 6f6d 0a79 6f75 7220  abase from.your 
-00003cd0: 7765 6220 6170 706c 6963 6174 696f 6e20  web application 
-00003ce0: 7573 696e 6720 5b53 514c 416c 6368 656d  using [SQLAlchem
-00003cf0: 7920 4f52 4d5d 2868 7474 7073 3a2f 2f64  y ORM](https://d
-00003d00: 6f63 732e 7371 6c61 6c63 6865 6d79 2e6f  ocs.sqlalchemy.o
-00003d10: 7267 2f65 6e2f 3134 2f6f 726d 2f29 0a74  rg/en/14/orm/).t
-00003d20: 6872 6f75 6768 2074 6865 2066 6f6c 6c6f  hrough the follo
-00003d30: 7769 6e67 3a0a 0a60 6060 7079 7468 6f6e  wing:..```python
-00003d40: 0a66 726f 6d20 7371 6c61 6c63 6865 6d79  .from sqlalchemy
-00003d50: 2069 6d70 6f72 7420 6372 6561 7465 5f65   import create_e
-00003d60: 6e67 696e 650a 6672 6f6d 2073 716c 616c  ngine.from sqlal
-00003d70: 6368 656d 792e 6578 742e 6465 636c 6172  chemy.ext.declar
-00003d80: 6174 6976 6520 696d 706f 7274 2064 6563  ative import dec
-00003d90: 6c61 7261 7469 7665 5f62 6173 650a 6672  larative_base.fr
-00003da0: 6f6d 2073 716c 616c 6368 656d 792e 6f72  om sqlalchemy.or
-00003db0: 6d20 696d 706f 7274 2073 6573 7369 6f6e  m import session
-00003dc0: 6d61 6b65 720a 6672 6f6d 2067 6f6f 676c  maker.from googl
-00003dd0: 652e 636c 6f75 642e 7371 6c2e 636f 6e6e  e.cloud.sql.conn
-00003de0: 6563 746f 7220 696d 706f 7274 2043 6f6e  ector import Con
-00003df0: 6e65 6374 6f72 2c20 4950 5479 7065 730a  nector, IPTypes.
-00003e00: 0a23 2050 7974 686f 6e20 436f 6e6e 6563  .# Python Connec
-00003e10: 746f 7220 6461 7461 6261 7365 2063 6f6e  tor database con
-00003e20: 6e65 6374 696f 6e20 6675 6e63 7469 6f6e  nection function
-00003e30: 0a64 6566 2067 6574 636f 6e6e 2829 3a0a  .def getconn():.
-00003e40: 2020 2020 7769 7468 2043 6f6e 6e65 6374      with Connect
-00003e50: 6f72 2829 2061 7320 636f 6e6e 6563 746f  or() as connecto
-00003e60: 723a 0a20 2020 2020 2020 2063 6f6e 6e20  r:.        conn 
-00003e70: 3d20 636f 6e6e 6563 746f 722e 636f 6e6e  = connector.conn
-00003e80: 6563 7428 0a20 2020 2020 2020 2020 2020  ect(.           
-00003e90: 2022 7072 6f6a 6563 743a 7265 6769 6f6e   "project:region
-00003ea0: 3a69 6e73 7461 6e63 652d 6e61 6d65 222c  :instance-name",
-00003eb0: 2023 2043 6c6f 7564 2053 514c 2049 6e73   # Cloud SQL Ins
-00003ec0: 7461 6e63 6520 436f 6e6e 6563 7469 6f6e  tance Connection
-00003ed0: 204e 616d 650a 2020 2020 2020 2020 2020   Name.          
-00003ee0: 2020 2270 6738 3030 3022 2c0a 2020 2020    "pg8000",.    
-00003ef0: 2020 2020 2020 2020 7573 6572 3d22 6d79          user="my
-00003f00: 2d75 7365 7222 2c0a 2020 2020 2020 2020  -user",.        
-00003f10: 2020 2020 7061 7373 776f 7264 3d22 6d79      password="my
-00003f20: 2d70 6173 7377 6f72 6422 2c0a 2020 2020  -password",.    
-00003f30: 2020 2020 2020 2020 6462 3d22 6d79 2d64          db="my-d
-00003f40: 6174 6162 6173 6522 2c0a 2020 2020 2020  atabase",.      
-00003f50: 2020 2020 2020 6970 5f74 7970 653d 2049        ip_type= I
-00003f60: 5054 7970 6573 2e50 5542 4c49 4320 2023  PTypes.PUBLIC  #
-00003f70: 2049 5054 7970 6573 2e50 5249 5641 5445   IPTypes.PRIVATE
-00003f80: 2066 6f72 2070 7269 7661 7465 2049 500a   for private IP.
-00003f90: 2020 2020 2020 2020 290a 2020 2020 7265          ).    re
-00003fa0: 7475 726e 2063 6f6e 6e0a 0a53 514c 414c  turn conn..SQLAL
-00003fb0: 4348 454d 595f 4441 5441 4241 5345 5f55  CHEMY_DATABASE_U
-00003fc0: 524c 203d 2022 706f 7374 6772 6573 716c  RL = "postgresql
-00003fd0: 2b70 6738 3030 303a 2f2f 220a 0a65 6e67  +pg8000://"..eng
-00003fe0: 696e 6520 3d20 6372 6561 7465 5f65 6e67  ine = create_eng
-00003ff0: 696e 6528 0a20 2020 2053 514c 414c 4348  ine(.    SQLALCH
-00004000: 454d 595f 4441 5441 4241 5345 5f55 524c  EMY_DATABASE_URL
-00004010: 202c 2063 7265 6174 6f72 3d67 6574 636f   , creator=getco
-00004020: 6e6e 0a29 0a0a 2320 6372 6561 7465 2053  nn.)..# create S
-00004030: 514c 416c 6368 656d 7920 4f52 4d20 7365  QLAlchemy ORM se
-00004040: 7373 696f 6e0a 5365 7373 696f 6e4c 6f63  ssion.SessionLoc
-00004050: 616c 203d 2073 6573 7369 6f6e 6d61 6b65  al = sessionmake
-00004060: 7228 6175 746f 636f 6d6d 6974 3d46 616c  r(autocommit=Fal
-00004070: 7365 2c20 6175 746f 666c 7573 683d 4661  se, autoflush=Fa
-00004080: 6c73 652c 2062 696e 643d 656e 6769 6e65  lse, bind=engine
-00004090: 290a 0a42 6173 6520 3d20 6465 636c 6172  )..Base = declar
-000040a0: 6174 6976 655f 6261 7365 2829 0a60 6060  ative_base().```
-000040b0: 0a0a 546f 206c 6561 726e 206d 6f72 6520  ..To learn more 
-000040c0: 6162 6f75 7420 696e 7465 6772 6174 696e  about integratin
-000040d0: 6720 6120 6461 7461 6261 7365 2069 6e74  g a database int
-000040e0: 6f20 796f 7572 2046 6173 7441 5049 2061  o your FastAPI a
-000040f0: 7070 6c69 6361 7469 6f6e 2c0a 666f 6c6c  pplication,.foll
-00004100: 6f77 2061 6c6f 6e67 2074 6865 205b 4661  ow along the [Fa
-00004110: 7374 4150 4920 5351 4c20 4461 7461 6261  stAPI SQL Databa
-00004120: 7365 2067 7569 6465 5d28 6874 7470 733a  se guide](https:
-00004130: 2f2f 6661 7374 6170 692e 7469 616e 676f  //fastapi.tiango
-00004140: 6c6f 2e63 6f6d 2f74 7574 6f72 6961 6c2f  lo.com/tutorial/
-00004150: 7371 6c2d 6461 7461 6261 7365 732f 2363  sql-databases/#c
-00004160: 7265 6174 652d 7468 652d 6461 7461 6261  reate-the-databa
-00004170: 7365 2d6d 6f64 656c 7329 2e0a 0a23 2323  se-models)...###
-00004180: 2041 7379 6e63 2044 7269 7665 7220 5573   Async Driver Us
-00004190: 6167 650a 0a54 6865 2043 6c6f 7564 2053  age..The Cloud S
-000041a0: 514c 2043 6f6e 6e65 6374 6f72 2069 7320  QL Connector is 
-000041b0: 636f 6d70 6174 6962 6c65 2077 6974 680a  compatible with.
-000041c0: 5b61 7379 6e63 696f 5d28 6874 7470 733a  [asyncio](https:
-000041d0: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
-000041e0: 672f 332f 6c69 6272 6172 792f 6173 796e  g/3/library/asyn
-000041f0: 6369 6f2e 6874 6d6c 2920 746f 2069 6d70  cio.html) to imp
-00004200: 726f 7665 2074 6865 2073 7065 6564 0a61  rove the speed.a
-00004210: 6e64 2065 6666 6963 6965 6e63 7920 6f66  nd efficiency of
-00004220: 2064 6174 6162 6173 6520 636f 6e6e 6563   database connec
-00004230: 7469 6f6e 7320 7468 726f 7567 6820 636f  tions through co
-00004240: 6e63 7572 7265 6e63 792e 2059 6f75 2063  ncurrency. You c
-00004250: 616e 2075 7365 2061 6c6c 0a6e 6f6e 2d61  an use all.non-a
-00004260: 7379 6e63 696f 2064 7269 7665 7273 2074  syncio drivers t
-00004270: 6872 6f75 6768 2074 6865 2060 436f 6e6e  hrough the `Conn
-00004280: 6563 746f 722e 636f 6e6e 6563 745f 6173  ector.connect_as
-00004290: 796e 6360 2066 756e 6374 696f 6e2c 2069  ync` function, i
-000042a0: 6e20 6164 6469 7469 6f6e 0a74 6f20 7468  n addition.to th
-000042b0: 6520 666f 6c6c 6f77 696e 6720 6173 796e  e following asyn
-000042c0: 6369 6f20 6461 7461 6261 7365 2064 7269  cio database dri
-000042d0: 7665 7273 3a0a 2d20 5b61 7379 6e63 7067  vers:.- [asyncpg
-000042e0: 5d28 6874 7470 733a 2f2f 6d61 6769 6373  ](https://magics
-000042f0: 7461 636b 2e67 6974 6875 622e 696f 2f61  tack.github.io/a
-00004300: 7379 6e63 7067 2920 2850 6f73 7467 7265  syncpg) (Postgre
-00004310: 7329 0a0a 5468 6520 436c 6f75 6420 5351  s)..The Cloud SQ
-00004320: 4c20 436f 6e6e 6563 746f 7220 6861 7320  L Connector has 
-00004330: 6120 6865 6c70 6572 2060 6372 6561 7465  a helper `create
-00004340: 5f61 7379 6e63 5f63 6f6e 6e65 6374 6f72  _async_connector
-00004350: 6020 6675 6e63 7469 6f6e 2074 6861 7420  ` function that 
-00004360: 6973 0a72 6563 6f6d 6d65 6e64 6564 2066  is.recommended f
-00004370: 6f72 2061 7379 6e63 696f 2064 6174 6162  or asyncio datab
-00004380: 6173 6520 636f 6e6e 6563 7469 6f6e 732e  ase connections.
-00004390: 2049 7420 7265 7475 726e 7320 6120 6043   It returns a `C
-000043a0: 6f6e 6e65 6374 6f72 600a 6f62 6a65 6374  onnector`.object
-000043b0: 2074 6861 7420 7573 6573 2074 6865 2063   that uses the c
-000043c0: 7572 7265 6e74 2074 6872 6561 6427 7320  urrent thread's 
-000043d0: 7275 6e6e 696e 6720 6576 656e 7420 6c6f  running event lo
-000043e0: 6f70 2e20 5468 6973 2069 7320 6469 6666  op. This is diff
-000043f0: 6572 656e 740a 7468 616e 2060 436f 6e6e  erent.than `Conn
-00004400: 6563 746f 7228 2960 2077 6869 6368 2062  ector()` which b
-00004410: 7920 6465 6661 756c 7420 696e 6974 6961  y default initia
-00004420: 6c69 7a65 7320 6120 6e65 7720 6576 656e  lizes a new even
-00004430: 7420 6c6f 6f70 2069 6e20 610a 6261 636b  t loop in a.back
-00004440: 6772 6f75 6e64 2074 6872 6561 642e 0a0a  ground thread...
-00004450: 5468 6520 6063 7265 6174 655f 6173 796e  The `create_asyn
-00004460: 635f 636f 6e6e 6563 746f 7260 2061 6c6c  c_connector` all
-00004470: 6f77 7320 616c 6c20 7468 6520 7361 6d65  ows all the same
-00004480: 2069 6e70 7574 2061 7267 756d 656e 7473   input arguments
-00004490: 2061 7320 7468 650a 5b43 6f6e 6e65 6374   as the.[Connect
-000044a0: 6f72 5d28 2363 6f6e 6669 6775 7269 6e67  or](#configuring
-000044b0: 2d74 6865 2d63 6f6e 6e65 6374 6f72 2920  -the-connector) 
-000044c0: 6f62 6a65 6374 2e0a 0a4f 6e63 6520 6120  object...Once a 
-000044d0: 6043 6f6e 6e65 6374 6f72 6020 6f62 6a65  `Connector` obje
-000044e0: 6374 2069 7320 7265 7475 726e 6564 2062  ct is returned b
-000044f0: 7920 6063 7265 6174 655f 6173 796e 635f  y `create_async_
-00004500: 636f 6e6e 6563 746f 7260 2079 6f75 2063  connector` you c
-00004510: 616e 2063 616c 6c0a 6974 7320 6063 6f6e  an call.its `con
-00004520: 6e65 6374 5f61 7379 6e63 6020 6d65 7468  nect_async` meth
-00004530: 6f64 2c20 6a75 7374 2061 7320 796f 7520  od, just as you 
-00004540: 776f 756c 6420 7468 6520 6063 6f6e 6e65  would the `conne
-00004550: 6374 6020 6d65 7468 6f64 3a0a 0a60 6060  ct` method:..```
-00004560: 7079 7468 6f6e 0a69 6d70 6f72 7420 6173  python.import as
-00004570: 796e 6370 670a 0a69 6d70 6f72 7420 7371  yncpg..import sq
-00004580: 6c61 6c63 6865 6d79 0a66 726f 6d20 7371  lalchemy.from sq
-00004590: 6c61 6c63 6865 6d79 2e65 7874 2e61 7379  lalchemy.ext.asy
-000045a0: 6e63 696f 2069 6d70 6f72 7420 4173 796e  ncio import Asyn
-000045b0: 6345 6e67 696e 652c 2063 7265 6174 655f  cEngine, create_
-000045c0: 6173 796e 635f 656e 6769 6e65 0a0a 6672  async_engine..fr
-000045d0: 6f6d 2067 6f6f 676c 652e 636c 6f75 642e  om google.cloud.
-000045e0: 7371 6c2e 636f 6e6e 6563 746f 7220 696d  sql.connector im
-000045f0: 706f 7274 2043 6f6e 6e65 6374 6f72 2c20  port Connector, 
-00004600: 6372 6561 7465 5f61 7379 6e63 5f63 6f6e  create_async_con
-00004610: 6e65 6374 6f72 0a0a 6173 796e 6320 6465  nector..async de
-00004620: 6620 696e 6974 5f63 6f6e 6e65 6374 696f  f init_connectio
-00004630: 6e5f 706f 6f6c 2863 6f6e 6e65 6374 6f72  n_pool(connector
-00004640: 3a20 436f 6e6e 6563 746f 7229 202d 3e20  : Connector) -> 
-00004650: 4173 796e 6345 6e67 696e 653a 0a20 2020  AsyncEngine:.   
-00004660: 2023 2069 6e69 7469 616c 697a 6520 436f   # initialize Co
-00004670: 6e6e 6563 746f 7220 6f62 6a65 6374 2066  nnector object f
-00004680: 6f72 2063 6f6e 6e65 6374 696f 6e73 2074  or connections t
-00004690: 6f20 436c 6f75 6420 5351 4c0a 2020 2020  o Cloud SQL.    
-000046a0: 6173 796e 6320 6465 6620 6765 7463 6f6e  async def getcon
-000046b0: 6e28 2920 2d3e 2061 7379 6e63 7067 2e43  n() -> asyncpg.C
-000046c0: 6f6e 6e65 6374 696f 6e3a 0a20 2020 2020  onnection:.     
-000046d0: 2020 2063 6f6e 6e3a 2061 7379 6e63 7067     conn: asyncpg
-000046e0: 2e43 6f6e 6e65 6374 696f 6e20 3d20 6177  .Connection = aw
-000046f0: 6169 7420 636f 6e6e 6563 746f 722e 636f  ait connector.co
-00004700: 6e6e 6563 745f 6173 796e 6328 0a20 2020  nnect_async(.   
-00004710: 2020 2020 2020 2020 2022 7072 6f6a 6563           "projec
-00004720: 743a 7265 6769 6f6e 3a69 6e73 7461 6e63  t:region:instanc
-00004730: 6522 2c20 2023 2043 6c6f 7564 2053 514c  e",  # Cloud SQL
-00004740: 2069 6e73 7461 6e63 6520 636f 6e6e 6563   instance connec
-00004750: 7469 6f6e 206e 616d 650a 2020 2020 2020  tion name.      
-00004760: 2020 2020 2020 2261 7379 6e63 7067 222c        "asyncpg",
-00004770: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
-00004780: 723d 226d 792d 7573 6572 222c 0a20 2020  r="my-user",.   
-00004790: 2020 2020 2020 2020 2070 6173 7377 6f72           passwor
-000047a0: 643d 226d 792d 7061 7373 776f 7264 222c  d="my-password",
-000047b0: 0a20 2020 2020 2020 2020 2020 2064 623d  .            db=
-000047c0: 226d 792d 6462 2d6e 616d 6522 0a20 2020  "my-db-name".   
-000047d0: 2020 2020 2020 2020 2023 202e 2e2e 2061           # ... a
-000047e0: 6464 6974 696f 6e61 6c20 6461 7461 6261  dditional databa
-000047f0: 7365 2064 7269 7665 7220 6172 6773 0a20  se driver args. 
-00004800: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00004810: 2072 6574 7572 6e20 636f 6e6e 0a0a 2020   return conn..  
-00004820: 2020 2320 5468 6520 436c 6f75 6420 5351    # The Cloud SQ
-00004830: 4c20 5079 7468 6f6e 2043 6f6e 6e65 6374  L Python Connect
-00004840: 6f72 2063 616e 2062 6520 7573 6564 2061  or can be used a
-00004850: 6c6f 6e67 2077 6974 6820 5351 4c41 6c63  long with SQLAlc
-00004860: 6865 6d79 2075 7369 6e67 2074 6865 0a20  hemy using the. 
-00004870: 2020 2023 2027 6173 796e 635f 6372 6561     # 'async_crea
-00004880: 746f 7227 2061 7267 756d 656e 7420 746f  tor' argument to
-00004890: 2027 6372 6561 7465 5f61 7379 6e63 5f65   'create_async_e
-000048a0: 6e67 696e 6527 0a20 2020 2070 6f6f 6c20  ngine'.    pool 
-000048b0: 3d20 6372 6561 7465 5f61 7379 6e63 5f65  = create_async_e
-000048c0: 6e67 696e 6528 0a20 2020 2020 2020 2022  ngine(.        "
-000048d0: 706f 7374 6772 6573 716c 2b61 7379 6e63  postgresql+async
-000048e0: 7067 3a2f 2f22 2c0a 2020 2020 2020 2020  pg://",.        
-000048f0: 6173 796e 635f 6372 6561 746f 723d 6765  async_creator=ge
-00004900: 7463 6f6e 6e2c 0a20 2020 2029 0a20 2020  tconn,.    ).   
-00004910: 2072 6574 7572 6e20 706f 6f6c 0a0a 6173   return pool..as
-00004920: 796e 6320 6465 6620 6d61 696e 2829 3a0a  ync def main():.
-00004930: 2020 2020 2320 696e 6974 6961 6c69 7a65      # initialize
-00004940: 2043 6f6e 6e65 6374 6f72 206f 626a 6563   Connector objec
-00004950: 7420 666f 7220 636f 6e6e 6563 7469 6f6e  t for connection
-00004960: 7320 746f 2043 6c6f 7564 2053 514c 0a20  s to Cloud SQL. 
-00004970: 2020 2063 6f6e 6e65 6374 6f72 203d 2061     connector = a
-00004980: 7761 6974 2063 7265 6174 655f 6173 796e  wait create_asyn
-00004990: 635f 636f 6e6e 6563 746f 7228 290a 0a20  c_connector().. 
-000049a0: 2020 2023 2069 6e69 7469 616c 697a 6520     # initialize 
-000049b0: 636f 6e6e 6563 7469 6f6e 2070 6f6f 6c0a  connection pool.
-000049c0: 2020 2020 706f 6f6c 203d 2061 7761 6974      pool = await
-000049d0: 2069 6e69 745f 636f 6e6e 6563 7469 6f6e   init_connection
-000049e0: 5f70 6f6f 6c28 636f 6e6e 6563 746f 7229  _pool(connector)
-000049f0: 0a0a 2020 2020 2320 6578 616d 706c 6520  ..    # example 
-00004a00: 7175 6572 790a 2020 2020 6173 796e 6320  query.    async 
-00004a10: 7769 7468 2070 6f6f 6c2e 636f 6e6e 6563  with pool.connec
-00004a20: 7428 2920 6173 2063 6f6e 6e3a 0a20 2020  t() as conn:.   
-00004a30: 2020 2020 2061 7761 6974 2063 6f6e 6e2e       await conn.
-00004a40: 6578 6563 7574 6528 7371 6c61 6c63 6865  execute(sqlalche
-00004a50: 6d79 2e74 6578 7428 2253 454c 4543 5420  my.text("SELECT 
-00004a60: 4e4f 5728 2922 2929 0a0a 2020 2020 2320  NOW()"))..    # 
-00004a70: 636c 6f73 6520 436f 6e6e 6563 746f 720a  close Connector.
-00004a80: 2020 2020 6177 6169 7420 636f 6e6e 6563      await connec
-00004a90: 746f 722e 636c 6f73 655f 6173 796e 6328  tor.close_async(
-00004aa0: 290a 0a20 2020 2023 2064 6973 706f 7365  )..    # dispose
-00004ab0: 206f 6620 636f 6e6e 6563 7469 6f6e 2070   of connection p
-00004ac0: 6f6f 6c0a 2020 2020 6177 6169 7420 706f  ool.    await po
-00004ad0: 6f6c 2e64 6973 706f 7365 2829 0a60 6060  ol.dispose().```
-00004ae0: 0a0a 466f 7220 6d6f 7265 2064 6574 6169  ..For more detai
-00004af0: 6c73 206f 6e20 6164 6469 7469 6f6e 616c  ls on additional
-00004b00: 2064 6174 6162 6173 6520 6172 6775 6d65   database argume
-00004b10: 6e74 7320 7769 7468 2061 6e20 6061 7379  nts with an `asy
-00004b20: 6e63 7067 2e43 6f6e 6e65 6374 696f 6e60  ncpg.Connection`
-00004b30: 0a2c 2070 6c65 6173 6520 7669 7369 7420  ., please visit 
-00004b40: 7468 650a 5b6f 6666 6963 6961 6c20 646f  the.[official do
-00004b50: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
-00004b60: 7073 3a2f 2f6d 6167 6963 7374 6163 6b2e  ps://magicstack.
-00004b70: 6769 7468 7562 2e69 6f2f 6173 796e 6370  github.io/asyncp
-00004b80: 672f 6375 7272 656e 742f 6170 692f 696e  g/current/api/in
-00004b90: 6465 782e 6874 6d6c 292e 0a0a 2323 2320  dex.html)...### 
-00004ba0: 4173 796e 6320 436f 6e74 6578 7420 4d61  Async Context Ma
-00004bb0: 6e61 6765 720a 0a41 6e20 616c 7465 726e  nager..An altern
-00004bc0: 6174 6976 6520 746f 2075 7369 6e67 2074  ative to using t
-00004bd0: 6865 2060 6372 6561 7465 5f61 7379 6e63  he `create_async
-00004be0: 5f63 6f6e 6e65 6374 6f72 6020 6675 6e63  _connector` func
-00004bf0: 7469 6f6e 2069 7320 696e 6974 6961 6c69  tion is initiali
-00004c00: 7a69 6e67 0a61 2060 436f 6e6e 6563 746f  zing.a `Connecto
-00004c10: 7260 2061 7320 616e 2061 7379 6e63 2063  r` as an async c
-00004c20: 6f6e 7465 7874 206d 616e 6167 6572 2c20  ontext manager, 
-00004c30: 7265 6d6f 7669 6e67 2074 6865 206e 6565  removing the nee
-00004c40: 6420 666f 7220 6578 706c 6963 6974 0a63  d for explicit.c
-00004c50: 616c 6c73 2074 6f20 6063 6f6e 6e65 6374  alls to `connect
-00004c60: 6f72 2e63 6c6f 7365 5f61 7379 6e63 2829  or.close_async()
-00004c70: 6020 746f 2063 6c65 616e 7570 2072 6573  ` to cleanup res
-00004c80: 6f75 7263 6573 2e0a 0a2a 2a4e 6f74 653a  ources...**Note:
-00004c90: 2a2a 2054 6869 7320 616c 7465 726e 6174  ** This alternat
-00004ca0: 6976 6520 7265 7175 6972 6573 2074 6861  ive requires tha
-00004cb0: 7420 7468 6520 7275 6e6e 696e 6720 6576  t the running ev
-00004cc0: 656e 7420 6c6f 6f70 2062 650a 7061 7373  ent loop be.pass
-00004cd0: 6564 2069 6e20 6173 2074 6865 2060 6c6f  ed in as the `lo
-00004ce0: 6f70 6020 6172 6775 6d65 6e74 2074 6f20  op` argument to 
-00004cf0: 6043 6f6e 6e65 6374 6f72 2829 602e 0a0a  `Connector()`...
-00004d00: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
-00004d10: 2061 7379 6e63 696f 0a69 6d70 6f72 7420   asyncio.import 
-00004d20: 6173 796e 6370 670a 0a69 6d70 6f72 7420  asyncpg..import 
-00004d30: 7371 6c61 6c63 6865 6d79 0a66 726f 6d20  sqlalchemy.from 
-00004d40: 7371 6c61 6c63 6865 6d79 2e65 7874 2e61  sqlalchemy.ext.a
-00004d50: 7379 6e63 696f 2069 6d70 6f72 7420 4173  syncio import As
-00004d60: 796e 6345 6e67 696e 652c 2063 7265 6174  yncEngine, creat
-00004d70: 655f 6173 796e 635f 656e 6769 6e65 0a0a  e_async_engine..
-00004d80: 6672 6f6d 2067 6f6f 676c 652e 636c 6f75  from google.clou
-00004d90: 642e 7371 6c2e 636f 6e6e 6563 746f 7220  d.sql.connector 
-00004da0: 696d 706f 7274 2043 6f6e 6e65 6374 6f72  import Connector
-00004db0: 0a0a 6173 796e 6320 6465 6620 696e 6974  ..async def init
-00004dc0: 5f63 6f6e 6e65 6374 696f 6e5f 706f 6f6c  _connection_pool
-00004dd0: 2863 6f6e 6e65 6374 6f72 3a20 436f 6e6e  (connector: Conn
-00004de0: 6563 746f 7229 202d 3e20 4173 796e 6345  ector) -> AsyncE
-00004df0: 6e67 696e 653a 0a20 2020 2023 2069 6e69  ngine:.    # ini
-00004e00: 7469 616c 697a 6520 436f 6e6e 6563 746f  tialize Connecto
-00004e10: 7220 6f62 6a65 6374 2066 6f72 2063 6f6e  r object for con
-00004e20: 6e65 6374 696f 6e73 2074 6f20 436c 6f75  nections to Clou
-00004e30: 6420 5351 4c0a 2020 2020 6173 796e 6320  d SQL.    async 
-00004e40: 6465 6620 6765 7463 6f6e 6e28 2920 2d3e  def getconn() ->
-00004e50: 2061 7379 6e63 7067 2e43 6f6e 6e65 6374   asyncpg.Connect
-00004e60: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-00004e70: 2063 6f6e 6e3a 2061 7379 6e63 7067 2e43   conn: asyncpg.C
-00004e80: 6f6e 6e65 6374 696f 6e20 3d20 6177 6169  onnection = awai
-00004e90: 7420 636f 6e6e 6563 746f 722e 636f 6e6e  t connector.conn
-00004ea0: 6563 745f 6173 796e 6328 0a20 2020 2020  ect_async(.     
-00004eb0: 2020 2020 2020 2020 2020 2022 7072 6f6a             "proj
-00004ec0: 6563 743a 7265 6769 6f6e 3a69 6e73 7461  ect:region:insta
-00004ed0: 6e63 6522 2c20 2023 2043 6c6f 7564 2053  nce",  # Cloud S
-00004ee0: 514c 2069 6e73 7461 6e63 6520 636f 6e6e  QL instance conn
-00004ef0: 6563 7469 6f6e 206e 616d 650a 2020 2020  ection name.    
-00004f00: 2020 2020 2020 2020 2020 2020 2261 7379              "asy
-00004f10: 6e63 7067 222c 0a20 2020 2020 2020 2020  ncpg",.         
-00004f20: 2020 2020 2020 2075 7365 723d 226d 792d         user="my-
-00004f30: 7573 6572 222c 0a20 2020 2020 2020 2020  user",.         
-00004f40: 2020 2020 2020 2070 6173 7377 6f72 643d         password=
-00004f50: 226d 792d 7061 7373 776f 7264 222c 0a20  "my-password",. 
-00004f60: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004f70: 623d 226d 792d 6462 2d6e 616d 6522 0a20  b="my-db-name". 
-00004f80: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00004f90: 202e 2e2e 2061 6464 6974 696f 6e61 6c20   ... additional 
-00004fa0: 6461 7461 6261 7365 2064 7269 7665 7220  database driver 
-00004fb0: 6172 6773 0a20 2020 2020 2020 2020 2020  args.           
-00004fc0: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
-00004fd0: 6574 7572 6e20 636f 6e6e 0a0a 2020 2020  eturn conn..    
-00004fe0: 2320 5468 6520 436c 6f75 6420 5351 4c20  # The Cloud SQL 
-00004ff0: 5079 7468 6f6e 2043 6f6e 6e65 6374 6f72  Python Connector
-00005000: 2063 616e 2062 6520 7573 6564 2061 6c6f   can be used alo
-00005010: 6e67 2077 6974 6820 5351 4c41 6c63 6865  ng with SQLAlche
-00005020: 6d79 2075 7369 6e67 2074 6865 0a20 2020  my using the.   
-00005030: 2023 2027 6173 796e 635f 6372 6561 746f   # 'async_creato
-00005040: 7227 2061 7267 756d 656e 7420 746f 2027  r' argument to '
-00005050: 6372 6561 7465 5f61 7379 6e63 5f65 6e67  create_async_eng
-00005060: 696e 6527 0a20 2020 2070 6f6f 6c20 3d20  ine'.    pool = 
-00005070: 6372 6561 7465 5f61 7379 6e63 5f65 6e67  create_async_eng
-00005080: 696e 6528 0a20 2020 2020 2020 2022 706f  ine(.        "po
-00005090: 7374 6772 6573 716c 2b61 7379 6e63 7067  stgresql+asyncpg
-000050a0: 3a2f 2f22 2c0a 2020 2020 2020 2020 6173  ://",.        as
-000050b0: 796e 635f 6372 6561 746f 723d 6765 7463  ync_creator=getc
-000050c0: 6f6e 6e2c 0a20 2020 2029 0a20 2020 2072  onn,.    ).    r
-000050d0: 6574 7572 6e20 706f 6f6c 0a0a 6173 796e  eturn pool..asyn
-000050e0: 6320 6465 6620 6d61 696e 2829 3a0a 2020  c def main():.  
-000050f0: 2020 2320 696e 6974 6961 6c69 7a65 2043    # initialize C
-00005100: 6f6e 6e65 6374 6f72 206f 626a 6563 7420  onnector object 
-00005110: 666f 7220 636f 6e6e 6563 7469 6f6e 7320  for connections 
-00005120: 746f 2043 6c6f 7564 2053 514c 0a20 2020  to Cloud SQL.   
-00005130: 206c 6f6f 7020 3d20 6173 796e 6369 6f2e   loop = asyncio.
-00005140: 6765 745f 7275 6e6e 696e 675f 6c6f 6f70  get_running_loop
-00005150: 2829 0a20 2020 2061 7379 6e63 2077 6974  ().    async wit
-00005160: 6820 436f 6e6e 6563 746f 7228 6c6f 6f70  h Connector(loop
-00005170: 3d6c 6f6f 7029 2061 7320 636f 6e6e 6563  =loop) as connec
-00005180: 746f 723a 0a20 2020 2020 2020 2023 2069  tor:.        # i
-00005190: 6e69 7469 616c 697a 6520 636f 6e6e 6563  nitialize connec
-000051a0: 7469 6f6e 2070 6f6f 6c0a 2020 2020 2020  tion pool.      
-000051b0: 2020 706f 6f6c 203d 2061 7761 6974 2069    pool = await i
-000051c0: 6e69 745f 636f 6e6e 6563 7469 6f6e 5f70  nit_connection_p
-000051d0: 6f6f 6c28 636f 6e6e 6563 746f 7229 0a0a  ool(connector)..
-000051e0: 2020 2020 2020 2020 2320 6578 616d 706c          # exampl
-000051f0: 6520 7175 6572 790a 2020 2020 2020 2020  e query.        
-00005200: 6173 796e 6320 7769 7468 2070 6f6f 6c2e  async with pool.
-00005210: 636f 6e6e 6563 7428 2920 6173 2063 6f6e  connect() as con
-00005220: 6e3a 0a20 2020 2020 2020 2020 2020 2061  n:.            a
-00005230: 7761 6974 2063 6f6e 6e2e 6578 6563 7574  wait conn.execut
-00005240: 6528 7371 6c61 6c63 6865 6d79 2e74 6578  e(sqlalchemy.tex
-00005250: 7428 2253 454c 4543 5420 4e4f 5728 2922  t("SELECT NOW()"
-00005260: 2929 0a0a 2020 2020 2020 2020 2320 6469  ))..        # di
-00005270: 7370 6f73 6520 6f66 2063 6f6e 6e65 6374  spose of connect
-00005280: 696f 6e20 706f 6f6c 0a20 2020 2020 2020  ion pool.       
-00005290: 2061 7761 6974 2070 6f6f 6c2e 6469 7370   await pool.disp
-000052a0: 6f73 6528 290a 6060 600a 0a23 2320 5375  ose().```..## Su
-000052b0: 7070 6f72 7420 706f 6c69 6379 0a0a 2323  pport policy..##
-000052c0: 2320 4d61 6a6f 7220 7665 7273 696f 6e20  # Major version 
-000052d0: 6c69 6665 6379 636c 650a 0a54 6869 7320  lifecycle..This 
-000052e0: 7072 6f6a 6563 7420 7573 6573 205b 7365  project uses [se
-000052f0: 6d61 6e74 6963 2076 6572 7369 6f6e 696e  mantic versionin
-00005300: 675d 2868 7474 7073 3a2f 2f73 656d 7665  g](https://semve
-00005310: 722e 6f72 672f 292c 2061 6e64 2075 7365  r.org/), and use
-00005320: 7320 7468 650a 666f 6c6c 6f77 696e 6720  s the.following 
-00005330: 6c69 6665 6379 636c 6520 7265 6761 7264  lifecycle regard
-00005340: 696e 6720 7375 7070 6f72 7420 666f 7220  ing support for 
-00005350: 6120 6d61 6a6f 7220 7665 7273 696f 6e3a  a major version:
-00005360: 0a0a 2a2a 4163 7469 7665 2a2a 202d 2041  ..**Active** - A
-00005370: 6374 6976 6520 7665 7273 696f 6e73 2067  ctive versions g
-00005380: 6574 2061 6c6c 206e 6577 2066 6561 7475  et all new featu
-00005390: 7265 7320 616e 6420 7365 6375 7269 7479  res and security
-000053a0: 2066 6978 6573 2028 7468 6174 0a77 6f75   fixes (that.wou
-000053b0: 6c64 6ee2 8099 7420 6f74 6865 7277 6973  ldn...t otherwis
-000053c0: 6520 696e 7472 6f64 7563 6520 6120 6272  e introduce a br
-000053d0: 6561 6b69 6e67 2063 6861 6e67 6529 2e20  eaking change). 
-000053e0: 4e65 7720 6d61 6a6f 7220 7665 7273 696f  New major versio
-000053f0: 6e73 2061 7265 0a67 7561 7261 6e74 6565  ns are.guarantee
-00005400: 6420 746f 2062 6520 2261 6374 6976 6522  d to be "active"
-00005410: 2066 6f72 2061 206d 696e 696d 756d 206f   for a minimum o
-00005420: 6620 3120 7965 6172 2e0a 2a2a 4465 7072  f 1 year..**Depr
-00005430: 6563 6174 6564 2a2a 202d 2044 6570 7265  ecated** - Depre
-00005440: 6361 7465 6420 7665 7273 696f 6e73 2063  cated versions c
-00005450: 6f6e 7469 6e75 6520 746f 2072 6563 6569  ontinue to recei
-00005460: 7665 2073 6563 7572 6974 7920 616e 6420  ve security and 
-00005470: 6372 6974 6963 616c 0a62 7567 2066 6978  critical.bug fix
-00005480: 6573 2c20 6275 7420 646f 206e 6f74 2072  es, but do not r
-00005490: 6563 6569 7665 206e 6577 2066 6561 7475  eceive new featu
-000054a0: 7265 732e 2044 6570 7265 6361 7465 6420  res. Deprecated 
-000054b0: 7665 7273 696f 6e73 2077 696c 6c20 6265  versions will be
-000054c0: 2070 7562 6c69 636c 790a 7375 7070 6f72   publicly.suppor
-000054d0: 7465 6420 666f 7220 3120 7965 6172 2e0a  ted for 1 year..
-000054e0: 2a2a 556e 7375 7070 6f72 7465 642a 2a20  **Unsupported** 
-000054f0: 2d20 416e 7920 6d61 6a6f 7220 7665 7273  - Any major vers
-00005500: 696f 6e20 7468 6174 2068 6173 2062 6565  ion that has bee
-00005510: 6e20 6465 7072 6563 6174 6564 2066 6f72  n deprecated for
-00005520: 203e 3d31 2079 6561 7220 6973 0a63 6f6e   >=1 year is.con
-00005530: 7369 6465 7265 6420 7075 626c 6963 6c79  sidered publicly
-00005540: 2075 6e73 7570 706f 7274 6564 2e0a 0a23   unsupported...#
-00005550: 2320 5375 7070 6f72 7465 6420 5079 7468  # Supported Pyth
-00005560: 6f6e 2056 6572 7369 6f6e 730a 0a57 6520  on Versions..We 
-00005570: 7465 7374 2061 6e64 2073 7570 706f 7274  test and support
-00005580: 2061 7420 6120 6d69 6e69 6d75 6d2c 2065   at a minimum, e
-00005590: 7665 7279 205b 6163 7469 7665 2076 6572  very [active ver
-000055a0: 7369 6f6e 2075 6e74 696c 2069 7427 730a  sion until it's.
-000055b0: 656e 642d 6f66 2d6c 6966 6520 6461 7465  end-of-life date
-000055c0: 5d5b 7079 7665 725d 2e20 4368 616e 6765  ][pyver]. Change
-000055d0: 7320 696e 2073 7570 706f 7274 6564 2050  s in supported P
-000055e0: 7974 686f 6e20 7665 7273 696f 6e73 2077  ython versions w
-000055f0: 696c 6c20 6265 0a63 6f6e 7369 6465 7265  ill be.considere
-00005600: 6420 6120 6d69 6e6f 7220 6368 616e 6765  d a minor change
-00005610: 2c20 616e 6420 7769 6c6c 2062 6520 6c69  , and will be li
-00005620: 7374 6564 2069 6e20 7468 6520 7265 6c65  sted in the rele
-00005630: 6173 6520 6e6f 7465 732e 0a0a 5b70 7976  ase notes...[pyv
-00005640: 6572 5d3a 2068 7474 7073 3a2f 2f64 6576  er]: https://dev
-00005650: 6775 6964 652e 7079 7468 6f6e 2e6f 7267  guide.python.org
-00005660: 2f23 7374 6174 7573 2d6f 662d 7079 7468  /#status-of-pyth
-00005670: 6f6e 2d62 7261 6e63 6865 730a 0a23 2323  on-branches..###
-00005680: 2052 656c 6561 7365 2063 6164 656e 6365   Release cadence
-00005690: 0a54 6869 7320 7072 6f6a 6563 7420 6169  .This project ai
-000056a0: 6d73 2066 6f72 2061 206d 696e 696d 756d  ms for a minimum
-000056b0: 206d 6f6e 7468 6c79 2072 656c 6561 7365   monthly release
-000056c0: 2063 6164 656e 6365 2e20 4966 206e 6f20   cadence. If no 
-000056d0: 6e65 770a 6665 6174 7572 6573 206f 7220  new.features or 
-000056e0: 6669 7865 7320 6861 7665 2062 6565 6e20  fixes have been 
-000056f0: 6164 6465 642c 2061 206e 6577 2050 4154  added, a new PAT
-00005700: 4348 2076 6572 7369 6f6e 2077 6974 6820  CH version with 
-00005710: 7468 6520 6c61 7465 7374 0a64 6570 656e  the latest.depen
-00005720: 6465 6e63 6965 7320 6973 2072 656c 6561  dencies is relea
-00005730: 7365 642e 0a0a 2323 2320 436f 6e74 7269  sed...### Contri
-00005740: 6275 7469 6e67 0a0a 5765 2077 656c 636f  buting..We welco
-00005750: 6d65 206f 7574 7369 6465 2063 6f6e 7472  me outside contr
-00005760: 6962 7574 696f 6e73 2e20 506c 6561 7365  ibutions. Please
-00005770: 2073 6565 206f 7572 0a5b 436f 6e74 7269   see our.[Contri
-00005780: 6275 7469 6e67 2047 7569 6465 5d28 434f  buting Guide](CO
-00005790: 4e54 5249 4255 5449 4e47 2e6d 6429 2066  NTRIBUTING.md) f
-000057a0: 6f72 2064 6574 6169 6c73 206f 6e20 686f  or details on ho
-000057b0: 7720 6265 7374 2074 6f20 636f 6e74 7269  w best to contri
-000057c0: 6275 7465 2e0a                           bute..
+00000360: 3130 0a43 6c61 7373 6966 6965 723a 2050  10.Classifier: P
+00000370: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000380: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000390: 2033 2e31 310a 5265 7175 6972 6573 2d50   3.11.Requires-P
+000003a0: 7974 686f 6e3a 203e 3d33 2e38 0a44 6573  ython: >=3.8.Des
+000003b0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+000003c0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+000003d0: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
+000003e0: 7472 613a 2070 796d 7973 716c 0a50 726f  tra: pymysql.Pro
+000003f0: 7669 6465 732d 4578 7472 613a 2070 6738  vides-Extra: pg8
+00000400: 3030 300a 5072 6f76 6964 6573 2d45 7874  000.Provides-Ext
+00000410: 7261 3a20 7079 7464 730a 5072 6f76 6964  ra: pytds.Provid
+00000420: 6573 2d45 7874 7261 3a20 6173 796e 6370  es-Extra: asyncp
+00000430: 670a 4c69 6365 6e73 652d 4669 6c65 3a20  g.License-File: 
+00000440: 4c49 4345 4e53 450a 0a3c 7020 616c 6967  LICENSE..<p alig
+00000450: 6e3d 2263 656e 7465 7222 3e0a 2020 2020  n="center">.    
+00000460: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000470: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
+00000480: 6d2f 626c 6f67 2f74 6f70 6963 732f 6465  m/blog/topics/de
+00000490: 7665 6c6f 7065 7273 2d70 7261 6374 6974  velopers-practit
+000004a0: 696f 6e65 7273 2f68 6f77 2d63 6f6e 6e65  ioners/how-conne
+000004b0: 6374 2d63 6c6f 7564 2d73 716c 2d75 7369  ct-cloud-sql-usi
+000004c0: 6e67 2d70 7974 686f 6e2d 6561 7379 2d77  ng-python-easy-w
+000004d0: 6179 223e 0a20 2020 2020 2020 203c 696d  ay">.        <im
+000004e0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+000004f0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00000500: 7465 6e74 2e63 6f6d 2f47 6f6f 676c 6543  tent.com/GoogleC
+00000510: 6c6f 7564 506c 6174 666f 726d 2f63 6c6f  loudPlatform/clo
+00000520: 7564 2d73 716c 2d70 7974 686f 6e2d 636f  ud-sql-python-co
+00000530: 6e6e 6563 746f 722f 6d61 696e 2f64 6f63  nnector/main/doc
+00000540: 732f 696d 6167 6573 2f63 6c6f 7564 2d73  s/images/cloud-s
+00000550: 716c 2d70 7974 686f 6e2d 636f 6e6e 6563  ql-python-connec
+00000560: 746f 722e 706e 6722 2061 6c74 3d22 636c  tor.png" alt="cl
+00000570: 6f75 642d 7371 6c2d 7079 7468 6f6e 2d63  oud-sql-python-c
+00000580: 6f6e 6e65 6374 6f72 2069 6d61 6765 223e  onnector image">
+00000590: 0a20 2020 203c 2f61 3e0a 3c2f 703e 0a0a  .    </a>.</p>..
+000005a0: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+000005b0: 7222 3e43 6c6f 7564 2053 514c 2050 7974  r">Cloud SQL Pyt
+000005c0: 686f 6e20 436f 6e6e 6563 746f 723c 2f68  hon Connector</h
+000005d0: 313e 0a0a 5b21 5b4f 7065 6e20 496e 2043  1>..[![Open In C
+000005e0: 6f6c 6162 5d5b 636f 6c61 622d 6261 6467  olab][colab-badg
+000005f0: 655d 5d5b 636f 6c61 622d 6e6f 7465 626f  e]][colab-notebo
+00000600: 6f6b 5d0a 5b21 5b43 495d 5b63 692d 6261  ok].[![CI][ci-ba
+00000610: 6467 655d 5d5b 6369 2d62 7569 6c64 5d0a  dge]][ci-build].
+00000620: 5b21 5b70 7970 695d 5b70 7970 692d 6261  [![pypi][pypi-ba
+00000630: 6467 655d 5d5b 7079 7069 2d64 6f63 735d  dge]][pypi-docs]
+00000640: 0a5b 215b 5079 5049 2064 6f77 6e6c 6f61  .[![PyPI downloa
+00000650: 6420 6d6f 6e74 685d 5b70 7970 692d 646f  d month][pypi-do
+00000660: 776e 6c6f 6164 735d 5d5b 7079 7069 2d64  wnloads]][pypi-d
+00000670: 6f63 735d 0a5b 215b 7079 7468 6f6e 5d5b  ocs].[![python][
+00000680: 7079 7468 6f6e 2d76 6572 7369 6f6e 735d  python-versions]
+00000690: 5d5b 7079 7069 2d64 6f63 735d 0a0a 5b63  ][pypi-docs]..[c
+000006a0: 6f6c 6162 2d62 6164 6765 5d3a 2068 7474  olab-badge]: htt
+000006b0: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+000006c0: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f61  rch.google.com/a
+000006d0: 7373 6574 732f 636f 6c61 622d 6261 6467  ssets/colab-badg
+000006e0: 652e 7376 670a 5b63 6f6c 6162 2d6e 6f74  e.svg.[colab-not
+000006f0: 6562 6f6f 6b5d 3a20 6874 7470 733a 2f2f  ebook]: https://
+00000700: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+00000710: 6f6f 676c 652e 636f 6d2f 6769 7468 7562  oogle.com/github
+00000720: 2f47 6f6f 676c 6543 6c6f 7564 506c 6174  /GoogleCloudPlat
+00000730: 666f 726d 2f63 6c6f 7564 2d73 716c 2d70  form/cloud-sql-p
+00000740: 7974 686f 6e2d 636f 6e6e 6563 746f 722f  ython-connector/
+00000750: 626c 6f62 2f6d 6169 6e2f 7361 6d70 6c65  blob/main/sample
+00000760: 732f 6e6f 7465 626f 6f6b 732f 706f 7374  s/notebooks/post
+00000770: 6772 6573 5f70 7974 686f 6e5f 636f 6e6e  gres_python_conn
+00000780: 6563 746f 722e 6970 796e 620a 5b63 692d  ector.ipynb.[ci-
+00000790: 6261 6467 655d 3a20 6874 7470 733a 2f2f  badge]: https://
+000007a0: 6769 7468 7562 2e63 6f6d 2f47 6f6f 676c  github.com/Googl
+000007b0: 6543 6c6f 7564 506c 6174 666f 726d 2f63  eCloudPlatform/c
+000007c0: 6c6f 7564 2d73 716c 2d70 7974 686f 6e2d  loud-sql-python-
+000007d0: 636f 6e6e 6563 746f 722f 6163 7469 6f6e  connector/action
+000007e0: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
+000007f0: 732e 796d 6c2f 6261 6467 652e 7376 673f  s.yml/badge.svg?
+00000800: 6576 656e 743d 7075 7368 0a5b 6369 2d62  event=push.[ci-b
+00000810: 7569 6c64 5d3a 2068 7474 7073 3a2f 2f67  uild]: https://g
+00000820: 6974 6875 622e 636f 6d2f 476f 6f67 6c65  ithub.com/Google
+00000830: 436c 6f75 6450 6c61 7466 6f72 6d2f 636c  CloudPlatform/cl
+00000840: 6f75 642d 7371 6c2d 7079 7468 6f6e 2d63  oud-sql-python-c
+00000850: 6f6e 6e65 6374 6f72 2f61 6374 696f 6e73  onnector/actions
+00000860: 2f77 6f72 6b66 6c6f 7773 2f74 6573 7473  /workflows/tests
+00000870: 2e79 6d6c 3f71 7565 7279 3d65 7665 6e74  .yml?query=event
+00000880: 2533 4170 7573 682b 6272 616e 6368 2533  %3Apush+branch%3
+00000890: 416d 6169 6e0a 5b70 7970 692d 6261 6467  Amain.[pypi-badg
+000008a0: 655d 3a20 6874 7470 733a 2f2f 696d 672e  e]: https://img.
+000008b0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+000008c0: 762f 636c 6f75 642d 7371 6c2d 7079 7468  v/cloud-sql-pyth
+000008d0: 6f6e 2d63 6f6e 6e65 6374 6f72 0a5b 7079  on-connector.[py
+000008e0: 7069 2d64 6f63 735d 3a20 6874 7470 733a  pi-docs]: https:
+000008f0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000900: 6374 2f63 6c6f 7564 2d73 716c 2d70 7974  ct/cloud-sql-pyt
+00000910: 686f 6e2d 636f 6e6e 6563 746f 720a 5b70  hon-connector.[p
+00000920: 7970 692d 646f 776e 6c6f 6164 735d 3a20  ypi-downloads]: 
+00000930: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000940: 6c64 732e 696f 2f70 7970 692f 646d 2f63  lds.io/pypi/dm/c
+00000950: 6c6f 7564 2d73 716c 2d70 7974 686f 6e2d  loud-sql-python-
+00000960: 636f 6e6e 6563 746f 722e 7376 670a 5b70  connector.svg.[p
+00000970: 7974 686f 6e2d 7665 7273 696f 6e73 5d3a  ython-versions]:
+00000980: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
+00000990: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
+000009a0: 6572 7369 6f6e 732f 636c 6f75 642d 7371  ersions/cloud-sq
+000009b0: 6c2d 7079 7468 6f6e 2d63 6f6e 6e65 6374  l-python-connect
+000009c0: 6f72 0a0a 5468 6520 5f43 6c6f 7564 2053  or..The _Cloud S
+000009d0: 514c 2050 7974 686f 6e20 436f 6e6e 6563  QL Python Connec
+000009e0: 746f 725f 2069 7320 6120 436c 6f75 6420  tor_ is a Cloud 
+000009f0: 5351 4c20 636f 6e6e 6563 746f 7220 6465  SQL connector de
+00000a00: 7369 676e 6564 2066 6f72 2075 7365 2077  signed for use w
+00000a10: 6974 6820 7468 650a 5079 7468 6f6e 206c  ith the.Python l
+00000a20: 616e 6775 6167 652e 2055 7369 6e67 2061  anguage. Using a
+00000a30: 2043 6c6f 7564 2053 514c 2063 6f6e 6e65   Cloud SQL conne
+00000a40: 6374 6f72 2070 726f 7669 6465 7320 6120  ctor provides a 
+00000a50: 6e61 7469 7665 2061 6c74 6572 6e61 7469  native alternati
+00000a60: 7665 2074 6f20 7468 650a 5b43 6c6f 7564  ve to the.[Cloud
+00000a70: 2053 514c 2041 7574 6820 5072 6f78 795d   SQL Auth Proxy]
+00000a80: 2868 7474 7073 3a2f 2f63 6c6f 7564 2e67  (https://cloud.g
+00000a90: 6f6f 676c 652e 636f 6d2f 7371 6c2f 646f  oogle.com/sql/do
+00000aa0: 6373 2f6d 7973 716c 2f73 716c 2d70 726f  cs/mysql/sql-pro
+00000ab0: 7879 2920 7768 696c 650a 7072 6f76 6964  xy) while.provid
+00000ac0: 696e 6720 7468 6520 666f 6c6c 6f77 696e  ing the followin
+00000ad0: 6720 6265 6e65 6669 7473 3a0a 0a2a 202a  g benefits:..* *
+00000ae0: 2a49 414d 2041 7574 686f 7269 7a61 7469  *IAM Authorizati
+00000af0: 6f6e 3a2a 2a20 7573 6573 2049 414d 2070  on:** uses IAM p
+00000b00: 6572 6d69 7373 696f 6e73 2074 6f20 636f  ermissions to co
+00000b10: 6e74 726f 6c20 7768 6f2f 7768 6174 2063  ntrol who/what c
+00000b20: 616e 2063 6f6e 6e65 6374 2074 6f0a 2020  an connect to.  
+00000b30: 796f 7572 2043 6c6f 7564 2053 514c 2069  your Cloud SQL i
+00000b40: 6e73 7461 6e63 6573 0a2a 202a 2a49 6d70  nstances.* **Imp
+00000b50: 726f 7665 6420 5365 6375 7269 7479 3a2a  roved Security:*
+00000b60: 2a20 7573 6573 2072 6f62 7573 742c 2075  * uses robust, u
+00000b70: 7064 6174 6564 2054 4c53 2031 2e33 2065  pdated TLS 1.3 e
+00000b80: 6e63 7279 7074 696f 6e20 616e 640a 2020  ncryption and.  
+00000b90: 6964 656e 7469 7479 2076 6572 6966 6963  identity verific
+00000ba0: 6174 696f 6e20 6265 7477 6565 6e20 7468  ation between th
+00000bb0: 6520 636c 6965 6e74 2063 6f6e 6e65 6374  e client connect
+00000bc0: 6f72 2061 6e64 2074 6865 2073 6572 7665  or and the serve
+00000bd0: 722d 7369 6465 2070 726f 7879 2c0a 2020  r-side proxy,.  
+00000be0: 696e 6465 7065 6e64 656e 7420 6f66 2074  independent of t
+00000bf0: 6865 2064 6174 6162 6173 6520 7072 6f74  he database prot
+00000c00: 6f63 6f6c 2e0a 2a20 2a2a 436f 6e76 656e  ocol..* **Conven
+00000c10: 6965 6e63 653a 2a2a 2072 656d 6f76 6573  ience:** removes
+00000c20: 2074 6865 2072 6571 7569 7265 6d65 6e74   the requirement
+00000c30: 2074 6f20 7573 6520 616e 6420 6469 7374   to use and dist
+00000c40: 7269 6275 7465 2053 534c 0a20 2063 6572  ribute SSL.  cer
+00000c50: 7469 6669 6361 7465 732c 2061 7320 7765  tificates, as we
+00000c60: 6c6c 2061 7320 6d61 6e61 6765 2066 6972  ll as manage fir
+00000c70: 6577 616c 6c73 206f 7220 736f 7572 6365  ewalls or source
+00000c80: 2f64 6573 7469 6e61 7469 6f6e 2049 5020  /destination IP 
+00000c90: 6164 6472 6573 7365 732e 0a2a 2028 6f70  addresses..* (op
+00000ca0: 7469 6f6e 616c 6c79 2920 2a2a 4941 4d20  tionally) **IAM 
+00000cb0: 4442 2041 7574 6865 6e74 6963 6174 696f  DB Authenticatio
+00000cc0: 6e3a 2a2a 2070 726f 7669 6465 7320 7375  n:** provides su
+00000cd0: 7070 6f72 7420 666f 720a 2020 5b43 6c6f  pport for.  [Clo
+00000ce0: 7564 2053 514c e280 9973 2061 7574 6f6d  ud SQL...s autom
+00000cf0: 6174 6963 2049 414d 2044 4220 4175 7468  atic IAM DB Auth
+00000d00: 4e5d 5b69 616d 2d64 622d 6175 7468 6e5d  N][iam-db-authn]
+00000d10: 2066 6561 7475 7265 2e0a 0a5b 6961 6d2d   feature...[iam-
+00000d20: 6462 2d61 7574 686e 5d3a 2068 7474 7073  db-authn]: https
+00000d30: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
+00000d40: 636f 6d2f 7371 6c2f 646f 6373 2f70 6f73  com/sql/docs/pos
+00000d50: 7467 7265 732f 6175 7468 656e 7469 6361  tgres/authentica
+00000d60: 7469 6f6e 0a0a 5468 6520 436c 6f75 6420  tion..The Cloud 
+00000d70: 5351 4c20 5079 7468 6f6e 2043 6f6e 6e65  SQL Python Conne
+00000d80: 6374 6f72 2069 7320 6120 7061 636b 6167  ctor is a packag
+00000d90: 6520 746f 2062 6520 7573 6564 2061 6c6f  e to be used alo
+00000da0: 6e67 7369 6465 2061 2064 6174 6162 6173  ngside a databas
+00000db0: 6520 6472 6976 6572 2e0a 4375 7272 656e  e driver..Curren
+00000dc0: 746c 7920 7375 7070 6f72 7465 6420 6472  tly supported dr
+00000dd0: 6976 6572 7320 6172 653a 0a20 2d20 5b60  ivers are:. - [`
+00000de0: 7079 6d79 7371 6c60 5d28 6874 7470 733a  pymysql`](https:
+00000df0: 2f2f 6769 7468 7562 2e63 6f6d 2f50 794d  //github.com/PyM
+00000e00: 7953 514c 2f50 794d 7953 514c 2920 284d  ySQL/PyMySQL) (M
+00000e10: 7953 514c 290a 202d 205b 6070 6738 3030  ySQL). - [`pg800
+00000e20: 3060 5d28 6874 7470 733a 2f2f 6769 7468  0`](https://gith
+00000e30: 7562 2e63 6f6d 2f74 6c6f 636b 652f 7067  ub.com/tlocke/pg
+00000e40: 3830 3030 2920 2850 6f73 7467 7265 5351  8000) (PostgreSQ
+00000e50: 4c29 0a20 2d20 5b60 6173 796e 6370 6760  L). - [`asyncpg`
+00000e60: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000e70: 2e63 6f6d 2f4d 6167 6963 5374 6163 6b2f  .com/MagicStack/
+00000e80: 6173 796e 6370 6729 2028 506f 7374 6772  asyncpg) (Postgr
+00000e90: 6553 514c 290a 202d 205b 6070 7974 6473  eSQL). - [`pytds
+00000ea0: 605d 2868 7474 7073 3a2f 2f67 6974 6875  `](https://githu
+00000eb0: 622e 636f 6d2f 6465 6e69 7365 6e6b 6f6d  b.com/denisenkom
+00000ec0: 2f70 7974 6473 2920 2853 514c 2053 6572  /pytds) (SQL Ser
+00000ed0: 7665 7229 0a0a 0a23 2320 496e 7374 616c  ver)...## Instal
+00000ee0: 6c61 7469 6f6e 0a0a 596f 7520 6361 6e20  lation..You can 
+00000ef0: 696e 7374 616c 6c20 7468 6973 206c 6962  install this lib
+00000f00: 7261 7279 2077 6974 6820 6070 6970 2069  rary with `pip i
+00000f10: 6e73 7461 6c6c 602c 2073 7065 6369 6679  nstall`, specify
+00000f20: 696e 6720 7468 6520 6472 6976 6572 0a62  ing the driver.b
+00000f30: 6173 6564 206f 6e20 796f 7572 2064 6174  ased on your dat
+00000f40: 6162 6173 6520 6469 616c 6563 742e 0a0a  abase dialect...
+00000f50: 2323 2320 4d79 5351 4c0a 6060 600a 7069  ### MySQL.```.pi
+00000f60: 7020 696e 7374 616c 6c20 2263 6c6f 7564  p install "cloud
+00000f70: 2d73 716c 2d70 7974 686f 6e2d 636f 6e6e  -sql-python-conn
+00000f80: 6563 746f 725b 7079 6d79 7371 6c5d 220a  ector[pymysql]".
+00000f90: 6060 600a 2323 2320 506f 7374 6772 6573  ```.### Postgres
+00000fa0: 0a54 6865 7265 2061 7265 2074 776f 2064  .There are two d
+00000fb0: 6966 6665 7265 6e74 2064 6174 6162 6173  ifferent databas
+00000fc0: 6520 6472 6976 6572 7320 7468 6174 2061  e drivers that a
+00000fd0: 7265 2073 7570 706f 7274 6564 2066 6f72  re supported for
+00000fe0: 2074 6865 2050 6f73 7467 7265 7320 6469   the Postgres di
+00000ff0: 616c 6563 743a 0a0a 2323 2323 2070 6738  alect:..#### pg8
+00001000: 3030 300a 6060 600a 7069 7020 696e 7374  000.```.pip inst
+00001010: 616c 6c20 2263 6c6f 7564 2d73 716c 2d70  all "cloud-sql-p
+00001020: 7974 686f 6e2d 636f 6e6e 6563 746f 725b  ython-connector[
+00001030: 7067 3830 3030 5d22 0a60 6060 0a23 2323  pg8000]".```.###
+00001040: 2320 6173 796e 6370 670a 6060 600a 7069  # asyncpg.```.pi
+00001050: 7020 696e 7374 616c 6c20 2263 6c6f 7564  p install "cloud
+00001060: 2d73 716c 2d70 7974 686f 6e2d 636f 6e6e  -sql-python-conn
+00001070: 6563 746f 725b 6173 796e 6370 675d 220a  ector[asyncpg]".
+00001080: 6060 600a 2323 2320 5351 4c20 5365 7276  ```.### SQL Serv
+00001090: 6572 0a60 6060 0a70 6970 2069 6e73 7461  er.```.pip insta
+000010a0: 6c6c 2022 636c 6f75 642d 7371 6c2d 7079  ll "cloud-sql-py
+000010b0: 7468 6f6e 2d63 6f6e 6e65 6374 6f72 5b70  thon-connector[p
+000010c0: 7974 6473 5d22 0a60 6060 0a23 2320 5573  ytds]".```.## Us
+000010d0: 6167 650a 0a54 6869 7320 7061 636b 6167  age..This packag
+000010e0: 6520 7072 6f76 6964 6573 2073 6576 6572  e provides sever
+000010f0: 616c 2066 756e 6374 696f 6e73 2066 6f72  al functions for
+00001100: 2061 7574 686f 7269 7a69 6e67 2061 6e64   authorizing and
+00001110: 2065 6e63 7279 7074 696e 670a 636f 6e6e   encrypting.conn
+00001120: 6563 7469 6f6e 732e 2054 6865 7365 2066  ections. These f
+00001130: 756e 6374 696f 6e73 2061 7265 2075 7365  unctions are use
+00001140: 6420 7769 7468 2079 6f75 7220 6461 7461  d with your data
+00001150: 6261 7365 2064 7269 7665 7220 746f 2063  base driver to c
+00001160: 6f6e 6e65 6374 2074 6f0a 796f 7572 2043  onnect to.your C
+00001170: 6c6f 7564 2053 514c 2069 6e73 7461 6e63  loud SQL instanc
+00001180: 652e 0a0a 5468 6520 696e 7374 616e 6365  e...The instance
+00001190: 2063 6f6e 6e65 6374 696f 6e20 6e61 6d65   connection name
+000011a0: 2066 6f72 2079 6f75 7220 436c 6f75 6420   for your Cloud 
+000011b0: 5351 4c20 696e 7374 616e 6365 2069 7320  SQL instance is 
+000011c0: 616c 7761 7973 2069 6e20 7468 650a 666f  always in the.fo
+000011d0: 726d 6174 2022 7072 6f6a 6563 743a 7265  rmat "project:re
+000011e0: 6769 6f6e 3a69 6e73 7461 6e63 6522 2e0a  gion:instance"..
+000011f0: 0a23 2323 2041 5049 7320 616e 6420 5365  .### APIs and Se
+00001200: 7276 6963 6573 0a0a 5468 6973 2070 6163  rvices..This pac
+00001210: 6b61 6765 2072 6571 7569 7265 7320 7468  kage requires th
+00001220: 6520 666f 6c6c 6f77 696e 6720 746f 2073  e following to s
+00001230: 7563 6365 7373 6675 6c6c 7920 6d61 6b65  uccessfully make
+00001240: 2043 6c6f 7564 2053 514c 2043 6f6e 6e65   Cloud SQL Conne
+00001250: 6374 696f 6e73 3a0a 0a2d 2049 414d 2070  ctions:..- IAM p
+00001260: 7269 6e63 6970 616c 2028 7573 6572 2c20  rincipal (user, 
+00001270: 7365 7276 6963 6520 6163 636f 756e 742c  service account,
+00001280: 2065 7463 2e29 2077 6974 6820 7468 650a   etc.) with the.
+00001290: 5b43 6c6f 7564 2053 514c 2043 6c69 656e  [Cloud SQL Clien
+000012a0: 745d 5b63 6c69 656e 742d 726f 6c65 5d20  t][client-role] 
+000012b0: 726f 6c65 2e20 5468 6973 2049 414d 2070  role. This IAM p
+000012c0: 7269 6e63 6970 616c 2077 696c 6c20 6265  rincipal will be
+000012d0: 2075 7365 6420 666f 720a 5b63 7265 6465   used for.[crede
+000012e0: 6e74 6961 6c73 5d28 2363 7265 6465 6e74  ntials](#credent
+000012f0: 6961 6c73 292e 0a2d 2054 6865 205b 436c  ials)..- The [Cl
+00001300: 6f75 6420 5351 4c20 4164 6d69 6e20 4150  oud SQL Admin AP
+00001310: 495d 5b61 646d 696e 2d61 7069 5d20 746f  I][admin-api] to
+00001320: 2062 6520 656e 6162 6c65 6420 7769 7468   be enabled with
+00001330: 696e 2079 6f75 7220 476f 6f67 6c65 2043  in your Google C
+00001340: 6c6f 7564 0a50 726f 6a65 6374 2e20 4279  loud.Project. By
+00001350: 2064 6566 6175 6c74 2c20 7468 6520 4150   default, the AP
+00001360: 4920 7769 6c6c 2062 6520 6361 6c6c 6564  I will be called
+00001370: 2069 6e20 7468 6520 7072 6f6a 6563 7420   in the project 
+00001380: 6173 736f 6369 6174 6564 2077 6974 680a  associated with.
+00001390: 7468 6520 4941 4d20 7072 696e 6369 7061  the IAM principa
+000013a0: 6c2e 0a0a 5b61 646d 696e 2d61 7069 5d3a  l...[admin-api]:
+000013b0: 2068 7474 7073 3a2f 2f63 6f6e 736f 6c65   https://console
+000013c0: 2e63 6c6f 7564 2e67 6f6f 676c 652e 636f  .cloud.google.co
+000013d0: 6d2f 6170 6973 2f61 7069 2f73 716c 6164  m/apis/api/sqlad
+000013e0: 6d69 6e2e 676f 6f67 6c65 6170 6973 2e63  min.googleapis.c
+000013f0: 6f6d 0a5b 636c 6965 6e74 2d72 6f6c 655d  om.[client-role]
+00001400: 3a20 6874 7470 733a 2f2f 636c 6f75 642e  : https://cloud.
+00001410: 676f 6f67 6c65 2e63 6f6d 2f73 716c 2f64  google.com/sql/d
+00001420: 6f63 732f 6d79 7371 6c2f 726f 6c65 732d  ocs/mysql/roles-
+00001430: 616e 642d 7065 726d 6973 7369 6f6e 730a  and-permissions.
+00001440: 0a23 2323 2043 7265 6465 6e74 6961 6c73  .### Credentials
+00001450: 0a0a 5468 6973 206c 6962 7261 7279 2075  ..This library u
+00001460: 7365 7320 7468 6520 5b41 7070 6c69 6361  ses the [Applica
+00001470: 7469 6f6e 2044 6566 6175 6c74 2043 7265  tion Default Cre
+00001480: 6465 6e74 6961 6c73 2028 4144 4329 5d5b  dentials (ADC)][
+00001490: 6164 635d 2073 7472 6174 6567 7920 666f  adc] strategy fo
+000014a0: 720a 7265 736f 6c76 696e 6720 6372 6564  r.resolving cred
+000014b0: 656e 7469 616c 732e 2050 6c65 6173 6520  entials. Please 
+000014c0: 7365 6520 5b74 6865 7365 2069 6e73 7472  see [these instr
+000014d0: 7563 7469 6f6e 7320 666f 7220 686f 7720  uctions for how 
+000014e0: 746f 2073 6574 2079 6f75 7220 4144 435d  to set your ADC]
+000014f0: 5b73 6574 2d61 6463 5d0a 2847 6f6f 676c  [set-adc].(Googl
+00001500: 6520 436c 6f75 6420 4170 706c 6963 6174  e Cloud Applicat
+00001510: 696f 6e20 7673 204c 6f63 616c 2044 6576  ion vs Local Dev
+00001520: 656c 6f70 6d65 6e74 2c20 4941 4d20 7573  elopment, IAM us
+00001530: 6572 2076 7320 7365 7276 6963 6520 6163  er vs service ac
+00001540: 636f 756e 7420 6372 6564 656e 7469 616c  count credential
+00001550: 7329 2c0a 6f72 2063 6f6e 7375 6c74 2074  s),.or consult t
+00001560: 6865 205b 676f 6f67 6c65 2e61 7574 685d  he [google.auth]
+00001570: 5b67 6f6f 676c 652d 6175 7468 5d20 7061  [google-auth] pa
+00001580: 636b 6167 652e 0a0a 546f 2065 7870 6c69  ckage...To expli
+00001590: 6369 746c 7920 7365 7420 6120 7370 6563  citly set a spec
+000015a0: 6966 6963 2073 6f75 7263 6520 666f 7220  ific source for 
+000015b0: 7468 6520 6372 6564 656e 7469 616c 732c  the credentials,
+000015c0: 2073 6565 0a5b 436f 6e66 6967 7572 696e   see.[Configurin
+000015d0: 6720 7468 6520 436f 6e6e 6563 746f 725d  g the Connector]
+000015e0: 2823 636f 6e66 6967 7572 696e 672d 7468  (#configuring-th
+000015f0: 652d 636f 6e6e 6563 746f 7229 2062 656c  e-connector) bel
+00001600: 6f77 2e0a 0a5b 6164 635d 3a20 6874 7470  ow...[adc]: http
+00001610: 733a 2f2f 636c 6f75 642e 676f 6f67 6c65  s://cloud.google
+00001620: 2e63 6f6d 2f64 6f63 732f 6175 7468 656e  .com/docs/authen
+00001630: 7469 6361 7469 6f6e 2361 6463 0a5b 7365  tication#adc.[se
+00001640: 742d 6164 635d 3a20 6874 7470 733a 2f2f  t-adc]: https://
+00001650: 636c 6f75 642e 676f 6f67 6c65 2e63 6f6d  cloud.google.com
+00001660: 2f64 6f63 732f 6175 7468 656e 7469 6361  /docs/authentica
+00001670: 7469 6f6e 2f70 726f 7669 6465 2d63 7265  tion/provide-cre
+00001680: 6465 6e74 6961 6c73 2d61 6463 0a5b 676f  dentials-adc.[go
+00001690: 6f67 6c65 2d61 7574 685d 3a20 6874 7470  ogle-auth]: http
+000016a0: 733a 2f2f 676f 6f67 6c65 2d61 7574 682e  s://google-auth.
+000016b0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+000016c0: 6e2f 6d61 7374 6572 2f72 6566 6572 656e  n/master/referen
+000016d0: 6365 2f67 6f6f 676c 652e 6175 7468 2e68  ce/google.auth.h
+000016e0: 746d 6c0a 0a23 2323 2048 6f77 2074 6f20  tml..### How to 
+000016f0: 7573 6520 7468 6973 2043 6f6e 6e65 6374  use this Connect
+00001700: 6f72 0a0a 546f 2063 6f6e 6e65 6374 2074  or..To connect t
+00001710: 6f20 436c 6f75 6420 5351 4c20 7573 696e  o Cloud SQL usin
+00001720: 6720 7468 6520 636f 6e6e 6563 746f 722c  g the connector,
+00001730: 2069 6e69 7469 7461 6c69 7a65 2061 2060   inititalize a `
+00001740: 436f 6e6e 6563 746f 7260 0a6f 626a 6563  Connector`.objec
+00001750: 7420 616e 6420 6361 6c6c 2069 7427 7320  t and call it's 
+00001760: 6063 6f6e 6e65 6374 6020 6d65 7468 6f64  `connect` method
+00001770: 2077 6974 6820 7468 6520 7072 6f70 6572   with the proper
+00001780: 2069 6e70 7574 2070 6172 616d 6574 6572   input parameter
+00001790: 732e 0a0a 5468 6520 6043 6f6e 6e65 6374  s...The `Connect
+000017a0: 6f72 6020 6974 7365 6c66 2063 7265 6174  or` itself creat
+000017b0: 6573 2063 6f6e 6e65 6374 696f 6e20 6f62  es connection ob
+000017c0: 6a65 6374 7320 6279 2063 616c 6c69 6e67  jects by calling
+000017d0: 2069 7473 2060 636f 6e6e 6563 7460 206d   its `connect` m
+000017e0: 6574 686f 6420 6275 7420 646f 6573 206e  ethod but does n
+000017f0: 6f74 206d 616e 6167 6520 6461 7461 6261  ot manage databa
+00001800: 7365 2063 6f6e 6e65 6374 696f 6e20 706f  se connection po
+00001810: 6f6c 696e 672e 2046 6f72 2074 6869 7320  oling. For this 
+00001820: 7265 6173 6f6e 2c20 6974 2069 7320 7265  reason, it is re
+00001830: 636f 6d6d 656e 6465 6420 746f 2075 7365  commended to use
+00001840: 2074 6865 2063 6f6e 6e65 6374 6f72 2061   the connector a
+00001850: 6c6f 6e67 7369 6465 2061 206c 6962 7261  longside a libra
+00001860: 7279 2074 6861 7420 6361 6e20 6372 6561  ry that can crea
+00001870: 7465 2063 6f6e 6e65 6374 696f 6e20 706f  te connection po
+00001880: 6f6c 732c 2073 7563 6820 6173 205b 5351  ols, such as [SQ
+00001890: 4c41 6c63 6865 6d79 5d28 6874 7470 733a  LAlchemy](https:
+000018a0: 2f2f 7777 772e 7371 6c61 6c63 6865 6d79  //www.sqlalchemy
+000018b0: 2e6f 7267 2f29 2e20 5468 6973 2077 696c  .org/). This wil
+000018c0: 6c20 616c 6c6f 7720 666f 7220 636f 6e6e  l allow for conn
+000018d0: 6563 7469 6f6e 7320 746f 2072 656d 6169  ections to remai
+000018e0: 6e20 6f70 656e 2061 6e64 2062 6520 7265  n open and be re
+000018f0: 7573 6564 2c20 7265 6475 6369 6e67 2063  used, reducing c
+00001900: 6f6e 6e65 6374 696f 6e20 6f76 6572 6865  onnection overhe
+00001910: 6164 2061 6e64 2074 6865 206e 756d 6265  ad and the numbe
+00001920: 7220 6f66 2063 6f6e 6e65 6374 696f 6e73  r of connections
+00001930: 206e 6565 6465 642e 0a0a 496e 2074 6865   needed...In the
+00001940: 2043 6f6e 6e65 6374 6f72 2773 2060 636f   Connector's `co
+00001950: 6e6e 6563 7460 206d 6574 686f 6420 6265  nnect` method be
+00001960: 6c6f 772c 2069 6e70 7574 2079 6f75 7220  low, input your 
+00001970: 636f 6e6e 6563 7469 6f6e 2073 7472 696e  connection strin
+00001980: 6720 6173 2074 6865 2066 6972 7374 2070  g as the first p
+00001990: 6f73 6974 696f 6e61 6c20 6172 6775 6d65  ositional argume
+000019a0: 6e74 2061 6e64 2074 6865 206e 616d 6520  nt and the name 
+000019b0: 6f66 2074 6865 2064 6174 6162 6173 6520  of the database 
+000019c0: 6472 6976 6572 2066 6f72 2074 6865 2073  driver for the s
+000019d0: 6563 6f6e 6420 706f 7369 7469 6f6e 616c  econd positional
+000019e0: 2061 7267 756d 656e 742e 2049 6e73 6572   argument. Inser
+000019f0: 7420 7468 6520 7265 7374 206f 6620 796f  t the rest of yo
+00001a00: 7572 2063 6f6e 6e65 6374 696f 6e20 6b65  ur connection ke
+00001a10: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
+00001a20: 6c69 6b65 2075 7365 722c 2070 6173 7377  like user, passw
+00001a30: 6f72 6420 616e 6420 6461 7461 6261 7365  ord and database
+00001a40: 2e20 596f 7520 6361 6e20 616c 736f 2073  . You can also s
+00001a50: 6574 2074 6865 206f 7074 696f 6e61 6c20  et the optional 
+00001a60: 6074 696d 656f 7574 6020 6f72 2060 6970  `timeout` or `ip
+00001a70: 5f74 7970 6560 206b 6579 776f 7264 2061  _type` keyword a
+00001a80: 7267 756d 656e 7473 2e0a 0a54 6f20 7573  rguments...To us
+00001a90: 6520 7468 6973 2063 6f6e 6e65 6374 6f72  e this connector
+00001aa0: 2077 6974 6820 5351 4c41 6c63 6865 6d79   with SQLAlchemy
+00001ab0: 2c20 7573 6520 7468 6520 6063 7265 6174  , use the `creat
+00001ac0: 6f72 6020 6172 6775 6d65 6e74 2066 6f72  or` argument for
+00001ad0: 2060 7371 6c61 6c63 6865 6d79 2e63 7265   `sqlalchemy.cre
+00001ae0: 6174 655f 656e 6769 6e65 603a 0a0a 6060  ate_engine`:..``
+00001af0: 6070 7974 686f 6e0a 6672 6f6d 2067 6f6f  `python.from goo
+00001b00: 676c 652e 636c 6f75 642e 7371 6c2e 636f  gle.cloud.sql.co
+00001b10: 6e6e 6563 746f 7220 696d 706f 7274 2043  nnector import C
+00001b20: 6f6e 6e65 6374 6f72 0a69 6d70 6f72 7420  onnector.import 
+00001b30: 7371 6c61 6c63 6865 6d79 0a0a 2320 696e  sqlalchemy..# in
+00001b40: 6974 6961 6c69 7a65 2043 6f6e 6e65 6374  itialize Connect
+00001b50: 6f72 206f 626a 6563 740a 636f 6e6e 6563  or object.connec
+00001b60: 746f 7220 3d20 436f 6e6e 6563 746f 7228  tor = Connector(
+00001b70: 290a 0a23 2066 756e 6374 696f 6e20 746f  )..# function to
+00001b80: 2072 6574 7572 6e20 7468 6520 6461 7461   return the data
+00001b90: 6261 7365 2063 6f6e 6e65 6374 696f 6e0a  base connection.
+00001ba0: 6465 6620 6765 7463 6f6e 6e28 2920 2d3e  def getconn() ->
+00001bb0: 2070 796d 7973 716c 2e63 6f6e 6e65 6374   pymysql.connect
+00001bc0: 696f 6e73 2e43 6f6e 6e65 6374 696f 6e3a  ions.Connection:
+00001bd0: 0a20 2020 2063 6f6e 6e3a 2070 796d 7973  .    conn: pymys
+00001be0: 716c 2e63 6f6e 6e65 6374 696f 6e73 2e43  ql.connections.C
+00001bf0: 6f6e 6e65 6374 696f 6e20 3d20 636f 6e6e  onnection = conn
+00001c00: 6563 746f 722e 636f 6e6e 6563 7428 0a20  ector.connect(. 
+00001c10: 2020 2020 2020 2022 7072 6f6a 6563 743a         "project:
+00001c20: 7265 6769 6f6e 3a69 6e73 7461 6e63 6522  region:instance"
+00001c30: 2c0a 2020 2020 2020 2020 2270 796d 7973  ,.        "pymys
+00001c40: 716c 222c 0a20 2020 2020 2020 2075 7365  ql",.        use
+00001c50: 723d 226d 792d 7573 6572 222c 0a20 2020  r="my-user",.   
+00001c60: 2020 2020 2070 6173 7377 6f72 643d 226d       password="m
+00001c70: 792d 7061 7373 776f 7264 222c 0a20 2020  y-password",.   
+00001c80: 2020 2020 2064 623d 226d 792d 6462 2d6e       db="my-db-n
+00001c90: 616d 6522 0a20 2020 2029 0a20 2020 2072  ame".    ).    r
+00001ca0: 6574 7572 6e20 636f 6e6e 0a0a 2320 6372  eturn conn..# cr
+00001cb0: 6561 7465 2063 6f6e 6e65 6374 696f 6e20  eate connection 
+00001cc0: 706f 6f6c 0a70 6f6f 6c20 3d20 7371 6c61  pool.pool = sqla
+00001cd0: 6c63 6865 6d79 2e63 7265 6174 655f 656e  lchemy.create_en
+00001ce0: 6769 6e65 280a 2020 2020 226d 7973 716c  gine(.    "mysql
+00001cf0: 2b70 796d 7973 716c 3a2f 2f22 2c0a 2020  +pymysql://",.  
+00001d00: 2020 6372 6561 746f 723d 6765 7463 6f6e    creator=getcon
+00001d10: 6e2c 0a29 0a60 6060 0a0a 5468 6520 7265  n,.).```..The re
+00001d20: 7475 726e 6564 2063 6f6e 6e65 6374 696f  turned connectio
+00001d30: 6e20 706f 6f6c 2065 6e67 696e 6520 6361  n pool engine ca
+00001d40: 6e20 7468 656e 2062 6520 7573 6564 2074  n then be used t
+00001d50: 6f20 7175 6572 7920 616e 6420 6d6f 6469  o query and modi
+00001d60: 6679 2074 6865 2064 6174 6162 6173 652e  fy the database.
+00001d70: 0a0a 6060 6070 7974 686f 6e0a 2320 696e  ..```python.# in
+00001d80: 7365 7274 2073 7461 7465 6d65 6e74 0a69  sert statement.i
+00001d90: 6e73 6572 745f 7374 6d74 203d 2073 716c  nsert_stmt = sql
+00001da0: 616c 6368 656d 792e 7465 7874 280a 2020  alchemy.text(.  
+00001db0: 2020 2249 4e53 4552 5420 494e 544f 206d    "INSERT INTO m
+00001dc0: 795f 7461 626c 6520 2869 642c 2074 6974  y_table (id, tit
+00001dd0: 6c65 2920 5641 4c55 4553 2028 3a69 642c  le) VALUES (:id,
+00001de0: 203a 7469 746c 6529 222c 0a29 0a0a 7769   :title)",.)..wi
+00001df0: 7468 2070 6f6f 6c2e 636f 6e6e 6563 7428  th pool.connect(
+00001e00: 2920 6173 2064 625f 636f 6e6e 3a0a 2020  ) as db_conn:.  
+00001e10: 2020 2320 696e 7365 7274 2069 6e74 6f20    # insert into 
+00001e20: 6461 7461 6261 7365 0a20 2020 2064 625f  database.    db_
+00001e30: 636f 6e6e 2e65 7865 6375 7465 2869 6e73  conn.execute(ins
+00001e40: 6572 745f 7374 6d74 2c20 7061 7261 6d65  ert_stmt, parame
+00001e50: 7465 7273 3d7b 2269 6422 3a20 2262 6f6f  ters={"id": "boo
+00001e60: 6b31 222c 2022 7469 746c 6522 3a20 2242  k1", "title": "B
+00001e70: 6f6f 6b20 4f6e 6522 7d29 0a0a 2020 2020  ook One"})..    
+00001e80: 2320 7175 6572 7920 6461 7461 6261 7365  # query database
+00001e90: 0a20 2020 2072 6573 756c 7420 3d20 6462  .    result = db
+00001ea0: 5f63 6f6e 6e2e 6578 6563 7574 6528 7371  _conn.execute(sq
+00001eb0: 6c61 6c63 6865 6d79 2e74 6578 7428 2253  lalchemy.text("S
+00001ec0: 454c 4543 5420 2a20 6672 6f6d 206d 795f  ELECT * from my_
+00001ed0: 7461 626c 6522 2929 2e66 6574 6368 616c  table")).fetchal
+00001ee0: 6c28 290a 0a20 2020 2023 2063 6f6d 6d69  l()..    # commi
+00001ef0: 7420 7472 616e 7361 6374 696f 6e20 2853  t transaction (S
+00001f00: 514c 416c 6368 656d 7920 7632 2e58 2e58  QLAlchemy v2.X.X
+00001f10: 2069 7320 636f 6d6d 6974 2061 7320 796f   is commit as yo
+00001f20: 7520 676f 290a 2020 2020 6462 5f63 6f6e  u go).    db_con
+00001f30: 6e2e 636f 6d6d 6974 2829 0a0a 2020 2020  n.commit()..    
+00001f40: 2320 446f 2073 6f6d 6574 6869 6e67 2077  # Do something w
+00001f50: 6974 6820 7468 6520 7265 7375 6c74 730a  ith the results.
+00001f60: 2020 2020 666f 7220 726f 7720 696e 2072      for row in r
+00001f70: 6573 756c 743a 0a20 2020 2020 2020 2070  esult:.        p
+00001f80: 7269 6e74 2872 6f77 290a 6060 600a 0a54  rint(row).```..T
+00001f90: 6f20 636c 6f73 6520 7468 6520 6043 6f6e  o close the `Con
+00001fa0: 6e65 6374 6f72 6020 6f62 6a65 6374 2773  nector` object's
+00001fb0: 2062 6163 6b67 726f 756e 6420 7265 736f   background reso
+00001fc0: 7572 6365 732c 2063 616c 6c20 6974 2773  urces, call it's
+00001fd0: 2060 636c 6f73 6528 2960 206d 6574 686f   `close()` metho
+00001fe0: 6420 6173 2066 6f6c 6c6f 7773 3a0a 0a60  d as follows:..`
+00001ff0: 6060 7079 7468 6f6e 0a63 6f6e 6e65 6374  ``python.connect
+00002000: 6f72 2e63 6c6f 7365 2829 0a60 6060 0a0a  or.close().```..
+00002010: 2a2a 4e6f 7465 2a2a 3a20 466f 7220 6d6f  **Note**: For mo
+00002020: 7265 2065 7861 6d70 6c65 7320 6f66 2075  re examples of u
+00002030: 7369 6e67 2053 514c 416c 6368 656d 7920  sing SQLAlchemy 
+00002040: 746f 206d 616e 6167 6520 636f 6e6e 6563  to manage connec
+00002050: 7469 6f6e 2070 6f6f 6c69 6e67 2077 6974  tion pooling wit
+00002060: 6820 7468 6520 636f 6e6e 6563 746f 722c  h the connector,
+00002070: 2070 6c65 6173 6520 7365 6520 5b43 6c6f   please see [Clo
+00002080: 7564 2053 514c 2053 514c 416c 6368 656d  ud SQL SQLAlchem
+00002090: 7920 5361 6d70 6c65 735d 2868 7474 7073  y Samples](https
+000020a0: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
+000020b0: 636f 6d2f 7371 6c2f 646f 6373 2f70 6f73  com/sql/docs/pos
+000020c0: 7467 7265 732f 636f 6e6e 6563 742d 636f  tgres/connect-co
+000020d0: 6e6e 6563 746f 7273 2370 7974 686f 6e5f  nnectors#python_
+000020e0: 3129 2e0a 0a2a 2a4e 6f74 6520 666f 7220  1)...**Note for 
+000020f0: 5351 4c20 5365 7276 6572 2075 7365 7273  SQL Server users
+00002100: 2a2a 3a20 4966 2079 6f75 7220 5351 4c20  **: If your SQL 
+00002110: 5365 7276 6572 2069 6e73 7461 6e63 6520  Server instance 
+00002120: 7265 7175 6972 6573 2053 534c 2c20 796f  requires SSL, yo
+00002130: 7520 6e65 6564 2074 6f20 646f 776e 6c6f  u need to downlo
+00002140: 6164 2074 6865 2043 4120 6365 7274 6966  ad the CA certif
+00002150: 6963 6174 6520 666f 7220 796f 7572 2069  icate for your i
+00002160: 6e73 7461 6e63 6520 616e 6420 696e 636c  nstance and incl
+00002170: 7564 6520 6063 6166 696c 653d 7b70 6174  ude `cafile={pat
+00002180: 6820 746f 2064 6f77 6e6c 6f61 6465 6420  h to downloaded 
+00002190: 6365 7274 6966 6963 6174 657d 6020 616e  certificate}` an
+000021a0: 6420 6076 616c 6964 6174 655f 686f 7374  d `validate_host
+000021b0: 3d46 616c 7365 602e 2054 6869 7320 6973  =False`. This is
+000021c0: 2061 2077 6f72 6b61 726f 756e 6420 666f   a workaround fo
+000021d0: 7220 6120 5b6b 6e6f 776e 2069 7373 7565  r a [known issue
+000021e0: 5d28 6874 7470 733a 2f2f 6973 7375 6574  ](https://issuet
+000021f0: 7261 636b 6572 2e67 6f6f 676c 652e 636f  racker.google.co
+00002200: 6d2f 3138 3438 3637 3134 3729 2e0a 0a23  m/184867147)...#
+00002210: 2323 2043 6f6e 6669 6775 7269 6e67 2074  ## Configuring t
+00002220: 6865 2043 6f6e 6e65 6374 6f72 0a0a 4966  he Connector..If
+00002230: 2079 6f75 206e 6565 6420 746f 2063 7573   you need to cus
+00002240: 746f 6d69 7a65 2073 6f6d 6574 6869 6e67  tomize something
+00002250: 2061 626f 7574 2074 6865 2063 6f6e 6e65   about the conne
+00002260: 6374 6f72 2c20 6f72 2077 616e 7420 746f  ctor, or want to
+00002270: 2073 7065 6369 6679 0a64 6566 6175 6c74   specify.default
+00002280: 7320 666f 7220 6561 6368 2063 6f6e 6e65  s for each conne
+00002290: 6374 696f 6e20 746f 206d 616b 652c 2079  ction to make, y
+000022a0: 6f75 2063 616e 2069 6e69 7469 616c 697a  ou can initializ
+000022b0: 6520 610a 6043 6f6e 6e65 6374 6f72 6020  e a.`Connector` 
+000022c0: 6f62 6a65 6374 2061 7320 666f 6c6c 6f77  object as follow
+000022d0: 733a 0a0a 6060 6070 7974 686f 6e0a 6672  s:..```python.fr
+000022e0: 6f6d 2067 6f6f 676c 652e 636c 6f75 642e  om google.cloud.
+000022f0: 7371 6c2e 636f 6e6e 6563 746f 7220 696d  sql.connector im
+00002300: 706f 7274 2043 6f6e 6e65 6374 6f72 2c20  port Connector, 
+00002310: 4950 5479 7065 730a 0a23 204e 6f74 653a  IPTypes..# Note:
+00002320: 2061 6c6c 2070 6172 616d 6574 6572 7320   all parameters 
+00002330: 6265 6c6f 7720 6172 6520 6f70 7469 6f6e  below are option
+00002340: 616c 0a63 6f6e 6e65 6374 6f72 203d 2043  al.connector = C
+00002350: 6f6e 6e65 6374 6f72 280a 2020 2020 6970  onnector(.    ip
+00002360: 5f74 7970 653d 4950 5479 7065 732e 5055  _type=IPTypes.PU
+00002370: 424c 4943 2c0a 2020 2020 656e 6162 6c65  BLIC,.    enable
+00002380: 5f69 616d 5f61 7574 683d 4661 6c73 652c  _iam_auth=False,
+00002390: 0a20 2020 2074 696d 656f 7574 3d33 302c  .    timeout=30,
+000023a0: 0a20 2020 2063 7265 6465 6e74 6961 6c73  .    credentials
+000023b0: 3d63 7573 746f 6d5f 6372 6564 7320 2320  =custom_creds # 
+000023c0: 676f 6f67 6c65 2e61 7574 682e 6372 6564  google.auth.cred
+000023d0: 656e 7469 616c 732e 4372 6564 656e 7469  entials.Credenti
+000023e0: 616c 730a 290a 6060 600a 0a23 2323 2055  als.).```..### U
+000023f0: 7369 6e67 2043 6f6e 6e65 6374 6f72 2061  sing Connector a
+00002400: 7320 6120 436f 6e74 6578 7420 4d61 6e61  s a Context Mana
+00002410: 6765 720a 0a54 6865 2060 436f 6e6e 6563  ger..The `Connec
+00002420: 746f 7260 206f 626a 6563 7420 6361 6e20  tor` object can 
+00002430: 616c 736f 2062 6520 7573 6564 2061 7320  also be used as 
+00002440: 6120 636f 6e74 6578 7420 6d61 6e61 6765  a context manage
+00002450: 7220 696e 206f 7264 6572 2074 6f0a 6175  r in order to.au
+00002460: 746f 6d61 7469 6361 6c6c 7920 636c 6f73  tomatically clos
+00002470: 6520 616e 6420 636c 6561 6e75 7020 7265  e and cleanup re
+00002480: 736f 7572 6365 732c 2072 656d 6f76 696e  sources, removin
+00002490: 6720 7468 6520 6e65 6564 2066 6f72 2065  g the need for e
+000024a0: 7870 6c69 6369 740a 6361 6c6c 7320 746f  xplicit.calls to
+000024b0: 2060 636f 6e6e 6563 746f 722e 636c 6f73   `connector.clos
+000024c0: 6528 2960 2e0a 0a43 6f6e 6e65 6374 6f72  e()`...Connector
+000024d0: 2061 7320 6120 636f 6e74 6578 7420 6d61   as a context ma
+000024e0: 6e61 6765 723a 0a0a 6060 6070 7974 686f  nager:..```pytho
+000024f0: 6e0a 6672 6f6d 2067 6f6f 676c 652e 636c  n.from google.cl
+00002500: 6f75 642e 7371 6c2e 636f 6e6e 6563 746f  oud.sql.connecto
+00002510: 7220 696d 706f 7274 2043 6f6e 6e65 6374  r import Connect
+00002520: 6f72 0a69 6d70 6f72 7420 7079 6d79 7371  or.import pymysq
+00002530: 6c0a 696d 706f 7274 2073 716c 616c 6368  l.import sqlalch
+00002540: 656d 790a 0a23 2068 656c 7065 7220 6675  emy..# helper fu
+00002550: 6e63 7469 6f6e 2074 6f20 7265 7475 726e  nction to return
+00002560: 2053 514c 416c 6368 656d 7920 636f 6e6e   SQLAlchemy conn
+00002570: 6563 7469 6f6e 2070 6f6f 6c0a 6465 6620  ection pool.def 
+00002580: 696e 6974 5f63 6f6e 6e65 6374 696f 6e5f  init_connection_
+00002590: 706f 6f6c 2863 6f6e 6e65 6374 6f72 3a20  pool(connector: 
+000025a0: 436f 6e6e 6563 746f 7229 202d 3e20 7371  Connector) -> sq
+000025b0: 6c61 6c63 6865 6d79 2e65 6e67 696e 652e  lalchemy.engine.
+000025c0: 456e 6769 6e65 3a0a 2020 2020 2320 6675  Engine:.    # fu
+000025d0: 6e63 7469 6f6e 2075 7365 6420 746f 2067  nction used to g
+000025e0: 656e 6572 6174 6520 6461 7461 6261 7365  enerate database
+000025f0: 2063 6f6e 6e65 6374 696f 6e0a 2020 2020   connection.    
+00002600: 6465 6620 6765 7463 6f6e 6e28 2920 2d3e  def getconn() ->
+00002610: 2070 796d 7973 716c 2e63 6f6e 6e65 6374   pymysql.connect
+00002620: 696f 6e73 2e43 6f6e 6e65 6374 696f 6e3a  ions.Connection:
+00002630: 0a20 2020 2020 2020 2063 6f6e 6e20 3d20  .        conn = 
+00002640: 636f 6e6e 6563 746f 722e 636f 6e6e 6563  connector.connec
+00002650: 7428 0a20 2020 2020 2020 2020 2020 2022  t(.            "
+00002660: 7072 6f6a 6563 743a 7265 6769 6f6e 3a69  project:region:i
+00002670: 6e73 7461 6e63 6522 2c0a 2020 2020 2020  nstance",.      
+00002680: 2020 2020 2020 2270 796d 7973 716c 222c        "pymysql",
+00002690: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+000026a0: 723d 226d 792d 7573 6572 222c 0a20 2020  r="my-user",.   
+000026b0: 2020 2020 2020 2020 2070 6173 7377 6f72           passwor
+000026c0: 643d 226d 792d 7061 7373 776f 7264 222c  d="my-password",
+000026d0: 0a20 2020 2020 2020 2020 2020 2064 623d  .            db=
+000026e0: 226d 792d 6462 2d6e 616d 6522 0a20 2020  "my-db-name".   
+000026f0: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
+00002700: 6574 7572 6e20 636f 6e6e 0a0a 2020 2020  eturn conn..    
+00002710: 2320 6372 6561 7465 2063 6f6e 6e65 6374  # create connect
+00002720: 696f 6e20 706f 6f6c 0a20 2020 2070 6f6f  ion pool.    poo
+00002730: 6c20 3d20 7371 6c61 6c63 6865 6d79 2e63  l = sqlalchemy.c
+00002740: 7265 6174 655f 656e 6769 6e65 280a 2020  reate_engine(.  
+00002750: 2020 2020 2020 226d 7973 716c 2b70 796d        "mysql+pym
+00002760: 7973 716c 3a2f 2f22 2c0a 2020 2020 2020  ysql://",.      
+00002770: 2020 6372 6561 746f 723d 6765 7463 6f6e    creator=getcon
+00002780: 6e2c 0a20 2020 2029 0a20 2020 2072 6574  n,.    ).    ret
+00002790: 7572 6e20 706f 6f6c 0a0a 2320 696e 6974  urn pool..# init
+000027a0: 6961 6c69 7a65 2043 6c6f 7564 2053 514c  ialize Cloud SQL
+000027b0: 2050 7974 686f 6e20 436f 6e6e 6563 746f   Python Connecto
+000027c0: 7220 6173 2063 6f6e 7465 7874 206d 616e  r as context man
+000027d0: 6167 6572 0a77 6974 6820 436f 6e6e 6563  ager.with Connec
+000027e0: 746f 7228 2920 6173 2063 6f6e 6e65 6374  tor() as connect
+000027f0: 6f72 3a0a 2020 2020 2320 696e 6974 6961  or:.    # initia
+00002800: 6c69 7a65 2063 6f6e 6e65 6374 696f 6e20  lize connection 
+00002810: 706f 6f6c 0a20 2020 2070 6f6f 6c20 3d20  pool.    pool = 
+00002820: 696e 6974 5f63 6f6e 6e65 6374 696f 6e5f  init_connection_
+00002830: 706f 6f6c 2863 6f6e 6e65 6374 6f72 290a  pool(connector).
+00002840: 2020 2020 2320 696e 7365 7274 2073 7461      # insert sta
+00002850: 7465 6d65 6e74 0a20 2020 2069 6e73 6572  tement.    inser
+00002860: 745f 7374 6d74 203d 2073 716c 616c 6368  t_stmt = sqlalch
+00002870: 656d 792e 7465 7874 280a 2020 2020 2020  emy.text(.      
+00002880: 2020 2249 4e53 4552 5420 494e 544f 206d    "INSERT INTO m
+00002890: 795f 7461 626c 6520 2869 642c 2074 6974  y_table (id, tit
+000028a0: 6c65 2920 5641 4c55 4553 2028 3a69 642c  le) VALUES (:id,
+000028b0: 203a 7469 746c 6529 222c 0a20 2020 2029   :title)",.    )
+000028c0: 0a0a 2020 2020 2320 696e 7465 7261 6374  ..    # interact
+000028d0: 2077 6974 6820 436c 6f75 6420 5351 4c20   with Cloud SQL 
+000028e0: 6461 7461 6261 7365 2075 7369 6e67 2063  database using c
+000028f0: 6f6e 6e65 6374 696f 6e20 706f 6f6c 0a20  onnection pool. 
+00002900: 2020 2077 6974 6820 706f 6f6c 2e63 6f6e     with pool.con
+00002910: 6e65 6374 2829 2061 7320 6462 5f63 6f6e  nect() as db_con
+00002920: 6e3a 0a20 2020 2020 2020 2023 2069 6e73  n:.        # ins
+00002930: 6572 7420 696e 746f 2064 6174 6162 6173  ert into databas
+00002940: 650a 2020 2020 2020 2020 6462 5f63 6f6e  e.        db_con
+00002950: 6e2e 6578 6563 7574 6528 696e 7365 7274  n.execute(insert
+00002960: 5f73 746d 742c 2070 6172 616d 6574 6572  _stmt, parameter
+00002970: 733d 7b22 6964 223a 2022 626f 6f6b 3122  s={"id": "book1"
+00002980: 2c20 2274 6974 6c65 223a 2022 426f 6f6b  , "title": "Book
+00002990: 204f 6e65 227d 290a 0a20 2020 2020 2020   One"})..       
+000029a0: 2023 2063 6f6d 6d69 7420 7472 616e 7361   # commit transa
+000029b0: 6374 696f 6e20 2853 514c 416c 6368 656d  ction (SQLAlchem
+000029c0: 7920 7632 2e58 2e58 2069 7320 636f 6d6d  y v2.X.X is comm
+000029d0: 6974 2061 7320 796f 7520 676f 290a 2020  it as you go).  
+000029e0: 2020 2020 2020 6462 5f63 6f6e 6e2e 636f        db_conn.co
+000029f0: 6d6d 6974 2829 0a0a 2020 2020 2020 2020  mmit()..        
+00002a00: 2320 7175 6572 7920 6461 7461 6261 7365  # query database
+00002a10: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00002a20: 3d20 6462 5f63 6f6e 6e2e 6578 6563 7574  = db_conn.execut
+00002a30: 6528 7371 6c61 6c63 6865 6d79 2e74 6578  e(sqlalchemy.tex
+00002a40: 7428 2253 454c 4543 5420 2a20 6672 6f6d  t("SELECT * from
+00002a50: 206d 795f 7461 626c 6522 2929 2e66 6574   my_table")).fet
+00002a60: 6368 616c 6c28 290a 0a20 2020 2020 2020  chall()..       
+00002a70: 2023 2044 6f20 736f 6d65 7468 696e 6720   # Do something 
+00002a80: 7769 7468 2074 6865 2072 6573 756c 7473  with the results
+00002a90: 0a20 2020 2020 2020 2066 6f72 2072 6f77  .        for row
+00002aa0: 2069 6e20 7265 7375 6c74 3a0a 2020 2020   in result:.    
+00002ab0: 2020 2020 2020 2020 7072 696e 7428 726f          print(ro
+00002ac0: 7729 0a60 6060 0a0a 2323 2320 5370 6563  w).```..### Spec
+00002ad0: 6966 7969 6e67 2049 5020 4164 6472 6573  ifying IP Addres
+00002ae0: 7320 5479 7065 0a0a 5468 6520 436c 6f75  s Type..The Clou
+00002af0: 6420 5351 4c20 5079 7468 6f6e 2043 6f6e  d SQL Python Con
+00002b00: 6e65 6374 6f72 2063 616e 2062 6520 7573  nector can be us
+00002b10: 6564 2074 6f20 636f 6e6e 6563 7420 746f  ed to connect to
+00002b20: 2043 6c6f 7564 2053 514c 2069 6e73 7461   Cloud SQL insta
+00002b30: 6e63 6573 0a75 7369 6e67 2062 6f74 6820  nces.using both 
+00002b40: 7075 626c 6963 2061 6e64 2070 7269 7661  public and priva
+00002b50: 7465 2049 5020 6164 6472 6573 7365 732c  te IP addresses,
+00002b60: 2061 7320 7765 6c6c 2061 730a 5b50 7269   as well as.[Pri
+00002b70: 7661 7465 2053 6572 7669 6365 2043 6f6e  vate Service Con
+00002b80: 6e65 6374 5d5b 7073 635d 2028 5053 4329  nect][psc] (PSC)
+00002b90: 2e20 546f 2073 7065 6369 6679 2077 6869  . To specify whi
+00002ba0: 6368 2049 5020 6164 6472 6573 7320 7479  ch IP address ty
+00002bb0: 7065 2074 6f20 636f 6e6e 6563 740a 7769  pe to connect.wi
+00002bc0: 7468 2c20 7365 7420 7468 6520 6069 705f  th, set the `ip_
+00002bd0: 7479 7065 6020 6b65 7977 6f72 6420 6172  type` keyword ar
+00002be0: 6775 6d65 6e74 2077 6865 6e20 696e 6974  gument when init
+00002bf0: 6961 6c69 7a69 6e67 2061 2060 436f 6e6e  ializing a `Conn
+00002c00: 6563 746f 7228 2960 206f 7220 7768 656e  ector()` or when
+00002c10: 0a63 616c 6c69 6e67 2060 636f 6e6e 6563  .calling `connec
+00002c20: 746f 722e 636f 6e6e 6563 7428 2960 2e0a  tor.connect()`..
+00002c30: 0a50 6f73 7369 626c 6520 7661 6c75 6573  .Possible values
+00002c40: 2066 6f72 2060 6970 5f74 7970 6560 2061   for `ip_type` a
+00002c50: 7265 2060 4950 5479 7065 732e 5055 424c  re `IPTypes.PUBL
+00002c60: 4943 6020 2864 6566 6175 6c74 2076 616c  IC` (default val
+00002c70: 7565 292c 0a60 4950 5479 7065 732e 5052  ue),.`IPTypes.PR
+00002c80: 4956 4154 4560 2c20 616e 6420 6049 5054  IVATE`, and `IPT
+00002c90: 7970 6573 2e50 5343 602e 0a0a 4578 616d  ypes.PSC`...Exam
+00002ca0: 706c 653a 0a0a 6060 6070 7974 686f 6e0a  ple:..```python.
+00002cb0: 6672 6f6d 2067 6f6f 676c 652e 636c 6f75  from google.clou
+00002cc0: 642e 7371 6c2e 636f 6e6e 6563 746f 7220  d.sql.connector 
+00002cd0: 696d 706f 7274 2049 5054 7970 6573 0a0a  import IPTypes..
+00002ce0: 636f 6e6e 203d 2063 6f6e 6e65 6374 6f72  conn = connector
+00002cf0: 2e63 6f6e 6e65 6374 280a 2020 2020 2270  .connect(.    "p
+00002d00: 726f 6a65 6374 3a72 6567 696f 6e3a 696e  roject:region:in
+00002d10: 7374 616e 6365 222c 0a20 2020 2022 7079  stance",.    "py
+00002d20: 6d79 7371 6c22 2c0a 2020 2020 6970 5f74  mysql",.    ip_t
+00002d30: 7970 653d 4950 5479 7065 732e 5052 4956  ype=IPTypes.PRIV
+00002d40: 4154 4520 2320 7573 6520 7072 6976 6174  ATE # use privat
+00002d50: 6520 4950 0a2e 2e2e 2069 6e73 6572 7420  e IP.... insert 
+00002d60: 6f74 6865 7220 6b77 6172 6773 202e 2e2e  other kwargs ...
+00002d70: 0a29 0a60 6060 0a0a 4e6f 7465 3a20 4966  .).```..Note: If
+00002d80: 2073 7065 6369 6679 696e 6720 5072 6976   specifying Priv
+00002d90: 6174 6520 4950 206f 7220 5072 6976 6174  ate IP or Privat
+00002da0: 6520 5365 7276 6963 6520 436f 6e6e 6563  e Service Connec
+00002db0: 742c 2079 6f75 7220 6170 706c 6963 6174  t, your applicat
+00002dc0: 696f 6e20 6d75 7374 2062 650a 6174 7461  ion must be.atta
+00002dd0: 6368 6564 2074 6f20 7468 6520 7072 6f70  ched to the prop
+00002de0: 6572 2056 5043 206e 6574 776f 726b 2074  er VPC network t
+00002df0: 6f20 636f 6e6e 6563 7420 746f 2079 6f75  o connect to you
+00002e00: 7220 436c 6f75 6420 5351 4c20 696e 7374  r Cloud SQL inst
+00002e10: 616e 6365 2e20 466f 7220 6d6f 7374 0a61  ance. For most.a
+00002e20: 7070 6c69 6361 7469 6f6e 7320 7468 6973  pplications this
+00002e30: 2077 696c 6c20 7265 7175 6972 6520 7468   will require th
+00002e40: 6520 7573 6520 6f66 2061 205b 5650 4320  e use of a [VPC 
+00002e50: 436f 6e6e 6563 746f 725d 5b76 7063 2d63  Connector][vpc-c
+00002e60: 6f6e 6e65 6374 6f72 5d2e 0a0a 5b70 7363  onnector]...[psc
+00002e70: 5d3a 2068 7474 7073 3a2f 2f63 6c6f 7564  ]: https://cloud
+00002e80: 2e67 6f6f 676c 652e 636f 6d2f 7670 632f  .google.com/vpc/
+00002e90: 646f 6373 2f70 7269 7661 7465 2d73 6572  docs/private-ser
+00002ea0: 7669 6365 2d63 6f6e 6e65 6374 0a5b 7670  vice-connect.[vp
+00002eb0: 632d 636f 6e6e 6563 746f 725d 3a20 6874  c-connector]: ht
+00002ec0: 7470 733a 2f2f 636c 6f75 642e 676f 6f67  tps://cloud.goog
+00002ed0: 6c65 2e63 6f6d 2f76 7063 2f64 6f63 732f  le.com/vpc/docs/
+00002ee0: 636f 6e66 6967 7572 652d 7365 7276 6572  configure-server
+00002ef0: 6c65 7373 2d76 7063 2d61 6363 6573 7323  less-vpc-access#
+00002f00: 6372 6561 7465 2d63 6f6e 6e65 6374 6f72  create-connector
+00002f10: 0a0a 2323 2320 4175 746f 6d61 7469 6320  ..### Automatic 
+00002f20: 4941 4d20 4461 7461 6261 7365 2041 7574  IAM Database Aut
+00002f30: 6865 6e74 6963 6174 696f 6e0a 0a43 6f6e  hentication..Con
+00002f40: 6e65 6374 696f 6e73 2075 7369 6e67 205b  nections using [
+00002f50: 4175 746f 6d61 7469 6320 4941 4d20 6461  Automatic IAM da
+00002f60: 7461 6261 7365 2061 7574 6865 6e74 6963  tabase authentic
+00002f70: 6174 696f 6e5d 2868 7474 7073 3a2f 2f63  ation](https://c
+00002f80: 6c6f 7564 2e67 6f6f 676c 652e 636f 6d2f  loud.google.com/
+00002f90: 7371 6c2f 646f 6373 2f70 6f73 7467 7265  sql/docs/postgre
+00002fa0: 732f 6175 7468 656e 7469 6361 7469 6f6e  s/authentication
+00002fb0: 2361 7574 6f6d 6174 6963 2920 6172 6520  #automatic) are 
+00002fc0: 7375 7070 6f72 7465 6420 7768 656e 2075  supported when u
+00002fd0: 7369 6e67 2050 6f73 7467 7265 7320 6f72  sing Postgres or
+00002fe0: 204d 7953 514c 2064 7269 7665 7273 2e0a   MySQL drivers..
+00002ff0: 4669 7273 742c 206d 616b 6520 7375 7265  First, make sure
+00003000: 2074 6f20 5b63 6f6e 6669 6775 7265 2079   to [configure y
+00003010: 6f75 7220 436c 6f75 6420 5351 4c20 496e  our Cloud SQL In
+00003020: 7374 616e 6365 2074 6f20 616c 6c6f 7720  stance to allow 
+00003030: 4941 4d20 6175 7468 656e 7469 6361 7469  IAM authenticati
+00003040: 6f6e 5d28 6874 7470 733a 2f2f 636c 6f75  on](https://clou
+00003050: 642e 676f 6f67 6c65 2e63 6f6d 2f73 716c  d.google.com/sql
+00003060: 2f64 6f63 732f 706f 7374 6772 6573 2f63  /docs/postgres/c
+00003070: 7265 6174 652d 6564 6974 2d69 616d 2d69  reate-edit-iam-i
+00003080: 6e73 7461 6e63 6573 2363 6f6e 6669 6775  nstances#configu
+00003090: 7265 2d69 616d 2d64 622d 696e 7374 616e  re-iam-db-instan
+000030a0: 6365 290a 616e 6420 5b61 6464 2061 6e20  ce).and [add an 
+000030b0: 4941 4d20 6461 7461 6261 7365 2075 7365  IAM database use
+000030c0: 725d 2868 7474 7073 3a2f 2f63 6c6f 7564  r](https://cloud
+000030d0: 2e67 6f6f 676c 652e 636f 6d2f 7371 6c2f  .google.com/sql/
+000030e0: 646f 6373 2f70 6f73 7467 7265 732f 6372  docs/postgres/cr
+000030f0: 6561 7465 2d6d 616e 6167 652d 6961 6d2d  eate-manage-iam-
+00003100: 7573 6572 7323 6372 6561 7469 6e67 2d61  users#creating-a
+00003110: 2d64 6174 6162 6173 652d 7573 6572 292e  -database-user).
+00003120: 0a0a 4e6f 772c 2079 6f75 2063 616e 2063  ..Now, you can c
+00003130: 6f6e 6e65 6374 2075 7369 6e67 2075 7365  onnect using use
+00003140: 7220 6f72 2073 6572 7669 6365 2061 6363  r or service acc
+00003150: 6f75 6e74 2063 7265 6465 6e74 6961 6c73  ount credentials
+00003160: 2069 6e73 7465 6164 206f 6620 6120 7061   instead of a pa
+00003170: 7373 776f 7264 2e0a 496e 2074 6865 2063  ssword..In the c
+00003180: 616c 6c20 746f 2063 6f6e 6e65 6374 2c20  all to connect, 
+00003190: 7365 7420 7468 6520 6065 6e61 626c 655f  set the `enable_
+000031a0: 6961 6d5f 6175 7468 6020 6b65 7977 6f72  iam_auth` keywor
+000031b0: 6420 6172 6775 6d65 6e74 2074 6f20 7472  d argument to tr
+000031c0: 7565 2061 6e64 2074 6865 2060 7573 6572  ue and the `user
+000031d0: 6020 6172 6775 6d65 6e74 2074 6f20 7468  ` argument to th
+000031e0: 6520 6170 7072 6f70 7269 6174 656c 7920  e appropriately 
+000031f0: 666f 726d 6174 7465 6420 4941 4d20 7072  formatted IAM pr
+00003200: 696e 6369 7061 6c2e 0a3e 2050 6f73 7467  incipal..> Postg
+00003210: 7265 733a 2046 6f72 2061 6e20 4941 4d20  res: For an IAM 
+00003220: 7573 6572 2061 6363 6f75 6e74 2c20 7468  user account, th
+00003230: 6973 2069 7320 7468 6520 7573 6572 2773  is is the user's
+00003240: 2065 6d61 696c 2061 6464 7265 7373 2e20   email address. 
+00003250: 466f 7220 6120 7365 7276 6963 6520 6163  For a service ac
+00003260: 636f 756e 742c 2069 7420 6973 2074 6865  count, it is the
+00003270: 2073 6572 7669 6365 2061 6363 6f75 6e74   service account
+00003280: 2773 2065 6d61 696c 2077 6974 686f 7574  's email without
+00003290: 2074 6865 2060 2e67 7365 7276 6963 6561   the `.gservicea
+000032a0: 6363 6f75 6e74 2e63 6f6d 6020 646f 6d61  ccount.com` doma
+000032b0: 696e 2073 7566 6669 782e 0a0a 3e20 4d79  in suffix...> My
+000032c0: 5351 4c3a 2046 6f72 2061 6e20 4941 4d20  SQL: For an IAM 
+000032d0: 7573 6572 2061 6363 6f75 6e74 2c20 7468  user account, th
+000032e0: 6973 2069 7320 7468 6520 7573 6572 2773  is is the user's
+000032f0: 2065 6d61 696c 2061 6464 7265 7373 2c20   email address, 
+00003300: 7769 7468 6f75 7420 7468 6520 4020 6f72  without the @ or
+00003310: 2064 6f6d 6169 6e20 6e61 6d65 2e20 466f   domain name. Fo
+00003320: 7220 6578 616d 706c 652c 2066 6f72 2060  r example, for `
+00003330: 7465 7374 2d75 7365 7240 676d 6169 6c2e  test-user@gmail.
+00003340: 636f 6d60 2c20 7365 7420 7468 6520 6075  com`, set the `u
+00003350: 7365 7260 2061 7267 756d 656e 7420 746f  ser` argument to
+00003360: 2060 7465 7374 2d75 7365 7260 2e20 466f   `test-user`. Fo
+00003370: 7220 6120 7365 7276 6963 6520 6163 636f  r a service acco
+00003380: 756e 742c 2074 6869 7320 6973 2074 6865  unt, this is the
+00003390: 2073 6572 7669 6365 2061 6363 6f75 6e74   service account
+000033a0: 2773 2065 6d61 696c 2061 6464 7265 7373  's email address
+000033b0: 2077 6974 686f 7574 2074 6865 2060 4070   without the `@p
+000033c0: 726f 6a65 6374 2d69 642e 6961 6d2e 6773  roject-id.iam.gs
+000033d0: 6572 7669 6365 6163 636f 756e 742e 636f  erviceaccount.co
+000033e0: 6d60 2073 7566 6669 782e 0a0a 4578 616d  m` suffix...Exam
+000033f0: 706c 653a 0a0a 6060 6070 7974 686f 6e0a  ple:..```python.
+00003400: 636f 6e6e 203d 2063 6f6e 6e65 6374 6f72  conn = connector
+00003410: 2e63 6f6e 6e65 6374 280a 2020 2020 2022  .connect(.     "
+00003420: 7072 6f6a 6563 743a 7265 6769 6f6e 3a69  project:region:i
+00003430: 6e73 7461 6e63 6522 2c0a 2020 2020 2022  nstance",.     "
+00003440: 7067 3830 3030 222c 0a20 2020 2020 7573  pg8000",.     us
+00003450: 6572 3d22 706f 7374 6772 6573 2d69 616d  er="postgres-iam
+00003460: 2d75 7365 7240 676d 6169 6c2e 636f 6d22  -user@gmail.com"
+00003470: 2c0a 2020 2020 2064 623d 226d 792d 6462  ,.     db="my-db
+00003480: 2d6e 616d 6522 2c0a 2020 2020 2065 6e61  -name",.     ena
+00003490: 626c 655f 6961 6d5f 6175 7468 3d54 7275  ble_iam_auth=Tru
+000034a0: 652c 0a20 290a 6060 600a 0a23 2323 2053  e,. ).```..### S
+000034b0: 514c 2053 6572 7665 7220 4163 7469 7665  QL Server Active
+000034c0: 2044 6972 6563 746f 7279 2041 7574 6865   Directory Authe
+000034d0: 6e74 6963 6174 696f 6e0a 0a41 6374 6976  ntication..Activ
+000034e0: 6520 4469 7265 6374 6f72 7920 6175 7468  e Directory auth
+000034f0: 656e 7469 6361 7469 6f6e 2066 6f72 2053  entication for S
+00003500: 514c 2053 6572 7665 7220 696e 7374 616e  QL Server instan
+00003510: 6365 7320 6973 2063 7572 7265 6e74 6c79  ces is currently
+00003520: 206f 6e6c 7920 7375 7070 6f72 7465 6420   only supported 
+00003530: 6f6e 2057 696e 646f 7773 2e20 4669 7273  on Windows. Firs
+00003540: 742c 206d 616b 6520 7375 7265 2074 6f20  t, make sure to 
+00003550: 666f 6c6c 6f77 205b 7468 6573 6520 7374  follow [these st
+00003560: 6570 735d 2868 7474 7073 3a2f 2f63 6c6f  eps](https://clo
+00003570: 7564 2e67 6f6f 676c 652e 636f 6d2f 626c  ud.google.com/bl
+00003580: 6f67 2f74 6f70 6963 732f 6465 7665 6c6f  og/topics/develo
+00003590: 7065 7273 2d70 7261 6374 6974 696f 6e65  pers-practitione
+000035a0: 7273 2f63 7265 6174 696e 672d 7371 6c2d  rs/creating-sql-
+000035b0: 7365 7276 6572 2d69 6e73 7461 6e63 652d  server-instance-
+000035c0: 696e 7465 6772 6174 6564 2d61 6374 6976  integrated-activ
+000035d0: 652d 6469 7265 6374 6f72 792d 7573 696e  e-directory-usin
+000035e0: 672d 676f 6f67 6c65 2d63 6c6f 7564 2d73  g-google-cloud-s
+000035f0: 716c 2920 746f 2073 6574 2075 7020 6120  ql) to set up a 
+00003600: 4d61 6e61 6765 6420 4144 2064 6f6d 6169  Managed AD domai
+00003610: 6e20 616e 6420 6a6f 696e 2079 6f75 7220  n and join your 
+00003620: 436c 6f75 6420 5351 4c20 696e 7374 616e  Cloud SQL instan
+00003630: 6365 2074 6f20 7468 6520 646f 6d61 696e  ce to the domain
+00003640: 2e20 5b53 6565 2068 6572 6520 666f 7220  . [See here for 
+00003650: 6d6f 7265 2069 6e66 6f20 6f6e 2043 6c6f  more info on Clo
+00003660: 7564 2053 514c 2041 6374 6976 6520 4469  ud SQL Active Di
+00003670: 7265 6374 6f72 7920 696e 7465 6772 6174  rectory integrat
+00003680: 696f 6e5d 2868 7474 7073 3a2f 2f63 6c6f  ion](https://clo
+00003690: 7564 2e67 6f6f 676c 652e 636f 6d2f 7371  ud.google.com/sq
+000036a0: 6c2f 646f 6373 2f73 716c 7365 7276 6572  l/docs/sqlserver
+000036b0: 2f61 6429 2e0a 0a4f 6e63 6520 796f 7520  /ad)...Once you 
+000036c0: 6861 7665 2066 6f6c 6c6f 7765 6420 7468  have followed th
+000036d0: 6520 7374 6570 7320 6c69 6e6b 6564 2061  e steps linked a
+000036e0: 626f 7665 2c20 796f 7520 6361 6e20 7275  bove, you can ru
+000036f0: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
+00003700: 636f 6465 2074 6f20 7265 7475 726e 2061  code to return a
+00003710: 2063 6f6e 6e65 6374 696f 6e20 6f62 6a65   connection obje
+00003720: 6374 3a0a 0a60 6060 7079 7468 6f6e 0a63  ct:..```python.c
+00003730: 6f6e 6e20 3d20 636f 6e6e 6563 746f 722e  onn = connector.
+00003740: 636f 6e6e 6563 7428 0a20 2020 2022 7072  connect(.    "pr
+00003750: 6f6a 6563 743a 7265 6769 6f6e 3a69 6e73  oject:region:ins
+00003760: 7461 6e63 6522 2c0a 2020 2020 2270 7974  tance",.    "pyt
+00003770: 6473 222c 0a20 2020 2064 623d 226d 792d  ds",.    db="my-
+00003780: 6462 2d6e 616d 6522 2c0a 2020 2020 6163  db-name",.    ac
+00003790: 7469 7665 5f64 6972 6563 746f 7279 5f61  tive_directory_a
+000037a0: 7574 683d 5472 7565 2c0a 2020 2020 7365  uth=True,.    se
+000037b0: 7276 6572 5f6e 616d 653d 2270 7562 6c69  rver_name="publi
+000037c0: 632e 5b69 6e73 7461 6e63 655d 2e5b 6c6f  c.[instance].[lo
+000037d0: 6361 7469 6f6e 5d2e 5b70 726f 6a65 6374  cation].[project
+000037e0: 5d2e 636c 6f75 6473 716c 2e5b 646f 6d61  ].cloudsql.[doma
+000037f0: 696e 5d22 2c0a 290a 6060 600a 0a4f 722c  in]",.).```..Or,
+00003800: 2069 6620 7573 696e 6720 5072 6976 6174   if using Privat
+00003810: 6520 4950 3a0a 0a60 6060 7079 7468 6f6e  e IP:..```python
+00003820: 0a63 6f6e 6e20 3d20 636f 6e6e 6563 746f  .conn = connecto
+00003830: 722e 636f 6e6e 6563 7428 0a20 2020 2022  r.connect(.    "
+00003840: 7072 6f6a 6563 743a 7265 6769 6f6e 3a69  project:region:i
+00003850: 6e73 7461 6e63 6522 2c0a 2020 2020 2270  nstance",.    "p
+00003860: 7974 6473 222c 0a20 2020 2064 623d 226d  ytds",.    db="m
+00003870: 792d 6462 2d6e 616d 6522 2c0a 2020 2020  y-db-name",.    
+00003880: 6163 7469 7665 5f64 6972 6563 746f 7279  active_directory
+00003890: 5f61 7574 683d 5472 7565 2c0a 2020 2020  _auth=True,.    
+000038a0: 7365 7276 6572 5f6e 616d 653d 2270 7269  server_name="pri
+000038b0: 7661 7465 2e5b 696e 7374 616e 6365 5d2e  vate.[instance].
+000038c0: 5b6c 6f63 6174 696f 6e5d 2e5b 7072 6f6a  [location].[proj
+000038d0: 6563 745d 2e63 6c6f 7564 7371 6c2e 5b64  ect].cloudsql.[d
+000038e0: 6f6d 6169 6e5d 222c 0a20 2020 2069 705f  omain]",.    ip_
+000038f0: 7479 7065 3d49 5054 7970 6573 2e50 5249  type=IPTypes.PRI
+00003900: 5641 5445 0a29 0a60 6060 0a0a 2323 2320  VATE.).```..### 
+00003910: 5573 696e 6720 7468 6520 5079 7468 6f6e  Using the Python
+00003920: 2043 6f6e 6e65 6374 6f72 2077 6974 6820   Connector with 
+00003930: 5079 7468 6f6e 2057 6562 2046 7261 6d65  Python Web Frame
+00003940: 776f 726b 730a 0a54 6865 2050 7974 686f  works..The Pytho
+00003950: 6e20 436f 6e6e 6563 746f 7220 6361 6e20  n Connector can 
+00003960: 6265 2075 7365 6420 616c 6f6e 6773 6964  be used alongsid
+00003970: 6520 706f 7075 6c61 7220 5079 7468 6f6e  e popular Python
+00003980: 2077 6562 2066 7261 6d65 776f 726b 7320   web frameworks 
+00003990: 7375 6368 0a61 7320 466c 6173 6b2c 2046  such.as Flask, F
+000039a0: 6173 7441 5049 2c20 6574 632c 2074 6f20  astAPI, etc, to 
+000039b0: 696e 7465 6772 6174 6520 436c 6f75 6420  integrate Cloud 
+000039c0: 5351 4c20 6461 7461 6261 7365 7320 7769  SQL databases wi
+000039d0: 7468 696e 2079 6f75 720a 7765 6220 6170  thin your.web ap
+000039e0: 706c 6963 6174 696f 6e73 2e0a 0a23 2323  plications...###
+000039f0: 2320 466c 6173 6b2d 5351 4c41 6c63 6865  # Flask-SQLAlche
+00003a00: 6d79 0a0a 5b46 6c61 736b 2d53 514c 416c  my..[Flask-SQLAl
+00003a10: 6368 656d 795d 2868 7474 7073 3a2f 2f66  chemy](https://f
+00003a20: 6c61 736b 2d73 716c 616c 6368 656d 792e  lask-sqlalchemy.
+00003a30: 7061 6c6c 6574 7370 726f 6a65 6374 732e  palletsprojects.
+00003a40: 636f 6d2f 656e 2f32 2e78 2f29 0a69 7320  com/en/2.x/).is 
+00003a50: 616e 2065 7874 656e 7369 6f6e 2066 6f72  an extension for
+00003a60: 205b 466c 6173 6b5d 2868 7474 7073 3a2f   [Flask](https:/
+00003a70: 2f66 6c61 736b 2e70 616c 6c65 7473 7072  /flask.palletspr
+00003a80: 6f6a 6563 7473 2e63 6f6d 2f65 6e2f 322e  ojects.com/en/2.
+00003a90: 322e 782f 290a 7468 6174 2061 6464 7320  2.x/).that adds 
+00003aa0: 7375 7070 6f72 7420 666f 7220 5b53 514c  support for [SQL
+00003ab0: 416c 6368 656d 795d 2868 7474 7073 3a2f  Alchemy](https:/
+00003ac0: 2f77 7777 2e73 716c 616c 6368 656d 792e  /www.sqlalchemy.
+00003ad0: 6f72 672f 2920 746f 2079 6f75 720a 6170  org/) to your.ap
+00003ae0: 706c 6963 6174 696f 6e2e 2049 7420 6169  plication. It ai
+00003af0: 6d73 2074 6f20 7369 6d70 6c69 6679 2075  ms to simplify u
+00003b00: 7369 6e67 2053 514c 416c 6368 656d 7920  sing SQLAlchemy 
+00003b10: 7769 7468 2046 6c61 736b 2062 7920 7072  with Flask by pr
+00003b20: 6f76 6964 696e 670a 7573 6566 756c 2064  oviding.useful d
+00003b30: 6566 6175 6c74 7320 616e 6420 6578 7472  efaults and extr
+00003b40: 6120 6865 6c70 6572 7320 7468 6174 206d  a helpers that m
+00003b50: 616b 6520 6974 2065 6173 6965 7220 746f  ake it easier to
+00003b60: 2061 6363 6f6d 706c 6973 680a 636f 6d6d   accomplish.comm
+00003b70: 6f6e 2074 6173 6b73 2e0a 0a59 6f75 2063  on tasks...You c
+00003b80: 616e 2063 6f6e 6669 6775 7265 2046 6c61  an configure Fla
+00003b90: 736b 2d53 514c 416c 6368 656d 7920 746f  sk-SQLAlchemy to
+00003ba0: 2063 6f6e 6e65 6374 2074 6f20 6120 436c   connect to a Cl
+00003bb0: 6f75 6420 5351 4c20 6461 7461 6261 7365  oud SQL database
+00003bc0: 2066 726f 6d0a 796f 7572 2077 6562 2061   from.your web a
+00003bd0: 7070 6c69 6361 7469 6f6e 2074 6872 6f75  pplication throu
+00003be0: 6768 2074 6865 2066 6f6c 6c6f 7769 6e67  gh the following
+00003bf0: 3a0a 0a60 6060 7079 7468 6f6e 0a66 726f  :..```python.fro
+00003c00: 6d20 666c 6173 6b20 696d 706f 7274 2046  m flask import F
+00003c10: 6c61 736b 0a66 726f 6d20 666c 6173 6b5f  lask.from flask_
+00003c20: 7371 6c61 6c63 6865 6d79 2069 6d70 6f72  sqlalchemy impor
+00003c30: 7420 5351 4c41 6c63 6865 6d79 0a66 726f  t SQLAlchemy.fro
+00003c40: 6d20 676f 6f67 6c65 2e63 6c6f 7564 2e73  m google.cloud.s
+00003c50: 716c 2e63 6f6e 6e65 6374 6f72 2069 6d70  ql.connector imp
+00003c60: 6f72 7420 436f 6e6e 6563 746f 722c 2049  ort Connector, I
+00003c70: 5054 7970 6573 0a0a 0a23 2069 6e69 7469  PTypes...# initi
+00003c80: 616c 697a 6520 5079 7468 6f6e 2043 6f6e  alize Python Con
+00003c90: 6e65 6374 6f72 206f 626a 6563 740a 636f  nector object.co
+00003ca0: 6e6e 6563 746f 7220 3d20 436f 6e6e 6563  nnector = Connec
+00003cb0: 746f 7228 290a 0a23 2050 7974 686f 6e20  tor()..# Python 
+00003cc0: 436f 6e6e 6563 746f 7220 6461 7461 6261  Connector databa
+00003cd0: 7365 2063 6f6e 6e65 6374 696f 6e20 6675  se connection fu
+00003ce0: 6e63 7469 6f6e 0a64 6566 2067 6574 636f  nction.def getco
+00003cf0: 6e6e 2829 3a0a 2020 2020 636f 6e6e 203d  nn():.    conn =
+00003d00: 2063 6f6e 6e65 6374 6f72 2e63 6f6e 6e65   connector.conne
+00003d10: 6374 280a 2020 2020 2020 2020 2270 726f  ct(.        "pro
+00003d20: 6a65 6374 3a72 6567 696f 6e3a 696e 7374  ject:region:inst
+00003d30: 616e 6365 2d6e 616d 6522 2c20 2320 436c  ance-name", # Cl
+00003d40: 6f75 6420 5351 4c20 496e 7374 616e 6365  oud SQL Instance
+00003d50: 2043 6f6e 6e65 6374 696f 6e20 4e61 6d65   Connection Name
+00003d60: 0a20 2020 2020 2020 2022 7067 3830 3030  .        "pg8000
+00003d70: 222c 0a20 2020 2020 2020 2075 7365 723d  ",.        user=
+00003d80: 226d 792d 7573 6572 222c 0a20 2020 2020  "my-user",.     
+00003d90: 2020 2070 6173 7377 6f72 643d 226d 792d     password="my-
+00003da0: 7061 7373 776f 7264 222c 0a20 2020 2020  password",.     
+00003db0: 2020 2064 623d 226d 792d 6461 7461 6261     db="my-databa
+00003dc0: 7365 222c 0a20 2020 2020 2020 2069 705f  se",.        ip_
+00003dd0: 7479 7065 3d20 4950 5479 7065 732e 5055  type= IPTypes.PU
+00003de0: 424c 4943 2020 2320 4950 5479 7065 732e  BLIC  # IPTypes.
+00003df0: 5052 4956 4154 4520 666f 7220 7072 6976  PRIVATE for priv
+00003e00: 6174 6520 4950 0a20 2020 2029 0a20 2020  ate IP.    ).   
+00003e10: 2072 6574 7572 6e20 636f 6e6e 0a0a 0a61   return conn...a
+00003e20: 7070 203d 2046 6c61 736b 285f 5f6e 616d  pp = Flask(__nam
+00003e30: 655f 5f29 0a0a 2320 636f 6e66 6967 7572  e__)..# configur
+00003e40: 6520 466c 6173 6b2d 5351 4c41 6c63 6865  e Flask-SQLAlche
+00003e50: 6d79 2074 6f20 7573 6520 5079 7468 6f6e  my to use Python
+00003e60: 2043 6f6e 6e65 6374 6f72 0a61 7070 2e63   Connector.app.c
+00003e70: 6f6e 6669 675b 2753 514c 414c 4348 454d  onfig['SQLALCHEM
+00003e80: 595f 4441 5441 4241 5345 5f55 5249 275d  Y_DATABASE_URI']
+00003e90: 203d 2022 706f 7374 6772 6573 716c 2b70   = "postgresql+p
+00003ea0: 6738 3030 303a 2f2f 220a 6170 702e 636f  g8000://".app.co
+00003eb0: 6e66 6967 5b27 5351 4c41 4c43 4845 4d59  nfig['SQLALCHEMY
+00003ec0: 5f45 4e47 494e 455f 4f50 5449 4f4e 5327  _ENGINE_OPTIONS'
+00003ed0: 5d20 3d20 7b0a 2020 2020 2263 7265 6174  ] = {.    "creat
+00003ee0: 6f72 223a 2067 6574 636f 6e6e 0a7d 0a0a  or": getconn.}..
+00003ef0: 2320 696e 6974 6961 6c69 7a65 2074 6865  # initialize the
+00003f00: 2061 7070 2077 6974 6820 7468 6520 6578   app with the ex
+00003f10: 7465 6e73 696f 6e0a 6462 203d 2053 514c  tension.db = SQL
+00003f20: 416c 6368 656d 7928 290a 6462 2e69 6e69  Alchemy().db.ini
+00003f30: 745f 6170 7028 6170 7029 0a60 6060 0a0a  t_app(app).```..
+00003f40: 466f 7220 6d6f 7265 2064 6574 6169 6c73  For more details
+00003f50: 206f 6e20 686f 7720 746f 2075 7365 2046   on how to use F
+00003f60: 6c61 736b 2d53 514c 416c 6368 656d 792c  lask-SQLAlchemy,
+00003f70: 2063 6865 636b 206f 7574 2074 6865 0a5b   check out the.[
+00003f80: 466c 6173 6b2d 5351 4c41 6c63 6865 6d79  Flask-SQLAlchemy
+00003f90: 2051 7569 636b 7374 6172 7473 5d28 6874   Quickstarts](ht
+00003fa0: 7470 733a 2f2f 666c 6173 6b2d 7371 6c61  tps://flask-sqla
+00003fb0: 6c63 6865 6d79 2e70 616c 6c65 7473 7072  lchemy.palletspr
+00003fc0: 6f6a 6563 7473 2e63 6f6d 2f65 6e2f 332e  ojects.com/en/3.
+00003fd0: 302e 782f 7175 6963 6b73 7461 7274 2f29  0.x/quickstart/)
+00003fe0: 0a0a 2323 2323 2046 6173 7441 5049 0a0a  ..#### FastAPI..
+00003ff0: 5b46 6173 7441 5049 5d28 6874 7470 733a  [FastAPI](https:
+00004000: 2f2f 6661 7374 6170 692e 7469 616e 676f  //fastapi.tiango
+00004010: 6c6f 2e63 6f6d 2f29 2069 7320 6120 6d6f  lo.com/) is a mo
+00004020: 6465 726e 2c20 6661 7374 2028 6869 6768  dern, fast (high
+00004030: 2d70 6572 666f 726d 616e 6365 292c 0a77  -performance),.w
+00004040: 6562 2066 7261 6d65 776f 726b 2066 6f72  eb framework for
+00004050: 2062 7569 6c64 696e 6720 4150 4973 2077   building APIs w
+00004060: 6974 6820 5079 7468 6f6e 2062 6173 6564  ith Python based
+00004070: 206f 6e20 7374 616e 6461 7264 2050 7974   on standard Pyt
+00004080: 686f 6e20 7479 7065 2068 696e 7473 2e0a  hon type hints..
+00004090: 0a59 6f75 2063 616e 2063 6f6e 6669 6775  .You can configu
+000040a0: 7265 2046 6173 7441 5049 2074 6f20 636f  re FastAPI to co
+000040b0: 6e6e 6563 7420 746f 2061 2043 6c6f 7564  nnect to a Cloud
+000040c0: 2053 514c 2064 6174 6162 6173 6520 6672   SQL database fr
+000040d0: 6f6d 0a79 6f75 7220 7765 6220 6170 706c  om.your web appl
+000040e0: 6963 6174 696f 6e20 7573 696e 6720 5b53  ication using [S
+000040f0: 514c 416c 6368 656d 7920 4f52 4d5d 2868  QLAlchemy ORM](h
+00004100: 7474 7073 3a2f 2f64 6f63 732e 7371 6c61  ttps://docs.sqla
+00004110: 6c63 6865 6d79 2e6f 7267 2f65 6e2f 3134  lchemy.org/en/14
+00004120: 2f6f 726d 2f29 0a74 6872 6f75 6768 2074  /orm/).through t
+00004130: 6865 2066 6f6c 6c6f 7769 6e67 3a0a 0a60  he following:..`
+00004140: 6060 7079 7468 6f6e 0a66 726f 6d20 7371  ``python.from sq
+00004150: 6c61 6c63 6865 6d79 2069 6d70 6f72 7420  lalchemy import 
+00004160: 6372 6561 7465 5f65 6e67 696e 650a 6672  create_engine.fr
+00004170: 6f6d 2073 716c 616c 6368 656d 792e 656e  om sqlalchemy.en
+00004180: 6769 6e65 2069 6d70 6f72 7420 456e 6769  gine import Engi
+00004190: 6e65 0a66 726f 6d20 7371 6c61 6c63 6865  ne.from sqlalche
+000041a0: 6d79 2e65 7874 2e64 6563 6c61 7261 7469  my.ext.declarati
+000041b0: 7665 2069 6d70 6f72 7420 6465 636c 6172  ve import declar
+000041c0: 6174 6976 655f 6261 7365 0a66 726f 6d20  ative_base.from 
+000041d0: 7371 6c61 6c63 6865 6d79 2e6f 726d 2069  sqlalchemy.orm i
+000041e0: 6d70 6f72 7420 7365 7373 696f 6e6d 616b  mport sessionmak
+000041f0: 6572 0a66 726f 6d20 676f 6f67 6c65 2e63  er.from google.c
+00004200: 6c6f 7564 2e73 716c 2e63 6f6e 6e65 6374  loud.sql.connect
+00004210: 6f72 2069 6d70 6f72 7420 436f 6e6e 6563  or import Connec
+00004220: 746f 722c 2049 5054 7970 6573 0a0a 2320  tor, IPTypes..# 
+00004230: 6865 6c70 6572 2066 756e 6374 696f 6e20  helper function 
+00004240: 746f 2072 6574 7572 6e20 5351 4c41 6c63  to return SQLAlc
+00004250: 6865 6d79 2063 6f6e 6e65 6374 696f 6e20  hemy connection 
+00004260: 706f 6f6c 0a64 6566 2069 6e69 745f 636f  pool.def init_co
+00004270: 6e6e 6563 7469 6f6e 5f70 6f6f 6c28 636f  nnection_pool(co
+00004280: 6e6e 6563 746f 723a 2043 6f6e 6e65 6374  nnector: Connect
+00004290: 6f72 2920 2d3e 2045 6e67 696e 653a 0a20  or) -> Engine:. 
+000042a0: 2020 2023 2050 7974 686f 6e20 436f 6e6e     # Python Conn
+000042b0: 6563 746f 7220 6461 7461 6261 7365 2063  ector database c
+000042c0: 6f6e 6e65 6374 696f 6e20 6675 6e63 7469  onnection functi
+000042d0: 6f6e 0a20 2020 2064 6566 2067 6574 636f  on.    def getco
+000042e0: 6e6e 2829 3a0a 2020 2020 2020 2020 636f  nn():.        co
+000042f0: 6e6e 203d 2063 6f6e 6e65 6374 6f72 2e63  nn = connector.c
+00004300: 6f6e 6e65 6374 280a 2020 2020 2020 2020  onnect(.        
+00004310: 2020 2020 2270 726f 6a65 6374 3a72 6567      "project:reg
+00004320: 696f 6e3a 696e 7374 616e 6365 2d6e 616d  ion:instance-nam
+00004330: 6522 2c20 2320 436c 6f75 6420 5351 4c20  e", # Cloud SQL 
+00004340: 496e 7374 616e 6365 2043 6f6e 6e65 6374  Instance Connect
+00004350: 696f 6e20 4e61 6d65 0a20 2020 2020 2020  ion Name.       
+00004360: 2020 2020 2022 7067 3830 3030 222c 0a20       "pg8000",. 
+00004370: 2020 2020 2020 2020 2020 2075 7365 723d             user=
+00004380: 226d 792d 7573 6572 222c 0a20 2020 2020  "my-user",.     
+00004390: 2020 2020 2020 2070 6173 7377 6f72 643d         password=
+000043a0: 226d 792d 7061 7373 776f 7264 222c 0a20  "my-password",. 
+000043b0: 2020 2020 2020 2020 2020 2064 623d 226d             db="m
+000043c0: 792d 6461 7461 6261 7365 222c 0a20 2020  y-database",.   
+000043d0: 2020 2020 2020 2020 2069 705f 7479 7065           ip_type
+000043e0: 3d20 4950 5479 7065 732e 5055 424c 4943  = IPTypes.PUBLIC
+000043f0: 2020 2320 4950 5479 7065 732e 5052 4956    # IPTypes.PRIV
+00004400: 4154 4520 666f 7220 7072 6976 6174 6520  ATE for private 
+00004410: 4950 0a20 2020 2020 2020 2029 0a20 2020  IP.        ).   
+00004420: 2020 2020 2072 6574 7572 6e20 636f 6e6e       return conn
+00004430: 0a0a 2020 2020 5351 4c41 4c43 4845 4d59  ..    SQLALCHEMY
+00004440: 5f44 4154 4142 4153 455f 5552 4c20 3d20  _DATABASE_URL = 
+00004450: 2270 6f73 7467 7265 7371 6c2b 7067 3830  "postgresql+pg80
+00004460: 3030 3a2f 2f22 0a0a 2020 2020 656e 6769  00://"..    engi
+00004470: 6e65 203d 2063 7265 6174 655f 656e 6769  ne = create_engi
+00004480: 6e65 280a 2020 2020 2020 2020 5351 4c41  ne(.        SQLA
+00004490: 4c43 4845 4d59 5f44 4154 4142 4153 455f  LCHEMY_DATABASE_
+000044a0: 5552 4c20 2c20 6372 6561 746f 723d 6765  URL , creator=ge
+000044b0: 7463 6f6e 6e0a 2020 2020 290a 2020 2020  tconn.    ).    
+000044c0: 7265 7475 726e 2065 6e67 696e 650a 0a23  return engine..#
+000044d0: 2069 6e69 7469 616c 697a 6520 436c 6f75   initialize Clou
+000044e0: 6420 5351 4c20 5079 7468 6f6e 2043 6f6e  d SQL Python Con
+000044f0: 6e65 6374 6f72 0a63 6f6e 6e65 6374 6f72  nector.connector
+00004500: 203d 2043 6f6e 6e65 6374 6f72 2829 0a0a   = Connector()..
+00004510: 2320 6372 6561 7465 2063 6f6e 6e65 6374  # create connect
+00004520: 696f 6e20 706f 6f6c 2065 6e67 696e 650a  ion pool engine.
+00004530: 656e 6769 6e65 203d 2069 6e69 745f 636f  engine = init_co
+00004540: 6e6e 6563 7469 6f6e 5f70 6f6f 6c28 636f  nnection_pool(co
+00004550: 6e6e 6563 746f 7229 0a0a 2320 6372 6561  nnector)..# crea
+00004560: 7465 2053 514c 416c 6368 656d 7920 4f52  te SQLAlchemy OR
+00004570: 4d20 7365 7373 696f 6e0a 5365 7373 696f  M session.Sessio
+00004580: 6e4c 6f63 616c 203d 2073 6573 7369 6f6e  nLocal = session
+00004590: 6d61 6b65 7228 6175 746f 636f 6d6d 6974  maker(autocommit
+000045a0: 3d46 616c 7365 2c20 6175 746f 666c 7573  =False, autoflus
+000045b0: 683d 4661 6c73 652c 2062 696e 643d 656e  h=False, bind=en
+000045c0: 6769 6e65 290a 0a42 6173 6520 3d20 6465  gine)..Base = de
+000045d0: 636c 6172 6174 6976 655f 6261 7365 2829  clarative_base()
+000045e0: 0a60 6060 0a0a 546f 206c 6561 726e 206d  .```..To learn m
+000045f0: 6f72 6520 6162 6f75 7420 696e 7465 6772  ore about integr
+00004600: 6174 696e 6720 6120 6461 7461 6261 7365  ating a database
+00004610: 2069 6e74 6f20 796f 7572 2046 6173 7441   into your FastA
+00004620: 5049 2061 7070 6c69 6361 7469 6f6e 2c0a  PI application,.
+00004630: 666f 6c6c 6f77 2061 6c6f 6e67 2074 6865  follow along the
+00004640: 205b 4661 7374 4150 4920 5351 4c20 4461   [FastAPI SQL Da
+00004650: 7461 6261 7365 2067 7569 6465 5d28 6874  tabase guide](ht
+00004660: 7470 733a 2f2f 6661 7374 6170 692e 7469  tps://fastapi.ti
+00004670: 616e 676f 6c6f 2e63 6f6d 2f74 7574 6f72  angolo.com/tutor
+00004680: 6961 6c2f 7371 6c2d 6461 7461 6261 7365  ial/sql-database
+00004690: 732f 2363 7265 6174 652d 7468 652d 6461  s/#create-the-da
+000046a0: 7461 6261 7365 2d6d 6f64 656c 7329 2e0a  tabase-models)..
+000046b0: 0a23 2323 2041 7379 6e63 2044 7269 7665  .### Async Drive
+000046c0: 7220 5573 6167 650a 0a54 6865 2043 6c6f  r Usage..The Clo
+000046d0: 7564 2053 514c 2043 6f6e 6e65 6374 6f72  ud SQL Connector
+000046e0: 2069 7320 636f 6d70 6174 6962 6c65 2077   is compatible w
+000046f0: 6974 680a 5b61 7379 6e63 696f 5d28 6874  ith.[asyncio](ht
+00004700: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
+00004710: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
+00004720: 6173 796e 6369 6f2e 6874 6d6c 2920 746f  asyncio.html) to
+00004730: 2069 6d70 726f 7665 2074 6865 2073 7065   improve the spe
+00004740: 6564 0a61 6e64 2065 6666 6963 6965 6e63  ed.and efficienc
+00004750: 7920 6f66 2064 6174 6162 6173 6520 636f  y of database co
+00004760: 6e6e 6563 7469 6f6e 7320 7468 726f 7567  nnections throug
+00004770: 6820 636f 6e63 7572 7265 6e63 792e 2059  h concurrency. Y
+00004780: 6f75 2063 616e 2075 7365 2061 6c6c 0a6e  ou can use all.n
+00004790: 6f6e 2d61 7379 6e63 696f 2064 7269 7665  on-asyncio drive
+000047a0: 7273 2074 6872 6f75 6768 2074 6865 2060  rs through the `
+000047b0: 436f 6e6e 6563 746f 722e 636f 6e6e 6563  Connector.connec
+000047c0: 745f 6173 796e 6360 2066 756e 6374 696f  t_async` functio
+000047d0: 6e2c 2069 6e20 6164 6469 7469 6f6e 0a74  n, in addition.t
+000047e0: 6f20 7468 6520 666f 6c6c 6f77 696e 6720  o the following 
+000047f0: 6173 796e 6369 6f20 6461 7461 6261 7365  asyncio database
+00004800: 2064 7269 7665 7273 3a0a 2d20 5b61 7379   drivers:.- [asy
+00004810: 6e63 7067 5d28 6874 7470 733a 2f2f 6d61  ncpg](https://ma
+00004820: 6769 6373 7461 636b 2e67 6974 6875 622e  gicstack.github.
+00004830: 696f 2f61 7379 6e63 7067 2920 2850 6f73  io/asyncpg) (Pos
+00004840: 7467 7265 7329 0a0a 5468 6520 436c 6f75  tgres)..The Clou
+00004850: 6420 5351 4c20 436f 6e6e 6563 746f 7220  d SQL Connector 
+00004860: 6861 7320 6120 6865 6c70 6572 2060 6372  has a helper `cr
+00004870: 6561 7465 5f61 7379 6e63 5f63 6f6e 6e65  eate_async_conne
+00004880: 6374 6f72 6020 6675 6e63 7469 6f6e 2074  ctor` function t
+00004890: 6861 7420 6973 0a72 6563 6f6d 6d65 6e64  hat is.recommend
+000048a0: 6564 2066 6f72 2061 7379 6e63 696f 2064  ed for asyncio d
+000048b0: 6174 6162 6173 6520 636f 6e6e 6563 7469  atabase connecti
+000048c0: 6f6e 732e 2049 7420 7265 7475 726e 7320  ons. It returns 
+000048d0: 6120 6043 6f6e 6e65 6374 6f72 600a 6f62  a `Connector`.ob
+000048e0: 6a65 6374 2074 6861 7420 7573 6573 2074  ject that uses t
+000048f0: 6865 2063 7572 7265 6e74 2074 6872 6561  he current threa
+00004900: 6427 7320 7275 6e6e 696e 6720 6576 656e  d's running even
+00004910: 7420 6c6f 6f70 2e20 5468 6973 2069 7320  t loop. This is 
+00004920: 6469 6666 6572 656e 740a 7468 616e 2060  different.than `
+00004930: 436f 6e6e 6563 746f 7228 2960 2077 6869  Connector()` whi
+00004940: 6368 2062 7920 6465 6661 756c 7420 696e  ch by default in
+00004950: 6974 6961 6c69 7a65 7320 6120 6e65 7720  itializes a new 
+00004960: 6576 656e 7420 6c6f 6f70 2069 6e20 610a  event loop in a.
+00004970: 6261 636b 6772 6f75 6e64 2074 6872 6561  background threa
+00004980: 642e 0a0a 5468 6520 6063 7265 6174 655f  d...The `create_
+00004990: 6173 796e 635f 636f 6e6e 6563 746f 7260  async_connector`
+000049a0: 2061 6c6c 6f77 7320 616c 6c20 7468 6520   allows all the 
+000049b0: 7361 6d65 2069 6e70 7574 2061 7267 756d  same input argum
+000049c0: 656e 7473 2061 7320 7468 650a 5b43 6f6e  ents as the.[Con
+000049d0: 6e65 6374 6f72 5d28 2363 6f6e 6669 6775  nector](#configu
+000049e0: 7269 6e67 2d74 6865 2d63 6f6e 6e65 6374  ring-the-connect
+000049f0: 6f72 2920 6f62 6a65 6374 2e0a 0a4f 6e63  or) object...Onc
+00004a00: 6520 6120 6043 6f6e 6e65 6374 6f72 6020  e a `Connector` 
+00004a10: 6f62 6a65 6374 2069 7320 7265 7475 726e  object is return
+00004a20: 6564 2062 7920 6063 7265 6174 655f 6173  ed by `create_as
+00004a30: 796e 635f 636f 6e6e 6563 746f 7260 2079  ync_connector` y
+00004a40: 6f75 2063 616e 2063 616c 6c0a 6974 7320  ou can call.its 
+00004a50: 6063 6f6e 6e65 6374 5f61 7379 6e63 6020  `connect_async` 
+00004a60: 6d65 7468 6f64 2c20 6a75 7374 2061 7320  method, just as 
+00004a70: 796f 7520 776f 756c 6420 7468 6520 6063  you would the `c
+00004a80: 6f6e 6e65 6374 6020 6d65 7468 6f64 3a0a  onnect` method:.
+00004a90: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
+00004aa0: 7420 6173 796e 6370 670a 0a69 6d70 6f72  t asyncpg..impor
+00004ab0: 7420 7371 6c61 6c63 6865 6d79 0a66 726f  t sqlalchemy.fro
+00004ac0: 6d20 7371 6c61 6c63 6865 6d79 2e65 7874  m sqlalchemy.ext
+00004ad0: 2e61 7379 6e63 696f 2069 6d70 6f72 7420  .asyncio import 
+00004ae0: 4173 796e 6345 6e67 696e 652c 2063 7265  AsyncEngine, cre
+00004af0: 6174 655f 6173 796e 635f 656e 6769 6e65  ate_async_engine
+00004b00: 0a0a 6672 6f6d 2067 6f6f 676c 652e 636c  ..from google.cl
+00004b10: 6f75 642e 7371 6c2e 636f 6e6e 6563 746f  oud.sql.connecto
+00004b20: 7220 696d 706f 7274 2043 6f6e 6e65 6374  r import Connect
+00004b30: 6f72 2c20 6372 6561 7465 5f61 7379 6e63  or, create_async
+00004b40: 5f63 6f6e 6e65 6374 6f72 0a0a 6173 796e  _connector..asyn
+00004b50: 6320 6465 6620 696e 6974 5f63 6f6e 6e65  c def init_conne
+00004b60: 6374 696f 6e5f 706f 6f6c 2863 6f6e 6e65  ction_pool(conne
+00004b70: 6374 6f72 3a20 436f 6e6e 6563 746f 7229  ctor: Connector)
+00004b80: 202d 3e20 4173 796e 6345 6e67 696e 653a   -> AsyncEngine:
+00004b90: 0a20 2020 2023 2069 6e69 7469 616c 697a  .    # initializ
+00004ba0: 6520 436f 6e6e 6563 746f 7220 6f62 6a65  e Connector obje
+00004bb0: 6374 2066 6f72 2063 6f6e 6e65 6374 696f  ct for connectio
+00004bc0: 6e73 2074 6f20 436c 6f75 6420 5351 4c0a  ns to Cloud SQL.
+00004bd0: 2020 2020 6173 796e 6320 6465 6620 6765      async def ge
+00004be0: 7463 6f6e 6e28 2920 2d3e 2061 7379 6e63  tconn() -> async
+00004bf0: 7067 2e43 6f6e 6e65 6374 696f 6e3a 0a20  pg.Connection:. 
+00004c00: 2020 2020 2020 2063 6f6e 6e3a 2061 7379         conn: asy
+00004c10: 6e63 7067 2e43 6f6e 6e65 6374 696f 6e20  ncpg.Connection 
+00004c20: 3d20 6177 6169 7420 636f 6e6e 6563 746f  = await connecto
+00004c30: 722e 636f 6e6e 6563 745f 6173 796e 6328  r.connect_async(
+00004c40: 0a20 2020 2020 2020 2020 2020 2022 7072  .            "pr
+00004c50: 6f6a 6563 743a 7265 6769 6f6e 3a69 6e73  oject:region:ins
+00004c60: 7461 6e63 6522 2c20 2023 2043 6c6f 7564  tance",  # Cloud
+00004c70: 2053 514c 2069 6e73 7461 6e63 6520 636f   SQL instance co
+00004c80: 6e6e 6563 7469 6f6e 206e 616d 650a 2020  nnection name.  
+00004c90: 2020 2020 2020 2020 2020 2261 7379 6e63            "async
+00004ca0: 7067 222c 0a20 2020 2020 2020 2020 2020  pg",.           
+00004cb0: 2075 7365 723d 226d 792d 7573 6572 222c   user="my-user",
+00004cc0: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
+00004cd0: 7377 6f72 643d 226d 792d 7061 7373 776f  sword="my-passwo
+00004ce0: 7264 222c 0a20 2020 2020 2020 2020 2020  rd",.           
+00004cf0: 2064 623d 226d 792d 6462 2d6e 616d 6522   db="my-db-name"
+00004d00: 0a20 2020 2020 2020 2020 2020 2023 202e  .            # .
+00004d10: 2e2e 2061 6464 6974 696f 6e61 6c20 6461  .. additional da
+00004d20: 7461 6261 7365 2064 7269 7665 7220 6172  tabase driver ar
+00004d30: 6773 0a20 2020 2020 2020 2029 0a20 2020  gs.        ).   
+00004d40: 2020 2020 2072 6574 7572 6e20 636f 6e6e       return conn
+00004d50: 0a0a 2020 2020 2320 5468 6520 436c 6f75  ..    # The Clou
+00004d60: 6420 5351 4c20 5079 7468 6f6e 2043 6f6e  d SQL Python Con
+00004d70: 6e65 6374 6f72 2063 616e 2062 6520 7573  nector can be us
+00004d80: 6564 2061 6c6f 6e67 2077 6974 6820 5351  ed along with SQ
+00004d90: 4c41 6c63 6865 6d79 2075 7369 6e67 2074  LAlchemy using t
+00004da0: 6865 0a20 2020 2023 2027 6173 796e 635f  he.    # 'async_
+00004db0: 6372 6561 746f 7227 2061 7267 756d 656e  creator' argumen
+00004dc0: 7420 746f 2027 6372 6561 7465 5f61 7379  t to 'create_asy
+00004dd0: 6e63 5f65 6e67 696e 6527 0a20 2020 2070  nc_engine'.    p
+00004de0: 6f6f 6c20 3d20 6372 6561 7465 5f61 7379  ool = create_asy
+00004df0: 6e63 5f65 6e67 696e 6528 0a20 2020 2020  nc_engine(.     
+00004e00: 2020 2022 706f 7374 6772 6573 716c 2b61     "postgresql+a
+00004e10: 7379 6e63 7067 3a2f 2f22 2c0a 2020 2020  syncpg://",.    
+00004e20: 2020 2020 6173 796e 635f 6372 6561 746f      async_creato
+00004e30: 723d 6765 7463 6f6e 6e2c 0a20 2020 2029  r=getconn,.    )
+00004e40: 0a20 2020 2072 6574 7572 6e20 706f 6f6c  .    return pool
+00004e50: 0a0a 6173 796e 6320 6465 6620 6d61 696e  ..async def main
+00004e60: 2829 3a0a 2020 2020 2320 696e 6974 6961  ():.    # initia
+00004e70: 6c69 7a65 2043 6f6e 6e65 6374 6f72 206f  lize Connector o
+00004e80: 626a 6563 7420 666f 7220 636f 6e6e 6563  bject for connec
+00004e90: 7469 6f6e 7320 746f 2043 6c6f 7564 2053  tions to Cloud S
+00004ea0: 514c 0a20 2020 2063 6f6e 6e65 6374 6f72  QL.    connector
+00004eb0: 203d 2061 7761 6974 2063 7265 6174 655f   = await create_
+00004ec0: 6173 796e 635f 636f 6e6e 6563 746f 7228  async_connector(
+00004ed0: 290a 0a20 2020 2023 2069 6e69 7469 616c  )..    # initial
+00004ee0: 697a 6520 636f 6e6e 6563 7469 6f6e 2070  ize connection p
+00004ef0: 6f6f 6c0a 2020 2020 706f 6f6c 203d 2061  ool.    pool = a
+00004f00: 7761 6974 2069 6e69 745f 636f 6e6e 6563  wait init_connec
+00004f10: 7469 6f6e 5f70 6f6f 6c28 636f 6e6e 6563  tion_pool(connec
+00004f20: 746f 7229 0a0a 2020 2020 2320 6578 616d  tor)..    # exam
+00004f30: 706c 6520 7175 6572 790a 2020 2020 6173  ple query.    as
+00004f40: 796e 6320 7769 7468 2070 6f6f 6c2e 636f  ync with pool.co
+00004f50: 6e6e 6563 7428 2920 6173 2063 6f6e 6e3a  nnect() as conn:
+00004f60: 0a20 2020 2020 2020 2061 7761 6974 2063  .        await c
+00004f70: 6f6e 6e2e 6578 6563 7574 6528 7371 6c61  onn.execute(sqla
+00004f80: 6c63 6865 6d79 2e74 6578 7428 2253 454c  lchemy.text("SEL
+00004f90: 4543 5420 4e4f 5728 2922 2929 0a0a 2020  ECT NOW()"))..  
+00004fa0: 2020 2320 636c 6f73 6520 436f 6e6e 6563    # close Connec
+00004fb0: 746f 720a 2020 2020 6177 6169 7420 636f  tor.    await co
+00004fc0: 6e6e 6563 746f 722e 636c 6f73 655f 6173  nnector.close_as
+00004fd0: 796e 6328 290a 0a20 2020 2023 2064 6973  ync()..    # dis
+00004fe0: 706f 7365 206f 6620 636f 6e6e 6563 7469  pose of connecti
+00004ff0: 6f6e 2070 6f6f 6c0a 2020 2020 6177 6169  on pool.    awai
+00005000: 7420 706f 6f6c 2e64 6973 706f 7365 2829  t pool.dispose()
+00005010: 0a60 6060 0a0a 466f 7220 6d6f 7265 2064  .```..For more d
+00005020: 6574 6169 6c73 206f 6e20 6164 6469 7469  etails on additi
+00005030: 6f6e 616c 2064 6174 6162 6173 6520 6172  onal database ar
+00005040: 6775 6d65 6e74 7320 7769 7468 2061 6e20  guments with an 
+00005050: 6061 7379 6e63 7067 2e43 6f6e 6e65 6374  `asyncpg.Connect
+00005060: 696f 6e60 0a2c 2070 6c65 6173 6520 7669  ion`., please vi
+00005070: 7369 7420 7468 650a 5b6f 6666 6963 6961  sit the.[officia
+00005080: 6c20 646f 6375 6d65 6e74 6174 696f 6e5d  l documentation]
+00005090: 2868 7474 7073 3a2f 2f6d 6167 6963 7374  (https://magicst
+000050a0: 6163 6b2e 6769 7468 7562 2e69 6f2f 6173  ack.github.io/as
+000050b0: 796e 6370 672f 6375 7272 656e 742f 6170  yncpg/current/ap
+000050c0: 692f 696e 6465 782e 6874 6d6c 292e 0a0a  i/index.html)...
+000050d0: 2323 2320 4173 796e 6320 436f 6e74 6578  ### Async Contex
+000050e0: 7420 4d61 6e61 6765 720a 0a41 6e20 616c  t Manager..An al
+000050f0: 7465 726e 6174 6976 6520 746f 2075 7369  ternative to usi
+00005100: 6e67 2074 6865 2060 6372 6561 7465 5f61  ng the `create_a
+00005110: 7379 6e63 5f63 6f6e 6e65 6374 6f72 6020  sync_connector` 
+00005120: 6675 6e63 7469 6f6e 2069 7320 696e 6974  function is init
+00005130: 6961 6c69 7a69 6e67 0a61 2060 436f 6e6e  ializing.a `Conn
+00005140: 6563 746f 7260 2061 7320 616e 2061 7379  ector` as an asy
+00005150: 6e63 2063 6f6e 7465 7874 206d 616e 6167  nc context manag
+00005160: 6572 2c20 7265 6d6f 7669 6e67 2074 6865  er, removing the
+00005170: 206e 6565 6420 666f 7220 6578 706c 6963   need for explic
+00005180: 6974 0a63 616c 6c73 2074 6f20 6063 6f6e  it.calls to `con
+00005190: 6e65 6374 6f72 2e63 6c6f 7365 5f61 7379  nector.close_asy
+000051a0: 6e63 2829 6020 746f 2063 6c65 616e 7570  nc()` to cleanup
+000051b0: 2072 6573 6f75 7263 6573 2e0a 0a2a 2a4e   resources...**N
+000051c0: 6f74 653a 2a2a 2054 6869 7320 616c 7465  ote:** This alte
+000051d0: 726e 6174 6976 6520 7265 7175 6972 6573  rnative requires
+000051e0: 2074 6861 7420 7468 6520 7275 6e6e 696e   that the runnin
+000051f0: 6720 6576 656e 7420 6c6f 6f70 2062 650a  g event loop be.
+00005200: 7061 7373 6564 2069 6e20 6173 2074 6865  passed in as the
+00005210: 2060 6c6f 6f70 6020 6172 6775 6d65 6e74   `loop` argument
+00005220: 2074 6f20 6043 6f6e 6e65 6374 6f72 2829   to `Connector()
+00005230: 602e 0a0a 6060 6070 7974 686f 6e0a 696d  `...```python.im
+00005240: 706f 7274 2061 7379 6e63 696f 0a69 6d70  port asyncio.imp
+00005250: 6f72 7420 6173 796e 6370 670a 0a69 6d70  ort asyncpg..imp
+00005260: 6f72 7420 7371 6c61 6c63 6865 6d79 0a66  ort sqlalchemy.f
+00005270: 726f 6d20 7371 6c61 6c63 6865 6d79 2e65  rom sqlalchemy.e
+00005280: 7874 2e61 7379 6e63 696f 2069 6d70 6f72  xt.asyncio impor
+00005290: 7420 4173 796e 6345 6e67 696e 652c 2063  t AsyncEngine, c
+000052a0: 7265 6174 655f 6173 796e 635f 656e 6769  reate_async_engi
+000052b0: 6e65 0a0a 6672 6f6d 2067 6f6f 676c 652e  ne..from google.
+000052c0: 636c 6f75 642e 7371 6c2e 636f 6e6e 6563  cloud.sql.connec
+000052d0: 746f 7220 696d 706f 7274 2043 6f6e 6e65  tor import Conne
+000052e0: 6374 6f72 0a0a 6173 796e 6320 6465 6620  ctor..async def 
+000052f0: 696e 6974 5f63 6f6e 6e65 6374 696f 6e5f  init_connection_
+00005300: 706f 6f6c 2863 6f6e 6e65 6374 6f72 3a20  pool(connector: 
+00005310: 436f 6e6e 6563 746f 7229 202d 3e20 4173  Connector) -> As
+00005320: 796e 6345 6e67 696e 653a 0a20 2020 2023  yncEngine:.    #
+00005330: 2069 6e69 7469 616c 697a 6520 436f 6e6e   initialize Conn
+00005340: 6563 746f 7220 6f62 6a65 6374 2066 6f72  ector object for
+00005350: 2063 6f6e 6e65 6374 696f 6e73 2074 6f20   connections to 
+00005360: 436c 6f75 6420 5351 4c0a 2020 2020 6173  Cloud SQL.    as
+00005370: 796e 6320 6465 6620 6765 7463 6f6e 6e28  ync def getconn(
+00005380: 2920 2d3e 2061 7379 6e63 7067 2e43 6f6e  ) -> asyncpg.Con
+00005390: 6e65 6374 696f 6e3a 0a20 2020 2020 2020  nection:.       
+000053a0: 2020 2020 2063 6f6e 6e3a 2061 7379 6e63       conn: async
+000053b0: 7067 2e43 6f6e 6e65 6374 696f 6e20 3d20  pg.Connection = 
+000053c0: 6177 6169 7420 636f 6e6e 6563 746f 722e  await connector.
+000053d0: 636f 6e6e 6563 745f 6173 796e 6328 0a20  connect_async(. 
+000053e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000053f0: 7072 6f6a 6563 743a 7265 6769 6f6e 3a69  project:region:i
+00005400: 6e73 7461 6e63 6522 2c20 2023 2043 6c6f  nstance",  # Clo
+00005410: 7564 2053 514c 2069 6e73 7461 6e63 6520  ud SQL instance 
+00005420: 636f 6e6e 6563 7469 6f6e 206e 616d 650a  connection name.
+00005430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005440: 2261 7379 6e63 7067 222c 0a20 2020 2020  "asyncpg",.     
+00005450: 2020 2020 2020 2020 2020 2075 7365 723d             user=
+00005460: 226d 792d 7573 6572 222c 0a20 2020 2020  "my-user",.     
+00005470: 2020 2020 2020 2020 2020 2070 6173 7377             passw
+00005480: 6f72 643d 226d 792d 7061 7373 776f 7264  ord="my-password
+00005490: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000054a0: 2020 2064 623d 226d 792d 6462 2d6e 616d     db="my-db-nam
+000054b0: 6522 0a20 2020 2020 2020 2020 2020 2020  e".             
+000054c0: 2020 2023 202e 2e2e 2061 6464 6974 696f     # ... additio
+000054d0: 6e61 6c20 6461 7461 6261 7365 2064 7269  nal database dri
+000054e0: 7665 7220 6172 6773 0a20 2020 2020 2020  ver args.       
+000054f0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00005500: 2020 2072 6574 7572 6e20 636f 6e6e 0a0a     return conn..
+00005510: 2020 2020 2320 5468 6520 436c 6f75 6420      # The Cloud 
+00005520: 5351 4c20 5079 7468 6f6e 2043 6f6e 6e65  SQL Python Conne
+00005530: 6374 6f72 2063 616e 2062 6520 7573 6564  ctor can be used
+00005540: 2061 6c6f 6e67 2077 6974 6820 5351 4c41   along with SQLA
+00005550: 6c63 6865 6d79 2075 7369 6e67 2074 6865  lchemy using the
+00005560: 0a20 2020 2023 2027 6173 796e 635f 6372  .    # 'async_cr
+00005570: 6561 746f 7227 2061 7267 756d 656e 7420  eator' argument 
+00005580: 746f 2027 6372 6561 7465 5f61 7379 6e63  to 'create_async
+00005590: 5f65 6e67 696e 6527 0a20 2020 2070 6f6f  _engine'.    poo
+000055a0: 6c20 3d20 6372 6561 7465 5f61 7379 6e63  l = create_async
+000055b0: 5f65 6e67 696e 6528 0a20 2020 2020 2020  _engine(.       
+000055c0: 2022 706f 7374 6772 6573 716c 2b61 7379   "postgresql+asy
+000055d0: 6e63 7067 3a2f 2f22 2c0a 2020 2020 2020  ncpg://",.      
+000055e0: 2020 6173 796e 635f 6372 6561 746f 723d    async_creator=
+000055f0: 6765 7463 6f6e 6e2c 0a20 2020 2029 0a20  getconn,.    ). 
+00005600: 2020 2072 6574 7572 6e20 706f 6f6c 0a0a     return pool..
+00005610: 6173 796e 6320 6465 6620 6d61 696e 2829  async def main()
+00005620: 3a0a 2020 2020 2320 696e 6974 6961 6c69  :.    # initiali
+00005630: 7a65 2043 6f6e 6e65 6374 6f72 206f 626a  ze Connector obj
+00005640: 6563 7420 666f 7220 636f 6e6e 6563 7469  ect for connecti
+00005650: 6f6e 7320 746f 2043 6c6f 7564 2053 514c  ons to Cloud SQL
+00005660: 0a20 2020 206c 6f6f 7020 3d20 6173 796e  .    loop = asyn
+00005670: 6369 6f2e 6765 745f 7275 6e6e 696e 675f  cio.get_running_
+00005680: 6c6f 6f70 2829 0a20 2020 2061 7379 6e63  loop().    async
+00005690: 2077 6974 6820 436f 6e6e 6563 746f 7228   with Connector(
+000056a0: 6c6f 6f70 3d6c 6f6f 7029 2061 7320 636f  loop=loop) as co
+000056b0: 6e6e 6563 746f 723a 0a20 2020 2020 2020  nnector:.       
+000056c0: 2023 2069 6e69 7469 616c 697a 6520 636f   # initialize co
+000056d0: 6e6e 6563 7469 6f6e 2070 6f6f 6c0a 2020  nnection pool.  
+000056e0: 2020 2020 2020 706f 6f6c 203d 2061 7761        pool = awa
+000056f0: 6974 2069 6e69 745f 636f 6e6e 6563 7469  it init_connecti
+00005700: 6f6e 5f70 6f6f 6c28 636f 6e6e 6563 746f  on_pool(connecto
+00005710: 7229 0a0a 2020 2020 2020 2020 2320 6578  r)..        # ex
+00005720: 616d 706c 6520 7175 6572 790a 2020 2020  ample query.    
+00005730: 2020 2020 6173 796e 6320 7769 7468 2070      async with p
+00005740: 6f6f 6c2e 636f 6e6e 6563 7428 2920 6173  ool.connect() as
+00005750: 2063 6f6e 6e3a 0a20 2020 2020 2020 2020   conn:.         
+00005760: 2020 2061 7761 6974 2063 6f6e 6e2e 6578     await conn.ex
+00005770: 6563 7574 6528 7371 6c61 6c63 6865 6d79  ecute(sqlalchemy
+00005780: 2e74 6578 7428 2253 454c 4543 5420 4e4f  .text("SELECT NO
+00005790: 5728 2922 2929 0a0a 2020 2020 2020 2020  W()"))..        
+000057a0: 2320 6469 7370 6f73 6520 6f66 2063 6f6e  # dispose of con
+000057b0: 6e65 6374 696f 6e20 706f 6f6c 0a20 2020  nection pool.   
+000057c0: 2020 2020 2061 7761 6974 2070 6f6f 6c2e       await pool.
+000057d0: 6469 7370 6f73 6528 290a 6060 600a 0a23  dispose().```..#
+000057e0: 2320 5375 7070 6f72 7420 706f 6c69 6379  # Support policy
+000057f0: 0a0a 2323 2320 4d61 6a6f 7220 7665 7273  ..### Major vers
+00005800: 696f 6e20 6c69 6665 6379 636c 650a 0a54  ion lifecycle..T
+00005810: 6869 7320 7072 6f6a 6563 7420 7573 6573  his project uses
+00005820: 205b 7365 6d61 6e74 6963 2076 6572 7369   [semantic versi
+00005830: 6f6e 696e 675d 2868 7474 7073 3a2f 2f73  oning](https://s
+00005840: 656d 7665 722e 6f72 672f 292c 2061 6e64  emver.org/), and
+00005850: 2075 7365 7320 7468 650a 666f 6c6c 6f77   uses the.follow
+00005860: 696e 6720 6c69 6665 6379 636c 6520 7265  ing lifecycle re
+00005870: 6761 7264 696e 6720 7375 7070 6f72 7420  garding support 
+00005880: 666f 7220 6120 6d61 6a6f 7220 7665 7273  for a major vers
+00005890: 696f 6e3a 0a0a 2a2a 4163 7469 7665 2a2a  ion:..**Active**
+000058a0: 202d 2041 6374 6976 6520 7665 7273 696f   - Active versio
+000058b0: 6e73 2067 6574 2061 6c6c 206e 6577 2066  ns get all new f
+000058c0: 6561 7475 7265 7320 616e 6420 7365 6375  eatures and secu
+000058d0: 7269 7479 2066 6978 6573 2028 7468 6174  rity fixes (that
+000058e0: 0a77 6f75 6c64 6ee2 8099 7420 6f74 6865  .wouldn...t othe
+000058f0: 7277 6973 6520 696e 7472 6f64 7563 6520  rwise introduce 
+00005900: 6120 6272 6561 6b69 6e67 2063 6861 6e67  a breaking chang
+00005910: 6529 2e20 4e65 7720 6d61 6a6f 7220 7665  e). New major ve
+00005920: 7273 696f 6e73 2061 7265 0a67 7561 7261  rsions are.guara
+00005930: 6e74 6565 6420 746f 2062 6520 2261 6374  nteed to be "act
+00005940: 6976 6522 2066 6f72 2061 206d 696e 696d  ive" for a minim
+00005950: 756d 206f 6620 3120 7965 6172 2e0a 2a2a  um of 1 year..**
+00005960: 4465 7072 6563 6174 6564 2a2a 202d 2044  Deprecated** - D
+00005970: 6570 7265 6361 7465 6420 7665 7273 696f  eprecated versio
+00005980: 6e73 2063 6f6e 7469 6e75 6520 746f 2072  ns continue to r
+00005990: 6563 6569 7665 2073 6563 7572 6974 7920  eceive security 
+000059a0: 616e 6420 6372 6974 6963 616c 0a62 7567  and critical.bug
+000059b0: 2066 6978 6573 2c20 6275 7420 646f 206e   fixes, but do n
+000059c0: 6f74 2072 6563 6569 7665 206e 6577 2066  ot receive new f
+000059d0: 6561 7475 7265 732e 2044 6570 7265 6361  eatures. Depreca
+000059e0: 7465 6420 7665 7273 696f 6e73 2077 696c  ted versions wil
+000059f0: 6c20 6265 2070 7562 6c69 636c 790a 7375  l be publicly.su
+00005a00: 7070 6f72 7465 6420 666f 7220 3120 7965  pported for 1 ye
+00005a10: 6172 2e0a 2a2a 556e 7375 7070 6f72 7465  ar..**Unsupporte
+00005a20: 642a 2a20 2d20 416e 7920 6d61 6a6f 7220  d** - Any major 
+00005a30: 7665 7273 696f 6e20 7468 6174 2068 6173  version that has
+00005a40: 2062 6565 6e20 6465 7072 6563 6174 6564   been deprecated
+00005a50: 2066 6f72 203e 3d31 2079 6561 7220 6973   for >=1 year is
+00005a60: 0a63 6f6e 7369 6465 7265 6420 7075 626c  .considered publ
+00005a70: 6963 6c79 2075 6e73 7570 706f 7274 6564  icly unsupported
+00005a80: 2e0a 0a23 2320 5375 7070 6f72 7465 6420  ...## Supported 
+00005a90: 5079 7468 6f6e 2056 6572 7369 6f6e 730a  Python Versions.
+00005aa0: 0a57 6520 666f 6c6c 6f77 2074 6865 205b  .We follow the [
+00005ab0: 5079 7468 6f6e 2056 6572 7369 6f6e 2053  Python Version S
+00005ac0: 7570 706f 7274 2050 6f6c 6963 795d 5b70  upport Policy][p
+00005ad0: 7976 6572 5d20 7573 6564 2062 7920 476f  yver] used by Go
+00005ae0: 6f67 6c65 2043 6c6f 7564 0a4c 6962 7261  ogle Cloud.Libra
+00005af0: 7269 6573 2066 6f72 2050 7974 686f 6e2e  ries for Python.
+00005b00: 2043 6861 6e67 6573 2069 6e20 7375 7070   Changes in supp
+00005b10: 6f72 7465 6420 5079 7468 6f6e 2076 6572  orted Python ver
+00005b20: 7369 6f6e 7320 7769 6c6c 2062 650a 636f  sions will be.co
+00005b30: 6e73 6964 6572 6564 2061 206d 696e 6f72  nsidered a minor
+00005b40: 2063 6861 6e67 652c 2061 6e64 2077 696c   change, and wil
+00005b50: 6c20 6265 206c 6973 7465 6420 696e 2074  l be listed in t
+00005b60: 6865 2072 656c 6561 7365 206e 6f74 6573  he release notes
+00005b70: 2e0a 0a5b 7079 7665 725d 3a20 6874 7470  ...[pyver]: http
+00005b80: 733a 2f2f 636c 6f75 642e 676f 6f67 6c65  s://cloud.google
+00005b90: 2e63 6f6d 2f70 7974 686f 6e2f 646f 6373  .com/python/docs
+00005ba0: 2f73 7570 706f 7274 6564 2d70 7974 686f  /supported-pytho
+00005bb0: 6e2d 7665 7273 696f 6e73 0a0a 2323 2320  n-versions..### 
+00005bc0: 5265 6c65 6173 6520 6361 6465 6e63 650a  Release cadence.
+00005bd0: 5468 6973 2070 726f 6a65 6374 2061 696d  This project aim
+00005be0: 7320 666f 7220 6120 6d69 6e69 6d75 6d20  s for a minimum 
+00005bf0: 6d6f 6e74 686c 7920 7265 6c65 6173 6520  monthly release 
+00005c00: 6361 6465 6e63 652e 2049 6620 6e6f 206e  cadence. If no n
+00005c10: 6577 0a66 6561 7475 7265 7320 6f72 2066  ew.features or f
+00005c20: 6978 6573 2068 6176 6520 6265 656e 2061  ixes have been a
+00005c30: 6464 6564 2c20 6120 6e65 7720 5041 5443  dded, a new PATC
+00005c40: 4820 7665 7273 696f 6e20 7769 7468 2074  H version with t
+00005c50: 6865 206c 6174 6573 740a 6465 7065 6e64  he latest.depend
+00005c60: 656e 6369 6573 2069 7320 7265 6c65 6173  encies is releas
+00005c70: 6564 2e0a 0a23 2323 2043 6f6e 7472 6962  ed...### Contrib
+00005c80: 7574 696e 670a 0a57 6520 7765 6c63 6f6d  uting..We welcom
+00005c90: 6520 6f75 7473 6964 6520 636f 6e74 7269  e outside contri
+00005ca0: 6275 7469 6f6e 732e 2050 6c65 6173 6520  butions. Please 
+00005cb0: 7365 6520 6f75 720a 5b43 6f6e 7472 6962  see our.[Contrib
+00005cc0: 7574 696e 6720 4775 6964 655d 2843 4f4e  uting Guide](CON
+00005cd0: 5452 4942 5554 494e 472e 6d64 2920 666f  TRIBUTING.md) fo
+00005ce0: 7220 6465 7461 696c 7320 6f6e 2068 6f77  r details on how
+00005cf0: 2062 6573 7420 746f 2063 6f6e 7472 6962   best to contrib
+00005d00: 7574 652e 0a                             ute..
```

### Comparing `cloud-sql-python-connector-1.2.4/README.md` & `cloud-sql-python-connector-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -90,1244 +90,1331 @@
 00000590: 2043 6f6e 6e65 6374 6f72 5f20 6973 2061   Connector_ is a
 000005a0: 2043 6c6f 7564 2053 514c 2063 6f6e 6e65   Cloud SQL conne
 000005b0: 6374 6f72 2064 6573 6967 6e65 6420 666f  ctor designed fo
 000005c0: 7220 7573 6520 7769 7468 2074 6865 0a50  r use with the.P
 000005d0: 7974 686f 6e20 6c61 6e67 7561 6765 2e20  ython language. 
 000005e0: 5573 696e 6720 6120 436c 6f75 6420 5351  Using a Cloud SQ
 000005f0: 4c20 636f 6e6e 6563 746f 7220 7072 6f76  L connector prov
-00000600: 6964 6573 2074 6865 2066 6f6c 6c6f 7769  ides the followi
-00000610: 6e67 2062 656e 6566 6974 733a 0a2a 202a  ng benefits:.* *
-00000620: 2a49 414d 2041 7574 686f 7269 7a61 7469  *IAM Authorizati
-00000630: 6f6e 3a2a 2a20 7573 6573 2049 414d 2070  on:** uses IAM p
-00000640: 6572 6d69 7373 696f 6e73 2074 6f20 636f  ermissions to co
-00000650: 6e74 726f 6c20 7768 6f2f 7768 6174 2063  ntrol who/what c
-00000660: 616e 2063 6f6e 6e65 6374 2074 6f0a 2020  an connect to.  
-00000670: 796f 7572 2043 6c6f 7564 2053 514c 2069  your Cloud SQL i
-00000680: 6e73 7461 6e63 6573 0a2a 202a 2a49 6d70  nstances.* **Imp
-00000690: 726f 7665 6420 5365 6375 7269 7479 3a2a  roved Security:*
-000006a0: 2a20 7573 6573 2072 6f62 7573 742c 2075  * uses robust, u
-000006b0: 7064 6174 6564 2054 4c53 2031 2e33 2065  pdated TLS 1.3 e
-000006c0: 6e63 7279 7074 696f 6e20 616e 640a 2020  ncryption and.  
-000006d0: 6964 656e 7469 7479 2076 6572 6966 6963  identity verific
-000006e0: 6174 696f 6e20 6265 7477 6565 6e20 7468  ation between th
-000006f0: 6520 636c 6965 6e74 2063 6f6e 6e65 6374  e client connect
-00000700: 6f72 2061 6e64 2074 6865 2073 6572 7665  or and the serve
-00000710: 722d 7369 6465 2070 726f 7879 2c0a 2020  r-side proxy,.  
-00000720: 696e 6465 7065 6e64 656e 7420 6f66 2074  independent of t
-00000730: 6865 2064 6174 6162 6173 6520 7072 6f74  he database prot
-00000740: 6f63 6f6c 2e0a 2a20 2a2a 436f 6e76 656e  ocol..* **Conven
-00000750: 6965 6e63 653a 2a2a 2072 656d 6f76 6573  ience:** removes
-00000760: 2074 6865 2072 6571 7569 7265 6d65 6e74   the requirement
-00000770: 2074 6f20 7573 6520 616e 6420 6469 7374   to use and dist
-00000780: 7269 6275 7465 2053 534c 0a20 2063 6572  ribute SSL.  cer
-00000790: 7469 6669 6361 7465 732c 2061 7320 7765  tificates, as we
-000007a0: 6c6c 2061 7320 6d61 6e61 6765 2066 6972  ll as manage fir
-000007b0: 6577 616c 6c73 206f 7220 736f 7572 6365  ewalls or source
-000007c0: 2f64 6573 7469 6e61 7469 6f6e 2049 5020  /destination IP 
-000007d0: 6164 6472 6573 7365 732e 0a2a 2028 6f70  addresses..* (op
-000007e0: 7469 6f6e 616c 6c79 2920 2a2a 4941 4d20  tionally) **IAM 
-000007f0: 4442 2041 7574 6865 6e74 6963 6174 696f  DB Authenticatio
-00000800: 6e3a 2a2a 2070 726f 7669 6465 7320 7375  n:** provides su
-00000810: 7070 6f72 7420 666f 720a 2020 5b43 6c6f  pport for.  [Clo
-00000820: 7564 2053 514c e280 9973 2061 7574 6f6d  ud SQL...s autom
-00000830: 6174 6963 2049 414d 2044 4220 4175 7468  atic IAM DB Auth
-00000840: 4e5d 5b69 616d 2d64 622d 6175 7468 6e5d  N][iam-db-authn]
-00000850: 2066 6561 7475 7265 2e0a 0a5b 6961 6d2d   feature...[iam-
-00000860: 6462 2d61 7574 686e 5d3a 2068 7474 7073  db-authn]: https
-00000870: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
-00000880: 636f 6d2f 7371 6c2f 646f 6373 2f70 6f73  com/sql/docs/pos
-00000890: 7467 7265 732f 6175 7468 656e 7469 6361  tgres/authentica
-000008a0: 7469 6f6e 0a0a 5468 6520 436c 6f75 6420  tion..The Cloud 
-000008b0: 5351 4c20 5079 7468 6f6e 2043 6f6e 6e65  SQL Python Conne
-000008c0: 6374 6f72 2069 7320 6120 7061 636b 6167  ctor is a packag
-000008d0: 6520 746f 2062 6520 7573 6564 2061 6c6f  e to be used alo
-000008e0: 6e67 7369 6465 2061 2064 6174 6162 6173  ngside a databas
-000008f0: 6520 6472 6976 6572 2e0a 4375 7272 656e  e driver..Curren
-00000900: 746c 7920 7375 7070 6f72 7465 6420 6472  tly supported dr
-00000910: 6976 6572 7320 6172 653a 0a20 2d20 5b60  ivers are:. - [`
-00000920: 7079 6d79 7371 6c60 5d28 6874 7470 733a  pymysql`](https:
-00000930: 2f2f 6769 7468 7562 2e63 6f6d 2f50 794d  //github.com/PyM
-00000940: 7953 514c 2f50 794d 7953 514c 2920 284d  ySQL/PyMySQL) (M
-00000950: 7953 514c 290a 202d 205b 6070 6738 3030  ySQL). - [`pg800
-00000960: 3060 5d28 6874 7470 733a 2f2f 6769 7468  0`](https://gith
-00000970: 7562 2e63 6f6d 2f74 6c6f 636b 652f 7067  ub.com/tlocke/pg
-00000980: 3830 3030 2920 2850 6f73 7467 7265 5351  8000) (PostgreSQ
-00000990: 4c29 0a20 2d20 5b60 6173 796e 6370 6760  L). - [`asyncpg`
-000009a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000009b0: 2e63 6f6d 2f4d 6167 6963 5374 6163 6b2f  .com/MagicStack/
-000009c0: 6173 796e 6370 6729 2028 506f 7374 6772  asyncpg) (Postgr
-000009d0: 6553 514c 290a 202d 205b 6070 7974 6473  eSQL). - [`pytds
-000009e0: 605d 2868 7474 7073 3a2f 2f67 6974 6875  `](https://githu
-000009f0: 622e 636f 6d2f 6465 6e69 7365 6e6b 6f6d  b.com/denisenkom
-00000a00: 2f70 7974 6473 2920 2853 514c 2053 6572  /pytds) (SQL Ser
-00000a10: 7665 7229 0a0a 0a23 2320 496e 7374 616c  ver)...## Instal
-00000a20: 6c61 7469 6f6e 0a0a 596f 7520 6361 6e20  lation..You can 
-00000a30: 696e 7374 616c 6c20 7468 6973 206c 6962  install this lib
-00000a40: 7261 7279 2077 6974 6820 6070 6970 2069  rary with `pip i
-00000a50: 6e73 7461 6c6c 602c 2073 7065 6369 6679  nstall`, specify
-00000a60: 696e 6720 7468 6520 6472 6976 6572 0a62  ing the driver.b
-00000a70: 6173 6564 206f 6e20 796f 7572 2064 6174  ased on your dat
-00000a80: 6162 6173 6520 6469 616c 6563 742e 0a0a  abase dialect...
-00000a90: 2323 2320 4d79 5351 4c0a 6060 600a 7069  ### MySQL.```.pi
-00000aa0: 7020 696e 7374 616c 6c20 2263 6c6f 7564  p install "cloud
-00000ab0: 2d73 716c 2d70 7974 686f 6e2d 636f 6e6e  -sql-python-conn
-00000ac0: 6563 746f 725b 7079 6d79 7371 6c5d 220a  ector[pymysql]".
-00000ad0: 6060 600a 2323 2320 506f 7374 6772 6573  ```.### Postgres
-00000ae0: 0a54 6865 7265 2061 7265 2074 776f 2064  .There are two d
-00000af0: 6966 6665 7265 6e74 2064 6174 6162 6173  ifferent databas
-00000b00: 6520 6472 6976 6572 7320 7468 6174 2061  e drivers that a
-00000b10: 7265 2073 7570 706f 7274 6564 2066 6f72  re supported for
-00000b20: 2074 6865 2050 6f73 7467 7265 7320 6469   the Postgres di
-00000b30: 616c 6563 743a 0a0a 2323 2323 2070 6738  alect:..#### pg8
-00000b40: 3030 300a 6060 600a 7069 7020 696e 7374  000.```.pip inst
-00000b50: 616c 6c20 2263 6c6f 7564 2d73 716c 2d70  all "cloud-sql-p
-00000b60: 7974 686f 6e2d 636f 6e6e 6563 746f 725b  ython-connector[
-00000b70: 7067 3830 3030 5d22 0a60 6060 0a23 2323  pg8000]".```.###
-00000b80: 2320 6173 796e 6370 670a 6060 600a 7069  # asyncpg.```.pi
-00000b90: 7020 696e 7374 616c 6c20 2263 6c6f 7564  p install "cloud
-00000ba0: 2d73 716c 2d70 7974 686f 6e2d 636f 6e6e  -sql-python-conn
-00000bb0: 6563 746f 725b 6173 796e 6370 675d 220a  ector[asyncpg]".
-00000bc0: 6060 600a 2323 2320 5351 4c20 5365 7276  ```.### SQL Serv
-00000bd0: 6572 0a60 6060 0a70 6970 2069 6e73 7461  er.```.pip insta
-00000be0: 6c6c 2022 636c 6f75 642d 7371 6c2d 7079  ll "cloud-sql-py
-00000bf0: 7468 6f6e 2d63 6f6e 6e65 6374 6f72 5b70  thon-connector[p
-00000c00: 7974 6473 5d22 0a60 6060 0a23 2320 5573  ytds]".```.## Us
-00000c10: 6167 650a 0a54 6869 7320 7061 636b 6167  age..This packag
-00000c20: 6520 7072 6f76 6964 6573 2073 6576 6572  e provides sever
-00000c30: 616c 2066 756e 6374 696f 6e73 2066 6f72  al functions for
-00000c40: 2061 7574 686f 7269 7a69 6e67 2061 6e64   authorizing and
-00000c50: 2065 6e63 7279 7074 696e 670a 636f 6e6e   encrypting.conn
-00000c60: 6563 7469 6f6e 732e 2054 6865 7365 2066  ections. These f
-00000c70: 756e 6374 696f 6e73 2061 7265 2075 7365  unctions are use
-00000c80: 6420 7769 7468 2079 6f75 7220 6461 7461  d with your data
-00000c90: 6261 7365 2064 7269 7665 7220 746f 2063  base driver to c
-00000ca0: 6f6e 6e65 6374 2074 6f0a 796f 7572 2043  onnect to.your C
-00000cb0: 6c6f 7564 2053 514c 2069 6e73 7461 6e63  loud SQL instanc
-00000cc0: 652e 0a0a 5468 6520 696e 7374 616e 6365  e...The instance
-00000cd0: 2063 6f6e 6e65 6374 696f 6e20 6e61 6d65   connection name
-00000ce0: 2066 6f72 2079 6f75 7220 436c 6f75 6420   for your Cloud 
-00000cf0: 5351 4c20 696e 7374 616e 6365 2069 7320  SQL instance is 
-00000d00: 616c 7761 7973 2069 6e20 7468 650a 666f  always in the.fo
-00000d10: 726d 6174 2022 7072 6f6a 6563 743a 7265  rmat "project:re
-00000d20: 6769 6f6e 3a69 6e73 7461 6e63 6522 2e0a  gion:instance"..
-00000d30: 0a23 2323 2041 5049 7320 616e 6420 5365  .### APIs and Se
-00000d40: 7276 6963 6573 0a0a 5468 6973 2070 6163  rvices..This pac
-00000d50: 6b61 6765 2072 6571 7569 7265 7320 7468  kage requires th
-00000d60: 6520 666f 6c6c 6f77 696e 6720 746f 2073  e following to s
-00000d70: 7563 6365 7373 6675 6c6c 7920 6d61 6b65  uccessfully make
-00000d80: 2043 6c6f 7564 2053 514c 2043 6f6e 6e65   Cloud SQL Conne
-00000d90: 6374 696f 6e73 3a0a 0a2d 2049 414d 2070  ctions:..- IAM p
-00000da0: 7269 6e63 6970 616c 2028 7573 6572 2c20  rincipal (user, 
-00000db0: 7365 7276 6963 6520 6163 636f 756e 742c  service account,
-00000dc0: 2065 7463 2e29 2077 6974 6820 7468 650a   etc.) with the.
-00000dd0: 5b43 6c6f 7564 2053 514c 2043 6c69 656e  [Cloud SQL Clien
-00000de0: 745d 5b63 6c69 656e 742d 726f 6c65 5d20  t][client-role] 
-00000df0: 726f 6c65 2e20 5468 6973 2049 414d 2070  role. This IAM p
-00000e00: 7269 6e63 6970 616c 2077 696c 6c20 6265  rincipal will be
-00000e10: 2075 7365 6420 666f 720a 5b63 7265 6465   used for.[crede
-00000e20: 6e74 6961 6c73 5d28 2363 7265 6465 6e74  ntials](#credent
-00000e30: 6961 6c73 292e 0a2d 2054 6865 205b 436c  ials)..- The [Cl
-00000e40: 6f75 6420 5351 4c20 4164 6d69 6e20 4150  oud SQL Admin AP
-00000e50: 495d 5b61 646d 696e 2d61 7069 5d20 746f  I][admin-api] to
-00000e60: 2062 6520 656e 6162 6c65 6420 7769 7468   be enabled with
-00000e70: 696e 2079 6f75 7220 476f 6f67 6c65 2043  in your Google C
-00000e80: 6c6f 7564 0a50 726f 6a65 6374 2e20 4279  loud.Project. By
-00000e90: 2064 6566 6175 6c74 2c20 7468 6520 4150   default, the AP
-00000ea0: 4920 7769 6c6c 2062 6520 6361 6c6c 6564  I will be called
-00000eb0: 2069 6e20 7468 6520 7072 6f6a 6563 7420   in the project 
-00000ec0: 6173 736f 6369 6174 6564 2077 6974 680a  associated with.
-00000ed0: 7468 6520 4941 4d20 7072 696e 6369 7061  the IAM principa
-00000ee0: 6c2e 0a0a 5b61 646d 696e 2d61 7069 5d3a  l...[admin-api]:
-00000ef0: 2068 7474 7073 3a2f 2f63 6f6e 736f 6c65   https://console
-00000f00: 2e63 6c6f 7564 2e67 6f6f 676c 652e 636f  .cloud.google.co
-00000f10: 6d2f 6170 6973 2f61 7069 2f73 716c 6164  m/apis/api/sqlad
-00000f20: 6d69 6e2e 676f 6f67 6c65 6170 6973 2e63  min.googleapis.c
-00000f30: 6f6d 0a5b 636c 6965 6e74 2d72 6f6c 655d  om.[client-role]
-00000f40: 3a20 6874 7470 733a 2f2f 636c 6f75 642e  : https://cloud.
-00000f50: 676f 6f67 6c65 2e63 6f6d 2f73 716c 2f64  google.com/sql/d
-00000f60: 6f63 732f 6d79 7371 6c2f 726f 6c65 732d  ocs/mysql/roles-
-00000f70: 616e 642d 7065 726d 6973 7369 6f6e 730a  and-permissions.
-00000f80: 0a23 2323 2043 7265 6465 6e74 6961 6c73  .### Credentials
-00000f90: 0a0a 5468 6973 206c 6962 7261 7279 2075  ..This library u
-00000fa0: 7365 7320 7468 6520 5b41 7070 6c69 6361  ses the [Applica
-00000fb0: 7469 6f6e 2044 6566 6175 6c74 2043 7265  tion Default Cre
-00000fc0: 6465 6e74 6961 6c73 2028 4144 4329 5d5b  dentials (ADC)][
-00000fd0: 6164 635d 2073 7472 6174 6567 7920 666f  adc] strategy fo
-00000fe0: 720a 7265 736f 6c76 696e 6720 6372 6564  r.resolving cred
-00000ff0: 656e 7469 616c 732e 2050 6c65 6173 6520  entials. Please 
-00001000: 7365 6520 5b74 6865 7365 2069 6e73 7472  see [these instr
-00001010: 7563 7469 6f6e 7320 666f 7220 686f 7720  uctions for how 
-00001020: 746f 2073 6574 2079 6f75 7220 4144 435d  to set your ADC]
-00001030: 5b73 6574 2d61 6463 5d0a 2847 6f6f 676c  [set-adc].(Googl
-00001040: 6520 436c 6f75 6420 4170 706c 6963 6174  e Cloud Applicat
-00001050: 696f 6e20 7673 204c 6f63 616c 2044 6576  ion vs Local Dev
-00001060: 656c 6f70 6d65 6e74 2c20 4941 4d20 7573  elopment, IAM us
-00001070: 6572 2076 7320 7365 7276 6963 6520 6163  er vs service ac
-00001080: 636f 756e 7420 6372 6564 656e 7469 616c  count credential
-00001090: 7329 2c0a 6f72 2063 6f6e 7375 6c74 2074  s),.or consult t
-000010a0: 6865 205b 676f 6f67 6c65 2e61 7574 685d  he [google.auth]
-000010b0: 5b67 6f6f 676c 652d 6175 7468 5d20 7061  [google-auth] pa
-000010c0: 636b 6167 652e 0a0a 546f 2065 7870 6c69  ckage...To expli
-000010d0: 6369 746c 7920 7365 7420 6120 7370 6563  citly set a spec
-000010e0: 6966 6963 2073 6f75 7263 6520 666f 7220  ific source for 
-000010f0: 7468 6520 6372 6564 656e 7469 616c 732c  the credentials,
-00001100: 2073 6565 0a5b 436f 6e66 6967 7572 696e   see.[Configurin
-00001110: 6720 7468 6520 436f 6e6e 6563 746f 725d  g the Connector]
-00001120: 2823 636f 6e66 6967 7572 696e 672d 7468  (#configuring-th
-00001130: 652d 636f 6e6e 6563 746f 7229 2062 656c  e-connector) bel
-00001140: 6f77 2e0a 0a5b 6164 635d 3a20 6874 7470  ow...[adc]: http
-00001150: 733a 2f2f 636c 6f75 642e 676f 6f67 6c65  s://cloud.google
-00001160: 2e63 6f6d 2f64 6f63 732f 6175 7468 656e  .com/docs/authen
-00001170: 7469 6361 7469 6f6e 2361 6463 0a5b 7365  tication#adc.[se
-00001180: 742d 6164 635d 3a20 6874 7470 733a 2f2f  t-adc]: https://
-00001190: 636c 6f75 642e 676f 6f67 6c65 2e63 6f6d  cloud.google.com
-000011a0: 2f64 6f63 732f 6175 7468 656e 7469 6361  /docs/authentica
-000011b0: 7469 6f6e 2f70 726f 7669 6465 2d63 7265  tion/provide-cre
-000011c0: 6465 6e74 6961 6c73 2d61 6463 0a5b 676f  dentials-adc.[go
-000011d0: 6f67 6c65 2d61 7574 685d 3a20 6874 7470  ogle-auth]: http
-000011e0: 733a 2f2f 676f 6f67 6c65 2d61 7574 682e  s://google-auth.
-000011f0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00001200: 6e2f 6d61 7374 6572 2f72 6566 6572 656e  n/master/referen
-00001210: 6365 2f67 6f6f 676c 652e 6175 7468 2e68  ce/google.auth.h
-00001220: 746d 6c0a 0a23 2323 2048 6f77 2074 6f20  tml..### How to 
-00001230: 7573 6520 7468 6973 2043 6f6e 6e65 6374  use this Connect
-00001240: 6f72 0a0a 546f 2063 6f6e 6e65 6374 2074  or..To connect t
-00001250: 6f20 436c 6f75 6420 5351 4c20 7573 696e  o Cloud SQL usin
-00001260: 6720 7468 6520 636f 6e6e 6563 746f 722c  g the connector,
-00001270: 2069 6e69 7469 7461 6c69 7a65 2061 2060   inititalize a `
-00001280: 436f 6e6e 6563 746f 7260 0a6f 626a 6563  Connector`.objec
-00001290: 7420 616e 6420 6361 6c6c 2069 7427 7320  t and call it's 
-000012a0: 6063 6f6e 6e65 6374 6020 6d65 7468 6f64  `connect` method
-000012b0: 2077 6974 6820 7468 6520 7072 6f70 6572   with the proper
-000012c0: 2069 6e70 7574 2070 6172 616d 6574 6572   input parameter
-000012d0: 732e 0a0a 5468 6520 6043 6f6e 6e65 6374  s...The `Connect
-000012e0: 6f72 6020 6974 7365 6c66 2063 7265 6174  or` itself creat
-000012f0: 6573 2063 6f6e 6e65 6374 696f 6e20 6f62  es connection ob
-00001300: 6a65 6374 7320 6279 2063 616c 6c69 6e67  jects by calling
-00001310: 2069 7473 2060 636f 6e6e 6563 7460 206d   its `connect` m
-00001320: 6574 686f 6420 6275 7420 646f 6573 206e  ethod but does n
-00001330: 6f74 206d 616e 6167 6520 6461 7461 6261  ot manage databa
-00001340: 7365 2063 6f6e 6e65 6374 696f 6e20 706f  se connection po
-00001350: 6f6c 696e 672e 2046 6f72 2074 6869 7320  oling. For this 
-00001360: 7265 6173 6f6e 2c20 6974 2069 7320 7265  reason, it is re
-00001370: 636f 6d6d 656e 6465 6420 746f 2075 7365  commended to use
-00001380: 2074 6865 2063 6f6e 6e65 6374 6f72 2061   the connector a
-00001390: 6c6f 6e67 7369 6465 2061 206c 6962 7261  longside a libra
-000013a0: 7279 2074 6861 7420 6361 6e20 6372 6561  ry that can crea
-000013b0: 7465 2063 6f6e 6e65 6374 696f 6e20 706f  te connection po
-000013c0: 6f6c 732c 2073 7563 6820 6173 205b 5351  ols, such as [SQ
-000013d0: 4c41 6c63 6865 6d79 5d28 6874 7470 733a  LAlchemy](https:
-000013e0: 2f2f 7777 772e 7371 6c61 6c63 6865 6d79  //www.sqlalchemy
-000013f0: 2e6f 7267 2f29 2e20 5468 6973 2077 696c  .org/). This wil
-00001400: 6c20 616c 6c6f 7720 666f 7220 636f 6e6e  l allow for conn
-00001410: 6563 7469 6f6e 7320 746f 2072 656d 6169  ections to remai
-00001420: 6e20 6f70 656e 2061 6e64 2062 6520 7265  n open and be re
-00001430: 7573 6564 2c20 7265 6475 6369 6e67 2063  used, reducing c
-00001440: 6f6e 6e65 6374 696f 6e20 6f76 6572 6865  onnection overhe
-00001450: 6164 2061 6e64 2074 6865 206e 756d 6265  ad and the numbe
-00001460: 7220 6f66 2063 6f6e 6e65 6374 696f 6e73  r of connections
-00001470: 206e 6565 6465 642e 0a0a 496e 2074 6865   needed...In the
-00001480: 2043 6f6e 6e65 6374 6f72 2773 2060 636f   Connector's `co
-00001490: 6e6e 6563 7460 206d 6574 686f 6420 6265  nnect` method be
-000014a0: 6c6f 772c 2069 6e70 7574 2079 6f75 7220  low, input your 
-000014b0: 636f 6e6e 6563 7469 6f6e 2073 7472 696e  connection strin
-000014c0: 6720 6173 2074 6865 2066 6972 7374 2070  g as the first p
-000014d0: 6f73 6974 696f 6e61 6c20 6172 6775 6d65  ositional argume
-000014e0: 6e74 2061 6e64 2074 6865 206e 616d 6520  nt and the name 
-000014f0: 6f66 2074 6865 2064 6174 6162 6173 6520  of the database 
-00001500: 6472 6976 6572 2066 6f72 2074 6865 2073  driver for the s
-00001510: 6563 6f6e 6420 706f 7369 7469 6f6e 616c  econd positional
-00001520: 2061 7267 756d 656e 742e 2049 6e73 6572   argument. Inser
-00001530: 7420 7468 6520 7265 7374 206f 6620 796f  t the rest of yo
-00001540: 7572 2063 6f6e 6e65 6374 696f 6e20 6b65  ur connection ke
-00001550: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
-00001560: 6c69 6b65 2075 7365 722c 2070 6173 7377  like user, passw
-00001570: 6f72 6420 616e 6420 6461 7461 6261 7365  ord and database
-00001580: 2e20 596f 7520 6361 6e20 616c 736f 2073  . You can also s
-00001590: 6574 2074 6865 206f 7074 696f 6e61 6c20  et the optional 
-000015a0: 6074 696d 656f 7574 6020 6f72 2060 6970  `timeout` or `ip
-000015b0: 5f74 7970 6560 206b 6579 776f 7264 2061  _type` keyword a
-000015c0: 7267 756d 656e 7473 2e0a 0a54 6f20 7573  rguments...To us
-000015d0: 6520 7468 6973 2063 6f6e 6e65 6374 6f72  e this connector
-000015e0: 2077 6974 6820 5351 4c41 6c63 6865 6d79   with SQLAlchemy
-000015f0: 2c20 7573 6520 7468 6520 6063 7265 6174  , use the `creat
-00001600: 6f72 6020 6172 6775 6d65 6e74 2066 6f72  or` argument for
-00001610: 2060 7371 6c61 6c63 6865 6d79 2e63 7265   `sqlalchemy.cre
-00001620: 6174 655f 656e 6769 6e65 603a 0a0a 6060  ate_engine`:..``
-00001630: 6070 7974 686f 6e0a 6672 6f6d 2067 6f6f  `python.from goo
-00001640: 676c 652e 636c 6f75 642e 7371 6c2e 636f  gle.cloud.sql.co
-00001650: 6e6e 6563 746f 7220 696d 706f 7274 2043  nnector import C
-00001660: 6f6e 6e65 6374 6f72 0a69 6d70 6f72 7420  onnector.import 
-00001670: 7371 6c61 6c63 6865 6d79 0a0a 2320 696e  sqlalchemy..# in
-00001680: 6974 6961 6c69 7a65 2043 6f6e 6e65 6374  itialize Connect
-00001690: 6f72 206f 626a 6563 740a 636f 6e6e 6563  or object.connec
-000016a0: 746f 7220 3d20 436f 6e6e 6563 746f 7228  tor = Connector(
-000016b0: 290a 0a23 2066 756e 6374 696f 6e20 746f  )..# function to
-000016c0: 2072 6574 7572 6e20 7468 6520 6461 7461   return the data
-000016d0: 6261 7365 2063 6f6e 6e65 6374 696f 6e0a  base connection.
-000016e0: 6465 6620 6765 7463 6f6e 6e28 2920 2d3e  def getconn() ->
-000016f0: 2070 796d 7973 716c 2e63 6f6e 6e65 6374   pymysql.connect
-00001700: 696f 6e73 2e43 6f6e 6e65 6374 696f 6e3a  ions.Connection:
-00001710: 0a20 2020 2063 6f6e 6e3a 2070 796d 7973  .    conn: pymys
-00001720: 716c 2e63 6f6e 6e65 6374 696f 6e73 2e43  ql.connections.C
-00001730: 6f6e 6e65 6374 696f 6e20 3d20 636f 6e6e  onnection = conn
-00001740: 6563 746f 722e 636f 6e6e 6563 7428 0a20  ector.connect(. 
-00001750: 2020 2020 2020 2022 7072 6f6a 6563 743a         "project:
-00001760: 7265 6769 6f6e 3a69 6e73 7461 6e63 6522  region:instance"
-00001770: 2c0a 2020 2020 2020 2020 2270 796d 7973  ,.        "pymys
-00001780: 716c 222c 0a20 2020 2020 2020 2075 7365  ql",.        use
-00001790: 723d 226d 792d 7573 6572 222c 0a20 2020  r="my-user",.   
-000017a0: 2020 2020 2070 6173 7377 6f72 643d 226d       password="m
-000017b0: 792d 7061 7373 776f 7264 222c 0a20 2020  y-password",.   
-000017c0: 2020 2020 2064 623d 226d 792d 6462 2d6e       db="my-db-n
-000017d0: 616d 6522 0a20 2020 2029 0a20 2020 2072  ame".    ).    r
-000017e0: 6574 7572 6e20 636f 6e6e 0a0a 2320 6372  eturn conn..# cr
-000017f0: 6561 7465 2063 6f6e 6e65 6374 696f 6e20  eate connection 
-00001800: 706f 6f6c 0a70 6f6f 6c20 3d20 7371 6c61  pool.pool = sqla
-00001810: 6c63 6865 6d79 2e63 7265 6174 655f 656e  lchemy.create_en
-00001820: 6769 6e65 280a 2020 2020 226d 7973 716c  gine(.    "mysql
-00001830: 2b70 796d 7973 716c 3a2f 2f22 2c0a 2020  +pymysql://",.  
-00001840: 2020 6372 6561 746f 723d 6765 7463 6f6e    creator=getcon
-00001850: 6e2c 0a29 0a60 6060 0a0a 5468 6520 7265  n,.).```..The re
-00001860: 7475 726e 6564 2063 6f6e 6e65 6374 696f  turned connectio
-00001870: 6e20 706f 6f6c 2065 6e67 696e 6520 6361  n pool engine ca
-00001880: 6e20 7468 656e 2062 6520 7573 6564 2074  n then be used t
-00001890: 6f20 7175 6572 7920 616e 6420 6d6f 6469  o query and modi
-000018a0: 6679 2074 6865 2064 6174 6162 6173 652e  fy the database.
-000018b0: 0a0a 6060 6070 7974 686f 6e0a 2320 696e  ..```python.# in
-000018c0: 7365 7274 2073 7461 7465 6d65 6e74 0a69  sert statement.i
-000018d0: 6e73 6572 745f 7374 6d74 203d 2073 716c  nsert_stmt = sql
-000018e0: 616c 6368 656d 792e 7465 7874 280a 2020  alchemy.text(.  
-000018f0: 2020 2249 4e53 4552 5420 494e 544f 206d    "INSERT INTO m
-00001900: 795f 7461 626c 6520 2869 642c 2074 6974  y_table (id, tit
-00001910: 6c65 2920 5641 4c55 4553 2028 3a69 642c  le) VALUES (:id,
-00001920: 203a 7469 746c 6529 222c 0a29 0a0a 7769   :title)",.)..wi
-00001930: 7468 2070 6f6f 6c2e 636f 6e6e 6563 7428  th pool.connect(
-00001940: 2920 6173 2064 625f 636f 6e6e 3a0a 2020  ) as db_conn:.  
-00001950: 2020 2320 696e 7365 7274 2069 6e74 6f20    # insert into 
-00001960: 6461 7461 6261 7365 0a20 2020 2064 625f  database.    db_
-00001970: 636f 6e6e 2e65 7865 6375 7465 2869 6e73  conn.execute(ins
-00001980: 6572 745f 7374 6d74 2c20 7061 7261 6d65  ert_stmt, parame
-00001990: 7465 7273 3d7b 2269 6422 3a20 2262 6f6f  ters={"id": "boo
-000019a0: 6b31 222c 2022 7469 746c 6522 3a20 2242  k1", "title": "B
-000019b0: 6f6f 6b20 4f6e 6522 7d29 0a0a 2020 2020  ook One"})..    
-000019c0: 2320 7175 6572 7920 6461 7461 6261 7365  # query database
-000019d0: 0a20 2020 2072 6573 756c 7420 3d20 6462  .    result = db
-000019e0: 5f63 6f6e 6e2e 6578 6563 7574 6528 7371  _conn.execute(sq
-000019f0: 6c61 6c63 6865 6d79 2e74 6578 7428 2253  lalchemy.text("S
-00001a00: 454c 4543 5420 2a20 6672 6f6d 206d 795f  ELECT * from my_
-00001a10: 7461 626c 6522 2929 2e66 6574 6368 616c  table")).fetchal
-00001a20: 6c28 290a 0a20 2020 2023 2063 6f6d 6d69  l()..    # commi
-00001a30: 7420 7472 616e 7361 6374 696f 6e20 2853  t transaction (S
-00001a40: 514c 416c 6368 656d 7920 7632 2e58 2e58  QLAlchemy v2.X.X
-00001a50: 2069 7320 636f 6d6d 6974 2061 7320 796f   is commit as yo
-00001a60: 7520 676f 290a 2020 2020 6462 5f63 6f6e  u go).    db_con
-00001a70: 6e2e 636f 6d6d 6974 2829 0a0a 2020 2020  n.commit()..    
-00001a80: 2320 446f 2073 6f6d 6574 6869 6e67 2077  # Do something w
-00001a90: 6974 6820 7468 6520 7265 7375 6c74 730a  ith the results.
-00001aa0: 2020 2020 666f 7220 726f 7720 696e 2072      for row in r
-00001ab0: 6573 756c 743a 0a20 2020 2020 2020 2070  esult:.        p
-00001ac0: 7269 6e74 2872 6f77 290a 6060 600a 0a54  rint(row).```..T
-00001ad0: 6f20 636c 6f73 6520 7468 6520 6043 6f6e  o close the `Con
-00001ae0: 6e65 6374 6f72 6020 6f62 6a65 6374 2773  nector` object's
-00001af0: 2062 6163 6b67 726f 756e 6420 7265 736f   background reso
-00001b00: 7572 6365 732c 2063 616c 6c20 6974 2773  urces, call it's
-00001b10: 2060 636c 6f73 6528 2960 206d 6574 686f   `close()` metho
-00001b20: 6420 6173 2066 6f6c 6c6f 7773 3a0a 0a60  d as follows:..`
-00001b30: 6060 7079 7468 6f6e 0a63 6f6e 6e65 6374  ``python.connect
-00001b40: 6f72 2e63 6c6f 7365 2829 0a60 6060 0a0a  or.close().```..
-00001b50: 2a2a 4e6f 7465 2a2a 3a20 466f 7220 6d6f  **Note**: For mo
-00001b60: 7265 2065 7861 6d70 6c65 7320 6f66 2075  re examples of u
-00001b70: 7369 6e67 2053 514c 416c 6368 656d 7920  sing SQLAlchemy 
-00001b80: 746f 206d 616e 6167 6520 636f 6e6e 6563  to manage connec
-00001b90: 7469 6f6e 2070 6f6f 6c69 6e67 2077 6974  tion pooling wit
-00001ba0: 6820 7468 6520 636f 6e6e 6563 746f 722c  h the connector,
-00001bb0: 2070 6c65 6173 6520 7365 6520 5b43 6c6f   please see [Clo
-00001bc0: 7564 2053 514c 2053 514c 416c 6368 656d  ud SQL SQLAlchem
-00001bd0: 7920 5361 6d70 6c65 735d 2868 7474 7073  y Samples](https
-00001be0: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
-00001bf0: 636f 6d2f 7371 6c2f 646f 6373 2f70 6f73  com/sql/docs/pos
-00001c00: 7467 7265 732f 636f 6e6e 6563 742d 636f  tgres/connect-co
-00001c10: 6e6e 6563 746f 7273 2370 7974 686f 6e5f  nnectors#python_
-00001c20: 3129 2e0a 0a2a 2a4e 6f74 6520 666f 7220  1)...**Note for 
-00001c30: 5351 4c20 5365 7276 6572 2075 7365 7273  SQL Server users
-00001c40: 2a2a 3a20 4966 2079 6f75 7220 5351 4c20  **: If your SQL 
-00001c50: 5365 7276 6572 2069 6e73 7461 6e63 6520  Server instance 
-00001c60: 7265 7175 6972 6573 2053 534c 2c20 796f  requires SSL, yo
-00001c70: 7520 6e65 6564 2074 6f20 646f 776e 6c6f  u need to downlo
-00001c80: 6164 2074 6865 2043 4120 6365 7274 6966  ad the CA certif
-00001c90: 6963 6174 6520 666f 7220 796f 7572 2069  icate for your i
-00001ca0: 6e73 7461 6e63 6520 616e 6420 696e 636c  nstance and incl
-00001cb0: 7564 6520 6063 6166 696c 653d 7b70 6174  ude `cafile={pat
-00001cc0: 6820 746f 2064 6f77 6e6c 6f61 6465 6420  h to downloaded 
-00001cd0: 6365 7274 6966 6963 6174 657d 6020 616e  certificate}` an
-00001ce0: 6420 6076 616c 6964 6174 655f 686f 7374  d `validate_host
-00001cf0: 3d46 616c 7365 602e 2054 6869 7320 6973  =False`. This is
-00001d00: 2061 2077 6f72 6b61 726f 756e 6420 666f   a workaround fo
-00001d10: 7220 6120 5b6b 6e6f 776e 2069 7373 7565  r a [known issue
-00001d20: 5d28 6874 7470 733a 2f2f 6973 7375 6574  ](https://issuet
-00001d30: 7261 636b 6572 2e67 6f6f 676c 652e 636f  racker.google.co
-00001d40: 6d2f 3138 3438 3637 3134 3729 2e0a 0a23  m/184867147)...#
-00001d50: 2323 2043 6f6e 6669 6775 7269 6e67 2074  ## Configuring t
-00001d60: 6865 2043 6f6e 6e65 6374 6f72 0a0a 4966  he Connector..If
-00001d70: 2079 6f75 206e 6565 6420 746f 2063 7573   you need to cus
-00001d80: 746f 6d69 7a65 2073 6f6d 6574 6869 6e67  tomize something
-00001d90: 2061 626f 7574 2074 6865 2063 6f6e 6e65   about the conne
-00001da0: 6374 6f72 2c20 6f72 2077 616e 7420 746f  ctor, or want to
-00001db0: 2073 7065 6369 6679 0a64 6566 6175 6c74   specify.default
-00001dc0: 7320 666f 7220 6561 6368 2063 6f6e 6e65  s for each conne
-00001dd0: 6374 696f 6e20 746f 206d 616b 652c 2079  ction to make, y
-00001de0: 6f75 2063 616e 2069 6e69 7469 616c 697a  ou can initializ
-00001df0: 6520 610a 6043 6f6e 6e65 6374 6f72 6020  e a.`Connector` 
-00001e00: 6f62 6a65 6374 2061 7320 666f 6c6c 6f77  object as follow
-00001e10: 733a 0a0a 6060 6070 7974 686f 6e0a 6672  s:..```python.fr
-00001e20: 6f6d 2067 6f6f 676c 652e 636c 6f75 642e  om google.cloud.
-00001e30: 7371 6c2e 636f 6e6e 6563 746f 7220 696d  sql.connector im
-00001e40: 706f 7274 2043 6f6e 6e65 6374 6f72 2c20  port Connector, 
-00001e50: 4950 5479 7065 730a 0a23 204e 6f74 653a  IPTypes..# Note:
-00001e60: 2061 6c6c 2070 6172 616d 6574 6572 7320   all parameters 
-00001e70: 6265 6c6f 7720 6172 6520 6f70 7469 6f6e  below are option
-00001e80: 616c 0a63 6f6e 6e65 6374 6f72 203d 2043  al.connector = C
-00001e90: 6f6e 6e65 6374 6f72 280a 2020 2020 6970  onnector(.    ip
-00001ea0: 5f74 7970 653d 4950 5479 7065 732e 5055  _type=IPTypes.PU
-00001eb0: 424c 4943 2c0a 2020 2020 656e 6162 6c65  BLIC,.    enable
-00001ec0: 5f69 616d 5f61 7574 683d 4661 6c73 652c  _iam_auth=False,
-00001ed0: 0a20 2020 2074 696d 656f 7574 3d33 302c  .    timeout=30,
-00001ee0: 0a20 2020 2063 7265 6465 6e74 6961 6c73  .    credentials
-00001ef0: 3d63 7573 746f 6d5f 6372 6564 7320 2320  =custom_creds # 
-00001f00: 676f 6f67 6c65 2e61 7574 682e 6372 6564  google.auth.cred
-00001f10: 656e 7469 616c 732e 4372 6564 656e 7469  entials.Credenti
-00001f20: 616c 730a 290a 6060 600a 0a23 2323 2055  als.).```..### U
-00001f30: 7369 6e67 2043 6f6e 6e65 6374 6f72 2061  sing Connector a
-00001f40: 7320 6120 436f 6e74 6578 7420 4d61 6e61  s a Context Mana
-00001f50: 6765 720a 0a54 6865 2060 436f 6e6e 6563  ger..The `Connec
-00001f60: 746f 7260 206f 626a 6563 7420 6361 6e20  tor` object can 
-00001f70: 616c 736f 2062 6520 7573 6564 2061 7320  also be used as 
-00001f80: 6120 636f 6e74 6578 7420 6d61 6e61 6765  a context manage
-00001f90: 7220 696e 206f 7264 6572 2074 6f0a 6175  r in order to.au
-00001fa0: 746f 6d61 7469 6361 6c6c 7920 636c 6f73  tomatically clos
-00001fb0: 6520 616e 6420 636c 6561 6e75 7020 7265  e and cleanup re
-00001fc0: 736f 7572 6365 732c 2072 656d 6f76 696e  sources, removin
-00001fd0: 6720 7468 6520 6e65 6564 2066 6f72 2065  g the need for e
-00001fe0: 7870 6c69 6369 740a 6361 6c6c 7320 746f  xplicit.calls to
-00001ff0: 2060 636f 6e6e 6563 746f 722e 636c 6f73   `connector.clos
-00002000: 6528 2960 2e0a 0a43 6f6e 6e65 6374 6f72  e()`...Connector
-00002010: 2061 7320 6120 636f 6e74 6578 7420 6d61   as a context ma
-00002020: 6e61 6765 723a 0a0a 6060 6070 7974 686f  nager:..```pytho
-00002030: 6e0a 6672 6f6d 2067 6f6f 676c 652e 636c  n.from google.cl
-00002040: 6f75 642e 7371 6c2e 636f 6e6e 6563 746f  oud.sql.connecto
-00002050: 7220 696d 706f 7274 2043 6f6e 6e65 6374  r import Connect
-00002060: 6f72 0a69 6d70 6f72 7420 7371 6c61 6c63  or.import sqlalc
-00002070: 6865 6d79 0a0a 2320 6275 696c 6420 636f  hemy..# build co
-00002080: 6e6e 6563 7469 6f6e 0a64 6566 2067 6574  nnection.def get
-00002090: 636f 6e6e 2829 202d 3e20 7079 6d79 7371  conn() -> pymysq
-000020a0: 6c2e 636f 6e6e 6563 7469 6f6e 732e 436f  l.connections.Co
-000020b0: 6e6e 6563 7469 6f6e 3a0a 2020 2020 7769  nnection:.    wi
-000020c0: 7468 2043 6f6e 6e65 6374 6f72 2829 2061  th Connector() a
-000020d0: 7320 636f 6e6e 6563 746f 723a 0a20 2020  s connector:.   
-000020e0: 2020 2020 2063 6f6e 6e20 3d20 636f 6e6e       conn = conn
-000020f0: 6563 746f 722e 636f 6e6e 6563 7428 0a20  ector.connect(. 
-00002100: 2020 2020 2020 2020 2020 2022 7072 6f6a             "proj
-00002110: 6563 743a 7265 6769 6f6e 3a69 6e73 7461  ect:region:insta
-00002120: 6e63 6522 2c0a 2020 2020 2020 2020 2020  nce",.          
-00002130: 2020 2270 796d 7973 716c 222c 0a20 2020    "pymysql",.   
-00002140: 2020 2020 2020 2020 2075 7365 723d 226d           user="m
-00002150: 792d 7573 6572 222c 0a20 2020 2020 2020  y-user",.       
-00002160: 2020 2020 2070 6173 7377 6f72 643d 226d       password="m
-00002170: 792d 7061 7373 776f 7264 222c 0a20 2020  y-password",.   
-00002180: 2020 2020 2020 2020 2064 623d 226d 792d           db="my-
-00002190: 6462 2d6e 616d 6522 0a20 2020 2020 2020  db-name".       
-000021a0: 2029 0a20 2020 2072 6574 7572 6e20 636f   ).    return co
-000021b0: 6e6e 0a0a 2320 6372 6561 7465 2063 6f6e  nn..# create con
-000021c0: 6e65 6374 696f 6e20 706f 6f6c 0a70 6f6f  nection pool.poo
-000021d0: 6c20 3d20 7371 6c61 6c63 6865 6d79 2e63  l = sqlalchemy.c
-000021e0: 7265 6174 655f 656e 6769 6e65 280a 2020  reate_engine(.  
-000021f0: 2020 226d 7973 716c 2b70 796d 7973 716c    "mysql+pymysql
-00002200: 3a2f 2f22 2c0a 2020 2020 6372 6561 746f  ://",.    creato
-00002210: 723d 6765 7463 6f6e 6e2c 0a29 0a0a 2320  r=getconn,.)..# 
-00002220: 696e 7365 7274 2073 7461 7465 6d65 6e74  insert statement
-00002230: 0a69 6e73 6572 745f 7374 6d74 203d 2073  .insert_stmt = s
-00002240: 716c 616c 6368 656d 792e 7465 7874 280a  qlalchemy.text(.
-00002250: 2020 2020 2249 4e53 4552 5420 494e 544f      "INSERT INTO
-00002260: 206d 795f 7461 626c 6520 2869 642c 2074   my_table (id, t
-00002270: 6974 6c65 2920 5641 4c55 4553 2028 3a69  itle) VALUES (:i
-00002280: 642c 203a 7469 746c 6529 222c 0a29 0a0a  d, :title)",.)..
-00002290: 2320 696e 7465 7261 6374 2077 6974 6820  # interact with 
-000022a0: 436c 6f75 6420 5351 4c20 6461 7461 6261  Cloud SQL databa
-000022b0: 7365 2075 7369 6e67 2063 6f6e 6e65 6374  se using connect
-000022c0: 696f 6e20 706f 6f6c 0a77 6974 6820 706f  ion pool.with po
-000022d0: 6f6c 2e63 6f6e 6e65 6374 2829 2061 7320  ol.connect() as 
-000022e0: 6462 5f63 6f6e 6e3a 0a20 2020 2023 2069  db_conn:.    # i
-000022f0: 6e73 6572 7420 696e 746f 2064 6174 6162  nsert into datab
-00002300: 6173 650a 2020 2020 6462 5f63 6f6e 6e2e  ase.    db_conn.
-00002310: 6578 6563 7574 6528 696e 7365 7274 5f73  execute(insert_s
-00002320: 746d 742c 2070 6172 616d 6574 6572 733d  tmt, parameters=
-00002330: 7b22 6964 223a 2022 626f 6f6b 3122 2c20  {"id": "book1", 
-00002340: 2274 6974 6c65 223a 2022 426f 6f6b 204f  "title": "Book O
-00002350: 6e65 227d 290a 0a20 2020 2023 2063 6f6d  ne"})..    # com
-00002360: 6d69 7420 7472 616e 7361 6374 696f 6e20  mit transaction 
-00002370: 2853 514c 416c 6368 656d 7920 7632 2e58  (SQLAlchemy v2.X
-00002380: 2e58 2069 7320 636f 6d6d 6974 2061 7320  .X is commit as 
-00002390: 796f 7520 676f 290a 2020 2020 6462 5f63  you go).    db_c
-000023a0: 6f6e 6e2e 636f 6d6d 6974 2829 0a0a 2020  onn.commit()..  
-000023b0: 2020 2320 7175 6572 7920 6461 7461 6261    # query databa
-000023c0: 7365 0a20 2020 2072 6573 756c 7420 3d20  se.    result = 
-000023d0: 6462 5f63 6f6e 6e2e 6578 6563 7574 6528  db_conn.execute(
-000023e0: 7371 6c61 6c63 6865 6d79 2e74 6578 7428  sqlalchemy.text(
-000023f0: 2253 454c 4543 5420 2a20 6672 6f6d 206d  "SELECT * from m
-00002400: 795f 7461 626c 6522 2929 2e66 6574 6368  y_table")).fetch
-00002410: 616c 6c28 290a 0a20 2020 2023 2044 6f20  all()..    # Do 
-00002420: 736f 6d65 7468 696e 6720 7769 7468 2074  something with t
-00002430: 6865 2072 6573 756c 7473 0a20 2020 2066  he results.    f
-00002440: 6f72 2072 6f77 2069 6e20 7265 7375 6c74  or row in result
-00002450: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
-00002460: 726f 7729 0a60 6060 0a0a 2323 2320 5370  row).```..### Sp
-00002470: 6563 6966 7969 6e67 2050 7562 6c69 6320  ecifying Public 
-00002480: 6f72 2050 7269 7661 7465 2049 500a 0a54  or Private IP..T
-00002490: 6865 2043 6c6f 7564 2053 514c 2043 6f6e  he Cloud SQL Con
-000024a0: 6e65 6374 6f72 2066 6f72 2050 7974 686f  nector for Pytho
-000024b0: 6e20 6361 6e20 6265 2075 7365 6420 746f  n can be used to
-000024c0: 2063 6f6e 6e65 6374 2074 6f20 436c 6f75   connect to Clou
-000024d0: 6420 5351 4c20 696e 7374 616e 6365 7320  d SQL instances 
-000024e0: 7573 696e 6720 626f 7468 2070 7562 6c69  using both publi
-000024f0: 6320 616e 6420 7072 6976 6174 6520 4950  c and private IP
-00002500: 2061 6464 7265 7373 6573 2e20 546f 2073   addresses. To s
-00002510: 7065 6369 6679 2077 6869 6368 2049 5020  pecify which IP 
-00002520: 6164 6472 6573 7320 746f 2075 7365 2074  address to use t
-00002530: 6f20 636f 6e6e 6563 742c 2073 6574 2074  o connect, set t
-00002540: 6865 2060 6970 5f74 7970 6560 206b 6579  he `ip_type` key
-00002550: 776f 7264 2061 7267 756d 656e 7420 506f  word argument Po
-00002560: 7373 6962 6c65 2076 616c 7565 7320 6172  ssible values ar
-00002570: 6520 6049 5054 7970 6573 2e50 5542 4c49  e `IPTypes.PUBLI
-00002580: 4360 2061 6e64 2060 4950 5479 7065 732e  C` and `IPTypes.
-00002590: 5052 4956 4154 4560 2e0a 4578 616d 706c  PRIVATE`..Exampl
-000025a0: 653a 0a0a 6060 6070 7974 686f 6e0a 6672  e:..```python.fr
-000025b0: 6f6d 2067 6f6f 676c 652e 636c 6f75 642e  om google.cloud.
-000025c0: 7371 6c2e 636f 6e6e 6563 746f 7220 696d  sql.connector im
-000025d0: 706f 7274 2049 5054 7970 6573 0a0a 636f  port IPTypes..co
-000025e0: 6e6e 6563 746f 722e 636f 6e6e 6563 7428  nnector.connect(
-000025f0: 0a20 2020 2022 7072 6f6a 6563 743a 7265  .    "project:re
-00002600: 6769 6f6e 3a69 6e73 7461 6e63 6522 2c0a  gion:instance",.
-00002610: 2020 2020 2270 796d 7973 716c 222c 0a20      "pymysql",. 
-00002620: 2020 2069 705f 7479 7065 3d49 5054 7970     ip_type=IPTyp
-00002630: 6573 2e50 5249 5641 5445 2023 2075 7365  es.PRIVATE # use
-00002640: 2070 7269 7661 7465 2049 500a 2e2e 2e20   private IP.... 
-00002650: 696e 7365 7274 206f 7468 6572 206b 7761  insert other kwa
-00002660: 7267 7320 2e2e 2e0a 290a 6060 600a 0a4e  rgs ....).```..N
-00002670: 6f74 653a 2049 6620 7370 6563 6966 7969  ote: If specifyi
-00002680: 6e67 2050 7269 7661 7465 2049 502c 2079  ng Private IP, y
-00002690: 6f75 7220 6170 706c 6963 6174 696f 6e20  our application 
-000026a0: 6d75 7374 2061 6c72 6561 6479 2062 6520  must already be 
-000026b0: 696e 2074 6865 2073 616d 6520 5650 4320  in the same VPC 
-000026c0: 6e65 7477 6f72 6b20 6173 2079 6f75 7220  network as your 
-000026d0: 436c 6f75 6420 5351 4c20 496e 7374 616e  Cloud SQL Instan
-000026e0: 6365 2e0a 0a23 2323 2049 414d 2041 7574  ce...### IAM Aut
-000026f0: 6865 6e74 6963 6174 696f 6e0a 0a43 6f6e  hentication..Con
-00002700: 6e65 6374 696f 6e73 2075 7369 6e67 205b  nections using [
-00002710: 4175 746f 6d61 7469 6320 4941 4d20 6461  Automatic IAM da
-00002720: 7461 6261 7365 2061 7574 6865 6e74 6963  tabase authentic
-00002730: 6174 696f 6e5d 2868 7474 7073 3a2f 2f63  ation](https://c
-00002740: 6c6f 7564 2e67 6f6f 676c 652e 636f 6d2f  loud.google.com/
-00002750: 7371 6c2f 646f 6373 2f70 6f73 7467 7265  sql/docs/postgre
-00002760: 732f 6175 7468 656e 7469 6361 7469 6f6e  s/authentication
-00002770: 2361 7574 6f6d 6174 6963 2920 6172 6520  #automatic) are 
-00002780: 7375 7070 6f72 7465 6420 7768 656e 2075  supported when u
-00002790: 7369 6e67 2050 6f73 7467 7265 7320 6f72  sing Postgres or
-000027a0: 204d 7953 514c 2064 7269 7665 7273 2e0a   MySQL drivers..
-000027b0: 4669 7273 742c 206d 616b 6520 7375 7265  First, make sure
-000027c0: 2074 6f20 5b63 6f6e 6669 6775 7265 2079   to [configure y
-000027d0: 6f75 7220 436c 6f75 6420 5351 4c20 496e  our Cloud SQL In
-000027e0: 7374 616e 6365 2074 6f20 616c 6c6f 7720  stance to allow 
-000027f0: 4941 4d20 6175 7468 656e 7469 6361 7469  IAM authenticati
-00002800: 6f6e 5d28 6874 7470 733a 2f2f 636c 6f75  on](https://clou
-00002810: 642e 676f 6f67 6c65 2e63 6f6d 2f73 716c  d.google.com/sql
-00002820: 2f64 6f63 732f 706f 7374 6772 6573 2f63  /docs/postgres/c
-00002830: 7265 6174 652d 6564 6974 2d69 616d 2d69  reate-edit-iam-i
-00002840: 6e73 7461 6e63 6573 2363 6f6e 6669 6775  nstances#configu
-00002850: 7265 2d69 616d 2d64 622d 696e 7374 616e  re-iam-db-instan
-00002860: 6365 290a 616e 6420 5b61 6464 2061 6e20  ce).and [add an 
-00002870: 4941 4d20 6461 7461 6261 7365 2075 7365  IAM database use
-00002880: 725d 2868 7474 7073 3a2f 2f63 6c6f 7564  r](https://cloud
-00002890: 2e67 6f6f 676c 652e 636f 6d2f 7371 6c2f  .google.com/sql/
-000028a0: 646f 6373 2f70 6f73 7467 7265 732f 6372  docs/postgres/cr
-000028b0: 6561 7465 2d6d 616e 6167 652d 6961 6d2d  eate-manage-iam-
-000028c0: 7573 6572 7323 6372 6561 7469 6e67 2d61  users#creating-a
-000028d0: 2d64 6174 6162 6173 652d 7573 6572 292e  -database-user).
-000028e0: 0a0a 4e6f 772c 2079 6f75 2063 616e 2063  ..Now, you can c
-000028f0: 6f6e 6e65 6374 2075 7369 6e67 2075 7365  onnect using use
-00002900: 7220 6f72 2073 6572 7669 6365 2061 6363  r or service acc
-00002910: 6f75 6e74 2063 7265 6465 6e74 6961 6c73  ount credentials
-00002920: 2069 6e73 7465 6164 206f 6620 6120 7061   instead of a pa
-00002930: 7373 776f 7264 2e0a 496e 2074 6865 2063  ssword..In the c
-00002940: 616c 6c20 746f 2063 6f6e 6e65 6374 2c20  all to connect, 
-00002950: 7365 7420 7468 6520 6065 6e61 626c 655f  set the `enable_
-00002960: 6961 6d5f 6175 7468 6020 6b65 7977 6f72  iam_auth` keywor
-00002970: 6420 6172 6775 6d65 6e74 2074 6f20 7472  d argument to tr
-00002980: 7565 2061 6e64 2074 6865 2060 7573 6572  ue and the `user
-00002990: 6020 6172 6775 6d65 6e74 2074 6f20 7468  ` argument to th
-000029a0: 6520 6170 7072 6f70 7269 6174 656c 7920  e appropriately 
-000029b0: 666f 726d 6174 7465 6420 4941 4d20 7072  formatted IAM pr
-000029c0: 696e 6369 7061 6c2e 0a3e 2050 6f73 7467  incipal..> Postg
-000029d0: 7265 733a 2046 6f72 2061 6e20 4941 4d20  res: For an IAM 
-000029e0: 7573 6572 2061 6363 6f75 6e74 2c20 7468  user account, th
-000029f0: 6973 2069 7320 7468 6520 7573 6572 2773  is is the user's
-00002a00: 2065 6d61 696c 2061 6464 7265 7373 2e20   email address. 
-00002a10: 466f 7220 6120 7365 7276 6963 6520 6163  For a service ac
-00002a20: 636f 756e 742c 2069 7420 6973 2074 6865  count, it is the
-00002a30: 2073 6572 7669 6365 2061 6363 6f75 6e74   service account
-00002a40: 2773 2065 6d61 696c 2077 6974 686f 7574  's email without
-00002a50: 2074 6865 2060 2e67 7365 7276 6963 6561   the `.gservicea
-00002a60: 6363 6f75 6e74 2e63 6f6d 6020 646f 6d61  ccount.com` doma
-00002a70: 696e 2073 7566 6669 782e 0a0a 3e20 4d79  in suffix...> My
-00002a80: 5351 4c3a 2046 6f72 2061 6e20 4941 4d20  SQL: For an IAM 
-00002a90: 7573 6572 2061 6363 6f75 6e74 2c20 7468  user account, th
-00002aa0: 6973 2069 7320 7468 6520 7573 6572 2773  is is the user's
-00002ab0: 2065 6d61 696c 2061 6464 7265 7373 2c20   email address, 
-00002ac0: 7769 7468 6f75 7420 7468 6520 4020 6f72  without the @ or
-00002ad0: 2064 6f6d 6169 6e20 6e61 6d65 2e20 466f   domain name. Fo
-00002ae0: 7220 6578 616d 706c 652c 2066 6f72 2060  r example, for `
-00002af0: 7465 7374 2d75 7365 7240 676d 6169 6c2e  test-user@gmail.
-00002b00: 636f 6d60 2c20 7365 7420 7468 6520 6075  com`, set the `u
-00002b10: 7365 7260 2061 7267 756d 656e 7420 746f  ser` argument to
-00002b20: 2060 7465 7374 2d75 7365 7260 2e20 466f   `test-user`. Fo
-00002b30: 7220 6120 7365 7276 6963 6520 6163 636f  r a service acco
-00002b40: 756e 742c 2074 6869 7320 6973 2074 6865  unt, this is the
-00002b50: 2073 6572 7669 6365 2061 6363 6f75 6e74   service account
-00002b60: 2773 2065 6d61 696c 2061 6464 7265 7373  's email address
-00002b70: 2077 6974 686f 7574 2074 6865 2060 4070   without the `@p
-00002b80: 726f 6a65 6374 2d69 642e 6961 6d2e 6773  roject-id.iam.gs
-00002b90: 6572 7669 6365 6163 636f 756e 742e 636f  erviceaccount.co
-00002ba0: 6d60 2073 7566 6669 782e 0a0a 4578 616d  m` suffix...Exam
-00002bb0: 706c 653a 0a0a 6060 6070 7974 686f 6e0a  ple:..```python.
-00002bc0: 636f 6e6e 6563 746f 722e 636f 6e6e 6563  connector.connec
-00002bd0: 7428 0a20 2020 2020 2270 726f 6a65 6374  t(.     "project
-00002be0: 3a72 6567 696f 6e3a 696e 7374 616e 6365  :region:instance
-00002bf0: 222c 0a20 2020 2020 2270 6738 3030 3022  ",.     "pg8000"
-00002c00: 2c0a 2020 2020 2075 7365 723d 2270 6f73  ,.     user="pos
-00002c10: 7467 7265 732d 6961 6d2d 7573 6572 4067  tgres-iam-user@g
-00002c20: 6d61 696c 2e63 6f6d 222c 0a20 2020 2020  mail.com",.     
-00002c30: 6462 3d22 6d79 2d64 622d 6e61 6d65 222c  db="my-db-name",
-00002c40: 0a20 2020 2020 656e 6162 6c65 5f69 616d  .     enable_iam
-00002c50: 5f61 7574 683d 5472 7565 2c0a 2029 0a60  _auth=True,. ).`
-00002c60: 6060 0a0a 2323 2320 5351 4c20 5365 7276  ``..### SQL Serv
-00002c70: 6572 2041 6374 6976 6520 4469 7265 6374  er Active Direct
-00002c80: 6f72 7920 4175 7468 656e 7469 6361 7469  ory Authenticati
-00002c90: 6f6e 0a0a 4163 7469 7665 2044 6972 6563  on..Active Direc
-00002ca0: 746f 7279 2061 7574 6865 6e74 6963 6174  tory authenticat
-00002cb0: 696f 6e20 666f 7220 5351 4c20 5365 7276  ion for SQL Serv
-00002cc0: 6572 2069 6e73 7461 6e63 6573 2069 7320  er instances is 
-00002cd0: 6375 7272 656e 746c 7920 6f6e 6c79 2073  currently only s
-00002ce0: 7570 706f 7274 6564 206f 6e20 5769 6e64  upported on Wind
-00002cf0: 6f77 732e 2046 6972 7374 2c20 6d61 6b65  ows. First, make
-00002d00: 2073 7572 6520 746f 2066 6f6c 6c6f 7720   sure to follow 
-00002d10: 5b74 6865 7365 2073 7465 7073 5d28 6874  [these steps](ht
-00002d20: 7470 733a 2f2f 636c 6f75 642e 676f 6f67  tps://cloud.goog
-00002d30: 6c65 2e63 6f6d 2f62 6c6f 672f 746f 7069  le.com/blog/topi
-00002d40: 6373 2f64 6576 656c 6f70 6572 732d 7072  cs/developers-pr
-00002d50: 6163 7469 7469 6f6e 6572 732f 6372 6561  actitioners/crea
-00002d60: 7469 6e67 2d73 716c 2d73 6572 7665 722d  ting-sql-server-
-00002d70: 696e 7374 616e 6365 2d69 6e74 6567 7261  instance-integra
-00002d80: 7465 642d 6163 7469 7665 2d64 6972 6563  ted-active-direc
-00002d90: 746f 7279 2d75 7369 6e67 2d67 6f6f 676c  tory-using-googl
-00002da0: 652d 636c 6f75 642d 7371 6c29 2074 6f20  e-cloud-sql) to 
-00002db0: 7365 7420 7570 2061 204d 616e 6167 6564  set up a Managed
-00002dc0: 2041 4420 646f 6d61 696e 2061 6e64 206a   AD domain and j
-00002dd0: 6f69 6e20 796f 7572 2043 6c6f 7564 2053  oin your Cloud S
-00002de0: 514c 2069 6e73 7461 6e63 6520 746f 2074  QL instance to t
-00002df0: 6865 2064 6f6d 6169 6e2e 205b 5365 6520  he domain. [See 
-00002e00: 6865 7265 2066 6f72 206d 6f72 6520 696e  here for more in
-00002e10: 666f 206f 6e20 436c 6f75 6420 5351 4c20  fo on Cloud SQL 
-00002e20: 4163 7469 7665 2044 6972 6563 746f 7279  Active Directory
-00002e30: 2069 6e74 6567 7261 7469 6f6e 5d28 6874   integration](ht
-00002e40: 7470 733a 2f2f 636c 6f75 642e 676f 6f67  tps://cloud.goog
-00002e50: 6c65 2e63 6f6d 2f73 716c 2f64 6f63 732f  le.com/sql/docs/
-00002e60: 7371 6c73 6572 7665 722f 6164 292e 0a0a  sqlserver/ad)...
-00002e70: 4f6e 6365 2079 6f75 2068 6176 6520 666f  Once you have fo
-00002e80: 6c6c 6f77 6564 2074 6865 2073 7465 7073  llowed the steps
-00002e90: 206c 696e 6b65 6420 6162 6f76 652c 2079   linked above, y
-00002ea0: 6f75 2063 616e 2072 756e 2074 6865 2066  ou can run the f
-00002eb0: 6f6c 6c6f 7769 6e67 2063 6f64 6520 746f  ollowing code to
-00002ec0: 2072 6574 7572 6e20 6120 636f 6e6e 6563   return a connec
-00002ed0: 7469 6f6e 206f 626a 6563 743a 0a0a 6060  tion object:..``
-00002ee0: 6070 7974 686f 6e0a 636f 6e6e 6563 746f  `python.connecto
-00002ef0: 722e 636f 6e6e 6563 7428 0a20 2020 2022  r.connect(.    "
-00002f00: 7072 6f6a 6563 743a 7265 6769 6f6e 3a69  project:region:i
-00002f10: 6e73 7461 6e63 6522 2c0a 2020 2020 2270  nstance",.    "p
-00002f20: 7974 6473 222c 0a20 2020 2064 623d 226d  ytds",.    db="m
-00002f30: 792d 6462 2d6e 616d 6522 2c0a 2020 2020  y-db-name",.    
-00002f40: 6163 7469 7665 5f64 6972 6563 746f 7279  active_directory
-00002f50: 5f61 7574 683d 5472 7565 2c0a 2020 2020  _auth=True,.    
-00002f60: 7365 7276 6572 5f6e 616d 653d 2270 7562  server_name="pub
-00002f70: 6c69 632e 5b69 6e73 7461 6e63 655d 2e5b  lic.[instance].[
-00002f80: 6c6f 6361 7469 6f6e 5d2e 5b70 726f 6a65  location].[proje
-00002f90: 6374 5d2e 636c 6f75 6473 716c 2e5b 646f  ct].cloudsql.[do
-00002fa0: 6d61 696e 5d22 2c0a 290a 6060 600a 0a4f  main]",.).```..O
-00002fb0: 722c 2069 6620 7573 696e 6720 5072 6976  r, if using Priv
-00002fc0: 6174 6520 4950 3a0a 0a60 6060 7079 7468  ate IP:..```pyth
-00002fd0: 6f6e 0a63 6f6e 6e65 6374 6f72 2e63 6f6e  on.connector.con
-00002fe0: 6e65 6374 280a 2020 2020 2270 726f 6a65  nect(.    "proje
-00002ff0: 6374 3a72 6567 696f 6e3a 696e 7374 616e  ct:region:instan
-00003000: 6365 222c 0a20 2020 2022 7079 7464 7322  ce",.    "pytds"
-00003010: 2c0a 2020 2020 6462 3d22 6d79 2d64 622d  ,.    db="my-db-
-00003020: 6e61 6d65 222c 0a20 2020 2061 6374 6976  name",.    activ
-00003030: 655f 6469 7265 6374 6f72 795f 6175 7468  e_directory_auth
-00003040: 3d54 7275 652c 0a20 2020 2073 6572 7665  =True,.    serve
-00003050: 725f 6e61 6d65 3d22 7072 6976 6174 652e  r_name="private.
-00003060: 5b69 6e73 7461 6e63 655d 2e5b 6c6f 6361  [instance].[loca
-00003070: 7469 6f6e 5d2e 5b70 726f 6a65 6374 5d2e  tion].[project].
-00003080: 636c 6f75 6473 716c 2e5b 646f 6d61 696e  cloudsql.[domain
-00003090: 5d22 2c0a 2020 2020 6970 5f74 7970 653d  ]",.    ip_type=
-000030a0: 4950 5479 7065 732e 5052 4956 4154 450a  IPTypes.PRIVATE.
-000030b0: 290a 6060 600a 0a23 2323 2055 7369 6e67  ).```..### Using
-000030c0: 2074 6865 2050 7974 686f 6e20 436f 6e6e   the Python Conn
-000030d0: 6563 746f 7220 7769 7468 2050 7974 686f  ector with Pytho
-000030e0: 6e20 5765 6220 4672 616d 6577 6f72 6b73  n Web Frameworks
-000030f0: 0a0a 5468 6520 5079 7468 6f6e 2043 6f6e  ..The Python Con
-00003100: 6e65 6374 6f72 2063 616e 2062 6520 7573  nector can be us
-00003110: 6564 2061 6c6f 6e67 7369 6465 2070 6f70  ed alongside pop
-00003120: 756c 6172 2050 7974 686f 6e20 7765 6220  ular Python web 
-00003130: 6672 616d 6577 6f72 6b73 2073 7563 680a  frameworks such.
-00003140: 6173 2046 6c61 736b 2c20 4661 7374 4150  as Flask, FastAP
-00003150: 492c 2065 7463 2c20 746f 2069 6e74 6567  I, etc, to integ
-00003160: 7261 7465 2043 6c6f 7564 2053 514c 2064  rate Cloud SQL d
-00003170: 6174 6162 6173 6573 2077 6974 6869 6e20  atabases within 
-00003180: 796f 7572 0a77 6562 2061 7070 6c69 6361  your.web applica
-00003190: 7469 6f6e 732e 0a0a 2323 2323 2046 6c61  tions...#### Fla
-000031a0: 736b 2d53 514c 416c 6368 656d 790a 0a5b  sk-SQLAlchemy..[
-000031b0: 466c 6173 6b2d 5351 4c41 6c63 6865 6d79  Flask-SQLAlchemy
-000031c0: 5d28 6874 7470 733a 2f2f 666c 6173 6b2d  ](https://flask-
-000031d0: 7371 6c61 6c63 6865 6d79 2e70 616c 6c65  sqlalchemy.palle
-000031e0: 7473 7072 6f6a 6563 7473 2e63 6f6d 2f65  tsprojects.com/e
-000031f0: 6e2f 322e 782f 290a 6973 2061 6e20 6578  n/2.x/).is an ex
-00003200: 7465 6e73 696f 6e20 666f 7220 5b46 6c61  tension for [Fla
-00003210: 736b 5d28 6874 7470 733a 2f2f 666c 6173  sk](https://flas
-00003220: 6b2e 7061 6c6c 6574 7370 726f 6a65 6374  k.palletsproject
-00003230: 732e 636f 6d2f 656e 2f32 2e32 2e78 2f29  s.com/en/2.2.x/)
-00003240: 0a74 6861 7420 6164 6473 2073 7570 706f  .that adds suppo
-00003250: 7274 2066 6f72 205b 5351 4c41 6c63 6865  rt for [SQLAlche
-00003260: 6d79 5d28 6874 7470 733a 2f2f 7777 772e  my](https://www.
-00003270: 7371 6c61 6c63 6865 6d79 2e6f 7267 2f29  sqlalchemy.org/)
-00003280: 2074 6f20 796f 7572 0a61 7070 6c69 6361   to your.applica
-00003290: 7469 6f6e 2e20 4974 2061 696d 7320 746f  tion. It aims to
-000032a0: 2073 696d 706c 6966 7920 7573 696e 6720   simplify using 
-000032b0: 5351 4c41 6c63 6865 6d79 2077 6974 6820  SQLAlchemy with 
-000032c0: 466c 6173 6b20 6279 2070 726f 7669 6469  Flask by providi
-000032d0: 6e67 0a75 7365 6675 6c20 6465 6661 756c  ng.useful defaul
-000032e0: 7473 2061 6e64 2065 7874 7261 2068 656c  ts and extra hel
-000032f0: 7065 7273 2074 6861 7420 6d61 6b65 2069  pers that make i
-00003300: 7420 6561 7369 6572 2074 6f20 6163 636f  t easier to acco
-00003310: 6d70 6c69 7368 0a63 6f6d 6d6f 6e20 7461  mplish.common ta
-00003320: 736b 732e 0a0a 596f 7520 6361 6e20 636f  sks...You can co
-00003330: 6e66 6967 7572 6520 466c 6173 6b2d 5351  nfigure Flask-SQ
-00003340: 4c41 6c63 6865 6d79 2074 6f20 636f 6e6e  LAlchemy to conn
-00003350: 6563 7420 746f 2061 2043 6c6f 7564 2053  ect to a Cloud S
-00003360: 514c 2064 6174 6162 6173 6520 6672 6f6d  QL database from
-00003370: 0a79 6f75 7220 7765 6220 6170 706c 6963  .your web applic
-00003380: 6174 696f 6e20 7468 726f 7567 6820 7468  ation through th
-00003390: 6520 666f 6c6c 6f77 696e 673a 0a0a 6060  e following:..``
-000033a0: 6070 7974 686f 6e0a 6672 6f6d 2066 6c61  `python.from fla
-000033b0: 736b 2069 6d70 6f72 7420 466c 6173 6b0a  sk import Flask.
-000033c0: 6672 6f6d 2066 6c61 736b 5f73 716c 616c  from flask_sqlal
-000033d0: 6368 656d 7920 696d 706f 7274 2053 514c  chemy import SQL
-000033e0: 416c 6368 656d 790a 6672 6f6d 2067 6f6f  Alchemy.from goo
-000033f0: 676c 652e 636c 6f75 642e 7371 6c2e 636f  gle.cloud.sql.co
-00003400: 6e6e 6563 746f 7220 696d 706f 7274 2043  nnector import C
-00003410: 6f6e 6e65 6374 6f72 2c20 4950 5479 7065  onnector, IPType
-00003420: 730a 0a0a 2320 5079 7468 6f6e 2043 6f6e  s...# Python Con
-00003430: 6e65 6374 6f72 2064 6174 6162 6173 6520  nector database 
-00003440: 636f 6e6e 6563 7469 6f6e 2066 756e 6374  connection funct
-00003450: 696f 6e0a 6465 6620 6765 7463 6f6e 6e28  ion.def getconn(
-00003460: 293a 0a20 2020 2077 6974 6820 436f 6e6e  ):.    with Conn
-00003470: 6563 746f 7228 2920 6173 2063 6f6e 6e65  ector() as conne
-00003480: 6374 6f72 3a0a 2020 2020 2020 2020 636f  ctor:.        co
-00003490: 6e6e 203d 2063 6f6e 6e65 6374 6f72 2e63  nn = connector.c
-000034a0: 6f6e 6e65 6374 280a 2020 2020 2020 2020  onnect(.        
-000034b0: 2020 2020 2270 726f 6a65 6374 3a72 6567      "project:reg
-000034c0: 696f 6e3a 696e 7374 616e 6365 2d6e 616d  ion:instance-nam
-000034d0: 6522 2c20 2320 436c 6f75 6420 5351 4c20  e", # Cloud SQL 
-000034e0: 496e 7374 616e 6365 2043 6f6e 6e65 6374  Instance Connect
-000034f0: 696f 6e20 4e61 6d65 0a20 2020 2020 2020  ion Name.       
-00003500: 2020 2020 2022 7067 3830 3030 222c 0a20       "pg8000",. 
-00003510: 2020 2020 2020 2020 2020 2075 7365 723d             user=
-00003520: 226d 792d 7573 6572 222c 0a20 2020 2020  "my-user",.     
-00003530: 2020 2020 2020 2070 6173 7377 6f72 643d         password=
-00003540: 226d 792d 7061 7373 776f 7264 222c 0a20  "my-password",. 
-00003550: 2020 2020 2020 2020 2020 2064 623d 226d             db="m
-00003560: 792d 6461 7461 6261 7365 222c 0a20 2020  y-database",.   
-00003570: 2020 2020 2020 2020 2069 705f 7479 7065           ip_type
-00003580: 3d20 4950 5479 7065 732e 5055 424c 4943  = IPTypes.PUBLIC
-00003590: 2020 2320 4950 5479 7065 732e 5052 4956    # IPTypes.PRIV
-000035a0: 4154 4520 666f 7220 7072 6976 6174 6520  ATE for private 
-000035b0: 4950 0a20 2020 2020 2020 2029 0a20 2020  IP.        ).   
-000035c0: 2020 2020 2072 6574 7572 6e20 636f 6e6e       return conn
-000035d0: 0a0a 0a61 7070 203d 2046 6c61 736b 285f  ...app = Flask(_
-000035e0: 5f6e 616d 655f 5f29 0a0a 2320 636f 6e66  _name__)..# conf
-000035f0: 6967 7572 6520 466c 6173 6b2d 5351 4c41  igure Flask-SQLA
-00003600: 6c63 6865 6d79 2074 6f20 7573 6520 5079  lchemy to use Py
-00003610: 7468 6f6e 2043 6f6e 6e65 6374 6f72 0a61  thon Connector.a
-00003620: 7070 2e63 6f6e 6669 675b 2753 514c 414c  pp.config['SQLAL
-00003630: 4348 454d 595f 4441 5441 4241 5345 5f55  CHEMY_DATABASE_U
-00003640: 5249 275d 203d 2022 706f 7374 6772 6573  RI'] = "postgres
-00003650: 716c 2b70 6738 3030 303a 2f2f 220a 6170  ql+pg8000://".ap
-00003660: 702e 636f 6e66 6967 5b27 5351 4c41 4c43  p.config['SQLALC
-00003670: 4845 4d59 5f45 4e47 494e 455f 4f50 5449  HEMY_ENGINE_OPTI
-00003680: 4f4e 5327 5d20 3d20 7b0a 2020 2020 2263  ONS'] = {.    "c
-00003690: 7265 6174 6f72 223a 2067 6574 636f 6e6e  reator": getconn
-000036a0: 0a7d 0a0a 6462 203d 2053 514c 416c 6368  .}..db = SQLAlch
-000036b0: 656d 7928 6170 7029 0a60 6060 0a0a 466f  emy(app).```..Fo
-000036c0: 7220 6d6f 7265 2064 6574 6169 6c73 206f  r more details o
-000036d0: 6e20 686f 7720 746f 2075 7365 2046 6c61  n how to use Fla
-000036e0: 736b 2d53 514c 416c 6368 656d 792c 2063  sk-SQLAlchemy, c
-000036f0: 6865 636b 206f 7574 2074 6865 0a5b 466c  heck out the.[Fl
-00003700: 6173 6b2d 5351 4c41 6c63 6865 6d79 2051  ask-SQLAlchemy Q
-00003710: 7569 636b 7374 6172 7473 5d28 6874 7470  uickstarts](http
-00003720: 733a 2f2f 666c 6173 6b2d 7371 6c61 6c63  s://flask-sqlalc
-00003730: 6865 6d79 2e70 616c 6c65 7473 7072 6f6a  hemy.palletsproj
-00003740: 6563 7473 2e63 6f6d 2f65 6e2f 322e 782f  ects.com/en/2.x/
-00003750: 7175 6963 6b73 7461 7274 2f23 290a 0a23  quickstart/#)..#
-00003760: 2323 2320 4661 7374 4150 490a 0a5b 4661  ### FastAPI..[Fa
-00003770: 7374 4150 495d 2868 7474 7073 3a2f 2f66  stAPI](https://f
-00003780: 6173 7461 7069 2e74 6961 6e67 6f6c 6f2e  astapi.tiangolo.
-00003790: 636f 6d2f 2920 6973 2061 206d 6f64 6572  com/) is a moder
-000037a0: 6e2c 2066 6173 7420 2868 6967 682d 7065  n, fast (high-pe
-000037b0: 7266 6f72 6d61 6e63 6529 2c0a 7765 6220  rformance),.web 
-000037c0: 6672 616d 6577 6f72 6b20 666f 7220 6275  framework for bu
-000037d0: 696c 6469 6e67 2041 5049 7320 7769 7468  ilding APIs with
-000037e0: 2050 7974 686f 6e20 6261 7365 6420 6f6e   Python based on
-000037f0: 2073 7461 6e64 6172 6420 5079 7468 6f6e   standard Python
-00003800: 2074 7970 6520 6869 6e74 732e 0a0a 596f   type hints...Yo
-00003810: 7520 6361 6e20 636f 6e66 6967 7572 6520  u can configure 
-00003820: 4661 7374 4150 4920 746f 2063 6f6e 6e65  FastAPI to conne
-00003830: 6374 2074 6f20 6120 436c 6f75 6420 5351  ct to a Cloud SQ
-00003840: 4c20 6461 7461 6261 7365 2066 726f 6d0a  L database from.
-00003850: 796f 7572 2077 6562 2061 7070 6c69 6361  your web applica
-00003860: 7469 6f6e 2075 7369 6e67 205b 5351 4c41  tion using [SQLA
-00003870: 6c63 6865 6d79 204f 524d 5d28 6874 7470  lchemy ORM](http
-00003880: 733a 2f2f 646f 6373 2e73 716c 616c 6368  s://docs.sqlalch
-00003890: 656d 792e 6f72 672f 656e 2f31 342f 6f72  emy.org/en/14/or
-000038a0: 6d2f 290a 7468 726f 7567 6820 7468 6520  m/).through the 
-000038b0: 666f 6c6c 6f77 696e 673a 0a0a 6060 6070  following:..```p
-000038c0: 7974 686f 6e0a 6672 6f6d 2073 716c 616c  ython.from sqlal
-000038d0: 6368 656d 7920 696d 706f 7274 2063 7265  chemy import cre
-000038e0: 6174 655f 656e 6769 6e65 0a66 726f 6d20  ate_engine.from 
-000038f0: 7371 6c61 6c63 6865 6d79 2e65 7874 2e64  sqlalchemy.ext.d
-00003900: 6563 6c61 7261 7469 7665 2069 6d70 6f72  eclarative impor
-00003910: 7420 6465 636c 6172 6174 6976 655f 6261  t declarative_ba
-00003920: 7365 0a66 726f 6d20 7371 6c61 6c63 6865  se.from sqlalche
-00003930: 6d79 2e6f 726d 2069 6d70 6f72 7420 7365  my.orm import se
-00003940: 7373 696f 6e6d 616b 6572 0a66 726f 6d20  ssionmaker.from 
-00003950: 676f 6f67 6c65 2e63 6c6f 7564 2e73 716c  google.cloud.sql
-00003960: 2e63 6f6e 6e65 6374 6f72 2069 6d70 6f72  .connector impor
-00003970: 7420 436f 6e6e 6563 746f 722c 2049 5054  t Connector, IPT
-00003980: 7970 6573 0a0a 2320 5079 7468 6f6e 2043  ypes..# Python C
-00003990: 6f6e 6e65 6374 6f72 2064 6174 6162 6173  onnector databas
-000039a0: 6520 636f 6e6e 6563 7469 6f6e 2066 756e  e connection fun
-000039b0: 6374 696f 6e0a 6465 6620 6765 7463 6f6e  ction.def getcon
-000039c0: 6e28 293a 0a20 2020 2077 6974 6820 436f  n():.    with Co
-000039d0: 6e6e 6563 746f 7228 2920 6173 2063 6f6e  nnector() as con
-000039e0: 6e65 6374 6f72 3a0a 2020 2020 2020 2020  nector:.        
-000039f0: 636f 6e6e 203d 2063 6f6e 6e65 6374 6f72  conn = connector
-00003a00: 2e63 6f6e 6e65 6374 280a 2020 2020 2020  .connect(.      
-00003a10: 2020 2020 2020 2270 726f 6a65 6374 3a72        "project:r
-00003a20: 6567 696f 6e3a 696e 7374 616e 6365 2d6e  egion:instance-n
-00003a30: 616d 6522 2c20 2320 436c 6f75 6420 5351  ame", # Cloud SQ
-00003a40: 4c20 496e 7374 616e 6365 2043 6f6e 6e65  L Instance Conne
-00003a50: 6374 696f 6e20 4e61 6d65 0a20 2020 2020  ction Name.     
-00003a60: 2020 2020 2020 2022 7067 3830 3030 222c         "pg8000",
-00003a70: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
-00003a80: 723d 226d 792d 7573 6572 222c 0a20 2020  r="my-user",.   
-00003a90: 2020 2020 2020 2020 2070 6173 7377 6f72           passwor
-00003aa0: 643d 226d 792d 7061 7373 776f 7264 222c  d="my-password",
-00003ab0: 0a20 2020 2020 2020 2020 2020 2064 623d  .            db=
-00003ac0: 226d 792d 6461 7461 6261 7365 222c 0a20  "my-database",. 
-00003ad0: 2020 2020 2020 2020 2020 2069 705f 7479             ip_ty
-00003ae0: 7065 3d20 4950 5479 7065 732e 5055 424c  pe= IPTypes.PUBL
-00003af0: 4943 2020 2320 4950 5479 7065 732e 5052  IC  # IPTypes.PR
-00003b00: 4956 4154 4520 666f 7220 7072 6976 6174  IVATE for privat
-00003b10: 6520 4950 0a20 2020 2020 2020 2029 0a20  e IP.        ). 
-00003b20: 2020 2072 6574 7572 6e20 636f 6e6e 0a0a     return conn..
-00003b30: 5351 4c41 4c43 4845 4d59 5f44 4154 4142  SQLALCHEMY_DATAB
-00003b40: 4153 455f 5552 4c20 3d20 2270 6f73 7467  ASE_URL = "postg
-00003b50: 7265 7371 6c2b 7067 3830 3030 3a2f 2f22  resql+pg8000://"
-00003b60: 0a0a 656e 6769 6e65 203d 2063 7265 6174  ..engine = creat
-00003b70: 655f 656e 6769 6e65 280a 2020 2020 5351  e_engine(.    SQ
-00003b80: 4c41 4c43 4845 4d59 5f44 4154 4142 4153  LALCHEMY_DATABAS
-00003b90: 455f 5552 4c20 2c20 6372 6561 746f 723d  E_URL , creator=
-00003ba0: 6765 7463 6f6e 6e0a 290a 0a23 2063 7265  getconn.)..# cre
-00003bb0: 6174 6520 5351 4c41 6c63 6865 6d79 204f  ate SQLAlchemy O
-00003bc0: 524d 2073 6573 7369 6f6e 0a53 6573 7369  RM session.Sessi
-00003bd0: 6f6e 4c6f 6361 6c20 3d20 7365 7373 696f  onLocal = sessio
-00003be0: 6e6d 616b 6572 2861 7574 6f63 6f6d 6d69  nmaker(autocommi
-00003bf0: 743d 4661 6c73 652c 2061 7574 6f66 6c75  t=False, autoflu
-00003c00: 7368 3d46 616c 7365 2c20 6269 6e64 3d65  sh=False, bind=e
-00003c10: 6e67 696e 6529 0a0a 4261 7365 203d 2064  ngine)..Base = d
-00003c20: 6563 6c61 7261 7469 7665 5f62 6173 6528  eclarative_base(
-00003c30: 290a 6060 600a 0a54 6f20 6c65 6172 6e20  ).```..To learn 
-00003c40: 6d6f 7265 2061 626f 7574 2069 6e74 6567  more about integ
-00003c50: 7261 7469 6e67 2061 2064 6174 6162 6173  rating a databas
-00003c60: 6520 696e 746f 2079 6f75 7220 4661 7374  e into your Fast
-00003c70: 4150 4920 6170 706c 6963 6174 696f 6e2c  API application,
-00003c80: 0a66 6f6c 6c6f 7720 616c 6f6e 6720 7468  .follow along th
-00003c90: 6520 5b46 6173 7441 5049 2053 514c 2044  e [FastAPI SQL D
-00003ca0: 6174 6162 6173 6520 6775 6964 655d 2868  atabase guide](h
-00003cb0: 7474 7073 3a2f 2f66 6173 7461 7069 2e74  ttps://fastapi.t
-00003cc0: 6961 6e67 6f6c 6f2e 636f 6d2f 7475 746f  iangolo.com/tuto
-00003cd0: 7269 616c 2f73 716c 2d64 6174 6162 6173  rial/sql-databas
-00003ce0: 6573 2f23 6372 6561 7465 2d74 6865 2d64  es/#create-the-d
-00003cf0: 6174 6162 6173 652d 6d6f 6465 6c73 292e  atabase-models).
-00003d00: 0a0a 2323 2320 4173 796e 6320 4472 6976  ..### Async Driv
-00003d10: 6572 2055 7361 6765 0a0a 5468 6520 436c  er Usage..The Cl
-00003d20: 6f75 6420 5351 4c20 436f 6e6e 6563 746f  oud SQL Connecto
-00003d30: 7220 6973 2063 6f6d 7061 7469 626c 6520  r is compatible 
-00003d40: 7769 7468 0a5b 6173 796e 6369 6f5d 2868  with.[asyncio](h
-00003d50: 7474 7073 3a2f 2f64 6f63 732e 7079 7468  ttps://docs.pyth
-00003d60: 6f6e 2e6f 7267 2f33 2f6c 6962 7261 7279  on.org/3/library
-00003d70: 2f61 7379 6e63 696f 2e68 746d 6c29 2074  /asyncio.html) t
-00003d80: 6f20 696d 7072 6f76 6520 7468 6520 7370  o improve the sp
-00003d90: 6565 640a 616e 6420 6566 6669 6369 656e  eed.and efficien
-00003da0: 6379 206f 6620 6461 7461 6261 7365 2063  cy of database c
-00003db0: 6f6e 6e65 6374 696f 6e73 2074 6872 6f75  onnections throu
-00003dc0: 6768 2063 6f6e 6375 7272 656e 6379 2e20  gh concurrency. 
-00003dd0: 596f 7520 6361 6e20 7573 6520 616c 6c0a  You can use all.
-00003de0: 6e6f 6e2d 6173 796e 6369 6f20 6472 6976  non-asyncio driv
-00003df0: 6572 7320 7468 726f 7567 6820 7468 6520  ers through the 
-00003e00: 6043 6f6e 6e65 6374 6f72 2e63 6f6e 6e65  `Connector.conne
-00003e10: 6374 5f61 7379 6e63 6020 6675 6e63 7469  ct_async` functi
-00003e20: 6f6e 2c20 696e 2061 6464 6974 696f 6e0a  on, in addition.
-00003e30: 746f 2074 6865 2066 6f6c 6c6f 7769 6e67  to the following
-00003e40: 2061 7379 6e63 696f 2064 6174 6162 6173   asyncio databas
-00003e50: 6520 6472 6976 6572 733a 0a2d 205b 6173  e drivers:.- [as
-00003e60: 796e 6370 675d 2868 7474 7073 3a2f 2f6d  yncpg](https://m
-00003e70: 6167 6963 7374 6163 6b2e 6769 7468 7562  agicstack.github
-00003e80: 2e69 6f2f 6173 796e 6370 6729 2028 506f  .io/asyncpg) (Po
-00003e90: 7374 6772 6573 290a 0a54 6865 2043 6c6f  stgres)..The Clo
-00003ea0: 7564 2053 514c 2043 6f6e 6e65 6374 6f72  ud SQL Connector
-00003eb0: 2068 6173 2061 2068 656c 7065 7220 6063   has a helper `c
-00003ec0: 7265 6174 655f 6173 796e 635f 636f 6e6e  reate_async_conn
-00003ed0: 6563 746f 7260 2066 756e 6374 696f 6e20  ector` function 
-00003ee0: 7468 6174 2069 730a 7265 636f 6d6d 656e  that is.recommen
-00003ef0: 6465 6420 666f 7220 6173 796e 6369 6f20  ded for asyncio 
-00003f00: 6461 7461 6261 7365 2063 6f6e 6e65 6374  database connect
-00003f10: 696f 6e73 2e20 4974 2072 6574 7572 6e73  ions. It returns
-00003f20: 2061 2060 436f 6e6e 6563 746f 7260 0a6f   a `Connector`.o
-00003f30: 626a 6563 7420 7468 6174 2075 7365 7320  bject that uses 
-00003f40: 7468 6520 6375 7272 656e 7420 7468 7265  the current thre
-00003f50: 6164 2773 2072 756e 6e69 6e67 2065 7665  ad's running eve
-00003f60: 6e74 206c 6f6f 702e 2054 6869 7320 6973  nt loop. This is
-00003f70: 2064 6966 6665 7265 6e74 0a74 6861 6e20   different.than 
-00003f80: 6043 6f6e 6e65 6374 6f72 2829 6020 7768  `Connector()` wh
-00003f90: 6963 6820 6279 2064 6566 6175 6c74 2069  ich by default i
-00003fa0: 6e69 7469 616c 697a 6573 2061 206e 6577  nitializes a new
-00003fb0: 2065 7665 6e74 206c 6f6f 7020 696e 2061   event loop in a
-00003fc0: 0a62 6163 6b67 726f 756e 6420 7468 7265  .background thre
-00003fd0: 6164 2e0a 0a54 6865 2060 6372 6561 7465  ad...The `create
-00003fe0: 5f61 7379 6e63 5f63 6f6e 6e65 6374 6f72  _async_connector
-00003ff0: 6020 616c 6c6f 7773 2061 6c6c 2074 6865  ` allows all the
-00004000: 2073 616d 6520 696e 7075 7420 6172 6775   same input argu
-00004010: 6d65 6e74 7320 6173 2074 6865 0a5b 436f  ments as the.[Co
-00004020: 6e6e 6563 746f 725d 2823 636f 6e66 6967  nnector](#config
-00004030: 7572 696e 672d 7468 652d 636f 6e6e 6563  uring-the-connec
-00004040: 746f 7229 206f 626a 6563 742e 0a0a 4f6e  tor) object...On
-00004050: 6365 2061 2060 436f 6e6e 6563 746f 7260  ce a `Connector`
-00004060: 206f 626a 6563 7420 6973 2072 6574 7572   object is retur
-00004070: 6e65 6420 6279 2060 6372 6561 7465 5f61  ned by `create_a
-00004080: 7379 6e63 5f63 6f6e 6e65 6374 6f72 6020  sync_connector` 
-00004090: 796f 7520 6361 6e20 6361 6c6c 0a69 7473  you can call.its
-000040a0: 2060 636f 6e6e 6563 745f 6173 796e 6360   `connect_async`
-000040b0: 206d 6574 686f 642c 206a 7573 7420 6173   method, just as
-000040c0: 2079 6f75 2077 6f75 6c64 2074 6865 2060   you would the `
-000040d0: 636f 6e6e 6563 7460 206d 6574 686f 643a  connect` method:
-000040e0: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
-000040f0: 7274 2061 7379 6e63 7067 0a0a 696d 706f  rt asyncpg..impo
-00004100: 7274 2073 716c 616c 6368 656d 790a 6672  rt sqlalchemy.fr
-00004110: 6f6d 2073 716c 616c 6368 656d 792e 6578  om sqlalchemy.ex
-00004120: 742e 6173 796e 6369 6f20 696d 706f 7274  t.asyncio import
-00004130: 2041 7379 6e63 456e 6769 6e65 2c20 6372   AsyncEngine, cr
-00004140: 6561 7465 5f61 7379 6e63 5f65 6e67 696e  eate_async_engin
-00004150: 650a 0a66 726f 6d20 676f 6f67 6c65 2e63  e..from google.c
-00004160: 6c6f 7564 2e73 716c 2e63 6f6e 6e65 6374  loud.sql.connect
-00004170: 6f72 2069 6d70 6f72 7420 436f 6e6e 6563  or import Connec
-00004180: 746f 722c 2063 7265 6174 655f 6173 796e  tor, create_asyn
-00004190: 635f 636f 6e6e 6563 746f 720a 0a61 7379  c_connector..asy
-000041a0: 6e63 2064 6566 2069 6e69 745f 636f 6e6e  nc def init_conn
-000041b0: 6563 7469 6f6e 5f70 6f6f 6c28 636f 6e6e  ection_pool(conn
-000041c0: 6563 746f 723a 2043 6f6e 6e65 6374 6f72  ector: Connector
-000041d0: 2920 2d3e 2041 7379 6e63 456e 6769 6e65  ) -> AsyncEngine
-000041e0: 3a0a 2020 2020 2320 696e 6974 6961 6c69  :.    # initiali
-000041f0: 7a65 2043 6f6e 6e65 6374 6f72 206f 626a  ze Connector obj
-00004200: 6563 7420 666f 7220 636f 6e6e 6563 7469  ect for connecti
-00004210: 6f6e 7320 746f 2043 6c6f 7564 2053 514c  ons to Cloud SQL
-00004220: 0a20 2020 2061 7379 6e63 2064 6566 2067  .    async def g
-00004230: 6574 636f 6e6e 2829 202d 3e20 6173 796e  etconn() -> asyn
-00004240: 6370 672e 436f 6e6e 6563 7469 6f6e 3a0a  cpg.Connection:.
-00004250: 2020 2020 2020 2020 636f 6e6e 3a20 6173          conn: as
-00004260: 796e 6370 672e 436f 6e6e 6563 7469 6f6e  yncpg.Connection
-00004270: 203d 2061 7761 6974 2063 6f6e 6e65 6374   = await connect
-00004280: 6f72 2e63 6f6e 6e65 6374 5f61 7379 6e63  or.connect_async
-00004290: 280a 2020 2020 2020 2020 2020 2020 2270  (.            "p
-000042a0: 726f 6a65 6374 3a72 6567 696f 6e3a 696e  roject:region:in
-000042b0: 7374 616e 6365 222c 2020 2320 436c 6f75  stance",  # Clou
-000042c0: 6420 5351 4c20 696e 7374 616e 6365 2063  d SQL instance c
-000042d0: 6f6e 6e65 6374 696f 6e20 6e61 6d65 0a20  onnection name. 
-000042e0: 2020 2020 2020 2020 2020 2022 6173 796e             "asyn
-000042f0: 6370 6722 2c0a 2020 2020 2020 2020 2020  cpg",.          
-00004300: 2020 7573 6572 3d22 6d79 2d75 7365 7222    user="my-user"
-00004310: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
-00004320: 7373 776f 7264 3d22 6d79 2d70 6173 7377  ssword="my-passw
-00004330: 6f72 6422 2c0a 2020 2020 2020 2020 2020  ord",.          
-00004340: 2020 6462 3d22 6d79 2d64 622d 6e61 6d65    db="my-db-name
-00004350: 220a 2020 2020 2020 2020 2020 2020 2320  ".            # 
-00004360: 2e2e 2e20 6164 6469 7469 6f6e 616c 2064  ... additional d
-00004370: 6174 6162 6173 6520 6472 6976 6572 2061  atabase driver a
-00004380: 7267 730a 2020 2020 2020 2020 290a 2020  rgs.        ).  
-00004390: 2020 2020 2020 7265 7475 726e 2063 6f6e        return con
-000043a0: 6e0a 0a20 2020 2023 2054 6865 2043 6c6f  n..    # The Clo
-000043b0: 7564 2053 514c 2050 7974 686f 6e20 436f  ud SQL Python Co
-000043c0: 6e6e 6563 746f 7220 6361 6e20 6265 2075  nnector can be u
-000043d0: 7365 6420 616c 6f6e 6720 7769 7468 2053  sed along with S
-000043e0: 514c 416c 6368 656d 7920 7573 696e 6720  QLAlchemy using 
-000043f0: 7468 650a 2020 2020 2320 2761 7379 6e63  the.    # 'async
-00004400: 5f63 7265 6174 6f72 2720 6172 6775 6d65  _creator' argume
-00004410: 6e74 2074 6f20 2763 7265 6174 655f 6173  nt to 'create_as
-00004420: 796e 635f 656e 6769 6e65 270a 2020 2020  ync_engine'.    
-00004430: 706f 6f6c 203d 2063 7265 6174 655f 6173  pool = create_as
-00004440: 796e 635f 656e 6769 6e65 280a 2020 2020  ync_engine(.    
-00004450: 2020 2020 2270 6f73 7467 7265 7371 6c2b      "postgresql+
-00004460: 6173 796e 6370 673a 2f2f 222c 0a20 2020  asyncpg://",.   
-00004470: 2020 2020 2061 7379 6e63 5f63 7265 6174       async_creat
-00004480: 6f72 3d67 6574 636f 6e6e 2c0a 2020 2020  or=getconn,.    
-00004490: 290a 2020 2020 7265 7475 726e 2070 6f6f  ).    return poo
-000044a0: 6c0a 0a61 7379 6e63 2064 6566 206d 6169  l..async def mai
-000044b0: 6e28 293a 0a20 2020 2023 2069 6e69 7469  n():.    # initi
-000044c0: 616c 697a 6520 436f 6e6e 6563 746f 7220  alize Connector 
-000044d0: 6f62 6a65 6374 2066 6f72 2063 6f6e 6e65  object for conne
-000044e0: 6374 696f 6e73 2074 6f20 436c 6f75 6420  ctions to Cloud 
-000044f0: 5351 4c0a 2020 2020 636f 6e6e 6563 746f  SQL.    connecto
-00004500: 7220 3d20 6177 6169 7420 6372 6561 7465  r = await create
-00004510: 5f61 7379 6e63 5f63 6f6e 6e65 6374 6f72  _async_connector
-00004520: 2829 0a0a 2020 2020 2320 696e 6974 6961  ()..    # initia
-00004530: 6c69 7a65 2063 6f6e 6e65 6374 696f 6e20  lize connection 
-00004540: 706f 6f6c 0a20 2020 2070 6f6f 6c20 3d20  pool.    pool = 
-00004550: 6177 6169 7420 696e 6974 5f63 6f6e 6e65  await init_conne
-00004560: 6374 696f 6e5f 706f 6f6c 2863 6f6e 6e65  ction_pool(conne
-00004570: 6374 6f72 290a 0a20 2020 2023 2065 7861  ctor)..    # exa
-00004580: 6d70 6c65 2071 7565 7279 0a20 2020 2061  mple query.    a
-00004590: 7379 6e63 2077 6974 6820 706f 6f6c 2e63  sync with pool.c
-000045a0: 6f6e 6e65 6374 2829 2061 7320 636f 6e6e  onnect() as conn
-000045b0: 3a0a 2020 2020 2020 2020 6177 6169 7420  :.        await 
-000045c0: 636f 6e6e 2e65 7865 6375 7465 2873 716c  conn.execute(sql
-000045d0: 616c 6368 656d 792e 7465 7874 2822 5345  alchemy.text("SE
-000045e0: 4c45 4354 204e 4f57 2829 2229 290a 0a20  LECT NOW()")).. 
-000045f0: 2020 2023 2063 6c6f 7365 2043 6f6e 6e65     # close Conne
-00004600: 6374 6f72 0a20 2020 2061 7761 6974 2063  ctor.    await c
-00004610: 6f6e 6e65 6374 6f72 2e63 6c6f 7365 5f61  onnector.close_a
-00004620: 7379 6e63 2829 0a0a 2020 2020 2320 6469  sync()..    # di
-00004630: 7370 6f73 6520 6f66 2063 6f6e 6e65 6374  spose of connect
-00004640: 696f 6e20 706f 6f6c 0a20 2020 2061 7761  ion pool.    awa
-00004650: 6974 2070 6f6f 6c2e 6469 7370 6f73 6528  it pool.dispose(
-00004660: 290a 6060 600a 0a46 6f72 206d 6f72 6520  ).```..For more 
-00004670: 6465 7461 696c 7320 6f6e 2061 6464 6974  details on addit
-00004680: 696f 6e61 6c20 6461 7461 6261 7365 2061  ional database a
-00004690: 7267 756d 656e 7473 2077 6974 6820 616e  rguments with an
-000046a0: 2060 6173 796e 6370 672e 436f 6e6e 6563   `asyncpg.Connec
-000046b0: 7469 6f6e 600a 2c20 706c 6561 7365 2076  tion`., please v
-000046c0: 6973 6974 2074 6865 0a5b 6f66 6669 6369  isit the.[offici
-000046d0: 616c 2064 6f63 756d 656e 7461 7469 6f6e  al documentation
-000046e0: 5d28 6874 7470 733a 2f2f 6d61 6769 6373  ](https://magics
-000046f0: 7461 636b 2e67 6974 6875 622e 696f 2f61  tack.github.io/a
-00004700: 7379 6e63 7067 2f63 7572 7265 6e74 2f61  syncpg/current/a
-00004710: 7069 2f69 6e64 6578 2e68 746d 6c29 2e0a  pi/index.html)..
-00004720: 0a23 2323 2041 7379 6e63 2043 6f6e 7465  .### Async Conte
-00004730: 7874 204d 616e 6167 6572 0a0a 416e 2061  xt Manager..An a
-00004740: 6c74 6572 6e61 7469 7665 2074 6f20 7573  lternative to us
-00004750: 696e 6720 7468 6520 6063 7265 6174 655f  ing the `create_
-00004760: 6173 796e 635f 636f 6e6e 6563 746f 7260  async_connector`
-00004770: 2066 756e 6374 696f 6e20 6973 2069 6e69   function is ini
-00004780: 7469 616c 697a 696e 670a 6120 6043 6f6e  tializing.a `Con
-00004790: 6e65 6374 6f72 6020 6173 2061 6e20 6173  nector` as an as
-000047a0: 796e 6320 636f 6e74 6578 7420 6d61 6e61  ync context mana
-000047b0: 6765 722c 2072 656d 6f76 696e 6720 7468  ger, removing th
-000047c0: 6520 6e65 6564 2066 6f72 2065 7870 6c69  e need for expli
-000047d0: 6369 740a 6361 6c6c 7320 746f 2060 636f  cit.calls to `co
-000047e0: 6e6e 6563 746f 722e 636c 6f73 655f 6173  nnector.close_as
-000047f0: 796e 6328 2960 2074 6f20 636c 6561 6e75  ync()` to cleanu
-00004800: 7020 7265 736f 7572 6365 732e 0a0a 2a2a  p resources...**
-00004810: 4e6f 7465 3a2a 2a20 5468 6973 2061 6c74  Note:** This alt
-00004820: 6572 6e61 7469 7665 2072 6571 7569 7265  ernative require
-00004830: 7320 7468 6174 2074 6865 2072 756e 6e69  s that the runni
-00004840: 6e67 2065 7665 6e74 206c 6f6f 7020 6265  ng event loop be
-00004850: 0a70 6173 7365 6420 696e 2061 7320 7468  .passed in as th
-00004860: 6520 606c 6f6f 7060 2061 7267 756d 656e  e `loop` argumen
-00004870: 7420 746f 2060 436f 6e6e 6563 746f 7228  t to `Connector(
-00004880: 2960 2e0a 0a60 6060 7079 7468 6f6e 0a69  )`...```python.i
-00004890: 6d70 6f72 7420 6173 796e 6369 6f0a 696d  mport asyncio.im
-000048a0: 706f 7274 2061 7379 6e63 7067 0a0a 696d  port asyncpg..im
-000048b0: 706f 7274 2073 716c 616c 6368 656d 790a  port sqlalchemy.
-000048c0: 6672 6f6d 2073 716c 616c 6368 656d 792e  from sqlalchemy.
-000048d0: 6578 742e 6173 796e 6369 6f20 696d 706f  ext.asyncio impo
-000048e0: 7274 2041 7379 6e63 456e 6769 6e65 2c20  rt AsyncEngine, 
-000048f0: 6372 6561 7465 5f61 7379 6e63 5f65 6e67  create_async_eng
-00004900: 696e 650a 0a66 726f 6d20 676f 6f67 6c65  ine..from google
-00004910: 2e63 6c6f 7564 2e73 716c 2e63 6f6e 6e65  .cloud.sql.conne
-00004920: 6374 6f72 2069 6d70 6f72 7420 436f 6e6e  ctor import Conn
-00004930: 6563 746f 720a 0a61 7379 6e63 2064 6566  ector..async def
-00004940: 2069 6e69 745f 636f 6e6e 6563 7469 6f6e   init_connection
-00004950: 5f70 6f6f 6c28 636f 6e6e 6563 746f 723a  _pool(connector:
-00004960: 2043 6f6e 6e65 6374 6f72 2920 2d3e 2041   Connector) -> A
-00004970: 7379 6e63 456e 6769 6e65 3a0a 2020 2020  syncEngine:.    
-00004980: 2320 696e 6974 6961 6c69 7a65 2043 6f6e  # initialize Con
-00004990: 6e65 6374 6f72 206f 626a 6563 7420 666f  nector object fo
-000049a0: 7220 636f 6e6e 6563 7469 6f6e 7320 746f  r connections to
-000049b0: 2043 6c6f 7564 2053 514c 0a20 2020 2061   Cloud SQL.    a
-000049c0: 7379 6e63 2064 6566 2067 6574 636f 6e6e  sync def getconn
-000049d0: 2829 202d 3e20 6173 796e 6370 672e 436f  () -> asyncpg.Co
-000049e0: 6e6e 6563 7469 6f6e 3a0a 2020 2020 2020  nnection:.      
-000049f0: 2020 2020 2020 636f 6e6e 3a20 6173 796e        conn: asyn
-00004a00: 6370 672e 436f 6e6e 6563 7469 6f6e 203d  cpg.Connection =
-00004a10: 2061 7761 6974 2063 6f6e 6e65 6374 6f72   await connector
-00004a20: 2e63 6f6e 6e65 6374 5f61 7379 6e63 280a  .connect_async(.
-00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a40: 2270 726f 6a65 6374 3a72 6567 696f 6e3a  "project:region:
-00004a50: 696e 7374 616e 6365 222c 2020 2320 436c  instance",  # Cl
-00004a60: 6f75 6420 5351 4c20 696e 7374 616e 6365  oud SQL instance
-00004a70: 2063 6f6e 6e65 6374 696f 6e20 6e61 6d65   connection name
-00004a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004a90: 2022 6173 796e 6370 6722 2c0a 2020 2020   "asyncpg",.    
-00004aa0: 2020 2020 2020 2020 2020 2020 7573 6572              user
-00004ab0: 3d22 6d79 2d75 7365 7222 2c0a 2020 2020  ="my-user",.    
-00004ac0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00004ad0: 776f 7264 3d22 6d79 2d70 6173 7377 6f72  word="my-passwor
-00004ae0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
-00004af0: 2020 2020 6462 3d22 6d79 2d64 622d 6e61      db="my-db-na
-00004b00: 6d65 220a 2020 2020 2020 2020 2020 2020  me".            
-00004b10: 2020 2020 2320 2e2e 2e20 6164 6469 7469      # ... additi
-00004b20: 6f6e 616c 2064 6174 6162 6173 6520 6472  onal database dr
-00004b30: 6976 6572 2061 7267 730a 2020 2020 2020  iver args.      
-00004b40: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00004b50: 2020 2020 7265 7475 726e 2063 6f6e 6e0a      return conn.
-00004b60: 0a20 2020 2023 2054 6865 2043 6c6f 7564  .    # The Cloud
-00004b70: 2053 514c 2050 7974 686f 6e20 436f 6e6e   SQL Python Conn
-00004b80: 6563 746f 7220 6361 6e20 6265 2075 7365  ector can be use
-00004b90: 6420 616c 6f6e 6720 7769 7468 2053 514c  d along with SQL
-00004ba0: 416c 6368 656d 7920 7573 696e 6720 7468  Alchemy using th
-00004bb0: 650a 2020 2020 2320 2761 7379 6e63 5f63  e.    # 'async_c
-00004bc0: 7265 6174 6f72 2720 6172 6775 6d65 6e74  reator' argument
-00004bd0: 2074 6f20 2763 7265 6174 655f 6173 796e   to 'create_asyn
-00004be0: 635f 656e 6769 6e65 270a 2020 2020 706f  c_engine'.    po
-00004bf0: 6f6c 203d 2063 7265 6174 655f 6173 796e  ol = create_asyn
-00004c00: 635f 656e 6769 6e65 280a 2020 2020 2020  c_engine(.      
-00004c10: 2020 2270 6f73 7467 7265 7371 6c2b 6173    "postgresql+as
-00004c20: 796e 6370 673a 2f2f 222c 0a20 2020 2020  yncpg://",.     
-00004c30: 2020 2061 7379 6e63 5f63 7265 6174 6f72     async_creator
-00004c40: 3d67 6574 636f 6e6e 2c0a 2020 2020 290a  =getconn,.    ).
-00004c50: 2020 2020 7265 7475 726e 2070 6f6f 6c0a      return pool.
-00004c60: 0a61 7379 6e63 2064 6566 206d 6169 6e28  .async def main(
-00004c70: 293a 0a20 2020 2023 2069 6e69 7469 616c  ):.    # initial
-00004c80: 697a 6520 436f 6e6e 6563 746f 7220 6f62  ize Connector ob
-00004c90: 6a65 6374 2066 6f72 2063 6f6e 6e65 6374  ject for connect
-00004ca0: 696f 6e73 2074 6f20 436c 6f75 6420 5351  ions to Cloud SQ
-00004cb0: 4c0a 2020 2020 6c6f 6f70 203d 2061 7379  L.    loop = asy
-00004cc0: 6e63 696f 2e67 6574 5f72 756e 6e69 6e67  ncio.get_running
-00004cd0: 5f6c 6f6f 7028 290a 2020 2020 6173 796e  _loop().    asyn
-00004ce0: 6320 7769 7468 2043 6f6e 6e65 6374 6f72  c with Connector
-00004cf0: 286c 6f6f 703d 6c6f 6f70 2920 6173 2063  (loop=loop) as c
-00004d00: 6f6e 6e65 6374 6f72 3a0a 2020 2020 2020  onnector:.      
-00004d10: 2020 2320 696e 6974 6961 6c69 7a65 2063    # initialize c
-00004d20: 6f6e 6e65 6374 696f 6e20 706f 6f6c 0a20  onnection pool. 
-00004d30: 2020 2020 2020 2070 6f6f 6c20 3d20 6177         pool = aw
-00004d40: 6169 7420 696e 6974 5f63 6f6e 6e65 6374  ait init_connect
-00004d50: 696f 6e5f 706f 6f6c 2863 6f6e 6e65 6374  ion_pool(connect
-00004d60: 6f72 290a 0a20 2020 2020 2020 2023 2065  or)..        # e
-00004d70: 7861 6d70 6c65 2071 7565 7279 0a20 2020  xample query.   
-00004d80: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
-00004d90: 706f 6f6c 2e63 6f6e 6e65 6374 2829 2061  pool.connect() a
-00004da0: 7320 636f 6e6e 3a0a 2020 2020 2020 2020  s conn:.        
-00004db0: 2020 2020 6177 6169 7420 636f 6e6e 2e65      await conn.e
-00004dc0: 7865 6375 7465 2873 716c 616c 6368 656d  xecute(sqlalchem
-00004dd0: 792e 7465 7874 2822 5345 4c45 4354 204e  y.text("SELECT N
-00004de0: 4f57 2829 2229 290a 0a20 2020 2020 2020  OW()"))..       
-00004df0: 2023 2064 6973 706f 7365 206f 6620 636f   # dispose of co
-00004e00: 6e6e 6563 7469 6f6e 2070 6f6f 6c0a 2020  nnection pool.  
-00004e10: 2020 2020 2020 6177 6169 7420 706f 6f6c        await pool
-00004e20: 2e64 6973 706f 7365 2829 0a60 6060 0a0a  .dispose().```..
-00004e30: 2323 2053 7570 706f 7274 2070 6f6c 6963  ## Support polic
-00004e40: 790a 0a23 2323 204d 616a 6f72 2076 6572  y..### Major ver
-00004e50: 7369 6f6e 206c 6966 6563 7963 6c65 0a0a  sion lifecycle..
-00004e60: 5468 6973 2070 726f 6a65 6374 2075 7365  This project use
-00004e70: 7320 5b73 656d 616e 7469 6320 7665 7273  s [semantic vers
-00004e80: 696f 6e69 6e67 5d28 6874 7470 733a 2f2f  ioning](https://
-00004e90: 7365 6d76 6572 2e6f 7267 2f29 2c20 616e  semver.org/), an
-00004ea0: 6420 7573 6573 2074 6865 0a66 6f6c 6c6f  d uses the.follo
-00004eb0: 7769 6e67 206c 6966 6563 7963 6c65 2072  wing lifecycle r
-00004ec0: 6567 6172 6469 6e67 2073 7570 706f 7274  egarding support
-00004ed0: 2066 6f72 2061 206d 616a 6f72 2076 6572   for a major ver
-00004ee0: 7369 6f6e 3a0a 0a2a 2a41 6374 6976 652a  sion:..**Active*
-00004ef0: 2a20 2d20 4163 7469 7665 2076 6572 7369  * - Active versi
-00004f00: 6f6e 7320 6765 7420 616c 6c20 6e65 7720  ons get all new 
-00004f10: 6665 6174 7572 6573 2061 6e64 2073 6563  features and sec
-00004f20: 7572 6974 7920 6669 7865 7320 2874 6861  urity fixes (tha
-00004f30: 740a 776f 756c 646e e280 9974 206f 7468  t.wouldn...t oth
-00004f40: 6572 7769 7365 2069 6e74 726f 6475 6365  erwise introduce
-00004f50: 2061 2062 7265 616b 696e 6720 6368 616e   a breaking chan
-00004f60: 6765 292e 204e 6577 206d 616a 6f72 2076  ge). New major v
-00004f70: 6572 7369 6f6e 7320 6172 650a 6775 6172  ersions are.guar
-00004f80: 616e 7465 6564 2074 6f20 6265 2022 6163  anteed to be "ac
-00004f90: 7469 7665 2220 666f 7220 6120 6d69 6e69  tive" for a mini
-00004fa0: 6d75 6d20 6f66 2031 2079 6561 722e 0a2a  mum of 1 year..*
-00004fb0: 2a44 6570 7265 6361 7465 642a 2a20 2d20  *Deprecated** - 
-00004fc0: 4465 7072 6563 6174 6564 2076 6572 7369  Deprecated versi
-00004fd0: 6f6e 7320 636f 6e74 696e 7565 2074 6f20  ons continue to 
-00004fe0: 7265 6365 6976 6520 7365 6375 7269 7479  receive security
-00004ff0: 2061 6e64 2063 7269 7469 6361 6c0a 6275   and critical.bu
-00005000: 6720 6669 7865 732c 2062 7574 2064 6f20  g fixes, but do 
-00005010: 6e6f 7420 7265 6365 6976 6520 6e65 7720  not receive new 
-00005020: 6665 6174 7572 6573 2e20 4465 7072 6563  features. Deprec
-00005030: 6174 6564 2076 6572 7369 6f6e 7320 7769  ated versions wi
-00005040: 6c6c 2062 6520 7075 626c 6963 6c79 0a73  ll be publicly.s
-00005050: 7570 706f 7274 6564 2066 6f72 2031 2079  upported for 1 y
-00005060: 6561 722e 0a2a 2a55 6e73 7570 706f 7274  ear..**Unsupport
-00005070: 6564 2a2a 202d 2041 6e79 206d 616a 6f72  ed** - Any major
-00005080: 2076 6572 7369 6f6e 2074 6861 7420 6861   version that ha
-00005090: 7320 6265 656e 2064 6570 7265 6361 7465  s been deprecate
-000050a0: 6420 666f 7220 3e3d 3120 7965 6172 2069  d for >=1 year i
-000050b0: 730a 636f 6e73 6964 6572 6564 2070 7562  s.considered pub
-000050c0: 6c69 636c 7920 756e 7375 7070 6f72 7465  licly unsupporte
-000050d0: 642e 0a0a 2323 2053 7570 706f 7274 6564  d...## Supported
-000050e0: 2050 7974 686f 6e20 5665 7273 696f 6e73   Python Versions
-000050f0: 0a0a 5765 2074 6573 7420 616e 6420 7375  ..We test and su
-00005100: 7070 6f72 7420 6174 2061 206d 696e 696d  pport at a minim
-00005110: 756d 2c20 6576 6572 7920 5b61 6374 6976  um, every [activ
-00005120: 6520 7665 7273 696f 6e20 756e 7469 6c20  e version until 
-00005130: 6974 2773 0a65 6e64 2d6f 662d 6c69 6665  it's.end-of-life
-00005140: 2064 6174 655d 5b70 7976 6572 5d2e 2043   date][pyver]. C
-00005150: 6861 6e67 6573 2069 6e20 7375 7070 6f72  hanges in suppor
-00005160: 7465 6420 5079 7468 6f6e 2076 6572 7369  ted Python versi
-00005170: 6f6e 7320 7769 6c6c 2062 650a 636f 6e73  ons will be.cons
-00005180: 6964 6572 6564 2061 206d 696e 6f72 2063  idered a minor c
-00005190: 6861 6e67 652c 2061 6e64 2077 696c 6c20  hange, and will 
-000051a0: 6265 206c 6973 7465 6420 696e 2074 6865  be listed in the
-000051b0: 2072 656c 6561 7365 206e 6f74 6573 2e0a   release notes..
-000051c0: 0a5b 7079 7665 725d 3a20 6874 7470 733a  .[pyver]: https:
-000051d0: 2f2f 6465 7667 7569 6465 2e70 7974 686f  //devguide.pytho
-000051e0: 6e2e 6f72 672f 2373 7461 7475 732d 6f66  n.org/#status-of
-000051f0: 2d70 7974 686f 6e2d 6272 616e 6368 6573  -python-branches
-00005200: 0a0a 2323 2320 5265 6c65 6173 6520 6361  ..### Release ca
-00005210: 6465 6e63 650a 5468 6973 2070 726f 6a65  dence.This proje
-00005220: 6374 2061 696d 7320 666f 7220 6120 6d69  ct aims for a mi
-00005230: 6e69 6d75 6d20 6d6f 6e74 686c 7920 7265  nimum monthly re
-00005240: 6c65 6173 6520 6361 6465 6e63 652e 2049  lease cadence. I
-00005250: 6620 6e6f 206e 6577 0a66 6561 7475 7265  f no new.feature
-00005260: 7320 6f72 2066 6978 6573 2068 6176 6520  s or fixes have 
-00005270: 6265 656e 2061 6464 6564 2c20 6120 6e65  been added, a ne
-00005280: 7720 5041 5443 4820 7665 7273 696f 6e20  w PATCH version 
-00005290: 7769 7468 2074 6865 206c 6174 6573 740a  with the latest.
-000052a0: 6465 7065 6e64 656e 6369 6573 2069 7320  dependencies is 
-000052b0: 7265 6c65 6173 6564 2e0a 0a23 2323 2043  released...### C
-000052c0: 6f6e 7472 6962 7574 696e 670a 0a57 6520  ontributing..We 
-000052d0: 7765 6c63 6f6d 6520 6f75 7473 6964 6520  welcome outside 
-000052e0: 636f 6e74 7269 6275 7469 6f6e 732e 2050  contributions. P
-000052f0: 6c65 6173 6520 7365 6520 6f75 720a 5b43  lease see our.[C
-00005300: 6f6e 7472 6962 7574 696e 6720 4775 6964  ontributing Guid
-00005310: 655d 2843 4f4e 5452 4942 5554 494e 472e  e](CONTRIBUTING.
-00005320: 6d64 2920 666f 7220 6465 7461 696c 7320  md) for details 
-00005330: 6f6e 2068 6f77 2062 6573 7420 746f 2063  on how best to c
-00005340: 6f6e 7472 6962 7574 652e 0a              ontribute..
+00000600: 6964 6573 2061 206e 6174 6976 6520 616c  ides a native al
+00000610: 7465 726e 6174 6976 6520 746f 2074 6865  ternative to the
+00000620: 0a5b 436c 6f75 6420 5351 4c20 4175 7468  .[Cloud SQL Auth
+00000630: 2050 726f 7879 5d28 6874 7470 733a 2f2f   Proxy](https://
+00000640: 636c 6f75 642e 676f 6f67 6c65 2e63 6f6d  cloud.google.com
+00000650: 2f73 716c 2f64 6f63 732f 6d79 7371 6c2f  /sql/docs/mysql/
+00000660: 7371 6c2d 7072 6f78 7929 2077 6869 6c65  sql-proxy) while
+00000670: 0a70 726f 7669 6469 6e67 2074 6865 2066  .providing the f
+00000680: 6f6c 6c6f 7769 6e67 2062 656e 6566 6974  ollowing benefit
+00000690: 733a 0a0a 2a20 2a2a 4941 4d20 4175 7468  s:..* **IAM Auth
+000006a0: 6f72 697a 6174 696f 6e3a 2a2a 2075 7365  orization:** use
+000006b0: 7320 4941 4d20 7065 726d 6973 7369 6f6e  s IAM permission
+000006c0: 7320 746f 2063 6f6e 7472 6f6c 2077 686f  s to control who
+000006d0: 2f77 6861 7420 6361 6e20 636f 6e6e 6563  /what can connec
+000006e0: 7420 746f 0a20 2079 6f75 7220 436c 6f75  t to.  your Clou
+000006f0: 6420 5351 4c20 696e 7374 616e 6365 730a  d SQL instances.
+00000700: 2a20 2a2a 496d 7072 6f76 6564 2053 6563  * **Improved Sec
+00000710: 7572 6974 793a 2a2a 2075 7365 7320 726f  urity:** uses ro
+00000720: 6275 7374 2c20 7570 6461 7465 6420 544c  bust, updated TL
+00000730: 5320 312e 3320 656e 6372 7970 7469 6f6e  S 1.3 encryption
+00000740: 2061 6e64 0a20 2069 6465 6e74 6974 7920   and.  identity 
+00000750: 7665 7269 6669 6361 7469 6f6e 2062 6574  verification bet
+00000760: 7765 656e 2074 6865 2063 6c69 656e 7420  ween the client 
+00000770: 636f 6e6e 6563 746f 7220 616e 6420 7468  connector and th
+00000780: 6520 7365 7276 6572 2d73 6964 6520 7072  e server-side pr
+00000790: 6f78 792c 0a20 2069 6e64 6570 656e 6465  oxy,.  independe
+000007a0: 6e74 206f 6620 7468 6520 6461 7461 6261  nt of the databa
+000007b0: 7365 2070 726f 746f 636f 6c2e 0a2a 202a  se protocol..* *
+000007c0: 2a43 6f6e 7665 6e69 656e 6365 3a2a 2a20  *Convenience:** 
+000007d0: 7265 6d6f 7665 7320 7468 6520 7265 7175  removes the requ
+000007e0: 6972 656d 656e 7420 746f 2075 7365 2061  irement to use a
+000007f0: 6e64 2064 6973 7472 6962 7574 6520 5353  nd distribute SS
+00000800: 4c0a 2020 6365 7274 6966 6963 6174 6573  L.  certificates
+00000810: 2c20 6173 2077 656c 6c20 6173 206d 616e  , as well as man
+00000820: 6167 6520 6669 7265 7761 6c6c 7320 6f72  age firewalls or
+00000830: 2073 6f75 7263 652f 6465 7374 696e 6174   source/destinat
+00000840: 696f 6e20 4950 2061 6464 7265 7373 6573  ion IP addresses
+00000850: 2e0a 2a20 286f 7074 696f 6e61 6c6c 7929  ..* (optionally)
+00000860: 202a 2a49 414d 2044 4220 4175 7468 656e   **IAM DB Authen
+00000870: 7469 6361 7469 6f6e 3a2a 2a20 7072 6f76  tication:** prov
+00000880: 6964 6573 2073 7570 706f 7274 2066 6f72  ides support for
+00000890: 0a20 205b 436c 6f75 6420 5351 4ce2 8099  .  [Cloud SQL...
+000008a0: 7320 6175 746f 6d61 7469 6320 4941 4d20  s automatic IAM 
+000008b0: 4442 2041 7574 684e 5d5b 6961 6d2d 6462  DB AuthN][iam-db
+000008c0: 2d61 7574 686e 5d20 6665 6174 7572 652e  -authn] feature.
+000008d0: 0a0a 5b69 616d 2d64 622d 6175 7468 6e5d  ..[iam-db-authn]
+000008e0: 3a20 6874 7470 733a 2f2f 636c 6f75 642e  : https://cloud.
+000008f0: 676f 6f67 6c65 2e63 6f6d 2f73 716c 2f64  google.com/sql/d
+00000900: 6f63 732f 706f 7374 6772 6573 2f61 7574  ocs/postgres/aut
+00000910: 6865 6e74 6963 6174 696f 6e0a 0a54 6865  hentication..The
+00000920: 2043 6c6f 7564 2053 514c 2050 7974 686f   Cloud SQL Pytho
+00000930: 6e20 436f 6e6e 6563 746f 7220 6973 2061  n Connector is a
+00000940: 2070 6163 6b61 6765 2074 6f20 6265 2075   package to be u
+00000950: 7365 6420 616c 6f6e 6773 6964 6520 6120  sed alongside a 
+00000960: 6461 7461 6261 7365 2064 7269 7665 722e  database driver.
+00000970: 0a43 7572 7265 6e74 6c79 2073 7570 706f  .Currently suppo
+00000980: 7274 6564 2064 7269 7665 7273 2061 7265  rted drivers are
+00000990: 3a0a 202d 205b 6070 796d 7973 716c 605d  :. - [`pymysql`]
+000009a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000009b0: 636f 6d2f 5079 4d79 5351 4c2f 5079 4d79  com/PyMySQL/PyMy
+000009c0: 5351 4c29 2028 4d79 5351 4c29 0a20 2d20  SQL) (MySQL). - 
+000009d0: 5b60 7067 3830 3030 605d 2868 7474 7073  [`pg8000`](https
+000009e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 746c  ://github.com/tl
+000009f0: 6f63 6b65 2f70 6738 3030 3029 2028 506f  ocke/pg8000) (Po
+00000a00: 7374 6772 6553 514c 290a 202d 205b 6061  stgreSQL). - [`a
+00000a10: 7379 6e63 7067 605d 2868 7474 7073 3a2f  syncpg`](https:/
+00000a20: 2f67 6974 6875 622e 636f 6d2f 4d61 6769  /github.com/Magi
+00000a30: 6353 7461 636b 2f61 7379 6e63 7067 2920  cStack/asyncpg) 
+00000a40: 2850 6f73 7467 7265 5351 4c29 0a20 2d20  (PostgreSQL). - 
+00000a50: 5b60 7079 7464 7360 5d28 6874 7470 733a  [`pytds`](https:
+00000a60: 2f2f 6769 7468 7562 2e63 6f6d 2f64 656e  //github.com/den
+00000a70: 6973 656e 6b6f 6d2f 7079 7464 7329 2028  isenkom/pytds) (
+00000a80: 5351 4c20 5365 7276 6572 290a 0a0a 2323  SQL Server)...##
+00000a90: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a59   Installation..Y
+00000aa0: 6f75 2063 616e 2069 6e73 7461 6c6c 2074  ou can install t
+00000ab0: 6869 7320 6c69 6272 6172 7920 7769 7468  his library with
+00000ac0: 2060 7069 7020 696e 7374 616c 6c60 2c20   `pip install`, 
+00000ad0: 7370 6563 6966 7969 6e67 2074 6865 2064  specifying the d
+00000ae0: 7269 7665 720a 6261 7365 6420 6f6e 2079  river.based on y
+00000af0: 6f75 7220 6461 7461 6261 7365 2064 6961  our database dia
+00000b00: 6c65 6374 2e0a 0a23 2323 204d 7953 514c  lect...### MySQL
+00000b10: 0a60 6060 0a70 6970 2069 6e73 7461 6c6c  .```.pip install
+00000b20: 2022 636c 6f75 642d 7371 6c2d 7079 7468   "cloud-sql-pyth
+00000b30: 6f6e 2d63 6f6e 6e65 6374 6f72 5b70 796d  on-connector[pym
+00000b40: 7973 716c 5d22 0a60 6060 0a23 2323 2050  ysql]".```.### P
+00000b50: 6f73 7467 7265 730a 5468 6572 6520 6172  ostgres.There ar
+00000b60: 6520 7477 6f20 6469 6666 6572 656e 7420  e two different 
+00000b70: 6461 7461 6261 7365 2064 7269 7665 7273  database drivers
+00000b80: 2074 6861 7420 6172 6520 7375 7070 6f72   that are suppor
+00000b90: 7465 6420 666f 7220 7468 6520 506f 7374  ted for the Post
+00000ba0: 6772 6573 2064 6961 6c65 6374 3a0a 0a23  gres dialect:..#
+00000bb0: 2323 2320 7067 3830 3030 0a60 6060 0a70  ### pg8000.```.p
+00000bc0: 6970 2069 6e73 7461 6c6c 2022 636c 6f75  ip install "clou
+00000bd0: 642d 7371 6c2d 7079 7468 6f6e 2d63 6f6e  d-sql-python-con
+00000be0: 6e65 6374 6f72 5b70 6738 3030 305d 220a  nector[pg8000]".
+00000bf0: 6060 600a 2323 2323 2061 7379 6e63 7067  ```.#### asyncpg
+00000c00: 0a60 6060 0a70 6970 2069 6e73 7461 6c6c  .```.pip install
+00000c10: 2022 636c 6f75 642d 7371 6c2d 7079 7468   "cloud-sql-pyth
+00000c20: 6f6e 2d63 6f6e 6e65 6374 6f72 5b61 7379  on-connector[asy
+00000c30: 6e63 7067 5d22 0a60 6060 0a23 2323 2053  ncpg]".```.### S
+00000c40: 514c 2053 6572 7665 720a 6060 600a 7069  QL Server.```.pi
+00000c50: 7020 696e 7374 616c 6c20 2263 6c6f 7564  p install "cloud
+00000c60: 2d73 716c 2d70 7974 686f 6e2d 636f 6e6e  -sql-python-conn
+00000c70: 6563 746f 725b 7079 7464 735d 220a 6060  ector[pytds]".``
+00000c80: 600a 2323 2055 7361 6765 0a0a 5468 6973  `.## Usage..This
+00000c90: 2070 6163 6b61 6765 2070 726f 7669 6465   package provide
+00000ca0: 7320 7365 7665 7261 6c20 6675 6e63 7469  s several functi
+00000cb0: 6f6e 7320 666f 7220 6175 7468 6f72 697a  ons for authoriz
+00000cc0: 696e 6720 616e 6420 656e 6372 7970 7469  ing and encrypti
+00000cd0: 6e67 0a63 6f6e 6e65 6374 696f 6e73 2e20  ng.connections. 
+00000ce0: 5468 6573 6520 6675 6e63 7469 6f6e 7320  These functions 
+00000cf0: 6172 6520 7573 6564 2077 6974 6820 796f  are used with yo
+00000d00: 7572 2064 6174 6162 6173 6520 6472 6976  ur database driv
+00000d10: 6572 2074 6f20 636f 6e6e 6563 7420 746f  er to connect to
+00000d20: 0a79 6f75 7220 436c 6f75 6420 5351 4c20  .your Cloud SQL 
+00000d30: 696e 7374 616e 6365 2e0a 0a54 6865 2069  instance...The i
+00000d40: 6e73 7461 6e63 6520 636f 6e6e 6563 7469  nstance connecti
+00000d50: 6f6e 206e 616d 6520 666f 7220 796f 7572  on name for your
+00000d60: 2043 6c6f 7564 2053 514c 2069 6e73 7461   Cloud SQL insta
+00000d70: 6e63 6520 6973 2061 6c77 6179 7320 696e  nce is always in
+00000d80: 2074 6865 0a66 6f72 6d61 7420 2270 726f   the.format "pro
+00000d90: 6a65 6374 3a72 6567 696f 6e3a 696e 7374  ject:region:inst
+00000da0: 616e 6365 222e 0a0a 2323 2320 4150 4973  ance"...### APIs
+00000db0: 2061 6e64 2053 6572 7669 6365 730a 0a54   and Services..T
+00000dc0: 6869 7320 7061 636b 6167 6520 7265 7175  his package requ
+00000dd0: 6972 6573 2074 6865 2066 6f6c 6c6f 7769  ires the followi
+00000de0: 6e67 2074 6f20 7375 6363 6573 7366 756c  ng to successful
+00000df0: 6c79 206d 616b 6520 436c 6f75 6420 5351  ly make Cloud SQ
+00000e00: 4c20 436f 6e6e 6563 7469 6f6e 733a 0a0a  L Connections:..
+00000e10: 2d20 4941 4d20 7072 696e 6369 7061 6c20  - IAM principal 
+00000e20: 2875 7365 722c 2073 6572 7669 6365 2061  (user, service a
+00000e30: 6363 6f75 6e74 2c20 6574 632e 2920 7769  ccount, etc.) wi
+00000e40: 7468 2074 6865 0a5b 436c 6f75 6420 5351  th the.[Cloud SQ
+00000e50: 4c20 436c 6965 6e74 5d5b 636c 6965 6e74  L Client][client
+00000e60: 2d72 6f6c 655d 2072 6f6c 652e 2054 6869  -role] role. Thi
+00000e70: 7320 4941 4d20 7072 696e 6369 7061 6c20  s IAM principal 
+00000e80: 7769 6c6c 2062 6520 7573 6564 2066 6f72  will be used for
+00000e90: 0a5b 6372 6564 656e 7469 616c 735d 2823  .[credentials](#
+00000ea0: 6372 6564 656e 7469 616c 7329 2e0a 2d20  credentials)..- 
+00000eb0: 5468 6520 5b43 6c6f 7564 2053 514c 2041  The [Cloud SQL A
+00000ec0: 646d 696e 2041 5049 5d5b 6164 6d69 6e2d  dmin API][admin-
+00000ed0: 6170 695d 2074 6f20 6265 2065 6e61 626c  api] to be enabl
+00000ee0: 6564 2077 6974 6869 6e20 796f 7572 2047  ed within your G
+00000ef0: 6f6f 676c 6520 436c 6f75 640a 5072 6f6a  oogle Cloud.Proj
+00000f00: 6563 742e 2042 7920 6465 6661 756c 742c  ect. By default,
+00000f10: 2074 6865 2041 5049 2077 696c 6c20 6265   the API will be
+00000f20: 2063 616c 6c65 6420 696e 2074 6865 2070   called in the p
+00000f30: 726f 6a65 6374 2061 7373 6f63 6961 7465  roject associate
+00000f40: 6420 7769 7468 0a74 6865 2049 414d 2070  d with.the IAM p
+00000f50: 7269 6e63 6970 616c 2e0a 0a5b 6164 6d69  rincipal...[admi
+00000f60: 6e2d 6170 695d 3a20 6874 7470 733a 2f2f  n-api]: https://
+00000f70: 636f 6e73 6f6c 652e 636c 6f75 642e 676f  console.cloud.go
+00000f80: 6f67 6c65 2e63 6f6d 2f61 7069 732f 6170  ogle.com/apis/ap
+00000f90: 692f 7371 6c61 646d 696e 2e67 6f6f 676c  i/sqladmin.googl
+00000fa0: 6561 7069 732e 636f 6d0a 5b63 6c69 656e  eapis.com.[clien
+00000fb0: 742d 726f 6c65 5d3a 2068 7474 7073 3a2f  t-role]: https:/
+00000fc0: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
+00000fd0: 6d2f 7371 6c2f 646f 6373 2f6d 7973 716c  m/sql/docs/mysql
+00000fe0: 2f72 6f6c 6573 2d61 6e64 2d70 6572 6d69  /roles-and-permi
+00000ff0: 7373 696f 6e73 0a0a 2323 2320 4372 6564  ssions..### Cred
+00001000: 656e 7469 616c 730a 0a54 6869 7320 6c69  entials..This li
+00001010: 6272 6172 7920 7573 6573 2074 6865 205b  brary uses the [
+00001020: 4170 706c 6963 6174 696f 6e20 4465 6661  Application Defa
+00001030: 756c 7420 4372 6564 656e 7469 616c 7320  ult Credentials 
+00001040: 2841 4443 295d 5b61 6463 5d20 7374 7261  (ADC)][adc] stra
+00001050: 7465 6779 2066 6f72 0a72 6573 6f6c 7669  tegy for.resolvi
+00001060: 6e67 2063 7265 6465 6e74 6961 6c73 2e20  ng credentials. 
+00001070: 506c 6561 7365 2073 6565 205b 7468 6573  Please see [thes
+00001080: 6520 696e 7374 7275 6374 696f 6e73 2066  e instructions f
+00001090: 6f72 2068 6f77 2074 6f20 7365 7420 796f  or how to set yo
+000010a0: 7572 2041 4443 5d5b 7365 742d 6164 635d  ur ADC][set-adc]
+000010b0: 0a28 476f 6f67 6c65 2043 6c6f 7564 2041  .(Google Cloud A
+000010c0: 7070 6c69 6361 7469 6f6e 2076 7320 4c6f  pplication vs Lo
+000010d0: 6361 6c20 4465 7665 6c6f 706d 656e 742c  cal Development,
+000010e0: 2049 414d 2075 7365 7220 7673 2073 6572   IAM user vs ser
+000010f0: 7669 6365 2061 6363 6f75 6e74 2063 7265  vice account cre
+00001100: 6465 6e74 6961 6c73 292c 0a6f 7220 636f  dentials),.or co
+00001110: 6e73 756c 7420 7468 6520 5b67 6f6f 676c  nsult the [googl
+00001120: 652e 6175 7468 5d5b 676f 6f67 6c65 2d61  e.auth][google-a
+00001130: 7574 685d 2070 6163 6b61 6765 2e0a 0a54  uth] package...T
+00001140: 6f20 6578 706c 6963 6974 6c79 2073 6574  o explicitly set
+00001150: 2061 2073 7065 6369 6669 6320 736f 7572   a specific sour
+00001160: 6365 2066 6f72 2074 6865 2063 7265 6465  ce for the crede
+00001170: 6e74 6961 6c73 2c20 7365 650a 5b43 6f6e  ntials, see.[Con
+00001180: 6669 6775 7269 6e67 2074 6865 2043 6f6e  figuring the Con
+00001190: 6e65 6374 6f72 5d28 2363 6f6e 6669 6775  nector](#configu
+000011a0: 7269 6e67 2d74 6865 2d63 6f6e 6e65 6374  ring-the-connect
+000011b0: 6f72 2920 6265 6c6f 772e 0a0a 5b61 6463  or) below...[adc
+000011c0: 5d3a 2068 7474 7073 3a2f 2f63 6c6f 7564  ]: https://cloud
+000011d0: 2e67 6f6f 676c 652e 636f 6d2f 646f 6373  .google.com/docs
+000011e0: 2f61 7574 6865 6e74 6963 6174 696f 6e23  /authentication#
+000011f0: 6164 630a 5b73 6574 2d61 6463 5d3a 2068  adc.[set-adc]: h
+00001200: 7474 7073 3a2f 2f63 6c6f 7564 2e67 6f6f  ttps://cloud.goo
+00001210: 676c 652e 636f 6d2f 646f 6373 2f61 7574  gle.com/docs/aut
+00001220: 6865 6e74 6963 6174 696f 6e2f 7072 6f76  hentication/prov
+00001230: 6964 652d 6372 6564 656e 7469 616c 732d  ide-credentials-
+00001240: 6164 630a 5b67 6f6f 676c 652d 6175 7468  adc.[google-auth
+00001250: 5d3a 2068 7474 7073 3a2f 2f67 6f6f 676c  ]: https://googl
+00001260: 652d 6175 7468 2e72 6561 6474 6865 646f  e-auth.readthedo
+00001270: 6373 2e69 6f2f 656e 2f6d 6173 7465 722f  cs.io/en/master/
+00001280: 7265 6665 7265 6e63 652f 676f 6f67 6c65  reference/google
+00001290: 2e61 7574 682e 6874 6d6c 0a0a 2323 2320  .auth.html..### 
+000012a0: 486f 7720 746f 2075 7365 2074 6869 7320  How to use this 
+000012b0: 436f 6e6e 6563 746f 720a 0a54 6f20 636f  Connector..To co
+000012c0: 6e6e 6563 7420 746f 2043 6c6f 7564 2053  nnect to Cloud S
+000012d0: 514c 2075 7369 6e67 2074 6865 2063 6f6e  QL using the con
+000012e0: 6e65 6374 6f72 2c20 696e 6974 6974 616c  nector, initital
+000012f0: 697a 6520 6120 6043 6f6e 6e65 6374 6f72  ize a `Connector
+00001300: 600a 6f62 6a65 6374 2061 6e64 2063 616c  `.object and cal
+00001310: 6c20 6974 2773 2060 636f 6e6e 6563 7460  l it's `connect`
+00001320: 206d 6574 686f 6420 7769 7468 2074 6865   method with the
+00001330: 2070 726f 7065 7220 696e 7075 7420 7061   proper input pa
+00001340: 7261 6d65 7465 7273 2e0a 0a54 6865 2060  rameters...The `
+00001350: 436f 6e6e 6563 746f 7260 2069 7473 656c  Connector` itsel
+00001360: 6620 6372 6561 7465 7320 636f 6e6e 6563  f creates connec
+00001370: 7469 6f6e 206f 626a 6563 7473 2062 7920  tion objects by 
+00001380: 6361 6c6c 696e 6720 6974 7320 6063 6f6e  calling its `con
+00001390: 6e65 6374 6020 6d65 7468 6f64 2062 7574  nect` method but
+000013a0: 2064 6f65 7320 6e6f 7420 6d61 6e61 6765   does not manage
+000013b0: 2064 6174 6162 6173 6520 636f 6e6e 6563   database connec
+000013c0: 7469 6f6e 2070 6f6f 6c69 6e67 2e20 466f  tion pooling. Fo
+000013d0: 7220 7468 6973 2072 6561 736f 6e2c 2069  r this reason, i
+000013e0: 7420 6973 2072 6563 6f6d 6d65 6e64 6564  t is recommended
+000013f0: 2074 6f20 7573 6520 7468 6520 636f 6e6e   to use the conn
+00001400: 6563 746f 7220 616c 6f6e 6773 6964 6520  ector alongside 
+00001410: 6120 6c69 6272 6172 7920 7468 6174 2063  a library that c
+00001420: 616e 2063 7265 6174 6520 636f 6e6e 6563  an create connec
+00001430: 7469 6f6e 2070 6f6f 6c73 2c20 7375 6368  tion pools, such
+00001440: 2061 7320 5b53 514c 416c 6368 656d 795d   as [SQLAlchemy]
+00001450: 2868 7474 7073 3a2f 2f77 7777 2e73 716c  (https://www.sql
+00001460: 616c 6368 656d 792e 6f72 672f 292e 2054  alchemy.org/). T
+00001470: 6869 7320 7769 6c6c 2061 6c6c 6f77 2066  his will allow f
+00001480: 6f72 2063 6f6e 6e65 6374 696f 6e73 2074  or connections t
+00001490: 6f20 7265 6d61 696e 206f 7065 6e20 616e  o remain open an
+000014a0: 6420 6265 2072 6575 7365 642c 2072 6564  d be reused, red
+000014b0: 7563 696e 6720 636f 6e6e 6563 7469 6f6e  ucing connection
+000014c0: 206f 7665 7268 6561 6420 616e 6420 7468   overhead and th
+000014d0: 6520 6e75 6d62 6572 206f 6620 636f 6e6e  e number of conn
+000014e0: 6563 7469 6f6e 7320 6e65 6564 6564 2e0a  ections needed..
+000014f0: 0a49 6e20 7468 6520 436f 6e6e 6563 746f  .In the Connecto
+00001500: 7227 7320 6063 6f6e 6e65 6374 6020 6d65  r's `connect` me
+00001510: 7468 6f64 2062 656c 6f77 2c20 696e 7075  thod below, inpu
+00001520: 7420 796f 7572 2063 6f6e 6e65 6374 696f  t your connectio
+00001530: 6e20 7374 7269 6e67 2061 7320 7468 6520  n string as the 
+00001540: 6669 7273 7420 706f 7369 7469 6f6e 616c  first positional
+00001550: 2061 7267 756d 656e 7420 616e 6420 7468   argument and th
+00001560: 6520 6e61 6d65 206f 6620 7468 6520 6461  e name of the da
+00001570: 7461 6261 7365 2064 7269 7665 7220 666f  tabase driver fo
+00001580: 7220 7468 6520 7365 636f 6e64 2070 6f73  r the second pos
+00001590: 6974 696f 6e61 6c20 6172 6775 6d65 6e74  itional argument
+000015a0: 2e20 496e 7365 7274 2074 6865 2072 6573  . Insert the res
+000015b0: 7420 6f66 2079 6f75 7220 636f 6e6e 6563  t of your connec
+000015c0: 7469 6f6e 206b 6579 776f 7264 2061 7267  tion keyword arg
+000015d0: 756d 656e 7473 206c 696b 6520 7573 6572  uments like user
+000015e0: 2c20 7061 7373 776f 7264 2061 6e64 2064  , password and d
+000015f0: 6174 6162 6173 652e 2059 6f75 2063 616e  atabase. You can
+00001600: 2061 6c73 6f20 7365 7420 7468 6520 6f70   also set the op
+00001610: 7469 6f6e 616c 2060 7469 6d65 6f75 7460  tional `timeout`
+00001620: 206f 7220 6069 705f 7479 7065 6020 6b65   or `ip_type` ke
+00001630: 7977 6f72 6420 6172 6775 6d65 6e74 732e  yword arguments.
+00001640: 0a0a 546f 2075 7365 2074 6869 7320 636f  ..To use this co
+00001650: 6e6e 6563 746f 7220 7769 7468 2053 514c  nnector with SQL
+00001660: 416c 6368 656d 792c 2075 7365 2074 6865  Alchemy, use the
+00001670: 2060 6372 6561 746f 7260 2061 7267 756d   `creator` argum
+00001680: 656e 7420 666f 7220 6073 716c 616c 6368  ent for `sqlalch
+00001690: 656d 792e 6372 6561 7465 5f65 6e67 696e  emy.create_engin
+000016a0: 6560 3a0a 0a60 6060 7079 7468 6f6e 0a66  e`:..```python.f
+000016b0: 726f 6d20 676f 6f67 6c65 2e63 6c6f 7564  rom google.cloud
+000016c0: 2e73 716c 2e63 6f6e 6e65 6374 6f72 2069  .sql.connector i
+000016d0: 6d70 6f72 7420 436f 6e6e 6563 746f 720a  mport Connector.
+000016e0: 696d 706f 7274 2073 716c 616c 6368 656d  import sqlalchem
+000016f0: 790a 0a23 2069 6e69 7469 616c 697a 6520  y..# initialize 
+00001700: 436f 6e6e 6563 746f 7220 6f62 6a65 6374  Connector object
+00001710: 0a63 6f6e 6e65 6374 6f72 203d 2043 6f6e  .connector = Con
+00001720: 6e65 6374 6f72 2829 0a0a 2320 6675 6e63  nector()..# func
+00001730: 7469 6f6e 2074 6f20 7265 7475 726e 2074  tion to return t
+00001740: 6865 2064 6174 6162 6173 6520 636f 6e6e  he database conn
+00001750: 6563 7469 6f6e 0a64 6566 2067 6574 636f  ection.def getco
+00001760: 6e6e 2829 202d 3e20 7079 6d79 7371 6c2e  nn() -> pymysql.
+00001770: 636f 6e6e 6563 7469 6f6e 732e 436f 6e6e  connections.Conn
+00001780: 6563 7469 6f6e 3a0a 2020 2020 636f 6e6e  ection:.    conn
+00001790: 3a20 7079 6d79 7371 6c2e 636f 6e6e 6563  : pymysql.connec
+000017a0: 7469 6f6e 732e 436f 6e6e 6563 7469 6f6e  tions.Connection
+000017b0: 203d 2063 6f6e 6e65 6374 6f72 2e63 6f6e   = connector.con
+000017c0: 6e65 6374 280a 2020 2020 2020 2020 2270  nect(.        "p
+000017d0: 726f 6a65 6374 3a72 6567 696f 6e3a 696e  roject:region:in
+000017e0: 7374 616e 6365 222c 0a20 2020 2020 2020  stance",.       
+000017f0: 2022 7079 6d79 7371 6c22 2c0a 2020 2020   "pymysql",.    
+00001800: 2020 2020 7573 6572 3d22 6d79 2d75 7365      user="my-use
+00001810: 7222 2c0a 2020 2020 2020 2020 7061 7373  r",.        pass
+00001820: 776f 7264 3d22 6d79 2d70 6173 7377 6f72  word="my-passwor
+00001830: 6422 2c0a 2020 2020 2020 2020 6462 3d22  d",.        db="
+00001840: 6d79 2d64 622d 6e61 6d65 220a 2020 2020  my-db-name".    
+00001850: 290a 2020 2020 7265 7475 726e 2063 6f6e  ).    return con
+00001860: 6e0a 0a23 2063 7265 6174 6520 636f 6e6e  n..# create conn
+00001870: 6563 7469 6f6e 2070 6f6f 6c0a 706f 6f6c  ection pool.pool
+00001880: 203d 2073 716c 616c 6368 656d 792e 6372   = sqlalchemy.cr
+00001890: 6561 7465 5f65 6e67 696e 6528 0a20 2020  eate_engine(.   
+000018a0: 2022 6d79 7371 6c2b 7079 6d79 7371 6c3a   "mysql+pymysql:
+000018b0: 2f2f 222c 0a20 2020 2063 7265 6174 6f72  //",.    creator
+000018c0: 3d67 6574 636f 6e6e 2c0a 290a 6060 600a  =getconn,.).```.
+000018d0: 0a54 6865 2072 6574 7572 6e65 6420 636f  .The returned co
+000018e0: 6e6e 6563 7469 6f6e 2070 6f6f 6c20 656e  nnection pool en
+000018f0: 6769 6e65 2063 616e 2074 6865 6e20 6265  gine can then be
+00001900: 2075 7365 6420 746f 2071 7565 7279 2061   used to query a
+00001910: 6e64 206d 6f64 6966 7920 7468 6520 6461  nd modify the da
+00001920: 7461 6261 7365 2e0a 0a60 6060 7079 7468  tabase...```pyth
+00001930: 6f6e 0a23 2069 6e73 6572 7420 7374 6174  on.# insert stat
+00001940: 656d 656e 740a 696e 7365 7274 5f73 746d  ement.insert_stm
+00001950: 7420 3d20 7371 6c61 6c63 6865 6d79 2e74  t = sqlalchemy.t
+00001960: 6578 7428 0a20 2020 2022 494e 5345 5254  ext(.    "INSERT
+00001970: 2049 4e54 4f20 6d79 5f74 6162 6c65 2028   INTO my_table (
+00001980: 6964 2c20 7469 746c 6529 2056 414c 5545  id, title) VALUE
+00001990: 5320 283a 6964 2c20 3a74 6974 6c65 2922  S (:id, :title)"
+000019a0: 2c0a 290a 0a77 6974 6820 706f 6f6c 2e63  ,.)..with pool.c
+000019b0: 6f6e 6e65 6374 2829 2061 7320 6462 5f63  onnect() as db_c
+000019c0: 6f6e 6e3a 0a20 2020 2023 2069 6e73 6572  onn:.    # inser
+000019d0: 7420 696e 746f 2064 6174 6162 6173 650a  t into database.
+000019e0: 2020 2020 6462 5f63 6f6e 6e2e 6578 6563      db_conn.exec
+000019f0: 7574 6528 696e 7365 7274 5f73 746d 742c  ute(insert_stmt,
+00001a00: 2070 6172 616d 6574 6572 733d 7b22 6964   parameters={"id
+00001a10: 223a 2022 626f 6f6b 3122 2c20 2274 6974  ": "book1", "tit
+00001a20: 6c65 223a 2022 426f 6f6b 204f 6e65 227d  le": "Book One"}
+00001a30: 290a 0a20 2020 2023 2071 7565 7279 2064  )..    # query d
+00001a40: 6174 6162 6173 650a 2020 2020 7265 7375  atabase.    resu
+00001a50: 6c74 203d 2064 625f 636f 6e6e 2e65 7865  lt = db_conn.exe
+00001a60: 6375 7465 2873 716c 616c 6368 656d 792e  cute(sqlalchemy.
+00001a70: 7465 7874 2822 5345 4c45 4354 202a 2066  text("SELECT * f
+00001a80: 726f 6d20 6d79 5f74 6162 6c65 2229 292e  rom my_table")).
+00001a90: 6665 7463 6861 6c6c 2829 0a0a 2020 2020  fetchall()..    
+00001aa0: 2320 636f 6d6d 6974 2074 7261 6e73 6163  # commit transac
+00001ab0: 7469 6f6e 2028 5351 4c41 6c63 6865 6d79  tion (SQLAlchemy
+00001ac0: 2076 322e 582e 5820 6973 2063 6f6d 6d69   v2.X.X is commi
+00001ad0: 7420 6173 2079 6f75 2067 6f29 0a20 2020  t as you go).   
+00001ae0: 2064 625f 636f 6e6e 2e63 6f6d 6d69 7428   db_conn.commit(
+00001af0: 290a 0a20 2020 2023 2044 6f20 736f 6d65  )..    # Do some
+00001b00: 7468 696e 6720 7769 7468 2074 6865 2072  thing with the r
+00001b10: 6573 756c 7473 0a20 2020 2066 6f72 2072  esults.    for r
+00001b20: 6f77 2069 6e20 7265 7375 6c74 3a0a 2020  ow in result:.  
+00001b30: 2020 2020 2020 7072 696e 7428 726f 7729        print(row)
+00001b40: 0a60 6060 0a0a 546f 2063 6c6f 7365 2074  .```..To close t
+00001b50: 6865 2060 436f 6e6e 6563 746f 7260 206f  he `Connector` o
+00001b60: 626a 6563 7427 7320 6261 636b 6772 6f75  bject's backgrou
+00001b70: 6e64 2072 6573 6f75 7263 6573 2c20 6361  nd resources, ca
+00001b80: 6c6c 2069 7427 7320 6063 6c6f 7365 2829  ll it's `close()
+00001b90: 6020 6d65 7468 6f64 2061 7320 666f 6c6c  ` method as foll
+00001ba0: 6f77 733a 0a0a 6060 6070 7974 686f 6e0a  ows:..```python.
+00001bb0: 636f 6e6e 6563 746f 722e 636c 6f73 6528  connector.close(
+00001bc0: 290a 6060 600a 0a2a 2a4e 6f74 652a 2a3a  ).```..**Note**:
+00001bd0: 2046 6f72 206d 6f72 6520 6578 616d 706c   For more exampl
+00001be0: 6573 206f 6620 7573 696e 6720 5351 4c41  es of using SQLA
+00001bf0: 6c63 6865 6d79 2074 6f20 6d61 6e61 6765  lchemy to manage
+00001c00: 2063 6f6e 6e65 6374 696f 6e20 706f 6f6c   connection pool
+00001c10: 696e 6720 7769 7468 2074 6865 2063 6f6e  ing with the con
+00001c20: 6e65 6374 6f72 2c20 706c 6561 7365 2073  nector, please s
+00001c30: 6565 205b 436c 6f75 6420 5351 4c20 5351  ee [Cloud SQL SQ
+00001c40: 4c41 6c63 6865 6d79 2053 616d 706c 6573  LAlchemy Samples
+00001c50: 5d28 6874 7470 733a 2f2f 636c 6f75 642e  ](https://cloud.
+00001c60: 676f 6f67 6c65 2e63 6f6d 2f73 716c 2f64  google.com/sql/d
+00001c70: 6f63 732f 706f 7374 6772 6573 2f63 6f6e  ocs/postgres/con
+00001c80: 6e65 6374 2d63 6f6e 6e65 6374 6f72 7323  nect-connectors#
+00001c90: 7079 7468 6f6e 5f31 292e 0a0a 2a2a 4e6f  python_1)...**No
+00001ca0: 7465 2066 6f72 2053 514c 2053 6572 7665  te for SQL Serve
+00001cb0: 7220 7573 6572 732a 2a3a 2049 6620 796f  r users**: If yo
+00001cc0: 7572 2053 514c 2053 6572 7665 7220 696e  ur SQL Server in
+00001cd0: 7374 616e 6365 2072 6571 7569 7265 7320  stance requires 
+00001ce0: 5353 4c2c 2079 6f75 206e 6565 6420 746f  SSL, you need to
+00001cf0: 2064 6f77 6e6c 6f61 6420 7468 6520 4341   download the CA
+00001d00: 2063 6572 7469 6669 6361 7465 2066 6f72   certificate for
+00001d10: 2079 6f75 7220 696e 7374 616e 6365 2061   your instance a
+00001d20: 6e64 2069 6e63 6c75 6465 2060 6361 6669  nd include `cafi
+00001d30: 6c65 3d7b 7061 7468 2074 6f20 646f 776e  le={path to down
+00001d40: 6c6f 6164 6564 2063 6572 7469 6669 6361  loaded certifica
+00001d50: 7465 7d60 2061 6e64 2060 7661 6c69 6461  te}` and `valida
+00001d60: 7465 5f68 6f73 743d 4661 6c73 6560 2e20  te_host=False`. 
+00001d70: 5468 6973 2069 7320 6120 776f 726b 6172  This is a workar
+00001d80: 6f75 6e64 2066 6f72 2061 205b 6b6e 6f77  ound for a [know
+00001d90: 6e20 6973 7375 655d 2868 7474 7073 3a2f  n issue](https:/
+00001da0: 2f69 7373 7565 7472 6163 6b65 722e 676f  /issuetracker.go
+00001db0: 6f67 6c65 2e63 6f6d 2f31 3834 3836 3731  ogle.com/1848671
+00001dc0: 3437 292e 0a0a 2323 2320 436f 6e66 6967  47)...### Config
+00001dd0: 7572 696e 6720 7468 6520 436f 6e6e 6563  uring the Connec
+00001de0: 746f 720a 0a49 6620 796f 7520 6e65 6564  tor..If you need
+00001df0: 2074 6f20 6375 7374 6f6d 697a 6520 736f   to customize so
+00001e00: 6d65 7468 696e 6720 6162 6f75 7420 7468  mething about th
+00001e10: 6520 636f 6e6e 6563 746f 722c 206f 7220  e connector, or 
+00001e20: 7761 6e74 2074 6f20 7370 6563 6966 790a  want to specify.
+00001e30: 6465 6661 756c 7473 2066 6f72 2065 6163  defaults for eac
+00001e40: 6820 636f 6e6e 6563 7469 6f6e 2074 6f20  h connection to 
+00001e50: 6d61 6b65 2c20 796f 7520 6361 6e20 696e  make, you can in
+00001e60: 6974 6961 6c69 7a65 2061 0a60 436f 6e6e  itialize a.`Conn
+00001e70: 6563 746f 7260 206f 626a 6563 7420 6173  ector` object as
+00001e80: 2066 6f6c 6c6f 7773 3a0a 0a60 6060 7079   follows:..```py
+00001e90: 7468 6f6e 0a66 726f 6d20 676f 6f67 6c65  thon.from google
+00001ea0: 2e63 6c6f 7564 2e73 716c 2e63 6f6e 6e65  .cloud.sql.conne
+00001eb0: 6374 6f72 2069 6d70 6f72 7420 436f 6e6e  ctor import Conn
+00001ec0: 6563 746f 722c 2049 5054 7970 6573 0a0a  ector, IPTypes..
+00001ed0: 2320 4e6f 7465 3a20 616c 6c20 7061 7261  # Note: all para
+00001ee0: 6d65 7465 7273 2062 656c 6f77 2061 7265  meters below are
+00001ef0: 206f 7074 696f 6e61 6c0a 636f 6e6e 6563   optional.connec
+00001f00: 746f 7220 3d20 436f 6e6e 6563 746f 7228  tor = Connector(
+00001f10: 0a20 2020 2069 705f 7479 7065 3d49 5054  .    ip_type=IPT
+00001f20: 7970 6573 2e50 5542 4c49 432c 0a20 2020  ypes.PUBLIC,.   
+00001f30: 2065 6e61 626c 655f 6961 6d5f 6175 7468   enable_iam_auth
+00001f40: 3d46 616c 7365 2c0a 2020 2020 7469 6d65  =False,.    time
+00001f50: 6f75 743d 3330 2c0a 2020 2020 6372 6564  out=30,.    cred
+00001f60: 656e 7469 616c 733d 6375 7374 6f6d 5f63  entials=custom_c
+00001f70: 7265 6473 2023 2067 6f6f 676c 652e 6175  reds # google.au
+00001f80: 7468 2e63 7265 6465 6e74 6961 6c73 2e43  th.credentials.C
+00001f90: 7265 6465 6e74 6961 6c73 0a29 0a60 6060  redentials.).```
+00001fa0: 0a0a 2323 2320 5573 696e 6720 436f 6e6e  ..### Using Conn
+00001fb0: 6563 746f 7220 6173 2061 2043 6f6e 7465  ector as a Conte
+00001fc0: 7874 204d 616e 6167 6572 0a0a 5468 6520  xt Manager..The 
+00001fd0: 6043 6f6e 6e65 6374 6f72 6020 6f62 6a65  `Connector` obje
+00001fe0: 6374 2063 616e 2061 6c73 6f20 6265 2075  ct can also be u
+00001ff0: 7365 6420 6173 2061 2063 6f6e 7465 7874  sed as a context
+00002000: 206d 616e 6167 6572 2069 6e20 6f72 6465   manager in orde
+00002010: 7220 746f 0a61 7574 6f6d 6174 6963 616c  r to.automatical
+00002020: 6c79 2063 6c6f 7365 2061 6e64 2063 6c65  ly close and cle
+00002030: 616e 7570 2072 6573 6f75 7263 6573 2c20  anup resources, 
+00002040: 7265 6d6f 7669 6e67 2074 6865 206e 6565  removing the nee
+00002050: 6420 666f 7220 6578 706c 6963 6974 0a63  d for explicit.c
+00002060: 616c 6c73 2074 6f20 6063 6f6e 6e65 6374  alls to `connect
+00002070: 6f72 2e63 6c6f 7365 2829 602e 0a0a 436f  or.close()`...Co
+00002080: 6e6e 6563 746f 7220 6173 2061 2063 6f6e  nnector as a con
+00002090: 7465 7874 206d 616e 6167 6572 3a0a 0a60  text manager:..`
+000020a0: 6060 7079 7468 6f6e 0a66 726f 6d20 676f  ``python.from go
+000020b0: 6f67 6c65 2e63 6c6f 7564 2e73 716c 2e63  ogle.cloud.sql.c
+000020c0: 6f6e 6e65 6374 6f72 2069 6d70 6f72 7420  onnector import 
+000020d0: 436f 6e6e 6563 746f 720a 696d 706f 7274  Connector.import
+000020e0: 2070 796d 7973 716c 0a69 6d70 6f72 7420   pymysql.import 
+000020f0: 7371 6c61 6c63 6865 6d79 0a0a 2320 6865  sqlalchemy..# he
+00002100: 6c70 6572 2066 756e 6374 696f 6e20 746f  lper function to
+00002110: 2072 6574 7572 6e20 5351 4c41 6c63 6865   return SQLAlche
+00002120: 6d79 2063 6f6e 6e65 6374 696f 6e20 706f  my connection po
+00002130: 6f6c 0a64 6566 2069 6e69 745f 636f 6e6e  ol.def init_conn
+00002140: 6563 7469 6f6e 5f70 6f6f 6c28 636f 6e6e  ection_pool(conn
+00002150: 6563 746f 723a 2043 6f6e 6e65 6374 6f72  ector: Connector
+00002160: 2920 2d3e 2073 716c 616c 6368 656d 792e  ) -> sqlalchemy.
+00002170: 656e 6769 6e65 2e45 6e67 696e 653a 0a20  engine.Engine:. 
+00002180: 2020 2023 2066 756e 6374 696f 6e20 7573     # function us
+00002190: 6564 2074 6f20 6765 6e65 7261 7465 2064  ed to generate d
+000021a0: 6174 6162 6173 6520 636f 6e6e 6563 7469  atabase connecti
+000021b0: 6f6e 0a20 2020 2064 6566 2067 6574 636f  on.    def getco
+000021c0: 6e6e 2829 202d 3e20 7079 6d79 7371 6c2e  nn() -> pymysql.
+000021d0: 636f 6e6e 6563 7469 6f6e 732e 436f 6e6e  connections.Conn
+000021e0: 6563 7469 6f6e 3a0a 2020 2020 2020 2020  ection:.        
+000021f0: 636f 6e6e 203d 2063 6f6e 6e65 6374 6f72  conn = connector
+00002200: 2e63 6f6e 6e65 6374 280a 2020 2020 2020  .connect(.      
+00002210: 2020 2020 2020 2270 726f 6a65 6374 3a72        "project:r
+00002220: 6567 696f 6e3a 696e 7374 616e 6365 222c  egion:instance",
+00002230: 0a20 2020 2020 2020 2020 2020 2022 7079  .            "py
+00002240: 6d79 7371 6c22 2c0a 2020 2020 2020 2020  mysql",.        
+00002250: 2020 2020 7573 6572 3d22 6d79 2d75 7365      user="my-use
+00002260: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
+00002270: 7061 7373 776f 7264 3d22 6d79 2d70 6173  password="my-pas
+00002280: 7377 6f72 6422 2c0a 2020 2020 2020 2020  sword",.        
+00002290: 2020 2020 6462 3d22 6d79 2d64 622d 6e61      db="my-db-na
+000022a0: 6d65 220a 2020 2020 2020 2020 290a 2020  me".        ).  
+000022b0: 2020 2020 2020 7265 7475 726e 2063 6f6e        return con
+000022c0: 6e0a 0a20 2020 2023 2063 7265 6174 6520  n..    # create 
+000022d0: 636f 6e6e 6563 7469 6f6e 2070 6f6f 6c0a  connection pool.
+000022e0: 2020 2020 706f 6f6c 203d 2073 716c 616c      pool = sqlal
+000022f0: 6368 656d 792e 6372 6561 7465 5f65 6e67  chemy.create_eng
+00002300: 696e 6528 0a20 2020 2020 2020 2022 6d79  ine(.        "my
+00002310: 7371 6c2b 7079 6d79 7371 6c3a 2f2f 222c  sql+pymysql://",
+00002320: 0a20 2020 2020 2020 2063 7265 6174 6f72  .        creator
+00002330: 3d67 6574 636f 6e6e 2c0a 2020 2020 290a  =getconn,.    ).
+00002340: 2020 2020 7265 7475 726e 2070 6f6f 6c0a      return pool.
+00002350: 0a23 2069 6e69 7469 616c 697a 6520 436c  .# initialize Cl
+00002360: 6f75 6420 5351 4c20 5079 7468 6f6e 2043  oud SQL Python C
+00002370: 6f6e 6e65 6374 6f72 2061 7320 636f 6e74  onnector as cont
+00002380: 6578 7420 6d61 6e61 6765 720a 7769 7468  ext manager.with
+00002390: 2043 6f6e 6e65 6374 6f72 2829 2061 7320   Connector() as 
+000023a0: 636f 6e6e 6563 746f 723a 0a20 2020 2023  connector:.    #
+000023b0: 2069 6e69 7469 616c 697a 6520 636f 6e6e   initialize conn
+000023c0: 6563 7469 6f6e 2070 6f6f 6c0a 2020 2020  ection pool.    
+000023d0: 706f 6f6c 203d 2069 6e69 745f 636f 6e6e  pool = init_conn
+000023e0: 6563 7469 6f6e 5f70 6f6f 6c28 636f 6e6e  ection_pool(conn
+000023f0: 6563 746f 7229 0a20 2020 2023 2069 6e73  ector).    # ins
+00002400: 6572 7420 7374 6174 656d 656e 740a 2020  ert statement.  
+00002410: 2020 696e 7365 7274 5f73 746d 7420 3d20    insert_stmt = 
+00002420: 7371 6c61 6c63 6865 6d79 2e74 6578 7428  sqlalchemy.text(
+00002430: 0a20 2020 2020 2020 2022 494e 5345 5254  .        "INSERT
+00002440: 2049 4e54 4f20 6d79 5f74 6162 6c65 2028   INTO my_table (
+00002450: 6964 2c20 7469 746c 6529 2056 414c 5545  id, title) VALUE
+00002460: 5320 283a 6964 2c20 3a74 6974 6c65 2922  S (:id, :title)"
+00002470: 2c0a 2020 2020 290a 0a20 2020 2023 2069  ,.    )..    # i
+00002480: 6e74 6572 6163 7420 7769 7468 2043 6c6f  nteract with Clo
+00002490: 7564 2053 514c 2064 6174 6162 6173 6520  ud SQL database 
+000024a0: 7573 696e 6720 636f 6e6e 6563 7469 6f6e  using connection
+000024b0: 2070 6f6f 6c0a 2020 2020 7769 7468 2070   pool.    with p
+000024c0: 6f6f 6c2e 636f 6e6e 6563 7428 2920 6173  ool.connect() as
+000024d0: 2064 625f 636f 6e6e 3a0a 2020 2020 2020   db_conn:.      
+000024e0: 2020 2320 696e 7365 7274 2069 6e74 6f20    # insert into 
+000024f0: 6461 7461 6261 7365 0a20 2020 2020 2020  database.       
+00002500: 2064 625f 636f 6e6e 2e65 7865 6375 7465   db_conn.execute
+00002510: 2869 6e73 6572 745f 7374 6d74 2c20 7061  (insert_stmt, pa
+00002520: 7261 6d65 7465 7273 3d7b 2269 6422 3a20  rameters={"id": 
+00002530: 2262 6f6f 6b31 222c 2022 7469 746c 6522  "book1", "title"
+00002540: 3a20 2242 6f6f 6b20 4f6e 6522 7d29 0a0a  : "Book One"})..
+00002550: 2020 2020 2020 2020 2320 636f 6d6d 6974          # commit
+00002560: 2074 7261 6e73 6163 7469 6f6e 2028 5351   transaction (SQ
+00002570: 4c41 6c63 6865 6d79 2076 322e 582e 5820  LAlchemy v2.X.X 
+00002580: 6973 2063 6f6d 6d69 7420 6173 2079 6f75  is commit as you
+00002590: 2067 6f29 0a20 2020 2020 2020 2064 625f   go).        db_
+000025a0: 636f 6e6e 2e63 6f6d 6d69 7428 290a 0a20  conn.commit().. 
+000025b0: 2020 2020 2020 2023 2071 7565 7279 2064         # query d
+000025c0: 6174 6162 6173 650a 2020 2020 2020 2020  atabase.        
+000025d0: 7265 7375 6c74 203d 2064 625f 636f 6e6e  result = db_conn
+000025e0: 2e65 7865 6375 7465 2873 716c 616c 6368  .execute(sqlalch
+000025f0: 656d 792e 7465 7874 2822 5345 4c45 4354  emy.text("SELECT
+00002600: 202a 2066 726f 6d20 6d79 5f74 6162 6c65   * from my_table
+00002610: 2229 292e 6665 7463 6861 6c6c 2829 0a0a  ")).fetchall()..
+00002620: 2020 2020 2020 2020 2320 446f 2073 6f6d          # Do som
+00002630: 6574 6869 6e67 2077 6974 6820 7468 6520  ething with the 
+00002640: 7265 7375 6c74 730a 2020 2020 2020 2020  results.        
+00002650: 666f 7220 726f 7720 696e 2072 6573 756c  for row in resul
+00002660: 743a 0a20 2020 2020 2020 2020 2020 2070  t:.            p
+00002670: 7269 6e74 2872 6f77 290a 6060 600a 0a23  rint(row).```..#
+00002680: 2323 2053 7065 6369 6679 696e 6720 4950  ## Specifying IP
+00002690: 2041 6464 7265 7373 2054 7970 650a 0a54   Address Type..T
+000026a0: 6865 2043 6c6f 7564 2053 514c 2050 7974  he Cloud SQL Pyt
+000026b0: 686f 6e20 436f 6e6e 6563 746f 7220 6361  hon Connector ca
+000026c0: 6e20 6265 2075 7365 6420 746f 2063 6f6e  n be used to con
+000026d0: 6e65 6374 2074 6f20 436c 6f75 6420 5351  nect to Cloud SQ
+000026e0: 4c20 696e 7374 616e 6365 730a 7573 696e  L instances.usin
+000026f0: 6720 626f 7468 2070 7562 6c69 6320 616e  g both public an
+00002700: 6420 7072 6976 6174 6520 4950 2061 6464  d private IP add
+00002710: 7265 7373 6573 2c20 6173 2077 656c 6c20  resses, as well 
+00002720: 6173 0a5b 5072 6976 6174 6520 5365 7276  as.[Private Serv
+00002730: 6963 6520 436f 6e6e 6563 745d 5b70 7363  ice Connect][psc
+00002740: 5d20 2850 5343 292e 2054 6f20 7370 6563  ] (PSC). To spec
+00002750: 6966 7920 7768 6963 6820 4950 2061 6464  ify which IP add
+00002760: 7265 7373 2074 7970 6520 746f 2063 6f6e  ress type to con
+00002770: 6e65 6374 0a77 6974 682c 2073 6574 2074  nect.with, set t
+00002780: 6865 2060 6970 5f74 7970 6560 206b 6579  he `ip_type` key
+00002790: 776f 7264 2061 7267 756d 656e 7420 7768  word argument wh
+000027a0: 656e 2069 6e69 7469 616c 697a 696e 6720  en initializing 
+000027b0: 6120 6043 6f6e 6e65 6374 6f72 2829 6020  a `Connector()` 
+000027c0: 6f72 2077 6865 6e0a 6361 6c6c 696e 6720  or when.calling 
+000027d0: 6063 6f6e 6e65 6374 6f72 2e63 6f6e 6e65  `connector.conne
+000027e0: 6374 2829 602e 0a0a 506f 7373 6962 6c65  ct()`...Possible
+000027f0: 2076 616c 7565 7320 666f 7220 6069 705f   values for `ip_
+00002800: 7479 7065 6020 6172 6520 6049 5054 7970  type` are `IPTyp
+00002810: 6573 2e50 5542 4c49 4360 2028 6465 6661  es.PUBLIC` (defa
+00002820: 756c 7420 7661 6c75 6529 2c0a 6049 5054  ult value),.`IPT
+00002830: 7970 6573 2e50 5249 5641 5445 602c 2061  ypes.PRIVATE`, a
+00002840: 6e64 2060 4950 5479 7065 732e 5053 4360  nd `IPTypes.PSC`
+00002850: 2e0a 0a45 7861 6d70 6c65 3a0a 0a60 6060  ...Example:..```
+00002860: 7079 7468 6f6e 0a66 726f 6d20 676f 6f67  python.from goog
+00002870: 6c65 2e63 6c6f 7564 2e73 716c 2e63 6f6e  le.cloud.sql.con
+00002880: 6e65 6374 6f72 2069 6d70 6f72 7420 4950  nector import IP
+00002890: 5479 7065 730a 0a63 6f6e 6e20 3d20 636f  Types..conn = co
+000028a0: 6e6e 6563 746f 722e 636f 6e6e 6563 7428  nnector.connect(
+000028b0: 0a20 2020 2022 7072 6f6a 6563 743a 7265  .    "project:re
+000028c0: 6769 6f6e 3a69 6e73 7461 6e63 6522 2c0a  gion:instance",.
+000028d0: 2020 2020 2270 796d 7973 716c 222c 0a20      "pymysql",. 
+000028e0: 2020 2069 705f 7479 7065 3d49 5054 7970     ip_type=IPTyp
+000028f0: 6573 2e50 5249 5641 5445 2023 2075 7365  es.PRIVATE # use
+00002900: 2070 7269 7661 7465 2049 500a 2e2e 2e20   private IP.... 
+00002910: 696e 7365 7274 206f 7468 6572 206b 7761  insert other kwa
+00002920: 7267 7320 2e2e 2e0a 290a 6060 600a 0a4e  rgs ....).```..N
+00002930: 6f74 653a 2049 6620 7370 6563 6966 7969  ote: If specifyi
+00002940: 6e67 2050 7269 7661 7465 2049 5020 6f72  ng Private IP or
+00002950: 2050 7269 7661 7465 2053 6572 7669 6365   Private Service
+00002960: 2043 6f6e 6e65 6374 2c20 796f 7572 2061   Connect, your a
+00002970: 7070 6c69 6361 7469 6f6e 206d 7573 7420  pplication must 
+00002980: 6265 0a61 7474 6163 6865 6420 746f 2074  be.attached to t
+00002990: 6865 2070 726f 7065 7220 5650 4320 6e65  he proper VPC ne
+000029a0: 7477 6f72 6b20 746f 2063 6f6e 6e65 6374  twork to connect
+000029b0: 2074 6f20 796f 7572 2043 6c6f 7564 2053   to your Cloud S
+000029c0: 514c 2069 6e73 7461 6e63 652e 2046 6f72  QL instance. For
+000029d0: 206d 6f73 740a 6170 706c 6963 6174 696f   most.applicatio
+000029e0: 6e73 2074 6869 7320 7769 6c6c 2072 6571  ns this will req
+000029f0: 7569 7265 2074 6865 2075 7365 206f 6620  uire the use of 
+00002a00: 6120 5b56 5043 2043 6f6e 6e65 6374 6f72  a [VPC Connector
+00002a10: 5d5b 7670 632d 636f 6e6e 6563 746f 725d  ][vpc-connector]
+00002a20: 2e0a 0a5b 7073 635d 3a20 6874 7470 733a  ...[psc]: https:
+00002a30: 2f2f 636c 6f75 642e 676f 6f67 6c65 2e63  //cloud.google.c
+00002a40: 6f6d 2f76 7063 2f64 6f63 732f 7072 6976  om/vpc/docs/priv
+00002a50: 6174 652d 7365 7276 6963 652d 636f 6e6e  ate-service-conn
+00002a60: 6563 740a 5b76 7063 2d63 6f6e 6e65 6374  ect.[vpc-connect
+00002a70: 6f72 5d3a 2068 7474 7073 3a2f 2f63 6c6f  or]: https://clo
+00002a80: 7564 2e67 6f6f 676c 652e 636f 6d2f 7670  ud.google.com/vp
+00002a90: 632f 646f 6373 2f63 6f6e 6669 6775 7265  c/docs/configure
+00002aa0: 2d73 6572 7665 726c 6573 732d 7670 632d  -serverless-vpc-
+00002ab0: 6163 6365 7373 2363 7265 6174 652d 636f  access#create-co
+00002ac0: 6e6e 6563 746f 720a 0a23 2323 2041 7574  nnector..### Aut
+00002ad0: 6f6d 6174 6963 2049 414d 2044 6174 6162  omatic IAM Datab
+00002ae0: 6173 6520 4175 7468 656e 7469 6361 7469  ase Authenticati
+00002af0: 6f6e 0a0a 436f 6e6e 6563 7469 6f6e 7320  on..Connections 
+00002b00: 7573 696e 6720 5b41 7574 6f6d 6174 6963  using [Automatic
+00002b10: 2049 414d 2064 6174 6162 6173 6520 6175   IAM database au
+00002b20: 7468 656e 7469 6361 7469 6f6e 5d28 6874  thentication](ht
+00002b30: 7470 733a 2f2f 636c 6f75 642e 676f 6f67  tps://cloud.goog
+00002b40: 6c65 2e63 6f6d 2f73 716c 2f64 6f63 732f  le.com/sql/docs/
+00002b50: 706f 7374 6772 6573 2f61 7574 6865 6e74  postgres/authent
+00002b60: 6963 6174 696f 6e23 6175 746f 6d61 7469  ication#automati
+00002b70: 6329 2061 7265 2073 7570 706f 7274 6564  c) are supported
+00002b80: 2077 6865 6e20 7573 696e 6720 506f 7374   when using Post
+00002b90: 6772 6573 206f 7220 4d79 5351 4c20 6472  gres or MySQL dr
+00002ba0: 6976 6572 732e 0a46 6972 7374 2c20 6d61  ivers..First, ma
+00002bb0: 6b65 2073 7572 6520 746f 205b 636f 6e66  ke sure to [conf
+00002bc0: 6967 7572 6520 796f 7572 2043 6c6f 7564  igure your Cloud
+00002bd0: 2053 514c 2049 6e73 7461 6e63 6520 746f   SQL Instance to
+00002be0: 2061 6c6c 6f77 2049 414d 2061 7574 6865   allow IAM authe
+00002bf0: 6e74 6963 6174 696f 6e5d 2868 7474 7073  ntication](https
+00002c00: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
+00002c10: 636f 6d2f 7371 6c2f 646f 6373 2f70 6f73  com/sql/docs/pos
+00002c20: 7467 7265 732f 6372 6561 7465 2d65 6469  tgres/create-edi
+00002c30: 742d 6961 6d2d 696e 7374 616e 6365 7323  t-iam-instances#
+00002c40: 636f 6e66 6967 7572 652d 6961 6d2d 6462  configure-iam-db
+00002c50: 2d69 6e73 7461 6e63 6529 0a61 6e64 205b  -instance).and [
+00002c60: 6164 6420 616e 2049 414d 2064 6174 6162  add an IAM datab
+00002c70: 6173 6520 7573 6572 5d28 6874 7470 733a  ase user](https:
+00002c80: 2f2f 636c 6f75 642e 676f 6f67 6c65 2e63  //cloud.google.c
+00002c90: 6f6d 2f73 716c 2f64 6f63 732f 706f 7374  om/sql/docs/post
+00002ca0: 6772 6573 2f63 7265 6174 652d 6d61 6e61  gres/create-mana
+00002cb0: 6765 2d69 616d 2d75 7365 7273 2363 7265  ge-iam-users#cre
+00002cc0: 6174 696e 672d 612d 6461 7461 6261 7365  ating-a-database
+00002cd0: 2d75 7365 7229 2e0a 0a4e 6f77 2c20 796f  -user)...Now, yo
+00002ce0: 7520 6361 6e20 636f 6e6e 6563 7420 7573  u can connect us
+00002cf0: 696e 6720 7573 6572 206f 7220 7365 7276  ing user or serv
+00002d00: 6963 6520 6163 636f 756e 7420 6372 6564  ice account cred
+00002d10: 656e 7469 616c 7320 696e 7374 6561 6420  entials instead 
+00002d20: 6f66 2061 2070 6173 7377 6f72 642e 0a49  of a password..I
+00002d30: 6e20 7468 6520 6361 6c6c 2074 6f20 636f  n the call to co
+00002d40: 6e6e 6563 742c 2073 6574 2074 6865 2060  nnect, set the `
+00002d50: 656e 6162 6c65 5f69 616d 5f61 7574 6860  enable_iam_auth`
+00002d60: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
+00002d70: 7420 746f 2074 7275 6520 616e 6420 7468  t to true and th
+00002d80: 6520 6075 7365 7260 2061 7267 756d 656e  e `user` argumen
+00002d90: 7420 746f 2074 6865 2061 7070 726f 7072  t to the appropr
+00002da0: 6961 7465 6c79 2066 6f72 6d61 7474 6564  iately formatted
+00002db0: 2049 414d 2070 7269 6e63 6970 616c 2e0a   IAM principal..
+00002dc0: 3e20 506f 7374 6772 6573 3a20 466f 7220  > Postgres: For 
+00002dd0: 616e 2049 414d 2075 7365 7220 6163 636f  an IAM user acco
+00002de0: 756e 742c 2074 6869 7320 6973 2074 6865  unt, this is the
+00002df0: 2075 7365 7227 7320 656d 6169 6c20 6164   user's email ad
+00002e00: 6472 6573 732e 2046 6f72 2061 2073 6572  dress. For a ser
+00002e10: 7669 6365 2061 6363 6f75 6e74 2c20 6974  vice account, it
+00002e20: 2069 7320 7468 6520 7365 7276 6963 6520   is the service 
+00002e30: 6163 636f 756e 7427 7320 656d 6169 6c20  account's email 
+00002e40: 7769 7468 6f75 7420 7468 6520 602e 6773  without the `.gs
+00002e50: 6572 7669 6365 6163 636f 756e 742e 636f  erviceaccount.co
+00002e60: 6d60 2064 6f6d 6169 6e20 7375 6666 6978  m` domain suffix
+00002e70: 2e0a 0a3e 204d 7953 514c 3a20 466f 7220  ...> MySQL: For 
+00002e80: 616e 2049 414d 2075 7365 7220 6163 636f  an IAM user acco
+00002e90: 756e 742c 2074 6869 7320 6973 2074 6865  unt, this is the
+00002ea0: 2075 7365 7227 7320 656d 6169 6c20 6164   user's email ad
+00002eb0: 6472 6573 732c 2077 6974 686f 7574 2074  dress, without t
+00002ec0: 6865 2040 206f 7220 646f 6d61 696e 206e  he @ or domain n
+00002ed0: 616d 652e 2046 6f72 2065 7861 6d70 6c65  ame. For example
+00002ee0: 2c20 666f 7220 6074 6573 742d 7573 6572  , for `test-user
+00002ef0: 4067 6d61 696c 2e63 6f6d 602c 2073 6574  @gmail.com`, set
+00002f00: 2074 6865 2060 7573 6572 6020 6172 6775   the `user` argu
+00002f10: 6d65 6e74 2074 6f20 6074 6573 742d 7573  ment to `test-us
+00002f20: 6572 602e 2046 6f72 2061 2073 6572 7669  er`. For a servi
+00002f30: 6365 2061 6363 6f75 6e74 2c20 7468 6973  ce account, this
+00002f40: 2069 7320 7468 6520 7365 7276 6963 6520   is the service 
+00002f50: 6163 636f 756e 7427 7320 656d 6169 6c20  account's email 
+00002f60: 6164 6472 6573 7320 7769 7468 6f75 7420  address without 
+00002f70: 7468 6520 6040 7072 6f6a 6563 742d 6964  the `@project-id
+00002f80: 2e69 616d 2e67 7365 7276 6963 6561 6363  .iam.gserviceacc
+00002f90: 6f75 6e74 2e63 6f6d 6020 7375 6666 6978  ount.com` suffix
+00002fa0: 2e0a 0a45 7861 6d70 6c65 3a0a 0a60 6060  ...Example:..```
+00002fb0: 7079 7468 6f6e 0a63 6f6e 6e20 3d20 636f  python.conn = co
+00002fc0: 6e6e 6563 746f 722e 636f 6e6e 6563 7428  nnector.connect(
+00002fd0: 0a20 2020 2020 2270 726f 6a65 6374 3a72  .     "project:r
+00002fe0: 6567 696f 6e3a 696e 7374 616e 6365 222c  egion:instance",
+00002ff0: 0a20 2020 2020 2270 6738 3030 3022 2c0a  .     "pg8000",.
+00003000: 2020 2020 2075 7365 723d 2270 6f73 7467       user="postg
+00003010: 7265 732d 6961 6d2d 7573 6572 4067 6d61  res-iam-user@gma
+00003020: 696c 2e63 6f6d 222c 0a20 2020 2020 6462  il.com",.     db
+00003030: 3d22 6d79 2d64 622d 6e61 6d65 222c 0a20  ="my-db-name",. 
+00003040: 2020 2020 656e 6162 6c65 5f69 616d 5f61      enable_iam_a
+00003050: 7574 683d 5472 7565 2c0a 2029 0a60 6060  uth=True,. ).```
+00003060: 0a0a 2323 2320 5351 4c20 5365 7276 6572  ..### SQL Server
+00003070: 2041 6374 6976 6520 4469 7265 6374 6f72   Active Director
+00003080: 7920 4175 7468 656e 7469 6361 7469 6f6e  y Authentication
+00003090: 0a0a 4163 7469 7665 2044 6972 6563 746f  ..Active Directo
+000030a0: 7279 2061 7574 6865 6e74 6963 6174 696f  ry authenticatio
+000030b0: 6e20 666f 7220 5351 4c20 5365 7276 6572  n for SQL Server
+000030c0: 2069 6e73 7461 6e63 6573 2069 7320 6375   instances is cu
+000030d0: 7272 656e 746c 7920 6f6e 6c79 2073 7570  rrently only sup
+000030e0: 706f 7274 6564 206f 6e20 5769 6e64 6f77  ported on Window
+000030f0: 732e 2046 6972 7374 2c20 6d61 6b65 2073  s. First, make s
+00003100: 7572 6520 746f 2066 6f6c 6c6f 7720 5b74  ure to follow [t
+00003110: 6865 7365 2073 7465 7073 5d28 6874 7470  hese steps](http
+00003120: 733a 2f2f 636c 6f75 642e 676f 6f67 6c65  s://cloud.google
+00003130: 2e63 6f6d 2f62 6c6f 672f 746f 7069 6373  .com/blog/topics
+00003140: 2f64 6576 656c 6f70 6572 732d 7072 6163  /developers-prac
+00003150: 7469 7469 6f6e 6572 732f 6372 6561 7469  titioners/creati
+00003160: 6e67 2d73 716c 2d73 6572 7665 722d 696e  ng-sql-server-in
+00003170: 7374 616e 6365 2d69 6e74 6567 7261 7465  stance-integrate
+00003180: 642d 6163 7469 7665 2d64 6972 6563 746f  d-active-directo
+00003190: 7279 2d75 7369 6e67 2d67 6f6f 676c 652d  ry-using-google-
+000031a0: 636c 6f75 642d 7371 6c29 2074 6f20 7365  cloud-sql) to se
+000031b0: 7420 7570 2061 204d 616e 6167 6564 2041  t up a Managed A
+000031c0: 4420 646f 6d61 696e 2061 6e64 206a 6f69  D domain and joi
+000031d0: 6e20 796f 7572 2043 6c6f 7564 2053 514c  n your Cloud SQL
+000031e0: 2069 6e73 7461 6e63 6520 746f 2074 6865   instance to the
+000031f0: 2064 6f6d 6169 6e2e 205b 5365 6520 6865   domain. [See he
+00003200: 7265 2066 6f72 206d 6f72 6520 696e 666f  re for more info
+00003210: 206f 6e20 436c 6f75 6420 5351 4c20 4163   on Cloud SQL Ac
+00003220: 7469 7665 2044 6972 6563 746f 7279 2069  tive Directory i
+00003230: 6e74 6567 7261 7469 6f6e 5d28 6874 7470  ntegration](http
+00003240: 733a 2f2f 636c 6f75 642e 676f 6f67 6c65  s://cloud.google
+00003250: 2e63 6f6d 2f73 716c 2f64 6f63 732f 7371  .com/sql/docs/sq
+00003260: 6c73 6572 7665 722f 6164 292e 0a0a 4f6e  lserver/ad)...On
+00003270: 6365 2079 6f75 2068 6176 6520 666f 6c6c  ce you have foll
+00003280: 6f77 6564 2074 6865 2073 7465 7073 206c  owed the steps l
+00003290: 696e 6b65 6420 6162 6f76 652c 2079 6f75  inked above, you
+000032a0: 2063 616e 2072 756e 2074 6865 2066 6f6c   can run the fol
+000032b0: 6c6f 7769 6e67 2063 6f64 6520 746f 2072  lowing code to r
+000032c0: 6574 7572 6e20 6120 636f 6e6e 6563 7469  eturn a connecti
+000032d0: 6f6e 206f 626a 6563 743a 0a0a 6060 6070  on object:..```p
+000032e0: 7974 686f 6e0a 636f 6e6e 203d 2063 6f6e  ython.conn = con
+000032f0: 6e65 6374 6f72 2e63 6f6e 6e65 6374 280a  nector.connect(.
+00003300: 2020 2020 2270 726f 6a65 6374 3a72 6567      "project:reg
+00003310: 696f 6e3a 696e 7374 616e 6365 222c 0a20  ion:instance",. 
+00003320: 2020 2022 7079 7464 7322 2c0a 2020 2020     "pytds",.    
+00003330: 6462 3d22 6d79 2d64 622d 6e61 6d65 222c  db="my-db-name",
+00003340: 0a20 2020 2061 6374 6976 655f 6469 7265  .    active_dire
+00003350: 6374 6f72 795f 6175 7468 3d54 7275 652c  ctory_auth=True,
+00003360: 0a20 2020 2073 6572 7665 725f 6e61 6d65  .    server_name
+00003370: 3d22 7075 626c 6963 2e5b 696e 7374 616e  ="public.[instan
+00003380: 6365 5d2e 5b6c 6f63 6174 696f 6e5d 2e5b  ce].[location].[
+00003390: 7072 6f6a 6563 745d 2e63 6c6f 7564 7371  project].cloudsq
+000033a0: 6c2e 5b64 6f6d 6169 6e5d 222c 0a29 0a60  l.[domain]",.).`
+000033b0: 6060 0a0a 4f72 2c20 6966 2075 7369 6e67  ``..Or, if using
+000033c0: 2050 7269 7661 7465 2049 503a 0a0a 6060   Private IP:..``
+000033d0: 6070 7974 686f 6e0a 636f 6e6e 203d 2063  `python.conn = c
+000033e0: 6f6e 6e65 6374 6f72 2e63 6f6e 6e65 6374  onnector.connect
+000033f0: 280a 2020 2020 2270 726f 6a65 6374 3a72  (.    "project:r
+00003400: 6567 696f 6e3a 696e 7374 616e 6365 222c  egion:instance",
+00003410: 0a20 2020 2022 7079 7464 7322 2c0a 2020  .    "pytds",.  
+00003420: 2020 6462 3d22 6d79 2d64 622d 6e61 6d65    db="my-db-name
+00003430: 222c 0a20 2020 2061 6374 6976 655f 6469  ",.    active_di
+00003440: 7265 6374 6f72 795f 6175 7468 3d54 7275  rectory_auth=Tru
+00003450: 652c 0a20 2020 2073 6572 7665 725f 6e61  e,.    server_na
+00003460: 6d65 3d22 7072 6976 6174 652e 5b69 6e73  me="private.[ins
+00003470: 7461 6e63 655d 2e5b 6c6f 6361 7469 6f6e  tance].[location
+00003480: 5d2e 5b70 726f 6a65 6374 5d2e 636c 6f75  ].[project].clou
+00003490: 6473 716c 2e5b 646f 6d61 696e 5d22 2c0a  dsql.[domain]",.
+000034a0: 2020 2020 6970 5f74 7970 653d 4950 5479      ip_type=IPTy
+000034b0: 7065 732e 5052 4956 4154 450a 290a 6060  pes.PRIVATE.).``
+000034c0: 600a 0a23 2323 2055 7369 6e67 2074 6865  `..### Using the
+000034d0: 2050 7974 686f 6e20 436f 6e6e 6563 746f   Python Connecto
+000034e0: 7220 7769 7468 2050 7974 686f 6e20 5765  r with Python We
+000034f0: 6220 4672 616d 6577 6f72 6b73 0a0a 5468  b Frameworks..Th
+00003500: 6520 5079 7468 6f6e 2043 6f6e 6e65 6374  e Python Connect
+00003510: 6f72 2063 616e 2062 6520 7573 6564 2061  or can be used a
+00003520: 6c6f 6e67 7369 6465 2070 6f70 756c 6172  longside popular
+00003530: 2050 7974 686f 6e20 7765 6220 6672 616d   Python web fram
+00003540: 6577 6f72 6b73 2073 7563 680a 6173 2046  eworks such.as F
+00003550: 6c61 736b 2c20 4661 7374 4150 492c 2065  lask, FastAPI, e
+00003560: 7463 2c20 746f 2069 6e74 6567 7261 7465  tc, to integrate
+00003570: 2043 6c6f 7564 2053 514c 2064 6174 6162   Cloud SQL datab
+00003580: 6173 6573 2077 6974 6869 6e20 796f 7572  ases within your
+00003590: 0a77 6562 2061 7070 6c69 6361 7469 6f6e  .web application
+000035a0: 732e 0a0a 2323 2323 2046 6c61 736b 2d53  s...#### Flask-S
+000035b0: 514c 416c 6368 656d 790a 0a5b 466c 6173  QLAlchemy..[Flas
+000035c0: 6b2d 5351 4c41 6c63 6865 6d79 5d28 6874  k-SQLAlchemy](ht
+000035d0: 7470 733a 2f2f 666c 6173 6b2d 7371 6c61  tps://flask-sqla
+000035e0: 6c63 6865 6d79 2e70 616c 6c65 7473 7072  lchemy.palletspr
+000035f0: 6f6a 6563 7473 2e63 6f6d 2f65 6e2f 322e  ojects.com/en/2.
+00003600: 782f 290a 6973 2061 6e20 6578 7465 6e73  x/).is an extens
+00003610: 696f 6e20 666f 7220 5b46 6c61 736b 5d28  ion for [Flask](
+00003620: 6874 7470 733a 2f2f 666c 6173 6b2e 7061  https://flask.pa
+00003630: 6c6c 6574 7370 726f 6a65 6374 732e 636f  lletsprojects.co
+00003640: 6d2f 656e 2f32 2e32 2e78 2f29 0a74 6861  m/en/2.2.x/).tha
+00003650: 7420 6164 6473 2073 7570 706f 7274 2066  t adds support f
+00003660: 6f72 205b 5351 4c41 6c63 6865 6d79 5d28  or [SQLAlchemy](
+00003670: 6874 7470 733a 2f2f 7777 772e 7371 6c61  https://www.sqla
+00003680: 6c63 6865 6d79 2e6f 7267 2f29 2074 6f20  lchemy.org/) to 
+00003690: 796f 7572 0a61 7070 6c69 6361 7469 6f6e  your.application
+000036a0: 2e20 4974 2061 696d 7320 746f 2073 696d  . It aims to sim
+000036b0: 706c 6966 7920 7573 696e 6720 5351 4c41  plify using SQLA
+000036c0: 6c63 6865 6d79 2077 6974 6820 466c 6173  lchemy with Flas
+000036d0: 6b20 6279 2070 726f 7669 6469 6e67 0a75  k by providing.u
+000036e0: 7365 6675 6c20 6465 6661 756c 7473 2061  seful defaults a
+000036f0: 6e64 2065 7874 7261 2068 656c 7065 7273  nd extra helpers
+00003700: 2074 6861 7420 6d61 6b65 2069 7420 6561   that make it ea
+00003710: 7369 6572 2074 6f20 6163 636f 6d70 6c69  sier to accompli
+00003720: 7368 0a63 6f6d 6d6f 6e20 7461 736b 732e  sh.common tasks.
+00003730: 0a0a 596f 7520 6361 6e20 636f 6e66 6967  ..You can config
+00003740: 7572 6520 466c 6173 6b2d 5351 4c41 6c63  ure Flask-SQLAlc
+00003750: 6865 6d79 2074 6f20 636f 6e6e 6563 7420  hemy to connect 
+00003760: 746f 2061 2043 6c6f 7564 2053 514c 2064  to a Cloud SQL d
+00003770: 6174 6162 6173 6520 6672 6f6d 0a79 6f75  atabase from.you
+00003780: 7220 7765 6220 6170 706c 6963 6174 696f  r web applicatio
+00003790: 6e20 7468 726f 7567 6820 7468 6520 666f  n through the fo
+000037a0: 6c6c 6f77 696e 673a 0a0a 6060 6070 7974  llowing:..```pyt
+000037b0: 686f 6e0a 6672 6f6d 2066 6c61 736b 2069  hon.from flask i
+000037c0: 6d70 6f72 7420 466c 6173 6b0a 6672 6f6d  mport Flask.from
+000037d0: 2066 6c61 736b 5f73 716c 616c 6368 656d   flask_sqlalchem
+000037e0: 7920 696d 706f 7274 2053 514c 416c 6368  y import SQLAlch
+000037f0: 656d 790a 6672 6f6d 2067 6f6f 676c 652e  emy.from google.
+00003800: 636c 6f75 642e 7371 6c2e 636f 6e6e 6563  cloud.sql.connec
+00003810: 746f 7220 696d 706f 7274 2043 6f6e 6e65  tor import Conne
+00003820: 6374 6f72 2c20 4950 5479 7065 730a 0a0a  ctor, IPTypes...
+00003830: 2320 696e 6974 6961 6c69 7a65 2050 7974  # initialize Pyt
+00003840: 686f 6e20 436f 6e6e 6563 746f 7220 6f62  hon Connector ob
+00003850: 6a65 6374 0a63 6f6e 6e65 6374 6f72 203d  ject.connector =
+00003860: 2043 6f6e 6e65 6374 6f72 2829 0a0a 2320   Connector()..# 
+00003870: 5079 7468 6f6e 2043 6f6e 6e65 6374 6f72  Python Connector
+00003880: 2064 6174 6162 6173 6520 636f 6e6e 6563   database connec
+00003890: 7469 6f6e 2066 756e 6374 696f 6e0a 6465  tion function.de
+000038a0: 6620 6765 7463 6f6e 6e28 293a 0a20 2020  f getconn():.   
+000038b0: 2063 6f6e 6e20 3d20 636f 6e6e 6563 746f   conn = connecto
+000038c0: 722e 636f 6e6e 6563 7428 0a20 2020 2020  r.connect(.     
+000038d0: 2020 2022 7072 6f6a 6563 743a 7265 6769     "project:regi
+000038e0: 6f6e 3a69 6e73 7461 6e63 652d 6e61 6d65  on:instance-name
+000038f0: 222c 2023 2043 6c6f 7564 2053 514c 2049  ", # Cloud SQL I
+00003900: 6e73 7461 6e63 6520 436f 6e6e 6563 7469  nstance Connecti
+00003910: 6f6e 204e 616d 650a 2020 2020 2020 2020  on Name.        
+00003920: 2270 6738 3030 3022 2c0a 2020 2020 2020  "pg8000",.      
+00003930: 2020 7573 6572 3d22 6d79 2d75 7365 7222    user="my-user"
+00003940: 2c0a 2020 2020 2020 2020 7061 7373 776f  ,.        passwo
+00003950: 7264 3d22 6d79 2d70 6173 7377 6f72 6422  rd="my-password"
+00003960: 2c0a 2020 2020 2020 2020 6462 3d22 6d79  ,.        db="my
+00003970: 2d64 6174 6162 6173 6522 2c0a 2020 2020  -database",.    
+00003980: 2020 2020 6970 5f74 7970 653d 2049 5054      ip_type= IPT
+00003990: 7970 6573 2e50 5542 4c49 4320 2023 2049  ypes.PUBLIC  # I
+000039a0: 5054 7970 6573 2e50 5249 5641 5445 2066  PTypes.PRIVATE f
+000039b0: 6f72 2070 7269 7661 7465 2049 500a 2020  or private IP.  
+000039c0: 2020 290a 2020 2020 7265 7475 726e 2063    ).    return c
+000039d0: 6f6e 6e0a 0a0a 6170 7020 3d20 466c 6173  onn...app = Flas
+000039e0: 6b28 5f5f 6e61 6d65 5f5f 290a 0a23 2063  k(__name__)..# c
+000039f0: 6f6e 6669 6775 7265 2046 6c61 736b 2d53  onfigure Flask-S
+00003a00: 514c 416c 6368 656d 7920 746f 2075 7365  QLAlchemy to use
+00003a10: 2050 7974 686f 6e20 436f 6e6e 6563 746f   Python Connecto
+00003a20: 720a 6170 702e 636f 6e66 6967 5b27 5351  r.app.config['SQ
+00003a30: 4c41 4c43 4845 4d59 5f44 4154 4142 4153  LALCHEMY_DATABAS
+00003a40: 455f 5552 4927 5d20 3d20 2270 6f73 7467  E_URI'] = "postg
+00003a50: 7265 7371 6c2b 7067 3830 3030 3a2f 2f22  resql+pg8000://"
+00003a60: 0a61 7070 2e63 6f6e 6669 675b 2753 514c  .app.config['SQL
+00003a70: 414c 4348 454d 595f 454e 4749 4e45 5f4f  ALCHEMY_ENGINE_O
+00003a80: 5054 494f 4e53 275d 203d 207b 0a20 2020  PTIONS'] = {.   
+00003a90: 2022 6372 6561 746f 7222 3a20 6765 7463   "creator": getc
+00003aa0: 6f6e 6e0a 7d0a 0a23 2069 6e69 7469 616c  onn.}..# initial
+00003ab0: 697a 6520 7468 6520 6170 7020 7769 7468  ize the app with
+00003ac0: 2074 6865 2065 7874 656e 7369 6f6e 0a64   the extension.d
+00003ad0: 6220 3d20 5351 4c41 6c63 6865 6d79 2829  b = SQLAlchemy()
+00003ae0: 0a64 622e 696e 6974 5f61 7070 2861 7070  .db.init_app(app
+00003af0: 290a 6060 600a 0a46 6f72 206d 6f72 6520  ).```..For more 
+00003b00: 6465 7461 696c 7320 6f6e 2068 6f77 2074  details on how t
+00003b10: 6f20 7573 6520 466c 6173 6b2d 5351 4c41  o use Flask-SQLA
+00003b20: 6c63 6865 6d79 2c20 6368 6563 6b20 6f75  lchemy, check ou
+00003b30: 7420 7468 650a 5b46 6c61 736b 2d53 514c  t the.[Flask-SQL
+00003b40: 416c 6368 656d 7920 5175 6963 6b73 7461  Alchemy Quicksta
+00003b50: 7274 735d 2868 7474 7073 3a2f 2f66 6c61  rts](https://fla
+00003b60: 736b 2d73 716c 616c 6368 656d 792e 7061  sk-sqlalchemy.pa
+00003b70: 6c6c 6574 7370 726f 6a65 6374 732e 636f  lletsprojects.co
+00003b80: 6d2f 656e 2f33 2e30 2e78 2f71 7569 636b  m/en/3.0.x/quick
+00003b90: 7374 6172 742f 290a 0a23 2323 2320 4661  start/)..#### Fa
+00003ba0: 7374 4150 490a 0a5b 4661 7374 4150 495d  stAPI..[FastAPI]
+00003bb0: 2868 7474 7073 3a2f 2f66 6173 7461 7069  (https://fastapi
+00003bc0: 2e74 6961 6e67 6f6c 6f2e 636f 6d2f 2920  .tiangolo.com/) 
+00003bd0: 6973 2061 206d 6f64 6572 6e2c 2066 6173  is a modern, fas
+00003be0: 7420 2868 6967 682d 7065 7266 6f72 6d61  t (high-performa
+00003bf0: 6e63 6529 2c0a 7765 6220 6672 616d 6577  nce),.web framew
+00003c00: 6f72 6b20 666f 7220 6275 696c 6469 6e67  ork for building
+00003c10: 2041 5049 7320 7769 7468 2050 7974 686f   APIs with Pytho
+00003c20: 6e20 6261 7365 6420 6f6e 2073 7461 6e64  n based on stand
+00003c30: 6172 6420 5079 7468 6f6e 2074 7970 6520  ard Python type 
+00003c40: 6869 6e74 732e 0a0a 596f 7520 6361 6e20  hints...You can 
+00003c50: 636f 6e66 6967 7572 6520 4661 7374 4150  configure FastAP
+00003c60: 4920 746f 2063 6f6e 6e65 6374 2074 6f20  I to connect to 
+00003c70: 6120 436c 6f75 6420 5351 4c20 6461 7461  a Cloud SQL data
+00003c80: 6261 7365 2066 726f 6d0a 796f 7572 2077  base from.your w
+00003c90: 6562 2061 7070 6c69 6361 7469 6f6e 2075  eb application u
+00003ca0: 7369 6e67 205b 5351 4c41 6c63 6865 6d79  sing [SQLAlchemy
+00003cb0: 204f 524d 5d28 6874 7470 733a 2f2f 646f   ORM](https://do
+00003cc0: 6373 2e73 716c 616c 6368 656d 792e 6f72  cs.sqlalchemy.or
+00003cd0: 672f 656e 2f31 342f 6f72 6d2f 290a 7468  g/en/14/orm/).th
+00003ce0: 726f 7567 6820 7468 6520 666f 6c6c 6f77  rough the follow
+00003cf0: 696e 673a 0a0a 6060 6070 7974 686f 6e0a  ing:..```python.
+00003d00: 6672 6f6d 2073 716c 616c 6368 656d 7920  from sqlalchemy 
+00003d10: 696d 706f 7274 2063 7265 6174 655f 656e  import create_en
+00003d20: 6769 6e65 0a66 726f 6d20 7371 6c61 6c63  gine.from sqlalc
+00003d30: 6865 6d79 2e65 6e67 696e 6520 696d 706f  hemy.engine impo
+00003d40: 7274 2045 6e67 696e 650a 6672 6f6d 2073  rt Engine.from s
+00003d50: 716c 616c 6368 656d 792e 6578 742e 6465  qlalchemy.ext.de
+00003d60: 636c 6172 6174 6976 6520 696d 706f 7274  clarative import
+00003d70: 2064 6563 6c61 7261 7469 7665 5f62 6173   declarative_bas
+00003d80: 650a 6672 6f6d 2073 716c 616c 6368 656d  e.from sqlalchem
+00003d90: 792e 6f72 6d20 696d 706f 7274 2073 6573  y.orm import ses
+00003da0: 7369 6f6e 6d61 6b65 720a 6672 6f6d 2067  sionmaker.from g
+00003db0: 6f6f 676c 652e 636c 6f75 642e 7371 6c2e  oogle.cloud.sql.
+00003dc0: 636f 6e6e 6563 746f 7220 696d 706f 7274  connector import
+00003dd0: 2043 6f6e 6e65 6374 6f72 2c20 4950 5479   Connector, IPTy
+00003de0: 7065 730a 0a23 2068 656c 7065 7220 6675  pes..# helper fu
+00003df0: 6e63 7469 6f6e 2074 6f20 7265 7475 726e  nction to return
+00003e00: 2053 514c 416c 6368 656d 7920 636f 6e6e   SQLAlchemy conn
+00003e10: 6563 7469 6f6e 2070 6f6f 6c0a 6465 6620  ection pool.def 
+00003e20: 696e 6974 5f63 6f6e 6e65 6374 696f 6e5f  init_connection_
+00003e30: 706f 6f6c 2863 6f6e 6e65 6374 6f72 3a20  pool(connector: 
+00003e40: 436f 6e6e 6563 746f 7229 202d 3e20 456e  Connector) -> En
+00003e50: 6769 6e65 3a0a 2020 2020 2320 5079 7468  gine:.    # Pyth
+00003e60: 6f6e 2043 6f6e 6e65 6374 6f72 2064 6174  on Connector dat
+00003e70: 6162 6173 6520 636f 6e6e 6563 7469 6f6e  abase connection
+00003e80: 2066 756e 6374 696f 6e0a 2020 2020 6465   function.    de
+00003e90: 6620 6765 7463 6f6e 6e28 293a 0a20 2020  f getconn():.   
+00003ea0: 2020 2020 2063 6f6e 6e20 3d20 636f 6e6e       conn = conn
+00003eb0: 6563 746f 722e 636f 6e6e 6563 7428 0a20  ector.connect(. 
+00003ec0: 2020 2020 2020 2020 2020 2022 7072 6f6a             "proj
+00003ed0: 6563 743a 7265 6769 6f6e 3a69 6e73 7461  ect:region:insta
+00003ee0: 6e63 652d 6e61 6d65 222c 2023 2043 6c6f  nce-name", # Clo
+00003ef0: 7564 2053 514c 2049 6e73 7461 6e63 6520  ud SQL Instance 
+00003f00: 436f 6e6e 6563 7469 6f6e 204e 616d 650a  Connection Name.
+00003f10: 2020 2020 2020 2020 2020 2020 2270 6738              "pg8
+00003f20: 3030 3022 2c0a 2020 2020 2020 2020 2020  000",.          
+00003f30: 2020 7573 6572 3d22 6d79 2d75 7365 7222    user="my-user"
+00003f40: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
+00003f50: 7373 776f 7264 3d22 6d79 2d70 6173 7377  ssword="my-passw
+00003f60: 6f72 6422 2c0a 2020 2020 2020 2020 2020  ord",.          
+00003f70: 2020 6462 3d22 6d79 2d64 6174 6162 6173    db="my-databas
+00003f80: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00003f90: 6970 5f74 7970 653d 2049 5054 7970 6573  ip_type= IPTypes
+00003fa0: 2e50 5542 4c49 4320 2023 2049 5054 7970  .PUBLIC  # IPTyp
+00003fb0: 6573 2e50 5249 5641 5445 2066 6f72 2070  es.PRIVATE for p
+00003fc0: 7269 7661 7465 2049 500a 2020 2020 2020  rivate IP.      
+00003fd0: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
+00003fe0: 726e 2063 6f6e 6e0a 0a20 2020 2053 514c  rn conn..    SQL
+00003ff0: 414c 4348 454d 595f 4441 5441 4241 5345  ALCHEMY_DATABASE
+00004000: 5f55 524c 203d 2022 706f 7374 6772 6573  _URL = "postgres
+00004010: 716c 2b70 6738 3030 303a 2f2f 220a 0a20  ql+pg8000://".. 
+00004020: 2020 2065 6e67 696e 6520 3d20 6372 6561     engine = crea
+00004030: 7465 5f65 6e67 696e 6528 0a20 2020 2020  te_engine(.     
+00004040: 2020 2053 514c 414c 4348 454d 595f 4441     SQLALCHEMY_DA
+00004050: 5441 4241 5345 5f55 524c 202c 2063 7265  TABASE_URL , cre
+00004060: 6174 6f72 3d67 6574 636f 6e6e 0a20 2020  ator=getconn.   
+00004070: 2029 0a20 2020 2072 6574 7572 6e20 656e   ).    return en
+00004080: 6769 6e65 0a0a 2320 696e 6974 6961 6c69  gine..# initiali
+00004090: 7a65 2043 6c6f 7564 2053 514c 2050 7974  ze Cloud SQL Pyt
+000040a0: 686f 6e20 436f 6e6e 6563 746f 720a 636f  hon Connector.co
+000040b0: 6e6e 6563 746f 7220 3d20 436f 6e6e 6563  nnector = Connec
+000040c0: 746f 7228 290a 0a23 2063 7265 6174 6520  tor()..# create 
+000040d0: 636f 6e6e 6563 7469 6f6e 2070 6f6f 6c20  connection pool 
+000040e0: 656e 6769 6e65 0a65 6e67 696e 6520 3d20  engine.engine = 
+000040f0: 696e 6974 5f63 6f6e 6e65 6374 696f 6e5f  init_connection_
+00004100: 706f 6f6c 2863 6f6e 6e65 6374 6f72 290a  pool(connector).
+00004110: 0a23 2063 7265 6174 6520 5351 4c41 6c63  .# create SQLAlc
+00004120: 6865 6d79 204f 524d 2073 6573 7369 6f6e  hemy ORM session
+00004130: 0a53 6573 7369 6f6e 4c6f 6361 6c20 3d20  .SessionLocal = 
+00004140: 7365 7373 696f 6e6d 616b 6572 2861 7574  sessionmaker(aut
+00004150: 6f63 6f6d 6d69 743d 4661 6c73 652c 2061  ocommit=False, a
+00004160: 7574 6f66 6c75 7368 3d46 616c 7365 2c20  utoflush=False, 
+00004170: 6269 6e64 3d65 6e67 696e 6529 0a0a 4261  bind=engine)..Ba
+00004180: 7365 203d 2064 6563 6c61 7261 7469 7665  se = declarative
+00004190: 5f62 6173 6528 290a 6060 600a 0a54 6f20  _base().```..To 
+000041a0: 6c65 6172 6e20 6d6f 7265 2061 626f 7574  learn more about
+000041b0: 2069 6e74 6567 7261 7469 6e67 2061 2064   integrating a d
+000041c0: 6174 6162 6173 6520 696e 746f 2079 6f75  atabase into you
+000041d0: 7220 4661 7374 4150 4920 6170 706c 6963  r FastAPI applic
+000041e0: 6174 696f 6e2c 0a66 6f6c 6c6f 7720 616c  ation,.follow al
+000041f0: 6f6e 6720 7468 6520 5b46 6173 7441 5049  ong the [FastAPI
+00004200: 2053 514c 2044 6174 6162 6173 6520 6775   SQL Database gu
+00004210: 6964 655d 2868 7474 7073 3a2f 2f66 6173  ide](https://fas
+00004220: 7461 7069 2e74 6961 6e67 6f6c 6f2e 636f  tapi.tiangolo.co
+00004230: 6d2f 7475 746f 7269 616c 2f73 716c 2d64  m/tutorial/sql-d
+00004240: 6174 6162 6173 6573 2f23 6372 6561 7465  atabases/#create
+00004250: 2d74 6865 2d64 6174 6162 6173 652d 6d6f  -the-database-mo
+00004260: 6465 6c73 292e 0a0a 2323 2320 4173 796e  dels)...### Asyn
+00004270: 6320 4472 6976 6572 2055 7361 6765 0a0a  c Driver Usage..
+00004280: 5468 6520 436c 6f75 6420 5351 4c20 436f  The Cloud SQL Co
+00004290: 6e6e 6563 746f 7220 6973 2063 6f6d 7061  nnector is compa
+000042a0: 7469 626c 6520 7769 7468 0a5b 6173 796e  tible with.[asyn
+000042b0: 6369 6f5d 2868 7474 7073 3a2f 2f64 6f63  cio](https://doc
+000042c0: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f6c  s.python.org/3/l
+000042d0: 6962 7261 7279 2f61 7379 6e63 696f 2e68  ibrary/asyncio.h
+000042e0: 746d 6c29 2074 6f20 696d 7072 6f76 6520  tml) to improve 
+000042f0: 7468 6520 7370 6565 640a 616e 6420 6566  the speed.and ef
+00004300: 6669 6369 656e 6379 206f 6620 6461 7461  ficiency of data
+00004310: 6261 7365 2063 6f6e 6e65 6374 696f 6e73  base connections
+00004320: 2074 6872 6f75 6768 2063 6f6e 6375 7272   through concurr
+00004330: 656e 6379 2e20 596f 7520 6361 6e20 7573  ency. You can us
+00004340: 6520 616c 6c0a 6e6f 6e2d 6173 796e 6369  e all.non-asynci
+00004350: 6f20 6472 6976 6572 7320 7468 726f 7567  o drivers throug
+00004360: 6820 7468 6520 6043 6f6e 6e65 6374 6f72  h the `Connector
+00004370: 2e63 6f6e 6e65 6374 5f61 7379 6e63 6020  .connect_async` 
+00004380: 6675 6e63 7469 6f6e 2c20 696e 2061 6464  function, in add
+00004390: 6974 696f 6e0a 746f 2074 6865 2066 6f6c  ition.to the fol
+000043a0: 6c6f 7769 6e67 2061 7379 6e63 696f 2064  lowing asyncio d
+000043b0: 6174 6162 6173 6520 6472 6976 6572 733a  atabase drivers:
+000043c0: 0a2d 205b 6173 796e 6370 675d 2868 7474  .- [asyncpg](htt
+000043d0: 7073 3a2f 2f6d 6167 6963 7374 6163 6b2e  ps://magicstack.
+000043e0: 6769 7468 7562 2e69 6f2f 6173 796e 6370  github.io/asyncp
+000043f0: 6729 2028 506f 7374 6772 6573 290a 0a54  g) (Postgres)..T
+00004400: 6865 2043 6c6f 7564 2053 514c 2043 6f6e  he Cloud SQL Con
+00004410: 6e65 6374 6f72 2068 6173 2061 2068 656c  nector has a hel
+00004420: 7065 7220 6063 7265 6174 655f 6173 796e  per `create_asyn
+00004430: 635f 636f 6e6e 6563 746f 7260 2066 756e  c_connector` fun
+00004440: 6374 696f 6e20 7468 6174 2069 730a 7265  ction that is.re
+00004450: 636f 6d6d 656e 6465 6420 666f 7220 6173  commended for as
+00004460: 796e 6369 6f20 6461 7461 6261 7365 2063  yncio database c
+00004470: 6f6e 6e65 6374 696f 6e73 2e20 4974 2072  onnections. It r
+00004480: 6574 7572 6e73 2061 2060 436f 6e6e 6563  eturns a `Connec
+00004490: 746f 7260 0a6f 626a 6563 7420 7468 6174  tor`.object that
+000044a0: 2075 7365 7320 7468 6520 6375 7272 656e   uses the curren
+000044b0: 7420 7468 7265 6164 2773 2072 756e 6e69  t thread's runni
+000044c0: 6e67 2065 7665 6e74 206c 6f6f 702e 2054  ng event loop. T
+000044d0: 6869 7320 6973 2064 6966 6665 7265 6e74  his is different
+000044e0: 0a74 6861 6e20 6043 6f6e 6e65 6374 6f72  .than `Connector
+000044f0: 2829 6020 7768 6963 6820 6279 2064 6566  ()` which by def
+00004500: 6175 6c74 2069 6e69 7469 616c 697a 6573  ault initializes
+00004510: 2061 206e 6577 2065 7665 6e74 206c 6f6f   a new event loo
+00004520: 7020 696e 2061 0a62 6163 6b67 726f 756e  p in a.backgroun
+00004530: 6420 7468 7265 6164 2e0a 0a54 6865 2060  d thread...The `
+00004540: 6372 6561 7465 5f61 7379 6e63 5f63 6f6e  create_async_con
+00004550: 6e65 6374 6f72 6020 616c 6c6f 7773 2061  nector` allows a
+00004560: 6c6c 2074 6865 2073 616d 6520 696e 7075  ll the same inpu
+00004570: 7420 6172 6775 6d65 6e74 7320 6173 2074  t arguments as t
+00004580: 6865 0a5b 436f 6e6e 6563 746f 725d 2823  he.[Connector](#
+00004590: 636f 6e66 6967 7572 696e 672d 7468 652d  configuring-the-
+000045a0: 636f 6e6e 6563 746f 7229 206f 626a 6563  connector) objec
+000045b0: 742e 0a0a 4f6e 6365 2061 2060 436f 6e6e  t...Once a `Conn
+000045c0: 6563 746f 7260 206f 626a 6563 7420 6973  ector` object is
+000045d0: 2072 6574 7572 6e65 6420 6279 2060 6372   returned by `cr
+000045e0: 6561 7465 5f61 7379 6e63 5f63 6f6e 6e65  eate_async_conne
+000045f0: 6374 6f72 6020 796f 7520 6361 6e20 6361  ctor` you can ca
+00004600: 6c6c 0a69 7473 2060 636f 6e6e 6563 745f  ll.its `connect_
+00004610: 6173 796e 6360 206d 6574 686f 642c 206a  async` method, j
+00004620: 7573 7420 6173 2079 6f75 2077 6f75 6c64  ust as you would
+00004630: 2074 6865 2060 636f 6e6e 6563 7460 206d   the `connect` m
+00004640: 6574 686f 643a 0a0a 6060 6070 7974 686f  ethod:..```pytho
+00004650: 6e0a 696d 706f 7274 2061 7379 6e63 7067  n.import asyncpg
+00004660: 0a0a 696d 706f 7274 2073 716c 616c 6368  ..import sqlalch
+00004670: 656d 790a 6672 6f6d 2073 716c 616c 6368  emy.from sqlalch
+00004680: 656d 792e 6578 742e 6173 796e 6369 6f20  emy.ext.asyncio 
+00004690: 696d 706f 7274 2041 7379 6e63 456e 6769  import AsyncEngi
+000046a0: 6e65 2c20 6372 6561 7465 5f61 7379 6e63  ne, create_async
+000046b0: 5f65 6e67 696e 650a 0a66 726f 6d20 676f  _engine..from go
+000046c0: 6f67 6c65 2e63 6c6f 7564 2e73 716c 2e63  ogle.cloud.sql.c
+000046d0: 6f6e 6e65 6374 6f72 2069 6d70 6f72 7420  onnector import 
+000046e0: 436f 6e6e 6563 746f 722c 2063 7265 6174  Connector, creat
+000046f0: 655f 6173 796e 635f 636f 6e6e 6563 746f  e_async_connecto
+00004700: 720a 0a61 7379 6e63 2064 6566 2069 6e69  r..async def ini
+00004710: 745f 636f 6e6e 6563 7469 6f6e 5f70 6f6f  t_connection_poo
+00004720: 6c28 636f 6e6e 6563 746f 723a 2043 6f6e  l(connector: Con
+00004730: 6e65 6374 6f72 2920 2d3e 2041 7379 6e63  nector) -> Async
+00004740: 456e 6769 6e65 3a0a 2020 2020 2320 696e  Engine:.    # in
+00004750: 6974 6961 6c69 7a65 2043 6f6e 6e65 6374  itialize Connect
+00004760: 6f72 206f 626a 6563 7420 666f 7220 636f  or object for co
+00004770: 6e6e 6563 7469 6f6e 7320 746f 2043 6c6f  nnections to Clo
+00004780: 7564 2053 514c 0a20 2020 2061 7379 6e63  ud SQL.    async
+00004790: 2064 6566 2067 6574 636f 6e6e 2829 202d   def getconn() -
+000047a0: 3e20 6173 796e 6370 672e 436f 6e6e 6563  > asyncpg.Connec
+000047b0: 7469 6f6e 3a0a 2020 2020 2020 2020 636f  tion:.        co
+000047c0: 6e6e 3a20 6173 796e 6370 672e 436f 6e6e  nn: asyncpg.Conn
+000047d0: 6563 7469 6f6e 203d 2061 7761 6974 2063  ection = await c
+000047e0: 6f6e 6e65 6374 6f72 2e63 6f6e 6e65 6374  onnector.connect
+000047f0: 5f61 7379 6e63 280a 2020 2020 2020 2020  _async(.        
+00004800: 2020 2020 2270 726f 6a65 6374 3a72 6567      "project:reg
+00004810: 696f 6e3a 696e 7374 616e 6365 222c 2020  ion:instance",  
+00004820: 2320 436c 6f75 6420 5351 4c20 696e 7374  # Cloud SQL inst
+00004830: 616e 6365 2063 6f6e 6e65 6374 696f 6e20  ance connection 
+00004840: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
+00004850: 2022 6173 796e 6370 6722 2c0a 2020 2020   "asyncpg",.    
+00004860: 2020 2020 2020 2020 7573 6572 3d22 6d79          user="my
+00004870: 2d75 7365 7222 2c0a 2020 2020 2020 2020  -user",.        
+00004880: 2020 2020 7061 7373 776f 7264 3d22 6d79      password="my
+00004890: 2d70 6173 7377 6f72 6422 2c0a 2020 2020  -password",.    
+000048a0: 2020 2020 2020 2020 6462 3d22 6d79 2d64          db="my-d
+000048b0: 622d 6e61 6d65 220a 2020 2020 2020 2020  b-name".        
+000048c0: 2020 2020 2320 2e2e 2e20 6164 6469 7469      # ... additi
+000048d0: 6f6e 616c 2064 6174 6162 6173 6520 6472  onal database dr
+000048e0: 6976 6572 2061 7267 730a 2020 2020 2020  iver args.      
+000048f0: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
+00004900: 726e 2063 6f6e 6e0a 0a20 2020 2023 2054  rn conn..    # T
+00004910: 6865 2043 6c6f 7564 2053 514c 2050 7974  he Cloud SQL Pyt
+00004920: 686f 6e20 436f 6e6e 6563 746f 7220 6361  hon Connector ca
+00004930: 6e20 6265 2075 7365 6420 616c 6f6e 6720  n be used along 
+00004940: 7769 7468 2053 514c 416c 6368 656d 7920  with SQLAlchemy 
+00004950: 7573 696e 6720 7468 650a 2020 2020 2320  using the.    # 
+00004960: 2761 7379 6e63 5f63 7265 6174 6f72 2720  'async_creator' 
+00004970: 6172 6775 6d65 6e74 2074 6f20 2763 7265  argument to 'cre
+00004980: 6174 655f 6173 796e 635f 656e 6769 6e65  ate_async_engine
+00004990: 270a 2020 2020 706f 6f6c 203d 2063 7265  '.    pool = cre
+000049a0: 6174 655f 6173 796e 635f 656e 6769 6e65  ate_async_engine
+000049b0: 280a 2020 2020 2020 2020 2270 6f73 7467  (.        "postg
+000049c0: 7265 7371 6c2b 6173 796e 6370 673a 2f2f  resql+asyncpg://
+000049d0: 222c 0a20 2020 2020 2020 2061 7379 6e63  ",.        async
+000049e0: 5f63 7265 6174 6f72 3d67 6574 636f 6e6e  _creator=getconn
+000049f0: 2c0a 2020 2020 290a 2020 2020 7265 7475  ,.    ).    retu
+00004a00: 726e 2070 6f6f 6c0a 0a61 7379 6e63 2064  rn pool..async d
+00004a10: 6566 206d 6169 6e28 293a 0a20 2020 2023  ef main():.    #
+00004a20: 2069 6e69 7469 616c 697a 6520 436f 6e6e   initialize Conn
+00004a30: 6563 746f 7220 6f62 6a65 6374 2066 6f72  ector object for
+00004a40: 2063 6f6e 6e65 6374 696f 6e73 2074 6f20   connections to 
+00004a50: 436c 6f75 6420 5351 4c0a 2020 2020 636f  Cloud SQL.    co
+00004a60: 6e6e 6563 746f 7220 3d20 6177 6169 7420  nnector = await 
+00004a70: 6372 6561 7465 5f61 7379 6e63 5f63 6f6e  create_async_con
+00004a80: 6e65 6374 6f72 2829 0a0a 2020 2020 2320  nector()..    # 
+00004a90: 696e 6974 6961 6c69 7a65 2063 6f6e 6e65  initialize conne
+00004aa0: 6374 696f 6e20 706f 6f6c 0a20 2020 2070  ction pool.    p
+00004ab0: 6f6f 6c20 3d20 6177 6169 7420 696e 6974  ool = await init
+00004ac0: 5f63 6f6e 6e65 6374 696f 6e5f 706f 6f6c  _connection_pool
+00004ad0: 2863 6f6e 6e65 6374 6f72 290a 0a20 2020  (connector)..   
+00004ae0: 2023 2065 7861 6d70 6c65 2071 7565 7279   # example query
+00004af0: 0a20 2020 2061 7379 6e63 2077 6974 6820  .    async with 
+00004b00: 706f 6f6c 2e63 6f6e 6e65 6374 2829 2061  pool.connect() a
+00004b10: 7320 636f 6e6e 3a0a 2020 2020 2020 2020  s conn:.        
+00004b20: 6177 6169 7420 636f 6e6e 2e65 7865 6375  await conn.execu
+00004b30: 7465 2873 716c 616c 6368 656d 792e 7465  te(sqlalchemy.te
+00004b40: 7874 2822 5345 4c45 4354 204e 4f57 2829  xt("SELECT NOW()
+00004b50: 2229 290a 0a20 2020 2023 2063 6c6f 7365  "))..    # close
+00004b60: 2043 6f6e 6e65 6374 6f72 0a20 2020 2061   Connector.    a
+00004b70: 7761 6974 2063 6f6e 6e65 6374 6f72 2e63  wait connector.c
+00004b80: 6c6f 7365 5f61 7379 6e63 2829 0a0a 2020  lose_async()..  
+00004b90: 2020 2320 6469 7370 6f73 6520 6f66 2063    # dispose of c
+00004ba0: 6f6e 6e65 6374 696f 6e20 706f 6f6c 0a20  onnection pool. 
+00004bb0: 2020 2061 7761 6974 2070 6f6f 6c2e 6469     await pool.di
+00004bc0: 7370 6f73 6528 290a 6060 600a 0a46 6f72  spose().```..For
+00004bd0: 206d 6f72 6520 6465 7461 696c 7320 6f6e   more details on
+00004be0: 2061 6464 6974 696f 6e61 6c20 6461 7461   additional data
+00004bf0: 6261 7365 2061 7267 756d 656e 7473 2077  base arguments w
+00004c00: 6974 6820 616e 2060 6173 796e 6370 672e  ith an `asyncpg.
+00004c10: 436f 6e6e 6563 7469 6f6e 600a 2c20 706c  Connection`., pl
+00004c20: 6561 7365 2076 6973 6974 2074 6865 0a5b  ease visit the.[
+00004c30: 6f66 6669 6369 616c 2064 6f63 756d 656e  official documen
+00004c40: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+00004c50: 6d61 6769 6373 7461 636b 2e67 6974 6875  magicstack.githu
+00004c60: 622e 696f 2f61 7379 6e63 7067 2f63 7572  b.io/asyncpg/cur
+00004c70: 7265 6e74 2f61 7069 2f69 6e64 6578 2e68  rent/api/index.h
+00004c80: 746d 6c29 2e0a 0a23 2323 2041 7379 6e63  tml)...### Async
+00004c90: 2043 6f6e 7465 7874 204d 616e 6167 6572   Context Manager
+00004ca0: 0a0a 416e 2061 6c74 6572 6e61 7469 7665  ..An alternative
+00004cb0: 2074 6f20 7573 696e 6720 7468 6520 6063   to using the `c
+00004cc0: 7265 6174 655f 6173 796e 635f 636f 6e6e  reate_async_conn
+00004cd0: 6563 746f 7260 2066 756e 6374 696f 6e20  ector` function 
+00004ce0: 6973 2069 6e69 7469 616c 697a 696e 670a  is initializing.
+00004cf0: 6120 6043 6f6e 6e65 6374 6f72 6020 6173  a `Connector` as
+00004d00: 2061 6e20 6173 796e 6320 636f 6e74 6578   an async contex
+00004d10: 7420 6d61 6e61 6765 722c 2072 656d 6f76  t manager, remov
+00004d20: 696e 6720 7468 6520 6e65 6564 2066 6f72  ing the need for
+00004d30: 2065 7870 6c69 6369 740a 6361 6c6c 7320   explicit.calls 
+00004d40: 746f 2060 636f 6e6e 6563 746f 722e 636c  to `connector.cl
+00004d50: 6f73 655f 6173 796e 6328 2960 2074 6f20  ose_async()` to 
+00004d60: 636c 6561 6e75 7020 7265 736f 7572 6365  cleanup resource
+00004d70: 732e 0a0a 2a2a 4e6f 7465 3a2a 2a20 5468  s...**Note:** Th
+00004d80: 6973 2061 6c74 6572 6e61 7469 7665 2072  is alternative r
+00004d90: 6571 7569 7265 7320 7468 6174 2074 6865  equires that the
+00004da0: 2072 756e 6e69 6e67 2065 7665 6e74 206c   running event l
+00004db0: 6f6f 7020 6265 0a70 6173 7365 6420 696e  oop be.passed in
+00004dc0: 2061 7320 7468 6520 606c 6f6f 7060 2061   as the `loop` a
+00004dd0: 7267 756d 656e 7420 746f 2060 436f 6e6e  rgument to `Conn
+00004de0: 6563 746f 7228 2960 2e0a 0a60 6060 7079  ector()`...```py
+00004df0: 7468 6f6e 0a69 6d70 6f72 7420 6173 796e  thon.import asyn
+00004e00: 6369 6f0a 696d 706f 7274 2061 7379 6e63  cio.import async
+00004e10: 7067 0a0a 696d 706f 7274 2073 716c 616c  pg..import sqlal
+00004e20: 6368 656d 790a 6672 6f6d 2073 716c 616c  chemy.from sqlal
+00004e30: 6368 656d 792e 6578 742e 6173 796e 6369  chemy.ext.asynci
+00004e40: 6f20 696d 706f 7274 2041 7379 6e63 456e  o import AsyncEn
+00004e50: 6769 6e65 2c20 6372 6561 7465 5f61 7379  gine, create_asy
+00004e60: 6e63 5f65 6e67 696e 650a 0a66 726f 6d20  nc_engine..from 
+00004e70: 676f 6f67 6c65 2e63 6c6f 7564 2e73 716c  google.cloud.sql
+00004e80: 2e63 6f6e 6e65 6374 6f72 2069 6d70 6f72  .connector impor
+00004e90: 7420 436f 6e6e 6563 746f 720a 0a61 7379  t Connector..asy
+00004ea0: 6e63 2064 6566 2069 6e69 745f 636f 6e6e  nc def init_conn
+00004eb0: 6563 7469 6f6e 5f70 6f6f 6c28 636f 6e6e  ection_pool(conn
+00004ec0: 6563 746f 723a 2043 6f6e 6e65 6374 6f72  ector: Connector
+00004ed0: 2920 2d3e 2041 7379 6e63 456e 6769 6e65  ) -> AsyncEngine
+00004ee0: 3a0a 2020 2020 2320 696e 6974 6961 6c69  :.    # initiali
+00004ef0: 7a65 2043 6f6e 6e65 6374 6f72 206f 626a  ze Connector obj
+00004f00: 6563 7420 666f 7220 636f 6e6e 6563 7469  ect for connecti
+00004f10: 6f6e 7320 746f 2043 6c6f 7564 2053 514c  ons to Cloud SQL
+00004f20: 0a20 2020 2061 7379 6e63 2064 6566 2067  .    async def g
+00004f30: 6574 636f 6e6e 2829 202d 3e20 6173 796e  etconn() -> asyn
+00004f40: 6370 672e 436f 6e6e 6563 7469 6f6e 3a0a  cpg.Connection:.
+00004f50: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
+00004f60: 3a20 6173 796e 6370 672e 436f 6e6e 6563  : asyncpg.Connec
+00004f70: 7469 6f6e 203d 2061 7761 6974 2063 6f6e  tion = await con
+00004f80: 6e65 6374 6f72 2e63 6f6e 6e65 6374 5f61  nector.connect_a
+00004f90: 7379 6e63 280a 2020 2020 2020 2020 2020  sync(.          
+00004fa0: 2020 2020 2020 2270 726f 6a65 6374 3a72        "project:r
+00004fb0: 6567 696f 6e3a 696e 7374 616e 6365 222c  egion:instance",
+00004fc0: 2020 2320 436c 6f75 6420 5351 4c20 696e    # Cloud SQL in
+00004fd0: 7374 616e 6365 2063 6f6e 6e65 6374 696f  stance connectio
+00004fe0: 6e20 6e61 6d65 0a20 2020 2020 2020 2020  n name.         
+00004ff0: 2020 2020 2020 2022 6173 796e 6370 6722         "asyncpg"
+00005000: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005010: 2020 7573 6572 3d22 6d79 2d75 7365 7222    user="my-user"
+00005020: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005030: 2020 7061 7373 776f 7264 3d22 6d79 2d70    password="my-p
+00005040: 6173 7377 6f72 6422 2c0a 2020 2020 2020  assword",.      
+00005050: 2020 2020 2020 2020 2020 6462 3d22 6d79            db="my
+00005060: 2d64 622d 6e61 6d65 220a 2020 2020 2020  -db-name".      
+00005070: 2020 2020 2020 2020 2020 2320 2e2e 2e20            # ... 
+00005080: 6164 6469 7469 6f6e 616c 2064 6174 6162  additional datab
+00005090: 6173 6520 6472 6976 6572 2061 7267 730a  ase driver args.
+000050a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000050b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000050c0: 2063 6f6e 6e0a 0a20 2020 2023 2054 6865   conn..    # The
+000050d0: 2043 6c6f 7564 2053 514c 2050 7974 686f   Cloud SQL Pytho
+000050e0: 6e20 436f 6e6e 6563 746f 7220 6361 6e20  n Connector can 
+000050f0: 6265 2075 7365 6420 616c 6f6e 6720 7769  be used along wi
+00005100: 7468 2053 514c 416c 6368 656d 7920 7573  th SQLAlchemy us
+00005110: 696e 6720 7468 650a 2020 2020 2320 2761  ing the.    # 'a
+00005120: 7379 6e63 5f63 7265 6174 6f72 2720 6172  sync_creator' ar
+00005130: 6775 6d65 6e74 2074 6f20 2763 7265 6174  gument to 'creat
+00005140: 655f 6173 796e 635f 656e 6769 6e65 270a  e_async_engine'.
+00005150: 2020 2020 706f 6f6c 203d 2063 7265 6174      pool = creat
+00005160: 655f 6173 796e 635f 656e 6769 6e65 280a  e_async_engine(.
+00005170: 2020 2020 2020 2020 2270 6f73 7467 7265          "postgre
+00005180: 7371 6c2b 6173 796e 6370 673a 2f2f 222c  sql+asyncpg://",
+00005190: 0a20 2020 2020 2020 2061 7379 6e63 5f63  .        async_c
+000051a0: 7265 6174 6f72 3d67 6574 636f 6e6e 2c0a  reator=getconn,.
+000051b0: 2020 2020 290a 2020 2020 7265 7475 726e      ).    return
+000051c0: 2070 6f6f 6c0a 0a61 7379 6e63 2064 6566   pool..async def
+000051d0: 206d 6169 6e28 293a 0a20 2020 2023 2069   main():.    # i
+000051e0: 6e69 7469 616c 697a 6520 436f 6e6e 6563  nitialize Connec
+000051f0: 746f 7220 6f62 6a65 6374 2066 6f72 2063  tor object for c
+00005200: 6f6e 6e65 6374 696f 6e73 2074 6f20 436c  onnections to Cl
+00005210: 6f75 6420 5351 4c0a 2020 2020 6c6f 6f70  oud SQL.    loop
+00005220: 203d 2061 7379 6e63 696f 2e67 6574 5f72   = asyncio.get_r
+00005230: 756e 6e69 6e67 5f6c 6f6f 7028 290a 2020  unning_loop().  
+00005240: 2020 6173 796e 6320 7769 7468 2043 6f6e    async with Con
+00005250: 6e65 6374 6f72 286c 6f6f 703d 6c6f 6f70  nector(loop=loop
+00005260: 2920 6173 2063 6f6e 6e65 6374 6f72 3a0a  ) as connector:.
+00005270: 2020 2020 2020 2020 2320 696e 6974 6961          # initia
+00005280: 6c69 7a65 2063 6f6e 6e65 6374 696f 6e20  lize connection 
+00005290: 706f 6f6c 0a20 2020 2020 2020 2070 6f6f  pool.        poo
+000052a0: 6c20 3d20 6177 6169 7420 696e 6974 5f63  l = await init_c
+000052b0: 6f6e 6e65 6374 696f 6e5f 706f 6f6c 2863  onnection_pool(c
+000052c0: 6f6e 6e65 6374 6f72 290a 0a20 2020 2020  onnector)..     
+000052d0: 2020 2023 2065 7861 6d70 6c65 2071 7565     # example que
+000052e0: 7279 0a20 2020 2020 2020 2061 7379 6e63  ry.        async
+000052f0: 2077 6974 6820 706f 6f6c 2e63 6f6e 6e65   with pool.conne
+00005300: 6374 2829 2061 7320 636f 6e6e 3a0a 2020  ct() as conn:.  
+00005310: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00005320: 636f 6e6e 2e65 7865 6375 7465 2873 716c  conn.execute(sql
+00005330: 616c 6368 656d 792e 7465 7874 2822 5345  alchemy.text("SE
+00005340: 4c45 4354 204e 4f57 2829 2229 290a 0a20  LECT NOW()")).. 
+00005350: 2020 2020 2020 2023 2064 6973 706f 7365         # dispose
+00005360: 206f 6620 636f 6e6e 6563 7469 6f6e 2070   of connection p
+00005370: 6f6f 6c0a 2020 2020 2020 2020 6177 6169  ool.        awai
+00005380: 7420 706f 6f6c 2e64 6973 706f 7365 2829  t pool.dispose()
+00005390: 0a60 6060 0a0a 2323 2053 7570 706f 7274  .```..## Support
+000053a0: 2070 6f6c 6963 790a 0a23 2323 204d 616a   policy..### Maj
+000053b0: 6f72 2076 6572 7369 6f6e 206c 6966 6563  or version lifec
+000053c0: 7963 6c65 0a0a 5468 6973 2070 726f 6a65  ycle..This proje
+000053d0: 6374 2075 7365 7320 5b73 656d 616e 7469  ct uses [semanti
+000053e0: 6320 7665 7273 696f 6e69 6e67 5d28 6874  c versioning](ht
+000053f0: 7470 733a 2f2f 7365 6d76 6572 2e6f 7267  tps://semver.org
+00005400: 2f29 2c20 616e 6420 7573 6573 2074 6865  /), and uses the
+00005410: 0a66 6f6c 6c6f 7769 6e67 206c 6966 6563  .following lifec
+00005420: 7963 6c65 2072 6567 6172 6469 6e67 2073  ycle regarding s
+00005430: 7570 706f 7274 2066 6f72 2061 206d 616a  upport for a maj
+00005440: 6f72 2076 6572 7369 6f6e 3a0a 0a2a 2a41  or version:..**A
+00005450: 6374 6976 652a 2a20 2d20 4163 7469 7665  ctive** - Active
+00005460: 2076 6572 7369 6f6e 7320 6765 7420 616c   versions get al
+00005470: 6c20 6e65 7720 6665 6174 7572 6573 2061  l new features a
+00005480: 6e64 2073 6563 7572 6974 7920 6669 7865  nd security fixe
+00005490: 7320 2874 6861 740a 776f 756c 646e e280  s (that.wouldn..
+000054a0: 9974 206f 7468 6572 7769 7365 2069 6e74  .t otherwise int
+000054b0: 726f 6475 6365 2061 2062 7265 616b 696e  roduce a breakin
+000054c0: 6720 6368 616e 6765 292e 204e 6577 206d  g change). New m
+000054d0: 616a 6f72 2076 6572 7369 6f6e 7320 6172  ajor versions ar
+000054e0: 650a 6775 6172 616e 7465 6564 2074 6f20  e.guaranteed to 
+000054f0: 6265 2022 6163 7469 7665 2220 666f 7220  be "active" for 
+00005500: 6120 6d69 6e69 6d75 6d20 6f66 2031 2079  a minimum of 1 y
+00005510: 6561 722e 0a2a 2a44 6570 7265 6361 7465  ear..**Deprecate
+00005520: 642a 2a20 2d20 4465 7072 6563 6174 6564  d** - Deprecated
+00005530: 2076 6572 7369 6f6e 7320 636f 6e74 696e   versions contin
+00005540: 7565 2074 6f20 7265 6365 6976 6520 7365  ue to receive se
+00005550: 6375 7269 7479 2061 6e64 2063 7269 7469  curity and criti
+00005560: 6361 6c0a 6275 6720 6669 7865 732c 2062  cal.bug fixes, b
+00005570: 7574 2064 6f20 6e6f 7420 7265 6365 6976  ut do not receiv
+00005580: 6520 6e65 7720 6665 6174 7572 6573 2e20  e new features. 
+00005590: 4465 7072 6563 6174 6564 2076 6572 7369  Deprecated versi
+000055a0: 6f6e 7320 7769 6c6c 2062 6520 7075 626c  ons will be publ
+000055b0: 6963 6c79 0a73 7570 706f 7274 6564 2066  icly.supported f
+000055c0: 6f72 2031 2079 6561 722e 0a2a 2a55 6e73  or 1 year..**Uns
+000055d0: 7570 706f 7274 6564 2a2a 202d 2041 6e79  upported** - Any
+000055e0: 206d 616a 6f72 2076 6572 7369 6f6e 2074   major version t
+000055f0: 6861 7420 6861 7320 6265 656e 2064 6570  hat has been dep
+00005600: 7265 6361 7465 6420 666f 7220 3e3d 3120  recated for >=1 
+00005610: 7965 6172 2069 730a 636f 6e73 6964 6572  year is.consider
+00005620: 6564 2070 7562 6c69 636c 7920 756e 7375  ed publicly unsu
+00005630: 7070 6f72 7465 642e 0a0a 2323 2053 7570  pported...## Sup
+00005640: 706f 7274 6564 2050 7974 686f 6e20 5665  ported Python Ve
+00005650: 7273 696f 6e73 0a0a 5765 2066 6f6c 6c6f  rsions..We follo
+00005660: 7720 7468 6520 5b50 7974 686f 6e20 5665  w the [Python Ve
+00005670: 7273 696f 6e20 5375 7070 6f72 7420 506f  rsion Support Po
+00005680: 6c69 6379 5d5b 7079 7665 725d 2075 7365  licy][pyver] use
+00005690: 6420 6279 2047 6f6f 676c 6520 436c 6f75  d by Google Clou
+000056a0: 640a 4c69 6272 6172 6965 7320 666f 7220  d.Libraries for 
+000056b0: 5079 7468 6f6e 2e20 4368 616e 6765 7320  Python. Changes 
+000056c0: 696e 2073 7570 706f 7274 6564 2050 7974  in supported Pyt
+000056d0: 686f 6e20 7665 7273 696f 6e73 2077 696c  hon versions wil
+000056e0: 6c20 6265 0a63 6f6e 7369 6465 7265 6420  l be.considered 
+000056f0: 6120 6d69 6e6f 7220 6368 616e 6765 2c20  a minor change, 
+00005700: 616e 6420 7769 6c6c 2062 6520 6c69 7374  and will be list
+00005710: 6564 2069 6e20 7468 6520 7265 6c65 6173  ed in the releas
+00005720: 6520 6e6f 7465 732e 0a0a 5b70 7976 6572  e notes...[pyver
+00005730: 5d3a 2068 7474 7073 3a2f 2f63 6c6f 7564  ]: https://cloud
+00005740: 2e67 6f6f 676c 652e 636f 6d2f 7079 7468  .google.com/pyth
+00005750: 6f6e 2f64 6f63 732f 7375 7070 6f72 7465  on/docs/supporte
+00005760: 642d 7079 7468 6f6e 2d76 6572 7369 6f6e  d-python-version
+00005770: 730a 0a23 2323 2052 656c 6561 7365 2063  s..### Release c
+00005780: 6164 656e 6365 0a54 6869 7320 7072 6f6a  adence.This proj
+00005790: 6563 7420 6169 6d73 2066 6f72 2061 206d  ect aims for a m
+000057a0: 696e 696d 756d 206d 6f6e 7468 6c79 2072  inimum monthly r
+000057b0: 656c 6561 7365 2063 6164 656e 6365 2e20  elease cadence. 
+000057c0: 4966 206e 6f20 6e65 770a 6665 6174 7572  If no new.featur
+000057d0: 6573 206f 7220 6669 7865 7320 6861 7665  es or fixes have
+000057e0: 2062 6565 6e20 6164 6465 642c 2061 206e   been added, a n
+000057f0: 6577 2050 4154 4348 2076 6572 7369 6f6e  ew PATCH version
+00005800: 2077 6974 6820 7468 6520 6c61 7465 7374   with the latest
+00005810: 0a64 6570 656e 6465 6e63 6965 7320 6973  .dependencies is
+00005820: 2072 656c 6561 7365 642e 0a0a 2323 2320   released...### 
+00005830: 436f 6e74 7269 6275 7469 6e67 0a0a 5765  Contributing..We
+00005840: 2077 656c 636f 6d65 206f 7574 7369 6465   welcome outside
+00005850: 2063 6f6e 7472 6962 7574 696f 6e73 2e20   contributions. 
+00005860: 506c 6561 7365 2073 6565 206f 7572 0a5b  Please see our.[
+00005870: 436f 6e74 7269 6275 7469 6e67 2047 7569  Contributing Gui
+00005880: 6465 5d28 434f 4e54 5249 4255 5449 4e47  de](CONTRIBUTING
+00005890: 2e6d 6429 2066 6f72 2064 6574 6169 6c73  .md) for details
+000058a0: 206f 6e20 686f 7720 6265 7374 2074 6f20   on how best to 
+000058b0: 636f 6e74 7269 6275 7465 2e0a            contribute..
```

### Comparing `cloud-sql-python-connector-1.2.4/cloud_sql_python_connector.egg-info/PKG-INFO` & `cloud-sql-python-connector-1.3.0/cloud_sql_python_connector.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 636c 6f75  : 2.1.Name: clou
 00000020: 642d 7371 6c2d 7079 7468 6f6e 2d63 6f6e  d-sql-python-con
 00000030: 6e65 6374 6f72 0a56 6572 7369 6f6e 3a20  nector.Version: 
-00000040: 312e 322e 340a 5375 6d6d 6172 793a 2054  1.2.4.Summary: T
+00000040: 312e 332e 300a 5375 6d6d 6172 793a 2054  1.3.0.Summary: T
 00000050: 6865 2043 6c6f 7564 2053 514c 2050 7974  he Cloud SQL Pyt
 00000060: 686f 6e20 436f 6e6e 6563 746f 7220 6973  hon Connector is
 00000070: 2061 206c 6962 7261 7279 2074 6861 7420   a library that 
 00000080: 6361 6e20 6265 2075 7365 6420 616c 6f6e  can be used alon
 00000090: 6773 6964 6520 6120 6461 7461 6261 7365  gside a database
 000000a0: 2064 7269 7665 7220 746f 2061 6c6c 6f77   driver to allow
 000000b0: 2075 7365 7273 2077 6974 6820 7375 6666   users with suff
@@ -41,1365 +41,1449 @@
 00000280: 726f 7665 6420 3a3a 2041 7061 6368 6520  roved :: Apache 
 00000290: 536f 6674 7761 7265 204c 6963 656e 7365  Software License
 000002a0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
 000002b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 000002c0: 6520 3a3a 2050 7974 686f 6e0a 436c 6173  e :: Python.Clas
 000002d0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
 000002e0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000002f0: 5079 7468 6f6e 203a 3a20 332e 370a 436c  Python :: 3.7.Cl
+000002f0: 5079 7468 6f6e 203a 3a20 332e 380a 436c  Python :: 3.8.Cl
 00000300: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
 00000310: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000320: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
+00000320: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
 00000330: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
 00000340: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 00000350: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000360: 390a 436c 6173 7369 6669 6572 3a20 5072  9.Classifier: Pr
-00000370: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000380: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000390: 332e 3130 0a43 6c61 7373 6966 6965 723a  3.10.Classifier:
-000003a0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000003b0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000003c0: 3a3a 2033 2e31 310a 5265 7175 6972 6573  :: 3.11.Requires
-000003d0: 2d50 7974 686f 6e3a 203e 3d33 2e37 0a44  -Python: >=3.7.D
-000003e0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-000003f0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-00000400: 726b 646f 776e 0a50 726f 7669 6465 732d  rkdown.Provides-
-00000410: 4578 7472 613a 2070 796d 7973 716c 0a50  Extra: pymysql.P
-00000420: 726f 7669 6465 732d 4578 7472 613a 2070  rovides-Extra: p
-00000430: 6738 3030 300a 5072 6f76 6964 6573 2d45  g8000.Provides-E
-00000440: 7874 7261 3a20 7079 7464 730a 5072 6f76  xtra: pytds.Prov
-00000450: 6964 6573 2d45 7874 7261 3a20 6173 796e  ides-Extra: asyn
-00000460: 6370 670a 4c69 6365 6e73 652d 4669 6c65  cpg.License-File
-00000470: 3a20 4c49 4345 4e53 450a 0a3c 7020 616c  : LICENSE..<p al
-00000480: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
-00000490: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-000004a0: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
-000004b0: 636f 6d2f 626c 6f67 2f74 6f70 6963 732f  com/blog/topics/
-000004c0: 6465 7665 6c6f 7065 7273 2d70 7261 6374  developers-pract
-000004d0: 6974 696f 6e65 7273 2f68 6f77 2d63 6f6e  itioners/how-con
-000004e0: 6e65 6374 2d63 6c6f 7564 2d73 716c 2d75  nect-cloud-sql-u
-000004f0: 7369 6e67 2d70 7974 686f 6e2d 6561 7379  sing-python-easy
-00000500: 2d77 6179 223e 0a20 2020 2020 2020 203c  -way">.        <
-00000510: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000520: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00000530: 6f6e 7465 6e74 2e63 6f6d 2f47 6f6f 676c  ontent.com/Googl
-00000540: 6543 6c6f 7564 506c 6174 666f 726d 2f63  eCloudPlatform/c
-00000550: 6c6f 7564 2d73 716c 2d70 7974 686f 6e2d  loud-sql-python-
-00000560: 636f 6e6e 6563 746f 722f 6d61 696e 2f64  connector/main/d
-00000570: 6f63 732f 696d 6167 6573 2f63 6c6f 7564  ocs/images/cloud
-00000580: 2d73 716c 2d70 7974 686f 6e2d 636f 6e6e  -sql-python-conn
-00000590: 6563 746f 722e 706e 6722 2061 6c74 3d22  ector.png" alt="
-000005a0: 636c 6f75 642d 7371 6c2d 7079 7468 6f6e  cloud-sql-python
-000005b0: 2d63 6f6e 6e65 6374 6f72 2069 6d61 6765  -connector image
-000005c0: 223e 0a20 2020 203c 2f61 3e0a 3c2f 703e  ">.    </a>.</p>
-000005d0: 0a0a 3c68 3120 616c 6967 6e3d 2263 656e  ..<h1 align="cen
-000005e0: 7465 7222 3e43 6c6f 7564 2053 514c 2050  ter">Cloud SQL P
-000005f0: 7974 686f 6e20 436f 6e6e 6563 746f 723c  ython Connector<
-00000600: 2f68 313e 0a0a 5b21 5b4f 7065 6e20 496e  /h1>..[![Open In
-00000610: 2043 6f6c 6162 5d5b 636f 6c61 622d 6261   Colab][colab-ba
-00000620: 6467 655d 5d5b 636f 6c61 622d 6e6f 7465  dge]][colab-note
-00000630: 626f 6f6b 5d0a 5b21 5b43 495d 5b63 692d  book].[![CI][ci-
-00000640: 6261 6467 655d 5d5b 6369 2d62 7569 6c64  badge]][ci-build
-00000650: 5d0a 5b21 5b70 7970 695d 5b70 7970 692d  ].[![pypi][pypi-
-00000660: 6261 6467 655d 5d5b 7079 7069 2d64 6f63  badge]][pypi-doc
-00000670: 735d 0a5b 215b 5079 5049 2064 6f77 6e6c  s].[![PyPI downl
-00000680: 6f61 6420 6d6f 6e74 685d 5b70 7970 692d  oad month][pypi-
-00000690: 646f 776e 6c6f 6164 735d 5d5b 7079 7069  downloads]][pypi
-000006a0: 2d64 6f63 735d 0a5b 215b 7079 7468 6f6e  -docs].[![python
-000006b0: 5d5b 7079 7468 6f6e 2d76 6572 7369 6f6e  ][python-version
-000006c0: 735d 5d5b 7079 7069 2d64 6f63 735d 0a0a  s]][pypi-docs]..
-000006d0: 5b63 6f6c 6162 2d62 6164 6765 5d3a 2068  [colab-badge]: h
-000006e0: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
-000006f0: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
-00000700: 2f61 7373 6574 732f 636f 6c61 622d 6261  /assets/colab-ba
-00000710: 6467 652e 7376 670a 5b63 6f6c 6162 2d6e  dge.svg.[colab-n
-00000720: 6f74 6562 6f6f 6b5d 3a20 6874 7470 733a  otebook]: https:
-00000730: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-00000740: 2e67 6f6f 676c 652e 636f 6d2f 6769 7468  .google.com/gith
-00000750: 7562 2f47 6f6f 676c 6543 6c6f 7564 506c  ub/GoogleCloudPl
-00000760: 6174 666f 726d 2f63 6c6f 7564 2d73 716c  atform/cloud-sql
-00000770: 2d70 7974 686f 6e2d 636f 6e6e 6563 746f  -python-connecto
-00000780: 722f 626c 6f62 2f6d 6169 6e2f 7361 6d70  r/blob/main/samp
-00000790: 6c65 732f 6e6f 7465 626f 6f6b 732f 706f  les/notebooks/po
-000007a0: 7374 6772 6573 5f70 7974 686f 6e5f 636f  stgres_python_co
-000007b0: 6e6e 6563 746f 722e 6970 796e 620a 5b63  nnector.ipynb.[c
-000007c0: 692d 6261 6467 655d 3a20 6874 7470 733a  i-badge]: https:
-000007d0: 2f2f 6769 7468 7562 2e63 6f6d 2f47 6f6f  //github.com/Goo
-000007e0: 676c 6543 6c6f 7564 506c 6174 666f 726d  gleCloudPlatform
-000007f0: 2f63 6c6f 7564 2d73 716c 2d70 7974 686f  /cloud-sql-pytho
-00000800: 6e2d 636f 6e6e 6563 746f 722f 6163 7469  n-connector/acti
-00000810: 6f6e 732f 776f 726b 666c 6f77 732f 7465  ons/workflows/te
-00000820: 7374 732e 796d 6c2f 6261 6467 652e 7376  sts.yml/badge.sv
-00000830: 673f 6576 656e 743d 7075 7368 0a5b 6369  g?event=push.[ci
-00000840: 2d62 7569 6c64 5d3a 2068 7474 7073 3a2f  -build]: https:/
-00000850: 2f67 6974 6875 622e 636f 6d2f 476f 6f67  /github.com/Goog
-00000860: 6c65 436c 6f75 6450 6c61 7466 6f72 6d2f  leCloudPlatform/
-00000870: 636c 6f75 642d 7371 6c2d 7079 7468 6f6e  cloud-sql-python
-00000880: 2d63 6f6e 6e65 6374 6f72 2f61 6374 696f  -connector/actio
-00000890: 6e73 2f77 6f72 6b66 6c6f 7773 2f74 6573  ns/workflows/tes
-000008a0: 7473 2e79 6d6c 3f71 7565 7279 3d65 7665  ts.yml?query=eve
-000008b0: 6e74 2533 4170 7573 682b 6272 616e 6368  nt%3Apush+branch
-000008c0: 2533 416d 6169 6e0a 5b70 7970 692d 6261  %3Amain.[pypi-ba
-000008d0: 6467 655d 3a20 6874 7470 733a 2f2f 696d  dge]: https://im
-000008e0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-000008f0: 692f 762f 636c 6f75 642d 7371 6c2d 7079  i/v/cloud-sql-py
-00000900: 7468 6f6e 2d63 6f6e 6e65 6374 6f72 0a5b  thon-connector.[
-00000910: 7079 7069 2d64 6f63 735d 3a20 6874 7470  pypi-docs]: http
-00000920: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000930: 6a65 6374 2f63 6c6f 7564 2d73 716c 2d70  ject/cloud-sql-p
-00000940: 7974 686f 6e2d 636f 6e6e 6563 746f 720a  ython-connector.
-00000950: 5b70 7970 692d 646f 776e 6c6f 6164 735d  [pypi-downloads]
-00000960: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00000970: 6965 6c64 732e 696f 2f70 7970 692f 646d  ields.io/pypi/dm
-00000980: 2f63 6c6f 7564 2d73 716c 2d70 7974 686f  /cloud-sql-pytho
-00000990: 6e2d 636f 6e6e 6563 746f 722e 7376 670a  n-connector.svg.
-000009a0: 5b70 7974 686f 6e2d 7665 7273 696f 6e73  [python-versions
-000009b0: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
-000009c0: 6869 656c 6473 2e69 6f2f 7079 7069 2f70  hields.io/pypi/p
-000009d0: 7976 6572 7369 6f6e 732f 636c 6f75 642d  yversions/cloud-
-000009e0: 7371 6c2d 7079 7468 6f6e 2d63 6f6e 6e65  sql-python-conne
-000009f0: 6374 6f72 0a0a 5468 6520 5f43 6c6f 7564  ctor..The _Cloud
-00000a00: 2053 514c 2050 7974 686f 6e20 436f 6e6e   SQL Python Conn
-00000a10: 6563 746f 725f 2069 7320 6120 436c 6f75  ector_ is a Clou
-00000a20: 6420 5351 4c20 636f 6e6e 6563 746f 7220  d SQL connector 
-00000a30: 6465 7369 676e 6564 2066 6f72 2075 7365  designed for use
-00000a40: 2077 6974 6820 7468 650a 5079 7468 6f6e   with the.Python
-00000a50: 206c 616e 6775 6167 652e 2055 7369 6e67   language. Using
-00000a60: 2061 2043 6c6f 7564 2053 514c 2063 6f6e   a Cloud SQL con
-00000a70: 6e65 6374 6f72 2070 726f 7669 6465 7320  nector provides 
-00000a80: 7468 6520 666f 6c6c 6f77 696e 6720 6265  the following be
-00000a90: 6e65 6669 7473 3a0a 2a20 2a2a 4941 4d20  nefits:.* **IAM 
-00000aa0: 4175 7468 6f72 697a 6174 696f 6e3a 2a2a  Authorization:**
-00000ab0: 2075 7365 7320 4941 4d20 7065 726d 6973   uses IAM permis
-00000ac0: 7369 6f6e 7320 746f 2063 6f6e 7472 6f6c  sions to control
-00000ad0: 2077 686f 2f77 6861 7420 6361 6e20 636f   who/what can co
-00000ae0: 6e6e 6563 7420 746f 0a20 2079 6f75 7220  nnect to.  your 
-00000af0: 436c 6f75 6420 5351 4c20 696e 7374 616e  Cloud SQL instan
-00000b00: 6365 730a 2a20 2a2a 496d 7072 6f76 6564  ces.* **Improved
-00000b10: 2053 6563 7572 6974 793a 2a2a 2075 7365   Security:** use
-00000b20: 7320 726f 6275 7374 2c20 7570 6461 7465  s robust, update
-00000b30: 6420 544c 5320 312e 3320 656e 6372 7970  d TLS 1.3 encryp
-00000b40: 7469 6f6e 2061 6e64 0a20 2069 6465 6e74  tion and.  ident
-00000b50: 6974 7920 7665 7269 6669 6361 7469 6f6e  ity verification
-00000b60: 2062 6574 7765 656e 2074 6865 2063 6c69   between the cli
-00000b70: 656e 7420 636f 6e6e 6563 746f 7220 616e  ent connector an
-00000b80: 6420 7468 6520 7365 7276 6572 2d73 6964  d the server-sid
-00000b90: 6520 7072 6f78 792c 0a20 2069 6e64 6570  e proxy,.  indep
-00000ba0: 656e 6465 6e74 206f 6620 7468 6520 6461  endent of the da
-00000bb0: 7461 6261 7365 2070 726f 746f 636f 6c2e  tabase protocol.
-00000bc0: 0a2a 202a 2a43 6f6e 7665 6e69 656e 6365  .* **Convenience
-00000bd0: 3a2a 2a20 7265 6d6f 7665 7320 7468 6520  :** removes the 
-00000be0: 7265 7175 6972 656d 656e 7420 746f 2075  requirement to u
-00000bf0: 7365 2061 6e64 2064 6973 7472 6962 7574  se and distribut
-00000c00: 6520 5353 4c0a 2020 6365 7274 6966 6963  e SSL.  certific
-00000c10: 6174 6573 2c20 6173 2077 656c 6c20 6173  ates, as well as
-00000c20: 206d 616e 6167 6520 6669 7265 7761 6c6c   manage firewall
-00000c30: 7320 6f72 2073 6f75 7263 652f 6465 7374  s or source/dest
-00000c40: 696e 6174 696f 6e20 4950 2061 6464 7265  ination IP addre
-00000c50: 7373 6573 2e0a 2a20 286f 7074 696f 6e61  sses..* (optiona
-00000c60: 6c6c 7929 202a 2a49 414d 2044 4220 4175  lly) **IAM DB Au
-00000c70: 7468 656e 7469 6361 7469 6f6e 3a2a 2a20  thentication:** 
-00000c80: 7072 6f76 6964 6573 2073 7570 706f 7274  provides support
-00000c90: 2066 6f72 0a20 205b 436c 6f75 6420 5351   for.  [Cloud SQ
-00000ca0: 4ce2 8099 7320 6175 746f 6d61 7469 6320  L...s automatic 
-00000cb0: 4941 4d20 4442 2041 7574 684e 5d5b 6961  IAM DB AuthN][ia
-00000cc0: 6d2d 6462 2d61 7574 686e 5d20 6665 6174  m-db-authn] feat
-00000cd0: 7572 652e 0a0a 5b69 616d 2d64 622d 6175  ure...[iam-db-au
-00000ce0: 7468 6e5d 3a20 6874 7470 733a 2f2f 636c  thn]: https://cl
-00000cf0: 6f75 642e 676f 6f67 6c65 2e63 6f6d 2f73  oud.google.com/s
-00000d00: 716c 2f64 6f63 732f 706f 7374 6772 6573  ql/docs/postgres
-00000d10: 2f61 7574 6865 6e74 6963 6174 696f 6e0a  /authentication.
-00000d20: 0a54 6865 2043 6c6f 7564 2053 514c 2050  .The Cloud SQL P
-00000d30: 7974 686f 6e20 436f 6e6e 6563 746f 7220  ython Connector 
-00000d40: 6973 2061 2070 6163 6b61 6765 2074 6f20  is a package to 
-00000d50: 6265 2075 7365 6420 616c 6f6e 6773 6964  be used alongsid
-00000d60: 6520 6120 6461 7461 6261 7365 2064 7269  e a database dri
-00000d70: 7665 722e 0a43 7572 7265 6e74 6c79 2073  ver..Currently s
-00000d80: 7570 706f 7274 6564 2064 7269 7665 7273  upported drivers
-00000d90: 2061 7265 3a0a 202d 205b 6070 796d 7973   are:. - [`pymys
-00000da0: 716c 605d 2868 7474 7073 3a2f 2f67 6974  ql`](https://git
-00000db0: 6875 622e 636f 6d2f 5079 4d79 5351 4c2f  hub.com/PyMySQL/
-00000dc0: 5079 4d79 5351 4c29 2028 4d79 5351 4c29  PyMySQL) (MySQL)
-00000dd0: 0a20 2d20 5b60 7067 3830 3030 605d 2868  . - [`pg8000`](h
-00000de0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000df0: 6d2f 746c 6f63 6b65 2f70 6738 3030 3029  m/tlocke/pg8000)
-00000e00: 2028 506f 7374 6772 6553 514c 290a 202d   (PostgreSQL). -
-00000e10: 205b 6061 7379 6e63 7067 605d 2868 7474   [`asyncpg`](htt
-00000e20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000e30: 4d61 6769 6353 7461 636b 2f61 7379 6e63  MagicStack/async
-00000e40: 7067 2920 2850 6f73 7467 7265 5351 4c29  pg) (PostgreSQL)
-00000e50: 0a20 2d20 5b60 7079 7464 7360 5d28 6874  . - [`pytds`](ht
-00000e60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000e70: 2f64 656e 6973 656e 6b6f 6d2f 7079 7464  /denisenkom/pytd
-00000e80: 7329 2028 5351 4c20 5365 7276 6572 290a  s) (SQL Server).
-00000e90: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-00000ea0: 6e0a 0a59 6f75 2063 616e 2069 6e73 7461  n..You can insta
-00000eb0: 6c6c 2074 6869 7320 6c69 6272 6172 7920  ll this library 
-00000ec0: 7769 7468 2060 7069 7020 696e 7374 616c  with `pip instal
-00000ed0: 6c60 2c20 7370 6563 6966 7969 6e67 2074  l`, specifying t
-00000ee0: 6865 2064 7269 7665 720a 6261 7365 6420  he driver.based 
-00000ef0: 6f6e 2079 6f75 7220 6461 7461 6261 7365  on your database
-00000f00: 2064 6961 6c65 6374 2e0a 0a23 2323 204d   dialect...### M
-00000f10: 7953 514c 0a60 6060 0a70 6970 2069 6e73  ySQL.```.pip ins
-00000f20: 7461 6c6c 2022 636c 6f75 642d 7371 6c2d  tall "cloud-sql-
-00000f30: 7079 7468 6f6e 2d63 6f6e 6e65 6374 6f72  python-connector
-00000f40: 5b70 796d 7973 716c 5d22 0a60 6060 0a23  [pymysql]".```.#
-00000f50: 2323 2050 6f73 7467 7265 730a 5468 6572  ## Postgres.Ther
-00000f60: 6520 6172 6520 7477 6f20 6469 6666 6572  e are two differ
-00000f70: 656e 7420 6461 7461 6261 7365 2064 7269  ent database dri
-00000f80: 7665 7273 2074 6861 7420 6172 6520 7375  vers that are su
-00000f90: 7070 6f72 7465 6420 666f 7220 7468 6520  pported for the 
-00000fa0: 506f 7374 6772 6573 2064 6961 6c65 6374  Postgres dialect
-00000fb0: 3a0a 0a23 2323 2320 7067 3830 3030 0a60  :..#### pg8000.`
-00000fc0: 6060 0a70 6970 2069 6e73 7461 6c6c 2022  ``.pip install "
-00000fd0: 636c 6f75 642d 7371 6c2d 7079 7468 6f6e  cloud-sql-python
-00000fe0: 2d63 6f6e 6e65 6374 6f72 5b70 6738 3030  -connector[pg800
-00000ff0: 305d 220a 6060 600a 2323 2323 2061 7379  0]".```.#### asy
-00001000: 6e63 7067 0a60 6060 0a70 6970 2069 6e73  ncpg.```.pip ins
-00001010: 7461 6c6c 2022 636c 6f75 642d 7371 6c2d  tall "cloud-sql-
-00001020: 7079 7468 6f6e 2d63 6f6e 6e65 6374 6f72  python-connector
-00001030: 5b61 7379 6e63 7067 5d22 0a60 6060 0a23  [asyncpg]".```.#
-00001040: 2323 2053 514c 2053 6572 7665 720a 6060  ## SQL Server.``
-00001050: 600a 7069 7020 696e 7374 616c 6c20 2263  `.pip install "c
-00001060: 6c6f 7564 2d73 716c 2d70 7974 686f 6e2d  loud-sql-python-
-00001070: 636f 6e6e 6563 746f 725b 7079 7464 735d  connector[pytds]
-00001080: 220a 6060 600a 2323 2055 7361 6765 0a0a  ".```.## Usage..
-00001090: 5468 6973 2070 6163 6b61 6765 2070 726f  This package pro
-000010a0: 7669 6465 7320 7365 7665 7261 6c20 6675  vides several fu
-000010b0: 6e63 7469 6f6e 7320 666f 7220 6175 7468  nctions for auth
-000010c0: 6f72 697a 696e 6720 616e 6420 656e 6372  orizing and encr
-000010d0: 7970 7469 6e67 0a63 6f6e 6e65 6374 696f  ypting.connectio
-000010e0: 6e73 2e20 5468 6573 6520 6675 6e63 7469  ns. These functi
-000010f0: 6f6e 7320 6172 6520 7573 6564 2077 6974  ons are used wit
-00001100: 6820 796f 7572 2064 6174 6162 6173 6520  h your database 
-00001110: 6472 6976 6572 2074 6f20 636f 6e6e 6563  driver to connec
-00001120: 7420 746f 0a79 6f75 7220 436c 6f75 6420  t to.your Cloud 
-00001130: 5351 4c20 696e 7374 616e 6365 2e0a 0a54  SQL instance...T
-00001140: 6865 2069 6e73 7461 6e63 6520 636f 6e6e  he instance conn
-00001150: 6563 7469 6f6e 206e 616d 6520 666f 7220  ection name for 
-00001160: 796f 7572 2043 6c6f 7564 2053 514c 2069  your Cloud SQL i
-00001170: 6e73 7461 6e63 6520 6973 2061 6c77 6179  nstance is alway
-00001180: 7320 696e 2074 6865 0a66 6f72 6d61 7420  s in the.format 
-00001190: 2270 726f 6a65 6374 3a72 6567 696f 6e3a  "project:region:
-000011a0: 696e 7374 616e 6365 222e 0a0a 2323 2320  instance"...### 
-000011b0: 4150 4973 2061 6e64 2053 6572 7669 6365  APIs and Service
-000011c0: 730a 0a54 6869 7320 7061 636b 6167 6520  s..This package 
-000011d0: 7265 7175 6972 6573 2074 6865 2066 6f6c  requires the fol
-000011e0: 6c6f 7769 6e67 2074 6f20 7375 6363 6573  lowing to succes
-000011f0: 7366 756c 6c79 206d 616b 6520 436c 6f75  sfully make Clou
-00001200: 6420 5351 4c20 436f 6e6e 6563 7469 6f6e  d SQL Connection
-00001210: 733a 0a0a 2d20 4941 4d20 7072 696e 6369  s:..- IAM princi
-00001220: 7061 6c20 2875 7365 722c 2073 6572 7669  pal (user, servi
-00001230: 6365 2061 6363 6f75 6e74 2c20 6574 632e  ce account, etc.
-00001240: 2920 7769 7468 2074 6865 0a5b 436c 6f75  ) with the.[Clou
-00001250: 6420 5351 4c20 436c 6965 6e74 5d5b 636c  d SQL Client][cl
-00001260: 6965 6e74 2d72 6f6c 655d 2072 6f6c 652e  ient-role] role.
-00001270: 2054 6869 7320 4941 4d20 7072 696e 6369   This IAM princi
-00001280: 7061 6c20 7769 6c6c 2062 6520 7573 6564  pal will be used
-00001290: 2066 6f72 0a5b 6372 6564 656e 7469 616c   for.[credential
-000012a0: 735d 2823 6372 6564 656e 7469 616c 7329  s](#credentials)
-000012b0: 2e0a 2d20 5468 6520 5b43 6c6f 7564 2053  ..- The [Cloud S
-000012c0: 514c 2041 646d 696e 2041 5049 5d5b 6164  QL Admin API][ad
-000012d0: 6d69 6e2d 6170 695d 2074 6f20 6265 2065  min-api] to be e
-000012e0: 6e61 626c 6564 2077 6974 6869 6e20 796f  nabled within yo
-000012f0: 7572 2047 6f6f 676c 6520 436c 6f75 640a  ur Google Cloud.
-00001300: 5072 6f6a 6563 742e 2042 7920 6465 6661  Project. By defa
-00001310: 756c 742c 2074 6865 2041 5049 2077 696c  ult, the API wil
-00001320: 6c20 6265 2063 616c 6c65 6420 696e 2074  l be called in t
-00001330: 6865 2070 726f 6a65 6374 2061 7373 6f63  he project assoc
-00001340: 6961 7465 6420 7769 7468 0a74 6865 2049  iated with.the I
-00001350: 414d 2070 7269 6e63 6970 616c 2e0a 0a5b  AM principal...[
-00001360: 6164 6d69 6e2d 6170 695d 3a20 6874 7470  admin-api]: http
-00001370: 733a 2f2f 636f 6e73 6f6c 652e 636c 6f75  s://console.clou
-00001380: 642e 676f 6f67 6c65 2e63 6f6d 2f61 7069  d.google.com/api
-00001390: 732f 6170 692f 7371 6c61 646d 696e 2e67  s/api/sqladmin.g
-000013a0: 6f6f 676c 6561 7069 732e 636f 6d0a 5b63  oogleapis.com.[c
-000013b0: 6c69 656e 742d 726f 6c65 5d3a 2068 7474  lient-role]: htt
-000013c0: 7073 3a2f 2f63 6c6f 7564 2e67 6f6f 676c  ps://cloud.googl
-000013d0: 652e 636f 6d2f 7371 6c2f 646f 6373 2f6d  e.com/sql/docs/m
-000013e0: 7973 716c 2f72 6f6c 6573 2d61 6e64 2d70  ysql/roles-and-p
-000013f0: 6572 6d69 7373 696f 6e73 0a0a 2323 2320  ermissions..### 
-00001400: 4372 6564 656e 7469 616c 730a 0a54 6869  Credentials..Thi
-00001410: 7320 6c69 6272 6172 7920 7573 6573 2074  s library uses t
-00001420: 6865 205b 4170 706c 6963 6174 696f 6e20  he [Application 
-00001430: 4465 6661 756c 7420 4372 6564 656e 7469  Default Credenti
-00001440: 616c 7320 2841 4443 295d 5b61 6463 5d20  als (ADC)][adc] 
-00001450: 7374 7261 7465 6779 2066 6f72 0a72 6573  strategy for.res
-00001460: 6f6c 7669 6e67 2063 7265 6465 6e74 6961  olving credentia
-00001470: 6c73 2e20 506c 6561 7365 2073 6565 205b  ls. Please see [
-00001480: 7468 6573 6520 696e 7374 7275 6374 696f  these instructio
-00001490: 6e73 2066 6f72 2068 6f77 2074 6f20 7365  ns for how to se
-000014a0: 7420 796f 7572 2041 4443 5d5b 7365 742d  t your ADC][set-
-000014b0: 6164 635d 0a28 476f 6f67 6c65 2043 6c6f  adc].(Google Clo
-000014c0: 7564 2041 7070 6c69 6361 7469 6f6e 2076  ud Application v
-000014d0: 7320 4c6f 6361 6c20 4465 7665 6c6f 706d  s Local Developm
-000014e0: 656e 742c 2049 414d 2075 7365 7220 7673  ent, IAM user vs
-000014f0: 2073 6572 7669 6365 2061 6363 6f75 6e74   service account
-00001500: 2063 7265 6465 6e74 6961 6c73 292c 0a6f   credentials),.o
-00001510: 7220 636f 6e73 756c 7420 7468 6520 5b67  r consult the [g
-00001520: 6f6f 676c 652e 6175 7468 5d5b 676f 6f67  oogle.auth][goog
-00001530: 6c65 2d61 7574 685d 2070 6163 6b61 6765  le-auth] package
-00001540: 2e0a 0a54 6f20 6578 706c 6963 6974 6c79  ...To explicitly
-00001550: 2073 6574 2061 2073 7065 6369 6669 6320   set a specific 
-00001560: 736f 7572 6365 2066 6f72 2074 6865 2063  source for the c
-00001570: 7265 6465 6e74 6961 6c73 2c20 7365 650a  redentials, see.
-00001580: 5b43 6f6e 6669 6775 7269 6e67 2074 6865  [Configuring the
-00001590: 2043 6f6e 6e65 6374 6f72 5d28 2363 6f6e   Connector](#con
-000015a0: 6669 6775 7269 6e67 2d74 6865 2d63 6f6e  figuring-the-con
-000015b0: 6e65 6374 6f72 2920 6265 6c6f 772e 0a0a  nector) below...
-000015c0: 5b61 6463 5d3a 2068 7474 7073 3a2f 2f63  [adc]: https://c
-000015d0: 6c6f 7564 2e67 6f6f 676c 652e 636f 6d2f  loud.google.com/
-000015e0: 646f 6373 2f61 7574 6865 6e74 6963 6174  docs/authenticat
-000015f0: 696f 6e23 6164 630a 5b73 6574 2d61 6463  ion#adc.[set-adc
-00001600: 5d3a 2068 7474 7073 3a2f 2f63 6c6f 7564  ]: https://cloud
-00001610: 2e67 6f6f 676c 652e 636f 6d2f 646f 6373  .google.com/docs
-00001620: 2f61 7574 6865 6e74 6963 6174 696f 6e2f  /authentication/
-00001630: 7072 6f76 6964 652d 6372 6564 656e 7469  provide-credenti
-00001640: 616c 732d 6164 630a 5b67 6f6f 676c 652d  als-adc.[google-
-00001650: 6175 7468 5d3a 2068 7474 7073 3a2f 2f67  auth]: https://g
-00001660: 6f6f 676c 652d 6175 7468 2e72 6561 6474  oogle-auth.readt
-00001670: 6865 646f 6373 2e69 6f2f 656e 2f6d 6173  hedocs.io/en/mas
-00001680: 7465 722f 7265 6665 7265 6e63 652f 676f  ter/reference/go
-00001690: 6f67 6c65 2e61 7574 682e 6874 6d6c 0a0a  ogle.auth.html..
-000016a0: 2323 2320 486f 7720 746f 2075 7365 2074  ### How to use t
-000016b0: 6869 7320 436f 6e6e 6563 746f 720a 0a54  his Connector..T
-000016c0: 6f20 636f 6e6e 6563 7420 746f 2043 6c6f  o connect to Clo
-000016d0: 7564 2053 514c 2075 7369 6e67 2074 6865  ud SQL using the
-000016e0: 2063 6f6e 6e65 6374 6f72 2c20 696e 6974   connector, init
-000016f0: 6974 616c 697a 6520 6120 6043 6f6e 6e65  italize a `Conne
-00001700: 6374 6f72 600a 6f62 6a65 6374 2061 6e64  ctor`.object and
-00001710: 2063 616c 6c20 6974 2773 2060 636f 6e6e   call it's `conn
-00001720: 6563 7460 206d 6574 686f 6420 7769 7468  ect` method with
-00001730: 2074 6865 2070 726f 7065 7220 696e 7075   the proper inpu
-00001740: 7420 7061 7261 6d65 7465 7273 2e0a 0a54  t parameters...T
-00001750: 6865 2060 436f 6e6e 6563 746f 7260 2069  he `Connector` i
-00001760: 7473 656c 6620 6372 6561 7465 7320 636f  tself creates co
-00001770: 6e6e 6563 7469 6f6e 206f 626a 6563 7473  nnection objects
-00001780: 2062 7920 6361 6c6c 696e 6720 6974 7320   by calling its 
-00001790: 6063 6f6e 6e65 6374 6020 6d65 7468 6f64  `connect` method
-000017a0: 2062 7574 2064 6f65 7320 6e6f 7420 6d61   but does not ma
-000017b0: 6e61 6765 2064 6174 6162 6173 6520 636f  nage database co
-000017c0: 6e6e 6563 7469 6f6e 2070 6f6f 6c69 6e67  nnection pooling
-000017d0: 2e20 466f 7220 7468 6973 2072 6561 736f  . For this reaso
-000017e0: 6e2c 2069 7420 6973 2072 6563 6f6d 6d65  n, it is recomme
-000017f0: 6e64 6564 2074 6f20 7573 6520 7468 6520  nded to use the 
-00001800: 636f 6e6e 6563 746f 7220 616c 6f6e 6773  connector alongs
-00001810: 6964 6520 6120 6c69 6272 6172 7920 7468  ide a library th
-00001820: 6174 2063 616e 2063 7265 6174 6520 636f  at can create co
-00001830: 6e6e 6563 7469 6f6e 2070 6f6f 6c73 2c20  nnection pools, 
-00001840: 7375 6368 2061 7320 5b53 514c 416c 6368  such as [SQLAlch
-00001850: 656d 795d 2868 7474 7073 3a2f 2f77 7777  emy](https://www
-00001860: 2e73 716c 616c 6368 656d 792e 6f72 672f  .sqlalchemy.org/
-00001870: 292e 2054 6869 7320 7769 6c6c 2061 6c6c  ). This will all
-00001880: 6f77 2066 6f72 2063 6f6e 6e65 6374 696f  ow for connectio
-00001890: 6e73 2074 6f20 7265 6d61 696e 206f 7065  ns to remain ope
-000018a0: 6e20 616e 6420 6265 2072 6575 7365 642c  n and be reused,
-000018b0: 2072 6564 7563 696e 6720 636f 6e6e 6563   reducing connec
-000018c0: 7469 6f6e 206f 7665 7268 6561 6420 616e  tion overhead an
-000018d0: 6420 7468 6520 6e75 6d62 6572 206f 6620  d the number of 
-000018e0: 636f 6e6e 6563 7469 6f6e 7320 6e65 6564  connections need
-000018f0: 6564 2e0a 0a49 6e20 7468 6520 436f 6e6e  ed...In the Conn
-00001900: 6563 746f 7227 7320 6063 6f6e 6e65 6374  ector's `connect
-00001910: 6020 6d65 7468 6f64 2062 656c 6f77 2c20  ` method below, 
-00001920: 696e 7075 7420 796f 7572 2063 6f6e 6e65  input your conne
-00001930: 6374 696f 6e20 7374 7269 6e67 2061 7320  ction string as 
-00001940: 7468 6520 6669 7273 7420 706f 7369 7469  the first positi
-00001950: 6f6e 616c 2061 7267 756d 656e 7420 616e  onal argument an
-00001960: 6420 7468 6520 6e61 6d65 206f 6620 7468  d the name of th
-00001970: 6520 6461 7461 6261 7365 2064 7269 7665  e database drive
-00001980: 7220 666f 7220 7468 6520 7365 636f 6e64  r for the second
-00001990: 2070 6f73 6974 696f 6e61 6c20 6172 6775   positional argu
-000019a0: 6d65 6e74 2e20 496e 7365 7274 2074 6865  ment. Insert the
-000019b0: 2072 6573 7420 6f66 2079 6f75 7220 636f   rest of your co
-000019c0: 6e6e 6563 7469 6f6e 206b 6579 776f 7264  nnection keyword
-000019d0: 2061 7267 756d 656e 7473 206c 696b 6520   arguments like 
-000019e0: 7573 6572 2c20 7061 7373 776f 7264 2061  user, password a
-000019f0: 6e64 2064 6174 6162 6173 652e 2059 6f75  nd database. You
-00001a00: 2063 616e 2061 6c73 6f20 7365 7420 7468   can also set th
-00001a10: 6520 6f70 7469 6f6e 616c 2060 7469 6d65  e optional `time
-00001a20: 6f75 7460 206f 7220 6069 705f 7479 7065  out` or `ip_type
-00001a30: 6020 6b65 7977 6f72 6420 6172 6775 6d65  ` keyword argume
-00001a40: 6e74 732e 0a0a 546f 2075 7365 2074 6869  nts...To use thi
-00001a50: 7320 636f 6e6e 6563 746f 7220 7769 7468  s connector with
-00001a60: 2053 514c 416c 6368 656d 792c 2075 7365   SQLAlchemy, use
-00001a70: 2074 6865 2060 6372 6561 746f 7260 2061   the `creator` a
-00001a80: 7267 756d 656e 7420 666f 7220 6073 716c  rgument for `sql
-00001a90: 616c 6368 656d 792e 6372 6561 7465 5f65  alchemy.create_e
-00001aa0: 6e67 696e 6560 3a0a 0a60 6060 7079 7468  ngine`:..```pyth
-00001ab0: 6f6e 0a66 726f 6d20 676f 6f67 6c65 2e63  on.from google.c
-00001ac0: 6c6f 7564 2e73 716c 2e63 6f6e 6e65 6374  loud.sql.connect
-00001ad0: 6f72 2069 6d70 6f72 7420 436f 6e6e 6563  or import Connec
-00001ae0: 746f 720a 696d 706f 7274 2073 716c 616c  tor.import sqlal
-00001af0: 6368 656d 790a 0a23 2069 6e69 7469 616c  chemy..# initial
-00001b00: 697a 6520 436f 6e6e 6563 746f 7220 6f62  ize Connector ob
-00001b10: 6a65 6374 0a63 6f6e 6e65 6374 6f72 203d  ject.connector =
-00001b20: 2043 6f6e 6e65 6374 6f72 2829 0a0a 2320   Connector()..# 
-00001b30: 6675 6e63 7469 6f6e 2074 6f20 7265 7475  function to retu
-00001b40: 726e 2074 6865 2064 6174 6162 6173 6520  rn the database 
-00001b50: 636f 6e6e 6563 7469 6f6e 0a64 6566 2067  connection.def g
-00001b60: 6574 636f 6e6e 2829 202d 3e20 7079 6d79  etconn() -> pymy
-00001b70: 7371 6c2e 636f 6e6e 6563 7469 6f6e 732e  sql.connections.
-00001b80: 436f 6e6e 6563 7469 6f6e 3a0a 2020 2020  Connection:.    
-00001b90: 636f 6e6e 3a20 7079 6d79 7371 6c2e 636f  conn: pymysql.co
-00001ba0: 6e6e 6563 7469 6f6e 732e 436f 6e6e 6563  nnections.Connec
-00001bb0: 7469 6f6e 203d 2063 6f6e 6e65 6374 6f72  tion = connector
-00001bc0: 2e63 6f6e 6e65 6374 280a 2020 2020 2020  .connect(.      
-00001bd0: 2020 2270 726f 6a65 6374 3a72 6567 696f    "project:regio
-00001be0: 6e3a 696e 7374 616e 6365 222c 0a20 2020  n:instance",.   
-00001bf0: 2020 2020 2022 7079 6d79 7371 6c22 2c0a       "pymysql",.
-00001c00: 2020 2020 2020 2020 7573 6572 3d22 6d79          user="my
-00001c10: 2d75 7365 7222 2c0a 2020 2020 2020 2020  -user",.        
-00001c20: 7061 7373 776f 7264 3d22 6d79 2d70 6173  password="my-pas
-00001c30: 7377 6f72 6422 2c0a 2020 2020 2020 2020  sword",.        
-00001c40: 6462 3d22 6d79 2d64 622d 6e61 6d65 220a  db="my-db-name".
-00001c50: 2020 2020 290a 2020 2020 7265 7475 726e      ).    return
-00001c60: 2063 6f6e 6e0a 0a23 2063 7265 6174 6520   conn..# create 
-00001c70: 636f 6e6e 6563 7469 6f6e 2070 6f6f 6c0a  connection pool.
-00001c80: 706f 6f6c 203d 2073 716c 616c 6368 656d  pool = sqlalchem
-00001c90: 792e 6372 6561 7465 5f65 6e67 696e 6528  y.create_engine(
-00001ca0: 0a20 2020 2022 6d79 7371 6c2b 7079 6d79  .    "mysql+pymy
-00001cb0: 7371 6c3a 2f2f 222c 0a20 2020 2063 7265  sql://",.    cre
-00001cc0: 6174 6f72 3d67 6574 636f 6e6e 2c0a 290a  ator=getconn,.).
-00001cd0: 6060 600a 0a54 6865 2072 6574 7572 6e65  ```..The returne
-00001ce0: 6420 636f 6e6e 6563 7469 6f6e 2070 6f6f  d connection poo
-00001cf0: 6c20 656e 6769 6e65 2063 616e 2074 6865  l engine can the
-00001d00: 6e20 6265 2075 7365 6420 746f 2071 7565  n be used to que
-00001d10: 7279 2061 6e64 206d 6f64 6966 7920 7468  ry and modify th
-00001d20: 6520 6461 7461 6261 7365 2e0a 0a60 6060  e database...```
-00001d30: 7079 7468 6f6e 0a23 2069 6e73 6572 7420  python.# insert 
-00001d40: 7374 6174 656d 656e 740a 696e 7365 7274  statement.insert
-00001d50: 5f73 746d 7420 3d20 7371 6c61 6c63 6865  _stmt = sqlalche
-00001d60: 6d79 2e74 6578 7428 0a20 2020 2022 494e  my.text(.    "IN
-00001d70: 5345 5254 2049 4e54 4f20 6d79 5f74 6162  SERT INTO my_tab
-00001d80: 6c65 2028 6964 2c20 7469 746c 6529 2056  le (id, title) V
-00001d90: 414c 5545 5320 283a 6964 2c20 3a74 6974  ALUES (:id, :tit
-00001da0: 6c65 2922 2c0a 290a 0a77 6974 6820 706f  le)",.)..with po
-00001db0: 6f6c 2e63 6f6e 6e65 6374 2829 2061 7320  ol.connect() as 
-00001dc0: 6462 5f63 6f6e 6e3a 0a20 2020 2023 2069  db_conn:.    # i
-00001dd0: 6e73 6572 7420 696e 746f 2064 6174 6162  nsert into datab
-00001de0: 6173 650a 2020 2020 6462 5f63 6f6e 6e2e  ase.    db_conn.
-00001df0: 6578 6563 7574 6528 696e 7365 7274 5f73  execute(insert_s
-00001e00: 746d 742c 2070 6172 616d 6574 6572 733d  tmt, parameters=
-00001e10: 7b22 6964 223a 2022 626f 6f6b 3122 2c20  {"id": "book1", 
-00001e20: 2274 6974 6c65 223a 2022 426f 6f6b 204f  "title": "Book O
-00001e30: 6e65 227d 290a 0a20 2020 2023 2071 7565  ne"})..    # que
-00001e40: 7279 2064 6174 6162 6173 650a 2020 2020  ry database.    
-00001e50: 7265 7375 6c74 203d 2064 625f 636f 6e6e  result = db_conn
-00001e60: 2e65 7865 6375 7465 2873 716c 616c 6368  .execute(sqlalch
-00001e70: 656d 792e 7465 7874 2822 5345 4c45 4354  emy.text("SELECT
-00001e80: 202a 2066 726f 6d20 6d79 5f74 6162 6c65   * from my_table
-00001e90: 2229 292e 6665 7463 6861 6c6c 2829 0a0a  ")).fetchall()..
-00001ea0: 2020 2020 2320 636f 6d6d 6974 2074 7261      # commit tra
-00001eb0: 6e73 6163 7469 6f6e 2028 5351 4c41 6c63  nsaction (SQLAlc
-00001ec0: 6865 6d79 2076 322e 582e 5820 6973 2063  hemy v2.X.X is c
-00001ed0: 6f6d 6d69 7420 6173 2079 6f75 2067 6f29  ommit as you go)
-00001ee0: 0a20 2020 2064 625f 636f 6e6e 2e63 6f6d  .    db_conn.com
-00001ef0: 6d69 7428 290a 0a20 2020 2023 2044 6f20  mit()..    # Do 
-00001f00: 736f 6d65 7468 696e 6720 7769 7468 2074  something with t
-00001f10: 6865 2072 6573 756c 7473 0a20 2020 2066  he results.    f
-00001f20: 6f72 2072 6f77 2069 6e20 7265 7375 6c74  or row in result
-00001f30: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
-00001f40: 726f 7729 0a60 6060 0a0a 546f 2063 6c6f  row).```..To clo
-00001f50: 7365 2074 6865 2060 436f 6e6e 6563 746f  se the `Connecto
-00001f60: 7260 206f 626a 6563 7427 7320 6261 636b  r` object's back
-00001f70: 6772 6f75 6e64 2072 6573 6f75 7263 6573  ground resources
-00001f80: 2c20 6361 6c6c 2069 7427 7320 6063 6c6f  , call it's `clo
-00001f90: 7365 2829 6020 6d65 7468 6f64 2061 7320  se()` method as 
-00001fa0: 666f 6c6c 6f77 733a 0a0a 6060 6070 7974  follows:..```pyt
-00001fb0: 686f 6e0a 636f 6e6e 6563 746f 722e 636c  hon.connector.cl
-00001fc0: 6f73 6528 290a 6060 600a 0a2a 2a4e 6f74  ose().```..**Not
-00001fd0: 652a 2a3a 2046 6f72 206d 6f72 6520 6578  e**: For more ex
-00001fe0: 616d 706c 6573 206f 6620 7573 696e 6720  amples of using 
-00001ff0: 5351 4c41 6c63 6865 6d79 2074 6f20 6d61  SQLAlchemy to ma
-00002000: 6e61 6765 2063 6f6e 6e65 6374 696f 6e20  nage connection 
-00002010: 706f 6f6c 696e 6720 7769 7468 2074 6865  pooling with the
-00002020: 2063 6f6e 6e65 6374 6f72 2c20 706c 6561   connector, plea
-00002030: 7365 2073 6565 205b 436c 6f75 6420 5351  se see [Cloud SQ
-00002040: 4c20 5351 4c41 6c63 6865 6d79 2053 616d  L SQLAlchemy Sam
-00002050: 706c 6573 5d28 6874 7470 733a 2f2f 636c  ples](https://cl
-00002060: 6f75 642e 676f 6f67 6c65 2e63 6f6d 2f73  oud.google.com/s
-00002070: 716c 2f64 6f63 732f 706f 7374 6772 6573  ql/docs/postgres
-00002080: 2f63 6f6e 6e65 6374 2d63 6f6e 6e65 6374  /connect-connect
-00002090: 6f72 7323 7079 7468 6f6e 5f31 292e 0a0a  ors#python_1)...
-000020a0: 2a2a 4e6f 7465 2066 6f72 2053 514c 2053  **Note for SQL S
-000020b0: 6572 7665 7220 7573 6572 732a 2a3a 2049  erver users**: I
-000020c0: 6620 796f 7572 2053 514c 2053 6572 7665  f your SQL Serve
-000020d0: 7220 696e 7374 616e 6365 2072 6571 7569  r instance requi
-000020e0: 7265 7320 5353 4c2c 2079 6f75 206e 6565  res SSL, you nee
-000020f0: 6420 746f 2064 6f77 6e6c 6f61 6420 7468  d to download th
-00002100: 6520 4341 2063 6572 7469 6669 6361 7465  e CA certificate
-00002110: 2066 6f72 2079 6f75 7220 696e 7374 616e   for your instan
-00002120: 6365 2061 6e64 2069 6e63 6c75 6465 2060  ce and include `
-00002130: 6361 6669 6c65 3d7b 7061 7468 2074 6f20  cafile={path to 
-00002140: 646f 776e 6c6f 6164 6564 2063 6572 7469  downloaded certi
-00002150: 6669 6361 7465 7d60 2061 6e64 2060 7661  ficate}` and `va
-00002160: 6c69 6461 7465 5f68 6f73 743d 4661 6c73  lidate_host=Fals
-00002170: 6560 2e20 5468 6973 2069 7320 6120 776f  e`. This is a wo
-00002180: 726b 6172 6f75 6e64 2066 6f72 2061 205b  rkaround for a [
-00002190: 6b6e 6f77 6e20 6973 7375 655d 2868 7474  known issue](htt
-000021a0: 7073 3a2f 2f69 7373 7565 7472 6163 6b65  ps://issuetracke
-000021b0: 722e 676f 6f67 6c65 2e63 6f6d 2f31 3834  r.google.com/184
-000021c0: 3836 3731 3437 292e 0a0a 2323 2320 436f  867147)...### Co
-000021d0: 6e66 6967 7572 696e 6720 7468 6520 436f  nfiguring the Co
-000021e0: 6e6e 6563 746f 720a 0a49 6620 796f 7520  nnector..If you 
-000021f0: 6e65 6564 2074 6f20 6375 7374 6f6d 697a  need to customiz
-00002200: 6520 736f 6d65 7468 696e 6720 6162 6f75  e something abou
-00002210: 7420 7468 6520 636f 6e6e 6563 746f 722c  t the connector,
-00002220: 206f 7220 7761 6e74 2074 6f20 7370 6563   or want to spec
-00002230: 6966 790a 6465 6661 756c 7473 2066 6f72  ify.defaults for
-00002240: 2065 6163 6820 636f 6e6e 6563 7469 6f6e   each connection
-00002250: 2074 6f20 6d61 6b65 2c20 796f 7520 6361   to make, you ca
-00002260: 6e20 696e 6974 6961 6c69 7a65 2061 0a60  n initialize a.`
-00002270: 436f 6e6e 6563 746f 7260 206f 626a 6563  Connector` objec
-00002280: 7420 6173 2066 6f6c 6c6f 7773 3a0a 0a60  t as follows:..`
-00002290: 6060 7079 7468 6f6e 0a66 726f 6d20 676f  ``python.from go
-000022a0: 6f67 6c65 2e63 6c6f 7564 2e73 716c 2e63  ogle.cloud.sql.c
-000022b0: 6f6e 6e65 6374 6f72 2069 6d70 6f72 7420  onnector import 
-000022c0: 436f 6e6e 6563 746f 722c 2049 5054 7970  Connector, IPTyp
-000022d0: 6573 0a0a 2320 4e6f 7465 3a20 616c 6c20  es..# Note: all 
-000022e0: 7061 7261 6d65 7465 7273 2062 656c 6f77  parameters below
-000022f0: 2061 7265 206f 7074 696f 6e61 6c0a 636f   are optional.co
-00002300: 6e6e 6563 746f 7220 3d20 436f 6e6e 6563  nnector = Connec
-00002310: 746f 7228 0a20 2020 2069 705f 7479 7065  tor(.    ip_type
-00002320: 3d49 5054 7970 6573 2e50 5542 4c49 432c  =IPTypes.PUBLIC,
-00002330: 0a20 2020 2065 6e61 626c 655f 6961 6d5f  .    enable_iam_
-00002340: 6175 7468 3d46 616c 7365 2c0a 2020 2020  auth=False,.    
-00002350: 7469 6d65 6f75 743d 3330 2c0a 2020 2020  timeout=30,.    
-00002360: 6372 6564 656e 7469 616c 733d 6375 7374  credentials=cust
-00002370: 6f6d 5f63 7265 6473 2023 2067 6f6f 676c  om_creds # googl
-00002380: 652e 6175 7468 2e63 7265 6465 6e74 6961  e.auth.credentia
-00002390: 6c73 2e43 7265 6465 6e74 6961 6c73 0a29  ls.Credentials.)
-000023a0: 0a60 6060 0a0a 2323 2320 5573 696e 6720  .```..### Using 
-000023b0: 436f 6e6e 6563 746f 7220 6173 2061 2043  Connector as a C
-000023c0: 6f6e 7465 7874 204d 616e 6167 6572 0a0a  ontext Manager..
-000023d0: 5468 6520 6043 6f6e 6e65 6374 6f72 6020  The `Connector` 
-000023e0: 6f62 6a65 6374 2063 616e 2061 6c73 6f20  object can also 
-000023f0: 6265 2075 7365 6420 6173 2061 2063 6f6e  be used as a con
-00002400: 7465 7874 206d 616e 6167 6572 2069 6e20  text manager in 
-00002410: 6f72 6465 7220 746f 0a61 7574 6f6d 6174  order to.automat
-00002420: 6963 616c 6c79 2063 6c6f 7365 2061 6e64  ically close and
-00002430: 2063 6c65 616e 7570 2072 6573 6f75 7263   cleanup resourc
-00002440: 6573 2c20 7265 6d6f 7669 6e67 2074 6865  es, removing the
-00002450: 206e 6565 6420 666f 7220 6578 706c 6963   need for explic
-00002460: 6974 0a63 616c 6c73 2074 6f20 6063 6f6e  it.calls to `con
-00002470: 6e65 6374 6f72 2e63 6c6f 7365 2829 602e  nector.close()`.
-00002480: 0a0a 436f 6e6e 6563 746f 7220 6173 2061  ..Connector as a
-00002490: 2063 6f6e 7465 7874 206d 616e 6167 6572   context manager
-000024a0: 3a0a 0a60 6060 7079 7468 6f6e 0a66 726f  :..```python.fro
-000024b0: 6d20 676f 6f67 6c65 2e63 6c6f 7564 2e73  m google.cloud.s
-000024c0: 716c 2e63 6f6e 6e65 6374 6f72 2069 6d70  ql.connector imp
-000024d0: 6f72 7420 436f 6e6e 6563 746f 720a 696d  ort Connector.im
-000024e0: 706f 7274 2073 716c 616c 6368 656d 790a  port sqlalchemy.
-000024f0: 0a23 2062 7569 6c64 2063 6f6e 6e65 6374  .# build connect
-00002500: 696f 6e0a 6465 6620 6765 7463 6f6e 6e28  ion.def getconn(
-00002510: 2920 2d3e 2070 796d 7973 716c 2e63 6f6e  ) -> pymysql.con
-00002520: 6e65 6374 696f 6e73 2e43 6f6e 6e65 6374  nections.Connect
-00002530: 696f 6e3a 0a20 2020 2077 6974 6820 436f  ion:.    with Co
-00002540: 6e6e 6563 746f 7228 2920 6173 2063 6f6e  nnector() as con
-00002550: 6e65 6374 6f72 3a0a 2020 2020 2020 2020  nector:.        
-00002560: 636f 6e6e 203d 2063 6f6e 6e65 6374 6f72  conn = connector
-00002570: 2e63 6f6e 6e65 6374 280a 2020 2020 2020  .connect(.      
-00002580: 2020 2020 2020 2270 726f 6a65 6374 3a72        "project:r
-00002590: 6567 696f 6e3a 696e 7374 616e 6365 222c  egion:instance",
-000025a0: 0a20 2020 2020 2020 2020 2020 2022 7079  .            "py
-000025b0: 6d79 7371 6c22 2c0a 2020 2020 2020 2020  mysql",.        
-000025c0: 2020 2020 7573 6572 3d22 6d79 2d75 7365      user="my-use
-000025d0: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
-000025e0: 7061 7373 776f 7264 3d22 6d79 2d70 6173  password="my-pas
-000025f0: 7377 6f72 6422 2c0a 2020 2020 2020 2020  sword",.        
-00002600: 2020 2020 6462 3d22 6d79 2d64 622d 6e61      db="my-db-na
-00002610: 6d65 220a 2020 2020 2020 2020 290a 2020  me".        ).  
-00002620: 2020 7265 7475 726e 2063 6f6e 6e0a 0a23    return conn..#
-00002630: 2063 7265 6174 6520 636f 6e6e 6563 7469   create connecti
-00002640: 6f6e 2070 6f6f 6c0a 706f 6f6c 203d 2073  on pool.pool = s
-00002650: 716c 616c 6368 656d 792e 6372 6561 7465  qlalchemy.create
-00002660: 5f65 6e67 696e 6528 0a20 2020 2022 6d79  _engine(.    "my
-00002670: 7371 6c2b 7079 6d79 7371 6c3a 2f2f 222c  sql+pymysql://",
-00002680: 0a20 2020 2063 7265 6174 6f72 3d67 6574  .    creator=get
-00002690: 636f 6e6e 2c0a 290a 0a23 2069 6e73 6572  conn,.)..# inser
-000026a0: 7420 7374 6174 656d 656e 740a 696e 7365  t statement.inse
-000026b0: 7274 5f73 746d 7420 3d20 7371 6c61 6c63  rt_stmt = sqlalc
-000026c0: 6865 6d79 2e74 6578 7428 0a20 2020 2022  hemy.text(.    "
-000026d0: 494e 5345 5254 2049 4e54 4f20 6d79 5f74  INSERT INTO my_t
-000026e0: 6162 6c65 2028 6964 2c20 7469 746c 6529  able (id, title)
-000026f0: 2056 414c 5545 5320 283a 6964 2c20 3a74   VALUES (:id, :t
-00002700: 6974 6c65 2922 2c0a 290a 0a23 2069 6e74  itle)",.)..# int
-00002710: 6572 6163 7420 7769 7468 2043 6c6f 7564  eract with Cloud
-00002720: 2053 514c 2064 6174 6162 6173 6520 7573   SQL database us
-00002730: 696e 6720 636f 6e6e 6563 7469 6f6e 2070  ing connection p
-00002740: 6f6f 6c0a 7769 7468 2070 6f6f 6c2e 636f  ool.with pool.co
-00002750: 6e6e 6563 7428 2920 6173 2064 625f 636f  nnect() as db_co
-00002760: 6e6e 3a0a 2020 2020 2320 696e 7365 7274  nn:.    # insert
-00002770: 2069 6e74 6f20 6461 7461 6261 7365 0a20   into database. 
-00002780: 2020 2064 625f 636f 6e6e 2e65 7865 6375     db_conn.execu
-00002790: 7465 2869 6e73 6572 745f 7374 6d74 2c20  te(insert_stmt, 
-000027a0: 7061 7261 6d65 7465 7273 3d7b 2269 6422  parameters={"id"
-000027b0: 3a20 2262 6f6f 6b31 222c 2022 7469 746c  : "book1", "titl
-000027c0: 6522 3a20 2242 6f6f 6b20 4f6e 6522 7d29  e": "Book One"})
-000027d0: 0a0a 2020 2020 2320 636f 6d6d 6974 2074  ..    # commit t
-000027e0: 7261 6e73 6163 7469 6f6e 2028 5351 4c41  ransaction (SQLA
-000027f0: 6c63 6865 6d79 2076 322e 582e 5820 6973  lchemy v2.X.X is
-00002800: 2063 6f6d 6d69 7420 6173 2079 6f75 2067   commit as you g
-00002810: 6f29 0a20 2020 2064 625f 636f 6e6e 2e63  o).    db_conn.c
-00002820: 6f6d 6d69 7428 290a 0a20 2020 2023 2071  ommit()..    # q
-00002830: 7565 7279 2064 6174 6162 6173 650a 2020  uery database.  
-00002840: 2020 7265 7375 6c74 203d 2064 625f 636f    result = db_co
-00002850: 6e6e 2e65 7865 6375 7465 2873 716c 616c  nn.execute(sqlal
-00002860: 6368 656d 792e 7465 7874 2822 5345 4c45  chemy.text("SELE
-00002870: 4354 202a 2066 726f 6d20 6d79 5f74 6162  CT * from my_tab
-00002880: 6c65 2229 292e 6665 7463 6861 6c6c 2829  le")).fetchall()
-00002890: 0a0a 2020 2020 2320 446f 2073 6f6d 6574  ..    # Do somet
-000028a0: 6869 6e67 2077 6974 6820 7468 6520 7265  hing with the re
-000028b0: 7375 6c74 730a 2020 2020 666f 7220 726f  sults.    for ro
-000028c0: 7720 696e 2072 6573 756c 743a 0a20 2020  w in result:.   
-000028d0: 2020 2020 2070 7269 6e74 2872 6f77 290a       print(row).
-000028e0: 6060 600a 0a23 2323 2053 7065 6369 6679  ```..### Specify
-000028f0: 696e 6720 5075 626c 6963 206f 7220 5072  ing Public or Pr
-00002900: 6976 6174 6520 4950 0a0a 5468 6520 436c  ivate IP..The Cl
-00002910: 6f75 6420 5351 4c20 436f 6e6e 6563 746f  oud SQL Connecto
-00002920: 7220 666f 7220 5079 7468 6f6e 2063 616e  r for Python can
-00002930: 2062 6520 7573 6564 2074 6f20 636f 6e6e   be used to conn
-00002940: 6563 7420 746f 2043 6c6f 7564 2053 514c  ect to Cloud SQL
-00002950: 2069 6e73 7461 6e63 6573 2075 7369 6e67   instances using
-00002960: 2062 6f74 6820 7075 626c 6963 2061 6e64   both public and
-00002970: 2070 7269 7661 7465 2049 5020 6164 6472   private IP addr
-00002980: 6573 7365 732e 2054 6f20 7370 6563 6966  esses. To specif
-00002990: 7920 7768 6963 6820 4950 2061 6464 7265  y which IP addre
-000029a0: 7373 2074 6f20 7573 6520 746f 2063 6f6e  ss to use to con
-000029b0: 6e65 6374 2c20 7365 7420 7468 6520 6069  nect, set the `i
-000029c0: 705f 7479 7065 6020 6b65 7977 6f72 6420  p_type` keyword 
-000029d0: 6172 6775 6d65 6e74 2050 6f73 7369 626c  argument Possibl
-000029e0: 6520 7661 6c75 6573 2061 7265 2060 4950  e values are `IP
-000029f0: 5479 7065 732e 5055 424c 4943 6020 616e  Types.PUBLIC` an
-00002a00: 6420 6049 5054 7970 6573 2e50 5249 5641  d `IPTypes.PRIVA
-00002a10: 5445 602e 0a45 7861 6d70 6c65 3a0a 0a60  TE`..Example:..`
-00002a20: 6060 7079 7468 6f6e 0a66 726f 6d20 676f  ``python.from go
-00002a30: 6f67 6c65 2e63 6c6f 7564 2e73 716c 2e63  ogle.cloud.sql.c
-00002a40: 6f6e 6e65 6374 6f72 2069 6d70 6f72 7420  onnector import 
-00002a50: 4950 5479 7065 730a 0a63 6f6e 6e65 6374  IPTypes..connect
-00002a60: 6f72 2e63 6f6e 6e65 6374 280a 2020 2020  or.connect(.    
-00002a70: 2270 726f 6a65 6374 3a72 6567 696f 6e3a  "project:region:
-00002a80: 696e 7374 616e 6365 222c 0a20 2020 2022  instance",.    "
-00002a90: 7079 6d79 7371 6c22 2c0a 2020 2020 6970  pymysql",.    ip
-00002aa0: 5f74 7970 653d 4950 5479 7065 732e 5052  _type=IPTypes.PR
-00002ab0: 4956 4154 4520 2320 7573 6520 7072 6976  IVATE # use priv
-00002ac0: 6174 6520 4950 0a2e 2e2e 2069 6e73 6572  ate IP.... inser
-00002ad0: 7420 6f74 6865 7220 6b77 6172 6773 202e  t other kwargs .
-00002ae0: 2e2e 0a29 0a60 6060 0a0a 4e6f 7465 3a20  ...).```..Note: 
-00002af0: 4966 2073 7065 6369 6679 696e 6720 5072  If specifying Pr
-00002b00: 6976 6174 6520 4950 2c20 796f 7572 2061  ivate IP, your a
-00002b10: 7070 6c69 6361 7469 6f6e 206d 7573 7420  pplication must 
-00002b20: 616c 7265 6164 7920 6265 2069 6e20 7468  already be in th
-00002b30: 6520 7361 6d65 2056 5043 206e 6574 776f  e same VPC netwo
-00002b40: 726b 2061 7320 796f 7572 2043 6c6f 7564  rk as your Cloud
-00002b50: 2053 514c 2049 6e73 7461 6e63 652e 0a0a   SQL Instance...
-00002b60: 2323 2320 4941 4d20 4175 7468 656e 7469  ### IAM Authenti
-00002b70: 6361 7469 6f6e 0a0a 436f 6e6e 6563 7469  cation..Connecti
-00002b80: 6f6e 7320 7573 696e 6720 5b41 7574 6f6d  ons using [Autom
-00002b90: 6174 6963 2049 414d 2064 6174 6162 6173  atic IAM databas
-00002ba0: 6520 6175 7468 656e 7469 6361 7469 6f6e  e authentication
-00002bb0: 5d28 6874 7470 733a 2f2f 636c 6f75 642e  ](https://cloud.
-00002bc0: 676f 6f67 6c65 2e63 6f6d 2f73 716c 2f64  google.com/sql/d
-00002bd0: 6f63 732f 706f 7374 6772 6573 2f61 7574  ocs/postgres/aut
-00002be0: 6865 6e74 6963 6174 696f 6e23 6175 746f  hentication#auto
-00002bf0: 6d61 7469 6329 2061 7265 2073 7570 706f  matic) are suppo
-00002c00: 7274 6564 2077 6865 6e20 7573 696e 6720  rted when using 
-00002c10: 506f 7374 6772 6573 206f 7220 4d79 5351  Postgres or MySQ
-00002c20: 4c20 6472 6976 6572 732e 0a46 6972 7374  L drivers..First
-00002c30: 2c20 6d61 6b65 2073 7572 6520 746f 205b  , make sure to [
-00002c40: 636f 6e66 6967 7572 6520 796f 7572 2043  configure your C
-00002c50: 6c6f 7564 2053 514c 2049 6e73 7461 6e63  loud SQL Instanc
-00002c60: 6520 746f 2061 6c6c 6f77 2049 414d 2061  e to allow IAM a
-00002c70: 7574 6865 6e74 6963 6174 696f 6e5d 2868  uthentication](h
-00002c80: 7474 7073 3a2f 2f63 6c6f 7564 2e67 6f6f  ttps://cloud.goo
-00002c90: 676c 652e 636f 6d2f 7371 6c2f 646f 6373  gle.com/sql/docs
-00002ca0: 2f70 6f73 7467 7265 732f 6372 6561 7465  /postgres/create
-00002cb0: 2d65 6469 742d 6961 6d2d 696e 7374 616e  -edit-iam-instan
-00002cc0: 6365 7323 636f 6e66 6967 7572 652d 6961  ces#configure-ia
-00002cd0: 6d2d 6462 2d69 6e73 7461 6e63 6529 0a61  m-db-instance).a
-00002ce0: 6e64 205b 6164 6420 616e 2049 414d 2064  nd [add an IAM d
-00002cf0: 6174 6162 6173 6520 7573 6572 5d28 6874  atabase user](ht
-00002d00: 7470 733a 2f2f 636c 6f75 642e 676f 6f67  tps://cloud.goog
-00002d10: 6c65 2e63 6f6d 2f73 716c 2f64 6f63 732f  le.com/sql/docs/
-00002d20: 706f 7374 6772 6573 2f63 7265 6174 652d  postgres/create-
-00002d30: 6d61 6e61 6765 2d69 616d 2d75 7365 7273  manage-iam-users
-00002d40: 2363 7265 6174 696e 672d 612d 6461 7461  #creating-a-data
-00002d50: 6261 7365 2d75 7365 7229 2e0a 0a4e 6f77  base-user)...Now
-00002d60: 2c20 796f 7520 6361 6e20 636f 6e6e 6563  , you can connec
-00002d70: 7420 7573 696e 6720 7573 6572 206f 7220  t using user or 
-00002d80: 7365 7276 6963 6520 6163 636f 756e 7420  service account 
-00002d90: 6372 6564 656e 7469 616c 7320 696e 7374  credentials inst
-00002da0: 6561 6420 6f66 2061 2070 6173 7377 6f72  ead of a passwor
-00002db0: 642e 0a49 6e20 7468 6520 6361 6c6c 2074  d..In the call t
-00002dc0: 6f20 636f 6e6e 6563 742c 2073 6574 2074  o connect, set t
-00002dd0: 6865 2060 656e 6162 6c65 5f69 616d 5f61  he `enable_iam_a
-00002de0: 7574 6860 206b 6579 776f 7264 2061 7267  uth` keyword arg
-00002df0: 756d 656e 7420 746f 2074 7275 6520 616e  ument to true an
-00002e00: 6420 7468 6520 6075 7365 7260 2061 7267  d the `user` arg
-00002e10: 756d 656e 7420 746f 2074 6865 2061 7070  ument to the app
-00002e20: 726f 7072 6961 7465 6c79 2066 6f72 6d61  ropriately forma
-00002e30: 7474 6564 2049 414d 2070 7269 6e63 6970  tted IAM princip
-00002e40: 616c 2e0a 3e20 506f 7374 6772 6573 3a20  al..> Postgres: 
-00002e50: 466f 7220 616e 2049 414d 2075 7365 7220  For an IAM user 
-00002e60: 6163 636f 756e 742c 2074 6869 7320 6973  account, this is
-00002e70: 2074 6865 2075 7365 7227 7320 656d 6169   the user's emai
-00002e80: 6c20 6164 6472 6573 732e 2046 6f72 2061  l address. For a
-00002e90: 2073 6572 7669 6365 2061 6363 6f75 6e74   service account
-00002ea0: 2c20 6974 2069 7320 7468 6520 7365 7276  , it is the serv
-00002eb0: 6963 6520 6163 636f 756e 7427 7320 656d  ice account's em
-00002ec0: 6169 6c20 7769 7468 6f75 7420 7468 6520  ail without the 
-00002ed0: 602e 6773 6572 7669 6365 6163 636f 756e  `.gserviceaccoun
-00002ee0: 742e 636f 6d60 2064 6f6d 6169 6e20 7375  t.com` domain su
-00002ef0: 6666 6978 2e0a 0a3e 204d 7953 514c 3a20  ffix...> MySQL: 
-00002f00: 466f 7220 616e 2049 414d 2075 7365 7220  For an IAM user 
-00002f10: 6163 636f 756e 742c 2074 6869 7320 6973  account, this is
-00002f20: 2074 6865 2075 7365 7227 7320 656d 6169   the user's emai
-00002f30: 6c20 6164 6472 6573 732c 2077 6974 686f  l address, witho
-00002f40: 7574 2074 6865 2040 206f 7220 646f 6d61  ut the @ or doma
-00002f50: 696e 206e 616d 652e 2046 6f72 2065 7861  in name. For exa
-00002f60: 6d70 6c65 2c20 666f 7220 6074 6573 742d  mple, for `test-
-00002f70: 7573 6572 4067 6d61 696c 2e63 6f6d 602c  user@gmail.com`,
-00002f80: 2073 6574 2074 6865 2060 7573 6572 6020   set the `user` 
-00002f90: 6172 6775 6d65 6e74 2074 6f20 6074 6573  argument to `tes
-00002fa0: 742d 7573 6572 602e 2046 6f72 2061 2073  t-user`. For a s
-00002fb0: 6572 7669 6365 2061 6363 6f75 6e74 2c20  ervice account, 
-00002fc0: 7468 6973 2069 7320 7468 6520 7365 7276  this is the serv
-00002fd0: 6963 6520 6163 636f 756e 7427 7320 656d  ice account's em
-00002fe0: 6169 6c20 6164 6472 6573 7320 7769 7468  ail address with
-00002ff0: 6f75 7420 7468 6520 6040 7072 6f6a 6563  out the `@projec
-00003000: 742d 6964 2e69 616d 2e67 7365 7276 6963  t-id.iam.gservic
-00003010: 6561 6363 6f75 6e74 2e63 6f6d 6020 7375  eaccount.com` su
-00003020: 6666 6978 2e0a 0a45 7861 6d70 6c65 3a0a  ffix...Example:.
-00003030: 0a60 6060 7079 7468 6f6e 0a63 6f6e 6e65  .```python.conne
-00003040: 6374 6f72 2e63 6f6e 6e65 6374 280a 2020  ctor.connect(.  
-00003050: 2020 2022 7072 6f6a 6563 743a 7265 6769     "project:regi
-00003060: 6f6e 3a69 6e73 7461 6e63 6522 2c0a 2020  on:instance",.  
-00003070: 2020 2022 7067 3830 3030 222c 0a20 2020     "pg8000",.   
-00003080: 2020 7573 6572 3d22 706f 7374 6772 6573    user="postgres
-00003090: 2d69 616d 2d75 7365 7240 676d 6169 6c2e  -iam-user@gmail.
-000030a0: 636f 6d22 2c0a 2020 2020 2064 623d 226d  com",.     db="m
-000030b0: 792d 6462 2d6e 616d 6522 2c0a 2020 2020  y-db-name",.    
-000030c0: 2065 6e61 626c 655f 6961 6d5f 6175 7468   enable_iam_auth
-000030d0: 3d54 7275 652c 0a20 290a 6060 600a 0a23  =True,. ).```..#
-000030e0: 2323 2053 514c 2053 6572 7665 7220 4163  ## SQL Server Ac
-000030f0: 7469 7665 2044 6972 6563 746f 7279 2041  tive Directory A
-00003100: 7574 6865 6e74 6963 6174 696f 6e0a 0a41  uthentication..A
-00003110: 6374 6976 6520 4469 7265 6374 6f72 7920  ctive Directory 
-00003120: 6175 7468 656e 7469 6361 7469 6f6e 2066  authentication f
-00003130: 6f72 2053 514c 2053 6572 7665 7220 696e  or SQL Server in
-00003140: 7374 616e 6365 7320 6973 2063 7572 7265  stances is curre
-00003150: 6e74 6c79 206f 6e6c 7920 7375 7070 6f72  ntly only suppor
-00003160: 7465 6420 6f6e 2057 696e 646f 7773 2e20  ted on Windows. 
-00003170: 4669 7273 742c 206d 616b 6520 7375 7265  First, make sure
-00003180: 2074 6f20 666f 6c6c 6f77 205b 7468 6573   to follow [thes
-00003190: 6520 7374 6570 735d 2868 7474 7073 3a2f  e steps](https:/
-000031a0: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
-000031b0: 6d2f 626c 6f67 2f74 6f70 6963 732f 6465  m/blog/topics/de
-000031c0: 7665 6c6f 7065 7273 2d70 7261 6374 6974  velopers-practit
-000031d0: 696f 6e65 7273 2f63 7265 6174 696e 672d  ioners/creating-
-000031e0: 7371 6c2d 7365 7276 6572 2d69 6e73 7461  sql-server-insta
-000031f0: 6e63 652d 696e 7465 6772 6174 6564 2d61  nce-integrated-a
-00003200: 6374 6976 652d 6469 7265 6374 6f72 792d  ctive-directory-
-00003210: 7573 696e 672d 676f 6f67 6c65 2d63 6c6f  using-google-clo
-00003220: 7564 2d73 716c 2920 746f 2073 6574 2075  ud-sql) to set u
-00003230: 7020 6120 4d61 6e61 6765 6420 4144 2064  p a Managed AD d
-00003240: 6f6d 6169 6e20 616e 6420 6a6f 696e 2079  omain and join y
-00003250: 6f75 7220 436c 6f75 6420 5351 4c20 696e  our Cloud SQL in
-00003260: 7374 616e 6365 2074 6f20 7468 6520 646f  stance to the do
-00003270: 6d61 696e 2e20 5b53 6565 2068 6572 6520  main. [See here 
-00003280: 666f 7220 6d6f 7265 2069 6e66 6f20 6f6e  for more info on
-00003290: 2043 6c6f 7564 2053 514c 2041 6374 6976   Cloud SQL Activ
-000032a0: 6520 4469 7265 6374 6f72 7920 696e 7465  e Directory inte
-000032b0: 6772 6174 696f 6e5d 2868 7474 7073 3a2f  gration](https:/
-000032c0: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
-000032d0: 6d2f 7371 6c2f 646f 6373 2f73 716c 7365  m/sql/docs/sqlse
-000032e0: 7276 6572 2f61 6429 2e0a 0a4f 6e63 6520  rver/ad)...Once 
-000032f0: 796f 7520 6861 7665 2066 6f6c 6c6f 7765  you have followe
-00003300: 6420 7468 6520 7374 6570 7320 6c69 6e6b  d the steps link
-00003310: 6564 2061 626f 7665 2c20 796f 7520 6361  ed above, you ca
-00003320: 6e20 7275 6e20 7468 6520 666f 6c6c 6f77  n run the follow
-00003330: 696e 6720 636f 6465 2074 6f20 7265 7475  ing code to retu
-00003340: 726e 2061 2063 6f6e 6e65 6374 696f 6e20  rn a connection 
-00003350: 6f62 6a65 6374 3a0a 0a60 6060 7079 7468  object:..```pyth
-00003360: 6f6e 0a63 6f6e 6e65 6374 6f72 2e63 6f6e  on.connector.con
-00003370: 6e65 6374 280a 2020 2020 2270 726f 6a65  nect(.    "proje
-00003380: 6374 3a72 6567 696f 6e3a 696e 7374 616e  ct:region:instan
-00003390: 6365 222c 0a20 2020 2022 7079 7464 7322  ce",.    "pytds"
-000033a0: 2c0a 2020 2020 6462 3d22 6d79 2d64 622d  ,.    db="my-db-
-000033b0: 6e61 6d65 222c 0a20 2020 2061 6374 6976  name",.    activ
-000033c0: 655f 6469 7265 6374 6f72 795f 6175 7468  e_directory_auth
-000033d0: 3d54 7275 652c 0a20 2020 2073 6572 7665  =True,.    serve
-000033e0: 725f 6e61 6d65 3d22 7075 626c 6963 2e5b  r_name="public.[
-000033f0: 696e 7374 616e 6365 5d2e 5b6c 6f63 6174  instance].[locat
-00003400: 696f 6e5d 2e5b 7072 6f6a 6563 745d 2e63  ion].[project].c
-00003410: 6c6f 7564 7371 6c2e 5b64 6f6d 6169 6e5d  loudsql.[domain]
-00003420: 222c 0a29 0a60 6060 0a0a 4f72 2c20 6966  ",.).```..Or, if
-00003430: 2075 7369 6e67 2050 7269 7661 7465 2049   using Private I
-00003440: 503a 0a0a 6060 6070 7974 686f 6e0a 636f  P:..```python.co
-00003450: 6e6e 6563 746f 722e 636f 6e6e 6563 7428  nnector.connect(
-00003460: 0a20 2020 2022 7072 6f6a 6563 743a 7265  .    "project:re
-00003470: 6769 6f6e 3a69 6e73 7461 6e63 6522 2c0a  gion:instance",.
-00003480: 2020 2020 2270 7974 6473 222c 0a20 2020      "pytds",.   
-00003490: 2064 623d 226d 792d 6462 2d6e 616d 6522   db="my-db-name"
-000034a0: 2c0a 2020 2020 6163 7469 7665 5f64 6972  ,.    active_dir
-000034b0: 6563 746f 7279 5f61 7574 683d 5472 7565  ectory_auth=True
-000034c0: 2c0a 2020 2020 7365 7276 6572 5f6e 616d  ,.    server_nam
-000034d0: 653d 2270 7269 7661 7465 2e5b 696e 7374  e="private.[inst
-000034e0: 616e 6365 5d2e 5b6c 6f63 6174 696f 6e5d  ance].[location]
-000034f0: 2e5b 7072 6f6a 6563 745d 2e63 6c6f 7564  .[project].cloud
-00003500: 7371 6c2e 5b64 6f6d 6169 6e5d 222c 0a20  sql.[domain]",. 
-00003510: 2020 2069 705f 7479 7065 3d49 5054 7970     ip_type=IPTyp
-00003520: 6573 2e50 5249 5641 5445 0a29 0a60 6060  es.PRIVATE.).```
-00003530: 0a0a 2323 2320 5573 696e 6720 7468 6520  ..### Using the 
-00003540: 5079 7468 6f6e 2043 6f6e 6e65 6374 6f72  Python Connector
-00003550: 2077 6974 6820 5079 7468 6f6e 2057 6562   with Python Web
-00003560: 2046 7261 6d65 776f 726b 730a 0a54 6865   Frameworks..The
-00003570: 2050 7974 686f 6e20 436f 6e6e 6563 746f   Python Connecto
-00003580: 7220 6361 6e20 6265 2075 7365 6420 616c  r can be used al
-00003590: 6f6e 6773 6964 6520 706f 7075 6c61 7220  ongside popular 
-000035a0: 5079 7468 6f6e 2077 6562 2066 7261 6d65  Python web frame
-000035b0: 776f 726b 7320 7375 6368 0a61 7320 466c  works such.as Fl
-000035c0: 6173 6b2c 2046 6173 7441 5049 2c20 6574  ask, FastAPI, et
-000035d0: 632c 2074 6f20 696e 7465 6772 6174 6520  c, to integrate 
-000035e0: 436c 6f75 6420 5351 4c20 6461 7461 6261  Cloud SQL databa
-000035f0: 7365 7320 7769 7468 696e 2079 6f75 720a  ses within your.
-00003600: 7765 6220 6170 706c 6963 6174 696f 6e73  web applications
-00003610: 2e0a 0a23 2323 2320 466c 6173 6b2d 5351  ...#### Flask-SQ
-00003620: 4c41 6c63 6865 6d79 0a0a 5b46 6c61 736b  LAlchemy..[Flask
-00003630: 2d53 514c 416c 6368 656d 795d 2868 7474  -SQLAlchemy](htt
-00003640: 7073 3a2f 2f66 6c61 736b 2d73 716c 616c  ps://flask-sqlal
-00003650: 6368 656d 792e 7061 6c6c 6574 7370 726f  chemy.palletspro
-00003660: 6a65 6374 732e 636f 6d2f 656e 2f32 2e78  jects.com/en/2.x
-00003670: 2f29 0a69 7320 616e 2065 7874 656e 7369  /).is an extensi
-00003680: 6f6e 2066 6f72 205b 466c 6173 6b5d 2868  on for [Flask](h
-00003690: 7474 7073 3a2f 2f66 6c61 736b 2e70 616c  ttps://flask.pal
-000036a0: 6c65 7473 7072 6f6a 6563 7473 2e63 6f6d  letsprojects.com
-000036b0: 2f65 6e2f 322e 322e 782f 290a 7468 6174  /en/2.2.x/).that
-000036c0: 2061 6464 7320 7375 7070 6f72 7420 666f   adds support fo
-000036d0: 7220 5b53 514c 416c 6368 656d 795d 2868  r [SQLAlchemy](h
-000036e0: 7474 7073 3a2f 2f77 7777 2e73 716c 616c  ttps://www.sqlal
-000036f0: 6368 656d 792e 6f72 672f 2920 746f 2079  chemy.org/) to y
-00003700: 6f75 720a 6170 706c 6963 6174 696f 6e2e  our.application.
-00003710: 2049 7420 6169 6d73 2074 6f20 7369 6d70   It aims to simp
-00003720: 6c69 6679 2075 7369 6e67 2053 514c 416c  lify using SQLAl
-00003730: 6368 656d 7920 7769 7468 2046 6c61 736b  chemy with Flask
-00003740: 2062 7920 7072 6f76 6964 696e 670a 7573   by providing.us
-00003750: 6566 756c 2064 6566 6175 6c74 7320 616e  eful defaults an
-00003760: 6420 6578 7472 6120 6865 6c70 6572 7320  d extra helpers 
-00003770: 7468 6174 206d 616b 6520 6974 2065 6173  that make it eas
-00003780: 6965 7220 746f 2061 6363 6f6d 706c 6973  ier to accomplis
-00003790: 680a 636f 6d6d 6f6e 2074 6173 6b73 2e0a  h.common tasks..
-000037a0: 0a59 6f75 2063 616e 2063 6f6e 6669 6775  .You can configu
-000037b0: 7265 2046 6c61 736b 2d53 514c 416c 6368  re Flask-SQLAlch
-000037c0: 656d 7920 746f 2063 6f6e 6e65 6374 2074  emy to connect t
-000037d0: 6f20 6120 436c 6f75 6420 5351 4c20 6461  o a Cloud SQL da
-000037e0: 7461 6261 7365 2066 726f 6d0a 796f 7572  tabase from.your
-000037f0: 2077 6562 2061 7070 6c69 6361 7469 6f6e   web application
-00003800: 2074 6872 6f75 6768 2074 6865 2066 6f6c   through the fol
-00003810: 6c6f 7769 6e67 3a0a 0a60 6060 7079 7468  lowing:..```pyth
-00003820: 6f6e 0a66 726f 6d20 666c 6173 6b20 696d  on.from flask im
-00003830: 706f 7274 2046 6c61 736b 0a66 726f 6d20  port Flask.from 
-00003840: 666c 6173 6b5f 7371 6c61 6c63 6865 6d79  flask_sqlalchemy
-00003850: 2069 6d70 6f72 7420 5351 4c41 6c63 6865   import SQLAlche
-00003860: 6d79 0a66 726f 6d20 676f 6f67 6c65 2e63  my.from google.c
-00003870: 6c6f 7564 2e73 716c 2e63 6f6e 6e65 6374  loud.sql.connect
-00003880: 6f72 2069 6d70 6f72 7420 436f 6e6e 6563  or import Connec
-00003890: 746f 722c 2049 5054 7970 6573 0a0a 0a23  tor, IPTypes...#
-000038a0: 2050 7974 686f 6e20 436f 6e6e 6563 746f   Python Connecto
-000038b0: 7220 6461 7461 6261 7365 2063 6f6e 6e65  r database conne
-000038c0: 6374 696f 6e20 6675 6e63 7469 6f6e 0a64  ction function.d
-000038d0: 6566 2067 6574 636f 6e6e 2829 3a0a 2020  ef getconn():.  
-000038e0: 2020 7769 7468 2043 6f6e 6e65 6374 6f72    with Connector
-000038f0: 2829 2061 7320 636f 6e6e 6563 746f 723a  () as connector:
-00003900: 0a20 2020 2020 2020 2063 6f6e 6e20 3d20  .        conn = 
-00003910: 636f 6e6e 6563 746f 722e 636f 6e6e 6563  connector.connec
-00003920: 7428 0a20 2020 2020 2020 2020 2020 2022  t(.            "
-00003930: 7072 6f6a 6563 743a 7265 6769 6f6e 3a69  project:region:i
-00003940: 6e73 7461 6e63 652d 6e61 6d65 222c 2023  nstance-name", #
-00003950: 2043 6c6f 7564 2053 514c 2049 6e73 7461   Cloud SQL Insta
-00003960: 6e63 6520 436f 6e6e 6563 7469 6f6e 204e  nce Connection N
-00003970: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-00003980: 2270 6738 3030 3022 2c0a 2020 2020 2020  "pg8000",.      
-00003990: 2020 2020 2020 7573 6572 3d22 6d79 2d75        user="my-u
-000039a0: 7365 7222 2c0a 2020 2020 2020 2020 2020  ser",.          
-000039b0: 2020 7061 7373 776f 7264 3d22 6d79 2d70    password="my-p
-000039c0: 6173 7377 6f72 6422 2c0a 2020 2020 2020  assword",.      
-000039d0: 2020 2020 2020 6462 3d22 6d79 2d64 6174        db="my-dat
-000039e0: 6162 6173 6522 2c0a 2020 2020 2020 2020  abase",.        
-000039f0: 2020 2020 6970 5f74 7970 653d 2049 5054      ip_type= IPT
-00003a00: 7970 6573 2e50 5542 4c49 4320 2023 2049  ypes.PUBLIC  # I
-00003a10: 5054 7970 6573 2e50 5249 5641 5445 2066  PTypes.PRIVATE f
-00003a20: 6f72 2070 7269 7661 7465 2049 500a 2020  or private IP.  
-00003a30: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00003a40: 7265 7475 726e 2063 6f6e 6e0a 0a0a 6170  return conn...ap
-00003a50: 7020 3d20 466c 6173 6b28 5f5f 6e61 6d65  p = Flask(__name
-00003a60: 5f5f 290a 0a23 2063 6f6e 6669 6775 7265  __)..# configure
-00003a70: 2046 6c61 736b 2d53 514c 416c 6368 656d   Flask-SQLAlchem
-00003a80: 7920 746f 2075 7365 2050 7974 686f 6e20  y to use Python 
-00003a90: 436f 6e6e 6563 746f 720a 6170 702e 636f  Connector.app.co
-00003aa0: 6e66 6967 5b27 5351 4c41 4c43 4845 4d59  nfig['SQLALCHEMY
-00003ab0: 5f44 4154 4142 4153 455f 5552 4927 5d20  _DATABASE_URI'] 
-00003ac0: 3d20 2270 6f73 7467 7265 7371 6c2b 7067  = "postgresql+pg
-00003ad0: 3830 3030 3a2f 2f22 0a61 7070 2e63 6f6e  8000://".app.con
-00003ae0: 6669 675b 2753 514c 414c 4348 454d 595f  fig['SQLALCHEMY_
-00003af0: 454e 4749 4e45 5f4f 5054 494f 4e53 275d  ENGINE_OPTIONS']
-00003b00: 203d 207b 0a20 2020 2022 6372 6561 746f   = {.    "creato
-00003b10: 7222 3a20 6765 7463 6f6e 6e0a 7d0a 0a64  r": getconn.}..d
-00003b20: 6220 3d20 5351 4c41 6c63 6865 6d79 2861  b = SQLAlchemy(a
-00003b30: 7070 290a 6060 600a 0a46 6f72 206d 6f72  pp).```..For mor
-00003b40: 6520 6465 7461 696c 7320 6f6e 2068 6f77  e details on how
-00003b50: 2074 6f20 7573 6520 466c 6173 6b2d 5351   to use Flask-SQ
-00003b60: 4c41 6c63 6865 6d79 2c20 6368 6563 6b20  LAlchemy, check 
-00003b70: 6f75 7420 7468 650a 5b46 6c61 736b 2d53  out the.[Flask-S
-00003b80: 514c 416c 6368 656d 7920 5175 6963 6b73  QLAlchemy Quicks
-00003b90: 7461 7274 735d 2868 7474 7073 3a2f 2f66  tarts](https://f
-00003ba0: 6c61 736b 2d73 716c 616c 6368 656d 792e  lask-sqlalchemy.
-00003bb0: 7061 6c6c 6574 7370 726f 6a65 6374 732e  palletsprojects.
-00003bc0: 636f 6d2f 656e 2f32 2e78 2f71 7569 636b  com/en/2.x/quick
-00003bd0: 7374 6172 742f 2329 0a0a 2323 2323 2046  start/#)..#### F
-00003be0: 6173 7441 5049 0a0a 5b46 6173 7441 5049  astAPI..[FastAPI
-00003bf0: 5d28 6874 7470 733a 2f2f 6661 7374 6170  ](https://fastap
-00003c00: 692e 7469 616e 676f 6c6f 2e63 6f6d 2f29  i.tiangolo.com/)
-00003c10: 2069 7320 6120 6d6f 6465 726e 2c20 6661   is a modern, fa
-00003c20: 7374 2028 6869 6768 2d70 6572 666f 726d  st (high-perform
-00003c30: 616e 6365 292c 0a77 6562 2066 7261 6d65  ance),.web frame
-00003c40: 776f 726b 2066 6f72 2062 7569 6c64 696e  work for buildin
-00003c50: 6720 4150 4973 2077 6974 6820 5079 7468  g APIs with Pyth
-00003c60: 6f6e 2062 6173 6564 206f 6e20 7374 616e  on based on stan
-00003c70: 6461 7264 2050 7974 686f 6e20 7479 7065  dard Python type
-00003c80: 2068 696e 7473 2e0a 0a59 6f75 2063 616e   hints...You can
-00003c90: 2063 6f6e 6669 6775 7265 2046 6173 7441   configure FastA
-00003ca0: 5049 2074 6f20 636f 6e6e 6563 7420 746f  PI to connect to
-00003cb0: 2061 2043 6c6f 7564 2053 514c 2064 6174   a Cloud SQL dat
-00003cc0: 6162 6173 6520 6672 6f6d 0a79 6f75 7220  abase from.your 
-00003cd0: 7765 6220 6170 706c 6963 6174 696f 6e20  web application 
-00003ce0: 7573 696e 6720 5b53 514c 416c 6368 656d  using [SQLAlchem
-00003cf0: 7920 4f52 4d5d 2868 7474 7073 3a2f 2f64  y ORM](https://d
-00003d00: 6f63 732e 7371 6c61 6c63 6865 6d79 2e6f  ocs.sqlalchemy.o
-00003d10: 7267 2f65 6e2f 3134 2f6f 726d 2f29 0a74  rg/en/14/orm/).t
-00003d20: 6872 6f75 6768 2074 6865 2066 6f6c 6c6f  hrough the follo
-00003d30: 7769 6e67 3a0a 0a60 6060 7079 7468 6f6e  wing:..```python
-00003d40: 0a66 726f 6d20 7371 6c61 6c63 6865 6d79  .from sqlalchemy
-00003d50: 2069 6d70 6f72 7420 6372 6561 7465 5f65   import create_e
-00003d60: 6e67 696e 650a 6672 6f6d 2073 716c 616c  ngine.from sqlal
-00003d70: 6368 656d 792e 6578 742e 6465 636c 6172  chemy.ext.declar
-00003d80: 6174 6976 6520 696d 706f 7274 2064 6563  ative import dec
-00003d90: 6c61 7261 7469 7665 5f62 6173 650a 6672  larative_base.fr
-00003da0: 6f6d 2073 716c 616c 6368 656d 792e 6f72  om sqlalchemy.or
-00003db0: 6d20 696d 706f 7274 2073 6573 7369 6f6e  m import session
-00003dc0: 6d61 6b65 720a 6672 6f6d 2067 6f6f 676c  maker.from googl
-00003dd0: 652e 636c 6f75 642e 7371 6c2e 636f 6e6e  e.cloud.sql.conn
-00003de0: 6563 746f 7220 696d 706f 7274 2043 6f6e  ector import Con
-00003df0: 6e65 6374 6f72 2c20 4950 5479 7065 730a  nector, IPTypes.
-00003e00: 0a23 2050 7974 686f 6e20 436f 6e6e 6563  .# Python Connec
-00003e10: 746f 7220 6461 7461 6261 7365 2063 6f6e  tor database con
-00003e20: 6e65 6374 696f 6e20 6675 6e63 7469 6f6e  nection function
-00003e30: 0a64 6566 2067 6574 636f 6e6e 2829 3a0a  .def getconn():.
-00003e40: 2020 2020 7769 7468 2043 6f6e 6e65 6374      with Connect
-00003e50: 6f72 2829 2061 7320 636f 6e6e 6563 746f  or() as connecto
-00003e60: 723a 0a20 2020 2020 2020 2063 6f6e 6e20  r:.        conn 
-00003e70: 3d20 636f 6e6e 6563 746f 722e 636f 6e6e  = connector.conn
-00003e80: 6563 7428 0a20 2020 2020 2020 2020 2020  ect(.           
-00003e90: 2022 7072 6f6a 6563 743a 7265 6769 6f6e   "project:region
-00003ea0: 3a69 6e73 7461 6e63 652d 6e61 6d65 222c  :instance-name",
-00003eb0: 2023 2043 6c6f 7564 2053 514c 2049 6e73   # Cloud SQL Ins
-00003ec0: 7461 6e63 6520 436f 6e6e 6563 7469 6f6e  tance Connection
-00003ed0: 204e 616d 650a 2020 2020 2020 2020 2020   Name.          
-00003ee0: 2020 2270 6738 3030 3022 2c0a 2020 2020    "pg8000",.    
-00003ef0: 2020 2020 2020 2020 7573 6572 3d22 6d79          user="my
-00003f00: 2d75 7365 7222 2c0a 2020 2020 2020 2020  -user",.        
-00003f10: 2020 2020 7061 7373 776f 7264 3d22 6d79      password="my
-00003f20: 2d70 6173 7377 6f72 6422 2c0a 2020 2020  -password",.    
-00003f30: 2020 2020 2020 2020 6462 3d22 6d79 2d64          db="my-d
-00003f40: 6174 6162 6173 6522 2c0a 2020 2020 2020  atabase",.      
-00003f50: 2020 2020 2020 6970 5f74 7970 653d 2049        ip_type= I
-00003f60: 5054 7970 6573 2e50 5542 4c49 4320 2023  PTypes.PUBLIC  #
-00003f70: 2049 5054 7970 6573 2e50 5249 5641 5445   IPTypes.PRIVATE
-00003f80: 2066 6f72 2070 7269 7661 7465 2049 500a   for private IP.
-00003f90: 2020 2020 2020 2020 290a 2020 2020 7265          ).    re
-00003fa0: 7475 726e 2063 6f6e 6e0a 0a53 514c 414c  turn conn..SQLAL
-00003fb0: 4348 454d 595f 4441 5441 4241 5345 5f55  CHEMY_DATABASE_U
-00003fc0: 524c 203d 2022 706f 7374 6772 6573 716c  RL = "postgresql
-00003fd0: 2b70 6738 3030 303a 2f2f 220a 0a65 6e67  +pg8000://"..eng
-00003fe0: 696e 6520 3d20 6372 6561 7465 5f65 6e67  ine = create_eng
-00003ff0: 696e 6528 0a20 2020 2053 514c 414c 4348  ine(.    SQLALCH
-00004000: 454d 595f 4441 5441 4241 5345 5f55 524c  EMY_DATABASE_URL
-00004010: 202c 2063 7265 6174 6f72 3d67 6574 636f   , creator=getco
-00004020: 6e6e 0a29 0a0a 2320 6372 6561 7465 2053  nn.)..# create S
-00004030: 514c 416c 6368 656d 7920 4f52 4d20 7365  QLAlchemy ORM se
-00004040: 7373 696f 6e0a 5365 7373 696f 6e4c 6f63  ssion.SessionLoc
-00004050: 616c 203d 2073 6573 7369 6f6e 6d61 6b65  al = sessionmake
-00004060: 7228 6175 746f 636f 6d6d 6974 3d46 616c  r(autocommit=Fal
-00004070: 7365 2c20 6175 746f 666c 7573 683d 4661  se, autoflush=Fa
-00004080: 6c73 652c 2062 696e 643d 656e 6769 6e65  lse, bind=engine
-00004090: 290a 0a42 6173 6520 3d20 6465 636c 6172  )..Base = declar
-000040a0: 6174 6976 655f 6261 7365 2829 0a60 6060  ative_base().```
-000040b0: 0a0a 546f 206c 6561 726e 206d 6f72 6520  ..To learn more 
-000040c0: 6162 6f75 7420 696e 7465 6772 6174 696e  about integratin
-000040d0: 6720 6120 6461 7461 6261 7365 2069 6e74  g a database int
-000040e0: 6f20 796f 7572 2046 6173 7441 5049 2061  o your FastAPI a
-000040f0: 7070 6c69 6361 7469 6f6e 2c0a 666f 6c6c  pplication,.foll
-00004100: 6f77 2061 6c6f 6e67 2074 6865 205b 4661  ow along the [Fa
-00004110: 7374 4150 4920 5351 4c20 4461 7461 6261  stAPI SQL Databa
-00004120: 7365 2067 7569 6465 5d28 6874 7470 733a  se guide](https:
-00004130: 2f2f 6661 7374 6170 692e 7469 616e 676f  //fastapi.tiango
-00004140: 6c6f 2e63 6f6d 2f74 7574 6f72 6961 6c2f  lo.com/tutorial/
-00004150: 7371 6c2d 6461 7461 6261 7365 732f 2363  sql-databases/#c
-00004160: 7265 6174 652d 7468 652d 6461 7461 6261  reate-the-databa
-00004170: 7365 2d6d 6f64 656c 7329 2e0a 0a23 2323  se-models)...###
-00004180: 2041 7379 6e63 2044 7269 7665 7220 5573   Async Driver Us
-00004190: 6167 650a 0a54 6865 2043 6c6f 7564 2053  age..The Cloud S
-000041a0: 514c 2043 6f6e 6e65 6374 6f72 2069 7320  QL Connector is 
-000041b0: 636f 6d70 6174 6962 6c65 2077 6974 680a  compatible with.
-000041c0: 5b61 7379 6e63 696f 5d28 6874 7470 733a  [asyncio](https:
-000041d0: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
-000041e0: 672f 332f 6c69 6272 6172 792f 6173 796e  g/3/library/asyn
-000041f0: 6369 6f2e 6874 6d6c 2920 746f 2069 6d70  cio.html) to imp
-00004200: 726f 7665 2074 6865 2073 7065 6564 0a61  rove the speed.a
-00004210: 6e64 2065 6666 6963 6965 6e63 7920 6f66  nd efficiency of
-00004220: 2064 6174 6162 6173 6520 636f 6e6e 6563   database connec
-00004230: 7469 6f6e 7320 7468 726f 7567 6820 636f  tions through co
-00004240: 6e63 7572 7265 6e63 792e 2059 6f75 2063  ncurrency. You c
-00004250: 616e 2075 7365 2061 6c6c 0a6e 6f6e 2d61  an use all.non-a
-00004260: 7379 6e63 696f 2064 7269 7665 7273 2074  syncio drivers t
-00004270: 6872 6f75 6768 2074 6865 2060 436f 6e6e  hrough the `Conn
-00004280: 6563 746f 722e 636f 6e6e 6563 745f 6173  ector.connect_as
-00004290: 796e 6360 2066 756e 6374 696f 6e2c 2069  ync` function, i
-000042a0: 6e20 6164 6469 7469 6f6e 0a74 6f20 7468  n addition.to th
-000042b0: 6520 666f 6c6c 6f77 696e 6720 6173 796e  e following asyn
-000042c0: 6369 6f20 6461 7461 6261 7365 2064 7269  cio database dri
-000042d0: 7665 7273 3a0a 2d20 5b61 7379 6e63 7067  vers:.- [asyncpg
-000042e0: 5d28 6874 7470 733a 2f2f 6d61 6769 6373  ](https://magics
-000042f0: 7461 636b 2e67 6974 6875 622e 696f 2f61  tack.github.io/a
-00004300: 7379 6e63 7067 2920 2850 6f73 7467 7265  syncpg) (Postgre
-00004310: 7329 0a0a 5468 6520 436c 6f75 6420 5351  s)..The Cloud SQ
-00004320: 4c20 436f 6e6e 6563 746f 7220 6861 7320  L Connector has 
-00004330: 6120 6865 6c70 6572 2060 6372 6561 7465  a helper `create
-00004340: 5f61 7379 6e63 5f63 6f6e 6e65 6374 6f72  _async_connector
-00004350: 6020 6675 6e63 7469 6f6e 2074 6861 7420  ` function that 
-00004360: 6973 0a72 6563 6f6d 6d65 6e64 6564 2066  is.recommended f
-00004370: 6f72 2061 7379 6e63 696f 2064 6174 6162  or asyncio datab
-00004380: 6173 6520 636f 6e6e 6563 7469 6f6e 732e  ase connections.
-00004390: 2049 7420 7265 7475 726e 7320 6120 6043   It returns a `C
-000043a0: 6f6e 6e65 6374 6f72 600a 6f62 6a65 6374  onnector`.object
-000043b0: 2074 6861 7420 7573 6573 2074 6865 2063   that uses the c
-000043c0: 7572 7265 6e74 2074 6872 6561 6427 7320  urrent thread's 
-000043d0: 7275 6e6e 696e 6720 6576 656e 7420 6c6f  running event lo
-000043e0: 6f70 2e20 5468 6973 2069 7320 6469 6666  op. This is diff
-000043f0: 6572 656e 740a 7468 616e 2060 436f 6e6e  erent.than `Conn
-00004400: 6563 746f 7228 2960 2077 6869 6368 2062  ector()` which b
-00004410: 7920 6465 6661 756c 7420 696e 6974 6961  y default initia
-00004420: 6c69 7a65 7320 6120 6e65 7720 6576 656e  lizes a new even
-00004430: 7420 6c6f 6f70 2069 6e20 610a 6261 636b  t loop in a.back
-00004440: 6772 6f75 6e64 2074 6872 6561 642e 0a0a  ground thread...
-00004450: 5468 6520 6063 7265 6174 655f 6173 796e  The `create_asyn
-00004460: 635f 636f 6e6e 6563 746f 7260 2061 6c6c  c_connector` all
-00004470: 6f77 7320 616c 6c20 7468 6520 7361 6d65  ows all the same
-00004480: 2069 6e70 7574 2061 7267 756d 656e 7473   input arguments
-00004490: 2061 7320 7468 650a 5b43 6f6e 6e65 6374   as the.[Connect
-000044a0: 6f72 5d28 2363 6f6e 6669 6775 7269 6e67  or](#configuring
-000044b0: 2d74 6865 2d63 6f6e 6e65 6374 6f72 2920  -the-connector) 
-000044c0: 6f62 6a65 6374 2e0a 0a4f 6e63 6520 6120  object...Once a 
-000044d0: 6043 6f6e 6e65 6374 6f72 6020 6f62 6a65  `Connector` obje
-000044e0: 6374 2069 7320 7265 7475 726e 6564 2062  ct is returned b
-000044f0: 7920 6063 7265 6174 655f 6173 796e 635f  y `create_async_
-00004500: 636f 6e6e 6563 746f 7260 2079 6f75 2063  connector` you c
-00004510: 616e 2063 616c 6c0a 6974 7320 6063 6f6e  an call.its `con
-00004520: 6e65 6374 5f61 7379 6e63 6020 6d65 7468  nect_async` meth
-00004530: 6f64 2c20 6a75 7374 2061 7320 796f 7520  od, just as you 
-00004540: 776f 756c 6420 7468 6520 6063 6f6e 6e65  would the `conne
-00004550: 6374 6020 6d65 7468 6f64 3a0a 0a60 6060  ct` method:..```
-00004560: 7079 7468 6f6e 0a69 6d70 6f72 7420 6173  python.import as
-00004570: 796e 6370 670a 0a69 6d70 6f72 7420 7371  yncpg..import sq
-00004580: 6c61 6c63 6865 6d79 0a66 726f 6d20 7371  lalchemy.from sq
-00004590: 6c61 6c63 6865 6d79 2e65 7874 2e61 7379  lalchemy.ext.asy
-000045a0: 6e63 696f 2069 6d70 6f72 7420 4173 796e  ncio import Asyn
-000045b0: 6345 6e67 696e 652c 2063 7265 6174 655f  cEngine, create_
-000045c0: 6173 796e 635f 656e 6769 6e65 0a0a 6672  async_engine..fr
-000045d0: 6f6d 2067 6f6f 676c 652e 636c 6f75 642e  om google.cloud.
-000045e0: 7371 6c2e 636f 6e6e 6563 746f 7220 696d  sql.connector im
-000045f0: 706f 7274 2043 6f6e 6e65 6374 6f72 2c20  port Connector, 
-00004600: 6372 6561 7465 5f61 7379 6e63 5f63 6f6e  create_async_con
-00004610: 6e65 6374 6f72 0a0a 6173 796e 6320 6465  nector..async de
-00004620: 6620 696e 6974 5f63 6f6e 6e65 6374 696f  f init_connectio
-00004630: 6e5f 706f 6f6c 2863 6f6e 6e65 6374 6f72  n_pool(connector
-00004640: 3a20 436f 6e6e 6563 746f 7229 202d 3e20  : Connector) -> 
-00004650: 4173 796e 6345 6e67 696e 653a 0a20 2020  AsyncEngine:.   
-00004660: 2023 2069 6e69 7469 616c 697a 6520 436f   # initialize Co
-00004670: 6e6e 6563 746f 7220 6f62 6a65 6374 2066  nnector object f
-00004680: 6f72 2063 6f6e 6e65 6374 696f 6e73 2074  or connections t
-00004690: 6f20 436c 6f75 6420 5351 4c0a 2020 2020  o Cloud SQL.    
-000046a0: 6173 796e 6320 6465 6620 6765 7463 6f6e  async def getcon
-000046b0: 6e28 2920 2d3e 2061 7379 6e63 7067 2e43  n() -> asyncpg.C
-000046c0: 6f6e 6e65 6374 696f 6e3a 0a20 2020 2020  onnection:.     
-000046d0: 2020 2063 6f6e 6e3a 2061 7379 6e63 7067     conn: asyncpg
-000046e0: 2e43 6f6e 6e65 6374 696f 6e20 3d20 6177  .Connection = aw
-000046f0: 6169 7420 636f 6e6e 6563 746f 722e 636f  ait connector.co
-00004700: 6e6e 6563 745f 6173 796e 6328 0a20 2020  nnect_async(.   
-00004710: 2020 2020 2020 2020 2022 7072 6f6a 6563           "projec
-00004720: 743a 7265 6769 6f6e 3a69 6e73 7461 6e63  t:region:instanc
-00004730: 6522 2c20 2023 2043 6c6f 7564 2053 514c  e",  # Cloud SQL
-00004740: 2069 6e73 7461 6e63 6520 636f 6e6e 6563   instance connec
-00004750: 7469 6f6e 206e 616d 650a 2020 2020 2020  tion name.      
-00004760: 2020 2020 2020 2261 7379 6e63 7067 222c        "asyncpg",
-00004770: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
-00004780: 723d 226d 792d 7573 6572 222c 0a20 2020  r="my-user",.   
-00004790: 2020 2020 2020 2020 2070 6173 7377 6f72           passwor
-000047a0: 643d 226d 792d 7061 7373 776f 7264 222c  d="my-password",
-000047b0: 0a20 2020 2020 2020 2020 2020 2064 623d  .            db=
-000047c0: 226d 792d 6462 2d6e 616d 6522 0a20 2020  "my-db-name".   
-000047d0: 2020 2020 2020 2020 2023 202e 2e2e 2061           # ... a
-000047e0: 6464 6974 696f 6e61 6c20 6461 7461 6261  dditional databa
-000047f0: 7365 2064 7269 7665 7220 6172 6773 0a20  se driver args. 
-00004800: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00004810: 2072 6574 7572 6e20 636f 6e6e 0a0a 2020   return conn..  
-00004820: 2020 2320 5468 6520 436c 6f75 6420 5351    # The Cloud SQ
-00004830: 4c20 5079 7468 6f6e 2043 6f6e 6e65 6374  L Python Connect
-00004840: 6f72 2063 616e 2062 6520 7573 6564 2061  or can be used a
-00004850: 6c6f 6e67 2077 6974 6820 5351 4c41 6c63  long with SQLAlc
-00004860: 6865 6d79 2075 7369 6e67 2074 6865 0a20  hemy using the. 
-00004870: 2020 2023 2027 6173 796e 635f 6372 6561     # 'async_crea
-00004880: 746f 7227 2061 7267 756d 656e 7420 746f  tor' argument to
-00004890: 2027 6372 6561 7465 5f61 7379 6e63 5f65   'create_async_e
-000048a0: 6e67 696e 6527 0a20 2020 2070 6f6f 6c20  ngine'.    pool 
-000048b0: 3d20 6372 6561 7465 5f61 7379 6e63 5f65  = create_async_e
-000048c0: 6e67 696e 6528 0a20 2020 2020 2020 2022  ngine(.        "
-000048d0: 706f 7374 6772 6573 716c 2b61 7379 6e63  postgresql+async
-000048e0: 7067 3a2f 2f22 2c0a 2020 2020 2020 2020  pg://",.        
-000048f0: 6173 796e 635f 6372 6561 746f 723d 6765  async_creator=ge
-00004900: 7463 6f6e 6e2c 0a20 2020 2029 0a20 2020  tconn,.    ).   
-00004910: 2072 6574 7572 6e20 706f 6f6c 0a0a 6173   return pool..as
-00004920: 796e 6320 6465 6620 6d61 696e 2829 3a0a  ync def main():.
-00004930: 2020 2020 2320 696e 6974 6961 6c69 7a65      # initialize
-00004940: 2043 6f6e 6e65 6374 6f72 206f 626a 6563   Connector objec
-00004950: 7420 666f 7220 636f 6e6e 6563 7469 6f6e  t for connection
-00004960: 7320 746f 2043 6c6f 7564 2053 514c 0a20  s to Cloud SQL. 
-00004970: 2020 2063 6f6e 6e65 6374 6f72 203d 2061     connector = a
-00004980: 7761 6974 2063 7265 6174 655f 6173 796e  wait create_asyn
-00004990: 635f 636f 6e6e 6563 746f 7228 290a 0a20  c_connector().. 
-000049a0: 2020 2023 2069 6e69 7469 616c 697a 6520     # initialize 
-000049b0: 636f 6e6e 6563 7469 6f6e 2070 6f6f 6c0a  connection pool.
-000049c0: 2020 2020 706f 6f6c 203d 2061 7761 6974      pool = await
-000049d0: 2069 6e69 745f 636f 6e6e 6563 7469 6f6e   init_connection
-000049e0: 5f70 6f6f 6c28 636f 6e6e 6563 746f 7229  _pool(connector)
-000049f0: 0a0a 2020 2020 2320 6578 616d 706c 6520  ..    # example 
-00004a00: 7175 6572 790a 2020 2020 6173 796e 6320  query.    async 
-00004a10: 7769 7468 2070 6f6f 6c2e 636f 6e6e 6563  with pool.connec
-00004a20: 7428 2920 6173 2063 6f6e 6e3a 0a20 2020  t() as conn:.   
-00004a30: 2020 2020 2061 7761 6974 2063 6f6e 6e2e       await conn.
-00004a40: 6578 6563 7574 6528 7371 6c61 6c63 6865  execute(sqlalche
-00004a50: 6d79 2e74 6578 7428 2253 454c 4543 5420  my.text("SELECT 
-00004a60: 4e4f 5728 2922 2929 0a0a 2020 2020 2320  NOW()"))..    # 
-00004a70: 636c 6f73 6520 436f 6e6e 6563 746f 720a  close Connector.
-00004a80: 2020 2020 6177 6169 7420 636f 6e6e 6563      await connec
-00004a90: 746f 722e 636c 6f73 655f 6173 796e 6328  tor.close_async(
-00004aa0: 290a 0a20 2020 2023 2064 6973 706f 7365  )..    # dispose
-00004ab0: 206f 6620 636f 6e6e 6563 7469 6f6e 2070   of connection p
-00004ac0: 6f6f 6c0a 2020 2020 6177 6169 7420 706f  ool.    await po
-00004ad0: 6f6c 2e64 6973 706f 7365 2829 0a60 6060  ol.dispose().```
-00004ae0: 0a0a 466f 7220 6d6f 7265 2064 6574 6169  ..For more detai
-00004af0: 6c73 206f 6e20 6164 6469 7469 6f6e 616c  ls on additional
-00004b00: 2064 6174 6162 6173 6520 6172 6775 6d65   database argume
-00004b10: 6e74 7320 7769 7468 2061 6e20 6061 7379  nts with an `asy
-00004b20: 6e63 7067 2e43 6f6e 6e65 6374 696f 6e60  ncpg.Connection`
-00004b30: 0a2c 2070 6c65 6173 6520 7669 7369 7420  ., please visit 
-00004b40: 7468 650a 5b6f 6666 6963 6961 6c20 646f  the.[official do
-00004b50: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
-00004b60: 7073 3a2f 2f6d 6167 6963 7374 6163 6b2e  ps://magicstack.
-00004b70: 6769 7468 7562 2e69 6f2f 6173 796e 6370  github.io/asyncp
-00004b80: 672f 6375 7272 656e 742f 6170 692f 696e  g/current/api/in
-00004b90: 6465 782e 6874 6d6c 292e 0a0a 2323 2320  dex.html)...### 
-00004ba0: 4173 796e 6320 436f 6e74 6578 7420 4d61  Async Context Ma
-00004bb0: 6e61 6765 720a 0a41 6e20 616c 7465 726e  nager..An altern
-00004bc0: 6174 6976 6520 746f 2075 7369 6e67 2074  ative to using t
-00004bd0: 6865 2060 6372 6561 7465 5f61 7379 6e63  he `create_async
-00004be0: 5f63 6f6e 6e65 6374 6f72 6020 6675 6e63  _connector` func
-00004bf0: 7469 6f6e 2069 7320 696e 6974 6961 6c69  tion is initiali
-00004c00: 7a69 6e67 0a61 2060 436f 6e6e 6563 746f  zing.a `Connecto
-00004c10: 7260 2061 7320 616e 2061 7379 6e63 2063  r` as an async c
-00004c20: 6f6e 7465 7874 206d 616e 6167 6572 2c20  ontext manager, 
-00004c30: 7265 6d6f 7669 6e67 2074 6865 206e 6565  removing the nee
-00004c40: 6420 666f 7220 6578 706c 6963 6974 0a63  d for explicit.c
-00004c50: 616c 6c73 2074 6f20 6063 6f6e 6e65 6374  alls to `connect
-00004c60: 6f72 2e63 6c6f 7365 5f61 7379 6e63 2829  or.close_async()
-00004c70: 6020 746f 2063 6c65 616e 7570 2072 6573  ` to cleanup res
-00004c80: 6f75 7263 6573 2e0a 0a2a 2a4e 6f74 653a  ources...**Note:
-00004c90: 2a2a 2054 6869 7320 616c 7465 726e 6174  ** This alternat
-00004ca0: 6976 6520 7265 7175 6972 6573 2074 6861  ive requires tha
-00004cb0: 7420 7468 6520 7275 6e6e 696e 6720 6576  t the running ev
-00004cc0: 656e 7420 6c6f 6f70 2062 650a 7061 7373  ent loop be.pass
-00004cd0: 6564 2069 6e20 6173 2074 6865 2060 6c6f  ed in as the `lo
-00004ce0: 6f70 6020 6172 6775 6d65 6e74 2074 6f20  op` argument to 
-00004cf0: 6043 6f6e 6e65 6374 6f72 2829 602e 0a0a  `Connector()`...
-00004d00: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
-00004d10: 2061 7379 6e63 696f 0a69 6d70 6f72 7420   asyncio.import 
-00004d20: 6173 796e 6370 670a 0a69 6d70 6f72 7420  asyncpg..import 
-00004d30: 7371 6c61 6c63 6865 6d79 0a66 726f 6d20  sqlalchemy.from 
-00004d40: 7371 6c61 6c63 6865 6d79 2e65 7874 2e61  sqlalchemy.ext.a
-00004d50: 7379 6e63 696f 2069 6d70 6f72 7420 4173  syncio import As
-00004d60: 796e 6345 6e67 696e 652c 2063 7265 6174  yncEngine, creat
-00004d70: 655f 6173 796e 635f 656e 6769 6e65 0a0a  e_async_engine..
-00004d80: 6672 6f6d 2067 6f6f 676c 652e 636c 6f75  from google.clou
-00004d90: 642e 7371 6c2e 636f 6e6e 6563 746f 7220  d.sql.connector 
-00004da0: 696d 706f 7274 2043 6f6e 6e65 6374 6f72  import Connector
-00004db0: 0a0a 6173 796e 6320 6465 6620 696e 6974  ..async def init
-00004dc0: 5f63 6f6e 6e65 6374 696f 6e5f 706f 6f6c  _connection_pool
-00004dd0: 2863 6f6e 6e65 6374 6f72 3a20 436f 6e6e  (connector: Conn
-00004de0: 6563 746f 7229 202d 3e20 4173 796e 6345  ector) -> AsyncE
-00004df0: 6e67 696e 653a 0a20 2020 2023 2069 6e69  ngine:.    # ini
-00004e00: 7469 616c 697a 6520 436f 6e6e 6563 746f  tialize Connecto
-00004e10: 7220 6f62 6a65 6374 2066 6f72 2063 6f6e  r object for con
-00004e20: 6e65 6374 696f 6e73 2074 6f20 436c 6f75  nections to Clou
-00004e30: 6420 5351 4c0a 2020 2020 6173 796e 6320  d SQL.    async 
-00004e40: 6465 6620 6765 7463 6f6e 6e28 2920 2d3e  def getconn() ->
-00004e50: 2061 7379 6e63 7067 2e43 6f6e 6e65 6374   asyncpg.Connect
-00004e60: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-00004e70: 2063 6f6e 6e3a 2061 7379 6e63 7067 2e43   conn: asyncpg.C
-00004e80: 6f6e 6e65 6374 696f 6e20 3d20 6177 6169  onnection = awai
-00004e90: 7420 636f 6e6e 6563 746f 722e 636f 6e6e  t connector.conn
-00004ea0: 6563 745f 6173 796e 6328 0a20 2020 2020  ect_async(.     
-00004eb0: 2020 2020 2020 2020 2020 2022 7072 6f6a             "proj
-00004ec0: 6563 743a 7265 6769 6f6e 3a69 6e73 7461  ect:region:insta
-00004ed0: 6e63 6522 2c20 2023 2043 6c6f 7564 2053  nce",  # Cloud S
-00004ee0: 514c 2069 6e73 7461 6e63 6520 636f 6e6e  QL instance conn
-00004ef0: 6563 7469 6f6e 206e 616d 650a 2020 2020  ection name.    
-00004f00: 2020 2020 2020 2020 2020 2020 2261 7379              "asy
-00004f10: 6e63 7067 222c 0a20 2020 2020 2020 2020  ncpg",.         
-00004f20: 2020 2020 2020 2075 7365 723d 226d 792d         user="my-
-00004f30: 7573 6572 222c 0a20 2020 2020 2020 2020  user",.         
-00004f40: 2020 2020 2020 2070 6173 7377 6f72 643d         password=
-00004f50: 226d 792d 7061 7373 776f 7264 222c 0a20  "my-password",. 
-00004f60: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004f70: 623d 226d 792d 6462 2d6e 616d 6522 0a20  b="my-db-name". 
-00004f80: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00004f90: 202e 2e2e 2061 6464 6974 696f 6e61 6c20   ... additional 
-00004fa0: 6461 7461 6261 7365 2064 7269 7665 7220  database driver 
-00004fb0: 6172 6773 0a20 2020 2020 2020 2020 2020  args.           
-00004fc0: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
-00004fd0: 6574 7572 6e20 636f 6e6e 0a0a 2020 2020  eturn conn..    
-00004fe0: 2320 5468 6520 436c 6f75 6420 5351 4c20  # The Cloud SQL 
-00004ff0: 5079 7468 6f6e 2043 6f6e 6e65 6374 6f72  Python Connector
-00005000: 2063 616e 2062 6520 7573 6564 2061 6c6f   can be used alo
-00005010: 6e67 2077 6974 6820 5351 4c41 6c63 6865  ng with SQLAlche
-00005020: 6d79 2075 7369 6e67 2074 6865 0a20 2020  my using the.   
-00005030: 2023 2027 6173 796e 635f 6372 6561 746f   # 'async_creato
-00005040: 7227 2061 7267 756d 656e 7420 746f 2027  r' argument to '
-00005050: 6372 6561 7465 5f61 7379 6e63 5f65 6e67  create_async_eng
-00005060: 696e 6527 0a20 2020 2070 6f6f 6c20 3d20  ine'.    pool = 
-00005070: 6372 6561 7465 5f61 7379 6e63 5f65 6e67  create_async_eng
-00005080: 696e 6528 0a20 2020 2020 2020 2022 706f  ine(.        "po
-00005090: 7374 6772 6573 716c 2b61 7379 6e63 7067  stgresql+asyncpg
-000050a0: 3a2f 2f22 2c0a 2020 2020 2020 2020 6173  ://",.        as
-000050b0: 796e 635f 6372 6561 746f 723d 6765 7463  ync_creator=getc
-000050c0: 6f6e 6e2c 0a20 2020 2029 0a20 2020 2072  onn,.    ).    r
-000050d0: 6574 7572 6e20 706f 6f6c 0a0a 6173 796e  eturn pool..asyn
-000050e0: 6320 6465 6620 6d61 696e 2829 3a0a 2020  c def main():.  
-000050f0: 2020 2320 696e 6974 6961 6c69 7a65 2043    # initialize C
-00005100: 6f6e 6e65 6374 6f72 206f 626a 6563 7420  onnector object 
-00005110: 666f 7220 636f 6e6e 6563 7469 6f6e 7320  for connections 
-00005120: 746f 2043 6c6f 7564 2053 514c 0a20 2020  to Cloud SQL.   
-00005130: 206c 6f6f 7020 3d20 6173 796e 6369 6f2e   loop = asyncio.
-00005140: 6765 745f 7275 6e6e 696e 675f 6c6f 6f70  get_running_loop
-00005150: 2829 0a20 2020 2061 7379 6e63 2077 6974  ().    async wit
-00005160: 6820 436f 6e6e 6563 746f 7228 6c6f 6f70  h Connector(loop
-00005170: 3d6c 6f6f 7029 2061 7320 636f 6e6e 6563  =loop) as connec
-00005180: 746f 723a 0a20 2020 2020 2020 2023 2069  tor:.        # i
-00005190: 6e69 7469 616c 697a 6520 636f 6e6e 6563  nitialize connec
-000051a0: 7469 6f6e 2070 6f6f 6c0a 2020 2020 2020  tion pool.      
-000051b0: 2020 706f 6f6c 203d 2061 7761 6974 2069    pool = await i
-000051c0: 6e69 745f 636f 6e6e 6563 7469 6f6e 5f70  nit_connection_p
-000051d0: 6f6f 6c28 636f 6e6e 6563 746f 7229 0a0a  ool(connector)..
-000051e0: 2020 2020 2020 2020 2320 6578 616d 706c          # exampl
-000051f0: 6520 7175 6572 790a 2020 2020 2020 2020  e query.        
-00005200: 6173 796e 6320 7769 7468 2070 6f6f 6c2e  async with pool.
-00005210: 636f 6e6e 6563 7428 2920 6173 2063 6f6e  connect() as con
-00005220: 6e3a 0a20 2020 2020 2020 2020 2020 2061  n:.            a
-00005230: 7761 6974 2063 6f6e 6e2e 6578 6563 7574  wait conn.execut
-00005240: 6528 7371 6c61 6c63 6865 6d79 2e74 6578  e(sqlalchemy.tex
-00005250: 7428 2253 454c 4543 5420 4e4f 5728 2922  t("SELECT NOW()"
-00005260: 2929 0a0a 2020 2020 2020 2020 2320 6469  ))..        # di
-00005270: 7370 6f73 6520 6f66 2063 6f6e 6e65 6374  spose of connect
-00005280: 696f 6e20 706f 6f6c 0a20 2020 2020 2020  ion pool.       
-00005290: 2061 7761 6974 2070 6f6f 6c2e 6469 7370   await pool.disp
-000052a0: 6f73 6528 290a 6060 600a 0a23 2320 5375  ose().```..## Su
-000052b0: 7070 6f72 7420 706f 6c69 6379 0a0a 2323  pport policy..##
-000052c0: 2320 4d61 6a6f 7220 7665 7273 696f 6e20  # Major version 
-000052d0: 6c69 6665 6379 636c 650a 0a54 6869 7320  lifecycle..This 
-000052e0: 7072 6f6a 6563 7420 7573 6573 205b 7365  project uses [se
-000052f0: 6d61 6e74 6963 2076 6572 7369 6f6e 696e  mantic versionin
-00005300: 675d 2868 7474 7073 3a2f 2f73 656d 7665  g](https://semve
-00005310: 722e 6f72 672f 292c 2061 6e64 2075 7365  r.org/), and use
-00005320: 7320 7468 650a 666f 6c6c 6f77 696e 6720  s the.following 
-00005330: 6c69 6665 6379 636c 6520 7265 6761 7264  lifecycle regard
-00005340: 696e 6720 7375 7070 6f72 7420 666f 7220  ing support for 
-00005350: 6120 6d61 6a6f 7220 7665 7273 696f 6e3a  a major version:
-00005360: 0a0a 2a2a 4163 7469 7665 2a2a 202d 2041  ..**Active** - A
-00005370: 6374 6976 6520 7665 7273 696f 6e73 2067  ctive versions g
-00005380: 6574 2061 6c6c 206e 6577 2066 6561 7475  et all new featu
-00005390: 7265 7320 616e 6420 7365 6375 7269 7479  res and security
-000053a0: 2066 6978 6573 2028 7468 6174 0a77 6f75   fixes (that.wou
-000053b0: 6c64 6ee2 8099 7420 6f74 6865 7277 6973  ldn...t otherwis
-000053c0: 6520 696e 7472 6f64 7563 6520 6120 6272  e introduce a br
-000053d0: 6561 6b69 6e67 2063 6861 6e67 6529 2e20  eaking change). 
-000053e0: 4e65 7720 6d61 6a6f 7220 7665 7273 696f  New major versio
-000053f0: 6e73 2061 7265 0a67 7561 7261 6e74 6565  ns are.guarantee
-00005400: 6420 746f 2062 6520 2261 6374 6976 6522  d to be "active"
-00005410: 2066 6f72 2061 206d 696e 696d 756d 206f   for a minimum o
-00005420: 6620 3120 7965 6172 2e0a 2a2a 4465 7072  f 1 year..**Depr
-00005430: 6563 6174 6564 2a2a 202d 2044 6570 7265  ecated** - Depre
-00005440: 6361 7465 6420 7665 7273 696f 6e73 2063  cated versions c
-00005450: 6f6e 7469 6e75 6520 746f 2072 6563 6569  ontinue to recei
-00005460: 7665 2073 6563 7572 6974 7920 616e 6420  ve security and 
-00005470: 6372 6974 6963 616c 0a62 7567 2066 6978  critical.bug fix
-00005480: 6573 2c20 6275 7420 646f 206e 6f74 2072  es, but do not r
-00005490: 6563 6569 7665 206e 6577 2066 6561 7475  eceive new featu
-000054a0: 7265 732e 2044 6570 7265 6361 7465 6420  res. Deprecated 
-000054b0: 7665 7273 696f 6e73 2077 696c 6c20 6265  versions will be
-000054c0: 2070 7562 6c69 636c 790a 7375 7070 6f72   publicly.suppor
-000054d0: 7465 6420 666f 7220 3120 7965 6172 2e0a  ted for 1 year..
-000054e0: 2a2a 556e 7375 7070 6f72 7465 642a 2a20  **Unsupported** 
-000054f0: 2d20 416e 7920 6d61 6a6f 7220 7665 7273  - Any major vers
-00005500: 696f 6e20 7468 6174 2068 6173 2062 6565  ion that has bee
-00005510: 6e20 6465 7072 6563 6174 6564 2066 6f72  n deprecated for
-00005520: 203e 3d31 2079 6561 7220 6973 0a63 6f6e   >=1 year is.con
-00005530: 7369 6465 7265 6420 7075 626c 6963 6c79  sidered publicly
-00005540: 2075 6e73 7570 706f 7274 6564 2e0a 0a23   unsupported...#
-00005550: 2320 5375 7070 6f72 7465 6420 5079 7468  # Supported Pyth
-00005560: 6f6e 2056 6572 7369 6f6e 730a 0a57 6520  on Versions..We 
-00005570: 7465 7374 2061 6e64 2073 7570 706f 7274  test and support
-00005580: 2061 7420 6120 6d69 6e69 6d75 6d2c 2065   at a minimum, e
-00005590: 7665 7279 205b 6163 7469 7665 2076 6572  very [active ver
-000055a0: 7369 6f6e 2075 6e74 696c 2069 7427 730a  sion until it's.
-000055b0: 656e 642d 6f66 2d6c 6966 6520 6461 7465  end-of-life date
-000055c0: 5d5b 7079 7665 725d 2e20 4368 616e 6765  ][pyver]. Change
-000055d0: 7320 696e 2073 7570 706f 7274 6564 2050  s in supported P
-000055e0: 7974 686f 6e20 7665 7273 696f 6e73 2077  ython versions w
-000055f0: 696c 6c20 6265 0a63 6f6e 7369 6465 7265  ill be.considere
-00005600: 6420 6120 6d69 6e6f 7220 6368 616e 6765  d a minor change
-00005610: 2c20 616e 6420 7769 6c6c 2062 6520 6c69  , and will be li
-00005620: 7374 6564 2069 6e20 7468 6520 7265 6c65  sted in the rele
-00005630: 6173 6520 6e6f 7465 732e 0a0a 5b70 7976  ase notes...[pyv
-00005640: 6572 5d3a 2068 7474 7073 3a2f 2f64 6576  er]: https://dev
-00005650: 6775 6964 652e 7079 7468 6f6e 2e6f 7267  guide.python.org
-00005660: 2f23 7374 6174 7573 2d6f 662d 7079 7468  /#status-of-pyth
-00005670: 6f6e 2d62 7261 6e63 6865 730a 0a23 2323  on-branches..###
-00005680: 2052 656c 6561 7365 2063 6164 656e 6365   Release cadence
-00005690: 0a54 6869 7320 7072 6f6a 6563 7420 6169  .This project ai
-000056a0: 6d73 2066 6f72 2061 206d 696e 696d 756d  ms for a minimum
-000056b0: 206d 6f6e 7468 6c79 2072 656c 6561 7365   monthly release
-000056c0: 2063 6164 656e 6365 2e20 4966 206e 6f20   cadence. If no 
-000056d0: 6e65 770a 6665 6174 7572 6573 206f 7220  new.features or 
-000056e0: 6669 7865 7320 6861 7665 2062 6565 6e20  fixes have been 
-000056f0: 6164 6465 642c 2061 206e 6577 2050 4154  added, a new PAT
-00005700: 4348 2076 6572 7369 6f6e 2077 6974 6820  CH version with 
-00005710: 7468 6520 6c61 7465 7374 0a64 6570 656e  the latest.depen
-00005720: 6465 6e63 6965 7320 6973 2072 656c 6561  dencies is relea
-00005730: 7365 642e 0a0a 2323 2320 436f 6e74 7269  sed...### Contri
-00005740: 6275 7469 6e67 0a0a 5765 2077 656c 636f  buting..We welco
-00005750: 6d65 206f 7574 7369 6465 2063 6f6e 7472  me outside contr
-00005760: 6962 7574 696f 6e73 2e20 506c 6561 7365  ibutions. Please
-00005770: 2073 6565 206f 7572 0a5b 436f 6e74 7269   see our.[Contri
-00005780: 6275 7469 6e67 2047 7569 6465 5d28 434f  buting Guide](CO
-00005790: 4e54 5249 4255 5449 4e47 2e6d 6429 2066  NTRIBUTING.md) f
-000057a0: 6f72 2064 6574 6169 6c73 206f 6e20 686f  or details on ho
-000057b0: 7720 6265 7374 2074 6f20 636f 6e74 7269  w best to contri
-000057c0: 6275 7465 2e0a                           bute..
+00000360: 3130 0a43 6c61 7373 6966 6965 723a 2050  10.Classifier: P
+00000370: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000380: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000390: 2033 2e31 310a 5265 7175 6972 6573 2d50   3.11.Requires-P
+000003a0: 7974 686f 6e3a 203e 3d33 2e38 0a44 6573  ython: >=3.8.Des
+000003b0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+000003c0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+000003d0: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
+000003e0: 7472 613a 2070 796d 7973 716c 0a50 726f  tra: pymysql.Pro
+000003f0: 7669 6465 732d 4578 7472 613a 2070 6738  vides-Extra: pg8
+00000400: 3030 300a 5072 6f76 6964 6573 2d45 7874  000.Provides-Ext
+00000410: 7261 3a20 7079 7464 730a 5072 6f76 6964  ra: pytds.Provid
+00000420: 6573 2d45 7874 7261 3a20 6173 796e 6370  es-Extra: asyncp
+00000430: 670a 4c69 6365 6e73 652d 4669 6c65 3a20  g.License-File: 
+00000440: 4c49 4345 4e53 450a 0a3c 7020 616c 6967  LICENSE..<p alig
+00000450: 6e3d 2263 656e 7465 7222 3e0a 2020 2020  n="center">.    
+00000460: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000470: 2f63 6c6f 7564 2e67 6f6f 676c 652e 636f  /cloud.google.co
+00000480: 6d2f 626c 6f67 2f74 6f70 6963 732f 6465  m/blog/topics/de
+00000490: 7665 6c6f 7065 7273 2d70 7261 6374 6974  velopers-practit
+000004a0: 696f 6e65 7273 2f68 6f77 2d63 6f6e 6e65  ioners/how-conne
+000004b0: 6374 2d63 6c6f 7564 2d73 716c 2d75 7369  ct-cloud-sql-usi
+000004c0: 6e67 2d70 7974 686f 6e2d 6561 7379 2d77  ng-python-easy-w
+000004d0: 6179 223e 0a20 2020 2020 2020 203c 696d  ay">.        <im
+000004e0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+000004f0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00000500: 7465 6e74 2e63 6f6d 2f47 6f6f 676c 6543  tent.com/GoogleC
+00000510: 6c6f 7564 506c 6174 666f 726d 2f63 6c6f  loudPlatform/clo
+00000520: 7564 2d73 716c 2d70 7974 686f 6e2d 636f  ud-sql-python-co
+00000530: 6e6e 6563 746f 722f 6d61 696e 2f64 6f63  nnector/main/doc
+00000540: 732f 696d 6167 6573 2f63 6c6f 7564 2d73  s/images/cloud-s
+00000550: 716c 2d70 7974 686f 6e2d 636f 6e6e 6563  ql-python-connec
+00000560: 746f 722e 706e 6722 2061 6c74 3d22 636c  tor.png" alt="cl
+00000570: 6f75 642d 7371 6c2d 7079 7468 6f6e 2d63  oud-sql-python-c
+00000580: 6f6e 6e65 6374 6f72 2069 6d61 6765 223e  onnector image">
+00000590: 0a20 2020 203c 2f61 3e0a 3c2f 703e 0a0a  .    </a>.</p>..
+000005a0: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+000005b0: 7222 3e43 6c6f 7564 2053 514c 2050 7974  r">Cloud SQL Pyt
+000005c0: 686f 6e20 436f 6e6e 6563 746f 723c 2f68  hon Connector</h
+000005d0: 313e 0a0a 5b21 5b4f 7065 6e20 496e 2043  1>..[![Open In C
+000005e0: 6f6c 6162 5d5b 636f 6c61 622d 6261 6467  olab][colab-badg
+000005f0: 655d 5d5b 636f 6c61 622d 6e6f 7465 626f  e]][colab-notebo
+00000600: 6f6b 5d0a 5b21 5b43 495d 5b63 692d 6261  ok].[![CI][ci-ba
+00000610: 6467 655d 5d5b 6369 2d62 7569 6c64 5d0a  dge]][ci-build].
+00000620: 5b21 5b70 7970 695d 5b70 7970 692d 6261  [![pypi][pypi-ba
+00000630: 6467 655d 5d5b 7079 7069 2d64 6f63 735d  dge]][pypi-docs]
+00000640: 0a5b 215b 5079 5049 2064 6f77 6e6c 6f61  .[![PyPI downloa
+00000650: 6420 6d6f 6e74 685d 5b70 7970 692d 646f  d month][pypi-do
+00000660: 776e 6c6f 6164 735d 5d5b 7079 7069 2d64  wnloads]][pypi-d
+00000670: 6f63 735d 0a5b 215b 7079 7468 6f6e 5d5b  ocs].[![python][
+00000680: 7079 7468 6f6e 2d76 6572 7369 6f6e 735d  python-versions]
+00000690: 5d5b 7079 7069 2d64 6f63 735d 0a0a 5b63  ][pypi-docs]..[c
+000006a0: 6f6c 6162 2d62 6164 6765 5d3a 2068 7474  olab-badge]: htt
+000006b0: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+000006c0: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f61  rch.google.com/a
+000006d0: 7373 6574 732f 636f 6c61 622d 6261 6467  ssets/colab-badg
+000006e0: 652e 7376 670a 5b63 6f6c 6162 2d6e 6f74  e.svg.[colab-not
+000006f0: 6562 6f6f 6b5d 3a20 6874 7470 733a 2f2f  ebook]: https://
+00000700: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+00000710: 6f6f 676c 652e 636f 6d2f 6769 7468 7562  oogle.com/github
+00000720: 2f47 6f6f 676c 6543 6c6f 7564 506c 6174  /GoogleCloudPlat
+00000730: 666f 726d 2f63 6c6f 7564 2d73 716c 2d70  form/cloud-sql-p
+00000740: 7974 686f 6e2d 636f 6e6e 6563 746f 722f  ython-connector/
+00000750: 626c 6f62 2f6d 6169 6e2f 7361 6d70 6c65  blob/main/sample
+00000760: 732f 6e6f 7465 626f 6f6b 732f 706f 7374  s/notebooks/post
+00000770: 6772 6573 5f70 7974 686f 6e5f 636f 6e6e  gres_python_conn
+00000780: 6563 746f 722e 6970 796e 620a 5b63 692d  ector.ipynb.[ci-
+00000790: 6261 6467 655d 3a20 6874 7470 733a 2f2f  badge]: https://
+000007a0: 6769 7468 7562 2e63 6f6d 2f47 6f6f 676c  github.com/Googl
+000007b0: 6543 6c6f 7564 506c 6174 666f 726d 2f63  eCloudPlatform/c
+000007c0: 6c6f 7564 2d73 716c 2d70 7974 686f 6e2d  loud-sql-python-
+000007d0: 636f 6e6e 6563 746f 722f 6163 7469 6f6e  connector/action
+000007e0: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
+000007f0: 732e 796d 6c2f 6261 6467 652e 7376 673f  s.yml/badge.svg?
+00000800: 6576 656e 743d 7075 7368 0a5b 6369 2d62  event=push.[ci-b
+00000810: 7569 6c64 5d3a 2068 7474 7073 3a2f 2f67  uild]: https://g
+00000820: 6974 6875 622e 636f 6d2f 476f 6f67 6c65  ithub.com/Google
+00000830: 436c 6f75 6450 6c61 7466 6f72 6d2f 636c  CloudPlatform/cl
+00000840: 6f75 642d 7371 6c2d 7079 7468 6f6e 2d63  oud-sql-python-c
+00000850: 6f6e 6e65 6374 6f72 2f61 6374 696f 6e73  onnector/actions
+00000860: 2f77 6f72 6b66 6c6f 7773 2f74 6573 7473  /workflows/tests
+00000870: 2e79 6d6c 3f71 7565 7279 3d65 7665 6e74  .yml?query=event
+00000880: 2533 4170 7573 682b 6272 616e 6368 2533  %3Apush+branch%3
+00000890: 416d 6169 6e0a 5b70 7970 692d 6261 6467  Amain.[pypi-badg
+000008a0: 655d 3a20 6874 7470 733a 2f2f 696d 672e  e]: https://img.
+000008b0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+000008c0: 762f 636c 6f75 642d 7371 6c2d 7079 7468  v/cloud-sql-pyth
+000008d0: 6f6e 2d63 6f6e 6e65 6374 6f72 0a5b 7079  on-connector.[py
+000008e0: 7069 2d64 6f63 735d 3a20 6874 7470 733a  pi-docs]: https:
+000008f0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000900: 6374 2f63 6c6f 7564 2d73 716c 2d70 7974  ct/cloud-sql-pyt
+00000910: 686f 6e2d 636f 6e6e 6563 746f 720a 5b70  hon-connector.[p
+00000920: 7970 692d 646f 776e 6c6f 6164 735d 3a20  ypi-downloads]: 
+00000930: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000940: 6c64 732e 696f 2f70 7970 692f 646d 2f63  lds.io/pypi/dm/c
+00000950: 6c6f 7564 2d73 716c 2d70 7974 686f 6e2d  loud-sql-python-
+00000960: 636f 6e6e 6563 746f 722e 7376 670a 5b70  connector.svg.[p
+00000970: 7974 686f 6e2d 7665 7273 696f 6e73 5d3a  ython-versions]:
+00000980: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
+00000990: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
+000009a0: 6572 7369 6f6e 732f 636c 6f75 642d 7371  ersions/cloud-sq
+000009b0: 6c2d 7079 7468 6f6e 2d63 6f6e 6e65 6374  l-python-connect
+000009c0: 6f72 0a0a 5468 6520 5f43 6c6f 7564 2053  or..The _Cloud S
+000009d0: 514c 2050 7974 686f 6e20 436f 6e6e 6563  QL Python Connec
+000009e0: 746f 725f 2069 7320 6120 436c 6f75 6420  tor_ is a Cloud 
+000009f0: 5351 4c20 636f 6e6e 6563 746f 7220 6465  SQL connector de
+00000a00: 7369 676e 6564 2066 6f72 2075 7365 2077  signed for use w
+00000a10: 6974 6820 7468 650a 5079 7468 6f6e 206c  ith the.Python l
+00000a20: 616e 6775 6167 652e 2055 7369 6e67 2061  anguage. Using a
+00000a30: 2043 6c6f 7564 2053 514c 2063 6f6e 6e65   Cloud SQL conne
+00000a40: 6374 6f72 2070 726f 7669 6465 7320 6120  ctor provides a 
+00000a50: 6e61 7469 7665 2061 6c74 6572 6e61 7469  native alternati
+00000a60: 7665 2074 6f20 7468 650a 5b43 6c6f 7564  ve to the.[Cloud
+00000a70: 2053 514c 2041 7574 6820 5072 6f78 795d   SQL Auth Proxy]
+00000a80: 2868 7474 7073 3a2f 2f63 6c6f 7564 2e67  (https://cloud.g
+00000a90: 6f6f 676c 652e 636f 6d2f 7371 6c2f 646f  oogle.com/sql/do
+00000aa0: 6373 2f6d 7973 716c 2f73 716c 2d70 726f  cs/mysql/sql-pro
+00000ab0: 7879 2920 7768 696c 650a 7072 6f76 6964  xy) while.provid
+00000ac0: 696e 6720 7468 6520 666f 6c6c 6f77 696e  ing the followin
+00000ad0: 6720 6265 6e65 6669 7473 3a0a 0a2a 202a  g benefits:..* *
+00000ae0: 2a49 414d 2041 7574 686f 7269 7a61 7469  *IAM Authorizati
+00000af0: 6f6e 3a2a 2a20 7573 6573 2049 414d 2070  on:** uses IAM p
+00000b00: 6572 6d69 7373 696f 6e73 2074 6f20 636f  ermissions to co
+00000b10: 6e74 726f 6c20 7768 6f2f 7768 6174 2063  ntrol who/what c
+00000b20: 616e 2063 6f6e 6e65 6374 2074 6f0a 2020  an connect to.  
+00000b30: 796f 7572 2043 6c6f 7564 2053 514c 2069  your Cloud SQL i
+00000b40: 6e73 7461 6e63 6573 0a2a 202a 2a49 6d70  nstances.* **Imp
+00000b50: 726f 7665 6420 5365 6375 7269 7479 3a2a  roved Security:*
+00000b60: 2a20 7573 6573 2072 6f62 7573 742c 2075  * uses robust, u
+00000b70: 7064 6174 6564 2054 4c53 2031 2e33 2065  pdated TLS 1.3 e
+00000b80: 6e63 7279 7074 696f 6e20 616e 640a 2020  ncryption and.  
+00000b90: 6964 656e 7469 7479 2076 6572 6966 6963  identity verific
+00000ba0: 6174 696f 6e20 6265 7477 6565 6e20 7468  ation between th
+00000bb0: 6520 636c 6965 6e74 2063 6f6e 6e65 6374  e client connect
+00000bc0: 6f72 2061 6e64 2074 6865 2073 6572 7665  or and the serve
+00000bd0: 722d 7369 6465 2070 726f 7879 2c0a 2020  r-side proxy,.  
+00000be0: 696e 6465 7065 6e64 656e 7420 6f66 2074  independent of t
+00000bf0: 6865 2064 6174 6162 6173 6520 7072 6f74  he database prot
+00000c00: 6f63 6f6c 2e0a 2a20 2a2a 436f 6e76 656e  ocol..* **Conven
+00000c10: 6965 6e63 653a 2a2a 2072 656d 6f76 6573  ience:** removes
+00000c20: 2074 6865 2072 6571 7569 7265 6d65 6e74   the requirement
+00000c30: 2074 6f20 7573 6520 616e 6420 6469 7374   to use and dist
+00000c40: 7269 6275 7465 2053 534c 0a20 2063 6572  ribute SSL.  cer
+00000c50: 7469 6669 6361 7465 732c 2061 7320 7765  tificates, as we
+00000c60: 6c6c 2061 7320 6d61 6e61 6765 2066 6972  ll as manage fir
+00000c70: 6577 616c 6c73 206f 7220 736f 7572 6365  ewalls or source
+00000c80: 2f64 6573 7469 6e61 7469 6f6e 2049 5020  /destination IP 
+00000c90: 6164 6472 6573 7365 732e 0a2a 2028 6f70  addresses..* (op
+00000ca0: 7469 6f6e 616c 6c79 2920 2a2a 4941 4d20  tionally) **IAM 
+00000cb0: 4442 2041 7574 6865 6e74 6963 6174 696f  DB Authenticatio
+00000cc0: 6e3a 2a2a 2070 726f 7669 6465 7320 7375  n:** provides su
+00000cd0: 7070 6f72 7420 666f 720a 2020 5b43 6c6f  pport for.  [Clo
+00000ce0: 7564 2053 514c e280 9973 2061 7574 6f6d  ud SQL...s autom
+00000cf0: 6174 6963 2049 414d 2044 4220 4175 7468  atic IAM DB Auth
+00000d00: 4e5d 5b69 616d 2d64 622d 6175 7468 6e5d  N][iam-db-authn]
+00000d10: 2066 6561 7475 7265 2e0a 0a5b 6961 6d2d   feature...[iam-
+00000d20: 6462 2d61 7574 686e 5d3a 2068 7474 7073  db-authn]: https
+00000d30: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
+00000d40: 636f 6d2f 7371 6c2f 646f 6373 2f70 6f73  com/sql/docs/pos
+00000d50: 7467 7265 732f 6175 7468 656e 7469 6361  tgres/authentica
+00000d60: 7469 6f6e 0a0a 5468 6520 436c 6f75 6420  tion..The Cloud 
+00000d70: 5351 4c20 5079 7468 6f6e 2043 6f6e 6e65  SQL Python Conne
+00000d80: 6374 6f72 2069 7320 6120 7061 636b 6167  ctor is a packag
+00000d90: 6520 746f 2062 6520 7573 6564 2061 6c6f  e to be used alo
+00000da0: 6e67 7369 6465 2061 2064 6174 6162 6173  ngside a databas
+00000db0: 6520 6472 6976 6572 2e0a 4375 7272 656e  e driver..Curren
+00000dc0: 746c 7920 7375 7070 6f72 7465 6420 6472  tly supported dr
+00000dd0: 6976 6572 7320 6172 653a 0a20 2d20 5b60  ivers are:. - [`
+00000de0: 7079 6d79 7371 6c60 5d28 6874 7470 733a  pymysql`](https:
+00000df0: 2f2f 6769 7468 7562 2e63 6f6d 2f50 794d  //github.com/PyM
+00000e00: 7953 514c 2f50 794d 7953 514c 2920 284d  ySQL/PyMySQL) (M
+00000e10: 7953 514c 290a 202d 205b 6070 6738 3030  ySQL). - [`pg800
+00000e20: 3060 5d28 6874 7470 733a 2f2f 6769 7468  0`](https://gith
+00000e30: 7562 2e63 6f6d 2f74 6c6f 636b 652f 7067  ub.com/tlocke/pg
+00000e40: 3830 3030 2920 2850 6f73 7467 7265 5351  8000) (PostgreSQ
+00000e50: 4c29 0a20 2d20 5b60 6173 796e 6370 6760  L). - [`asyncpg`
+00000e60: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000e70: 2e63 6f6d 2f4d 6167 6963 5374 6163 6b2f  .com/MagicStack/
+00000e80: 6173 796e 6370 6729 2028 506f 7374 6772  asyncpg) (Postgr
+00000e90: 6553 514c 290a 202d 205b 6070 7974 6473  eSQL). - [`pytds
+00000ea0: 605d 2868 7474 7073 3a2f 2f67 6974 6875  `](https://githu
+00000eb0: 622e 636f 6d2f 6465 6e69 7365 6e6b 6f6d  b.com/denisenkom
+00000ec0: 2f70 7974 6473 2920 2853 514c 2053 6572  /pytds) (SQL Ser
+00000ed0: 7665 7229 0a0a 0a23 2320 496e 7374 616c  ver)...## Instal
+00000ee0: 6c61 7469 6f6e 0a0a 596f 7520 6361 6e20  lation..You can 
+00000ef0: 696e 7374 616c 6c20 7468 6973 206c 6962  install this lib
+00000f00: 7261 7279 2077 6974 6820 6070 6970 2069  rary with `pip i
+00000f10: 6e73 7461 6c6c 602c 2073 7065 6369 6679  nstall`, specify
+00000f20: 696e 6720 7468 6520 6472 6976 6572 0a62  ing the driver.b
+00000f30: 6173 6564 206f 6e20 796f 7572 2064 6174  ased on your dat
+00000f40: 6162 6173 6520 6469 616c 6563 742e 0a0a  abase dialect...
+00000f50: 2323 2320 4d79 5351 4c0a 6060 600a 7069  ### MySQL.```.pi
+00000f60: 7020 696e 7374 616c 6c20 2263 6c6f 7564  p install "cloud
+00000f70: 2d73 716c 2d70 7974 686f 6e2d 636f 6e6e  -sql-python-conn
+00000f80: 6563 746f 725b 7079 6d79 7371 6c5d 220a  ector[pymysql]".
+00000f90: 6060 600a 2323 2320 506f 7374 6772 6573  ```.### Postgres
+00000fa0: 0a54 6865 7265 2061 7265 2074 776f 2064  .There are two d
+00000fb0: 6966 6665 7265 6e74 2064 6174 6162 6173  ifferent databas
+00000fc0: 6520 6472 6976 6572 7320 7468 6174 2061  e drivers that a
+00000fd0: 7265 2073 7570 706f 7274 6564 2066 6f72  re supported for
+00000fe0: 2074 6865 2050 6f73 7467 7265 7320 6469   the Postgres di
+00000ff0: 616c 6563 743a 0a0a 2323 2323 2070 6738  alect:..#### pg8
+00001000: 3030 300a 6060 600a 7069 7020 696e 7374  000.```.pip inst
+00001010: 616c 6c20 2263 6c6f 7564 2d73 716c 2d70  all "cloud-sql-p
+00001020: 7974 686f 6e2d 636f 6e6e 6563 746f 725b  ython-connector[
+00001030: 7067 3830 3030 5d22 0a60 6060 0a23 2323  pg8000]".```.###
+00001040: 2320 6173 796e 6370 670a 6060 600a 7069  # asyncpg.```.pi
+00001050: 7020 696e 7374 616c 6c20 2263 6c6f 7564  p install "cloud
+00001060: 2d73 716c 2d70 7974 686f 6e2d 636f 6e6e  -sql-python-conn
+00001070: 6563 746f 725b 6173 796e 6370 675d 220a  ector[asyncpg]".
+00001080: 6060 600a 2323 2320 5351 4c20 5365 7276  ```.### SQL Serv
+00001090: 6572 0a60 6060 0a70 6970 2069 6e73 7461  er.```.pip insta
+000010a0: 6c6c 2022 636c 6f75 642d 7371 6c2d 7079  ll "cloud-sql-py
+000010b0: 7468 6f6e 2d63 6f6e 6e65 6374 6f72 5b70  thon-connector[p
+000010c0: 7974 6473 5d22 0a60 6060 0a23 2320 5573  ytds]".```.## Us
+000010d0: 6167 650a 0a54 6869 7320 7061 636b 6167  age..This packag
+000010e0: 6520 7072 6f76 6964 6573 2073 6576 6572  e provides sever
+000010f0: 616c 2066 756e 6374 696f 6e73 2066 6f72  al functions for
+00001100: 2061 7574 686f 7269 7a69 6e67 2061 6e64   authorizing and
+00001110: 2065 6e63 7279 7074 696e 670a 636f 6e6e   encrypting.conn
+00001120: 6563 7469 6f6e 732e 2054 6865 7365 2066  ections. These f
+00001130: 756e 6374 696f 6e73 2061 7265 2075 7365  unctions are use
+00001140: 6420 7769 7468 2079 6f75 7220 6461 7461  d with your data
+00001150: 6261 7365 2064 7269 7665 7220 746f 2063  base driver to c
+00001160: 6f6e 6e65 6374 2074 6f0a 796f 7572 2043  onnect to.your C
+00001170: 6c6f 7564 2053 514c 2069 6e73 7461 6e63  loud SQL instanc
+00001180: 652e 0a0a 5468 6520 696e 7374 616e 6365  e...The instance
+00001190: 2063 6f6e 6e65 6374 696f 6e20 6e61 6d65   connection name
+000011a0: 2066 6f72 2079 6f75 7220 436c 6f75 6420   for your Cloud 
+000011b0: 5351 4c20 696e 7374 616e 6365 2069 7320  SQL instance is 
+000011c0: 616c 7761 7973 2069 6e20 7468 650a 666f  always in the.fo
+000011d0: 726d 6174 2022 7072 6f6a 6563 743a 7265  rmat "project:re
+000011e0: 6769 6f6e 3a69 6e73 7461 6e63 6522 2e0a  gion:instance"..
+000011f0: 0a23 2323 2041 5049 7320 616e 6420 5365  .### APIs and Se
+00001200: 7276 6963 6573 0a0a 5468 6973 2070 6163  rvices..This pac
+00001210: 6b61 6765 2072 6571 7569 7265 7320 7468  kage requires th
+00001220: 6520 666f 6c6c 6f77 696e 6720 746f 2073  e following to s
+00001230: 7563 6365 7373 6675 6c6c 7920 6d61 6b65  uccessfully make
+00001240: 2043 6c6f 7564 2053 514c 2043 6f6e 6e65   Cloud SQL Conne
+00001250: 6374 696f 6e73 3a0a 0a2d 2049 414d 2070  ctions:..- IAM p
+00001260: 7269 6e63 6970 616c 2028 7573 6572 2c20  rincipal (user, 
+00001270: 7365 7276 6963 6520 6163 636f 756e 742c  service account,
+00001280: 2065 7463 2e29 2077 6974 6820 7468 650a   etc.) with the.
+00001290: 5b43 6c6f 7564 2053 514c 2043 6c69 656e  [Cloud SQL Clien
+000012a0: 745d 5b63 6c69 656e 742d 726f 6c65 5d20  t][client-role] 
+000012b0: 726f 6c65 2e20 5468 6973 2049 414d 2070  role. This IAM p
+000012c0: 7269 6e63 6970 616c 2077 696c 6c20 6265  rincipal will be
+000012d0: 2075 7365 6420 666f 720a 5b63 7265 6465   used for.[crede
+000012e0: 6e74 6961 6c73 5d28 2363 7265 6465 6e74  ntials](#credent
+000012f0: 6961 6c73 292e 0a2d 2054 6865 205b 436c  ials)..- The [Cl
+00001300: 6f75 6420 5351 4c20 4164 6d69 6e20 4150  oud SQL Admin AP
+00001310: 495d 5b61 646d 696e 2d61 7069 5d20 746f  I][admin-api] to
+00001320: 2062 6520 656e 6162 6c65 6420 7769 7468   be enabled with
+00001330: 696e 2079 6f75 7220 476f 6f67 6c65 2043  in your Google C
+00001340: 6c6f 7564 0a50 726f 6a65 6374 2e20 4279  loud.Project. By
+00001350: 2064 6566 6175 6c74 2c20 7468 6520 4150   default, the AP
+00001360: 4920 7769 6c6c 2062 6520 6361 6c6c 6564  I will be called
+00001370: 2069 6e20 7468 6520 7072 6f6a 6563 7420   in the project 
+00001380: 6173 736f 6369 6174 6564 2077 6974 680a  associated with.
+00001390: 7468 6520 4941 4d20 7072 696e 6369 7061  the IAM principa
+000013a0: 6c2e 0a0a 5b61 646d 696e 2d61 7069 5d3a  l...[admin-api]:
+000013b0: 2068 7474 7073 3a2f 2f63 6f6e 736f 6c65   https://console
+000013c0: 2e63 6c6f 7564 2e67 6f6f 676c 652e 636f  .cloud.google.co
+000013d0: 6d2f 6170 6973 2f61 7069 2f73 716c 6164  m/apis/api/sqlad
+000013e0: 6d69 6e2e 676f 6f67 6c65 6170 6973 2e63  min.googleapis.c
+000013f0: 6f6d 0a5b 636c 6965 6e74 2d72 6f6c 655d  om.[client-role]
+00001400: 3a20 6874 7470 733a 2f2f 636c 6f75 642e  : https://cloud.
+00001410: 676f 6f67 6c65 2e63 6f6d 2f73 716c 2f64  google.com/sql/d
+00001420: 6f63 732f 6d79 7371 6c2f 726f 6c65 732d  ocs/mysql/roles-
+00001430: 616e 642d 7065 726d 6973 7369 6f6e 730a  and-permissions.
+00001440: 0a23 2323 2043 7265 6465 6e74 6961 6c73  .### Credentials
+00001450: 0a0a 5468 6973 206c 6962 7261 7279 2075  ..This library u
+00001460: 7365 7320 7468 6520 5b41 7070 6c69 6361  ses the [Applica
+00001470: 7469 6f6e 2044 6566 6175 6c74 2043 7265  tion Default Cre
+00001480: 6465 6e74 6961 6c73 2028 4144 4329 5d5b  dentials (ADC)][
+00001490: 6164 635d 2073 7472 6174 6567 7920 666f  adc] strategy fo
+000014a0: 720a 7265 736f 6c76 696e 6720 6372 6564  r.resolving cred
+000014b0: 656e 7469 616c 732e 2050 6c65 6173 6520  entials. Please 
+000014c0: 7365 6520 5b74 6865 7365 2069 6e73 7472  see [these instr
+000014d0: 7563 7469 6f6e 7320 666f 7220 686f 7720  uctions for how 
+000014e0: 746f 2073 6574 2079 6f75 7220 4144 435d  to set your ADC]
+000014f0: 5b73 6574 2d61 6463 5d0a 2847 6f6f 676c  [set-adc].(Googl
+00001500: 6520 436c 6f75 6420 4170 706c 6963 6174  e Cloud Applicat
+00001510: 696f 6e20 7673 204c 6f63 616c 2044 6576  ion vs Local Dev
+00001520: 656c 6f70 6d65 6e74 2c20 4941 4d20 7573  elopment, IAM us
+00001530: 6572 2076 7320 7365 7276 6963 6520 6163  er vs service ac
+00001540: 636f 756e 7420 6372 6564 656e 7469 616c  count credential
+00001550: 7329 2c0a 6f72 2063 6f6e 7375 6c74 2074  s),.or consult t
+00001560: 6865 205b 676f 6f67 6c65 2e61 7574 685d  he [google.auth]
+00001570: 5b67 6f6f 676c 652d 6175 7468 5d20 7061  [google-auth] pa
+00001580: 636b 6167 652e 0a0a 546f 2065 7870 6c69  ckage...To expli
+00001590: 6369 746c 7920 7365 7420 6120 7370 6563  citly set a spec
+000015a0: 6966 6963 2073 6f75 7263 6520 666f 7220  ific source for 
+000015b0: 7468 6520 6372 6564 656e 7469 616c 732c  the credentials,
+000015c0: 2073 6565 0a5b 436f 6e66 6967 7572 696e   see.[Configurin
+000015d0: 6720 7468 6520 436f 6e6e 6563 746f 725d  g the Connector]
+000015e0: 2823 636f 6e66 6967 7572 696e 672d 7468  (#configuring-th
+000015f0: 652d 636f 6e6e 6563 746f 7229 2062 656c  e-connector) bel
+00001600: 6f77 2e0a 0a5b 6164 635d 3a20 6874 7470  ow...[adc]: http
+00001610: 733a 2f2f 636c 6f75 642e 676f 6f67 6c65  s://cloud.google
+00001620: 2e63 6f6d 2f64 6f63 732f 6175 7468 656e  .com/docs/authen
+00001630: 7469 6361 7469 6f6e 2361 6463 0a5b 7365  tication#adc.[se
+00001640: 742d 6164 635d 3a20 6874 7470 733a 2f2f  t-adc]: https://
+00001650: 636c 6f75 642e 676f 6f67 6c65 2e63 6f6d  cloud.google.com
+00001660: 2f64 6f63 732f 6175 7468 656e 7469 6361  /docs/authentica
+00001670: 7469 6f6e 2f70 726f 7669 6465 2d63 7265  tion/provide-cre
+00001680: 6465 6e74 6961 6c73 2d61 6463 0a5b 676f  dentials-adc.[go
+00001690: 6f67 6c65 2d61 7574 685d 3a20 6874 7470  ogle-auth]: http
+000016a0: 733a 2f2f 676f 6f67 6c65 2d61 7574 682e  s://google-auth.
+000016b0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+000016c0: 6e2f 6d61 7374 6572 2f72 6566 6572 656e  n/master/referen
+000016d0: 6365 2f67 6f6f 676c 652e 6175 7468 2e68  ce/google.auth.h
+000016e0: 746d 6c0a 0a23 2323 2048 6f77 2074 6f20  tml..### How to 
+000016f0: 7573 6520 7468 6973 2043 6f6e 6e65 6374  use this Connect
+00001700: 6f72 0a0a 546f 2063 6f6e 6e65 6374 2074  or..To connect t
+00001710: 6f20 436c 6f75 6420 5351 4c20 7573 696e  o Cloud SQL usin
+00001720: 6720 7468 6520 636f 6e6e 6563 746f 722c  g the connector,
+00001730: 2069 6e69 7469 7461 6c69 7a65 2061 2060   inititalize a `
+00001740: 436f 6e6e 6563 746f 7260 0a6f 626a 6563  Connector`.objec
+00001750: 7420 616e 6420 6361 6c6c 2069 7427 7320  t and call it's 
+00001760: 6063 6f6e 6e65 6374 6020 6d65 7468 6f64  `connect` method
+00001770: 2077 6974 6820 7468 6520 7072 6f70 6572   with the proper
+00001780: 2069 6e70 7574 2070 6172 616d 6574 6572   input parameter
+00001790: 732e 0a0a 5468 6520 6043 6f6e 6e65 6374  s...The `Connect
+000017a0: 6f72 6020 6974 7365 6c66 2063 7265 6174  or` itself creat
+000017b0: 6573 2063 6f6e 6e65 6374 696f 6e20 6f62  es connection ob
+000017c0: 6a65 6374 7320 6279 2063 616c 6c69 6e67  jects by calling
+000017d0: 2069 7473 2060 636f 6e6e 6563 7460 206d   its `connect` m
+000017e0: 6574 686f 6420 6275 7420 646f 6573 206e  ethod but does n
+000017f0: 6f74 206d 616e 6167 6520 6461 7461 6261  ot manage databa
+00001800: 7365 2063 6f6e 6e65 6374 696f 6e20 706f  se connection po
+00001810: 6f6c 696e 672e 2046 6f72 2074 6869 7320  oling. For this 
+00001820: 7265 6173 6f6e 2c20 6974 2069 7320 7265  reason, it is re
+00001830: 636f 6d6d 656e 6465 6420 746f 2075 7365  commended to use
+00001840: 2074 6865 2063 6f6e 6e65 6374 6f72 2061   the connector a
+00001850: 6c6f 6e67 7369 6465 2061 206c 6962 7261  longside a libra
+00001860: 7279 2074 6861 7420 6361 6e20 6372 6561  ry that can crea
+00001870: 7465 2063 6f6e 6e65 6374 696f 6e20 706f  te connection po
+00001880: 6f6c 732c 2073 7563 6820 6173 205b 5351  ols, such as [SQ
+00001890: 4c41 6c63 6865 6d79 5d28 6874 7470 733a  LAlchemy](https:
+000018a0: 2f2f 7777 772e 7371 6c61 6c63 6865 6d79  //www.sqlalchemy
+000018b0: 2e6f 7267 2f29 2e20 5468 6973 2077 696c  .org/). This wil
+000018c0: 6c20 616c 6c6f 7720 666f 7220 636f 6e6e  l allow for conn
+000018d0: 6563 7469 6f6e 7320 746f 2072 656d 6169  ections to remai
+000018e0: 6e20 6f70 656e 2061 6e64 2062 6520 7265  n open and be re
+000018f0: 7573 6564 2c20 7265 6475 6369 6e67 2063  used, reducing c
+00001900: 6f6e 6e65 6374 696f 6e20 6f76 6572 6865  onnection overhe
+00001910: 6164 2061 6e64 2074 6865 206e 756d 6265  ad and the numbe
+00001920: 7220 6f66 2063 6f6e 6e65 6374 696f 6e73  r of connections
+00001930: 206e 6565 6465 642e 0a0a 496e 2074 6865   needed...In the
+00001940: 2043 6f6e 6e65 6374 6f72 2773 2060 636f   Connector's `co
+00001950: 6e6e 6563 7460 206d 6574 686f 6420 6265  nnect` method be
+00001960: 6c6f 772c 2069 6e70 7574 2079 6f75 7220  low, input your 
+00001970: 636f 6e6e 6563 7469 6f6e 2073 7472 696e  connection strin
+00001980: 6720 6173 2074 6865 2066 6972 7374 2070  g as the first p
+00001990: 6f73 6974 696f 6e61 6c20 6172 6775 6d65  ositional argume
+000019a0: 6e74 2061 6e64 2074 6865 206e 616d 6520  nt and the name 
+000019b0: 6f66 2074 6865 2064 6174 6162 6173 6520  of the database 
+000019c0: 6472 6976 6572 2066 6f72 2074 6865 2073  driver for the s
+000019d0: 6563 6f6e 6420 706f 7369 7469 6f6e 616c  econd positional
+000019e0: 2061 7267 756d 656e 742e 2049 6e73 6572   argument. Inser
+000019f0: 7420 7468 6520 7265 7374 206f 6620 796f  t the rest of yo
+00001a00: 7572 2063 6f6e 6e65 6374 696f 6e20 6b65  ur connection ke
+00001a10: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
+00001a20: 6c69 6b65 2075 7365 722c 2070 6173 7377  like user, passw
+00001a30: 6f72 6420 616e 6420 6461 7461 6261 7365  ord and database
+00001a40: 2e20 596f 7520 6361 6e20 616c 736f 2073  . You can also s
+00001a50: 6574 2074 6865 206f 7074 696f 6e61 6c20  et the optional 
+00001a60: 6074 696d 656f 7574 6020 6f72 2060 6970  `timeout` or `ip
+00001a70: 5f74 7970 6560 206b 6579 776f 7264 2061  _type` keyword a
+00001a80: 7267 756d 656e 7473 2e0a 0a54 6f20 7573  rguments...To us
+00001a90: 6520 7468 6973 2063 6f6e 6e65 6374 6f72  e this connector
+00001aa0: 2077 6974 6820 5351 4c41 6c63 6865 6d79   with SQLAlchemy
+00001ab0: 2c20 7573 6520 7468 6520 6063 7265 6174  , use the `creat
+00001ac0: 6f72 6020 6172 6775 6d65 6e74 2066 6f72  or` argument for
+00001ad0: 2060 7371 6c61 6c63 6865 6d79 2e63 7265   `sqlalchemy.cre
+00001ae0: 6174 655f 656e 6769 6e65 603a 0a0a 6060  ate_engine`:..``
+00001af0: 6070 7974 686f 6e0a 6672 6f6d 2067 6f6f  `python.from goo
+00001b00: 676c 652e 636c 6f75 642e 7371 6c2e 636f  gle.cloud.sql.co
+00001b10: 6e6e 6563 746f 7220 696d 706f 7274 2043  nnector import C
+00001b20: 6f6e 6e65 6374 6f72 0a69 6d70 6f72 7420  onnector.import 
+00001b30: 7371 6c61 6c63 6865 6d79 0a0a 2320 696e  sqlalchemy..# in
+00001b40: 6974 6961 6c69 7a65 2043 6f6e 6e65 6374  itialize Connect
+00001b50: 6f72 206f 626a 6563 740a 636f 6e6e 6563  or object.connec
+00001b60: 746f 7220 3d20 436f 6e6e 6563 746f 7228  tor = Connector(
+00001b70: 290a 0a23 2066 756e 6374 696f 6e20 746f  )..# function to
+00001b80: 2072 6574 7572 6e20 7468 6520 6461 7461   return the data
+00001b90: 6261 7365 2063 6f6e 6e65 6374 696f 6e0a  base connection.
+00001ba0: 6465 6620 6765 7463 6f6e 6e28 2920 2d3e  def getconn() ->
+00001bb0: 2070 796d 7973 716c 2e63 6f6e 6e65 6374   pymysql.connect
+00001bc0: 696f 6e73 2e43 6f6e 6e65 6374 696f 6e3a  ions.Connection:
+00001bd0: 0a20 2020 2063 6f6e 6e3a 2070 796d 7973  .    conn: pymys
+00001be0: 716c 2e63 6f6e 6e65 6374 696f 6e73 2e43  ql.connections.C
+00001bf0: 6f6e 6e65 6374 696f 6e20 3d20 636f 6e6e  onnection = conn
+00001c00: 6563 746f 722e 636f 6e6e 6563 7428 0a20  ector.connect(. 
+00001c10: 2020 2020 2020 2022 7072 6f6a 6563 743a         "project:
+00001c20: 7265 6769 6f6e 3a69 6e73 7461 6e63 6522  region:instance"
+00001c30: 2c0a 2020 2020 2020 2020 2270 796d 7973  ,.        "pymys
+00001c40: 716c 222c 0a20 2020 2020 2020 2075 7365  ql",.        use
+00001c50: 723d 226d 792d 7573 6572 222c 0a20 2020  r="my-user",.   
+00001c60: 2020 2020 2070 6173 7377 6f72 643d 226d       password="m
+00001c70: 792d 7061 7373 776f 7264 222c 0a20 2020  y-password",.   
+00001c80: 2020 2020 2064 623d 226d 792d 6462 2d6e       db="my-db-n
+00001c90: 616d 6522 0a20 2020 2029 0a20 2020 2072  ame".    ).    r
+00001ca0: 6574 7572 6e20 636f 6e6e 0a0a 2320 6372  eturn conn..# cr
+00001cb0: 6561 7465 2063 6f6e 6e65 6374 696f 6e20  eate connection 
+00001cc0: 706f 6f6c 0a70 6f6f 6c20 3d20 7371 6c61  pool.pool = sqla
+00001cd0: 6c63 6865 6d79 2e63 7265 6174 655f 656e  lchemy.create_en
+00001ce0: 6769 6e65 280a 2020 2020 226d 7973 716c  gine(.    "mysql
+00001cf0: 2b70 796d 7973 716c 3a2f 2f22 2c0a 2020  +pymysql://",.  
+00001d00: 2020 6372 6561 746f 723d 6765 7463 6f6e    creator=getcon
+00001d10: 6e2c 0a29 0a60 6060 0a0a 5468 6520 7265  n,.).```..The re
+00001d20: 7475 726e 6564 2063 6f6e 6e65 6374 696f  turned connectio
+00001d30: 6e20 706f 6f6c 2065 6e67 696e 6520 6361  n pool engine ca
+00001d40: 6e20 7468 656e 2062 6520 7573 6564 2074  n then be used t
+00001d50: 6f20 7175 6572 7920 616e 6420 6d6f 6469  o query and modi
+00001d60: 6679 2074 6865 2064 6174 6162 6173 652e  fy the database.
+00001d70: 0a0a 6060 6070 7974 686f 6e0a 2320 696e  ..```python.# in
+00001d80: 7365 7274 2073 7461 7465 6d65 6e74 0a69  sert statement.i
+00001d90: 6e73 6572 745f 7374 6d74 203d 2073 716c  nsert_stmt = sql
+00001da0: 616c 6368 656d 792e 7465 7874 280a 2020  alchemy.text(.  
+00001db0: 2020 2249 4e53 4552 5420 494e 544f 206d    "INSERT INTO m
+00001dc0: 795f 7461 626c 6520 2869 642c 2074 6974  y_table (id, tit
+00001dd0: 6c65 2920 5641 4c55 4553 2028 3a69 642c  le) VALUES (:id,
+00001de0: 203a 7469 746c 6529 222c 0a29 0a0a 7769   :title)",.)..wi
+00001df0: 7468 2070 6f6f 6c2e 636f 6e6e 6563 7428  th pool.connect(
+00001e00: 2920 6173 2064 625f 636f 6e6e 3a0a 2020  ) as db_conn:.  
+00001e10: 2020 2320 696e 7365 7274 2069 6e74 6f20    # insert into 
+00001e20: 6461 7461 6261 7365 0a20 2020 2064 625f  database.    db_
+00001e30: 636f 6e6e 2e65 7865 6375 7465 2869 6e73  conn.execute(ins
+00001e40: 6572 745f 7374 6d74 2c20 7061 7261 6d65  ert_stmt, parame
+00001e50: 7465 7273 3d7b 2269 6422 3a20 2262 6f6f  ters={"id": "boo
+00001e60: 6b31 222c 2022 7469 746c 6522 3a20 2242  k1", "title": "B
+00001e70: 6f6f 6b20 4f6e 6522 7d29 0a0a 2020 2020  ook One"})..    
+00001e80: 2320 7175 6572 7920 6461 7461 6261 7365  # query database
+00001e90: 0a20 2020 2072 6573 756c 7420 3d20 6462  .    result = db
+00001ea0: 5f63 6f6e 6e2e 6578 6563 7574 6528 7371  _conn.execute(sq
+00001eb0: 6c61 6c63 6865 6d79 2e74 6578 7428 2253  lalchemy.text("S
+00001ec0: 454c 4543 5420 2a20 6672 6f6d 206d 795f  ELECT * from my_
+00001ed0: 7461 626c 6522 2929 2e66 6574 6368 616c  table")).fetchal
+00001ee0: 6c28 290a 0a20 2020 2023 2063 6f6d 6d69  l()..    # commi
+00001ef0: 7420 7472 616e 7361 6374 696f 6e20 2853  t transaction (S
+00001f00: 514c 416c 6368 656d 7920 7632 2e58 2e58  QLAlchemy v2.X.X
+00001f10: 2069 7320 636f 6d6d 6974 2061 7320 796f   is commit as yo
+00001f20: 7520 676f 290a 2020 2020 6462 5f63 6f6e  u go).    db_con
+00001f30: 6e2e 636f 6d6d 6974 2829 0a0a 2020 2020  n.commit()..    
+00001f40: 2320 446f 2073 6f6d 6574 6869 6e67 2077  # Do something w
+00001f50: 6974 6820 7468 6520 7265 7375 6c74 730a  ith the results.
+00001f60: 2020 2020 666f 7220 726f 7720 696e 2072      for row in r
+00001f70: 6573 756c 743a 0a20 2020 2020 2020 2070  esult:.        p
+00001f80: 7269 6e74 2872 6f77 290a 6060 600a 0a54  rint(row).```..T
+00001f90: 6f20 636c 6f73 6520 7468 6520 6043 6f6e  o close the `Con
+00001fa0: 6e65 6374 6f72 6020 6f62 6a65 6374 2773  nector` object's
+00001fb0: 2062 6163 6b67 726f 756e 6420 7265 736f   background reso
+00001fc0: 7572 6365 732c 2063 616c 6c20 6974 2773  urces, call it's
+00001fd0: 2060 636c 6f73 6528 2960 206d 6574 686f   `close()` metho
+00001fe0: 6420 6173 2066 6f6c 6c6f 7773 3a0a 0a60  d as follows:..`
+00001ff0: 6060 7079 7468 6f6e 0a63 6f6e 6e65 6374  ``python.connect
+00002000: 6f72 2e63 6c6f 7365 2829 0a60 6060 0a0a  or.close().```..
+00002010: 2a2a 4e6f 7465 2a2a 3a20 466f 7220 6d6f  **Note**: For mo
+00002020: 7265 2065 7861 6d70 6c65 7320 6f66 2075  re examples of u
+00002030: 7369 6e67 2053 514c 416c 6368 656d 7920  sing SQLAlchemy 
+00002040: 746f 206d 616e 6167 6520 636f 6e6e 6563  to manage connec
+00002050: 7469 6f6e 2070 6f6f 6c69 6e67 2077 6974  tion pooling wit
+00002060: 6820 7468 6520 636f 6e6e 6563 746f 722c  h the connector,
+00002070: 2070 6c65 6173 6520 7365 6520 5b43 6c6f   please see [Clo
+00002080: 7564 2053 514c 2053 514c 416c 6368 656d  ud SQL SQLAlchem
+00002090: 7920 5361 6d70 6c65 735d 2868 7474 7073  y Samples](https
+000020a0: 3a2f 2f63 6c6f 7564 2e67 6f6f 676c 652e  ://cloud.google.
+000020b0: 636f 6d2f 7371 6c2f 646f 6373 2f70 6f73  com/sql/docs/pos
+000020c0: 7467 7265 732f 636f 6e6e 6563 742d 636f  tgres/connect-co
+000020d0: 6e6e 6563 746f 7273 2370 7974 686f 6e5f  nnectors#python_
+000020e0: 3129 2e0a 0a2a 2a4e 6f74 6520 666f 7220  1)...**Note for 
+000020f0: 5351 4c20 5365 7276 6572 2075 7365 7273  SQL Server users
+00002100: 2a2a 3a20 4966 2079 6f75 7220 5351 4c20  **: If your SQL 
+00002110: 5365 7276 6572 2069 6e73 7461 6e63 6520  Server instance 
+00002120: 7265 7175 6972 6573 2053 534c 2c20 796f  requires SSL, yo
+00002130: 7520 6e65 6564 2074 6f20 646f 776e 6c6f  u need to downlo
+00002140: 6164 2074 6865 2043 4120 6365 7274 6966  ad the CA certif
+00002150: 6963 6174 6520 666f 7220 796f 7572 2069  icate for your i
+00002160: 6e73 7461 6e63 6520 616e 6420 696e 636c  nstance and incl
+00002170: 7564 6520 6063 6166 696c 653d 7b70 6174  ude `cafile={pat
+00002180: 6820 746f 2064 6f77 6e6c 6f61 6465 6420  h to downloaded 
+00002190: 6365 7274 6966 6963 6174 657d 6020 616e  certificate}` an
+000021a0: 6420 6076 616c 6964 6174 655f 686f 7374  d `validate_host
+000021b0: 3d46 616c 7365 602e 2054 6869 7320 6973  =False`. This is
+000021c0: 2061 2077 6f72 6b61 726f 756e 6420 666f   a workaround fo
+000021d0: 7220 6120 5b6b 6e6f 776e 2069 7373 7565  r a [known issue
+000021e0: 5d28 6874 7470 733a 2f2f 6973 7375 6574  ](https://issuet
+000021f0: 7261 636b 6572 2e67 6f6f 676c 652e 636f  racker.google.co
+00002200: 6d2f 3138 3438 3637 3134 3729 2e0a 0a23  m/184867147)...#
+00002210: 2323 2043 6f6e 6669 6775 7269 6e67 2074  ## Configuring t
+00002220: 6865 2043 6f6e 6e65 6374 6f72 0a0a 4966  he Connector..If
+00002230: 2079 6f75 206e 6565 6420 746f 2063 7573   you need to cus
+00002240: 746f 6d69 7a65 2073 6f6d 6574 6869 6e67  tomize something
+00002250: 2061 626f 7574 2074 6865 2063 6f6e 6e65   about the conne
+00002260: 6374 6f72 2c20 6f72 2077 616e 7420 746f  ctor, or want to
+00002270: 2073 7065 6369 6679 0a64 6566 6175 6c74   specify.default
+00002280: 7320 666f 7220 6561 6368 2063 6f6e 6e65  s for each conne
+00002290: 6374 696f 6e20 746f 206d 616b 652c 2079  ction to make, y
+000022a0: 6f75 2063 616e 2069 6e69 7469 616c 697a  ou can initializ
+000022b0: 6520 610a 6043 6f6e 6e65 6374 6f72 6020  e a.`Connector` 
+000022c0: 6f62 6a65 6374 2061 7320 666f 6c6c 6f77  object as follow
+000022d0: 733a 0a0a 6060 6070 7974 686f 6e0a 6672  s:..```python.fr
+000022e0: 6f6d 2067 6f6f 676c 652e 636c 6f75 642e  om google.cloud.
+000022f0: 7371 6c2e 636f 6e6e 6563 746f 7220 696d  sql.connector im
+00002300: 706f 7274 2043 6f6e 6e65 6374 6f72 2c20  port Connector, 
+00002310: 4950 5479 7065 730a 0a23 204e 6f74 653a  IPTypes..# Note:
+00002320: 2061 6c6c 2070 6172 616d 6574 6572 7320   all parameters 
+00002330: 6265 6c6f 7720 6172 6520 6f70 7469 6f6e  below are option
+00002340: 616c 0a63 6f6e 6e65 6374 6f72 203d 2043  al.connector = C
+00002350: 6f6e 6e65 6374 6f72 280a 2020 2020 6970  onnector(.    ip
+00002360: 5f74 7970 653d 4950 5479 7065 732e 5055  _type=IPTypes.PU
+00002370: 424c 4943 2c0a 2020 2020 656e 6162 6c65  BLIC,.    enable
+00002380: 5f69 616d 5f61 7574 683d 4661 6c73 652c  _iam_auth=False,
+00002390: 0a20 2020 2074 696d 656f 7574 3d33 302c  .    timeout=30,
+000023a0: 0a20 2020 2063 7265 6465 6e74 6961 6c73  .    credentials
+000023b0: 3d63 7573 746f 6d5f 6372 6564 7320 2320  =custom_creds # 
+000023c0: 676f 6f67 6c65 2e61 7574 682e 6372 6564  google.auth.cred
+000023d0: 656e 7469 616c 732e 4372 6564 656e 7469  entials.Credenti
+000023e0: 616c 730a 290a 6060 600a 0a23 2323 2055  als.).```..### U
+000023f0: 7369 6e67 2043 6f6e 6e65 6374 6f72 2061  sing Connector a
+00002400: 7320 6120 436f 6e74 6578 7420 4d61 6e61  s a Context Mana
+00002410: 6765 720a 0a54 6865 2060 436f 6e6e 6563  ger..The `Connec
+00002420: 746f 7260 206f 626a 6563 7420 6361 6e20  tor` object can 
+00002430: 616c 736f 2062 6520 7573 6564 2061 7320  also be used as 
+00002440: 6120 636f 6e74 6578 7420 6d61 6e61 6765  a context manage
+00002450: 7220 696e 206f 7264 6572 2074 6f0a 6175  r in order to.au
+00002460: 746f 6d61 7469 6361 6c6c 7920 636c 6f73  tomatically clos
+00002470: 6520 616e 6420 636c 6561 6e75 7020 7265  e and cleanup re
+00002480: 736f 7572 6365 732c 2072 656d 6f76 696e  sources, removin
+00002490: 6720 7468 6520 6e65 6564 2066 6f72 2065  g the need for e
+000024a0: 7870 6c69 6369 740a 6361 6c6c 7320 746f  xplicit.calls to
+000024b0: 2060 636f 6e6e 6563 746f 722e 636c 6f73   `connector.clos
+000024c0: 6528 2960 2e0a 0a43 6f6e 6e65 6374 6f72  e()`...Connector
+000024d0: 2061 7320 6120 636f 6e74 6578 7420 6d61   as a context ma
+000024e0: 6e61 6765 723a 0a0a 6060 6070 7974 686f  nager:..```pytho
+000024f0: 6e0a 6672 6f6d 2067 6f6f 676c 652e 636c  n.from google.cl
+00002500: 6f75 642e 7371 6c2e 636f 6e6e 6563 746f  oud.sql.connecto
+00002510: 7220 696d 706f 7274 2043 6f6e 6e65 6374  r import Connect
+00002520: 6f72 0a69 6d70 6f72 7420 7079 6d79 7371  or.import pymysq
+00002530: 6c0a 696d 706f 7274 2073 716c 616c 6368  l.import sqlalch
+00002540: 656d 790a 0a23 2068 656c 7065 7220 6675  emy..# helper fu
+00002550: 6e63 7469 6f6e 2074 6f20 7265 7475 726e  nction to return
+00002560: 2053 514c 416c 6368 656d 7920 636f 6e6e   SQLAlchemy conn
+00002570: 6563 7469 6f6e 2070 6f6f 6c0a 6465 6620  ection pool.def 
+00002580: 696e 6974 5f63 6f6e 6e65 6374 696f 6e5f  init_connection_
+00002590: 706f 6f6c 2863 6f6e 6e65 6374 6f72 3a20  pool(connector: 
+000025a0: 436f 6e6e 6563 746f 7229 202d 3e20 7371  Connector) -> sq
+000025b0: 6c61 6c63 6865 6d79 2e65 6e67 696e 652e  lalchemy.engine.
+000025c0: 456e 6769 6e65 3a0a 2020 2020 2320 6675  Engine:.    # fu
+000025d0: 6e63 7469 6f6e 2075 7365 6420 746f 2067  nction used to g
+000025e0: 656e 6572 6174 6520 6461 7461 6261 7365  enerate database
+000025f0: 2063 6f6e 6e65 6374 696f 6e0a 2020 2020   connection.    
+00002600: 6465 6620 6765 7463 6f6e 6e28 2920 2d3e  def getconn() ->
+00002610: 2070 796d 7973 716c 2e63 6f6e 6e65 6374   pymysql.connect
+00002620: 696f 6e73 2e43 6f6e 6e65 6374 696f 6e3a  ions.Connection:
+00002630: 0a20 2020 2020 2020 2063 6f6e 6e20 3d20  .        conn = 
+00002640: 636f 6e6e 6563 746f 722e 636f 6e6e 6563  connector.connec
+00002650: 7428 0a20 2020 2020 2020 2020 2020 2022  t(.            "
+00002660: 7072 6f6a 6563 743a 7265 6769 6f6e 3a69  project:region:i
+00002670: 6e73 7461 6e63 6522 2c0a 2020 2020 2020  nstance",.      
+00002680: 2020 2020 2020 2270 796d 7973 716c 222c        "pymysql",
+00002690: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+000026a0: 723d 226d 792d 7573 6572 222c 0a20 2020  r="my-user",.   
+000026b0: 2020 2020 2020 2020 2070 6173 7377 6f72           passwor
+000026c0: 643d 226d 792d 7061 7373 776f 7264 222c  d="my-password",
+000026d0: 0a20 2020 2020 2020 2020 2020 2064 623d  .            db=
+000026e0: 226d 792d 6462 2d6e 616d 6522 0a20 2020  "my-db-name".   
+000026f0: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
+00002700: 6574 7572 6e20 636f 6e6e 0a0a 2020 2020  eturn conn..    
+00002710: 2320 6372 6561 7465 2063 6f6e 6e65 6374  # create connect
+00002720: 696f 6e20 706f 6f6c 0a20 2020 2070 6f6f  ion pool.    poo
+00002730: 6c20 3d20 7371 6c61 6c63 6865 6d79 2e63  l = sqlalchemy.c
+00002740: 7265 6174 655f 656e 6769 6e65 280a 2020  reate_engine(.  
+00002750: 2020 2020 2020 226d 7973 716c 2b70 796d        "mysql+pym
+00002760: 7973 716c 3a2f 2f22 2c0a 2020 2020 2020  ysql://",.      
+00002770: 2020 6372 6561 746f 723d 6765 7463 6f6e    creator=getcon
+00002780: 6e2c 0a20 2020 2029 0a20 2020 2072 6574  n,.    ).    ret
+00002790: 7572 6e20 706f 6f6c 0a0a 2320 696e 6974  urn pool..# init
+000027a0: 6961 6c69 7a65 2043 6c6f 7564 2053 514c  ialize Cloud SQL
+000027b0: 2050 7974 686f 6e20 436f 6e6e 6563 746f   Python Connecto
+000027c0: 7220 6173 2063 6f6e 7465 7874 206d 616e  r as context man
+000027d0: 6167 6572 0a77 6974 6820 436f 6e6e 6563  ager.with Connec
+000027e0: 746f 7228 2920 6173 2063 6f6e 6e65 6374  tor() as connect
+000027f0: 6f72 3a0a 2020 2020 2320 696e 6974 6961  or:.    # initia
+00002800: 6c69 7a65 2063 6f6e 6e65 6374 696f 6e20  lize connection 
+00002810: 706f 6f6c 0a20 2020 2070 6f6f 6c20 3d20  pool.    pool = 
+00002820: 696e 6974 5f63 6f6e 6e65 6374 696f 6e5f  init_connection_
+00002830: 706f 6f6c 2863 6f6e 6e65 6374 6f72 290a  pool(connector).
+00002840: 2020 2020 2320 696e 7365 7274 2073 7461      # insert sta
+00002850: 7465 6d65 6e74 0a20 2020 2069 6e73 6572  tement.    inser
+00002860: 745f 7374 6d74 203d 2073 716c 616c 6368  t_stmt = sqlalch
+00002870: 656d 792e 7465 7874 280a 2020 2020 2020  emy.text(.      
+00002880: 2020 2249 4e53 4552 5420 494e 544f 206d    "INSERT INTO m
+00002890: 795f 7461 626c 6520 2869 642c 2074 6974  y_table (id, tit
+000028a0: 6c65 2920 5641 4c55 4553 2028 3a69 642c  le) VALUES (:id,
+000028b0: 203a 7469 746c 6529 222c 0a20 2020 2029   :title)",.    )
+000028c0: 0a0a 2020 2020 2320 696e 7465 7261 6374  ..    # interact
+000028d0: 2077 6974 6820 436c 6f75 6420 5351 4c20   with Cloud SQL 
+000028e0: 6461 7461 6261 7365 2075 7369 6e67 2063  database using c
+000028f0: 6f6e 6e65 6374 696f 6e20 706f 6f6c 0a20  onnection pool. 
+00002900: 2020 2077 6974 6820 706f 6f6c 2e63 6f6e     with pool.con
+00002910: 6e65 6374 2829 2061 7320 6462 5f63 6f6e  nect() as db_con
+00002920: 6e3a 0a20 2020 2020 2020 2023 2069 6e73  n:.        # ins
+00002930: 6572 7420 696e 746f 2064 6174 6162 6173  ert into databas
+00002940: 650a 2020 2020 2020 2020 6462 5f63 6f6e  e.        db_con
+00002950: 6e2e 6578 6563 7574 6528 696e 7365 7274  n.execute(insert
+00002960: 5f73 746d 742c 2070 6172 616d 6574 6572  _stmt, parameter
+00002970: 733d 7b22 6964 223a 2022 626f 6f6b 3122  s={"id": "book1"
+00002980: 2c20 2274 6974 6c65 223a 2022 426f 6f6b  , "title": "Book
+00002990: 204f 6e65 227d 290a 0a20 2020 2020 2020   One"})..       
+000029a0: 2023 2063 6f6d 6d69 7420 7472 616e 7361   # commit transa
+000029b0: 6374 696f 6e20 2853 514c 416c 6368 656d  ction (SQLAlchem
+000029c0: 7920 7632 2e58 2e58 2069 7320 636f 6d6d  y v2.X.X is comm
+000029d0: 6974 2061 7320 796f 7520 676f 290a 2020  it as you go).  
+000029e0: 2020 2020 2020 6462 5f63 6f6e 6e2e 636f        db_conn.co
+000029f0: 6d6d 6974 2829 0a0a 2020 2020 2020 2020  mmit()..        
+00002a00: 2320 7175 6572 7920 6461 7461 6261 7365  # query database
+00002a10: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00002a20: 3d20 6462 5f63 6f6e 6e2e 6578 6563 7574  = db_conn.execut
+00002a30: 6528 7371 6c61 6c63 6865 6d79 2e74 6578  e(sqlalchemy.tex
+00002a40: 7428 2253 454c 4543 5420 2a20 6672 6f6d  t("SELECT * from
+00002a50: 206d 795f 7461 626c 6522 2929 2e66 6574   my_table")).fet
+00002a60: 6368 616c 6c28 290a 0a20 2020 2020 2020  chall()..       
+00002a70: 2023 2044 6f20 736f 6d65 7468 696e 6720   # Do something 
+00002a80: 7769 7468 2074 6865 2072 6573 756c 7473  with the results
+00002a90: 0a20 2020 2020 2020 2066 6f72 2072 6f77  .        for row
+00002aa0: 2069 6e20 7265 7375 6c74 3a0a 2020 2020   in result:.    
+00002ab0: 2020 2020 2020 2020 7072 696e 7428 726f          print(ro
+00002ac0: 7729 0a60 6060 0a0a 2323 2320 5370 6563  w).```..### Spec
+00002ad0: 6966 7969 6e67 2049 5020 4164 6472 6573  ifying IP Addres
+00002ae0: 7320 5479 7065 0a0a 5468 6520 436c 6f75  s Type..The Clou
+00002af0: 6420 5351 4c20 5079 7468 6f6e 2043 6f6e  d SQL Python Con
+00002b00: 6e65 6374 6f72 2063 616e 2062 6520 7573  nector can be us
+00002b10: 6564 2074 6f20 636f 6e6e 6563 7420 746f  ed to connect to
+00002b20: 2043 6c6f 7564 2053 514c 2069 6e73 7461   Cloud SQL insta
+00002b30: 6e63 6573 0a75 7369 6e67 2062 6f74 6820  nces.using both 
+00002b40: 7075 626c 6963 2061 6e64 2070 7269 7661  public and priva
+00002b50: 7465 2049 5020 6164 6472 6573 7365 732c  te IP addresses,
+00002b60: 2061 7320 7765 6c6c 2061 730a 5b50 7269   as well as.[Pri
+00002b70: 7661 7465 2053 6572 7669 6365 2043 6f6e  vate Service Con
+00002b80: 6e65 6374 5d5b 7073 635d 2028 5053 4329  nect][psc] (PSC)
+00002b90: 2e20 546f 2073 7065 6369 6679 2077 6869  . To specify whi
+00002ba0: 6368 2049 5020 6164 6472 6573 7320 7479  ch IP address ty
+00002bb0: 7065 2074 6f20 636f 6e6e 6563 740a 7769  pe to connect.wi
+00002bc0: 7468 2c20 7365 7420 7468 6520 6069 705f  th, set the `ip_
+00002bd0: 7479 7065 6020 6b65 7977 6f72 6420 6172  type` keyword ar
+00002be0: 6775 6d65 6e74 2077 6865 6e20 696e 6974  gument when init
+00002bf0: 6961 6c69 7a69 6e67 2061 2060 436f 6e6e  ializing a `Conn
+00002c00: 6563 746f 7228 2960 206f 7220 7768 656e  ector()` or when
+00002c10: 0a63 616c 6c69 6e67 2060 636f 6e6e 6563  .calling `connec
+00002c20: 746f 722e 636f 6e6e 6563 7428 2960 2e0a  tor.connect()`..
+00002c30: 0a50 6f73 7369 626c 6520 7661 6c75 6573  .Possible values
+00002c40: 2066 6f72 2060 6970 5f74 7970 6560 2061   for `ip_type` a
+00002c50: 7265 2060 4950 5479 7065 732e 5055 424c  re `IPTypes.PUBL
+00002c60: 4943 6020 2864 6566 6175 6c74 2076 616c  IC` (default val
+00002c70: 7565 292c 0a60 4950 5479 7065 732e 5052  ue),.`IPTypes.PR
+00002c80: 4956 4154 4560 2c20 616e 6420 6049 5054  IVATE`, and `IPT
+00002c90: 7970 6573 2e50 5343 602e 0a0a 4578 616d  ypes.PSC`...Exam
+00002ca0: 706c 653a 0a0a 6060 6070 7974 686f 6e0a  ple:..```python.
+00002cb0: 6672 6f6d 2067 6f6f 676c 652e 636c 6f75  from google.clou
+00002cc0: 642e 7371 6c2e 636f 6e6e 6563 746f 7220  d.sql.connector 
+00002cd0: 696d 706f 7274 2049 5054 7970 6573 0a0a  import IPTypes..
+00002ce0: 636f 6e6e 203d 2063 6f6e 6e65 6374 6f72  conn = connector
+00002cf0: 2e63 6f6e 6e65 6374 280a 2020 2020 2270  .connect(.    "p
+00002d00: 726f 6a65 6374 3a72 6567 696f 6e3a 696e  roject:region:in
+00002d10: 7374 616e 6365 222c 0a20 2020 2022 7079  stance",.    "py
+00002d20: 6d79 7371 6c22 2c0a 2020 2020 6970 5f74  mysql",.    ip_t
+00002d30: 7970 653d 4950 5479 7065 732e 5052 4956  ype=IPTypes.PRIV
+00002d40: 4154 4520 2320 7573 6520 7072 6976 6174  ATE # use privat
+00002d50: 6520 4950 0a2e 2e2e 2069 6e73 6572 7420  e IP.... insert 
+00002d60: 6f74 6865 7220 6b77 6172 6773 202e 2e2e  other kwargs ...
+00002d70: 0a29 0a60 6060 0a0a 4e6f 7465 3a20 4966  .).```..Note: If
+00002d80: 2073 7065 6369 6679 696e 6720 5072 6976   specifying Priv
+00002d90: 6174 6520 4950 206f 7220 5072 6976 6174  ate IP or Privat
+00002da0: 6520 5365 7276 6963 6520 436f 6e6e 6563  e Service Connec
+00002db0: 742c 2079 6f75 7220 6170 706c 6963 6174  t, your applicat
+00002dc0: 696f 6e20 6d75 7374 2062 650a 6174 7461  ion must be.atta
+00002dd0: 6368 6564 2074 6f20 7468 6520 7072 6f70  ched to the prop
+00002de0: 6572 2056 5043 206e 6574 776f 726b 2074  er VPC network t
+00002df0: 6f20 636f 6e6e 6563 7420 746f 2079 6f75  o connect to you
+00002e00: 7220 436c 6f75 6420 5351 4c20 696e 7374  r Cloud SQL inst
+00002e10: 616e 6365 2e20 466f 7220 6d6f 7374 0a61  ance. For most.a
+00002e20: 7070 6c69 6361 7469 6f6e 7320 7468 6973  pplications this
+00002e30: 2077 696c 6c20 7265 7175 6972 6520 7468   will require th
+00002e40: 6520 7573 6520 6f66 2061 205b 5650 4320  e use of a [VPC 
+00002e50: 436f 6e6e 6563 746f 725d 5b76 7063 2d63  Connector][vpc-c
+00002e60: 6f6e 6e65 6374 6f72 5d2e 0a0a 5b70 7363  onnector]...[psc
+00002e70: 5d3a 2068 7474 7073 3a2f 2f63 6c6f 7564  ]: https://cloud
+00002e80: 2e67 6f6f 676c 652e 636f 6d2f 7670 632f  .google.com/vpc/
+00002e90: 646f 6373 2f70 7269 7661 7465 2d73 6572  docs/private-ser
+00002ea0: 7669 6365 2d63 6f6e 6e65 6374 0a5b 7670  vice-connect.[vp
+00002eb0: 632d 636f 6e6e 6563 746f 725d 3a20 6874  c-connector]: ht
+00002ec0: 7470 733a 2f2f 636c 6f75 642e 676f 6f67  tps://cloud.goog
+00002ed0: 6c65 2e63 6f6d 2f76 7063 2f64 6f63 732f  le.com/vpc/docs/
+00002ee0: 636f 6e66 6967 7572 652d 7365 7276 6572  configure-server
+00002ef0: 6c65 7373 2d76 7063 2d61 6363 6573 7323  less-vpc-access#
+00002f00: 6372 6561 7465 2d63 6f6e 6e65 6374 6f72  create-connector
+00002f10: 0a0a 2323 2320 4175 746f 6d61 7469 6320  ..### Automatic 
+00002f20: 4941 4d20 4461 7461 6261 7365 2041 7574  IAM Database Aut
+00002f30: 6865 6e74 6963 6174 696f 6e0a 0a43 6f6e  hentication..Con
+00002f40: 6e65 6374 696f 6e73 2075 7369 6e67 205b  nections using [
+00002f50: 4175 746f 6d61 7469 6320 4941 4d20 6461  Automatic IAM da
+00002f60: 7461 6261 7365 2061 7574 6865 6e74 6963  tabase authentic
+00002f70: 6174 696f 6e5d 2868 7474 7073 3a2f 2f63  ation](https://c
+00002f80: 6c6f 7564 2e67 6f6f 676c 652e 636f 6d2f  loud.google.com/
+00002f90: 7371 6c2f 646f 6373 2f70 6f73 7467 7265  sql/docs/postgre
+00002fa0: 732f 6175 7468 656e 7469 6361 7469 6f6e  s/authentication
+00002fb0: 2361 7574 6f6d 6174 6963 2920 6172 6520  #automatic) are 
+00002fc0: 7375 7070 6f72 7465 6420 7768 656e 2075  supported when u
+00002fd0: 7369 6e67 2050 6f73 7467 7265 7320 6f72  sing Postgres or
+00002fe0: 204d 7953 514c 2064 7269 7665 7273 2e0a   MySQL drivers..
+00002ff0: 4669 7273 742c 206d 616b 6520 7375 7265  First, make sure
+00003000: 2074 6f20 5b63 6f6e 6669 6775 7265 2079   to [configure y
+00003010: 6f75 7220 436c 6f75 6420 5351 4c20 496e  our Cloud SQL In
+00003020: 7374 616e 6365 2074 6f20 616c 6c6f 7720  stance to allow 
+00003030: 4941 4d20 6175 7468 656e 7469 6361 7469  IAM authenticati
+00003040: 6f6e 5d28 6874 7470 733a 2f2f 636c 6f75  on](https://clou
+00003050: 642e 676f 6f67 6c65 2e63 6f6d 2f73 716c  d.google.com/sql
+00003060: 2f64 6f63 732f 706f 7374 6772 6573 2f63  /docs/postgres/c
+00003070: 7265 6174 652d 6564 6974 2d69 616d 2d69  reate-edit-iam-i
+00003080: 6e73 7461 6e63 6573 2363 6f6e 6669 6775  nstances#configu
+00003090: 7265 2d69 616d 2d64 622d 696e 7374 616e  re-iam-db-instan
+000030a0: 6365 290a 616e 6420 5b61 6464 2061 6e20  ce).and [add an 
+000030b0: 4941 4d20 6461 7461 6261 7365 2075 7365  IAM database use
+000030c0: 725d 2868 7474 7073 3a2f 2f63 6c6f 7564  r](https://cloud
+000030d0: 2e67 6f6f 676c 652e 636f 6d2f 7371 6c2f  .google.com/sql/
+000030e0: 646f 6373 2f70 6f73 7467 7265 732f 6372  docs/postgres/cr
+000030f0: 6561 7465 2d6d 616e 6167 652d 6961 6d2d  eate-manage-iam-
+00003100: 7573 6572 7323 6372 6561 7469 6e67 2d61  users#creating-a
+00003110: 2d64 6174 6162 6173 652d 7573 6572 292e  -database-user).
+00003120: 0a0a 4e6f 772c 2079 6f75 2063 616e 2063  ..Now, you can c
+00003130: 6f6e 6e65 6374 2075 7369 6e67 2075 7365  onnect using use
+00003140: 7220 6f72 2073 6572 7669 6365 2061 6363  r or service acc
+00003150: 6f75 6e74 2063 7265 6465 6e74 6961 6c73  ount credentials
+00003160: 2069 6e73 7465 6164 206f 6620 6120 7061   instead of a pa
+00003170: 7373 776f 7264 2e0a 496e 2074 6865 2063  ssword..In the c
+00003180: 616c 6c20 746f 2063 6f6e 6e65 6374 2c20  all to connect, 
+00003190: 7365 7420 7468 6520 6065 6e61 626c 655f  set the `enable_
+000031a0: 6961 6d5f 6175 7468 6020 6b65 7977 6f72  iam_auth` keywor
+000031b0: 6420 6172 6775 6d65 6e74 2074 6f20 7472  d argument to tr
+000031c0: 7565 2061 6e64 2074 6865 2060 7573 6572  ue and the `user
+000031d0: 6020 6172 6775 6d65 6e74 2074 6f20 7468  ` argument to th
+000031e0: 6520 6170 7072 6f70 7269 6174 656c 7920  e appropriately 
+000031f0: 666f 726d 6174 7465 6420 4941 4d20 7072  formatted IAM pr
+00003200: 696e 6369 7061 6c2e 0a3e 2050 6f73 7467  incipal..> Postg
+00003210: 7265 733a 2046 6f72 2061 6e20 4941 4d20  res: For an IAM 
+00003220: 7573 6572 2061 6363 6f75 6e74 2c20 7468  user account, th
+00003230: 6973 2069 7320 7468 6520 7573 6572 2773  is is the user's
+00003240: 2065 6d61 696c 2061 6464 7265 7373 2e20   email address. 
+00003250: 466f 7220 6120 7365 7276 6963 6520 6163  For a service ac
+00003260: 636f 756e 742c 2069 7420 6973 2074 6865  count, it is the
+00003270: 2073 6572 7669 6365 2061 6363 6f75 6e74   service account
+00003280: 2773 2065 6d61 696c 2077 6974 686f 7574  's email without
+00003290: 2074 6865 2060 2e67 7365 7276 6963 6561   the `.gservicea
+000032a0: 6363 6f75 6e74 2e63 6f6d 6020 646f 6d61  ccount.com` doma
+000032b0: 696e 2073 7566 6669 782e 0a0a 3e20 4d79  in suffix...> My
+000032c0: 5351 4c3a 2046 6f72 2061 6e20 4941 4d20  SQL: For an IAM 
+000032d0: 7573 6572 2061 6363 6f75 6e74 2c20 7468  user account, th
+000032e0: 6973 2069 7320 7468 6520 7573 6572 2773  is is the user's
+000032f0: 2065 6d61 696c 2061 6464 7265 7373 2c20   email address, 
+00003300: 7769 7468 6f75 7420 7468 6520 4020 6f72  without the @ or
+00003310: 2064 6f6d 6169 6e20 6e61 6d65 2e20 466f   domain name. Fo
+00003320: 7220 6578 616d 706c 652c 2066 6f72 2060  r example, for `
+00003330: 7465 7374 2d75 7365 7240 676d 6169 6c2e  test-user@gmail.
+00003340: 636f 6d60 2c20 7365 7420 7468 6520 6075  com`, set the `u
+00003350: 7365 7260 2061 7267 756d 656e 7420 746f  ser` argument to
+00003360: 2060 7465 7374 2d75 7365 7260 2e20 466f   `test-user`. Fo
+00003370: 7220 6120 7365 7276 6963 6520 6163 636f  r a service acco
+00003380: 756e 742c 2074 6869 7320 6973 2074 6865  unt, this is the
+00003390: 2073 6572 7669 6365 2061 6363 6f75 6e74   service account
+000033a0: 2773 2065 6d61 696c 2061 6464 7265 7373  's email address
+000033b0: 2077 6974 686f 7574 2074 6865 2060 4070   without the `@p
+000033c0: 726f 6a65 6374 2d69 642e 6961 6d2e 6773  roject-id.iam.gs
+000033d0: 6572 7669 6365 6163 636f 756e 742e 636f  erviceaccount.co
+000033e0: 6d60 2073 7566 6669 782e 0a0a 4578 616d  m` suffix...Exam
+000033f0: 706c 653a 0a0a 6060 6070 7974 686f 6e0a  ple:..```python.
+00003400: 636f 6e6e 203d 2063 6f6e 6e65 6374 6f72  conn = connector
+00003410: 2e63 6f6e 6e65 6374 280a 2020 2020 2022  .connect(.     "
+00003420: 7072 6f6a 6563 743a 7265 6769 6f6e 3a69  project:region:i
+00003430: 6e73 7461 6e63 6522 2c0a 2020 2020 2022  nstance",.     "
+00003440: 7067 3830 3030 222c 0a20 2020 2020 7573  pg8000",.     us
+00003450: 6572 3d22 706f 7374 6772 6573 2d69 616d  er="postgres-iam
+00003460: 2d75 7365 7240 676d 6169 6c2e 636f 6d22  -user@gmail.com"
+00003470: 2c0a 2020 2020 2064 623d 226d 792d 6462  ,.     db="my-db
+00003480: 2d6e 616d 6522 2c0a 2020 2020 2065 6e61  -name",.     ena
+00003490: 626c 655f 6961 6d5f 6175 7468 3d54 7275  ble_iam_auth=Tru
+000034a0: 652c 0a20 290a 6060 600a 0a23 2323 2053  e,. ).```..### S
+000034b0: 514c 2053 6572 7665 7220 4163 7469 7665  QL Server Active
+000034c0: 2044 6972 6563 746f 7279 2041 7574 6865   Directory Authe
+000034d0: 6e74 6963 6174 696f 6e0a 0a41 6374 6976  ntication..Activ
+000034e0: 6520 4469 7265 6374 6f72 7920 6175 7468  e Directory auth
+000034f0: 656e 7469 6361 7469 6f6e 2066 6f72 2053  entication for S
+00003500: 514c 2053 6572 7665 7220 696e 7374 616e  QL Server instan
+00003510: 6365 7320 6973 2063 7572 7265 6e74 6c79  ces is currently
+00003520: 206f 6e6c 7920 7375 7070 6f72 7465 6420   only supported 
+00003530: 6f6e 2057 696e 646f 7773 2e20 4669 7273  on Windows. Firs
+00003540: 742c 206d 616b 6520 7375 7265 2074 6f20  t, make sure to 
+00003550: 666f 6c6c 6f77 205b 7468 6573 6520 7374  follow [these st
+00003560: 6570 735d 2868 7474 7073 3a2f 2f63 6c6f  eps](https://clo
+00003570: 7564 2e67 6f6f 676c 652e 636f 6d2f 626c  ud.google.com/bl
+00003580: 6f67 2f74 6f70 6963 732f 6465 7665 6c6f  og/topics/develo
+00003590: 7065 7273 2d70 7261 6374 6974 696f 6e65  pers-practitione
+000035a0: 7273 2f63 7265 6174 696e 672d 7371 6c2d  rs/creating-sql-
+000035b0: 7365 7276 6572 2d69 6e73 7461 6e63 652d  server-instance-
+000035c0: 696e 7465 6772 6174 6564 2d61 6374 6976  integrated-activ
+000035d0: 652d 6469 7265 6374 6f72 792d 7573 696e  e-directory-usin
+000035e0: 672d 676f 6f67 6c65 2d63 6c6f 7564 2d73  g-google-cloud-s
+000035f0: 716c 2920 746f 2073 6574 2075 7020 6120  ql) to set up a 
+00003600: 4d61 6e61 6765 6420 4144 2064 6f6d 6169  Managed AD domai
+00003610: 6e20 616e 6420 6a6f 696e 2079 6f75 7220  n and join your 
+00003620: 436c 6f75 6420 5351 4c20 696e 7374 616e  Cloud SQL instan
+00003630: 6365 2074 6f20 7468 6520 646f 6d61 696e  ce to the domain
+00003640: 2e20 5b53 6565 2068 6572 6520 666f 7220  . [See here for 
+00003650: 6d6f 7265 2069 6e66 6f20 6f6e 2043 6c6f  more info on Clo
+00003660: 7564 2053 514c 2041 6374 6976 6520 4469  ud SQL Active Di
+00003670: 7265 6374 6f72 7920 696e 7465 6772 6174  rectory integrat
+00003680: 696f 6e5d 2868 7474 7073 3a2f 2f63 6c6f  ion](https://clo
+00003690: 7564 2e67 6f6f 676c 652e 636f 6d2f 7371  ud.google.com/sq
+000036a0: 6c2f 646f 6373 2f73 716c 7365 7276 6572  l/docs/sqlserver
+000036b0: 2f61 6429 2e0a 0a4f 6e63 6520 796f 7520  /ad)...Once you 
+000036c0: 6861 7665 2066 6f6c 6c6f 7765 6420 7468  have followed th
+000036d0: 6520 7374 6570 7320 6c69 6e6b 6564 2061  e steps linked a
+000036e0: 626f 7665 2c20 796f 7520 6361 6e20 7275  bove, you can ru
+000036f0: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
+00003700: 636f 6465 2074 6f20 7265 7475 726e 2061  code to return a
+00003710: 2063 6f6e 6e65 6374 696f 6e20 6f62 6a65   connection obje
+00003720: 6374 3a0a 0a60 6060 7079 7468 6f6e 0a63  ct:..```python.c
+00003730: 6f6e 6e20 3d20 636f 6e6e 6563 746f 722e  onn = connector.
+00003740: 636f 6e6e 6563 7428 0a20 2020 2022 7072  connect(.    "pr
+00003750: 6f6a 6563 743a 7265 6769 6f6e 3a69 6e73  oject:region:ins
+00003760: 7461 6e63 6522 2c0a 2020 2020 2270 7974  tance",.    "pyt
+00003770: 6473 222c 0a20 2020 2064 623d 226d 792d  ds",.    db="my-
+00003780: 6462 2d6e 616d 6522 2c0a 2020 2020 6163  db-name",.    ac
+00003790: 7469 7665 5f64 6972 6563 746f 7279 5f61  tive_directory_a
+000037a0: 7574 683d 5472 7565 2c0a 2020 2020 7365  uth=True,.    se
+000037b0: 7276 6572 5f6e 616d 653d 2270 7562 6c69  rver_name="publi
+000037c0: 632e 5b69 6e73 7461 6e63 655d 2e5b 6c6f  c.[instance].[lo
+000037d0: 6361 7469 6f6e 5d2e 5b70 726f 6a65 6374  cation].[project
+000037e0: 5d2e 636c 6f75 6473 716c 2e5b 646f 6d61  ].cloudsql.[doma
+000037f0: 696e 5d22 2c0a 290a 6060 600a 0a4f 722c  in]",.).```..Or,
+00003800: 2069 6620 7573 696e 6720 5072 6976 6174   if using Privat
+00003810: 6520 4950 3a0a 0a60 6060 7079 7468 6f6e  e IP:..```python
+00003820: 0a63 6f6e 6e20 3d20 636f 6e6e 6563 746f  .conn = connecto
+00003830: 722e 636f 6e6e 6563 7428 0a20 2020 2022  r.connect(.    "
+00003840: 7072 6f6a 6563 743a 7265 6769 6f6e 3a69  project:region:i
+00003850: 6e73 7461 6e63 6522 2c0a 2020 2020 2270  nstance",.    "p
+00003860: 7974 6473 222c 0a20 2020 2064 623d 226d  ytds",.    db="m
+00003870: 792d 6462 2d6e 616d 6522 2c0a 2020 2020  y-db-name",.    
+00003880: 6163 7469 7665 5f64 6972 6563 746f 7279  active_directory
+00003890: 5f61 7574 683d 5472 7565 2c0a 2020 2020  _auth=True,.    
+000038a0: 7365 7276 6572 5f6e 616d 653d 2270 7269  server_name="pri
+000038b0: 7661 7465 2e5b 696e 7374 616e 6365 5d2e  vate.[instance].
+000038c0: 5b6c 6f63 6174 696f 6e5d 2e5b 7072 6f6a  [location].[proj
+000038d0: 6563 745d 2e63 6c6f 7564 7371 6c2e 5b64  ect].cloudsql.[d
+000038e0: 6f6d 6169 6e5d 222c 0a20 2020 2069 705f  omain]",.    ip_
+000038f0: 7479 7065 3d49 5054 7970 6573 2e50 5249  type=IPTypes.PRI
+00003900: 5641 5445 0a29 0a60 6060 0a0a 2323 2320  VATE.).```..### 
+00003910: 5573 696e 6720 7468 6520 5079 7468 6f6e  Using the Python
+00003920: 2043 6f6e 6e65 6374 6f72 2077 6974 6820   Connector with 
+00003930: 5079 7468 6f6e 2057 6562 2046 7261 6d65  Python Web Frame
+00003940: 776f 726b 730a 0a54 6865 2050 7974 686f  works..The Pytho
+00003950: 6e20 436f 6e6e 6563 746f 7220 6361 6e20  n Connector can 
+00003960: 6265 2075 7365 6420 616c 6f6e 6773 6964  be used alongsid
+00003970: 6520 706f 7075 6c61 7220 5079 7468 6f6e  e popular Python
+00003980: 2077 6562 2066 7261 6d65 776f 726b 7320   web frameworks 
+00003990: 7375 6368 0a61 7320 466c 6173 6b2c 2046  such.as Flask, F
+000039a0: 6173 7441 5049 2c20 6574 632c 2074 6f20  astAPI, etc, to 
+000039b0: 696e 7465 6772 6174 6520 436c 6f75 6420  integrate Cloud 
+000039c0: 5351 4c20 6461 7461 6261 7365 7320 7769  SQL databases wi
+000039d0: 7468 696e 2079 6f75 720a 7765 6220 6170  thin your.web ap
+000039e0: 706c 6963 6174 696f 6e73 2e0a 0a23 2323  plications...###
+000039f0: 2320 466c 6173 6b2d 5351 4c41 6c63 6865  # Flask-SQLAlche
+00003a00: 6d79 0a0a 5b46 6c61 736b 2d53 514c 416c  my..[Flask-SQLAl
+00003a10: 6368 656d 795d 2868 7474 7073 3a2f 2f66  chemy](https://f
+00003a20: 6c61 736b 2d73 716c 616c 6368 656d 792e  lask-sqlalchemy.
+00003a30: 7061 6c6c 6574 7370 726f 6a65 6374 732e  palletsprojects.
+00003a40: 636f 6d2f 656e 2f32 2e78 2f29 0a69 7320  com/en/2.x/).is 
+00003a50: 616e 2065 7874 656e 7369 6f6e 2066 6f72  an extension for
+00003a60: 205b 466c 6173 6b5d 2868 7474 7073 3a2f   [Flask](https:/
+00003a70: 2f66 6c61 736b 2e70 616c 6c65 7473 7072  /flask.palletspr
+00003a80: 6f6a 6563 7473 2e63 6f6d 2f65 6e2f 322e  ojects.com/en/2.
+00003a90: 322e 782f 290a 7468 6174 2061 6464 7320  2.x/).that adds 
+00003aa0: 7375 7070 6f72 7420 666f 7220 5b53 514c  support for [SQL
+00003ab0: 416c 6368 656d 795d 2868 7474 7073 3a2f  Alchemy](https:/
+00003ac0: 2f77 7777 2e73 716c 616c 6368 656d 792e  /www.sqlalchemy.
+00003ad0: 6f72 672f 2920 746f 2079 6f75 720a 6170  org/) to your.ap
+00003ae0: 706c 6963 6174 696f 6e2e 2049 7420 6169  plication. It ai
+00003af0: 6d73 2074 6f20 7369 6d70 6c69 6679 2075  ms to simplify u
+00003b00: 7369 6e67 2053 514c 416c 6368 656d 7920  sing SQLAlchemy 
+00003b10: 7769 7468 2046 6c61 736b 2062 7920 7072  with Flask by pr
+00003b20: 6f76 6964 696e 670a 7573 6566 756c 2064  oviding.useful d
+00003b30: 6566 6175 6c74 7320 616e 6420 6578 7472  efaults and extr
+00003b40: 6120 6865 6c70 6572 7320 7468 6174 206d  a helpers that m
+00003b50: 616b 6520 6974 2065 6173 6965 7220 746f  ake it easier to
+00003b60: 2061 6363 6f6d 706c 6973 680a 636f 6d6d   accomplish.comm
+00003b70: 6f6e 2074 6173 6b73 2e0a 0a59 6f75 2063  on tasks...You c
+00003b80: 616e 2063 6f6e 6669 6775 7265 2046 6c61  an configure Fla
+00003b90: 736b 2d53 514c 416c 6368 656d 7920 746f  sk-SQLAlchemy to
+00003ba0: 2063 6f6e 6e65 6374 2074 6f20 6120 436c   connect to a Cl
+00003bb0: 6f75 6420 5351 4c20 6461 7461 6261 7365  oud SQL database
+00003bc0: 2066 726f 6d0a 796f 7572 2077 6562 2061   from.your web a
+00003bd0: 7070 6c69 6361 7469 6f6e 2074 6872 6f75  pplication throu
+00003be0: 6768 2074 6865 2066 6f6c 6c6f 7769 6e67  gh the following
+00003bf0: 3a0a 0a60 6060 7079 7468 6f6e 0a66 726f  :..```python.fro
+00003c00: 6d20 666c 6173 6b20 696d 706f 7274 2046  m flask import F
+00003c10: 6c61 736b 0a66 726f 6d20 666c 6173 6b5f  lask.from flask_
+00003c20: 7371 6c61 6c63 6865 6d79 2069 6d70 6f72  sqlalchemy impor
+00003c30: 7420 5351 4c41 6c63 6865 6d79 0a66 726f  t SQLAlchemy.fro
+00003c40: 6d20 676f 6f67 6c65 2e63 6c6f 7564 2e73  m google.cloud.s
+00003c50: 716c 2e63 6f6e 6e65 6374 6f72 2069 6d70  ql.connector imp
+00003c60: 6f72 7420 436f 6e6e 6563 746f 722c 2049  ort Connector, I
+00003c70: 5054 7970 6573 0a0a 0a23 2069 6e69 7469  PTypes...# initi
+00003c80: 616c 697a 6520 5079 7468 6f6e 2043 6f6e  alize Python Con
+00003c90: 6e65 6374 6f72 206f 626a 6563 740a 636f  nector object.co
+00003ca0: 6e6e 6563 746f 7220 3d20 436f 6e6e 6563  nnector = Connec
+00003cb0: 746f 7228 290a 0a23 2050 7974 686f 6e20  tor()..# Python 
+00003cc0: 436f 6e6e 6563 746f 7220 6461 7461 6261  Connector databa
+00003cd0: 7365 2063 6f6e 6e65 6374 696f 6e20 6675  se connection fu
+00003ce0: 6e63 7469 6f6e 0a64 6566 2067 6574 636f  nction.def getco
+00003cf0: 6e6e 2829 3a0a 2020 2020 636f 6e6e 203d  nn():.    conn =
+00003d00: 2063 6f6e 6e65 6374 6f72 2e63 6f6e 6e65   connector.conne
+00003d10: 6374 280a 2020 2020 2020 2020 2270 726f  ct(.        "pro
+00003d20: 6a65 6374 3a72 6567 696f 6e3a 696e 7374  ject:region:inst
+00003d30: 616e 6365 2d6e 616d 6522 2c20 2320 436c  ance-name", # Cl
+00003d40: 6f75 6420 5351 4c20 496e 7374 616e 6365  oud SQL Instance
+00003d50: 2043 6f6e 6e65 6374 696f 6e20 4e61 6d65   Connection Name
+00003d60: 0a20 2020 2020 2020 2022 7067 3830 3030  .        "pg8000
+00003d70: 222c 0a20 2020 2020 2020 2075 7365 723d  ",.        user=
+00003d80: 226d 792d 7573 6572 222c 0a20 2020 2020  "my-user",.     
+00003d90: 2020 2070 6173 7377 6f72 643d 226d 792d     password="my-
+00003da0: 7061 7373 776f 7264 222c 0a20 2020 2020  password",.     
+00003db0: 2020 2064 623d 226d 792d 6461 7461 6261     db="my-databa
+00003dc0: 7365 222c 0a20 2020 2020 2020 2069 705f  se",.        ip_
+00003dd0: 7479 7065 3d20 4950 5479 7065 732e 5055  type= IPTypes.PU
+00003de0: 424c 4943 2020 2320 4950 5479 7065 732e  BLIC  # IPTypes.
+00003df0: 5052 4956 4154 4520 666f 7220 7072 6976  PRIVATE for priv
+00003e00: 6174 6520 4950 0a20 2020 2029 0a20 2020  ate IP.    ).   
+00003e10: 2072 6574 7572 6e20 636f 6e6e 0a0a 0a61   return conn...a
+00003e20: 7070 203d 2046 6c61 736b 285f 5f6e 616d  pp = Flask(__nam
+00003e30: 655f 5f29 0a0a 2320 636f 6e66 6967 7572  e__)..# configur
+00003e40: 6520 466c 6173 6b2d 5351 4c41 6c63 6865  e Flask-SQLAlche
+00003e50: 6d79 2074 6f20 7573 6520 5079 7468 6f6e  my to use Python
+00003e60: 2043 6f6e 6e65 6374 6f72 0a61 7070 2e63   Connector.app.c
+00003e70: 6f6e 6669 675b 2753 514c 414c 4348 454d  onfig['SQLALCHEM
+00003e80: 595f 4441 5441 4241 5345 5f55 5249 275d  Y_DATABASE_URI']
+00003e90: 203d 2022 706f 7374 6772 6573 716c 2b70   = "postgresql+p
+00003ea0: 6738 3030 303a 2f2f 220a 6170 702e 636f  g8000://".app.co
+00003eb0: 6e66 6967 5b27 5351 4c41 4c43 4845 4d59  nfig['SQLALCHEMY
+00003ec0: 5f45 4e47 494e 455f 4f50 5449 4f4e 5327  _ENGINE_OPTIONS'
+00003ed0: 5d20 3d20 7b0a 2020 2020 2263 7265 6174  ] = {.    "creat
+00003ee0: 6f72 223a 2067 6574 636f 6e6e 0a7d 0a0a  or": getconn.}..
+00003ef0: 2320 696e 6974 6961 6c69 7a65 2074 6865  # initialize the
+00003f00: 2061 7070 2077 6974 6820 7468 6520 6578   app with the ex
+00003f10: 7465 6e73 696f 6e0a 6462 203d 2053 514c  tension.db = SQL
+00003f20: 416c 6368 656d 7928 290a 6462 2e69 6e69  Alchemy().db.ini
+00003f30: 745f 6170 7028 6170 7029 0a60 6060 0a0a  t_app(app).```..
+00003f40: 466f 7220 6d6f 7265 2064 6574 6169 6c73  For more details
+00003f50: 206f 6e20 686f 7720 746f 2075 7365 2046   on how to use F
+00003f60: 6c61 736b 2d53 514c 416c 6368 656d 792c  lask-SQLAlchemy,
+00003f70: 2063 6865 636b 206f 7574 2074 6865 0a5b   check out the.[
+00003f80: 466c 6173 6b2d 5351 4c41 6c63 6865 6d79  Flask-SQLAlchemy
+00003f90: 2051 7569 636b 7374 6172 7473 5d28 6874   Quickstarts](ht
+00003fa0: 7470 733a 2f2f 666c 6173 6b2d 7371 6c61  tps://flask-sqla
+00003fb0: 6c63 6865 6d79 2e70 616c 6c65 7473 7072  lchemy.palletspr
+00003fc0: 6f6a 6563 7473 2e63 6f6d 2f65 6e2f 332e  ojects.com/en/3.
+00003fd0: 302e 782f 7175 6963 6b73 7461 7274 2f29  0.x/quickstart/)
+00003fe0: 0a0a 2323 2323 2046 6173 7441 5049 0a0a  ..#### FastAPI..
+00003ff0: 5b46 6173 7441 5049 5d28 6874 7470 733a  [FastAPI](https:
+00004000: 2f2f 6661 7374 6170 692e 7469 616e 676f  //fastapi.tiango
+00004010: 6c6f 2e63 6f6d 2f29 2069 7320 6120 6d6f  lo.com/) is a mo
+00004020: 6465 726e 2c20 6661 7374 2028 6869 6768  dern, fast (high
+00004030: 2d70 6572 666f 726d 616e 6365 292c 0a77  -performance),.w
+00004040: 6562 2066 7261 6d65 776f 726b 2066 6f72  eb framework for
+00004050: 2062 7569 6c64 696e 6720 4150 4973 2077   building APIs w
+00004060: 6974 6820 5079 7468 6f6e 2062 6173 6564  ith Python based
+00004070: 206f 6e20 7374 616e 6461 7264 2050 7974   on standard Pyt
+00004080: 686f 6e20 7479 7065 2068 696e 7473 2e0a  hon type hints..
+00004090: 0a59 6f75 2063 616e 2063 6f6e 6669 6775  .You can configu
+000040a0: 7265 2046 6173 7441 5049 2074 6f20 636f  re FastAPI to co
+000040b0: 6e6e 6563 7420 746f 2061 2043 6c6f 7564  nnect to a Cloud
+000040c0: 2053 514c 2064 6174 6162 6173 6520 6672   SQL database fr
+000040d0: 6f6d 0a79 6f75 7220 7765 6220 6170 706c  om.your web appl
+000040e0: 6963 6174 696f 6e20 7573 696e 6720 5b53  ication using [S
+000040f0: 514c 416c 6368 656d 7920 4f52 4d5d 2868  QLAlchemy ORM](h
+00004100: 7474 7073 3a2f 2f64 6f63 732e 7371 6c61  ttps://docs.sqla
+00004110: 6c63 6865 6d79 2e6f 7267 2f65 6e2f 3134  lchemy.org/en/14
+00004120: 2f6f 726d 2f29 0a74 6872 6f75 6768 2074  /orm/).through t
+00004130: 6865 2066 6f6c 6c6f 7769 6e67 3a0a 0a60  he following:..`
+00004140: 6060 7079 7468 6f6e 0a66 726f 6d20 7371  ``python.from sq
+00004150: 6c61 6c63 6865 6d79 2069 6d70 6f72 7420  lalchemy import 
+00004160: 6372 6561 7465 5f65 6e67 696e 650a 6672  create_engine.fr
+00004170: 6f6d 2073 716c 616c 6368 656d 792e 656e  om sqlalchemy.en
+00004180: 6769 6e65 2069 6d70 6f72 7420 456e 6769  gine import Engi
+00004190: 6e65 0a66 726f 6d20 7371 6c61 6c63 6865  ne.from sqlalche
+000041a0: 6d79 2e65 7874 2e64 6563 6c61 7261 7469  my.ext.declarati
+000041b0: 7665 2069 6d70 6f72 7420 6465 636c 6172  ve import declar
+000041c0: 6174 6976 655f 6261 7365 0a66 726f 6d20  ative_base.from 
+000041d0: 7371 6c61 6c63 6865 6d79 2e6f 726d 2069  sqlalchemy.orm i
+000041e0: 6d70 6f72 7420 7365 7373 696f 6e6d 616b  mport sessionmak
+000041f0: 6572 0a66 726f 6d20 676f 6f67 6c65 2e63  er.from google.c
+00004200: 6c6f 7564 2e73 716c 2e63 6f6e 6e65 6374  loud.sql.connect
+00004210: 6f72 2069 6d70 6f72 7420 436f 6e6e 6563  or import Connec
+00004220: 746f 722c 2049 5054 7970 6573 0a0a 2320  tor, IPTypes..# 
+00004230: 6865 6c70 6572 2066 756e 6374 696f 6e20  helper function 
+00004240: 746f 2072 6574 7572 6e20 5351 4c41 6c63  to return SQLAlc
+00004250: 6865 6d79 2063 6f6e 6e65 6374 696f 6e20  hemy connection 
+00004260: 706f 6f6c 0a64 6566 2069 6e69 745f 636f  pool.def init_co
+00004270: 6e6e 6563 7469 6f6e 5f70 6f6f 6c28 636f  nnection_pool(co
+00004280: 6e6e 6563 746f 723a 2043 6f6e 6e65 6374  nnector: Connect
+00004290: 6f72 2920 2d3e 2045 6e67 696e 653a 0a20  or) -> Engine:. 
+000042a0: 2020 2023 2050 7974 686f 6e20 436f 6e6e     # Python Conn
+000042b0: 6563 746f 7220 6461 7461 6261 7365 2063  ector database c
+000042c0: 6f6e 6e65 6374 696f 6e20 6675 6e63 7469  onnection functi
+000042d0: 6f6e 0a20 2020 2064 6566 2067 6574 636f  on.    def getco
+000042e0: 6e6e 2829 3a0a 2020 2020 2020 2020 636f  nn():.        co
+000042f0: 6e6e 203d 2063 6f6e 6e65 6374 6f72 2e63  nn = connector.c
+00004300: 6f6e 6e65 6374 280a 2020 2020 2020 2020  onnect(.        
+00004310: 2020 2020 2270 726f 6a65 6374 3a72 6567      "project:reg
+00004320: 696f 6e3a 696e 7374 616e 6365 2d6e 616d  ion:instance-nam
+00004330: 6522 2c20 2320 436c 6f75 6420 5351 4c20  e", # Cloud SQL 
+00004340: 496e 7374 616e 6365 2043 6f6e 6e65 6374  Instance Connect
+00004350: 696f 6e20 4e61 6d65 0a20 2020 2020 2020  ion Name.       
+00004360: 2020 2020 2022 7067 3830 3030 222c 0a20       "pg8000",. 
+00004370: 2020 2020 2020 2020 2020 2075 7365 723d             user=
+00004380: 226d 792d 7573 6572 222c 0a20 2020 2020  "my-user",.     
+00004390: 2020 2020 2020 2070 6173 7377 6f72 643d         password=
+000043a0: 226d 792d 7061 7373 776f 7264 222c 0a20  "my-password",. 
+000043b0: 2020 2020 2020 2020 2020 2064 623d 226d             db="m
+000043c0: 792d 6461 7461 6261 7365 222c 0a20 2020  y-database",.   
+000043d0: 2020 2020 2020 2020 2069 705f 7479 7065           ip_type
+000043e0: 3d20 4950 5479 7065 732e 5055 424c 4943  = IPTypes.PUBLIC
+000043f0: 2020 2320 4950 5479 7065 732e 5052 4956    # IPTypes.PRIV
+00004400: 4154 4520 666f 7220 7072 6976 6174 6520  ATE for private 
+00004410: 4950 0a20 2020 2020 2020 2029 0a20 2020  IP.        ).   
+00004420: 2020 2020 2072 6574 7572 6e20 636f 6e6e       return conn
+00004430: 0a0a 2020 2020 5351 4c41 4c43 4845 4d59  ..    SQLALCHEMY
+00004440: 5f44 4154 4142 4153 455f 5552 4c20 3d20  _DATABASE_URL = 
+00004450: 2270 6f73 7467 7265 7371 6c2b 7067 3830  "postgresql+pg80
+00004460: 3030 3a2f 2f22 0a0a 2020 2020 656e 6769  00://"..    engi
+00004470: 6e65 203d 2063 7265 6174 655f 656e 6769  ne = create_engi
+00004480: 6e65 280a 2020 2020 2020 2020 5351 4c41  ne(.        SQLA
+00004490: 4c43 4845 4d59 5f44 4154 4142 4153 455f  LCHEMY_DATABASE_
+000044a0: 5552 4c20 2c20 6372 6561 746f 723d 6765  URL , creator=ge
+000044b0: 7463 6f6e 6e0a 2020 2020 290a 2020 2020  tconn.    ).    
+000044c0: 7265 7475 726e 2065 6e67 696e 650a 0a23  return engine..#
+000044d0: 2069 6e69 7469 616c 697a 6520 436c 6f75   initialize Clou
+000044e0: 6420 5351 4c20 5079 7468 6f6e 2043 6f6e  d SQL Python Con
+000044f0: 6e65 6374 6f72 0a63 6f6e 6e65 6374 6f72  nector.connector
+00004500: 203d 2043 6f6e 6e65 6374 6f72 2829 0a0a   = Connector()..
+00004510: 2320 6372 6561 7465 2063 6f6e 6e65 6374  # create connect
+00004520: 696f 6e20 706f 6f6c 2065 6e67 696e 650a  ion pool engine.
+00004530: 656e 6769 6e65 203d 2069 6e69 745f 636f  engine = init_co
+00004540: 6e6e 6563 7469 6f6e 5f70 6f6f 6c28 636f  nnection_pool(co
+00004550: 6e6e 6563 746f 7229 0a0a 2320 6372 6561  nnector)..# crea
+00004560: 7465 2053 514c 416c 6368 656d 7920 4f52  te SQLAlchemy OR
+00004570: 4d20 7365 7373 696f 6e0a 5365 7373 696f  M session.Sessio
+00004580: 6e4c 6f63 616c 203d 2073 6573 7369 6f6e  nLocal = session
+00004590: 6d61 6b65 7228 6175 746f 636f 6d6d 6974  maker(autocommit
+000045a0: 3d46 616c 7365 2c20 6175 746f 666c 7573  =False, autoflus
+000045b0: 683d 4661 6c73 652c 2062 696e 643d 656e  h=False, bind=en
+000045c0: 6769 6e65 290a 0a42 6173 6520 3d20 6465  gine)..Base = de
+000045d0: 636c 6172 6174 6976 655f 6261 7365 2829  clarative_base()
+000045e0: 0a60 6060 0a0a 546f 206c 6561 726e 206d  .```..To learn m
+000045f0: 6f72 6520 6162 6f75 7420 696e 7465 6772  ore about integr
+00004600: 6174 696e 6720 6120 6461 7461 6261 7365  ating a database
+00004610: 2069 6e74 6f20 796f 7572 2046 6173 7441   into your FastA
+00004620: 5049 2061 7070 6c69 6361 7469 6f6e 2c0a  PI application,.
+00004630: 666f 6c6c 6f77 2061 6c6f 6e67 2074 6865  follow along the
+00004640: 205b 4661 7374 4150 4920 5351 4c20 4461   [FastAPI SQL Da
+00004650: 7461 6261 7365 2067 7569 6465 5d28 6874  tabase guide](ht
+00004660: 7470 733a 2f2f 6661 7374 6170 692e 7469  tps://fastapi.ti
+00004670: 616e 676f 6c6f 2e63 6f6d 2f74 7574 6f72  angolo.com/tutor
+00004680: 6961 6c2f 7371 6c2d 6461 7461 6261 7365  ial/sql-database
+00004690: 732f 2363 7265 6174 652d 7468 652d 6461  s/#create-the-da
+000046a0: 7461 6261 7365 2d6d 6f64 656c 7329 2e0a  tabase-models)..
+000046b0: 0a23 2323 2041 7379 6e63 2044 7269 7665  .### Async Drive
+000046c0: 7220 5573 6167 650a 0a54 6865 2043 6c6f  r Usage..The Clo
+000046d0: 7564 2053 514c 2043 6f6e 6e65 6374 6f72  ud SQL Connector
+000046e0: 2069 7320 636f 6d70 6174 6962 6c65 2077   is compatible w
+000046f0: 6974 680a 5b61 7379 6e63 696f 5d28 6874  ith.[asyncio](ht
+00004700: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
+00004710: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
+00004720: 6173 796e 6369 6f2e 6874 6d6c 2920 746f  asyncio.html) to
+00004730: 2069 6d70 726f 7665 2074 6865 2073 7065   improve the spe
+00004740: 6564 0a61 6e64 2065 6666 6963 6965 6e63  ed.and efficienc
+00004750: 7920 6f66 2064 6174 6162 6173 6520 636f  y of database co
+00004760: 6e6e 6563 7469 6f6e 7320 7468 726f 7567  nnections throug
+00004770: 6820 636f 6e63 7572 7265 6e63 792e 2059  h concurrency. Y
+00004780: 6f75 2063 616e 2075 7365 2061 6c6c 0a6e  ou can use all.n
+00004790: 6f6e 2d61 7379 6e63 696f 2064 7269 7665  on-asyncio drive
+000047a0: 7273 2074 6872 6f75 6768 2074 6865 2060  rs through the `
+000047b0: 436f 6e6e 6563 746f 722e 636f 6e6e 6563  Connector.connec
+000047c0: 745f 6173 796e 6360 2066 756e 6374 696f  t_async` functio
+000047d0: 6e2c 2069 6e20 6164 6469 7469 6f6e 0a74  n, in addition.t
+000047e0: 6f20 7468 6520 666f 6c6c 6f77 696e 6720  o the following 
+000047f0: 6173 796e 6369 6f20 6461 7461 6261 7365  asyncio database
+00004800: 2064 7269 7665 7273 3a0a 2d20 5b61 7379   drivers:.- [asy
+00004810: 6e63 7067 5d28 6874 7470 733a 2f2f 6d61  ncpg](https://ma
+00004820: 6769 6373 7461 636b 2e67 6974 6875 622e  gicstack.github.
+00004830: 696f 2f61 7379 6e63 7067 2920 2850 6f73  io/asyncpg) (Pos
+00004840: 7467 7265 7329 0a0a 5468 6520 436c 6f75  tgres)..The Clou
+00004850: 6420 5351 4c20 436f 6e6e 6563 746f 7220  d SQL Connector 
+00004860: 6861 7320 6120 6865 6c70 6572 2060 6372  has a helper `cr
+00004870: 6561 7465 5f61 7379 6e63 5f63 6f6e 6e65  eate_async_conne
+00004880: 6374 6f72 6020 6675 6e63 7469 6f6e 2074  ctor` function t
+00004890: 6861 7420 6973 0a72 6563 6f6d 6d65 6e64  hat is.recommend
+000048a0: 6564 2066 6f72 2061 7379 6e63 696f 2064  ed for asyncio d
+000048b0: 6174 6162 6173 6520 636f 6e6e 6563 7469  atabase connecti
+000048c0: 6f6e 732e 2049 7420 7265 7475 726e 7320  ons. It returns 
+000048d0: 6120 6043 6f6e 6e65 6374 6f72 600a 6f62  a `Connector`.ob
+000048e0: 6a65 6374 2074 6861 7420 7573 6573 2074  ject that uses t
+000048f0: 6865 2063 7572 7265 6e74 2074 6872 6561  he current threa
+00004900: 6427 7320 7275 6e6e 696e 6720 6576 656e  d's running even
+00004910: 7420 6c6f 6f70 2e20 5468 6973 2069 7320  t loop. This is 
+00004920: 6469 6666 6572 656e 740a 7468 616e 2060  different.than `
+00004930: 436f 6e6e 6563 746f 7228 2960 2077 6869  Connector()` whi
+00004940: 6368 2062 7920 6465 6661 756c 7420 696e  ch by default in
+00004950: 6974 6961 6c69 7a65 7320 6120 6e65 7720  itializes a new 
+00004960: 6576 656e 7420 6c6f 6f70 2069 6e20 610a  event loop in a.
+00004970: 6261 636b 6772 6f75 6e64 2074 6872 6561  background threa
+00004980: 642e 0a0a 5468 6520 6063 7265 6174 655f  d...The `create_
+00004990: 6173 796e 635f 636f 6e6e 6563 746f 7260  async_connector`
+000049a0: 2061 6c6c 6f77 7320 616c 6c20 7468 6520   allows all the 
+000049b0: 7361 6d65 2069 6e70 7574 2061 7267 756d  same input argum
+000049c0: 656e 7473 2061 7320 7468 650a 5b43 6f6e  ents as the.[Con
+000049d0: 6e65 6374 6f72 5d28 2363 6f6e 6669 6775  nector](#configu
+000049e0: 7269 6e67 2d74 6865 2d63 6f6e 6e65 6374  ring-the-connect
+000049f0: 6f72 2920 6f62 6a65 6374 2e0a 0a4f 6e63  or) object...Onc
+00004a00: 6520 6120 6043 6f6e 6e65 6374 6f72 6020  e a `Connector` 
+00004a10: 6f62 6a65 6374 2069 7320 7265 7475 726e  object is return
+00004a20: 6564 2062 7920 6063 7265 6174 655f 6173  ed by `create_as
+00004a30: 796e 635f 636f 6e6e 6563 746f 7260 2079  ync_connector` y
+00004a40: 6f75 2063 616e 2063 616c 6c0a 6974 7320  ou can call.its 
+00004a50: 6063 6f6e 6e65 6374 5f61 7379 6e63 6020  `connect_async` 
+00004a60: 6d65 7468 6f64 2c20 6a75 7374 2061 7320  method, just as 
+00004a70: 796f 7520 776f 756c 6420 7468 6520 6063  you would the `c
+00004a80: 6f6e 6e65 6374 6020 6d65 7468 6f64 3a0a  onnect` method:.
+00004a90: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
+00004aa0: 7420 6173 796e 6370 670a 0a69 6d70 6f72  t asyncpg..impor
+00004ab0: 7420 7371 6c61 6c63 6865 6d79 0a66 726f  t sqlalchemy.fro
+00004ac0: 6d20 7371 6c61 6c63 6865 6d79 2e65 7874  m sqlalchemy.ext
+00004ad0: 2e61 7379 6e63 696f 2069 6d70 6f72 7420  .asyncio import 
+00004ae0: 4173 796e 6345 6e67 696e 652c 2063 7265  AsyncEngine, cre
+00004af0: 6174 655f 6173 796e 635f 656e 6769 6e65  ate_async_engine
+00004b00: 0a0a 6672 6f6d 2067 6f6f 676c 652e 636c  ..from google.cl
+00004b10: 6f75 642e 7371 6c2e 636f 6e6e 6563 746f  oud.sql.connecto
+00004b20: 7220 696d 706f 7274 2043 6f6e 6e65 6374  r import Connect
+00004b30: 6f72 2c20 6372 6561 7465 5f61 7379 6e63  or, create_async
+00004b40: 5f63 6f6e 6e65 6374 6f72 0a0a 6173 796e  _connector..asyn
+00004b50: 6320 6465 6620 696e 6974 5f63 6f6e 6e65  c def init_conne
+00004b60: 6374 696f 6e5f 706f 6f6c 2863 6f6e 6e65  ction_pool(conne
+00004b70: 6374 6f72 3a20 436f 6e6e 6563 746f 7229  ctor: Connector)
+00004b80: 202d 3e20 4173 796e 6345 6e67 696e 653a   -> AsyncEngine:
+00004b90: 0a20 2020 2023 2069 6e69 7469 616c 697a  .    # initializ
+00004ba0: 6520 436f 6e6e 6563 746f 7220 6f62 6a65  e Connector obje
+00004bb0: 6374 2066 6f72 2063 6f6e 6e65 6374 696f  ct for connectio
+00004bc0: 6e73 2074 6f20 436c 6f75 6420 5351 4c0a  ns to Cloud SQL.
+00004bd0: 2020 2020 6173 796e 6320 6465 6620 6765      async def ge
+00004be0: 7463 6f6e 6e28 2920 2d3e 2061 7379 6e63  tconn() -> async
+00004bf0: 7067 2e43 6f6e 6e65 6374 696f 6e3a 0a20  pg.Connection:. 
+00004c00: 2020 2020 2020 2063 6f6e 6e3a 2061 7379         conn: asy
+00004c10: 6e63 7067 2e43 6f6e 6e65 6374 696f 6e20  ncpg.Connection 
+00004c20: 3d20 6177 6169 7420 636f 6e6e 6563 746f  = await connecto
+00004c30: 722e 636f 6e6e 6563 745f 6173 796e 6328  r.connect_async(
+00004c40: 0a20 2020 2020 2020 2020 2020 2022 7072  .            "pr
+00004c50: 6f6a 6563 743a 7265 6769 6f6e 3a69 6e73  oject:region:ins
+00004c60: 7461 6e63 6522 2c20 2023 2043 6c6f 7564  tance",  # Cloud
+00004c70: 2053 514c 2069 6e73 7461 6e63 6520 636f   SQL instance co
+00004c80: 6e6e 6563 7469 6f6e 206e 616d 650a 2020  nnection name.  
+00004c90: 2020 2020 2020 2020 2020 2261 7379 6e63            "async
+00004ca0: 7067 222c 0a20 2020 2020 2020 2020 2020  pg",.           
+00004cb0: 2075 7365 723d 226d 792d 7573 6572 222c   user="my-user",
+00004cc0: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
+00004cd0: 7377 6f72 643d 226d 792d 7061 7373 776f  sword="my-passwo
+00004ce0: 7264 222c 0a20 2020 2020 2020 2020 2020  rd",.           
+00004cf0: 2064 623d 226d 792d 6462 2d6e 616d 6522   db="my-db-name"
+00004d00: 0a20 2020 2020 2020 2020 2020 2023 202e  .            # .
+00004d10: 2e2e 2061 6464 6974 696f 6e61 6c20 6461  .. additional da
+00004d20: 7461 6261 7365 2064 7269 7665 7220 6172  tabase driver ar
+00004d30: 6773 0a20 2020 2020 2020 2029 0a20 2020  gs.        ).   
+00004d40: 2020 2020 2072 6574 7572 6e20 636f 6e6e       return conn
+00004d50: 0a0a 2020 2020 2320 5468 6520 436c 6f75  ..    # The Clou
+00004d60: 6420 5351 4c20 5079 7468 6f6e 2043 6f6e  d SQL Python Con
+00004d70: 6e65 6374 6f72 2063 616e 2062 6520 7573  nector can be us
+00004d80: 6564 2061 6c6f 6e67 2077 6974 6820 5351  ed along with SQ
+00004d90: 4c41 6c63 6865 6d79 2075 7369 6e67 2074  LAlchemy using t
+00004da0: 6865 0a20 2020 2023 2027 6173 796e 635f  he.    # 'async_
+00004db0: 6372 6561 746f 7227 2061 7267 756d 656e  creator' argumen
+00004dc0: 7420 746f 2027 6372 6561 7465 5f61 7379  t to 'create_asy
+00004dd0: 6e63 5f65 6e67 696e 6527 0a20 2020 2070  nc_engine'.    p
+00004de0: 6f6f 6c20 3d20 6372 6561 7465 5f61 7379  ool = create_asy
+00004df0: 6e63 5f65 6e67 696e 6528 0a20 2020 2020  nc_engine(.     
+00004e00: 2020 2022 706f 7374 6772 6573 716c 2b61     "postgresql+a
+00004e10: 7379 6e63 7067 3a2f 2f22 2c0a 2020 2020  syncpg://",.    
+00004e20: 2020 2020 6173 796e 635f 6372 6561 746f      async_creato
+00004e30: 723d 6765 7463 6f6e 6e2c 0a20 2020 2029  r=getconn,.    )
+00004e40: 0a20 2020 2072 6574 7572 6e20 706f 6f6c  .    return pool
+00004e50: 0a0a 6173 796e 6320 6465 6620 6d61 696e  ..async def main
+00004e60: 2829 3a0a 2020 2020 2320 696e 6974 6961  ():.    # initia
+00004e70: 6c69 7a65 2043 6f6e 6e65 6374 6f72 206f  lize Connector o
+00004e80: 626a 6563 7420 666f 7220 636f 6e6e 6563  bject for connec
+00004e90: 7469 6f6e 7320 746f 2043 6c6f 7564 2053  tions to Cloud S
+00004ea0: 514c 0a20 2020 2063 6f6e 6e65 6374 6f72  QL.    connector
+00004eb0: 203d 2061 7761 6974 2063 7265 6174 655f   = await create_
+00004ec0: 6173 796e 635f 636f 6e6e 6563 746f 7228  async_connector(
+00004ed0: 290a 0a20 2020 2023 2069 6e69 7469 616c  )..    # initial
+00004ee0: 697a 6520 636f 6e6e 6563 7469 6f6e 2070  ize connection p
+00004ef0: 6f6f 6c0a 2020 2020 706f 6f6c 203d 2061  ool.    pool = a
+00004f00: 7761 6974 2069 6e69 745f 636f 6e6e 6563  wait init_connec
+00004f10: 7469 6f6e 5f70 6f6f 6c28 636f 6e6e 6563  tion_pool(connec
+00004f20: 746f 7229 0a0a 2020 2020 2320 6578 616d  tor)..    # exam
+00004f30: 706c 6520 7175 6572 790a 2020 2020 6173  ple query.    as
+00004f40: 796e 6320 7769 7468 2070 6f6f 6c2e 636f  ync with pool.co
+00004f50: 6e6e 6563 7428 2920 6173 2063 6f6e 6e3a  nnect() as conn:
+00004f60: 0a20 2020 2020 2020 2061 7761 6974 2063  .        await c
+00004f70: 6f6e 6e2e 6578 6563 7574 6528 7371 6c61  onn.execute(sqla
+00004f80: 6c63 6865 6d79 2e74 6578 7428 2253 454c  lchemy.text("SEL
+00004f90: 4543 5420 4e4f 5728 2922 2929 0a0a 2020  ECT NOW()"))..  
+00004fa0: 2020 2320 636c 6f73 6520 436f 6e6e 6563    # close Connec
+00004fb0: 746f 720a 2020 2020 6177 6169 7420 636f  tor.    await co
+00004fc0: 6e6e 6563 746f 722e 636c 6f73 655f 6173  nnector.close_as
+00004fd0: 796e 6328 290a 0a20 2020 2023 2064 6973  ync()..    # dis
+00004fe0: 706f 7365 206f 6620 636f 6e6e 6563 7469  pose of connecti
+00004ff0: 6f6e 2070 6f6f 6c0a 2020 2020 6177 6169  on pool.    awai
+00005000: 7420 706f 6f6c 2e64 6973 706f 7365 2829  t pool.dispose()
+00005010: 0a60 6060 0a0a 466f 7220 6d6f 7265 2064  .```..For more d
+00005020: 6574 6169 6c73 206f 6e20 6164 6469 7469  etails on additi
+00005030: 6f6e 616c 2064 6174 6162 6173 6520 6172  onal database ar
+00005040: 6775 6d65 6e74 7320 7769 7468 2061 6e20  guments with an 
+00005050: 6061 7379 6e63 7067 2e43 6f6e 6e65 6374  `asyncpg.Connect
+00005060: 696f 6e60 0a2c 2070 6c65 6173 6520 7669  ion`., please vi
+00005070: 7369 7420 7468 650a 5b6f 6666 6963 6961  sit the.[officia
+00005080: 6c20 646f 6375 6d65 6e74 6174 696f 6e5d  l documentation]
+00005090: 2868 7474 7073 3a2f 2f6d 6167 6963 7374  (https://magicst
+000050a0: 6163 6b2e 6769 7468 7562 2e69 6f2f 6173  ack.github.io/as
+000050b0: 796e 6370 672f 6375 7272 656e 742f 6170  yncpg/current/ap
+000050c0: 692f 696e 6465 782e 6874 6d6c 292e 0a0a  i/index.html)...
+000050d0: 2323 2320 4173 796e 6320 436f 6e74 6578  ### Async Contex
+000050e0: 7420 4d61 6e61 6765 720a 0a41 6e20 616c  t Manager..An al
+000050f0: 7465 726e 6174 6976 6520 746f 2075 7369  ternative to usi
+00005100: 6e67 2074 6865 2060 6372 6561 7465 5f61  ng the `create_a
+00005110: 7379 6e63 5f63 6f6e 6e65 6374 6f72 6020  sync_connector` 
+00005120: 6675 6e63 7469 6f6e 2069 7320 696e 6974  function is init
+00005130: 6961 6c69 7a69 6e67 0a61 2060 436f 6e6e  ializing.a `Conn
+00005140: 6563 746f 7260 2061 7320 616e 2061 7379  ector` as an asy
+00005150: 6e63 2063 6f6e 7465 7874 206d 616e 6167  nc context manag
+00005160: 6572 2c20 7265 6d6f 7669 6e67 2074 6865  er, removing the
+00005170: 206e 6565 6420 666f 7220 6578 706c 6963   need for explic
+00005180: 6974 0a63 616c 6c73 2074 6f20 6063 6f6e  it.calls to `con
+00005190: 6e65 6374 6f72 2e63 6c6f 7365 5f61 7379  nector.close_asy
+000051a0: 6e63 2829 6020 746f 2063 6c65 616e 7570  nc()` to cleanup
+000051b0: 2072 6573 6f75 7263 6573 2e0a 0a2a 2a4e   resources...**N
+000051c0: 6f74 653a 2a2a 2054 6869 7320 616c 7465  ote:** This alte
+000051d0: 726e 6174 6976 6520 7265 7175 6972 6573  rnative requires
+000051e0: 2074 6861 7420 7468 6520 7275 6e6e 696e   that the runnin
+000051f0: 6720 6576 656e 7420 6c6f 6f70 2062 650a  g event loop be.
+00005200: 7061 7373 6564 2069 6e20 6173 2074 6865  passed in as the
+00005210: 2060 6c6f 6f70 6020 6172 6775 6d65 6e74   `loop` argument
+00005220: 2074 6f20 6043 6f6e 6e65 6374 6f72 2829   to `Connector()
+00005230: 602e 0a0a 6060 6070 7974 686f 6e0a 696d  `...```python.im
+00005240: 706f 7274 2061 7379 6e63 696f 0a69 6d70  port asyncio.imp
+00005250: 6f72 7420 6173 796e 6370 670a 0a69 6d70  ort asyncpg..imp
+00005260: 6f72 7420 7371 6c61 6c63 6865 6d79 0a66  ort sqlalchemy.f
+00005270: 726f 6d20 7371 6c61 6c63 6865 6d79 2e65  rom sqlalchemy.e
+00005280: 7874 2e61 7379 6e63 696f 2069 6d70 6f72  xt.asyncio impor
+00005290: 7420 4173 796e 6345 6e67 696e 652c 2063  t AsyncEngine, c
+000052a0: 7265 6174 655f 6173 796e 635f 656e 6769  reate_async_engi
+000052b0: 6e65 0a0a 6672 6f6d 2067 6f6f 676c 652e  ne..from google.
+000052c0: 636c 6f75 642e 7371 6c2e 636f 6e6e 6563  cloud.sql.connec
+000052d0: 746f 7220 696d 706f 7274 2043 6f6e 6e65  tor import Conne
+000052e0: 6374 6f72 0a0a 6173 796e 6320 6465 6620  ctor..async def 
+000052f0: 696e 6974 5f63 6f6e 6e65 6374 696f 6e5f  init_connection_
+00005300: 706f 6f6c 2863 6f6e 6e65 6374 6f72 3a20  pool(connector: 
+00005310: 436f 6e6e 6563 746f 7229 202d 3e20 4173  Connector) -> As
+00005320: 796e 6345 6e67 696e 653a 0a20 2020 2023  yncEngine:.    #
+00005330: 2069 6e69 7469 616c 697a 6520 436f 6e6e   initialize Conn
+00005340: 6563 746f 7220 6f62 6a65 6374 2066 6f72  ector object for
+00005350: 2063 6f6e 6e65 6374 696f 6e73 2074 6f20   connections to 
+00005360: 436c 6f75 6420 5351 4c0a 2020 2020 6173  Cloud SQL.    as
+00005370: 796e 6320 6465 6620 6765 7463 6f6e 6e28  ync def getconn(
+00005380: 2920 2d3e 2061 7379 6e63 7067 2e43 6f6e  ) -> asyncpg.Con
+00005390: 6e65 6374 696f 6e3a 0a20 2020 2020 2020  nection:.       
+000053a0: 2020 2020 2063 6f6e 6e3a 2061 7379 6e63       conn: async
+000053b0: 7067 2e43 6f6e 6e65 6374 696f 6e20 3d20  pg.Connection = 
+000053c0: 6177 6169 7420 636f 6e6e 6563 746f 722e  await connector.
+000053d0: 636f 6e6e 6563 745f 6173 796e 6328 0a20  connect_async(. 
+000053e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000053f0: 7072 6f6a 6563 743a 7265 6769 6f6e 3a69  project:region:i
+00005400: 6e73 7461 6e63 6522 2c20 2023 2043 6c6f  nstance",  # Clo
+00005410: 7564 2053 514c 2069 6e73 7461 6e63 6520  ud SQL instance 
+00005420: 636f 6e6e 6563 7469 6f6e 206e 616d 650a  connection name.
+00005430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005440: 2261 7379 6e63 7067 222c 0a20 2020 2020  "asyncpg",.     
+00005450: 2020 2020 2020 2020 2020 2075 7365 723d             user=
+00005460: 226d 792d 7573 6572 222c 0a20 2020 2020  "my-user",.     
+00005470: 2020 2020 2020 2020 2020 2070 6173 7377             passw
+00005480: 6f72 643d 226d 792d 7061 7373 776f 7264  ord="my-password
+00005490: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000054a0: 2020 2064 623d 226d 792d 6462 2d6e 616d     db="my-db-nam
+000054b0: 6522 0a20 2020 2020 2020 2020 2020 2020  e".             
+000054c0: 2020 2023 202e 2e2e 2061 6464 6974 696f     # ... additio
+000054d0: 6e61 6c20 6461 7461 6261 7365 2064 7269  nal database dri
+000054e0: 7665 7220 6172 6773 0a20 2020 2020 2020  ver args.       
+000054f0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00005500: 2020 2072 6574 7572 6e20 636f 6e6e 0a0a     return conn..
+00005510: 2020 2020 2320 5468 6520 436c 6f75 6420      # The Cloud 
+00005520: 5351 4c20 5079 7468 6f6e 2043 6f6e 6e65  SQL Python Conne
+00005530: 6374 6f72 2063 616e 2062 6520 7573 6564  ctor can be used
+00005540: 2061 6c6f 6e67 2077 6974 6820 5351 4c41   along with SQLA
+00005550: 6c63 6865 6d79 2075 7369 6e67 2074 6865  lchemy using the
+00005560: 0a20 2020 2023 2027 6173 796e 635f 6372  .    # 'async_cr
+00005570: 6561 746f 7227 2061 7267 756d 656e 7420  eator' argument 
+00005580: 746f 2027 6372 6561 7465 5f61 7379 6e63  to 'create_async
+00005590: 5f65 6e67 696e 6527 0a20 2020 2070 6f6f  _engine'.    poo
+000055a0: 6c20 3d20 6372 6561 7465 5f61 7379 6e63  l = create_async
+000055b0: 5f65 6e67 696e 6528 0a20 2020 2020 2020  _engine(.       
+000055c0: 2022 706f 7374 6772 6573 716c 2b61 7379   "postgresql+asy
+000055d0: 6e63 7067 3a2f 2f22 2c0a 2020 2020 2020  ncpg://",.      
+000055e0: 2020 6173 796e 635f 6372 6561 746f 723d    async_creator=
+000055f0: 6765 7463 6f6e 6e2c 0a20 2020 2029 0a20  getconn,.    ). 
+00005600: 2020 2072 6574 7572 6e20 706f 6f6c 0a0a     return pool..
+00005610: 6173 796e 6320 6465 6620 6d61 696e 2829  async def main()
+00005620: 3a0a 2020 2020 2320 696e 6974 6961 6c69  :.    # initiali
+00005630: 7a65 2043 6f6e 6e65 6374 6f72 206f 626a  ze Connector obj
+00005640: 6563 7420 666f 7220 636f 6e6e 6563 7469  ect for connecti
+00005650: 6f6e 7320 746f 2043 6c6f 7564 2053 514c  ons to Cloud SQL
+00005660: 0a20 2020 206c 6f6f 7020 3d20 6173 796e  .    loop = asyn
+00005670: 6369 6f2e 6765 745f 7275 6e6e 696e 675f  cio.get_running_
+00005680: 6c6f 6f70 2829 0a20 2020 2061 7379 6e63  loop().    async
+00005690: 2077 6974 6820 436f 6e6e 6563 746f 7228   with Connector(
+000056a0: 6c6f 6f70 3d6c 6f6f 7029 2061 7320 636f  loop=loop) as co
+000056b0: 6e6e 6563 746f 723a 0a20 2020 2020 2020  nnector:.       
+000056c0: 2023 2069 6e69 7469 616c 697a 6520 636f   # initialize co
+000056d0: 6e6e 6563 7469 6f6e 2070 6f6f 6c0a 2020  nnection pool.  
+000056e0: 2020 2020 2020 706f 6f6c 203d 2061 7761        pool = awa
+000056f0: 6974 2069 6e69 745f 636f 6e6e 6563 7469  it init_connecti
+00005700: 6f6e 5f70 6f6f 6c28 636f 6e6e 6563 746f  on_pool(connecto
+00005710: 7229 0a0a 2020 2020 2020 2020 2320 6578  r)..        # ex
+00005720: 616d 706c 6520 7175 6572 790a 2020 2020  ample query.    
+00005730: 2020 2020 6173 796e 6320 7769 7468 2070      async with p
+00005740: 6f6f 6c2e 636f 6e6e 6563 7428 2920 6173  ool.connect() as
+00005750: 2063 6f6e 6e3a 0a20 2020 2020 2020 2020   conn:.         
+00005760: 2020 2061 7761 6974 2063 6f6e 6e2e 6578     await conn.ex
+00005770: 6563 7574 6528 7371 6c61 6c63 6865 6d79  ecute(sqlalchemy
+00005780: 2e74 6578 7428 2253 454c 4543 5420 4e4f  .text("SELECT NO
+00005790: 5728 2922 2929 0a0a 2020 2020 2020 2020  W()"))..        
+000057a0: 2320 6469 7370 6f73 6520 6f66 2063 6f6e  # dispose of con
+000057b0: 6e65 6374 696f 6e20 706f 6f6c 0a20 2020  nection pool.   
+000057c0: 2020 2020 2061 7761 6974 2070 6f6f 6c2e       await pool.
+000057d0: 6469 7370 6f73 6528 290a 6060 600a 0a23  dispose().```..#
+000057e0: 2320 5375 7070 6f72 7420 706f 6c69 6379  # Support policy
+000057f0: 0a0a 2323 2320 4d61 6a6f 7220 7665 7273  ..### Major vers
+00005800: 696f 6e20 6c69 6665 6379 636c 650a 0a54  ion lifecycle..T
+00005810: 6869 7320 7072 6f6a 6563 7420 7573 6573  his project uses
+00005820: 205b 7365 6d61 6e74 6963 2076 6572 7369   [semantic versi
+00005830: 6f6e 696e 675d 2868 7474 7073 3a2f 2f73  oning](https://s
+00005840: 656d 7665 722e 6f72 672f 292c 2061 6e64  emver.org/), and
+00005850: 2075 7365 7320 7468 650a 666f 6c6c 6f77   uses the.follow
+00005860: 696e 6720 6c69 6665 6379 636c 6520 7265  ing lifecycle re
+00005870: 6761 7264 696e 6720 7375 7070 6f72 7420  garding support 
+00005880: 666f 7220 6120 6d61 6a6f 7220 7665 7273  for a major vers
+00005890: 696f 6e3a 0a0a 2a2a 4163 7469 7665 2a2a  ion:..**Active**
+000058a0: 202d 2041 6374 6976 6520 7665 7273 696f   - Active versio
+000058b0: 6e73 2067 6574 2061 6c6c 206e 6577 2066  ns get all new f
+000058c0: 6561 7475 7265 7320 616e 6420 7365 6375  eatures and secu
+000058d0: 7269 7479 2066 6978 6573 2028 7468 6174  rity fixes (that
+000058e0: 0a77 6f75 6c64 6ee2 8099 7420 6f74 6865  .wouldn...t othe
+000058f0: 7277 6973 6520 696e 7472 6f64 7563 6520  rwise introduce 
+00005900: 6120 6272 6561 6b69 6e67 2063 6861 6e67  a breaking chang
+00005910: 6529 2e20 4e65 7720 6d61 6a6f 7220 7665  e). New major ve
+00005920: 7273 696f 6e73 2061 7265 0a67 7561 7261  rsions are.guara
+00005930: 6e74 6565 6420 746f 2062 6520 2261 6374  nteed to be "act
+00005940: 6976 6522 2066 6f72 2061 206d 696e 696d  ive" for a minim
+00005950: 756d 206f 6620 3120 7965 6172 2e0a 2a2a  um of 1 year..**
+00005960: 4465 7072 6563 6174 6564 2a2a 202d 2044  Deprecated** - D
+00005970: 6570 7265 6361 7465 6420 7665 7273 696f  eprecated versio
+00005980: 6e73 2063 6f6e 7469 6e75 6520 746f 2072  ns continue to r
+00005990: 6563 6569 7665 2073 6563 7572 6974 7920  eceive security 
+000059a0: 616e 6420 6372 6974 6963 616c 0a62 7567  and critical.bug
+000059b0: 2066 6978 6573 2c20 6275 7420 646f 206e   fixes, but do n
+000059c0: 6f74 2072 6563 6569 7665 206e 6577 2066  ot receive new f
+000059d0: 6561 7475 7265 732e 2044 6570 7265 6361  eatures. Depreca
+000059e0: 7465 6420 7665 7273 696f 6e73 2077 696c  ted versions wil
+000059f0: 6c20 6265 2070 7562 6c69 636c 790a 7375  l be publicly.su
+00005a00: 7070 6f72 7465 6420 666f 7220 3120 7965  pported for 1 ye
+00005a10: 6172 2e0a 2a2a 556e 7375 7070 6f72 7465  ar..**Unsupporte
+00005a20: 642a 2a20 2d20 416e 7920 6d61 6a6f 7220  d** - Any major 
+00005a30: 7665 7273 696f 6e20 7468 6174 2068 6173  version that has
+00005a40: 2062 6565 6e20 6465 7072 6563 6174 6564   been deprecated
+00005a50: 2066 6f72 203e 3d31 2079 6561 7220 6973   for >=1 year is
+00005a60: 0a63 6f6e 7369 6465 7265 6420 7075 626c  .considered publ
+00005a70: 6963 6c79 2075 6e73 7570 706f 7274 6564  icly unsupported
+00005a80: 2e0a 0a23 2320 5375 7070 6f72 7465 6420  ...## Supported 
+00005a90: 5079 7468 6f6e 2056 6572 7369 6f6e 730a  Python Versions.
+00005aa0: 0a57 6520 666f 6c6c 6f77 2074 6865 205b  .We follow the [
+00005ab0: 5079 7468 6f6e 2056 6572 7369 6f6e 2053  Python Version S
+00005ac0: 7570 706f 7274 2050 6f6c 6963 795d 5b70  upport Policy][p
+00005ad0: 7976 6572 5d20 7573 6564 2062 7920 476f  yver] used by Go
+00005ae0: 6f67 6c65 2043 6c6f 7564 0a4c 6962 7261  ogle Cloud.Libra
+00005af0: 7269 6573 2066 6f72 2050 7974 686f 6e2e  ries for Python.
+00005b00: 2043 6861 6e67 6573 2069 6e20 7375 7070   Changes in supp
+00005b10: 6f72 7465 6420 5079 7468 6f6e 2076 6572  orted Python ver
+00005b20: 7369 6f6e 7320 7769 6c6c 2062 650a 636f  sions will be.co
+00005b30: 6e73 6964 6572 6564 2061 206d 696e 6f72  nsidered a minor
+00005b40: 2063 6861 6e67 652c 2061 6e64 2077 696c   change, and wil
+00005b50: 6c20 6265 206c 6973 7465 6420 696e 2074  l be listed in t
+00005b60: 6865 2072 656c 6561 7365 206e 6f74 6573  he release notes
+00005b70: 2e0a 0a5b 7079 7665 725d 3a20 6874 7470  ...[pyver]: http
+00005b80: 733a 2f2f 636c 6f75 642e 676f 6f67 6c65  s://cloud.google
+00005b90: 2e63 6f6d 2f70 7974 686f 6e2f 646f 6373  .com/python/docs
+00005ba0: 2f73 7570 706f 7274 6564 2d70 7974 686f  /supported-pytho
+00005bb0: 6e2d 7665 7273 696f 6e73 0a0a 2323 2320  n-versions..### 
+00005bc0: 5265 6c65 6173 6520 6361 6465 6e63 650a  Release cadence.
+00005bd0: 5468 6973 2070 726f 6a65 6374 2061 696d  This project aim
+00005be0: 7320 666f 7220 6120 6d69 6e69 6d75 6d20  s for a minimum 
+00005bf0: 6d6f 6e74 686c 7920 7265 6c65 6173 6520  monthly release 
+00005c00: 6361 6465 6e63 652e 2049 6620 6e6f 206e  cadence. If no n
+00005c10: 6577 0a66 6561 7475 7265 7320 6f72 2066  ew.features or f
+00005c20: 6978 6573 2068 6176 6520 6265 656e 2061  ixes have been a
+00005c30: 6464 6564 2c20 6120 6e65 7720 5041 5443  dded, a new PATC
+00005c40: 4820 7665 7273 696f 6e20 7769 7468 2074  H version with t
+00005c50: 6865 206c 6174 6573 740a 6465 7065 6e64  he latest.depend
+00005c60: 656e 6369 6573 2069 7320 7265 6c65 6173  encies is releas
+00005c70: 6564 2e0a 0a23 2323 2043 6f6e 7472 6962  ed...### Contrib
+00005c80: 7574 696e 670a 0a57 6520 7765 6c63 6f6d  uting..We welcom
+00005c90: 6520 6f75 7473 6964 6520 636f 6e74 7269  e outside contri
+00005ca0: 6275 7469 6f6e 732e 2050 6c65 6173 6520  butions. Please 
+00005cb0: 7365 6520 6f75 720a 5b43 6f6e 7472 6962  see our.[Contrib
+00005cc0: 7574 696e 6720 4775 6964 655d 2843 4f4e  uting Guide](CON
+00005cd0: 5452 4942 5554 494e 472e 6d64 2920 666f  TRIBUTING.md) fo
+00005ce0: 7220 6465 7461 696c 7320 6f6e 2068 6f77  r details on how
+00005cf0: 2062 6573 7420 746f 2063 6f6e 7472 6962   best to contrib
+00005d00: 7574 652e 0a                             ute..
```

### Comparing `cloud-sql-python-connector-1.2.4/cloud_sql_python_connector.egg-info/SOURCES.txt` & `cloud-sql-python-connector-1.3.0/cloud_sql_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.4/google/__init__.py` & `cloud-sql-python-connector-1.3.0/google/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.4/google/cloud/__init__.py` & `cloud-sql-python-connector-1.3.0/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/__init__.py` & `cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/asyncpg.py` & `cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/asyncpg.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/connector.py` & `cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,20 +14,24 @@
 limitations under the License.
 """
 from __future__ import annotations
 
 import asyncio
 from functools import partial
 import logging
+import socket
 from threading import Thread
 from types import TracebackType
 from typing import Any, Dict, Optional, Type, TYPE_CHECKING
 
 import google.cloud.sql.connector.asyncpg as asyncpg
-from google.cloud.sql.connector.exceptions import ConnectorLoopError
+from google.cloud.sql.connector.exceptions import (
+    ConnectorLoopError,
+    DnsNameResolutionError,
+)
 from google.cloud.sql.connector.instance import (
     Instance,
     IPTypes,
 )
 import google.cloud.sql.connector.pg8000 as pg8000
 import google.cloud.sql.connector.pymysql as pymysql
 import google.cloud.sql.connector.pytds as pytds
@@ -234,14 +238,29 @@
         kwargs.pop("host", None)
         kwargs.pop("ssl", None)
         kwargs.pop("port", None)
 
         # attempt to make connection to Cloud SQL instance
         try:
             instance_data, ip_address = await instance.connect_info(ip_type)
+            # resolve DNS name into IP address for PSC
+            if ip_type.value == "PSC":
+                addr_info = await self._loop.getaddrinfo(
+                    ip_address, None, family=socket.AF_INET, type=socket.SOCK_STREAM
+                )
+                # getaddrinfo returns a list of 5-tuples that contain socket
+                # connection info in the form
+                # (family, type, proto, canonname, sockaddr), where sockaddr is a
+                # 2-tuple in the form (ip_address, port)
+                try:
+                    ip_address = addr_info[0][4][0]
+                except IndexError as e:
+                    raise DnsNameResolutionError(
+                        f"['{instance_connection_string}']: DNS name could not be resolved into IP address"
+                    ) from e
 
             # format `user` param for automatic IAM database authn
             if enable_iam_auth:
                 formatted_user = format_database_user(
                     instance_data.database_version, kwargs["user"]
                 )
                 if formatted_user != kwargs["user"]:
```

### Comparing `cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/exceptions.py` & `cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,7 +59,14 @@
 class AutoIAMAuthNotSupported(Exception):
     """
     Exception to be raised when Automatic IAM Authentication is not
     supported with database engine version.
     """
 
     pass
+
+
+class DnsNameResolutionError(Exception):
+    """
+    Exception to be raised when the DnsName of a PSC connection to a
+    Cloud SQL instance can not be resolved to a proper IP address.
+    """
```

### Comparing `cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/instance.py` & `cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
 APPLICATION_NAME = "cloud-sql-python-connector"
 
 
 class IPTypes(Enum):
     PUBLIC: str = "PRIMARY"
     PRIVATE: str = "PRIVATE"
+    PSC: str = "PSC"
 
 
 class InstanceMetadata:
     ip_addrs: Dict[str, Any]
     context: ssl.SSLContext
     database_version: str
     expiration: datetime.datetime
```

### Comparing `cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/pg8000.py` & `cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/pg8000.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/pymysql.py` & `cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/pymysql.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/pytds.py` & `cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/pytds.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/rate_limiter.py` & `cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/refresh_utils.py` & `cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/refresh_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,24 @@
     ret_dict = await resp.json()
 
     if ret_dict["region"] != region:
         raise ValueError(
             f'[{project}:{region}:{instance}]: Provided region was mismatched - got region {region}, expected {ret_dict["region"]}.'
         )
 
+    ip_addresses = (
+        {ip["type"]: ip["ipAddress"] for ip in ret_dict["ipAddresses"]}
+        if "ipAddresses" in ret_dict
+        else {}
+    )
+    if "dnsName" in ret_dict:
+        ip_addresses["PSC"] = ret_dict["dnsName"]
+
     metadata = {
-        "ip_addresses": {ip["type"]: ip["ipAddress"] for ip in ret_dict["ipAddresses"]},
+        "ip_addresses": ip_addresses,
         "server_ca_cert": ret_dict["serverCaCert"]["cert"],
         "database_version": ret_dict["databaseVersion"],
     }
 
     return metadata
```

### Comparing `cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/utils.py` & `cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.4/google/cloud/sql/connector/version.py` & `cloud-sql-python-connector-1.3.0/google/cloud/sql/connector/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.2.4"
+__version__ = "1.3.0"
```

### Comparing `cloud-sql-python-connector-1.2.4/setup.py` & `cloud-sql-python-connector-1.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,27 +60,26 @@
     license="Apache 2.0",
     url="https://github.com/GoogleCloudPlatform/cloud-sql-python-connector",
     classifiers=[
         release_status,
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     platforms="Posix; MacOS X; Windows",
     packages=packages,
     namespace_packages=namespaces,
     install_requires=core_dependencies,
     extras_require={
-        "pymysql": ["PyMySQL==1.0.3"],
-        "pg8000": ["pg8000==1.29.6"],
+        "pymysql": ["PyMySQL==1.1.0"],
+        "pg8000": ["pg8000==1.29.8"],
         "pytds": ["python-tds==1.12.0"],
-        "asyncpg": ["asyncpg==0.27.0"]
+        "asyncpg": ["asyncpg==0.28.0"]
     },
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     include_package_data=True,
     zip_safe=False,
 )
```

