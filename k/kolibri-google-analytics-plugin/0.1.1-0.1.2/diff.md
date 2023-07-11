# Comparing `tmp/kolibri_google_analytics_plugin-0.1.1.tar.gz` & `tmp/kolibri_google_analytics_plugin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolibri_google_analytics_plugin-0.1.1.tar", last modified: Fri Jun  9 18:10:57 2023, max compression
+gzip compressed data, was "kolibri_google_analytics_plugin-0.1.2.tar", last modified: Tue Jul 11 12:52:56 2023, max compression
```

## Comparing `kolibri_google_analytics_plugin-0.1.1.tar` & `kolibri_google_analytics_plugin-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-09 18:10:57.812943 kolibri_google_analytics_plugin-0.1.1/
--rw-rw-r--   0 philip    (1000) philip    (1000)     1092 2023-06-09 13:50:47.000000 kolibri_google_analytics_plugin-0.1.1/LICENSE
--rw-rw-r--   0 philip    (1000) philip    (1000)      365 2023-06-09 18:08:58.000000 kolibri_google_analytics_plugin-0.1.1/MANIFEST.in
--rw-r--r--   0 philip    (1000) philip    (1000)      979 2023-06-09 18:10:57.812943 kolibri_google_analytics_plugin-0.1.1/PKG-INFO
--rw-rw-r--   0 philip    (1000) philip    (1000)     1238 2023-06-09 16:58:21.000000 kolibri_google_analytics_plugin-0.1.1/README.rst
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-09 18:10:57.811943 kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin/
--rw-rw-r--   0 philip    (1000) philip    (1000)       22 2023-06-09 18:10:28.000000 kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin/__init__.py
--rw-rw-r--   0 philip    (1000) philip    (1000)     1343 2023-06-09 16:27:55.000000 kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin/kolibri_plugin.py
--rw-rw-r--   0 philip    (1000) philip    (1000)      352 2023-06-09 16:32:04.000000 kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin/options.py
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-09 18:10:57.812943 kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin/templates/
--rw-r--r--   0 philip    (1000) philip    (1000)      379 2023-06-09 16:31:08.000000 kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin/templates/head_snippet.html
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-06-09 18:10:57.812943 kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin.egg-info/
--rw-r--r--   0 philip    (1000) philip    (1000)      979 2023-06-09 18:10:57.000000 kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin.egg-info/PKG-INFO
--rw-r--r--   0 philip    (1000) philip    (1000)      568 2023-06-09 18:10:57.000000 kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 philip    (1000) philip    (1000)        1 2023-06-09 18:10:57.000000 kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 philip    (1000) philip    (1000)       84 2023-06-09 18:10:57.000000 kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin.egg-info/entry_points.txt
--rw-r--r--   0 philip    (1000) philip    (1000)        1 2023-06-09 18:10:57.000000 kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin.egg-info/not-zip-safe
--rw-r--r--   0 philip    (1000) philip    (1000)       32 2023-06-09 18:10:57.000000 kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin.egg-info/top_level.txt
--rw-r--r--   0 philip    (1000) philip    (1000)       38 2023-06-09 18:10:57.812943 kolibri_google_analytics_plugin-0.1.1/setup.cfg
--rw-rw-r--   0 philip    (1000) philip    (1000)     1766 2023-06-09 17:04:01.000000 kolibri_google_analytics_plugin-0.1.1/setup.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 12:52:56.529790 kolibri_google_analytics_plugin-0.1.2/
+-rw-rw-r--   0 philip    (1000) philip    (1000)     1092 2023-06-09 13:50:47.000000 kolibri_google_analytics_plugin-0.1.2/LICENSE
+-rw-rw-r--   0 philip    (1000) philip    (1000)      365 2023-06-09 18:08:58.000000 kolibri_google_analytics_plugin-0.1.2/MANIFEST.in
+-rw-r--r--   0 philip    (1000) philip    (1000)      979 2023-07-11 12:52:56.529790 kolibri_google_analytics_plugin-0.1.2/PKG-INFO
+-rw-rw-r--   0 philip    (1000) philip    (1000)     1238 2023-06-09 16:58:21.000000 kolibri_google_analytics_plugin-0.1.2/README.rst
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 12:52:56.528790 kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin/
+-rw-rw-r--   0 philip    (1000) philip    (1000)       22 2023-07-11 12:51:32.000000 kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin/__init__.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     1325 2023-07-11 12:49:09.000000 kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin/kolibri_plugin.py
+-rw-rw-r--   0 philip    (1000) philip    (1000)      352 2023-06-09 16:32:04.000000 kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin/options.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 12:52:56.527790 kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin/templates/
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 12:52:56.528790 kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin/templates/google_analytics/
+-rw-r--r--   0 philip    (1000) philip    (1000)      379 2023-07-11 12:49:09.000000 kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin/templates/google_analytics/head_snippet.html
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2023-07-11 12:52:56.528790 kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin.egg-info/
+-rw-r--r--   0 philip    (1000) philip    (1000)      979 2023-07-11 12:52:56.000000 kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 philip    (1000) philip    (1000)      585 2023-07-11 12:52:56.000000 kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)        1 2023-07-11 12:52:56.000000 kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)       84 2023-07-11 12:52:56.000000 kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)        1 2023-07-11 12:52:56.000000 kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 philip    (1000) philip    (1000)       32 2023-07-11 12:52:56.000000 kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin.egg-info/top_level.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)       38 2023-07-11 12:52:56.529790 kolibri_google_analytics_plugin-0.1.2/setup.cfg
+-rw-rw-r--   0 philip    (1000) philip    (1000)     1766 2023-06-09 17:04:01.000000 kolibri_google_analytics_plugin-0.1.2/setup.py
```

### Comparing `kolibri_google_analytics_plugin-0.1.1/LICENSE` & `kolibri_google_analytics_plugin-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kolibri_google_analytics_plugin-0.1.1/PKG-INFO` & `kolibri_google_analytics_plugin-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolibri_google_analytics_plugin
-Version: 0.1.1
+Version: 0.1.2
 Summary: A plugin to provide Google Analytics support for Kolibri
 Home-page: https://github.com/endlessm/kolibri-google-analytics-plugin
 Author: Endless OS Foundation
 Author-email: maintainers@endlessos.org
 License: MIT
 Keywords: kolibri
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kolibri_google_analytics_plugin-0.1.1/README.rst` & `kolibri_google_analytics_plugin-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin/kolibri_plugin.py` & `kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin/kolibri_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     @property
     def head_html(self):
         measurement_id = conf.OPTIONS["GoogleAnalytics"]["MEASUREMENT_ID"]
         if not measurement_id:
             logger.info("Google Analytics support enabled but MEASUREMENT_ID not set in options")
             return ""
 
-        return render_to_string("head_snippet.html", {
-            "measurement_id": conf.OPTIONS["GoogleAnalytics"]["MEASUREMENT_ID"],
+        return render_to_string("google_analytics/head_snippet.html", {
+            "measurement_id": measurement_id,
         })
```

### Comparing `kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin.egg-info/PKG-INFO` & `kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolibri-google-analytics-plugin
-Version: 0.1.1
+Version: 0.1.2
 Summary: A plugin to provide Google Analytics support for Kolibri
 Home-page: https://github.com/endlessm/kolibri-google-analytics-plugin
 Author: Endless OS Foundation
 Author-email: maintainers@endlessos.org
 License: MIT
 Keywords: kolibri
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kolibri_google_analytics_plugin-0.1.1/kolibri_google_analytics_plugin.egg-info/SOURCES.txt` & `kolibri_google_analytics_plugin-0.1.2/kolibri_google_analytics_plugin.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 kolibri_google_analytics_plugin/options.py
 kolibri_google_analytics_plugin.egg-info/PKG-INFO
 kolibri_google_analytics_plugin.egg-info/SOURCES.txt
 kolibri_google_analytics_plugin.egg-info/dependency_links.txt
 kolibri_google_analytics_plugin.egg-info/entry_points.txt
 kolibri_google_analytics_plugin.egg-info/not-zip-safe
 kolibri_google_analytics_plugin.egg-info/top_level.txt
-kolibri_google_analytics_plugin/templates/head_snippet.html
+kolibri_google_analytics_plugin/templates/google_analytics/head_snippet.html
```

### Comparing `kolibri_google_analytics_plugin-0.1.1/setup.py` & `kolibri_google_analytics_plugin-0.1.2/setup.py`

 * *Files identical despite different names*

