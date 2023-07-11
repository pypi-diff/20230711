# Comparing `tmp/temboard-agent-8.0b6.tar.gz` & `tmp/temboard-agent-8.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temboard-agent-8.0b6.tar", last modified: Thu Nov  3 09:18:33 2022, max compression
+gzip compressed data, was "temboard-agent-8.1b1.tar", last modified: Tue Jul 11 12:20:06 2023, max compression
```

## Comparing `temboard-agent-8.0b6.tar` & `temboard-agent-8.1b1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.382340 temboard-agent-8.0b6/
--rw-r--r--   0 root         (0) root         (0)      898 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      215 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      928 2022-11-03 09:18:33.382340 temboard-agent-8.0b6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      201 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.370339 temboard-agent-8.0b6/packaging/
--rw-r--r--   0 root         (0) root         (0)      433 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/packaging/temboard-agent@.service
--rw-r--r--   0 root         (0) root         (0)      213 2022-11-03 09:18:33.382340 temboard-agent-8.0b6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2444 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.374340 temboard-agent-8.0b6/share/
--rwxr-xr-x   0 root         (0) root         (0)    10550 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/share/auto_configure.sh
--rwxr-xr-x   0 root         (0) root         (0)      748 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/share/purge.sh
--rwxr-xr-x   0 root         (0) root         (0)      328 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/share/restart-all.sh
--rw-r--r--   0 root         (0) root         (0)     1704 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/share/temboard-agent_CHANGEME.key
--rw-r--r--   0 root         (0) root         (0)     1123 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/share/temboard-agent_CHANGEME.pem
--rw-r--r--   0 root         (0) root         (0)     1233 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/share/temboard-agent_ca_certs_CHANGEME.pem
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.374340 temboard-agent-8.0b6/temboard_agent.egg-info/
--rw-r--r--   0 root         (0) root         (0)      928 2022-11-03 09:18:33.000000 temboard-agent-8.0b6/temboard_agent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3001 2022-11-03 09:18:33.000000 temboard-agent-8.0b6/temboard_agent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-03 09:18:33.000000 temboard-agent-8.0b6/temboard_agent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      524 2022-11-03 09:18:33.000000 temboard-agent-8.0b6/temboard_agent.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-11-03 09:18:33.000000 temboard-agent-8.0b6/temboard_agent.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-11-03 09:18:33.000000 temboard-agent-8.0b6/temboard_agent.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.374340 temboard-agent-8.0b6/temboardagent/
--rw-r--r--   0 root         (0) root         (0)      165 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/__init__.py
--rw-r--r--   0 root         (0) root         (0)      718 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.374340 temboard-agent-8.0b6/temboardagent/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9758 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/cli/app.py
--rw-r--r--   0 root         (0) root         (0)      447 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/cli/discover.py
--rw-r--r--   0 root         (0) root         (0)     1529 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/cli/fetch_key.py
--rw-r--r--   0 root         (0) root         (0)     6735 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/cli/register.py
--rw-r--r--   0 root         (0) root         (0)     1344 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/cli/routes.py
--rw-r--r--   0 root         (0) root         (0)      631 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/cli/runscript.py
--rw-r--r--   0 root         (0) root         (0)      832 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/cli/runtask.py
--rw-r--r--   0 root         (0) root         (0)     1271 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/cli/serve.py
--rw-r--r--   0 root         (0) root         (0)     1147 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/cli/tasks.py
--rw-r--r--   0 root         (0) root         (0)      343 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/cli/web.py
--rw-r--r--   0 root         (0) root         (0)     1160 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/command.py
--rw-r--r--   0 root         (0) root         (0)       69 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/core.py
--rw-r--r--   0 root         (0) root         (0)     2240 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/daemon.py
--rw-r--r--   0 root         (0) root         (0)     7242 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/discover.py
--rw-r--r--   0 root         (0) root         (0)      244 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/errors.py
--rw-r--r--   0 root         (0) root         (0)     8279 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/inventory.py
--rw-r--r--   0 root         (0) root         (0)     3624 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/notification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.374340 temboard-agent-8.0b6/temboardagent/plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.374340 temboard-agent-8.0b6/temboardagent/plugins/activity/
--rw-r--r--   0 root         (0) root         (0)     4761 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/activity/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10622 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/activity/functions.py
--rw-r--r--   0 root         (0) root         (0)     5903 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/activity/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.374340 temboard-agent-8.0b6/temboardagent/plugins/administration/
--rw-r--r--   0 root         (0) root         (0)     3160 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/administration/__init__.py
--rw-r--r--   0 root         (0) root         (0)       90 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/administration/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.378340 temboard-agent-8.0b6/temboardagent/plugins/dashboard/
--rw-r--r--   0 root         (0) root         (0)     4050 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/dashboard/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1939 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/dashboard/db.py
--rw-r--r--   0 root         (0) root         (0)     8627 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/dashboard/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.378340 temboard-agent-8.0b6/temboardagent/plugins/maintenance/
--rw-r--r--   0 root         (0) root         (0)     7874 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/maintenance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26868 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/maintenance/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.378340 temboard-agent-8.0b6/temboardagent/plugins/monitoring/
--rw-r--r--   0 root         (0) root         (0)     6820 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4338 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/monitoring/db.py
--rw-r--r--   0 root         (0) root         (0)     2978 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/monitoring/inventory.py
--rw-r--r--   0 root         (0) root         (0)    20989 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/monitoring/openmetrics.py
--rw-r--r--   0 root         (0) root         (0)      305 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/monitoring/output.py
--rw-r--r--   0 root         (0) root         (0)    30099 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/monitoring/probes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.378340 temboard-agent-8.0b6/temboardagent/plugins/pgconf/
--rw-r--r--   0 root         (0) root         (0)     1546 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/pgconf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4467 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/pgconf/filemgmt.py
--rw-r--r--   0 root         (0) root         (0)    13324 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/pgconf/functions.py
--rw-r--r--   0 root         (0) root         (0)      140 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/pgconf/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.378340 temboard-agent-8.0b6/temboardagent/plugins/statements/
--rw-r--r--   0 root         (0) root         (0)     1766 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/plugins/statements/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8753 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.378340 temboard-agent-8.0b6/temboardagent/queries/
--rw-r--r--   0 root         (0) root         (0)       76 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/queries/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1671 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/queries/activity-locks.sql
--rw-r--r--   0 root         (0) root         (0)      959 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/queries/activity-sessions.sql
--rw-r--r--   0 root         (0) root         (0)      425 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/queries/discover-settings.sql
--rw-r--r--   0 root         (0) root         (0)      268 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/queries/discover.sql
--rw-r--r--   0 root         (0) root         (0)      209 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.378340 temboard-agent-8.0b6/temboardagent/toolkit/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16397 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/app.py
--rw-r--r--   0 root         (0) root         (0)     7309 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/configuration.py
--rw-r--r--   0 root         (0) root         (0)      272 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/errors.py
--rw-r--r--   0 root         (0) root         (0)     5624 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/http.py
--rw-r--r--   0 root         (0) root         (0)     5726 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/log.py
--rw-r--r--   0 root         (0) root         (0)     2455 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/perf.py
--rw-r--r--   0 root         (0) root         (0)     8038 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/proctitle.py
--rw-r--r--   0 root         (0) root         (0)      629 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/pycompat.py
--rw-r--r--   0 root         (0) root         (0)     1886 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/queries.py
--rw-r--r--   0 root         (0) root         (0)     7118 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/services.py
--rw-r--r--   0 root         (0) root         (0)     2450 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/signing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.382340 temboard-agent-8.0b6/temboardagent/toolkit/tasklist/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/tasklist/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11784 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/tasklist/sqlite3_engine.py
--rw-r--r--   0 root         (0) root         (0)    30519 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/taskmanager.py
--rw-r--r--   0 root         (0) root         (0)     2094 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/utils.py
--rw-r--r--   0 root         (0) root         (0)     3479 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/validators.py
--rw-r--r--   0 root         (0) root         (0)     1465 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/toolkit/versions.py
--rw-r--r--   0 root         (0) root         (0)     3970 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/tools.py
--rw-r--r--   0 root         (0) root         (0)       22 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.382340 temboard-agent-8.0b6/temboardagent/web/
--rw-r--r--   0 root         (0) root         (0)       62 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5810 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/web/app.py
--rw-r--r--   0 root         (0) root         (0)     2175 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/web/core.py
--rw-r--r--   0 root         (0) root         (0)     1891 2022-11-03 09:18:32.000000 temboard-agent-8.0b6/temboardagent/web/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.762332 temboard-agent-8.1b1/
+-rw-r--r--   0 root         (0) root         (0)      898 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      215 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      928 2023-07-11 12:20:06.762332 temboard-agent-8.1b1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      201 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.754332 temboard-agent-8.1b1/packaging/
+-rw-r--r--   0 root         (0) root         (0)      433 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/packaging/temboard-agent@.service
+-rw-r--r--   0 root         (0) root         (0)      213 2023-07-11 12:20:06.762332 temboard-agent-8.1b1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.754332 temboard-agent-8.1b1/share/
+-rwxr-xr-x   0 root         (0) root         (0)    10754 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/share/auto_configure.sh
+-rwxr-xr-x   0 root         (0) root         (0)      748 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/share/purge.sh
+-rwxr-xr-x   0 root         (0) root         (0)      328 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/share/restart-all.sh
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/share/temboard-agent_CHANGEME.key
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/share/temboard-agent_CHANGEME.pem
+-rw-r--r--   0 root         (0) root         (0)     1233 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/share/temboard-agent_ca_certs_CHANGEME.pem
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.754332 temboard-agent-8.1b1/temboard_agent.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      928 2023-07-11 12:20:06.000000 temboard-agent-8.1b1/temboard_agent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3001 2023-07-11 12:20:06.000000 temboard-agent-8.1b1/temboard_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 12:20:06.000000 temboard-agent-8.1b1/temboard_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      524 2023-07-11 12:20:06.000000 temboard-agent-8.1b1/temboard_agent.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-11 12:20:06.000000 temboard-agent-8.1b1/temboard_agent.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-11 12:20:06.000000 temboard-agent-8.1b1/temboard_agent.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.758332 temboard-agent-8.1b1/temboardagent/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.758332 temboard-agent-8.1b1/temboardagent/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9758 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/cli/app.py
+-rw-r--r--   0 root         (0) root         (0)      447 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/cli/discover.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/cli/fetch_key.py
+-rw-r--r--   0 root         (0) root         (0)     6735 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/cli/register.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/cli/routes.py
+-rw-r--r--   0 root         (0) root         (0)      631 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/cli/runscript.py
+-rw-r--r--   0 root         (0) root         (0)      832 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/cli/runtask.py
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/cli/serve.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/cli/tasks.py
+-rw-r--r--   0 root         (0) root         (0)      343 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/cli/web.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/command.py
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/core.py
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     7242 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/discover.py
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/errors.py
+-rw-r--r--   0 root         (0) root         (0)     8279 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/inventory.py
+-rw-r--r--   0 root         (0) root         (0)     3624 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/notification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.758332 temboard-agent-8.1b1/temboardagent/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.758332 temboard-agent-8.1b1/temboardagent/plugins/activity/
+-rw-r--r--   0 root         (0) root         (0)     4761 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/activity/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10622 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/activity/functions.py
+-rw-r--r--   0 root         (0) root         (0)     5903 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/activity/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.758332 temboard-agent-8.1b1/temboardagent/plugins/administration/
+-rw-r--r--   0 root         (0) root         (0)     3160 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/administration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/administration/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.758332 temboard-agent-8.1b1/temboardagent/plugins/dashboard/
+-rw-r--r--   0 root         (0) root         (0)     4048 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/dashboard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/dashboard/db.py
+-rw-r--r--   0 root         (0) root         (0)     8625 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/dashboard/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.758332 temboard-agent-8.1b1/temboardagent/plugins/maintenance/
+-rw-r--r--   0 root         (0) root         (0)     8366 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/maintenance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26868 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/maintenance/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.758332 temboard-agent-8.1b1/temboardagent/plugins/monitoring/
+-rw-r--r--   0 root         (0) root         (0)     6820 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4338 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/monitoring/db.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/monitoring/inventory.py
+-rw-r--r--   0 root         (0) root         (0)    20989 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/monitoring/openmetrics.py
+-rw-r--r--   0 root         (0) root         (0)      305 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/monitoring/output.py
+-rw-r--r--   0 root         (0) root         (0)    30100 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/monitoring/probes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.758332 temboard-agent-8.1b1/temboardagent/plugins/pgconf/
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/pgconf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4467 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/pgconf/filemgmt.py
+-rw-r--r--   0 root         (0) root         (0)    13324 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/pgconf/functions.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/pgconf/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.758332 temboard-agent-8.1b1/temboardagent/plugins/statements/
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/plugins/statements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9684 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.758332 temboard-agent-8.1b1/temboardagent/queries/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/queries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/queries/activity-locks.sql
+-rw-r--r--   0 root         (0) root         (0)      959 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/queries/activity-sessions.sql
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/queries/discover-settings.sql
+-rw-r--r--   0 root         (0) root         (0)      268 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/queries/discover.sql
+-rw-r--r--   0 root         (0) root         (0)      209 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.762332 temboard-agent-8.1b1/temboardagent/toolkit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16397 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/app.py
+-rw-r--r--   0 root         (0) root         (0)     7309 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/configuration.py
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5624 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/http.py
+-rw-r--r--   0 root         (0) root         (0)     5716 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/log.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/perf.py
+-rw-r--r--   0 root         (0) root         (0)     8038 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/proctitle.py
+-rw-r--r--   0 root         (0) root         (0)      629 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/pycompat.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7118 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/services.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/signing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.762332 temboard-agent-8.1b1/temboardagent/toolkit/tasklist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/tasklist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11784 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/tasklist/sqlite3_engine.py
+-rw-r--r--   0 root         (0) root         (0)    30519 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/taskmanager.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3479 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/validators.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/toolkit/versions.py
+-rw-r--r--   0 root         (0) root         (0)     3970 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/tools.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:06.762332 temboard-agent-8.1b1/temboardagent/web/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6017 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/web/app.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/web/core.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-07-11 12:20:05.000000 temboard-agent-8.1b1/temboardagent/web/service.py
```

### Comparing `temboard-agent-8.0b6/LICENSE` & `temboard-agent-8.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/PKG-INFO` & `temboard-agent-8.1b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temboard-agent
-Version: 8.0b6
+Version: 8.1b1
 Summary: PostgreSQL Remote Control Agent
 Home-page: https://labs.dalibo.com/temboard
 Author: Dalibo
 Author-email: contact@dalibo.com
 License: PostgreSQL
 Description: # temBoard Agent
```

### Comparing `temboard-agent-8.0b6/setup.py` & `temboard-agent-8.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,10 +57,10 @@
             'maintenance = temboardagent.plugins.maintenance:MaintenancePlugin',  # noqa
             'monitoring = temboardagent.plugins.monitoring:MonitoringPlugin',
             'pgconf = temboardagent.plugins.pgconf:PgConfPlugin',
             'statements = temboardagent.plugins.statements:StatementsPlugin',
         ],
     },
     packages=find_packages(),
-    long_description=open('README.md').read(),
+    long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
 ))
```

### Comparing `temboard-agent-8.0b6/share/auto_configure.sh` & `temboard-agent-8.1b1/share/auto_configure.sh`

 * *Files 2% similar despite different names*

```diff
@@ -92,18 +92,22 @@
 	local sslcert=$1; shift
 	local sslkey=$1; shift
 	local instance=$1; shift
 	local has_statements=$1; shift
 
 	local pg_ctl
 	local port
+	local version
 
 	sudo -u "$SYSUSER" test -r "$sslkey"
 	sudo -u "$SYSUSER" test -r "$sslcert"
 
+	version="$(temboard-agent --version | sed 's/^/# /')"
+	created="$(date)"
+
 	port="${TEMBOARD_PORT-$(find_next_free_port)}"
 	test -n "$port"
 	log "Configuring temboard-agent to run on port ${port}."
 	if ! pg_ctl="$(command -v pg_ctl)" ; then
 		pg_ctl="/bin/false"
 		log "Can't find pg_ctl in PATH."
 		log "Please configure it manually to enable restart feature."
@@ -122,15 +126,20 @@
 	    usepeer=1
 	fi
 
 	cat <<-EOF
 	#
 	#   T E M B O A R D   A G E N T   C O N F I G U R A T I O N
 	#
-	# Generated by ${BASH_SOURCE[0]} on $(date +%Y-%m-%d).
+	# Generated by ${BASH_SOURCE[0]} on $created.
+	#
+	$version
+	#
+	# See https://temboard.rtfd.io/ for details on configuration
+	# possibilities.
 	#
 
 
 	#
 	# General temBoard agent configuration
 	#
 	[temboard]
@@ -289,14 +298,16 @@
 		chmod 0640 "$sslkey"
 		chgrp "$(id --group --name "$SYSUSER")" "$sslcert" "$sslkey"
 	fi
 
 	readlink -e "$sslcert" "$sslkey"
 }
 
+exec 0>&-  # Close stdin.
+
 if [ -n "${DEBUG-}" ] ; then
 	exec 3>/dev/null
 else
 	exec 3>&2 2>"${LOGFILE}" 1>&2
 	chmod 0600 "${LOGFILE}"
 	trap 'catchall' INT EXIT TERM
 fi
```

### Comparing `temboard-agent-8.0b6/share/purge.sh` & `temboard-agent-8.1b1/share/purge.sh`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/share/temboard-agent_CHANGEME.key` & `temboard-agent-8.1b1/share/temboard-agent_CHANGEME.key`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/share/temboard-agent_CHANGEME.pem` & `temboard-agent-8.1b1/share/temboard-agent_CHANGEME.pem`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/share/temboard-agent_ca_certs_CHANGEME.pem` & `temboard-agent-8.1b1/share/temboard-agent_ca_certs_CHANGEME.pem`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboard_agent.egg-info/PKG-INFO` & `temboard-agent-8.1b1/temboard_agent.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temboard-agent
-Version: 8.0b6
+Version: 8.1b1
 Summary: PostgreSQL Remote Control Agent
 Home-page: https://labs.dalibo.com/temboard
 Author: Dalibo
 Author-email: contact@dalibo.com
 License: PostgreSQL
 Description: # temBoard Agent
```

### Comparing `temboard-agent-8.0b6/temboard_agent.egg-info/SOURCES.txt` & `temboard-agent-8.1b1/temboard_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboard_agent.egg-info/entry_points.txt` & `temboard-agent-8.1b1/temboard_agent.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/__main__.py` & `temboard-agent-8.1b1/temboardagent/__main__.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/cli/app.py` & `temboard-agent-8.1b1/temboardagent/cli/app.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/cli/fetch_key.py` & `temboard-agent-8.1b1/temboardagent/cli/fetch_key.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/cli/register.py` & `temboard-agent-8.1b1/temboardagent/cli/register.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/cli/routes.py` & `temboard-agent-8.1b1/temboardagent/cli/routes.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/cli/runscript.py` & `temboard-agent-8.1b1/temboardagent/cli/runscript.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/cli/runtask.py` & `temboard-agent-8.1b1/temboardagent/cli/runtask.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/cli/serve.py` & `temboard-agent-8.1b1/temboardagent/cli/serve.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/cli/tasks.py` & `temboard-agent-8.1b1/temboardagent/cli/tasks.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/command.py` & `temboard-agent-8.1b1/temboardagent/command.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/daemon.py` & `temboard-agent-8.1b1/temboardagent/daemon.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/discover.py` & `temboard-agent-8.1b1/temboardagent/discover.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/inventory.py` & `temboard-agent-8.1b1/temboardagent/inventory.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/notification.py` & `temboard-agent-8.1b1/temboardagent/notification.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/activity/__init__.py` & `temboard-agent-8.1b1/temboardagent/plugins/activity/__init__.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/activity/functions.py` & `temboard-agent-8.1b1/temboardagent/plugins/activity/functions.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/activity/process.py` & `temboard-agent-8.1b1/temboardagent/plugins/activity/process.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/administration/__init__.py` & `temboard-agent-8.1b1/temboardagent/plugins/administration/__init__.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/dashboard/__init__.py` & `temboard-agent-8.1b1/temboardagent/plugins/dashboard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
         try:
             pool = pool or app.postgres.pool()
         except Exception as e:
             logger.error("Failed to connect to Postgres: %s", e)
         else:
             try:
-                for attempt in pool.retry_connection():
+                for attempt in pool.auto_reconnect():
                     with attempt:
                         dashboard_collector_worker(app, pool)
             except Exception as e:
                 logger.error("Dashboard collector error: %s", e)
 
         elapsed = utcnow() - start
         elapsed = elapsed.total_seconds()
```

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/dashboard/db.py` & `temboard-agent-8.1b1/temboardagent/plugins/dashboard/db.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/dashboard/metrics.py` & `temboard-agent-8.1b1/temboardagent/plugins/dashboard/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ...inventory import SysInfo
 
 
 def get_metrics(app, pool=None):
     res = dict()
     pool = pool or app.postgres.pool()
     discover = app.discover.ensure_latest()
-    for attempt in pool.retry_connection():
+    for attempt in pool.auto_reconnect():
         with attempt() as conn:
             dm = DashboardMetrics(conn)
             pgdiscover = discover['postgres']
             res.update(dict(
                 buffers=dm.get_buffers(),
                 hitratio=dm.get_hitratio(),
                 active_backends=dm.get_active_backends(),
```

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/maintenance/__init__.py` & `temboard-agent-8.1b1/temboardagent/plugins/maintenance/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,47 +19,51 @@
     rows = functions.get_databases(pgconn)
 
     databases = []
     for database in rows:
         database = dict(database)
         # we need to connect with a different database
         dbname = database['datname']
-        dbconn = pgpool.getconn(dbname)
-        database.update(**functions.get_database(dbconn))
+        for getconn in pgpool.auto_reconnect():
+            with getconn(dbname) as dbconn:
+                database.update(**functions.get_database(dbconn))
         databases.append(database)
 
     return {'instance': instance, 'databases': databases}
 
 
 T_VACUUM_MODE = b'(((^|,)(full|freeze|analyze))+$)'
 T_TIMESTAMP_UTC = b'(^[0-9]{4}-[0-9]{2}-[0-9]{2}T[0-9]{2}:[0-9]{2}:[0-9]{2}Z$)'
 
 
 @bottle.get('/<dbname>')
 def get_database(pgpool, dbname):
-    conn = pgpool.getconn(dbname)
-    database = functions.get_database_size(conn)
-    schemas = functions.get_schemas(conn)
+    for getconn in pgpool.auto_reconnect():
+        with getconn(dbname) as conn:
+            database = functions.get_database_size(conn)
+            schemas = functions.get_schemas(conn)
     return dict(database, **{'schemas': schemas})
 
 
 @bottle.get('/<dbname>/schema/<schema>')
 def get_schema(pgpool, dbname, schema):
-    conn = pgpool.getconn(dbname)
-    tables = functions.get_tables(conn, schema)
-    indexes = functions.get_schema_indexes(conn, schema)
-    schema = functions.get_schema(conn, schema)
+    for getconn in pgpool.auto_reconnect():
+        with getconn(dbname) as conn:
+            tables = functions.get_tables(conn, schema)
+            indexes = functions.get_schema_indexes(conn, schema)
+            schema = functions.get_schema(conn, schema)
     return dict(dict(tables, **indexes), **schema)
 
 
 @bottle.get('/<dbname>/schema/<schema>/table/<table>')
 def get_table(pgpool, dbname, schema, table):
-    conn = pgpool.getconn(dbname)
-    ret = functions.get_table(conn, schema, table)
-    ret.update(**functions.get_table_indexes(conn, schema, table))
+    for getconn in pgpool.auto_reconnect():
+        with getconn(dbname) as conn:
+            ret = functions.get_table(conn, schema, table)
+            ret.update(**functions.get_table_indexes(conn, schema, table))
     return ret
 
 
 @bottle.post('/<dbname>/vacuum')
 def post_vacuum_database(pgpool, dbname):
     return post_vacuum(pgpool, request.json, dbname)
 
@@ -79,16 +83,18 @@
     dt = post.get('datetime', datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%SZ"))
     if 'mode' in post:
         validate_parameters(post, [
             ('mode', T_VACUUM_MODE, False),
         ])
     mode = post.get('mode', '')
 
-    return functions.schedule_vacuum(
-        pgpool.getconn(dbname), dbname, mode, dt, app, schema, table)
+    for getconn in pgpool.auto_reconnect():
+        with getconn(dbname) as conn:
+            return functions.schedule_vacuum(
+                conn, dbname, mode, dt, app, schema, table)
 
 
 @bottle.get('/<dbname>/vacuum/scheduled')
 def scheduled_vacuum_database(dbname):
     app = default_app().temboard
     return functions.list_scheduled_vacuum(app, dbname=dbname)
 
@@ -131,17 +137,18 @@
     app = default_app().temboard
     # Parameters format validation
     if 'datetime' in post:
         validate_parameters(post, [
             ('datetime', T_TIMESTAMP_UTC, False),
         ])
     dt = post.get('datetime', datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%SZ"))
-
-    conn = pgpool.getconn(dbname)
-    return functions.schedule_analyze(conn, dbname, dt, app, schema, table)
+    for getconn in pgpool.auto_reconnect():
+        with getconn(dbname) as conn:
+            return functions.schedule_analyze(
+                conn, dbname, dt, app, schema, table)
 
 
 @bottle.get('/<dbname>/analyze/scheduled')
 def scheduled_analyze_database(dbname):
     app = default_app().temboard
     return functions.list_scheduled_analyze(app, dbname=dbname)
 
@@ -191,16 +198,18 @@
     # Parameters format validation
     if 'datetime' in post:
         validate_parameters(post, [
             ('datetime', T_TIMESTAMP_UTC, False),
         ])
     dt = post.get('datetime', datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%SZ"))
 
-    return functions.schedule_reindex(
-        pgpool.getconn(dbname), dbname, dt, app, schema, table, index)
+    for getconn in pgpool.auto_reconnect():
+        with getconn(dbname) as conn:
+            return functions.schedule_reindex(
+                conn, dbname, dt, app, schema, table, index)
 
 
 @bottle.get('/<dbname>/reindex/scheduled')
 def scheduled_reindex_database(dbname):
     app = default_app().temboard
     return functions.list_scheduled_reindex(app, dbname=dbname)
```

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/maintenance/functions.py` & `temboard-agent-8.1b1/temboardagent/plugins/maintenance/functions.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/monitoring/__init__.py` & `temboard-agent-8.1b1/temboardagent/plugins/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/monitoring/db.py` & `temboard-agent-8.1b1/temboardagent/plugins/monitoring/db.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/monitoring/inventory.py` & `temboard-agent-8.1b1/temboardagent/plugins/monitoring/inventory.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/monitoring/openmetrics.py` & `temboard-agent-8.1b1/temboardagent/plugins/monitoring/openmetrics.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/monitoring/probes.py` & `temboard-agent-8.1b1/temboardagent/plugins/monitoring/probes.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
     def check(self):
         """Check if the probe can run on this system."""
         if self.system is not None:
             if self.system != os.uname()[0]:
                 return False
 
         version = [int(x) for x
-                   in re.sub(r'[-_].*$', '', os.uname()[2]).split('.')]
+                   in re.sub(r'[-_+].*$', '', os.uname()[2]).split('.')]
         if self.min_version is not None:
             if version[0:len(self.min_version)] < self.min_version:
                 return False
 
         if self.max_version is not None:
             if version[0:len(self.max_version)] > self.max_version:
                 return False
```

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/pgconf/__init__.py` & `temboard-agent-8.1b1/temboardagent/plugins/pgconf/__init__.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/pgconf/filemgmt.py` & `temboard-agent-8.1b1/temboardagent/plugins/pgconf/filemgmt.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/pgconf/functions.py` & `temboard-agent-8.1b1/temboardagent/plugins/pgconf/functions.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/plugins/statements/__init__.py` & `temboard-agent-8.1b1/temboardagent/plugins/statements/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,16 +26,17 @@
     """Return a snapshot of latest statistics of executed SQL statements
     """
     app = default_app().temboard
     config = app.config
     dbname = config.statements.dbname
     snapshot_datetime = now()
     try:
-        conn = pgpool.getconn(dbname)
-        data = list(conn.query(query))
+        for connect in pgpool.auto_reconnect():
+            with connect(dbname) as conn:
+                data = list(conn.query(query))
     except Exception as e:
         discover = app.discover.ensure_latest()
         pg_version = discover['postgres']['version_num']
         if (
             pg_version < 90600 or
             'relation "pg_stat_statements" does not exist' in str(e)
         ):
```

### Comparing `temboard-agent-8.0b6/temboardagent/postgres.py` & `temboard-agent-8.1b1/temboardagent/postgres.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,50 +101,14 @@
         )
 
     def notify_observers(self):
         for observer in self.connection_lost_observers:
             observer()
 
 
-class DBConnectionPool:
-    # Pool one connection per database.
-    #
-    # Not thread-safe.
-
-    def __init__(self, postgres):
-        self.postgres = postgres
-        self.pool = dict()
-
-    def getconn(self, dbname=None):
-        dbname = dbname or self.postgres.dbname
-        conn = self.pool.get(dbname)
-        if not conn:
-            logger.debug("Opening connection to db %s.", dbname)
-            pqvars = self.postgres.pqvars(dbname=dbname)
-            conn = retry_connect(connect, self.postgres.app, **pqvars)
-            self.pool[dbname] = conn
-
-        return conn
-
-    def closeall(self):
-        for dbname in list(self.pool):
-            conn = self.pool.pop(dbname)
-            logger.debug("Closing pooled connection to %s.", dbname)
-            conn.close()
-
-    def __del__(self):
-        self.closeall()
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, *_):
-        self.closeall()
-
-
 class FactoryConnection(psycopg2.extensions.connection):  # pragma: nocover
     def cursor(self, *a, **kw):
         row_factory = kw.pop('row_factory', None)
         kw['cursor_factory'] = FactoryCursor.make_factory(
             row_factory=row_factory)
         return super(FactoryConnection, self).cursor(*a, **kw)
 
@@ -202,76 +166,106 @@
 
 
 def scalar(**kw):
     # Row factory for scalar.
     return next(iter(kw.values()))
 
 
-class RetryManager(object):
-    def __init__(self, pool):
-        self.pool = pool
-        self.conn = None
-        self.retry = False
-
-    def __call__(self):
-        return self
-
-    def __enter__(self):
-        self.conn = self.pool.getconn()
-        self.retry = False
-        return self.conn
-
-    def __exit__(self, exc_type, e, exc_tb):
-        if isinstance(e, Psycopg2Error):
-            if e.pgcode is None:
-                logger.debug("Retrying lost connection: %s", e)
-                self.pool.close_all_connections()
-                self.conn = None
-                self.retry = True
-                return True
-
-        # Else, just clean conn and let exception bubble.
-        self.pool.putconn(self.conn)
-        self.conn = None
-
-
 class ConnectionPool(ThreadedConnectionPool):
     def __init__(self, app, observers=None, **kw):
         self.app = app
         self.observers = observers
         super(ConnectionPool, self).__init__(**kw)
 
     def _connect(self, *a, **kw):
         return retry_connect(
             super(ConnectionPool, self)._connect, self.app, *a, **kw)
 
-    def retry_connection(self):
-        # Helper to retry a code block on connection lost.
+    def auto_reconnect(self):
+        # Helper to recover a connection lost in a code block
         #
         # Manage pooled connection lost. Yield a context manager for one or two
         # attempt. The first attempt uses the connection as returned by the
         # pool. The second attempt closes pool and request a fresh connection.
         #
-        # for attempt in postgres.retry_connection_pool():
+        # for attempt in pool.auto_reconnect():
         #     with attempt() as conn:
         #         conn.queryscalar("SELECT 1")
         #
-        manager = RetryManager(self)
+        manager = ReconnectManager(self)
         for try_ in 0, 1:
             yield manager
             if not manager.retry:
                 break
 
-    def close_all_connections(self):
+    def closeall(self):
         # Close all connection, keeping pool opened.
         for conn in self._pool + list(self._used.values()):
             conn.close()
             self.putconn(conn)
 
 
+class DBConnectionPool:
+    # Pool one connection per database.
+    #
+    # Not thread-safe.
+
+    def __init__(self, postgres):
+        self.postgres = postgres
+        self.pool = dict()
+
+    def getconn(self, dbname=None):
+        dbname = dbname or self.postgres.dbname
+        conn = self.pool.get(dbname)
+        if not conn:
+            logger.debug("Opening connection to db %s.", dbname)
+            pqvars = self.postgres.pqvars(dbname=dbname)
+            conn = retry_connect(connect, self.postgres.app, **pqvars)
+            self.pool[dbname] = conn
+
+        return conn
+
+    def auto_reconnect(self, dbname=None):
+        # Helper to recover a connection lost in a code block
+        #
+        # Manage pooled connection lost. Yield a context manager for one or two
+        # attempt. The first attempt uses the connection as returned by the
+        # pool. The second attempt closes pool and request a fresh connection.
+        #
+        # for attempt in dbpool.auto_reconnect():
+        #     with attempt() as conn:
+        #         conn.queryscalar("SELECT 1")
+        #
+        manager = ReconnectManager(self, dbname)
+        for try_ in 0, 1:
+            yield manager
+            if not manager.retry:
+                break
+
+    def putconn(self, *_):
+        # Keep a single connection open, per database. Closes only upon pool
+        # closing.
+        pass
+
+    def closeall(self):
+        for dbname in list(self.pool):
+            conn = self.pool.pop(dbname)
+            logger.debug("Closing pooled connection to %s.", dbname)
+            conn.close()
+
+    def __del__(self):
+        self.closeall()
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *_):
+        self.closeall()
+
+
 def retry_connect(connect, app, *a, **kw):
     # Retry 3 times, 1 second wait between each try. This allows to wait for
     # Postgres to restart, but give up to consider Postgres as unavailable.
     for wait in [1] * 3 + [0]:
         try:
             conn = connect(*a, **kw)
             if not app.status.data['postgres']['available']:
@@ -283,7 +277,38 @@
         except Exception as e:
             app.status.data['postgres']['available'] = False
             if wait:
                 logger.debug("Retrying connection open in %ss: %s", wait, e)
                 sleep(wait)
             else:  # Last wait is 0. Just give up.
                 raise
+
+
+class ReconnectManager(object):
+    def __init__(self, pool, *connect_args):
+        self.pool = pool
+        self.connect_args = connect_args
+        self.conn = None
+        self.retry = False
+
+    def __call__(self, *connect_args):
+        if connect_args:
+            self.connect_args = connect_args
+        return self
+
+    def __enter__(self):
+        self.conn = self.pool.getconn(*self.connect_args)
+        self.retry = False
+        return self.conn
+
+    def __exit__(self, exc_type, e, exc_tb):
+        if isinstance(e, Psycopg2Error):
+            if e.pgcode is None:
+                logger.debug("Retrying lost connection: %s", e)
+                self.pool.closeall()
+                self.conn = None
+                self.retry = True
+                return True
+
+        # Else, just clean conn and let exception bubble.
+        self.pool.putconn(self.conn)
+        self.conn = None
```

### Comparing `temboard-agent-8.0b6/temboardagent/queries/activity-locks.sql` & `temboard-agent-8.1b1/temboardagent/queries/activity-locks.sql`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/queries/activity-sessions.sql` & `temboard-agent-8.1b1/temboardagent/queries/activity-sessions.sql`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/toolkit/app.py` & `temboard-agent-8.1b1/temboardagent/toolkit/app.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/toolkit/configuration.py` & `temboard-agent-8.1b1/temboardagent/toolkit/configuration.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/toolkit/http.py` & `temboard-agent-8.1b1/temboardagent/toolkit/http.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/toolkit/log.py` & `temboard-agent-8.1b1/temboardagent/toolkit/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from logging.handlers import SysLogHandler
 import sys
 
 
 class ColoredStreamHandler(logging.StreamHandler):
 
     _color_map = {  # Colors code from systemctl/journalctl
-        logging.DEBUG: '38;5;245',
-        logging.INFO: '1;39',
+        logging.DEBUG: '2',
+        logging.INFO: '1',
         logging.WARN: '38;5;185',
         logging.ERROR: '31',
         logging.CRITICAL: '1;91',
     }
 
     def format(self, record):
         lines = logging.StreamHandler.format(self, record)
```

### Comparing `temboard-agent-8.0b6/temboardagent/toolkit/perf.py` & `temboard-agent-8.1b1/temboardagent/toolkit/perf.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/toolkit/proctitle.py` & `temboard-agent-8.1b1/temboardagent/toolkit/proctitle.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/toolkit/pycompat.py` & `temboard-agent-8.1b1/temboardagent/toolkit/pycompat.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/toolkit/queries.py` & `temboard-agent-8.1b1/temboardagent/toolkit/queries.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
         for path in self.iter_files():
             filename = os.path.basename(path)
             name, ext = os.path.splitext(filename)
             with open(path) as fo:
                 if pg_version:
                     sql = ''.join(filter(
-                        lambda l: filter_pragma_version(l, pg_version),
+                        lambda line: filter_pragma_version(line, pg_version),
                         fo,
                     ))
                 else:
                     sql = fo.read()
             self[name] = fmt % (path, sql)
 
     def iter_files(self):
```

### Comparing `temboard-agent-8.0b6/temboardagent/toolkit/services.py` & `temboard-agent-8.1b1/temboardagent/toolkit/services.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/toolkit/signing.py` & `temboard-agent-8.1b1/temboardagent/toolkit/signing.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/toolkit/tasklist/sqlite3_engine.py` & `temboard-agent-8.1b1/temboardagent/toolkit/tasklist/sqlite3_engine.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/toolkit/taskmanager.py` & `temboard-agent-8.1b1/temboardagent/toolkit/taskmanager.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/toolkit/utils.py` & `temboard-agent-8.1b1/temboardagent/toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/toolkit/validators.py` & `temboard-agent-8.1b1/temboardagent/toolkit/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     return raw
 
 
 def fqdn(raw):
     if '\n' in raw:
         raise ValueError("New line in FQDN.")
     if not re.match(
-        r"(?=^.{4,253}$)"  # check length between 4 and 253
+        r"(?=^.{1,253}$)"  # check length between 4 and 253
         r"(^((?!-)[a-zA-Z0-9-]{1,63}(?<!-))"
         r"(\.(?!-)[a-zA-Z0-9-]{1,63}(?<!-))*$)",
         raw,
     ):
         raise ValueError("%s is not an FQDN" % raw)
     return raw
```

### Comparing `temboard-agent-8.0b6/temboardagent/toolkit/versions.py` & `temboard-agent-8.1b1/temboardagent/toolkit/versions.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/tools.py` & `temboard-agent-8.1b1/temboardagent/tools.py`

 * *Files identical despite different names*

### Comparing `temboard-agent-8.0b6/temboardagent/web/app.py` & `temboard-agent-8.1b1/temboardagent/web/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,50 +6,75 @@
 
 from bottle import (
     Bottle,
     HTTPError, HTTPResponse, Response,
     default_app, request, response,
 )
 
-from ..toolkit.utils import JSONEncoder, utcnow
 from ..toolkit.http import format_date
-from ..toolkit.signing import (
-    InvalidSignature,
-    canonicalize_request,
-    verify_v1,
-)
+from ..toolkit.signing import InvalidSignature, canonicalize_request, verify_v1
+from ..toolkit.utils import JSONEncoder, utcnow
 
+# getfullargspec does not exist in python <= 2.7
+# getargspec no longer exist in python 3.11
+getargspec = (
+    inspect.getfullargspec
+    if not hasattr(inspect, "getargspec")
+    else inspect.getargspec
+)
 
 logger = logging.getLogger(__name__)
 
 
 def create_app(temboard):
     Response.default_content_type = 'text/plain'
     app = CustomBottle(autojson=False)
     app.temboard = temboard
     app.add_hook('before_request', before_request_log)
-    app.add_hook('after_request', after_request_log)
     # First declared, first executed.
     app.install(JSONPlugin())
-    app.install(ErrorPlugin())
     app.install(SignaturePlugin())
     app.install(PostgresPlugin())
     return app
 
 
 class CustomBottle(Bottle):
     def default_error_handler(self, res):
         # Skip HTML template.
-        return res.body
+
+        headers = response.headers.dict.copy()
+        headers['Content-Type'] = 'application/json'
+
+        # res.exception is set by the bottle's catchall
+        if res.exception:
+            logger.exception(
+                "Unhandled error:",
+                exc_info=res.exception
+            )
+        if isinstance(res.body, str):
+            res.body = {'error': res.body}
+        return HTTPResponse(
+            json.dumps(res.body),
+            res.status,
+            headers=headers
+        )
 
     def mount(self, prefix, app, **options):
         for plugin in self.plugins:
             app.install(plugin)
         return super(CustomBottle, self).mount(prefix, app, **options)
 
+    def wsgi(self, environ, start_response):
+        # We don't use after_request hook because it doesn't handle errors
+        # correctly, for example we were seeing 200 status request in log
+        # but error 500 on web page.
+        result = super().wsgi(environ, start_response)
+        after_request_log()
+        return result
+
 
 def before_request_log():
     logger.debug("New web request: %s %s", request.method, request.path)
 
 
 def after_request_log():
     if response.status_code > 500:
@@ -85,53 +110,32 @@
         def wrapper(*a, **kw):
             if 'pgpool' in wanted:
                 # dbpool is not threadsafe! But wsgiref simple server is
                 # not threaded.
                 kw['pgpool'] = self.dbpool
 
             # Assume callbacks idempotence.
-            for attempt in self.pool.retry_connection():
+            for attempt in self.pool.auto_reconnect():
                 with attempt() as conn:
                     if 'pgconn' in wanted:
                         kw['pgconn'] = conn
 
                     return callback(*a, **kw)
 
                 if attempt.retry:
                     # Propagate connection lost to dbpool.
                     self.dbpool.closeall()
 
         return wrapper
 
     def wants_postgres(self, callback):
-        argspec = inspect.getargspec(callback)
+        argspec = getargspec(callback)
         return [a for a in argspec.args if a in ('pgconn', 'pgpool')]
 
 
-class ErrorPlugin(object):
-    def apply(self, callback, route):
-        @functools.wraps(callback)
-        def wrapper(*a, **kw):
-            try:
-                response = callback(*a, **kw)
-            except HTTPError as e:
-                if isinstance(e.body, str):
-                    e.body = {'error': e.body}
-                # Use HTTPResponse to customize body.
-                response = HTTPResponse(e.body, e.status)
-            except HTTPResponse as e:
-                response = e
-            except Exception:
-                logger.exception("Unhandled error:")
-                response = HTTPResponse({'error': 'Internal error.'}, 500)
-
-            return response
-        return wrapper
-
-
 class JSONPlugin(object):
     # Bottle jsonify only dict. JSON Array was a security issue for some
     # browser.
     def apply(self, callback, route):
         @functools.wraps(callback)
         def wrapper(*a, **kw):
             res = callback(*a, **kw)
```

### Comparing `temboard-agent-8.0b6/temboardagent/web/core.py` & `temboard-agent-8.1b1/temboardagent/web/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 import logging
 
-from bottle import default_app, get, post, request, response
+from bottle import (
+    default_app, get, post, request, response, HTTPError, HTTPResponse
+)
 
 from ..notification import NotificationMgmt
 from ..toolkit.signing import canonicalize_request, verify_v1, InvalidSignature
 from ..version import __version__ as version
 
 
 logger = logging.getLogger(__name__)
 
 
+@get('/error/<error_code:int>', skip=['signature'])
+def get_error(error_code):
+    if error_code < 400:
+        raise HTTPResponse('HTTPResponse raised', error_code)
+    elif error_code < 500:
+        raise HTTPError(error_code, 'HTTPError raised')
+    else:
+        raise Exception("This is an Exception %s" % error_code)
+
+
 @get('/discover', skip=['signature'])
 def get_discover():
     app = default_app().temboard
     discover = app.discover.ensure_latest().copy()
     discover['signature_status'] = 'enabled'
 
     signature = request.headers.get('x-temboard-signature')
```

### Comparing `temboard-agent-8.0b6/temboardagent/web/service.py` & `temboard-agent-8.1b1/temboardagent/web/service.py`

 * *Files identical despite different names*

