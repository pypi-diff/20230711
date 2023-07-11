# Comparing `tmp/peek-office-service-3.4.7.tar.gz` & `tmp/peek-office-service-3.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-office-service-3.4.7.tar", last modified: Mon Jul  3 08:33:54 2023, max compression
+gzip compressed data, was "peek-office-service-3.4.8.tar", last modified: Tue Jul 11 02:52:59 2023, max compression
```

## Comparing `peek-office-service-3.4.7.tar` & `peek-office-service-3.4.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:33:54.975247 peek-office-service-3.4.7/
--rw-r--r--   0 root         (0) root         (0)      377 2023-07-03 08:33:54.975247 peek-office-service-3.4.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      246 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:33:54.974247 peek-office-service-3.4.7/peek_office_service/
--rw-r--r--   0 root         (0) root         (0)     1508 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/PeekClientConfig.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/PeekClientConfigTest.py
--rw-r--r--   0 root         (0) root         (0)      460 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-07-03 08:33:54.000000 peek-office-service-3.4.7/peek_office_service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:33:54.974247 peek-office-service-3.4.7/peek_office_service/backend/
--rw-r--r--   0 root         (0) root         (0)      450 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/backend/ClientObservable.py
--rw-r--r--   0 root         (0) root         (0)     2251 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/backend/SiteRootResource.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:33:54.974247 peek-office-service-3.4.7/peek_office_service/plugin/
--rw-r--r--   0 root         (0) root         (0)     1587 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/plugin/ClientFrontendBuildersMixin.py
--rw-r--r--   0 root         (0) root         (0)     2790 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/plugin/ClientPluginLoader.py
--rw-r--r--   0 root         (0) root         (0)     1629 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/plugin/ClientPluginLoaderTest.py
--rw-r--r--   0 root         (0) root         (0)     3107 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/plugin/PeekClientPlatformHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3919 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/run_peek_office_service.py
--rw-r--r--   0 root         (0) root         (0)     4000 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/run_peek_office_service_build_only.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:33:54.974247 peek-office-service-3.4.7/peek_office_service/sw_install/
--rw-r--r--   0 root         (0) root         (0)      792 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/sw_install/PeekSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/sw_install/PluginSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/sw_install/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1412 2023-07-03 08:32:06.000000 peek-office-service-3.4.7/peek_office_service/winsvc_peek_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:33:54.974247 peek-office-service-3.4.7/peek_office_service.egg-info/
--rw-r--r--   0 root         (0) root         (0)      377 2023-07-03 08:33:54.000000 peek-office-service-3.4.7/peek_office_service.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1173 2023-07-03 08:33:54.000000 peek-office-service-3.4.7/peek_office_service.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 08:33:54.000000 peek-office-service-3.4.7/peek_office_service.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      272 2023-07-03 08:33:54.000000 peek-office-service-3.4.7/peek_office_service.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 08:33:54.000000 peek-office-service-3.4.7/peek_office_service.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      123 2023-07-03 08:33:54.000000 peek-office-service-3.4.7/peek_office_service.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-03 08:33:54.000000 peek-office-service-3.4.7/peek_office_service.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 08:33:54.975247 peek-office-service-3.4.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3117 2023-07-03 08:33:54.000000 peek-office-service-3.4.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:59.046999 peek-office-service-3.4.8/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-07-11 02:52:59.046999 peek-office-service-3.4.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      246 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:59.045998 peek-office-service-3.4.8/peek_office_service/
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/PeekClientConfig.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/PeekClientConfigTest.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-07-11 02:52:58.000000 peek-office-service-3.4.8/peek_office_service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:59.045998 peek-office-service-3.4.8/peek_office_service/backend/
+-rw-r--r--   0 root         (0) root         (0)      450 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/backend/ClientObservable.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/backend/SiteRootResource.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:59.045998 peek-office-service-3.4.8/peek_office_service/plugin/
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/plugin/ClientFrontendBuildersMixin.py
+-rw-r--r--   0 root         (0) root         (0)     2790 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/plugin/ClientPluginLoader.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/plugin/ClientPluginLoaderTest.py
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/plugin/PeekClientPlatformHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3919 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/run_peek_office_service.py
+-rw-r--r--   0 root         (0) root         (0)     4000 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/run_peek_office_service_build_only.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:59.045998 peek-office-service-3.4.8/peek_office_service/sw_install/
+-rw-r--r--   0 root         (0) root         (0)      792 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/sw_install/PeekSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/sw_install/PluginSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/sw_install/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1412 2023-07-11 02:51:11.000000 peek-office-service-3.4.8/peek_office_service/winsvc_peek_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:59.045998 peek-office-service-3.4.8/peek_office_service.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-07-11 02:52:59.000000 peek-office-service-3.4.8/peek_office_service.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-07-11 02:52:59.000000 peek-office-service-3.4.8/peek_office_service.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:52:59.000000 peek-office-service-3.4.8/peek_office_service.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-11 02:52:59.000000 peek-office-service-3.4.8/peek_office_service.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:52:59.000000 peek-office-service-3.4.8/peek_office_service.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      123 2023-07-11 02:52:59.000000 peek-office-service-3.4.8/peek_office_service.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-11 02:52:59.000000 peek-office-service-3.4.8/peek_office_service.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 02:52:59.046999 peek-office-service-3.4.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3117 2023-07-11 02:52:58.000000 peek-office-service-3.4.8/setup.py
```

### Comparing `peek-office-service-3.4.7/peek_office_service/PeekClientConfig.py` & `peek-office-service-3.4.8/peek_office_service/PeekClientConfig.py`

 * *Files identical despite different names*

### Comparing `peek-office-service-3.4.7/peek_office_service/PeekClientConfigTest.py` & `peek-office-service-3.4.8/peek_office_service/PeekClientConfigTest.py`

 * *Files identical despite different names*

### Comparing `peek-office-service-3.4.7/peek_office_service/backend/SiteRootResource.py` & `peek-office-service-3.4.8/peek_office_service/backend/SiteRootResource.py`

 * *Files identical despite different names*

### Comparing `peek-office-service-3.4.7/peek_office_service/plugin/ClientFrontendBuildersMixin.py` & `peek-office-service-3.4.8/peek_office_service/plugin/ClientFrontendBuildersMixin.py`

 * *Files identical despite different names*

### Comparing `peek-office-service-3.4.7/peek_office_service/plugin/ClientPluginLoader.py` & `peek-office-service-3.4.8/peek_office_service/plugin/ClientPluginLoader.py`

 * *Files identical despite different names*

### Comparing `peek-office-service-3.4.7/peek_office_service/plugin/ClientPluginLoaderTest.py` & `peek-office-service-3.4.8/peek_office_service/plugin/ClientPluginLoaderTest.py`

 * *Files identical despite different names*

### Comparing `peek-office-service-3.4.7/peek_office_service/plugin/PeekClientPlatformHook.py` & `peek-office-service-3.4.8/peek_office_service/plugin/PeekClientPlatformHook.py`

 * *Files identical despite different names*

### Comparing `peek-office-service-3.4.7/peek_office_service/run_peek_office_service.py` & `peek-office-service-3.4.8/peek_office_service/run_peek_office_service.py`

 * *Files identical despite different names*

### Comparing `peek-office-service-3.4.7/peek_office_service/run_peek_office_service_build_only.py` & `peek-office-service-3.4.8/peek_office_service/run_peek_office_service_build_only.py`

 * *Files identical despite different names*

### Comparing `peek-office-service-3.4.7/peek_office_service/sw_install/PeekSwInstallManager.py` & `peek-office-service-3.4.8/peek_office_service/sw_install/PeekSwInstallManager.py`

 * *Files identical despite different names*

### Comparing `peek-office-service-3.4.7/peek_office_service/winsvc_peek_client.py` & `peek-office-service-3.4.8/peek_office_service/winsvc_peek_client.py`

 * *Files identical despite different names*

### Comparing `peek-office-service-3.4.7/peek_office_service.egg-info/SOURCES.txt` & `peek-office-service-3.4.8/peek_office_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-office-service-3.4.7/setup.py` & `peek-office-service-3.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_office_service"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.7"
+package_version = "3.4.8"
 description = "Peek Office Service."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

