# Comparing `tmp/dbt-cratedb-1.5.2.tar.gz` & `tmp/dbt-cratedb-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-cratedb-1.5.2.tar", last modified: Mon Jul 10 21:03:18 2023, max compression
+gzip compressed data, was "dbt-cratedb-1.5.3.tar", last modified: Tue Jul 11 16:12:01 2023, max compression
```

## Comparing `dbt-cratedb-1.5.2.tar` & `dbt-cratedb-1.5.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.156522 dbt-cratedb-1.5.2/
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       46 2023-07-03 22:05:42.000000 dbt-cratedb-1.5.2/MANIFEST.in
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     1243 2023-07-10 21:03:18.156522 dbt-cratedb-1.5.2/PKG-INFO
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)      539 2023-07-03 23:13:55.000000 dbt-cratedb-1.5.2/README.md
-drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.152522 dbt-cratedb-1.5.2/dbt/
-drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.152522 dbt-cratedb-1.5.2/dbt/adapters/
-drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.152522 dbt-cratedb-1.5.2/dbt/adapters/cratedb/
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)      639 2023-07-10 20:50:03.000000 dbt-cratedb-1.5.2/dbt/adapters/cratedb/__init__.py
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       17 2023-07-03 22:53:10.000000 dbt-cratedb-1.5.2/dbt/adapters/cratedb/__version__.py
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       77 2023-07-04 19:23:08.000000 dbt-cratedb-1.5.2/dbt/adapters/cratedb/column.py
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     6025 2023-07-10 20:01:04.000000 dbt-cratedb-1.5.2/dbt/adapters/cratedb/connections.py
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     2971 2023-07-10 20:22:35.000000 dbt-cratedb-1.5.2/dbt/adapters/cratedb/impl.py
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)      259 2023-07-05 15:57:50.000000 dbt-cratedb-1.5.2/dbt/adapters/cratedb/relation.py
-drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.152522 dbt-cratedb-1.5.2/dbt/include/
-drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.152522 dbt-cratedb-1.5.2/dbt/include/cratedb/
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       52 2023-07-04 19:34:23.000000 dbt-cratedb-1.5.2/dbt/include/cratedb/__init__.py
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       77 2023-07-04 19:51:16.000000 dbt-cratedb-1.5.2/dbt/include/cratedb/dbt_project.yml
-drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.152522 dbt-cratedb-1.5.2/dbt/include/cratedb/macros/
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     3996 2023-07-10 19:57:54.000000 dbt-cratedb-1.5.2/dbt/include/cratedb/macros/adapters.sql
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     2814 2023-07-06 18:53:30.000000 dbt-cratedb-1.5.2/dbt/include/cratedb/macros/catalog.sql
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)      203 2023-07-03 22:53:10.000000 dbt-cratedb-1.5.2/dbt/include/cratedb/sample_profiles.yml
-drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-10 21:03:18.156522 dbt-cratedb-1.5.2/dbt_cratedb.egg-info/
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     1243 2023-07-10 21:03:18.000000 dbt-cratedb-1.5.2/dbt_cratedb.egg-info/PKG-INFO
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)      623 2023-07-10 21:03:18.000000 dbt-cratedb-1.5.2/dbt_cratedb.egg-info/SOURCES.txt
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)        1 2023-07-10 21:03:18.000000 dbt-cratedb-1.5.2/dbt_cratedb.egg-info/dependency_links.txt
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)        1 2023-07-04 19:58:52.000000 dbt-cratedb-1.5.2/dbt_cratedb.egg-info/not-zip-safe
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       30 2023-07-10 21:03:18.000000 dbt-cratedb-1.5.2/dbt_cratedb.egg-info/requires.txt
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)        4 2023-07-10 21:03:18.000000 dbt-cratedb-1.5.2/dbt_cratedb.egg-info/top_level.txt
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       38 2023-07-10 21:03:18.156522 dbt-cratedb-1.5.2/setup.cfg
--rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     2436 2023-07-10 20:50:52.000000 dbt-cratedb-1.5.2/setup.py
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-11 16:12:01.022060 dbt-cratedb-1.5.3/
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       46 2023-07-03 22:05:42.000000 dbt-cratedb-1.5.3/MANIFEST.in
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     1243 2023-07-11 16:12:01.022060 dbt-cratedb-1.5.3/PKG-INFO
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)      539 2023-07-03 23:13:55.000000 dbt-cratedb-1.5.3/README.md
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-11 16:12:01.022060 dbt-cratedb-1.5.3/dbt/
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-11 16:12:01.022060 dbt-cratedb-1.5.3/dbt/adapters/
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-11 16:12:01.022060 dbt-cratedb-1.5.3/dbt/adapters/cratedb/
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)      639 2023-07-10 20:50:03.000000 dbt-cratedb-1.5.3/dbt/adapters/cratedb/__init__.py
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       18 2023-07-11 16:11:16.000000 dbt-cratedb-1.5.3/dbt/adapters/cratedb/__version__.py
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       77 2023-07-04 19:23:08.000000 dbt-cratedb-1.5.3/dbt/adapters/cratedb/column.py
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     6025 2023-07-10 20:01:04.000000 dbt-cratedb-1.5.3/dbt/adapters/cratedb/connections.py
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     2971 2023-07-10 20:22:35.000000 dbt-cratedb-1.5.3/dbt/adapters/cratedb/impl.py
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)      259 2023-07-05 15:57:50.000000 dbt-cratedb-1.5.3/dbt/adapters/cratedb/relation.py
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-11 16:12:01.022060 dbt-cratedb-1.5.3/dbt/include/
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-11 16:12:01.022060 dbt-cratedb-1.5.3/dbt/include/cratedb/
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       52 2023-07-04 19:34:23.000000 dbt-cratedb-1.5.3/dbt/include/cratedb/__init__.py
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       77 2023-07-04 19:51:16.000000 dbt-cratedb-1.5.3/dbt/include/cratedb/dbt_project.yml
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-11 16:12:01.022060 dbt-cratedb-1.5.3/dbt/include/cratedb/macros/
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     3996 2023-07-10 19:57:54.000000 dbt-cratedb-1.5.3/dbt/include/cratedb/macros/adapters.sql
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     2771 2023-07-10 21:26:10.000000 dbt-cratedb-1.5.3/dbt/include/cratedb/macros/catalog.sql
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)      355 2023-07-11 16:02:24.000000 dbt-cratedb-1.5.3/dbt/include/cratedb/sample_profiles.yml
+drwxrwxr-x   0 aymaru    (1000) aymaru    (1000)        0 2023-07-11 16:12:01.022060 dbt-cratedb-1.5.3/dbt_cratedb.egg-info/
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     1243 2023-07-11 16:12:01.000000 dbt-cratedb-1.5.3/dbt_cratedb.egg-info/PKG-INFO
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)      623 2023-07-11 16:12:01.000000 dbt-cratedb-1.5.3/dbt_cratedb.egg-info/SOURCES.txt
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)        1 2023-07-11 16:12:01.000000 dbt-cratedb-1.5.3/dbt_cratedb.egg-info/dependency_links.txt
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)        1 2023-07-04 19:58:52.000000 dbt-cratedb-1.5.3/dbt_cratedb.egg-info/not-zip-safe
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       30 2023-07-11 16:12:01.000000 dbt-cratedb-1.5.3/dbt_cratedb.egg-info/requires.txt
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)        4 2023-07-11 16:12:01.000000 dbt-cratedb-1.5.3/dbt_cratedb.egg-info/top_level.txt
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)       38 2023-07-11 16:12:01.022060 dbt-cratedb-1.5.3/setup.cfg
+-rw-rw-r--   0 aymaru    (1000) aymaru    (1000)     2436 2023-07-10 20:50:52.000000 dbt-cratedb-1.5.3/setup.py
```

### Comparing `dbt-cratedb-1.5.2/PKG-INFO` & `dbt-cratedb-1.5.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-cratedb
-Version: 1.5.2
+Version: 1.5.3
 Summary: The crate adapter plugin for dbt (data build tool)
 Home-page: 
 Author: Smartnow
 Author-email: julio@smartnow.la
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-cratedb-1.5.2/README.md` & `dbt-cratedb-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-cratedb-1.5.2/dbt/adapters/cratedb/__init__.py` & `dbt-cratedb-1.5.3/dbt/adapters/cratedb/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-cratedb-1.5.2/dbt/adapters/cratedb/connections.py` & `dbt-cratedb-1.5.3/dbt/adapters/cratedb/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-cratedb-1.5.2/dbt/adapters/cratedb/impl.py` & `dbt-cratedb-1.5.3/dbt/adapters/cratedb/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-cratedb-1.5.2/dbt/include/cratedb/macros/adapters.sql` & `dbt-cratedb-1.5.3/dbt/include/cratedb/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-cratedb-1.5.2/dbt/include/cratedb/macros/catalog.sql` & `dbt-cratedb-1.5.3/dbt/include/cratedb/macros/catalog.sql`

 * *Files 8% similar despite different names*

```diff
@@ -22,18 +22,17 @@
   {% endcall %}
 {% endmacro %}
 
 {% macro cratedb__get_catalog(information_schema, schemas) -%}
 
   {%- call statement('catalog', fetch_result=True) -%}
     {% set database = information_schema.database %}
-    {{ adapter.verify_database(database) }}
 
     select
-    '{{ database }}' as table_database
+    '{{ database }}' as table_database,
     sch.nspname as table_schema,
     tbl.relname as table_name,
     case tbl.relkind
         when 'v' then 'VIEW'
         else 'BASE TABLE'
     end as table_type,
     tbl_desc.description as table_comment,
```

### Comparing `dbt-cratedb-1.5.2/dbt_cratedb.egg-info/PKG-INFO` & `dbt-cratedb-1.5.3/dbt_cratedb.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-cratedb
-Version: 1.5.2
+Version: 1.5.3
 Summary: The crate adapter plugin for dbt (data build tool)
 Home-page: 
 Author: Smartnow
 Author-email: julio@smartnow.la
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-cratedb-1.5.2/dbt_cratedb.egg-info/SOURCES.txt` & `dbt-cratedb-1.5.3/dbt_cratedb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-cratedb-1.5.2/setup.py` & `dbt-cratedb-1.5.3/setup.py`

 * *Files identical despite different names*

