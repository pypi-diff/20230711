# Comparing `tmp/django-phac_aspc-helpers-0.5.1.tar.gz` & `tmp/django-phac_aspc-helpers-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-phac_aspc-helpers-0.5.1.tar", last modified: Fri Jun 16 16:52:35 2023, max compression
+gzip compressed data, was "django-phac_aspc-helpers-0.6.0.tar", last modified: Tue Jul 11 19:42:27 2023, max compression
```

## Comparing `django-phac_aspc-helpers-0.5.1.tar` & `django-phac_aspc-helpers-0.6.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.410827 django-phac_aspc-helpers-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-06-16 16:52:35.410827 django-phac_aspc-helpers-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15862 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.406827 django-phac_aspc-helpers-0.5.1/django_phac_aspc_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-06-16 16:52:35.000000 django-phac_aspc-helpers-0.5.1/django_phac_aspc_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-16 16:52:35.000000 django-phac_aspc-helpers-0.5.1/django_phac_aspc_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:52:35.000000 django-phac_aspc-helpers-0.5.1/django_phac_aspc_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-16 16:52:35.000000 django-phac_aspc-helpers-0.5.1/django_phac_aspc_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 16:52:35.000000 django-phac_aspc-helpers-0.5.1/django_phac_aspc_helpers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.406827 django-phac_aspc-helpers-0.5.1/phac_aspc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.406827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.406827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.406827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/admin/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/admin/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/admin/decorators/admin_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/admin/decorators/test_admin_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.406827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.406827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/auth/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.406827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.402827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/en_CA/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.406827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.402827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.406827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/language.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.410827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/ready/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/ready/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/ready/ready.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/ready/test_ready.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.402827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.410827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/static/phac_aspc_helpers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.402827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.410827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/buttons/ms-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18943 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.402827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.402827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.406827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.410827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.410827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/microsoft.html
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.410827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_page_description.html
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_retry.html
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_title.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_general.html
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_oauth.html
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/microsoft_logo.html
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/signin_with_microsoft.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.410827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/session_timeout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.410827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templatetags/phac_aspc_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templatetags/phac_aspc_localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/test_phac_aspc_localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/test_phac_aspc_wet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.410827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/urls/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/urls/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/urls/wet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.410827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/views/wet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.410827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/localization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/localization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.410827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/localization/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/localization/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/localization/decorators/localization_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/localization/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:35.410827 django-phac_aspc-helpers-0.5.1/phac_aspc/django/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/settings/localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/settings/security.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/settings/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/settings/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/phac_aspc/django/settings/wet.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-16 16:52:35.414827 django-phac_aspc-helpers-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 16:52:17.000000 django-phac_aspc-helpers-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.054618 django-phac_aspc-helpers-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17414 2023-07-11 19:42:27.054618 django-phac_aspc-helpers-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.046618 django-phac_aspc-helpers-0.6.0/django_phac_aspc_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17414 2023-07-11 19:42:27.000000 django-phac_aspc-helpers-0.6.0/django_phac_aspc_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-11 19:42:27.000000 django-phac_aspc-helpers-0.6.0/django_phac_aspc_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:42:27.000000 django-phac_aspc-helpers-0.6.0/django_phac_aspc_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 19:42:27.000000 django-phac_aspc-helpers-0.6.0/django_phac_aspc_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 19:42:27.000000 django-phac_aspc-helpers-0.6.0/django_phac_aspc_helpers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.046618 django-phac_aspc-helpers-0.6.0/phac_aspc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.050618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.050618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.050618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/admin/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/admin/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/admin/decorators/admin_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/admin/decorators/test_admin_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.050618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.050618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/auth/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.050618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.046618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/en_CA/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.050618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.046618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.050618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/language.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.050618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/ready/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/ready/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/ready/ready.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/ready/test_ready.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.046618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.050618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/static/phac_aspc_helpers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.046618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.050618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/buttons/ms-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18943 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.046618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.046618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.046618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.050618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.050618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/microsoft.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.054618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_page_description.html
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_retry.html
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_title.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_general.html
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_oauth.html
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/microsoft_logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/signin_with_microsoft.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.054618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/session_timeout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.054618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templatetags/phac_aspc_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templatetags/phac_aspc_localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/test_phac_aspc_localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/test_phac_aspc_wet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.054618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/urls/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/urls/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/urls/wet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.054618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/views/wet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.054618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/localization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/localization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.054618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/localization/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/localization/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/localization/decorators/localization_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/localization/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:42:27.054618 django-phac_aspc-helpers-0.6.0/phac_aspc/django/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/settings/localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/settings/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/settings/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/settings/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/phac_aspc/django/settings/wet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-11 19:42:27.054618 django-phac_aspc-helpers-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 19:42:10.000000 django-phac_aspc-helpers-0.6.0/setup.py
```

### Comparing `django-phac_aspc-helpers-0.5.1/LICENSE` & `django-phac_aspc-helpers-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/PKG-INFO` & `django-phac_aspc-helpers-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-phac_aspc-helpers
-Version: 0.5.1
+Version: 0.6.0
 Summary: Set of helpers for Django used at PHAC-ASPC
 Home-page: https://github.com/PHACDataHub/django-phac_aspc-helpers
 Author: Luc Belliveau
 Author-email: luc.belliveau@phac-aspc.gc.ca
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -233,14 +233,16 @@
 customize this behaviour, a custom authentication backend class can be specified
 via `PHAC_ASPC_OAUTH_USE_BACKEND` in `settings.py`.
 
 After successful authentication, the user is redirected to `/`.  To customize
 this behaviour, set `PHAC_ASPC_OAUTH_REDIRECT_ON_LOGIN` in `settings.py` to the
 name of the desired route.
 
+Redirecting to a specific page is also supported through the `?next=<url>` query parameter. See "Template Tag" examples below.
+
 ```python
 
 PHAC_ASPC_OAUTH_USE_BACKEND = "custom.authentication.backend"
 PHAC_ASPC_OAUTH_REDIRECT_ON_LOGIN = "home"
 
 # pylint: disable=wrong-import-position, unused-wildcard-import, wildcard-import
 from phac_aspc.django.settings import *
@@ -319,14 +321,23 @@
 A "Sign in with Microsoft" button is available as a template tag:
 
 ```django
 {% load phac_aspc_auth %}
 {% phac_aspc_auth_signin_microsoft_button %}
 ```
 
+To redirect to a specific page after logging in, pass the `next` query parameter through to the template tag as an argument.
+
+e.g. with Jinja, on a login page where the URL ends with `?next=/some-protected-page/`:
+
+```
+{{ phac_aspc.phac_aspc_auth_signin_microsoft_button(request.GET.urlencode()) }}
+```
+
+
 #### Handling Errors
 
 If there are any errors during the authentication flow, they are displayed to
 the user via the [error.html](phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html)
 template.  The template can be extended using standard django templating by
 creating a `templates/phac_aspc/helpers/auth/error.html` file in the host
 project.
```

### Comparing `django-phac_aspc-helpers-0.5.1/README.md` & `django-phac_aspc-helpers-0.6.0/django_phac_aspc_helpers.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: django-phac-aspc-helpers
+Version: 0.6.0
+Summary: Set of helpers for Django used at PHAC-ASPC
+Home-page: https://github.com/PHACDataHub/django-phac_aspc-helpers
+Author: Luc Belliveau
+Author-email: luc.belliveau@phac-aspc.gc.ca
+License: MIT
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.1
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development :: Localization
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Django Helpers
 
 Provides a series of helpers to provide a consistent experience across
 PHAC-ASPC's Django based projects.
 
 ## Third party applications
 
@@ -205,14 +233,16 @@
 customize this behaviour, a custom authentication backend class can be specified
 via `PHAC_ASPC_OAUTH_USE_BACKEND` in `settings.py`.
 
 After successful authentication, the user is redirected to `/`.  To customize
 this behaviour, set `PHAC_ASPC_OAUTH_REDIRECT_ON_LOGIN` in `settings.py` to the
 name of the desired route.
 
+Redirecting to a specific page is also supported through the `?next=<url>` query parameter. See "Template Tag" examples below.
+
 ```python
 
 PHAC_ASPC_OAUTH_USE_BACKEND = "custom.authentication.backend"
 PHAC_ASPC_OAUTH_REDIRECT_ON_LOGIN = "home"
 
 # pylint: disable=wrong-import-position, unused-wildcard-import, wildcard-import
 from phac_aspc.django.settings import *
@@ -291,14 +321,23 @@
 A "Sign in with Microsoft" button is available as a template tag:
 
 ```django
 {% load phac_aspc_auth %}
 {% phac_aspc_auth_signin_microsoft_button %}
 ```
 
+To redirect to a specific page after logging in, pass the `next` query parameter through to the template tag as an argument.
+
+e.g. with Jinja, on a login page where the URL ends with `?next=/some-protected-page/`:
+
+```
+{{ phac_aspc.phac_aspc_auth_signin_microsoft_button(request.GET.urlencode()) }}
+```
+
+
 #### Handling Errors
 
 If there are any errors during the authentication flow, they are displayed to
 the user via the [error.html](phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html)
 template.  The template can be extended using standard django templating by
 creating a `templates/phac_aspc/helpers/auth/error.html` file in the host
 project.
```

### Comparing `django-phac_aspc-helpers-0.5.1/django_phac_aspc_helpers.egg-info/PKG-INFO` & `django-phac_aspc-helpers-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: django-phac-aspc-helpers
-Version: 0.5.1
-Summary: Set of helpers for Django used at PHAC-ASPC
-Home-page: https://github.com/PHACDataHub/django-phac_aspc-helpers
-Author: Luc Belliveau
-Author-email: luc.belliveau@phac-aspc.gc.ca
-License: MIT
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.1
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development :: Localization
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Django Helpers
 
 Provides a series of helpers to provide a consistent experience across
 PHAC-ASPC's Django based projects.
 
 ## Third party applications
 
@@ -233,14 +205,16 @@
 customize this behaviour, a custom authentication backend class can be specified
 via `PHAC_ASPC_OAUTH_USE_BACKEND` in `settings.py`.
 
 After successful authentication, the user is redirected to `/`.  To customize
 this behaviour, set `PHAC_ASPC_OAUTH_REDIRECT_ON_LOGIN` in `settings.py` to the
 name of the desired route.
 
+Redirecting to a specific page is also supported through the `?next=<url>` query parameter. See "Template Tag" examples below.
+
 ```python
 
 PHAC_ASPC_OAUTH_USE_BACKEND = "custom.authentication.backend"
 PHAC_ASPC_OAUTH_REDIRECT_ON_LOGIN = "home"
 
 # pylint: disable=wrong-import-position, unused-wildcard-import, wildcard-import
 from phac_aspc.django.settings import *
@@ -319,14 +293,23 @@
 A "Sign in with Microsoft" button is available as a template tag:
 
 ```django
 {% load phac_aspc_auth %}
 {% phac_aspc_auth_signin_microsoft_button %}
 ```
 
+To redirect to a specific page after logging in, pass the `next` query parameter through to the template tag as an argument.
+
+e.g. with Jinja, on a login page where the URL ends with `?next=/some-protected-page/`:
+
+```
+{{ phac_aspc.phac_aspc_auth_signin_microsoft_button(request.GET.urlencode()) }}
+```
+
+
 #### Handling Errors
 
 If there are any errors during the authentication flow, they are displayed to
 the user via the [error.html](phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html)
 template.  The template can be extended using standard django templating by
 creating a `templates/phac_aspc/helpers/auth/error.html` file in the host
 project.
```

### Comparing `django-phac_aspc-helpers-0.5.1/django_phac_aspc_helpers.egg-info/SOURCES.txt` & `django-phac_aspc-helpers-0.6.0/django_phac_aspc_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/admin/decorators/admin_decorators.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/admin/decorators/admin_decorators.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/admin/decorators/test_admin_decorators.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/admin/decorators/test_admin_decorators.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/apps.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/apps.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/auth/backend.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/auth/backend.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/auth/views.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/auth/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """OAuth authentication related views"""
-from django.http import HttpResponseRedirect
-from django.shortcuts import render
+from urllib import parse
+
+from django.conf import settings
 from django.contrib.auth import authenticate
-from django.urls import reverse
 from django.contrib.auth import login as auth_login
-from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
+from django.http import HttpResponseRedirect
+from django.shortcuts import render
+from django.urls import reverse
 
 from authlib.integrations.django_client import OAuth, OAuthError
 
 oauth = OAuth()
 
 PROVIDER = getattr(settings, "PHAC_ASPC_HELPER_OAUTH_PROVIDER", False)
 BACKEND = getattr(settings, "PHAC_ASPC_OAUTH_USE_BACKEND", False)
@@ -27,37 +29,47 @@
     return use_tenant in value
 
 
 def login(request):
     """Redirect users to the provider's login page"""
     if PROVIDER:
         client = oauth.create_client(PROVIDER)
+        auth_url_extra_params = {"state": request.build_absolute_uri()}
         return client.authorize_redirect(
-            request, request.build_absolute_uri(reverse("phac_aspc_authorize"))
+            request,
+            request.build_absolute_uri(reverse("phac_aspc_authorize")),
+            **auth_url_extra_params
         )
     raise ImproperlyConfigured("The login route is not configured.")
 
 
 def authorize(request):
     """Verify the token received and perform authentication"""
     if PROVIDER:
         try:
             client = oauth.create_client(PROVIDER)
             token = client.authorize_access_token(
                 request,
                 claims_options={"iss": {"essential": True, "validate": validate_iss}},
             )
             user_info = token["userinfo"]
+            query_params = dict(
+                parse.parse_qsl(parse.urlsplit(request.GET["state"]).query)
+            )
             user = authenticate(request, user_info=user_info)
             if user is not None:
                 auth_login(
                     request,
                     user=user,
                     backend=BACKEND,
                 )
+
+                if "next" in query_params:
+                    return HttpResponseRedirect(query_params["next"])
+
                 return HttpResponseRedirect(
                     reverse(REDIRECT_LOGIN) if REDIRECT_LOGIN else "/"
                 )
             return render(
                 request,
                 "phac_aspc/helpers/auth/error.html",
                 {
```

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.po` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.mo` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.po` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/locale/language.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/locale/language.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/ready/__init__.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/ready/__init__.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/ready/test_ready.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/ready/test_ready.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/microsoft.html` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/microsoft.html`

 * *Files 5% similar despite different names*

```diff
@@ -9,21 +9,21 @@
         color: #5e5e5e;
         background-color: #fff;
         height: 41px;
         align-items: center;
         display: inline-flex;
         padding: 0 12px 0 0;
         text-decoration: none;
-        }
-        
-        .btn-ms-login img {
+    }
+    
+    .btn-ms-login img {
         margin: 0 12px 0 12px;
-        }
+    }
 </style>
-<a href="{% url 'phac_aspc_helper_login' %}"
+<a href="{% url 'phac_aspc_helper_login' %}{% if query_params %}?{{query_params}}{% endif %}"
    class="btn-ms-login align-self-end">
     <img width="21"
          height="21"
          src="{% static 'phac_aspc_helpers/auth/buttons/ms-logo.svg' %}"
          alt="{% use_string "microsoft_logo" %}" />
     {% use_string "signin_with_microsoft" %}
 </a>
```

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templatetags/__init__.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templatetags/phac_aspc_localization.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templatetags/phac_aspc_localization.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/test_phac_aspc_wet.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/test_phac_aspc_wet.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/helpers/views/wet.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/helpers/views/wet.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/localization/decorators/localization_decorators.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/localization/decorators/localization_decorators.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/settings/security.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/settings/security.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/settings/test_utils.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/settings/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/phac_aspc/django/settings/utils.py` & `django-phac_aspc-helpers-0.6.0/phac_aspc/django/settings/utils.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.5.1/setup.cfg` & `django-phac_aspc-helpers-0.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-phac_aspc-helpers
-version = 0.5.1
+version = 0.6.0
 description = Set of helpers for Django used at PHAC-ASPC
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/PHACDataHub/django-phac_aspc-helpers
 author = Luc Belliveau
 author_email = luc.belliveau@phac-aspc.gc.ca
 license = MIT
```

