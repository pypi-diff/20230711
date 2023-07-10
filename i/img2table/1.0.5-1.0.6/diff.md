# Comparing `tmp/img2table-1.0.5.tar.gz` & `tmp/img2table-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/img2table-1.0.5.tar", last modified: Wed Jun 21 22:15:37 2023, max compression
+gzip compressed data, was "dist/img2table-1.0.6.tar", last modified: Mon Jul 10 22:54:14 2023, max compression
```

## Comparing `img2table-1.0.5.tar` & `img2table-1.0.6.tar`

### file list

```diff
@@ -1,305 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-21 22:13:27.000000 img2table-1.0.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-21 22:13:27.000000 img2table-1.0.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-21 22:13:27.000000 img2table-1.0.5/.github/workflows/test_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-21 22:13:27.000000 img2table-1.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-21 22:13:27.000000 img2table-1.0.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-06-21 22:15:37.000000 img2table-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-06-21 22:13:27.000000 img2table-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-21 22:13:27.000000 img2table-1.0.5/activate_venv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/Basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/Implicit_rows.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   727975 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/borderless.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/examples/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/examples/data/borderless/
--rw-r--r--   0 runner    (1001) docker     (123)    47122 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/borderless/1.png
--rw-r--r--   0 runner    (1001) docker     (123)   177004 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/borderless/2.png
--rw-r--r--   0 runner    (1001) docker     (123)   182800 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/borderless/3.png
--rw-r--r--   0 runner    (1001) docker     (123)   132335 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/borderless/4.png
--rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/borderless.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/tables.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/tables.png
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/data/tables.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-21 22:13:27.000000 img2table-1.0.5/examples/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 22:13:27.000000 img2table-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-21 22:13:27.000000 img2table-1.0.5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-21 22:13:27.000000 img2table-1.0.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-21 22:13:27.000000 img2table-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-21 22:15:37.000000 img2table-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 22:13:27.000000 img2table-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/document/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/document/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/document/base/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/document/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/document/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/aws_textract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/easyocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/google_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/paddle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/ocr/tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/objects/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/objects/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/objects/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/objects/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/objects/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/cells/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/column_delimiters/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/rows/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/rows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/rows/coherency.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/table/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/borderless_tables/table/table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-21 22:13:27.000000 img2table-1.0.5/src/img2table/tables/processing/text/titles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 22:15:36.000000 img2table-1.0.5/src/img2table.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/_mock_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/_mock_data/azure.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/_mock_data/tesseract_hocr.html
--rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/_mock_data/textract.json
--rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/_mock_data/vision.json
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/_mock_data/vision.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/document/base/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/base/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/base/test_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/document/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/document/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/image/test_data/dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/image/test_data/expected.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/image/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/document/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/document/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/document/pdf/test_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/aws_textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/aws_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/aws_textract/test_aws_textract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/aws_textract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/aws_textract/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/aws_textract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/aws_textract/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/azure/test_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/azure/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/azure/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/azure/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/data/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/data/test_data/expected_table.json
--rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/data/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/data/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/data/test_ocr_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/easyocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/easyocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/easyocr/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/easyocr/test_data/ocr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/easyocr/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/easyocr/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/easyocr/test_easyocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/google_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/google_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/google_vision/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/google_vision/test_data/expected_content.json
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/google_vision/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/google_vision/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/google_vision/test_google_vision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/paddle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/paddle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/paddle/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/paddle/test_data/hocr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/paddle/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/paddle/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/paddle/test_paddle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/pdf/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/pdf/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/pdf/test_pdf_ocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/tesseract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/tesseract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/ocr/tesseract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/tesseract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/tesseract/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/ocr/tesseract/test_tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/image/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/image/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/image/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/objects/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/test_data/expected_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/test_data/tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/test_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/test_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/objects/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:36.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_data/contours.json
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/cells.json
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/borderless_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/borderless_tables/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/borderless_tables/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    50091 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_coherency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_data/rows.json
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_rows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/segment_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/segment_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/segment_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    50091 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_data/rows.json
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/common/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/common/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/common/test_data/test.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/prepare_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/prepare_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/prepare_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/prepare_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/prepare_image/test_prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:15:37.000000 img2table-1.0.5/tests/tables/processing/text/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/text/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/text/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/text/test_data/test.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-21 22:13:27.000000 img2table-1.0.5/tests/tables/processing/text/test_titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 22:52:02.000000 img2table-1.0.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-10 22:52:02.000000 img2table-1.0.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-10 22:52:02.000000 img2table-1.0.6/.github/workflows/test_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-10 22:52:02.000000 img2table-1.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-10 22:52:02.000000 img2table-1.0.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-07-10 22:54:14.000000 img2table-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-07-10 22:52:02.000000 img2table-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-10 22:52:02.000000 img2table-1.0.6/activate_venv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-07-10 22:52:02.000000 img2table-1.0.6/examples/Basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-07-10 22:52:02.000000 img2table-1.0.6/examples/Implicit_rows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   727975 2023-07-10 22:52:02.000000 img2table-1.0.6/examples/borderless.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/examples/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/examples/data/borderless/
+-rw-r--r--   0 runner    (1001) docker     (123)    47122 2023-07-10 22:52:02.000000 img2table-1.0.6/examples/data/borderless/1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   177004 2023-07-10 22:52:02.000000 img2table-1.0.6/examples/data/borderless/2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   182800 2023-07-10 22:52:02.000000 img2table-1.0.6/examples/data/borderless/3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   132335 2023-07-10 22:52:02.000000 img2table-1.0.6/examples/data/borderless/4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-07-10 22:52:02.000000 img2table-1.0.6/examples/data/borderless.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-07-10 22:52:02.000000 img2table-1.0.6/examples/data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-07-10 22:52:02.000000 img2table-1.0.6/examples/data/tables.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-10 22:52:02.000000 img2table-1.0.6/examples/data/tables.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-07-10 22:52:02.000000 img2table-1.0.6/examples/data/tables.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-10 22:52:02.000000 img2table-1.0.6/examples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 22:52:02.000000 img2table-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 22:52:02.000000 img2table-1.0.6/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-10 22:52:02.000000 img2table-1.0.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-10 22:52:02.000000 img2table-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-10 22:54:14.000000 img2table-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-10 22:52:02.000000 img2table-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/document/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/document/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/document/base/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/document/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/document/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/ocr/aws_textract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/ocr/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/ocr/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/ocr/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/ocr/easyocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/ocr/google_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/ocr/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/ocr/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/ocr/tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/objects/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/objects/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/objects/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/objects/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/bordered_tables/cells/identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/bordered_tables/lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/image_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/image_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/image_segmentation/column_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/image_segmentation/segment_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/image_segmentation/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/rows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/rows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/rows/coherency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/table/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/borderless_tables/table/table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-10 22:52:02.000000 img2table-1.0.6/src/img2table/tables/processing/text/titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 22:54:14.000000 img2table-1.0.6/src/img2table.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/_mock_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/_mock_data/azure.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/_mock_data/tesseract_hocr.html
+-rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/_mock_data/textract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/_mock_data/vision.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/_mock_data/vision.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/document/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/document/base/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/document/base/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/document/base/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/document/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/document/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/document/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/document/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/document/image/test_data/dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/document/image/test_data/expected.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/document/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/document/image/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/document/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/document/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/document/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/document/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/document/pdf/test_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/aws_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/aws_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/aws_textract/test_aws_textract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/aws_textract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/aws_textract/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/aws_textract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/aws_textract/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/azure/test_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/azure/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/azure/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/azure/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/data/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/data/test_data/expected_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/data/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/data/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/data/test_ocr_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/easyocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/easyocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/easyocr/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/easyocr/test_data/ocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/easyocr/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/easyocr/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/easyocr/test_easyocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/google_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/google_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/google_vision/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/google_vision/test_data/expected_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/google_vision/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/google_vision/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/google_vision/test_google_vision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/paddle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/paddle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/paddle/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/paddle/test_data/hocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/paddle/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/paddle/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/paddle/test_paddle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/pdf/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/pdf/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/pdf/test_pdf_ocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/tesseract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/tesseract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/ocr/tesseract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/tesseract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/tesseract/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/ocr/tesseract/test_tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/image/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/image/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/image/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/objects/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/objects/test_data/expected_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/objects/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/objects/test_data/tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/objects/test_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/objects/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/objects/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/objects/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/cells/test_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/cells/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/cells/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/lines/test_data/contours.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/lines/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/lines/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/contours.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/borderless_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/borderless_tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/borderless_tables/test_data/contours.json
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/borderless_tables/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50091 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/column_delimiters/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/image_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/image_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/image_segmentation/test_column_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/image_segmentation/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/image_segmentation/test_data/contours.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/image_segmentation/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)  3446838 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/image_segmentation/test_data/test.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/image_segmentation/test_image_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/image_segmentation/test_segment_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/image_segmentation/test_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/rows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/rows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/rows/test_coherency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/rows/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/rows/test_data/rows.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/rows/test_rows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/table/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/table/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/table/test_data/rows.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/table/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/table/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/borderless_tables/table/test_table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/common/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/common/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/common/test_data/test.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/prepare_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/prepare_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/prepare_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/prepare_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/prepare_image/test_prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:54:14.000000 img2table-1.0.6/tests/tables/processing/text/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/text/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/text/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/text/test_data/test.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-10 22:52:02.000000 img2table-1.0.6/tests/tables/processing/text/test_titles.py
```

### Comparing `img2table-1.0.5/LICENSE.txt` & `img2table-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/Makefile` & `img2table-1.0.6/Makefile`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/PKG-INFO` & `img2table-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 1.0.5
+Version: 1.0.6
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 1.0.5 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 1.0.6 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
```

### Comparing `img2table-1.0.5/README.md` & `img2table-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/examples/Basic_usage.ipynb` & `img2table-1.0.6/examples/Basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/examples/Implicit_rows.ipynb` & `img2table-1.0.6/examples/Implicit_rows.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/examples/borderless.ipynb` & `img2table-1.0.6/examples/borderless.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/examples/data/borderless/1.png` & `img2table-1.0.6/examples/data/borderless/1.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/examples/data/borderless/2.png` & `img2table-1.0.6/examples/data/borderless/2.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/examples/data/borderless/3.png` & `img2table-1.0.6/examples/data/borderless/3.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/examples/data/borderless/4.png` & `img2table-1.0.6/examples/data/borderless/4.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/examples/data/borderless.jpg` & `img2table-1.0.6/examples/data/borderless.jpg`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/examples/data/implicit.png` & `img2table-1.0.6/examples/data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/examples/data/tables.pdf` & `img2table-1.0.6/examples/data/tables.pdf`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/examples/data/tables.png` & `img2table-1.0.6/examples/data/tables.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/examples/data/tables.xlsx` & `img2table-1.0.6/examples/data/tables.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/examples/utils.py` & `img2table-1.0.6/examples/utils.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/setup.cfg` & `img2table-1.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/__init__.py` & `img2table-1.0.6/src/img2table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/document/base/__init__.py` & `img2table-1.0.6/src/img2table/document/base/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/document/base/rotation.py` & `img2table-1.0.6/src/img2table/document/base/rotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     """
     # Thresholding
     _, thresh = cv2.threshold(img, 0, 255, cv2.THRESH_BINARY_INV + cv2.THRESH_OTSU)
 
     # Connected components
     _, _, stats, _ = cv2.connectedComponentsWithStats(thresh, 8, cv2.CV_32S)
 
-    # Remove connected components with less than 15 pixels
-    mask_pixels = stats[:, cv2.CC_STAT_AREA] > 15
+    # Remove connected components with less than 5 pixels
+    mask_pixels = stats[:, cv2.CC_STAT_AREA] > 5
     stats = stats[mask_pixels]
 
     # Compute median width and height
     median_width = np.median(stats[:, cv2.CC_STAT_WIDTH])
     median_height = np.median(stats[:, cv2.CC_STAT_HEIGHT])
 
     # Compute bbox area bounds
```

### Comparing `img2table-1.0.5/src/img2table/document/image.py` & `img2table-1.0.6/src/img2table/document/image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/document/pdf.py` & `img2table-1.0.6/src/img2table/document/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/ocr/aws_textract.py` & `img2table-1.0.6/src/img2table/ocr/aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/ocr/azure.py` & `img2table-1.0.6/src/img2table/ocr/azure.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/ocr/base.py` & `img2table-1.0.6/src/img2table/ocr/base.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/ocr/data.py` & `img2table-1.0.6/src/img2table/ocr/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,70 +91,73 @@
         """
         Identify text located in Table object
         :param table: Table object
         :param page_number: page number of the cell
         :param min_confidence: minimum confidence in order to include a word, from 0 (worst) to 99 (best)
         :return: table with content set on all cells
         """
-        # Filter dataframe on relevant page
-        df_words = self.df.filter(pl.col('class') == "ocrx_word")
-        if page_number:
-            df_words = df_words.filter(pl.col('page') == page_number)
-        # Filter dataframe on relevant words
-        df_words = df_words.filter(pl.col('value').is_not_null() & (pl.col('confidence') >= min_confidence))
-
-        # Create dataframe containing all coordinates of Cell objects
-        list_cells = [{"row": id_row, "col": id_col, "x1_w": cell.x1, "x2_w": cell.x2, "y1_w": cell.y1, "y2_w": cell.y2}
-                      for id_row, row in enumerate(table.items)
-                      for id_col, cell in enumerate(row.items)]
-        df_cells = pl.LazyFrame(data=list_cells)
-
-        # Cartesian product between two dataframes
-        df_word_cells = df_words.join(other=df_cells, how="cross")
-
-        # Compute coordinates of intersection
-        df_word_cells = df_word_cells.with_columns([pl.max([pl.col('x1'), pl.col('x1_w')]).alias('x_left'),
-                                                    pl.max([pl.col('y1'), pl.col('y1_w')]).alias('y_top'),
-                                                    pl.min([pl.col('x2'), pl.col('x2_w')]).alias('x_right'),
-                                                    pl.min([pl.col('y2'), pl.col('y2_w')]).alias('y_bottom'),
-                                                    ])
-
-        # Filter where intersection is not empty
-        df_intersection = (df_word_cells.filter(pl.col("x_right") > pl.col("x_left"))
-                           .filter(pl.col("y_bottom") > pl.col("y_top"))
-                           )
-
-        # Compute area of word bbox and intersection
-        df_areas = (df_intersection.with_columns([
-            ((pl.col('x2') - pl.col('x1')) * (pl.col('y2') - pl.col('y1'))).alias('w_area'),
-            ((pl.col('x_right') - pl.col('x_left')) * (pl.col('y_bottom') - pl.col('y_top'))).alias('int_area')
-        ])
-        )
-
-        # Filter on words where its bbox is contained in area
-        df_words_contained = df_areas.filter(pl.col('int_area') / pl.col('w_area') >= 0.75)
-
-        # Group text by parent
-        df_text_parent = (df_words_contained
-                          .groupby(['row', 'col', 'parent'])
-                          .agg([pl.col('x1').min(),
-                                pl.col('x2').max(),
-                                pl.col('y1').min(),
-                                pl.col('y2').max(),
-                                pl.col('value').apply(lambda x: ' '.join(x), return_dtype=str).alias('value')])
-                          .sort([pl.col("row"), pl.col("col"), pl.col('y1'), pl.col('x1')])
-                          .groupby(['row', 'col'])
-                          .agg(pl.col('value').apply(lambda x: '\n'.join(x).strip(), return_dtype=str).alias('text'))
-                          )
-
-        # Implement found values to table cells content
-        for rec in df_text_parent.collect(streaming=True).to_dicts():
-            table.items[rec.get('row')].items[rec.get('col')].content = rec.get('text') or None
-
-        return table
+        try:
+            # Filter dataframe on relevant page
+            df_words = self.df.filter(pl.col('class') == "ocrx_word")
+            if page_number:
+                df_words = df_words.filter(pl.col('page') == page_number)
+            # Filter dataframe on relevant words
+            df_words = df_words.filter(pl.col('value').is_not_null() & (pl.col('confidence') >= min_confidence))
+
+            # Create dataframe containing all coordinates of Cell objects
+            list_cells = [{"row": id_row, "col": id_col, "x1_w": cell.x1, "x2_w": cell.x2, "y1_w": cell.y1, "y2_w": cell.y2}
+                          for id_row, row in enumerate(table.items)
+                          for id_col, cell in enumerate(row.items)]
+            df_cells = pl.LazyFrame(data=list_cells)
+
+            # Cartesian product between two dataframes
+            df_word_cells = df_words.join(other=df_cells, how="cross")
+
+            # Compute coordinates of intersection
+            df_word_cells = df_word_cells.with_columns([pl.max([pl.col('x1'), pl.col('x1_w')]).alias('x_left'),
+                                                        pl.max([pl.col('y1'), pl.col('y1_w')]).alias('y_top'),
+                                                        pl.min([pl.col('x2'), pl.col('x2_w')]).alias('x_right'),
+                                                        pl.min([pl.col('y2'), pl.col('y2_w')]).alias('y_bottom'),
+                                                        ])
+
+            # Filter where intersection is not empty
+            df_intersection = (df_word_cells.filter(pl.col("x_right") > pl.col("x_left"))
+                               .filter(pl.col("y_bottom") > pl.col("y_top"))
+                               )
+
+            # Compute area of word bbox and intersection
+            df_areas = (df_intersection.with_columns([
+                ((pl.col('x2') - pl.col('x1')) * (pl.col('y2') - pl.col('y1'))).alias('w_area'),
+                ((pl.col('x_right') - pl.col('x_left')) * (pl.col('y_bottom') - pl.col('y_top'))).alias('int_area')
+            ])
+            )
+
+            # Filter on words where its bbox is contained in area
+            df_words_contained = df_areas.filter(pl.col('int_area') / pl.col('w_area') >= 0.75)
+
+            # Group text by parent
+            df_text_parent = (df_words_contained
+                              .groupby(['row', 'col', 'parent'])
+                              .agg([pl.col('x1').min(),
+                                    pl.col('x2').max(),
+                                    pl.col('y1').min(),
+                                    pl.col('y2').max(),
+                                    pl.col('value').apply(lambda x: ' '.join(x), return_dtype=str).alias('value')])
+                              .sort([pl.col("row"), pl.col("col"), pl.col('y1'), pl.col('x1')])
+                              .groupby(['row', 'col'])
+                              .agg(pl.col('value').apply(lambda x: '\n'.join(x).strip(), return_dtype=str).alias('text'))
+                              )
+
+            # Implement found values to table cells content
+            for rec in df_text_parent.collect(streaming=True).to_dicts():
+                table.items[rec.get('row')].items[rec.get('col')].content = rec.get('text') or None
+
+            return table
+        except pl.PolarsPanicError:
+            return table
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             try:
                 assert self.df.collect(streaming=True).sort(by=['id']).frame_equal(other.df.collect(streaming=True).sort(by=['id']))
                 return True
             except AssertionError:
```

### Comparing `img2table-1.0.5/src/img2table/ocr/easyocr.py` & `img2table-1.0.6/src/img2table/ocr/easyocr.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/ocr/google_vision.py` & `img2table-1.0.6/src/img2table/ocr/google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/ocr/paddle.py` & `img2table-1.0.6/src/img2table/ocr/paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/ocr/pdf.py` & `img2table-1.0.6/src/img2table/ocr/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/ocr/tesseract.py` & `img2table-1.0.6/src/img2table/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/__init__.py` & `img2table-1.0.6/src/img2table/tables/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     :return: list of list of items based on clustering function
     """
     # Create clusters based on clustering function between items
     clusters = list()
     for i in range(len(items)):
         for j in range(i, len(items)):
             # Check if both items corresponds according to the clustering function
-            corresponds = clustering_func(items[i], items[j])
+            corresponds = clustering_func(items[i], items[j]) or (items[i] == items[j])
 
             # If both items correspond, find matching clusters or create a new one
             if corresponds:
                 matching_clusters = [idx for idx, cl in enumerate(clusters) if {i, j}.intersection(cl)]
                 if matching_clusters:
                     remaining_clusters = [cl for idx, cl in enumerate(clusters) if idx not in matching_clusters]
                     new_cluster = {i, j}.union(*[cl for idx, cl in enumerate(clusters) if idx in matching_clusters])
```

### Comparing `img2table-1.0.5/src/img2table/tables/image.py` & `img2table-1.0.6/src/img2table/tables/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf-8
 import copy
 from dataclasses import dataclass
 
+from img2table.ocr.data import OCRDataframe
 from img2table.tables.metrics import compute_img_metrics
 from img2table.tables.objects.cell import Cell
 
 try:
     from functools import cached_property
 except ImportError:
     from cached_property import cached_property
@@ -87,36 +88,38 @@
 
         # Create tables from rows
         self.tables = get_tables(cells=cells)
 
         # If necessary, detect implicit rows
         if implicit_rows:
             self.tables = handle_implicit_rows(img=self.white_img,
-                                               tables=self.tables)
+                                               tables=self.tables,
+                                               contours=self.contours)
 
         # If ocr_df is available, get tables content
         if self.ocr_df is not None:
             # Get content
             self.tables = [table.get_content(ocr_df=self.ocr_df, min_confidence=self.min_confidence)
                            for table in self.tables]
 
-        self.tables = [table for table in self.tables if table.nb_rows * table.nb_columns > 1]
+        self.tables = [tb for tb in self.tables if min(tb.nb_rows, tb.nb_columns) >= 2]
 
     def extract_borderless_tables(self):
         """
         Identify and extract borderless tables from image
         :return:
         """
         # Median line separation needs to be not null to extract borderless tables
         if self.median_line_sep is not None:
             # Extract borderless tables
             borderless_tbs = identify_borderless_tables(img=self.img,
                                                         char_length=self.char_length,
                                                         median_line_sep=self.median_line_sep,
                                                         lines=self.lines,
+                                                        contours=self.contours,
                                                         existing_tables=self.tables)
 
             # If ocr_df is available, get tables content
             if self.ocr_df is not None:
                 # Get content
                 borderless_tbs = [table.get_content(ocr_df=self.ocr_df, min_confidence=self.min_confidence)
                                   for table in borderless_tbs]
```

### Comparing `img2table-1.0.5/src/img2table/tables/metrics.py` & `img2table-1.0.6/src/img2table/tables/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     """
     # Thresholding
     _, thresh = cv2.threshold(img, 0, 255, cv2.THRESH_BINARY_INV + cv2.THRESH_OTSU)
 
     # Connected components
     _, _, stats, _ = cv2.connectedComponentsWithStats(thresh, 8, cv2.CV_32S)
 
-    # Remove connected components with less than 15 pixels
-    mask_pixels = stats[:, cv2.CC_STAT_AREA] > 15
+    # Remove connected components with less than 5 pixels
+    mask_pixels = stats[:, cv2.CC_STAT_AREA] > 5
     stats = stats[mask_pixels]
 
     if len(stats) == 0:
         return None, None
 
     # Create mask to remove connected components corresponding to the complete image
     mask_height = img.shape[0] > stats[:, cv2.CC_STAT_HEIGHT]
@@ -42,16 +42,16 @@
 
     # Filter components based on aspect ratio
     mask_lower_ar = 0.2 < stats[:, cv2.CC_STAT_WIDTH] / stats[:, cv2.CC_STAT_HEIGHT]
     mask_upper_ar = 5 > stats[:, cv2.CC_STAT_WIDTH] / stats[:, cv2.CC_STAT_HEIGHT]
     mask_ar = mask_lower_ar & mask_upper_ar
 
     # Filter connected components according to their area
-    mask_lower_area = lower_bound < stats[:, cv2.CC_STAT_WIDTH] * stats[:, cv2.CC_STAT_HEIGHT]
-    mask_upper_area = upper_bound > stats[:, cv2.CC_STAT_WIDTH] * stats[:, cv2.CC_STAT_HEIGHT]
+    mask_lower_area = lower_bound <= stats[:, cv2.CC_STAT_WIDTH] * stats[:, cv2.CC_STAT_HEIGHT]
+    mask_upper_area = upper_bound >= stats[:, cv2.CC_STAT_WIDTH] * stats[:, cv2.CC_STAT_HEIGHT]
     mask_area = mask_lower_area & mask_upper_area
 
     # Filter connected components from mask
     stats = stats[mask_img & mask_area & mask_ar]
 
     if len(stats) > 0:
         # Compute average character length
@@ -76,15 +76,15 @@
     for c in cc:
         cv2.rectangle(black_img,
                       (c[cv2.CC_STAT_LEFT], c[cv2.CC_STAT_TOP]),
                       (c[cv2.CC_STAT_LEFT] + c[cv2.CC_STAT_WIDTH], c[cv2.CC_STAT_TOP] + c[cv2.CC_STAT_HEIGHT]),
                       (255, 255, 255), -1)
 
     # Dilate image
-    kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (max(int(round(char_length)), 1), 1))
+    kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (max(int(round(1.25 * char_length)), 1), 1))
     dilate = cv2.dilate(black_img, kernel, iterations=1)
 
     # Find and map contours
     cnts, _ = cv2.findContours(dilate, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
 
     contours = list()
     for idx, cnt in enumerate(cnts):
```

### Comparing `img2table-1.0.5/src/img2table/tables/objects/__init__.py` & `img2table-1.0.6/src/img2table/tables/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/objects/extraction.py` & `img2table-1.0.6/src/img2table/tables/objects/extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/objects/line.py` & `img2table-1.0.6/src/img2table/tables/objects/line.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/objects/row.py` & `img2table-1.0.6/src/img2table/tables/objects/row.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/objects/table.py` & `img2table-1.0.6/src/img2table/tables/objects/table.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/processing/bordered_tables/cells/__init__.py` & `img2table-1.0.6/src/img2table/tables/processing/bordered_tables/cells/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/processing/bordered_tables/cells/deduplication.py` & `img2table-1.0.6/src/img2table/tables/processing/bordered_tables/cells/deduplication.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/processing/bordered_tables/cells/identification.py` & `img2table-1.0.6/src/img2table/tables/processing/bordered_tables/cells/identification.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/processing/bordered_tables/lines.py` & `img2table-1.0.6/src/img2table/tables/processing/bordered_tables/lines.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,20 @@
     Threshold image by differentiating areas with light and dark backgrounds
     :param img: image array
     :param char_length: average character length
     :return: threshold image
     """
     # Get threshold on image and binary image
     blur = cv2.GaussianBlur(img, (3, 3), 0)
-    thresh = cv2.adaptiveThreshold(blur, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, 21, 10)
-    binary_thresh = cv2.adaptiveThreshold(255 - blur, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, 21, 10)
+
+    thresh_kernel = max(int(round(char_length)), 1) if char_length else 21
+    thresh_kernel = thresh_kernel + 1 if thresh_kernel % 2 == 0 else thresh_kernel
+
+    thresh = cv2.adaptiveThreshold(blur, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, thresh_kernel, 5)
+    binary_thresh = cv2.adaptiveThreshold(255 - blur, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, thresh_kernel, 5)
 
     # Mask on areas with dark background
     blur_size = min(255, max(int(2 * char_length) + 1 - int(2 * char_length) % 2, 1) if char_length else 11)
     blur = cv2.medianBlur(img, blur_size)
     mask = cv2.inRange(blur, 0, 100)
 
     # Get contours of dark areas
@@ -191,28 +195,28 @@
     # - vertical case
     vert_int = (
         (((pl.col('x1') + pl.col('x2')) / 2 - pl.col('x1_line')).abs() / (pl.col('x2') - pl.col('x1')) < 0.45)
         * pl.max([(pl.min([pl.col('y2'), pl.col('y2_line')]) - pl.max([pl.col('y1'), pl.col('y1_line')])), pl.lit(0)])
     )
     # - horizontal case
     hor_int = (
-        (((pl.col('y1') + pl.col('y2')) / 2 - pl.col('y1_line')).abs() / (pl.col('y2') - pl.col('y1')) < 0.4)
+        (((pl.col('y1') + pl.col('y2')) / 2 - pl.col('y1_line')).abs() / (pl.col('y2') - pl.col('y1')) < 0.33)
         * pl.max([(pl.min([pl.col('x2'), pl.col('x2_line')]) - pl.max([pl.col('x1'), pl.col('x1_line')])), pl.lit(0)])
     )
     df_words_lines = df_words_lines.with_columns((pl.col('vertical') * vert_int
                                                   + (1 - pl.col('vertical')) * hor_int).alias('intersection')
                                                  )
 
     # Compute total intersection for each line
     df_inter = (df_words_lines.groupby(['line_id', 'length'])
                 .agg(pl.col('intersection').sum().alias('intersection'))
                 )
 
     # Identify rows that intersect contours
-    intersecting_lines = (df_inter.filter(pl.col('intersection') / pl.col('length') > 0.5)
+    intersecting_lines = (df_inter.filter(pl.col('intersection') / pl.col('length') > 0.25)
                           .collect(streaming=True)
                           .get_column('line_id')
                           .to_list()
                           )
 
     return [line for idx, line in enumerate(lines) if idx not in intersecting_lines]
```

### Comparing `img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/__init__.py` & `img2table-1.0.6/src/img2table/tables/processing/bordered_tables/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py` & `img2table-1.0.6/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,24 +13,24 @@
     """
     # Check correspondence on vertical borders
     overlapping_y = min(cell_1.y2, cell_2.y2) - max(cell_1.y1, cell_2.y1)
     diff_x = min(abs(cell_1.x2 - cell_2.x1),
                  abs(cell_1.x1 - cell_2.x2),
                  abs(cell_1.x1 - cell_2.x1),
                  abs(cell_1.x2 - cell_2.x2))
-    if overlapping_y > 5 and diff_x / max(cell_1.width, cell_2.width) <= 0.05:
+    if overlapping_y > 5 and diff_x <= min(min(cell_1.width, cell_2.width) * 0.05, 5):
         return True
 
     # Check correspondence on horizontal borders
     overlapping_x = min(cell_1.x2, cell_2.x2) - max(cell_1.x1, cell_2.x1)
     diff_y = min(abs(cell_1.y2 - cell_2.y1),
                  abs(cell_1.y1 - cell_2.y2),
                  abs(cell_1.y1 - cell_2.y1),
                  abs(cell_1.y2 - cell_2.y2))
-    if overlapping_x > 5 and diff_y / max(cell_1.height, cell_2.height) <= 0.05:
+    if overlapping_x > 5 and diff_y <= min(min(cell_1.height, cell_2.height) * 0.05, 5):
         return True
 
     return False
 
 
 def cluster_cells_in_tables(cells: List[Cell]) -> List[List[Cell]]:
     """
```

### Comparing `img2table-1.0.5/src/img2table/tables/processing/bordered_tables/tables/table_creation.py` & `img2table-1.0.6/src/img2table/tables/processing/bordered_tables/tables/table_creation.py`

 * *Files 20% similar despite different names*

```diff
@@ -56,23 +56,32 @@
 
     # Get list of horizontal delimiters
     h_delims = sorted(list(set([x_val for cell in cluster_cells for x_val in [cell.x1, cell.x2]])))
 
     # Create rows and cells
     list_rows = list()
     for y_top, y_bottom in zip(v_delims, v_delims[1:]):
+        # Get matching cell
+        matching_cells = [c for c in cluster_cells
+                          if min(c.y2, y_bottom) - max(c.y1, y_top) >= 0.9 * (y_bottom - y_top)]
         list_cells = list()
         for x_left, x_right in zip(h_delims, h_delims[1:]):
             # Create default cell
             default_cell = Cell(x1=x_left, y1=y_top, x2=x_right, y2=y_bottom)
 
             # Check cells that contain the default cell
-            containing_cells = sorted([c for c in cluster_cells
+            containing_cells = sorted([c for c in matching_cells
                                        if is_contained_cell(inner_cell=default_cell, outer_cell=c, percentage=0.9)],
                                       key=lambda c: c.area)
 
-            # Append either a cell that contain the default cell, or the default cell itself
-            list_cells.append(containing_cells.pop(0) if containing_cells else default_cell)
+            # Append either a cell that contain the default cell
+            if containing_cells:
+                list_cells.append(containing_cells.pop(0))
+            else:
+                # Get x value of closest matching cells
+                x_value = sorted([x_val for cell in matching_cells for x_val in [cell.x1, cell.x2]],
+                                 key=lambda x: min(abs(x - x_left), abs(x - x_right))).pop(0)
+                list_cells.append(Cell(x1=x_value, y1=y_top, x2=x_value, y2=y_bottom))
 
         list_rows.append(Row(cells=list_cells))
 
     return Table(rows=list_rows)
```

### Comparing `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/__init__.py` & `img2table-1.0.6/src/img2table/tables/processing/borderless_tables/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # coding: utf-8
 from typing import List
 
 import numpy as np
 
+from img2table.tables.objects.cell import Cell
 from img2table.tables.objects.line import Line
 from img2table.tables.objects.table import Table
 from img2table.tables.processing.borderless_tables.column_delimiters import identify_column_groups
+from img2table.tables.processing.borderless_tables.image_segmentation import segment_image
 from img2table.tables.processing.borderless_tables.rows import detect_delimiter_group_rows
-from img2table.tables.processing.borderless_tables.segment_image import segment_image
 from img2table.tables.processing.borderless_tables.table import identify_table
 from img2table.tables.processing.common import is_contained_cell
 
 
 def deduplicate_tables(identified_tables: List[Table], existing_tables: List[Table]) -> List[Table]:
     """
     Deduplicate identified borderless tables with already identified tables in order to avoid duplicates and overlap
@@ -30,29 +31,31 @@
                     for tb in existing_tables + final_tables]):
             final_tables.append(table)
 
     return final_tables
 
 
 def identify_borderless_tables(img: np.ndarray, lines: List[Line], char_length: float, median_line_sep: float,
-                               existing_tables: List[Table]) -> List[Table]:
+                               contours: List[Cell], existing_tables: List[Table]) -> List[Table]:
     """
     Identify borderless tables in image
     :param img: image array
     :param lines: list of rows detected in image
     :param char_length: average character length
     :param median_line_sep: median line separation
+    :param contours: list of image contours
     :param existing_tables: list of detected bordered tables
     :return: list of detected borderless tables
     """
     # Segment image
     img_segments = segment_image(img=img,
                                  lines=lines,
                                  char_length=char_length,
-                                 median_line_sep=median_line_sep)
+                                 median_line_sep=median_line_sep,
+                                 contours=contours)
 
     # In each segment, create groups of rows and identify tables
     tables = list()
     for seg in img_segments:
         # Identify column groups in segment
         column_groups = identify_column_groups(segment=seg,
                                                char_length=char_length)
```

### Comparing `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py` & `img2table-1.0.6/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py` & `img2table-1.0.6/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,17 @@
     """
     # Get elements that correspond to the delimiter group
     delim_elements = [el for el in segment.elements
                       if el.y1 >= delimiter_group.y1 and el.y2 <= delimiter_group.y2
                       and el.x1 >= min([d.x2 for d in delimiter_group.delimiters])
                       and el.x2 <= max([d.x1 for d in delimiter_group.delimiters])]
 
+    if len(delim_elements) == 0:
+        return delimiter_group
+
     # Group elements in rows
     seq = iter(sorted(delim_elements, key=lambda el: (el.y1, el.y2)))
     lines = [[next(seq)]]
     for el in seq:
         y2_line = max([el.y2 for el in lines[-1]])
         if el.y1 >= y2_line:
             lines.append([])
```

### Comparing `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py` & `img2table-1.0.6/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/model.py` & `img2table-1.0.6/src/img2table/tables/processing/borderless_tables/model.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/rows/__init__.py` & `img2table-1.0.6/src/img2table/tables/processing/borderless_tables/rows/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/rows/coherency.py` & `img2table-1.0.6/src/img2table/tables/processing/borderless_tables/rows/coherency.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py` & `img2table-1.0.6/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/table/__init__.py` & `img2table-1.0.6/src/img2table/tables/processing/borderless_tables/table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/table/headers.py` & `img2table-1.0.6/src/img2table/tables/processing/borderless_tables/table/headers.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/processing/borderless_tables/table/table_creation.py` & `img2table-1.0.6/src/img2table/tables/processing/borderless_tables/table/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/processing/common.py` & `img2table-1.0.6/src/img2table/tables/processing/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,19 +26,16 @@
 
     # Compute common coordinates
     x_left = max(inner_cell.x1, outer_cell.x1)
     y_top = max(inner_cell.y1, outer_cell.y1)
     x_right = min(inner_cell.x2, outer_cell.x2)
     y_bottom = min(inner_cell.y2, outer_cell.y2)
 
-    if x_right < x_left or y_bottom < y_top:
-        return False
-
     # Compute intersection area as well as inner cell area
-    intersection_area = (x_right - x_left) * (y_bottom - y_top)
+    intersection_area = max(0, (x_right - x_left)) * max(0, (y_bottom - y_top))
 
     return intersection_area / inner_cell.area >= percentage
 
 
 def merge_overlapping_contours(contours: List[Cell]) -> List[Cell]:
     """
     Merge overlapping contours
```

### Comparing `img2table-1.0.5/src/img2table/tables/processing/prepare_image.py` & `img2table-1.0.6/src/img2table/tables/processing/prepare_image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table/tables/processing/text/titles.py` & `img2table-1.0.6/src/img2table/tables/processing/text/titles.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/src/img2table.egg-info/PKG-INFO` & `img2table-1.0.6/src/img2table.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 1.0.5
+Version: 1.0.6
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 1.0.5 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 1.0.6 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
```

### Comparing `img2table-1.0.5/src/img2table.egg-info/SOURCES.txt` & `img2table-1.0.6/src/img2table.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -66,18 +66,21 @@
 src/img2table/tables/processing/bordered_tables/cells/identification.py
 src/img2table/tables/processing/bordered_tables/tables/__init__.py
 src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
 src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
 src/img2table/tables/processing/bordered_tables/tables/table_creation.py
 src/img2table/tables/processing/borderless_tables/__init__.py
 src/img2table/tables/processing/borderless_tables/model.py
-src/img2table/tables/processing/borderless_tables/segment_image.py
 src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py
 src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py
 src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py
+src/img2table/tables/processing/borderless_tables/image_segmentation/__init__.py
+src/img2table/tables/processing/borderless_tables/image_segmentation/column_segmentation.py
+src/img2table/tables/processing/borderless_tables/image_segmentation/segment_elements.py
+src/img2table/tables/processing/borderless_tables/image_segmentation/segmentation.py
 src/img2table/tables/processing/borderless_tables/rows/__init__.py
 src/img2table/tables/processing/borderless_tables/rows/coherency.py
 src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py
 src/img2table/tables/processing/borderless_tables/table/__init__.py
 src/img2table/tables/processing/borderless_tables/table/headers.py
 src/img2table/tables/processing/borderless_tables/table/table_creation.py
 src/img2table/tables/processing/text/__init__.py
@@ -176,39 +179,45 @@
 tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
 tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
 tests/tables/processing/bordered_tables/tables/test_table_creation.py
 tests/tables/processing/bordered_tables/tables/test_tables.py
 tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
 tests/tables/processing/bordered_tables/tables/test_data/cells.json
 tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
+tests/tables/processing/bordered_tables/tables/test_data/contours.json
 tests/tables/processing/bordered_tables/tables/test_data/expected.json
 tests/tables/processing/bordered_tables/tables/test_data/implicit.png
 tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
 tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
 tests/tables/processing/bordered_tables/tables/test_data/word_image.png
 tests/tables/processing/borderless_tables/__init__.py
 tests/tables/processing/borderless_tables/borderless_tables/__init__.py
 tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py
+tests/tables/processing/borderless_tables/borderless_tables/test_data/contours.json
 tests/tables/processing/borderless_tables/borderless_tables/test_data/lines.json
 tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png
 tests/tables/processing/borderless_tables/column_delimiters/__init__.py
 tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
 tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py
 tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py
 tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json
+tests/tables/processing/borderless_tables/image_segmentation/__init__.py
+tests/tables/processing/borderless_tables/image_segmentation/test_column_segmentation.py
+tests/tables/processing/borderless_tables/image_segmentation/test_image_segmentation.py
+tests/tables/processing/borderless_tables/image_segmentation/test_segment_elements.py
+tests/tables/processing/borderless_tables/image_segmentation/test_segmentation.py
+tests/tables/processing/borderless_tables/image_segmentation/test_data/contours.json
+tests/tables/processing/borderless_tables/image_segmentation/test_data/lines.json
+tests/tables/processing/borderless_tables/image_segmentation/test_data/test.bmp
 tests/tables/processing/borderless_tables/rows/__init__.py
 tests/tables/processing/borderless_tables/rows/test_coherency.py
 tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py
 tests/tables/processing/borderless_tables/rows/test_rows.py
 tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json
 tests/tables/processing/borderless_tables/rows/test_data/rows.json
-tests/tables/processing/borderless_tables/segment_image/__init__.py
-tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
-tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
-tests/tables/processing/borderless_tables/segment_image/test_data/test.png
 tests/tables/processing/borderless_tables/table/__init__.py
 tests/tables/processing/borderless_tables/table/test_headers.py
 tests/tables/processing/borderless_tables/table/test_table.py
 tests/tables/processing/borderless_tables/table/test_table_creation.py
 tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json
 tests/tables/processing/borderless_tables/table/test_data/lines.json
 tests/tables/processing/borderless_tables/table/test_data/rows.json
```

### Comparing `img2table-1.0.5/tests/_mock_data/azure.pkl` & `img2table-1.0.6/tests/_mock_data/azure.pkl`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/_mock_data/tesseract_hocr.html` & `img2table-1.0.6/tests/_mock_data/tesseract_hocr.html`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/_mock_data/textract.json` & `img2table-1.0.6/tests/_mock_data/textract.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/_mock_data/vision.json` & `img2table-1.0.6/tests/_mock_data/vision.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/_mock_data/vision.pkl` & `img2table-1.0.6/tests/_mock_data/vision.pkl`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/conftest.py` & `img2table-1.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/document/base/test_data/test.png` & `img2table-1.0.6/tests/document/base/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/document/base/test_rotation.py` & `img2table-1.0.6/tests/document/base/test_rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/document/image/test_data/blank.png` & `img2table-1.0.6/tests/document/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/document/image/test_data/dark.png` & `img2table-1.0.6/tests/document/image/test_data/dark.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/document/image/test_data/expected.xlsx` & `img2table-1.0.6/tests/document/image/test_data/expected.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/document/image/test_data/test.png` & `img2table-1.0.6/tests/document/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/document/image/test_image.py` & `img2table-1.0.6/tests/document/image/test_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,34 +64,34 @@
                 detect_rotation=True)
 
     result = img.extract_tables(ocr=ocr, implicit_rows=True, min_confidence=50)
 
     assert len(result) == 2
 
     assert result[0].title is None
-    assert result[0].bbox == BBox(x1=35, y1=20, x2=770, y2=327)
+    assert result[0].bbox == BBox(x1=36, y1=20, x2=770, y2=326)
     assert len(result[0].content) == 6
     assert len(result[0].content[0]) == 3
 
     assert result[1].title is None
-    assert result[1].bbox == BBox(x1=962, y1=20, x2=1154, y2=123)
+    assert result[1].bbox == BBox(x1=962, y1=21, x2=1154, y2=122)
     assert len(result[1].content) == 2
     assert len(result[1].content[0]) == 2
 
 
 def test_no_ocr():
     img = Image(src="test_data/dark.png",
                 detect_rotation=True)
 
     result = img.extract_tables(implicit_rows=True, min_confidence=50)
 
     assert len(result) == 1
 
     assert result[0].title is None
-    assert result[0].bbox == BBox(x1=36, y1=40, x2=840, y2=529)
+    assert result[0].bbox == BBox(x1=36, y1=38, x2=840, y2=530)
     assert len(result[0].content) == 19
     assert len(result[0].content[0]) == 7
 
 
 def test_image_excel(mock_tesseract):
     ocr = TesseractOCR()
     img = Image(src="test_data/test.png",
```

### Comparing `img2table-1.0.5/tests/document/pdf/test_data/test.pdf` & `img2table-1.0.6/tests/document/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/document/pdf/test_pdf.py` & `img2table-1.0.6/tests/document/pdf/test_pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,24 +49,24 @@
     ocr = TesseractOCR()
     pdf = PDF(src="test_data/test.pdf")
 
     result = pdf.extract_tables(ocr=ocr, implicit_rows=True, min_confidence=50)
 
     assert result[0][0].title == "Example of Data Table 1"
     if sys.version_info.minor < 11:
-        assert result[0][0].bbox == BBox(x1=235, y1=249, x2=1442, y2=543)
+        assert result[0][0].bbox == BBox(x1=236, y1=249, x2=1442, y2=543)
     assert (len(result[0][0].content), len(result[0][0].content[0])) == (5, 4)
 
     assert result[0][1].title == "Example of Data Table 2"
     if sys.version_info.minor < 11:
-        assert result[0][1].bbox == BBox(x1=235, y1=671, x2=1451, y2=971)
+        assert result[0][1].bbox == BBox(x1=236, y1=672, x2=1451, y2=971)
     assert (len(result[0][1].content), len(result[0][1].content[0])) == (5, 4)
 
     assert result[1][0].title == "Example of Data Table 3"
     if sys.version_info.minor < 11:
         assert result[1][0].bbox == BBox(x1=236, y1=249, x2=1442, y2=543)
     assert (len(result[1][0].content), len(result[1][0].content[0])) == (5, 4)
 
     assert result[1][1].title == "Example of Data Table 4"
     if sys.version_info.minor < 11:
-        assert result[1][1].bbox == BBox(x1=235, y1=671, x2=1451, y2=971)
+        assert result[1][1].bbox == BBox(x1=236, y1=672, x2=1451, y2=971)
     assert (len(result[1][1].content), len(result[1][1].content[0])) == (5, 4)
```

### Comparing `img2table-1.0.5/tests/ocr/aws_textract/test_aws_textract.py` & `img2table-1.0.6/tests/ocr/aws_textract/test_aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/aws_textract/test_data/content.json` & `img2table-1.0.6/tests/ocr/aws_textract/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/aws_textract/test_data/ocr_df.csv` & `img2table-1.0.6/tests/ocr/aws_textract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/aws_textract/test_data/test.png` & `img2table-1.0.6/tests/ocr/aws_textract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/azure/test_azure.py` & `img2table-1.0.6/tests/ocr/azure/test_azure.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/azure/test_data/ocr_df.csv` & `img2table-1.0.6/tests/ocr/azure/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/azure/test_data/test.png` & `img2table-1.0.6/tests/ocr/azure/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/data/test_data/expected_table.json` & `img2table-1.0.6/tests/ocr/data/test_data/expected_table.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/data/test_data/ocr_df.csv` & `img2table-1.0.6/tests/ocr/data/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/data/test_ocr_data.py` & `img2table-1.0.6/tests/ocr/data/test_ocr_data.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/easyocr/test_data/ocr.json` & `img2table-1.0.6/tests/ocr/easyocr/test_data/ocr.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/easyocr/test_data/ocr_df.csv` & `img2table-1.0.6/tests/ocr/easyocr/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/easyocr/test_data/test.png` & `img2table-1.0.6/tests/ocr/easyocr/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/easyocr/test_easyocr.py` & `img2table-1.0.6/tests/ocr/easyocr/test_easyocr.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/google_vision/test_data/expected_content.json` & `img2table-1.0.6/tests/ocr/google_vision/test_data/expected_content.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/google_vision/test_data/ocr_df.csv` & `img2table-1.0.6/tests/ocr/google_vision/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/google_vision/test_data/test.png` & `img2table-1.0.6/tests/ocr/google_vision/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/google_vision/test_google_vision.py` & `img2table-1.0.6/tests/ocr/google_vision/test_google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/paddle/test_data/hocr.json` & `img2table-1.0.6/tests/ocr/paddle/test_data/hocr.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/paddle/test_data/ocr_df.csv` & `img2table-1.0.6/tests/ocr/paddle/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/paddle/test_data/test.png` & `img2table-1.0.6/tests/ocr/paddle/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/paddle/test_paddle.py` & `img2table-1.0.6/tests/ocr/paddle/test_paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/pdf/test_data/content.json` & `img2table-1.0.6/tests/ocr/pdf/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/pdf/test_data/ocr_df.csv` & `img2table-1.0.6/tests/ocr/pdf/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/pdf/test_data/test.pdf` & `img2table-1.0.6/tests/ocr/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/pdf/test_pdf_ocr.py` & `img2table-1.0.6/tests/ocr/pdf/test_pdf_ocr.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/tesseract/test_data/ocr_df.csv` & `img2table-1.0.6/tests/ocr/tesseract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/tesseract/test_data/test.png` & `img2table-1.0.6/tests/ocr/tesseract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/ocr/tesseract/test_tesseract.py` & `img2table-1.0.6/tests/ocr/tesseract/test_tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/image/test_data/blank.png` & `img2table-1.0.6/tests/tables/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/image/test_data/ocr.csv` & `img2table-1.0.6/tests/tables/image/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/image/test_data/test.png` & `img2table-1.0.6/tests/tables/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/image/test_image.py` & `img2table-1.0.6/tests/tables/image/test_image.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 
     tb_image = TableImage(img=image,
                           ocr_df=ocr_df,
                           min_confidence=50)
 
     result = tb_image.extract_tables(implicit_rows=True)
 
-    assert result[0].bbox == BBox(x1=35, y1=20, x2=770, y2=327)
+    assert result[0].bbox == BBox(x1=36, y1=20, x2=770, y2=326)
     assert (len(result[0].content), len(result[0].content[0])) == (6, 3)
 
-    assert result[1].bbox == BBox(x1=962, y1=20, x2=1154, y2=123)
+    assert result[1].bbox == BBox(x1=962, y1=21, x2=1154, y2=122)
     assert (len(result[1].content), len(result[1].content[0])) == (2, 2)
```

### Comparing `img2table-1.0.5/tests/tables/image/test_metrics.py` & `img2table-1.0.6/tests/tables/image/test_metrics.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/objects/test_data/expected_tables.json` & `img2table-1.0.6/tests/tables/objects/test_data/expected_tables.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/objects/test_data/ocr.csv` & `img2table-1.0.6/tests/tables/objects/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/objects/test_data/tables.json` & `img2table-1.0.6/tests/tables/objects/test_data/tables.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/objects/test_extraction.py` & `img2table-1.0.6/tests/tables/objects/test_extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/objects/test_line.py` & `img2table-1.0.6/tests/tables/objects/test_line.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/objects/test_row.py` & `img2table-1.0.6/tests/tables/objects/test_row.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/objects/test_table.py` & `img2table-1.0.6/tests/tables/objects/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_cells.py` & `img2table-1.0.6/tests/tables/processing/bordered_tables/cells/test_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/expected.csv` & `img2table-1.0.6/tests/tables/processing/bordered_tables/cells/test_data/expected.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_data/lines.json` & `img2table-1.0.6/tests/tables/processing/bordered_tables/cells/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py` & `img2table-1.0.6/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/cells/test_identification_cells.py` & `img2table-1.0.6/tests/tables/processing/bordered_tables/cells/test_identification_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_data/contours.json` & `img2table-1.0.6/tests/tables/processing/bordered_tables/lines/test_data/contours.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_data/expected.json` & `img2table-1.0.6/tests/tables/processing/bordered_tables/lines/test_data/expected.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8321428571428572%*

 * *Differences: {"'h_lines'": "{0: {'x2': 773, 'thickness': 1}, 1: {'x1': 961, 'y1': 20, 'x2': 1158, 'y2': 20, "*

 * *              "'thickness': 1}, 2: {'x1': 35, 'x2': 773, 'thickness': 1}, 3: {'x1': 961, 'x2': "*

 * *              "1158, 'thickness': 1}, 4: {'x1': 35, 'x2': 773, 'thickness': 1}, 5: {'y1': 122, "*

 * *              "'x2': 1158, 'y2': 122, 'thickness': 1}, 6: {'x1': 35, 'x2': 279, 'thickness': 1}, "*

 * *              "7: {'x1': 494, 'x2': 773, 'thickness': 1}, 8: {'x1': 35, 'y1': 224, 'x2': 279, "*

 * *              "'y2': 224}, […]*

```diff
@@ -1,146 +1,139 @@
 {
     "h_lines": [
         {
-            "thickness": 3,
+            "thickness": 1,
             "x1": 35,
-            "x2": 772,
+            "x2": 773,
             "y1": 20,
             "y2": 20
         },
         {
-            "thickness": 3,
-            "x1": 966,
-            "x2": 1156,
-            "y1": 21,
-            "y2": 21
+            "thickness": 1,
+            "x1": 961,
+            "x2": 1158,
+            "y1": 20,
+            "y2": 20
         },
         {
-            "thickness": 3,
-            "x1": 36,
-            "x2": 771,
+            "thickness": 1,
+            "x1": 35,
+            "x2": 773,
             "y1": 72,
             "y2": 72
         },
         {
-            "thickness": 3,
-            "x1": 962,
-            "x2": 1156,
+            "thickness": 1,
+            "x1": 961,
+            "x2": 1158,
             "y1": 72,
             "y2": 72
         },
         {
-            "thickness": 3,
-            "x1": 36,
-            "x2": 771,
+            "thickness": 1,
+            "x1": 35,
+            "x2": 773,
             "y1": 122,
             "y2": 122
         },
         {
-            "thickness": 3,
+            "thickness": 1,
             "x1": 961,
-            "x2": 1156,
-            "y1": 123,
-            "y2": 123
+            "x2": 1158,
+            "y1": 122,
+            "y2": 122
         },
         {
-            "thickness": 3,
-            "x1": 36,
-            "x2": 277,
+            "thickness": 1,
+            "x1": 35,
+            "x2": 279,
             "y1": 173,
             "y2": 173
         },
         {
-            "thickness": 3,
-            "x1": 495,
-            "x2": 771,
+            "thickness": 1,
+            "x1": 494,
+            "x2": 773,
             "y1": 174,
             "y2": 174
         },
         {
             "thickness": 1,
-            "x1": 417,
-            "x2": 446,
-            "y1": 199,
-            "y2": 199
-        },
-        {
-            "thickness": 3,
-            "x1": 36,
-            "x2": 277,
-            "y1": 225,
-            "y2": 225
+            "x1": 35,
+            "x2": 279,
+            "y1": 224,
+            "y2": 224
         },
         {
-            "thickness": 3,
-            "x1": 495,
-            "x2": 771,
-            "y1": 225,
-            "y2": 225
+            "thickness": 1,
+            "x1": 494,
+            "x2": 773,
+            "y1": 224,
+            "y2": 224
         },
         {
-            "thickness": 3,
-            "x1": 36,
-            "x2": 772,
+            "thickness": 1,
+            "x1": 35,
+            "x2": 774,
             "y1": 276,
             "y2": 276
         },
         {
-            "thickness": 3,
+            "thickness": 1,
             "x1": 35,
-            "x2": 772,
-            "y1": 327,
-            "y2": 327
+            "x2": 774,
+            "y1": 326,
+            "y2": 326
         }
     ],
     "v_lines": [
         {
-            "thickness": 3,
-            "x1": 35,
-            "x2": 35,
+            "thickness": 1,
+            "x1": 36,
+            "x2": 36,
             "y1": 20,
-            "y2": 329
+            "y2": 330
         },
         {
-            "thickness": 3,
+            "thickness": 1,
             "x1": 276,
             "x2": 276,
-            "y1": 72,
-            "y2": 328
+            "y1": 71,
+            "y2": 330
         },
         {
             "thickness": 1,
             "x1": 494,
             "x2": 494,
-            "y1": 72,
-            "y2": 328
+            "y1": 71,
+            "y2": 330
         },
         {
-            "thickness": 3,
+            "thickness": 1,
             "x1": 770,
             "x2": 770,
             "y1": 20,
-            "y2": 329
+            "y2": 330
         },
         {
-            "thickness": 2,
-            "x1": 961,
-            "x2": 961,
+            "thickness": 1,
+            "x1": 962,
+            "x2": 962,
             "y1": 20,
-            "y2": 125
+            "y2": 126
         },
         {
             "thickness": 1,
             "x1": 1058,
             "x2": 1058,
-            "y1": 21,
-            "y2": 124
+            "y1": 20,
+            "y2": 126
         },
         {
-            "thickness": 3,
+            "thickness": 1,
             "x1": 1154,
             "x2": 1154,
             "y1": 20,
-            "y2": 125
+            "y2": 126
         }
     ]
 }
```

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_data/test.png` & `img2table-1.0.6/tests/tables/processing/bordered_tables/lines/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/lines/test_lines.py` & `img2table-1.0.6/tests/tables/processing/bordered_tables/lines/test_lines.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py` & `img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json` & `img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/cells.json` & `img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/cells.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json` & `img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/expected.json` & `img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/implicit.png` & `img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json` & `img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_data/word_image.png` & `img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_data/word_image.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py` & `img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,32 +3,55 @@
 
 import cv2
 
 from img2table.tables.objects.cell import Cell
 from img2table.tables.objects.row import Row
 from img2table.tables.objects.table import Table
 from img2table.tables.processing.bordered_tables.tables.implicit_rows import handle_implicit_rows_table, \
-    handle_implicit_rows
+    handle_implicit_rows, compute_table_median_row_sep
+
+
+def test_compute_table_median_row_sep():
+    with open("test_data/contours.json", "r") as f:
+        contours = [Cell(**el) for el in json.load(f)]
+
+    with open("test_data/implicit_table.json", 'r') as f:
+        table = Table(rows=[Row(cells=[Cell(**el) for el in row]) for row in json.load(f)])
+
+    result = compute_table_median_row_sep(table=table,
+                                          contours=contours)
+
+    assert round(result, 2) == 51.0
 
 
 def test_handle_implicit_rows_table():
     img = cv2.imread("test_data/implicit.png", cv2.IMREAD_GRAYSCALE)
 
     with open("test_data/implicit_table.json", 'r') as f:
         table = Table(rows=[Row(cells=[Cell(**el) for el in row]) for row in json.load(f)])
 
-    result = handle_implicit_rows_table(img=img, table=table)
+    with open("test_data/contours.json", "r") as f:
+        contours = [Cell(**el) for el in json.load(f)]
+
+    result = handle_implicit_rows_table(img=img,
+                                        table=table,
+                                        contours=contours)
 
     # Check that 2 more rows have been created
     assert result.nb_rows == table.nb_rows + 2
 
 
 def test_handle_implicit_rows():
     img = cv2.imread("test_data/implicit.png", cv2.IMREAD_GRAYSCALE)
 
     with open("test_data/implicit_table.json", 'r') as f:
         table = Table(rows=[Row(cells=[Cell(**el) for el in row]) for row in json.load(f)])
 
-    result = handle_implicit_rows(img=img, tables=[table])
+    with open("test_data/contours.json", "r") as f:
+        contours = [Cell(**el) for el in json.load(f)]
+
+    result = handle_implicit_rows(img=img,
+                                  tables=[table],
+                                  contours=contours)
 
     # Check that 2 more rows have been created
     assert result[0].nb_rows == table.nb_rows + 2
```

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_table_creation.py` & `img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/bordered_tables/tables/test_tables.py` & `img2table-1.0.6/tests/tables/processing/bordered_tables/tables/test_tables.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png` & `img2table-1.0.6/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py` & `img2table-1.0.6/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py` & `img2table-1.0.6/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json` & `img2table-1.0.6/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py` & `img2table-1.0.6/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_coherency.py` & `img2table-1.0.6/tests/tables/processing/borderless_tables/rows/test_coherency.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json` & `img2table-1.0.6/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_data/rows.json` & `img2table-1.0.6/tests/tables/processing/borderless_tables/rows/test_data/rows.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py` & `img2table-1.0.6/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/rows/test_rows.py` & `img2table-1.0.6/tests/tables/processing/borderless_tables/rows/test_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py` & `img2table-1.0.6/tests/tables/processing/borderless_tables/image_segmentation/test_segment_elements.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,26 @@
 # coding: utf-8
 import json
 
 import cv2
 
 from img2table.tables.objects.line import Line
+from img2table.tables.processing.borderless_tables.image_segmentation import get_segment_elements
 from img2table.tables.processing.borderless_tables.model import ImageSegment
-from img2table.tables.processing.borderless_tables.segment_image import create_image_segments, get_segment_elements, \
-    segment_image
-
-
-def test_create_image_segments():
-    img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-
-    result = create_image_segments(img=img,
-                                   median_line_sep=66,
-                                   char_length=7.24)
-
-    assert result == [ImageSegment(x1=56, y1=0, x2=1273, y2=1173)]
 
 
 def test_get_segment_elements():
-    img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-    img_segments = [ImageSegment(x1=53, y1=0, x2=1277, y2=1173)]
+    img = cv2.imread("test_data/test.bmp", cv2.IMREAD_GRAYSCALE)
+    img_segments = [ImageSegment(x1=61, y1=92, x2=390, y2=652)]
 
     with open("test_data/lines.json", 'r') as f:
         data = json.load(f)
     lines = [Line(**el) for el in data.get('h_lines') + data.get('v_lines')]
 
     result = get_segment_elements(img=img,
                                   lines=lines,
                                   img_segments=img_segments,
                                   blur_size=3,
-                                  char_length=7.24,
-                                  median_line_sep=66)
-
-    assert len(result[0].elements) == 164
-
-
-def test_segment_image():
-    img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-    with open("test_data/lines.json", 'r') as f:
-        data = json.load(f)
-    lines = [Line(**el) for el in data.get('h_lines') + data.get('v_lines')]
-
-    result = segment_image(img=img,
-                           char_length=7.24,
-                           median_line_sep=66,
-                           lines=lines)
+                                  char_length=4.66,
+                                  median_line_sep=16)
 
-    assert len(result[0].elements) == 164
+    assert len(result[0].elements) == 67
```

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json` & `img2table-1.0.6/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_data/rows.json` & `img2table-1.0.6/tests/tables/processing/borderless_tables/table/test_data/rows.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_headers.py` & `img2table-1.0.6/tests/tables/processing/borderless_tables/table/test_headers.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_table.py` & `img2table-1.0.6/tests/tables/processing/borderless_tables/table/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/borderless_tables/table/test_table_creation.py` & `img2table-1.0.6/tests/tables/processing/borderless_tables/table/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/common/test_common.py` & `img2table-1.0.6/tests/tables/processing/common/test_common.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/common/test_data/test.jpg` & `img2table-1.0.6/tests/tables/processing/common/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/prepare_image/test_data/test.png` & `img2table-1.0.6/tests/tables/processing/prepare_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/text/test_data/ocr.csv` & `img2table-1.0.6/tests/tables/processing/text/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/text/test_data/table.json` & `img2table-1.0.6/tests/tables/processing/text/test_data/table.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/text/test_data/test.jpg` & `img2table-1.0.6/tests/tables/processing/text/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-1.0.5/tests/tables/processing/text/test_titles.py` & `img2table-1.0.6/tests/tables/processing/text/test_titles.py`

 * *Files identical despite different names*

