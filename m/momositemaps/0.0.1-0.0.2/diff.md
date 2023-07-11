# Comparing `tmp/momositemaps-0.0.1.tar.gz` & `tmp/momositemaps-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\momositemaps-0.0.1.tar", last modified: Tue Jul 11 13:41:49 2023, max compression
+gzip compressed data, was "dist\momositemaps-0.0.2.tar", last modified: Tue Jul 11 13:56:48 2023, max compression
```

## Comparing `momositemaps-0.0.1.tar` & `momositemaps-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 13:41:49.784876 momositemaps-0.0.1/
--rw-rw-rw-   0        0        0      548 2023-07-11 13:41:49.778791 momositemaps-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 13:41:49.758993 momositemaps-0.0.1/momositemaps/
--rw-rw-rw-   0        0        0     3780 2023-07-11 13:38:54.000000 momositemaps-0.0.1/momositemaps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 13:41:49.776781 momositemaps-0.0.1/momositemaps.egg-info/
--rw-rw-rw-   0        0        0      548 2023-07-11 13:41:49.000000 momositemaps-0.0.1/momositemaps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-07-11 13:41:49.000000 momositemaps-0.0.1/momositemaps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 13:41:49.000000 momositemaps-0.0.1/momositemaps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-11 13:41:49.000000 momositemaps-0.0.1/momositemaps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-11 13:41:49.000000 momositemaps-0.0.1/momositemaps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 13:41:49.786014 momositemaps-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      856 2023-07-11 13:25:14.000000 momositemaps-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:56:48.843482 momositemaps-0.0.2/
+-rw-rw-rw-   0        0        0      548 2023-07-11 13:56:48.840750 momositemaps-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-11 13:56:48.819490 momositemaps-0.0.2/momositemaps/
+-rw-rw-rw-   0        0        0     4073 2023-07-11 13:56:16.000000 momositemaps-0.0.2/momositemaps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:56:48.838604 momositemaps-0.0.2/momositemaps.egg-info/
+-rw-rw-rw-   0        0        0      548 2023-07-11 13:56:48.000000 momositemaps-0.0.2/momositemaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-07-11 13:56:48.000000 momositemaps-0.0.2/momositemaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 13:56:48.000000 momositemaps-0.0.2/momositemaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-11 13:56:48.000000 momositemaps-0.0.2/momositemaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-11 13:56:48.000000 momositemaps-0.0.2/momositemaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 13:56:48.844457 momositemaps-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      856 2023-07-11 13:56:16.000000 momositemaps-0.0.2/setup.py
```

### Comparing `momositemaps-0.0.1/PKG-INFO` & `momositemaps-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momositemaps
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sitemap Builder
 Author: Momo Sitemaps
 Author-email: <momo@cleardex.io>
 Keywords: python,sitemap builder,seo,sitemaps,link indexer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `momositemaps-0.0.1/momositemaps/__init__.py` & `momositemaps-0.0.2/momositemaps/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -52,34 +52,37 @@
         database= database
     )
     mycursor = mydb.cursor()
     mycursor.execute("SELECT COUNT(*) FROM yourls_url")
     result = mycursor.fetchone()
     row_count = result[0]
     numberToDo = row_count/5000
-    print("Sitemaps to make: " + str(row_count))
+    print("Links in database: " + str(row_count))
     print("Sitemaps to make: " + str(numberToDo))
     x = 1
+    print("Creating sitemaps. This may take some time depending on the number needed")
     while x - 1 < numberToDo:
         mycursor = mydb.cursor()
         offset = (x-1) * 5000
         mycursor.execute("SELECT * FROM yourls_url LIMIT 5000 OFFSET " + str(offset))
         myresult = mycursor.fetchall()
         with open("sitemap_" + str(x) + ".xml", 'w') as fp:
             fp.writelines('<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">')
             for link in myresult:
                 fp.writelines('<url>')
-                fp.writelines('<loc>https://' + domain + 'cleardex.io/' + str(link[0].decode()) + '</loc>')
+                fp.writelines('<loc>https://' + domain + '/' + str(link[0].decode()) + '</loc>')
                 fp.writelines('<lastmod>2023-07-08T15:15:27+00:00</lastmod>')
                 fp.writelines('<changefreq>Daily</changefreq>')
                 fp.writelines('<priority>0.9</priority>')
                 fp.writelines('</url>')
 
             fp.writelines('</urlset>')
+            print("Number of sitemaps created so far: " + str(x))
         x = x + 1
+    print("Created " + str(x) + " sitemaps. Now will create the index of the sitemaps, sitemap_index.xml. This is the file to submit to IndexNow")
     x = 1
     with open("sitemap_index.xml", 'w') as fp:
         fp.writelines('<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">')
         while x - 1 < numberToDo:
             fp.writelines('<url>')
             fp.writelines('<loc>https://' + domain + '/' + directory +'/sitemap_' + str(x) + '.xml</loc>')
             fp.writelines('<lastmod>2023-07-08T15:15:27+00:00</lastmod>')
```

### Comparing `momositemaps-0.0.1/momositemaps.egg-info/PKG-INFO` & `momositemaps-0.0.2/momositemaps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momositemaps
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sitemap Builder
 Author: Momo Sitemaps
 Author-email: <momo@cleardex.io>
 Keywords: python,sitemap builder,seo,sitemaps,link indexer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `momositemaps-0.0.1/setup.py` & `momositemaps-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Sitemap Builder'
 LONG_DESCRIPTION = 'A free sitemap builder to handle millions of links.'
 
 # Setup Parameters
 setup(
     name="momositemaps",
     version=VERSION,
```

