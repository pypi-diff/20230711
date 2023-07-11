# Comparing `tmp/perseus_restful_api_framework-1.27.0.tar.gz` & `tmp/perseus_restful_api_framework-1.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perseus_restful_api_framework-1.27.0.tar", max compression
+gzip compressed data, was "perseus_restful_api_framework-1.27.1.tar", max compression
```

## Comparing `perseus_restful_api_framework-1.27.0.tar` & `perseus_restful_api_framework-1.27.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0    10124 2023-07-10 03:12:09.684175 perseus_restful_api_framework-1.27.0/CHANGELOG.md
--rw-r--r--   0        0        0     1089 2020-11-12 14:26:46.553799 perseus_restful_api_framework-1.27.0/LICENSE
--rw-r--r--   0        0        0     4530 2022-10-02 05:19:36.696561 perseus_restful_api_framework-1.27.0/README.md
--rw-r--r--   0        0        0     1140 2023-07-10 03:12:20.885001 perseus_restful_api_framework-1.27.0/pyproject.toml
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404748 perseus_restful_api_framework-1.27.0/src/majormode/__init__.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404886 perseus_restful_api_framework-1.27.0/src/majormode/perseus/__init__.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.405009 perseus_restful_api_framework-1.27.0/src/majormode/perseus/agent/__init__.py
--rwxr-xr-x   0        0        0    11953 2023-02-09 01:22:31.663266 perseus_restful_api_framework-1.27.0/src/majormode/perseus/agent/email_address_verification_agent.py
--rw-r--r--   0        0        0     3603 2023-02-09 01:21:55.716946 perseus_restful_api_framework-1.27.0/src/majormode/perseus/agent/email_sender_agent.py
--rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.405462 perseus_restful_api_framework-1.27.0/src/majormode/perseus/bootstrap/__init__.py
--rw-r--r--   0        0        0    17545 2023-02-09 01:22:31.663215 perseus_restful_api_framework-1.27.0/src/majormode/perseus/bootstrap/tornado_handler.py
--rw-r--r--   0        0        0     4900 2022-11-23 10:31:53.406176 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_currency_dataset.sql
--rwxr-xr-x   0        0        0     1892 2023-02-09 01:21:55.716943 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_exception_function.sql
--rw-r--r--   0        0        0     1547 2022-11-23 10:31:53.406510 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_geometry_function.sql
--rwxr-xr-x   0        0        0     1215 2022-11-23 10:31:53.406646 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_label_type.sql
--rwxr-xr-x   0        0        0     2684 2022-11-23 10:31:53.406769 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_locale_function.sql
--rwxr-xr-x   0        0        0     1269 2022-11-23 10:31:53.406909 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_object_constant.sql
--rw-r--r--   0        0        0     6696 2022-11-23 10:31:53.407036 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_object_table.sql
--rwxr-xr-x   0        0        0     1037 2022-11-23 10:31:53.407142 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_visibility_constant.sql
--rwxr-xr-x   0        0        0    13514 2023-02-09 01:22:42.266123 perseus_restful_api_framework-1.27.0/src/majormode/perseus/manage.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.407888 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/__init__.py
--rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.408088 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/__init__.py
--rwxr-xr-x   0        0        0   158602 2023-07-05 09:05:07.016526 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/account_service.py
--rw-r--r--   0        0        0    53061 2023-02-08 13:43:19.667427 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/contact_service.py
--rwxr-xr-x   0        0        0     3551 2023-03-03 01:25:29.385031 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_constraint.sql
--rwxr-xr-x   0        0        0     7947 2023-01-30 00:41:55.092554 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_function.sql
--rw-r--r--   0        0        0     1287 2022-11-23 10:31:53.411326 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_index.sql
--rwxr-xr-x   0        0        0    19425 2023-05-19 10:16:08.747757 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_table.sql
--rwxr-xr-x   0        0        0     1093 2022-11-23 10:31:53.412248 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_constraint.sql
--rwxr-xr-x   0        0        0     1101 2022-11-23 10:31:53.412521 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_function.sql
--rwxr-xr-x   0        0        0      989 2022-11-23 10:31:53.412719 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_index.sql
--rwxr-xr-x   0        0        0     1637 2022-11-23 10:31:53.413015 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_table.sql
--rwxr-xr-x   0        0        0     2093 2022-11-23 10:31:53.413203 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table.718.sql
--rwxr-xr-x   0        0        0      870 2022-11-23 10:31:53.413470 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql
--rwxr-xr-x   0        0        0     1033 2022-11-23 10:31:53.413751 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql
--rw-r--r--   0        0        0     1115 2022-11-23 10:31:53.414028 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql
--rw-r--r--   0        0        0     2599 2022-11-23 10:31:53.414316 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql
--rw-r--r--   0        0        0     1182 2022-11-23 10:31:53.414599 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql
--rw-r--r--   0        0        0      854 2022-11-23 10:31:53.416384 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql
--rw-r--r--   0        0        0     1877 2022-11-23 10:31:53.416723 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql
--rw-r--r--   0        0        0     1139 2022-11-23 10:31:53.417010 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql
--rw-r--r--   0        0        0     1179 2023-01-30 00:54:22.647572 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql
--rw-r--r--   0        0        0     3165 2023-03-10 00:12:11.857881 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql
--rw-r--r--   0        0        0     6259 2022-11-23 10:31:53.422782 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/oauth_service.py
--rwxr-xr-x   0        0        0    15044 2023-06-12 12:14:13.452381 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/session_service.py
--rw-r--r--   0        0        0      371 2022-11-23 10:31:53.423592 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/template/default_verify_email_eng-US.txt
--rw-r--r--   0        0        0      496 2022-11-23 10:31:53.423820 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/template/default_verify_email_fra-FR.txt
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424102 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/test/__init__.py
--rwxr-xr-x   0        0        0     7955 2022-11-23 10:31:53.424296 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/test/account_service_unittest.py
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424502 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/__init__.py
--rwxr-xr-x   0        0        0    36170 2023-02-09 01:22:42.266180 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/application_service.py
--rwxr-xr-x   0        0        0     1581 2022-11-23 10:31:53.426329 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/db/create_application_constraint.sql
--rwxr-xr-x   0        0        0     1226 2022-11-23 10:31:53.426580 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/db/create_application_index.sql
--rwxr-xr-x   0        0        0     5129 2022-11-23 10:31:53.426913 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/db/create_application_table.sql
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.428345 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/test/__init__.py
--rwxr-xr-x   0        0        0     5285 2023-01-30 01:58:24.717658 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/test/application_service_unittest.py
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.429024 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/__init__.py
--rw-r--r--   0        0        0    38030 2023-02-09 01:22:31.541021 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/area_service.py
--rwxr-xr-x   0        0        0     5918 2022-11-23 10:31:53.430300 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/data/vietnam/area2sql.py
--rw-r--r--   0        0        0     5064 2022-11-23 10:31:53.430550 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/data/vietnam/area_extractor.py
--rw-r--r--   0        0        0  5506086 2022-11-23 10:31:53.441911 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip
--rwxr-xr-x   0        0        0     1534 2022-11-23 10:31:53.442964 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_constraint.sql
--rw-r--r--   0        0        0     3013 2022-11-23 10:31:53.443144 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_dataset.sql
--rw-r--r--   0        0        0    27948 2022-11-23 10:31:53.443409 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_function.sql
--rw-r--r--   0        0        0     1324 2022-11-23 10:31:53.443571 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_index.sql
--rwxr-xr-x   0        0        0     5732 2022-11-23 10:31:53.443741 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_table.sql
--rwxr-xr-x   0        0        0     2447 2022-11-23 10:31:53.443964 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_type.sql
--rwxr-xr-x   0        0        0     1097 2022-11-23 10:31:53.444132 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_geoip_constraint.sql
--rw-r--r--   0        0        0      908 2022-11-23 10:31:53.444276 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_geoip_index.sql
--rw-r--r--   0        0        0     7276 2022-11-23 10:31:53.444639 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_geoip_table.sql
--rwxr-xr-x   0        0        0      923 2022-11-23 10:31:53.444789 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql
--rwxr-xr-x   0        0        0     1631 2022-11-23 10:31:53.444977 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql
--rw-r--r--   0        0        0     5679 2022-11-23 10:31:53.445111 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_rir_table.sql
--rw-r--r--   0        0        0     1597 2022-11-23 10:31:53.445206 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/migrate_area_dataset.sql
--rw-r--r--   0        0        0     1512 2022-11-23 10:31:53.445958 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/script/_geolite_importer.py
--rw-r--r--   0        0        0     6460 2022-11-23 10:31:53.446070 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/script/_rir_importer.py
--rwxr-xr-x   0        0        0    17479 2022-11-23 10:31:53.446283 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/script/geoip2sql.py
--rw-r--r--   0        0        0    64867 2023-07-10 03:10:00.295237 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_http_handler.py
--rw-r--r--   0        0        0     1331 2022-11-23 10:31:53.448135 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_job_service.py
--rwxr-xr-x   0        0        0     3067 2023-02-09 01:22:42.266212 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_rdbms_service.py
--rwxr-xr-x   0        0        0     4565 2023-02-09 01:21:55.697787 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_service.py
--rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.448685 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/__init__.py
--rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.448883 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/agent/__init__.py
--rwxr-xr-x   0        0        0    13128 2022-11-23 10:31:53.449162 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/agent/push_notification.py
--rw-r--r--   0        0        0      899 2022-11-23 10:31:53.449426 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/db/create_notification_constraint.sql
--rw-r--r--   0        0        0     1167 2022-11-23 10:31:53.449636 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/db/create_notification_index.sql
--rw-r--r--   0        0        0    10511 2022-11-23 10:31:53.449859 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/db/create_notification_table.sql
--rw-r--r--   0        0        0     2254 2022-11-23 10:31:53.450914 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/gcm.py
--rw-r--r--   0        0        0    65115 2023-02-09 01:22:31.540956 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/notification_service.py
--rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.451539 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/__init__.py
--rw-r--r--   0        0        0      802 2022-11-23 10:31:53.451813 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/doc/api/get_ping.rst
--rw-r--r--   0        0        0      927 2023-02-08 01:28:29.061642 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/doc/api/get_status.rst
--rw-r--r--   0        0        0      609 2023-02-08 01:24:00.319004 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/doc/api/index.rst
--rw-r--r--   0        0        0     7536 2022-11-23 10:31:53.452507 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/status_service.py
--rw-r--r--   0        0        0     2427 2022-11-23 10:31:53.452658 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/status_service_http_handler.py
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.453023 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/__init__.py
--rw-r--r--   0        0        0     2469 2022-11-23 10:31:53.453234 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/agent/team_invite.py
--rw-r--r--   0        0        0     2647 2022-11-23 10:31:53.453512 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_constraint.sql
--rw-r--r--   0        0        0     3769 2022-11-23 10:31:53.453654 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_function.sql
--rw-r--r--   0        0        0      968 2023-05-19 09:03:02.094015 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_index.sql
--rw-r--r--   0        0        0     9034 2023-05-19 09:32:28.819485 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_table.sql
--rw-r--r--   0        0        0      253 2022-11-23 10:31:53.454170 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/migrate_20190501.sql
--rw-r--r--   0        0        0     2513 2022-11-23 10:31:53.454566 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql
--rwxr-xr-x   0        0        0   124076 2023-05-25 02:34:43.732136 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/team_service.py
--rw-r--r--   0        0        0      623 2022-11-23 10:31:53.458700 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/template/default_invite_email.txt
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.458921 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/test/__init__.py
--rwxr-xr-x   0        0        0     6049 2022-11-23 10:31:53.459109 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/test/team_service_unittest.py
--rw-r--r--   0        0        0      830 2022-11-23 10:31:53.459329 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/__init__.py
--rw-r--r--   0        0        0     2734 2023-02-08 01:36:23.016572 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/doc/api/get_version.rst
--rw-r--r--   0        0        0     1913 2023-02-08 01:37:27.596508 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/doc/api/index.rst
--rwxr-xr-x   0        0        0      836 2022-11-23 10:31:53.461396 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/test/__init__.py
--rwxr-xr-x   0        0        0     4574 2022-11-23 10:31:53.461950 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/test/version_service_unittest.py
--rwxr-xr-x   0        0        0     2448 2023-01-17 06:08:31.898328 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/version_service.py
--rw-r--r--   0        0        0     1720 2023-01-17 03:47:01.966678 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/version_service_http_handler.py
--rw-r--r--   0        0        0     6855 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.27.0/setup.py
--rw-r--r--   0        0        0     5871 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.27.0/PKG-INFO
+-rw-r--r--   0        0        0    10202 2023-07-11 02:57:49.328434 perseus_restful_api_framework-1.27.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1089 2020-11-12 14:26:46.553799 perseus_restful_api_framework-1.27.1/LICENSE
+-rw-r--r--   0        0        0     4530 2022-10-02 05:19:36.696561 perseus_restful_api_framework-1.27.1/README.md
+-rw-r--r--   0        0        0     1140 2023-07-11 02:57:02.853879 perseus_restful_api_framework-1.27.1/pyproject.toml
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404748 perseus_restful_api_framework-1.27.1/src/majormode/__init__.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404886 perseus_restful_api_framework-1.27.1/src/majormode/perseus/__init__.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.405009 perseus_restful_api_framework-1.27.1/src/majormode/perseus/agent/__init__.py
+-rwxr-xr-x   0        0        0    11953 2023-02-09 01:22:31.663266 perseus_restful_api_framework-1.27.1/src/majormode/perseus/agent/email_address_verification_agent.py
+-rw-r--r--   0        0        0     3603 2023-02-09 01:21:55.716946 perseus_restful_api_framework-1.27.1/src/majormode/perseus/agent/email_sender_agent.py
+-rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.405462 perseus_restful_api_framework-1.27.1/src/majormode/perseus/bootstrap/__init__.py
+-rw-r--r--   0        0        0    17545 2023-02-09 01:22:31.663215 perseus_restful_api_framework-1.27.1/src/majormode/perseus/bootstrap/tornado_handler.py
+-rw-r--r--   0        0        0     4900 2022-11-23 10:31:53.406176 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_currency_dataset.sql
+-rwxr-xr-x   0        0        0     1892 2023-02-09 01:21:55.716943 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_exception_function.sql
+-rw-r--r--   0        0        0     1547 2022-11-23 10:31:53.406510 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_geometry_function.sql
+-rwxr-xr-x   0        0        0     1215 2022-11-23 10:31:53.406646 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_label_type.sql
+-rwxr-xr-x   0        0        0     2684 2022-11-23 10:31:53.406769 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_locale_function.sql
+-rwxr-xr-x   0        0        0     1269 2022-11-23 10:31:53.406909 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_object_constant.sql
+-rw-r--r--   0        0        0     6696 2022-11-23 10:31:53.407036 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_object_table.sql
+-rwxr-xr-x   0        0        0     1037 2022-11-23 10:31:53.407142 perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_visibility_constant.sql
+-rwxr-xr-x   0        0        0    13514 2023-02-09 01:22:42.266123 perseus_restful_api_framework-1.27.1/src/majormode/perseus/manage.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.407888 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/__init__.py
+-rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.408088 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/__init__.py
+-rwxr-xr-x   0        0        0   169815 2023-07-11 02:41:20.297680 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/account_service.py
+-rw-r--r--   0        0        0    53061 2023-02-08 13:43:19.667427 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/contact_service.py
+-rwxr-xr-x   0        0        0     4095 2023-07-11 00:53:28.787995 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_constraint.sql
+-rwxr-xr-x   0        0        0     7947 2023-01-30 00:41:55.092554 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_function.sql
+-rw-r--r--   0        0        0     1287 2022-11-23 10:31:53.411326 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_index.sql
+-rwxr-xr-x   0        0        0    21758 2023-07-11 00:53:51.665719 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_table.sql
+-rwxr-xr-x   0        0        0     1093 2022-11-23 10:31:53.412248 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_constraint.sql
+-rwxr-xr-x   0        0        0     1101 2022-11-23 10:31:53.412521 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_function.sql
+-rwxr-xr-x   0        0        0      989 2022-11-23 10:31:53.412719 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_index.sql
+-rwxr-xr-x   0        0        0     1637 2022-11-23 10:31:53.413015 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_table.sql
+-rwxr-xr-x   0        0        0     2093 2022-11-23 10:31:53.413203 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table.718.sql
+-rwxr-xr-x   0        0        0      870 2022-11-23 10:31:53.413470 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql
+-rwxr-xr-x   0        0        0     1033 2022-11-23 10:31:53.413751 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql
+-rw-r--r--   0        0        0     1115 2022-11-23 10:31:53.414028 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql
+-rw-r--r--   0        0        0     2599 2022-11-23 10:31:53.414316 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql
+-rw-r--r--   0        0        0     1182 2022-11-23 10:31:53.414599 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql
+-rw-r--r--   0        0        0      854 2022-11-23 10:31:53.416384 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql
+-rw-r--r--   0        0        0     1877 2022-11-23 10:31:53.416723 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql
+-rw-r--r--   0        0        0     1139 2022-11-23 10:31:53.417010 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql
+-rw-r--r--   0        0        0     1179 2023-01-30 00:54:22.647572 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql
+-rw-r--r--   0        0        0     3165 2023-03-10 00:12:11.857881 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql
+-rw-r--r--   0        0        0     6259 2022-11-23 10:31:53.422782 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/oauth_service.py
+-rwxr-xr-x   0        0        0    15044 2023-06-12 12:14:13.452381 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/session_service.py
+-rw-r--r--   0        0        0      371 2022-11-23 10:31:53.423592 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/template/default_verify_email_eng-US.txt
+-rw-r--r--   0        0        0      496 2022-11-23 10:31:53.423820 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/template/default_verify_email_fra-FR.txt
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424102 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/test/__init__.py
+-rwxr-xr-x   0        0        0     7955 2022-11-23 10:31:53.424296 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/test/account_service_unittest.py
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424502 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/__init__.py
+-rwxr-xr-x   0        0        0    36170 2023-02-09 01:22:42.266180 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/application_service.py
+-rwxr-xr-x   0        0        0     1581 2022-11-23 10:31:53.426329 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/db/create_application_constraint.sql
+-rwxr-xr-x   0        0        0     1226 2022-11-23 10:31:53.426580 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/db/create_application_index.sql
+-rwxr-xr-x   0        0        0     5129 2022-11-23 10:31:53.426913 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/db/create_application_table.sql
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.428345 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/test/__init__.py
+-rwxr-xr-x   0        0        0     5285 2023-01-30 01:58:24.717658 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/test/application_service_unittest.py
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.429024 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/__init__.py
+-rw-r--r--   0        0        0    38030 2023-02-09 01:22:31.541021 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/area_service.py
+-rwxr-xr-x   0        0        0     5918 2022-11-23 10:31:53.430300 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/data/vietnam/area2sql.py
+-rw-r--r--   0        0        0     5064 2022-11-23 10:31:53.430550 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/data/vietnam/area_extractor.py
+-rw-r--r--   0        0        0  5506086 2022-11-23 10:31:53.441911 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip
+-rwxr-xr-x   0        0        0     1534 2022-11-23 10:31:53.442964 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_constraint.sql
+-rw-r--r--   0        0        0     3013 2022-11-23 10:31:53.443144 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_dataset.sql
+-rw-r--r--   0        0        0    27948 2022-11-23 10:31:53.443409 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_function.sql
+-rw-r--r--   0        0        0     1324 2022-11-23 10:31:53.443571 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_index.sql
+-rwxr-xr-x   0        0        0     5732 2022-11-23 10:31:53.443741 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_table.sql
+-rwxr-xr-x   0        0        0     2447 2022-11-23 10:31:53.443964 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_type.sql
+-rwxr-xr-x   0        0        0     1097 2022-11-23 10:31:53.444132 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_geoip_constraint.sql
+-rw-r--r--   0        0        0      908 2022-11-23 10:31:53.444276 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_geoip_index.sql
+-rw-r--r--   0        0        0     7276 2022-11-23 10:31:53.444639 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_geoip_table.sql
+-rwxr-xr-x   0        0        0      923 2022-11-23 10:31:53.444789 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql
+-rwxr-xr-x   0        0        0     1631 2022-11-23 10:31:53.444977 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql
+-rw-r--r--   0        0        0     5679 2022-11-23 10:31:53.445111 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_rir_table.sql
+-rw-r--r--   0        0        0     1597 2022-11-23 10:31:53.445206 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/migrate_area_dataset.sql
+-rw-r--r--   0        0        0     1512 2022-11-23 10:31:53.445958 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/script/_geolite_importer.py
+-rw-r--r--   0        0        0     6460 2022-11-23 10:31:53.446070 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/script/_rir_importer.py
+-rwxr-xr-x   0        0        0    17479 2022-11-23 10:31:53.446283 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/script/geoip2sql.py
+-rw-r--r--   0        0        0    64867 2023-07-10 03:10:00.295237 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_http_handler.py
+-rw-r--r--   0        0        0     1331 2022-11-23 10:31:53.448135 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_job_service.py
+-rwxr-xr-x   0        0        0     3067 2023-02-09 01:22:42.266212 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_rdbms_service.py
+-rwxr-xr-x   0        0        0     4565 2023-02-09 01:21:55.697787 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_service.py
+-rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.448685 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/__init__.py
+-rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.448883 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/agent/__init__.py
+-rwxr-xr-x   0        0        0    13128 2022-11-23 10:31:53.449162 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/agent/push_notification.py
+-rw-r--r--   0        0        0      899 2022-11-23 10:31:53.449426 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/db/create_notification_constraint.sql
+-rw-r--r--   0        0        0     1167 2022-11-23 10:31:53.449636 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/db/create_notification_index.sql
+-rw-r--r--   0        0        0    10511 2022-11-23 10:31:53.449859 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/db/create_notification_table.sql
+-rw-r--r--   0        0        0     2254 2022-11-23 10:31:53.450914 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/gcm.py
+-rw-r--r--   0        0        0    65115 2023-02-09 01:22:31.540956 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/notification_service.py
+-rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.451539 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/__init__.py
+-rw-r--r--   0        0        0      802 2022-11-23 10:31:53.451813 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/doc/api/get_ping.rst
+-rw-r--r--   0        0        0      927 2023-02-08 01:28:29.061642 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/doc/api/get_status.rst
+-rw-r--r--   0        0        0      609 2023-02-08 01:24:00.319004 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/doc/api/index.rst
+-rw-r--r--   0        0        0     7536 2022-11-23 10:31:53.452507 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/status_service.py
+-rw-r--r--   0        0        0     2427 2022-11-23 10:31:53.452658 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/status_service_http_handler.py
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.453023 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/__init__.py
+-rw-r--r--   0        0        0     2469 2022-11-23 10:31:53.453234 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/agent/team_invite.py
+-rw-r--r--   0        0        0     2647 2022-11-23 10:31:53.453512 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_constraint.sql
+-rw-r--r--   0        0        0     3769 2022-11-23 10:31:53.453654 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_function.sql
+-rw-r--r--   0        0        0      968 2023-05-19 09:03:02.094015 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_index.sql
+-rw-r--r--   0        0        0     9034 2023-05-19 09:32:28.819485 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_table.sql
+-rw-r--r--   0        0        0      253 2022-11-23 10:31:53.454170 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/migrate_20190501.sql
+-rw-r--r--   0        0        0     2513 2022-11-23 10:31:53.454566 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql
+-rwxr-xr-x   0        0        0   124076 2023-05-25 02:34:43.732136 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/team_service.py
+-rw-r--r--   0        0        0      623 2022-11-23 10:31:53.458700 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/template/default_invite_email.txt
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.458921 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/test/__init__.py
+-rwxr-xr-x   0        0        0     6049 2022-11-23 10:31:53.459109 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/test/team_service_unittest.py
+-rw-r--r--   0        0        0      830 2022-11-23 10:31:53.459329 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/__init__.py
+-rw-r--r--   0        0        0     2734 2023-02-08 01:36:23.016572 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/doc/api/get_version.rst
+-rw-r--r--   0        0        0     1913 2023-02-08 01:37:27.596508 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/doc/api/index.rst
+-rwxr-xr-x   0        0        0      836 2022-11-23 10:31:53.461396 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/test/__init__.py
+-rwxr-xr-x   0        0        0     4574 2022-11-23 10:31:53.461950 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/test/version_service_unittest.py
+-rwxr-xr-x   0        0        0     2448 2023-01-17 06:08:31.898328 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/version_service.py
+-rw-r--r--   0        0        0     1720 2023-01-17 03:47:01.966678 perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/version_service_http_handler.py
+-rw-r--r--   0        0        0     6855 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.27.1/setup.py
+-rw-r--r--   0        0        0     5871 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.27.1/PKG-INFO
```

### Comparing `perseus_restful_api_framework-1.27.0/CHANGELOG.md` & `perseus_restful_api_framework-1.27.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), 
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.27.1] - 2023-07-11
+# Added
+- Add user account's preferences management
+
 ## [1.27.0] - 2023-07-10
 # Changed
 - HTTP request handlers return a dictionary object itself instead of embedding it in a `{ "data": dict }`
 
 ## [1.26.17] - 2023-06-10
 # Fixed
 - Return the generated password when creating a new account without specifying a password
```

### Comparing `perseus_restful_api_framework-1.27.0/LICENSE` & `perseus_restful_api_framework-1.27.1/LICENSE`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/README.md` & `perseus_restful_api_framework-1.27.1/README.md`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/pyproject.toml` & `perseus_restful_api_framework-1.27.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 keywords = ["perseus", "resful", "api", "server", "framework"]
 license = "Proprietary"
 name = "perseus-restful-api-framework"
 packages = [{ include = "majormode", from = "src" }]
 readme = "README.md"
 repository = "https://github.com/majormode/perseus-restful-api-server-framework"
-version = "1.27.0"
+version = "1.27.1"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 psutil = "^5.9.4"
 tornado = "^6.2"
 perseus-core-library = "^1.18.24"
 pillow = "^9.4.0"
```

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/agent/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/agent/email_address_verification_agent.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/agent/email_address_verification_agent.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/agent/email_sender_agent.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/agent/email_sender_agent.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/bootstrap/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/bootstrap/tornado_handler.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/bootstrap/tornado_handler.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_currency_dataset.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_currency_dataset.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_exception_function.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_exception_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_geometry_function.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_geometry_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_label_type.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_label_type.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_locale_function.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_locale_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_object_constant.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_object_constant.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_object_table.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_object_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_visibility_constant.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/db/create_visibility_constant.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/manage.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/manage.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/account_service.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/account_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,25 +136,30 @@
     PASSWORD_ALLOWED_SPECIAL_CHARACTERS_LIST = string.punctuation
 
     # The maximum time difference (in milliseconds) that the service
     # tolerates between the time on the client clock and the time on the
     # service server.
     MAXIMUM_TOLERANCE_FOR_COMPUTER_CLOCK_SYNCHRONIZATION = 4000
 
-    # Regular expression to whether a password complies with the following
-    # complexity requirements:
+    # Regular expression to check whether a password complies with the
+    # following complexity requirements:
     #
     # - Be at least eight characters
     # - Contain at least one numeric character (0-9)
     # - Contain at least one uppercase letter (A-Z)
     # - Contain at least one lowercase letter (a-z)
     # - Contain at least one special character (i.e., other than alphanumeric
     #   character)
     REGEX_PASSWORD_COMPLEXITY_REQUIREMENTS = re.compile(r'^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[^\da-zA-Z]).{8,}$')
 
+    # Regular expression to check whether the packaged name of a user's
+    # preference complies with the reverse domain name notation.
+    REGEX_PREFERENCE_PROPERTY_NAME = r'^[a-zA-Z_][a-zA-Z0-9_]*(\.[a-zA-Z_][a-zA-Z0-9_]*)*$'
+    REGEX_PATTERN_PREFERENCE_PROPERTY_NAME = re.compile(REGEX_PREFERENCE_PROPERTY_NAME)
+
     def __add_picture(
             self,
             app_id: uuid.UUID,
             account_id: uuid.UUID,
             submitter_account_id: uuid.UUID,
             capture_time: ISO8601DateTime,
             image: Image,
@@ -693,14 +698,29 @@
                     'account_id': account_id,
                     'password': self.__encrypt_password(password),
                 }
             )
 
             return cursor.get_row_count() == 1
 
+    @classmethod
+    def __is_preference_property_name_valid(cls, property_name: str) -> bool:
+        """
+        Indicate whether a property name, representing a user's preference,
+        complies with the naming convention.
+
+
+        :param property_name: The package named of a user's preference.
+
+
+        :return: ``True`` if the property name complies with the reverse domain
+            name notation; ``False`` otherwise.
+        """
+        return cls.REGEX_PATTERN_PREFERENCE_PROPERTY_NAME.match(property_name) is not None
+
     def __set_picture_status(
             self,
             picture_id,
             status,
             connection=None):
         """
         Set the current status of a picture.
@@ -2162,14 +2182,169 @@
             if not include_sys_info:
                 del picture.app_id
                 del picture.creation_time
                 del picture.submitter_account_id
 
             return picture
 
+    def get_preferences(
+            self,
+            app_id: uuid.UUID,
+            account_id: uuid.UUID,
+            connection: RdbmsConnection = None,
+            include_app_specific_preferences: bool = True,
+            include_global_preferences: bool = False,
+            include_subcategories: bool = False,
+            limit: int = None,
+            offset: int = None,
+            preference_category_name: str = None,
+            sync_time: ISO8601DateTime = None) -> dict[str, str]:
+        """
+        Return the user's preferences.
+
+
+        :warning: The current implementation of the function returns the
+            stringified values of the user's preferences.
+
+
+        :param app_id: The identifier of the client application that fetches
+            a list of the user's preferences.
+
+        :param account_id: The identifier of the account of a user to return a
+            list of preferences.
+
+        :param connection: A connection to the user account database.
+
+        :param include_app_specific_preferences: Indicate whether to return
+            the user's preferences for the specified client application.
+
+        :param include_global_preferences: Indicate whether to return the
+            user's global preferences.
+
+        :param include_subcategories: Indicate whether to return the user's
+            preferences for every subcategory.  When this argument is set to
+            ``True``, the argument ``preference_category_name`` MUST be passed
+            to this function.
+
+        :param limit: Constrain the number of preferences to return to the
+            specified number.  If not specified, the default value is
+            ``GuardianService.DEFAULT_LIMIT``.  The maximum value is
+            ``GuardianService.MAXIMUM_LIMIT``.
+
+        :param offset: Require to skip that many preferences before beginning
+            to return preferences.  Default value is ``0``.  If both ``offset``
+            and ``limit`` are specified, then ``offset`` preferences are
+            skipped before starting to count the limit preferences that are
+            returned.
+
+        :param preference_category_name: The package name of the category to
+            return the user's preferences.  For instance, if the category
+            ``com.example.whatever`` is specified, the function returns the
+            following preference examples:
+
+            - ``com.example.whatever.preference1``
+            - ``com.example.whatever.preference2``
+            - ``com.example.whatever.preference3``
+
+            To return the user's preferences for any subcategories
+            ``com.example.whatever.*``, refer to the argument
+            ``include_subcategories``.
+
+            When this argument is not specified, the function returns all the
+            user's preferences.
+
+        :param sync_time: The earliest non-inclusive time to filter the user's
+            preferences based on the time of the most recent modification of
+            their value.  If not specified, no time filter is applied; all the
+            preferences that match the criteria are returned.
+
+
+        :return: A dictionary of the guardian's preferences with the packaged
+            name of each preference as the key, and the value of each
+            preference.
+
+
+        :raise InvalidArgumentException: If some arguments are invalid.
+        """
+        if not include_app_specific_preferences and not include_global_preferences:
+            raise self.InvalidArgumentException(
+                "Application specific and/or global preferences MUST be requested"
+            )
+
+        if include_subcategories and not preference_category_name:
+            raise self.InvalidArgumentException(
+                "The argument 'preference_category_name' MUST be specified "
+                "when the argument 'include_subcategories' is 'true`"
+            )
+
+        if preference_category_name:
+            if not self.__is_preference_property_name_valid(preference_category_name):
+                raise self.InvalidArgumentException(
+                    f"The preference category name '{preference_category_name}' is invalid"
+                )
+
+            # Escape the period character `.`, that represents any single character
+            # in regular expression.
+            preference_category_name = preference_category_name.replace('.', '\.')
+
+            # Add the last package name separator.
+            preference_category_name += '\.'
+
+            # Match or not subcategories.
+            preference_category_name += r'.*' if include_subcategories else r'[^\.]*'
+
+            # Complete the regular expression with the caret character `^` that
+            # matches the beginning of a category, and the dollar character `$` that
+            # matches the end of a category.
+            preference_category_name = f'^{preference_category_name}$'
+
+        with self.acquire_rdbms_connection(auto_commit=False, connection=connection) as connection:
+            cursor = connection.execute(
+                '''
+                SELECT
+                    app_id,
+                    property_name,
+                    property_value
+                  FROM
+                    account_preference
+                  WHERE
+                    account_id = %(account_id)s
+                    AND (
+                        (%(include_app_specific_preferences)s AND app_id = %(app_id)s)
+                        OR (%(include_global_preferences)s AND app_id IS NULL)
+                    )
+                    AND (%(preference_category_name)s IS NULL OR property_name ~ %(preference_category_name)s)
+                    AND (%(sync_time)s IS NULL OR update_time > %(sync_time)s)
+                  ORDER BY
+                    property_name ASC
+                  OFFSET %(offset)s
+                  LIMIT %(limit)s
+                ''',
+                {
+                    'account_id': account_id,
+                    'app_id': app_id,
+                    'include_app_specific_preferences': include_app_specific_preferences,
+                    'include_global_preferences': include_global_preferences,
+                    'limit': min(limit or self.DEFAULT_LIMIT, self.MAXIMUM_LIMIT),
+                    'offset': offset or 0,
+                    'preference_category_name': preference_category_name,
+                    'sync_time': sync_time,
+                }
+            )
+
+            preferences = {
+                preference.property_name: preference.property_value
+                for preference in [
+                    row.get_object()
+                    for row in cursor.fetch_all()
+                ]
+            }
+
+            return preferences
+
     def get_sns_data_deletion(self, app_id, request_id):
         """
         Return information about a request sent to the platform to delete the
         data of auser that an application has collected from the given Social
         Networking Service about this user.
 
 
@@ -3066,14 +3241,104 @@
                 """,
                 {
                     'account_id': account_id,
                     'object_status': object_status,
                 }
             )
 
+    def set_preferences(
+            self,
+            account_id: uuid.UUID,
+            preferences: dict[str, str],
+            app_id: uuid.UUID = None,
+            connection: RdbmsConnection = None,
+            is_global: bool = False) -> dict[str, any]:
+        """
+        Set a list of the user's preferences.
+
+
+        :param account_id: The identifier of the user's account whose
+            preferences are set.
+
+        :param preferences: A dictionary of properties corresponding to the
+            preferences to set.
+
+        :param app_id: The identifier of the client application that submits
+            this request.
+
+        :param connection: A connection to the user account database.
+
+        :param is_global: Indicate whether these user's preferences are not
+            specific to the current application.  By default, the user's
+            preferences are specific to the current application.
+
+
+        @return: A dictionary of the user's preferences that were inserted or
+            updated.  The function doesn't return the user's preferences that
+            were not changed.
+        """
+        for property_name in preferences.keys():
+            if not self.__is_preference_property_name_valid(property_name):
+                raise self.InvalidArgumentException(
+                    f"The property name '{property_name} doesn't comply with the package naming convention"
+                )
+
+        with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
+            cursor = connection.execute(
+                '''
+                INSERT INTO account_preference (
+                    account_id,
+                    app_id,
+                    property_name,
+                    property_value
+                  )
+                  VALUES 
+                    %[values]s
+                  ON CONFLICT (account_id, property_name, app_id) DO
+                    UPDATE
+                      SET
+                        app_id = EXCLUDED.app_id,
+                        property_value = EXCLUDED.property_value,
+                        update_time = current_timestamp
+                      WHERE
+                        account_preference.account_id = EXCLUDED.account_id
+                        AND account_preference.property_name = EXCLUDED.property_name
+                        AND (
+                          (EXCLUDED.app_id IS NULL AND account_preference.app_id IS NULL)
+                          OR account_preference.app_id = EXCLUDED.app_id
+                        )
+                        AND account_preference.property_value <> EXCLUDED.property_value
+                  RETURNING
+                    property_name
+                ''',
+                {
+                    'values': [
+                        (
+                            account_id,
+                            None if is_global else app_id,
+                            property_name,
+                            property_value  # @warning: Unfortunately converted to a string!
+                        )
+                        for property_name, property_value in preferences.items()
+                    ]
+                }
+            )
+
+            updated_preferences = {
+                # @note: Keep the initial data type instead of the stringified version
+                #     stored into the database.
+                updated_preference.property_name: preferences[updated_preference.property_name]
+                for updated_preference in [
+                    row.get_object()
+                    for row in cursor.fetch_all()
+                ]
+            }
+
+            return updated_preferences
+
     def set_username(
             self,
             app_id,
             account_id,
             username,
             connection=None):
         """
```

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/contact_service.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/contact_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_constraint.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_constraint.sql`

 * *Files 11% similar despite different names*

```diff
@@ -102,7 +102,30 @@
 
 ALTER TABLE account_picture
   ADD CONSTRAINT fk_account_picture_team_id
       FOREIGN KEY (team_id)
       REFERENCES team (team_id)
       ON DELETE SET NULL
       ON UPDATE CASCADE;
+
+
+ALTER TABLE account_preference
+  ADD CONSTRAINT fk_account_preference_account_id
+      FOREIGN KEY (account_id)
+      REFERENCES account (account_id)
+      ON DELETE CASCADE
+      ON UPDATE CASCADE;
+
+ALTER TABLE account_preference
+  ADD CONSTRAINT fk_account_preference_app_id
+      FOREIGN KEY (app_id)
+      REFERENCES application (app_id)
+      ON DELETE CASCADE
+      ON UPDATE CASCADE;
+
+ALTER TABLE account_preference
+  ADD CONSTRAINT cst_account_preference_unique
+    UNIQUE (
+      account_id,
+      property_name,
+      app_id
+    );
```

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_function.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_index.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_table.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_account_table.sql`

 * *Files 8% similar despite different names*

```diff
@@ -516,7 +516,72 @@
 
   -- The time when this photo has been registered.
   creation_time timestamptz(3) NOT NULL DEFAULT current_timestamp,
 
   -- The time of the most recent modification of the status of this picture.
   update_time timestamptz(3) NOT NULL DEFAULT current_timestamp
 );
+
+
+/**
+ * The list of user's preferences.
+ *
+ * Preferences, also confusingly known as _settings_, allow users to
+ * change the functionality and behavior of an application.  Preferences
+ * can affect background behavior, such as how often the application
+ * synchronizes data with the cloud, or they can be more wide-reaching,
+ * such as changing the contents and presentation of the user interface.
+ *
+ * A preference is identified with a symbolic name that follows the
+ * package name style syntax, borrowed from the [reverse domain name
+ * notation](https://en.wikipedia.org/wiki/Reverse_domain_name_notation>).
+ *
+ * Preference symbolic names SHOULD be written in all lower case with
+ * underscores.  For instance as `com.example.my_preference`.
+ *
+ * Package name style syntax allows to group preferences by _sections_,
+ * also known as _categories_:
+ *
+ * - ``io.xebus.notification.outward_trip.is_checkin_notification_enabled``
+ * - ``io.xebus.notification.outward_trip.is_checkout_notification_enabled``
+ * - ``io.xebus.notification.outward_trip.is_school_bus_departure_notification_enabled``
+ * - ``io.xebus.notification.outward_trip.is_school_bus_arrival_notification_enabled``
+ * - ``io.xebus.notification.outward_trip.school_bus_eta_notification_lead_time``
+ *
+ *
+ * @note: If a _setting_ comes with a default value, then that _setting_
+ *     is not a _preference_ until the user changes it.
+ *
+ * @note: Preferences defined with default values SHOULD be removed from
+ *     the storage.  It's more unlikely that the default value of a
+ *     preference changes over the time, meaning that we SHOULD not need
+ *     to keep user preference that corresponds to the default value.
+ */
+CREATE TABLE account_preference (
+  /**
+   * The identifier of the account of the user who defined this
+   * preference.
+   */
+  account_id uuid NOT NULL,
+
+  /**
+   * The identifier of the client application for which this preference is
+   * specific.
+   */
+  app_id uuid NULL,
+
+  /**
+   * The code name of a user preference.
+   */
+  property_name text NOT NULL,
+
+  /**
+   * The string representation of the preference's value.
+   */
+  property_value text NOT NULL,
+
+  /**
+   * The time of the most recent modification of the value of this user's
+   * preference.
+   */
+  update_time timestamptz(3) NOT NULL DEFAULT current_timestamp
+);
```

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_constraint.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_function.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_index.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_table.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/create_session_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table.718.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table.718.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/oauth_service.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/oauth_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/session_service.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/session_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/test/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/test/account_service_unittest.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/account/test/account_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/application_service.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/application_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/db/create_application_constraint.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/db/create_application_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/db/create_application_index.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/db/create_application_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/db/create_application_table.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/db/create_application_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/test/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/test/application_service_unittest.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/application/test/application_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/area_service.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/area_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/data/vietnam/area2sql.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/data/vietnam/area2sql.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/data/vietnam/area_extractor.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/data/vietnam/area_extractor.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_constraint.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_dataset.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_dataset.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_function.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_index.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_table.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_type.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_area_type.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_geoip_constraint.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_geoip_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_geoip_index.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_geoip_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_geoip_table.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_geoip_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_rir_table.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/create_rir_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/migrate_area_dataset.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/db/migrate_area_dataset.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/script/_geolite_importer.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/script/_geolite_importer.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/script/_rir_importer.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/script/_rir_importer.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/script/geoip2sql.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/area/script/geoip2sql.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_http_handler.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_http_handler.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_job_service.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_job_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_rdbms_service.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_rdbms_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_service.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/base_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/agent/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/agent/push_notification.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/agent/push_notification.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/db/create_notification_constraint.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/db/create_notification_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/db/create_notification_index.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/db/create_notification_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/db/create_notification_table.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/db/create_notification_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/gcm.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/gcm.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/notification_service.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/notification/notification_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/doc/api/get_ping.rst` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/doc/api/get_ping.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/doc/api/get_status.rst` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/doc/api/get_status.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/doc/api/index.rst` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/doc/api/index.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/status_service.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/status_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/status_service_http_handler.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/status/status_service_http_handler.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/agent/team_invite.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/agent/team_invite.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_constraint.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_function.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_index.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_table.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/create_team_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/team_service.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/team_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/template/default_invite_email.txt` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/template/default_invite_email.txt`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/test/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/test/team_service_unittest.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/team/test/team_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/doc/api/get_version.rst` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/doc/api/get_version.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/doc/api/index.rst` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/doc/api/index.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/test/__init__.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/test/version_service_unittest.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/test/version_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/version_service.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/version_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/version_service_http_handler.py` & `perseus_restful_api_framework-1.27.1/src/majormode/perseus/service/version/version_service_http_handler.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.27.0/setup.py` & `perseus_restful_api_framework-1.27.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
  'prosoponym>=1.0.7,<2.0.0',
  'psutil>=5.9.4,<6.0.0',
  'pymemcache>=4.0.0,<5.0.0',
  'tornado>=6.2,<7.0']
 
 setup_kwargs = {
     'name': 'perseus-restful-api-framework',
-    'version': '1.27.0',
+    'version': '1.27.1',
     'description': 'Python server framework for quickly building RESTful APIs with minimal effort',
     'long_description': '# Perseus: RESTful API Server Framework\n\nPerseus is a Python framework for quickly building RESTful API servers with minimal effort.\n\nPerseus provides an initial set of core services that supports the following features:\n\n- Client application registration with API keys generation\n- Client application access control with RESTful request signature\n- Client application and RESTful API server version compatibility check\n- User authentication and session management\n- Team/group management\n- RESTful request logging with data sensitiveness support\n- RESTful service automatic discovery\n- HTTP request query parameters & body JSON message automatically parsing (depending on the HTTP method used) with data type check and conversion\n\nPerseus is based on [Tornado](https://www.tornadoweb.org/) for handling client network connection.\n\n## RESTful API Request Handler\n\n```python\nfrom majormode.perseus.service.base_http_handler import HttpRequest\nfrom majormode.perseus.service.base_http_handler import HttpRequestHandler\nfrom majormode.perseus.service.base_http_handler import http_request\n\nimport AttendantService\n\n\nclass AttendantServiceHttpRequestHandler(HttpRequestHandler):\n    @http_request(r\'^/attendant/session$\',\n                  http_method=HttpRequest.HttpMethod.POST,\n                  authentication_required=False,\n                  sensitive_data=True,\n                  signature_required=False)\n    def sign_in(self, request):\n        email_address = request.get_argument(\n            \'email_address\',\n            data_type=HttpRequest.ArgumentDataType.email_address,\n            is_required=True)\n\n        password = request.get_argument(\n            \'password\',\n            data_type=HttpRequest.ArgumentDataType.string,\n            is_required=True)\n\n        return AttendantService().sign_in(request.app_id, email_address, password)\n```\n\n## Configure the environment variables\n\n```env\n# Copyright (C) 2021 Majormode.  All rights reserved.\n#\n# Permission is hereby granted, free of charge, to any person obtaining\n# a copy of this software and associated documentation files (the\n# "Software"), to deal in the Software without restriction, including\n# without limitation the rights to use, copy, modify, merge, publish,\n# distribute, sublicense, and/or sell copies of the Software, and to\n# permit persons to whom the Software is furnished to do so, subject to\n# the following conditions:\n#\n# The above copyright notice and this permission notice shall be\n# included in all copies or substantial portions of the Software.\n#\n# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,\n# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n# MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n# IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\n# CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\n# TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\n# SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n\n# Connection properties of the RESTful API server instances.  Defaults\n# to 127.0.0.1:8081.\nAPI_SERVER_HOSTNAME=127.0.0.1\nAPI_SERVER_PORTS=\n\n# Root path of the Network File System (NFS) -- referring to the\n# distributed file system (not the protocol) -- where the Content\n# Delivery Network (CDN) files are stored into, such as avatars, etc.\nCDN_NFS_ROOT_PATH=\n\n# Hostname of the Content Delivery Network (CDN) server that hosts media\n# files such as avatars, etc.\nCDN_URL_HOSTNAME=\n\n# Environment stage of the API server instances.  Possible values are:\n#\n# - dev\n# - int\n# - staging\n# - prod\n#\n# Defaults to `dev`.\nENVIRONMENT_STAGE=\n\n# Connection properties to a Memcached server (a distributed memory\n# object caching system).  Defaults to 127.0.0.1:11211.\nMEMCACHED_HOSTNAME = \'127.0.0.1\'\nMEMCACHED_PORT = 11211\n\n# Threshold for the logger to level.  Logging messages which are less\n# severe than the specified level will be ignored; logging messages\n# which have this severity level or higher will be emitted.  Possible\n# values are:\n#\n# - debug\n# - info\n# - warning\n# - error\n# - critical\n#\n# Default to \'debug\'.\nLOGGING_LEVEL=\n\n# Environment variables to select default parameter values to connect\n# to PostgreSQL Relational Database Management System.\nPG_HOSTNAME=localhost\nPG_PORT=5432\nPG_DATABASE_NAME=\nPG_USERNAME=\nPG_PASSWORD=\n```\n\n## Run the RESTful API Server Processes\n\n```bash\n$ fab start --port=65180,65181,...\n```\n\nHashtags/Topics: `#perseus` `#restful` `#api` `#server` `#framework` `#python`\n',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel.caune@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/majormode/perseus-restful-api-server-framework',
```

### Comparing `perseus_restful_api_framework-1.27.0/PKG-INFO` & `perseus_restful_api_framework-1.27.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perseus-restful-api-framework
-Version: 1.27.0
+Version: 1.27.1
 Summary: Python server framework for quickly building RESTful APIs with minimal effort
 Home-page: https://github.com/majormode/perseus-restful-api-server-framework
 License: Proprietary
 Keywords: perseus,resful,api,server,framework
 Author: Daniel CAUNE
 Author-email: daniel.caune@gmail.com
 Requires-Python: >=3.9,<4.0
```

