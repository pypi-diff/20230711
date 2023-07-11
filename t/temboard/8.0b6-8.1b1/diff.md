# Comparing `tmp/temboard-8.0b6.tar.gz` & `tmp/temboard-8.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temboard-8.0b6.tar", last modified: Thu Nov  3 09:18:33 2022, max compression
+gzip compressed data, was "temboard-8.1b1.tar", last modified: Tue Jul 11 12:20:07 2023, max compression
```

## Comparing `temboard-8.0b6.tar` & `temboard-8.1b1.tar`

### file list

```diff
@@ -1,282 +1,282 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.750341 temboard-8.0b6/
--rw-r--r--   0 root         (0) root         (0)     1079 2022-11-03 09:18:32.000000 temboard-8.0b6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      969 2022-11-03 09:18:32.000000 temboard-8.0b6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3713 2022-11-03 09:18:33.750341 temboard-8.0b6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2497 2022-11-03 09:18:32.000000 temboard-8.0b6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.722340 temboard-8.0b6/packaging/
--rw-r--r--   0 root         (0) root         (0)      265 2022-11-03 09:18:32.000000 temboard-8.0b6/packaging/temboard.service
--rw-r--r--   0 root         (0) root         (0)      180 2022-11-03 09:18:33.750341 temboard-8.0b6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3327 2022-11-03 09:18:32.000000 temboard-8.0b6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.722340 temboard-8.0b6/share/
--rwxr-xr-x   0 root         (0) root         (0)     5089 2022-11-03 09:18:32.000000 temboard-8.0b6/share/auto_configure.sh
--rwxr-xr-x   0 root         (0) root         (0)     2328 2022-11-03 09:18:32.000000 temboard-8.0b6/share/create_repository.sh
--rwxr-xr-x   0 root         (0) root         (0)     1350 2022-11-03 09:18:32.000000 temboard-8.0b6/share/purge.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.722340 temboard-8.0b6/share/sql/
--rw-r--r--   0 root         (0) root         (0)     2763 2022-11-03 09:18:32.000000 temboard-8.0b6/share/sql/dev-fixture.sql
--rw-r--r--   0 root         (0) root         (0)       51 2022-11-03 09:18:32.000000 temboard-8.0b6/share/sql/pg_stat_statements-create-extension.sql
--rw-r--r--   0 root         (0) root         (0)     2235 2022-11-03 09:18:32.000000 temboard-8.0b6/share/sql/reassign.sql
--rw-r--r--   0 root         (0) root         (0)      420 2022-11-03 09:18:32.000000 temboard-8.0b6/share/sql/upgrade-4-5.sql
--rw-r--r--   0 root         (0) root         (0)    37305 2022-11-03 09:18:32.000000 temboard-8.0b6/share/sql/upgrade-monitoring-purge-instances.sql
--rw-r--r--   0 root         (0) root         (0)     1615 2022-11-03 09:18:32.000000 temboard-8.0b6/share/temboard.conf
--rw-r--r--   0 root         (0) root         (0)     1704 2022-11-03 09:18:32.000000 temboard-8.0b6/share/temboard_CHANGEME.key
--rw-r--r--   0 root         (0) root         (0)     1123 2022-11-03 09:18:32.000000 temboard-8.0b6/share/temboard_CHANGEME.pem
--rw-r--r--   0 root         (0) root         (0)     1229 2022-11-03 09:18:32.000000 temboard-8.0b6/share/temboard_ca_certs_CHANGEME.pem
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.726341 temboard-8.0b6/temboard.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3713 2022-11-03 09:18:33.000000 temboard-8.0b6/temboard.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9301 2022-11-03 09:18:33.000000 temboard-8.0b6/temboard.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-03 09:18:33.000000 temboard-8.0b6/temboard.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      419 2022-11-03 09:18:33.000000 temboard-8.0b6/temboard.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-03 09:18:33.000000 temboard-8.0b6/temboard.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       81 2022-11-03 09:18:33.000000 temboard-8.0b6/temboard.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-11-03 09:18:33.000000 temboard-8.0b6/temboard.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.726341 temboard-8.0b6/temboardui/
--rw-r--r--   0 root         (0) root         (0)      165 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1577 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2116 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/agentclient.py
--rw-r--r--   0 root         (0) root         (0)    24212 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/application.py
--rw-r--r--   0 root         (0) root         (0)    11762 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/autossl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.726341 temboard-8.0b6/temboardui/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2994 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/cli/apikey.py
--rw-r--r--   0 root         (0) root         (0)    14683 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/cli/app.py
--rw-r--r--   0 root         (0) root         (0)     1421 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/cli/generate_key.py
--rw-r--r--   0 root         (0) root         (0)     1489 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/cli/migratedb.py
--rw-r--r--   0 root         (0) root         (0)     2051 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/cli/query_agent.py
--rw-r--r--   0 root         (0) root         (0)     7553 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/cli/register_instance.py
--rw-r--r--   0 root         (0) root         (0)     1524 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/cli/routes.py
--rw-r--r--   0 root         (0) root         (0)      843 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/cli/serve.py
--rw-r--r--   0 root         (0) root         (0)     2672 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/cli/tasks.py
--rw-r--r--   0 root         (0) root         (0)      582 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/cli/web.py
--rw-r--r--   0 root         (0) root         (0)     1284 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/core.py
--rw-r--r--   0 root         (0) root         (0)     2350 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/daemon.py
--rw-r--r--   0 root         (0) root         (0)      372 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.726341 temboard-8.0b6/temboardui/handlers/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      329 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/handlers/core.py
--rw-r--r--   0 root         (0) root         (0)     1287 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/handlers/home.py
--rw-r--r--   0 root         (0) root         (0)      577 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/handlers/notification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.726341 temboard-8.0b6/temboardui/handlers/settings/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/handlers/settings/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3478 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/handlers/settings/group.py
--rw-r--r--   0 root         (0) root         (0)     9154 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/handlers/settings/instance.py
--rw-r--r--   0 root         (0) root         (0)     1034 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/handlers/settings/metadata.py
--rw-r--r--   0 root         (0) root         (0)     1698 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/handlers/settings/notifications.py
--rw-r--r--   0 root         (0) root         (0)     5169 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/handlers/settings/user.py
--rw-r--r--   0 root         (0) root         (0)     4205 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/handlers/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.726341 temboard-8.0b6/temboardui/model/
--rw-r--r--   0 root         (0) root         (0)     2457 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3407 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/migrator.py
--rw-r--r--   0 root         (0) root         (0)     9705 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/orm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.730341 temboard-8.0b6/temboardui/model/queries/
--rw-r--r--   0 root         (0) root         (0)       80 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/queries/apikeys-delete.sql
--rw-r--r--   0 root         (0) root         (0)       97 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/queries/apikeys-insert.sql
--rw-r--r--   0 root         (0) root         (0)       85 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/queries/apikeys-purge.sql
--rw-r--r--   0 root         (0) root         (0)       95 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/queries/apikeys-select-active.sql
--rw-r--r--   0 root         (0) root         (0)       98 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/queries/apikeys-select-secret.sql
--rw-r--r--   0 root         (0) root         (0)      977 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/queries/copy-instances-as-csv.sql
--rw-r--r--   0 root         (0) root         (0)     5022 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/tables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.730341 temboard-8.0b6/temboardui/model/versions/
--rw-r--r--   0 root         (0) root         (0)      197 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/versions/000_init.sql
--rw-r--r--   0 root         (0) root         (0)     3243 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/versions/001_application.sql
--rw-r--r--   0 root         (0) root         (0)    48335 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/versions/002_monitoring.sql
--rw-r--r--   0 root         (0) root         (0)     5894 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/versions/003_alerting.sql
--rw-r--r--   0 root         (0) root         (0)    13351 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/versions/005_statements.sql
--rw-r--r--   0 root         (0) root         (0)      212 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/versions/007_drop-alembic.sql
--rw-r--r--   0 root         (0) root         (0)      938 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/versions/008_monitoring-archive-wait-lock.sql
--rw-r--r--   0 root         (0) root         (0)      245 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/versions/009_apikey.sql
--rw-r--r--   0 root         (0) root         (0)      761 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/model/versions/010_discover.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.730341 temboard-8.0b6/temboardui/plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.730341 temboard-8.0b6/temboardui/plugins/activity/
--rw-r--r--   0 root         (0) root         (0)     1390 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/activity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.730341 temboard-8.0b6/temboardui/plugins/activity/templates/
--rw-r--r--   0 root         (0) root         (0)     4542 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/activity/templates/activity.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.730341 temboard-8.0b6/temboardui/plugins/dashboard/
--rw-r--r--   0 root         (0) root         (0)     1832 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/dashboard/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.722340 temboard-8.0b6/temboardui/plugins/dashboard/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.730341 temboard-8.0b6/temboardui/plugins/dashboard/static/js/
--rw-r--r--   0 root         (0) root         (0)    12634 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/dashboard/static/js/temboard.dashboard.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.730341 temboard-8.0b6/temboardui/plugins/dashboard/templates/
--rw-r--r--   0 root         (0) root         (0)    10085 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/dashboard/templates/dashboard.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.730341 temboard-8.0b6/temboardui/plugins/maintenance/
--rw-r--r--   0 root         (0) root         (0)     3484 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.722340 temboard-8.0b6/temboardui/plugins/maintenance/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.730341 temboard-8.0b6/temboardui/plugins/maintenance/static/js/
--rw-r--r--   0 root         (0) root         (0)     9348 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/static/js/temboard.maintenance.database.js
--rw-r--r--   0 root         (0) root         (0)      357 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/static/js/temboard.maintenance.errors.js
--rw-r--r--   0 root         (0) root         (0)     2035 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/static/js/temboard.maintenance.js
--rw-r--r--   0 root         (0) root         (0)     5872 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/static/js/temboard.maintenance.schema.js
--rw-r--r--   0 root         (0) root         (0)    10188 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/static/js/temboard.maintenance.table.js
--rw-r--r--   0 root         (0) root         (0)      275 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/static/js/vue.filter.relative-time.js
--rw-r--r--   0 root         (0) root         (0)     2532 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/static/js/vue.size-distribution-bar.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.730341 temboard-8.0b6/temboardui/plugins/maintenance/templates/
--rw-r--r--   0 root         (0) root         (0)     1473 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/templates/breadcrumb.html
--rw-r--r--   0 root         (0) root         (0)     8301 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/templates/database.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.734341 temboard-8.0b6/temboardui/plugins/maintenance/templates/includes/
--rw-r--r--   0 root         (0) root         (0)     2318 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/templates/includes/analyze_modal.html
--rw-r--r--   0 root         (0) root         (0)     2507 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/templates/includes/reindex_modal.html
--rw-r--r--   0 root         (0) root         (0)     1785 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/templates/includes/scheduled_analyze.html
--rw-r--r--   0 root         (0) root         (0)     2179 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/templates/includes/scheduled_reindex.html
--rw-r--r--   0 root         (0) root         (0)     1846 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/templates/includes/scheduled_vacuum.html
--rw-r--r--   0 root         (0) root         (0)     3959 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/templates/includes/vacuum_modal.html
--rw-r--r--   0 root         (0) root         (0)     6671 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/templates/index.html
--rw-r--r--   0 root         (0) root         (0)    11657 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/templates/schema.html
--rw-r--r--   0 root         (0) root         (0)    11926 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/maintenance/templates/table.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.734341 temboard-8.0b6/temboardui/plugins/monitoring/
--rw-r--r--   0 root         (0) root         (0)    22322 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11834 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/alerting.py
--rw-r--r--   0 root         (0) root         (0)    36201 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/chartdata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.734341 temboard-8.0b6/temboardui/plugins/monitoring/handlers/
--rw-r--r--   0 root         (0) root         (0)      200 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9003 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/handlers/alerting.py
--rw-r--r--   0 root         (0) root         (0)     2058 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/handlers/monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.734341 temboard-8.0b6/temboardui/plugins/monitoring/model/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14860 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/model/db.py
--rw-r--r--   0 root         (0) root         (0)     2601 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/model/orm.py
--rw-r--r--   0 root         (0) root         (0)     2806 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/model/tables.py
--rw-r--r--   0 root         (0) root         (0)     1163 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/pivot.py
--rw-r--r--   0 root         (0) root         (0)      224 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/routes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.722340 temboard-8.0b6/temboardui/plugins/monitoring/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.734341 temboard-8.0b6/temboardui/plugins/monitoring/static/js/
--rw-r--r--   0 root         (0) root         (0)     3335 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/static/js/datemath.js
--rw-r--r--   0 root         (0) root         (0)     9101 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/static/js/daterangepicker.vue.js
--rw-r--r--   0 root         (0) root         (0)     5756 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/static/js/rangeutils.js
--rw-r--r--   0 root         (0) root         (0)    11576 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/static/js/temboard.check.js
--rw-r--r--   0 root         (0) root         (0)      707 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/static/js/temboard.checks.js
--rw-r--r--   0 root         (0) root         (0)    12434 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/static/js/temboard.monitoring.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.734341 temboard-8.0b6/temboardui/plugins/monitoring/templates/
--rw-r--r--   0 root         (0) root         (0)     5365 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/templates/alerting.check.html
--rw-r--r--   0 root         (0) root         (0)     1888 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/templates/alerting.checks.html
--rw-r--r--   0 root         (0) root         (0)     5328 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/templates/index.html
--rw-r--r--   0 root         (0) root         (0)    14507 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/monitoring/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.734341 temboard-8.0b6/temboardui/plugins/pgconf/
--rw-r--r--   0 root         (0) root         (0)     3116 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/pgconf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.722340 temboard-8.0b6/temboardui/plugins/pgconf/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.734341 temboard-8.0b6/temboardui/plugins/pgconf/static/css/
--rw-r--r--   0 root         (0) root         (0)       33 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/pgconf/static/css/temboard.pgconf.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.734341 temboard-8.0b6/temboardui/plugins/pgconf/static/js/
--rw-r--r--   0 root         (0) root         (0)     1911 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/pgconf/static/js/temboard.pgconf.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.734341 temboard-8.0b6/temboardui/plugins/pgconf/templates/
--rw-r--r--   0 root         (0) root         (0)    10865 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/pgconf/templates/configuration.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.734341 temboard-8.0b6/temboardui/plugins/statements/
--rw-r--r--   0 root         (0) root         (0)    28007 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/statements/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.722340 temboard-8.0b6/temboardui/plugins/statements/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.734341 temboard-8.0b6/temboardui/plugins/statements/static/js/
--rw-r--r--   0 root         (0) root         (0)     9001 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/statements/static/js/temboard.statements.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.734341 temboard-8.0b6/temboardui/plugins/statements/templates/
--rw-r--r--   0 root         (0) root         (0)     6155 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/plugins/statements/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.738341 temboard-8.0b6/temboardui/static/
--rw-r--r--   0 root         (0) root         (0)     1324 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/Error.20e0c905.js
--rw-r--r--   0 root         (0) root         (0)      129 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/_commonjsHelpers.04e31c8c.js
--rw-r--r--   0 root         (0) root         (0)     1145 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/activity.d1cda23a.css
--rw-r--r--   0 root         (0) root         (0)  1052919 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/activity.d489418d.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.742341 temboard-8.0b6/temboardui/static/css/
--rw-r--r--   0 root         (0) root         (0)     1509 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/css/bootstrap-multiselect.css
--rw-r--r--   0 root         (0) root         (0)    22608 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/css/bootstrap-theme.css
--rw-r--r--   0 root         (0) root         (0)    43339 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/css/bootstrap-theme.css.map
--rw-r--r--   0 root         (0) root         (0)    19963 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/css/bootstrap-theme.min.css
--rw-r--r--   0 root         (0) root         (0)     1590 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/css/bootstrap-toggle.min.css
--rw-r--r--   0 root         (0) root         (0)    66677 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/css/bootstrap-vue.min.css
--rw-r--r--   0 root         (0) root         (0)   162264 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   654593 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/css/bootstrap.min.css.map
--rw-r--r--   0 root         (0) root         (0)     2642 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/css/dygraph.css
--rw-r--r--   0 root         (0) root         (0)    10766 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/dataTables.0be85286.css
--rw-r--r--   0 root         (0) root         (0)   181164 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/dataTables.bootstrap4.9ae7027a.js
--rw-r--r--   0 root         (0) root         (0)    77160 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/fontawesome-webfont.2adefcbc.woff2
--rw-r--r--   0 root         (0) root         (0)   165742 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/fontawesome-webfont.7bfcab6d.eot
--rw-r--r--   0 root         (0) root         (0)   165548 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/fontawesome-webfont.aa58f33f.ttf
--rw-r--r--   0 root         (0) root         (0)   444379 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/fontawesome-webfont.ad615792.svg
--rw-r--r--   0 root         (0) root         (0)    98024 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/fontawesome-webfont.ba0c59de.woff
--rw-r--r--   0 root         (0) root         (0)   285375 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/home.31a23655.js
--rw-r--r--   0 root         (0) root         (0)     1222 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/home.a0d294e3.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.742341 temboard-8.0b6/temboardui/static/images/
--rw-r--r--   0 root         (0) root         (0)      529 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/images/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    61261 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/images/heron.png
--rw-r--r--   0 root         (0) root         (0)      609 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/images/ring-alt.svg
--rw-r--r--   0 root         (0) root         (0)      160 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/images/sort_asc.png
--rw-r--r--   0 root         (0) root         (0)      148 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/images/sort_asc_disabled.png
--rw-r--r--   0 root         (0) root         (0)      201 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/images/sort_both.png
--rw-r--r--   0 root         (0) root         (0)      158 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/images/sort_desc.png
--rw-r--r--   0 root         (0) root         (0)      146 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/images/sort_desc_disabled.png
--rw-r--r--   0 root         (0) root         (0)     3217 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/images/temboard-150x32-w.png
--rw-r--r--   0 root         (0) root         (0)    24047 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/images/temboard-logo.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.746341 temboard-8.0b6/temboardui/static/js/
--rw-r--r--   0 root         (0) root         (0)   159638 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/Chart.min.js
--rw-r--r--   0 root         (0) root         (0)    15369 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/Sortable.min.js
--rw-r--r--   0 root         (0) root         (0)    68977 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/bootstrap-multiselect.js
--rw-r--r--   0 root         (0) root         (0)     4129 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/bootstrap-toggle.min.js
--rw-r--r--   0 root         (0) root         (0)   363092 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/bootstrap-vue.min.js
--rw-r--r--   0 root         (0) root         (0)    62563 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/bootstrap.min.js
--rw-r--r--   0 root         (0) root         (0)   185257 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/bootstrap.min.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.746341 temboard-8.0b6/temboardui/static/js/datatables/
--rw-r--r--   0 root         (0) root         (0)    20297 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/datatables/datatables.min.css
--rw-r--r--   0 root         (0) root         (0)   147324 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/datatables/datatables.min.js
--rw-r--r--   0 root         (0) root         (0)    69586 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/daterangepicker.js
--rw-r--r--   0 root         (0) root         (0)   123910 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/dygraph.min.js
--rw-r--r--   0 root         (0) root         (0)     1355 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/filesize.min.js
--rw-r--r--   0 root         (0) root         (0)     2519 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/fscreen.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.746341 temboard-8.0b6/temboardui/static/js/highlightjs/
--rw-r--r--   0 root         (0) root         (0)     1159 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/highlightjs/default.css
--rw-r--r--   0 root         (0) root         (0)    19707 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/highlightjs/highlight.pack.js
--rw-r--r--   0 root         (0) root         (0)    84345 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/jquery-2.1.4.min.js
--rw-r--r--   0 root         (0) root         (0)    73157 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/lodash.min.js
--rw-r--r--   0 root         (0) root         (0)    40732 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/moment.min.js
--rw-r--r--   0 root         (0) root         (0)     2958 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/moment.preciseDiff.js
--rw-r--r--   0 root         (0) root         (0)    19188 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/popper.min.js
--rw-r--r--   0 root         (0) root         (0)    16337 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/temboard.settings.group.js
--rw-r--r--   0 root         (0) root         (0)      966 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/temboard.settings.notifications.js
--rw-r--r--   0 root         (0) root         (0)    17547 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/temboard.settings.user.js
--rw-r--r--   0 root         (0) root         (0)    24084 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/vue-router.min.js
--rw-r--r--   0 root         (0) root         (0)    93670 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/vue.min.js
--rw-r--r--   0 root         (0) root         (0)     6708 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/js/vuedraggable.min.js
--rw-r--r--   0 root         (0) root         (0)     3389 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/manifest.json
--rw-r--r--   0 root         (0) root         (0)      754 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/plugin-vue2_normalizer.ed7092a9.js
--rw-r--r--   0 root         (0) root         (0)    44661 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/settings.instance.be0dadd5.js
--rw-r--r--   0 root         (0) root         (0)   214816 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/temboard.9b8cf8f1.css
--rw-r--r--   0 root         (0) root         (0)     1644 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/temboard.beba2dfa.js
--rw-r--r--   0 root         (0) root         (0)   102035 2022-11-03 09:18:06.000000 temboard-8.0b6/temboardui/static/vue.esm.6bf4157d.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.746341 temboard-8.0b6/temboardui/templates/
--rw-r--r--   0 root         (0) root         (0)     2447 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/templates/about.html
--rw-r--r--   0 root         (0) root         (0)     1893 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/templates/agent-login.html
--rw-r--r--   0 root         (0) root         (0)     7926 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/templates/base.html
--rw-r--r--   0 root         (0) root         (0)      425 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/templates/error.html
--rw-r--r--   0 root         (0) root         (0)      639 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/templates/home.html
--rw-r--r--   0 root         (0) root         (0)     4021 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/templates/instance-about.html
--rw-r--r--   0 root         (0) root         (0)     1229 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/templates/login.html
--rw-r--r--   0 root         (0) root         (0)     1046 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/templates/notifications.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.746341 temboard-8.0b6/temboardui/templates/settings/
--rw-r--r--   0 root         (0) root         (0)      454 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/templates/settings/error.html
--rw-r--r--   0 root         (0) root         (0)     3738 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/templates/settings/group.html
--rw-r--r--   0 root         (0) root         (0)     3516 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/templates/settings/instance.html
--rw-r--r--   0 root         (0) root         (0)      506 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/templates/settings/menu.html
--rw-r--r--   0 root         (0) root         (0)     1954 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/templates/settings/notifications.html
--rw-r--r--   0 root         (0) root         (0)     3972 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/templates/settings/user.html
--rw-r--r--   0 root         (0) root         (0)      471 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/templates/unauthorized.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.750341 temboard-8.0b6/temboardui/toolkit/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16397 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/app.py
--rw-r--r--   0 root         (0) root         (0)     7309 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/configuration.py
--rw-r--r--   0 root         (0) root         (0)      272 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/errors.py
--rw-r--r--   0 root         (0) root         (0)     5624 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/http.py
--rw-r--r--   0 root         (0) root         (0)     5726 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/log.py
--rw-r--r--   0 root         (0) root         (0)     2455 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/perf.py
--rw-r--r--   0 root         (0) root         (0)     8038 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/proctitle.py
--rw-r--r--   0 root         (0) root         (0)      629 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/pycompat.py
--rw-r--r--   0 root         (0) root         (0)     1886 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/queries.py
--rw-r--r--   0 root         (0) root         (0)     7118 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/services.py
--rw-r--r--   0 root         (0) root         (0)     2450 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/signing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.750341 temboard-8.0b6/temboardui/toolkit/tasklist/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/tasklist/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11784 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/tasklist/sqlite3_engine.py
--rw-r--r--   0 root         (0) root         (0)    30519 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/taskmanager.py
--rw-r--r--   0 root         (0) root         (0)     2094 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/utils.py
--rw-r--r--   0 root         (0) root         (0)     3479 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/validators.py
--rw-r--r--   0 root         (0) root         (0)     1465 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/toolkit/versions.py
--rw-r--r--   0 root         (0) root         (0)     1280 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 09:18:33.750341 temboard-8.0b6/temboardui/web/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9000 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/web/flask.py
--rw-r--r--   0 root         (0) root         (0)     4083 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/web/routes.py
--rw-r--r--   0 root         (0) root         (0)    23259 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/web/tornado.py
--rw-r--r--   0 root         (0) root         (0)     1985 2022-11-03 09:18:32.000000 temboard-8.0b6/temboardui/web/vitejs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.158332 temboard-8.1b1/
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-07-11 12:20:05.000000 temboard-8.1b1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      969 2023-07-11 12:20:05.000000 temboard-8.1b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-07-11 12:20:07.158332 temboard-8.1b1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-07-11 12:20:05.000000 temboard-8.1b1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.130332 temboard-8.1b1/packaging/
+-rw-r--r--   0 root         (0) root         (0)      270 2023-07-11 12:20:05.000000 temboard-8.1b1/packaging/temboard.service
+-rw-r--r--   0 root         (0) root         (0)      180 2023-07-11 12:20:07.158332 temboard-8.1b1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3412 2023-07-11 12:20:05.000000 temboard-8.1b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.134332 temboard-8.1b1/share/
+-rwxr-xr-x   0 root         (0) root         (0)     4695 2023-07-11 12:20:05.000000 temboard-8.1b1/share/auto_configure.sh
+-rwxr-xr-x   0 root         (0) root         (0)     2328 2023-07-11 12:20:05.000000 temboard-8.1b1/share/create_repository.sh
+-rwxr-xr-x   0 root         (0) root         (0)     1350 2023-07-11 12:20:05.000000 temboard-8.1b1/share/purge.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.134332 temboard-8.1b1/share/sql/
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-07-11 12:20:05.000000 temboard-8.1b1/share/sql/dev-fixture.sql
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-11 12:20:05.000000 temboard-8.1b1/share/sql/pg_stat_statements-create-extension.sql
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-07-11 12:20:05.000000 temboard-8.1b1/share/sql/reassign.sql
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-11 12:20:05.000000 temboard-8.1b1/share/sql/upgrade-4-5.sql
+-rw-r--r--   0 root         (0) root         (0)    37305 2023-07-11 12:20:05.000000 temboard-8.1b1/share/sql/upgrade-monitoring-purge-instances.sql
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-07-11 12:20:05.000000 temboard-8.1b1/share/temboard.conf
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-07-11 12:20:05.000000 temboard-8.1b1/share/temboard_CHANGEME.key
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-07-11 12:20:05.000000 temboard-8.1b1/share/temboard_CHANGEME.pem
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-07-11 12:20:05.000000 temboard-8.1b1/share/temboard_ca_certs_CHANGEME.pem
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.134332 temboard-8.1b1/temboard.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-07-11 12:20:07.000000 temboard-8.1b1/temboard.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9301 2023-07-11 12:20:07.000000 temboard-8.1b1/temboard.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 12:20:07.000000 temboard-8.1b1/temboard.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-11 12:20:07.000000 temboard-8.1b1/temboard.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 12:20:07.000000 temboard-8.1b1/temboard.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-11 12:20:07.000000 temboard-8.1b1/temboard.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 12:20:07.000000 temboard-8.1b1/temboard.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.134332 temboard-8.1b1/temboardui/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/agentclient.py
+-rw-r--r--   0 root         (0) root         (0)    24212 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/application.py
+-rw-r--r--   0 root         (0) root         (0)    11762 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/autossl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.134332 temboard-8.1b1/temboardui/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2994 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/cli/apikey.py
+-rw-r--r--   0 root         (0) root         (0)    14812 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/cli/app.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/cli/generate_key.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/cli/migratedb.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/cli/query_agent.py
+-rw-r--r--   0 root         (0) root         (0)     7553 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/cli/register_instance.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/cli/routes.py
+-rw-r--r--   0 root         (0) root         (0)      843 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/cli/serve.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/cli/tasks.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/cli/web.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/core.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/daemon.py
+-rw-r--r--   0 root         (0) root         (0)      372 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.138332 temboard-8.1b1/temboardui/handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      329 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/handlers/core.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/handlers/home.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/handlers/notification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.138332 temboard-8.1b1/temboardui/handlers/settings/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/handlers/settings/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/handlers/settings/group.py
+-rw-r--r--   0 root         (0) root         (0)     9154 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/handlers/settings/instance.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/handlers/settings/metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/handlers/settings/notifications.py
+-rw-r--r--   0 root         (0) root         (0)     5169 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/handlers/settings/user.py
+-rw-r--r--   0 root         (0) root         (0)     4205 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/handlers/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.138332 temboard-8.1b1/temboardui/model/
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3407 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/migrator.py
+-rw-r--r--   0 root         (0) root         (0)     9705 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/orm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.138332 temboard-8.1b1/temboardui/model/queries/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/queries/apikeys-delete.sql
+-rw-r--r--   0 root         (0) root         (0)       97 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/queries/apikeys-insert.sql
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/queries/apikeys-purge.sql
+-rw-r--r--   0 root         (0) root         (0)       95 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/queries/apikeys-select-active.sql
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/queries/apikeys-select-secret.sql
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/queries/copy-instances-as-csv.sql
+-rw-r--r--   0 root         (0) root         (0)     5022 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/tables.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.138332 temboard-8.1b1/temboardui/model/versions/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/versions/000_init.sql
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/versions/001_application.sql
+-rw-r--r--   0 root         (0) root         (0)    48335 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/versions/002_monitoring.sql
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/versions/003_alerting.sql
+-rw-r--r--   0 root         (0) root         (0)    13351 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/versions/005_statements.sql
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/versions/007_drop-alembic.sql
+-rw-r--r--   0 root         (0) root         (0)      949 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/versions/008_monitoring-archive-wait-lock.sql
+-rw-r--r--   0 root         (0) root         (0)      245 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/versions/009_apikey.sql
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/model/versions/010_discover.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.138332 temboard-8.1b1/temboardui/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.138332 temboard-8.1b1/temboardui/plugins/activity/
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/activity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.138332 temboard-8.1b1/temboardui/plugins/activity/templates/
+-rw-r--r--   0 root         (0) root         (0)     4521 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/activity/templates/activity.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.138332 temboard-8.1b1/temboardui/plugins/dashboard/
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/dashboard/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.130332 temboard-8.1b1/temboardui/plugins/dashboard/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.138332 temboard-8.1b1/temboardui/plugins/dashboard/static/js/
+-rw-r--r--   0 root         (0) root         (0)    12634 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/dashboard/static/js/temboard.dashboard.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.138332 temboard-8.1b1/temboardui/plugins/dashboard/templates/
+-rw-r--r--   0 root         (0) root         (0)    10092 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/dashboard/templates/dashboard.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.138332 temboard-8.1b1/temboardui/plugins/maintenance/
+-rw-r--r--   0 root         (0) root         (0)     3484 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.130332 temboard-8.1b1/temboardui/plugins/maintenance/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.142332 temboard-8.1b1/temboardui/plugins/maintenance/static/js/
+-rw-r--r--   0 root         (0) root         (0)     9348 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/static/js/temboard.maintenance.database.js
+-rw-r--r--   0 root         (0) root         (0)      357 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/static/js/temboard.maintenance.errors.js
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/static/js/temboard.maintenance.js
+-rw-r--r--   0 root         (0) root         (0)     5872 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/static/js/temboard.maintenance.schema.js
+-rw-r--r--   0 root         (0) root         (0)    10188 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/static/js/temboard.maintenance.table.js
+-rw-r--r--   0 root         (0) root         (0)      275 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/static/js/vue.filter.relative-time.js
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/static/js/vue.size-distribution-bar.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.142332 temboard-8.1b1/temboardui/plugins/maintenance/templates/
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/templates/breadcrumb.html
+-rw-r--r--   0 root         (0) root         (0)     8301 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/templates/database.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.142332 temboard-8.1b1/temboardui/plugins/maintenance/templates/includes/
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/templates/includes/analyze_modal.html
+-rw-r--r--   0 root         (0) root         (0)     2507 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/templates/includes/reindex_modal.html
+-rw-r--r--   0 root         (0) root         (0)     1785 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/templates/includes/scheduled_analyze.html
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/templates/includes/scheduled_reindex.html
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/templates/includes/scheduled_vacuum.html
+-rw-r--r--   0 root         (0) root         (0)     3959 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/templates/includes/vacuum_modal.html
+-rw-r--r--   0 root         (0) root         (0)     6671 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/templates/index.html
+-rw-r--r--   0 root         (0) root         (0)    11657 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/templates/schema.html
+-rw-r--r--   0 root         (0) root         (0)    11926 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/maintenance/templates/table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.142332 temboard-8.1b1/temboardui/plugins/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    22322 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11834 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/alerting.py
+-rw-r--r--   0 root         (0) root         (0)    36201 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/chartdata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.142332 temboard-8.1b1/temboardui/plugins/monitoring/handlers/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9003 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/handlers/alerting.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/handlers/monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.142332 temboard-8.1b1/temboardui/plugins/monitoring/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14860 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/model/db.py
+-rw-r--r--   0 root         (0) root         (0)     2601 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/model/orm.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/model/tables.py
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/pivot.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/routes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.130332 temboard-8.1b1/temboardui/plugins/monitoring/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.142332 temboard-8.1b1/temboardui/plugins/monitoring/static/js/
+-rw-r--r--   0 root         (0) root         (0)     3335 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/static/js/datemath.js
+-rw-r--r--   0 root         (0) root         (0)     9101 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/static/js/daterangepicker.vue.js
+-rw-r--r--   0 root         (0) root         (0)     5756 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/static/js/rangeutils.js
+-rw-r--r--   0 root         (0) root         (0)    11576 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/static/js/temboard.check.js
+-rw-r--r--   0 root         (0) root         (0)      707 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/static/js/temboard.checks.js
+-rw-r--r--   0 root         (0) root         (0)    12434 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/static/js/temboard.monitoring.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.142332 temboard-8.1b1/temboardui/plugins/monitoring/templates/
+-rw-r--r--   0 root         (0) root         (0)     5344 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/templates/alerting.check.html
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/templates/alerting.checks.html
+-rw-r--r--   0 root         (0) root         (0)     5307 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/templates/index.html
+-rw-r--r--   0 root         (0) root         (0)    14507 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/monitoring/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.142332 temboard-8.1b1/temboardui/plugins/pgconf/
+-rw-r--r--   0 root         (0) root         (0)     3116 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/pgconf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.130332 temboard-8.1b1/temboardui/plugins/pgconf/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.142332 temboard-8.1b1/temboardui/plugins/pgconf/static/css/
+-rw-r--r--   0 root         (0) root         (0)       33 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/pgconf/static/css/temboard.pgconf.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.142332 temboard-8.1b1/temboardui/plugins/pgconf/static/js/
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/pgconf/static/js/temboard.pgconf.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.142332 temboard-8.1b1/temboardui/plugins/pgconf/templates/
+-rw-r--r--   0 root         (0) root         (0)    10865 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/pgconf/templates/configuration.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.146332 temboard-8.1b1/temboardui/plugins/statements/
+-rw-r--r--   0 root         (0) root         (0)    28007 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/statements/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.130332 temboard-8.1b1/temboardui/plugins/statements/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.146332 temboard-8.1b1/temboardui/plugins/statements/static/js/
+-rw-r--r--   0 root         (0) root         (0)     9001 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/statements/static/js/temboard.statements.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.146332 temboard-8.1b1/temboardui/plugins/statements/templates/
+-rw-r--r--   0 root         (0) root         (0)     6155 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/plugins/statements/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.150332 temboard-8.1b1/temboardui/static/
+-rw-r--r--   0 root         (0) root         (0)     1324 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/Error.20e0c905.js
+-rw-r--r--   0 root         (0) root         (0)      129 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/_commonjsHelpers.04e31c8c.js
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/activity.d1cda23a.css
+-rw-r--r--   0 root         (0) root         (0)  1052919 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/activity.d489418d.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.150332 temboard-8.1b1/temboardui/static/css/
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/css/bootstrap-multiselect.css
+-rw-r--r--   0 root         (0) root         (0)    22608 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/css/bootstrap-theme.css
+-rw-r--r--   0 root         (0) root         (0)    43339 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/css/bootstrap-theme.css.map
+-rw-r--r--   0 root         (0) root         (0)    19963 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/css/bootstrap-theme.min.css
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/css/bootstrap-toggle.min.css
+-rw-r--r--   0 root         (0) root         (0)    66677 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/css/bootstrap-vue.min.css
+-rw-r--r--   0 root         (0) root         (0)   162264 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   654593 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/css/bootstrap.min.css.map
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/css/dygraph.css
+-rw-r--r--   0 root         (0) root         (0)    10766 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/dataTables.0be85286.css
+-rw-r--r--   0 root         (0) root         (0)   181164 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/dataTables.bootstrap4.9ae7027a.js
+-rw-r--r--   0 root         (0) root         (0)    77160 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/fontawesome-webfont.2adefcbc.woff2
+-rw-r--r--   0 root         (0) root         (0)   165742 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/fontawesome-webfont.7bfcab6d.eot
+-rw-r--r--   0 root         (0) root         (0)   165548 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/fontawesome-webfont.aa58f33f.ttf
+-rw-r--r--   0 root         (0) root         (0)   444379 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/fontawesome-webfont.ad615792.svg
+-rw-r--r--   0 root         (0) root         (0)    98024 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/fontawesome-webfont.ba0c59de.woff
+-rw-r--r--   0 root         (0) root         (0)   285275 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/home.8a0237c8.js
+-rw-r--r--   0 root         (0) root         (0)     1222 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/home.a0d294e3.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.150332 temboard-8.1b1/temboardui/static/images/
+-rw-r--r--   0 root         (0) root         (0)      529 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/images/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    61261 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/images/heron.png
+-rw-r--r--   0 root         (0) root         (0)      609 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/images/ring-alt.svg
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/images/sort_asc.png
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/images/sort_asc_disabled.png
+-rw-r--r--   0 root         (0) root         (0)      201 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/images/sort_both.png
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/images/sort_desc.png
+-rw-r--r--   0 root         (0) root         (0)      146 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/images/sort_desc_disabled.png
+-rw-r--r--   0 root         (0) root         (0)     3217 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/images/temboard-150x32-w.png
+-rw-r--r--   0 root         (0) root         (0)    24047 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/images/temboard-logo.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.154332 temboard-8.1b1/temboardui/static/js/
+-rw-r--r--   0 root         (0) root         (0)   159638 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/Chart.min.js
+-rw-r--r--   0 root         (0) root         (0)    15369 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/Sortable.min.js
+-rw-r--r--   0 root         (0) root         (0)    68977 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/bootstrap-multiselect.js
+-rw-r--r--   0 root         (0) root         (0)     4129 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/bootstrap-toggle.min.js
+-rw-r--r--   0 root         (0) root         (0)   363092 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/bootstrap-vue.min.js
+-rw-r--r--   0 root         (0) root         (0)    62563 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/bootstrap.min.js
+-rw-r--r--   0 root         (0) root         (0)   185257 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/bootstrap.min.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.154332 temboard-8.1b1/temboardui/static/js/datatables/
+-rw-r--r--   0 root         (0) root         (0)    20297 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/datatables/datatables.min.css
+-rw-r--r--   0 root         (0) root         (0)   147324 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/datatables/datatables.min.js
+-rw-r--r--   0 root         (0) root         (0)    69586 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/daterangepicker.js
+-rw-r--r--   0 root         (0) root         (0)   123910 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/dygraph.min.js
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/filesize.min.js
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/fscreen.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.154332 temboard-8.1b1/temboardui/static/js/highlightjs/
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/highlightjs/default.css
+-rw-r--r--   0 root         (0) root         (0)    19707 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/highlightjs/highlight.pack.js
+-rw-r--r--   0 root         (0) root         (0)    84345 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/jquery-2.1.4.min.js
+-rw-r--r--   0 root         (0) root         (0)    73157 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/lodash.min.js
+-rw-r--r--   0 root         (0) root         (0)    40732 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/moment.min.js
+-rw-r--r--   0 root         (0) root         (0)     2958 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/moment.preciseDiff.js
+-rw-r--r--   0 root         (0) root         (0)    19188 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/popper.min.js
+-rw-r--r--   0 root         (0) root         (0)    16337 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/temboard.settings.group.js
+-rw-r--r--   0 root         (0) root         (0)      966 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/temboard.settings.notifications.js
+-rw-r--r--   0 root         (0) root         (0)    17547 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/temboard.settings.user.js
+-rw-r--r--   0 root         (0) root         (0)    24084 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/vue-router.min.js
+-rw-r--r--   0 root         (0) root         (0)    93670 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/vue.min.js
+-rw-r--r--   0 root         (0) root         (0)     6708 2023-07-11 12:19:36.000000 temboard-8.1b1/temboardui/static/js/vuedraggable.min.js
+-rw-r--r--   0 root         (0) root         (0)     3389 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/manifest.json
+-rw-r--r--   0 root         (0) root         (0)      754 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/plugin-vue2_normalizer.ed7092a9.js
+-rw-r--r--   0 root         (0) root         (0)    44661 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/settings.instance.be0dadd5.js
+-rw-r--r--   0 root         (0) root         (0)   214816 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/temboard.9b8cf8f1.css
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/temboard.beba2dfa.js
+-rw-r--r--   0 root         (0) root         (0)   102035 2023-07-11 12:19:37.000000 temboard-8.1b1/temboardui/static/vue.esm.6bf4157d.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.154332 temboard-8.1b1/temboardui/templates/
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/templates/about.html
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/templates/agent-login.html
+-rw-r--r--   0 root         (0) root         (0)     7926 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)      417 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/templates/error.html
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/templates/home.html
+-rw-r--r--   0 root         (0) root         (0)     4030 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/templates/instance-about.html
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/templates/login.html
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/templates/notifications.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.158332 temboard-8.1b1/temboardui/templates/settings/
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/templates/settings/error.html
+-rw-r--r--   0 root         (0) root         (0)     3738 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/templates/settings/group.html
+-rw-r--r--   0 root         (0) root         (0)     3516 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/templates/settings/instance.html
+-rw-r--r--   0 root         (0) root         (0)      506 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/templates/settings/menu.html
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/templates/settings/notifications.html
+-rw-r--r--   0 root         (0) root         (0)     3980 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/templates/settings/user.html
+-rw-r--r--   0 root         (0) root         (0)      463 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/templates/unauthorized.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.158332 temboard-8.1b1/temboardui/toolkit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16397 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/app.py
+-rw-r--r--   0 root         (0) root         (0)     7309 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/configuration.py
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5624 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/http.py
+-rw-r--r--   0 root         (0) root         (0)     5716 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/log.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/perf.py
+-rw-r--r--   0 root         (0) root         (0)     8038 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/proctitle.py
+-rw-r--r--   0 root         (0) root         (0)      629 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/pycompat.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7118 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/services.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/signing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.158332 temboard-8.1b1/temboardui/toolkit/tasklist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/tasklist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11784 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/tasklist/sqlite3_engine.py
+-rw-r--r--   0 root         (0) root         (0)    30519 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/taskmanager.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3479 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/validators.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/toolkit/versions.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:20:07.158332 temboard-8.1b1/temboardui/web/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9000 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/web/flask.py
+-rw-r--r--   0 root         (0) root         (0)     4083 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/web/routes.py
+-rw-r--r--   0 root         (0) root         (0)    23356 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/web/tornado.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-07-11 12:20:05.000000 temboard-8.1b1/temboardui/web/vitejs.py
```

### Comparing `temboard-8.0b6/LICENSE` & `temboard-8.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/MANIFEST.in` & `temboard-8.1b1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/PKG-INFO` & `temboard-8.1b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temboard
-Version: 8.0b6
+Version: 8.1b1
 Summary: temBoard User Interface.
 Home-page: https://labs.dalibo.com/temboard
 Author: Dalibo
 Author-email: contact@dalibo.com
 License: PostgreSQL
 Description: <p align="center">
             <img src="https://github.com/dalibo/temboard/raw/master/docs/assets/temboard-logo-slogan.png" />
@@ -79,14 +79,16 @@
         
         # License
         
         temBoard is available under the [PostgreSQL License].
         
         [PostgreSQL License]: https://github.com/dalibo/temboard/blob/master/LICENSE
         
+        Candy Scordia drew *héron garde-bœuf* sketches.
+        
 Platform: UNKNOWN
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Database :: Database Engines/Servers
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: temboard Version: 8.0b6 Summary: temBoard User
+Metadata-Version: 2.1 Name: temboard Version: 8.1b1 Summary: temBoard User
 Interface. Home-page: https://labs.dalibo.com/temboard Author: Dalibo Author-
 email: contact@dalibo.com License: PostgreSQL Description:
    [https://github.com/dalibo/temboard/raw/master/docs/assets/temboard-logo-
                                   slogan.png]
         Monitor, optimize and configure multiple PostgreSQL instances.
  [PyPI_version] [Supported_Python_versions] [CI_status] [Documentation_status]
    [https://github.com/dalibo/temboard/raw/master/docs/screenshots/instance-
@@ -20,13 +20,14 @@
 temBoard project provides packages for RHEL and clones as well as Debian. See
 [temboard.readthedocs.io](http://temboard.readthedocs.io/en/latest/) for
 installation instructions. # Contribute temBoard is an open project. Any
 contribution to improve it is welcome. Want to contribute? Please first read
 our guide on [contributing](https://github.com/dalibo/temboard/blob/master/
 CONTRIBUTING.md) if you\'re interested in getting involved. # License temBoard
 is available under the [PostgreSQL License]. [PostgreSQL License]: https://
-github.com/dalibo/temboard/blob/master/LICENSE Platform: UNKNOWN Classifier:
-Intended Audience :: System Administrators Classifier: License :: OSI Approved
-Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
-:: Python :: 2.7 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Topic :: Database :: Database Engines/Servers Classifier: Topic :: System ::
-Monitoring Description-Content-Type: text/markdown
+github.com/dalibo/temboard/blob/master/LICENSE Candy Scordia drew *hÃ©ron
+garde-bÅuf* sketches. Platform: UNKNOWN Classifier: Intended Audience ::
+System Administrators Classifier: License :: OSI Approved Classifier: Operating
+System :: POSIX :: Linux Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.6 Classifier: Topic :: Database
+:: Database Engines/Servers Classifier: Topic :: System :: Monitoring
+Description-Content-Type: text/markdown
```

### Comparing `temboard-8.0b6/README.md` & `temboard-8.1b1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -70,7 +70,9 @@
 
 
 # License
 
 temBoard is available under the [PostgreSQL License].
 
 [PostgreSQL License]: https://github.com/dalibo/temboard/blob/master/LICENSE
+
+Candy Scordia drew *héron garde-bœuf* sketches.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -17,8 +17,9 @@
 temBoard project provides packages for RHEL and clones as well as Debian. See
 [temboard.readthedocs.io](http://temboard.readthedocs.io/en/latest/) for
 installation instructions. # Contribute temBoard is an open project. Any
 contribution to improve it is welcome. Want to contribute? Please first read
 our guide on [contributing](https://github.com/dalibo/temboard/blob/master/
 CONTRIBUTING.md) if you\'re interested in getting involved. # License temBoard
 is available under the [PostgreSQL License]. [PostgreSQL License]: https://
-github.com/dalibo/temboard/blob/master/LICENSE
+github.com/dalibo/temboard/blob/master/LICENSE Candy Scordia drew *hÃ©ron
+garde-bÅuf* sketches.
```

### Comparing `temboard-8.0b6/setup.py` & `temboard-8.1b1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,27 +15,31 @@
     __version__ = __version__.replace('+', '.')
 
 # Accept Tornado 5.X on Python 2.7.9+
 # Accept Tornado 6.X on Python 3+
 BLEEDING_EDGE_TORNADO = '7'
 if sys.version_info < (2, 7, 9):
     BLEEDING_EDGE_TORNADO = '4.5'
+    open_kw = dict()
 elif sys.version_info < (3,):
     BLEEDING_EDGE_TORNADO = '6'
+    open_kw = dict()
+else:
+    open_kw = dict(encoding='utf-8')
 
 install_requires = [
     'cryptography',
     'flask',
     'python-dateutil>=1.5',
     # There is no hard dependency on psycopg2 to allow using
     # psycopg2-binary instead. psycopg2 is not provided by psycopg2-binary
     # and there is no way to state an OR dependency in Python. It's up to
     # the user or package manager to ensure psycopg2 dependency. See
     # documentation.
-    'sqlalchemy>=0.9.8',
+    'sqlalchemy>=0.9.8,<2',
     'tornado>=3.2,<' + BLEEDING_EDGE_TORNADO,
     'future',
 ]
 
 if sys.version_info < (3,):
     install_requires.append('futures')
 
@@ -92,12 +96,12 @@
         ]
     },
 )
 
 
 if __name__ == '__main__':
     setup(
-        long_description=open(setup_path + '/README.md').read(),
+        long_description=open('README.md', **open_kw).read(),
         long_description_content_type='text/markdown',
         packages=find_packages(),
         **SETUP_KWARGS
     )
```

### Comparing `temboard-8.0b6/share/auto_configure.sh` & `temboard-8.1b1/share/auto_configure.sh`

 * *Files 18% similar despite different names*

```diff
@@ -47,35 +47,14 @@
 	fi
 
 	# Now, log everything.
 	set -x
 }
 
 
-setup_pq() {
-	local psql
-
-	# Ensure used libpq vars are defined for configuration template.
-
-	export PGHOST=${PGHOST-/var/run/postgresql}
-	export PGPORT=${PGPORT-5432}
-	export PGUSER=${PGUSER-postgres}
-
-	if [ -d "$PGHOST" ] ; then
-		psql=(sudo -nEu "$PGUSER" psql)
-	else
-		psql=(psql)
-	fi
-
-	if ! "${psql[@]}" -tc "SELECT 'Postgres connection working.';" ; then
-		fatal "Can't connect to Postgres cluster."
-	fi
-}
-
-
 setup_ssl() {
 	local pki;
 	for d in /etc/pki/tls /etc/ssl /etc/temboard; do
 		if [ -d $d ] ; then
 			pki=$d
 			break
 		fi
@@ -103,63 +82,73 @@
 	readlink -e $sslcert $sslkey
 }
 
 
 generate_configuration() {
 	local sslcert=$1; shift
 	local sslkey=$1; shift
+	local created cookie_secret version
 
 	sudo -iu "$SYSUSER" test -r "$sslcert"
 	sudo -iu "$SYSUSER" test -r "$sslkey"
+	created="$(date)"
+	cookie_secret="$(pwgen 128)"
+	version="$(temboard --version | sed 's/^/# /')"
 
 	cat <<-EOF
-	# Configuration initiated by $0 on $(date)
+	#
+	#   T E M B O A R D   U I   C O N F I G U R A T I O N
+	#
+	# Generated by ${BASH_SOURCE[0]} on $created.
+	#
+	$version
 	#
 	# See https://temboard.rtfd.io/ for details on configuration
 	# possibilities.
+	#
 
 	[temboard]
 	port = ${TEMBOARD_PORT-8888}
 	ssl_cert_file = $sslcert
 	ssl_key_file = $sslkey
-	cookie_secret = $(pwgen 128)
+	cookie_secret = $cookie_secret
 	home = ${VARDIR}
 
 	[repository]
-	host = ${PGHOST}
-	port = ${PGPORT}
+	host = ${PGHOST-/var/run/postgresql}
+	port = ${PGPORT-5432}
 	user = temboard
 	password = ${TEMBOARD_PASSWORD}
 	dbname = ${TEMBOARD_DATABASE-temboard}
 
 	[logging]
 	method = stderr
 	level = ${TEMBOARD_LOGGING_LEVEL-INFO}
 
 	[monitoring]
 	# purge_after = 730
 
 	[statements]
 	# purge_after = 7
-
 	EOF
 }
 
 pwgen() {
 	# Generates a random password of 32 hexadecimal characters.
 	od -vN $((${1-32} / 2)) -An -tx1 /dev/urandom | tr -d ' \n'
 }
 
 
 #       M A I N
 
+exec 0>&-  # Close stdin.
+
 cd "$(readlink -m "${BASH_SOURCE[0]}/..")"
 
 setup_logging
-setup_pq
 
 export TEMBOARD_PASSWORD=${TEMBOARD_PASSWORD-$(pwgen)}
 if ! getent passwd "$SYSUSER" ; then
 	log "Creating system user temBoard."
 	useradd \
 		--system --user-group --shell "$SHELL" \
 		--home-dir "$VARDIR" \
@@ -179,30 +168,25 @@
 mapfile -t sslfiles < <(set -eu; setup_ssl)
 install -o "$SYSUSER" -g "$SYSUSER" -m 0750 -d "$ETCDIR" "$LOGDIR" "$VARDIR"
 install -o "$SYSUSER" -g "$SYSUSER" -m 0640 /dev/null "$ETCDIR/temboard.conf"
 generate_configuration "${sslfiles[@]}" > "$ETCDIR/temboard.conf"
 
 log "Creating Postgres user, database and schema."
 # For temboard migratedb
-DEBUG=y TEMBOARD_CONFIGFILE="$ETCDIR/temboard.conf" ./create_repository.sh
+TEMBOARD_CONFIGFILE="$ETCDIR/temboard.conf" ./create_repository.sh
 
 if [ "$(whoami)" != "$SYSUSER" ] ; then
 	# Run as temboard UNIX user. Wipe environment, this requires properly
 	# temboard.conf.
-	run_as_temboard=(sudo -Enu "$SYSUSER")
+	run_as_temboard=(sudo -nu "$SYSUSER")
 else
-	run_as_temboard=()
-fi
-
-dsn="postgres://temboard:${TEMBOARD_PASSWORD}@/${TEMBOARD_DATABASE-temboard}"
-if ! "${run_as_temboard[@]}" psql -Atc "SELECT 'CONNECTED';" "$dsn" | grep -q 'CONNECTED' ; then
-	fatal "Can't configure access to Postgres database."
+	run_as_temboard=(env)
 fi
 
-TEMBOARD_CONFIGFILE="$ETCDIR/temboard.conf" "${run_as_temboard[@]}" temboard generate-key
+"${run_as_temboard[@]}" TEMBOARD_CONFIGFILE="$ETCDIR/temboard.conf" temboard generate-key
 
 if grep -q systemd /proc/1/cmdline && [ -w /etc/systemd/system ] ; then
 	start_cmd="systemctl enable-now temboard"
 	if systemctl is-system-running &>/dev/null ; then
 		systemctl daemon-reload
 	fi
 else
```

### Comparing `temboard-8.0b6/share/create_repository.sh` & `temboard-8.1b1/share/create_repository.sh`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/share/purge.sh` & `temboard-8.1b1/share/purge.sh`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/share/sql/dev-fixture.sql` & `temboard-8.1b1/share/sql/dev-fixture.sql`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+DROP SCHEMA "public";
+
 \echo ---------------------------------
 \echo --
 \echo -- Adding some users and groups
 \echo --
 \echo ---------------------------------
 \echo
```

### Comparing `temboard-8.0b6/share/sql/reassign.sql` & `temboard-8.1b1/share/sql/reassign.sql`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/share/sql/upgrade-monitoring-purge-instances.sql` & `temboard-8.1b1/share/sql/upgrade-monitoring-purge-instances.sql`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/share/temboard.conf` & `temboard-8.1b1/share/temboard.conf`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/share/temboard_CHANGEME.key` & `temboard-8.1b1/share/temboard_CHANGEME.key`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/share/temboard_CHANGEME.pem` & `temboard-8.1b1/share/temboard_CHANGEME.pem`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/share/temboard_ca_certs_CHANGEME.pem` & `temboard-8.1b1/share/temboard_ca_certs_CHANGEME.pem`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboard.egg-info/PKG-INFO` & `temboard-8.1b1/temboard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temboard
-Version: 8.0b6
+Version: 8.1b1
 Summary: temBoard User Interface.
 Home-page: https://labs.dalibo.com/temboard
 Author: Dalibo
 Author-email: contact@dalibo.com
 License: PostgreSQL
 Description: <p align="center">
             <img src="https://github.com/dalibo/temboard/raw/master/docs/assets/temboard-logo-slogan.png" />
@@ -79,14 +79,16 @@
         
         # License
         
         temBoard is available under the [PostgreSQL License].
         
         [PostgreSQL License]: https://github.com/dalibo/temboard/blob/master/LICENSE
         
+        Candy Scordia drew *héron garde-bœuf* sketches.
+        
 Platform: UNKNOWN
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Database :: Database Engines/Servers
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: temboard Version: 8.0b6 Summary: temBoard User
+Metadata-Version: 2.1 Name: temboard Version: 8.1b1 Summary: temBoard User
 Interface. Home-page: https://labs.dalibo.com/temboard Author: Dalibo Author-
 email: contact@dalibo.com License: PostgreSQL Description:
    [https://github.com/dalibo/temboard/raw/master/docs/assets/temboard-logo-
                                   slogan.png]
         Monitor, optimize and configure multiple PostgreSQL instances.
  [PyPI_version] [Supported_Python_versions] [CI_status] [Documentation_status]
    [https://github.com/dalibo/temboard/raw/master/docs/screenshots/instance-
@@ -20,13 +20,14 @@
 temBoard project provides packages for RHEL and clones as well as Debian. See
 [temboard.readthedocs.io](http://temboard.readthedocs.io/en/latest/) for
 installation instructions. # Contribute temBoard is an open project. Any
 contribution to improve it is welcome. Want to contribute? Please first read
 our guide on [contributing](https://github.com/dalibo/temboard/blob/master/
 CONTRIBUTING.md) if you\'re interested in getting involved. # License temBoard
 is available under the [PostgreSQL License]. [PostgreSQL License]: https://
-github.com/dalibo/temboard/blob/master/LICENSE Platform: UNKNOWN Classifier:
-Intended Audience :: System Administrators Classifier: License :: OSI Approved
-Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
-:: Python :: 2.7 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Topic :: Database :: Database Engines/Servers Classifier: Topic :: System ::
-Monitoring Description-Content-Type: text/markdown
+github.com/dalibo/temboard/blob/master/LICENSE Candy Scordia drew *hÃ©ron
+garde-bÅuf* sketches. Platform: UNKNOWN Classifier: Intended Audience ::
+System Administrators Classifier: License :: OSI Approved Classifier: Operating
+System :: POSIX :: Linux Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.6 Classifier: Topic :: Database
+:: Database Engines/Servers Classifier: Topic :: System :: Monitoring
+Description-Content-Type: text/markdown
```

### Comparing `temboard-8.0b6/temboard.egg-info/SOURCES.txt` & `temboard-8.1b1/temboard.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 temboardui/static/dataTables.0be85286.css
 temboardui/static/dataTables.bootstrap4.9ae7027a.js
 temboardui/static/fontawesome-webfont.2adefcbc.woff2
 temboardui/static/fontawesome-webfont.7bfcab6d.eot
 temboardui/static/fontawesome-webfont.aa58f33f.ttf
 temboardui/static/fontawesome-webfont.ad615792.svg
 temboardui/static/fontawesome-webfont.ba0c59de.woff
-temboardui/static/home.31a23655.js
+temboardui/static/home.8a0237c8.js
 temboardui/static/home.a0d294e3.css
 temboardui/static/manifest.json
 temboardui/static/plugin-vue2_normalizer.ed7092a9.js
 temboardui/static/settings.instance.be0dadd5.js
 temboardui/static/temboard.9b8cf8f1.css
 temboardui/static/temboard.beba2dfa.js
 temboardui/static/vue.esm.6bf4157d.js
```

### Comparing `temboard-8.0b6/temboardui/__main__.py` & `temboard-8.1b1/temboardui/__main__.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/agentclient.py` & `temboard-8.1b1/temboardui/agentclient.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/application.py` & `temboard-8.1b1/temboardui/application.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/autossl.py` & `temboard-8.1b1/temboardui/autossl.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/cli/apikey.py` & `temboard-8.1b1/temboardui/cli/apikey.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/cli/app.py` & `temboard-8.1b1/temboardui/cli/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,14 +289,16 @@
         if config.temboard.ssl_key_file:
             ssl_ctx = {
                 'certfile': config.temboard.ssl_cert_file,
                 'keyfile': config.temboard.ssl_key_file,
             }
             server = AutoHTTPSServer(self.app.tornado_app, ssl_options=ssl_ctx)
         else:
+            # Use plain HTTP for development to mix vitejs dev server and
+            # tornado server in the same browser page.
             server = HTTPServer(self.app.tornado_app)
         try:
             server.listen(
                 config.temboard.port, address=config.temboard.address)
         except socket.error as e:
             logger.error("FATAL: " + str(e) + '. Quit')
             sys.exit(3)
```

### Comparing `temboard-8.0b6/temboardui/cli/generate_key.py` & `temboard-8.1b1/temboardui/cli/generate_key.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/cli/migratedb.py` & `temboard-8.1b1/temboardui/cli/migratedb.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/cli/query_agent.py` & `temboard-8.1b1/temboardui/cli/query_agent.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/cli/register_instance.py` & `temboard-8.1b1/temboardui/cli/register_instance.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/cli/routes.py` & `temboard-8.1b1/temboardui/cli/routes.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/cli/serve.py` & `temboard-8.1b1/temboardui/cli/serve.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/cli/tasks.py` & `temboard-8.1b1/temboardui/cli/tasks.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/cli/web.py` & `temboard-8.1b1/temboardui/cli/web.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/core.py` & `temboard-8.1b1/temboardui/core.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/daemon.py` & `temboard-8.1b1/temboardui/daemon.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/handlers/home.py` & `temboard-8.1b1/temboardui/handlers/home.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,25 +22,26 @@
     )
 
 
 @app.route("/about")
 def metadata(request):
     versions_info = inspect_versions()
     infos = {
+        "Browser": request.headers.get('User-Agent', 'Unknown'),
         "Version": "%(temboard)s (%(temboardbin)s)" % versions_info,
         "Uptime": app.start_time,
         "OS": "%(distname)s %(distversion)s" % versions_info,
         "Python": "%(python)s (%(pythonbin)s)" % versions_info,
-        "cryptography": "%(cryptography)s" % versions_info,
-        "Tornado": "%(tornado)s" % versions_info,
-        "libpq": "%(libpq)s" % versions_info,
-        "psycopg2": "%(psycopg2)s" % versions_info,
-        "SQLAlchemy": "%(sqlalchemy)s" % versions_info,
+        "cryptography": versions_info['cryptography'],
+        "Tornado": versions_info['tornado'],
+        "libpq": versions_info['libpq'],
+        "psycopg2": versions_info['psycopg2'],
+        "SQLAlchemy": versions_info['sqlalchemy'],
     }
-    temboard_version = "%(temboard)s" % versions_info
+    temboard_version = versions_info['temboard']
 
     return render_template(
         'about.html',
         nav=True,
         role=request.current_user,
         infos=infos,
         temboard_version=temboard_version
```

### Comparing `temboard-8.0b6/temboardui/handlers/notification.py` & `temboard-8.1b1/temboardui/handlers/notification.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/handlers/settings/group.py` & `temboard-8.1b1/temboardui/handlers/settings/group.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/handlers/settings/instance.py` & `temboard-8.1b1/temboardui/handlers/settings/instance.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/handlers/settings/metadata.py` & `temboard-8.1b1/temboardui/handlers/settings/metadata.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/handlers/settings/notifications.py` & `temboard-8.1b1/temboardui/handlers/settings/notifications.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/handlers/settings/user.py` & `temboard-8.1b1/temboardui/handlers/settings/user.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/handlers/user.py` & `temboard-8.1b1/temboardui/handlers/user.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/model/__init__.py` & `temboard-8.1b1/temboardui/model/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 def configure(dsn, **kwargs):
     if hasattr(dsn, 'items'):
         dsn = format_dsn(dsn)
 
     try:
         engine = create_engine(dsn)
-        check_connectivity(engine)
     except Exception as e:
         logger.warning("Connection to the database failed: %s", e)
         logger.warning("Please check your configuration.")
         sys.stderr.write("FATAL: %s\n" % e)
         exit(10)
     Session.configure(bind=engine, **kwargs)
 
@@ -73,11 +72,12 @@
     context.
     """
     return create_engine(format_dsn(dbconf))
 
 
 def check_schema():
     engine = Session.kw['bind']
+    check_connectivity(engine)
     migrator = Migrator()
     migrator.inspect_available_versions()
     migrator.inspect_current_version(engine.raw_connection().connection)
     migrator.check()
```

### Comparing `temboard-8.0b6/temboardui/model/migrator.py` & `temboard-8.1b1/temboardui/model/migrator.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/model/orm.py` & `temboard-8.1b1/temboardui/model/orm.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/model/queries/copy-instances-as-csv.sql` & `temboard-8.1b1/temboardui/model/queries/copy-instances-as-csv.sql`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 COPY (
   WITH
 		inventory AS (SELECT DISTINCT
 			i.hostname AS "Hostname",
 			i.pg_port AS "Port",
-			i.discover->'postgres'->'data' AS "PGDATA",
-			i.discover->'postgres'->'version_summary' AS "Version",
+			i.discover->'postgres'->'data_directory'#>>'{}' AS "PGDATA",
+			i.discover->'postgres'->'version_summary'#>>'{}' AS "Version",
 			string_agg(DISTINCT group_name, ',') AS "Groups",
 			i.agent_address AS "Agent Address",
 			i.agent_port AS "Agent Port",
-			string_agg(DISTINCT plugin_name, ',') AS "Plugins"
+			string_agg(DISTINCT plugin_name, ',') AS "Plugins",
+			i.comment AS "Comment"
 		FROM application.instances AS i
 		LEFT OUTER JOIN application.instance_groups AS groups
 				ON groups.agent_port = i.agent_port
 				AND groups.agent_address = i.agent_address
 		LEFT OUTER JOIN application.plugins
 				ON plugins.agent_address = i.agent_address
 				AND plugins.agent_port = i.agent_port
```

### Comparing `temboard-8.0b6/temboardui/model/tables.py` & `temboard-8.1b1/temboardui/model/tables.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/model/versions/001_application.sql` & `temboard-8.1b1/temboardui/model/versions/001_application.sql`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/model/versions/002_monitoring.sql` & `temboard-8.1b1/temboardui/model/versions/002_monitoring.sql`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/model/versions/003_alerting.sql` & `temboard-8.1b1/temboardui/model/versions/003_alerting.sql`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/model/versions/005_statements.sql` & `temboard-8.1b1/temboardui/model/versions/005_statements.sql`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/model/versions/008_monitoring-archive-wait-lock.sql` & `temboard-8.1b1/temboardui/model/versions/008_monitoring-archive-wait-lock.sql`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-CREATE OR REPLACE FUNCTION archive_current_metrics(table_name TEXT, record_type TEXT, query TEXT) RETURNS TABLE(tblname TEXT, nb_rows INTEGER)
+CREATE OR REPLACE FUNCTION monitoring.archive_current_metrics(table_name TEXT, record_type TEXT, query TEXT)
+RETURNS TABLE(tblname TEXT, nb_rows INTEGER)
 LANGUAGE plpgsql
 AS $$
 DECLARE
   v_table_current TEXT;
   v_table_history TEXT;
   v_query TEXT;
   i INTEGER;
```

### Comparing `temboard-8.0b6/temboardui/model/versions/010_discover.sql` & `temboard-8.1b1/temboardui/model/versions/010_discover.sql`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/activity/__init__.py` & `temboard-8.1b1/temboardui/plugins/activity/__init__.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/activity/templates/activity.html` & `temboard-8.1b1/temboardui/plugins/activity/templates/activity.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% autoescape None %}
 {% extends ../../../templates/base.html %}
 
-{% block title %}[{{instance.hostname}}:{{instance.pg_port}}] - Activity / {% if mode == 'waiting' %}Waiting{% elif mode == 'blocking' %}Blocking{% elif mode == 'running' %}Running{% end %} queries{% end %}
+{% block title %}temBoard / {{instance}} / Activity / {% if mode == 'waiting' %}Waiting{% elif mode == 'blocking' %}Blocking{% elif mode == 'running' %}Running{% end %} queries{% end %}
 
 {% block head %}
 {% for link in vitejs.css_links_for('activity.js') %}{% raw link %}{% end %}
 {% end %}
 
 {% block content %}
 <div class="modal fade" id="Modal" tabindex="-1" role="dialog" aria-labelledby="ModalLabel">
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
 {% autoescape None %} {% extends ../../../templates/base.html %} {% block title
-%}[{{instance.hostname}}:{{instance.pg_port}}] - Activity / {% if mode ==
-'waiting' %}Waiting{% elif mode == 'blocking' %}Blocking{% elif mode ==
-'running' %}Running{% end %} queries{% end %} {% block head %} {% for link in
-vitejs.css_links_for('activity.js') %}{% raw link %}{% end %} {% end %} {%
-block content %}
+%}temBoard / {{instance}} / Activity / {% if mode == 'waiting' %}Waiting{% elif
+mode == 'blocking' %}Blocking{% elif mode == 'running' %}Running{% end %}
+queries{% end %} {% block head %} {% for link in vitejs.css_links_for
+('activity.js') %}{% raw link %}{% end %} {% end %} {% block content %}
 ×
 Cancel
     * Running
     * Waiting
        
     * Blocking
```

### Comparing `temboard-8.0b6/temboardui/plugins/dashboard/__init__.py` & `temboard-8.1b1/temboardui/plugins/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/dashboard/static/js/temboard.dashboard.js` & `temboard-8.1b1/temboardui/plugins/dashboard/static/js/temboard.dashboard.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/dashboard/templates/dashboard.html` & `temboard-8.1b1/temboardui/plugins/dashboard/templates/dashboard.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends ../../../templates/base.html %}
 
-{% block title %}[{{instance.hostname}}:{{instance.pg_port}}] - Dashboard{% end %}
+{% block title %}temBoard / {{instance}} / Dashboard{% end %}
 
 {% block content %}
 <div class="position-absolute" style="z-index: 2;">
   <a class="btn btn-link fullscreen" href data-toggle="popover" data-trigger="hover" data-content="Full screen" data-placement="bottom">
     <i class="fa fa-expand"></i>
   </a>
 </div>
@@ -171,15 +171,15 @@
     <div class="text-center small">
       Current status
       <div class="position-absolute top-0 right-0 pr-2">
         <a href="alerting" class="small text-muted">More&hellip;</a>
       </div>
     </div>
     <div class="row small mb-2">
-      <template v-for="state in states">
+      <template v-for="state in states" v-if="state.state!='UNDEF'">
         <div class="col-3 col-xxl-2 p-1 text-center">
           <div class="p-1 rounded" v-bind:class="[getBorderColor(state.state), {'striped bg-light': !state.enabled }]">
             <a v-bind:href="'alerting/' + state.name"
                v-bind:class="{'text-muted': !state.enabled}">
               <div class="text-nowrap font-weight-bold"
                    style="overflow: hidden; text-overflow: ellipsis"
                    v-bind:title="state.description">
```

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/__init__.py` & `temboard-8.1b1/temboardui/plugins/maintenance/__init__.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/static/js/temboard.maintenance.database.js` & `temboard-8.1b1/temboardui/plugins/maintenance/static/js/temboard.maintenance.database.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/static/js/temboard.maintenance.js` & `temboard-8.1b1/temboardui/plugins/maintenance/static/js/temboard.maintenance.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/static/js/temboard.maintenance.schema.js` & `temboard-8.1b1/temboardui/plugins/maintenance/static/js/temboard.maintenance.schema.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/static/js/temboard.maintenance.table.js` & `temboard-8.1b1/temboardui/plugins/maintenance/static/js/temboard.maintenance.table.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/static/js/vue.size-distribution-bar.js` & `temboard-8.1b1/temboardui/plugins/maintenance/static/js/vue.size-distribution-bar.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/templates/breadcrumb.html` & `temboard-8.1b1/temboardui/plugins/maintenance/templates/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/templates/database.html` & `temboard-8.1b1/temboardui/plugins/maintenance/templates/database.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/templates/includes/analyze_modal.html` & `temboard-8.1b1/temboardui/plugins/maintenance/templates/includes/analyze_modal.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/templates/includes/reindex_modal.html` & `temboard-8.1b1/temboardui/plugins/maintenance/templates/includes/reindex_modal.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/templates/includes/scheduled_analyze.html` & `temboard-8.1b1/temboardui/plugins/maintenance/templates/includes/scheduled_analyze.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/templates/includes/scheduled_reindex.html` & `temboard-8.1b1/temboardui/plugins/maintenance/templates/includes/scheduled_reindex.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/templates/includes/scheduled_vacuum.html` & `temboard-8.1b1/temboardui/plugins/maintenance/templates/includes/scheduled_vacuum.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/templates/includes/vacuum_modal.html` & `temboard-8.1b1/temboardui/plugins/maintenance/templates/includes/vacuum_modal.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/templates/index.html` & `temboard-8.1b1/temboardui/plugins/maintenance/templates/index.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/templates/schema.html` & `temboard-8.1b1/temboardui/plugins/maintenance/templates/schema.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/maintenance/templates/table.html` & `temboard-8.1b1/temboardui/plugins/maintenance/templates/table.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/__init__.py` & `temboard-8.1b1/temboardui/plugins/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/alerting.py` & `temboard-8.1b1/temboardui/plugins/monitoring/alerting.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/chartdata.py` & `temboard-8.1b1/temboardui/plugins/monitoring/chartdata.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/handlers/alerting.py` & `temboard-8.1b1/temboardui/plugins/monitoring/handlers/alerting.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/handlers/monitoring.py` & `temboard-8.1b1/temboardui/plugins/monitoring/handlers/monitoring.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/model/db.py` & `temboard-8.1b1/temboardui/plugins/monitoring/model/db.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/model/orm.py` & `temboard-8.1b1/temboardui/plugins/monitoring/model/orm.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/model/tables.py` & `temboard-8.1b1/temboardui/plugins/monitoring/model/tables.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/pivot.py` & `temboard-8.1b1/temboardui/plugins/monitoring/pivot.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/static/js/datemath.js` & `temboard-8.1b1/temboardui/plugins/monitoring/static/js/datemath.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/static/js/daterangepicker.vue.js` & `temboard-8.1b1/temboardui/plugins/monitoring/static/js/daterangepicker.vue.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/static/js/rangeutils.js` & `temboard-8.1b1/temboardui/plugins/monitoring/static/js/rangeutils.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/static/js/temboard.check.js` & `temboard-8.1b1/temboardui/plugins/monitoring/static/js/temboard.check.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/static/js/temboard.checks.js` & `temboard-8.1b1/temboardui/plugins/monitoring/static/js/temboard.checks.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/static/js/temboard.monitoring.js` & `temboard-8.1b1/temboardui/plugins/monitoring/static/js/temboard.monitoring.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/templates/alerting.check.html` & `temboard-8.1b1/temboardui/plugins/monitoring/templates/alerting.check.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends ../../../templates/base.html %}
 
-{% block title %}[{{instance.hostname}}:{{instance.pg_port}}] - Monitoring{% end %}
+{% block title %}temBoard / {{instance}} / Monitoring{% end %}
 
 {% block head %}
 <link href="/css/dygraph.css" rel="stylesheet" />
 {% end %}
 
 {% block content %}
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-{% extends ../../../templates/base.html %} {% block title %}[{
-{instance.hostname}}:{{instance.pg_port}}] - Monitoring{% end %} {% block head
-%}
+{% extends ../../../templates/base.html %} {% block title %}temBoard / {
+{instance}} / Monitoring{% end %} {% block head %}
  {% end %} {% block content %}
    1. Status
    2. {{check['description']}}
 from.sync="from" :to.sync="to" ref="daterangepicker">
     * {'style="text-decoration:line-through;"'}}> Enabled:
  &horbar;  Warning: {{ '{0:g}'.format(float(check['warning'])) }}{% if
 value_type == 'percent' %}%{% end %}
```

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/templates/alerting.checks.html` & `temboard-8.1b1/temboardui/plugins/monitoring/templates/alerting.checks.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 {% extends ../../../templates/base.html %}
 
-{% block title %}[{{instance.hostname}}:{{instance.pg_port}}] - Monitoring{% end %}
+{% block title %}temBoard / {{instance}} / Monitoring{% end %}
 
 {% block content %}
 
 <div class="text-right text-muted small">Auto refresh every 1 min</div>
 <div id="checks-container" class="row" v-cloak>
-  <div class="col-3" v-for="check in checks">
+  <div class="col-3" v-for="check in checks" v-if="check.state!='UNDEF'">
     <div v-bind:id="'status-' + check.name" class="card mb-3 w-100 border" v-bind:class="['border-' + getBorderColor(check.state), {'striped bg-light': !check.enabled}]">
       <div class="card-body p-2">
         <div>
           <a v-bind:href="'alerting/' + check.name"
              v-bind:class="{'text-muted': !check.enabled}">
             <span v-bind:class="'badge badge-' + check.state.toLowerCase()">
               {{! check.state }}
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-{% extends ../../../templates/base.html %} {% block title %}[{
-{instance.hostname}}:{{instance.pg_port}}] - Monitoring{% end %} {% block
-content %}
+{% extends ../../../templates/base.html %} {% block title %}temBoard / {
+{instance}} / Monitoring{% end %} {% block content %}
 Auto refresh every 1 min
  {{! check.state }}  {{! check.description }}
 ===============================================================================
     *  {{! key.state }}  {{!key.key}}
 ===============================================================================
     * Warning: {{! check.warning }}{{! check.value_type == 'percent' ? '%' :
       ''}}
```

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/templates/index.html` & `temboard-8.1b1/temboardui/plugins/monitoring/templates/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends ../../../templates/base.html %}
 
-{% block title %}[{{instance.hostname}}:{{instance.pg_port}}] - Monitoring{% end %}
+{% block title %}temBoard / {{instance}} / Monitoring{% end %}
 
 {% block head %}
 <link href="/css/dygraph.css" rel="stylesheet" />
 {% end %}
 
 {% block content %}
 <div id="charts-container">
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-{% extends ../../../templates/base.html %} {% block title %}[{
-{instance.hostname}}:{{instance.pg_port}}] - Monitoring{% end %} {% block head
-%}
+{% extends ../../../templates/base.html %} {% block title %}temBoard / {
+{instance}} / Monitoring{% end %} {% block head %}
  {% end %} {% block content %}
  Metrics
 
 from.sync="from" :to.sync="to" ref="daterangepicker">
 System
     * id="'checkbox' + key" class="form-check-input" :checked="isVisible(key)"
       v-on:change="setVisible(key, $event)">
```

### Comparing `temboard-8.0b6/temboardui/plugins/monitoring/tools.py` & `temboard-8.1b1/temboardui/plugins/monitoring/tools.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/pgconf/__init__.py` & `temboard-8.1b1/temboardui/plugins/pgconf/__init__.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/pgconf/static/js/temboard.pgconf.js` & `temboard-8.1b1/temboardui/plugins/pgconf/static/js/temboard.pgconf.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/pgconf/templates/configuration.html` & `temboard-8.1b1/temboardui/plugins/pgconf/templates/configuration.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/statements/__init__.py` & `temboard-8.1b1/temboardui/plugins/statements/__init__.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/statements/static/js/temboard.statements.js` & `temboard-8.1b1/temboardui/plugins/statements/static/js/temboard.statements.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/plugins/statements/templates/index.html` & `temboard-8.1b1/temboardui/plugins/statements/templates/index.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/Error.20e0c905.js` & `temboard-8.1b1/temboardui/static/Error.20e0c905.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/activity.d1cda23a.css` & `temboard-8.1b1/temboardui/static/activity.d1cda23a.css`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/activity.d489418d.js` & `temboard-8.1b1/temboardui/static/activity.d489418d.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/css/bootstrap-multiselect.css` & `temboard-8.1b1/temboardui/static/css/bootstrap-multiselect.css`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/css/bootstrap-theme.css` & `temboard-8.1b1/temboardui/static/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/css/bootstrap-theme.css.map` & `temboard-8.1b1/temboardui/static/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/css/bootstrap-theme.min.css` & `temboard-8.1b1/temboardui/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/css/bootstrap-toggle.min.css` & `temboard-8.1b1/temboardui/static/css/bootstrap-toggle.min.css`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/css/bootstrap-vue.min.css` & `temboard-8.1b1/temboardui/static/css/bootstrap-vue.min.css`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/css/bootstrap.min.css` & `temboard-8.1b1/temboardui/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/css/bootstrap.min.css.map` & `temboard-8.1b1/temboardui/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/css/dygraph.css` & `temboard-8.1b1/temboardui/static/css/dygraph.css`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/dataTables.0be85286.css` & `temboard-8.1b1/temboardui/static/dataTables.0be85286.css`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/dataTables.bootstrap4.9ae7027a.js` & `temboard-8.1b1/temboardui/static/dataTables.bootstrap4.9ae7027a.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/fontawesome-webfont.2adefcbc.woff2` & `temboard-8.1b1/temboardui/static/fontawesome-webfont.2adefcbc.woff2`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/fontawesome-webfont.7bfcab6d.eot` & `temboard-8.1b1/temboardui/static/fontawesome-webfont.7bfcab6d.eot`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/fontawesome-webfont.aa58f33f.ttf` & `temboard-8.1b1/temboardui/static/fontawesome-webfont.aa58f33f.ttf`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/fontawesome-webfont.ad615792.svg` & `temboard-8.1b1/temboardui/static/fontawesome-webfont.ad615792.svg`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/fontawesome-webfont.ba0c59de.woff` & `temboard-8.1b1/temboardui/static/fontawesome-webfont.ba0c59de.woff`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/home.31a23655.js` & `temboard-8.1b1/temboardui/static/home.8a0237c8.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -12189,17 +12189,17 @@
                 }));
                 return e
             }
         },
         methods: {
             popoverContent: function(e) {
                 var t = e.checks.filter(function(l) {
-                        return l.state != "OK"
+                        return !["OK", "UNDEF"].includes(l.state)
                     }),
-                    r = ["CRITICAL", "WARNING", "UNDEF"],
+                    r = ["CRITICAL", "WARNING"],
                     a = Qr.sortBy(t, function(l) {
                         return r.indexOf(l.state)
                     }),
                     s = a.map(function(l) {
                         return '<span class="badge badge-' + l.state.toLowerCase() + '">' + l.description + "</span>"
                     });
                 return s.join("<br>")
@@ -12224,17 +12224,15 @@
                 attrs: {
                     title: "Unable to connect to Postgres"
                 }
             }, [t._v("UNAVAILABLE")]), t.checks.CRITICAL ? r("span", {
                 staticClass: "badge badge-critical mr-1"
             }, [t._v(" CRITICAL: " + t._s(t.checks.CRITICAL))]) : t._e(), t.checks.WARNING ? r("span", {
                 staticClass: "badge badge-warning mr-1"
-            }, [t._v(" WARNING: " + t._s(t.checks.WARNING))]) : t._e(), t.checks.UNDEF ? r("span", {
-                staticClass: "badge badge-undef mr-1"
-            }, [t._v(" UNDEF: " + t._s(t.checks.UNDEF))]) : t._e(), !t.checks.WARNING && !t.checks.CRITICAL && !t.checks.UNDEF && t.checks.OK ? r("span", {
+            }, [t._v(" WARNING: " + t._s(t.checks.WARNING))]) : t._e(), !t.checks.WARNING && !t.checks.CRITICAL && !t.checks.UNDEF && t.checks.OK ? r("span", {
                 staticClass: "badge badge-ok mr-1"
             }, [t._v("OK")]) : t._e()])
         },
         CA = [],
         EA = ns(DA, MA, CA, !1, null, null, null, null);
     const RA = EA.exports,
         LA = {
```

### Comparing `temboard-8.0b6/temboardui/static/home.a0d294e3.css` & `temboard-8.1b1/temboardui/static/home.a0d294e3.css`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/images/favicon.ico` & `temboard-8.1b1/temboardui/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/images/heron.png` & `temboard-8.1b1/temboardui/static/images/heron.png`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/images/ring-alt.svg` & `temboard-8.1b1/temboardui/static/images/ring-alt.svg`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/images/temboard-150x32-w.png` & `temboard-8.1b1/temboardui/static/images/temboard-150x32-w.png`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/images/temboard-logo.png` & `temboard-8.1b1/temboardui/static/images/temboard-logo.png`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/Chart.min.js` & `temboard-8.1b1/temboardui/static/js/Chart.min.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/Sortable.min.js` & `temboard-8.1b1/temboardui/static/js/Sortable.min.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/bootstrap-multiselect.js` & `temboard-8.1b1/temboardui/static/js/bootstrap-multiselect.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/bootstrap-toggle.min.js` & `temboard-8.1b1/temboardui/static/js/bootstrap-toggle.min.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/bootstrap-vue.min.js` & `temboard-8.1b1/temboardui/static/js/bootstrap-vue.min.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/bootstrap.min.js` & `temboard-8.1b1/temboardui/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/bootstrap.min.js.map` & `temboard-8.1b1/temboardui/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/datatables/datatables.min.css` & `temboard-8.1b1/temboardui/static/js/datatables/datatables.min.css`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/datatables/datatables.min.js` & `temboard-8.1b1/temboardui/static/js/datatables/datatables.min.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/daterangepicker.js` & `temboard-8.1b1/temboardui/static/js/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/dygraph.min.js` & `temboard-8.1b1/temboardui/static/js/dygraph.min.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/filesize.min.js` & `temboard-8.1b1/temboardui/static/js/filesize.min.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/fscreen.js` & `temboard-8.1b1/temboardui/static/js/fscreen.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/highlightjs/default.css` & `temboard-8.1b1/temboardui/static/js/highlightjs/default.css`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/highlightjs/highlight.pack.js` & `temboard-8.1b1/temboardui/static/js/highlightjs/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/jquery-2.1.4.min.js` & `temboard-8.1b1/temboardui/static/js/jquery-2.1.4.min.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/lodash.min.js` & `temboard-8.1b1/temboardui/static/js/lodash.min.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/moment.min.js` & `temboard-8.1b1/temboardui/static/js/moment.min.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/moment.preciseDiff.js` & `temboard-8.1b1/temboardui/static/js/moment.preciseDiff.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/popper.min.js` & `temboard-8.1b1/temboardui/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/temboard.settings.group.js` & `temboard-8.1b1/temboardui/static/js/temboard.settings.group.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/temboard.settings.notifications.js` & `temboard-8.1b1/temboardui/static/js/temboard.settings.notifications.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/temboard.settings.user.js` & `temboard-8.1b1/temboardui/static/js/temboard.settings.user.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/vue-router.min.js` & `temboard-8.1b1/temboardui/static/js/vue-router.min.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/vue.min.js` & `temboard-8.1b1/temboardui/static/js/vue.min.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/js/vuedraggable.min.js` & `temboard-8.1b1/temboardui/static/js/vuedraggable.min.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/manifest.json` & `temboard-8.1b1/temboardui/static/manifest.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972222222222222%*

 * *Differences: {"'home.js'": "{'file': 'home.8a0237c8.js'}"}*

```diff
@@ -68,15 +68,15 @@
         "file": "home.a0d294e3.css",
         "src": "home.css"
     },
     "home.js": {
         "css": [
             "home.a0d294e3.css"
         ],
-        "file": "home.31a23655.js",
+        "file": "home.8a0237c8.js",
         "imports": [
             "_vue.esm.6bf4157d.js",
             "__commonjsHelpers.04e31c8c.js",
             "_plugin-vue2_normalizer.ed7092a9.js"
         ],
         "isEntry": true,
         "src": "home.js"
```

### Comparing `temboard-8.0b6/temboardui/static/plugin-vue2_normalizer.ed7092a9.js` & `temboard-8.1b1/temboardui/static/plugin-vue2_normalizer.ed7092a9.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/settings.instance.be0dadd5.js` & `temboard-8.1b1/temboardui/static/settings.instance.be0dadd5.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/temboard.9b8cf8f1.css` & `temboard-8.1b1/temboardui/static/temboard.9b8cf8f1.css`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/temboard.beba2dfa.js` & `temboard-8.1b1/temboardui/static/temboard.beba2dfa.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/static/vue.esm.6bf4157d.js` & `temboard-8.1b1/temboardui/static/vue.esm.6bf4157d.js`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/templates/about.html` & `temboard-8.1b1/temboardui/templates/about.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends base.html %}
 
-{% block title %}About temBoard{% end %}
+{% block title %}temBoard / About{% end %}
 
 {% block content %}
 {% whitespace single %}
 <div class="row">
   <div class="col-12" id="content" style="font-size: 130%">
     <div style="max-width: 800px" class="mx-auto w-100 w-md-75">
       <div class="row justify-content-center">
```

### Comparing `temboard-8.0b6/temboardui/templates/agent-login.html` & `temboard-8.1b1/temboardui/templates/agent-login.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends base.html %}
 
-{% block title %}[{{instance.hostname}}:{{instance.pg_port}}] - Login{% end %}
+{% block title %}temBoard / {{instance}} / Login{% end %}
 
 {% block content %}
 {% if username is not None %}
 <div class="row d-flex justify-content-center">
   <div class="col-xl-4 col-md-6">
     <div class="alert alert-info" role="alert">
       <h4><i class="fa fa-info fa-fw"></i>Information</h4>
```

### Comparing `temboard-8.0b6/temboardui/templates/base.html` & `temboard-8.1b1/temboardui/templates/base.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/templates/home.html` & `temboard-8.1b1/temboardui/templates/home.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends base.html %}
 
-{% block title %}temBoard - Home{% end %}
+{% block title %}temBoard{% end %}
 
 {% block head %}
 {% for link in vitejs.css_links_for('home.js') %}{% raw link %}{% end %}
 {% end %}
 
 {% block content %}
 {% import json %}
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
-{% extends base.html %} {% block title %}temBoard - Home{% end %} {% block head
-%} {% for link in vitejs.css_links_for('home.js') %}{% raw link %}{% end %} {%
-end %} {% block content %} {% import json %}
+{% extends base.html %} {% block title %}temBoard{% end %} {% block head %} {%
+for link in vitejs.css_links_for('home.js') %}{% raw link %}{% end %} {% end %}
+{% block content %} {% import json %}
 {% end %}
```

### Comparing `temboard-8.0b6/temboardui/templates/instance-about.html` & `temboard-8.1b1/temboardui/templates/instance-about.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends base.html %}
 
-{% block title %}[{{instance}}] - About{% end %}
+{% block title %}temBoard / {{instance}} / About{% end %}
 
 {% block content %}
 <div class="text-center mt-4">
   <h1>{{ instance }} <span class="align-top badge badge-secondary">{{ instance.groups[0].group_name }}</span></h1>
   {% if len(instance.groups) > 1 %}
   <h3>
     {% for group in instance.groups %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% extends base.html %} {% block title %}[{{instance}}] - About{% end %} {%
-block content %}
+{% extends base.html %} {% block title %}temBoard / {{instance}} / About{% end
+%} {% block content %}
 ****** {{ instance }} {{ instance.groups[0].group_name }} ******
 {% if len(instance.groups) > 1 %}
 **** {% for group in instance.groups %} {{ group.group_name }} {% end %} ****
 {% end %}
 ***** {{ instance.pg_version_summary }} serving {{ instance.pg_data }}. *****
 {# Default if discover is None, this happen in development mode only. #} {% set
 discover = instance.discover or dict(postgres={}, temboard={}, system={}) %}
```

### Comparing `temboard-8.0b6/temboardui/templates/login.html` & `temboard-8.1b1/temboardui/templates/login.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends base.html %}
 
-{% block title %}temBoard - Login{% end %}
+{% block title %}temBoard / Login{% end %}
 
 {% block content %}
 <div class="row justify-content-center">
   <div class="col-12 col-md-6 col-lg-4">
     <div class="card" id="panelLogin">
       <div class="card-header bg-primary text-center">
         <img src="/images/temboard-150x32-w.png" />
```

### Comparing `temboard-8.0b6/temboardui/templates/notifications.html` & `temboard-8.1b1/temboardui/templates/notifications.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends base.html %}
 
-{% block title %}[{{instance.hostname}}:{{instance.pg_port}}] - Notifications{% end %}
+{% block title %}temBoard / [{{instance}} / Notifications{% end %}
 
 {% block head %}
 <!-- DataTables CSS -->
 <link href="/js/datatables/datatables.min.css" rel="stylesheet">
 {% end %}
 
 {% block content %}
```

### Comparing `temboard-8.0b6/temboardui/templates/settings/group.html` & `temboard-8.1b1/temboardui/templates/settings/group.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/templates/settings/instance.html` & `temboard-8.1b1/temboardui/templates/settings/instance.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/templates/settings/notifications.html` & `temboard-8.1b1/temboardui/templates/settings/notifications.html`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/templates/settings/user.html` & `temboard-8.1b1/temboardui/templates/settings/user.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends ../base.html %}
 
-{% block title %}temBoard - settings{% end %}
+{% block title %}temBoard / Settings / Users{% end %}
 
 {% block head %}
 <!-- DataTables CSS -->
 <link href="/js/datatables/datatables.min.css" rel="stylesheet">
 <!-- Multiselect -->
 <link href="/css/bootstrap-multiselect.css" rel="stylesheet">
 {% end %}
```

### Comparing `temboard-8.0b6/temboardui/toolkit/app.py` & `temboard-8.1b1/temboardui/toolkit/app.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/toolkit/configuration.py` & `temboard-8.1b1/temboardui/toolkit/configuration.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/toolkit/http.py` & `temboard-8.1b1/temboardui/toolkit/http.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/toolkit/log.py` & `temboard-8.1b1/temboardui/toolkit/log.py`

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

### Comparing `temboard-8.0b6/temboardui/toolkit/perf.py` & `temboard-8.1b1/temboardui/toolkit/perf.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/toolkit/proctitle.py` & `temboard-8.1b1/temboardui/toolkit/proctitle.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/toolkit/pycompat.py` & `temboard-8.1b1/temboardui/toolkit/pycompat.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/toolkit/queries.py` & `temboard-8.1b1/temboardui/toolkit/queries.py`

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

### Comparing `temboard-8.0b6/temboardui/toolkit/services.py` & `temboard-8.1b1/temboardui/toolkit/services.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/toolkit/signing.py` & `temboard-8.1b1/temboardui/toolkit/signing.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/toolkit/tasklist/sqlite3_engine.py` & `temboard-8.1b1/temboardui/toolkit/tasklist/sqlite3_engine.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/toolkit/taskmanager.py` & `temboard-8.1b1/temboardui/toolkit/taskmanager.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/toolkit/utils.py` & `temboard-8.1b1/temboardui/toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/toolkit/validators.py` & `temboard-8.1b1/temboardui/toolkit/validators.py`

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

### Comparing `temboard-8.0b6/temboardui/toolkit/versions.py` & `temboard-8.1b1/temboardui/toolkit/versions.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/version.py` & `temboard-8.1b1/temboardui/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 from platform import python_version
 
 
-__version__ = "8.0b6"
+__version__ = "8.1b1"
 
 
 # This output is parsed by tests/conftest.py::pytest_report_header.
 VERSION_FMT = """\
 temBoard %(temboard)s (%(temboardbin)s)
 System %(distname)s %(distversion)s
 Python %(python)s (%(pythonbin)s)
```

### Comparing `temboard-8.0b6/temboardui/web/flask.py` & `temboard-8.1b1/temboardui/web/flask.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/web/routes.py` & `temboard-8.1b1/temboardui/web/routes.py`

 * *Files identical despite different names*

### Comparing `temboard-8.0b6/temboardui/web/tornado.py` & `temboard-8.1b1/temboardui/web/tornado.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,14 +291,17 @@
 
     def __getattr__(self, name):
         return getattr(self.instance, name)
 
     def __repr__(self):
         return '<%s %s>' % (self.__class__.__name__, self.instance.hostname)
 
+    def __str__(self):
+        return "%s:%s" % (self.instance.hostname, self.instance.pg_port)
+
     def check_active_plugin(self, name):
         '''
         Ensure that the plugin is active for given instance
         '''
         if name not in [p.plugin_name for p in self.instance.plugins]:
             raise HTTPError(408, "Plugin %s not activated." % name)
```

### Comparing `temboard-8.0b6/temboardui/web/vitejs.py` & `temboard-8.1b1/temboardui/web/vitejs.py`

 * *Files identical despite different names*

