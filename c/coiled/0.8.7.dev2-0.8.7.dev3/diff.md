# Comparing `tmp/coiled-0.8.7.dev2.tar.gz` & `tmp/coiled-0.8.7.dev3.tar.gz`

## Comparing `coiled-0.8.7.dev2.tar` & `coiled-0.8.7.dev3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/_version.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/analytics.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/auth.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/compatibility.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/context.py
--rw-r--r--   0        0        0   102249 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/exceptions.py
--rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/magic.py
--rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/run.py
--rw-r--r--   0        0        0    20044 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/scan.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/shutdown.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/software.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/types.py
--rw-r--r--   0        0        0    54964 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/config.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/core.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/env.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/login.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/prefect.py
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/run.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    45605 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26906 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/cli/setup/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/extensions/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/extensions/prefect/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/extensions/prefect/runners.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/extensions/prefect/workers.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/v2/__init__.py
--rw-r--r--   0        0        0    92578 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/v2/cluster.py
--rw-r--r--   0        0        0    58959 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/v2/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/v2/cwi_log_link.py
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/v2/states.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/v2/widgets/__init__.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/v2/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/coiled/v2/widgets/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/pyproject.toml
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.8.7.dev2/PKG-INFO
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/_version.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/analytics.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/auth.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/compatibility.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/context.py
+-rw-r--r--   0        0        0   102249 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/exceptions.py
+-rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/magic.py
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/run.py
+-rw-r--r--   0        0        0    20044 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/scan.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/shutdown.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/software.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/types.py
+-rw-r--r--   0        0        0    54964 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/config.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/core.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/env.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/login.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/prefect.py
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/run.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    45605 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26906 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/extensions/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/extensions/prefect/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/extensions/prefect/runners.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/extensions/prefect/workers.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/v2/__init__.py
+-rw-r--r--   0        0        0    93181 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/v2/cluster.py
+-rw-r--r--   0        0        0    58959 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/v2/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/v2/cwi_log_link.py
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/v2/states.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/v2/widgets/__init__.py
+-rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/v2/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/coiled/v2/widgets/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.8.7.dev3/PKG-INFO
```

### Comparing `coiled-0.8.7.dev2/coiled/__init__.py` & `coiled-0.8.7.dev3/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/analytics.py` & `coiled-0.8.7.dev3/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/auth.py` & `coiled-0.8.7.dev3/coiled/auth.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cluster.py` & `coiled-0.8.7.dev3/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/coiled.yaml` & `coiled-0.8.7.dev3/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/context.py` & `coiled-0.8.7.dev3/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/core.py` & `coiled-0.8.7.dev3/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/exceptions.py` & `coiled-0.8.7.dev3/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/magic.py` & `coiled-0.8.7.dev3/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/run.py` & `coiled-0.8.7.dev3/coiled/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/scan.py` & `coiled-0.8.7.dev3/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/shutdown.py` & `coiled-0.8.7.dev3/coiled/shutdown.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/software.py` & `coiled-0.8.7.dev3/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/types.py` & `coiled-0.8.7.dev3/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/utils.py` & `coiled-0.8.7.dev3/coiled/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/websockets.py` & `coiled-0.8.7.dev3/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/config.py` & `coiled-0.8.7.dev3/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/core.py` & `coiled-0.8.7.dev3/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/curl.py` & `coiled-0.8.7.dev3/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/env.py` & `coiled-0.8.7.dev3/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/login.py` & `coiled-0.8.7.dev3/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/package_sync.py` & `coiled-0.8.7.dev3/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/prefect.py` & `coiled-0.8.7.dev3/coiled/cli/prefect.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/run.py` & `coiled-0.8.7.dev3/coiled/cli/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/utils.py` & `coiled-0.8.7.dev3/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/cluster/__init__.py` & `coiled-0.8.7.dev3/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/cluster/better_logs.py` & `coiled-0.8.7.dev3/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/cluster/logs.py` & `coiled-0.8.7.dev3/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/cluster/metrics.py` & `coiled-0.8.7.dev3/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/cluster/ssh.py` & `coiled-0.8.7.dev3/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/cluster/utils.py` & `coiled-0.8.7.dev3/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/notebook/__init__.py` & `coiled-0.8.7.dev3/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/notebook/notebook.py` & `coiled-0.8.7.dev3/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/setup/__init__.py` & `coiled-0.8.7.dev3/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/setup/amp.py` & `coiled-0.8.7.dev3/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/setup/aws.py` & `coiled-0.8.7.dev3/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/setup/entry.py` & `coiled-0.8.7.dev3/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/setup/gcp.py` & `coiled-0.8.7.dev3/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/cli/setup/prometheus.py` & `coiled-0.8.7.dev3/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/extensions/prefect/runners.py` & `coiled-0.8.7.dev3/coiled/extensions/prefect/runners.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/extensions/prefect/workers.py` & `coiled-0.8.7.dev3/coiled/extensions/prefect/workers.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/v2/__init__.py` & `coiled-0.8.7.dev3/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/v2/cluster.py` & `coiled-0.8.7.dev3/coiled/v2/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1312,19 +1312,27 @@
                 # Let's optimize it, and then move this code up outside the loop.
 
                 if num_workers_to_wait_for is None:
                     cluster_desired_workers = cluster_details["desired_workers"]
                     num_workers_to_wait_for = parse_wait_for_workers(
                         cluster_desired_workers, self._wait_for_workers_arg
                     )
-                    if not is_new_cluster and (self._start_n_workers != cluster_desired_workers):
-                        logging.warning(
-                            f"Ignoring your request for {self._start_n_workers} workers since you are "
-                            f"connecting to a cluster that had been requested with {cluster_desired_workers} workers"
-                        )
+                    if not is_new_cluster:
+                        if self.start_adaptive:
+                            # When re-attaching to existing cluster without specifying n_workers,
+                            # we don't want to start adaptive (which we'd do otherwise when n_workers isn't specified)
+                            # and we also don't want to show message that we're ignoring n_workers (since in this case
+                            # it was set as default because n_workers was unspecified).
+                            self.start_adaptive = False
+                        elif self._start_n_workers != cluster_desired_workers:
+                            logging.warning(
+                                f"Ignoring your request for {self._start_n_workers} workers since you are "
+                                f"connecting to a cluster that had been requested with {cluster_desired_workers} "
+                                "workers"
+                            )
 
                 await self._update_cluster_status_logs()
                 self._maybe_log_summary(cluster_details)
 
                 if widget:
                     widget.update(
                         cluster_details,
```

### Comparing `coiled-0.8.7.dev2/coiled/v2/core.py` & `coiled-0.8.7.dev3/coiled/v2/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/v2/cwi_log_link.py` & `coiled-0.8.7.dev3/coiled/v2/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/v2/states.py` & `coiled-0.8.7.dev3/coiled/v2/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/v2/widgets/__init__.py` & `coiled-0.8.7.dev3/coiled/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/v2/widgets/rich.py` & `coiled-0.8.7.dev3/coiled/v2/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/coiled/v2/widgets/util.py` & `coiled-0.8.7.dev3/coiled/v2/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/LICENSE` & `coiled-0.8.7.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/README.md` & `coiled-0.8.7.dev3/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/pyproject.toml` & `coiled-0.8.7.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.7.dev2/PKG-INFO` & `coiled-0.8.7.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.8.7.dev2
+Version: 0.8.7.dev3
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.8.7.dev2 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.8.7.dev3 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: packaging Requires-Dist: pip
 Requires-Dist: pip>=19.3 Requires-Dist: prometheus-client Requires-Dist:
```

