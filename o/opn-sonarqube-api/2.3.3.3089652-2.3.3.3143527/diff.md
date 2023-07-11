# Comparing `tmp/opn_sonarqube_api-2.3.3.3089652.tar.gz` & `tmp/opn_sonarqube_api-2.3.3.3143527.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opn_sonarqube_api-2.3.3.3089652.tar", last modified: Mon Jun 26 07:33:16 2023, max compression
+gzip compressed data, was "dist/opn_sonarqube_api-2.3.3.3143527.tar", last modified: Tue Jul 11 10:05:42 2023, max compression
```

## Comparing `opn_sonarqube_api-2.3.3.3089652.tar` & `opn_sonarqube_api-2.3.3.3143527.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/tests/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15993 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4135 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1128 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      208 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5918 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/DESCRIPTION.rst
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/
--rw-rw-rw-   0 root         (0) root         (0)      204 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3862 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/
--rw-rw-rw-   0 root         (0) root         (0)     3248 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/activate_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     5675 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/export_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     5331 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/migrate_rules.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18515 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonar.py
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/
--rw-rw-rw-   0 root         (0) root         (0)     7787 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/qualitygates.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/groups.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     3294 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/rules.py
--rw-rw-rw-   0 root         (0) root         (0)     6268 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/qualityprofiles.py
--rw-rw-rw-   0 root         (0) root         (0)     9702 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/users.py
--rw-rw-rw-   0 root         (0) root         (0)     1875 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/user_token.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/branches.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/components.py
--rw-rw-rw-   0 root         (0) root         (0)     4868 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/resources.py
--rw-rw-rw-   0 root         (0) root         (0)      764 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/projects.py
--rw-r--r--   0 root         (0) root         (0)     5918 2023-06-26 07:33:16.000000 opn_sonarqube_api-2.3.3.3089652/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-06-26 07:32:40.000000 opn_sonarqube_api-2.3.3.3089652/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:05:42.000000 opn_sonarqube_api-2.3.3.3143527/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 10:05:42.000000 opn_sonarqube_api-2.3.3.3143527/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:05:42.000000 opn_sonarqube_api-2.3.3.3143527/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15993 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/tests/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:05:42.000000 opn_sonarqube_api-2.3.3.3143527/opn_sonarqube_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-07-11 10:05:42.000000 opn_sonarqube_api-2.3.3.3143527/opn_sonarqube_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      208 2023-07-11 10:05:42.000000 opn_sonarqube_api-2.3.3.3143527/opn_sonarqube_api.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 10:05:42.000000 opn_sonarqube_api-2.3.3.3143527/opn_sonarqube_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-11 10:05:42.000000 opn_sonarqube_api-2.3.3.3143527/opn_sonarqube_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5918 2023-07-11 10:05:42.000000 opn_sonarqube_api-2.3.3.3143527/opn_sonarqube_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-11 10:05:42.000000 opn_sonarqube_api-2.3.3.3143527/opn_sonarqube_api.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/DESCRIPTION.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-07-11 10:05:41.000000 opn_sonarqube_api-2.3.3.3143527/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:05:42.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/
+-rw-rw-rw-   0 root         (0) root         (0)      204 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3862 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:05:42.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/cmd/
+-rw-rw-rw-   0 root         (0) root         (0)     3248 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/cmd/activate_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     5675 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/cmd/export_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     5331 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/cmd/migrate_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/cmd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18515 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonar.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 10:05:42.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/
+-rw-rw-rw-   0 root         (0) root         (0)     7787 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/qualitygates.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     3294 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     6274 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/qualityprofiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     9702 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/users.py
+-rw-rw-rw-   0 root         (0) root         (0)     1875 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/user_token.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/branches.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/components.py
+-rw-rw-rw-   0 root         (0) root         (0)     4868 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)      764 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/projects.py
+-rw-r--r--   0 root         (0) root         (0)     5918 2023-07-11 10:05:42.000000 opn_sonarqube_api-2.3.3.3143527/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-07-11 10:04:28.000000 opn_sonarqube_api-2.3.3.3143527/MANIFEST.in
```

### Comparing `opn_sonarqube_api-2.3.3.3089652/tests/test_api.py` & `opn_sonarqube_api-2.3.3.3143527/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/README.rst` & `opn_sonarqube_api-2.3.3.3143527/README.rst`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/SOURCES.txt` & `opn_sonarqube_api-2.3.3.3143527/opn_sonarqube_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/opn_sonarqube_api.egg-info/PKG-INFO` & `opn_sonarqube_api-2.3.3.3143527/opn_sonarqube_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: opn-sonarqube-api
-Version: 2.3.3.3089652
+Version: 2.3.3.3143527
 Summary: Open SonarQube API Handler
 Home-page: UNKNOWN
 Author: open sas
 Author-email: boost-support@open-groupe.com
 License: MIT
 Description: ====================
         Python SonarQube API
```

### Comparing `opn_sonarqube_api-2.3.3.3089652/setup.py` & `opn_sonarqube_api-2.3.3.3143527/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='opn_sonarqube_api',
 
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2.3.3.3089652',
+    version='2.3.3.3143527',
 
     description='Open SonarQube API Handler',
     long_description=long_description,
     author='open sas',
     author_email='boost-support@open-groupe.com',
     license='MIT',
```

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/api.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/api.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/activate_rules.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/cmd/activate_rules.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/export_rules.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/cmd/export_rules.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/cmd/migrate_rules.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/cmd/migrate_rules.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonar.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonar.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/qualitygates.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/qualitygates.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/groups.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/groups.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/metrics.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/metrics.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/authentication.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/authentication.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/rules.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/rules.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/qualityprofiles.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/qualityprofiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,20 +72,20 @@
         # Make call (might raise exception) and return
         res = self._api._get_call(self.SEARCH_QUALITY_PROFILE_ENDPOINT, params=combined)
         return res if res.status_code == 204 else json.loads(res.content)
 
     def delete_quality_profile(self, profile_name, language):
         """
 
-        :param profileName:
+        :param qualityProfile:
         :return:
         """
 
         data = {
-            'profileName': profile_name,
+            'qualityProfile': profile_name,
             'language': language
         }
 
         # Make call (return nothing)
         self._api._make_call('post', self.DELETE_QUALITY_PROFILE_ENDPOINT, data)
 
     def create_quality_profile(self, key, name, language, languagename,
```

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/permissions.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/permissions.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/settings.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/settings.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/user_token.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/user_token.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/branches.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/branches.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/components.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/components.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/resources.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/resources.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/sonarqube_api/sonarapi/projects.py` & `opn_sonarqube_api-2.3.3.3143527/sonarqube_api/sonarapi/projects.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.3.3.3089652/PKG-INFO` & `opn_sonarqube_api-2.3.3.3143527/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: opn_sonarqube_api
-Version: 2.3.3.3089652
+Version: 2.3.3.3143527
 Summary: Open SonarQube API Handler
 Home-page: UNKNOWN
 Author: open sas
 Author-email: boost-support@open-groupe.com
 License: MIT
 Description: ====================
         Python SonarQube API
```

