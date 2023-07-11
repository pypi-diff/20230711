# Comparing `tmp/aa-killtracker-0.9.1.tar.gz` & `tmp/aa-killtracker-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-killtracker-0.9.1.tar", last modified: Fri Oct 14 16:08:55 2022, max compression
+gzip compressed data, was "aa-killtracker-0.9.2.tar", last modified: Mon Oct 17 13:06:38 2022, max compression
```

## Comparing `aa-killtracker-0.9.1.tar` & `aa-killtracker-0.9.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.305410 aa-killtracker-0.9.1/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2020-12-08 23:35:55.000000 aa-killtracker-0.9.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      292 2022-07-16 12:04:16.000000 aa-killtracker-0.9.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12275 2022-10-14 16:08:55.305410 aa-killtracker-0.9.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11346 2021-05-26 14:33:43.000000 aa-killtracker-0.9.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.273410 aa-killtracker-0.9.1/aa_killtracker.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12275 2022-10-14 16:08:55.000000 aa-killtracker-0.9.1/aa_killtracker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2539 2022-10-14 16:08:55.000000 aa-killtracker-0.9.1/aa_killtracker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-14 16:08:55.000000 aa-killtracker-0.9.1/aa_killtracker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2022-10-14 16:08:55.000000 aa-killtracker-0.9.1/aa_killtracker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-10-14 16:08:55.000000 aa-killtracker-0.9.1/aa_killtracker.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.285410 aa-killtracker-0.9.1/killtracker/
--rw-rw-rw-   0 root         (0) root         (0)      245 2022-10-14 15:39:58.000000 aa-killtracker-0.9.1/killtracker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17741 2022-10-12 12:14:44.000000 aa-killtracker-0.9.1/killtracker/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2815 2022-10-14 15:31:47.000000 aa-killtracker-0.9.1/killtracker/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2022-06-16 20:00:05.000000 aa-killtracker-0.9.1/killtracker/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2022-07-15 19:50:31.000000 aa-killtracker-0.9.1/killtracker/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      305 2022-07-16 11:21:17.000000 aa-killtracker-0.9.1/killtracker/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.285410 aa-killtracker-0.9.1/killtracker/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-12-08 23:35:55.000000 aa-killtracker-0.9.1/killtracker/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10985 2022-09-21 18:17:31.000000 aa-killtracker-0.9.1/killtracker/core/discord_messages.py
--rw-rw-rw-   0 root         (0) root         (0)    14220 2022-10-14 15:31:47.000000 aa-killtracker-0.9.1/killtracker/core/killmails.py
--rw-rw-rw-   0 root         (0) root         (0)      713 2022-10-14 15:31:47.000000 aa-killtracker-0.9.1/killtracker/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5038 2022-06-04 18:12:40.000000 aa-killtracker-0.9.1/killtracker/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.261410 aa-killtracker-0.9.1/killtracker/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.289410 aa-killtracker-0.9.1/killtracker/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      979 2022-07-15 19:50:31.000000 aa-killtracker-0.9.1/killtracker/management/commands/killtracker_load_eve.py
--rw-rw-rw-   0 root         (0) root         (0)     4391 2022-10-12 12:14:44.000000 aa-killtracker-0.9.1/killtracker/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.293410 aa-killtracker-0.9.1/killtracker/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    27819 2022-10-12 12:14:44.000000 aa-killtracker-0.9.1/killtracker/migrations/0001_initial_new.py
--rw-rw-rw-   0 root         (0) root         (0)    26222 2022-09-21 18:41:47.000000 aa-killtracker-0.9.1/killtracker/migrations/0001_squashed_all.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2021-01-08 13:08:20.000000 aa-killtracker-0.9.1/killtracker/migrations/0002_fix_webhook_notes_field.py
--rw-rw-rw-   0 root         (0) root         (0)     1664 2021-05-25 21:27:13.000000 aa-killtracker-0.9.1/killtracker/migrations/0003_add_state_clauses.py
--rw-rw-rw-   0 root         (0) root         (0)     7543 2022-03-02 21:40:57.000000 aa-killtracker-0.9.1/killtracker/migrations/0004_django4_update.py
--rw-rw-rw-   0 root         (0) root         (0)    15551 2022-06-04 18:21:44.000000 aa-killtracker-0.9.1/killtracker/migrations/0005_add_final_blow_clause_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      570 2022-07-15 19:50:31.000000 aa-killtracker-0.9.1/killtracker/migrations/0006_evetypeplus.py
--rw-rw-rw-   0 root         (0) root         (0)     4693 2022-10-12 12:14:44.000000 aa-killtracker-0.9.1/killtracker/migrations/0007_restructure_killsmails.py
--rw-rw-rw-   0 root         (0) root         (0)     2373 2022-10-12 12:14:44.000000 aa-killtracker-0.9.1/killtracker/migrations/0008_copy_data_to_new_structure.py
--rw-rw-rw-   0 root         (0) root         (0)     1292 2022-10-12 12:14:44.000000 aa-killtracker-0.9.1/killtracker/migrations/0009_remove_old_models.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-12-08 23:35:55.000000 aa-killtracker-0.9.1/killtracker/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    44312 2022-10-12 12:14:44.000000 aa-killtracker-0.9.1/killtracker/models.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2022-06-16 20:00:05.000000 aa-killtracker-0.9.1/killtracker/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.261410 aa-killtracker-0.9.1/killtracker/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.293410 aa-killtracker-0.9.1/killtracker/static/killtracker/
--rw-rw-rw-   0 root         (0) root         (0)    74625 2020-12-08 23:35:55.000000 aa-killtracker-0.9.1/killtracker/static/killtracker/killtracker_logo.png
--rw-rw-rw-   0 root         (0) root         (0)      328 2020-12-08 23:35:55.000000 aa-killtracker-0.9.1/killtracker/static/killtracker/zkb_icon.png
--rw-rw-rw-   0 root         (0) root         (0)  1753397 2020-12-08 23:35:55.000000 aa-killtracker-0.9.1/killtracker/swagger.json
--rw-rw-rw-   0 root         (0) root         (0)     7848 2022-10-14 15:31:47.000000 aa-killtracker-0.9.1/killtracker/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.261410 aa-killtracker-0.9.1/killtracker/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.269410 aa-killtracker-0.9.1/killtracker/templates/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.269410 aa-killtracker-0.9.1/killtracker/templates/admin/killtracker/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.293410 aa-killtracker-0.9.1/killtracker/templates/admin/killtracker/tracker/
--rw-rw-rw-   0 root         (0) root         (0)      519 2022-07-16 16:34:37.000000 aa-killtracker-0.9.1/killtracker/templates/admin/killtracker/tracker/change_form.html
--rw-rw-rw-   0 root         (0) root         (0)      497 2022-07-15 19:50:31.000000 aa-killtracker-0.9.1/killtracker/templates/admin/killtracker/tracker/killmail_test.html
--rw-rw-rw-   0 root         (0) root         (0)      701 2022-07-16 16:34:37.000000 aa-killtracker-0.9.1/killtracker/templates/admin/killtracker/tracker/toogle_npc_button.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.297410 aa-killtracker-0.9.1/killtracker/tests/
--rw-rw-rw-   0 root         (0) root         (0)      278 2022-06-04 18:12:40.000000 aa-killtracker-0.9.1/killtracker/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.297410 aa-killtracker-0.9.1/killtracker/tests/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:53:07.000000 aa-killtracker-0.9.1/killtracker/tests/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2022-08-31 13:53:07.000000 aa-killtracker-0.9.1/killtracker/tests/core/test_discord_messages.py
--rw-rw-rw-   0 root         (0) root         (0)    10762 2022-10-14 15:31:47.000000 aa-killtracker-0.9.1/killtracker/tests/core/test_killmails.py
--rw-rw-rw-   0 root         (0) root         (0)    11439 2022-08-31 13:53:07.000000 aa-killtracker-0.9.1/killtracker/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1120 2021-02-18 15:20:33.000000 aa-killtracker-0.9.1/killtracker/tests/test_admin_2.py
--rw-rw-rw-   0 root         (0) root         (0)      316 2021-05-25 21:27:13.000000 aa-killtracker-0.9.1/killtracker/tests/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3154 2022-08-31 13:53:07.000000 aa-killtracker-0.9.1/killtracker/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)    17214 2022-10-12 12:14:44.000000 aa-killtracker-0.9.1/killtracker/tests/test_models_1.py
--rw-rw-rw-   0 root         (0) root         (0)    32539 2022-08-31 14:14:56.000000 aa-killtracker-0.9.1/killtracker/tests/test_models_2.py
--rw-rw-rw-   0 root         (0) root         (0)     4741 2022-08-31 14:14:56.000000 aa-killtracker-0.9.1/killtracker/tests/test_models_discord_service.py
--rw-rw-rw-   0 root         (0) root         (0)    13893 2022-10-14 15:31:47.000000 aa-killtracker-0.9.1/killtracker/tests/test_tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.301410 aa-killtracker-0.9.1/killtracker/tests/testdata/
--rw-rw-rw-   0 root         (0) root         (0)      255 2020-12-08 23:35:55.000000 aa-killtracker-0.9.1/killtracker/tests/testdata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      966 2022-07-16 12:04:16.000000 aa-killtracker-0.9.1/killtracker/tests/testdata/create_eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2020-12-08 23:35:55.000000 aa-killtracker-0.9.1/killtracker/tests/testdata/evealliances.json
--rw-rw-rw-   0 root         (0) root         (0)     1229 2020-12-08 23:35:55.000000 aa-killtracker-0.9.1/killtracker/tests/testdata/evecorporations.json
--rw-rw-rw-   0 root         (0) root         (0)     1459 2020-12-08 23:35:55.000000 aa-killtracker-0.9.1/killtracker/tests/testdata/eveentities.json
--rw-rw-rw-   0 root         (0) root         (0)    36117 2022-07-16 12:04:16.000000 aa-killtracker-0.9.1/killtracker/tests/testdata/eveuniverse.json
--rw-rw-rw-   0 root         (0) root         (0)     3276 2022-06-05 13:01:34.000000 aa-killtracker-0.9.1/killtracker/tests/testdata/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     4730 2021-05-25 21:27:13.000000 aa-killtracker-0.9.1/killtracker/tests/testdata/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    45366 2020-12-08 23:35:55.000000 aa-killtracker-0.9.1/killtracker/tests/testdata/killmails.json
--rw-rw-rw-   0 root         (0) root         (0)      388 2020-12-08 23:35:55.000000 aa-killtracker-0.9.1/killtracker/tests/testdata/load_eveuniverse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 16:08:55.301410 aa-killtracker-0.9.1/killtracker/tools/
--rw-rw-rw-   0 root         (0) root         (0)     1726 2021-01-03 23:24:51.000000 aa-killtracker-0.9.1/killtracker/tools/drop_tables_killtracker.sql
--rw-rw-rw-   0 root         (0) root         (0)      768 2020-12-08 23:35:55.000000 aa-killtracker-0.9.1/killtracker/tools/generate_conditions_text.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2022-07-16 16:34:37.000000 aa-killtracker-0.9.1/killtracker/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      832 2022-07-16 16:34:37.000000 aa-killtracker-0.9.1/killtracker/views.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-14 16:08:55.305410 aa-killtracker-0.9.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1666 2022-10-12 12:14:44.000000 aa-killtracker-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.499780 aa-killtracker-0.9.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2020-12-08 23:35:55.000000 aa-killtracker-0.9.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      292 2022-07-16 12:04:16.000000 aa-killtracker-0.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12275 2022-10-17 13:06:38.495780 aa-killtracker-0.9.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11346 2021-05-26 14:33:43.000000 aa-killtracker-0.9.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.467780 aa-killtracker-0.9.2/aa_killtracker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12275 2022-10-17 13:06:38.000000 aa-killtracker-0.9.2/aa_killtracker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2539 2022-10-17 13:06:38.000000 aa-killtracker-0.9.2/aa_killtracker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-10-17 13:06:38.000000 aa-killtracker-0.9.2/aa_killtracker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2022-10-17 13:06:38.000000 aa-killtracker-0.9.2/aa_killtracker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2022-10-17 13:06:38.000000 aa-killtracker-0.9.2/aa_killtracker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.483780 aa-killtracker-0.9.2/killtracker/
+-rw-rw-rw-   0 root         (0) root         (0)      245 2022-10-17 12:15:30.000000 aa-killtracker-0.9.2/killtracker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17920 2022-10-17 12:36:25.000000 aa-killtracker-0.9.2/killtracker/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2815 2022-10-14 15:31:47.000000 aa-killtracker-0.9.2/killtracker/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2022-06-16 20:00:05.000000 aa-killtracker-0.9.2/killtracker/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2022-07-15 19:50:31.000000 aa-killtracker-0.9.2/killtracker/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)      305 2022-07-16 11:21:17.000000 aa-killtracker-0.9.2/killtracker/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.483780 aa-killtracker-0.9.2/killtracker/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-12-08 23:35:55.000000 aa-killtracker-0.9.2/killtracker/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10985 2022-09-21 18:17:31.000000 aa-killtracker-0.9.2/killtracker/core/discord_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)    14421 2022-10-17 12:15:30.000000 aa-killtracker-0.9.2/killtracker/core/killmails.py
+-rw-rw-rw-   0 root         (0) root         (0)      713 2022-10-14 15:31:47.000000 aa-killtracker-0.9.2/killtracker/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5038 2022-06-04 18:12:40.000000 aa-killtracker-0.9.2/killtracker/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.463780 aa-killtracker-0.9.2/killtracker/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.483780 aa-killtracker-0.9.2/killtracker/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      979 2022-07-15 19:50:31.000000 aa-killtracker-0.9.2/killtracker/management/commands/killtracker_load_eve.py
+-rw-rw-rw-   0 root         (0) root         (0)     4391 2022-10-12 12:14:44.000000 aa-killtracker-0.9.2/killtracker/managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.487780 aa-killtracker-0.9.2/killtracker/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    27819 2022-10-12 12:14:44.000000 aa-killtracker-0.9.2/killtracker/migrations/0001_initial_new.py
+-rw-rw-rw-   0 root         (0) root         (0)    26222 2022-09-21 18:41:47.000000 aa-killtracker-0.9.2/killtracker/migrations/0001_squashed_all.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2021-01-08 13:08:20.000000 aa-killtracker-0.9.2/killtracker/migrations/0002_fix_webhook_notes_field.py
+-rw-rw-rw-   0 root         (0) root         (0)     1664 2021-05-25 21:27:13.000000 aa-killtracker-0.9.2/killtracker/migrations/0003_add_state_clauses.py
+-rw-rw-rw-   0 root         (0) root         (0)     7543 2022-03-02 21:40:57.000000 aa-killtracker-0.9.2/killtracker/migrations/0004_django4_update.py
+-rw-rw-rw-   0 root         (0) root         (0)    15551 2022-06-04 18:21:44.000000 aa-killtracker-0.9.2/killtracker/migrations/0005_add_final_blow_clause_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      570 2022-07-15 19:50:31.000000 aa-killtracker-0.9.2/killtracker/migrations/0006_evetypeplus.py
+-rw-rw-rw-   0 root         (0) root         (0)     4693 2022-10-12 12:14:44.000000 aa-killtracker-0.9.2/killtracker/migrations/0007_restructure_killsmails.py
+-rw-rw-rw-   0 root         (0) root         (0)     2373 2022-10-12 12:14:44.000000 aa-killtracker-0.9.2/killtracker/migrations/0008_copy_data_to_new_structure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2022-10-12 12:14:44.000000 aa-killtracker-0.9.2/killtracker/migrations/0009_remove_old_models.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-12-08 23:35:55.000000 aa-killtracker-0.9.2/killtracker/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    44312 2022-10-12 12:14:44.000000 aa-killtracker-0.9.2/killtracker/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2022-06-16 20:00:05.000000 aa-killtracker-0.9.2/killtracker/providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.463780 aa-killtracker-0.9.2/killtracker/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.487780 aa-killtracker-0.9.2/killtracker/static/killtracker/
+-rw-rw-rw-   0 root         (0) root         (0)    74625 2020-12-08 23:35:55.000000 aa-killtracker-0.9.2/killtracker/static/killtracker/killtracker_logo.png
+-rw-rw-rw-   0 root         (0) root         (0)      328 2020-12-08 23:35:55.000000 aa-killtracker-0.9.2/killtracker/static/killtracker/zkb_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)  1753397 2020-12-08 23:35:55.000000 aa-killtracker-0.9.2/killtracker/swagger.json
+-rw-rw-rw-   0 root         (0) root         (0)     7876 2022-10-17 12:15:30.000000 aa-killtracker-0.9.2/killtracker/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.467780 aa-killtracker-0.9.2/killtracker/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.467780 aa-killtracker-0.9.2/killtracker/templates/admin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.467780 aa-killtracker-0.9.2/killtracker/templates/admin/killtracker/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.487780 aa-killtracker-0.9.2/killtracker/templates/admin/killtracker/tracker/
+-rw-rw-rw-   0 root         (0) root         (0)      519 2022-07-16 16:34:37.000000 aa-killtracker-0.9.2/killtracker/templates/admin/killtracker/tracker/change_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      649 2022-10-17 12:36:25.000000 aa-killtracker-0.9.2/killtracker/templates/admin/killtracker/tracker/killmail_test.html
+-rw-rw-rw-   0 root         (0) root         (0)      701 2022-07-16 16:34:37.000000 aa-killtracker-0.9.2/killtracker/templates/admin/killtracker/tracker/toogle_npc_button.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.491780 aa-killtracker-0.9.2/killtracker/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      278 2022-06-04 18:12:40.000000 aa-killtracker-0.9.2/killtracker/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.491780 aa-killtracker-0.9.2/killtracker/tests/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-31 13:53:07.000000 aa-killtracker-0.9.2/killtracker/tests/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2022-08-31 13:53:07.000000 aa-killtracker-0.9.2/killtracker/tests/core/test_discord_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)    11692 2022-10-17 12:15:30.000000 aa-killtracker-0.9.2/killtracker/tests/core/test_killmails.py
+-rw-rw-rw-   0 root         (0) root         (0)    11439 2022-08-31 13:53:07.000000 aa-killtracker-0.9.2/killtracker/tests/test_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2021-02-18 15:20:33.000000 aa-killtracker-0.9.2/killtracker/tests/test_admin_2.py
+-rw-rw-rw-   0 root         (0) root         (0)      316 2021-05-25 21:27:13.000000 aa-killtracker-0.9.2/killtracker/tests/test_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3154 2022-08-31 13:53:07.000000 aa-killtracker-0.9.2/killtracker/tests/test_integration.py
+-rw-rw-rw-   0 root         (0) root         (0)    17214 2022-10-12 12:14:44.000000 aa-killtracker-0.9.2/killtracker/tests/test_models_1.py
+-rw-rw-rw-   0 root         (0) root         (0)    32539 2022-08-31 14:14:56.000000 aa-killtracker-0.9.2/killtracker/tests/test_models_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4741 2022-08-31 14:14:56.000000 aa-killtracker-0.9.2/killtracker/tests/test_models_discord_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    13893 2022-10-14 15:31:47.000000 aa-killtracker-0.9.2/killtracker/tests/test_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.495780 aa-killtracker-0.9.2/killtracker/tests/testdata/
+-rw-rw-rw-   0 root         (0) root         (0)      255 2020-12-08 23:35:55.000000 aa-killtracker-0.9.2/killtracker/tests/testdata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      966 2022-07-16 12:04:16.000000 aa-killtracker-0.9.2/killtracker/tests/testdata/create_eveuniverse.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2020-12-08 23:35:55.000000 aa-killtracker-0.9.2/killtracker/tests/testdata/evealliances.json
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2020-12-08 23:35:55.000000 aa-killtracker-0.9.2/killtracker/tests/testdata/evecorporations.json
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2020-12-08 23:35:55.000000 aa-killtracker-0.9.2/killtracker/tests/testdata/eveentities.json
+-rw-rw-rw-   0 root         (0) root         (0)    36117 2022-07-16 12:04:16.000000 aa-killtracker-0.9.2/killtracker/tests/testdata/eveuniverse.json
+-rw-rw-rw-   0 root         (0) root         (0)     3276 2022-06-05 13:01:34.000000 aa-killtracker-0.9.2/killtracker/tests/testdata/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)     4730 2021-05-25 21:27:13.000000 aa-killtracker-0.9.2/killtracker/tests/testdata/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    45366 2020-12-08 23:35:55.000000 aa-killtracker-0.9.2/killtracker/tests/testdata/killmails.json
+-rw-rw-rw-   0 root         (0) root         (0)      388 2020-12-08 23:35:55.000000 aa-killtracker-0.9.2/killtracker/tests/testdata/load_eveuniverse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 13:06:38.495780 aa-killtracker-0.9.2/killtracker/tools/
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2021-01-03 23:24:51.000000 aa-killtracker-0.9.2/killtracker/tools/drop_tables_killtracker.sql
+-rw-rw-rw-   0 root         (0) root         (0)      768 2020-12-08 23:35:55.000000 aa-killtracker-0.9.2/killtracker/tools/generate_conditions_text.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2022-07-16 16:34:37.000000 aa-killtracker-0.9.2/killtracker/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      832 2022-07-16 16:34:37.000000 aa-killtracker-0.9.2/killtracker/views.py
+-rw-r--r--   0 root         (0) root         (0)       38 2022-10-17 13:06:38.499780 aa-killtracker-0.9.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1666 2022-10-12 12:14:44.000000 aa-killtracker-0.9.2/setup.py
```

### Comparing `aa-killtracker-0.9.1/LICENSE` & `aa-killtracker-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/PKG-INFO` & `aa-killtracker-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-killtracker
-Version: 0.9.1
+Version: 0.9.2
 Summary: An app for running killmail trackers with Alliance Auth and Discord
 Home-page: https://gitlab.com/ErikKalkoken/aa-killtracker
 Author: Erik Kalkoken
 Author-email: kalkoken87@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `aa-killtracker-0.9.1/README.md` & `aa-killtracker-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/aa_killtracker.egg-info/PKG-INFO` & `aa-killtracker-0.9.2/aa_killtracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-killtracker
-Version: 0.9.1
+Version: 0.9.2
 Summary: An app for running killmail trackers with Alliance Auth and Discord
 Home-page: https://gitlab.com/ErikKalkoken/aa-killtracker
 Author: Erik Kalkoken
 Author-email: kalkoken87@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `aa-killtracker-0.9.1/aa_killtracker.egg-info/SOURCES.txt` & `aa-killtracker-0.9.2/aa_killtracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/admin.py` & `aa-killtracker-0.9.2/killtracker/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from django.db.models import Q
 from django.db.models.functions import Lower
 from django.http import HttpResponse, HttpResponseRedirect
 from django.shortcuts import get_object_or_404, render
 from django.utils.safestring import mark_safe
 from eveuniverse.models import EveGroup
 
+from allianceauth import NAME as site_header
 from allianceauth.eveonline.models import EveAllianceInfo, EveCorporationInfo
 
 from . import tasks
 from .constants import (
     SESSION_KEY_TOOGLE_NPC,
     SESSION_KEY_USES_NPC,
     EveCategoryId,
@@ -342,17 +343,18 @@
             if form.is_valid():
                 killmail_id = form.cleaned_data["killmail_id"]
                 killmail = Killmail.create_from_zkb_api(killmail_id)
                 if killmail:
                     request.session["last_killmail_id"] = killmail_id
                     actions_count = 0
                     for tracker in queryset:
+                        killmail.save()
                         tasks.run_tracker.delay(
                             tracker_pk=tracker.pk,
-                            killmail_json=killmail.asjson(),
+                            killmail_id=killmail_id,
                             ignore_max_age=True,
                         )
                         actions_count += 1
                     self.message_user(
                         request,
                         (
                             f"Started {actions_count} tracker(s) for "
@@ -372,17 +374,19 @@
         else:
             initial = None
         form = TrackerAdminKillmailIdForm(initial=initial)
         return render(
             request,
             "admin/killtracker/tracker/killmail_test.html",
             {
+                "title": "Run Test Killmail for Trackers",
+                "site_header": site_header,
+                "cl": {"opts": Tracker._meta},
                 "form": form,
-                "title": "Load Test Killmail for Tracker",
-                "queryset": queryset.all(),
+                "queryset": queryset.order_by("name"),
             },
         )
 
     def formfield_for_manytomany(self, db_field, request, **kwargs):
         """overriding this formfield to have sorted lists in the form"""
         show_npc_types = request.session.get(
             SESSION_KEY_USES_NPC, False
```

### Comparing `aa-killtracker-0.9.1/killtracker/app_settings.py` & `aa-killtracker-0.9.2/killtracker/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/core/discord_messages.py` & `aa-killtracker-0.9.2/killtracker/core/discord_messages.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/core/killmails.py` & `aa-killtracker-0.9.2/killtracker/core/killmails.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,14 +199,21 @@
         """Save this killmail to temporary storage."""
         cache.set(
             key=self._storage_key(self.id),
             value=self.asjson(),
             timeout=KILLTRACKER_STORAGE_KILLMAILS_LIFETIME,
         )
 
+    def delete(self) -> bool:
+        """Delete this killmail from temporary storage.
+
+        Returns True on success, else False.
+        """
+        return cache.delete(self._storage_key(self.id))
+
     @classmethod
     def get(cls, id: int) -> "Killmail":
         """Fetch a killmail from temporary storage."""
         data = cache.get(key=cls._storage_key(id))
         if not data:
             raise KillmailDoesNotExist(
                 f"Killmail with ID {id} does not exist in storage."
```

### Comparing `aa-killtracker-0.9.1/killtracker/exceptions.py` & `aa-killtracker-0.9.2/killtracker/exceptions.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/forms.py` & `aa-killtracker-0.9.2/killtracker/forms.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/management/commands/killtracker_load_eve.py` & `aa-killtracker-0.9.2/killtracker/management/commands/killtracker_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/managers.py` & `aa-killtracker-0.9.2/killtracker/managers.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/migrations/0001_initial_new.py` & `aa-killtracker-0.9.2/killtracker/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/migrations/0001_squashed_all.py` & `aa-killtracker-0.9.2/killtracker/migrations/0001_squashed_all.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/migrations/0003_add_state_clauses.py` & `aa-killtracker-0.9.2/killtracker/migrations/0003_add_state_clauses.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/migrations/0004_django4_update.py` & `aa-killtracker-0.9.2/killtracker/migrations/0004_django4_update.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/migrations/0005_add_final_blow_clause_and_more.py` & `aa-killtracker-0.9.2/killtracker/migrations/0005_add_final_blow_clause_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/migrations/0006_evetypeplus.py` & `aa-killtracker-0.9.2/killtracker/migrations/0006_evetypeplus.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/migrations/0007_restructure_killsmails.py` & `aa-killtracker-0.9.2/killtracker/migrations/0007_restructure_killsmails.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/migrations/0008_copy_data_to_new_structure.py` & `aa-killtracker-0.9.2/killtracker/migrations/0008_copy_data_to_new_structure.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/migrations/0009_remove_old_models.py` & `aa-killtracker-0.9.2/killtracker/migrations/0009_remove_old_models.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/models.py` & `aa-killtracker-0.9.2/killtracker/models.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/static/killtracker/killtracker_logo.png` & `aa-killtracker-0.9.2/killtracker/static/killtracker/killtracker_logo.png`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/swagger.json` & `aa-killtracker-0.9.2/killtracker/swagger.json`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tasks.py` & `aa-killtracker-0.9.2/killtracker/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     )
     logger.info("%s: Started running tracker", tracker)
     killmail = Killmail.get(killmail_id)
     killmail_new = tracker.process_killmail(
         killmail=killmail, ignore_max_age=ignore_max_age
     )
     if killmail_new:
+        killmail_new.save()
         generate_killmail_message.delay(tracker_pk=tracker_pk, killmail_id=killmail_id)
     elif tracker.webhook.main_queue.size():
         send_messages_to_webhook.delay(webhook_pk=tracker.webhook.pk)
 
 
 @shared_task(bind=True, max_retries=None)
 def generate_killmail_message(self, tracker_pk: int, killmail_id: int) -> None:
```

### Comparing `aa-killtracker-0.9.1/killtracker/templates/admin/killtracker/tracker/change_form.html` & `aa-killtracker-0.9.2/killtracker/templates/admin/killtracker/tracker/change_form.html`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/templates/admin/killtracker/tracker/toogle_npc_button.html` & `aa-killtracker-0.9.2/killtracker/templates/admin/killtracker/tracker/toogle_npc_button.html`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tests/core/test_discord_messages.py` & `aa-killtracker-0.9.2/killtracker/tests/core/test_discord_messages.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tests/core/test_killmails.py` & `aa-killtracker-0.9.2/killtracker/tests/core/test_killmails.py`

 * *Files 5% similar despite different names*

```diff
@@ -308,7 +308,38 @@
         # then
         self.assertEqual(killmail_1, killmail_2)
 
     def test_should_raise_error_when_killmail_does_not_exist(self):
         # when/then
         with self.assertRaises(KillmailDoesNotExist):
             Killmail.get(id=99)
+
+    def test_should_delete_killmail(self):
+        # given
+        killmail = KillmailFactory()
+        killmail.save()
+        # when
+        result = killmail.delete()
+        # then
+        self.assertTrue(result)
+        with self.assertRaises(KillmailDoesNotExist):
+            Killmail.get(id=killmail.id)
+
+    def test_should_return_false_when_delete_killmails_fails(self):
+        # given
+        killmail = KillmailFactory()
+        # when
+        result = killmail.delete()
+        # then
+        self.assertFalse(result)
+
+    def test_should_override_existing_killmail(self):
+        # given
+        killmail_1 = KillmailFactory(zkb__points=1)
+        killmail_1.save()
+        killmail_1.zkb.points = 2
+        # when
+        killmail_1.save()
+        # then
+        killmail_2 = Killmail.get(id=killmail_1.id)
+        self.assertEqual(killmail_1.id, killmail_2.id)
+        self.assertEqual(killmail_2.zkb.points, 2)
```

### Comparing `aa-killtracker-0.9.1/killtracker/tests/test_admin.py` & `aa-killtracker-0.9.2/killtracker/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tests/test_admin_2.py` & `aa-killtracker-0.9.2/killtracker/tests/test_admin_2.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tests/test_integration.py` & `aa-killtracker-0.9.2/killtracker/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tests/test_models_1.py` & `aa-killtracker-0.9.2/killtracker/tests/test_models_1.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tests/test_models_2.py` & `aa-killtracker-0.9.2/killtracker/tests/test_models_2.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tests/test_models_discord_service.py` & `aa-killtracker-0.9.2/killtracker/tests/test_models_discord_service.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tests/test_tasks.py` & `aa-killtracker-0.9.2/killtracker/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tests/testdata/create_eveuniverse.py` & `aa-killtracker-0.9.2/killtracker/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tests/testdata/evecorporations.json` & `aa-killtracker-0.9.2/killtracker/tests/testdata/evecorporations.json`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tests/testdata/eveentities.json` & `aa-killtracker-0.9.2/killtracker/tests/testdata/eveentities.json`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tests/testdata/eveuniverse.json` & `aa-killtracker-0.9.2/killtracker/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tests/testdata/factories.py` & `aa-killtracker-0.9.2/killtracker/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tests/testdata/helpers.py` & `aa-killtracker-0.9.2/killtracker/tests/testdata/helpers.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tests/testdata/killmails.json` & `aa-killtracker-0.9.2/killtracker/tests/testdata/killmails.json`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tools/drop_tables_killtracker.sql` & `aa-killtracker-0.9.2/killtracker/tools/drop_tables_killtracker.sql`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/tools/generate_conditions_text.py` & `aa-killtracker-0.9.2/killtracker/tools/generate_conditions_text.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/killtracker/views.py` & `aa-killtracker-0.9.2/killtracker/views.py`

 * *Files identical despite different names*

### Comparing `aa-killtracker-0.9.1/setup.py` & `aa-killtracker-0.9.2/setup.py`

 * *Files identical despite different names*

