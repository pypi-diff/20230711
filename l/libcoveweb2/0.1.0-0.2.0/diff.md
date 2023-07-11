# Comparing `tmp/libcoveweb2-0.1.0.tar.gz` & `tmp/libcoveweb2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcoveweb2-0.1.0.tar", last modified: Fri Jun 16 07:28:31 2023, max compression
+gzip compressed data, was "libcoveweb2-0.2.0.tar", last modified: Tue Jul 11 13:33:07 2023, max compression
```

## Comparing `libcoveweb2-0.1.0.tar` & `libcoveweb2-0.2.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.363057 libcoveweb2-0.1.0/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      295 2023-06-16 07:28:31.363057 libcoveweb2-0.1.0/PKG-INFO
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       15 2023-04-14 14:37:12.000000 libcoveweb2-0.1.0/README.md
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.355057 libcoveweb2-0.1.0/libcoveweb2/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:54.000000 libcoveweb2-0.1.0/libcoveweb2/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       65 2023-06-16 07:09:54.000000 libcoveweb2-0.1.0/libcoveweb2/admin.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      154 2023-06-16 07:09:54.000000 libcoveweb2-0.1.0/libcoveweb2/apps.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      568 2023-06-16 07:09:54.000000 libcoveweb2-0.1.0/libcoveweb2/background_worker.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1416 2023-06-16 07:11:50.000000 libcoveweb2-0.1.0/libcoveweb2/celery.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      542 2023-06-16 07:09:54.000000 libcoveweb2-0.1.0/libcoveweb2/context_processors.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:54.000000 libcoveweb2-0.1.0/libcoveweb2/forms.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.359057 libcoveweb2-0.1.0/libcoveweb2/management/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:54.000000 libcoveweb2-0.1.0/libcoveweb2/management/__init__.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.359057 libcoveweb2-0.1.0/libcoveweb2/management/commands/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:54.000000 libcoveweb2-0.1.0/libcoveweb2/management/commands/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      956 2023-06-16 07:11:50.000000 libcoveweb2-0.1.0/libcoveweb2/management/commands/expire_files.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      565 2023-06-16 07:09:54.000000 libcoveweb2-0.1.0/libcoveweb2/management/commands/reprocess_everything.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      354 2023-06-16 07:09:54.000000 libcoveweb2-0.1.0/libcoveweb2/middleware.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.359057 libcoveweb2-0.1.0/libcoveweb2/migrations/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1676 2023-06-16 07:12:05.000000 libcoveweb2-0.1.0/libcoveweb2/migrations/0001_initial.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      381 2023-06-16 07:12:05.000000 libcoveweb2-0.1.0/libcoveweb2/migrations/0002_supplieddatafile_meta.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      398 2023-06-16 07:12:05.000000 libcoveweb2-0.1.0/libcoveweb2/migrations/0003_supplieddata_expired.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      403 2023-06-16 07:12:05.000000 libcoveweb2-0.1.0/libcoveweb2/migrations/0004_supplieddatafile_source_method.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      580 2023-06-16 07:12:05.000000 libcoveweb2-0.1.0/libcoveweb2/migrations/0005_url_uploads.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      390 2023-06-16 07:12:05.000000 libcoveweb2-0.1.0/libcoveweb2/migrations/0006_supplieddata_processed.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      393 2023-06-16 07:12:05.000000 libcoveweb2-0.1.0/libcoveweb2/migrations/0007_supplieddata_error.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      551 2023-06-16 07:12:05.000000 libcoveweb2-0.1.0/libcoveweb2/migrations/0008_auto_20230414_0851.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/migrations/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     6209 2023-06-16 07:14:18.000000 libcoveweb2-0.1.0/libcoveweb2/models.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.359057 libcoveweb2-0.1.0/libcoveweb2/process/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/process/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2098 2023-06-16 07:12:26.000000 libcoveweb2-0.1.0/libcoveweb2/process/base.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.359057 libcoveweb2-0.1.0/libcoveweb2/process/common_tasks/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/process/common_tasks/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      854 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/process/common_tasks/download_data_task.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1965 2023-06-16 07:12:58.000000 libcoveweb2-0.1.0/libcoveweb2/process/common_tasks/task_with_state.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1983 2023-06-16 07:21:02.000000 libcoveweb2-0.1.0/libcoveweb2/process/utils.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     5367 2023-06-16 07:12:35.000000 libcoveweb2-0.1.0/libcoveweb2/settings.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.355057 libcoveweb2-0.1.0/libcoveweb2/static/
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.355057 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.359057 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/css/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1833 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/css/style.css
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.355057 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.359057 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/bootstrap/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    20127 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.eot
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)   108738 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.svg
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    45404 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.ttf
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    23424 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    18028 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.359057 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/tick/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      408 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/tick/tick.css
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2328 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/tick/tick.eot
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3063 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/tick/tick.svg
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2168 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/tick/tick.ttf
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1604 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/tick/tick.woff
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1064 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/tick/tick.woff2
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.355057 libcoveweb2-0.1.0/libcoveweb2/templates/
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.363057 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1114 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/500.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2811 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/additional_fields_table.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     4935 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/base.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      760 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/error.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      405 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/error_extra.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2431 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/explore.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      479 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/google_analytics.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1157 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/piwik.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      625 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/processing.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      121 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/show_json_value.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1154 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1966 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_conditions.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2137 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_conditions_intro.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2067 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_cookies.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      195 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_cookies_link_google_analytics.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      124 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_cookies_link_matmo.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      129 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_cookies_links.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      484 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_cookies_we_use.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      830 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_data_deleting.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      764 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_data_uploaded.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1357 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_disclaimer.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      525 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_links.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1460 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_privacy.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1044 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_privacy_intro.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      279 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_security.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_tracker_data_controller_international.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      804 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_tracker_google_analytics.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1221 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_tracker_matmo.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       81 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_tracker_no_international.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      981 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_tracker_sentry.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      880 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_tracker_server.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      475 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_trackers.html
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.363057 libcoveweb2-0.1.0/libcoveweb2/templatetags/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templatetags/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1738 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/templatetags/cove_tags.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.363057 libcoveweb2-0.1.0/libcoveweb2/tests/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/tests/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      767 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/tests/lib_functional.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      372 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/urls.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1585 2023-06-16 07:09:55.000000 libcoveweb2-0.1.0/libcoveweb2/utils.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    10088 2023-06-16 07:11:19.000000 libcoveweb2-0.1.0/libcoveweb2/views.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:28:31.359057 libcoveweb2-0.1.0/libcoveweb2.egg-info/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      295 2023-06-16 07:28:31.000000 libcoveweb2-0.1.0/libcoveweb2.egg-info/PKG-INFO
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     4106 2023-06-16 07:28:31.000000 libcoveweb2-0.1.0/libcoveweb2.egg-info/SOURCES.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        1 2023-06-16 07:28:31.000000 libcoveweb2-0.1.0/libcoveweb2.egg-info/dependency_links.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      105 2023-06-16 07:28:31.000000 libcoveweb2-0.1.0/libcoveweb2.egg-info/requires.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       12 2023-06-16 07:28:31.000000 libcoveweb2-0.1.0/libcoveweb2.egg-info/top_level.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       31 2023-05-09 14:49:49.000000 libcoveweb2-0.1.0/pyproject.toml
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       90 2023-06-16 07:28:31.363057 libcoveweb2-0.1.0/setup.cfg
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      840 2023-06-16 07:24:28.000000 libcoveweb2-0.1.0/setup.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.236936 libcoveweb2-0.2.0/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      295 2023-07-11 13:33:07.236936 libcoveweb2-0.2.0/PKG-INFO
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       15 2023-04-14 14:37:12.000000 libcoveweb2-0.2.0/README.md
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.228936 libcoveweb2-0.2.0/libcoveweb2/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:54.000000 libcoveweb2-0.2.0/libcoveweb2/__init__.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       65 2023-06-16 07:09:54.000000 libcoveweb2-0.2.0/libcoveweb2/admin.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      154 2023-06-16 07:09:54.000000 libcoveweb2-0.2.0/libcoveweb2/apps.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      568 2023-06-16 07:09:54.000000 libcoveweb2-0.2.0/libcoveweb2/background_worker.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1416 2023-06-16 07:11:50.000000 libcoveweb2-0.2.0/libcoveweb2/celery.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      542 2023-06-16 07:09:54.000000 libcoveweb2-0.2.0/libcoveweb2/context_processors.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:54.000000 libcoveweb2-0.2.0/libcoveweb2/forms.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.228936 libcoveweb2-0.2.0/libcoveweb2/management/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:54.000000 libcoveweb2-0.2.0/libcoveweb2/management/__init__.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.228936 libcoveweb2-0.2.0/libcoveweb2/management/commands/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:54.000000 libcoveweb2-0.2.0/libcoveweb2/management/commands/__init__.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      956 2023-06-16 07:11:50.000000 libcoveweb2-0.2.0/libcoveweb2/management/commands/expire_files.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      565 2023-06-16 07:09:54.000000 libcoveweb2-0.2.0/libcoveweb2/management/commands/reprocess_everything.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      354 2023-06-16 07:09:54.000000 libcoveweb2-0.2.0/libcoveweb2/middleware.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.232936 libcoveweb2-0.2.0/libcoveweb2/migrations/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1676 2023-06-16 07:12:05.000000 libcoveweb2-0.2.0/libcoveweb2/migrations/0001_initial.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      381 2023-06-16 07:12:05.000000 libcoveweb2-0.2.0/libcoveweb2/migrations/0002_supplieddatafile_meta.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      398 2023-06-16 07:12:05.000000 libcoveweb2-0.2.0/libcoveweb2/migrations/0003_supplieddata_expired.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      403 2023-06-16 07:12:05.000000 libcoveweb2-0.2.0/libcoveweb2/migrations/0004_supplieddatafile_source_method.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      580 2023-06-16 07:12:05.000000 libcoveweb2-0.2.0/libcoveweb2/migrations/0005_url_uploads.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      390 2023-06-16 07:12:05.000000 libcoveweb2-0.2.0/libcoveweb2/migrations/0006_supplieddata_processed.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      393 2023-06-16 07:12:05.000000 libcoveweb2-0.2.0/libcoveweb2/migrations/0007_supplieddata_error.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      551 2023-06-16 07:12:05.000000 libcoveweb2-0.2.0/libcoveweb2/migrations/0008_auto_20230414_0851.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/migrations/__init__.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     6594 2023-07-07 16:50:55.000000 libcoveweb2-0.2.0/libcoveweb2/models.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.232936 libcoveweb2-0.2.0/libcoveweb2/process/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/process/__init__.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2098 2023-06-16 07:12:26.000000 libcoveweb2-0.2.0/libcoveweb2/process/base.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.232936 libcoveweb2-0.2.0/libcoveweb2/process/common_tasks/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/process/common_tasks/__init__.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      854 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/process/common_tasks/download_data_task.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1965 2023-06-16 07:12:58.000000 libcoveweb2-0.2.0/libcoveweb2/process/common_tasks/task_with_state.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1983 2023-06-16 07:21:02.000000 libcoveweb2-0.2.0/libcoveweb2/process/utils.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     5367 2023-06-16 07:12:35.000000 libcoveweb2-0.2.0/libcoveweb2/settings.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.228936 libcoveweb2-0.2.0/libcoveweb2/static/
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.228936 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.232936 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/css/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1833 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/css/style.css
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.228936 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.232936 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/bootstrap/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)    20127 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.eot
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)   108738 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.svg
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)    45404 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)    23424 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)    18028 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.232936 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/tick/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      408 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/tick/tick.css
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2328 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/tick/tick.eot
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3063 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/tick/tick.svg
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2168 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/tick/tick.ttf
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1604 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/tick/tick.woff
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1064 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/tick/tick.woff2
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.228936 libcoveweb2-0.2.0/libcoveweb2/templates/
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.236936 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1114 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/500.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2811 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/additional_fields_table.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     4935 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/base.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      760 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/error.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      405 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/error_extra.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2431 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/explore.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      479 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/google_analytics.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1157 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/piwik.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      625 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/processing.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      121 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/show_json_value.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1154 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1966 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_conditions.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2137 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_conditions_intro.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2067 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_cookies.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      195 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_cookies_link_google_analytics.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      124 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_cookies_link_matmo.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      129 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_cookies_links.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      484 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_cookies_we_use.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      830 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_data_deleting.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      764 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_data_uploaded.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1357 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_disclaimer.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      525 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_links.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1460 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_privacy.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1044 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_privacy_intro.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      279 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_security.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_tracker_data_controller_international.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      804 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_tracker_google_analytics.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1221 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_tracker_matmo.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       81 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_tracker_no_international.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      981 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_tracker_sentry.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      880 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_tracker_server.html
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      475 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_trackers.html
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.236936 libcoveweb2-0.2.0/libcoveweb2/templatetags/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templatetags/__init__.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1738 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/templatetags/cove_tags.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.236936 libcoveweb2-0.2.0/libcoveweb2/tests/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/tests/__init__.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      767 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/tests/lib_functional.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      372 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/urls.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1585 2023-06-16 07:09:55.000000 libcoveweb2-0.2.0/libcoveweb2/utils.py
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)    10088 2023-07-11 13:31:25.000000 libcoveweb2-0.2.0/libcoveweb2/views.py
+drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2023-07-11 13:33:07.228936 libcoveweb2-0.2.0/libcoveweb2.egg-info/
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      295 2023-07-11 13:33:07.000000 libcoveweb2-0.2.0/libcoveweb2.egg-info/PKG-INFO
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)     4106 2023-07-11 13:33:07.000000 libcoveweb2-0.2.0/libcoveweb2.egg-info/SOURCES.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)        1 2023-07-11 13:33:07.000000 libcoveweb2-0.2.0/libcoveweb2.egg-info/dependency_links.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      105 2023-07-11 13:33:07.000000 libcoveweb2-0.2.0/libcoveweb2.egg-info/requires.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       12 2023-07-11 13:33:07.000000 libcoveweb2-0.2.0/libcoveweb2.egg-info/top_level.txt
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       31 2023-05-09 14:49:49.000000 libcoveweb2-0.2.0/pyproject.toml
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)       90 2023-07-11 13:33:07.236936 libcoveweb2-0.2.0/setup.cfg
+-rw-r--r--   0 odscjames  (1000) odscjames  (1000)      840 2023-07-11 13:31:46.000000 libcoveweb2-0.2.0/setup.py
```

### Comparing `libcoveweb2-0.1.0/libcoveweb2/background_worker.py` & `libcoveweb2-0.2.0/libcoveweb2/background_worker.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/celery.py` & `libcoveweb2-0.2.0/libcoveweb2/celery.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/context_processors.py` & `libcoveweb2-0.2.0/libcoveweb2/context_processors.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/management/commands/expire_files.py` & `libcoveweb2-0.2.0/libcoveweb2/management/commands/expire_files.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/management/commands/reprocess_everything.py` & `libcoveweb2-0.2.0/libcoveweb2/management/commands/reprocess_everything.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/migrations/0001_initial.py` & `libcoveweb2-0.2.0/libcoveweb2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/migrations/0005_url_uploads.py` & `libcoveweb2-0.2.0/libcoveweb2/migrations/0005_url_uploads.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/migrations/0008_auto_20230414_0851.py` & `libcoveweb2-0.2.0/libcoveweb2/migrations/0008_auto_20230414_0851.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/models.py` & `libcoveweb2-0.2.0/libcoveweb2/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,14 +134,27 @@
             settings.MEDIA_URL,
             str(self.supplied_data.id),
             "supplied_data",
             str(self.id),
             self.filename,
         )
 
+    def storage_name(self):
+        """For use with Django storage classes.
+        Returns full name in storage
+        Example use:
+        default_storage.open(os.path.join(supplied_data_file.storage_name())
+        """
+        return os.path.join(
+            str(self.supplied_data.id),
+            "supplied_data",
+            str(self.id),
+            self.filename,
+        )
+
     def does_exist_in_storage(self):
         return os.path.exists(self.upload_dir_and_filename())
 
     def is_download_from_source_url_needed(self) -> bool:
         return (
             not self.supplied_data.expired
             and self.source_url
```

### Comparing `libcoveweb2-0.1.0/libcoveweb2/process/base.py` & `libcoveweb2-0.2.0/libcoveweb2/process/base.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/process/common_tasks/download_data_task.py` & `libcoveweb2-0.2.0/libcoveweb2/process/common_tasks/download_data_task.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/process/common_tasks/task_with_state.py` & `libcoveweb2-0.2.0/libcoveweb2/process/common_tasks/task_with_state.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/process/utils.py` & `libcoveweb2-0.2.0/libcoveweb2/process/utils.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/settings.py` & `libcoveweb2-0.2.0/libcoveweb2/settings.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/css/style.css` & `libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/css/style.css`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.eot` & `libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.svg` & `libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.ttf` & `libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff` & `libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff2` & `libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/tick/tick.eot` & `libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/tick/tick.eot`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/tick/tick.svg` & `libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/tick/tick.svg`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/tick/tick.ttf` & `libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/tick/tick.ttf`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/tick/tick.woff` & `libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/tick/tick.woff`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/static/dataexplore/fonts/tick/tick.woff2` & `libcoveweb2-0.2.0/libcoveweb2/static/dataexplore/fonts/tick/tick.woff2`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/500.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/500.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/additional_fields_table.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/additional_fields_table.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/base.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/base.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/error.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/error.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/explore.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/explore.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/piwik.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/piwik.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/processing.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/processing.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_conditions.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_conditions.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_conditions_intro.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_conditions_intro.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_cookies.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_cookies.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_data_deleting.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_data_deleting.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_data_uploaded.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_data_uploaded.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_disclaimer.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_disclaimer.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_links.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_links.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_privacy.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_privacy.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_privacy_intro.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_privacy_intro.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_tracker_google_analytics.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_tracker_google_analytics.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_tracker_matmo.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_tracker_matmo.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_tracker_sentry.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_tracker_sentry.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templates/libcoveweb2/terms_tracker_server.html` & `libcoveweb2-0.2.0/libcoveweb2/templates/libcoveweb2/terms_tracker_server.html`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/templatetags/cove_tags.py` & `libcoveweb2-0.2.0/libcoveweb2/templatetags/cove_tags.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/tests/lib_functional.py` & `libcoveweb2-0.2.0/libcoveweb2/tests/lib_functional.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/utils.py` & `libcoveweb2-0.2.0/libcoveweb2/utils.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2/views.py` & `libcoveweb2-0.2.0/libcoveweb2/views.py`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/libcoveweb2.egg-info/SOURCES.txt` & `libcoveweb2-0.2.0/libcoveweb2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libcoveweb2-0.1.0/setup.py` & `libcoveweb2-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 install_requires = []
 
 setup(
     name="libcoveweb2",
-    version="0.1.0",
+    version="0.2.0",
     author="Open Data Services",
     author_email="code@opendataservices.coop",
     packages=find_packages(),
     package_data={
         "libcoveweb2": [
             "static/*",
             "static/*/*",
```

