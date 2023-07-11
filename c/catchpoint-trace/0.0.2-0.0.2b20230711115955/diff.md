# Comparing `tmp/catchpoint-trace-0.0.2.tar.gz` & `tmp/catchpoint-trace-0.0.2b20230711115955.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catchpoint-trace-0.0.2.tar", last modified: Tue Jul 11 12:11:24 2023, max compression
+gzip compressed data, was "catchpoint-trace-0.0.2b20230711115955.tar", last modified: Tue Jul 11 12:00:01 2023, max compression
```

## Comparing `catchpoint-trace-0.0.2.tar` & `catchpoint-trace-0.0.2b20230711115955.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.602413 catchpoint-trace-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-11 12:11:24.602413 catchpoint-trace-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22953 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.586413 catchpoint-trace-0.0.2/catchpoint/
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 12:11:18.000000 catchpoint-trace-0.0.2/catchpoint/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.586413 catchpoint-trace-0.0.2/catchpoint/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/application/application_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/application/application_info_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/application/global_application_info_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/catchpoint_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/composite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.586413 catchpoint-trace-0.0.2/catchpoint/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/config/config_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/config/config_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/config/config_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.586413 catchpoint-trace-0.0.2/catchpoint/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/context/context_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/context/execution_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/context/execution_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/context/global_execution_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/context/plugin_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/context/tracing_execution_context_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.586413 catchpoint-trace-0.0.2/catchpoint/debug/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/debug/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.590413 catchpoint-trace-0.0.2/catchpoint/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.590413 catchpoint-trace-0.0.2/catchpoint/integrations/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/aiohttp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/base_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/botocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.590413 catchpoint-trace-0.0.2/catchpoint/integrations/handler_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/handler_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/handler_wrappers/chalice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.590413 catchpoint-trace-0.0.2/catchpoint/integrations/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/botocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/django.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/modules/tornado.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/postgre.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/rdb_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/integrations/sqlite3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.590413 catchpoint-trace-0.0.2/catchpoint/listeners/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/listeners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/listeners/catchpoint_span_filterer.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/listeners/catchpoint_span_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/listeners/composite_span_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/listeners/error_injector_span_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/listeners/filtering_span_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/listeners/latency_injector_span_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/listeners/security_aware_span_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/listeners/tag_injector_span_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.590413 catchpoint-trace-0.0.2/catchpoint/opentracing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/opentracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.594413 catchpoint-trace-0.0.2/catchpoint/opentracing/propagation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/opentracing/propagation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/opentracing/propagation/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/opentracing/propagation/propagator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/opentracing/propagation/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/opentracing/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/opentracing/span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/opentracing/span_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/opentracing/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.594413 catchpoint-trace-0.0.2/catchpoint/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.594413 catchpoint-trace-0.0.2/catchpoint/plugins/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/config/base_plugin_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/config/catchpoint_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/config/log_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/config/metric_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/config/trace_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.594413 catchpoint-trace-0.0.2/catchpoint/plugins/invocation/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/invocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/invocation/invocation_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/invocation/invocation_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/invocation/invocation_trace_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.594413 catchpoint-trace-0.0.2/catchpoint/plugins/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/log/catchpoint_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/log/catchpoint_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/log/log_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/log/log_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.594413 catchpoint-trace-0.0.2/catchpoint/plugins/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/metric/metric_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/metric/metric_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.594413 catchpoint-trace-0.0.2/catchpoint/plugins/trace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/trace/patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/trace/trace_aware_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/trace/trace_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/trace/trace_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/plugins/trace/traceable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.594413 catchpoint-trace-0.0.2/catchpoint/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/samplers/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/samplers/composite_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/samplers/count_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/samplers/duration_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/samplers/error_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/samplers/time_aware_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.598413 catchpoint-trace-0.0.2/catchpoint/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.598413 catchpoint-trace-0.0.2/catchpoint/wrappers/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/aws_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/aws_lambda/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/aws_lambda/lambda_application_info_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/aws_lambda/lambda_event_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/aws_lambda/lambda_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/aws_lambda/lambda_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/base_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/cp_wrapper_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.598413 catchpoint-trace-0.0.2/catchpoint/wrappers/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/django/django_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/django/django_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/django/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.598413 catchpoint-trace-0.0.2/catchpoint/wrappers/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/fastapi/fastapi_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/fastapi/fastapi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/fastapi/fastapi_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/fastapi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.598413 catchpoint-trace-0.0.2/catchpoint/wrappers/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/flask/flask_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/flask/flask_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/flask/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.598413 catchpoint-trace-0.0.2/catchpoint/wrappers/tornado/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/tornado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/tornado/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/tornado/tornado_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/tornado/tornado_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/web_wrapper_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/wrapper_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/catchpoint/wrappers/wrapper_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.598413 catchpoint-trace-0.0.2/catchpoint_trace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-11 12:11:24.000000 catchpoint-trace-0.0.2/catchpoint_trace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-07-11 12:11:24.000000 catchpoint-trace-0.0.2/catchpoint_trace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:11:24.000000 catchpoint-trace-0.0.2/catchpoint_trace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 12:11:24.000000 catchpoint-trace-0.0.2/catchpoint_trace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 12:11:24.000000 catchpoint-trace-0.0.2/catchpoint_trace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:11:24.000000 catchpoint-trace-0.0.2/catchpoint_trace.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 12:11:24.602413 catchpoint-trace-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:11:24.602413 catchpoint-trace-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/tests/test_application_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/tests/test_catchpoint_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    22947 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/tests/test_lambda_event_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/tests/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-11 12:11:05.000000 catchpoint-trace-0.0.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.572870 catchpoint-trace-0.0.2b20230711115955/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-11 12:00:01.572870 catchpoint-trace-0.0.2b20230711115955/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22953 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.556869 catchpoint-trace-0.0.2b20230711115955/catchpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 11:59:55.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.556869 catchpoint-trace-0.0.2b20230711115955/catchpoint/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/application/application_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/application/application_info_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/application/global_application_info_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/catchpoint_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/composite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.556869 catchpoint-trace-0.0.2b20230711115955/catchpoint/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/config/config_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/config/config_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/config/config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.556869 catchpoint-trace-0.0.2b20230711115955/catchpoint/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/context/context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/context/execution_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/context/execution_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/context/global_execution_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/context/plugin_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/context/tracing_execution_context_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.556869 catchpoint-trace-0.0.2b20230711115955/catchpoint/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/debug/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.560869 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.560869 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/aiohttp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/base_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/botocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/elasticsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.560869 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/handler_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/handler_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/handler_wrappers/chalice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.560869 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/botocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/postgre.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/rdb_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/sqlite3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.564869 catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/catchpoint_span_filterer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/catchpoint_span_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/composite_span_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/error_injector_span_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/filtering_span_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/latency_injector_span_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/security_aware_span_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/tag_injector_span_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.564869 catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.564869 catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/propagation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/propagation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/propagation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/propagation/propagator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/propagation/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/span_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.564869 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.564869 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/config/base_plugin_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/config/catchpoint_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/config/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/config/metric_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/config/trace_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.564869 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/invocation/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/invocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/invocation/invocation_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/invocation/invocation_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/invocation/invocation_trace_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.564869 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/log/catchpoint_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/log/catchpoint_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/log/log_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/log/log_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.568869 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/metric/metric_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/metric/metric_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.568869 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/trace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/trace/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/trace/trace_aware_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/trace/trace_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/trace/trace_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/trace/traceable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.568869 catchpoint-trace-0.0.2b20230711115955/catchpoint/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/samplers/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/samplers/composite_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/samplers/count_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/samplers/duration_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/samplers/error_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/samplers/time_aware_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.568869 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.568869 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/aws_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/aws_lambda/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/aws_lambda/lambda_application_info_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/aws_lambda/lambda_event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/aws_lambda/lambda_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/aws_lambda/lambda_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/base_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/cp_wrapper_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.568869 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/django/django_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/django/django_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/django/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.572870 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/fastapi/fastapi_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/fastapi/fastapi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/fastapi/fastapi_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/fastapi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.572870 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/flask/flask_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/flask/flask_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/flask/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.572870 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/tornado/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/tornado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/tornado/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/tornado/tornado_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/tornado/tornado_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/web_wrapper_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/wrapper_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/wrapper_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.572870 catchpoint-trace-0.0.2b20230711115955/catchpoint_trace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-11 12:00:01.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint_trace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-07-11 12:00:01.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint_trace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:00:01.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint_trace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 12:00:01.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint_trace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 12:00:01.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint_trace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:00:01.000000 catchpoint-trace-0.0.2b20230711115955/catchpoint_trace.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 12:00:01.572870 catchpoint-trace-0.0.2b20230711115955/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:00:01.572870 catchpoint-trace-0.0.2b20230711115955/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/tests/test_application_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/tests/test_catchpoint_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22947 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/tests/test_lambda_event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-11 11:59:42.000000 catchpoint-trace-0.0.2b20230711115955/tests/test_utils.py
```

### Comparing `catchpoint-trace-0.0.2/LICENSE` & `catchpoint-trace-0.0.2b20230711115955/LICENSE`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/PKG-INFO` & `catchpoint-trace-0.0.2b20230711115955/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catchpoint-trace
-Version: 0.0.2
+Version: 0.0.2b20230711115955
 Summary: Catchpoint Python agent
 Home-page: https://github.com/thundra-io/cp-trace-python
 Author: Catchpoint
 Author-email: python@catchpoint.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `catchpoint-trace-0.0.2/README.md` & `catchpoint-trace-0.0.2b20230711115955/README.md`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/__init__.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/application/application_info.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/application/application_info.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/application/application_info_provider.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/application/application_info_provider.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/application/global_application_info_provider.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/application/global_application_info_provider.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/compat.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/compat.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/composite.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/composite.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/config/config_metadata.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/config/config_metadata.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/config/config_names.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/config/config_names.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/config/config_provider.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/config/config_provider.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/constants.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/constants.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/context/execution_context.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/context/execution_context.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/context/execution_context_manager.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/context/execution_context_manager.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/context/tracing_execution_context_provider.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/context/tracing_execution_context_provider.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/debug/bridge.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/debug/bridge.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/handler.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/handler.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/aiohttp/client.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/aiohttp/client.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/base_integration.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/base_integration.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/botocore.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/botocore.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/django.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/django.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/elasticsearch.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/handler_wrappers/__init__.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/handler_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/handler_wrappers/chalice.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/handler_wrappers/chalice.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/__init__.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/aiohttp.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/aiohttp.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/botocore.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/botocore.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/db.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/db.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/django.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/django.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/elasticsearch.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/fastapi.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/fastapi.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/flask.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/flask.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/mysql.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/mysql.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/psycopg2.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/psycopg2.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/pymongo.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/pymongo.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/redis.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/redis.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/requests.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/requests.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/sqlalchemy.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/sqlite3.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/sqlite3.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/modules/tornado.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/modules/tornado.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/mongodb.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/mongodb.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/mysql.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/mysql.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/postgre.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/postgre.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/redis.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/redis.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/requests.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/requests.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/sqlalchemy.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/integrations/sqlite3.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/integrations/sqlite3.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/listeners/__init__.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/listeners/catchpoint_span_filterer.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/catchpoint_span_filterer.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/listeners/catchpoint_span_listener.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/catchpoint_span_listener.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/listeners/composite_span_filter.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/composite_span_filter.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/listeners/error_injector_span_listener.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/error_injector_span_listener.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/listeners/filtering_span_listener.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/filtering_span_listener.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/listeners/latency_injector_span_listener.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/latency_injector_span_listener.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/listeners/security_aware_span_listener.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/security_aware_span_listener.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/listeners/tag_injector_span_listener.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/listeners/tag_injector_span_listener.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/opentracing/propagation/http.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/propagation/http.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/opentracing/propagation/text.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/propagation/text.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/opentracing/span.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/span.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/opentracing/span_context.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/span_context.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/opentracing/tracer.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/opentracing/tracer.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/plugins/config/catchpoint_config.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/config/catchpoint_config.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/plugins/invocation/invocation_plugin.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/invocation/invocation_plugin.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/plugins/invocation/invocation_support.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/invocation/invocation_support.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/plugins/invocation/invocation_trace_support.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/invocation/invocation_trace_support.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/plugins/log/catchpoint_log_handler.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/log/catchpoint_log_handler.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/plugins/log/catchpoint_logger.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/log/catchpoint_logger.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/plugins/log/log_plugin.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/log/log_plugin.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/plugins/metric/metric_plugin.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/metric/metric_plugin.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/plugins/trace/patcher.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/trace/patcher.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/plugins/trace/trace_aware_wrapper.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/trace/trace_aware_wrapper.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/plugins/trace/trace_plugin.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/trace/trace_plugin.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/plugins/trace/trace_support.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/trace/trace_support.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/plugins/trace/traceable.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/plugins/trace/traceable.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/reporter.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/reporter.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/samplers/composite_sampler.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/samplers/composite_sampler.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/samplers/count_aware_sampler.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/samplers/count_aware_sampler.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/samplers/time_aware_sampler.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/samplers/time_aware_sampler.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/timeout.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/timeout.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/utils.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/utils.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/aws_lambda/handler.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/aws_lambda/handler.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/aws_lambda/lambda_application_info_provider.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/aws_lambda/lambda_application_info_provider.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/aws_lambda/lambda_event_utils.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/aws_lambda/lambda_event_utils.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/aws_lambda/lambda_executor.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/aws_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/aws_lambda/lambda_wrapper.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/aws_lambda/lambda_wrapper.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/base_wrapper.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/cp_wrapper_utils.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/cp_wrapper_utils.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/django/django_executor.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/django/django_executor.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/django/django_wrapper.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/django/django_wrapper.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/django/middleware.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/django/middleware.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/fastapi/fastapi_executor.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/fastapi/fastapi_executor.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/fastapi/fastapi_utils.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/fastapi/fastapi_utils.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/fastapi/fastapi_wrapper.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/fastapi/fastapi_wrapper.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/fastapi/middleware.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/fastapi/middleware.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/flask/flask_executor.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/flask/flask_executor.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/flask/flask_wrapper.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/flask/flask_wrapper.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/flask/middleware.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/flask/middleware.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/tornado/middleware.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/tornado/middleware.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/tornado/tornado_executor.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/tornado/tornado_executor.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/tornado/tornado_wrapper.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/tornado/tornado_wrapper.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/web_wrapper_utils.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/web_wrapper_utils.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint/wrappers/wrapper_utils.py` & `catchpoint-trace-0.0.2b20230711115955/catchpoint/wrappers/wrapper_utils.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/catchpoint_trace.egg-info/PKG-INFO` & `catchpoint-trace-0.0.2b20230711115955/catchpoint_trace.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catchpoint-trace
-Version: 0.0.2
+Version: 0.0.2b20230711115955
 Summary: Catchpoint Python agent
 Home-page: https://github.com/thundra-io/cp-trace-python
 Author: Catchpoint
 Author-email: python@catchpoint.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `catchpoint-trace-0.0.2/catchpoint_trace.egg-info/SOURCES.txt` & `catchpoint-trace-0.0.2b20230711115955/catchpoint_trace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/setup.py` & `catchpoint-trace-0.0.2b20230711115955/setup.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/tests/test_application_support.py` & `catchpoint-trace-0.0.2b20230711115955/tests/test_application_support.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/tests/test_catchpoint_agent.py` & `catchpoint-trace-0.0.2b20230711115955/tests/test_catchpoint_agent.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/tests/test_lambda_event_utils.py` & `catchpoint-trace-0.0.2b20230711115955/tests/test_lambda_event_utils.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/tests/test_reporter.py` & `catchpoint-trace-0.0.2b20230711115955/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `catchpoint-trace-0.0.2/tests/test_utils.py` & `catchpoint-trace-0.0.2b20230711115955/tests/test_utils.py`

 * *Files identical despite different names*

