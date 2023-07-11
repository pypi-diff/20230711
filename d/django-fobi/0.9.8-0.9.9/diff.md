# Comparing `tmp/django-fobi-0.9.8.tar.gz` & `tmp/django-fobi-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-fobi-0.9.8.tar", last modified: Thu Oct 27 21:07:01 2016, max compression
+gzip compressed data, was "dist/django-fobi-0.9.9.tar", last modified: Sun Oct 30 23:53:52 2016, max compression
```

## Comparing `django-fobi-0.9.8.tar` & `django-fobi-0.9.9.tar`

### file list

```diff
@@ -1,1375 +1,1376 @@
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    26535 2016-10-17 01:11:03.000000 django-fobi-0.9.8/LICENSE_LGPL_2.1.txt
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     7858 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/dynamic.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1048 2016-10-12 20:25:10.000000 django-fobi-0.9.8/src/fobi/context_processors.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/integration/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-12-26 00:27:09.000000 django-fobi-0.9.8/src/fobi/integration/models.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    10825 2016-10-25 19:56:48.000000 django-fobi-0.9.8/src/fobi/integration/processors.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1321 2016-10-12 20:33:21.000000 django-fobi-0.9.8/src/fobi/integration/helpers.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-12-25 14:45:47.000000 django-fobi-0.9.8/src/fobi/integration/__init__.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    22087 2016-10-16 21:50:28.000000 django-fobi-0.9.8/src/fobi/models.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     5535 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     5360 2016-10-12 20:26:43.000000 django-fobi-0.9.8/src/fobi/form_importers.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4579 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/defaults.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/migrations/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1491 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/migrations/0010_formwizardhandler.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      707 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/migrations/0006_auto_20160911_1549.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      707 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/migrations/0005_auto_20160908_1457.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3260 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/migrations/0004_auto_20160906_1513.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    10070 2016-09-28 08:55:07.000000 django-fobi-0.9.8/src/fobi/migrations/0001_initial.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      647 2016-10-05 22:04:25.000000 django-fobi-0.9.8/src/fobi/migrations/0009_formwizardentry_wizard_type.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-09-12 22:38:11.000000 django-fobi-0.9.8/src/fobi/migrations/__init__.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2809 2016-10-16 21:53:41.000000 django-fobi-0.9.8/src/fobi/migrations/0007_auto_20160926_1652.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1121 2016-09-27 22:56:31.000000 django-fobi-0.9.8/src/fobi/migrations/0008_formwizardhandlerentry.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      627 2015-09-12 22:44:00.000000 django-fobi-0.9.8/src/fobi/migrations/0002_auto_20150912_1744.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2787 2016-05-19 23:04:44.000000 django-fobi-0.9.8/src/fobi/migrations/0003_auto_20160517_1005.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    98229 2016-10-26 21:34:44.000000 django-fobi-0.9.8/src/fobi/views.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/tests/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     8891 2016-09-28 08:32:39.000000 django-fobi-0.9.8/src/fobi/tests/data.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2144 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/tests/base.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1280 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/tests/test_dynamic_forms.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     5653 2016-09-28 08:48:14.000000 django-fobi-0.9.8/src/fobi/tests/test_form_importers_mailchimp.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      416 2016-09-28 08:31:03.000000 django-fobi-0.9.8/src/fobi/tests/constants.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     9380 2016-09-28 08:46:22.000000 django-fobi-0.9.8/src/fobi/tests/helpers.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    26237 2016-10-25 21:08:32.000000 django-fobi-0.9.8/src/fobi/tests/test_browser_build_dynamic_forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      456 2016-09-28 08:39:38.000000 django-fobi-0.9.8/src/fobi/tests/__init__.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4210 2016-09-28 08:26:11.000000 django-fobi-0.9.8/src/fobi/tests/test_core.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1804 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/tests/test_sortable_dict.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    27561 2016-10-26 21:55:10.000000 django-fobi-0.9.8/src/fobi/utils.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/urls/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1919 2016-10-12 21:26:54.000000 django-fobi-0.9.8/src/fobi/urls/view.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-09-24 00:00:28.000000 django-fobi-0.9.8/src/fobi/urls/__init__.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     7467 2016-10-26 21:30:21.000000 django-fobi-0.9.8/src/fobi/urls/edit.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      434 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/test.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/management/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-08-12 09:21:42.000000 django-fobi-0.9.8/src/fobi/management/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/management/commands/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2152 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/management/commands/fobi_find_broken_entries.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1007 2016-10-12 21:48:00.000000 django-fobi-0.9.8/src/fobi/management/commands/fobi_update_plugin_data.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      460 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/management/commands/fobi_sync_plugins.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-08-12 09:21:42.000000 django-fobi-0.9.8/src/fobi/management/commands/__init__.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      754 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/management/commands/fobi_migrate_03_to_04.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2814 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/widgets.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/js/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)   348978 2015-04-20 21:48:52.000000 django-fobi-0.9.8/src/fobi/static/js/moment-with-locales.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2976 2014-09-14 00:52:06.000000 django-fobi-0.9.8/src/fobi/static/js/fobi.core.js
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    12171 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/static/js/jquery.slugify.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    93107 2013-08-21 20:57:03.000000 django-fobi-0.9.8/src/fobi/static/js/jquery-1.10.2.min.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1521 2014-01-10 17:28:07.000000 django-fobi-0.9.8/src/fobi/static/js/jquery.slugify.license.txt
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1098 2014-01-10 17:31:08.000000 django-fobi-0.9.8/src/fobi/static/js/jquery.license.txt
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/js/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)   228539 2014-09-16 18:45:26.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/js/jquery-ui-1.10.4.custom.min.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)   436715 2014-09-16 18:45:26.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/js/jquery-ui-1.10.4.custom.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1335 2014-01-10 17:31:57.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/jquery-ui.license.txt
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    31438 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/index.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      212 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      335 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      262 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4549 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      262 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4549 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      332 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     6999 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_888888_256x240.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1738 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/animated-overlay.gif
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      280 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     6922 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_222222_256x240.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      208 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_flat_75_ffffff_40x100.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     6992 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_454545_256x240.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      207 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    32046 2013-08-31 05:16:52.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/jquery-ui-1.10.3.custom.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    26939 2013-08-31 05:16:54.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/jquery-ui-1.10.3.custom.min.css
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      212 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     6299 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_ffffff_256x240.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      335 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      262 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_glass_75_dadada_1x400.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4549 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_cd0a0a_256x240.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      208 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_flat_100_ffffff_40x100.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4549 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_bbbbcc_256x240.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      262 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      212 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_flat_30_aaaaaa_40x100.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4549 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_2e83ff_256x240.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      332 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     6999 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_888888_256x240.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      331 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_highlight-hard_75_7ca0c7_1x100.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1738 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/animated-overlay.gif
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     6992 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_454545_256x240.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      342 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_highlight-soft_75_7ca0c7_1x100.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    32365 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/jquery-ui-1.10.4.custom.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    27438 2014-09-19 13:42:24.000000 django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/jquery-ui-1.10.4.custom.min.css
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/css/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2786 2013-11-23 09:43:41.000000 django-fobi-0.9.8/src/fobi/static/css/admin_custom.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1286 2014-07-12 22:23:57.000000 django-fobi-0.9.8/src/fobi/static/css/fobi.core.css
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/less/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      742 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/less/path.less
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    17555 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/less/icons.less
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2084 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/less/bootstrap.less
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2101 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/less/core.less
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    19299 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/less/font-awesome-ie7.less
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1319 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/less/font-awesome.less
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     8888 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/less/variables.less
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1041 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/less/mixins.less
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2398 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/less/extras.less
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/css/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    22084 2013-06-26 15:40:33.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/css/font-awesome.min.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    41311 2013-06-26 15:40:33.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/css/font-awesome-ie7.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    37782 2013-06-26 15:40:33.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/css/font-awesome-ie7.min.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    27232 2013-06-26 15:40:33.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/css/font-awesome.css
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/scss/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1284 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/scss/font-awesome.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    17555 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/scss/_icons.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2157 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/scss/_core.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1078 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/scss/_mixins.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    22328 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/scss/font-awesome-ie7.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2088 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/scss/_bootstrap.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     8061 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/scss/_variables.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2406 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/scss/_extras.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      753 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/scss/_path.scss
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/font/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    37405 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/font/fontawesome-webfont.eot
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    79076 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/font/fontawesome-webfont.ttf
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4060 2014-01-10 17:36:01.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/font/license.txt
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    43572 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/font/fontawesome-webfont.woff
--rw-------   0 foreverchild  (1000) foreverchild  (1000)   197829 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/font/fontawesome-webfont.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    61896 2013-06-26 15:40:32.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/font/FontAwesome.otf
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1078 2014-01-10 17:35:14.000000 django-fobi-0.9.8/src/fobi/static/font-awesome/code.license.txt
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/colorbox/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/static/colorbox/images/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     9427 2013-07-22 06:23:09.000000 django-fobi-0.9.8/src/fobi/static/colorbox/images/loading.gif
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      112 2013-07-22 06:23:09.000000 django-fobi-0.9.8/src/fobi/static/colorbox/images/border.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      157 2013-07-22 06:23:09.000000 django-fobi-0.9.8/src/fobi/static/colorbox/images/loading_background.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      182 2013-07-22 06:23:09.000000 django-fobi-0.9.8/src/fobi/static/colorbox/images/overlay.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2893 2013-07-22 06:23:09.000000 django-fobi-0.9.8/src/fobi/static/colorbox/images/controls.png
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    10894 2013-07-22 06:23:09.000000 django-fobi-0.9.8/src/fobi/static/colorbox/jquery.colorbox-min.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     5552 2013-07-22 06:23:09.000000 django-fobi-0.9.8/src/fobi/static/colorbox/index.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4340 2013-07-22 06:23:09.000000 django-fobi-0.9.8/src/fobi/static/colorbox/colorbox.css
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)   102372 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/base.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      825 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/conf.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/south_migrations/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    17332 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/south_migrations/0003_auto__add_formwizardformentry__add_unique_formwizardformentry_form_wiz.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    18066 2016-09-28 08:56:07.000000 django-fobi-0.9.8/src/fobi/south_migrations/0001_initial.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-09-12 22:59:16.000000 django-fobi-0.9.8/src/fobi/south_migrations/__init__.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     9648 2016-09-28 08:56:41.000000 django-fobi-0.9.8/src/fobi/south_migrations/0002_auto__add_field_formentry_created__add_field_formentry_updated.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    16183 2016-10-26 20:50:21.000000 django-fobi-0.9.8/src/fobi/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1650 2016-10-12 20:25:00.000000 django-fobi-0.9.8/src/fobi/constants.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    27930 2016-10-26 21:00:28.000000 django-fobi-0.9.8/src/fobi/helpers.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/locale/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/locale/nl/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    67718 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/locale/nl/LC_MESSAGES/django.po
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    20358 2015-09-01 21:33:55.000000 django-fobi-0.9.8/src/fobi/locale/nl/LC_MESSAGES/django.mo
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/locale/de/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/locale/de/LC_MESSAGES/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    67245 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/locale/de/LC_MESSAGES/django.po
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    19060 2015-05-21 20:55:50.000000 django-fobi-0.9.8/src/fobi/locale/de/LC_MESSAGES/django.mo
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/locale/ru/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    73378 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/locale/ru/LC_MESSAGES/django.po
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    26568 2015-09-01 20:46:56.000000 django-fobi-0.9.8/src/fobi/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      320 2016-10-12 20:24:37.000000 django-fobi-0.9.8/src/fobi/compat.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/wizard/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       21 2016-10-09 19:25:24.000000 django-fobi-0.9.8/src/fobi/wizard/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/wizard/views/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    32774 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/wizard/views/dynamic.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2670 2016-10-12 08:21:29.000000 django-fobi-0.9.8/src/fobi/wizard/views/views.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       44 2016-10-09 19:50:24.000000 django-fobi-0.9.8/src/fobi/wizard/views/__init__.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      752 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/app.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     8147 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/data_structures.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3913 2016-10-12 20:25:24.000000 django-fobi-0.9.8/src/fobi/decorators.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    20455 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/admin.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      342 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      249 2016-10-27 20:30:30.000000 django-fobi-0.9.8/src/fobi/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/templates/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/templates/fobi/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/templates/fobi/integration/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      180 2014-12-25 15:34:14.000000 django-fobi-0.9.8/src/fobi/templates/fobi/integration/login_required.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      832 2016-10-26 22:23:19.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/view_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      648 2016-10-26 22:20:32.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/form_entry_submitted.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    11137 2016-10-26 22:17:29.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/edit_form_wizard_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      215 2015-08-26 20:42:27.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/import_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      310 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/add_form_handler_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      388 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/edit_form_element_entry_ajax.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      219 2016-09-27 20:51:04.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/create_form_wizard_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      212 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/create_form_entry_ajax.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3783 2016-10-26 21:47:11.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/form_wizards_dashboard.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      640 2016-10-26 22:20:40.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/form_importer.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3421 2016-10-26 09:32:40.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/dashboard.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     8519 2016-10-26 09:34:31.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/_base.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      314 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/edit_form_handler_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      216 2014-10-25 20:10:36.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/embed_form_entry_submitted_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      223 2015-09-25 23:25:31.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/form_importer_ajax.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1586 2016-10-26 22:23:57.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/edit_form_wizard_entry.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      331 2016-10-14 21:35:11.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/add_form_wizard_handler_entry_ajax.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      835 2016-10-26 22:24:11.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/create_form_wizard_entry.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1701 2015-12-21 23:09:23.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/forms_list.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      371 2014-10-24 23:38:47.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/view_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1307 2016-10-26 22:20:17.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/edit_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      703 2014-10-25 20:14:39.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/form_entry_submitted_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     9171 2016-10-04 21:23:15.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/edit_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      203 2014-10-24 23:42:05.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/view_embed_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      648 2016-10-26 22:19:49.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/create_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      384 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/add_form_element_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      215 2014-03-26 23:50:46.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/base.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      744 2016-10-26 22:20:00.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/add_form_handler_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      746 2016-10-26 22:20:10.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/edit_form_element_entry.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1356 2016-10-17 00:55:46.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_wizard_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      947 2014-08-14 22:08:03.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_edit_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1191 2016-10-17 00:38:56.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_view_ajax.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1291 2016-10-17 01:22:50.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_wizard_view_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3478 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_properties_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1170 2014-10-24 23:41:45.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      229 2014-03-27 00:10:11.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/messages_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       86 2014-12-02 23:33:06.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_non_field_and_hidden_errors_snippet.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4235 2016-10-16 22:24:36.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_wizard_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2238 2015-10-05 21:51:48.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_wizard.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4209 2016-10-19 02:09:19.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_snippet.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3478 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_wizard_properties_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      746 2016-10-26 22:20:24.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/edit_form_handler_entry.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1157 2016-10-17 01:24:55.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/view_form_wizard_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      648 2016-10-26 22:23:06.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/import_form_entry.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1047 2016-10-26 22:27:25.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/view_form_wizard_entry.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      738 2016-10-17 00:21:43.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/form_wizard_entry_submitted_ajax.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      765 2016-10-26 22:24:16.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/add_form_wizard_handler_entry.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      663 2016-10-26 22:23:49.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/form_wizard_entry_submitted.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4220 2013-12-26 16:34:28.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/theme.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      744 2016-10-26 22:19:42.000000 django-fobi-0.9.8/src/fobi/templates/fobi/generic/add_form_element_entry.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/templates/fobi/admin/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3834 2013-12-22 16:17:35.000000 django-fobi-0.9.8/src/fobi/templates/fobi/admin/bulk_change_plugins.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1034 2016-10-12 20:26:57.000000 django-fobi-0.9.8/src/fobi/form_utils.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1172 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/validators.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/db_store/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/db_store/models.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      829 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/db_store/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      645 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/db_store/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      424 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/db_store/__init__.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/js/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1789 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/js/fobi.djangocms_admin_style_theme.edit.js
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/css/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1286 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/css/fobi.djangocms_admin_style_theme.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4239 2016-10-04 21:21:18.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/css/fobi.djangocms_admin_style_theme.edit.css
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/admin/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/admin/img/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      932 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/admin/img/tooltag-add.gif
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      197 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/admin/img/tool-left.gif
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      336 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/admin/img/tooltag-add_over.gif
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     6862 2016-10-04 22:19:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/fobi_themes.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      486 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      389 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       49 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/view_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/form_entry_submitted.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2015-08-27 21:03:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/import_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/add_form_handler_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/edit_form_element_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/create_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3811 2015-12-16 01:49:29.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/dashboard.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       95 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/_base.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/edit_form_handler_entry_ajax.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2069 2015-12-21 23:10:38.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/forms_list.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/view_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      225 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/edit_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       59 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/form_entry_submitted_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     7989 2016-10-04 21:22:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/edit_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      175 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/create_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/add_form_element_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/base.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     6512 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/base_edit.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      507 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/add_form_handler_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      502 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/edit_form_element_entry.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      946 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_edit_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       57 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_view_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1752 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_properties_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      393 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       59 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/messages_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1466 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_edit_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2189 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      502 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/edit_form_handler_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      227 2015-08-27 21:03:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/import_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3193 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/base_view.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4220 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/theme.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      506 2015-02-10 23:12:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/add_form_element_entry.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/widgets/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-11-07 23:26:00.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/widgets/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/widgets/form_handlers/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/widgets/form_handlers/db_store/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-11-07 23:26:00.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/widgets/form_handlers/db_store/models.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      766 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/widgets/form_handlers/db_store/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      516 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/widgets/form_handlers/db_store/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      365 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/widgets/form_handlers/db_store/__init__.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-11-07 23:26:00.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/widgets/form_handlers/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/simple/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/simple/js/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1789 2014-09-23 23:49:06.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/simple/js/fobi.simple.edit.js
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/simple/css/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2984 2016-10-04 21:21:28.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/simple/css/fobi.simple.edit.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1242 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/simple/css/fobi.simple.css
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/admin/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/admin/img/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      932 2014-12-26 00:18:40.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/admin/img/tooltag-add.gif
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      197 2014-12-26 00:18:40.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/admin/img/tool-left.gif
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      336 2014-12-26 00:18:40.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/admin/img/tooltag-add_over.gif
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4266 2016-10-04 22:21:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/fobi_themes.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      423 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      300 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       49 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/view_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/form_entry_submitted.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2015-08-27 21:03:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/import_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/add_form_handler_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/edit_form_element_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2014-09-22 22:32:40.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/create_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3690 2015-12-16 01:49:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/dashboard.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       74 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/_base.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/edit_form_handler_entry_ajax.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2056 2015-12-21 23:10:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/forms_list.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/view_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      225 2014-09-23 01:29:25.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/edit_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       59 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/form_entry_submitted_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     7957 2016-10-04 21:23:02.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/edit_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      175 2014-09-25 22:08:26.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/create_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/add_form_element_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       33 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/base.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     5858 2014-10-11 21:13:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/base_edit.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      507 2014-09-25 22:08:26.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/add_form_handler_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      502 2014-09-25 22:08:26.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/edit_form_element_entry.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/snippets/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      946 2014-09-22 22:43:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/snippets/form_edit_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       57 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/snippets/form_view_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1752 2014-10-07 23:14:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/snippets/form_properties_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      393 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/snippets/form_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       59 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/snippets/messages_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1466 2014-10-07 23:14:21.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/snippets/form_edit_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2189 2014-12-04 01:26:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/snippets/form_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      502 2014-09-25 22:08:26.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/edit_form_handler_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      228 2015-08-27 21:03:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/import_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3193 2014-10-11 21:14:05.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/base_view.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4220 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/theme.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      506 2014-09-25 22:08:26.000000 django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/add_form_element_entry.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/static/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/static/foundation5/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/static/foundation5/js/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      358 2015-04-26 01:41:13.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/static/foundation5/js/fobi.plugin.date-foundation5-widget.js
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1027 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      634 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      422 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/static/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/static/foundation5/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/static/foundation5/js/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      377 2015-04-26 01:41:39.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/static/foundation5/js/fobi.plugin.datetime-foundation5-widget.js
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1075 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      646 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      430 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/__init__.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-04-25 21:34:17.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/dummy_foundation5_widget/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      892 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/dummy_foundation5_widget/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      637 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/dummy_foundation5_widget/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      424 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/dummy_foundation5_widget/__init__.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-11-07 23:08:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_handlers/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-11-07 23:24:49.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/models.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      939 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      646 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      430 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/templates/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/templates/db_store_foundation5_widget/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2205 2014-11-08 22:35:49.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/templates/db_store_foundation5_widget/view_saved_form_data_entries.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      178 2014-11-08 21:41:59.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/templates/db_store_foundation5_widget/plugin_data_repr.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-11-07 23:09:02.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_handlers/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/img/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        1 2014-08-21 21:50:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/img/.gitkeep
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    89082 2014-06-01 21:26:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation_template-4.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    95120 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation.min.js
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     8271 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/fastclick.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    11262 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/modernizr.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1415 2014-08-21 21:50:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/jquery.cookie.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    84621 2014-08-21 21:50:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/jquery.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2330 2014-08-21 21:50:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/placeholder.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    37736 2015-04-25 21:44:18.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation-datepicker.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1712 2014-09-14 00:38:39.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation5_fobi_extras.js
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    15318 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.orbit.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     7957 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.slider.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2100 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.equalizer.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    14068 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.reveal.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    11070 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.abide.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    14543 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.topbar.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1237 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.alert.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    29980 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.joyride.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     9922 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.dropdown.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     7057 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.magellan.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    10487 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.tooltip.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    18425 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    16859 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.clearing.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     5085 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.offcanvas.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     6401 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.tab.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2144 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.accordion.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     9228 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.interchange.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    54154 2015-04-25 23:05:35.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation-datetimepicker.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      106 2014-08-21 21:50:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/robots.txt
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/sass/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1303 2012-08-10 06:06:00.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/sass/accessibility_foundicons.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1032 2012-08-10 15:14:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/sass/accessibility_foundicons_ie7.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      775 2012-08-10 06:06:03.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/sass/_settings.scss
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/stylesheets/
--rwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)     2196 2015-10-23 23:38:38.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/stylesheets/accessibility_foundicons.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2920 2012-08-10 15:15:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/stylesheets/accessibility_foundicons_ie7.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     5508 2012-08-10 14:47:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/demo.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    15316 2012-08-10 08:07:26.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.eot
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     9188 2012-08-10 08:07:26.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.woff
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    15056 2012-08-10 08:07:26.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.ttf
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      628 2012-08-10 08:07:28.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.svg
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/0e61251fcc72078e76f7711e6e025bea2a2f1ce3/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4166 2012-08-10 06:06:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/0e61251fcc72078e76f7711e6e025bea2a2f1ce3/_settings.scssc
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     5690 2012-08-10 06:06:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/0e61251fcc72078e76f7711e6e025bea2a2f1ce3/accessibility_foundicons.scssc
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4526 2012-08-10 15:15:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/0e61251fcc72078e76f7711e6e025bea2a2f1ce3/accessibility_foundicons_ie7.scssc
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/sass/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1954 2012-08-10 14:40:25.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/sass/general_foundicons.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      763 2012-08-10 14:28:35.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/sass/_settings.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1704 2012-08-10 14:43:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/sass/general_foundicons_ie7.scss
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/stylesheets/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3177 2012-08-10 14:40:25.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/stylesheets/general_foundicons.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     5119 2012-08-10 14:43:45.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/stylesheets/general_foundicons_ie7.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     7812 2012-08-10 14:47:38.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/demo.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    15488 2012-08-10 08:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.ttf
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      616 2012-08-10 08:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     9728 2012-08-10 08:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.woff
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    15724 2012-08-10 08:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.eot
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4142 2012-08-10 14:25:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/_settings.scssc
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     8399 2012-08-10 14:40:25.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/general_foundicons.scssc
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     7277 2012-08-10 14:43:45.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/general_foundicons_ie7.scssc
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     5688 2012-08-10 14:24:32.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/accessibility_foundicons.scssc
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4524 2012-08-10 14:24:32.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/accessibility_foundicons_ie7.scssc
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/sass/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1704 2012-08-10 15:17:14.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/sass/general_enclosed_foundicons_ie7.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1954 2012-08-10 14:46:17.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/sass/general_enclosed_foundicons.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      780 2012-08-10 14:46:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/sass/_settings.scss
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/stylesheets/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     5127 2012-08-10 15:17:19.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/stylesheets/general_enclosed_foundicons_ie7.css
--rwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)     3246 2015-10-23 23:38:38.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/stylesheets/general_enclosed_foundicons.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     7879 2012-08-10 15:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/demo.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    18912 2012-08-10 08:07:40.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.eot
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      633 2012-08-10 08:07:40.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    18640 2012-08-10 08:07:40.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.ttf
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     9536 2012-08-10 08:07:40.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.woff
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/1ea694b23cbc52b68bcbd397d07df10b08a18c32/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4176 2012-08-10 14:44:32.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/1ea694b23cbc52b68bcbd397d07df10b08a18c32/_settings.scssc
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     8399 2012-08-10 14:46:18.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/1ea694b23cbc52b68bcbd397d07df10b08a18c32/general_enclosed_foundicons.scssc
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     7277 2012-08-10 15:17:19.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/1ea694b23cbc52b68bcbd397d07df10b08a18c32/general_enclosed_foundicons_ie7.scssc
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/sass/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1179 2012-08-10 14:54:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/sass/social_foundicons_ie7.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1447 2012-08-10 14:54:25.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/sass/social_foundicons.scss
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      761 2012-08-10 14:49:50.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/sass/_settings.scss
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/stylesheets/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3352 2012-08-10 14:54:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/stylesheets/social_foundicons_ie7.css
--rwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)     2355 2015-10-23 23:38:38.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/stylesheets/social_foundicons.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     5786 2012-08-10 15:09:12.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/demo.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    17112 2012-08-10 08:07:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.eot
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    10644 2012-08-10 08:07:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.woff
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    16880 2012-08-10 08:07:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.ttf
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      614 2012-08-10 08:07:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.svg
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/0bd576c1f1487db9a103f544ad85fa8a0f88a6ea/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4138 2012-08-10 14:49:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/0bd576c1f1487db9a103f544ad85fa8a0f88a6ea/_settings.scssc
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     6245 2012-08-10 14:54:17.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/0bd576c1f1487db9a103f544ad85fa8a0f88a6ea/social_foundicons.scssc
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     5088 2012-08-10 14:54:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/0bd576c1f1487db9a103f544ad85fa8a0f88a6ea/social_foundicons_ie7.scssc
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    32020 2013-08-23 16:25:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.woff
--rw-------   0 foreverchild  (1000) foreverchild  (1000)   324210 2013-08-23 16:59:19.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/preview.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2086 2013-08-23 02:50:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-trees.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1822 2013-08-23 02:50:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-steam.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1105 2013-08-23 03:07:46.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-layout.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1743 2013-08-23 03:21:32.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-zoom-in.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1928 2013-08-23 03:07:45.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-burst.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2879 2013-08-23 02:50:56.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-male-female.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2561 2013-08-23 03:21:32.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-calendar.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2171 2013-08-23 03:07:45.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-euro.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1384 2013-08-23 03:21:34.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-trend.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      756 2013-08-23 03:21:35.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-contrast.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1227 2013-08-23 03:21:31.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-upload.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1394 2013-08-23 02:50:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-trophy.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1273 2013-08-23 03:21:37.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-remove.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      827 2013-08-23 03:21:31.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-home.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1285 2013-08-23 03:03:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-xbox.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      835 2013-08-23 03:07:43.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-play.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2200 2013-08-23 02:50:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-no-dogs.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1537 2013-08-23 02:50:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-sheriff-badge.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      881 2013-08-23 03:21:34.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pencil.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1326 2013-08-23 03:07:46.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-price-tag.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1762 2013-08-23 02:50:56.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-wheelchair.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1352 2013-08-23 03:21:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-address-book.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      904 2013-08-23 03:07:41.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mobile.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4724 2013-08-23 03:21:36.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-sound.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1105 2013-08-23 03:07:41.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-usb.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      986 2013-08-23 03:07:45.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-credit-card.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1194 2013-08-23 03:21:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-annotate.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1345 2013-08-23 03:21:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torso-female.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1041 2013-08-23 03:21:31.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-star.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1396 2013-08-23 03:21:36.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-microphone.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1388 2013-08-23 02:50:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-stumbleupon.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1122 2013-08-23 02:50:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-foot.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1951 2013-08-23 03:21:34.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-database.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1369 2013-08-23 03:07:42.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-left.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1697 2013-08-23 02:50:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-six.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2013 2013-08-23 02:50:56.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-universal-access.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2421 2013-08-23 03:07:45.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-burst-new.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      681 2013-08-23 03:21:31.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-minus.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1140 2013-08-23 03:07:41.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-underline.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1356 2013-08-23 03:07:46.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-web.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1494 2013-08-23 03:21:32.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paperclip.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1219 2013-08-23 03:07:45.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-eject.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1307 2013-08-23 03:07:45.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shopping-cart.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1670 2013-08-23 03:21:37.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-csv.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1357 2013-08-23 03:21:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-folder-add.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2020 2013-08-23 03:07:42.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list-number.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1817 2013-08-23 02:50:56.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-blind.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      935 2013-08-23 03:07:46.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-html5.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2616 2013-08-23 03:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-google-plus.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1714 2013-08-23 03:21:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-male-female.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1718 2013-08-23 02:50:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-at-sign.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      835 2013-08-23 03:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-forrst.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1453 2013-08-23 03:21:36.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2487 2013-08-23 02:50:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-treehouse.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1897 2013-08-23 02:50:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-yelp.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      598 2013-08-23 03:07:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-delicious.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      869 2013-08-23 03:21:32.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-cloud.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      953 2013-08-23 03:07:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-dropbox.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1141 2013-08-23 02:50:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-safety-cone.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1069 2013-08-23 02:50:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-two.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1409 2013-08-23 02:50:56.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-male.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1504 2013-08-23 03:07:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-blogger.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1164 2013-08-23 03:21:36.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comments.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1190 2013-08-23 03:21:34.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-eye.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1811 2013-08-23 03:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-hi5.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2076 2013-08-23 02:50:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-skull.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1107 2013-08-23 02:50:50.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-rdio.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      950 2013-08-23 02:50:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-prohibited.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      713 2013-08-23 03:21:35.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-video.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1801 2013-08-23 03:07:46.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pricetag-multiple.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1644 2013-08-23 03:07:43.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-indent-more.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1568 2013-08-23 03:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-game-center.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1425 2013-08-23 03:21:35.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-alert.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     5365 2013-08-23 02:50:56.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-asl.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      959 2013-08-23 03:07:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-volume-none.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1052 2013-08-23 03:07:43.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-filter.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      883 2013-08-23 03:07:41.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-italic.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2065 2013-08-23 03:07:42.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-strikethrough.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3053 2013-08-23 02:50:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-skillshare.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2134 2013-08-23 02:50:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-spotify.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1411 2013-08-23 02:50:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clipboard.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1795 2013-08-23 02:50:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-power.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2862 2013-08-23 03:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-joomla.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1028 2013-08-23 03:21:32.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-magnifying-glass.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2398 2013-08-23 03:07:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-volume.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      911 2013-08-23 03:07:43.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-stop.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1564 2013-08-23 03:21:36.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bluetooth.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3133 2013-08-23 03:07:46.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-dollar-bill.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1041 2013-08-23 03:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-medium.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2325 2013-08-23 03:09:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mobile-signal.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1233 2013-08-23 03:21:32.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-zoom-out.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1318 2013-08-23 03:21:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-folder-lock.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1258 2013-08-23 03:21:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clock.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      984 2013-08-23 03:07:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-fast-forward.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2950 2013-08-23 02:50:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-lightbulb.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1073 2013-08-23 03:21:35.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-camera.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1052 2013-08-23 03:21:34.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-minus-circle.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1644 2013-08-23 03:07:42.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-indent-less.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1195 2013-08-23 02:50:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-compass.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      976 2013-08-23 03:07:41.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bold.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1178 2013-08-23 02:50:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-tumblr.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2334 2013-08-23 03:21:37.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export-doc.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2827 2013-08-23 02:50:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-squidoo.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1130 2013-08-23 03:21:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-share.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1448 2013-08-23 03:21:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      922 2013-08-23 03:21:29.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-right.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1758 2013-08-23 03:07:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-deviant-art.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1467 2013-08-23 03:21:37.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-edit.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1431 2013-08-23 03:21:29.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-expand.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1187 2013-08-23 02:50:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-target.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1455 2013-08-23 03:21:34.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-x-circle.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1693 2013-08-23 03:07:45.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-dollar.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1238 2013-08-23 03:21:35.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-telephone.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1975 2013-08-23 02:50:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-no-smoking.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1435 2013-08-23 03:21:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-compress.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1192 2013-08-23 03:07:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-play-circle.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1436 2013-08-23 02:50:50.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-pinterest.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1051 2013-08-23 03:21:31.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-marker.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1915 2013-08-23 02:50:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-vimeo.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1231 2013-08-23 03:21:31.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-download.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1314 2013-08-23 03:07:42.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-text-color.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1504 2013-08-23 03:21:37.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-search.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1135 2013-08-23 03:07:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-bing.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      937 2013-08-23 02:50:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-battery-full.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1094 2013-08-23 03:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-linkedin.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1237 2013-08-23 03:07:41.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-laptop.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1430 2013-08-23 03:21:37.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-add.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1645 2013-08-23 03:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-instagram.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3487 2013-08-23 02:50:56.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-elevator.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1925 2013-08-23 02:50:56.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-female.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1836 2013-08-23 02:50:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-snapchat.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1712 2013-08-23 02:50:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-map.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1158 2013-08-23 03:21:34.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-horizontal.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1883 2013-08-23 02:50:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-yahoo.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1533 2013-08-23 02:50:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-five.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1055 2013-08-23 03:21:31.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-plus.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1390 2013-08-23 03:07:42.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-right.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1334 2013-08-23 03:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-lastfm.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1821 2013-08-23 02:50:50.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-reddit.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1224 2013-08-23 02:50:56.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-male-symbol.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2323 2013-08-23 03:07:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-android.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      760 2013-08-23 02:50:56.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-braille.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1520 2013-08-23 03:21:32.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-wrench.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1674 2013-08-23 03:21:37.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-doc.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1796 2013-08-23 02:50:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-anchor.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3511 2013-08-23 03:07:43.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-unlink.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      929 2013-08-23 03:07:46.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-css3.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1423 2013-08-23 02:50:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-key.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2253 2013-08-23 03:07:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-evernote.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2960 2013-08-23 03:21:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-thumbnails.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1212 2013-08-23 03:07:43.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-photo.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      995 2013-08-23 03:21:32.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-unlock.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      921 2013-08-23 03:21:29.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-up.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1818 2013-08-23 02:50:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-crown.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1969 2013-08-23 03:07:42.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-superscript.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1042 2013-08-23 03:21:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torso.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1101 2013-08-23 02:50:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-zurb.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1352 2013-08-23 03:21:35.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-upload-cloud.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1865 2013-08-23 02:50:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-asterisk.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1749 2013-08-23 02:50:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-first-aid.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1814 2013-08-23 03:07:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-dribbble.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2306 2013-08-23 03:21:37.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export-csv.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1218 2013-08-23 03:21:31.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-refresh.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1132 2013-08-23 03:21:38.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-multiple.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1515 2013-08-23 03:21:35.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-dislike.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      984 2013-08-23 03:07:42.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-background-color.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      849 2013-08-23 03:07:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-record.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1325 2013-08-23 03:07:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-next.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2354 2013-08-23 03:21:29.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-out.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1285 2013-08-23 02:50:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-twitter.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      814 2013-08-23 03:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-hacker-news.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2226 2013-08-23 02:50:56.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-guide-dog.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2075 2013-08-23 03:21:37.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export-pdf.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1861 2013-08-23 02:50:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-ticket.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1163 2013-08-23 02:50:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-projection-screen.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1093 2013-08-23 03:21:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-flag.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2365 2013-08-23 03:21:29.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-in.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2562 2013-08-23 02:50:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-skype.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1385 2013-08-23 02:50:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-four.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1292 2013-08-23 03:07:42.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-justify.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      983 2013-08-23 03:07:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-rewind.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1688 2013-08-23 03:21:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torso-business.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1557 2013-08-23 03:21:35.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-like.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      919 2013-08-23 03:21:29.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-left.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1611 2013-08-23 03:07:43.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-link.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2292 2013-08-23 02:50:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-puzzle.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      921 2013-08-23 03:21:29.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-down.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1014 2013-08-23 03:07:41.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-tablet-landscape.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1004 2013-08-23 02:50:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mountains.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1840 2013-08-23 03:21:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-all-female.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2858 2013-08-23 03:21:36.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment-quotes.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      888 2013-08-23 03:21:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-play-video.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1845 2013-08-23 03:07:46.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paypal.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      882 2013-08-23 03:07:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-facebook.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1516 2013-08-23 03:21:37.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-delete.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1085 2013-08-23 03:07:43.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-print.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      816 2013-08-23 02:50:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shield.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      876 2013-08-23 02:50:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-battery-empty.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      770 2013-08-23 03:07:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-drive.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      805 2013-08-23 02:50:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-windows.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1798 2013-08-23 03:07:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-loop.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2438 2013-08-23 03:07:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-volume-strike.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1670 2013-08-23 03:21:36.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-megaphone.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1453 2013-08-23 02:50:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-target-two.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1398 2013-08-23 02:50:57.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-female-symbol.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3657 2013-08-23 02:50:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-youtube.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1325 2013-08-23 02:50:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paw.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1207 2013-08-23 03:21:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-crop.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      921 2013-08-23 03:21:31.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-heart.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1378 2013-08-23 03:21:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4361 2013-08-23 02:50:56.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-telephone-accessible.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1297 2013-08-23 03:07:43.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pause.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1477 2013-08-23 02:50:50.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-picasa.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1246 2013-08-23 03:07:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-apple.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1019 2013-08-23 03:21:38.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-filled.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1533 2013-08-23 03:07:43.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-save.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1460 2013-08-23 03:02:58.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-stack-overflow.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1418 2013-08-23 03:07:43.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paint-bucket.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4229 2013-08-23 03:07:46.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-foundation.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      941 2013-08-23 03:21:31.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-check.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1966 2013-08-23 03:07:42.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-subscript.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      902 2013-08-23 03:07:46.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shopping-bag.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1856 2013-08-23 03:21:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-all.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1910 2013-08-23 03:21:35.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mail.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1553 2013-08-23 03:21:32.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-rss.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1450 2013-08-23 02:50:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-book.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      990 2013-08-23 03:21:32.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-lock.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1707 2013-08-23 03:21:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-female-male.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3703 2013-08-23 03:07:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-digg.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2290 2013-08-23 03:21:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list-thumbnails.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1510 2013-08-23 02:50:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-book-bookmark.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2333 2013-08-23 03:07:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-behance.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2867 2013-08-23 03:21:34.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-results.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2850 2013-08-23 02:50:56.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-hearing-aid.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      940 2013-08-23 03:07:41.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-monitor.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1227 2013-08-23 02:50:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-three.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1976 2013-08-23 03:21:31.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-widget.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      827 2013-08-23 03:21:36.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1019 2013-08-23 03:21:32.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-trash.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3130 2013-08-23 02:50:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clipboard-notes.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1348 2013-08-23 03:21:34.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-bar.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1526 2013-08-23 03:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-foursquare.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2859 2013-08-23 03:07:46.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-500px.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      826 2013-08-23 03:21:33.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-folder.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1055 2013-08-23 03:07:49.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-orkut.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      881 2013-08-23 02:50:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-one.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      747 2013-08-23 03:07:46.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-adobe.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1061 2013-08-23 03:21:38.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-copy.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2798 2013-08-23 03:07:45.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-burst-sale.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2228 2013-08-23 03:07:45.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pound.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1239 2013-08-23 03:21:34.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-pie.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2414 2013-08-23 03:21:35.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-results-demographics.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1558 2013-08-23 03:21:34.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-archive.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      997 2013-08-23 02:50:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-info.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1961 2013-08-23 03:07:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-designer-news.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2614 2013-08-23 03:07:43.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-quote.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1041 2013-08-23 03:21:36.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment-video.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      926 2013-08-23 02:50:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-music.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3461 2013-08-23 16:21:31.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-smashing-mag.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1799 2013-08-23 03:07:45.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-yen.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      956 2013-08-23 02:50:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-battery-half.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1162 2013-08-23 03:21:36.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment-minus.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1458 2013-08-23 02:50:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-zerply.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2080 2013-08-23 03:07:45.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-rewind-ten.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      822 2013-08-23 03:21:36.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1372 2013-08-23 03:07:42.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-center.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2006 2013-08-23 02:50:56.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-closed-caption.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1797 2013-08-23 03:07:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shuffle.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1296 2013-08-23 03:07:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-previous.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1495 2013-08-23 03:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-github.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1775 2013-08-23 03:07:45.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bitcoin-circle.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1525 2013-08-23 03:07:49.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-myspace.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1450 2013-08-23 03:21:37.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-pdf.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1100 2013-08-23 03:21:31.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-x.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2028 2013-08-23 02:50:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clipboard-pencil.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      896 2013-08-23 03:21:35.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bookmark.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      923 2013-08-23 03:07:48.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-flickr.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1015 2013-08-23 03:07:41.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-tablet-portrait.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1332 2013-08-23 03:21:34.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-checkbox.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      977 2013-08-23 02:50:50.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-path.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2227 2013-08-23 03:07:45.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bitcoin.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1228 2013-08-23 03:07:42.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list-bullet.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2643 2013-08-23 03:07:46.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-amazon.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     6246 2013-08-23 04:32:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/.fontcustom-data
--rw-------   0 foreverchild  (1000) foreverchild  (1000)   150535 2013-08-23 16:25:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    19508 2013-08-23 16:57:53.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    54568 2013-08-23 16:25:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.eot
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    56976 2013-08-23 16:25:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.ttf
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     6424 2014-08-21 21:50:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/index.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/css/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     7783 2014-08-21 21:50:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/css/normalize.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      932 2015-04-25 23:06:13.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation_fobi_extras.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)   168084 2014-06-01 21:16:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation_template-4.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)   180512 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3404 2015-04-25 21:57:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation-datepicker.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4297 2015-04-25 23:05:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation-datetimepicker.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)   141825 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation.min.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      237 2014-08-21 21:50:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/humans.txt
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4787 2016-10-04 22:19:58.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/fobi_themes.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      438 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      308 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       49 2014-01-17 01:18:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/view_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2014-01-17 01:18:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/form_entry_submitted.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2015-08-27 21:03:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/import_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2014-01-17 01:18:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/add_form_handler_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2014-01-17 01:18:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/edit_form_element_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2014-01-17 01:18:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/create_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2665 2015-12-16 01:02:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/dashboard.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     5506 2014-09-26 02:16:06.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/_base.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2014-01-17 01:18:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/edit_form_handler_entry_ajax.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1363 2015-12-21 23:10:31.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/forms_list.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2014-01-17 01:18:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/view_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      151 2014-09-26 02:16:13.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/edit_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       59 2014-01-17 02:04:59.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/form_entry_submitted_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     8567 2016-10-04 21:22:49.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/edit_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       51 2014-01-17 01:18:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/create_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2014-01-17 01:18:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/add_form_element_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       38 2014-03-27 21:40:35.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/base.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2014-01-17 01:18:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/add_form_handler_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       57 2014-01-17 01:18:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/edit_form_element_entry.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3421 2014-10-07 22:38:28.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/form_properties_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1173 2014-09-30 22:34:58.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/form_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      138 2014-06-18 23:14:00.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/messages_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      331 2014-12-04 01:22:25.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/form_non_field_and_hidden_errors_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3668 2015-03-26 22:47:54.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/form_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       57 2014-01-17 01:18:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/edit_form_handler_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      154 2015-08-27 21:03:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/import_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4220 2014-01-17 01:18:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/theme.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2014-01-17 01:18:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/add_form_element_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-12-26 15:48:03.000000 django-fobi-0.9.8/src/fobi/contrib/themes/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/dummy_bootstrap3_widget/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      889 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/dummy_bootstrap3_widget/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      631 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/dummy_bootstrap3_widget/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      420 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/dummy_bootstrap3_widget/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/static/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/static/bootstrap3/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/static/bootstrap3/js/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      380 2015-04-26 01:43:03.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/static/bootstrap3/js/fobi.plugin.datetime-bootstrap3-widget.js
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1072 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      640 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      426 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/__init__.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-04-20 20:43:43.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/static/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/static/bootstrap3/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/static/bootstrap3/js/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      359 2015-04-26 01:42:37.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/static/bootstrap3/js/fobi.plugin.date-bootstrap3-widget.js
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1032 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      628 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      418 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/js/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      737 2016-10-27 20:27:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/js/fobi.plugin.slider-bootstrap3-widget.js
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    57251 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/js/bootstrap-slider.js
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    32390 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/js/bootstrap-slider.min.js
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/css/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     8404 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/css/bootstrap-slider.css
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      595 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/css/fobi.plugin.slider-bootstrap3-widget.css
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     7522 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/css/bootstrap-slider.min.css
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1010 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      634 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      422 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/__init__.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-04-20 20:43:46.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    58533 2013-12-05 16:40:18.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3253 2016-09-30 21:19:06.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap3_fobi_extras.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    30410 2015-03-07 16:32:25.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap-datetimepicker.min.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    27822 2013-12-05 16:40:19.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap.min.js
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    14716 2013-12-05 16:40:18.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap-theme.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    99548 2013-12-05 16:40:18.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap.min.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)   122848 2013-12-05 16:40:18.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     8860 2015-03-07 16:32:25.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap-datetimepicker.min.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      502 2015-03-25 01:06:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap3_fobi_extras.css
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    13135 2013-12-05 16:40:18.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap-theme.min.css
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    62850 2013-12-05 16:40:18.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.svg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    23292 2013-12-05 16:40:18.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.woff
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    20290 2013-12-05 16:40:18.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.eot
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    41236 2013-12-05 16:40:18.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     8326 2016-10-16 23:35:21.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/fobi_themes.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      435 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      312 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       49 2014-01-16 21:51:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/view_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2014-01-16 21:51:02.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/form_entry_submitted.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       61 2016-09-29 20:28:59.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_wizard_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2014-01-16 21:48:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/add_form_handler_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2014-01-16 21:50:13.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_element_entry_ajax.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       63 2016-09-27 21:07:24.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/create_form_wizard_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2014-01-16 21:49:42.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/create_form_entry_ajax.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       56 2016-10-16 23:34:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/form_wizards_dashboard.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       47 2015-10-05 21:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/form_importer.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       43 2014-01-16 21:49:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/dashboard.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      851 2016-10-26 09:36:19.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/_base.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2014-01-16 21:50:49.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_handler_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       65 2014-10-25 20:16:31.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/embed_form_entry_submitted_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       52 2015-10-05 21:40:14.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/form_importer_ajax.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       56 2016-09-29 20:28:52.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_wizard_entry.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       68 2016-10-14 21:36:17.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/add_form_wizard_handler_entry_ajax.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       58 2016-09-27 21:07:12.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/create_form_wizard_entry.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       44 2015-12-21 22:21:03.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/forms_list.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2014-01-16 21:51:41.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/view_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       49 2014-01-16 21:50:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       59 2014-01-17 02:04:51.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/form_entry_submitted_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2014-01-16 21:50:32.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       60 2014-10-24 22:17:58.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/view_embed_form_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       51 2014-01-16 21:49:27.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/create_form_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2014-01-16 21:48:11.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/add_form_element_entry_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       37 2014-01-16 21:49:07.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/base.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2014-01-16 21:48:40.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/add_form_handler_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       57 2014-01-16 21:50:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_element_entry.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      400 2016-10-14 21:51:03.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_wizard_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      931 2014-09-12 23:40:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_properties_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      393 2014-01-16 21:07:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_ajax.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       59 2014-01-16 21:45:13.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/messages_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      612 2014-12-02 23:30:22.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_non_field_and_hidden_errors_snippet.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      847 2016-09-30 21:16:34.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_wizard_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2015-10-05 21:39:47.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_wizard.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      840 2014-12-02 23:29:39.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_snippet.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      938 2016-10-13 20:25:30.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_wizard_properties_snippet.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       57 2014-01-16 21:50:41.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_handler_entry.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       61 2016-10-16 22:36:16.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/view_form_wizard_entry_ajax.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       56 2016-10-16 22:35:55.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/view_form_wizard_entry.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       63 2016-10-14 21:35:57.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/add_form_wizard_handler_entry.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     4220 2014-01-16 21:46:56.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/theme.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2014-01-16 21:47:37.000000 django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/add_form_element_entry.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-12-22 14:24:17.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_model_object/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      513 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_model_object/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      398 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_model_object/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1100 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_model_object/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2398 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_model_object/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3557 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_model_object/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      545 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_model_object/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      409 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_model_object/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      452 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      366 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1127 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4017 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3449 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      601 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      441 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/__init__.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1343 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/fields.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2588 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1826 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      513 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      394 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/textarea/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1921 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/textarea/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1447 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/textarea/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      495 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/textarea/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      376 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/textarea/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/integer/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2339 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/integer/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1831 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/integer/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      492 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/integer/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      373 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/integer/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      475 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date/widgets.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2222 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2380 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      523 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      404 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/ip_address/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2866 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/ip_address/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1607 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/ip_address/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      501 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/ip_address/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      382 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/ip_address/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/password/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2258 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/password/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1578 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/password/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      495 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/password/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      376 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/password/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      523 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      407 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1215 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2461 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3966 2016-10-24 22:31:25.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      616 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      456 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      364 2016-09-28 08:24:58.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/settings.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      305 2016-09-28 08:19:38.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/defaults.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1127 2016-09-28 08:19:19.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/conf.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2381 2016-09-28 08:23:34.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2841 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/fobi_form_elements.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      600 2016-09-28 08:18:17.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/apps.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      423 2016-09-28 08:17:43.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/input/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     5930 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/input/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1867 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/input/constants.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3018 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/input/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      486 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/input/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      367 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/input/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/regex/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3107 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/regex/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1627 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/regex/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      526 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/regex/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      407 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/regex/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slug/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2242 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slug/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1521 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slug/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      483 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slug/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      364 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slug/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/email/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2339 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/email/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1679 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/email/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      486 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/email/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      367 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/email/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/text/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2242 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/text/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1521 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/text/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      483 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/text/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      364 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/text/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      528 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      412 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1223 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2533 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4000 2016-10-24 22:41:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      631 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      471 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slider/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      455 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slider/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      340 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slider/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      512 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slider/widgets.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1028 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slider/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     7312 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slider/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1858 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slider/constants.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     5687 2016-10-24 23:29:05.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slider/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      489 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slider/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      370 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slider/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      518 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      417 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1135 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2419 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3577 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      601 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      441 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/float/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2325 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/float/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1781 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/float/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      486 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/float/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      367 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/float/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/radio/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      416 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/radio/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      330 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/radio/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      974 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/radio/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4070 2016-10-05 19:40:28.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/radio/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3050 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/radio/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      486 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/radio/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      367 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/radio/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/url/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2232 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/url/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1699 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/url/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      480 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/url/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      361 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/url/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      524 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      367 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1135 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3805 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3369 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      575 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      441 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/boolean/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1715 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/boolean/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1183 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/boolean/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      492 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/boolean/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      373 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/boolean/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      443 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      357 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1067 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3755 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3326 2016-10-24 22:38:08.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      516 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      397 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple/__init__.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-10-13 21:18:48.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/time/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2219 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/time/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2397 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/time/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      523 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/time/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      404 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/time/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1786 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1536 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      489 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      370 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/null_boolean/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1740 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/null_boolean/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1458 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/null_boolean/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      507 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/null_boolean/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      388 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/null_boolean/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      417 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      331 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1012 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3598 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3006 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      489 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      370 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/range_select/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      461 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/range_select/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      346 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/range_select/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1055 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/range_select/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3647 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/range_select/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1853 2016-10-24 23:29:30.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/range_select/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      507 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/range_select/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      388 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/range_select/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/decimal/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2793 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/decimal/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2152 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/decimal/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      532 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/decimal/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      413 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/decimal/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/datetime/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      491 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/datetime/widgets.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2256 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/datetime/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2458 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/datetime/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      535 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/datetime/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      416 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/datetime/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/file/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      364 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/file/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      309 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/file/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      969 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/file/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2006 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/file/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2586 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/file/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      483 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/file/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      364 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/file/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/honeypot/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      362 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/honeypot/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      272 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/honeypot/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      980 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/honeypot/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2291 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/honeypot/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1603 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/honeypot/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      501 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/honeypot/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      380 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/honeypot/__init__.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      878 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/honeypot/fields.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/recaptcha/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2339 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/recaptcha/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3853 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/recaptcha/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      504 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/recaptcha/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      383 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/recaptcha/__init__.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-12-01 22:10:29.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/captcha/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2284 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/captcha/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3730 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/captcha/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      498 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/captcha/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      377 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/captcha/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/test/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/test/dummy/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      437 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/test/dummy/widgets.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/test/dummy/static/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/test/dummy/static/dummy/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/test/dummy/static/dummy/js/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      202 2014-03-26 00:42:32.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/test/dummy/static/dummy/js/fobi.plugins.form_elements.dummy.js
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/test/dummy/static/dummy/css/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      202 2014-03-26 00:42:43.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/test/dummy/static/dummy/css/fobi.plugins.form_elements.dummy.css
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1284 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/test/dummy/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      480 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/test/dummy/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      363 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/test/dummy/__init__.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-11-08 22:49:39.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/test/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_text/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      776 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_text/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1364 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_text/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      510 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_text/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      390 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_text/__init__.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-12-26 10:44:00.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_video/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      484 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_video/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      454 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_video/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1036 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_video/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1307 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_video/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1487 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_video/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      513 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_video/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      393 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_video/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1888 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1954 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1024 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2059 2016-10-05 19:37:15.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3429 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/helpers.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2678 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/fobi_form_elements.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      513 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      393 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/templates/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/templates/content_image/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      539 2013-12-26 13:53:19.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/templates/content_image/render.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-08-16 17:45:03.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    10589 2016-10-16 21:35:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/fobi_form_handlers.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      377 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      315 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1165 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/widgets.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      946 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2029 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1540 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/helpers.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      502 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      364 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/templates/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/templates/mail/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      190 2015-04-25 21:23:12.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/templates/mail/plugin_data_repr.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1358 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/fields.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     7305 2016-10-19 22:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/fobi_form_handlers.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3698 2016-10-17 00:04:10.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/models.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      446 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      299 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/defaults.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/migrations/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1663 2016-10-15 23:35:40.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/migrations/0002_savedformwizarddataentry.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1772 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/migrations/0001_initial.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)        0 2016-05-12 20:03:09.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/migrations/__init__.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     6075 2016-10-25 18:37:30.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/views.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/urls/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2084 2016-10-12 20:46:18.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/urls/form_handlers.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2199 2016-10-12 20:46:29.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/urls/form_wizard_handlers.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      178 2016-10-12 09:12:58.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/urls/__init__.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      661 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/widgets.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/static/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/js/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     5417 2014-07-16 15:22:22.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/js/jquery.expander.min.js
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1193 2014-07-16 15:22:22.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/js/jquery.expander.license.txt
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      815 2014-08-08 20:40:45.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/js/db_store.js
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      967 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     5521 2016-10-25 18:37:07.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/helpers.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     5336 2016-10-25 18:45:54.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/admin.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      474 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      336 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/templates/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/templates/db_store/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2291 2016-10-12 09:25:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/templates/db_store/view_saved_form_wizard_data_entries.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     2228 2014-11-05 01:02:27.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/templates/db_store/view_saved_form_data_entries.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      178 2014-07-31 23:58:36.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/templates/db_store/plugin_data_repr.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-12-22 14:24:25.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/http_repost/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     6496 2016-10-17 01:09:51.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/http_repost/fobi_form_handlers.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      782 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/http_repost/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      483 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/http_repost/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      371 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/http_repost/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/http_repost/templates/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/http_repost/templates/http_repost/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      140 2014-06-18 23:19:41.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/http_repost/templates/http_repost/plugin_data_repr.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_importers/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_importers/mailchimp_importer/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2350 2016-10-24 20:37:52.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_importers/mailchimp_importer/views.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1370 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_importers/mailchimp_importer/forms.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2307 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_importers/mailchimp_importer/fobi_form_importers.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      507 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_importers/mailchimp_importer/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      385 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_importers/mailchimp_importer/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_importers/mailchimp_importer/templates/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_importers/mailchimp_importer/templates/mailchimp_importer/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       47 2016-10-09 20:11:58.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_importers/mailchimp_importer/templates/mailchimp_importer/1.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       47 2015-10-05 21:52:37.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_importers/mailchimp_importer/templates/mailchimp_importer/0.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-09-25 23:54:07.000000 django-fobi-0.9.8/src/fobi/contrib/plugins/form_importers/__init__.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-08-12 09:21:42.000000 django-fobi-0.9.8/src/fobi/contrib/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/apps/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2446 2016-09-26 21:03:37.000000 django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/models.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      993 2016-10-12 20:56:56.000000 django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      417 2016-10-12 20:56:33.000000 django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1000 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      999 2016-10-12 20:56:42.000000 django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/helpers.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      462 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      303 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/templates/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/templates/djangocms_integration/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      180 2014-11-18 23:29:06.000000 django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/templates/djangocms_integration/login_required.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)       58 2014-11-18 00:32:25.000000 django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/templates/djangocms_integration/widget.html
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1727 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/cms_plugins.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/apps/wagtail_integration_/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     3634 2016-09-28 08:54:07.000000 django-fobi-0.9.8/src/fobi/contrib/apps/wagtail_integration_/models.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)     1010 2016-09-28 08:54:19.000000 django-fobi-0.9.8/src/fobi/contrib/apps/wagtail_integration_/settings.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      425 2016-09-28 08:50:38.000000 django-fobi-0.9.8/src/fobi/contrib/apps/wagtail_integration_/defaults.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      995 2016-09-28 08:50:30.000000 django-fobi-0.9.8/src/fobi/contrib/apps/wagtail_integration_/conf.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      998 2016-09-28 08:51:18.000000 django-fobi-0.9.8/src/fobi/contrib/apps/wagtail_integration_/helpers.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      470 2016-09-28 08:50:05.000000 django-fobi-0.9.8/src/fobi/contrib/apps/wagtail_integration_/apps.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      313 2016-09-28 08:49:51.000000 django-fobi-0.9.8/src/fobi/contrib/apps/wagtail_integration_/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2636 2016-09-26 21:05:20.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/models.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1002 2016-10-12 20:58:08.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      417 2016-10-12 20:57:39.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1000 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1000 2016-10-12 20:57:48.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/helpers.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      359 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/admin.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      462 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      303 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/__init__.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1320 2016-10-12 20:58:00.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/page_processors.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/templates/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/templates/mezzanine_integration/
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/templates/mezzanine_integration/admin/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      539 2014-12-10 00:09:44.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/templates/mezzanine_integration/admin/change_form.html
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/templates/pages/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      630 2014-12-16 23:31:15.000000 django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/templates/pages/fobiformpage.html
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-09-28 11:50:14.000000 django-fobi-0.9.8/src/fobi/contrib/apps/__init__.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/contrib/apps/feincms_integration/
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-07-28 23:18:44.000000 django-fobi-0.9.8/src/fobi/contrib/apps/feincms_integration/models.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1000 2016-10-12 20:57:29.000000 django-fobi-0.9.8/src/fobi/contrib/apps/feincms_integration/settings.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      415 2016-10-12 20:57:10.000000 django-fobi-0.9.8/src/fobi/contrib/apps/feincms_integration/defaults.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3379 2016-09-26 21:04:30.000000 django-fobi-0.9.8/src/fobi/contrib/apps/feincms_integration/widgets.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      981 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/apps/feincms_integration/conf.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      994 2016-10-12 20:57:19.000000 django-fobi-0.9.8/src/fobi/contrib/apps/feincms_integration/helpers.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      456 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/apps/feincms_integration/apps.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      299 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/contrib/apps/feincms_integration/__init__.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2266 2016-10-12 20:39:47.000000 django-fobi-0.9.8/src/fobi/exceptions.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/fobi/templatetags/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    16767 2016-10-17 00:36:26.000000 django-fobi-0.9.8/src/fobi/templatetags/fobi_tags.py
--rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-08-12 09:21:42.000000 django-fobi-0.9.8/src/fobi/templatetags/__init__.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3862 2016-09-22 20:04:44.000000 django-fobi-0.9.8/src/fobi/templatetags/future_compat.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2891 2016-09-22 20:04:54.000000 django-fobi-0.9.8/src/fobi/discover.py
-drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/django_fobi.egg-info/
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)        1 2016-10-27 21:06:49.000000 django-fobi-0.9.8/src/django_fobi.egg-info/dependency_links.txt
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      219 2016-10-27 21:06:49.000000 django-fobi-0.9.8/src/django_fobi.egg-info/requires.txt
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    88708 2016-10-27 21:07:01.000000 django-fobi-0.9.8/src/django_fobi.egg-info/SOURCES.txt
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)        5 2016-10-27 21:06:49.000000 django-fobi-0.9.8/src/django_fobi.egg-info/top_level.txt
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)   101817 2016-10-27 21:06:49.000000 django-fobi-0.9.8/src/django_fobi.egg-info/PKG-INFO
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2899 2016-10-24 20:37:52.000000 django-fobi-0.9.8/MANIFEST.in
--rw-------   0 foreverchild  (1000) foreverchild  (1000)      740 2016-10-27 21:07:01.000000 django-fobi-0.9.8/setup.cfg
--rw-------   0 foreverchild  (1000) foreverchild  (1000)    18097 2016-10-17 01:10:54.000000 django-fobi-0.9.8/LICENSE_GPL2.0.txt
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    78289 2016-10-26 22:55:29.000000 django-fobi-0.9.8/README.rst
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    10445 2016-10-27 20:31:18.000000 django-fobi-0.9.8/setup.py
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    34990 2016-10-27 20:31:09.000000 django-fobi-0.9.8/CHANGELOG.rst
--rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)   101817 2016-10-27 21:07:01.000000 django-fobi-0.9.8/PKG-INFO
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    26535 2016-10-17 01:11:03.000000 django-fobi-0.9.9/LICENSE_LGPL_2.1.txt
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     7858 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/dynamic.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1048 2016-10-12 20:25:10.000000 django-fobi-0.9.9/src/fobi/context_processors.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/integration/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-12-26 00:27:09.000000 django-fobi-0.9.9/src/fobi/integration/models.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    10825 2016-10-25 19:56:48.000000 django-fobi-0.9.9/src/fobi/integration/processors.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1321 2016-10-12 20:33:21.000000 django-fobi-0.9.9/src/fobi/integration/helpers.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-12-25 14:45:47.000000 django-fobi-0.9.9/src/fobi/integration/__init__.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    22087 2016-10-16 21:50:28.000000 django-fobi-0.9.9/src/fobi/models.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     5535 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     5360 2016-10-12 20:26:43.000000 django-fobi-0.9.9/src/fobi/form_importers.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4579 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/defaults.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/migrations/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1491 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/migrations/0010_formwizardhandler.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      707 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/migrations/0006_auto_20160911_1549.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      707 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/migrations/0005_auto_20160908_1457.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3260 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/migrations/0004_auto_20160906_1513.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    10070 2016-09-28 08:55:07.000000 django-fobi-0.9.9/src/fobi/migrations/0001_initial.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      647 2016-10-05 22:04:25.000000 django-fobi-0.9.9/src/fobi/migrations/0009_formwizardentry_wizard_type.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-09-12 22:38:11.000000 django-fobi-0.9.9/src/fobi/migrations/__init__.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2809 2016-10-16 21:53:41.000000 django-fobi-0.9.9/src/fobi/migrations/0007_auto_20160926_1652.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1121 2016-09-27 22:56:31.000000 django-fobi-0.9.9/src/fobi/migrations/0008_formwizardhandlerentry.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      627 2015-09-12 22:44:00.000000 django-fobi-0.9.9/src/fobi/migrations/0002_auto_20150912_1744.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2787 2016-05-19 23:04:44.000000 django-fobi-0.9.9/src/fobi/migrations/0003_auto_20160517_1005.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    98229 2016-10-30 23:36:39.000000 django-fobi-0.9.9/src/fobi/views.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/tests/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     8891 2016-09-28 08:32:39.000000 django-fobi-0.9.9/src/fobi/tests/data.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2144 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/tests/base.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1280 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/tests/test_dynamic_forms.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     5653 2016-09-28 08:48:14.000000 django-fobi-0.9.9/src/fobi/tests/test_form_importers_mailchimp.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      416 2016-09-28 08:31:03.000000 django-fobi-0.9.9/src/fobi/tests/constants.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     9380 2016-09-28 08:46:22.000000 django-fobi-0.9.9/src/fobi/tests/helpers.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    26237 2016-10-25 21:08:32.000000 django-fobi-0.9.9/src/fobi/tests/test_browser_build_dynamic_forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      456 2016-09-28 08:39:38.000000 django-fobi-0.9.9/src/fobi/tests/__init__.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4210 2016-09-28 08:26:11.000000 django-fobi-0.9.9/src/fobi/tests/test_core.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1804 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/tests/test_sortable_dict.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    27561 2016-10-26 21:55:10.000000 django-fobi-0.9.9/src/fobi/utils.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/urls/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1919 2016-10-12 21:26:54.000000 django-fobi-0.9.9/src/fobi/urls/view.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-09-24 00:00:28.000000 django-fobi-0.9.9/src/fobi/urls/__init__.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     7467 2016-10-26 21:30:21.000000 django-fobi-0.9.9/src/fobi/urls/edit.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      434 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/test.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/management/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-08-12 09:21:42.000000 django-fobi-0.9.9/src/fobi/management/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/management/commands/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2152 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/management/commands/fobi_find_broken_entries.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1007 2016-10-12 21:48:00.000000 django-fobi-0.9.9/src/fobi/management/commands/fobi_update_plugin_data.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      460 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/management/commands/fobi_sync_plugins.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-08-12 09:21:42.000000 django-fobi-0.9.9/src/fobi/management/commands/__init__.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      754 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/management/commands/fobi_migrate_03_to_04.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2814 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/widgets.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/js/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)   348978 2015-04-20 21:48:52.000000 django-fobi-0.9.9/src/fobi/static/js/moment-with-locales.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2976 2014-09-14 00:52:06.000000 django-fobi-0.9.9/src/fobi/static/js/fobi.core.js
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    12171 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/static/js/jquery.slugify.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    93107 2013-08-21 20:57:03.000000 django-fobi-0.9.9/src/fobi/static/js/jquery-1.10.2.min.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1521 2014-01-10 17:28:07.000000 django-fobi-0.9.9/src/fobi/static/js/jquery.slugify.license.txt
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1098 2014-01-10 17:31:08.000000 django-fobi-0.9.9/src/fobi/static/js/jquery.license.txt
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/js/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)   228539 2014-09-16 18:45:26.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/js/jquery-ui-1.10.4.custom.min.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)   436715 2014-09-16 18:45:26.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/js/jquery-ui-1.10.4.custom.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1335 2014-01-10 17:31:57.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/jquery-ui.license.txt
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    31438 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/index.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      212 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      335 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      262 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4549 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      262 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4549 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      332 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     6999 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_888888_256x240.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1738 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/animated-overlay.gif
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      280 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     6922 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_222222_256x240.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      208 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_flat_75_ffffff_40x100.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     6992 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_454545_256x240.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      207 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    32046 2013-08-31 05:16:52.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/jquery-ui-1.10.3.custom.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    26939 2013-08-31 05:16:54.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/jquery-ui-1.10.3.custom.min.css
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      212 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     6299 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_ffffff_256x240.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      335 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      262 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_glass_75_dadada_1x400.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4549 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_cd0a0a_256x240.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      208 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_flat_100_ffffff_40x100.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4549 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_bbbbcc_256x240.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      262 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      212 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_flat_30_aaaaaa_40x100.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4549 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_2e83ff_256x240.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      332 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     6999 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_888888_256x240.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      331 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_highlight-hard_75_7ca0c7_1x100.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1738 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/animated-overlay.gif
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     6992 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_454545_256x240.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      342 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-bg_highlight-soft_75_7ca0c7_1x100.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    32365 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/jquery-ui-1.10.4.custom.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    27438 2014-09-19 13:42:24.000000 django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/jquery-ui-1.10.4.custom.min.css
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/css/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2786 2013-11-23 09:43:41.000000 django-fobi-0.9.9/src/fobi/static/css/admin_custom.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1286 2014-07-12 22:23:57.000000 django-fobi-0.9.9/src/fobi/static/css/fobi.core.css
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/less/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      742 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/less/path.less
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    17555 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/less/icons.less
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2084 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/less/bootstrap.less
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2101 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/less/core.less
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    19299 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/less/font-awesome-ie7.less
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1319 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/less/font-awesome.less
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     8888 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/less/variables.less
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1041 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/less/mixins.less
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2398 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/less/extras.less
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/css/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    22084 2013-06-26 15:40:33.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/css/font-awesome.min.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    41311 2013-06-26 15:40:33.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/css/font-awesome-ie7.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    37782 2013-06-26 15:40:33.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/css/font-awesome-ie7.min.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    27232 2013-06-26 15:40:33.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/css/font-awesome.css
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/scss/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1284 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/scss/font-awesome.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    17555 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/scss/_icons.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2157 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/scss/_core.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1078 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/scss/_mixins.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    22328 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/scss/font-awesome-ie7.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2088 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/scss/_bootstrap.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     8061 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/scss/_variables.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2406 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/scss/_extras.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      753 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/scss/_path.scss
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/font/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    37405 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/font/fontawesome-webfont.eot
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    79076 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/font/fontawesome-webfont.ttf
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4060 2014-01-10 17:36:01.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/font/license.txt
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    43572 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/font/fontawesome-webfont.woff
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)   197829 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/font/fontawesome-webfont.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    61896 2013-06-26 15:40:32.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/font/FontAwesome.otf
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1078 2014-01-10 17:35:14.000000 django-fobi-0.9.9/src/fobi/static/font-awesome/code.license.txt
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/colorbox/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/static/colorbox/images/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     9427 2013-07-22 06:23:09.000000 django-fobi-0.9.9/src/fobi/static/colorbox/images/loading.gif
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      112 2013-07-22 06:23:09.000000 django-fobi-0.9.9/src/fobi/static/colorbox/images/border.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      157 2013-07-22 06:23:09.000000 django-fobi-0.9.9/src/fobi/static/colorbox/images/loading_background.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      182 2013-07-22 06:23:09.000000 django-fobi-0.9.9/src/fobi/static/colorbox/images/overlay.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2893 2013-07-22 06:23:09.000000 django-fobi-0.9.9/src/fobi/static/colorbox/images/controls.png
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    10894 2013-07-22 06:23:09.000000 django-fobi-0.9.9/src/fobi/static/colorbox/jquery.colorbox-min.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     5552 2013-07-22 06:23:09.000000 django-fobi-0.9.9/src/fobi/static/colorbox/index.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4340 2013-07-22 06:23:09.000000 django-fobi-0.9.9/src/fobi/static/colorbox/colorbox.css
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)   102372 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/base.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      825 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/conf.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/south_migrations/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    17332 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/south_migrations/0003_auto__add_formwizardformentry__add_unique_formwizardformentry_form_wiz.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    18066 2016-09-28 08:56:07.000000 django-fobi-0.9.9/src/fobi/south_migrations/0001_initial.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-09-12 22:59:16.000000 django-fobi-0.9.9/src/fobi/south_migrations/__init__.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     9648 2016-09-28 08:56:41.000000 django-fobi-0.9.9/src/fobi/south_migrations/0002_auto__add_field_formentry_created__add_field_formentry_updated.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    16183 2016-10-26 20:50:21.000000 django-fobi-0.9.9/src/fobi/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1650 2016-10-12 20:25:00.000000 django-fobi-0.9.9/src/fobi/constants.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    28801 2016-10-30 22:36:58.000000 django-fobi-0.9.9/src/fobi/helpers.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/locale/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/locale/nl/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    67718 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/locale/nl/LC_MESSAGES/django.po
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    20358 2015-09-01 21:33:55.000000 django-fobi-0.9.9/src/fobi/locale/nl/LC_MESSAGES/django.mo
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/locale/de/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    67245 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/locale/de/LC_MESSAGES/django.po
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    19060 2015-05-21 20:55:50.000000 django-fobi-0.9.9/src/fobi/locale/de/LC_MESSAGES/django.mo
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/locale/ru/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    73378 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/locale/ru/LC_MESSAGES/django.po
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    26568 2015-09-01 20:46:56.000000 django-fobi-0.9.9/src/fobi/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      320 2016-10-12 20:24:37.000000 django-fobi-0.9.9/src/fobi/compat.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/wizard/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       21 2016-10-09 19:25:24.000000 django-fobi-0.9.9/src/fobi/wizard/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/wizard/views/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    32774 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/wizard/views/dynamic.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2670 2016-10-12 08:21:29.000000 django-fobi-0.9.9/src/fobi/wizard/views/views.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       44 2016-10-09 19:50:24.000000 django-fobi-0.9.9/src/fobi/wizard/views/__init__.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      752 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/app.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     8147 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/data_structures.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3913 2016-10-12 20:25:24.000000 django-fobi-0.9.9/src/fobi/decorators.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    20455 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/admin.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      342 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      249 2016-10-30 23:44:26.000000 django-fobi-0.9.9/src/fobi/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/templates/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/templates/fobi/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/templates/fobi/integration/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      180 2014-12-25 15:34:14.000000 django-fobi-0.9.9/src/fobi/templates/fobi/integration/login_required.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      832 2016-10-26 22:23:19.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/view_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      648 2016-10-26 22:20:32.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/form_entry_submitted.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    11137 2016-10-26 22:17:29.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/edit_form_wizard_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      215 2015-08-26 20:42:27.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/import_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      310 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/add_form_handler_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      388 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/edit_form_element_entry_ajax.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      219 2016-09-27 20:51:04.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/create_form_wizard_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      212 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/create_form_entry_ajax.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3783 2016-10-26 21:47:11.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/form_wizards_dashboard.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      640 2016-10-26 22:20:40.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/form_importer.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3421 2016-10-26 09:32:40.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/dashboard.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     8519 2016-10-26 09:34:31.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/_base.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      314 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/edit_form_handler_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      216 2014-10-25 20:10:36.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/embed_form_entry_submitted_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      223 2015-09-25 23:25:31.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/form_importer_ajax.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1586 2016-10-26 22:23:57.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/edit_form_wizard_entry.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      331 2016-10-14 21:35:11.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/add_form_wizard_handler_entry_ajax.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      835 2016-10-26 22:24:11.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/create_form_wizard_entry.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1701 2015-12-21 23:09:23.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/forms_list.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      371 2014-10-24 23:38:47.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/view_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1307 2016-10-26 22:20:17.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/edit_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      703 2014-10-25 20:14:39.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/form_entry_submitted_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     9171 2016-10-04 21:23:15.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/edit_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      203 2014-10-24 23:42:05.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/view_embed_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      648 2016-10-26 22:19:49.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/create_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      384 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/add_form_element_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      215 2014-03-26 23:50:46.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/base.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      744 2016-10-26 22:20:00.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/add_form_handler_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      875 2016-10-28 23:49:08.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/edit_form_element_entry.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1356 2016-10-17 00:55:46.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_wizard_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      947 2014-08-14 22:08:03.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_edit_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1191 2016-10-17 00:38:56.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_view_ajax.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1291 2016-10-17 01:22:50.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_wizard_view_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3478 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_properties_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1170 2014-10-24 23:41:45.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      229 2014-03-27 00:10:11.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/messages_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       86 2014-12-02 23:33:06.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_non_field_and_hidden_errors_snippet.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4235 2016-10-16 22:24:36.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_wizard_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2238 2015-10-05 21:51:48.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_wizard.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4209 2016-10-28 23:31:01.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_snippet.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3478 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_wizard_properties_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      746 2016-10-26 22:20:24.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/edit_form_handler_entry.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1157 2016-10-17 01:24:55.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/view_form_wizard_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      648 2016-10-26 22:23:06.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/import_form_entry.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1047 2016-10-26 22:27:25.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/view_form_wizard_entry.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      738 2016-10-17 00:21:43.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/form_wizard_entry_submitted_ajax.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      765 2016-10-26 22:24:16.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/add_form_wizard_handler_entry.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      663 2016-10-26 22:23:49.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/form_wizard_entry_submitted.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4220 2013-12-26 16:34:28.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/theme.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      744 2016-10-26 22:19:42.000000 django-fobi-0.9.9/src/fobi/templates/fobi/generic/add_form_element_entry.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/templates/fobi/admin/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3834 2013-12-22 16:17:35.000000 django-fobi-0.9.9/src/fobi/templates/fobi/admin/bulk_change_plugins.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1034 2016-10-12 20:26:57.000000 django-fobi-0.9.9/src/fobi/form_utils.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1172 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/validators.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/db_store/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/db_store/models.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      829 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/db_store/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      645 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/db_store/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      424 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/db_store/__init__.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/js/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1789 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/js/fobi.djangocms_admin_style_theme.edit.js
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/css/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1286 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/css/fobi.djangocms_admin_style_theme.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4239 2016-10-04 21:21:18.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/css/fobi.djangocms_admin_style_theme.edit.css
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/admin/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/admin/img/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      932 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/admin/img/tooltag-add.gif
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      197 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/admin/img/tool-left.gif
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      336 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/admin/img/tooltag-add_over.gif
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     6862 2016-10-04 22:19:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/fobi_themes.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      486 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      389 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       49 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/view_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/form_entry_submitted.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2015-08-27 21:03:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/import_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/add_form_handler_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/edit_form_element_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/create_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3811 2015-12-16 01:49:29.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/dashboard.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       95 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/_base.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/edit_form_handler_entry_ajax.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2069 2015-12-21 23:10:38.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/forms_list.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/view_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      225 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/edit_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       59 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/form_entry_submitted_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     7989 2016-10-04 21:22:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/edit_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      175 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/create_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/add_form_element_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/base.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     6512 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/base_edit.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      507 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/add_form_handler_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      502 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/edit_form_element_entry.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      946 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_edit_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       57 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_view_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1752 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_properties_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      393 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       59 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/messages_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1466 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_edit_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2189 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      502 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/edit_form_handler_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      227 2015-08-27 21:03:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/import_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3193 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/base_view.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4220 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/theme.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      506 2015-02-10 23:12:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/add_form_element_entry.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/widgets/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-11-07 23:26:00.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/widgets/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/widgets/form_handlers/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/widgets/form_handlers/db_store/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-11-07 23:26:00.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/widgets/form_handlers/db_store/models.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      766 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/widgets/form_handlers/db_store/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      516 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/widgets/form_handlers/db_store/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      365 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/widgets/form_handlers/db_store/__init__.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-11-07 23:26:00.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/widgets/form_handlers/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/simple/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/simple/js/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1789 2014-09-23 23:49:06.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/simple/js/fobi.simple.edit.js
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/simple/css/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2984 2016-10-04 21:21:28.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/simple/css/fobi.simple.edit.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1242 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/simple/css/fobi.simple.css
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/admin/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/admin/img/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      932 2014-12-26 00:18:40.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/admin/img/tooltag-add.gif
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      197 2014-12-26 00:18:40.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/admin/img/tool-left.gif
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      336 2014-12-26 00:18:40.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/admin/img/tooltag-add_over.gif
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4266 2016-10-04 22:21:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/fobi_themes.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      423 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      300 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       49 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/view_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/form_entry_submitted.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2015-08-27 21:03:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/import_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/add_form_handler_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/edit_form_element_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2014-09-22 22:32:40.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/create_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3690 2015-12-16 01:49:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/dashboard.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       74 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/_base.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/edit_form_handler_entry_ajax.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2056 2015-12-21 23:10:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/forms_list.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/view_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      225 2014-09-23 01:29:25.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/edit_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       59 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/form_entry_submitted_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     7957 2016-10-04 21:23:02.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/edit_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      175 2014-09-25 22:08:26.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/create_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/add_form_element_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       33 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/base.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     5858 2014-10-11 21:13:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/base_edit.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      507 2014-09-25 22:08:26.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/add_form_handler_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      502 2014-09-25 22:08:26.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/edit_form_element_entry.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/snippets/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      946 2014-09-22 22:43:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/snippets/form_edit_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       57 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/snippets/form_view_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1752 2014-10-07 23:14:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/snippets/form_properties_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      393 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/snippets/form_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       59 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/snippets/messages_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1466 2014-10-07 23:14:21.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/snippets/form_edit_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2189 2014-12-04 01:26:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/snippets/form_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      502 2014-09-25 22:08:26.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/edit_form_handler_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      228 2015-08-27 21:03:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/import_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3193 2014-10-11 21:14:05.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/base_view.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4220 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/theme.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      506 2014-09-25 22:08:26.000000 django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/add_form_element_entry.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/static/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/static/foundation5/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/static/foundation5/js/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      358 2015-04-26 01:41:13.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/static/foundation5/js/fobi.plugin.date-foundation5-widget.js
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1027 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      634 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      422 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/static/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/static/foundation5/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/static/foundation5/js/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      377 2015-04-26 01:41:39.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/static/foundation5/js/fobi.plugin.datetime-foundation5-widget.js
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1075 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      646 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      430 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/__init__.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-04-25 21:34:17.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/dummy_foundation5_widget/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      892 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/dummy_foundation5_widget/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      637 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/dummy_foundation5_widget/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      424 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/dummy_foundation5_widget/__init__.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-11-07 23:08:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_handlers/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-11-07 23:24:49.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/models.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      939 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      646 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      430 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/templates/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/templates/db_store_foundation5_widget/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2205 2014-11-08 22:35:49.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/templates/db_store_foundation5_widget/view_saved_form_data_entries.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      178 2014-11-08 21:41:59.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/templates/db_store_foundation5_widget/plugin_data_repr.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-11-07 23:09:02.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_handlers/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/img/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        1 2014-08-21 21:50:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/img/.gitkeep
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    89082 2014-06-01 21:26:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation_template-4.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    95120 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation.min.js
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     8271 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/fastclick.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    11262 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/modernizr.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1415 2014-08-21 21:50:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/jquery.cookie.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    84621 2014-08-21 21:50:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/jquery.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2330 2014-08-21 21:50:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/placeholder.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    37736 2015-04-25 21:44:18.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation-datepicker.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1712 2014-09-14 00:38:39.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation5_fobi_extras.js
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    15318 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.orbit.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     7957 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.slider.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2100 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.equalizer.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    14068 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.reveal.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    11070 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.abide.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    14543 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.topbar.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1237 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.alert.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    29980 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.joyride.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     9922 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.dropdown.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     7057 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.magellan.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    10487 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.tooltip.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    18425 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    16859 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.clearing.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     5085 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.offcanvas.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     6401 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.tab.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2144 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.accordion.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     9228 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.interchange.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    54154 2015-04-25 23:05:35.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation-datetimepicker.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      106 2014-08-21 21:50:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/robots.txt
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/sass/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1303 2012-08-10 06:06:00.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/sass/accessibility_foundicons.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1032 2012-08-10 15:14:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/sass/accessibility_foundicons_ie7.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      775 2012-08-10 06:06:03.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/sass/_settings.scss
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/stylesheets/
+-rwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)     2196 2015-10-23 23:38:38.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/stylesheets/accessibility_foundicons.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2920 2012-08-10 15:15:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/stylesheets/accessibility_foundicons_ie7.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     5508 2012-08-10 14:47:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/demo.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    15316 2012-08-10 08:07:26.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.eot
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     9188 2012-08-10 08:07:26.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.woff
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    15056 2012-08-10 08:07:26.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.ttf
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      628 2012-08-10 08:07:28.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.svg
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/0e61251fcc72078e76f7711e6e025bea2a2f1ce3/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4166 2012-08-10 06:06:01.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/0e61251fcc72078e76f7711e6e025bea2a2f1ce3/_settings.scssc
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     5690 2012-08-10 06:06:01.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/0e61251fcc72078e76f7711e6e025bea2a2f1ce3/accessibility_foundicons.scssc
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4526 2012-08-10 15:15:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/0e61251fcc72078e76f7711e6e025bea2a2f1ce3/accessibility_foundicons_ie7.scssc
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/sass/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1954 2012-08-10 14:40:25.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/sass/general_foundicons.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      763 2012-08-10 14:28:35.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/sass/_settings.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1704 2012-08-10 14:43:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/sass/general_foundicons_ie7.scss
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/stylesheets/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3177 2012-08-10 14:40:25.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/stylesheets/general_foundicons.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     5119 2012-08-10 14:43:45.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/stylesheets/general_foundicons_ie7.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     7812 2012-08-10 14:47:38.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/demo.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    15488 2012-08-10 08:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.ttf
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      616 2012-08-10 08:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     9728 2012-08-10 08:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.woff
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    15724 2012-08-10 08:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.eot
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4142 2012-08-10 14:25:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/_settings.scssc
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     8399 2012-08-10 14:40:25.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/general_foundicons.scssc
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     7277 2012-08-10 14:43:45.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/general_foundicons_ie7.scssc
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     5688 2012-08-10 14:24:32.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/accessibility_foundicons.scssc
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4524 2012-08-10 14:24:32.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/accessibility_foundicons_ie7.scssc
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/sass/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1704 2012-08-10 15:17:14.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/sass/general_enclosed_foundicons_ie7.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1954 2012-08-10 14:46:17.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/sass/general_enclosed_foundicons.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      780 2012-08-10 14:46:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/sass/_settings.scss
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/stylesheets/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     5127 2012-08-10 15:17:19.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/stylesheets/general_enclosed_foundicons_ie7.css
+-rwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)     3246 2015-10-23 23:38:38.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/stylesheets/general_enclosed_foundicons.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     7879 2012-08-10 15:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/demo.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    18912 2012-08-10 08:07:40.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.eot
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      633 2012-08-10 08:07:40.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    18640 2012-08-10 08:07:40.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.ttf
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     9536 2012-08-10 08:07:40.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.woff
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/1ea694b23cbc52b68bcbd397d07df10b08a18c32/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4176 2012-08-10 14:44:32.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/1ea694b23cbc52b68bcbd397d07df10b08a18c32/_settings.scssc
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     8399 2012-08-10 14:46:18.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/1ea694b23cbc52b68bcbd397d07df10b08a18c32/general_enclosed_foundicons.scssc
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     7277 2012-08-10 15:17:19.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/1ea694b23cbc52b68bcbd397d07df10b08a18c32/general_enclosed_foundicons_ie7.scssc
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/sass/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1179 2012-08-10 14:54:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/sass/social_foundicons_ie7.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1447 2012-08-10 14:54:25.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/sass/social_foundicons.scss
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      761 2012-08-10 14:49:50.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/sass/_settings.scss
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/stylesheets/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3352 2012-08-10 14:54:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/stylesheets/social_foundicons_ie7.css
+-rwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)     2355 2015-10-23 23:38:38.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/stylesheets/social_foundicons.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     5786 2012-08-10 15:09:12.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/demo.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    17112 2012-08-10 08:07:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.eot
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    10644 2012-08-10 08:07:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.woff
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    16880 2012-08-10 08:07:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.ttf
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      614 2012-08-10 08:07:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.svg
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/0bd576c1f1487db9a103f544ad85fa8a0f88a6ea/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4138 2012-08-10 14:49:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/0bd576c1f1487db9a103f544ad85fa8a0f88a6ea/_settings.scssc
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     6245 2012-08-10 14:54:17.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/0bd576c1f1487db9a103f544ad85fa8a0f88a6ea/social_foundicons.scssc
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     5088 2012-08-10 14:54:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/0bd576c1f1487db9a103f544ad85fa8a0f88a6ea/social_foundicons_ie7.scssc
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    32020 2013-08-23 16:25:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.woff
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)   324210 2013-08-23 16:59:19.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/preview.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2086 2013-08-23 02:50:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-trees.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1822 2013-08-23 02:50:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-steam.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1105 2013-08-23 03:07:46.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-layout.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1743 2013-08-23 03:21:32.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-zoom-in.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1928 2013-08-23 03:07:45.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-burst.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2879 2013-08-23 02:50:56.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-male-female.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2561 2013-08-23 03:21:32.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-calendar.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2171 2013-08-23 03:07:45.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-euro.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1384 2013-08-23 03:21:34.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-trend.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      756 2013-08-23 03:21:35.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-contrast.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1227 2013-08-23 03:21:31.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-upload.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1394 2013-08-23 02:50:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-trophy.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1273 2013-08-23 03:21:37.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-remove.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      827 2013-08-23 03:21:31.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-home.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1285 2013-08-23 03:03:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-xbox.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      835 2013-08-23 03:07:43.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-play.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2200 2013-08-23 02:50:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-no-dogs.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1537 2013-08-23 02:50:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-sheriff-badge.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      881 2013-08-23 03:21:34.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pencil.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1326 2013-08-23 03:07:46.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-price-tag.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1762 2013-08-23 02:50:56.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-wheelchair.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1352 2013-08-23 03:21:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-address-book.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      904 2013-08-23 03:07:41.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mobile.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4724 2013-08-23 03:21:36.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-sound.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1105 2013-08-23 03:07:41.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-usb.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      986 2013-08-23 03:07:45.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-credit-card.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1194 2013-08-23 03:21:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-annotate.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1345 2013-08-23 03:21:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torso-female.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1041 2013-08-23 03:21:31.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-star.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1396 2013-08-23 03:21:36.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-microphone.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1388 2013-08-23 02:50:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-stumbleupon.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1122 2013-08-23 02:50:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-foot.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1951 2013-08-23 03:21:34.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-database.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1369 2013-08-23 03:07:42.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-left.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1697 2013-08-23 02:50:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-six.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2013 2013-08-23 02:50:56.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-universal-access.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2421 2013-08-23 03:07:45.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-burst-new.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      681 2013-08-23 03:21:31.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-minus.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1140 2013-08-23 03:07:41.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-underline.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1356 2013-08-23 03:07:46.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-web.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1494 2013-08-23 03:21:32.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paperclip.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1219 2013-08-23 03:07:45.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-eject.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1307 2013-08-23 03:07:45.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shopping-cart.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1670 2013-08-23 03:21:37.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-csv.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1357 2013-08-23 03:21:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-folder-add.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2020 2013-08-23 03:07:42.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list-number.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1817 2013-08-23 02:50:56.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-blind.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      935 2013-08-23 03:07:46.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-html5.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2616 2013-08-23 03:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-google-plus.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1714 2013-08-23 03:21:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-male-female.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1718 2013-08-23 02:50:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-at-sign.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      835 2013-08-23 03:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-forrst.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1453 2013-08-23 03:21:36.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2487 2013-08-23 02:50:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-treehouse.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1897 2013-08-23 02:50:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-yelp.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      598 2013-08-23 03:07:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-delicious.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      869 2013-08-23 03:21:32.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-cloud.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      953 2013-08-23 03:07:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-dropbox.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1141 2013-08-23 02:50:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-safety-cone.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1069 2013-08-23 02:50:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-two.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1409 2013-08-23 02:50:56.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-male.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1504 2013-08-23 03:07:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-blogger.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1164 2013-08-23 03:21:36.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comments.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1190 2013-08-23 03:21:34.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-eye.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1811 2013-08-23 03:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-hi5.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2076 2013-08-23 02:50:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-skull.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1107 2013-08-23 02:50:50.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-rdio.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      950 2013-08-23 02:50:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-prohibited.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      713 2013-08-23 03:21:35.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-video.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1801 2013-08-23 03:07:46.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pricetag-multiple.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1644 2013-08-23 03:07:43.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-indent-more.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1568 2013-08-23 03:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-game-center.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1425 2013-08-23 03:21:35.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-alert.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     5365 2013-08-23 02:50:56.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-asl.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      959 2013-08-23 03:07:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-volume-none.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1052 2013-08-23 03:07:43.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-filter.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      883 2013-08-23 03:07:41.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-italic.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2065 2013-08-23 03:07:42.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-strikethrough.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3053 2013-08-23 02:50:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-skillshare.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2134 2013-08-23 02:50:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-spotify.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1411 2013-08-23 02:50:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clipboard.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1795 2013-08-23 02:50:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-power.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2862 2013-08-23 03:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-joomla.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1028 2013-08-23 03:21:32.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-magnifying-glass.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2398 2013-08-23 03:07:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-volume.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      911 2013-08-23 03:07:43.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-stop.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1564 2013-08-23 03:21:36.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bluetooth.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3133 2013-08-23 03:07:46.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-dollar-bill.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1041 2013-08-23 03:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-medium.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2325 2013-08-23 03:09:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mobile-signal.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1233 2013-08-23 03:21:32.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-zoom-out.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1318 2013-08-23 03:21:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-folder-lock.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1258 2013-08-23 03:21:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clock.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      984 2013-08-23 03:07:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-fast-forward.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2950 2013-08-23 02:50:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-lightbulb.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1073 2013-08-23 03:21:35.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-camera.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1052 2013-08-23 03:21:34.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-minus-circle.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1644 2013-08-23 03:07:42.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-indent-less.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1195 2013-08-23 02:50:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-compass.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      976 2013-08-23 03:07:41.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bold.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1178 2013-08-23 02:50:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-tumblr.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2334 2013-08-23 03:21:37.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export-doc.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2827 2013-08-23 02:50:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-squidoo.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1130 2013-08-23 03:21:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-share.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1448 2013-08-23 03:21:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      922 2013-08-23 03:21:29.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-right.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1758 2013-08-23 03:07:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-deviant-art.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1467 2013-08-23 03:21:37.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-edit.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1431 2013-08-23 03:21:29.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-expand.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1187 2013-08-23 02:50:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-target.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1455 2013-08-23 03:21:34.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-x-circle.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1693 2013-08-23 03:07:45.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-dollar.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1238 2013-08-23 03:21:35.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-telephone.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1975 2013-08-23 02:50:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-no-smoking.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1435 2013-08-23 03:21:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-compress.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1192 2013-08-23 03:07:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-play-circle.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1436 2013-08-23 02:50:50.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-pinterest.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1051 2013-08-23 03:21:31.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-marker.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1915 2013-08-23 02:50:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-vimeo.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1231 2013-08-23 03:21:31.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-download.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1314 2013-08-23 03:07:42.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-text-color.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1504 2013-08-23 03:21:37.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-search.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1135 2013-08-23 03:07:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-bing.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      937 2013-08-23 02:50:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-battery-full.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1094 2013-08-23 03:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-linkedin.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1237 2013-08-23 03:07:41.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-laptop.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1430 2013-08-23 03:21:37.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-add.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1645 2013-08-23 03:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-instagram.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3487 2013-08-23 02:50:56.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-elevator.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1925 2013-08-23 02:50:56.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-female.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1836 2013-08-23 02:50:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-snapchat.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1712 2013-08-23 02:50:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-map.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1158 2013-08-23 03:21:34.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-horizontal.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1883 2013-08-23 02:50:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-yahoo.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1533 2013-08-23 02:50:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-five.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1055 2013-08-23 03:21:31.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-plus.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1390 2013-08-23 03:07:42.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-right.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1334 2013-08-23 03:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-lastfm.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1821 2013-08-23 02:50:50.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-reddit.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1224 2013-08-23 02:50:56.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-male-symbol.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2323 2013-08-23 03:07:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-android.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      760 2013-08-23 02:50:56.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-braille.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1520 2013-08-23 03:21:32.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-wrench.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1674 2013-08-23 03:21:37.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-doc.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1796 2013-08-23 02:50:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-anchor.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3511 2013-08-23 03:07:43.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-unlink.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      929 2013-08-23 03:07:46.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-css3.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1423 2013-08-23 02:50:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-key.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2253 2013-08-23 03:07:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-evernote.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2960 2013-08-23 03:21:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-thumbnails.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1212 2013-08-23 03:07:43.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-photo.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      995 2013-08-23 03:21:32.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-unlock.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      921 2013-08-23 03:21:29.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-up.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1818 2013-08-23 02:50:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-crown.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1969 2013-08-23 03:07:42.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-superscript.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1042 2013-08-23 03:21:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torso.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1101 2013-08-23 02:50:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-zurb.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1352 2013-08-23 03:21:35.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-upload-cloud.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1865 2013-08-23 02:50:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-asterisk.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1749 2013-08-23 02:50:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-first-aid.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1814 2013-08-23 03:07:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-dribbble.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2306 2013-08-23 03:21:37.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export-csv.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1218 2013-08-23 03:21:31.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-refresh.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1132 2013-08-23 03:21:38.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-multiple.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1515 2013-08-23 03:21:35.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-dislike.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      984 2013-08-23 03:07:42.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-background-color.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      849 2013-08-23 03:07:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-record.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1325 2013-08-23 03:07:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-next.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2354 2013-08-23 03:21:29.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-out.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1285 2013-08-23 02:50:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-twitter.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      814 2013-08-23 03:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-hacker-news.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2226 2013-08-23 02:50:56.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-guide-dog.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2075 2013-08-23 03:21:37.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export-pdf.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1861 2013-08-23 02:50:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-ticket.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1163 2013-08-23 02:50:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-projection-screen.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1093 2013-08-23 03:21:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-flag.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2365 2013-08-23 03:21:29.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-in.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2562 2013-08-23 02:50:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-skype.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1385 2013-08-23 02:50:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-four.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1292 2013-08-23 03:07:42.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-justify.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      983 2013-08-23 03:07:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-rewind.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1688 2013-08-23 03:21:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torso-business.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1557 2013-08-23 03:21:35.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-like.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      919 2013-08-23 03:21:29.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-left.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1611 2013-08-23 03:07:43.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-link.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2292 2013-08-23 02:50:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-puzzle.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      921 2013-08-23 03:21:29.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-down.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1014 2013-08-23 03:07:41.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-tablet-landscape.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1004 2013-08-23 02:50:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mountains.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1840 2013-08-23 03:21:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-all-female.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2858 2013-08-23 03:21:36.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment-quotes.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      888 2013-08-23 03:21:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-play-video.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1845 2013-08-23 03:07:46.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paypal.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      882 2013-08-23 03:07:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-facebook.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1516 2013-08-23 03:21:37.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-delete.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1085 2013-08-23 03:07:43.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-print.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      816 2013-08-23 02:50:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shield.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      876 2013-08-23 02:50:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-battery-empty.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      770 2013-08-23 03:07:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-drive.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      805 2013-08-23 02:50:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-windows.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1798 2013-08-23 03:07:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-loop.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2438 2013-08-23 03:07:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-volume-strike.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1670 2013-08-23 03:21:36.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-megaphone.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1453 2013-08-23 02:50:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-target-two.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1398 2013-08-23 02:50:57.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-female-symbol.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3657 2013-08-23 02:50:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-youtube.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1325 2013-08-23 02:50:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paw.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1207 2013-08-23 03:21:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-crop.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      921 2013-08-23 03:21:31.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-heart.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1378 2013-08-23 03:21:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4361 2013-08-23 02:50:56.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-telephone-accessible.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1297 2013-08-23 03:07:43.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pause.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1477 2013-08-23 02:50:50.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-picasa.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1246 2013-08-23 03:07:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-apple.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1019 2013-08-23 03:21:38.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-filled.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1533 2013-08-23 03:07:43.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-save.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1460 2013-08-23 03:02:58.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-stack-overflow.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1418 2013-08-23 03:07:43.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paint-bucket.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4229 2013-08-23 03:07:46.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-foundation.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      941 2013-08-23 03:21:31.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-check.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1966 2013-08-23 03:07:42.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-subscript.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      902 2013-08-23 03:07:46.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shopping-bag.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1856 2013-08-23 03:21:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-all.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1910 2013-08-23 03:21:35.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mail.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1553 2013-08-23 03:21:32.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-rss.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1450 2013-08-23 02:50:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-book.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      990 2013-08-23 03:21:32.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-lock.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1707 2013-08-23 03:21:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-female-male.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3703 2013-08-23 03:07:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-digg.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2290 2013-08-23 03:21:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list-thumbnails.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1510 2013-08-23 02:50:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-book-bookmark.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2333 2013-08-23 03:07:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-behance.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2867 2013-08-23 03:21:34.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-results.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2850 2013-08-23 02:50:56.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-hearing-aid.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      940 2013-08-23 03:07:41.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-monitor.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1227 2013-08-23 02:50:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-three.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1976 2013-08-23 03:21:31.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-widget.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      827 2013-08-23 03:21:36.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1019 2013-08-23 03:21:32.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-trash.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3130 2013-08-23 02:50:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clipboard-notes.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1348 2013-08-23 03:21:34.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-bar.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1526 2013-08-23 03:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-foursquare.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2859 2013-08-23 03:07:46.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-500px.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      826 2013-08-23 03:21:33.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-folder.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1055 2013-08-23 03:07:49.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-orkut.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      881 2013-08-23 02:50:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-one.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      747 2013-08-23 03:07:46.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-adobe.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1061 2013-08-23 03:21:38.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-copy.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2798 2013-08-23 03:07:45.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-burst-sale.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2228 2013-08-23 03:07:45.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pound.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1239 2013-08-23 03:21:34.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-pie.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2414 2013-08-23 03:21:35.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-results-demographics.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1558 2013-08-23 03:21:34.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-archive.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      997 2013-08-23 02:50:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-info.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1961 2013-08-23 03:07:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-designer-news.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2614 2013-08-23 03:07:43.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-quote.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1041 2013-08-23 03:21:36.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment-video.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      926 2013-08-23 02:50:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-music.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3461 2013-08-23 16:21:31.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-smashing-mag.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1799 2013-08-23 03:07:45.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-yen.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      956 2013-08-23 02:50:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-battery-half.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1162 2013-08-23 03:21:36.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment-minus.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1458 2013-08-23 02:50:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-zerply.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2080 2013-08-23 03:07:45.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-rewind-ten.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      822 2013-08-23 03:21:36.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1372 2013-08-23 03:07:42.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-center.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2006 2013-08-23 02:50:56.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-closed-caption.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1797 2013-08-23 03:07:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shuffle.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1296 2013-08-23 03:07:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-previous.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1495 2013-08-23 03:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-github.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1775 2013-08-23 03:07:45.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bitcoin-circle.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1525 2013-08-23 03:07:49.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-myspace.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1450 2013-08-23 03:21:37.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-pdf.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1100 2013-08-23 03:21:31.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-x.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2028 2013-08-23 02:50:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clipboard-pencil.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      896 2013-08-23 03:21:35.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bookmark.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      923 2013-08-23 03:07:48.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-flickr.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1015 2013-08-23 03:07:41.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-tablet-portrait.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1332 2013-08-23 03:21:34.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-checkbox.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      977 2013-08-23 02:50:50.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-path.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2227 2013-08-23 03:07:45.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bitcoin.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1228 2013-08-23 03:07:42.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list-bullet.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2643 2013-08-23 03:07:46.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-amazon.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     6246 2013-08-23 04:32:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/.fontcustom-data
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)   150535 2013-08-23 16:25:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    19508 2013-08-23 16:57:53.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    54568 2013-08-23 16:25:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.eot
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    56976 2013-08-23 16:25:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.ttf
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     6424 2014-08-21 21:50:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/index.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/css/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     7783 2014-08-21 21:50:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/css/normalize.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      932 2015-04-25 23:06:13.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation_fobi_extras.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)   168084 2014-06-01 21:16:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation_template-4.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)   180512 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3404 2015-04-25 21:57:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation-datepicker.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4297 2015-04-25 23:05:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation-datetimepicker.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)   141825 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation.min.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      237 2014-08-21 21:50:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/humans.txt
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4787 2016-10-04 22:19:58.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/fobi_themes.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      438 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      308 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       49 2014-01-17 01:18:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/view_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2014-01-17 01:18:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/form_entry_submitted.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2015-08-27 21:03:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/import_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2014-01-17 01:18:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/add_form_handler_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2014-01-17 01:18:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/edit_form_element_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2014-01-17 01:18:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/create_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2665 2015-12-16 01:02:01.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/dashboard.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     5506 2014-09-26 02:16:06.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/_base.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2014-01-17 01:18:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/edit_form_handler_entry_ajax.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1363 2015-12-21 23:10:31.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/forms_list.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2014-01-17 01:18:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/view_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      151 2014-09-26 02:16:13.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/edit_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       59 2014-01-17 02:04:59.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/form_entry_submitted_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     8567 2016-10-04 21:22:49.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/edit_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       51 2014-01-17 01:18:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/create_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2014-01-17 01:18:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/add_form_element_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       38 2014-03-27 21:40:35.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/base.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2014-01-17 01:18:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/add_form_handler_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       57 2014-01-17 01:18:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/edit_form_element_entry.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3421 2014-10-07 22:38:28.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/form_properties_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1173 2014-09-30 22:34:58.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/form_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      138 2014-06-18 23:14:00.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/messages_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      331 2014-12-04 01:22:25.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/form_non_field_and_hidden_errors_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3668 2015-03-26 22:47:54.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/form_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       57 2014-01-17 01:18:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/edit_form_handler_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      154 2015-08-27 21:03:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/import_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4220 2014-01-17 01:18:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/theme.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2014-01-17 01:18:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/add_form_element_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-12-26 15:48:03.000000 django-fobi-0.9.9/src/fobi/contrib/themes/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/dummy_bootstrap3_widget/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      889 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/dummy_bootstrap3_widget/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      631 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/dummy_bootstrap3_widget/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      420 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/dummy_bootstrap3_widget/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/static/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/static/bootstrap3/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/static/bootstrap3/js/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      380 2015-04-26 01:43:03.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/static/bootstrap3/js/fobi.plugin.datetime-bootstrap3-widget.js
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1072 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      640 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      426 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/__init__.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-04-20 20:43:43.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/static/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/static/bootstrap3/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/static/bootstrap3/js/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      359 2015-04-26 01:42:37.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/static/bootstrap3/js/fobi.plugin.date-bootstrap3-widget.js
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1032 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      628 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      418 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/js/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      737 2016-10-27 20:27:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/js/fobi.plugin.slider-bootstrap3-widget.js
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    57251 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/js/bootstrap-slider.js
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    32390 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/js/bootstrap-slider.min.js
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/css/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     8404 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/css/bootstrap-slider.css
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      595 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/css/fobi.plugin.slider-bootstrap3-widget.css
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     7522 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/css/bootstrap-slider.min.css
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1010 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      634 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      422 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/__init__.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2015-04-20 20:43:46.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    58533 2013-12-05 16:40:18.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3253 2016-09-30 21:19:06.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap3_fobi_extras.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    30410 2015-03-07 16:32:25.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap-datetimepicker.min.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    27822 2013-12-05 16:40:19.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap.min.js
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    14716 2013-12-05 16:40:18.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap-theme.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    99548 2013-12-05 16:40:18.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap.min.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)   122848 2013-12-05 16:40:18.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     8860 2015-03-07 16:32:25.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap-datetimepicker.min.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      502 2015-03-25 01:06:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap3_fobi_extras.css
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    13135 2013-12-05 16:40:18.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap-theme.min.css
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    62850 2013-12-05 16:40:18.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.svg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    23292 2013-12-05 16:40:18.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.woff
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    20290 2013-12-05 16:40:18.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.eot
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    41236 2013-12-05 16:40:18.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     8326 2016-10-16 23:35:21.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/fobi_themes.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      435 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      312 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       49 2014-01-16 21:51:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/view_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2014-01-16 21:51:02.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/form_entry_submitted.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       61 2016-09-29 20:28:59.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_wizard_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2014-01-16 21:48:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/add_form_handler_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2014-01-16 21:50:13.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_element_entry_ajax.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       63 2016-09-27 21:07:24.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/create_form_wizard_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2014-01-16 21:49:42.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/create_form_entry_ajax.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       56 2016-10-16 23:34:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/form_wizards_dashboard.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       47 2015-10-05 21:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/form_importer.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       43 2014-01-16 21:49:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/dashboard.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      851 2016-10-26 09:36:19.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/_base.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       62 2014-01-16 21:50:49.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_handler_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       65 2014-10-25 20:16:31.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/embed_form_entry_submitted_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       52 2015-10-05 21:40:14.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/form_importer_ajax.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       56 2016-09-29 20:28:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_wizard_entry.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       68 2016-10-14 21:36:17.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/add_form_wizard_handler_entry_ajax.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       58 2016-09-27 21:07:12.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/create_form_wizard_entry.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       44 2015-12-21 22:21:03.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/forms_list.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2014-01-16 21:51:41.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/view_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       49 2014-01-16 21:50:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       59 2014-01-17 02:04:51.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/form_entry_submitted_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2014-01-16 21:50:32.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       60 2014-10-24 22:17:58.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/view_embed_form_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       51 2014-01-16 21:49:27.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/create_form_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       61 2014-01-16 21:48:11.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/add_form_element_entry_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       37 2014-01-16 21:49:07.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/base.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2014-01-16 21:48:40.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/add_form_handler_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       57 2014-01-16 21:50:01.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_element_entry.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      400 2016-10-14 21:51:03.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_wizard_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      931 2014-09-12 23:40:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_properties_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      393 2014-01-16 21:07:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_ajax.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       59 2014-01-16 21:45:13.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/messages_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      612 2014-12-02 23:30:22.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_non_field_and_hidden_errors_snippet.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      847 2016-09-30 21:16:34.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_wizard_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       54 2015-10-05 21:39:47.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_wizard.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      840 2014-12-02 23:29:39.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_snippet.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      938 2016-10-13 20:25:30.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_wizard_properties_snippet.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       57 2014-01-16 21:50:41.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/edit_form_handler_entry.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       61 2016-10-16 22:36:16.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/view_form_wizard_entry_ajax.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       56 2016-10-16 22:35:55.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/view_form_wizard_entry.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)       63 2016-10-14 21:35:57.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/add_form_wizard_handler_entry.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     4220 2014-01-16 21:46:56.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/theme.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       56 2014-01-16 21:47:37.000000 django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/add_form_element_entry.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-12-22 14:24:17.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_model_object/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      513 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_model_object/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      398 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_model_object/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1100 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_model_object/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2398 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_model_object/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3557 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_model_object/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      545 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_model_object/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      409 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_model_object/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      452 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      366 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1127 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4017 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3449 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      601 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      441 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/__init__.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1343 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/fields.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2588 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1826 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      513 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      394 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/textarea/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1921 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/textarea/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1447 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/textarea/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      495 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/textarea/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      376 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/textarea/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/integer/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2339 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/integer/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1831 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/integer/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      492 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/integer/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      373 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/integer/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      475 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date/widgets.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2222 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2380 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      523 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      404 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/ip_address/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2866 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/ip_address/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1607 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/ip_address/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      501 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/ip_address/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      382 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/ip_address/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/password/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2258 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/password/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1578 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/password/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      495 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/password/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      376 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/password/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      523 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      407 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1215 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2461 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3966 2016-10-24 22:31:25.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      616 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      456 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      364 2016-09-28 08:24:58.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/settings.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      305 2016-09-28 08:19:38.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/defaults.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1127 2016-09-28 08:19:19.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/conf.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2381 2016-09-28 08:23:34.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2841 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/fobi_form_elements.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      600 2016-09-28 08:18:17.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/apps.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      423 2016-09-28 08:17:43.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/input/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     5930 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/input/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1867 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/input/constants.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3018 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/input/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      486 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/input/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      367 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/input/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/regex/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3107 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/regex/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1627 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/regex/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      526 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/regex/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      407 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/regex/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slug/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2242 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slug/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1521 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slug/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      483 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slug/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      364 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slug/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/email/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2339 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/email/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1679 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/email/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      486 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/email/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      367 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/email/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/text/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2242 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/text/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1521 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/text/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      483 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/text/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      364 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/text/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      528 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      412 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1223 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2533 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4000 2016-10-24 22:41:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      631 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      471 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      455 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      340 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      512 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/widgets.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1028 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     7838 2016-10-28 22:10:10.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1858 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/constants.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1048 2016-10-30 22:39:11.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/helpers.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     6606 2016-10-28 22:01:47.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      489 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      370 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      518 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      417 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1135 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2419 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3577 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      601 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      441 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/float/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2325 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/float/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1781 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/float/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      486 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/float/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      367 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/float/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/radio/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      416 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/radio/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      330 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/radio/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      974 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/radio/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     4070 2016-10-05 19:40:28.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/radio/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3050 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/radio/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      486 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/radio/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      367 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/radio/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/url/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2232 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/url/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1699 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/url/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      480 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/url/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      361 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/url/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      524 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      367 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1135 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3805 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3369 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      575 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      441 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/boolean/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1715 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/boolean/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1183 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/boolean/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      492 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/boolean/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      373 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/boolean/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      443 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      357 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1067 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3755 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3326 2016-10-24 22:38:08.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      516 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      397 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple/__init__.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-10-13 21:18:48.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/time/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2219 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/time/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2397 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/time/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      523 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/time/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      404 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/time/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1786 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1536 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      489 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      370 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/null_boolean/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1740 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/null_boolean/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1458 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/null_boolean/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      507 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/null_boolean/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      388 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/null_boolean/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      417 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      331 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1012 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3598 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3006 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      489 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      370 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/range_select/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      461 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/range_select/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      346 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/range_select/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1055 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/range_select/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3647 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/range_select/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1853 2016-10-24 23:29:30.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/range_select/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      507 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/range_select/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      388 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/range_select/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/decimal/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2793 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/decimal/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2152 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/decimal/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      532 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/decimal/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      413 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/decimal/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/datetime/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      491 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/datetime/widgets.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2256 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/datetime/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2458 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/datetime/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      535 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/datetime/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      416 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/datetime/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/file/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      364 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/file/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      309 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/file/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      969 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/file/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2006 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/file/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2586 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/file/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      483 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/file/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      364 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/file/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/honeypot/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      362 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/honeypot/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      272 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/honeypot/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      980 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/honeypot/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2291 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/honeypot/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1603 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/honeypot/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      501 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/honeypot/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      380 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/honeypot/__init__.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      878 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/honeypot/fields.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/recaptcha/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2339 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/recaptcha/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3853 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/recaptcha/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      504 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/recaptcha/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      383 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/recaptcha/__init__.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-12-01 22:10:29.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/captcha/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2284 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/captcha/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3730 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/captcha/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      498 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/captcha/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      377 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/captcha/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/test/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/test/dummy/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      437 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/test/dummy/widgets.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/test/dummy/static/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/test/dummy/static/dummy/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/test/dummy/static/dummy/js/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      202 2014-03-26 00:42:32.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/test/dummy/static/dummy/js/fobi.plugins.form_elements.dummy.js
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/test/dummy/static/dummy/css/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      202 2014-03-26 00:42:43.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/test/dummy/static/dummy/css/fobi.plugins.form_elements.dummy.css
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1284 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/test/dummy/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      480 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/test/dummy/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      363 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/test/dummy/__init__.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-11-08 22:49:39.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/test/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_text/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      776 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_text/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1364 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_text/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      510 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_text/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      390 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_text/__init__.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-12-26 10:44:00.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_video/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      484 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_video/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      454 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_video/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1036 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_video/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1307 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_video/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1487 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_video/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      513 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_video/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      393 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_video/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1888 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1954 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1024 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2059 2016-10-05 19:37:15.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3429 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/helpers.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2678 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/fobi_form_elements.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      513 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      393 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/templates/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/templates/content_image/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      539 2013-12-26 13:53:19.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/templates/content_image/render.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-08-16 17:45:03.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    10589 2016-10-16 21:35:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/fobi_form_handlers.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      377 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      315 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1165 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/widgets.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      946 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2029 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1540 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/helpers.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      502 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      364 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/templates/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/templates/mail/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      190 2015-04-25 21:23:12.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/templates/mail/plugin_data_repr.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1358 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/fields.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     7305 2016-10-19 22:07:01.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/fobi_form_handlers.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3698 2016-10-17 00:04:10.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/models.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      446 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      299 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/defaults.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/migrations/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1663 2016-10-15 23:35:40.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/migrations/0002_savedformwizarddataentry.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1772 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/migrations/0001_initial.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)        0 2016-05-12 20:03:09.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/migrations/__init__.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     6075 2016-10-25 18:37:30.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/views.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/urls/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2084 2016-10-12 20:46:18.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/urls/form_handlers.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2199 2016-10-12 20:46:29.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/urls/form_wizard_handlers.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      178 2016-10-12 09:12:58.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/urls/__init__.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      661 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/widgets.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/static/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/js/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     5417 2014-07-16 15:22:22.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/js/jquery.expander.min.js
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1193 2014-07-16 15:22:22.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/js/jquery.expander.license.txt
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      815 2014-08-08 20:40:45.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/js/db_store.js
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      967 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     5521 2016-10-25 18:37:07.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/helpers.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     5336 2016-10-25 18:45:54.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/admin.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      474 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      336 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/templates/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/templates/db_store/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2291 2016-10-12 09:25:01.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/templates/db_store/view_saved_form_wizard_data_entries.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     2228 2014-11-05 01:02:27.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/templates/db_store/view_saved_form_data_entries.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      178 2014-07-31 23:58:36.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/templates/db_store/plugin_data_repr.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-12-22 14:24:25.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/http_repost/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     6496 2016-10-17 01:09:51.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/http_repost/fobi_form_handlers.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      782 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/http_repost/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      483 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/http_repost/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      371 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/http_repost/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/http_repost/templates/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/http_repost/templates/http_repost/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      140 2014-06-18 23:19:41.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/http_repost/templates/http_repost/plugin_data_repr.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_importers/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_importers/mailchimp_importer/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2350 2016-10-24 20:37:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_importers/mailchimp_importer/views.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1370 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_importers/mailchimp_importer/forms.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2307 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_importers/mailchimp_importer/fobi_form_importers.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      507 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_importers/mailchimp_importer/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      385 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_importers/mailchimp_importer/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_importers/mailchimp_importer/templates/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_importers/mailchimp_importer/templates/mailchimp_importer/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       47 2016-10-09 20:11:58.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_importers/mailchimp_importer/templates/mailchimp_importer/1.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       47 2015-10-05 21:52:37.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_importers/mailchimp_importer/templates/mailchimp_importer/0.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-09-25 23:54:07.000000 django-fobi-0.9.9/src/fobi/contrib/plugins/form_importers/__init__.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-08-12 09:21:42.000000 django-fobi-0.9.9/src/fobi/contrib/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/apps/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2446 2016-09-26 21:03:37.000000 django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/models.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      993 2016-10-12 20:56:56.000000 django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      417 2016-10-12 20:56:33.000000 django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1000 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      999 2016-10-12 20:56:42.000000 django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/helpers.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      462 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      303 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/templates/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/templates/djangocms_integration/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      180 2014-11-18 23:29:06.000000 django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/templates/djangocms_integration/login_required.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)       58 2014-11-18 00:32:25.000000 django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/templates/djangocms_integration/widget.html
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1727 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/cms_plugins.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/apps/wagtail_integration_/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     3634 2016-09-28 08:54:07.000000 django-fobi-0.9.9/src/fobi/contrib/apps/wagtail_integration_/models.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)     1010 2016-09-28 08:54:19.000000 django-fobi-0.9.9/src/fobi/contrib/apps/wagtail_integration_/settings.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      425 2016-09-28 08:50:38.000000 django-fobi-0.9.9/src/fobi/contrib/apps/wagtail_integration_/defaults.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      995 2016-09-28 08:50:30.000000 django-fobi-0.9.9/src/fobi/contrib/apps/wagtail_integration_/conf.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      998 2016-09-28 08:51:18.000000 django-fobi-0.9.9/src/fobi/contrib/apps/wagtail_integration_/helpers.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      470 2016-09-28 08:50:05.000000 django-fobi-0.9.9/src/fobi/contrib/apps/wagtail_integration_/apps.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      313 2016-09-28 08:49:51.000000 django-fobi-0.9.9/src/fobi/contrib/apps/wagtail_integration_/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2636 2016-09-26 21:05:20.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/models.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1002 2016-10-12 20:58:08.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      417 2016-10-12 20:57:39.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1000 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1000 2016-10-12 20:57:48.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/helpers.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      359 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/admin.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      462 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      303 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/__init__.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1320 2016-10-12 20:58:00.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/page_processors.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/templates/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/templates/mezzanine_integration/
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/templates/mezzanine_integration/admin/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      539 2014-12-10 00:09:44.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/templates/mezzanine_integration/admin/change_form.html
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/templates/pages/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      630 2014-12-16 23:31:15.000000 django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/templates/pages/fobiformpage.html
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-09-28 11:50:14.000000 django-fobi-0.9.9/src/fobi/contrib/apps/__init__.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/contrib/apps/feincms_integration/
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2014-07-28 23:18:44.000000 django-fobi-0.9.9/src/fobi/contrib/apps/feincms_integration/models.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     1000 2016-10-12 20:57:29.000000 django-fobi-0.9.9/src/fobi/contrib/apps/feincms_integration/settings.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      415 2016-10-12 20:57:10.000000 django-fobi-0.9.9/src/fobi/contrib/apps/feincms_integration/defaults.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3379 2016-09-26 21:04:30.000000 django-fobi-0.9.9/src/fobi/contrib/apps/feincms_integration/widgets.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      981 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/apps/feincms_integration/conf.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      994 2016-10-12 20:57:19.000000 django-fobi-0.9.9/src/fobi/contrib/apps/feincms_integration/helpers.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      456 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/apps/feincms_integration/apps.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      299 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/contrib/apps/feincms_integration/__init__.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2266 2016-10-12 20:39:47.000000 django-fobi-0.9.9/src/fobi/exceptions.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/fobi/templatetags/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    16767 2016-10-17 00:36:26.000000 django-fobi-0.9.9/src/fobi/templatetags/fobi_tags.py
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)        0 2013-08-12 09:21:42.000000 django-fobi-0.9.9/src/fobi/templatetags/__init__.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     3862 2016-09-22 20:04:44.000000 django-fobi-0.9.9/src/fobi/templatetags/future_compat.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2891 2016-09-22 20:04:54.000000 django-fobi-0.9.9/src/fobi/discover.py
+drwxrwxr-x   0 foreverchild  (1000) foreverchild  (1000)        0 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/django_fobi.egg-info/
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)        1 2016-10-30 23:53:37.000000 django-fobi-0.9.9/src/django_fobi.egg-info/dependency_links.txt
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)      219 2016-10-30 23:53:37.000000 django-fobi-0.9.9/src/django_fobi.egg-info/requires.txt
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    88772 2016-10-30 23:53:52.000000 django-fobi-0.9.9/src/django_fobi.egg-info/SOURCES.txt
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)        5 2016-10-30 23:53:37.000000 django-fobi-0.9.9/src/django_fobi.egg-info/top_level.txt
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)   101817 2016-10-30 23:53:37.000000 django-fobi-0.9.9/src/django_fobi.egg-info/PKG-INFO
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)     2899 2016-10-24 20:37:52.000000 django-fobi-0.9.9/MANIFEST.in
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)      740 2016-10-30 23:53:52.000000 django-fobi-0.9.9/setup.cfg
+-rw-------   0 foreverchild  (1000) foreverchild  (1000)    18097 2016-10-17 01:10:54.000000 django-fobi-0.9.9/LICENSE_GPL2.0.txt
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    78289 2016-10-26 22:55:29.000000 django-fobi-0.9.9/README.rst
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    10445 2016-10-30 23:45:24.000000 django-fobi-0.9.9/setup.py
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)    35078 2016-10-30 23:45:16.000000 django-fobi-0.9.9/CHANGELOG.rst
+-rw-rw-r--   0 foreverchild  (1000) foreverchild  (1000)   101817 2016-10-30 23:53:52.000000 django-fobi-0.9.9/PKG-INFO
```

### Comparing `django-fobi-0.9.8/LICENSE_LGPL_2.1.txt` & `django-fobi-0.9.9/LICENSE_LGPL_2.1.txt`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/dynamic.py` & `django-fobi-0.9.9/src/fobi/dynamic.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/context_processors.py` & `django-fobi-0.9.9/src/fobi/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/integration/processors.py` & `django-fobi-0.9.9/src/fobi/integration/processors.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/integration/helpers.py` & `django-fobi-0.9.9/src/fobi/integration/helpers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/models.py` & `django-fobi-0.9.9/src/fobi/models.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/settings.py` & `django-fobi-0.9.9/src/fobi/settings.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/form_importers.py` & `django-fobi-0.9.9/src/fobi/form_importers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/defaults.py` & `django-fobi-0.9.9/src/fobi/defaults.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/migrations/0010_formwizardhandler.py` & `django-fobi-0.9.9/src/fobi/migrations/0010_formwizardhandler.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/migrations/0006_auto_20160911_1549.py` & `django-fobi-0.9.9/src/fobi/migrations/0006_auto_20160911_1549.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/migrations/0005_auto_20160908_1457.py` & `django-fobi-0.9.9/src/fobi/migrations/0005_auto_20160908_1457.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/migrations/0004_auto_20160906_1513.py` & `django-fobi-0.9.9/src/fobi/migrations/0004_auto_20160906_1513.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/migrations/0001_initial.py` & `django-fobi-0.9.9/src/fobi/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/migrations/0009_formwizardentry_wizard_type.py` & `django-fobi-0.9.9/src/fobi/migrations/0009_formwizardentry_wizard_type.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/migrations/0007_auto_20160926_1652.py` & `django-fobi-0.9.9/src/fobi/migrations/0007_auto_20160926_1652.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/migrations/0008_formwizardhandlerentry.py` & `django-fobi-0.9.9/src/fobi/migrations/0008_formwizardhandlerentry.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/migrations/0002_auto_20150912_1744.py` & `django-fobi-0.9.9/src/fobi/migrations/0002_auto_20150912_1744.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/migrations/0003_auto_20160517_1005.py` & `django-fobi-0.9.9/src/fobi/migrations/0003_auto_20160517_1005.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/views.py` & `django-fobi-0.9.9/src/fobi/views.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/tests/data.py` & `django-fobi-0.9.9/src/fobi/tests/data.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/tests/base.py` & `django-fobi-0.9.9/src/fobi/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/tests/test_dynamic_forms.py` & `django-fobi-0.9.9/src/fobi/tests/test_dynamic_forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/tests/test_form_importers_mailchimp.py` & `django-fobi-0.9.9/src/fobi/tests/test_form_importers_mailchimp.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/tests/helpers.py` & `django-fobi-0.9.9/src/fobi/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/tests/test_browser_build_dynamic_forms.py` & `django-fobi-0.9.9/src/fobi/tests/test_browser_build_dynamic_forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/tests/test_core.py` & `django-fobi-0.9.9/src/fobi/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/tests/test_sortable_dict.py` & `django-fobi-0.9.9/src/fobi/tests/test_sortable_dict.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/utils.py` & `django-fobi-0.9.9/src/fobi/utils.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/urls/view.py` & `django-fobi-0.9.9/src/fobi/urls/view.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/urls/edit.py` & `django-fobi-0.9.9/src/fobi/urls/edit.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/management/commands/fobi_find_broken_entries.py` & `django-fobi-0.9.9/src/fobi/management/commands/fobi_find_broken_entries.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/management/commands/fobi_update_plugin_data.py` & `django-fobi-0.9.9/src/fobi/management/commands/fobi_update_plugin_data.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/management/commands/fobi_migrate_03_to_04.py` & `django-fobi-0.9.9/src/fobi/management/commands/fobi_migrate_03_to_04.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/widgets.py` & `django-fobi-0.9.9/src/fobi/widgets.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/js/moment-with-locales.js` & `django-fobi-0.9.9/src/fobi/static/js/moment-with-locales.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/js/fobi.core.js` & `django-fobi-0.9.9/src/fobi/static/js/fobi.core.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/js/jquery.slugify.js` & `django-fobi-0.9.9/src/fobi/static/js/jquery.slugify.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/js/jquery-1.10.2.min.js` & `django-fobi-0.9.9/src/fobi/static/js/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/js/jquery.slugify.license.txt` & `django-fobi-0.9.9/src/fobi/static/js/jquery.slugify.license.txt`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/js/jquery.license.txt` & `django-fobi-0.9.9/src/fobi/static/js/jquery.license.txt`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/js/jquery-ui-1.10.4.custom.min.js` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/js/jquery-ui-1.10.4.custom.min.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/js/jquery-ui-1.10.4.custom.js` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/js/jquery-ui-1.10.4.custom.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/jquery-ui.license.txt` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/jquery-ui.license.txt`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/index.html` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/index.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_cd0a0a_256x240.png` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_2e83ff_256x240.png` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_888888_256x240.png` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/animated-overlay.gif` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/animated-overlay.gif`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_222222_256x240.png` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_454545_256x240.png` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/jquery-ui-1.10.3.custom.css` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/jquery-ui-1.10.3.custom.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/smoothness/jquery-ui-1.10.3.custom.min.css` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/smoothness/jquery-ui-1.10.3.custom.min.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_ffffff_256x240.png` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_cd0a0a_256x240.png` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_bbbbcc_256x240.png` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_bbbbcc_256x240.png`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_2e83ff_256x240.png` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_888888_256x240.png` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/animated-overlay.gif` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/animated-overlay.gif`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_454545_256x240.png` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/jquery-ui-1.10.4.custom.css` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/jquery-ui-1.10.4.custom.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/jquery-ui/css/django-admin-theme/jquery-ui-1.10.4.custom.min.css` & `django-fobi-0.9.9/src/fobi/static/jquery-ui/css/django-admin-theme/jquery-ui-1.10.4.custom.min.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/css/admin_custom.css` & `django-fobi-0.9.9/src/fobi/static/css/admin_custom.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/css/fobi.core.css` & `django-fobi-0.9.9/src/fobi/static/css/fobi.core.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/less/path.less` & `django-fobi-0.9.9/src/fobi/static/font-awesome/less/path.less`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/less/icons.less` & `django-fobi-0.9.9/src/fobi/static/font-awesome/less/icons.less`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/less/bootstrap.less` & `django-fobi-0.9.9/src/fobi/static/font-awesome/less/bootstrap.less`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/less/core.less` & `django-fobi-0.9.9/src/fobi/static/font-awesome/less/core.less`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/less/font-awesome-ie7.less` & `django-fobi-0.9.9/src/fobi/static/font-awesome/less/font-awesome-ie7.less`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/less/font-awesome.less` & `django-fobi-0.9.9/src/fobi/static/font-awesome/less/font-awesome.less`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/less/variables.less` & `django-fobi-0.9.9/src/fobi/static/font-awesome/less/variables.less`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/less/mixins.less` & `django-fobi-0.9.9/src/fobi/static/font-awesome/less/mixins.less`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/less/extras.less` & `django-fobi-0.9.9/src/fobi/static/font-awesome/less/extras.less`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/css/font-awesome.min.css` & `django-fobi-0.9.9/src/fobi/static/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/css/font-awesome-ie7.css` & `django-fobi-0.9.9/src/fobi/static/font-awesome/css/font-awesome-ie7.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/css/font-awesome-ie7.min.css` & `django-fobi-0.9.9/src/fobi/static/font-awesome/css/font-awesome-ie7.min.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/css/font-awesome.css` & `django-fobi-0.9.9/src/fobi/static/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/scss/font-awesome.scss` & `django-fobi-0.9.9/src/fobi/static/font-awesome/scss/font-awesome.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/scss/_icons.scss` & `django-fobi-0.9.9/src/fobi/static/font-awesome/scss/_icons.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/scss/_core.scss` & `django-fobi-0.9.9/src/fobi/static/font-awesome/scss/_core.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/scss/_mixins.scss` & `django-fobi-0.9.9/src/fobi/static/font-awesome/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/scss/font-awesome-ie7.scss` & `django-fobi-0.9.9/src/fobi/static/font-awesome/scss/font-awesome-ie7.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/scss/_bootstrap.scss` & `django-fobi-0.9.9/src/fobi/static/font-awesome/scss/_bootstrap.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/scss/_variables.scss` & `django-fobi-0.9.9/src/fobi/static/font-awesome/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/scss/_extras.scss` & `django-fobi-0.9.9/src/fobi/static/font-awesome/scss/_extras.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/scss/_path.scss` & `django-fobi-0.9.9/src/fobi/static/font-awesome/scss/_path.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/font/fontawesome-webfont.eot` & `django-fobi-0.9.9/src/fobi/static/font-awesome/font/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/font/fontawesome-webfont.ttf` & `django-fobi-0.9.9/src/fobi/static/font-awesome/font/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/font/license.txt` & `django-fobi-0.9.9/src/fobi/static/font-awesome/font/license.txt`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/font/fontawesome-webfont.woff` & `django-fobi-0.9.9/src/fobi/static/font-awesome/font/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/font/fontawesome-webfont.svg` & `django-fobi-0.9.9/src/fobi/static/font-awesome/font/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/font/FontAwesome.otf` & `django-fobi-0.9.9/src/fobi/static/font-awesome/font/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/font-awesome/code.license.txt` & `django-fobi-0.9.9/src/fobi/static/font-awesome/code.license.txt`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/colorbox/images/loading.gif` & `django-fobi-0.9.9/src/fobi/static/colorbox/images/loading.gif`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/colorbox/images/controls.png` & `django-fobi-0.9.9/src/fobi/static/colorbox/images/controls.png`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/colorbox/jquery.colorbox-min.js` & `django-fobi-0.9.9/src/fobi/static/colorbox/jquery.colorbox-min.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/colorbox/index.html` & `django-fobi-0.9.9/src/fobi/static/colorbox/index.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/static/colorbox/colorbox.css` & `django-fobi-0.9.9/src/fobi/static/colorbox/colorbox.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/base.py` & `django-fobi-0.9.9/src/fobi/base.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/conf.py` & `django-fobi-0.9.9/src/fobi/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/south_migrations/0003_auto__add_formwizardformentry__add_unique_formwizardformentry_form_wiz.py` & `django-fobi-0.9.9/src/fobi/south_migrations/0003_auto__add_formwizardformentry__add_unique_formwizardformentry_form_wiz.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/south_migrations/0001_initial.py` & `django-fobi-0.9.9/src/fobi/south_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/south_migrations/0002_auto__add_field_formentry_created__add_field_formentry_updated.py` & `django-fobi-0.9.9/src/fobi/south_migrations/0002_auto__add_field_formentry_created__add_field_formentry_updated.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/forms.py` & `django-fobi-0.9.9/src/fobi/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/constants.py` & `django-fobi-0.9.9/src/fobi/constants.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/helpers.py` & `django-fobi-0.9.9/src/fobi/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,45 +392,70 @@
     if entry:
         plugin = entry.get_plugin(request=request)
         logger.debug(plugin)
         if plugin:
             return plugin._update_plugin_data(entry)
 
 
-def get_select_field_choices(raw_choices_data):
+def get_select_field_choices(raw_choices_data,
+                             key_type=None,
+                             value_type=None,
+                             fail_silently=True):
     """Get select field choices.
 
     Used in ``radio``, ``select`` and other choice based
     fields.
 
     :param str raw_choices_data:
+    :param type key_type:
+    :param type value_type:
+    :param bool fail_silently:
     :return list:
     """
     choices = []  # Holds return value
     keys = set([])  # For checking uniqueness of keys
     values = set([])  # For checking uniqueness of values
 
     # Looping through the raw data
     for choice in raw_choices_data.split('\n'):
         choice = choice.strip()
 
         # If comma separated key, value
         if ',' in choice:
             key, value = choice.split(',', 1)
             key = key.strip()
+
+            # If type specified, cast to the type
+            if key_type and key is not None:
+                try:
+                    key = key_type(key)
+                except (ValueError, TypeError):
+                    return [] if fail_silently else None
+
             value = value.strip()
-            if key and key not in keys and value not in values:
+            # If type specified, cast to the type
+            if value_type and value is not None:
+                try:
+                    value = value_type(value)
+                except (ValueError, TypeError):
+                    return [] if fail_silently else None
+
+            if key is not None \
+                    and key not in keys \
+                    and value not in values:
                 choices.append((key, value))
                 keys.add(key)
                 values.add(value)
 
         # If key is also the value
         else:
             choice = choice.strip()
-            if choice and choice not in keys and choice not in values:
+            if choice is not None \
+                    and choice not in keys \
+                    and choice not in values:
                 choices.append((choice, choice))
                 keys.add(choice)
                 values.add(choice)
 
     return choices
```

### Comparing `django-fobi-0.9.8/src/fobi/locale/nl/LC_MESSAGES/django.po` & `django-fobi-0.9.9/src/fobi/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/locale/nl/LC_MESSAGES/django.mo` & `django-fobi-0.9.9/src/fobi/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/locale/de/LC_MESSAGES/django.po` & `django-fobi-0.9.9/src/fobi/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/locale/de/LC_MESSAGES/django.mo` & `django-fobi-0.9.9/src/fobi/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/locale/ru/LC_MESSAGES/django.po` & `django-fobi-0.9.9/src/fobi/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/locale/ru/LC_MESSAGES/django.mo` & `django-fobi-0.9.9/src/fobi/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/wizard/views/dynamic.py` & `django-fobi-0.9.9/src/fobi/wizard/views/dynamic.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/wizard/views/views.py` & `django-fobi-0.9.9/src/fobi/wizard/views/views.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/app.py` & `django-fobi-0.9.9/src/fobi/app.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/data_structures.py` & `django-fobi-0.9.9/src/fobi/data_structures.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/decorators.py` & `django-fobi-0.9.9/src/fobi/decorators.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/admin.py` & `django-fobi-0.9.9/src/fobi/admin.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/view_form_entry.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/view_form_entry.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/form_entry_submitted.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/form_entry_submitted.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/edit_form_wizard_entry_ajax.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/edit_form_wizard_entry_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/form_wizards_dashboard.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/form_wizards_dashboard.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/form_importer.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/form_importer.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/dashboard.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/_base.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/_base.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/edit_form_wizard_entry.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/edit_form_wizard_entry.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/create_form_wizard_entry.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/create_form_wizard_entry.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/forms_list.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/forms_list.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/edit_form_entry.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/edit_form_entry.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/form_entry_submitted_ajax.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/form_entry_submitted_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/edit_form_entry_ajax.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/edit_form_entry_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/create_form_entry.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/create_form_entry.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/add_form_handler_entry.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/add_form_handler_entry.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/edit_form_element_entry.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/add_form_element_entry.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 {% extends fobi_theme.base_edit_template %}
 
 {% load i18n %}
 
-{% block page-title %}{% blocktrans with form_element_plugin.name as plugin_name %}Edit "{{ plugin_name }}" element of the form{% endblocktrans %}{% endblock page-title %}
+{% block page-title %}{% blocktrans with form_element_plugin.name as plugin_name %}Add "{{ plugin_name }}" element to the form{% endblocktrans %}{% endblock page-title %}
 
 {% block navbar-menu-content %}
 {% endblock navbar-menu-content %}
 
 {% block navbar-menu-right-content %}
             <li class="active"><a href="{% url 'fobi.dashboard' %}">{% trans "Forms" %}</a></li>
             <li><a href="{% url 'fobi.form_wizards_dashboard' %}">{% trans "Wizards" %}</a></li>
 {% endblock navbar-menu-right-content %}
 
 {% block content %}
-    {% include fobi_theme.edit_form_element_entry_ajax_template %}
+    {% include fobi_theme.add_form_element_entry_ajax_template %}
 {% endblock content %}
 
 {% block sidebar-content %}
 {% endblock sidebar-content %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends fobi_theme.base_edit_template %} {% load i18n %} {% block page-title
-%}{% blocktrans with form_element_plugin.name as plugin_name %}Edit "{
-{ plugin_name }}" element of the form{% endblocktrans %}{% endblock page-title
+%}{% blocktrans with form_element_plugin.name as plugin_name %}Add "{
+{ plugin_name }}" element to the form{% endblocktrans %}{% endblock page-title
 %} {% block navbar-menu-content %} {% endblock navbar-menu-content %} {% block
 navbar-menu-right-content %}
 {%_trans_"Forms"_%}
 {%_trans_"Wizards"_%}
 {% endblock navbar-menu-right-content %} {% block content %} {% include
-fobi_theme.edit_form_element_entry_ajax_template %} {% endblock content %} {%
+fobi_theme.add_form_element_entry_ajax_template %} {% endblock content %} {%
 block sidebar-content %} {% endblock sidebar-content %}
```

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_wizard_ajax.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_wizard_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_edit_ajax.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_edit_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_view_ajax.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_view_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_wizard_view_ajax.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_wizard_view_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_properties_snippet.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_properties_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_ajax.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_wizard_snippet.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_wizard_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_wizard.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_wizard.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_snippet.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/snippets/form_wizard_properties_snippet.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/snippets/form_wizard_properties_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/edit_form_handler_entry.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/edit_form_handler_entry.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/view_form_wizard_entry_ajax.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/view_form_wizard_entry_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/import_form_entry.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/import_form_entry.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/view_form_wizard_entry.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/view_form_wizard_entry.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/form_wizard_entry_submitted_ajax.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/form_wizard_entry_submitted_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/add_form_wizard_handler_entry.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/add_form_wizard_handler_entry.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/form_wizard_entry_submitted.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/form_wizard_entry_submitted.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/theme.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/theme.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/generic/add_form_element_entry.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/generic/edit_form_element_entry.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 {% extends fobi_theme.base_edit_template %}
 
 {% load i18n %}
 
-{% block page-title %}{% blocktrans with form_element_plugin.name as plugin_name %}Add "{{ plugin_name }}" element to the form{% endblocktrans %}{% endblock page-title %}
+{% block page-title %}{% blocktrans with form_element_plugin.name as plugin_name %}Edit "{{ plugin_name }}" element of the form{% endblocktrans %}{% endblock page-title %}
+
+{% block extrahead %}
+    {% if form %}
+        {{ form.media }}
+    {% endif %}
+    {{ block.super }}
+{% endblock extrahead %}
 
 {% block navbar-menu-content %}
 {% endblock navbar-menu-content %}
 
 {% block navbar-menu-right-content %}
             <li class="active"><a href="{% url 'fobi.dashboard' %}">{% trans "Forms" %}</a></li>
             <li><a href="{% url 'fobi.form_wizards_dashboard' %}">{% trans "Wizards" %}</a></li>
 {% endblock navbar-menu-right-content %}
 
 {% block content %}
-    {% include fobi_theme.add_form_element_entry_ajax_template %}
+    {% include fobi_theme.edit_form_element_entry_ajax_template %}
 {% endblock content %}
 
 {% block sidebar-content %}
 {% endblock sidebar-content %}
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends fobi_theme.base_edit_template %} {% load i18n %} {% block page-title
-%}{% blocktrans with form_element_plugin.name as plugin_name %}Add "{
-{ plugin_name }}" element to the form{% endblocktrans %}{% endblock page-title
-%} {% block navbar-menu-content %} {% endblock navbar-menu-content %} {% block
-navbar-menu-right-content %}
+%}{% blocktrans with form_element_plugin.name as plugin_name %}Edit "{
+{ plugin_name }}" element of the form{% endblocktrans %}{% endblock page-title
+%} {% block extrahead %} {% if form %} {{ form.media }} {% endif %} {
+{ block.super }} {% endblock extrahead %} {% block navbar-menu-content %} {%
+endblock navbar-menu-content %} {% block navbar-menu-right-content %}
 {%_trans_"Forms"_%}
 {%_trans_"Wizards"_%}
 {% endblock navbar-menu-right-content %} {% block content %} {% include
-fobi_theme.add_form_element_entry_ajax_template %} {% endblock content %} {%
+fobi_theme.edit_form_element_entry_ajax_template %} {% endblock content %} {%
 block sidebar-content %} {% endblock sidebar-content %}
```

### Comparing `django-fobi-0.9.8/src/fobi/templates/fobi/admin/bulk_change_plugins.html` & `django-fobi-0.9.9/src/fobi/templates/fobi/admin/bulk_change_plugins.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/form_utils.py` & `django-fobi-0.9.9/src/fobi/form_utils.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/validators.py` & `django-fobi-0.9.9/src/fobi/validators.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/db_store/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/db_store/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/db_store/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/widgets/form_handlers/db_store/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/js/fobi.djangocms_admin_style_theme.edit.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/js/fobi.djangocms_admin_style_theme.edit.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/css/fobi.djangocms_admin_style_theme.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/css/fobi.djangocms_admin_style_theme.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/css/fobi.djangocms_admin_style_theme.edit.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/djangocms_admin_style_theme/css/fobi.djangocms_admin_style_theme.edit.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/static/admin/img/tooltag-add.gif` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/static/admin/img/tooltag-add.gif`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/fobi_themes.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/fobi_themes.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/dashboard.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/forms_list.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/forms_list.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/edit_form_entry_ajax.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/edit_form_entry_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/base_edit.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/base_edit.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_edit_ajax.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_edit_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_properties_snippet.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_properties_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_edit_snippet.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_edit_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_snippet.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/snippets/form_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/base_view.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/base_view.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/theme.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/djangocms_admin_style_theme/templates/djangocms_admin_style_theme/theme.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/widgets/form_handlers/db_store/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/widgets/form_handlers/db_store/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/widgets/form_handlers/db_store/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/widgets/form_handlers/db_store/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/simple/js/fobi.simple.edit.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/simple/js/fobi.simple.edit.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/simple/css/fobi.simple.edit.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/simple/css/fobi.simple.edit.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/simple/css/fobi.simple.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/simple/css/fobi.simple.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/static/admin/img/tooltag-add.gif` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/static/admin/img/tooltag-add.gif`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/fobi_themes.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/fobi_themes.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/dashboard.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/forms_list.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/forms_list.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/edit_form_entry_ajax.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/edit_form_entry_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/base_edit.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/base_edit.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/snippets/form_edit_ajax.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/snippets/form_edit_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/snippets/form_properties_snippet.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/snippets/form_properties_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/snippets/form_edit_snippet.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/snippets/form_edit_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/snippets/form_snippet.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/snippets/form_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/base_view.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/base_view.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/simple/templates/simple/theme.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/simple/templates/simple/theme.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/date_foundation5_widget/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/datetime_foundation5_widget/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/dummy_foundation5_widget/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/dummy_foundation5_widget/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_elements/dummy_foundation5_widget/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_elements/dummy_foundation5_widget/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/templates/db_store_foundation5_widget/view_saved_form_data_entries.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/widgets/form_handlers/db_store_foundation5_widget/templates/db_store_foundation5_widget/view_saved_form_data_entries.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation_template-4.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation_template-4.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation.min.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation.min.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/fastclick.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/fastclick.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/modernizr.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/modernizr.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/jquery.cookie.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/jquery.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/jquery.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/placeholder.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/vendor/placeholder.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation-datepicker.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation-datepicker.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation5_fobi_extras.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation5_fobi_extras.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.orbit.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.orbit.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.slider.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.slider.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.equalizer.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.equalizer.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.reveal.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.reveal.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.abide.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.abide.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.topbar.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.topbar.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.alert.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.alert.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.joyride.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.joyride.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.dropdown.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.dropdown.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.magellan.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.magellan.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.tooltip.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.tooltip.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.clearing.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.clearing.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.offcanvas.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.offcanvas.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.tab.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.tab.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.accordion.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.accordion.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.interchange.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation/foundation.interchange.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation-datetimepicker.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/js/foundation-datetimepicker.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/sass/accessibility_foundicons.scss` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/sass/accessibility_foundicons.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/sass/accessibility_foundicons_ie7.scss` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/sass/accessibility_foundicons_ie7.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/sass/_settings.scss` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/sass/_settings.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/stylesheets/accessibility_foundicons.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/stylesheets/accessibility_foundicons.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/stylesheets/accessibility_foundicons_ie7.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/stylesheets/accessibility_foundicons_ie7.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/demo.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/demo.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.eot` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.eot`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.woff` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.woff`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.ttf` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.ttf`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/fonts/accessibility_foundicons.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/0e61251fcc72078e76f7711e6e025bea2a2f1ce3/_settings.scssc` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/0e61251fcc72078e76f7711e6e025bea2a2f1ce3/_settings.scssc`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/0e61251fcc72078e76f7711e6e025bea2a2f1ce3/accessibility_foundicons.scssc` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/0e61251fcc72078e76f7711e6e025bea2a2f1ce3/accessibility_foundicons.scssc`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/0e61251fcc72078e76f7711e6e025bea2a2f1ce3/accessibility_foundicons_ie7.scssc` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/accessibility/.sass-cache/0e61251fcc72078e76f7711e6e025bea2a2f1ce3/accessibility_foundicons_ie7.scssc`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/sass/general_foundicons.scss` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/sass/general_foundicons.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/sass/_settings.scss` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/sass/_settings.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/sass/general_foundicons_ie7.scss` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/sass/general_foundicons_ie7.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/stylesheets/general_foundicons.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/stylesheets/general_foundicons.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/stylesheets/general_foundicons_ie7.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/stylesheets/general_foundicons_ie7.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/demo.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/demo.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.ttf` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.ttf`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.woff` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.woff`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.eot` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/fonts/general_foundicons.eot`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/_settings.scssc` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/_settings.scssc`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/general_foundicons.scssc` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/general_foundicons.scssc`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/general_foundicons_ie7.scssc` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/general_foundicons_ie7.scssc`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/accessibility_foundicons.scssc` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/accessibility_foundicons.scssc`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/accessibility_foundicons_ie7.scssc` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general/.sass-cache/6e921d17dabf1f492bd178102bc1a8a4322f1198/accessibility_foundicons_ie7.scssc`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/sass/general_enclosed_foundicons_ie7.scss` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/sass/general_enclosed_foundicons_ie7.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/sass/general_enclosed_foundicons.scss` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/sass/general_enclosed_foundicons.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/sass/_settings.scss` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/sass/_settings.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/stylesheets/general_enclosed_foundicons_ie7.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/stylesheets/general_enclosed_foundicons_ie7.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/stylesheets/general_enclosed_foundicons.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/stylesheets/general_enclosed_foundicons.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/demo.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/demo.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.eot` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.eot`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.ttf` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.ttf`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.woff` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/fonts/general_enclosed_foundicons.woff`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/1ea694b23cbc52b68bcbd397d07df10b08a18c32/_settings.scssc` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/1ea694b23cbc52b68bcbd397d07df10b08a18c32/_settings.scssc`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/1ea694b23cbc52b68bcbd397d07df10b08a18c32/general_enclosed_foundicons.scssc` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/1ea694b23cbc52b68bcbd397d07df10b08a18c32/general_enclosed_foundicons.scssc`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/1ea694b23cbc52b68bcbd397d07df10b08a18c32/general_enclosed_foundicons_ie7.scssc` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/general_enclosed/.sass-cache/1ea694b23cbc52b68bcbd397d07df10b08a18c32/general_enclosed_foundicons_ie7.scssc`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/sass/social_foundicons_ie7.scss` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/sass/social_foundicons_ie7.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/sass/social_foundicons.scss` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/sass/social_foundicons.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/sass/_settings.scss` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/sass/_settings.scss`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/stylesheets/social_foundicons_ie7.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/stylesheets/social_foundicons_ie7.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/stylesheets/social_foundicons.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/stylesheets/social_foundicons.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/demo.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/demo.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.eot` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.eot`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.woff` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.woff`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.ttf` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.ttf`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/fonts/social_foundicons.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/0bd576c1f1487db9a103f544ad85fa8a0f88a6ea/_settings.scssc` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/0bd576c1f1487db9a103f544ad85fa8a0f88a6ea/_settings.scssc`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/0bd576c1f1487db9a103f544ad85fa8a0f88a6ea/social_foundicons.scssc` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/0bd576c1f1487db9a103f544ad85fa8a0f88a6ea/social_foundicons.scssc`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/0bd576c1f1487db9a103f544ad85fa8a0f88a6ea/social_foundicons_ie7.scssc` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/2/social/.sass-cache/0bd576c1f1487db9a103f544ad85fa8a0f88a6ea/social_foundicons_ie7.scssc`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.woff` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.woff`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/preview.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/preview.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-trees.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-trees.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-steam.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-steam.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-layout.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-layout.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-zoom-in.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-zoom-in.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-burst.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-burst.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-male-female.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-male-female.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-calendar.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-calendar.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-euro.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-euro.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-trend.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-trend.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-contrast.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-contrast.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-upload.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-upload.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-trophy.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-trophy.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-remove.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-remove.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-home.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-home.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-xbox.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-xbox.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-play.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-play.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-no-dogs.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-no-dogs.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-sheriff-badge.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-sheriff-badge.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pencil.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pencil.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-price-tag.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-price-tag.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-wheelchair.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-wheelchair.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-address-book.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-address-book.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mobile.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mobile.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-sound.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-sound.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-usb.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-usb.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-credit-card.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-credit-card.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-annotate.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-annotate.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torso-female.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torso-female.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-star.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-star.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-microphone.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-microphone.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-stumbleupon.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-stumbleupon.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-foot.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-foot.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-database.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-database.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-left.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-left.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-six.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-six.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-universal-access.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-universal-access.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-burst-new.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-burst-new.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-minus.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-minus.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-underline.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-underline.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-web.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-web.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paperclip.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paperclip.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-eject.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-eject.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shopping-cart.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shopping-cart.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-csv.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-csv.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-folder-add.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-folder-add.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list-number.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list-number.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-blind.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-blind.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-html5.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-html5.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-google-plus.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-google-plus.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-male-female.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-male-female.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-at-sign.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-at-sign.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-forrst.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-forrst.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-treehouse.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-treehouse.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-yelp.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-yelp.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-delicious.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-delicious.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-cloud.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-cloud.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-dropbox.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-dropbox.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-safety-cone.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-safety-cone.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-two.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-two.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-male.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-male.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-blogger.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-blogger.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comments.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comments.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-eye.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-eye.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-hi5.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-hi5.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-skull.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-skull.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-rdio.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-rdio.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-prohibited.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-prohibited.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-video.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-video.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pricetag-multiple.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pricetag-multiple.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-indent-more.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-indent-more.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-game-center.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-game-center.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-alert.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-alert.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-asl.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-asl.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-volume-none.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-volume-none.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-filter.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-filter.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-italic.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-italic.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-strikethrough.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-skillshare.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-skillshare.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-spotify.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-spotify.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clipboard.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clipboard.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-power.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-power.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-joomla.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-joomla.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-magnifying-glass.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-magnifying-glass.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-volume.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-volume.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-stop.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-stop.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bluetooth.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bluetooth.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-dollar-bill.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-dollar-bill.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-medium.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-medium.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mobile-signal.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mobile-signal.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-zoom-out.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-zoom-out.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-folder-lock.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-folder-lock.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clock.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clock.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-fast-forward.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-fast-forward.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-lightbulb.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-lightbulb.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-camera.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-camera.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-minus-circle.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-minus-circle.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-indent-less.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-indent-less.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-compass.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-compass.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bold.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bold.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-tumblr.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-tumblr.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export-doc.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export-doc.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-squidoo.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-squidoo.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-share.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-share.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-right.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-right.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-deviant-art.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-deviant-art.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-edit.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-edit.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-expand.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-expand.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-target.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-target.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-x-circle.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-x-circle.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-dollar.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-dollar.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-telephone.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-telephone.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-no-smoking.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-no-smoking.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-compress.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-compress.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-play-circle.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-play-circle.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-pinterest.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-pinterest.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-marker.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-marker.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-vimeo.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-vimeo.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-download.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-download.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-text-color.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-text-color.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-search.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-search.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-bing.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-bing.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-battery-full.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-battery-full.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-linkedin.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-linkedin.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-laptop.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-laptop.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-add.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-add.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-instagram.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-instagram.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-elevator.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-elevator.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-female.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-female.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-snapchat.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-snapchat.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-map.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-map.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-horizontal.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-horizontal.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-yahoo.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-yahoo.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-five.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-five.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-plus.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-plus.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-right.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-right.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-lastfm.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-lastfm.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-reddit.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-reddit.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-male-symbol.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-male-symbol.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-android.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-android.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-braille.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-braille.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-wrench.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-wrench.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-doc.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-doc.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-anchor.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-anchor.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-unlink.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-unlink.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-css3.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-css3.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-key.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-key.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-evernote.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-evernote.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-thumbnails.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-thumbnails.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-photo.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-photo.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-unlock.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-unlock.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-up.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-crown.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-crown.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-superscript.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-superscript.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torso.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torso.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-zurb.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-zurb.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-upload-cloud.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-upload-cloud.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-asterisk.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-asterisk.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-first-aid.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-first-aid.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-dribbble.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-dribbble.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export-csv.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export-csv.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-refresh.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-refresh.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-multiple.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-multiple.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-dislike.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-dislike.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-background-color.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-background-color.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-record.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-record.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-next.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-next.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-out.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-out.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-twitter.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-twitter.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-hacker-news.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-hacker-news.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-guide-dog.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-guide-dog.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export-pdf.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-export-pdf.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-ticket.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-ticket.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-projection-screen.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-projection-screen.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-flag.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-flag.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-in.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrows-in.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-skype.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-skype.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-four.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-four.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-justify.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-justify.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-rewind.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-rewind.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torso-business.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torso-business.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-like.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-like.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-left.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-left.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-link.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-link.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-puzzle.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-puzzle.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-down.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-arrow-down.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-tablet-landscape.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-tablet-landscape.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mountains.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mountains.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-all-female.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-all-female.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment-quotes.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment-quotes.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-play-video.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-play-video.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paypal.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paypal.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-facebook.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-facebook.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-delete.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-delete.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-print.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-print.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shield.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shield.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-battery-empty.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-battery-empty.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-drive.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-drive.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-windows.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-windows.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-loop.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-loop.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-volume-strike.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-volume-strike.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-megaphone.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-megaphone.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-target-two.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-target-two.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-female-symbol.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-female-symbol.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-youtube.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-youtube.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paw.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paw.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-crop.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-crop.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-heart.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-heart.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-telephone-accessible.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-telephone-accessible.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pause.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pause.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-picasa.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-picasa.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-apple.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-apple.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-filled.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-filled.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-save.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-save.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-stack-overflow.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-stack-overflow.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paint-bucket.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-paint-bucket.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-foundation.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-foundation.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-check.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-check.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-subscript.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-subscript.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shopping-bag.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shopping-bag.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-all.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-all.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mail.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-mail.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-rss.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-rss.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-book.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-book.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-lock.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-lock.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-female-male.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-torsos-female-male.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-digg.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-digg.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list-thumbnails.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list-thumbnails.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-book-bookmark.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-book-bookmark.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-behance.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-behance.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-results.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-results.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-hearing-aid.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-hearing-aid.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-monitor.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-monitor.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-three.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-three.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-widget.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-widget.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-trash.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-trash.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clipboard-notes.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clipboard-notes.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-bar.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-bar.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-foursquare.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-foursquare.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-500px.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-500px.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-folder.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-folder.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-orkut.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-orkut.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-one.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-die-one.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-adobe.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-adobe.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-copy.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-copy.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-burst-sale.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-burst-sale.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pound.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-pound.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-pie.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-graph-pie.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-results-demographics.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-results-demographics.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-archive.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-archive.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-info.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-info.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-designer-news.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-designer-news.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-quote.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-quote.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment-video.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment-video.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-music.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-music.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-smashing-mag.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-smashing-mag.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-yen.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-yen.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-battery-half.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-battery-half.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment-minus.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment-minus.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-zerply.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-zerply.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-rewind-ten.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-rewind-ten.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-comment.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-center.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-align-center.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-closed-caption.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-closed-caption.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shuffle.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-shuffle.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-previous.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-previous.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-github.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-github.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bitcoin-circle.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bitcoin-circle.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-myspace.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-myspace.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-pdf.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-page-pdf.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-x.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-x.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clipboard-pencil.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-clipboard-pencil.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bookmark.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bookmark.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-flickr.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-flickr.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-tablet-portrait.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-tablet-portrait.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-checkbox.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-checkbox.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-path.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-path.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bitcoin.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-bitcoin.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list-bullet.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-list-bullet.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-amazon.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/svgs/fi-social-amazon.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/.fontcustom-data` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/.fontcustom-data`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.eot` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.eot`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.ttf` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/icons/3/icons/foundation-icons.ttf`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/index.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/index.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/css/normalize.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/css/normalize.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation_fobi_extras.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation_fobi_extras.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation_template-4.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation_template-4.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation-datepicker.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation-datepicker.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation-datetimepicker.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation-datetimepicker.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation.min.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/static/foundation5/css/foundation.min.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/fobi_themes.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/fobi_themes.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/dashboard.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/_base.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/_base.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/forms_list.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/forms_list.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/edit_form_entry_ajax.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/edit_form_entry_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/form_properties_snippet.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/form_properties_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/form_ajax.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/form_ajax.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/form_snippet.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/snippets/form_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/foundation5/templates/foundation5/theme.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/foundation5/templates/foundation5/theme.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/dummy_bootstrap3_widget/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/dummy_bootstrap3_widget/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/dummy_bootstrap3_widget/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/dummy_bootstrap3_widget/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/datetime_bootstrap3_widget/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/date_bootstrap3_widget/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/js/fobi.plugin.slider-bootstrap3-widget.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/js/fobi.plugin.slider-bootstrap3-widget.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/js/bootstrap-slider.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/js/bootstrap-slider.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/js/bootstrap-slider.min.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/js/bootstrap-slider.min.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/css/bootstrap-slider.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/css/bootstrap-slider.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/css/fobi.plugin.slider-bootstrap3-widget.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/css/fobi.plugin.slider-bootstrap3-widget.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/css/bootstrap-slider.min.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/static/bootstrap3/css/bootstrap-slider.min.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/widgets/form_elements/slider_bootstrap3_widget/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap3_fobi_extras.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap3_fobi_extras.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap-datetimepicker.min.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap.min.js` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap-theme.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap.min.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap-datetimepicker.min.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap-datetimepicker.min.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap-theme.min.css` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.svg` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.woff` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.eot` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.ttf` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/static/bootstrap3/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/fobi_themes.py` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/fobi_themes.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/_base.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/_base.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_properties_snippet.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_properties_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_non_field_and_hidden_errors_snippet.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_non_field_and_hidden_errors_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_wizard_snippet.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_wizard_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_snippet.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_wizard_properties_snippet.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/snippets/form_wizard_properties_snippet.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/theme.html` & `django-fobi-0.9.9/src/fobi/contrib/themes/bootstrap3/templates/bootstrap3/theme.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_model_object/settings.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_model_object/settings.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_model_object/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_model_object/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_model_object/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_model_object/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_model_object/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_model_object/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_model_object/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_model_object/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/fields.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_with_max/fields.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date_drop_down/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/textarea/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/textarea/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/textarea/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/textarea/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/integer/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/integer/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/integer/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/integer/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/date/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/date/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/ip_address/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/ip_address/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/ip_address/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/ip_address/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/password/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/password/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/password/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/password/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/settings.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/settings.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_model_objects/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden_model_object/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/input/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/input/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/input/constants.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/input/constants.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/input/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/input/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/regex/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/regex/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/regex/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/regex/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/regex/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/regex/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slug/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slug/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slug/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slug/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/email/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/email/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/email/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/email/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/text/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/text/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/text/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/text/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/settings.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/settings.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple_mptt_model_objects/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slider/widgets.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/widgets.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slider/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slider/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/forms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django import forms
 from django.utils.translation import ugettext_lazy as _
 
 from fobi.base import BaseFormFieldPluginForm, get_theme
+from fobi.helpers import get_select_field_choices
 from fobi.widgets import NumberInput
 
 from .constants import (
     SLIDER_DEFAULT_TOOLTIP,
     SLIDER_DEFAULT_HANDLE,
     SLIDER_DEFAULT_SHOW_ENDPOINTS_AS,
     SLIDER_TOOLTIP_CHOICES,
@@ -40,15 +41,15 @@
         ("step", STEP),
         ("tooltip", SLIDER_DEFAULT_TOOLTIP),
         ("handle", SLIDER_DEFAULT_HANDLE),
         # ("disable_slider_background", False),
         ("show_endpoints_as", SLIDER_DEFAULT_SHOW_ENDPOINTS_AS),
         ("label_start", ""),
         ("label_end", ""),
-        # ("custom_ticks", ""),
+        ("custom_ticks", ""),
         ("help_text", ""),
         ("required", False)
     ]
 
     label = forms.CharField(
         label=_("Label"),
         required=True,
@@ -136,35 +137,35 @@
         label=_("End label"),
         help_text=_("End endpoint label"),
         required=False,
         widget=forms.widgets.TextInput(
             attrs={'class': theme.form_element_html_class}
         )
     )
-    # custom_ticks = forms.CharField(
-    #     label=_("Custom ticks"),
-    #     required=False,
-    #     help_text=_("Enter single values/pairs per line. Example:<code><br/>"
-    #                 "&nbsp;&nbsp;&nbsp;&nbsp;1<br/>"
-    #                 "&nbsp;&nbsp;&nbsp;&nbsp;2<br/>"
-    #                 "&nbsp;&nbsp;&nbsp;&nbsp;3, Alpha<br/>"
-    #                 "&nbsp;&nbsp;&nbsp;&nbsp;4, Beta<br/>"
-    #                 "</code><br/>"
-    #                 "It finally transforms into the following HTML "
-    #                 "code:<code><br/>"
-    #                 '&nbsp;&nbsp;&nbsp;&nbsp;'
-    #                 'data-slider-ticks="[1, 2, 3, 4]"<br/>'
-    #                 '&nbsp;&nbsp;&nbsp;&nbsp;'
-    #                 "data-slider-ticks-labels='"
-    #                 '["1", "2", "Alpha", "Beta"]'
-    #                 "'</code>"),
-    #     widget=forms.widgets.Textarea(
-    #         attrs={'class': theme.form_element_html_class}
-    #     )
-    # )
+    custom_ticks = forms.CharField(
+        label=_("Custom ticks"),
+        required=False,
+        help_text=_("Enter single values/pairs per line. Example:<code><br/>"
+                    "&nbsp;&nbsp;&nbsp;&nbsp;1<br/>"
+                    "&nbsp;&nbsp;&nbsp;&nbsp;2<br/>"
+                    "&nbsp;&nbsp;&nbsp;&nbsp;3, Alpha<br/>"
+                    "&nbsp;&nbsp;&nbsp;&nbsp;4, Beta<br/>"
+                    "</code><br/>"
+                    "It finally transforms into the following HTML "
+                    "code:<code><br/>"
+                    '&nbsp;&nbsp;&nbsp;&nbsp;'
+                    'data-slider-ticks="[1, 2, 3, 4]"<br/>'
+                    '&nbsp;&nbsp;&nbsp;&nbsp;'
+                    "data-slider-ticks-labels='"
+                    '["1", "2", "Alpha", "Beta"]'
+                    "'</code>"),
+        widget=forms.widgets.Textarea(
+            attrs={'class': theme.form_element_html_class}
+        )
+    )
     help_text = forms.CharField(
         label=_("Help text"),
         required=False,
         widget=forms.widgets.TextInput(
             attrs={'class': theme.form_element_html_class}
         )
     )
@@ -182,14 +183,15 @@
 
         max_value = self.cleaned_data['max_value']
         min_value = self.cleaned_data['min_value']
         initial = self.cleaned_data['initial']
         step = self.cleaned_data['step']
         show_endpoints_as = self.cleaned_data['show_endpoints_as']
         handle = self.cleaned_data['handle']
+        custom_ticks = self.cleaned_data['custom_ticks']
 
         if max_value < min_value:
             self.add_error(
                 'max_value',
                 _("`max_value` should be > than `min_value`.")
             )
 
@@ -218,7 +220,21 @@
         )
         if handle in label_handles and show_endpoints_as in tick_endpoints:
             self.add_error(
                 'handle',
                 _("You are not allowed to use Triangle or Custom handles "
                   "with ticks enabled.")
             )
+
+        if custom_ticks:
+            ticks = get_select_field_choices(
+                custom_ticks,
+                key_type=int,
+                value_type=str,
+                fail_silently=False
+            )
+            if ticks is None:
+                self.add_error(
+                    'custom_ticks',
+                    _("Invalid format. First value should be an integer, "
+                      "second value should be a string.")
+                )
```

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slider/constants.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/constants.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/slider/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/slider/fobi_form_elements.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,26 +2,32 @@
 
 from django.forms.fields import ChoiceField
 from django.forms.utils import flatatt
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django.utils.translation import ugettext_lazy as _
 
-from fobi.base import FormFieldPlugin, form_element_plugin_registry, get_theme
+from fobi.base import (
+    FormFieldPlugin,
+    form_element_plugin_registry,
+    get_theme
+)
+from fobi.helpers import get_select_field_choices
 from fobi.widgets import RichSelect
 
 from . import UID
 from .constants import (
     SLIDER_DEFAULT_TOOLTIP,
     SLIDER_DEFAULT_HANDLE,
     SLIDER_SHOW_ENDPOINTS_AS_LABELED_TICKS,
     SLIDER_SHOW_ENDPOINTS_AS_TICKS,
     SLIDER_DEFAULT_SHOW_ENDPOINTS_AS
 )
 from .forms import SliderInputForm
+from .helpers import generate_ticks
 from .settings import INITIAL, MAX_VALUE, MIN_VALUE, STEP
 
 __title__ = 'fobi.contrib.plugins.form_elements.fields.slider.' \
             'fobi_form_elements'
 __author__ = 'Artur Barseghyan <artur.barseghyan@gmail.com>'
 __copyright__ = '2014-2016 Artur Barseghyan'
 __license__ = 'GPL 2.0/LGPL 2.1'
@@ -49,17 +55,19 @@
         tooltip = self.data.tooltip \
             if self.data.tooltip \
             else SLIDER_DEFAULT_TOOLTIP
         handle = self.data.handle \
             if self.data.handle \
             else SLIDER_DEFAULT_HANDLE
 
-        # custom_ticks = get_select_field_choices(self.data.custom_ticks) \
-        #     if self.data.custom_ticks \
-        #     else []
+        custom_ticks = get_select_field_choices(self.data.custom_ticks,
+                                                key_type=int,
+                                                value_type=text_type) \
+            if self.data.custom_ticks \
+            else []
 
         _choices = range(min_value, max_value+1, step)
         choices = zip(_choices, _choices)
 
         # slider_html_class = "slider-no-background" \
         #     if self.data.disable_slider_background \
         #     else "slider"
@@ -84,42 +92,61 @@
 
         prepend_html_list = []
         append_html_list = []
 
         # Show endpoints as labeled ticks
         if SLIDER_SHOW_ENDPOINTS_AS_LABELED_TICKS == show_endpoints_as:
 
-            label_start = self.data.label_start \
-                if self.data.label_start \
-                else text_type(min_value)
-
-            label_end = self.data.label_end \
-                if self.data.label_end \
-                else text_type(max_value)
-
-            widget_attrs.update({
-                'data-slider-ticks': "[{0}, {1}]".format(
-                    min_value, max_value
-                ),
-                'data-slider-ticks-labels': '["{0!s}", "{1!s}"]'.format(
-                    label_start.encode('utf8'), label_end.encode('utf8')
-                ),
-            })
+            if custom_ticks:
+                ticks_data = generate_ticks(custom_ticks)
+            else:
+                ticks_data = generate_ticks([
+                    (min_value, self.data.label_start),
+                    (max_value, self.data.label_end),
+                ])
+            # label_start = self.data.label_start \
+            #     if self.data.label_start \
+            #     else text_type(min_value)
+            #
+            # label_end = self.data.label_end \
+            #     if self.data.label_end \
+            #     else text_type(max_value)
+
+            # widget_attrs.update({
+            #     'data-slider-ticks': "[{0}, {1}]".format(
+            #         min_value, max_value
+            #     ),
+            #     'data-slider-ticks-labels': '["{0!s}", "{1!s}"]'.format(
+            #         label_start.encode('utf8'), label_end.encode('utf8')
+            #     ),
+            # })
+
+            widget_attrs.update(ticks_data)
 
         # Show endpoints as ticks
         elif SLIDER_SHOW_ENDPOINTS_AS_TICKS == show_endpoints_as:
 
-            widget_attrs.update({
-                'data-slider-ticks': "[{0}, {1}]".format(
-                    min_value, max_value
-                ),
-                'data-slider-ticks-labels': '["{0}", "{1}"]'.format(
-                    "", ""
-                ),
-            })
+            if custom_ticks:
+                ticks_data = generate_ticks(custom_ticks, empty_labels=True)
+            else:
+                ticks_data = generate_ticks([
+                    (min_value, ""),
+                    (max_value, ""),
+                ])
+
+            # widget_attrs.update({
+            #     'data-slider-ticks': "[{0}, {1}]".format(
+            #         min_value, max_value
+            #     ),
+            #     'data-slider-ticks-labels': '["{0}", "{1}"]'.format(
+            #         "", ""
+            #     ),
+            # })
+
+            widget_attrs.update(ticks_data)
 
         # Show endpoints as labels
         else:
 
             if self.data.label_start:
                 prepend_html_list.append(
                     format_html(
```

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/settings.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/settings.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_mptt_model_object/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/float/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/float/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/float/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/float/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/radio/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/radio/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/radio/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/radio/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/radio/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/radio/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/url/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/url/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/url/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/url/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/settings.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/settings.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/checkbox_select_multiple/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/boolean/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/boolean/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/boolean/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/boolean/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select_multiple/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select_multiple/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/time/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/time/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/time/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/time/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/time/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/time/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/hidden/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/hidden/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/null_boolean/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/null_boolean/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/null_boolean/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/null_boolean/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/select/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/select/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/range_select/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/range_select/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/range_select/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/range_select/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/range_select/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/range_select/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/decimal/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/decimal/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/decimal/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/decimal/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/decimal/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/decimal/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/datetime/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/datetime/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/datetime/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/datetime/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/datetime/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/datetime/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/file/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/file/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/file/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/file/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/fields/file/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/fields/file/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/honeypot/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/honeypot/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/honeypot/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/honeypot/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/honeypot/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/honeypot/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/honeypot/fields.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/honeypot/fields.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/recaptcha/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/recaptcha/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/recaptcha/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/recaptcha/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/captcha/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/captcha/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/security/captcha/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/security/captcha/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/test/dummy/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/test/dummy/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_text/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_text/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_text/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_text/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_video/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_video/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_video/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_video/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_video/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_video/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_video/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_video/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/settings.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/settings.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/defaults.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/defaults.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/helpers.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/helpers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/fobi_form_elements.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/fobi_form_elements.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/apps.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/apps.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_elements/content/content_image/templates/content_image/render.html` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_elements/content/content_image/templates/content_image/render.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/fobi_form_handlers.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/fobi_form_handlers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/widgets.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/widgets.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/helpers.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/helpers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/mail/fields.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/mail/fields.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/fobi_form_handlers.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/fobi_form_handlers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/models.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/models.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/migrations/0002_savedformwizarddataentry.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/migrations/0002_savedformwizarddataentry.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/migrations/0001_initial.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/views.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/views.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/urls/form_handlers.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/urls/form_handlers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/urls/form_wizard_handlers.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/urls/form_wizard_handlers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/widgets.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/widgets.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/js/jquery.expander.min.js` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/js/jquery.expander.min.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/js/jquery.expander.license.txt` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/js/jquery.expander.license.txt`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/js/db_store.js` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/static/db_store/js/db_store.js`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/helpers.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/helpers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/admin.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/admin.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/templates/db_store/view_saved_form_wizard_data_entries.html` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/templates/db_store/view_saved_form_wizard_data_entries.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/db_store/templates/db_store/view_saved_form_data_entries.html` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/db_store/templates/db_store/view_saved_form_data_entries.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/http_repost/fobi_form_handlers.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/http_repost/fobi_form_handlers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_handlers/http_repost/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_handlers/http_repost/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_importers/mailchimp_importer/views.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_importers/mailchimp_importer/views.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_importers/mailchimp_importer/forms.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_importers/mailchimp_importer/forms.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/plugins/form_importers/mailchimp_importer/fobi_form_importers.py` & `django-fobi-0.9.9/src/fobi/contrib/plugins/form_importers/mailchimp_importer/fobi_form_importers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/models.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/models.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/settings.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/settings.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/helpers.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/helpers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/djangocms_integration/cms_plugins.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/djangocms_integration/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/wagtail_integration_/models.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/wagtail_integration_/models.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/wagtail_integration_/settings.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/wagtail_integration_/settings.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/wagtail_integration_/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/wagtail_integration_/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/wagtail_integration_/helpers.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/wagtail_integration_/helpers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/models.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/models.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/settings.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/settings.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/helpers.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/helpers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/page_processors.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/page_processors.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/templates/mezzanine_integration/admin/change_form.html` & `django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/templates/mezzanine_integration/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/mezzanine_integration/templates/pages/fobiformpage.html` & `django-fobi-0.9.9/src/fobi/contrib/apps/mezzanine_integration/templates/pages/fobiformpage.html`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/feincms_integration/settings.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/feincms_integration/settings.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/feincms_integration/widgets.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/feincms_integration/widgets.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/feincms_integration/conf.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/feincms_integration/conf.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/contrib/apps/feincms_integration/helpers.py` & `django-fobi-0.9.9/src/fobi/contrib/apps/feincms_integration/helpers.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/exceptions.py` & `django-fobi-0.9.9/src/fobi/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templatetags/fobi_tags.py` & `django-fobi-0.9.9/src/fobi/templatetags/fobi_tags.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/templatetags/future_compat.py` & `django-fobi-0.9.9/src/fobi/templatetags/future_compat.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/fobi/discover.py` & `django-fobi-0.9.9/src/fobi/discover.py`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/src/django_fobi.egg-info/SOURCES.txt` & `django-fobi-0.9.9/src/django_fobi.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -245,14 +245,15 @@
 src/fobi/contrib/plugins/form_elements/fields/slider/__init__.py
 src/fobi/contrib/plugins/form_elements/fields/slider/apps.py
 src/fobi/contrib/plugins/form_elements/fields/slider/conf.py
 src/fobi/contrib/plugins/form_elements/fields/slider/constants.py
 src/fobi/contrib/plugins/form_elements/fields/slider/defaults.py
 src/fobi/contrib/plugins/form_elements/fields/slider/fobi_form_elements.py
 src/fobi/contrib/plugins/form_elements/fields/slider/forms.py
+src/fobi/contrib/plugins/form_elements/fields/slider/helpers.py
 src/fobi/contrib/plugins/form_elements/fields/slider/settings.py
 src/fobi/contrib/plugins/form_elements/fields/slider/widgets.py
 src/fobi/contrib/plugins/form_elements/fields/slug/__init__.py
 src/fobi/contrib/plugins/form_elements/fields/slug/apps.py
 src/fobi/contrib/plugins/form_elements/fields/slug/fobi_form_elements.py
 src/fobi/contrib/plugins/form_elements/fields/slug/forms.py
 src/fobi/contrib/plugins/form_elements/fields/text/__init__.py
```

### Comparing `django-fobi-0.9.8/src/django_fobi.egg-info/PKG-INFO` & `django-fobi-0.9.9/src/django_fobi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-fobi
-Version: 0.9.8
+Version: 0.9.9
 Summary: Form generator/builder application for Django done right: customisable, modular, user- and developer- friendly.
 Home-page: https://github.com/barseghyanartur/django-fobi/
 Author: Artur Barseghyan
 Author-email: artur.barseghyan@gmail.com
 License: GPL 2.0/LGPL 2.1
 Description: ===========
         django-fobi
```

### Comparing `django-fobi-0.9.8/MANIFEST.in` & `django-fobi-0.9.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/setup.cfg` & `django-fobi-0.9.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/LICENSE_GPL2.0.txt` & `django-fobi-0.9.9/LICENSE_GPL2.0.txt`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/README.rst` & `django-fobi-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-fobi-0.9.8/setup.py` & `django-fobi-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 
 from distutils.version import LooseVersion
 from setuptools import setup, find_packages
 
-version = '0.9.8'
+version = '0.9.9'
 
 # ***************************************************************************
 # ************************** Django version *********************************
 # ***************************************************************************
 DJANGO_INSTALLED = False
 try:
     import django
```

### Comparing `django-fobi-0.9.8/CHANGELOG.rst` & `django-fobi-0.9.9/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 - It's always safe to upgrade within the same minor version (for example, from
   0.3 to 0.3.4).
 - Minor version changes might be backwards incompatible. Read the
   release notes carefully before upgrading (for example, when upgrading from
   0.3.4 to 0.4).
 - All backwards incompatible changes are mentioned in this document.
 
+0.9.9
+-----
+2016-10-31
+
+- Make it possible to add custom ticks to the `slider` plugin.
+
 0.9.8
 -----
 2016-10-27
 
 - Support multiple sliders in one form.
 
 0.9.7
```

### Comparing `django-fobi-0.9.8/PKG-INFO` & `django-fobi-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-fobi
-Version: 0.9.8
+Version: 0.9.9
 Summary: Form generator/builder application for Django done right: customisable, modular, user- and developer- friendly.
 Home-page: https://github.com/barseghyanartur/django-fobi/
 Author: Artur Barseghyan
 Author-email: artur.barseghyan@gmail.com
 License: GPL 2.0/LGPL 2.1
 Description: ===========
         django-fobi
```

