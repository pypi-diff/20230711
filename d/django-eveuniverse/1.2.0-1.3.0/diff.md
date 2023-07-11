# Comparing `tmp/django_eveuniverse-1.2.0.tar.gz` & `tmp/django_eveuniverse-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_eveuniverse-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_eveuniverse-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_eveuniverse-1.2.0.tar` & `django_eveuniverse-1.3.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1070 2020-10-23 18:01:44.555775 django_eveuniverse-1.2.0/LICENSE
--rw-r--r--   0        0        0     3082 2023-06-04 09:47:59.298497 django_eveuniverse-1.2.0/README.rst
--rw-r--r--   0        0        0      184 2023-06-15 19:16:53.976714 django_eveuniverse-1.2.0/eveuniverse/__init__.py
--rw-r--r--   0        0        0     1314 2020-10-23 18:01:44.567774 django_eveuniverse-1.2.0/eveuniverse/admin.py
--rw-r--r--   0        0        0     2857 2023-06-03 17:10:19.215764 django_eveuniverse-1.2.0/eveuniverse/app_settings.py
--rw-r--r--   0        0        0      254 2022-03-01 16:54:35.914600 django_eveuniverse-1.2.0/eveuniverse/apps.py
--rw-r--r--   0        0        0      873 2023-05-29 21:04:02.196043 django_eveuniverse-1.2.0/eveuniverse/backends.py
--rw-r--r--   0        0        0      370 2023-04-15 10:37:18.591750 django_eveuniverse-1.2.0/eveuniverse/constants.py
--rw-r--r--   0        0        0        0 2023-06-15 19:40:51.394095 django_eveuniverse-1.2.0/eveuniverse/core/__init__.py
--rw-r--r--   0        0        0     1781 2022-02-11 14:09:07.543015 django_eveuniverse-1.2.0/eveuniverse/core/dotlan.py
--rw-r--r--   0        0        0      423 2022-06-18 12:37:45.694321 django_eveuniverse-1.2.0/eveuniverse/core/esitools.py
--rw-r--r--   0        0        0     5127 2023-05-29 21:04:02.196043 django_eveuniverse-1.2.0/eveuniverse/core/eveimageserver.py
--rw-r--r--   0        0        0      358 2022-01-04 21:23:14.332955 django_eveuniverse-1.2.0/eveuniverse/core/eveitems.py
--rw-r--r--   0        0        0     2598 2023-05-29 21:04:02.196043 django_eveuniverse-1.2.0/eveuniverse/core/evemicros.py
--rw-r--r--   0        0        0     2431 2023-05-29 21:04:02.196043 django_eveuniverse-1.2.0/eveuniverse/core/evesdeapi.py
--rw-r--r--   0        0        0      457 2022-01-04 21:23:14.332955 django_eveuniverse-1.2.0/eveuniverse/core/eveskinserver.py
--rw-r--r--   0        0        0     1145 2023-05-29 21:04:02.196043 django_eveuniverse-1.2.0/eveuniverse/core/evewho.py
--rw-r--r--   0        0        0     2864 2022-02-11 14:41:18.613728 django_eveuniverse-1.2.0/eveuniverse/core/evexml.py
--rw-r--r--   0        0        0     1713 2023-05-29 21:04:02.196043 django_eveuniverse-1.2.0/eveuniverse/core/zkillboard.py
--rw-r--r--   0        0        0     1745 2023-05-30 19:50:16.531702 django_eveuniverse-1.2.0/eveuniverse/helpers.py
--rw-r--r--   0        0        0      365 2023-04-15 10:37:18.591750 django_eveuniverse-1.2.0/eveuniverse/management/commands/__init__.py
--rw-r--r--   0        0        0     4574 2023-04-15 10:37:18.591750 django_eveuniverse-1.2.0/eveuniverse/management/commands/eveuniverse_load_data.py
--rw-r--r--   0        0        0     5348 2023-04-15 10:37:18.591750 django_eveuniverse-1.2.0/eveuniverse/management/commands/eveuniverse_load_types.py
--rw-r--r--   0        0        0     1644 2021-04-16 13:44:19.227872 django_eveuniverse-1.2.0/eveuniverse/management/commands/eveuniverse_purge_data.py
--rw-r--r--   0        0        0    47900 2023-06-03 17:10:19.215764 django_eveuniverse-1.2.0/eveuniverse/managers.py
--rw-r--r--   0        0        0    51659 2023-04-15 17:15:38.755939 django_eveuniverse-1.2.0/eveuniverse/migrations/0001_initial.py
--rw-r--r--   0        0        0      968 2023-04-15 17:15:38.755939 django_eveuniverse-1.2.0/eveuniverse/migrations/0002_load_eveunit.py
--rw-r--r--   0        0        0     1009 2023-04-15 17:15:38.755939 django_eveuniverse-1.2.0/eveuniverse/migrations/0003_evemarketprice.py
--rw-r--r--   0        0        0      478 2023-04-15 17:15:38.755939 django_eveuniverse-1.2.0/eveuniverse/migrations/0004_effect_longer_name.py
--rw-r--r--   0        0        0     2702 2023-04-15 17:15:38.755939 django_eveuniverse-1.2.0/eveuniverse/migrations/0005_type_materials_and_sections.py
--rw-r--r--   0        0        0      429 2023-04-15 17:15:38.759939 django_eveuniverse-1.2.0/eveuniverse/migrations/0006_alter_evedogmaeffectmodifier_operator.py
--rw-r--r--   0        0        0      409 2023-04-15 17:15:38.759939 django_eveuniverse-1.2.0/eveuniverse/migrations/0007_evetype_description.py
--rw-r--r--   0        0        0     7547 2023-06-03 17:10:19.215764 django_eveuniverse-1.2.0/eveuniverse/migrations/0008_eveindustryactivity_alter_evetype_enabled_sections_and_more.py
--rw-r--r--   0        0        0      989 2023-06-03 17:10:19.215764 django_eveuniverse-1.2.0/eveuniverse/migrations/0009_load_industry_activities.py
--rw-r--r--   0        0        0     1768 2023-06-03 17:10:19.215764 django_eveuniverse-1.2.0/eveuniverse/migrations/0010_alter_eveindustryactivityduration_eve_type_and_more.py
--rw-r--r--   0        0        0        0 2023-06-15 19:40:51.398095 django_eveuniverse-1.2.0/eveuniverse/migrations/__init__.py
--rw-r--r--   0        0        0     5336 2020-11-20 16:10:16.158594 django_eveuniverse-1.2.0/eveuniverse/migrations/eve_unit.json
--rw-r--r--   0        0        0      934 2023-06-03 17:10:19.215764 django_eveuniverse-1.2.0/eveuniverse/migrations/industry_activities.json
--rw-r--r--   0        0        0    64475 2023-06-15 19:16:53.976714 django_eveuniverse-1.2.0/eveuniverse/models.py
--rw-r--r--   0        0        0      250 2022-06-18 12:37:45.694321 django_eveuniverse-1.2.0/eveuniverse/providers.py
--rw-r--r--   0        0        0    14542 2020-12-18 18:17:56.637925 django_eveuniverse-1.2.0/eveuniverse/static/eveuniverse/skin_generic_128.png
--rw-r--r--   0        0        0     2142 2020-12-18 18:17:56.637925 django_eveuniverse-1.2.0/eveuniverse/static/eveuniverse/skin_generic_32.png
--rw-r--r--   0        0        0     4141 2020-12-18 18:17:56.637925 django_eveuniverse-1.2.0/eveuniverse/static/eveuniverse/skin_generic_64.png
--rw-r--r--   0        0        0   887006 2022-06-18 12:37:45.702321 django_eveuniverse-1.2.0/eveuniverse/swagger.json
--rw-r--r--   0        0        0    10805 2023-05-30 19:50:16.535702 django_eveuniverse-1.2.0/eveuniverse/tasks.py
--rw-r--r--   0        0        0        0 2023-06-15 19:40:51.398095 django_eveuniverse-1.2.0/eveuniverse/tests/__init__.py
--rw-r--r--   0        0        0     1274 2023-04-15 17:15:38.759939 django_eveuniverse-1.2.0/eveuniverse/tests/pilot.py
--rw-r--r--   0        0        0     1046 2023-04-13 02:39:52.214185 django_eveuniverse-1.2.0/eveuniverse/tests/test_backends.py
--rw-r--r--   0        0        0    10286 2023-04-13 19:30:17.215558 django_eveuniverse-1.2.0/eveuniverse/tests/test_commands.py
--rw-r--r--   0        0        0    22736 2023-05-29 21:04:02.204043 django_eveuniverse-1.2.0/eveuniverse/tests/test_core.py
--rw-r--r--   0        0        0     2136 2023-05-29 21:04:02.204043 django_eveuniverse-1.2.0/eveuniverse/tests/test_helpers.py
--rw-r--r--   0        0        0    46753 2023-06-15 19:16:53.980714 django_eveuniverse-1.2.0/eveuniverse/tests/test_models_1.py
--rw-r--r--   0        0        0    28631 2023-04-15 12:19:39.042614 django_eveuniverse-1.2.0/eveuniverse/tests/test_models_2.py
--rw-r--r--   0        0        0    56203 2023-06-03 17:10:19.219764 django_eveuniverse-1.2.0/eveuniverse/tests/test_models_3.py
--rw-r--r--   0        0        0    30849 2023-04-15 12:19:39.042614 django_eveuniverse-1.2.0/eveuniverse/tests/test_models_4.py
--rw-r--r--   0        0        0     6759 2023-04-12 21:38:05.746923 django_eveuniverse-1.2.0/eveuniverse/tests/test_tasks.py
--rw-r--r--   0        0        0     2958 2021-04-16 13:44:19.231871 django_eveuniverse-1.2.0/eveuniverse/tests/test_tools_testdata.py
--rw-r--r--   0        0        0     3975 2023-04-15 17:15:38.759939 django_eveuniverse-1.2.0/eveuniverse/tests/test_utils.py
--rw-r--r--   0        0        0        0 2023-06-15 19:40:51.402095 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/__init__.py
--rw-r--r--   0        0        0     7725 2022-03-08 21:55:48.715606 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/esi.py
--rw-r--r--   0        0        0    81711 2023-06-03 17:10:19.219764 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/esi_data.json
--rw-r--r--   0        0        0     4500 2023-01-18 17:00:28.727344 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/factories.py
--rw-r--r--   0        0        0     1659 2023-06-03 17:10:19.219764 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/fetch_esi_raw_data.py
--rw-r--r--   0        0        0     1183 2023-04-05 13:26:14.320189 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/generate_sde.py
--rw-r--r--   0        0        0      610 2023-06-03 17:10:19.219764 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/sde.py
--rw-r--r--   0        0        0     5187 2023-06-03 17:10:19.219764 django_eveuniverse-1.2.0/eveuniverse/tests/testdata/sde_data.json
--rw-r--r--   0        0        0     4636 2020-11-20 16:10:16.170594 django_eveuniverse-1.2.0/eveuniverse/tests/testdata_example.json
--rw-r--r--   0        0        0        0 2023-06-15 19:40:51.402095 django_eveuniverse-1.2.0/eveuniverse/tests/tools/__init__.py
--rw-r--r--   0        0        0      760 2023-04-15 12:19:39.046614 django_eveuniverse-1.2.0/eveuniverse/tests/tools/clear_celery_once_locks.py
--rw-r--r--   0        0        0        0 2023-06-15 19:40:51.402095 django_eveuniverse-1.2.0/eveuniverse/tools/__init__.py
--rw-r--r--   0        0        0     1373 2020-11-20 16:10:16.170594 django_eveuniverse-1.2.0/eveuniverse/tools/drop_tables.sql
--rw-r--r--   0        0        0     5235 2023-04-12 22:26:32.188851 django_eveuniverse-1.2.0/eveuniverse/tools/testdata.py
--rw-r--r--   0        0        0     2817 2023-05-29 21:04:02.204043 django_eveuniverse-1.2.0/eveuniverse/utils.py
--rw-r--r--   0        0        0     1733 2023-06-04 09:47:59.302497 django_eveuniverse-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4432 1970-01-01 00:00:00.000000 django_eveuniverse-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-02 13:03:38.571581 django_eveuniverse-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3082 2023-07-02 13:03:38.571581 django_eveuniverse-1.3.0/README.rst
+-rw-r--r--   0        0        0      184 2023-07-11 20:13:24.749730 django_eveuniverse-1.3.0/eveuniverse/__init__.py
+-rw-r--r--   0        0        0     1314 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/admin.py
+-rw-r--r--   0        0        0     2857 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/app_settings.py
+-rw-r--r--   0        0        0      254 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/apps.py
+-rw-r--r--   0        0        0      873 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/backends.py
+-rw-r--r--   0        0        0      423 2023-07-11 20:13:24.749730 django_eveuniverse-1.3.0/eveuniverse/constants.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:24:19.171556 django_eveuniverse-1.3.0/eveuniverse/core/__init__.py
+-rw-r--r--   0        0        0     1781 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/dotlan.py
+-rw-r--r--   0        0        0      423 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/esitools.py
+-rw-r--r--   0        0        0     5127 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/eveimageserver.py
+-rw-r--r--   0        0        0      358 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/eveitems.py
+-rw-r--r--   0        0        0     2598 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/evemicros.py
+-rw-r--r--   0        0        0     2431 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/evesdeapi.py
+-rw-r--r--   0        0        0      457 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/eveskinserver.py
+-rw-r--r--   0        0        0     1145 2023-07-02 13:03:38.583581 django_eveuniverse-1.3.0/eveuniverse/core/evewho.py
+-rw-r--r--   0        0        0     2864 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/core/evexml.py
+-rw-r--r--   0        0        0     1713 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/core/zkillboard.py
+-rw-r--r--   0        0        0     1745 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/helpers.py
+-rw-r--r--   0        0        0      365 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/management/commands/__init__.py
+-rw-r--r--   0        0        0     4574 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/management/commands/eveuniverse_load_data.py
+-rw-r--r--   0        0        0     5348 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/management/commands/eveuniverse_load_types.py
+-rw-r--r--   0        0        0     1644 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/management/commands/eveuniverse_purge_data.py
+-rw-r--r--   0        0        0    47900 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/managers.py
+-rw-r--r--   0        0        0    51659 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0001_initial.py
+-rw-r--r--   0        0        0      968 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0002_load_eveunit.py
+-rw-r--r--   0        0        0     1009 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0003_evemarketprice.py
+-rw-r--r--   0        0        0      478 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0004_effect_longer_name.py
+-rw-r--r--   0        0        0     2702 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0005_type_materials_and_sections.py
+-rw-r--r--   0        0        0      429 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0006_alter_evedogmaeffectmodifier_operator.py
+-rw-r--r--   0        0        0      409 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0007_evetype_description.py
+-rw-r--r--   0        0        0     7547 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0008_eveindustryactivity_alter_evetype_enabled_sections_and_more.py
+-rw-r--r--   0        0        0      989 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0009_load_industry_activities.py
+-rw-r--r--   0        0        0     1768 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/0010_alter_eveindustryactivityduration_eve_type_and_more.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:24:19.175556 django_eveuniverse-1.3.0/eveuniverse/migrations/__init__.py
+-rw-r--r--   0        0        0     5336 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/eve_unit.json
+-rw-r--r--   0        0        0      934 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/migrations/industry_activities.json
+-rw-r--r--   0        0        0    65441 2023-07-11 20:13:24.749730 django_eveuniverse-1.3.0/eveuniverse/models.py
+-rw-r--r--   0        0        0      250 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/providers.py
+-rw-r--r--   0        0        0    14542 2023-07-02 13:03:38.587581 django_eveuniverse-1.3.0/eveuniverse/static/eveuniverse/skin_generic_128.png
+-rw-r--r--   0        0        0     2142 2023-07-02 13:03:38.591581 django_eveuniverse-1.3.0/eveuniverse/static/eveuniverse/skin_generic_32.png
+-rw-r--r--   0        0        0     4141 2023-07-02 13:03:38.591581 django_eveuniverse-1.3.0/eveuniverse/static/eveuniverse/skin_generic_64.png
+-rw-r--r--   0        0        0   887006 2023-07-02 13:03:38.591581 django_eveuniverse-1.3.0/eveuniverse/swagger.json
+-rw-r--r--   0        0        0    10805 2023-07-02 13:03:38.591581 django_eveuniverse-1.3.0/eveuniverse/tasks.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:24:19.175556 django_eveuniverse-1.3.0/eveuniverse/tests/__init__.py
+-rw-r--r--   0        0        0     1274 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/pilot.py
+-rw-r--r--   0        0        0     1046 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/test_backends.py
+-rw-r--r--   0        0        0    10307 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/test_commands.py
+-rw-r--r--   0        0        0    22736 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/test_core.py
+-rw-r--r--   0        0        0     2136 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/test_helpers.py
+-rw-r--r--   0        0        0    52520 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/test_models_1.py
+-rw-r--r--   0        0        0    28662 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/test_models_2.py
+-rw-r--r--   0        0        0    56264 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/test_models_3.py
+-rw-r--r--   0        0        0    30870 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/test_models_4.py
+-rw-r--r--   0        0        0     6759 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/test_tasks.py
+-rw-r--r--   0        0        0     3009 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/test_tools_testdata.py
+-rw-r--r--   0        0        0     4006 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:24:19.175556 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     7725 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/esi.py
+-rw-r--r--   0        0        0    83831 2023-07-11 20:13:24.753730 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/esi_data.json
+-rw-r--r--   0        0        0     4500 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/factories.py
+-rw-r--r--   0        0        0     1659 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/fetch_esi_raw_data.py
+-rw-r--r--   0        0        0     1183 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/generate_sde.py
+-rw-r--r--   0        0        0      610 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/sde.py
+-rw-r--r--   0        0        0     5187 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/testdata/sde_data.json
+-rw-r--r--   0        0        0     4636 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/testdata_example.json
+-rw-r--r--   0        0        0        0 2023-07-11 20:24:19.175556 django_eveuniverse-1.3.0/eveuniverse/tests/tools/__init__.py
+-rw-r--r--   0        0        0      760 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tests/tools/clear_celery_once_locks.py
+-rw-r--r--   0        0        0        0 2023-07-11 20:24:19.175556 django_eveuniverse-1.3.0/eveuniverse/tools/__init__.py
+-rw-r--r--   0        0        0     1373 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tools/drop_tables.sql
+-rw-r--r--   0        0        0     5235 2023-07-02 13:03:38.595582 django_eveuniverse-1.3.0/eveuniverse/tools/testdata.py
+-rw-r--r--   0        0        0     2821 2023-07-08 11:35:53.902984 django_eveuniverse-1.3.0/eveuniverse/utils.py
+-rw-r--r--   0        0        0     1733 2023-07-02 13:03:38.599582 django_eveuniverse-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4432 1970-01-01 00:00:00.000000 django_eveuniverse-1.3.0/PKG-INFO
```

### Comparing `django_eveuniverse-1.2.0/LICENSE` & `django_eveuniverse-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/README.rst` & `django_eveuniverse-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/admin.py` & `django_eveuniverse-1.3.0/eveuniverse/admin.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/app_settings.py` & `django_eveuniverse-1.3.0/eveuniverse/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/backends.py` & `django_eveuniverse-1.3.0/eveuniverse/backends.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/core/dotlan.py` & `django_eveuniverse-1.3.0/eveuniverse/core/dotlan.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/core/eveimageserver.py` & `django_eveuniverse-1.3.0/eveuniverse/core/eveimageserver.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/core/evemicros.py` & `django_eveuniverse-1.3.0/eveuniverse/core/evemicros.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/core/evesdeapi.py` & `django_eveuniverse-1.3.0/eveuniverse/core/evesdeapi.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/core/evewho.py` & `django_eveuniverse-1.3.0/eveuniverse/core/evewho.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/core/evexml.py` & `django_eveuniverse-1.3.0/eveuniverse/core/evexml.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/core/zkillboard.py` & `django_eveuniverse-1.3.0/eveuniverse/core/zkillboard.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/helpers.py` & `django_eveuniverse-1.3.0/eveuniverse/helpers.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/management/commands/eveuniverse_load_data.py` & `django_eveuniverse-1.3.0/eveuniverse/management/commands/eveuniverse_load_data.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/management/commands/eveuniverse_load_types.py` & `django_eveuniverse-1.3.0/eveuniverse/management/commands/eveuniverse_load_types.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/management/commands/eveuniverse_purge_data.py` & `django_eveuniverse-1.3.0/eveuniverse/management/commands/eveuniverse_purge_data.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/managers.py` & `django_eveuniverse-1.3.0/eveuniverse/managers.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/migrations/0001_initial.py` & `django_eveuniverse-1.3.0/eveuniverse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/migrations/0002_load_eveunit.py` & `django_eveuniverse-1.3.0/eveuniverse/migrations/0002_load_eveunit.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/migrations/0003_evemarketprice.py` & `django_eveuniverse-1.3.0/eveuniverse/migrations/0003_evemarketprice.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/migrations/0005_type_materials_and_sections.py` & `django_eveuniverse-1.3.0/eveuniverse/migrations/0005_type_materials_and_sections.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/migrations/0008_eveindustryactivity_alter_evetype_enabled_sections_and_more.py` & `django_eveuniverse-1.3.0/eveuniverse/migrations/0008_eveindustryactivity_alter_evetype_enabled_sections_and_more.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/migrations/0009_load_industry_activities.py` & `django_eveuniverse-1.3.0/eveuniverse/migrations/0009_load_industry_activities.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/migrations/0010_alter_eveindustryactivityduration_eve_type_and_more.py` & `django_eveuniverse-1.3.0/eveuniverse/migrations/0010_alter_eveindustryactivityduration_eve_type_and_more.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/migrations/eve_unit.json` & `django_eveuniverse-1.3.0/eveuniverse/migrations/eve_unit.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/migrations/industry_activities.json` & `django_eveuniverse-1.3.0/eveuniverse/migrations/industry_activities.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/models.py` & `django_eveuniverse-1.3.0/eveuniverse/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import math
 import re
 import sys
 from collections import namedtuple
 from typing import Any, Dict, Iterable, List, Optional, Set, Tuple
 
 from bitfield import BitField
-from bravado.exception import HTTPNotFound
 from django.contrib.staticfiles.storage import staticfiles_storage
 from django.db import models
+from django.utils.functional import cached_property
 
 from .app_settings import (
     EVEUNIVERSE_LOAD_ASTEROID_BELTS,
     EVEUNIVERSE_LOAD_DOGMAS,
     EVEUNIVERSE_LOAD_GRAPHICS,
     EVEUNIVERSE_LOAD_INDUSTRY_ACTIVITIES,
     EVEUNIVERSE_LOAD_MARKET_GROUPS,
@@ -23,15 +23,15 @@
     EVEUNIVERSE_LOAD_PLANETS,
     EVEUNIVERSE_LOAD_STARGATES,
     EVEUNIVERSE_LOAD_STARS,
     EVEUNIVERSE_LOAD_STATIONS,
     EVEUNIVERSE_LOAD_TYPE_MATERIALS,
     EVEUNIVERSE_USE_EVESKINSERVER,
 )
-from .constants import EveCategoryId, EveGroupId
+from .constants import EveCategoryId, EveGroupId, EveRegionId
 from .core import dotlan, eveimageserver, eveitems, evesdeapi, eveskinserver, evewho
 from .managers import (
     EveAsteroidBeltManager,
     EveEntityManager,
     EveIndustryActivityDurationManager,
     EveIndustryActivityMaterialManager,
     EveIndustryActivityProductManager,
@@ -1216,21 +1216,31 @@
     def is_low_sec(self) -> bool:
         """returns True if this solar system is in low sec, else False"""
         return 0 < round(self.security_status, 1) < 0.5
 
     @property
     def is_null_sec(self) -> bool:
         """returns True if this solar system is in null sec, else False"""
-        return round(self.security_status, 1) <= 0 and not self.is_w_space
+        return (
+            not self.is_w_space
+            and not self.is_trig_space
+            and round(self.security_status, 1) <= 0
+            and not self.is_w_space
+        )
 
     @property
     def is_w_space(self) -> bool:
         """returns True if this solar system is in wormhole space, else False"""
         return 31000000 <= self.id < 32000000
 
+    @cached_property
+    def is_trig_space(self) -> bool:
+        """returns True if this solar system is in Triglavian space, else False"""
+        return self.eve_constellation.eve_region_id == EveRegionId.POCHVEN
+
     @classmethod
     def eve_entity_category(cls) -> str:
         return EveEntity.CATEGORY_SOLAR_SYSTEM
 
     def distance_to(self, destination: "EveSolarSystem") -> Optional[float]:
         """Calculates the distance in meters between the current and the given solar system
 
@@ -1245,16 +1255,23 @@
         if (
             not destination
             or not destination.position_x
             or not destination.position_y
             or not destination.position_z
         ):
             return None
-        if self.is_w_space or destination.is_w_space:
+
+        if (
+            self.is_w_space
+            or destination.is_w_space
+            or self.is_trig_space
+            or destination.is_trig_space
+        ):
             return None
+
         return math.sqrt(
             (destination.position_x - self.position_x) ** 2
             + (destination.position_y - self.position_y) ** 2
             + (destination.position_z - self.position_z) ** 2
         )
 
     def route_to(
@@ -1262,33 +1279,52 @@
     ) -> Optional[List["EveSolarSystem"]]:
         """Calculates the shortest route between the current and the given solar system
 
         Args:
             destination: Other solar system to use in calculation
 
         Returns:
-            List of solar system objects incl. origin and destination or None if no route can be found (e.g. if one system is in WH space)
+            List of solar system objects incl. origin and destination
+            or None if no route can be found (e.g. if one system is in WH space)
         """
+        if (
+            self.is_w_space
+            or destination.is_w_space
+            or self.is_trig_space
+            or destination.is_trig_space
+        ):
+            return None
+
         path_ids = self._calc_route_esi(self.id, destination.id)
         if path_ids is None:
             return None
+
         return [
             EveSolarSystem.objects.get_or_create_esi(id=solar_system_id)
             for solar_system_id in path_ids
         ]
 
     def jumps_to(self, destination: "EveSolarSystem") -> Optional[int]:
         """Calculates the shortest route between the current and the given solar system
 
         Args:
             destination: Other solar system to use in calculation
 
         Returns:
-            Number of total jumps or None if no route can be found (e.g. if one system is in WH space)
+            Number of total jumps
+            or None if no route can be found (e.g. if one system is in WH space)
         """
+        if (
+            self.is_w_space
+            or destination.is_w_space
+            or self.is_trig_space
+            or destination.is_trig_space
+        ):
+            return None
+
         path_ids = self._calc_route_esi(self.id, destination.id)
         return len(path_ids) - 1 if path_ids is not None else None
 
     @staticmethod
     def _calc_route_esi(origin_id: int, destination_id: int) -> Optional[List[int]]:
         """returns the shortest route between two given solar systems.
 
@@ -1301,15 +1337,16 @@
             List of solar system IDs incl. origin and destination or None if no route can be found (e.g. if one system is in WH space)
         """
 
         try:
             return esi.client.Routes.get_route_origin_destination(
                 origin=origin_id, destination=destination_id
             ).results()
-        except HTTPNotFound:
+        except OSError:  # FIXME: ESI is supposed to return 404,
+            # but django-esi is actually returning an OSError
             return None
 
     def nearest_celestial(
         self, x: int, y: int, z: int, group_id: Optional[int] = None
     ) -> Optional[NearestCelestial]:
         """Determine nearest celestial to given coordinates as eveuniverse object.
```

### Comparing `django_eveuniverse-1.2.0/eveuniverse/static/eveuniverse/skin_generic_128.png` & `django_eveuniverse-1.3.0/eveuniverse/static/eveuniverse/skin_generic_128.png`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/static/eveuniverse/skin_generic_32.png` & `django_eveuniverse-1.3.0/eveuniverse/static/eveuniverse/skin_generic_32.png`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/static/eveuniverse/skin_generic_64.png` & `django_eveuniverse-1.3.0/eveuniverse/static/eveuniverse/skin_generic_64.png`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/swagger.json` & `django_eveuniverse-1.3.0/eveuniverse/swagger.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tasks.py` & `django_eveuniverse-1.3.0/eveuniverse/tasks.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/pilot.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/pilot.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/test_backends.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/test_commands.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/test_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from io import StringIO
 from unittest.mock import patch
 
 from django.core.management import call_command
 from django.test.utils import override_settings
 
-from ..models import EveCategory, EveGroup, EveType
-from ..utils import NoSocketsTestCase
+from eveuniverse.models import EveCategory, EveGroup, EveType
+from eveuniverse.utils import NoSocketsTestCase
+
 from .testdata.esi import EsiClientStub
 
 MODELS_PATH = "eveuniverse.models"
 PACKAGE_PATH = "eveuniverse.management.commands"
 
 
 @patch(PACKAGE_PATH + ".eveuniverse_load_data.is_esi_online", lambda: True)
```

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/test_core.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/test_helpers.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/test_models_1.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/test_models_1.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import unittest
 from unittest.mock import Mock, patch
 
 from bravado.exception import HTTPNotFound
 from django.test.utils import override_settings
 from django.utils.timezone import now
 
-from ..helpers import meters_to_ly
-from ..models import (
+from eveuniverse.helpers import meters_to_ly
+from eveuniverse.models import (
     EveAncestry,
     EveAsteroidBelt,
     EveBloodline,
     EveCategory,
     EveConstellation,
     EveDogmaAttribute,
     EveDogmaEffect,
@@ -38,15 +38,16 @@
     EveType,
     EveTypeDogmaAttribute,
     EveTypeDogmaEffect,
     EveTypeMaterial,
     EveUnit,
     EveUniverseBaseModel,
 )
-from ..utils import NoSocketsTestCase
+from eveuniverse.utils import NoSocketsTestCase
+
 from .testdata.esi import BravadoOperationStub, EsiClientStub
 
 unittest.util._MAX_LENGTH = 1000
 MODELS_PATH = "eveuniverse.models"
 MANAGERS_PATH = "eveuniverse.managers"
 
 
@@ -913,41 +914,55 @@
         mock_esi.client = EsiClientStub()
 
         jita, _ = EveSolarSystem.objects.get_or_create_esi(id=30000142)
         self.assertTrue(jita.is_high_sec)
         self.assertFalse(jita.is_low_sec)
         self.assertFalse(jita.is_null_sec)
         self.assertFalse(jita.is_w_space)
+        self.assertFalse(jita.is_trig_space)
 
     def test_can_identify_lowsec_system(self, mock_esi):
         mock_esi.client = EsiClientStub()
 
         enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
         self.assertTrue(enaluri.is_low_sec)
         self.assertFalse(enaluri.is_high_sec)
         self.assertFalse(enaluri.is_null_sec)
         self.assertFalse(enaluri.is_w_space)
+        self.assertFalse(enaluri.is_trig_space)
 
     def test_can_identify_nullsec_system(self, mock_esi):
         mock_esi.client = EsiClientStub()
 
         hed_gp, _ = EveSolarSystem.objects.get_or_create_esi(id=30001161)
         self.assertTrue(hed_gp.is_null_sec)
         self.assertFalse(hed_gp.is_low_sec)
         self.assertFalse(hed_gp.is_high_sec)
         self.assertFalse(hed_gp.is_w_space)
+        self.assertFalse(hed_gp.is_trig_space)
 
     def test_can_identify_ws_system(self, mock_esi):
         mock_esi.client = EsiClientStub()
 
         thera, _ = EveSolarSystem.objects.get_or_create_esi(id=31000005)
         self.assertTrue(thera.is_w_space)
         self.assertFalse(thera.is_null_sec)
         self.assertFalse(thera.is_low_sec)
         self.assertFalse(thera.is_high_sec)
+        self.assertFalse(thera.is_trig_space)
+
+    def test_can_identify_trig_system(self, mock_esi):
+        mock_esi.client = EsiClientStub()
+
+        otela, _ = EveSolarSystem.objects.get_or_create_esi(id=30000157)
+        self.assertFalse(otela.is_w_space)
+        self.assertFalse(otela.is_null_sec)
+        self.assertFalse(otela.is_low_sec)
+        self.assertFalse(otela.is_high_sec)
+        self.assertTrue(otela.is_trig_space)
 
     """
     @patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_STARGATES", True)
     @patch(MODELS_PATH + ".cache")
     def test_can_calculate_route(self, mock_cache, mock_esi):
         def my_get_or_set(key, func, timeout):
             return func()
@@ -1029,82 +1044,214 @@
         enaluri.position_z = None
         akidagi, _ = EveSolarSystem.objects.get_or_create_esi(id=30045342)
         # when
         result = akidagi.distance_to(enaluri)
         # then
         self.assertIsNone(result)
 
+    def test_should_return_none_when_one_system_is_in_trig_space_1(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
+        otela, _ = EveSolarSystem.objects.get_or_create_esi(id=30000157)
+        # when
+        result = enaluri.distance_to(otela)
+        # then
+        self.assertIsNone(result)
+
+    def test_should_return_none_when_one_system_is_in_trig_space_2(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
+        otela, _ = EveSolarSystem.objects.get_or_create_esi(id=30000157)
+        # when
+        result = otela.distance_to(enaluri)
+        # then
+        self.assertIsNone(result)
+
 
 @patch(MANAGERS_PATH + ".esi")
+@patch("eveuniverse.models.esi")
 class TestEveSolarSystemJumpsTo(NoSocketsTestCase):
-    @staticmethod
-    def esi_get_route_origin_destination(origin, destination, **kwargs):
-        routes = {
-            30045339: {30045342: [30045339, 30045342]},
-        }
-        if origin in routes and destination in routes[origin]:
-            return BravadoOperationStub(routes[origin][destination])
-        raise HTTPNotFound(Mock(**{"response.status_code": 404}))
-
-    @patch("eveuniverse.models.esi")
-    def test_can_calculate_jumps(self, mock_esi_2, mock_esi):
-        mock_esi.client = EsiClientStub()
-        mock_esi_2.client.Routes.get_route_origin_destination.side_effect = (
-            self.esi_get_route_origin_destination
+    def test_can_calculate_jumps(self, mock_esi_2, mock_esi_1):
+        # given
+        mock_esi_1.client = EsiClientStub()
+        mock_esi_2.client.Routes.get_route_origin_destination.return_value = (
+            BravadoOperationStub([30045339, 30045342])
         )
-
         enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
         akidagi, _ = EveSolarSystem.objects.get_or_create_esi(id=30045342)
+        # when/then
         self.assertEqual(enaluri.jumps_to(akidagi), 1)
 
-    @patch("eveuniverse.models.esi")
     def test_route_calc_returns_none_if_no_route_found(self, mock_esi_2, mock_esi):
+        # given
         mock_esi.client = EsiClientStub()
         mock_esi_2.client.Routes.get_route_origin_destination.side_effect = (
-            self.esi_get_route_origin_destination
+            HTTPNotFound(Mock(**{"response.status_code": 404}))
         )
-
         enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
         jita, _ = EveSolarSystem.objects.get_or_create_esi(id=30000142)
+        # when/then
         self.assertIsNone(enaluri.jumps_to(jita))
 
+    def test_should_return_none_if_any_system_is_in_wh_space_1(
+        self, mock_esi_2, mock_esi_1
+    ):
+        # given
+        mock_esi_1.client = EsiClientStub()
+        mock_esi_2.client.Routes.get_route_origin_destination.return_value = (
+            BravadoOperationStub([30045339, 30045342])
+        )
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
+        thera, _ = EveSolarSystem.objects.get_or_create_esi(id=31000005)
+        # when/then
+        self.assertIsNone(enaluri.jumps_to(thera))
+
+    def test_should_return_none_if_any_system_is_in_wh_space_2(
+        self, mock_esi_2, mock_esi_1
+    ):
+        # given
+        mock_esi_1.client = EsiClientStub()
+        mock_esi_2.client.Routes.get_route_origin_destination.return_value = (
+            BravadoOperationStub([30045339, 30045342])
+        )
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
+        thera, _ = EveSolarSystem.objects.get_or_create_esi(id=31000005)
+        # when/then
+        self.assertIsNone(thera.jumps_to(enaluri))
+
+    def test_should_return_none_if_any_system_is_in_trig_space_1(
+        self, mock_esi_2, mock_esi_1
+    ):
+        # given
+        mock_esi_1.client = EsiClientStub()
+        mock_esi_2.client.Routes.get_route_origin_destination.return_value = (
+            BravadoOperationStub([30045339, 30045342])
+        )
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
+        otela, _ = EveSolarSystem.objects.get_or_create_esi(id=30000157)
+        # when/then
+        self.assertIsNone(enaluri.jumps_to(otela))
+
+    def test_should_return_none_if_any_system_is_in_trig_space_2(
+        self, mock_esi_2, mock_esi_1
+    ):
+        # given
+        mock_esi_1.client = EsiClientStub()
+        mock_esi_2.client.Routes.get_route_origin_destination.return_value = (
+            BravadoOperationStub([30045339, 30045342])
+        )
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
+        otela, _ = EveSolarSystem.objects.get_or_create_esi(id=30000157)
+        # when/then
+        self.assertIsNone(otela.jumps_to(enaluri))
+
 
-@patch(MODELS_PATH + ".EveSolarSystem._calc_route_esi")
+@patch(MODELS_PATH + ".esi")
 @patch(MANAGERS_PATH + ".esi")
 class TestEveSolarSystemRouteTo(NoSocketsTestCase):
-    def test_should_return_valid_route(self, mock_esi, mock_calc_route_esi):
+    def test_should_return_valid_route(self, mock_esi_1, mock_esi_2):
         # given
-        mock_esi.client = EsiClientStub()
-        mock_calc_route_esi.return_value = [30045339, 30045342]
+        mock_esi_1.client = EsiClientStub()
+        mock_esi_2.client.Routes.get_route_origin_destination.return_value = (
+            BravadoOperationStub([30045339, 30045342])
+        )
         enaluri: EveSolarSystem = EveSolarSystem.objects.get_or_create_esi(id=30045339)[
             0
         ]
         akidagi: EveSolarSystem = EveSolarSystem.objects.get_or_create_esi(id=30045342)[
             0
         ]
         # when
         result = enaluri.route_to(akidagi)
         # then
         self.assertListEqual(result, [(enaluri, False), (akidagi, False)])
 
-    def test_should_return_none_when_no_route_found(
-        self, mock_esi, mock_calc_route_esi
+    def test_should_return_none_when_no_route_found(self, mock_esi_1, mock_esi_2):
+        # given
+        mock_esi_1.client = EsiClientStub()
+        mock_esi_2.client.Routes.get_route_origin_destination.side_effect = (
+            HTTPNotFound(Mock(**{"response.status_code": 404}))
+        )
+        enaluri: EveSolarSystem = EveSolarSystem.objects.get_or_create_esi(id=30045339)[
+            0
+        ]
+        akidagi: EveSolarSystem = EveSolarSystem.objects.get_or_create_esi(id=30045342)[
+            0
+        ]
+        # when
+        result = enaluri.route_to(akidagi)
+        # then
+        self.assertIsNone(result)
+
+    def test_should_return_none_if_any_system_is_in_wh_space_1(
+        self, mock_esi_1, mock_esi_2
     ):
         # given
-        mock_esi.client = EsiClientStub()
-        mock_calc_route_esi.return_value = None
+        mock_esi_1.client = EsiClientStub()
+        mock_esi_2.client.Routes.get_route_origin_destination.return_value = (
+            BravadoOperationStub([30045339, 30045342])
+        )
         enaluri: EveSolarSystem = EveSolarSystem.objects.get_or_create_esi(id=30045339)[
             0
         ]
-        thera, _ = EveSolarSystem.objects.get_or_create_esi(id=31000005)
+        thera: EveSolarSystem = EveSolarSystem.objects.get_or_create_esi(id=31000005)[0]
         # when
         result = enaluri.route_to(thera)
         # then
         self.assertIsNone(result)
 
+    def test_should_return_none_if_any_system_is_in_wh_space_2(
+        self, mock_esi_1, mock_esi_2
+    ):
+        # given
+        mock_esi_1.client = EsiClientStub()
+        mock_esi_2.client.Routes.get_route_origin_destination.return_value = (
+            BravadoOperationStub([30045339, 30045342])
+        )
+        enaluri: EveSolarSystem = EveSolarSystem.objects.get_or_create_esi(id=30045339)[
+            0
+        ]
+        thera: EveSolarSystem = EveSolarSystem.objects.get_or_create_esi(id=31000005)[0]
+        # when
+        result = thera.route_to(enaluri)
+        # then
+        self.assertIsNone(result)
+
+    def test_should_return_none_if_any_system_is_in_trig_space_1(
+        self, mock_esi_1, mock_esi_2
+    ):
+        # given
+        mock_esi_1.client = EsiClientStub()
+        mock_esi_2.client.Routes.get_route_origin_destination.return_value = (
+            BravadoOperationStub([30045339, 30045342])
+        )
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
+        otela, _ = EveSolarSystem.objects.get_or_create_esi(id=30000157)
+        # when
+        result = otela.route_to(enaluri)
+        # then
+        self.assertIsNone(result)
+
+    def test_should_return_none_if_any_system_is_in_trig_space_2(
+        self, mock_esi_1, mock_esi_2
+    ):
+        # given
+        mock_esi_1.client = EsiClientStub()
+        mock_esi_2.client.Routes.get_route_origin_destination.return_value = (
+            BravadoOperationStub([30045339, 30045342])
+        )
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
+        otela, _ = EveSolarSystem.objects.get_or_create_esi(id=30000157)
+        # when
+        result = enaluri.route_to(otela)
+        # then
+        self.assertIsNone(result)
+
 
 @patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_DOGMAS", False)
 @patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_MARKET_GROUPS", False)
 @patch(MANAGERS_PATH + ".esi")
 class TestEveStar(NoSocketsTestCase):
     def test_create_from_esi(self, mock_esi):
         mock_esi.client = EsiClientStub()
```

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/test_models_2.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/test_models_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 from unittest.mock import patch
 
 from django.test.utils import override_settings
 
-from ..constants import EveCategoryId
-from ..models import (
+from eveuniverse.constants import EveCategoryId
+from eveuniverse.models import (
     EsiMapping,
     EveAncestry,
     EveBloodline,
     EveCategory,
     EveConstellation,
     EveDogmaAttribute,
     EveDogmaEffect,
@@ -18,15 +18,16 @@
     EveMarketGroup,
     EveRegion,
     EveType,
     EveTypeDogmaEffect,
     EveUnit,
     EveUniverseEntityModel,
 )
-from ..utils import NoSocketsTestCase
+from eveuniverse.utils import NoSocketsTestCase
+
 from .testdata.esi import EsiClientStub
 
 unittest.util._MAX_LENGTH = 1000
 MODELS_PATH = "eveuniverse.models"
 MANAGERS_PATH = "eveuniverse.managers"
```

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/test_models_3.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/test_models_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from unittest.mock import patch
 
 import requests_mock
 
-from ..constants import EveGroupId
-from ..core import evesdeapi
-from ..models import (
+from eveuniverse.constants import EveGroupId
+from eveuniverse.core import evesdeapi
+from eveuniverse.models import (
     EveAsteroidBelt,
     EveIndustryActivityDuration,
     EveIndustryActivityMaterial,
     EveIndustryActivityProduct,
     EveIndustryActivitySkill,
     EveMoon,
     EvePlanet,
     EveSolarSystem,
     EveStar,
     EveStargate,
     EveStation,
     EveType,
     EveTypeMaterial,
 )
-from ..utils import NoSocketsTestCase
+from eveuniverse.utils import NoSocketsTestCase
+
 from .testdata.esi import EsiClientStub
 from .testdata.sde import cache_content, sde_data, type_materials_cache_content
 
 MODELS_PATH = "eveuniverse.models"
 MANAGERS_PATH = "eveuniverse.managers"
 
 
@@ -974,15 +975,15 @@
         # then
         self.assertEqual(
             set(
                 EveSolarSystem.objects.filter(
                     enabled_sections=EveSolarSystem.enabled_sections.planets
                 ).values_list("id", flat=True)
             ),
-            {30000142, 30001161, 30045339, 30045342, 31000005},
+            {30000142, 30001161, 30045339, 30045342, 31000005, 30000157},
         )
         self.assertEqual(
             set(EvePlanet.objects.values_list("id", flat=True)),
             {40009077, 40349467, 40349471},
         )
 
     @patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_PLANETS", False)
@@ -999,15 +1000,15 @@
         # then
         self.assertEqual(
             set(
                 EveSolarSystem.objects.filter(
                     enabled_sections=EveSolarSystem.enabled_sections.planets
                 ).values_list("id", flat=True)
             ),
-            {30000142, 30001161, 30045339, 30045342, 31000005},
+            {30000142, 30001161, 30045339, 30045342, 31000005, 30000157},
         )
         self.assertEqual(
             set(EvePlanet.objects.values_list("id", flat=True)),
             {40009077, 40349467, 40349471},
         )
 
     @patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_PLANETS", True)
```

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/test_models_4.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/test_models_4.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Eve Entity tests."""
 
 from unittest.mock import patch
 
-from ..models import EveEntity
-from ..utils import NoSocketsTestCase
+from eveuniverse.models import EveEntity
+from eveuniverse.utils import NoSocketsTestCase
+
 from .testdata.esi import BravadoOperationStub, EsiClientStub
 from .testdata.factories import create_eve_entity
 
 MANAGERS_PATH = "eveuniverse.managers"
 
 
 @patch(MANAGERS_PATH + ".esi")
```

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/test_tasks.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/test_tools_testdata.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/test_tools_testdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import inspect
 import json
 import os
 from collections import OrderedDict
 from unittest.mock import patch
 
-from ..models import EveCategory, EveGroup, EveRegion, EveType
-from ..tools.testdata import ModelSpec, create_testdata, load_testdata_from_file
-from ..utils import NoSocketsTestCase
+from eveuniverse.models import EveCategory, EveGroup, EveRegion, EveType
+from eveuniverse.tools.testdata import (
+    ModelSpec,
+    create_testdata,
+    load_testdata_from_file,
+)
+from eveuniverse.utils import NoSocketsTestCase
+
 from .testdata.esi import EsiClientStub
 
-_currentdir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
+_current_dir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 
 FILENAME_TESTDATA = "dummy.json"
 
 
 class TestTestData(NoSocketsTestCase):
     def setUp(self) -> None:
         EveCategory.objects.all().delete
@@ -32,15 +37,15 @@
         mock_esi.client = EsiClientStub()
 
         spec = [
             ModelSpec("EveType", ids=[603]),
             ModelSpec("EveType", ids=[621], enabled_sections=[EveType.Section.DOGMAS]),
             ModelSpec("EveSolarSystem", ids=[30045339], include_children=True),
         ]
-        filepath = f"{_currentdir}/{FILENAME_TESTDATA}"
+        filepath = f"{_current_dir}/{FILENAME_TESTDATA}"
         create_testdata(spec, filepath)
 
         with open(filepath, "r", encoding="utf-8") as f:
             testdata = json.load(f, object_pairs_hook=OrderedDict)
 
         # EveType
         # did load requested objects
@@ -62,15 +67,15 @@
 
         # did load children of solar systems as requested
         self.assertEqual(self._get_ids(testdata, "EveStargate"), {50016284, 50016286})
 
         os.remove(filepath)
 
     def test_load_testdata_from_file(self):
-        filepath = f"{_currentdir}/testdata_example.json"
+        filepath = f"{_current_dir}/testdata_example.json"
         load_testdata_from_file(filepath)
         self.assertTrue(EveCategory.objects.filter(id=6).exists())
         self.assertTrue(EveGroup.objects.filter(id=25).exists())
         self.assertTrue(EveGroup.objects.filter(id=26).exists())
         self.assertTrue(EveType.objects.filter(id=603).exists())
         self.assertTrue(EveType.objects.filter(id=621).exists())
         self.assertTrue(EveRegion.objects.filter(id=10000069).exists())
```

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/test_utils.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from unittest.mock import Mock, patch
 
 import requests
 from django.test import TestCase
 
-from ..utils import NoSocketsTestCase, SocketAccessError, chunks, clean_setting
+from eveuniverse.utils import (
+    NoSocketsTestCase,
+    SocketAccessError,
+    chunks,
+    clean_setting,
+)
 
 MODULE_PATH = "eveuniverse.utils"
 
 
 class TestChunks(TestCase):
     def test_chunks(self):
         a0 = [1, 2, 3, 4, 5, 6]
```

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/testdata/esi.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/testdata/esi.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/testdata/esi_data.json` & `django_eveuniverse-1.3.0/eveuniverse/tests/testdata/esi_data.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982291666666667%*

 * *Differences: {"'Universe'": "{'get_universe_constellations_constellation_id': {'20000787': "*

 * *               "OrderedDict([('constellation_id', 20000787), ('name', 'Krai Perun'), ('position', "*

 * *               "OrderedDict([('x', -162832101952226140), ('y', 50656681128061160), ('z', "*

 * *               "103886924951038770)])), ('region_id', 10000070), ('systems', [30000157])])}, "*

 * *               "'get_universe_regions_region_id': {'10000070': OrderedDict([('constellations', "*

 * *               "[20000787]), ('description', '<i> […]*

```diff
@@ -380,14 +380,27 @@
                     "z": 136029596082308480
                 },
                 "region_id": 10000069,
                 "systems": [
                     30045339
                 ]
             },
+            "20000787": {
+                "constellation_id": 20000787,
+                "name": "Krai Perun",
+                "position": {
+                    "x": -162832101952226140,
+                    "y": 50656681128061160,
+                    "z": 103886924951038770
+                },
+                "region_id": 10000070,
+                "systems": [
+                    30000157
+                ]
+            },
             "21000324": {
                 "constellation_id": 21000324,
                 "name": "G-C00324",
                 "position": {
                     "x": 7205800000000000000,
                     "y": 1539300000000000000,
                     "z": -9515100000000000000
@@ -767,14 +780,22 @@
                 "constellations": [
                     20000785
                 ],
                 "description": "For centuries, this volume of space remained inexplicably impenetrable to investigation. It possesses no apparent mass or dimension, but the abrupt disappearance of every expedition into the zone made it an effective bulwark against flanking attacks during the first Gallente-Caldari war, and the subsequent uneasy peace.<br><br>Several decades ago, a coalition of like-minded Caldari megacorps discovered ways to traverse Black Rise safely, and began a secret programme of colonization. The start of the Empyrean War forced them to show their hand, and the region soon became a key front in the conflict between Caldari and Gallente forces.<br><br>Today the region remains somewhat underdeveloped, but rich in raw materials. The poorly-understood phenomena that still manifest can make life awkward, but fluid router networks and jump travel permit unrestricted travel and communications. Of the many early expeditions, though, no trace has yet been found.",
                 "name": "Black Rise",
                 "region_id": 10000069
             },
+            "10000070": {
+                "constellations": [
+                    20000787
+                ],
+                "description": "<i>We are Zorya Triglav\r\n\r\nWe speak for the Convocation of Triglav Outside the Struggle\r\n\r\nHear the words of our prayer and heed them\r\n\r\nRealization of glorification pattern in totality approaches\r\n\r\nAncient Domains stability requires weaving of Final Liminality conduits\r\n\r\nTotality requires Triglav Exalted Final Liminality Dazh Elements\r\n\r\nSobornost Kybernauts are exhorted to realize glorification pattern in totality\r\n\r\nThe Flow of Vyraj requires realization of stability of Ancient Domains\r\n\r\nSobornost Kybernauts realizing glorification shall be in proven communion\r\n\r\nThe Domain of Pochven shall be three Krais of nine fields within clade\r\n\r\nThe Flow of Vyraj will bring Sobornost of Triglav in the Domain of Pochven\r\n\r\nWe speak for the Convocation of Triglav Outside the Struggle\r\n\r\nWe are Zorya Triglav</i>\r\n\r\n \u2013 Triglavian Invasion Communique by Zorya Triglav, YC122.09.17",
+                "name": "Pochven",
+                "region_id": 10000070
+            },
             "11000031": {
                 "constellations": [
                     21000324
                 ],
                 "name": "G-R00031",
                 "region_id": 11000031
             }
@@ -1010,14 +1031,30 @@
                 "security_status": 0.9459131360054016,
                 "star_id": 40009076,
                 "stations": [
                     60003760
                 ],
                 "system_id": 30000142
             },
+            "30000157": {
+                "constellation_id": 20000787,
+                "name": "Otela",
+                "planets": [],
+                "position": {
+                    "x": -89620400993906060,
+                    "y": 75048904312138340,
+                    "z": 93501974138973170
+                },
+                "security_class": "C",
+                "security_status": -1,
+                "star_id": 40009947,
+                "stargates": [],
+                "stations": [],
+                "system_id": 30000157
+            },
             "30001161": {
                 "constellation_id": 20000169,
                 "name": "HED-GP",
                 "planets": [],
                 "position": {
                     "x": -95413697560001200,
                     "y": 19654254337720636,
```

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/testdata/factories.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/testdata/fetch_esi_raw_data.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/testdata/fetch_esi_raw_data.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/testdata/generate_sde.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/testdata/generate_sde.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/testdata/sde.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/testdata/sde.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/testdata/sde_data.json` & `django_eveuniverse-1.3.0/eveuniverse/tests/testdata/sde_data.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/testdata_example.json` & `django_eveuniverse-1.3.0/eveuniverse/tests/testdata_example.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tests/tools/clear_celery_once_locks.py` & `django_eveuniverse-1.3.0/eveuniverse/tests/tools/clear_celery_once_locks.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tools/drop_tables.sql` & `django_eveuniverse-1.3.0/eveuniverse/tools/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/tools/testdata.py` & `django_eveuniverse-1.3.0/eveuniverse/tools/testdata.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/eveuniverse/utils.py` & `django_eveuniverse-1.3.0/eveuniverse/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,16 +65,16 @@
             isinstance(dirty_value, required_type)
             and (min_value is None or dirty_value >= min_value)
             and (max_value is None or dirty_value <= max_value)
             and (choices is None or dirty_value in choices)
         ):
             cleaned_value = dirty_value
         else:
-            logger.warn(
-                "You setting for {} it not valid. Please correct it. "
+            logger.warning(
+                "Your setting for {} it not valid. Please correct it. "
                 "Using default for now: {}".format(name, default_value)
             )
             cleaned_value = default_value
     return cleaned_value
 
 
 class SocketAccessError(Exception):
```

### Comparing `django_eveuniverse-1.2.0/pyproject.toml` & `django_eveuniverse-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.2.0/PKG-INFO` & `django_eveuniverse-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-eveuniverse
-Version: 1.2.0
+Version: 1.3.0
 Summary: Complete set of Eve Universe models with on-demand loading from ESI.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

