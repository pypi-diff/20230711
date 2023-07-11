# Comparing `tmp/document_merge_service-6.1.2.tar.gz` & `tmp/document_merge_service-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_merge_service-6.1.2.tar", max compression
+gzip compressed data, was "document_merge_service-6.2.0.tar", max compression
```

## Comparing `document_merge_service-6.1.2.tar` & `document_merge_service-6.2.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    10949 2023-05-10 08:26:29.528524 document_merge_service-6.1.2/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-05-10 08:26:29.528524 document_merge_service-6.1.2/LICENSE
--rw-r--r--   0        0        0     2261 2023-05-10 08:26:29.532523 document_merge_service-6.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-10 08:26:29.532523 document_merge_service-6.1.2/document_merge_service/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 08:26:29.532523 document_merge_service-6.1.2/document_merge_service/api/__init__.py
--rw-r--r--   0        0        0      405 2023-05-10 08:26:29.532523 document_merge_service-6.1.2/document_merge_service/api/apps.py
--rw-r--r--   0        0        0     3159 2023-05-10 08:26:29.532523 document_merge_service-6.1.2/document_merge_service/api/authentication.py
--rw-r--r--   0        0        0      504 2023-05-10 08:26:29.532523 document_merge_service-6.1.2/document_merge_service/api/data/__init__.py
--rw-r--r--   0        0        0      559 2023-05-10 08:26:29.532523 document_merge_service-6.1.2/document_merge_service/api/data/black.png
--rw-r--r--   0        0        0     9125 2023-05-10 08:26:29.532523 document_merge_service-6.1.2/document_merge_service/api/data/docx-mailmerge-syntax.docx
--rw-r--r--   0        0        0    11489 2023-05-10 08:26:29.532523 document_merge_service-6.1.2/document_merge_service/api/data/docx-mailmerge.docx
--rw-r--r--   0        0        0     5735 2023-05-10 08:26:29.532523 document_merge_service-6.1.2/document_merge_service/api/data/docx-template-filters.docx
--rw-r--r--   0        0        0     6087 2023-05-10 08:26:29.532523 document_merge_service-6.1.2/document_merge_service/api/data/docx-template-loopcontrols.docx
--rw-r--r--   0        0        0     5952 2023-05-10 08:26:29.532523 document_merge_service-6.1.2/document_merge_service/api/data/docx-template-placeholdercheck.docx
--rw-r--r--   0        0        0     5091 2023-05-10 08:26:29.532523 document_merge_service-6.1.2/document_merge_service/api/data/docx-template-syntax.docx
--rw-r--r--   0        0        0     5490 2023-05-10 08:26:29.532523 document_merge_service-6.1.2/document_merge_service/api/data/docx-template.docx
--rw-r--r--   0        0        0  1127936 2023-05-10 08:26:29.536523 document_merge_service-6.1.2/document_merge_service/api/data/loadtest/1.doc
--rw-r--r--   0        0        0   175922 2023-05-10 08:26:29.536523 document_merge_service-6.1.2/document_merge_service/api/data/loadtest/2.docx
--rw-r--r--   0        0        0   163307 2023-05-10 08:26:29.536523 document_merge_service-6.1.2/document_merge_service/api/data/loadtest/3.docx
--rw-r--r--   0        0        0   141498 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/data/loadtest/4.docx
--rw-r--r--   0        0        0       22 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/data/test.txt
--rw-r--r--   0        0        0        5 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/data/xlsx-not-valid.xlsx
--rw-r--r--   0        0        0     6467 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/data/xlsx-structure.xlsx
--rw-r--r--   0        0        0     6432 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/data/xlsx-syntax.xlsx
--rw-r--r--   0        0        0     4750 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/data/xlsx-template.xlsx
--rw-r--r--   0        0        0     9774 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/engines.py
--rw-r--r--   0        0        0      389 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/factories.py
--rw-r--r--   0        0        0     2841 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/filters.py
--rw-r--r--   0        0        0     2546 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/jinja.py
--rw-r--r--   0        0        0        0 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/management/commands/__init__.py
--rw-r--r--   0        0        0     1582 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/management/commands/clean_dangling_files.py
--rw-r--r--   0        0        0     1249 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      489 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/migrations/0002_template_group.py
--rw-r--r--   0        0        0      375 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/migrations/0003_template_meta.py
--rw-r--r--   0        0        0      145 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/migrations/0004_cleanup_files.py
--rw-r--r--   0        0        0     1005 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/migrations/0005_xlsx_template_engine.py
--rw-r--r--   0        0        0      328 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/migrations/0006_remove_template_group.py
--rw-r--r--   0        0        0        0 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/migrations/__init__.py
--rw-r--r--   0        0        0     1876 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/models.py
--rw-r--r--   0        0        0      231 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/pagination.py
--rw-r--r--   0        0        0      289 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/permissions.py
--rw-r--r--   0        0        0     4651 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/serializers.py
--rw-r--r--   0        0        0        0 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/tests/snapshots/__init__.py
--rw-r--r--   0        0        0    29399 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/tests/snapshots/snap_test_template.py
--rw-r--r--   0        0        0     2270 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/tests/test_authentication.py
--rw-r--r--   0        0        0      942 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/tests/test_clean_dangling_files.py
--rw-r--r--   0        0        0     1963 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/tests/test_excel.py
--rw-r--r--   0        0        0     1372 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/tests/test_filters.py
--rw-r--r--   0        0        0     1300 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/tests/test_jinja.py
--rw-r--r--   0        0        0      749 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/tests/test_pagination.py
--rw-r--r--   0        0        0    25635 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/tests/test_template.py
--rw-r--r--   0        0        0     3425 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/tests/test_unoconv.py
--rw-r--r--   0        0        0     6947 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/unoconv.py
--rw-r--r--   0        0        0      356 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/urls.py
--rw-r--r--   0        0        0     3570 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/api/views.py
--rw-r--r--   0        0        0     2794 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/conftest.py
--rw-r--r--   0        0        0      789 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/sentry.py
--rw-r--r--   0        0        0     8039 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/settings.py
--rw-r--r--   0        0        0        0 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/tests/__init__.py
--rw-r--r--   0        0        0      434 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/tests/test_sentry.py
--rw-r--r--   0        0        0      615 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/tests/test_settings.py
--rw-r--r--   0        0        0      225 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/urls.py
--rw-r--r--   0        0        0      412 2023-05-10 08:26:29.540524 document_merge_service-6.1.2/document_merge_service/wsgi.py
--rw-r--r--   0        0        0     3564 2023-05-10 08:26:29.544524 document_merge_service-6.1.2/pyproject.toml
--rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 document_merge_service-6.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11148 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/LICENSE
+-rw-r--r--   0        0        0     2261 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/__init__.py
+-rw-r--r--   0        0        0      405 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/apps.py
+-rw-r--r--   0        0        0     3159 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/authentication.py
+-rw-r--r--   0        0        0      504 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/__init__.py
+-rw-r--r--   0        0        0      559 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/black.png
+-rw-r--r--   0        0        0     9125 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/docx-mailmerge-syntax.docx
+-rw-r--r--   0        0        0    11489 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/docx-mailmerge.docx
+-rw-r--r--   0        0        0     5735 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/docx-template-filters.docx
+-rw-r--r--   0        0        0     6087 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/docx-template-loopcontrols.docx
+-rw-r--r--   0        0        0     5952 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/docx-template-placeholdercheck.docx
+-rw-r--r--   0        0        0     5091 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/docx-template-syntax.docx
+-rw-r--r--   0        0        0     5490 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/docx-template.docx
+-rw-r--r--   0        0        0  1127936 2023-07-11 13:55:30.169032 document_merge_service-6.2.0/document_merge_service/api/data/loadtest/1.doc
+-rw-r--r--   0        0        0   175922 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/loadtest/2.docx
+-rw-r--r--   0        0        0   163307 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/loadtest/3.docx
+-rw-r--r--   0        0        0   141498 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/loadtest/4.docx
+-rw-r--r--   0        0        0       22 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/test.txt
+-rw-r--r--   0        0        0        5 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/xlsx-not-valid.xlsx
+-rw-r--r--   0        0        0     6467 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/xlsx-structure.xlsx
+-rw-r--r--   0        0        0     6432 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/xlsx-syntax.xlsx
+-rw-r--r--   0        0        0     4750 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/xlsx-template.xlsx
+-rw-r--r--   0        0        0     9774 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/engines.py
+-rw-r--r--   0        0        0      389 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/factories.py
+-rw-r--r--   0        0        0     2841 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/filters.py
+-rw-r--r--   0        0        0     2546 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/jinja.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/management/commands/__init__.py
+-rw-r--r--   0        0        0     1582 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/management/commands/clean_dangling_files.py
+-rw-r--r--   0        0        0     1249 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      489 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/migrations/0002_template_group.py
+-rw-r--r--   0        0        0      375 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/migrations/0003_template_meta.py
+-rw-r--r--   0        0        0      145 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/migrations/0004_cleanup_files.py
+-rw-r--r--   0        0        0     1005 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py
+-rw-r--r--   0        0        0      328 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/migrations/0006_remove_template_group.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/migrations/__init__.py
+-rw-r--r--   0        0        0     1876 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/models.py
+-rw-r--r--   0        0        0      231 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/pagination.py
+-rw-r--r--   0        0        0      289 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/permissions.py
+-rw-r--r--   0        0        0     4651 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/serializers.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0    29399 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/tests/snapshots/snap_test_template.py
+-rw-r--r--   0        0        0     2270 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/tests/test_authentication.py
+-rw-r--r--   0        0        0      942 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/tests/test_clean_dangling_files.py
+-rw-r--r--   0        0        0     1963 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/tests/test_excel.py
+-rw-r--r--   0        0        0     1372 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/tests/test_filters.py
+-rw-r--r--   0        0        0     1300 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/tests/test_jinja.py
+-rw-r--r--   0        0        0      749 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/tests/test_pagination.py
+-rw-r--r--   0        0        0    25635 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/tests/test_template.py
+-rw-r--r--   0        0        0     3425 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/tests/test_unoconv.py
+-rw-r--r--   0        0        0     6947 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/unoconv.py
+-rw-r--r--   0        0        0      356 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/urls.py
+-rw-r--r--   0        0        0     3570 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/views.py
+-rw-r--r--   0        0        0     2794 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/conftest.py
+-rw-r--r--   0        0        0      789 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/sentry.py
+-rw-r--r--   0        0        0     8581 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/settings.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/tests/__init__.py
+-rw-r--r--   0        0        0      434 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/tests/test_sentry.py
+-rw-r--r--   0        0        0      615 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/tests/test_settings.py
+-rw-r--r--   0        0        0      225 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/urls.py
+-rw-r--r--   0        0        0      412 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/wsgi.py
+-rw-r--r--   0        0        0     3592 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4247 1970-01-01 00:00:00.000000 document_merge_service-6.2.0/PKG-INFO
```

### Comparing `document_merge_service-6.1.2/CHANGELOG.md` & `document_merge_service-6.2.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 6.2.0 (11 July 2023)
+### Feature
+* Add django storages and settings for s3 storage ([`6df1a83`](https://github.com/Yelinz/document-merge-service/commit/6df1a83a4befbb8687a951d45fe6910deba83272))
+
 ## 6.1.2 (10 May 2023)
 Maintenance release only containing dependency updates.
 
 ## 6.1.1 (03 May 2023)
 ### Fix
 * **excel:** Set `sheet_name` and `tpl_name` to load the correct sheet
 ([`13a2a07`](https://github.com/adfinis/document-merge-service/commit/13a2a073aa1a7f65cbf7c794210f460db1a2509e))
```

### Comparing `document_merge_service-6.1.2/LICENSE` & `document_merge_service-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/README.md` & `document_merge_service-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/authentication.py` & `document_merge_service-6.2.0/document_merge_service/api/authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/data/black.png` & `document_merge_service-6.2.0/document_merge_service/api/data/black.png`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/data/docx-mailmerge-syntax.docx` & `document_merge_service-6.2.0/document_merge_service/api/data/docx-mailmerge-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/data/docx-mailmerge.docx` & `document_merge_service-6.2.0/document_merge_service/api/data/docx-mailmerge.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/data/docx-template-filters.docx` & `document_merge_service-6.2.0/document_merge_service/api/data/docx-template-filters.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/data/docx-template-loopcontrols.docx` & `document_merge_service-6.2.0/document_merge_service/api/data/docx-template-loopcontrols.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/data/docx-template-placeholdercheck.docx` & `document_merge_service-6.2.0/document_merge_service/api/data/docx-template-placeholdercheck.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/data/docx-template-syntax.docx` & `document_merge_service-6.2.0/document_merge_service/api/data/docx-template-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/data/docx-template.docx` & `document_merge_service-6.2.0/document_merge_service/api/data/docx-template.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/data/loadtest/1.doc` & `document_merge_service-6.2.0/document_merge_service/api/data/loadtest/1.doc`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/data/loadtest/2.docx` & `document_merge_service-6.2.0/document_merge_service/api/data/loadtest/2.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/data/loadtest/3.docx` & `document_merge_service-6.2.0/document_merge_service/api/data/loadtest/3.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/data/loadtest/4.docx` & `document_merge_service-6.2.0/document_merge_service/api/data/loadtest/4.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/data/xlsx-structure.xlsx` & `document_merge_service-6.2.0/document_merge_service/api/data/xlsx-structure.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/data/xlsx-syntax.xlsx` & `document_merge_service-6.2.0/document_merge_service/api/data/xlsx-syntax.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/data/xlsx-template.xlsx` & `document_merge_service-6.2.0/document_merge_service/api/data/xlsx-template.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/engines.py` & `document_merge_service-6.2.0/document_merge_service/api/engines.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/filters.py` & `document_merge_service-6.2.0/document_merge_service/api/filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/jinja.py` & `document_merge_service-6.2.0/document_merge_service/api/jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/management/commands/clean_dangling_files.py` & `document_merge_service-6.2.0/document_merge_service/api/management/commands/clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/migrations/0001_initial.py` & `document_merge_service-6.2.0/document_merge_service/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/migrations/0005_xlsx_template_engine.py` & `document_merge_service-6.2.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/models.py` & `document_merge_service-6.2.0/document_merge_service/api/models.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/serializers.py` & `document_merge_service-6.2.0/document_merge_service/api/serializers.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/tests/snapshots/snap_test_template.py` & `document_merge_service-6.2.0/document_merge_service/api/tests/snapshots/snap_test_template.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/tests/test_authentication.py` & `document_merge_service-6.2.0/document_merge_service/api/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/tests/test_clean_dangling_files.py` & `document_merge_service-6.2.0/document_merge_service/api/tests/test_clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/tests/test_excel.py` & `document_merge_service-6.2.0/document_merge_service/api/tests/test_excel.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/tests/test_filters.py` & `document_merge_service-6.2.0/document_merge_service/api/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/tests/test_jinja.py` & `document_merge_service-6.2.0/document_merge_service/api/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/tests/test_pagination.py` & `document_merge_service-6.2.0/document_merge_service/api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/tests/test_template.py` & `document_merge_service-6.2.0/document_merge_service/api/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/tests/test_unoconv.py` & `document_merge_service-6.2.0/document_merge_service/api/tests/test_unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/unoconv.py` & `document_merge_service-6.2.0/document_merge_service/api/unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/api/views.py` & `document_merge_service-6.2.0/document_merge_service/api/views.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/conftest.py` & `document_merge_service-6.2.0/document_merge_service/conftest.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/sentry.py` & `document_merge_service-6.2.0/document_merge_service/sentry.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/document_merge_service/settings.py` & `document_merge_service-6.2.0/document_merge_service/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -148,19 +148,29 @@
 
 # Media files
 
 DEFAULT_FILE_STORAGE = env.str(
     "FILE_STORAGE", default="django.core.files.storage.FileSystemStorage"
 )
 MEDIA_ROOT = env.str("MEDIA_ROOT", "")
-
 # TODO: This should be removed in favor of storing the files in a bucket
 # https://code.djangoproject.com/ticket/32991
-MEDIA_URL = "api/v1/template/"
+MEDIA_URL = env.str("MEDIA_URL", "api/v1/template/")
+
+# django-storages S3 settings
+AWS_S3_ACCESS_KEY_ID = env.str("AWS_S3_ACCESS_KEY_ID", "")
+AWS_S3_SECRET_ACCESS_KEY = env.str("AWS_S3_SECRET_ACCESS_KEY", "")
+AWS_STORAGE_BUCKET_NAME = env.str("AWS_STORAGE_BUCKET_NAME", "")
+AWS_S3_ENDPOINT_URL = env.str("AWS_S3_ENDPOINT_URL", "")
+AWS_S3_REGION_NAME = env.str("AWS_S3_REGION_NAME", "")
+AWS_LOCATION = env.str("AWS_LOCATION", "")
+AWS_S3_FILE_OVERWRITE = env.bool("AWS_S3_FILE_OVERWRITE", False)
+AWS_S3_SIGNATURE_VERSION = env.str("AWS_S3_SIGNATURE_VERSION", "v2")
 
+# unoconv
 UNOCONV_ALLOWED_TYPES = env.list("UNOCOV_ALLOWED_TYPES", default=["pdf"])
 UNOCONV_PYTHON = env.str("UNOCONV_PYTHON", default="/usr/bin/python3")
 UNOCONV_PATH = env.str("UNOCONV_PATH", default="/usr/bin/unoconv")
 
 
 # Jinja2
 DOCXTEMPLATE_JINJA_EXTENSIONS = env.list(
```

### Comparing `document_merge_service-6.1.2/document_merge_service/tests/test_settings.py` & `document_merge_service-6.2.0/document_merge_service/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.1.2/pyproject.toml` & `document_merge_service-6.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "document-merge-service"
-version = "6.1.2"
+version = "6.2.0"
 description = "Merge Document Template Service"
 license = "GPL-3.0-or-later"
 authors = ["Adfinis AG <info@adfinis.com>"]
 homepage = "https://github.com/adfinis/document-merge-service"
 repository = "https://github.com/adfinis/document-merge-service"
 documentation = "https://github.com/adfinis/document-merge-service/blob/main/README.md"
 readme = "README.md"
@@ -36,14 +36,15 @@
 python-memcached = "^1.59"
 requests = "^2.28.1"
 uWSGI = "^2.0.21"
 xltpl = "^0.16"
 openpyxl = "^3.0.10"
 django-generic-api-permissions = "^0.2.0"
 sentry-sdk = "^1.12.1"
+django-storages = "^1.13.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "22.10.0"
 django-stubs = "1.13.0"
 factory-boy = "3.2.1"
 flake8 = "5.0.4"
 flake8-debugger = "4.1.2"
```

### Comparing `document_merge_service-6.1.2/PKG-INFO` & `document_merge_service-6.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: document-merge-service
-Version: 6.1.2
+Version: 6.2.0
 Summary: Merge Document Template Service
 Home-page: https://github.com/adfinis/document-merge-service
 License: GPL-3.0-or-later
 Author: Adfinis AG
 Author-email: info@adfinis.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: databases
 Provides-Extra: mysql
 Provides-Extra: pgsql
 Requires-Dist: Babel (>=2.11.0,<3.0.0)
 Requires-Dist: Django (>=3.2.16,<4.0.0)
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: django-cors-headers (>=3.13.0,<4.0.0)
 Requires-Dist: django-environ (>=0.9.0,<0.10.0)
 Requires-Dist: django-filter (>=22.1,<23.0)
 Requires-Dist: django-generic-api-permissions (>=0.2.0,<0.3.0)
+Requires-Dist: django-storages (>=1.13.2,<2.0.0)
 Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
 Requires-Dist: docx-mailmerge (>=0.5.0,<0.6.0)
 Requires-Dist: docxtpl (>=0.16.4,<0.17.0)
 Requires-Dist: mysqlclient (>=2.1.1,<3.0.0) ; extra == "mysql" or extra == "databases"
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0) ; extra == "pgsql" or extra == "databases"
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
```

