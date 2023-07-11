# Comparing `tmp/invenio-drafts-resources-1.4.2.tar.gz` & `tmp/invenio-drafts-resources-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-drafts-resources-1.4.2.tar", last modified: Wed Jul  5 11:54:31 2023, max compression
+gzip compressed data, was "dist/invenio-drafts-resources-1.5.0.tar", last modified: Tue Jul 11 15:40:26 2023, max compression
```

## Comparing `invenio-drafts-resources-1.4.2.tar` & `invenio-drafts-resources-1.5.0.tar`

### file list

```diff
@@ -1,326 +1,327 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/systemfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/systemfields/parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/systemfields/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/search_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    22127 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-05 11:54:30.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1905 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/jsonschemas/records/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/jsonschemas/records/parent-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/jsonschemas/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/mock_module/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/records/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/records/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/resources/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/resources/test_files_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/resources/test_record_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/resources/test_resource_links.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:54:31.000000 invenio-drafts-resources-1.4.2/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/test_record_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/test_record_service_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/test_record_service_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/test_record_service_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-05 11:54:24.000000 invenio-drafts-resources-1.4.2/tests/services/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/systemfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/systemfields/parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/systemfields/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/media_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/search_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22122 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-11 15:40:25.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1905 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/jsonschemas/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/jsonschemas/records/parent-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/jsonschemas/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/mock_module/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/records/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/resources/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/resources/test_files_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/resources/test_record_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/resources/test_resource_links.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:40:26.000000 invenio-drafts-resources-1.5.0/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/test_record_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/test_record_service_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/test_record_service_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/test_record_service_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-11 15:40:18.000000 invenio-drafts-resources-1.5.0/tests/services/utils.py
```

### Comparing `invenio-drafts-resources-1.4.2/.editorconfig` & `invenio-drafts-resources-1.5.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/.github/workflows/pypi-publish.yml` & `invenio-drafts-resources-1.5.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/.github/workflows/tests.yml` & `invenio-drafts-resources-1.5.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/.tx/config` & `invenio-drafts-resources-1.5.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/CHANGES.rst` & `invenio-drafts-resources-1.5.0/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,18 @@
     Invenio-Drafts-Resources is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 1.5.0 (2023-07-11)
+
+- add media files components
+
 Version 1.4.2 (2023-07-05)
 
 - transifex: update config
 - components: add default files enabled variable
 
 Version 1.4.1 (2023-06-06)
```

### Comparing `invenio-drafts-resources-1.4.2/CONTRIBUTING.rst` & `invenio-drafts-resources-1.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/LICENSE` & `invenio-drafts-resources-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/MANIFEST.in` & `invenio-drafts-resources-1.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/PKG-INFO` & `invenio-drafts-resources-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-drafts-resources
-Version: 1.4.2
+Version: 1.5.0
 Summary: Invenio Drafts Resources module to create REST APIs
 Home-page: https://github.com/inveniosoftware/Invenio-Drafts-Resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -47,14 +47,18 @@
             Invenio-Drafts-Resources is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 1.5.0 (2023-07-11)
+        
+        - add media files components
+        
         Version 1.4.2 (2023-07-05)
         
         - transifex: update config
         - components: add default files enabled variable
         
         Version 1.4.1 (2023-06-06)
```

### Comparing `invenio-drafts-resources-1.4.2/README.rst` & `invenio-drafts-resources-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/babel.ini` & `invenio-drafts-resources-1.5.0/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/docs/Makefile` & `invenio-drafts-resources-1.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/docs/conf.py` & `invenio-drafts-resources-1.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/docs/index.rst` & `invenio-drafts-resources-1.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/docs/make.bat` & `invenio-drafts-resources-1.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/__init__.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/api.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/models.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/systemfields/parent.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/systemfields/parent.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/records/systemfields/versions.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/records/systemfields/versions.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/args.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/args.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/config.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/errors.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/resources/records/resource.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/resources/records/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/__init__.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Record service component for drafts."""
 
 from .base import ServiceComponent
 from .files import DraftFilesComponent
+from .media_files import DraftMediaFilesComponent
 from .metadata import DraftMetadataComponent
 from .pid import PIDComponent
 from .relations import RelationsComponent
 
 __all__ = (
     "ServiceComponent",
     "DraftFilesComponent",
     "DraftMetadataComponent",
     "PIDComponent",
     "RelationsComponent",
+    "DraftMediaFilesComponent",
 )
```

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/metadata.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/pid.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/pid.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/components/relations.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/components/relations.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/config.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/config.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/permissions.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/schema.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/search_params.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/search_params.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/service.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
             self.require_permission(identity, "edit", record=draft)
             return self.result_item(
                 self, identity, draft, links_tpl=self.links_item_tpl
             )
         except NoResultFound:
             pass
 
-        # Draft does not exists - so get the main record we want to edit and
+        # Draft does not exist - so get the main record we want to edit and
         # create a draft from it
         record = self.record_cls.pid.resolve(id_)
         self.require_permission(identity, "edit", record=record)
         draft = self.draft_cls.edit(record)
 
         # Run components
         self.run_components("edit", identity, draft=draft, record=record, uow=uow)
@@ -355,29 +355,29 @@
             expandable_fields=self.expandable_fields,
             expand=expand,
         )
 
     @unit_of_work()
     def new_version(self, identity, id_, uow=None, expand=False):
         """Create a new version of a record."""
-        # Get the a record - i.e. you can only create a new version in case
+        # Get the record - i.e. you can only create a new version in case
         # at least one published record already exists.
         record = self.record_cls.pid.resolve(id_)
 
         # Check permissions
         self.require_permission(identity, "new_version", record=record)
 
         # Draft for new version already exists? if so return it
         if record.versions.next_draft_id:
             next_draft = self.draft_cls.get_record(record.versions.next_draft_id)
             return self.result_item(
                 self, identity, next_draft, links_tpl=self.links_item_tpl
             )
 
-        # Draft for new version does not exists, so create it
+        # Draft for new version does not exist, so create it
         next_draft = self.draft_cls.new_version(record)
 
         # Get the latest published record if it's not the current one.
         if not record.versions.is_latest:
             record = self.record_cls.get_record(record.versions.latest_id)
 
         # Run components
@@ -559,15 +559,15 @@
 
         # Note, the record may not be the latest published record, and we only
         # want to index the latest published.
         if record is None or latest_id != record.id:
             record = self.record_cls.get_record(latest_id)
         uow.register(RecordIndexOp(record, indexer=self.indexer, index_refresh=refresh))
 
-        # Note, a draft may or may not exists for a published record (depending
+        # Note, a draft may or may not exist for a published record (depending
         # on if it's being edited).
         try:
             draft = self.draft_cls.get_record(latest_id)
             uow.register(
                 RecordIndexOp(draft, indexer=self.indexer, index_refresh=refresh)
             )
         except NoResultFound:
```

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/services/records/tasks.py` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/services/records/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/messages.pot` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/PKG-INFO` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-drafts-resources
-Version: 1.4.2
+Version: 1.5.0
 Summary: Invenio Drafts Resources module to create REST APIs
 Home-page: https://github.com/inveniosoftware/Invenio-Drafts-Resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -47,14 +47,18 @@
             Invenio-Drafts-Resources is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 1.5.0 (2023-07-11)
+        
+        - add media files components
+        
         Version 1.4.2 (2023-07-05)
         
         - transifex: update config
         - components: add default files enabled variable
         
         Version 1.4.1 (2023-06-06)
```

### Comparing `invenio-drafts-resources-1.4.2/invenio_drafts_resources.egg-info/SOURCES.txt` & `invenio-drafts-resources-1.5.0/invenio_drafts_resources.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 invenio_drafts_resources/services/records/schema.py
 invenio_drafts_resources/services/records/search_params.py
 invenio_drafts_resources/services/records/service.py
 invenio_drafts_resources/services/records/tasks.py
 invenio_drafts_resources/services/records/components/__init__.py
 invenio_drafts_resources/services/records/components/base.py
 invenio_drafts_resources/services/records/components/files.py
+invenio_drafts_resources/services/records/components/media_files.py
 invenio_drafts_resources/services/records/components/metadata.py
 invenio_drafts_resources/services/records/components/pid.py
 invenio_drafts_resources/services/records/components/relations.py
 invenio_drafts_resources/translations/messages.pot
 invenio_drafts_resources/translations/af/LC_MESSAGES/messages.mo
 invenio_drafts_resources/translations/af/LC_MESSAGES/messages.po
 invenio_drafts_resources/translations/ar/LC_MESSAGES/messages.mo
```

### Comparing `invenio-drafts-resources-1.4.2/run-tests.sh` & `invenio-drafts-resources-1.5.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/setup.cfg` & `invenio-drafts-resources-1.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/conftest.py` & `invenio-drafts-resources-1.5.0/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 fixtures are available.
 """
 
 import pytest
 from flask_principal import Identity, Need, UserNeed
 from invenio_app.factory import create_api as _create_api
 from invenio_records_resources.services.files import FileService
-from mock_module.service import DraftFileServiceConfig, FileServiceConfig
+from mock_module.service import (
+    DraftFileServiceConfig,
+    DraftMediaFileServiceConfig,
+    FileServiceConfig,
+    MediaFileServiceConfig,
+)
 
 pytest_plugins = ("celery.contrib.pytest",)
 
 
 @pytest.fixture(scope="module")
 def app_config(app_config):
     """Override pytest-invenio app_config fixture.
@@ -80,14 +85,26 @@
 
 @pytest.fixture(scope="module")
 def draft_file_service():
     """File service fixture."""
     return FileService(DraftFileServiceConfig)
 
 
+@pytest.fixture(scope="module")
+def media_file_service():
+    """File service fixture."""
+    return FileService(MediaFileServiceConfig)
+
+
+@pytest.fixture(scope="module")
+def media_draft_file_service():
+    """File service fixture."""
+    return FileService(DraftMediaFileServiceConfig)
+
+
 @pytest.fixture()
 def identity_simple():
     """Simple identity fixture."""
     i = Identity(1)
     i.provides.add(UserNeed(1))
     i.provides.add(Need(method="system_role", value="any_user"))
     return i
```

### Comparing `invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json` & `invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json` & `invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v1/draftsresources/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json` & `invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json` & `invenio-drafts-resources-1.5.0/tests/mock_module/mappings/os-v2/draftsresources/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json` & `invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json` & `invenio-drafts-resources-1.5.0/tests/mock_module/mappings/v7/draftsresources/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/mock_module/models.py` & `invenio-drafts-resources-1.5.0/tests/mock_module/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Example of a record model."""
 
 from invenio_db import db
+from invenio_files_rest.models import Bucket
 from invenio_records.models import RecordMetadataBase
 from invenio_records_resources.records import FileRecordModelMixin
+from sqlalchemy_utils.types import UUIDType
 
 from invenio_drafts_resources.records import (
     DraftMetadataBase,
     ParentRecordMixin,
     ParentRecordStateMixin,
 )
 
@@ -43,13 +45,29 @@
     """Model for mock module record files."""
 
     __record_model_cls__ = RecordMetadata
 
     __tablename__ = "mock_record_files"
 
 
+class MediaFileRecordMetadata(db.Model, RecordMetadataBase, FileRecordModelMixin):
+    """Model for mock module record files."""
+
+    __record_model_cls__ = RecordMetadata
+
+    __tablename__ = "mock_record_media_files"
+
+
 class FileDraftMetadata(db.Model, RecordMetadataBase, FileRecordModelMixin):
     """Model for mock module draft files."""
 
     __record_model_cls__ = DraftMetadata
 
     __tablename__ = "mock_draft_files"
+
+
+class MediaFileDraftMetadata(db.Model, RecordMetadataBase, FileRecordModelMixin):
+    """File associated with a draft."""
+
+    __record_model_cls__ = DraftMetadata
+
+    __tablename__ = "mock_drafts_media_files"
```

### Comparing `invenio-drafts-resources-1.4.2/tests/mock_module/permissions.py` & `invenio-drafts-resources-1.5.0/tests/mock_module/permissions.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,21 @@
     can_publish = [AnyUser()]
     can_create_files = [AnyUser()]
     can_set_content_files = [AnyUser()]
     can_get_content_files = [AnyUser()]
     can_commit_files = [AnyUser()]
     can_read_files = [AnyUser()]
     can_update_files = [AnyUser()]
+    can_draft_media_create_files = [AnyUser()]
+    can_draft_media_set_content_files = [AnyUser()]
+    can_draft_media_get_content_files = [AnyUser()]
+    can_draft_media_commit_files = [AnyUser()]
+    can_draft_media_update_files = [AnyUser()]
+    can_draft_media_delete_files = [AnyUser()]
+
     can_draft_create_files = [AnyUser()]
     can_draft_set_content_files = [AnyUser()]
     can_draft_get_content_files = [AnyUser()]
     can_draft_commit_files = [AnyUser()]
     can_draft_read_files = [AnyUser()]
     can_draft_update_files = [AnyUser()]
     can_manage_files = [AnyUser()]
```

### Comparing `invenio-drafts-resources-1.4.2/tests/mock_module/resource.py` & `invenio-drafts-resources-1.5.0/tests/mock_module/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/mock_module/schemas.py` & `invenio-drafts-resources-1.5.0/tests/mock_module/schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 class MetadataSchema(Schema):
     """Basic metadata schema class."""
 
     title = fields.Str(required=True, validate=validate.Length(min=3))
 
 
-class FilesOptionsSchema(Schema):
-    """Basic files options schema class."""
+class FilesSchema(Schema):
+    """Basic files schema class."""
 
     enabled = fields.Bool(missing=True)
     # allow unsetting
     default_preview = SanitizedUnicode(allow_none=True)
 
     def get_attribute(self, obj, attr, default):
         """Override how attributes are retrieved when dumping.
@@ -48,15 +48,16 @@
         return value
 
 
 class RecordSchema(BaseRecordSchema):
     """Schema for records in JSON."""
 
     metadata = fields.Nested(MetadataSchema)
-    files = fields.Nested(FilesOptionsSchema)
+    files = fields.Nested(FilesSchema)
+    media_files = fields.Nested(FilesSchema)
 
     def get_attribute(self, obj, attr, default):
         """Override how attributes are retrieved when dumping.
 
         NOTE: We have to access by attribute because although we are loading
               from an external pure dict, but we are dumping from a data-layer
               object whose fields should be accessed by attributes and not
```

### Comparing `invenio-drafts-resources-1.4.2/tests/records/conftest.py` & `invenio-drafts-resources-1.5.0/tests/records/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/records/test_api.py` & `invenio-drafts-resources-1.5.0/tests/records/test_api.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/resources/conftest.py` & `invenio-drafts-resources-1.5.0/tests/resources/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,18 @@
     """Application factory fixture."""
     base_app.register_blueprint(record_resource.as_blueprint())
     base_app.register_blueprint(file_resource.as_blueprint())
     base_app.register_blueprint(draft_file_resource.as_blueprint())
 
     registry = base_app.extensions["invenio-records-resources"].registry
     registry.register(service, service_id="mock-records-service")
+
     registry.register(file_service, service_id="mock-files-service")
     registry.register(draft_file_service, service_id="mock-draftfiles-service")
+
     yield base_app
 
 
 @pytest.fixture()
 def headers():
     """Default headers for making requests."""
     return {
```

### Comparing `invenio-drafts-resources-1.4.2/tests/resources/test_files_resource.py` & `invenio-drafts-resources-1.5.0/tests/resources/test_files_resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/resources/test_record_resource.py` & `invenio-drafts-resources-1.5.0/tests/resources/test_record_resource.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/resources/test_resource_links.py` & `invenio-drafts-resources-1.5.0/tests/resources/test_resource_links.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/services/conftest.py` & `invenio-drafts-resources-1.5.0/tests/services/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,26 +12,40 @@
 See https://pytest-invenio.readthedocs.io/ for documentation on which test
 fixtures are available.
 """
 
 import pytest
 from invenio_records_resources.services.files import FileService
 from mock_module.api import Draft
-from mock_module.service import FileServiceConfig, ServiceConfig
+from mock_module.service import (
+    FileServiceConfig,
+    MediaFilesRecordServiceConfig,
+    ServiceConfig,
+)
 
 from invenio_drafts_resources.services.records import RecordService
 
 
 @pytest.fixture(scope="module")
 def service():
     """Service instance."""
     return RecordService(ServiceConfig)
 
 
 @pytest.fixture(scope="module")
+def service_with_media_files(media_file_service, media_draft_file_service):
+    """Service instance."""
+    return RecordService(
+        MediaFilesRecordServiceConfig,
+        files_service=media_file_service,
+        draft_files_service=media_draft_file_service,
+    )
+
+
+@pytest.fixture(scope="module")
 def file_service():
     """File service fixture."""
     return FileService(FileServiceConfig)
 
 
 @pytest.fixture()
 def example_record(app, db):
```

### Comparing `invenio-drafts-resources-1.4.2/tests/services/test_record_service.py` & `invenio-drafts-resources-1.5.0/tests/services/test_record_service.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/services/test_record_service_files.py` & `invenio-drafts-resources-1.5.0/tests/services/test_record_service_files.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 - Read with missing pid
 """
 
 from io import BytesIO
 from unittest.mock import MagicMock, patch
 
 import pytest
-from invenio_files_rest.errors import InvalidOperationError
+from invenio_files_rest.errors import BucketLockedError, InvalidOperationError
 from invenio_files_rest.models import Bucket, FileInstance, ObjectVersion
 from invenio_records_resources.services.files.transfer import TransferType
 from marshmallow.exceptions import ValidationError
 from mock_module.models import DraftMetadata, FileDraftMetadata, FileRecordMetadata
 from mock_module.permissions import PermissionPolicy
 from mock_module.service import ServiceConfig
 
@@ -33,34 +33,49 @@
 #
 # Fixtures
 #
 @pytest.fixture()
 def input_data(input_data):
     """Enable files."""
     input_data["files"]["enabled"] = True
+    input_data["media_files"] = {"enabled": False}
     return input_data
 
 
 @pytest.fixture(scope="module")
 def service(file_service, draft_file_service):
     """Service instance."""
     return RecordService(
         ServiceConfig,
         files_service=file_service,
         draft_files_service=draft_file_service,
     )
 
 
 @pytest.fixture(scope="module")
-def base_app(base_app, service, file_service, draft_file_service):
+def base_app(
+    base_app,
+    service,
+    file_service,
+    draft_file_service,
+    service_with_media_files,
+    media_file_service,
+    media_draft_file_service,
+):
     """Application factory fixture."""
     registry = base_app.extensions["invenio-records-resources"].registry
     registry.register(service, service_id="mock-records-service")
+    registry.register(service, service_id="mock-records-media-files,service")
     registry.register(file_service, service_id="mock-files-service")
     registry.register(draft_file_service, service_id="mock-draftfiles-service")
+    registry.register(
+        service_with_media_files, service_id="mock-record-media-files-service"
+    )
+    registry.register(media_draft_file_service, service_id="mock-draft-media-files")
+    registry.register(media_file_service, service_id="mock-media-files-service")
     yield base_app
 
 
 #
 # Helpers
 #
 def add_file_to_draft(draft_file_service, draft_id, file_id, identity):
@@ -87,185 +102,323 @@
 #
 def test_create_delete_draft(app, db, service, input_data, identity_simple):
     """Test creation and deletion of a draft."""
     assert_counts(buckets=0, objs=0, fileinstances=0, filedrafts=0)
 
     # Create draft
     draft = service.create(identity_simple, input_data)
-    assert_counts(buckets=1, objs=0, fileinstances=0, filedrafts=0)
+    assert_counts(buckets=2, objs=0, fileinstances=0, filedrafts=0)
 
     # Add file
     add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
-    assert_counts(buckets=1, objs=1, fileinstances=1, filedrafts=1)
+    assert_counts(buckets=2, objs=1, fileinstances=1, filedrafts=1)
 
     # Delete draft
     service.delete_draft(identity_simple, draft.id)
     assert_counts(buckets=0, objs=0, fileinstances=1, filedrafts=0)
 
 
 def test_create_publish(app, db, service, input_data, identity_simple):
     """Test creation and publish of a draft."""
     # Create draft and file
     draft = service.create(identity_simple, input_data)
     add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
-    assert_counts(buckets=1, objs=1, fileinstances=1, filedrafts=1)
+    assert_counts(buckets=2, objs=1, fileinstances=1, filedrafts=1)
 
     # Publish
     record = service.publish(identity_simple, draft.id)
-    assert_counts(buckets=1, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
+    assert_counts(buckets=2, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
     assert record._record.bucket.locked is True
 
 
 def test_edit_delete(app, db, service, input_data, identity_simple, monkeypatch):
     """Test edit with delete of a published draft."""
     # Create and publish
     draft = service.create(identity_simple, input_data)
     add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
     record = service.publish(identity_simple, draft.id)
-    assert_counts(buckets=1, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
+    assert_counts(buckets=2, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
 
     # Edit draft (when soft-deleted draft record exists)
     draft = service.edit(identity_simple, record.id)
-    assert_counts(buckets=2, objs=2, fileinstances=1, filedrafts=1, filerecords=1)
+    assert_counts(buckets=4, objs=2, fileinstances=1, filedrafts=1, filerecords=1)
     assert record._record.bucket.locked is True
-    assert draft._record.bucket.locked is False
+    # we don't want to allow modifying files on the draft - go through new version
+    assert draft._record.bucket.locked is True
 
     # Delete draft
     draft = service.delete_draft(identity_simple, draft.id)
-    assert_counts(buckets=1, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
+    assert_counts(buckets=2, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
 
     # Cleanup deleted drafts.
     c = DraftMetadata.query.filter(DraftMetadata.is_deleted == True).delete()  # noqa
     assert c == 1
     db.session.commit()
 
     # Search engine will complain if we try we don't wait a minute, so disable
     # the indexer.
     monkeypatch.setattr(service.config, "indexer_cls", MagicMock())
 
     # Edit draft (when no soft-deleted draft record exists)
     draft = service.edit(identity_simple, record.id)
-    assert_counts(buckets=2, objs=2, fileinstances=1, filedrafts=1, filerecords=1)
+    assert_counts(buckets=4, objs=2, fileinstances=1, filedrafts=1, filerecords=1)
 
     # Delete draft
     draft = service.delete_draft(identity_simple, draft.id)
-    assert_counts(buckets=1, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
+    assert_counts(buckets=2, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
+
+
+def test_edit_delete_media_files(
+    app, db, service, service_with_media_files, input_data, identity_simple, monkeypatch
+):
+    """Test edit with delete of a published draft."""
+    input_data["media_files"] = {"enabled": True}
+    # Create and publish
+    draft = service.create(identity_simple, input_data)
+    add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
+    # add media file
+    add_file_to_draft(
+        service_with_media_files.draft_files, draft.id, "test2", identity_simple
+    )
+    record = service.publish(identity_simple, draft.id)
+    assert_counts(buckets=2, objs=2, fileinstances=2, filedrafts=0, filerecords=1)
+
+    # Edit draft (when soft-deleted draft record exists)
+    draft = service.edit(identity_simple, record.id)
+
+    assert_counts(buckets=4, objs=4, fileinstances=2, filedrafts=1, filerecords=1)
+    assert record._record.bucket.locked is True
+    # we don't want to allow modifying files on the draft - go through new version
+    assert draft._record.bucket.locked is True
+    # make sure we can modify media files
+    assert draft._record.media_bucket.locked is False
+
+    # Delete draft
+    draft = service.delete_draft(identity_simple, draft.id)
+    assert_counts(buckets=2, objs=2, fileinstances=2, filedrafts=0, filerecords=1)
+
+    # Cleanup deleted drafts.
+    c = DraftMetadata.query.filter(DraftMetadata.is_deleted == True).delete()  # noqa
+    assert c == 1
+    db.session.commit()
+
+    # Search engine will complain if we try we don't wait a minute, so disable
+    # the indexer.
+    monkeypatch.setattr(service.config, "indexer_cls", MagicMock())
+
+    # Edit draft (when no soft-deleted draft record exists)
+    draft = service.edit(identity_simple, record.id)
+    assert_counts(buckets=4, objs=4, fileinstances=2, filedrafts=1, filerecords=1)
+
+    # Delete draft
+    draft = service.delete_draft(identity_simple, draft.id)
+    assert_counts(buckets=2, objs=2, fileinstances=2, filedrafts=0, filerecords=1)
 
 
 def test_edit_publish(app, db, service, input_data, identity_simple, monkeypatch):
     """Test edit and publish."""
     # Create, publish and edit draft.
     draft = service.create(identity_simple, input_data)
     add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
     record = service.publish(identity_simple, draft.id)
     draft = service.edit(identity_simple, record.id)
-    assert_counts(buckets=2, objs=2, fileinstances=1, filedrafts=1, filerecords=1)
+    assert_counts(buckets=4, objs=2, fileinstances=1, filedrafts=1, filerecords=1)
 
     # Publish the edits
     record = service.publish(identity_simple, draft.id)
-    assert_counts(buckets=1, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
+    assert_counts(buckets=2, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
 
     # Cleanup deleted drafts.
     c = DraftMetadata.query.filter(DraftMetadata.is_deleted == True).delete()  # noqa
     assert c == 1
     db.session.commit()
 
     # engine will complain if we try we don't wait a minute, so disable
     # the indexer.
     monkeypatch.setattr(service.config, "indexer_cls", MagicMock())
 
     # Edit
     draft = service.edit(identity_simple, record.id)
-    assert_counts(buckets=2, objs=2, fileinstances=1, filedrafts=1, filerecords=1)
+    assert_counts(buckets=4, objs=2, fileinstances=1, filedrafts=1, filerecords=1)
 
     # Publish
     record = service.publish(identity_simple, draft.id)
-    assert_counts(buckets=1, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
+    assert_counts(buckets=2, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
+
+
+def test_edit_draft_files(
+    app, db, service, service_with_media_files, input_data, identity_simple, monkeypatch
+):
+    """Test edit and publish."""
+    input_data["media_files"] = {"enabled": True}
+    # Create, publish and edit draft.
+    draft = service.create(identity_simple, input_data)
+    add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
+    add_file_to_draft(
+        service_with_media_files.draft_files, draft.id, "test2", identity_simple
+    )
+    record = service.publish(identity_simple, draft.id)
+    draft = service.edit(identity_simple, record.id)
+
+    # expected to go via new version after initial publish
+    with pytest.raises(BucketLockedError):
+        add_file_to_draft(service.draft_files, draft.id, "test2", identity_simple)
+
+    # add media file - the media files bucket should not be locked
+    add_file_to_draft(
+        service_with_media_files.draft_files, draft.id, "test23", identity_simple
+    )
 
 
 def test_new_version(app, db, service, input_data, identity_simple, monkeypatch):
     """Test new version."""
     # Create and publish
     draft = service.create(identity_simple, input_data)
     add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
     service.publish(identity_simple, draft.id)
 
     # New version
     draft = service.new_version(identity_simple, draft.id)
-    assert_counts(buckets=2, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
+    assert_counts(buckets=4, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
 
     # Add file
     add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
-    assert_counts(buckets=2, objs=2, fileinstances=2, filedrafts=1, filerecords=1)
+    assert_counts(buckets=4, objs=2, fileinstances=2, filedrafts=1, filerecords=1)
 
     # Publish
     service.publish(identity_simple, draft.id)
-    assert_counts(buckets=2, objs=2, fileinstances=2, filedrafts=0, filerecords=2)
+    assert_counts(buckets=4, objs=2, fileinstances=2, filedrafts=0, filerecords=2)
+
+
+def test_new_version_with_media_files(
+    app, db, service, service_with_media_files, input_data, identity_simple, monkeypatch
+):
+    """Test new version."""
+    # Create and publish
+    input_data["media_files"] = {"enabled": True}
+    draft = service.create(identity_simple, input_data)
+    add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
+    add_file_to_draft(
+        service_with_media_files.draft_files, draft.id, "test2", identity_simple
+    )
+    service.publish(identity_simple, draft.id)
+
+    # New version
+    draft = service.new_version(identity_simple, draft.id)
+
+    # objects: 1 media file of the record + 1 file of the record
+    # + 1 media file of the draft (copied to new version) = 3
+    # file instances: 1 media file of the draft, 1 media file of the new version record
+    assert_counts(buckets=4, objs=3, fileinstances=2, filedrafts=0, filerecords=1)
+
+    # Add file
+    add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
+    # add media file
+    add_file_to_draft(
+        service_with_media_files.draft_files, draft.id, "test23", identity_simple
+    )
+
+    # objects: added 1 file and 1 media file = 5
+    assert_counts(buckets=4, objs=5, fileinstances=4, filedrafts=1, filerecords=1)
+
+    # Publish
+    service.publish(identity_simple, draft.id)
+    assert_counts(buckets=4, objs=5, fileinstances=4, filedrafts=0, filerecords=2)
 
 
 def test_new_version_delete(app, db, service, input_data, identity_simple):
     """Test new version."""
     # Create, publish, new_version, add_file
     draft = service.create(identity_simple, input_data)
     add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
     service.publish(identity_simple, draft.id)
     draft = service.new_version(identity_simple, draft.id)
     add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
-    assert_counts(buckets=2, objs=2, fileinstances=2, filedrafts=1, filerecords=1)
+    assert_counts(buckets=4, objs=2, fileinstances=2, filedrafts=1, filerecords=1)
 
     # Delete new version
     service.delete_draft(identity_simple, draft.id)
-    assert_counts(buckets=1, objs=1, fileinstances=2, filedrafts=0, filerecords=1)
+    assert_counts(buckets=2, objs=1, fileinstances=2, filedrafts=0, filerecords=1)
+
+
+def test_new_version_with_media_files_delete(
+    app, db, service, service_with_media_files, input_data, identity_simple
+):
+    """Test new version."""
+    # Create, publish, new_version, add_file
+    input_data["media_files"] = {"enabled": True}
+    draft = service.create(identity_simple, input_data)
+    add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
+    add_file_to_draft(
+        service_with_media_files.draft_files, draft.id, "test2", identity_simple
+    )
+    service.publish(identity_simple, draft.id)
+    draft = service.new_version(identity_simple, draft.id)
+    add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
+    add_file_to_draft(
+        service_with_media_files.draft_files, draft.id, "test23", identity_simple
+    )
+
+    # objects: 1 media file of the record + 1 file of the record
+    #           + 1 media file of the draft (copied to new version) = 3
+    #           + 1 media file in a new version + 1 regular file in a new version
+    assert_counts(buckets=4, objs=5, fileinstances=4, filedrafts=1, filerecords=1)
+
+    # Delete new version
+    service.delete_draft(identity_simple, draft.id)
+    assert_counts(buckets=2, objs=2, fileinstances=4, filedrafts=0, filerecords=1)
 
 
 #
 # Test import files
 #
 def test_import_files(app, db, service, input_data, identity_simple):
     """Test new version."""
     # Create, publish, new_version
     draft = service.create(identity_simple, input_data)
     add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
     service.publish(identity_simple, draft.id)
     draft = service.new_version(identity_simple, draft.id)
-    assert_counts(buckets=2, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
+    assert_counts(buckets=4, objs=1, fileinstances=1, filedrafts=0, filerecords=1)
 
     # Import files
     service.import_files(identity_simple, draft.id)
-    assert_counts(buckets=2, objs=2, fileinstances=1, filedrafts=1, filerecords=1)
+    assert_counts(buckets=4, objs=2, fileinstances=1, filedrafts=1, filerecords=1)
 
 
 def test_import_files_disabled(app, db, service, input_data, identity_simple):
     """Test new version."""
     # Create, publish, new_version
     input_data["files"]["enabled"] = False
     draft = service.create(identity_simple, input_data)
     service.publish(identity_simple, draft.id)
     draft = service.new_version(identity_simple, draft.id)
-    assert_counts(buckets=2, objs=0, fileinstances=0, filedrafts=0, filerecords=0)
+    assert_counts(buckets=4, objs=0, fileinstances=0, filedrafts=0, filerecords=0)
 
     with pytest.raises(ValidationError):
         service.import_files(identity_simple, draft.id)
 
 
 #
 # Default preview
 #
 def test_edit_publish_default_preview(app, service, input_data, identity_simple):
     """Test edit and publish."""
     # Create, publish and edit draft.
+    input_data["media_files"] = {"enabled": False}
     draft = service.create(identity_simple, input_data)
     add_file_to_draft(service.draft_files, draft.id, "test", identity_simple)
     record = service.publish(identity_simple, draft.id)
     draft = service.edit(identity_simple, record.id)
     assert "default_preview" not in draft.data["files"]
 
     # Set the default preview
     data = draft.to_dict()
     data["files"]["default_preview"] = "test"
+    data["media_files"] = {"enabled": False}
     draft = service.update_draft(identity_simple, draft.id, data)
     # TODO: fails because it needs schema to load the value.
     assert draft.data["files"]["default_preview"] == "test"
 
     # Publish change
     record = service.publish(identity_simple, draft.id)
     assert record.data["files"]["default_preview"] == "test"
```

### Comparing `invenio-drafts-resources-1.4.2/tests/services/test_record_service_search.py` & `invenio-drafts-resources-1.5.0/tests/services/test_record_service_search.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/services/test_record_service_tasks.py` & `invenio-drafts-resources-1.5.0/tests/services/test_record_service_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/services/test_services.py` & `invenio-drafts-resources-1.5.0/tests/services/test_services.py`

 * *Files identical despite different names*

### Comparing `invenio-drafts-resources-1.4.2/tests/services/utils.py` & `invenio-drafts-resources-1.5.0/tests/services/utils.py`

 * *Files identical despite different names*

