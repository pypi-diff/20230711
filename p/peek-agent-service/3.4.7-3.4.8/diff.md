# Comparing `tmp/peek-agent-service-3.4.7.tar.gz` & `tmp/peek-agent-service-3.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-agent-service-3.4.7.tar", last modified: Mon Jul  3 08:32:50 2023, max compression
+gzip compressed data, was "peek-agent-service-3.4.8.tar", last modified: Tue Jul 11 02:51:55 2023, max compression
```

## Comparing `peek-agent-service-3.4.7.tar` & `peek-agent-service-3.4.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:32:50.508086 peek-agent-service-3.4.7/
--rw-r--r--   0 root         (0) root         (0)      373 2023-07-03 08:32:50.508086 peek-agent-service-3.4.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      239 2023-07-03 08:32:05.000000 peek-agent-service-3.4.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:32:50.507085 peek-agent-service-3.4.7/peek_agent_service/
--rw-r--r--   0 root         (0) root         (0)     1047 2023-07-03 08:32:05.000000 peek-agent-service-3.4.7/peek_agent_service/PeekAgentConfig.py
--rw-r--r--   0 root         (0) root         (0)     1305 2023-07-03 08:32:05.000000 peek-agent-service-3.4.7/peek_agent_service/PeekAgentConfigTest.py
--rw-r--r--   0 root         (0) root         (0)      460 2023-07-03 08:32:05.000000 peek-agent-service-3.4.7/peek_agent_service/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)       68 2023-07-03 08:32:50.000000 peek-agent-service-3.4.7/peek_agent_service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:32:50.507085 peek-agent-service-3.4.7/peek_agent_service/plugin/
--rw-r--r--   0 root         (0) root         (0)     1629 2023-07-03 08:32:05.000000 peek-agent-service-3.4.7/peek_agent_service/plugin/AgentPluginLoader.py
--rw-r--r--   0 root         (0) root         (0)     1615 2023-07-03 08:32:05.000000 peek-agent-service-3.4.7/peek_agent_service/plugin/AgentPluginLoaderTest.py
--rw-r--r--   0 root         (0) root         (0)     2476 2023-07-03 08:32:05.000000 peek-agent-service-3.4.7/peek_agent_service/plugin/PeekAgentPlatformHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 08:32:05.000000 peek-agent-service-3.4.7/peek_agent_service/plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7053 2023-07-03 08:32:05.000000 peek-agent-service-3.4.7/peek_agent_service/run_peek_agent_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:32:50.508086 peek-agent-service-3.4.7/peek_agent_service/sw_install/
--rw-r--r--   0 root         (0) root         (0)      790 2023-07-03 08:32:05.000000 peek-agent-service-3.4.7/peek_agent_service/sw_install/PeekSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-07-03 08:32:05.000000 peek-agent-service-3.4.7/peek_agent_service/sw_install/PluginSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-07-03 08:32:05.000000 peek-agent-service-3.4.7/peek_agent_service/sw_install/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1419 2023-07-03 08:32:05.000000 peek-agent-service-3.4.7/peek_agent_service/winsvc_peek_agent_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 08:32:50.507085 peek-agent-service-3.4.7/peek_agent_service.egg-info/
--rw-r--r--   0 root         (0) root         (0)      373 2023-07-03 08:32:50.000000 peek-agent-service-3.4.7/peek_agent_service.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      902 2023-07-03 08:32:50.000000 peek-agent-service-3.4.7/peek_agent_service.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 08:32:50.000000 peek-agent-service-3.4.7/peek_agent_service.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      169 2023-07-03 08:32:50.000000 peek-agent-service-3.4.7/peek_agent_service.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 08:32:50.000000 peek-agent-service-3.4.7/peek_agent_service.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-03 08:32:50.000000 peek-agent-service-3.4.7/peek_agent_service.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-03 08:32:50.000000 peek-agent-service-3.4.7/peek_agent_service.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 08:32:50.508086 peek-agent-service-3.4.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2940 2023-07-03 08:32:50.000000 peek-agent-service-3.4.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:51:55.679118 peek-agent-service-3.4.8/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-07-11 02:51:55.679118 peek-agent-service-3.4.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      239 2023-07-11 02:51:10.000000 peek-agent-service-3.4.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:51:55.678118 peek-agent-service-3.4.8/peek_agent_service/
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-07-11 02:51:10.000000 peek-agent-service-3.4.8/peek_agent_service/PeekAgentConfig.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-07-11 02:51:10.000000 peek-agent-service-3.4.8/peek_agent_service/PeekAgentConfigTest.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-11 02:51:10.000000 peek-agent-service-3.4.8/peek_agent_service/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)       68 2023-07-11 02:51:55.000000 peek-agent-service-3.4.8/peek_agent_service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:51:55.678118 peek-agent-service-3.4.8/peek_agent_service/plugin/
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-07-11 02:51:10.000000 peek-agent-service-3.4.8/peek_agent_service/plugin/AgentPluginLoader.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-07-11 02:51:10.000000 peek-agent-service-3.4.8/peek_agent_service/plugin/AgentPluginLoaderTest.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2023-07-11 02:51:10.000000 peek-agent-service-3.4.8/peek_agent_service/plugin/PeekAgentPlatformHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:10.000000 peek-agent-service-3.4.8/peek_agent_service/plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7053 2023-07-11 02:51:10.000000 peek-agent-service-3.4.8/peek_agent_service/run_peek_agent_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:51:55.678118 peek-agent-service-3.4.8/peek_agent_service/sw_install/
+-rw-r--r--   0 root         (0) root         (0)      790 2023-07-11 02:51:10.000000 peek-agent-service-3.4.8/peek_agent_service/sw_install/PeekSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-07-11 02:51:10.000000 peek-agent-service-3.4.8/peek_agent_service/sw_install/PluginSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-07-11 02:51:10.000000 peek-agent-service-3.4.8/peek_agent_service/sw_install/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-07-11 02:51:10.000000 peek-agent-service-3.4.8/peek_agent_service/winsvc_peek_agent_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:51:55.678118 peek-agent-service-3.4.8/peek_agent_service.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-07-11 02:51:55.000000 peek-agent-service-3.4.8/peek_agent_service.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      902 2023-07-11 02:51:55.000000 peek-agent-service-3.4.8/peek_agent_service.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:51:55.000000 peek-agent-service-3.4.8/peek_agent_service.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      169 2023-07-11 02:51:55.000000 peek-agent-service-3.4.8/peek_agent_service.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:51:55.000000 peek-agent-service-3.4.8/peek_agent_service.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-11 02:51:55.000000 peek-agent-service-3.4.8/peek_agent_service.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-11 02:51:55.000000 peek-agent-service-3.4.8/peek_agent_service.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 02:51:55.679118 peek-agent-service-3.4.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-07-11 02:51:55.000000 peek-agent-service-3.4.8/setup.py
```

### Comparing `peek-agent-service-3.4.7/peek_agent_service/PeekAgentConfig.py` & `peek-agent-service-3.4.8/peek_agent_service/PeekAgentConfig.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.7/peek_agent_service/PeekAgentConfigTest.py` & `peek-agent-service-3.4.8/peek_agent_service/PeekAgentConfigTest.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.7/peek_agent_service/plugin/AgentPluginLoader.py` & `peek-agent-service-3.4.8/peek_agent_service/plugin/AgentPluginLoader.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.7/peek_agent_service/plugin/AgentPluginLoaderTest.py` & `peek-agent-service-3.4.8/peek_agent_service/plugin/AgentPluginLoaderTest.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.7/peek_agent_service/plugin/PeekAgentPlatformHook.py` & `peek-agent-service-3.4.8/peek_agent_service/plugin/PeekAgentPlatformHook.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.7/peek_agent_service/run_peek_agent_service.py` & `peek-agent-service-3.4.8/peek_agent_service/run_peek_agent_service.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.7/peek_agent_service/sw_install/PeekSwInstallManager.py` & `peek-agent-service-3.4.8/peek_agent_service/sw_install/PeekSwInstallManager.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.7/peek_agent_service/winsvc_peek_agent_service.py` & `peek-agent-service-3.4.8/peek_agent_service/winsvc_peek_agent_service.py`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.7/peek_agent_service.egg-info/SOURCES.txt` & `peek-agent-service-3.4.8/peek_agent_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-agent-service-3.4.7/setup.py` & `peek-agent-service-3.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_agent_service"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.7"
+package_version = "3.4.8"
 description = "Peek Agent Service."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

