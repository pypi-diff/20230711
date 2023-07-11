# Comparing `tmp/allianceauth-3.4.0.tar.gz` & `tmp/allianceauth-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-3.4.0.tar", last modified: Tue Apr 25 11:33:30 2023, max compression
+gzip compressed data, was "allianceauth-3.5.0.tar", last modified: Tue Jul 11 03:16:08 2023, max compression
```

## Comparing `allianceauth-3.4.0.tar` & `allianceauth-3.5.0.tar`

### file list

```diff
@@ -1,903 +1,904 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.855531 allianceauth-3.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    18026 2023-04-25 11:33:08.000000 allianceauth-3.4.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-04-25 11:33:08.000000 allianceauth-3.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6285 2023-04-25 11:33:30.855531 allianceauth-3.4.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     4978 2023-04-25 11:33:08.000000 allianceauth-3.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.584512 allianceauth-3.4.0/allianceauth/
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.590512 allianceauth-3.4.0/allianceauth/analytics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.590512 allianceauth-3.4.0/allianceauth/analytics/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/fixtures/disable_analytics.json
--rw-rw-rw-   0 root         (0) root         (0)     2100 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.593512 allianceauth-3.4.0/allianceauth/analytics/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1664 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/migrations/0003_Generate_Identifier.py
--rw-rw-rw-   0 root         (0) root         (0)     1650 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/migrations/0004_auto_20211015_0502.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/migrations/0005_alter_analyticspath_ignore_path.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/migrations/0006_more_ignore_paths.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1496 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/signals.py
--rw-rw-rw-   0 root         (0) root         (0)     6605 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.595512 allianceauth-3.4.0/allianceauth/analytics/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4313 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)      783 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/tests/test_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)    10228 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/analytics/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.601513 allianceauth-3.4.0/allianceauth/authentication/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21206 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1345 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     5638 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/backends.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/checks.py
--rw-rw-rw-   0 root         (0) root         (0)     2486 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     2480 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/hmac_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.602513 allianceauth-3.4.0/allianceauth/authentication/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.603513 allianceauth-3.4.0/allianceauth/authentication/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/management/commands/checkmains.py
--rwxrwxrwx   0 root         (0) root         (0)     2709 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/managers.py
--rw-rw-rw-   0 root         (0) root         (0)     1999 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.611514 allianceauth-3.4.0/allianceauth/authentication/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     3147 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0002_auto_20160907_1914.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0003_authservicesinfo_state.py
--rw-rw-rw-   0 root         (0) root         (0)     2543 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0004_create_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1144 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0005_delete_perms.py
--rw-rw-rw-   0 root         (0) root         (0)     1324 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0006_auto_20160910_0542.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0007_remove_authservicesinfo_is_blue.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0008_set_state.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0009_auto_20161021_0228.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1914 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0013_service_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0014_fleetup_permission.py
--rw-rw-rw-   0 root         (0) root         (0)    13077 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0015_user_profiles.py
--rw-rw-rw-   0 root         (0) root         (0)     1637 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0016_ownershiprecord.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0018_alter_state_name_length.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0018_state_member_factions.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0019_merge_20211026_0919.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/migrations/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5632 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/models.py
--rw-rw-rw-   0 root         (0) root         (0)     7806 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.530508 allianceauth-3.4.0/allianceauth/authentication/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.530508 allianceauth-3.4.0/allianceauth/authentication/static/allianceauth/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.530508 allianceauth-3.4.0/allianceauth/authentication/static/allianceauth/authentication/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.611514 allianceauth-3.4.0/allianceauth/authentication/static/allianceauth/authentication/css/
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/static/allianceauth/authentication/css/admin.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.611514 allianceauth-3.4.0/allianceauth/authentication/static/allianceauth/authentication/img/
--rw-rw-rw-   0 root         (0) root         (0)   161344 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.612514 allianceauth-3.4.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/
--rw-rw-rw-   0 root         (0) root         (0)     2308 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png
--rw-rw-rw-   0 root         (0) root         (0)     2248 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.614514 allianceauth-3.4.0/allianceauth/authentication/task_statistics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/task_statistics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1465 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/task_statistics/counters.py
--rw-rw-rw-   0 root         (0) root         (0)     4042 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/task_statistics/event_series.py
--rw-rw-rw-   0 root         (0) root         (0)     1123 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/task_statistics/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.616514 allianceauth-3.4.0/allianceauth/authentication/task_statistics/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/task_statistics/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/task_statistics/tests/test_counters.py
--rw-rw-rw-   0 root         (0) root         (0)     5843 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/task_statistics/tests/test_event_series.py
--rw-rw-rw-   0 root         (0) root         (0)     2918 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/task_statistics/tests/test_signals.py
--rw-rw-rw-   0 root         (0) root         (0)     1661 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.533508 allianceauth-3.4.0/allianceauth/authentication/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.616514 allianceauth-3.4.0/allianceauth/authentication/templates/authentication/
--rw-rw-rw-   0 root         (0) root         (0)    10738 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/templates/authentication/dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     2613 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/templates/authentication/tokens.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.618514 allianceauth-3.4.0/allianceauth/authentication/templates/public/
--rw-rw-rw-   0 root         (0) root         (0)     1944 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/templates/public/base.html
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/templates/public/lang_select.html
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/templates/public/login.html
--rw-rw-rw-   0 root         (0) root         (0)     1433 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/templates/public/middle_box.html
--rw-rw-rw-   0 root         (0) root         (0)      846 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/templates/public/register.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.620514 allianceauth-3.4.0/allianceauth/authentication/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/templates/registration/activate.html
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/templates/registration/activation_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/templates/registration/activation_email_html.txt
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/templates/registration/activation_email_subject.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.623515 allianceauth-3.4.0/allianceauth/authentication/tests/
--rw-rw-rw-   0 root         (0) root         (0)      833 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29475 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     3456 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/tests/test_app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     7427 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/tests/test_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     1517 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/tests/test_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     2452 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/tests/test_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6316 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/tests/test_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)    11478 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     3154 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/tests/test_signals.py
--rw-rw-rw-   0 root         (0) root         (0)    10983 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/tests/test_templatetags.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    11597 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/authentication/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.624514 allianceauth-3.4.0/allianceauth/bin/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/bin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3555 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/bin/allianceauth.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/context_processors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.629515 allianceauth-3.4.0/allianceauth/corputils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1970 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.632515 allianceauth-3.4.0/allianceauth/corputils/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     5358 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/migrations/0002_migrate_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/migrations/0003_granular_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/migrations/0004_member_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/migrations/0005_cleanup_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7223 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/models.py
--rw-rw-rw-   0 root         (0) root         (0)   947431 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/swagger.json
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.534508 allianceauth-3.4.0/allianceauth/corputils/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.633515 allianceauth-3.4.0/allianceauth/corputils/templates/corputils/
--rw-rw-rw-   0 root         (0) root         (0)     2100 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/templates/corputils/base.html
--rw-rw-rw-   0 root         (0) root         (0)    14915 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/templates/corputils/corpstats.html
--rw-rw-rw-   0 root         (0) root         (0)     2540 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/templates/corputils/search.html
--rw-rw-rw-   0 root         (0) root         (0)    16016 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     6999 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/corputils/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.636515 allianceauth-3.4.0/allianceauth/eveonline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7277 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.638516 allianceauth-3.4.0/allianceauth/eveonline/autogroups/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/autogroups/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1347 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/autogroups/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/autogroups/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.639515 allianceauth-3.4.0/allianceauth/eveonline/autogroups/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     4024 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/autogroups/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/autogroups/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10691 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/autogroups/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/autogroups/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.640516 allianceauth-3.4.0/allianceauth/eveonline/autogroups/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1403 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/autogroups/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3221 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/autogroups/tests/test_managers.py
--rw-rw-rw-   0 root         (0) root         (0)    12356 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/autogroups/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     7961 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/autogroups/tests/test_signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.642516 allianceauth-3.4.0/allianceauth/eveonline/evelinks/
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/evelinks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1496 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/evelinks/dotlan.py
--rw-rw-rw-   0 root         (0) root         (0)     3730 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/evelinks/eveimageserver.py
--rw-rw-rw-   0 root         (0) root         (0)     1229 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/evelinks/evewho.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.643516 allianceauth-3.4.0/allianceauth/eveonline/evelinks/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/evelinks/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7329 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/evelinks/tests/test_evelinks.py
--rw-rw-rw-   0 root         (0) root         (0)    11505 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/evelinks/tests/test_templatetags.py
--rw-rw-rw-   0 root         (0) root         (0)     1700 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/evelinks/zkillboard.py
--rw-rw-rw-   0 root         (0) root         (0)     3350 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.650516 allianceauth-3.4.0/allianceauth/eveonline/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     3133 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0002_remove_eveapikeypair_error_count.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0004_eveapikeypair_sso_verified.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0005_remove_eveallianceinfo_member_count.py
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py
--rw-rw-rw-   0 root         (0) root         (0)     4599 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0007_unique_id_name.py
--rw-rw-rw-   0 root         (0) root         (0)      854 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0008_remove_apikeys.py
--rw-rw-rw-   0 root         (0) root         (0)      519 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0009_on_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0010_alliance_ticker.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0011_ids_to_integers.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0012_index_additions.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0013_evecorporationinfo_ceo_id.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0014_auto_20210105_1413.py
--rw-rw-rw-   0 root         (0) root         (0)     1201 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0015_factions.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0016_character_names_are_not_unique.py
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14052 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/models.py
--rw-rw-rw-   0 root         (0) root         (0)     9958 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/providers.py
--rw-rw-rw-   0 root         (0) root         (0)    41989 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/swagger.json
--rw-rw-rw-   0 root         (0) root         (0)     3808 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.651517 allianceauth-3.4.0/allianceauth/eveonline/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8354 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/templatetags/evelinks.py
--rw-rw-rw-   0 root         (0) root         (0)     4166 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/templatetags/examples.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.654517 allianceauth-3.4.0/allianceauth/eveonline/tests/
--rw-rw-rw-   0 root         (0) root         (0)      739 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6043 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/tests/esi_client_stub.py
--rw-rw-rw-   0 root         (0) root         (0)   297070 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/tests/swagger_old.json
--rw-rw-rw-   0 root         (0) root         (0)    10079 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/tests/test_managers.py
--rw-rw-rw-   0 root         (0) root         (0)    23361 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)    23834 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/tests/test_providers.py
--rw-rw-rw-   0 root         (0) root         (0)    10117 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/tests/test_tasks.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/eveonline/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.659517 allianceauth-3.4.0/allianceauth/fleetactivitytracking/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.661517 allianceauth-3.4.0/allianceauth/fleetactivitytracking/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/migrations/0002_auto_20160905_2220.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/migrations/0003_auto_20160906_2354.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/migrations/0004_make_strings_more_stringy.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/migrations/0005_remove_fat_name.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/migrations/0006_auto_20180803_0430.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/models.py
--rw-rw-rw-   0 root         (0) root         (0)   947431 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/swagger.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.538509 allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.664517 allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/
--rw-rw-rw-   0 root         (0) root         (0)     1340 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html
--rw-rw-rw-   0 root         (0) root         (0)     1208 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkformatter.html
--rw-rw-rw-   0 root         (0) root         (0)     2680 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html
--rw-rw-rw-   0 root         (0) root         (0)     3200 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html
--rw-rw-rw-   0 root         (0) root         (0)     1485 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html
--rw-rw-rw-   0 root         (0) root         (0)     2227 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html
--rw-rw-rw-   0 root         (0) root         (0)     2415 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html
--rw-rw-rw-   0 root         (0) root         (0)     4384 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html
--rw-rw-rw-   0 root         (0) root         (0)     1386 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    16667 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/fleetactivitytracking/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.668518 allianceauth-3.4.0/allianceauth/groupmanagement/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8978 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1370 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.676518 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2243 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0003_default_groups.py
--rw-rw-rw-   0 root         (0) root         (0)     4324 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0004_authgroup.py
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0005_authgroup_public.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0007_on_delete.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1100 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0009_requestlog.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0010_authgroup_states.py
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0011_requestlog_date.py
--rw-rw-rw-   0 root         (0) root         (0)      672 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0012_group_leads.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0013_fix_requestlog_date_field.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0014_auto_20200918_1412.py
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0016_remove_grouprequest_status_field.py
--rw-rw-rw-   0 root         (0) root         (0)     2296 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py
--rw-rw-rw-   0 root         (0) root         (0)      520 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8162 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1465 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/signals.py
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.540509 allianceauth-3.4.0/allianceauth/groupmanagement/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.679518 allianceauth-3.4.0/allianceauth/groupmanagement/templates/groupmanagement/
--rw-rw-rw-   0 root         (0) root         (0)     4886 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/templates/groupmanagement/audit.html
--rw-rw-rw-   0 root         (0) root         (0)     4784 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html
--rw-rw-rw-   0 root         (0) root         (0)     4195 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html
--rw-rw-rw-   0 root         (0) root         (0)     2948 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/templates/groupmanagement/groups.html
--rw-rw-rw-   0 root         (0) root         (0)     9513 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/templates/groupmanagement/index.html
--rw-rw-rw-   0 root         (0) root         (0)     1301 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/templates/groupmanagement/menu.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.681519 allianceauth-3.4.0/allianceauth/groupmanagement/tests/
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24713 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)    17375 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/tests/test_managers.py
--rw-rw-rw-   0 root         (0) root         (0)    11668 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     4950 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/tests/test_signals.py
--rw-rw-rw-   0 root         (0) root         (0)     3073 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)     1651 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/urls.py
--rwxrwxrwx   0 root         (0) root         (0)    19860 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/groupmanagement/views.py
--rw-rw-rw-   0 root         (0) root         (0)     4127 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.685519 allianceauth-3.4.0/allianceauth/hrapplications/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      717 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      987 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/auth_hooks.py
--rwxrwxrwx   0 root         (0) root         (0)      353 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.688519 allianceauth-3.4.0/allianceauth/hrapplications/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     6662 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/migrations/0002_choices_for_questions.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/migrations/0003_applicationquestion_multi_select.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py
--rw-rw-rw-   0 root         (0) root         (0)      558 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/migrations/0005_sorted_questions.py
--rw-rw-rw-   0 root         (0) root         (0)     1946 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/migrations/0007_auto_20200918_1412.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/migrations/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3237 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.541509 allianceauth-3.4.0/allianceauth/hrapplications/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.690519 allianceauth-3.4.0/allianceauth/hrapplications/templates/hrapplications/
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/templates/hrapplications/corpchoice.html
--rw-rw-rw-   0 root         (0) root         (0)     1915 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/templates/hrapplications/create.html
--rw-rw-rw-   0 root         (0) root         (0)    11885 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/templates/hrapplications/management.html
--rw-rw-rw-   0 root         (0) root         (0)     4107 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/templates/hrapplications/searchview.html
--rw-rw-rw-   0 root         (0) root         (0)     9294 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/templates/hrapplications/view.html
--rw-rw-rw-   0 root         (0) root         (0)     4165 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/tests.py
--rw-rw-rw-   0 root         (0) root         (0)     1113 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/urls.py
--rwxrwxrwx   0 root         (0) root         (0)    11984 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/hrapplications/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.547509 allianceauth-3.4.0/allianceauth/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.542509 allianceauth-3.4.0/allianceauth/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.690519 allianceauth-3.4.0/allianceauth/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    37872 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    84839 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.543509 allianceauth-3.4.0/allianceauth/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.691519 allianceauth-3.4.0/allianceauth/locale/en/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/en/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    70502 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.543509 allianceauth-3.4.0/allianceauth/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.692519 allianceauth-3.4.0/allianceauth/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    37814 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    84835 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.544509 allianceauth-3.4.0/allianceauth/locale/fr_FR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.693519 allianceauth-3.4.0/allianceauth/locale/fr_FR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    37724 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    85375 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.544509 allianceauth-3.4.0/allianceauth/locale/it_IT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.694519 allianceauth-3.4.0/allianceauth/locale/it_IT/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    17209 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/it_IT/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    77100 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/it_IT/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.545509 allianceauth-3.4.0/allianceauth/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.695520 allianceauth-3.4.0/allianceauth/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    41641 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/ja/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    88417 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.546509 allianceauth-3.4.0/allianceauth/locale/ko_KR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.696519 allianceauth-3.4.0/allianceauth/locale/ko_KR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    36909 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    84828 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.546509 allianceauth-3.4.0/allianceauth/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.697520 allianceauth-3.4.0/allianceauth/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    47123 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/ru/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    94195 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.547509 allianceauth-3.4.0/allianceauth/locale/uk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.698520 allianceauth-3.4.0/allianceauth/locale/uk/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    48143 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/uk/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    95082 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.547509 allianceauth-3.4.0/allianceauth/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.699520 allianceauth-3.4.0/allianceauth/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    27229 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    79576 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.702520 allianceauth-3.4.0/allianceauth/notifications/
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1113 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1320 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/core.py
--rw-rw-rw-   0 root         (0) root         (0)      998 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     3907 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.704520 allianceauth-3.4.0/allianceauth/notifications/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1117 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/migrations/0002_auto_20160910_1649.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/migrations/0004_performance_tuning.py
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/migrations/0005_fix_level_choices.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2772 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.548509 allianceauth-3.4.0/allianceauth/notifications/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.705520 allianceauth-3.4.0/allianceauth/notifications/templates/notifications/
--rw-rw-rw-   0 root         (0) root         (0)     1478 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/templates/notifications/list.html
--rw-rw-rw-   0 root         (0) root         (0)     1325 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/templates/notifications/list_partial.html
--rw-rw-rw-   0 root         (0) root         (0)      812 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/templates/notifications/view.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.706520 allianceauth-3.4.0/allianceauth/notifications/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/templatetags/auth_notifications.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.709520 allianceauth-3.4.0/allianceauth/notifications/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3073 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)     2392 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/tests/test_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     1120 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/tests/test_init.py
--rw-rw-rw-   0 root         (0) root         (0)     9437 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/tests/test_managers.py
--rw-rw-rw-   0 root         (0) root         (0)     2398 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     2975 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/tests/test_templatetags.py
--rw-rw-rw-   0 root         (0) root         (0)     1463 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     3519 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/notifications/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.713521 allianceauth-3.4.0/allianceauth/optimer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      763 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/form.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/form_widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.715521 allianceauth-3.4.0/allianceauth/optimer/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1452 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/migrations/0002_auto_20170413_0442.py
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/migrations/0004_on_delete.py
--rw-rw-rw-   0 root         (0) root         (0)     1447 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/migrations/0005_add_type_and_description.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1247 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.550509 allianceauth-3.4.0/allianceauth/optimer/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.716521 allianceauth-3.4.0/allianceauth/optimer/templates/optimer/
--rw-rw-rw-   0 root         (0) root         (0)     1486 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/templates/optimer/add.html
--rw-rw-rw-   0 root         (0) root         (0)     2630 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/templates/optimer/fleetoptable.html
--rw-rw-rw-   0 root         (0) root         (0)     3707 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/templates/optimer/management.html
--rw-rw-rw-   0 root         (0) root         (0)     1718 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/templates/optimer/update.html
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     5765 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/optimer/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.719521 allianceauth-3.4.0/allianceauth/permissions_tool/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/permissions_tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/permissions_tool/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      787 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/permissions_tool/auth_hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.720521 allianceauth-3.4.0/allianceauth/permissions_tool/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      589 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/permissions_tool/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/permissions_tool/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/permissions_tool/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.551509 allianceauth-3.4.0/allianceauth/permissions_tool/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.721521 allianceauth-3.4.0/allianceauth/permissions_tool/templates/permissions_tool/
--rw-rw-rw-   0 root         (0) root         (0)     3414 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/permissions_tool/templates/permissions_tool/audit.html
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html
--rw-rw-rw-   0 root         (0) root         (0)     4891 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/permissions_tool/templates/permissions_tool/overview.html
--rw-rw-rw-   0 root         (0) root         (0)     4968 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/permissions_tool/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/permissions_tool/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     2610 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/permissions_tool/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.722521 allianceauth-3.4.0/allianceauth/project_template/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/project_template/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.722521 allianceauth-3.4.0/allianceauth/project_template/log/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/project_template/log/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      821 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/project_template/manage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.724521 allianceauth-3.4.0/allianceauth/project_template/project_name/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/project_template/project_name/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/project_template/project_name/celery.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.725522 allianceauth-3.4.0/allianceauth/project_template/project_name/settings/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/project_template/project_name/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8741 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/project_template/project_name/settings/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2902 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/project_template/project_name/settings/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.725522 allianceauth-3.4.0/allianceauth/project_template/project_name/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/project_template/project_name/static/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.726522 allianceauth-3.4.0/allianceauth/project_template/project_name/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/project_template/project_name/templates/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/project_template/project_name/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/project_template/project_name/wsgi.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/project_template/supervisor.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.730522 allianceauth-3.4.0/allianceauth/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3954 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      656 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2117 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     8308 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.731522 allianceauth-3.4.0/allianceauth/services/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.731522 allianceauth-3.4.0/allianceauth/services/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      469 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/management/commands/verify_service_accounts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.733522 allianceauth-3.4.0/allianceauth/services/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      483 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/migrations/0001_squashed_0003_delete_groupcache.py
--rw-rw-rw-   0 root         (0) root         (0)     1220 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/migrations/0002_nameformatter.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/migrations/0003_remove_broken_link.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.733522 allianceauth-3.4.0/allianceauth/services/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.738523 allianceauth-3.4.0/allianceauth/services/modules/discord/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1024 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1290 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/api.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     4957 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     4446 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.740523 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    28936 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4590 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     3853 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.744523 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5027 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/example_objects.json
--rw-rw-rw-   0 root         (0) root         (0)     3013 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     2784 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py
--rw-rw-rw-   0 root         (0) root         (0)     4477 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md
--rw-rw-rw-   0 root         (0) root         (0)    56104 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/test_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9724 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     4966 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     6281 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.746523 allianceauth-3.4.0/allianceauth/services/modules/discord/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      680 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2067 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/migrations/0002_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1538 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7138 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/models.py
--rw-rw-rw-   0 root         (0) root         (0)     9517 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.557510 allianceauth-3.4.0/allianceauth/services/modules/discord/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.557510 allianceauth-3.4.0/allianceauth/services/modules/discord/templates/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.746523 allianceauth-3.4.0/allianceauth/services/modules/discord/templates/services/discord/
--rw-rw-rw-   0 root         (0) root         (0)     1428 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.751523 allianceauth-3.4.0/allianceauth/services/modules/discord/tests/
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/tests/factories.py
--rwxrwxrwx   0 root         (0) root         (0)     2639 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/tests/piloting_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)    10400 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)     6287 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     8456 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)    29543 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)    19956 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_managers.py
--rw-rw-rw-   0 root         (0) root         (0)    11474 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)    17995 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6783 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)      566 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     2561 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3635 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discord/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.755524 allianceauth-3.4.0/allianceauth/services/modules/discourse/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discourse/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discourse/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discourse/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1878 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discourse/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     7039 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discourse/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.756524 allianceauth-3.4.0/allianceauth/services/modules/discourse/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discourse/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2096 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discourse/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discourse/models.py
--rw-rw-rw-   0 root         (0) root         (0)      533 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discourse/providers.py
--rw-rw-rw-   0 root         (0) root         (0)     2273 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discourse/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.559510 allianceauth-3.4.0/allianceauth/services/modules/discourse/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.559510 allianceauth-3.4.0/allianceauth/services/modules/discourse/templates/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.757524 allianceauth-3.4.0/allianceauth/services/modules/discourse/templates/services/discourse/
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discourse/templates/services/discourse/discourse_service_ctrl.html
--rw-rw-rw-   0 root         (0) root         (0)     5209 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discourse/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discourse/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     3486 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/discourse/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.759524 allianceauth-3.4.0/allianceauth/services/modules/example/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/example/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/example/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1336 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/example/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/example/models.py
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/example/urls.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/example/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.762524 allianceauth-3.4.0/allianceauth/services/modules/ips4/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/ips4/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/ips4/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/ips4/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1554 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/ips4/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     4199 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/ips4/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.763524 allianceauth-3.4.0/allianceauth/services/modules/ips4/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      737 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/ips4/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/ips4/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      558 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/ips4/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/ips4/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     6035 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/ips4/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/ips4/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     4789 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/ips4/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.767525 allianceauth-3.4.0/allianceauth/services/modules/mumble/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      455 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     2958 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/auth_hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.772525 allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2868 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0002_auto_20161212_0100.py
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py
--rw-rw-rw-   0 root         (0) root         (0)     2063 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0008_mumbleuser_display_name.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0011_auto_20201011_1009.py
--rw-rw-rw-   0 root         (0) root         (0)     1508 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5630 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.561510 allianceauth-3.4.0/allianceauth/services/modules/mumble/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.561510 allianceauth-3.4.0/allianceauth/services/modules/mumble/templates/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.772525 allianceauth-3.4.0/allianceauth/services/modules/mumble/templates/services/mumble/
--rw-rw-rw-   0 root         (0) root         (0)     1336 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html
--rw-rw-rw-   0 root         (0) root         (0)     8632 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/mumble/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.776525 allianceauth-3.4.0/allianceauth/services/modules/openfire/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/openfire/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/openfire/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/openfire/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     3615 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/openfire/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/openfire/forms.py
--rwxrwxrwx   0 root         (0) root         (0)     8321 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/openfire/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.777525 allianceauth-3.4.0/allianceauth/services/modules/openfire/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      687 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/openfire/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2073 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/openfire/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/openfire/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2620 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/openfire/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.562510 allianceauth-3.4.0/allianceauth/services/modules/openfire/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.563510 allianceauth-3.4.0/allianceauth/services/modules/openfire/templates/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.778525 allianceauth-3.4.0/allianceauth/services/modules/openfire/templates/services/openfire/
--rwxrwxrwx   0 root         (0) root         (0)     1183 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html
--rw-rw-rw-   0 root         (0) root         (0)     9478 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/openfire/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/openfire/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     7688 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/openfire/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.782526 allianceauth-3.4.0/allianceauth/services/modules/phpbb3/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/phpbb3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/phpbb3/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/phpbb3/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/phpbb3/auth_hooks.py
--rwxrwxrwx   0 root         (0) root         (0)    13456 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/phpbb3/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.783526 allianceauth-3.4.0/allianceauth/services/modules/phpbb3/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      683 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/phpbb3/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2049 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/phpbb3/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/phpbb3/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/phpbb3/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     8189 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/phpbb3/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/phpbb3/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     5139 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/phpbb3/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.787526 allianceauth-3.4.0/allianceauth/services/modules/smf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/smf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/smf/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/smf/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/smf/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)    14780 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/smf/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.788526 allianceauth-3.4.0/allianceauth/services/modules/smf/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/smf/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/smf/migrations/0002_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      694 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/smf/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/smf/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3740 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/smf/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     8057 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/smf/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/smf/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     5143 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/smf/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.792526 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1860 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     2128 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/forms.py
--rwxrwxrwx   0 root         (0) root         (0)    12601 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.795527 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1995 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py
--rw-rw-rw-   0 root         (0) root         (0)      781 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py
--rw-rw-rw-   0 root         (0) root         (0)     2116 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      784 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1723 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/signals.py
--rw-rw-rw-   0 root         (0) root         (0)     3780 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.566511 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.565510 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/templates/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.565510 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/templates/admin/teamspeak3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.795527 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/templates/admin/teamspeak3/authts/
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/templates/admin/teamspeak3/authts/change_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.566511 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/templates/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.796527 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/
--rw-rw-rw-   0 root         (0) root         (0)     1330 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html
--rw-rw-rw-   0 root         (0) root         (0)     1098 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html
--rw-rw-rw-   0 root         (0) root         (0)    21468 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      689 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.796527 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/util/
--rwxrwxrwx   0 root         (0) root         (0)       23 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/util/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    15106 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/util/ts3.py
--rw-rw-rw-   0 root         (0) root         (0)     5058 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.800527 allianceauth-3.4.0/allianceauth/services/modules/xenforo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/xenforo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/xenforo/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/xenforo/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1779 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/xenforo/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     3685 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/xenforo/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.801527 allianceauth-3.4.0/allianceauth/services/modules/xenforo/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/xenforo/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2067 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/xenforo/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/xenforo/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/xenforo/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     7153 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/xenforo/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/xenforo/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     4821 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/modules/xenforo/views.py
--rw-rw-rw-   0 root         (0) root         (0)    10087 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.567510 allianceauth-3.4.0/allianceauth/services/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.567510 allianceauth-3.4.0/allianceauth/services/static/allianceauth/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.802527 allianceauth-3.4.0/allianceauth/services/static/allianceauth/services/
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/static/allianceauth/services/admin.css
--rw-rw-rw-   0 root         (0) root         (0)     1937 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.568511 allianceauth-3.4.0/allianceauth/services/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.802527 allianceauth-3.4.0/allianceauth/services/templates/public/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/templates/public/menublock.html
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/templates/public/menuitem.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.804527 allianceauth-3.4.0/allianceauth/services/templates/services/
--rw-rw-rw-   0 root         (0) root         (0)     1152 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/templates/services/fleetformattertool.html
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/templates/services/service_confirm_delete.html
--rw-rw-rw-   0 root         (0) root         (0)     1176 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/templates/services/service_credentials.html
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/templates/services/service_password.html
--rwxrwxrwx   0 root         (0) root         (0)     1058 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/templates/services/services.html
--rw-rw-rw-   0 root         (0) root         (0)     1309 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/templates/services/services_ctrl.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.805527 allianceauth-3.4.0/allianceauth/services/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/templatetags/menu_items.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.807527 allianceauth-3.4.0/allianceauth/services/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     4316 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/tests/test_nameformatter.py
--rw-rw-rw-   0 root         (0) root         (0)    12299 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/tests/test_signals.py
--rw-rw-rw-   0 root         (0) root         (0)     3248 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/urls.py
--rwxrwxrwx   0 root         (0) root         (0)     2450 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/services/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.811528 allianceauth-3.4.0/allianceauth/srp/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      205 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      926 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/auth_hooks.py
--rwxrwxrwx   0 root         (0) root         (0)     1724 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/form.py
--rw-rw-rw-   0 root         (0) root         (0)     1961 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.813528 allianceauth-3.4.0/allianceauth/srp/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2265 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/migrations/0002_srpuserrequest_srp_status_choices.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/migrations/0003_make_strings_more_stringy.py
--rw-rw-rw-   0 root         (0) root         (0)      746 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/migrations/0004_on_delete.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/migrations/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1991 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/models.py
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/providers.py
--rw-rw-rw-   0 root         (0) root         (0)    24877 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/swagger.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.570511 allianceauth-3.4.0/allianceauth/srp/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.815528 allianceauth-3.4.0/allianceauth/srp/templates/srp/
--rw-rw-rw-   0 root         (0) root         (0)     2091 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/templates/srp/add.html
--rw-rw-rw-   0 root         (0) root         (0)    13508 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/templates/srp/data.html
--rw-rw-rw-   0 root         (0) root         (0)     7269 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/templates/srp/management.html
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/templates/srp/request.html
--rw-rw-rw-   0 root         (0) root         (0)     1139 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/templates/srp/update.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.816528 allianceauth-3.4.0/allianceauth/srp/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3623 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/tests/test_managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.816528 allianceauth-3.4.0/allianceauth/srp/tests/testdata/
--rw-rw-rw-   0 root         (0) root         (0)    28605 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/tests/testdata/zkillboard_killmail_api_81973979.json
--rw-rw-rw-   0 root         (0) root         (0)     1342 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/urls.py
--rwxrwxrwx   0 root         (0) root         (0)    17762 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/srp/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.817528 allianceauth-3.4.0/allianceauth/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.573511 allianceauth-3.4.0/allianceauth/static/allianceauth/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.818528 allianceauth-3.4.0/allianceauth/static/allianceauth/css/
--rw-rw-rw-   0 root         (0) root         (0)     4636 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/css/auth-base.css
--rw-rw-rw-   0 root         (0) root         (0)     1173 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/css/checkbox.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.818528 allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.819528 allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/darkly/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/darkly/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.less
--rw-rw-rw-   0 root         (0) root         (0)   122466 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.821528 allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/flatly/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/flatly/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.less
--rw-rw-rw-   0 root         (0) root         (0)   123138 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/flatly-shared.less
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.823528 allianceauth-3.4.0/allianceauth/static/allianceauth/icons/
--rwxrwxrwx   0 root         (0) root         (0)    21465 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/icons/allianceauth.png
--rwxrwxrwx   0 root         (0) root         (0)     3508 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/icons/apple-touch-icon.png
--rwxrwxrwx   0 root         (0) root         (0)      483 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/icons/favicon-16x16.png
--rwxrwxrwx   0 root         (0) root         (0)      868 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/icons/favicon-32x32.png
--rwxrwxrwx   0 root         (0) root         (0)     2180 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/icons/favicon-96x96.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.824529 allianceauth-3.4.0/allianceauth/static/allianceauth/js/
--rw-rw-rw-   0 root         (0) root         (0)      558 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/js/eve-time.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.825528 allianceauth-3.4.0/allianceauth/static/allianceauth/js/filterDropDown/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/js/filterDropDown/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     8874 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js
--rw-rw-rw-   0 root         (0) root         (0)     2529 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.574511 allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.574511 allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.825528 allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.828529 allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/
--rw-rw-rw-   0 root         (0) root         (0)     7090 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     7074 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4618 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     7111 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4618 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     6487 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)    15830 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css
--rw-rw-rw-   0 root         (0) root         (0)     2482 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/js/refresh_notifications.js
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/allianceauth/js/timers.js
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/static/robots.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.576511 allianceauth-3.4.0/allianceauth/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.828529 allianceauth-3.4.0/allianceauth/templates/admin/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/admin/base_site.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.832529 allianceauth-3.4.0/allianceauth/templates/allianceauth/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.833529 allianceauth-3.4.0/allianceauth/templates/allianceauth/admin-status/
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/allianceauth/admin-status/celery_bar_partial.html
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/allianceauth/admin-status/include.html
--rw-rw-rw-   0 root         (0) root         (0)     6109 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/allianceauth/admin-status/overview.html
--rw-rw-rw-   0 root         (0) root         (0)     2299 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/allianceauth/base.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/allianceauth/icons.html
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/allianceauth/messages.html
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/allianceauth/night-toggle.html
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/allianceauth/notifications_menu_item.html
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/allianceauth/side-menu.html
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/allianceauth/top-menu-admin.html
--rw-rw-rw-   0 root         (0) root         (0)     2872 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/allianceauth/top-menu-user-dropdown.html
--rw-rw-rw-   0 root         (0) root         (0)     1489 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/allianceauth/top-menu.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.840530 allianceauth-3.4.0/allianceauth/templates/bundles/
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/auth-base-css.html
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/bootstrap-css.html
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/bootstrap-js.html
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/checkbox-css.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/clipboard-js.html
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/datatables-css.html
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/datatables-js.html
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/evetime-js.html
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/filterdropdown-js.html
--rw-rw-rw-   0 root         (0) root         (0)      349 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/fontawesome.html
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/jquery-datetimepicker-css.html
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/jquery-datetimepicker-js.html
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/jquery-ui-css.html
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/jquery-ui-js.html
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/jquery-visibility-js.html
--rw-rw-rw-   0 root         (0) root         (0)      527 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/moment-js.html
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/refresh-notifications-js.html
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/timers-js.html
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/x-editable-js.html
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templates/bundles/x-editable.css.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.841530 allianceauth-3.4.0/allianceauth/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6405 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/templatetags/admin_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.842530 allianceauth-3.4.0/allianceauth/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11465 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/tests/auth_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2061 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/tests/test_auth_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.842530 allianceauth-3.4.0/allianceauth/thirdparty/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/thirdparty/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.843530 allianceauth-3.4.0/allianceauth/thirdparty/navhelper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/thirdparty/navhelper/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.844530 allianceauth-3.4.0/allianceauth/thirdparty/navhelper/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/thirdparty/navhelper/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2672 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/thirdparty/navhelper/templatetags/navactive.py
--rw-rw-rw-   0 root         (0) root         (0)     3407 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/thirdparty/navhelper/tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.847530 allianceauth-3.4.0/allianceauth/timerboard/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      111 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/auth_hooks.py
--rwxrwxrwx   0 root         (0) root         (0)     4708 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/form.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.849530 allianceauth-3.4.0/allianceauth/timerboard/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1629 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py
--rw-rw-rw-   0 root         (0) root         (0)      763 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/migrations/0003_on_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/migrations/0004_timer_type.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/migrations/0005_alter_timer_planet_moon.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/migrations/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1593 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.579512 allianceauth-3.4.0/allianceauth/timerboard/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.851530 allianceauth-3.4.0/allianceauth/timerboard/templates/timerboard/
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/templates/timerboard/form.html
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/templates/timerboard/index_button.html
--rw-rw-rw-   0 root         (0) root         (0)      887 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/templates/timerboard/timer_create_form.html
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/templates/timerboard/timer_update_form.html
--rw-rw-rw-   0 root         (0) root         (0)    30990 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/templates/timerboard/view.html
--rw-rw-rw-   0 root         (0) root         (0)     8745 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/urls.py
--rwxrwxrwx   0 root         (0) root         (0)     2897 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/timerboard/views.py
--rwxrwxrwx   0 root         (0) root         (0)     1750 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.853531 allianceauth-3.4.0/allianceauth/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/utils/cache.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/utils/django.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/utils/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.854531 allianceauth-3.4.0/allianceauth/utils/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/utils/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1194 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/utils/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/utils/tests/test_django.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/utils/tests/test_testing.py
--rw-rw-rw-   0 root         (0) root         (0)     2204 2023-04-25 11:33:08.000000 allianceauth-3.4.0/allianceauth/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:33:30.587512 allianceauth-3.4.0/allianceauth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6285 2023-04-25 11:33:30.000000 allianceauth-3.4.0/allianceauth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    38148 2023-04-25 11:33:30.000000 allianceauth-3.4.0/allianceauth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:33:30.000000 allianceauth-3.4.0/allianceauth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-04-25 11:33:30.000000 allianceauth-3.4.0/allianceauth.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:33:30.000000 allianceauth-3.4.0/allianceauth.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      441 2023-04-25 11:33:30.000000 allianceauth-3.4.0/allianceauth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 11:33:30.000000 allianceauth-3.4.0/allianceauth.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-25 11:33:08.000000 allianceauth-3.4.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2009 2023-04-25 11:33:30.856531 allianceauth-3.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.457682 allianceauth-3.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)    18026 2023-07-11 03:15:51.000000 allianceauth-3.5.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-07-11 03:15:51.000000 allianceauth-3.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6285 2023-07-11 03:16:08.457682 allianceauth-3.5.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4978 2023-07-11 03:15:51.000000 allianceauth-3.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.292686 allianceauth-3.5.0/allianceauth/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.295685 allianceauth-3.5.0/allianceauth/analytics/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.295685 allianceauth-3.5.0/allianceauth/analytics/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/fixtures/disable_analytics.json
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.296686 allianceauth-3.5.0/allianceauth/analytics/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1664 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/migrations/0003_Generate_Identifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     1650 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/migrations/0004_auto_20211015_0502.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/migrations/0005_alter_analyticspath_ignore_path.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/migrations/0006_more_ignore_paths.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)     6605 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.298685 allianceauth-3.5.0/allianceauth/analytics/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4313 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/tests/test_integration.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/tests/test_middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    10228 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/analytics/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.301685 allianceauth-3.5.0/allianceauth/authentication/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21206 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     5638 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/backends.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2486 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/hmac_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.301685 allianceauth-3.5.0/allianceauth/authentication/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.301685 allianceauth-3.5.0/allianceauth/authentication/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/management/commands/checkmains.py
+-rwxrwxrwx   0 root         (0) root         (0)     2709 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/managers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1999 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.305685 allianceauth-3.5.0/allianceauth/authentication/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     3147 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0002_auto_20160907_1914.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0003_authservicesinfo_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     2543 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0004_create_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1144 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0005_delete_perms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1324 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0006_auto_20160910_0542.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0007_remove_authservicesinfo_is_blue.py
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0008_set_state.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0009_auto_20161021_0228.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1914 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0013_service_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0014_fleetup_permission.py
+-rw-rw-rw-   0 root         (0) root         (0)    13077 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0015_user_profiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0016_ownershiprecord.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0018_alter_state_name_length.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0018_state_member_factions.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0019_merge_20211026_0919.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/0021_alter_userprofile_language.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/migrations/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5810 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     7806 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.260686 allianceauth-3.5.0/allianceauth/authentication/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.260686 allianceauth-3.5.0/allianceauth/authentication/static/allianceauth/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.260686 allianceauth-3.5.0/allianceauth/authentication/static/allianceauth/authentication/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.305685 allianceauth-3.5.0/allianceauth/authentication/static/allianceauth/authentication/css/
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/static/allianceauth/authentication/css/admin.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.306685 allianceauth-3.5.0/allianceauth/authentication/static/allianceauth/authentication/img/
+-rw-rw-rw-   0 root         (0) root         (0)   161344 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.306685 allianceauth-3.5.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png
+-rw-rw-rw-   0 root         (0) root         (0)     2248 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.307685 allianceauth-3.5.0/allianceauth/authentication/task_statistics/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/task_statistics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1465 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/task_statistics/counters.py
+-rw-rw-rw-   0 root         (0) root         (0)     4042 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/task_statistics/event_series.py
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/task_statistics/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.308685 allianceauth-3.5.0/allianceauth/authentication/task_statistics/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/task_statistics/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/task_statistics/tests/test_counters.py
+-rw-rw-rw-   0 root         (0) root         (0)     5843 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/task_statistics/tests/test_event_series.py
+-rw-rw-rw-   0 root         (0) root         (0)     2918 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/task_statistics/tests/test_signals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1661 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.261686 allianceauth-3.5.0/allianceauth/authentication/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.308685 allianceauth-3.5.0/allianceauth/authentication/templates/authentication/
+-rw-rw-rw-   0 root         (0) root         (0)    10738 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/templates/authentication/dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     2613 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/templates/authentication/tokens.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.309685 allianceauth-3.5.0/allianceauth/authentication/templates/public/
+-rw-rw-rw-   0 root         (0) root         (0)     1944 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/templates/public/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      624 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/templates/public/lang_select.html
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/templates/public/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1433 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/templates/public/middle_box.html
+-rw-rw-rw-   0 root         (0) root         (0)      846 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/templates/public/register.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.310685 allianceauth-3.5.0/allianceauth/authentication/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/templates/registration/activate.html
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/templates/registration/activation_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/templates/registration/activation_email_html.txt
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/templates/registration/activation_email_subject.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.311685 allianceauth-3.5.0/allianceauth/authentication/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      833 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29475 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/tests/test_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3456 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/tests/test_app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     7427 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/tests/test_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     1517 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/tests/test_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     2452 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/tests/test_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6316 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/tests/test_middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)    11478 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3154 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/tests/test_signals.py
+-rw-rw-rw-   0 root         (0) root         (0)    10983 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/tests/test_templatetags.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    11597 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/authentication/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.312685 allianceauth-3.5.0/allianceauth/bin/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/bin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3555 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/bin/allianceauth.py
+-rw-rw-rw-   0 root         (0) root         (0)      274 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/context_processors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.315685 allianceauth-3.5.0/allianceauth/corputils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1970 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.316685 allianceauth-3.5.0/allianceauth/corputils/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     5358 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/migrations/0002_migrate_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/migrations/0003_granular_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/migrations/0004_member_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/migrations/0005_cleanup_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7223 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/models.py
+-rw-rw-rw-   0 root         (0) root         (0)   947431 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/swagger.json
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.262686 allianceauth-3.5.0/allianceauth/corputils/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.316685 allianceauth-3.5.0/allianceauth/corputils/templates/corputils/
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/templates/corputils/base.html
+-rw-rw-rw-   0 root         (0) root         (0)    14915 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/templates/corputils/corpstats.html
+-rw-rw-rw-   0 root         (0) root         (0)     2540 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/templates/corputils/search.html
+-rw-rw-rw-   0 root         (0) root         (0)    16016 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     6999 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/corputils/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.318685 allianceauth-3.5.0/allianceauth/eveonline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7277 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.319685 allianceauth-3.5.0/allianceauth/eveonline/autogroups/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/autogroups/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/autogroups/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/autogroups/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.320685 allianceauth-3.5.0/allianceauth/eveonline/autogroups/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     4024 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/autogroups/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/autogroups/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10691 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/autogroups/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/autogroups/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.321685 allianceauth-3.5.0/allianceauth/eveonline/autogroups/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/autogroups/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/autogroups/tests/test_managers.py
+-rw-rw-rw-   0 root         (0) root         (0)    12356 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/autogroups/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     7961 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/autogroups/tests/test_signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.322685 allianceauth-3.5.0/allianceauth/eveonline/evelinks/
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/evelinks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/evelinks/dotlan.py
+-rw-rw-rw-   0 root         (0) root         (0)     3730 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/evelinks/eveimageserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/evelinks/evewho.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.322685 allianceauth-3.5.0/allianceauth/eveonline/evelinks/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/evelinks/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7329 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/evelinks/tests/test_evelinks.py
+-rw-rw-rw-   0 root         (0) root         (0)    11505 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/evelinks/tests/test_templatetags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/evelinks/zkillboard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3350 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.327685 allianceauth-3.5.0/allianceauth/eveonline/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     3133 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0002_remove_eveapikeypair_error_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0004_eveapikeypair_sso_verified.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0005_remove_eveallianceinfo_member_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py
+-rw-rw-rw-   0 root         (0) root         (0)     4599 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0007_unique_id_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      854 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0008_remove_apikeys.py
+-rw-rw-rw-   0 root         (0) root         (0)      519 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0009_on_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0010_alliance_ticker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0011_ids_to_integers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0012_index_additions.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0013_evecorporationinfo_ceo_id.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0014_auto_20210105_1413.py
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0015_factions.py
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0016_character_names_are_not_unique.py
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14052 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     9958 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/providers.py
+-rw-rw-rw-   0 root         (0) root         (0)    41989 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/swagger.json
+-rw-rw-rw-   0 root         (0) root         (0)     3808 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.327685 allianceauth-3.5.0/allianceauth/eveonline/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8354 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/templatetags/evelinks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/templatetags/examples.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.329685 allianceauth-3.5.0/allianceauth/eveonline/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      739 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6043 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/tests/esi_client_stub.py
+-rw-rw-rw-   0 root         (0) root         (0)   297070 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/tests/swagger_old.json
+-rw-rw-rw-   0 root         (0) root         (0)    10079 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/tests/test_managers.py
+-rw-rw-rw-   0 root         (0) root         (0)    23361 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    23834 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/tests/test_providers.py
+-rw-rw-rw-   0 root         (0) root         (0)    10117 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/tests/test_tasks.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/eveonline/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.332685 allianceauth-3.5.0/allianceauth/fleetactivitytracking/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.334684 allianceauth-3.5.0/allianceauth/fleetactivitytracking/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/migrations/0002_auto_20160905_2220.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/migrations/0003_auto_20160906_2354.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/migrations/0004_make_strings_more_stringy.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/migrations/0005_remove_fat_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/migrations/0006_auto_20180803_0430.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/models.py
+-rw-rw-rw-   0 root         (0) root         (0)   947431 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/swagger.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.264686 allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.336685 allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html
+-rw-rw-rw-   0 root         (0) root         (0)     1208 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkformatter.html
+-rw-rw-rw-   0 root         (0) root         (0)     2680 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html
+-rw-rw-rw-   0 root         (0) root         (0)     3200 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html
+-rw-rw-rw-   0 root         (0) root         (0)     1485 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html
+-rw-rw-rw-   0 root         (0) root         (0)     2227 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html
+-rw-rw-rw-   0 root         (0) root         (0)     2415 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html
+-rw-rw-rw-   0 root         (0) root         (0)     4384 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    16667 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/fleetactivitytracking/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.338684 allianceauth-3.5.0/allianceauth/groupmanagement/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8978 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.343684 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2243 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0003_default_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     4324 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0004_authgroup.py
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0005_authgroup_public.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0007_on_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1100 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0009_requestlog.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0010_authgroup_states.py
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0011_requestlog_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      672 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0012_group_leads.py
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0013_fix_requestlog_date_field.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0014_auto_20200918_1412.py
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0016_remove_grouprequest_status_field.py
+-rw-rw-rw-   0 root         (0) root         (0)     2296 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py
+-rw-rw-rw-   0 root         (0) root         (0)      520 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8162 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1465 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.265686 allianceauth-3.5.0/allianceauth/groupmanagement/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.345684 allianceauth-3.5.0/allianceauth/groupmanagement/templates/groupmanagement/
+-rw-rw-rw-   0 root         (0) root         (0)     4886 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/templates/groupmanagement/audit.html
+-rw-rw-rw-   0 root         (0) root         (0)     4784 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html
+-rw-rw-rw-   0 root         (0) root         (0)     4195 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html
+-rw-rw-rw-   0 root         (0) root         (0)     2948 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/templates/groupmanagement/groups.html
+-rw-rw-rw-   0 root         (0) root         (0)     9513 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/templates/groupmanagement/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/templates/groupmanagement/menu.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.346684 allianceauth-3.5.0/allianceauth/groupmanagement/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24713 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/tests/test_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)    17375 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/tests/test_managers.py
+-rw-rw-rw-   0 root         (0) root         (0)    11668 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4950 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/tests/test_signals.py
+-rw-rw-rw-   0 root         (0) root         (0)     3073 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/tests/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1651 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/urls.py
+-rwxrwxrwx   0 root         (0) root         (0)    19860 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/groupmanagement/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     4127 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.348684 allianceauth-3.5.0/allianceauth/hrapplications/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      717 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      987 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/auth_hooks.py
+-rwxrwxrwx   0 root         (0) root         (0)      353 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.351684 allianceauth-3.5.0/allianceauth/hrapplications/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     6662 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/migrations/0002_choices_for_questions.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/migrations/0003_applicationquestion_multi_select.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/migrations/0005_sorted_questions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1946 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/migrations/0007_auto_20200918_1412.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/migrations/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3237 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.266686 allianceauth-3.5.0/allianceauth/hrapplications/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.352684 allianceauth-3.5.0/allianceauth/hrapplications/templates/hrapplications/
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/templates/hrapplications/corpchoice.html
+-rw-rw-rw-   0 root         (0) root         (0)     1915 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/templates/hrapplications/create.html
+-rw-rw-rw-   0 root         (0) root         (0)    11885 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/templates/hrapplications/management.html
+-rw-rw-rw-   0 root         (0) root         (0)     4107 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/templates/hrapplications/searchview.html
+-rw-rw-rw-   0 root         (0) root         (0)     9294 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/templates/hrapplications/view.html
+-rw-rw-rw-   0 root         (0) root         (0)     4165 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     1113 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/urls.py
+-rwxrwxrwx   0 root         (0) root         (0)    12011 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/hrapplications/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.269686 allianceauth-3.5.0/allianceauth/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.266686 allianceauth-3.5.0/allianceauth/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.352684 allianceauth-3.5.0/allianceauth/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    37872 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    84839 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.266686 allianceauth-3.5.0/allianceauth/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.353684 allianceauth-3.5.0/allianceauth/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    70502 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.267686 allianceauth-3.5.0/allianceauth/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.354684 allianceauth-3.5.0/allianceauth/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    37814 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    84835 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.267686 allianceauth-3.5.0/allianceauth/locale/fr_FR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.354684 allianceauth-3.5.0/allianceauth/locale/fr_FR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    37724 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    85375 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.268686 allianceauth-3.5.0/allianceauth/locale/it_IT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.355684 allianceauth-3.5.0/allianceauth/locale/it_IT/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    17209 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/it_IT/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    77100 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/it_IT/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.268686 allianceauth-3.5.0/allianceauth/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.355684 allianceauth-3.5.0/allianceauth/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    41641 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    88417 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.268686 allianceauth-3.5.0/allianceauth/locale/ko_KR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.356684 allianceauth-3.5.0/allianceauth/locale/ko_KR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    36909 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    84828 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.268686 allianceauth-3.5.0/allianceauth/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.357684 allianceauth-3.5.0/allianceauth/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    47123 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    94195 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.269686 allianceauth-3.5.0/allianceauth/locale/uk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.357684 allianceauth-3.5.0/allianceauth/locale/uk/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    48143 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    95082 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.269686 allianceauth-3.5.0/allianceauth/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.358684 allianceauth-3.5.0/allianceauth/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    27229 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    79576 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.360684 allianceauth-3.5.0/allianceauth/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1113 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1320 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      998 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3907 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.362684 allianceauth-3.5.0/allianceauth/notifications/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/migrations/0002_auto_20160910_1649.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/migrations/0004_performance_tuning.py
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/migrations/0005_fix_level_choices.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2772 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.270686 allianceauth-3.5.0/allianceauth/notifications/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.362684 allianceauth-3.5.0/allianceauth/notifications/templates/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/templates/notifications/list.html
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/templates/notifications/list_partial.html
+-rw-rw-rw-   0 root         (0) root         (0)      812 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/templates/notifications/view.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.363684 allianceauth-3.5.0/allianceauth/notifications/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/templatetags/auth_notifications.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.365684 allianceauth-3.5.0/allianceauth/notifications/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3073 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/tests/test_core.py
+-rw-rw-rw-   0 root         (0) root         (0)     2392 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/tests/test_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/tests/test_init.py
+-rw-rw-rw-   0 root         (0) root         (0)     9437 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/tests/test_managers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2398 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2975 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/tests/test_templatetags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/tests/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     3522 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/notifications/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.367684 allianceauth-3.5.0/allianceauth/optimer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      763 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/form.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/form_widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.368684 allianceauth-3.5.0/allianceauth/optimer/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/migrations/0002_auto_20170413_0442.py
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/migrations/0004_on_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/migrations/0005_add_type_and_description.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1247 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.271686 allianceauth-3.5.0/allianceauth/optimer/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.369684 allianceauth-3.5.0/allianceauth/optimer/templates/optimer/
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/templates/optimer/add.html
+-rw-rw-rw-   0 root         (0) root         (0)     2630 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/templates/optimer/fleetoptable.html
+-rw-rw-rw-   0 root         (0) root         (0)     3707 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/templates/optimer/management.html
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/templates/optimer/update.html
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     5765 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/optimer/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.371683 allianceauth-3.5.0/allianceauth/permissions_tool/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/permissions_tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      150 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/permissions_tool/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      787 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/permissions_tool/auth_hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.371683 allianceauth-3.5.0/allianceauth/permissions_tool/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/permissions_tool/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/permissions_tool/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/permissions_tool/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.272686 allianceauth-3.5.0/allianceauth/permissions_tool/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.372684 allianceauth-3.5.0/allianceauth/permissions_tool/templates/permissions_tool/
+-rw-rw-rw-   0 root         (0) root         (0)     3414 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/permissions_tool/templates/permissions_tool/audit.html
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html
+-rw-rw-rw-   0 root         (0) root         (0)     4891 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/permissions_tool/templates/permissions_tool/overview.html
+-rw-rw-rw-   0 root         (0) root         (0)     4968 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/permissions_tool/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/permissions_tool/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2610 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/permissions_tool/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.373684 allianceauth-3.5.0/allianceauth/project_template/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/project_template/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.373684 allianceauth-3.5.0/allianceauth/project_template/log/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/project_template/log/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      821 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/project_template/manage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.374683 allianceauth-3.5.0/allianceauth/project_template/project_name/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/project_template/project_name/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/project_template/project_name/celery.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.375683 allianceauth-3.5.0/allianceauth/project_template/project_name/settings/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/project_template/project_name/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8741 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/project_template/project_name/settings/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2902 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/project_template/project_name/settings/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.375683 allianceauth-3.5.0/allianceauth/project_template/project_name/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/project_template/project_name/static/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.375683 allianceauth-3.5.0/allianceauth/project_template/project_name/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/project_template/project_name/templates/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/project_template/project_name/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/project_template/project_name/wsgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/project_template/supervisor.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.378683 allianceauth-3.5.0/allianceauth/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3954 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     2165 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      656 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     8308 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.378683 allianceauth-3.5.0/allianceauth/services/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.378683 allianceauth-3.5.0/allianceauth/services/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/management/commands/verify_service_accounts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.379683 allianceauth-3.5.0/allianceauth/services/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      483 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/migrations/0001_squashed_0003_delete_groupcache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1220 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/migrations/0002_nameformatter.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/migrations/0003_remove_broken_link.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.380683 allianceauth-3.5.0/allianceauth/services/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.383683 allianceauth-3.5.0/allianceauth/services/modules/discord/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     4957 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4446 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.384683 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    28936 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4590 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3853 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.386683 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5027 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/example_objects.json
+-rw-rw-rw-   0 root         (0) root         (0)     3013 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)     2784 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py
+-rw-rw-rw-   0 root         (0) root         (0)     4477 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md
+-rw-rw-rw-   0 root         (0) root         (0)    56104 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/test_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9724 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4966 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6281 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.387683 allianceauth-3.5.0/allianceauth/services/modules/discord/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      680 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2067 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/migrations/0002_service_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7138 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     9517 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.275686 allianceauth-3.5.0/allianceauth/services/modules/discord/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.275686 allianceauth-3.5.0/allianceauth/services/modules/discord/templates/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.387683 allianceauth-3.5.0/allianceauth/services/modules/discord/templates/services/discord/
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.390683 allianceauth-3.5.0/allianceauth/services/modules/discord/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/tests/factories.py
+-rwxrwxrwx   0 root         (0) root         (0)     2639 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/tests/piloting_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)    10400 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     6287 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     8456 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_core.py
+-rw-rw-rw-   0 root         (0) root         (0)    29543 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_integration.py
+-rw-rw-rw-   0 root         (0) root         (0)    19956 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_managers.py
+-rw-rw-rw-   0 root         (0) root         (0)    11474 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    17995 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6783 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      566 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discord/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.392683 allianceauth-3.5.0/allianceauth/services/modules/discourse/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discourse/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discourse/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discourse/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1878 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discourse/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     7039 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discourse/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.393683 allianceauth-3.5.0/allianceauth/services/modules/discourse/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discourse/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2096 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discourse/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discourse/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      533 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discourse/providers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2276 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discourse/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.276686 allianceauth-3.5.0/allianceauth/services/modules/discourse/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.276686 allianceauth-3.5.0/allianceauth/services/modules/discourse/templates/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.393683 allianceauth-3.5.0/allianceauth/services/modules/discourse/templates/services/discourse/
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discourse/templates/services/discourse/discourse_service_ctrl.html
+-rw-rw-rw-   0 root         (0) root         (0)     5209 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discourse/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discourse/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     3486 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/discourse/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.395683 allianceauth-3.5.0/allianceauth/services/modules/example/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/example/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/example/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1336 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/example/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/example/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/example/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/example/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.397683 allianceauth-3.5.0/allianceauth/services/modules/ips4/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/ips4/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/ips4/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/ips4/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/ips4/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4199 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/ips4/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.398683 allianceauth-3.5.0/allianceauth/services/modules/ips4/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      737 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/ips4/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/ips4/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/ips4/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/ips4/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     6035 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/ips4/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/ips4/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     4789 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/ips4/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.400683 allianceauth-3.5.0/allianceauth/services/modules/mumble/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      455 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     2958 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/auth_hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.403683 allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0002_auto_20161212_0100.py
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py
+-rw-rw-rw-   0 root         (0) root         (0)     2063 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0008_mumbleuser_display_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0011_auto_20201011_1009.py
+-rw-rw-rw-   0 root         (0) root         (0)     1508 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5630 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.277686 allianceauth-3.5.0/allianceauth/services/modules/mumble/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.278686 allianceauth-3.5.0/allianceauth/services/modules/mumble/templates/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.403683 allianceauth-3.5.0/allianceauth/services/modules/mumble/templates/services/mumble/
+-rw-rw-rw-   0 root         (0) root         (0)     1336 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html
+-rw-rw-rw-   0 root         (0) root         (0)     8632 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/mumble/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.406683 allianceauth-3.5.0/allianceauth/services/modules/openfire/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/openfire/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/openfire/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/openfire/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3615 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/openfire/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/openfire/forms.py
+-rwxrwxrwx   0 root         (0) root         (0)     8321 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/openfire/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.407683 allianceauth-3.5.0/allianceauth/services/modules/openfire/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/openfire/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/openfire/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/openfire/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2620 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/openfire/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.278686 allianceauth-3.5.0/allianceauth/services/modules/openfire/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.278686 allianceauth-3.5.0/allianceauth/services/modules/openfire/templates/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.407683 allianceauth-3.5.0/allianceauth/services/modules/openfire/templates/services/openfire/
+-rwxrwxrwx   0 root         (0) root         (0)     1183 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html
+-rw-rw-rw-   0 root         (0) root         (0)     9478 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/openfire/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/openfire/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     7688 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/openfire/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.409683 allianceauth-3.5.0/allianceauth/services/modules/phpbb3/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/phpbb3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/phpbb3/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/phpbb3/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/phpbb3/auth_hooks.py
+-rwxrwxrwx   0 root         (0) root         (0)    13459 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/phpbb3/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.411682 allianceauth-3.5.0/allianceauth/services/modules/phpbb3/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      683 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/phpbb3/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2049 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/phpbb3/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/phpbb3/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/phpbb3/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     8189 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/phpbb3/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/phpbb3/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     5139 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/phpbb3/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.413683 allianceauth-3.5.0/allianceauth/services/modules/smf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/smf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/smf/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/smf/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/smf/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)    14780 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/smf/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.414682 allianceauth-3.5.0/allianceauth/services/modules/smf/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/smf/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/smf/migrations/0002_service_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      694 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/smf/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/smf/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3740 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/smf/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     8057 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/smf/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      517 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/smf/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     5143 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/smf/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.417683 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1860 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     2128 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/forms.py
+-rwxrwxrwx   0 root         (0) root         (0)    12601 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.418682 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1995 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py
+-rw-rw-rw-   0 root         (0) root         (0)      781 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py
+-rw-rw-rw-   0 root         (0) root         (0)     2116 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      784 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)     3780 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.281686 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.280686 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/templates/admin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.281686 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/templates/admin/teamspeak3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.419682 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/templates/admin/teamspeak3/authts/
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/templates/admin/teamspeak3/authts/change_list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.281686 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/templates/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.419682 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/
+-rw-rw-rw-   0 root         (0) root         (0)     1330 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html
+-rw-rw-rw-   0 root         (0) root         (0)    21468 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      689 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.420682 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/util/
+-rwxrwxrwx   0 root         (0) root         (0)       23 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/util/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15106 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/util/ts3.py
+-rw-rw-rw-   0 root         (0) root         (0)     5061 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.422682 allianceauth-3.5.0/allianceauth/services/modules/xenforo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/xenforo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/xenforo/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/xenforo/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1779 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/xenforo/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3685 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/xenforo/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.423682 allianceauth-3.5.0/allianceauth/services/modules/xenforo/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/xenforo/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2067 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/xenforo/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/xenforo/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/xenforo/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     7153 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/xenforo/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      557 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/xenforo/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     4821 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/modules/xenforo/views.py
+-rw-rw-rw-   0 root         (0) root         (0)    10087 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.282686 allianceauth-3.5.0/allianceauth/services/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.282686 allianceauth-3.5.0/allianceauth/services/static/allianceauth/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.423682 allianceauth-3.5.0/allianceauth/services/static/allianceauth/services/
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/static/allianceauth/services/admin.css
+-rw-rw-rw-   0 root         (0) root         (0)     1937 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.283686 allianceauth-3.5.0/allianceauth/services/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.423682 allianceauth-3.5.0/allianceauth/services/templates/public/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/templates/public/menublock.html
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/templates/public/menuitem.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.425682 allianceauth-3.5.0/allianceauth/services/templates/services/
+-rw-rw-rw-   0 root         (0) root         (0)     1152 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/templates/services/fleetformattertool.html
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/templates/services/service_confirm_delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/templates/services/service_credentials.html
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/templates/services/service_password.html
+-rwxrwxrwx   0 root         (0) root         (0)     1058 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/templates/services/services.html
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/templates/services/services_ctrl.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.425682 allianceauth-3.5.0/allianceauth/services/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/templatetags/menu_items.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.426682 allianceauth-3.5.0/allianceauth/services/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4316 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/tests/test_nameformatter.py
+-rw-rw-rw-   0 root         (0) root         (0)    12299 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/tests/test_signals.py
+-rw-rw-rw-   0 root         (0) root         (0)     3248 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/urls.py
+-rwxrwxrwx   0 root         (0) root         (0)     2450 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/services/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.429682 allianceauth-3.5.0/allianceauth/srp/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      205 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      926 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/auth_hooks.py
+-rwxrwxrwx   0 root         (0) root         (0)     1724 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/form.py
+-rw-rw-rw-   0 root         (0) root         (0)     1961 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.430682 allianceauth-3.5.0/allianceauth/srp/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/migrations/0002_srpuserrequest_srp_status_choices.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/migrations/0003_make_strings_more_stringy.py
+-rw-rw-rw-   0 root         (0) root         (0)      746 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/migrations/0004_on_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/migrations/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1991 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/providers.py
+-rw-rw-rw-   0 root         (0) root         (0)    24877 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/swagger.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.284686 allianceauth-3.5.0/allianceauth/srp/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.431682 allianceauth-3.5.0/allianceauth/srp/templates/srp/
+-rw-rw-rw-   0 root         (0) root         (0)     2091 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/templates/srp/add.html
+-rw-rw-rw-   0 root         (0) root         (0)    13508 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/templates/srp/data.html
+-rw-rw-rw-   0 root         (0) root         (0)     7269 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/templates/srp/management.html
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/templates/srp/request.html
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/templates/srp/update.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.432682 allianceauth-3.5.0/allianceauth/srp/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3623 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/tests/test_managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.432682 allianceauth-3.5.0/allianceauth/srp/tests/testdata/
+-rw-rw-rw-   0 root         (0) root         (0)    28605 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/tests/testdata/zkillboard_killmail_api_81973979.json
+-rw-rw-rw-   0 root         (0) root         (0)     1342 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/urls.py
+-rwxrwxrwx   0 root         (0) root         (0)    17762 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/srp/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.432682 allianceauth-3.5.0/allianceauth/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.286686 allianceauth-3.5.0/allianceauth/static/allianceauth/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.433682 allianceauth-3.5.0/allianceauth/static/allianceauth/css/
+-rw-rw-rw-   0 root         (0) root         (0)     4636 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/css/auth-base.css
+-rw-rw-rw-   0 root         (0) root         (0)     1173 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/css/checkbox.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.433682 allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.434682 allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/darkly/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/darkly/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      624 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.less
+-rw-rw-rw-   0 root         (0) root         (0)   122466 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.435682 allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/flatly/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/flatly/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.less
+-rw-rw-rw-   0 root         (0) root         (0)   123138 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/flatly-shared.less
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.436682 allianceauth-3.5.0/allianceauth/static/allianceauth/icons/
+-rwxrwxrwx   0 root         (0) root         (0)    21465 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/icons/allianceauth.png
+-rwxrwxrwx   0 root         (0) root         (0)     3508 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/icons/apple-touch-icon.png
+-rwxrwxrwx   0 root         (0) root         (0)      483 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/icons/favicon-16x16.png
+-rwxrwxrwx   0 root         (0) root         (0)      868 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/icons/favicon-32x32.png
+-rwxrwxrwx   0 root         (0) root         (0)     2180 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/icons/favicon-96x96.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.437682 allianceauth-3.5.0/allianceauth/static/allianceauth/js/
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/js/eve-time.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.438682 allianceauth-3.5.0/allianceauth/static/allianceauth/js/filterDropDown/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/js/filterDropDown/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     8874 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.286686 allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.287686 allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.438682 allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.439682 allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/
+-rw-rw-rw-   0 root         (0) root         (0)     7090 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     7074 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     4618 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     7111 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     4618 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     6487 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)    15830 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css
+-rw-rw-rw-   0 root         (0) root         (0)     2482 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/js/refresh_notifications.js
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/allianceauth/js/timers.js
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/static/robots.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.288686 allianceauth-3.5.0/allianceauth/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.439682 allianceauth-3.5.0/allianceauth/templates/admin/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/admin/base_site.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.442682 allianceauth-3.5.0/allianceauth/templates/allianceauth/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.443682 allianceauth-3.5.0/allianceauth/templates/allianceauth/admin-status/
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/allianceauth/admin-status/celery_bar_partial.html
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/allianceauth/admin-status/include.html
+-rw-rw-rw-   0 root         (0) root         (0)     6109 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/allianceauth/admin-status/overview.html
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/allianceauth/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/allianceauth/icons.html
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/allianceauth/messages.html
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/allianceauth/night-toggle.html
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/allianceauth/notifications_menu_item.html
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/allianceauth/side-menu.html
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/allianceauth/top-menu-admin.html
+-rw-rw-rw-   0 root         (0) root         (0)     2872 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/allianceauth/top-menu-user-dropdown.html
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/allianceauth/top-menu.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.448682 allianceauth-3.5.0/allianceauth/templates/bundles/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/auth-base-css.html
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/bootstrap-css.html
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/bootstrap-js.html
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/checkbox-css.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/clipboard-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/datatables-css.html
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/datatables-js.html
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/evetime-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/filterdropdown-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/fontawesome.html
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/jquery-datetimepicker-css.html
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/jquery-datetimepicker-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/jquery-ui-css.html
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/jquery-ui-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/jquery-visibility-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      527 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/moment-js.html
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/refresh-notifications-js.html
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/timers-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/x-editable-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templates/bundles/x-editable.css.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.448682 allianceauth-3.5.0/allianceauth/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6405 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/templatetags/admin_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.449682 allianceauth-3.5.0/allianceauth/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11465 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/tests/auth_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/tests/test_auth_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.449682 allianceauth-3.5.0/allianceauth/thirdparty/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/thirdparty/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.450682 allianceauth-3.5.0/allianceauth/thirdparty/navhelper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/thirdparty/navhelper/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.450682 allianceauth-3.5.0/allianceauth/thirdparty/navhelper/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/thirdparty/navhelper/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2672 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/thirdparty/navhelper/templatetags/navactive.py
+-rw-rw-rw-   0 root         (0) root         (0)     3407 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/thirdparty/navhelper/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.452682 allianceauth-3.5.0/allianceauth/timerboard/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      111 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/auth_hooks.py
+-rwxrwxrwx   0 root         (0) root         (0)     4708 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/form.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.454681 allianceauth-3.5.0/allianceauth/timerboard/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1629 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py
+-rw-rw-rw-   0 root         (0) root         (0)      763 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/migrations/0003_on_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/migrations/0004_timer_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/migrations/0005_alter_timer_planet_moon.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/migrations/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1593 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.289686 allianceauth-3.5.0/allianceauth/timerboard/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.455681 allianceauth-3.5.0/allianceauth/timerboard/templates/timerboard/
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/templates/timerboard/form.html
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/templates/timerboard/index_button.html
+-rw-rw-rw-   0 root         (0) root         (0)      887 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/templates/timerboard/timer_create_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/templates/timerboard/timer_update_form.html
+-rw-rw-rw-   0 root         (0) root         (0)    30990 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/templates/timerboard/view.html
+-rw-rw-rw-   0 root         (0) root         (0)     8745 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/urls.py
+-rwxrwxrwx   0 root         (0) root         (0)     2897 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/timerboard/views.py
+-rwxrwxrwx   0 root         (0) root         (0)     1750 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.456681 allianceauth-3.5.0/allianceauth/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/utils/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/utils/django.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/utils/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.457682 allianceauth-3.5.0/allianceauth/utils/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/utils/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/utils/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/utils/tests/test_django.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/utils/tests/test_testing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2204 2023-07-11 03:15:51.000000 allianceauth-3.5.0/allianceauth/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:16:08.294685 allianceauth-3.5.0/allianceauth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6285 2023-07-11 03:16:08.000000 allianceauth-3.5.0/allianceauth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    38222 2023-07-11 03:16:08.000000 allianceauth-3.5.0/allianceauth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 03:16:08.000000 allianceauth-3.5.0/allianceauth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-07-11 03:16:08.000000 allianceauth-3.5.0/allianceauth.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 03:16:07.000000 allianceauth-3.5.0/allianceauth.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      446 2023-07-11 03:16:08.000000 allianceauth-3.5.0/allianceauth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 03:16:08.000000 allianceauth-3.5.0/allianceauth.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-11 03:15:51.000000 allianceauth-3.5.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2015 2023-07-11 03:16:08.458681 allianceauth-3.5.0/setup.cfg
```

### Comparing `allianceauth-3.4.0/LICENSE` & `allianceauth-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/PKG-INFO` & `allianceauth-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth
-Version: 3.4.0
+Version: 3.5.0
 Summary: An auth system for EVE Online to help in-game organizations manage online service access.
 Home-page: https://gitlab.com/allianceauth/allianceauth
 Author: Alliance Auth
 Author-email: adarnof@gmail.com
 License: GPL-2.0
 Project-URL: Issue / Bug Reports, https://gitlab.com/allianceauth/allianceauth/-/issues
 Project-URL: Documentation, https://allianceauth.readthedocs.io/
```

### Comparing `allianceauth-3.4.0/README.md` & `allianceauth-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/admin.py` & `allianceauth-3.5.0/allianceauth/analytics/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/middleware.py` & `allianceauth-3.5.0/allianceauth/analytics/middleware.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/analytics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py` & `allianceauth-3.5.0/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/migrations/0003_Generate_Identifier.py` & `allianceauth-3.5.0/allianceauth/analytics/migrations/0003_Generate_Identifier.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/migrations/0004_auto_20211015_0502.py` & `allianceauth-3.5.0/allianceauth/analytics/migrations/0004_auto_20211015_0502.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/migrations/0006_more_ignore_paths.py` & `allianceauth-3.5.0/allianceauth/analytics/migrations/0006_more_ignore_paths.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/models.py` & `allianceauth-3.5.0/allianceauth/analytics/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/signals.py` & `allianceauth-3.5.0/allianceauth/analytics/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/tasks.py` & `allianceauth-3.5.0/allianceauth/analytics/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/tests/test_integration.py` & `allianceauth-3.5.0/allianceauth/analytics/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/tests/test_middleware.py` & `allianceauth-3.5.0/allianceauth/analytics/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/tests/test_models.py` & `allianceauth-3.5.0/allianceauth/analytics/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/tests/test_tasks.py` & `allianceauth-3.5.0/allianceauth/analytics/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/tests/test_utils.py` & `allianceauth-3.5.0/allianceauth/analytics/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/analytics/utils.py` & `allianceauth-3.5.0/allianceauth/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/admin.py` & `allianceauth-3.5.0/allianceauth/authentication/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/app_settings.py` & `allianceauth-3.5.0/allianceauth/authentication/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/apps.py` & `allianceauth-3.5.0/allianceauth/authentication/apps.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/backends.py` & `allianceauth-3.5.0/allianceauth/authentication/backends.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/decorators.py` & `allianceauth-3.5.0/allianceauth/authentication/decorators.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/forms.py` & `allianceauth-3.5.0/allianceauth/authentication/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/hmac_urls.py` & `allianceauth-3.5.0/allianceauth/authentication/hmac_urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/management/commands/checkmains.py` & `allianceauth-3.5.0/allianceauth/authentication/management/commands/checkmains.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/managers.py` & `allianceauth-3.5.0/allianceauth/authentication/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/middleware.py` & `allianceauth-3.5.0/allianceauth/authentication/middleware.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/authentication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/migrations/0004_create_permissions.py` & `allianceauth-3.5.0/allianceauth/authentication/migrations/0004_create_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/migrations/0005_delete_perms.py` & `allianceauth-3.5.0/allianceauth/authentication/migrations/0005_delete_perms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/migrations/0006_auto_20160910_0542.py` & `allianceauth-3.5.0/allianceauth/authentication/migrations/0006_auto_20160910_0542.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/migrations/0009_auto_20161021_0228.py` & `allianceauth-3.5.0/allianceauth/authentication/migrations/0009_auto_20161021_0228.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py` & `allianceauth-3.5.0/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py` & `allianceauth-3.5.0/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py` & `allianceauth-3.5.0/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/migrations/0013_service_modules.py` & `allianceauth-3.5.0/allianceauth/authentication/migrations/0013_service_modules.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/migrations/0014_fleetup_permission.py` & `allianceauth-3.5.0/allianceauth/authentication/migrations/0014_fleetup_permission.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/migrations/0015_user_profiles.py` & `allianceauth-3.5.0/allianceauth/authentication/migrations/0015_user_profiles.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/migrations/0016_ownershiprecord.py` & `allianceauth-3.5.0/allianceauth/authentication/migrations/0016_ownershiprecord.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py` & `allianceauth-3.5.0/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/migrations/0018_state_member_factions.py` & `allianceauth-3.5.0/allianceauth/authentication/migrations/0018_state_member_factions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py` & `allianceauth-3.5.0/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/models.py` & `allianceauth-3.5.0/allianceauth/authentication/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,41 +59,46 @@
     return get_guest_state().pk
 
 
 class UserProfile(models.Model):
     class Meta:
         default_permissions = ('change',)
 
+    class Language(models.TextChoices):
+        """
+        Choices for UserProfile.language
+        """
+
+        ENGLISH = 'en', _('English')
+        GERMAN = 'de', _('German')
+        SPANISH = 'es', _('Spanish')
+        CHINESE = 'zh-hans', _('Chinese Simplified')
+        RUSSIAN = 'ru', _('Russian')
+        KOREAN = 'ko', _('Korean')
+        FRENCH = 'fr', _('French')
+        JAPANESE = 'ja', _('Japanese')
+        ITALIAN = 'it', _('Italian')
+        UKRAINIAN = 'uk', _('Ukrainian')
+
     user = models.OneToOneField(
         User,
         related_name='profile',
         on_delete=models.CASCADE)
     main_character = models.OneToOneField(
         EveCharacter,
         blank=True,
         null=True,
         on_delete=models.SET_NULL)
     state = models.ForeignKey(
         State,
         on_delete=models.SET_DEFAULT,
         default=get_guest_state_pk)
-    LANGUAGE_CHOICES = [
-        ('en', _('English')),
-        ('de', _('German')),
-        ('es', _('Spanish')),
-        ('zh-hans', _('Chinese Simplified')),
-        ('ru', _('Russian')),
-        ('ko', _('Korean')),
-        ('fr', _('French')),
-        ('ja', _('Japanese')),
-        ('it', _('Italian')),
-    ]
     language = models.CharField(
         _("Language"), max_length=10,
-        choices=LANGUAGE_CHOICES,
+        choices=Language.choices,
         blank=True,
         default='')
     night_mode = models.BooleanField(
         _("Night Mode"),
         blank=True,
         null=True)
```

### Comparing `allianceauth-3.4.0/allianceauth/authentication/signals.py` & `allianceauth-3.5.0/allianceauth/authentication/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg` & `allianceauth-3.5.0/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png` & `allianceauth-3.5.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png` & `allianceauth-3.5.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/task_statistics/counters.py` & `allianceauth-3.5.0/allianceauth/authentication/task_statistics/counters.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/task_statistics/event_series.py` & `allianceauth-3.5.0/allianceauth/authentication/task_statistics/event_series.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/task_statistics/signals.py` & `allianceauth-3.5.0/allianceauth/authentication/task_statistics/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/task_statistics/tests/test_counters.py` & `allianceauth-3.5.0/allianceauth/authentication/task_statistics/tests/test_counters.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/task_statistics/tests/test_event_series.py` & `allianceauth-3.5.0/allianceauth/authentication/task_statistics/tests/test_event_series.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/task_statistics/tests/test_signals.py` & `allianceauth-3.5.0/allianceauth/authentication/task_statistics/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/tasks.py` & `allianceauth-3.5.0/allianceauth/authentication/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/templates/authentication/dashboard.html` & `allianceauth-3.5.0/allianceauth/authentication/templates/authentication/dashboard.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/templates/authentication/tokens.html` & `allianceauth-3.5.0/allianceauth/authentication/templates/authentication/tokens.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/templates/public/base.html` & `allianceauth-3.5.0/allianceauth/authentication/templates/public/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/templates/public/lang_select.html` & `allianceauth-3.5.0/allianceauth/authentication/templates/public/lang_select.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/templates/public/middle_box.html` & `allianceauth-3.5.0/allianceauth/authentication/templates/public/middle_box.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/templates/public/register.html` & `allianceauth-3.5.0/allianceauth/authentication/templates/public/register.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/tests/__init__.py` & `allianceauth-3.5.0/allianceauth/authentication/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/tests/test_admin.py` & `allianceauth-3.5.0/allianceauth/authentication/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/tests/test_app_settings.py` & `allianceauth-3.5.0/allianceauth/authentication/tests/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/tests/test_backend.py` & `allianceauth-3.5.0/allianceauth/authentication/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/tests/test_commands.py` & `allianceauth-3.5.0/allianceauth/authentication/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/tests/test_decorators.py` & `allianceauth-3.5.0/allianceauth/authentication/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/tests/test_middleware.py` & `allianceauth-3.5.0/allianceauth/authentication/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/tests/test_models.py` & `allianceauth-3.5.0/allianceauth/authentication/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/tests/test_signals.py` & `allianceauth-3.5.0/allianceauth/authentication/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/tests/test_templatetags.py` & `allianceauth-3.5.0/allianceauth/authentication/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/urls.py` & `allianceauth-3.5.0/allianceauth/authentication/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/authentication/views.py` & `allianceauth-3.5.0/allianceauth/authentication/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/bin/allianceauth.py` & `allianceauth-3.5.0/allianceauth/bin/allianceauth.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/corputils/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/corputils/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/corputils/managers.py` & `allianceauth-3.5.0/allianceauth/corputils/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/corputils/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/corputils/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/corputils/migrations/0002_migrate_permissions.py` & `allianceauth-3.5.0/allianceauth/corputils/migrations/0002_migrate_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/corputils/migrations/0003_granular_permissions.py` & `allianceauth-3.5.0/allianceauth/corputils/migrations/0003_granular_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/corputils/migrations/0004_member_models.py` & `allianceauth-3.5.0/allianceauth/corputils/migrations/0004_member_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/corputils/migrations/0005_cleanup_permissions.py` & `allianceauth-3.5.0/allianceauth/corputils/migrations/0005_cleanup_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/corputils/models.py` & `allianceauth-3.5.0/allianceauth/corputils/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/corputils/swagger.json` & `allianceauth-3.5.0/allianceauth/corputils/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/corputils/templates/corputils/base.html` & `allianceauth-3.5.0/allianceauth/corputils/templates/corputils/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/corputils/templates/corputils/corpstats.html` & `allianceauth-3.5.0/allianceauth/corputils/templates/corputils/corpstats.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/corputils/templates/corputils/search.html` & `allianceauth-3.5.0/allianceauth/corputils/templates/corputils/search.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/corputils/tests.py` & `allianceauth-3.5.0/allianceauth/corputils/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/corputils/views.py` & `allianceauth-3.5.0/allianceauth/corputils/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/admin.py` & `allianceauth-3.5.0/allianceauth/eveonline/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/autogroups/admin.py` & `allianceauth-3.5.0/allianceauth/eveonline/autogroups/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/autogroups/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/eveonline/autogroups/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/autogroups/models.py` & `allianceauth-3.5.0/allianceauth/eveonline/autogroups/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/autogroups/signals.py` & `allianceauth-3.5.0/allianceauth/eveonline/autogroups/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/autogroups/tests/__init__.py` & `allianceauth-3.5.0/allianceauth/eveonline/autogroups/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/autogroups/tests/test_managers.py` & `allianceauth-3.5.0/allianceauth/eveonline/autogroups/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/autogroups/tests/test_models.py` & `allianceauth-3.5.0/allianceauth/eveonline/autogroups/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/autogroups/tests/test_signals.py` & `allianceauth-3.5.0/allianceauth/eveonline/autogroups/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/evelinks/__init__.py` & `allianceauth-3.5.0/allianceauth/eveonline/evelinks/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/evelinks/dotlan.py` & `allianceauth-3.5.0/allianceauth/eveonline/evelinks/dotlan.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/evelinks/eveimageserver.py` & `allianceauth-3.5.0/allianceauth/eveonline/evelinks/eveimageserver.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/evelinks/evewho.py` & `allianceauth-3.5.0/allianceauth/eveonline/evelinks/evewho.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/evelinks/tests/test_evelinks.py` & `allianceauth-3.5.0/allianceauth/eveonline/evelinks/tests/test_evelinks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/evelinks/tests/test_templatetags.py` & `allianceauth-3.5.0/allianceauth/eveonline/evelinks/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/evelinks/zkillboard.py` & `allianceauth-3.5.0/allianceauth/eveonline/evelinks/zkillboard.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/managers.py` & `allianceauth-3.5.0/allianceauth/eveonline/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/eveonline/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py` & `allianceauth-3.5.0/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py` & `allianceauth-3.5.0/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/migrations/0007_unique_id_name.py` & `allianceauth-3.5.0/allianceauth/eveonline/migrations/0007_unique_id_name.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/migrations/0008_remove_apikeys.py` & `allianceauth-3.5.0/allianceauth/eveonline/migrations/0008_remove_apikeys.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/migrations/0009_on_delete.py` & `allianceauth-3.5.0/allianceauth/eveonline/migrations/0009_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/migrations/0010_alliance_ticker.py` & `allianceauth-3.5.0/allianceauth/eveonline/migrations/0010_alliance_ticker.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/migrations/0011_ids_to_integers.py` & `allianceauth-3.5.0/allianceauth/eveonline/migrations/0011_ids_to_integers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/migrations/0012_index_additions.py` & `allianceauth-3.5.0/allianceauth/eveonline/migrations/0012_index_additions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/migrations/0015_factions.py` & `allianceauth-3.5.0/allianceauth/eveonline/migrations/0015_factions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py` & `allianceauth-3.5.0/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/models.py` & `allianceauth-3.5.0/allianceauth/eveonline/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/providers.py` & `allianceauth-3.5.0/allianceauth/eveonline/providers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/swagger.json` & `allianceauth-3.5.0/allianceauth/eveonline/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/tasks.py` & `allianceauth-3.5.0/allianceauth/eveonline/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/templatetags/evelinks.py` & `allianceauth-3.5.0/allianceauth/eveonline/templatetags/evelinks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/templatetags/examples.html` & `allianceauth-3.5.0/allianceauth/eveonline/templatetags/examples.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/tests/__init__.py` & `allianceauth-3.5.0/allianceauth/eveonline/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/tests/esi_client_stub.py` & `allianceauth-3.5.0/allianceauth/eveonline/tests/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/tests/swagger_old.json` & `allianceauth-3.5.0/allianceauth/eveonline/tests/swagger_old.json`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/tests/test_managers.py` & `allianceauth-3.5.0/allianceauth/eveonline/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/tests/test_models.py` & `allianceauth-3.5.0/allianceauth/eveonline/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/tests/test_providers.py` & `allianceauth-3.5.0/allianceauth/eveonline/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/eveonline/tests/test_tasks.py` & `allianceauth-3.5.0/allianceauth/eveonline/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/fleetactivitytracking/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/fleetactivitytracking/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/fleetactivitytracking/models.py` & `allianceauth-3.5.0/allianceauth/fleetactivitytracking/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/fleetactivitytracking/swagger.json` & `allianceauth-3.5.0/allianceauth/fleetactivitytracking/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html` & `allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkformatter.html` & `allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkformatter.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html` & `allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html` & `allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html` & `allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html` & `allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html` & `allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html` & `allianceauth-3.5.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/fleetactivitytracking/urls.py` & `allianceauth-3.5.0/allianceauth/fleetactivitytracking/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/fleetactivitytracking/views.py` & `allianceauth-3.5.0/allianceauth/fleetactivitytracking/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/admin.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/forms.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/managers.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0004_authgroup.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0004_authgroup.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0005_authgroup_public.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0005_authgroup_public.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0007_on_delete.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0007_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0009_requestlog.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0009_requestlog.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0010_authgroup_states.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0010_authgroup_states.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0012_group_leads.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0012_group_leads.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/models.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/signals.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/templates/groupmanagement/audit.html` & `allianceauth-3.5.0/allianceauth/groupmanagement/templates/groupmanagement/audit.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html` & `allianceauth-3.5.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html` & `allianceauth-3.5.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/templates/groupmanagement/groups.html` & `allianceauth-3.5.0/allianceauth/groupmanagement/templates/groupmanagement/groups.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/templates/groupmanagement/index.html` & `allianceauth-3.5.0/allianceauth/groupmanagement/templates/groupmanagement/index.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/templates/groupmanagement/menu.html` & `allianceauth-3.5.0/allianceauth/groupmanagement/templates/groupmanagement/menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/tests/test_admin.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/tests/test_managers.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/tests/test_models.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/tests/test_signals.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/tests/test_views.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/urls.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/groupmanagement/views.py` & `allianceauth-3.5.0/allianceauth/groupmanagement/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hooks.py` & `allianceauth-3.5.0/allianceauth/hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/admin.py` & `allianceauth-3.5.0/allianceauth/hrapplications/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/hrapplications/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/managers.py` & `allianceauth-3.5.0/allianceauth/hrapplications/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/hrapplications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/migrations/0002_choices_for_questions.py` & `allianceauth-3.5.0/allianceauth/hrapplications/migrations/0002_choices_for_questions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py` & `allianceauth-3.5.0/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/migrations/0005_sorted_questions.py` & `allianceauth-3.5.0/allianceauth/hrapplications/migrations/0005_sorted_questions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py` & `allianceauth-3.5.0/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/models.py` & `allianceauth-3.5.0/allianceauth/hrapplications/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/templates/hrapplications/corpchoice.html` & `allianceauth-3.5.0/allianceauth/hrapplications/templates/hrapplications/corpchoice.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/templates/hrapplications/create.html` & `allianceauth-3.5.0/allianceauth/hrapplications/templates/hrapplications/create.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/templates/hrapplications/management.html` & `allianceauth-3.5.0/allianceauth/hrapplications/templates/hrapplications/management.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/templates/hrapplications/searchview.html` & `allianceauth-3.5.0/allianceauth/hrapplications/templates/hrapplications/searchview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/templates/hrapplications/view.html` & `allianceauth-3.5.0/allianceauth/hrapplications/templates/hrapplications/view.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/tests.py` & `allianceauth-3.5.0/allianceauth/hrapplications/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/urls.py` & `allianceauth-3.5.0/allianceauth/hrapplications/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/hrapplications/views.py` & `allianceauth-3.5.0/allianceauth/hrapplications/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 @login_required
 @user_passes_test(create_application_test)
 def hr_application_create_view(request, form_id=None):
     if form_id:
         app_form = get_object_or_404(ApplicationForm, id=form_id)
         if request.method == "POST":
             if Application.objects.filter(user=request.user).filter(form=app_form).exists():
-                logger.warn(f"User {request.user} attempting to duplicate application to {app_form.corp}")
+                logger.warning(f"User {request.user} attempting to duplicate application to {app_form.corp}")
             else:
                 application = Application(user=request.user, form=app_form)
                 application.save()
                 for question in app_form.questions.all():
                     response = ApplicationResponse(question=question, application=application)
                     response.answer = "\n".join(request.POST.getlist(str(question.pk), ""))
                     response.save()
@@ -88,30 +88,30 @@
             'responses': ApplicationResponse.objects.filter(application=app),
             'buttons': False,
             'comments': ApplicationComment.objects.filter(application=app),
             'comment_form': HRApplicationCommentForm(),
         }
         return render(request, 'hrapplications/view.html', context=context)
     else:
-        logger.warn(f"User {request.user} not authorized to view {app}")
+        logger.warning(f"User {request.user} not authorized to view {app}")
         return redirect('hrapplications:personal_view')
 
 
 @login_required
 def hr_application_personal_removal(request, app_id):
     logger.debug(f"hr_application_personal_removal called by user {request.user} for app id {app_id}")
     app = get_object_or_404(Application, pk=app_id)
     if app.user == request.user:
         if app.approved is None:
             logger.info(f"User {request.user} deleting {app}")
             app.delete()
         else:
-            logger.warn(f"User {request.user} attempting to delete reviewed app {app}")
+            logger.warning(f"User {request.user} attempting to delete reviewed app {app}")
     else:
-        logger.warn(f"User {request.user} not authorized to delete {app}")
+        logger.warning(f"User {request.user} not authorized to delete {app}")
     return redirect('hrapplications:index')
 
 
 @login_required
 @permission_required('auth.human_resources')
 def hr_application_view(request, app_id):
     logger.debug(f"hr_application_view called by user {request.user} for app id {app_id}")
@@ -128,15 +128,15 @@
                 comment.application = app
                 comment.user = request.user
                 comment.text = form.cleaned_data['comment']
                 comment.save()
                 logger.info(f"Saved comment by user {request.user} to {app}")
                 return redirect('hrapplications:view', app_id)
         else:
-            logger.warn("User %s does not have permission to add ApplicationComments" % request.user)
+            logger.warning("User %s does not have permission to add ApplicationComments" % request.user)
             return redirect('hrapplications:view', app_id)
     else:
         logger.debug("Returning blank HRApplication comment form.")
         form = HRApplicationCommentForm()
     context = {
         'app': app,
         'responses': app.responses.all(),
@@ -167,15 +167,15 @@
     app = get_object_or_404(Application, pk=app_id)
     if request.user.is_superuser or request.user == app.reviewer:
         logger.info(f"User {request.user} approving {app}")
         app.approved = True
         app.save()
         notify(app.user, "Application Accepted", message="Your application to %s has been approved." % app.form.corp, level="success")
     else:
-        logger.warn(f"User {request.user} not authorized to approve {app}")
+        logger.warning(f"User {request.user} not authorized to approve {app}")
     return redirect('hrapplications:index')
 
 
 @login_required
 @permission_required('auth.human_resources')
 @permission_required('hrapplications.reject_application')
 def hr_application_reject(request, app_id):
@@ -183,15 +183,15 @@
     app = get_object_or_404(Application, pk=app_id)
     if request.user.is_superuser or request.user == app.reviewer:
         logger.info(f"User {request.user} rejecting {app}")
         app.approved = False
         app.save()
         notify(app.user, "Application Rejected", message="Your application to %s has been rejected." % app.form.corp, level="danger")
     else:
-        logger.warn(f"User {request.user} not authorized to reject {app}")
+        logger.warning(f"User {request.user} not authorized to reject {app}")
     return redirect('hrapplications:index')
 
 
 @login_required
 @permission_required('auth.human_resources')
 def hr_application_search(request):
     logger.debug("hr_application_search called by user %s" % request.user)
@@ -204,15 +204,15 @@
             logger.debug(f"Searching for application with character name {searchstring} for user {request.user}")
             app_list = Application.objects.all()
             if not request.user.is_superuser:
                 try:
                     app_list = app_list.filter(
                         form__corp__corporation_id=request.user.profile.main_character.corporation_id)
                 except AttributeError:
-                    logger.warn(
+                    logger.warning(
                         "User %s missing main character model: unable to filter applications to search" % request.user)
 
             applications = app_list.filter(
                 Q(user__profile__main_character__character_name__icontains=searchstring) |
                 Q(user__profile__main_character__corporation_name__icontains=searchstring) |
                 Q(user__profile__main_character__alliance_name__icontains=searchstring) |
                 Q(user__character_ownerships__character__character_name__icontains=searchstring) |
@@ -242,10 +242,10 @@
     if not app.reviewer:
         logger.info(f"User {request.user} marking {app} in progress")
         app.reviewer = request.user
         app.reviewer_character = request.user.profile.main_character
         app.save()
         notify(app.user, "Application In Progress", message=f"Your application to {app.form.corp} is being reviewed by {app.reviewer_str}")
     else:
-        logger.warn(
+        logger.warning(
             f"User {request.user} unable to mark {app} in progress: already being reviewed by {app.reviewer}")
     return redirect("hrapplications:view", app_id)
```

### Comparing `allianceauth-3.4.0/allianceauth/locale/de/LC_MESSAGES/django.mo` & `allianceauth-3.5.0/allianceauth/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/de/LC_MESSAGES/django.po` & `allianceauth-3.5.0/allianceauth/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/en/LC_MESSAGES/django.po` & `allianceauth-3.5.0/allianceauth/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/es/LC_MESSAGES/django.mo` & `allianceauth-3.5.0/allianceauth/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/es/LC_MESSAGES/django.po` & `allianceauth-3.5.0/allianceauth/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo` & `allianceauth-3.5.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.po` & `allianceauth-3.5.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/it_IT/LC_MESSAGES/django.mo` & `allianceauth-3.5.0/allianceauth/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/it_IT/LC_MESSAGES/django.po` & `allianceauth-3.5.0/allianceauth/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/ja/LC_MESSAGES/django.mo` & `allianceauth-3.5.0/allianceauth/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/ja/LC_MESSAGES/django.po` & `allianceauth-3.5.0/allianceauth/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo` & `allianceauth-3.5.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.po` & `allianceauth-3.5.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/ru/LC_MESSAGES/django.mo` & `allianceauth-3.5.0/allianceauth/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/ru/LC_MESSAGES/django.po` & `allianceauth-3.5.0/allianceauth/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/uk/LC_MESSAGES/django.mo` & `allianceauth-3.5.0/allianceauth/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/uk/LC_MESSAGES/django.po` & `allianceauth-3.5.0/allianceauth/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo` & `allianceauth-3.5.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po` & `allianceauth-3.5.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/admin.py` & `allianceauth-3.5.0/allianceauth/notifications/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/core.py` & `allianceauth-3.5.0/allianceauth/notifications/core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/handlers.py` & `allianceauth-3.5.0/allianceauth/notifications/handlers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/managers.py` & `allianceauth-3.5.0/allianceauth/notifications/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py` & `allianceauth-3.5.0/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/migrations/0004_performance_tuning.py` & `allianceauth-3.5.0/allianceauth/notifications/migrations/0004_performance_tuning.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/migrations/0005_fix_level_choices.py` & `allianceauth-3.5.0/allianceauth/notifications/migrations/0005_fix_level_choices.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/models.py` & `allianceauth-3.5.0/allianceauth/notifications/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/templates/notifications/list.html` & `allianceauth-3.5.0/allianceauth/notifications/templates/notifications/list.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/templates/notifications/list_partial.html` & `allianceauth-3.5.0/allianceauth/notifications/templates/notifications/list_partial.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/templates/notifications/view.html` & `allianceauth-3.5.0/allianceauth/notifications/templates/notifications/view.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/templatetags/auth_notifications.py` & `allianceauth-3.5.0/allianceauth/notifications/templatetags/auth_notifications.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/tests/test_core.py` & `allianceauth-3.5.0/allianceauth/notifications/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/tests/test_handlers.py` & `allianceauth-3.5.0/allianceauth/notifications/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/tests/test_init.py` & `allianceauth-3.5.0/allianceauth/notifications/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/tests/test_managers.py` & `allianceauth-3.5.0/allianceauth/notifications/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/tests/test_models.py` & `allianceauth-3.5.0/allianceauth/notifications/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/tests/test_templatetags.py` & `allianceauth-3.5.0/allianceauth/notifications/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/tests/test_views.py` & `allianceauth-3.5.0/allianceauth/notifications/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/urls.py` & `allianceauth-3.5.0/allianceauth/notifications/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/notifications/views.py` & `allianceauth-3.5.0/allianceauth/notifications/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     notif = get_object_or_404(Notification, pk=notif_id)
     if notif.user == request.user:
         logger.debug("Providing notification for user %s", request.user)
         context = {'notif': notif}
         notif.mark_viewed()
         return render(request, 'notifications/view.html', context)
     else:
-        logger.warn(
+        logger.warning(
             "User %s not authorized to view notif_id %s belonging to user %s",
             request.user,
             notif_id, notif.user
         )
         messages.error(request, _('You are not authorized to view that notification.'))
         return redirect('notifications:list')
```

### Comparing `allianceauth-3.4.0/allianceauth/optimer/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/optimer/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/optimer/form.py` & `allianceauth-3.5.0/allianceauth/optimer/form.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/optimer/form_widgets.py` & `allianceauth-3.5.0/allianceauth/optimer/form_widgets.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/optimer/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/optimer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py` & `allianceauth-3.5.0/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/optimer/migrations/0005_add_type_and_description.py` & `allianceauth-3.5.0/allianceauth/optimer/migrations/0005_add_type_and_description.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/optimer/models.py` & `allianceauth-3.5.0/allianceauth/optimer/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/optimer/templates/optimer/add.html` & `allianceauth-3.5.0/allianceauth/optimer/templates/optimer/add.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/optimer/templates/optimer/fleetoptable.html` & `allianceauth-3.5.0/allianceauth/optimer/templates/optimer/fleetoptable.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/optimer/templates/optimer/management.html` & `allianceauth-3.5.0/allianceauth/optimer/templates/optimer/management.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/optimer/templates/optimer/update.html` & `allianceauth-3.5.0/allianceauth/optimer/templates/optimer/update.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/optimer/views.py` & `allianceauth-3.5.0/allianceauth/optimer/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/permissions_tool/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/permissions_tool/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/permissions_tool/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/permissions_tool/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/permissions_tool/templates/permissions_tool/audit.html` & `allianceauth-3.5.0/allianceauth/permissions_tool/templates/permissions_tool/audit.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html` & `allianceauth-3.5.0/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/permissions_tool/templates/permissions_tool/overview.html` & `allianceauth-3.5.0/allianceauth/permissions_tool/templates/permissions_tool/overview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/permissions_tool/tests.py` & `allianceauth-3.5.0/allianceauth/permissions_tool/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/permissions_tool/views.py` & `allianceauth-3.5.0/allianceauth/permissions_tool/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/project_template/manage.py` & `allianceauth-3.5.0/allianceauth/project_template/manage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/project_template/project_name/celery.py` & `allianceauth-3.5.0/allianceauth/project_template/project_name/celery.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/project_template/project_name/settings/base.py` & `allianceauth-3.5.0/allianceauth/project_template/project_name/settings/base.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/project_template/project_name/settings/local.py` & `allianceauth-3.5.0/allianceauth/project_template/project_name/settings/local.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/project_template/supervisor.conf` & `allianceauth-3.5.0/allianceauth/project_template/supervisor.conf`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/abstract.py` & `allianceauth-3.5.0/allianceauth/services/abstract.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/admin.py` & `allianceauth-3.5.0/allianceauth/services/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/services/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/forms.py` & `allianceauth-3.5.0/allianceauth/services/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/hooks.py` & `allianceauth-3.5.0/allianceauth/services/hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/migrations/0002_nameformatter.py` & `allianceauth-3.5.0/allianceauth/services/migrations/0002_nameformatter.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/migrations/0003_remove_broken_link.py` & `allianceauth-3.5.0/allianceauth/services/migrations/0003_remove_broken_link.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/models.py` & `allianceauth-3.5.0/allianceauth/services/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/admin.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/api.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/api.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/app_settings.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/core.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/app_settings.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/client.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/client.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/exceptions.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/helpers.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/models.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/example_objects.json` & `allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/example_objects.json`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/factories.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/factories.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md` & `allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/test_client.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/discord_client/tests/test_models.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/discord_client/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/managers.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/migrations/0002_service_permissions.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/models.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/tasks.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html` & `allianceauth-3.5.0/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/tests/factories.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/tests/factories.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/tests/piloting_tasks.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/tests/piloting_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_admin.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_api.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_auth_hooks.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_core.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_integration.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_managers.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_models.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_tasks.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_utils.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/tests/test_views.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/urls.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/utils.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discord/views.py` & `allianceauth-3.5.0/allianceauth/services/modules/discord/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discourse/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/services/modules/discourse/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discourse/manager.py` & `allianceauth-3.5.0/allianceauth/services/modules/discourse/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discourse/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/services/modules/discourse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py` & `allianceauth-3.5.0/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discourse/models.py` & `allianceauth-3.5.0/allianceauth/services/modules/discourse/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discourse/providers.py` & `allianceauth-3.5.0/allianceauth/services/modules/discourse/providers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discourse/tasks.py` & `allianceauth-3.5.0/allianceauth/services/modules/discourse/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def update_groups(self, pk):
         user = User.objects.get(pk=pk)
         logger.debug("Updating discourse groups for user %s" % user)
         try:
             DiscourseManager.update_groups(user)
         except Exception as e:
             logger.exception(e)
-            logger.warn("Discourse group sync failed for %s, retrying in 10 mins" % user)
+            logger.warning("Discourse group sync failed for %s, retrying in 10 mins" % user)
             raise self.retry(countdown=60 * 10)
         logger.debug("Updated user %s discourse groups." % user)
 
     @staticmethod
     @shared_task(name='discourse.update_all_groups')
     def update_all_groups():
         logger.debug("Updating ALL discourse groups")
```

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discourse/tests.py` & `allianceauth-3.5.0/allianceauth/services/modules/discourse/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/discourse/views.py` & `allianceauth-3.5.0/allianceauth/services/modules/discourse/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/example/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/services/modules/example/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/ips4/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/services/modules/ips4/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/ips4/manager.py` & `allianceauth-3.5.0/allianceauth/services/modules/ips4/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/ips4/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/services/modules/ips4/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py` & `allianceauth-3.5.0/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/ips4/models.py` & `allianceauth-3.5.0/allianceauth/services/modules/ips4/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/ips4/tasks.py` & `allianceauth-3.5.0/allianceauth/services/modules/ips4/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/ips4/tests.py` & `allianceauth-3.5.0/allianceauth/services/modules/ips4/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/ips4/urls.py` & `allianceauth-3.5.0/allianceauth/services/modules/ips4/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/ips4/views.py` & `allianceauth-3.5.0/allianceauth/services/modules/ips4/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/models.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/tasks.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/tests.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/urls.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/mumble/views.py` & `allianceauth-3.5.0/allianceauth/services/modules/mumble/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/openfire/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/services/modules/openfire/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/openfire/manager.py` & `allianceauth-3.5.0/allianceauth/services/modules/openfire/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/openfire/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/services/modules/openfire/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py` & `allianceauth-3.5.0/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/openfire/tasks.py` & `allianceauth-3.5.0/allianceauth/services/modules/openfire/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html` & `allianceauth-3.5.0/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/openfire/tests.py` & `allianceauth-3.5.0/allianceauth/services/modules/openfire/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/openfire/urls.py` & `allianceauth-3.5.0/allianceauth/services/modules/openfire/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/openfire/views.py` & `allianceauth-3.5.0/allianceauth/services/modules/openfire/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/phpbb3/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/services/modules/phpbb3/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/phpbb3/manager.py` & `allianceauth-3.5.0/allianceauth/services/modules/phpbb3/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
         username_clean = Phpbb3Manager.__santatize_username(username)
         password = Phpbb3Manager.__generate_random_pass()
         pwhash = Phpbb3Manager.__gen_hash(password)
         logger.debug(f"Proceeding to add phpbb user {username_clean} and pwhash starting with {pwhash[0:5]}")
         # check if the username was simply revoked
         if Phpbb3Manager.check_user(username_clean):
-            logger.warn("Unable to add phpbb user with username %s - already exists. Updating user instead." % username)
+            logger.warning("Unable to add phpbb user with username %s - already exists. Updating user instead." % username)
             Phpbb3Manager.__update_user_info(username_clean, email, pwhash)
         else:
             try:
 
                 cursor.execute(Phpbb3Manager.SQL_ADD_USER, [username_clean, username_clean, pwhash,
                                                             email, 2, Phpbb3Manager.__get_current_utc_date(),
                                                             "", ""])
```

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/phpbb3/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/services/modules/phpbb3/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py` & `allianceauth-3.5.0/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/phpbb3/tasks.py` & `allianceauth-3.5.0/allianceauth/services/modules/phpbb3/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/phpbb3/tests.py` & `allianceauth-3.5.0/allianceauth/services/modules/phpbb3/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/phpbb3/urls.py` & `allianceauth-3.5.0/allianceauth/services/modules/phpbb3/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/phpbb3/views.py` & `allianceauth-3.5.0/allianceauth/services/modules/phpbb3/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/smf/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/services/modules/smf/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/smf/manager.py` & `allianceauth-3.5.0/allianceauth/services/modules/smf/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/smf/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/services/modules/smf/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/smf/migrations/0002_service_permissions.py` & `allianceauth-3.5.0/allianceauth/services/modules/smf/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py` & `allianceauth-3.5.0/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/smf/tasks.py` & `allianceauth-3.5.0/allianceauth/services/modules/smf/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/smf/tests.py` & `allianceauth-3.5.0/allianceauth/services/modules/smf/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/smf/urls.py` & `allianceauth-3.5.0/allianceauth/services/modules/smf/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/smf/views.py` & `allianceauth-3.5.0/allianceauth/services/modules/smf/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/admin.py` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/manager.py` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/models.py` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/signals.py` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/tasks.py` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/tests.py` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/urls.py` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/util/ts3.py` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/util/ts3.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/teamspeak3/views.py` & `allianceauth-3.5.0/allianceauth/services/modules/teamspeak3/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 @login_required
 @permission_required(ACCESS_PERM)
 def verify_teamspeak3(request):
     logger.debug("verify_teamspeak3 called by user %s" % request.user)
     if not Teamspeak3Tasks.has_account(request.user):
-        logger.warn("Unable to validate user %s teamspeak: no teamspeak data" % request.user)
+        logger.warning("Unable to validate user %s teamspeak: no teamspeak data" % request.user)
         return redirect("services:services")
     if request.method == "POST":
         form = TeamspeakJoinForm(request.POST)
         if form.is_valid():
             Teamspeak3Tasks.update_groups.delay(request.user.pk)
             logger.debug("Validated user %s joined TS server" % request.user)
             return redirect("services:services")
```

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/xenforo/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/services/modules/xenforo/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/xenforo/manager.py` & `allianceauth-3.5.0/allianceauth/services/modules/xenforo/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/xenforo/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/services/modules/xenforo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py` & `allianceauth-3.5.0/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/xenforo/tasks.py` & `allianceauth-3.5.0/allianceauth/services/modules/xenforo/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/xenforo/tests.py` & `allianceauth-3.5.0/allianceauth/services/modules/xenforo/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/xenforo/urls.py` & `allianceauth-3.5.0/allianceauth/services/modules/xenforo/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/modules/xenforo/views.py` & `allianceauth-3.5.0/allianceauth/services/modules/xenforo/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/signals.py` & `allianceauth-3.5.0/allianceauth/services/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/tasks.py` & `allianceauth-3.5.0/allianceauth/services/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/templates/services/fleetformattertool.html` & `allianceauth-3.5.0/allianceauth/services/templates/services/fleetformattertool.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/templates/services/service_confirm_delete.html` & `allianceauth-3.5.0/allianceauth/services/templates/services/service_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/templates/services/service_credentials.html` & `allianceauth-3.5.0/allianceauth/services/templates/services/service_credentials.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/templates/services/service_password.html` & `allianceauth-3.5.0/allianceauth/services/templates/services/service_password.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/templates/services/services.html` & `allianceauth-3.5.0/allianceauth/services/templates/services/services.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/templates/services/services_ctrl.html` & `allianceauth-3.5.0/allianceauth/services/templates/services/services_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/templatetags/menu_items.py` & `allianceauth-3.5.0/allianceauth/services/templatetags/menu_items.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/tests/test_models.py` & `allianceauth-3.5.0/allianceauth/services/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/tests/test_nameformatter.py` & `allianceauth-3.5.0/allianceauth/services/tests/test_nameformatter.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/tests/test_signals.py` & `allianceauth-3.5.0/allianceauth/services/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/tests/test_tasks.py` & `allianceauth-3.5.0/allianceauth/services/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/urls.py` & `allianceauth-3.5.0/allianceauth/services/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/services/views.py` & `allianceauth-3.5.0/allianceauth/services/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/srp/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/form.py` & `allianceauth-3.5.0/allianceauth/srp/form.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/managers.py` & `allianceauth-3.5.0/allianceauth/srp/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/srp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/migrations/0003_make_strings_more_stringy.py` & `allianceauth-3.5.0/allianceauth/srp/migrations/0003_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/migrations/0004_on_delete.py` & `allianceauth-3.5.0/allianceauth/srp/migrations/0004_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/models.py` & `allianceauth-3.5.0/allianceauth/srp/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/swagger.json` & `allianceauth-3.5.0/allianceauth/srp/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/templates/srp/add.html` & `allianceauth-3.5.0/allianceauth/srp/templates/srp/add.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/templates/srp/data.html` & `allianceauth-3.5.0/allianceauth/srp/templates/srp/data.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/templates/srp/management.html` & `allianceauth-3.5.0/allianceauth/srp/templates/srp/management.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/templates/srp/request.html` & `allianceauth-3.5.0/allianceauth/srp/templates/srp/request.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/templates/srp/update.html` & `allianceauth-3.5.0/allianceauth/srp/templates/srp/update.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/tests/test_managers.py` & `allianceauth-3.5.0/allianceauth/srp/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json` & `allianceauth-3.5.0/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/urls.py` & `allianceauth-3.5.0/allianceauth/srp/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/srp/views.py` & `allianceauth-3.5.0/allianceauth/srp/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/css/auth-base.css` & `allianceauth-3.5.0/allianceauth/static/allianceauth/css/auth-base.css`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/css/checkbox.css` & `allianceauth-3.5.0/allianceauth/static/allianceauth/css/checkbox.css`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less` & `allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/darkly/LICENSE` & `allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/darkly/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.less` & `allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.less`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css` & `allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/flatly/LICENSE` & `allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/flatly/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.less` & `allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.less`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css` & `allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/css/themes/flatly-shared.less` & `allianceauth-3.5.0/allianceauth/static/allianceauth/css/themes/flatly-shared.less`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/icons/allianceauth.png` & `allianceauth-3.5.0/allianceauth/static/allianceauth/icons/allianceauth.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/icons/apple-touch-icon.png` & `allianceauth-3.5.0/allianceauth/static/allianceauth/icons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/icons/favicon-32x32.png` & `allianceauth-3.5.0/allianceauth/static/allianceauth/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/icons/favicon-96x96.png` & `allianceauth-3.5.0/allianceauth/static/allianceauth/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/js/eve-time.js` & `allianceauth-3.5.0/allianceauth/static/allianceauth/js/eve-time.js`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/js/filterDropDown/LICENSE` & `allianceauth-3.5.0/allianceauth/static/allianceauth/js/filterDropDown/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js` & `allianceauth-3.5.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js` & `allianceauth-3.5.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png` & `allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png` & `allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png` & `allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png` & `allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png` & `allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png` & `allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css` & `allianceauth-3.5.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/js/refresh_notifications.js` & `allianceauth-3.5.0/allianceauth/static/allianceauth/js/refresh_notifications.js`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/static/allianceauth/js/timers.js` & `allianceauth-3.5.0/allianceauth/static/allianceauth/js/timers.js`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/templates/allianceauth/admin-status/overview.html` & `allianceauth-3.5.0/allianceauth/templates/allianceauth/admin-status/overview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/templates/allianceauth/base.html` & `allianceauth-3.5.0/allianceauth/templates/allianceauth/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/templates/allianceauth/messages.html` & `allianceauth-3.5.0/allianceauth/templates/allianceauth/messages.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/templates/allianceauth/side-menu.html` & `allianceauth-3.5.0/allianceauth/templates/allianceauth/side-menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/templates/allianceauth/top-menu-admin.html` & `allianceauth-3.5.0/allianceauth/templates/allianceauth/top-menu-admin.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/templates/allianceauth/top-menu-user-dropdown.html` & `allianceauth-3.5.0/allianceauth/templates/allianceauth/top-menu-user-dropdown.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/templates/allianceauth/top-menu.html` & `allianceauth-3.5.0/allianceauth/templates/allianceauth/top-menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/templates/bundles/bootstrap-css.html` & `allianceauth-3.5.0/allianceauth/templates/bundles/bootstrap-css.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/templates/bundles/bootstrap-js.html` & `allianceauth-3.5.0/allianceauth/templates/bundles/bootstrap-js.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/templates/bundles/datatables-js.html` & `allianceauth-3.5.0/allianceauth/templates/bundles/datatables-js.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/templates/bundles/moment-js.html` & `allianceauth-3.5.0/allianceauth/templates/bundles/moment-js.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/templatetags/admin_status.py` & `allianceauth-3.5.0/allianceauth/templatetags/admin_status.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/tests/auth_utils.py` & `allianceauth-3.5.0/allianceauth/tests/auth_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/tests/test_auth_utils.py` & `allianceauth-3.5.0/allianceauth/tests/test_auth_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/thirdparty/navhelper/templatetags/navactive.py` & `allianceauth-3.5.0/allianceauth/thirdparty/navhelper/templatetags/navactive.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/thirdparty/navhelper/tests.py` & `allianceauth-3.5.0/allianceauth/thirdparty/navhelper/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/timerboard/auth_hooks.py` & `allianceauth-3.5.0/allianceauth/timerboard/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/timerboard/form.py` & `allianceauth-3.5.0/allianceauth/timerboard/form.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/timerboard/migrations/0001_initial.py` & `allianceauth-3.5.0/allianceauth/timerboard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py` & `allianceauth-3.5.0/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/timerboard/migrations/0003_on_delete.py` & `allianceauth-3.5.0/allianceauth/timerboard/migrations/0003_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/timerboard/migrations/0004_timer_type.py` & `allianceauth-3.5.0/allianceauth/timerboard/migrations/0004_timer_type.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/timerboard/models.py` & `allianceauth-3.5.0/allianceauth/timerboard/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/timerboard/templates/timerboard/form.html` & `allianceauth-3.5.0/allianceauth/timerboard/templates/timerboard/form.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html` & `allianceauth-3.5.0/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/timerboard/templates/timerboard/view.html` & `allianceauth-3.5.0/allianceauth/timerboard/templates/timerboard/view.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/timerboard/tests.py` & `allianceauth-3.5.0/allianceauth/timerboard/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/timerboard/views.py` & `allianceauth-3.5.0/allianceauth/timerboard/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/urls.py` & `allianceauth-3.5.0/allianceauth/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/utils/cache.py` & `allianceauth-3.5.0/allianceauth/utils/cache.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/utils/django.py` & `allianceauth-3.5.0/allianceauth/utils/django.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/utils/testing.py` & `allianceauth-3.5.0/allianceauth/utils/testing.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/utils/tests/test_cache.py` & `allianceauth-3.5.0/allianceauth/utils/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/utils/tests/test_django.py` & `allianceauth-3.5.0/allianceauth/utils/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth/views.py` & `allianceauth-3.5.0/allianceauth/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.4.0/allianceauth.egg-info/PKG-INFO` & `allianceauth-3.5.0/allianceauth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth
-Version: 3.4.0
+Version: 3.5.0
 Summary: An auth system for EVE Online to help in-game organizations manage online service access.
 Home-page: https://gitlab.com/allianceauth/allianceauth
 Author: Alliance Auth
 Author-email: adarnof@gmail.com
 License: GPL-2.0
 Project-URL: Issue / Bug Reports, https://gitlab.com/allianceauth/allianceauth/-/issues
 Project-URL: Documentation, https://allianceauth.readthedocs.io/
```

### Comparing `allianceauth-3.4.0/allianceauth.egg-info/SOURCES.txt` & `allianceauth-3.5.0/allianceauth.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 allianceauth/authentication/migrations/0015_user_profiles.py
 allianceauth/authentication/migrations/0016_ownershiprecord.py
 allianceauth/authentication/migrations/0017_remove_fleetup_permission.py
 allianceauth/authentication/migrations/0018_alter_state_name_length.py
 allianceauth/authentication/migrations/0018_state_member_factions.py
 allianceauth/authentication/migrations/0019_merge_20211026_0919.py
 allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py
+allianceauth/authentication/migrations/0021_alter_userprofile_language.py
 allianceauth/authentication/migrations/__init__.py
 allianceauth/authentication/static/allianceauth/authentication/css/admin.css
 allianceauth/authentication/static/allianceauth/authentication/img/background.jpg
 allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png
 allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png
 allianceauth/authentication/task_statistics/__init__.py
 allianceauth/authentication/task_statistics/counters.py
```

### Comparing `allianceauth-3.4.0/setup.cfg` & `allianceauth-3.5.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 version = attr: allianceauth.__version__
 description = An auth system for EVE Online to help in-game organizations manage online service access.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Alliance Auth
 author_email = adarnof@gmail.com
 license = GPL-2.0
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 4
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 	Operating System :: POSIX :: Linux
@@ -40,15 +40,15 @@
 	celery>=5.2.0,<6
 	celery-once>=3.0.1
 	django>=4.0.9,<4.1.0
 	django-bootstrap-form
 	django-celery-beat>=2.3.0
 	django-esi>=4.0.1
 	django-redis>=5.2.0
-	django-registration>=3.3
+	django-registration>=3.3,<3.4
 	django-sortedm2m
 	dnspython
 	mysqlclient>=2.1.0
 	openfire-restapi
 	packaging>=21.0
 	passlib
 	pydiscourse
```

