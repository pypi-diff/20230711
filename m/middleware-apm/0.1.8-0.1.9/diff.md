# Comparing `tmp/middleware-apm-0.1.8.tar.gz` & `tmp/middleware-apm-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "middleware-apm-0.1.8.tar", last modified: Fri Oct 28 11:57:22 2022, max compression
+gzip compressed data, was "middleware-apm-0.1.9.tar", last modified: Sat Oct 29 04:32:40 2022, max compression
```

## Comparing `middleware-apm-0.1.8.tar` & `middleware-apm-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:57:22.036053 middleware-apm-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-28 11:57:14.000000 middleware-apm-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-10-28 11:57:22.036053 middleware-apm-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-28 11:57:14.000000 middleware-apm-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:57:22.032053 middleware-apm-0.1.8/apmpythonpackage/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-28 11:57:14.000000 middleware-apm-0.1.8/apmpythonpackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2897 2022-10-28 11:57:14.000000 middleware-apm-0.1.8/apmpythonpackage/apmpythonpackage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 11:57:22.036053 middleware-apm-0.1.8/middleware_apm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-10-28 11:57:21.000000 middleware-apm-0.1.8/middleware_apm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-10-28 11:57:22.000000 middleware-apm-0.1.8/middleware_apm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-28 11:57:21.000000 middleware-apm-0.1.8/middleware_apm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-28 11:57:21.000000 middleware-apm-0.1.8/middleware_apm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-28 11:57:22.036053 middleware-apm-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-10-28 11:57:14.000000 middleware-apm-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 04:32:40.938949 middleware-apm-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-29 04:32:33.000000 middleware-apm-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-10-29 04:32:40.938949 middleware-apm-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-29 04:32:33.000000 middleware-apm-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 04:32:40.938949 middleware-apm-0.1.9/apmpythonpackage/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-29 04:32:33.000000 middleware-apm-0.1.9/apmpythonpackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2897 2022-10-29 04:32:33.000000 middleware-apm-0.1.9/apmpythonpackage/apmpythonpackage.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 04:32:40.938949 middleware-apm-0.1.9/middleware_apm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-10-29 04:32:40.000000 middleware-apm-0.1.9/middleware_apm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-10-29 04:32:40.000000 middleware-apm-0.1.9/middleware_apm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 04:32:40.000000 middleware-apm-0.1.9/middleware_apm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-29 04:32:40.000000 middleware-apm-0.1.9/middleware_apm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-29 04:32:40.938949 middleware-apm-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2022-10-29 04:32:33.000000 middleware-apm-0.1.9/setup.py
```

### Comparing `middleware-apm-0.1.8/LICENSE` & `middleware-apm-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `middleware-apm-0.1.8/apmpythonpackage/apmpythonpackage.py` & `middleware-apm-0.1.9/apmpythonpackage/apmpythonpackage.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,12 +78,12 @@
     def logemit(self, arg1, arg2):
         logger.emit(arg1, arg2)
 
     # tracing method
     def mw_tracer(self):
         trace.set_tracer_provider(TracerProvider())
         tracer = trace.get_tracer_provider().get_tracer(__name__)
-        otlp_exporter = OTLPSpanExporter(endpoint=mw_agent_target + ":4320", insecure=True)
+        otlp_exporter = OTLPSpanExporter(endpoint=mw_agent_target + ":9319", insecure=True)
         span_processor = BatchSpanProcessor(otlp_exporter)
         trace.get_tracer_provider().add_span_processor(
             span_processor)
         return tracer, trace, extract, collect_request_attributes
```

