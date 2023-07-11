# Comparing `tmp/hipscat-import-0.0.3.tar.gz` & `tmp/hipscat-import-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipscat-import-0.0.3.tar", last modified: Mon Apr  3 12:42:59 2023, max compression
+gzip compressed data, was "hipscat-import-0.0.4.tar", last modified: Tue Jul 11 19:29:51 2023, max compression
```

## Comparing `hipscat-import-0.0.3.tar` & `hipscat-import-0.0.4.tar`

### file list

```diff
@@ -1,121 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.952882 hipscat-import-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.936881 hipscat-import-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.940881 hipscat-import-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/.github/workflows/type-checking.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-03 12:42:59.952882 hipscat-import-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.940881 hipscat-import-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.940881 hipscat-import-0.0.3/docs/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/catalogs/allwise.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/catalogs/neowise.rst
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/catalogs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/catalogs/tic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.944882 hipscat-import-0.0.3/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/guide/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/guide/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/guide/resume.rst
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.944882 hipscat-import-0.0.3/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.944882 hipscat-import-0.0.3/docs/static/
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/static/allwise_types.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/static/neowise_types.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/docs/static/tic_types.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 12:42:59.952882 hipscat-import-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.944882 hipscat-import-0.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.944882 hipscat-import-0.0.3/src/hipscat_import/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/src/hipscat_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/src/hipscat_import/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-03 12:42:59.000000 hipscat-import-0.0.3/src/hipscat_import/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/src/hipscat_import/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/src/hipscat_import/command_line_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/src/hipscat_import/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/src/hipscat_import/file_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/src/hipscat_import/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/src/hipscat_import/resume_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/src/hipscat_import/run_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.944882 hipscat-import-0.0.3/src/hipscat_import.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-03 12:42:59.000000 hipscat-import-0.0.3/src/hipscat_import.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-03 12:42:59.000000 hipscat-import-0.0.3/src/hipscat_import.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 12:42:59.000000 hipscat-import-0.0.3/src/hipscat_import.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-03 12:42:59.000000 hipscat-import-0.0.3/src/hipscat_import.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-03 12:42:59.000000 hipscat-import-0.0.3/src/hipscat_import.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-03 12:42:59.000000 hipscat-import-0.0.3/src/hipscat_import.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.944882 hipscat-import-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.948882 hipscat-import-0.0.3/tests/hipscat_import/
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.936881 hipscat-import-0.0.3/tests/hipscat_import/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.948882 hipscat-import-0.0.3/tests/hipscat_import/data/blank/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/blank/blank.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.948882 hipscat-import-0.0.3/tests/hipscat_import/data/mixed_schema/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/mixed_schema/input_01.csv
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/mixed_schema/input_02.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/mixed_schema/schema.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.936881 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.936881 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.948882 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_44/
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_44/shard_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_44/shard_1.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_44/shard_2.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_44/shard_3.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_44/shard_4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.948882 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_45/
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_45/shard_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_45/shard_1.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_45/shard_2.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_45/shard_3.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_45/shard_4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.948882 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_46/
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_46/shard_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_46/shard_1.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_46/shard_2.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_46/shard_3.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_46/shard_4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.952882 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_47/
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_47/shard_0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_47/shard_1.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_47/shard_2.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_47/shard_3.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_47/shard_4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.936881 hipscat-import-0.0.3/tests/hipscat_import/data/resume/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.936881 hipscat-import-0.0.3/tests/hipscat_import/data/resume/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.952882 hipscat-import-0.0.3/tests/hipscat_import/data/resume/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.952882 hipscat-import-0.0.3/tests/hipscat_import/data/resume/intermediate/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/resume/intermediate/mapping_histogram.binary
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/resume/intermediate/reducing_log.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.952882 hipscat-import-0.0.3/tests/hipscat_import/data/small_sky/
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/small_sky/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.952882 hipscat-import-0.0.3/tests/hipscat_import/data/small_sky_parts/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:42:59.952882 hipscat-import-0.0.3/tests/hipscat_import/data/test_formats/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/test_formats/headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/test_formats/pipe_delimited.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/data/test_formats/small_sky.fits
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/test_argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/test_arguments_commandline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/test_file_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/test_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/test_resume_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-04-03 12:42:46.000000 hipscat-import-0.0.3/tests/hipscat_import/test_run_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.793901 hipscat-import-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.757902 hipscat-import-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.761901 hipscat-import-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.github/workflows/type-checking.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-11 19:29:51.793901 hipscat-import-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.761901 hipscat-import-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.761901 hipscat-import-0.0.4/docs/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/debug.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.761901 hipscat-import-0.0.4/docs/catalogs/public/
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/public/allwise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/public/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/public/neowise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/public/tic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/public/zubercal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/catalogs/resume.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.765901 hipscat-import-0.0.4/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/guide/association.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/guide/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/guide/index_table.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/guide/margin_cache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.765901 hipscat-import-0.0.4/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/notebooks/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9556 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/notebooks/estimate_pixel_threshold.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.765901 hipscat-import-0.0.4/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   136863 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/static/allwise_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/static/allwise_types.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/static/neowise_types.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/docs/static/tic_types.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:29:51.793901 hipscat-import-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.765901 hipscat-import-0.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    20793 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.765901 hipscat-import-0.0.4/src/hipscat_import/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 19:29:51.000000 hipscat-import-0.0.4/src/hipscat_import/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.769902 hipscat-import-0.0.4/src/hipscat_import/association/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/association/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/association/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/association/run_association.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.769902 hipscat-import-0.0.4/src/hipscat_import/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/catalog/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/catalog/file_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/catalog/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/catalog/resume_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/catalog/run_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.769902 hipscat-import-0.0.4/src/hipscat_import/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/index/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/index/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/index/run_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.769902 hipscat-import-0.0.4/src/hipscat_import/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/margin_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/margin_cache/margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/margin_cache/margin_cache_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/margin_cache/margin_cache_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/src/hipscat_import/runtime_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.769902 hipscat-import-0.0.4/src/hipscat_import.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-11 19:29:51.000000 hipscat-import-0.0.4/src/hipscat_import.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-07-11 19:29:51.000000 hipscat-import-0.0.4/src/hipscat_import.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:29:51.000000 hipscat-import-0.0.4/src/hipscat_import.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-11 19:29:51.000000 hipscat-import-0.0.4/src/hipscat_import.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 19:29:51.000000 hipscat-import-0.0.4/src/hipscat_import.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.769902 hipscat-import-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.773902 hipscat-import-0.0.4/tests/hipscat_import/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.773902 hipscat-import-0.0.4/tests/hipscat_import/association/
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/association/test_association_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/association/test_association_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/association/test_run_association.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.773902 hipscat-import-0.0.4/tests/hipscat_import/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/catalog/test_argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/catalog/test_file_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/catalog/test_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/catalog/test_resume_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/catalog/test_run_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/catalog/test_run_round_trip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.757902 hipscat-import-0.0.4/tests/hipscat_import/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.773902 hipscat-import-0.0.4/tests/hipscat_import/data/blank/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/blank/blank.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.773902 hipscat-import-0.0.4/tests/hipscat_import/data/mixed_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/mixed_schema/input_01.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/mixed_schema/input_02.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/mixed_schema/schema.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.753902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.753902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.753902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.773902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.753902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.753902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.777902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.777902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.777902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.777902 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.753902 hipscat-import-0.0.4/tests/hipscat_import/data/resume/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.753902 hipscat-import-0.0.4/tests/hipscat_import/data/resume/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.777902 hipscat-import-0.0.4/tests/hipscat_import/data/resume/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.781901 hipscat-import-0.0.4/tests/hipscat_import/data/resume/intermediate/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/resume/intermediate/mapping_histogram.binary
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/resume/intermediate/reducing_log.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.781901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.781901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.757902 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.781901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.781901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.781901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source/
+-rw-r--r--   0 runner    (1001) docker     (123)  1688789 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source/small_sky_source.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.785901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.757902 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.785901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.757902 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.785901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)   133704 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.757902 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.789901 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (123)    28379 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    86295 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    92667 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    99907 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    42210 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    54775 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    72993 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    67804 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    80298 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)   162097 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    31794 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    43738 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)    29241 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.789901 hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/catalog.starr
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/multiindex.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/pandasindex.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/pipe_delimited.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/small_sky.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.789901 hipscat-import-0.0.4/tests/hipscat_import/index/
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/index/test_index_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/index/test_index_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/index/test_run_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:29:51.793901 hipscat-import-0.0.4/tests/hipscat_import/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/margin_cache/test_margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-11 19:29:39.000000 hipscat-import-0.0.4/tests/hipscat_import/test_runtime_arguments.py
```

### Comparing `hipscat-import-0.0.3/.github/workflows/linting.yml` & `hipscat-import-0.0.4/.github/workflows/linting.yml`

 * *Files 18% similar despite different names*

```diff
@@ -8,20 +8,24 @@
     branches: [ main ]
   pull_request:
     branches: [ main ]
 
 jobs:
   build:
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: ['3.8', '3.9', '3.10']
+
     steps:
     - uses: actions/checkout@v3
-    - name: Set up Python 3.10
+    - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
-        python-version: '3.10'
+        python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         sudo apt-get update
         python -m pip install --upgrade pip
         pip install .
         pip install .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
```

### Comparing `hipscat-import-0.0.3/.github/workflows/publish-to-pypi.yml` & `hipscat-import-0.0.4/.github/workflows/publish-to-pypi.yml`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: '3.x'
+        python-version: '3.10'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
     - name: Publish package
```

### Comparing `hipscat-import-0.0.3/.github/workflows/smoke-test.yml` & `hipscat-import-0.0.4/.github/workflows/smoke-test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # It will install Python dependencies and run tests with a variety of Python versions.
 
 name: Unit test smoke test
 
 on:
   schedule:
     - cron: 45 6 * * *
+  # Allows you to run this workflow manually from the Actions tab
+  workflow_dispatch:
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
```

### Comparing `hipscat-import-0.0.3/.github/workflows/testing-and-coverage.yml` & `hipscat-import-0.0.4/.github/workflows/testing-and-coverage.yml`

 * *Files 6% similar despite different names*

```diff
@@ -23,18 +23,14 @@
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         sudo apt-get update
         python -m pip install --upgrade pip
-        pip install .
-        pip install .[dev]
+        pip install -e .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Run unit tests with pytest
       run: |
         python -m pytest tests --cov=hipscat_import --cov-report=xml
     - name: Upload coverage report to codecov
       uses: codecov/codecov-action@v3
-    - name: Build docs
-      run: |
-        sphinx-build -T -E -b html -d docs/build/doctrees ./docs docs/build/html
```

### Comparing `hipscat-import-0.0.3/.github/workflows/type-checking.yml` & `hipscat-import-0.0.4/.github/workflows/type-checking.yml`

 * *Files 14% similar despite different names*

```diff
@@ -8,20 +8,24 @@
     branches: [ main ]
   pull_request:
     branches: [ main ]
 
 jobs:
   build:
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: ['3.8', '3.9', '3.10']
+
     steps:
     - uses: actions/checkout@v3
-    - name: Set up Python 3.10
+    - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
-        python-version: '3.10'
+        python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         sudo apt-get update
         python -m pip install --upgrade pip
         pip install .
         pip install .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
```

### Comparing `hipscat-import-0.0.3/.gitignore` & `hipscat-import-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.3/.pre-commit-config.yaml` & `hipscat-import-0.0.4/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -11,54 +11,54 @@
         description: Compare current template version against latest
         verbose: true
 
     # Clear output from jupyter notebooks so that only the input cells are committed.
   - repo: local
     hooks:
       - id: jupyter-nb-clear-output
-        name: jupyter-nb-clear-output
+        name: Clear output from Jupyter notebooks
         description: Clear output from Jupyter notebooks.
         files: \.ipynb$
         stages: [commit]
         language: system
-        entry: jupyter nbconvert --ClearOutputPreprocessor.enabled=True --inplace
+        entry: jupyter nbconvert --clear-output
 
     # Run unit tests, verify that they pass. Note that coverage is run against
     # the ./src directory here because that is what will be committed. In the 
     # github workflow script, the coverage is run against the installed package
     # and uploaded to Codecov by calling pytest like so:
     # `python -m pytest --cov=<package_name> --cov-report=xml`
   - repo: local
     hooks:
       - id: pytest-check
-        name: pytest-check
+        name: Run unit tests
         description: Run unit tests with pytest.
         entry: bash -c "if python -m pytest --co -qq; then python -m pytest --cov=./src --cov-report=html; fi"
         language: system
         pass_filenames: false
         always_run: true
 
     # prevents committing directly branches named 'main' and 'master'.
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: no-commit-to-branch
-        name: Don't commit to main or master branch
+        name: Prevent main branch commits
         description: Prevent the user from committing directly to the primary branch.
       - id: check-added-large-files
         name: Check for large files
         description: Prevent the user from committing very large files.
         args: ['--maxkb=500']
 
     # verify that pyproject.toml is well formed
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.12.1
     hooks:
       - id: validate-pyproject
-        name: Validate syntax of pyproject.toml
+        name: Validate pyproject.toml
         description: Verify that pyproject.toml adheres to the established schema.
 
     # Automatically sort the imports used in .py files
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
@@ -112,27 +112,33 @@
         args:
           [
           
             "--ignore-missing-imports", # Ignore imports without type hints
           
           ]
 
-    # Make sure Sphinx can build the documentation without issues.
+    # Make sure Sphinx can build the documentation while explicitly omitting 
+    # notebooks from the docs, so users don't have to wait through the execution 
+    # of each notebook or each commit. By default, these will be checked in the 
+    # GitHub workflows.
   - repo: local
     hooks:
       - id: sphinx-build
         name: Build documentation with Sphinx
         entry: sphinx-build
         language: system
         always_run: true
         exclude_types: [file, symlink]
         args:
           [
+            "-M", # Run sphinx in make mode, so we can use -D flag later
+                  # Note: -M requires next 3 args to be builder, source, output
+            "html", # Specify builder
+            "./docs", # Source directory of documents
+            "./_readthedocs", # Output directory for rendered documents
             "-T", # Show full trace back on exception
-            "-E", # Don't use saved env. always read all files.
-            "-b", # Flag to select which builder to use
-            "html", # Use the HTML builder
+            "-E", # Don't use saved env; always read all files
             "-d", # Flag for cached environment and doctrees
-            "docs/build/doctrees", # directory
-            "./docs", # Source directory of documents
-            "docs/build/html", # Output directory for rendered documents.
-          ]
+            "./docs/_build/doctrees", # Directory
+            "-D", # Flag to override settings in conf.py
+            "exclude_patterns=notebooks/*", # Exclude our notebooks from pre-commit
+          ]
```

### Comparing `hipscat-import-0.0.3/LICENSE` & `hipscat-import-0.0.4/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, Astronomy Data Commons
+Copyright (c) 2023, LINCC Frameworks
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
 
@@ -21,8 +21,8 @@
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `hipscat-import-0.0.3/PKG-INFO` & `hipscat-import-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: hipscat-import
-Version: 0.0.3
+Version: 0.0.4
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
-        Copyright (c) 2023, Astronomy Data Commons
+        Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
         
@@ -26,14 +26,15 @@
         DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -64,7 +65,13 @@
 
 ## Contributing
 
 [![GitHub issue custom search in repo](https://img.shields.io/github/issues-search/astronomy-commons/hipscat-import?color=purple&label=Good%20first%20issues&query=is%3Aopen%20label%3A%22good%20first%20issue%22)](https://github.com/astronomy-commons/hipscat-import/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
 
 See the [contribution guide](https://hipscat-import.readthedocs.io/en/latest/overview/contributing.html)
 for complete installation instructions and contribution best practices.
+
+## Acknowledgements
+
+LINCC Frameworks is supported by Schmidt Futures, a philanthropic initiative
+founded by Eric and Wendy Schmidt, as part of the Virtual Institute of 
+Astrophysics (VIA).
```

### Comparing `hipscat-import-0.0.3/README.md` & `hipscat-import-0.0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -22,7 +22,13 @@
 
 ## Contributing
 
 [![GitHub issue custom search in repo](https://img.shields.io/github/issues-search/astronomy-commons/hipscat-import?color=purple&label=Good%20first%20issues&query=is%3Aopen%20label%3A%22good%20first%20issue%22)](https://github.com/astronomy-commons/hipscat-import/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
 
 See the [contribution guide](https://hipscat-import.readthedocs.io/en/latest/overview/contributing.html)
 for complete installation instructions and contribution best practices.
+
+## Acknowledgements
+
+LINCC Frameworks is supported by Schmidt Futures, a philanthropic initiative
+founded by Eric and Wendy Schmidt, as part of the Virtual Institute of 
+Astrophysics (VIA).
```

### Comparing `hipscat-import-0.0.3/docs/Makefile` & `hipscat-import-0.0.4/docs/Makefile`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # Makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
 SPHINXOPTS    ?= -T -E -d _build/doctrees -D language=en
+EXCLUDENB     ?= -D exclude_patterns="notebooks/*","_build","**.ipynb_checkpoints"
 SPHINXBUILD   ?= sphinx-build
 SOURCEDIR     = .
 BUILDDIR      = ../_readthedocs/
 
-.PHONY: help clean Makefile 
+.PHONY: help clean Makefile no-nb no-notebooks
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
+# Build all Sphinx docs locally, except the notebooks
+no-nb no-notebooks:
+	@$(SPHINXBUILD) -M html "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(EXCLUDENB) $(O)
+
 # Cleans up files generated by the build process
 clean:
 	rm -r "_build/doctrees"
 	rm -r "$(BUILDDIR)"
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
```

### Comparing `hipscat-import-0.0.3/docs/catalogs/allwise.rst` & `hipscat-import-0.0.4/docs/catalogs/public/neowise.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-AllWISE
+NEOWISE
 ===============================================================================
 
 Getting the data
 -------------------------------------------------------------------------------
 
 See docs at IRSA.
 
-https://irsa.ipac.caltech.edu/data/download/wise-allwise/
+https://irsa.ipac.caltech.edu/data/download/neowiser_year8/
 
 Challenges with this data set
 -------------------------------------------------------------------------------
 
 - The individual files are large, and so we want to use a chunked CSV reader.
 - The rows are wide, so the chunked reader cannot read too many rows at once.
 - The CSV files don't have a header, so we need to provide the column names and
   type hints to the reader.
 - The numeric fields may be null, which is not directly supported by the 
   ``int64`` type in pandas, so we must use the nullable ``Int64`` type.
 
-You can download the :download:`allwise_types</static/allwise_types.csv>` CSV file we used.
+You can download the :download:`neowise_types</static/neowise_types.csv>` CSV file we used.
 
 Example import
 -------------------------------------------------------------------------------
 
 .. code-block:: python
 
     import pandas as pd
 
-    import hipscat_import.run_import as runner
-    from hipscat_import.arguments import ImportArguments
-    from hipscat_import.file_readers import CsvReader
+    import hipscat_import.pipeline as runner
+    from hipscat_import.catalog.arguments import ImportArguments
+    from hipscat_import.catalog.file_readers import CsvReader
 
     # Load the column names and types from a side file.
-    type_frame = pd.read_csv("allwise_types.csv")
+    type_frame = pd.read_csv("neowise_types.csv")
     type_map = dict(zip(type_frame["name"], type_frame["type"]))
 
     args = ImportArguments(
-        catalog_name="allwise",
-        input_path="/path/to/allwise/",
+        output_catalog_name="neowise_1",
+        input_path="/path/to/neowiser_year8/",
         input_format="csv.bz2",
         file_reader=CsvReader(
             header=None,
             separator="|",
             column_names=type_frame["name"].values.tolist(),
             type_map=type_map,
             chunksize=250_000,
```

### Comparing `hipscat-import-0.0.3/docs/catalogs/neowise.rst` & `hipscat-import-0.0.4/docs/catalogs/public/allwise.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,59 @@
-NEOWISE
+AllWISE
 ===============================================================================
 
 Getting the data
 -------------------------------------------------------------------------------
 
 See docs at IRSA.
 
-https://irsa.ipac.caltech.edu/data/download/neowiser_year8/
+https://irsa.ipac.caltech.edu/data/download/wise-allwise/
 
 Challenges with this data set
 -------------------------------------------------------------------------------
 
 - The individual files are large, and so we want to use a chunked CSV reader.
 - The rows are wide, so the chunked reader cannot read too many rows at once.
 - The CSV files don't have a header, so we need to provide the column names and
   type hints to the reader.
 - The numeric fields may be null, which is not directly supported by the 
   ``int64`` type in pandas, so we must use the nullable ``Int64`` type.
 
-You can download the :download:`neowise_types</static/neowise_types.csv>` CSV file we used.
+You can download the :download:`allwise_types</static/allwise_types.csv>` CSV file we used,
+and the associated schema file :download:`allwise_schema</static/allwise_schema.parquet>`
+with column-level parquet metadata.
 
 Example import
 -------------------------------------------------------------------------------
 
 .. code-block:: python
 
     import pandas as pd
 
-    import hipscat_import.run_import as runner
-    from hipscat_import.arguments import ImportArguments
-    from hipscat_import.file_readers import CsvReader
+    import hipscat_import.pipeline as runner
+    from hipscat_import.catalog.arguments import ImportArguments
+    from hipscat_import.catalog.file_readers import CsvReader
 
     # Load the column names and types from a side file.
-    type_frame = pd.read_csv("neowise_types.csv")
+    type_frame = pd.read_csv("allwise_types.csv")
     type_map = dict(zip(type_frame["name"], type_frame["type"]))
 
     args = ImportArguments(
-        catalog_name="neowise_1",
-        input_path="/path/to/neowiser_year8/",
+        output_catalog_name="allwise",
+        input_path="/path/to/allwise/",
         input_format="csv.bz2",
         file_reader=CsvReader(
             header=None,
             separator="|",
             column_names=type_frame["name"].values.tolist(),
             type_map=type_map,
             chunksize=250_000,
-        ).read,
-        ra_column="RA",
-        dec_column="DEC",
-        id_column="SOURCE_ID",
+        ),
+        use_schema_file="allwise_schema.parquet",
+        ra_column="ra",
+        dec_column="dec",
+        id_column="source_id",
+        pixel_threshold=1_000_000,
+        highest_healpix_order=7,
         output_path="/path/to/catalogs/",
     )
-    runner.run(args)
+    runner.pipeline(args)
```

### Comparing `hipscat-import-0.0.3/docs/catalogs/tic.rst` & `hipscat-import-0.0.4/docs/catalogs/public/tic.rst`

 * *Files 8% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 Example import
 -------------------------------------------------------------------------------
 
 .. code-block:: python
 
     import pandas as pd
 
-    import hipscat_import.run_import as runner
-    from hipscat_import.arguments import ImportArguments
-    from hipscat_import.file_readers import CsvReader
+    import hipscat_import.pipeline as runner
+    from hipscat_import.catalog.arguments import ImportArguments
+    from hipscat_import.catalog.file_readers import CsvReader
 
     type_frame = pd.read_csv("tic_types.csv")
     type_map = dict(zip(type_frame["name"], type_frame["type"]))
     
     args = ImportArguments(
-        catalog_name="tic_1",
+        output_catalog_name="tic_1",
         input_path="/path/to/tic/",
         input_format="csv.gz",
         file_reader=CsvReader(
             header=None,
             column_names=type_frame["name"].values.tolist(),
             type_map=type_map,
             chunksize=250_000,
```

### Comparing `hipscat-import-0.0.3/docs/conf.py` & `hipscat-import-0.0.4/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ["sphinx.ext.mathjax", "sphinx.ext.napoleon", "sphinx.ext.viewcode"]
 
 extensions.append("autoapi.extension")
+extensions.append("nbsphinx")
 
 templates_path = []
 exclude_patterns = ["_build", "**.ipynb_checkpoints"]
 
 master_doc = "index"  # This assumes that sphinx-build is called from the root directory
 html_show_sourcelink = (
     False  # Remove 'view source code' from top of page (for html, not python)
```

### Comparing `hipscat-import-0.0.3/docs/guide/contributing.rst` & `hipscat-import-0.0.4/docs/guide/contributing.rst`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 
 If there isn't an issue for the work you want to do, please create one and include
 a description.
 
 You can reach the team with bug reports, feature requests, and general inquiries
 by creating a new GitHub issue.
 
+.. tip::
+   Want to help?
+
+   Do you want to help out, but you're not sure how? :doc:`/guide/contact`
+
 Create a branch
 -------------------------------------------------------------------------------
 
 It is preferable that you create a new branch with a name like 
 ``issue/##/<short-description>``. GitHub makes it pretty easy to associate 
 branches and tickets, but it's nice when it's in the name.
 
@@ -28,17 +33,30 @@
 .. code-block:: bash
 
     $ git clone https://github.com/astronomy-commons/hipscat-import
     $ cd hipscat-import
     $ pip install -e .
 
 .. tip::
-    Installing dev dependencies on Mac
+    Installing on Mac
+
+    ``healpy`` is a very necessary dependency for hipscat libraries at this time, but
+    native prebuilt binaries for healpy on Apple Silicon Macs 
+    `do not yet exist <https://healpy.readthedocs.io/en/latest/install.html#binary-installation-with-pip-recommended-for-most-other-python-users>`_, 
+    so it's recommended to install via conda before proceeding to hipscat-import.
 
-    (Make sure to include the single quotes)
+    .. code-block:: bash
+
+        $ conda config --add channels conda-forge
+        $ conda install healpy
+        $ git clone https://github.com/astronomy-commons/hipscat-import
+        $ cd hipscat-import
+        $ pip install -e .
+        
+    When installing dev dependencies, make sure to include the single quotes.
 
     .. code-block:: bash
         
         $ pip install -e '.[dev]'
 
 Testing
 -------------------------------------------------------------------------------
```

### Comparing `hipscat-import-0.0.3/docs/guide/resume.rst` & `hipscat-import-0.0.4/docs/catalogs/resume.rst`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.3/docs/static/allwise_types.csv` & `hipscat-import-0.0.4/docs/static/allwise_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.3/docs/static/neowise_types.csv` & `hipscat-import-0.0.4/docs/static/neowise_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.3/docs/static/tic_types.csv` & `hipscat-import-0.0.4/docs/static/tic_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.3/src/.pylintrc` & `hipscat-import-0.0.4/src/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
 # Maximum number of attributes for a class (see R0902).
 max-attributes=7
 
 # Maximum number of boolean expressions in an if statement (see R0916).
 max-bool-expr=5
 
 # Maximum number of branch for function / method body.
-max-branches=12
+max-branches=15
 
 # Maximum number of locals for function / method body.
 max-locals=15
 
 # Maximum number of parents for a class (see R0901).
 max-parents=7
 
@@ -328,15 +328,15 @@
 # tab).
 indent-string='    '
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module.
-max-module-lines=1000
+max-module-lines=500
 
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
@@ -439,16 +439,15 @@
 timeout-methods=requests.api.delete,requests.api.get,requests.api.head,requests.api.options,requests.api.patch,requests.api.post,requests.api.put,requests.api.request
 
 
 [MISCELLANEOUS]
 
 # List of note tags to take in consideration, separated by a comma.
 notes=FIXME,
-      XXX,
-      TODO
+      XXX
 
 # Regular expression of note tags to take in consideration.
 notes-rgx=
 
 
 [REFACTORING]
```

### Comparing `hipscat-import-0.0.3/src/hipscat_import/__init__.py` & `hipscat-import-0.0.4/src/hipscat_import/catalog/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-"""All modules for hipscat-import package"""
+"""All modules for importing new catalogs."""
 
 from .arguments import ImportArguments
-from .command_line_arguments import parse_command_line
-from .control import main
 from .file_readers import (
     CsvReader,
     FitsReader,
     InputReader,
     ParquetReader,
     get_file_reader,
 )
-from .map_reduce import map_to_pixels, reduce_pixel_shards
+from .map_reduce import map_to_pixels, reduce_pixel_shards, split_pixels
 from .resume_files import (
     clean_resume_files,
     is_mapping_done,
     is_reducing_done,
     read_histogram,
     read_mapping_keys,
     read_reducing_keys,
     set_mapping_done,
     set_reducing_done,
     write_histogram,
     write_mapping_done_key,
     write_mapping_start_key,
     write_reducing_key,
 )
-from .run_import import run, run_with_client
+from .run_import import run
```

### Comparing `hipscat-import-0.0.3/src/hipscat_import/arguments.py` & `hipscat-import-0.0.4/tests/hipscat_import/catalog/test_run_round_trip.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,295 +1,365 @@
-"""Utility to hold all arguments required throughout partitioning"""
+"""Test end-to-end execution of pipeline with different formats and configurations.
 
-from importlib.metadata import version
+Please add a brief description in the docstring of the features or specific 
+regression the test case is exercising.
+"""
 
-import pandas as pd
-from hipscat.catalog import CatalogParameters
-from hipscat.io import file_io
 
-from hipscat_import.file_readers import get_file_reader
+import os
 
-# pylint: disable=too-many-locals,too-many-arguments,too-many-instance-attributes,too-many-branches,too-few-public-methods
+import numpy as np
+import numpy.testing as npt
+import pandas as pd
+import pytest
+from hipscat.catalog.catalog import Catalog
 
+import hipscat_import.catalog.run_import as runner
+from hipscat_import.catalog.arguments import ImportArguments
+from hipscat_import.catalog.file_readers import CsvReader, get_file_reader
+
+
+@pytest.mark.dask
+def test_import_source_table(
+    dask_client,
+    small_sky_source_dir,
+    tmp_path,
+):
+    """Test basic execution, using a larger source file.
+    - catalog type should be source
+    - will have larger partition info than the corresponding object catalog
+    """
+    args = ImportArguments(
+        output_catalog_name="small_sky_source_catalog",
+        input_path=small_sky_source_dir,
+        input_format="csv",
+        catalog_type="source",
+        ra_column="source_ra",
+        dec_column="source_dec",
+        id_column="source_id",
+        output_path=tmp_path,
+        dask_tmp=tmp_path,
+        highest_healpix_order=2,
+        pixel_threshold=3_000,
+        overwrite=True,
+        progress_bar=False,
+    )
+
+    runner.run(args, dask_client)
+
+    # Check that the catalog metadata file exists
+    catalog = Catalog.read_from_hipscat(args.catalog_path)
+    assert catalog.on_disk
+    assert catalog.catalog_path == args.catalog_path
+    assert catalog.catalog_info.ra_column == "source_ra"
+    assert catalog.catalog_info.dec_column == "source_dec"
+    assert len(catalog.get_pixels()) == 14
+
+
+@pytest.mark.dask
+def test_import_mixed_schema_csv(
+    dask_client,
+    mixed_schema_csv_dir,
+    mixed_schema_csv_parquet,
+    assert_parquet_file_ids,
+    tmp_path,
+):
+    """Test basic execution, with a mixed schema.
+    - the two input file in `mixed_schema_csv_dir` have different *implied* schemas
+        when parsed by pandas. this verifies that they end up with the same schema
+        and can be combined into a single parquet file.
+    """
 
-class ImportArguments:
-    """Container class for holding partitioning arguments
-    
-    
-    Attributes:
-        catalog_name (str): short, convenient name for the catalog.
-        epoch (str): astronomical epoch for the data. defaults to "J2000"
-        `_input_path` (str): path to the input data
-        input_format (str): specifier of the input data format. This will
-            be used to find an appropriate file reader, and may be used to find
-            input files, via a match like "<input_path>/*<input_format>"
-        `_input_file_list` (list[str]): can be used instead of `input_format` to
-            import just a few files at a time.
-        input_paths (list[str]): resolved list of all files used in the importer
-        ra_column (str): column for right ascension
-        dec_column (str): column for declination
-        id_column (str): column for survey identifier, or other sortable column
-        `_output_path` (str): base path for catalog output
-        catalog_path (str): path for catalog output. This is generally formed
-            via <output_path>/<catalog_name>
-        overwrite (bool): if there is existing data at the `catalog_path`, should
-            we overwrite and create a new catalog.
-        resume (bool): if there are existing intermediate resume files, should we
-            read those and continue to create a new catalog where we left off.
-        highest_healpix_order (int): healpix order to use when mapping. this will
-            not necessarily be the order used in the final catalog, as we may combine
-            pixels that don't meed the threshold.
-        pixel_threshold (int): maximum number of rows for a single resulting pixel.
-            we may combine hierarchically until we near the `pixel_threshold`
-        debug_stats_only (bool): do not perform a map reduce and don't create a new
-            catalog. generate the partition info.
-        tmp_path (str): path for storing intermediate files
-        filter_function (function pointer): optional method which takes a pandas
-            dataframe as input, performs some filtering or transformation of the data,
-            and returns a dataframe with the rows that will be used to create the
-            new catalog.
-        file_reader (`InputReader`): instance of input reader that specifies arguments
-            necessary for reading from your input files.
-        `_tmp_dir` (str): base directory provided by the caller for temporary files.
-        progress_bar (bool): if true, a tqdm progress bar will be displayed for user
-            feedback of map reduce progress.
-        dask_tmp (str): directory for dask worker space. this should be local to
-            the execution of the pipeline, for speed of reads and writes.
-        dask_n_workers (int): number of workers for the dask client
-        dask_threads_per_worker (int): number of threads per dask worker.
+    schema_parquet = pd.read_parquet(mixed_schema_csv_parquet)
+    args = ImportArguments(
+        output_catalog_name="mixed_csv",
+        input_path=mixed_schema_csv_dir,
+        input_format="csv",
+        output_path=tmp_path,
+        dask_tmp=tmp_path,
+        highest_healpix_order=1,
+        file_reader=get_file_reader(
+            "csv", chunksize=1, type_map=schema_parquet.dtypes.to_dict()
+        ),
+        progress_bar=False,
+        use_schema_file=mixed_schema_csv_parquet,
+    )
+
+    runner.run(args, dask_client)
+
+    # Check that the catalog parquet file exists
+    output_file = os.path.join(
+        args.catalog_path, "Norder=0", "Dir=0", "Npix=11.parquet"
+    )
+
+    assert_parquet_file_ids(output_file, "id", [*range(700, 708)])
+
+
+@pytest.mark.dask
+def test_import_preserve_index(
+    dask_client,
+    formats_pandasindex,
+    assert_parquet_file_ids,
+    assert_parquet_file_index,
+    tmp_path,
+):
+    """Test basic execution, with input with pandas metadata.
+    - the input file is a parquet file with some pandas metadata.
+        this verifies that the parquet file at the end also has pandas
+        metadata, and the user's preferred id is retained as the index,
+        when requested.
     """
 
-    def __init__(
-        self,
-        catalog_name="",
-        epoch="J2000",
-        input_path="",
+    expected_indexes = [
+        "star1_1",
+        "star1_2",
+        "star1_3",
+        "star1_4",
+        "galaxy1_1",
+        "galaxy1_2",
+        "galaxy2_1",
+        "galaxy2_2",
+    ]
+    assert_parquet_file_index(formats_pandasindex, expected_indexes)
+    data_frame = pd.read_parquet(formats_pandasindex, engine="pyarrow")
+    assert data_frame.index.name == "obs_id"
+    npt.assert_array_equal(
+        data_frame.columns,
+        ["obj_id", "band", "ra", "dec", "mag"],
+    )
+
+    ## Don't generate a hipscat index. Verify that the original index remains.
+    args = ImportArguments(
+        output_catalog_name="pandasindex",
+        input_file_list=[formats_pandasindex],
         input_format="parquet",
-        input_file_list=None,
-        ra_column="ra",
-        dec_column="dec",
-        id_column="id",
+        id_column="obs_id",
+        add_hipscat_index=False,
+        output_path=tmp_path,
+        dask_tmp=tmp_path,
+        highest_healpix_order=1,
+        progress_bar=False,
+    )
+
+    runner.run(args, dask_client)
+
+    # Check that the catalog parquet file exists
+    output_file = os.path.join(
+        args.catalog_path, "Norder=0", "Dir=0", "Npix=11.parquet"
+    )
+
+    assert_parquet_file_index(output_file, expected_indexes)
+    data_frame = pd.read_parquet(output_file, engine="pyarrow")
+    assert data_frame.index.name == "obs_id"
+    npt.assert_array_equal(
+        data_frame.columns,
+        ["obj_id", "band", "ra", "dec", "mag", "Norder", "Dir", "Npix"],
+    )
+
+    ## DO generate a hipscat index. Verify that the original index is preserved in a column.
+    args = ImportArguments(
+        output_catalog_name="pandasindex_preserve",
+        input_file_list=[formats_pandasindex],
+        input_format="parquet",
+        id_column="obs_id",
         add_hipscat_index=True,
-        output_path="",
-        overwrite=False,
-        resume=False,
-        highest_healpix_order=10,
-        pixel_threshold=1_000_000,
-        debug_stats_only=False,
-        filter_function=None,
-        file_reader=None,
-        tmp_dir="",
-        progress_bar=True,
-        dask_tmp="",
-        dask_n_workers=1,
-        dask_threads_per_worker=1,
-    ):
-        self.catalog_name = catalog_name
-        self.epoch = epoch
-        self._input_path = file_io.get_file_pointer_from_path(input_path)
-        self.input_format = input_format
-        self._input_file_list = (
-            [file_io.get_file_pointer_from_path(x) for x in input_file_list]
-            if input_file_list
-            else None
-        )
-        self.input_paths = []
-
-        self.ra_column = ra_column
-        self.dec_column = dec_column
-        self.id_column = id_column
-        self.add_hipscat_index = add_hipscat_index
-
-        self._output_path = file_io.get_file_pointer_from_path(output_path)
-        self.overwrite = overwrite
-        self.resume = resume
-        self.highest_healpix_order = highest_healpix_order
-        self.pixel_threshold = pixel_threshold
-        self.debug_stats_only = debug_stats_only
-        self.catalog_path = ""
-        self.tmp_path = ""
-
-        self.filter_function = (
-            filter_function if filter_function else passthrough_filter_function
-        )
-        self.file_reader = (
-            file_reader if file_reader else get_file_reader(self.input_format)
-        )
-
-        self._tmp_dir = file_io.get_file_pointer_from_path(tmp_dir)
-        self.progress_bar = progress_bar
-        self.dask_tmp = file_io.get_file_pointer_from_path(dask_tmp)
-        self.dask_n_workers = dask_n_workers
-        self.dask_threads_per_worker = dask_threads_per_worker
-
-        self._check_arguments()
-        self._check_paths()
-
-    def _check_arguments(self):
-        """Check existence and consistency of argument values"""
-        if not self.catalog_name:
-            raise ValueError("catalog_name is required")
-        if not self.input_format:
-            raise ValueError("input_format is required")
-        if not self._output_path:
-            raise ValueError("output_path is required")
-
-        if not 0 <= self.highest_healpix_order <= 10:
-            raise ValueError("highest_healpix_order should be between 0 and 10")
-        if not 100 <= self.pixel_threshold <= 1_000_000:
-            raise ValueError("pixel_threshold should be between 100 and 1,000,000")
-
-        if self.dask_n_workers <= 0:
-            raise ValueError("dask_n_workers should be greather than 0")
-        if self.dask_threads_per_worker <= 0:
-            raise ValueError("dask_threads_per_worker should be greather than 0")
-
-    def _check_paths(self):
-        """Check existence and permissions on provided path arguments"""
-        if (not self._input_path and not self._input_file_list) or (
-            self._input_path and self._input_file_list
-        ):
-            raise ValueError("exactly one of input_path or input_file_list is required")
-
-        if not file_io.does_file_or_directory_exist(self._output_path):
-            raise FileNotFoundError(
-                f"output_path ({self._output_path}) not found on local storage"
-            )
-
-        # Catalog path should not already exist, unless we're overwriting. Create it.
-        self.catalog_path = file_io.append_paths_to_pointer(
-            self._output_path, self.catalog_name
-        )
-        if not self.overwrite:
-            if file_io.directory_has_contents(self.catalog_path):
-                raise ValueError(
-                    f"output_path ({self.catalog_path}) contains files."
-                    " choose a different directory or use --overwrite flag"
-                )
-        file_io.make_directory(self.catalog_path, exist_ok=True)
-
-        # Basic checks complete - make more checks and create directories where necessary
-        if self._input_path:
-            if not file_io.does_file_or_directory_exist(self._input_path):
-                raise FileNotFoundError("input_path not found on local storage")
-            self.input_paths = file_io.find_files_matching_path(
-                self._input_path, f"*{self.input_format}"
-            )
-
-            if len(self.input_paths) == 0:
-                raise FileNotFoundError(
-                    f"No files matched file pattern: {self._input_path}*{self.input_format} "
-                )
-        elif self._input_file_list:
-            self.input_paths = self._input_file_list
-            for test_path in self.input_paths:
-                if not file_io.does_file_or_directory_exist(test_path):
-                    raise FileNotFoundError(f"{test_path} not found on local storage")
-        if not self.input_paths:
-            raise FileNotFoundError("No input files found")
-        self.input_paths.sort()
-
-        if self._tmp_dir:
-            self.tmp_path = file_io.append_paths_to_pointer(
-                self._tmp_dir, self.catalog_name, "intermediate"
-            )
-        elif self.dask_tmp:
-            self.tmp_path = file_io.append_paths_to_pointer(
-                self.dask_tmp, self.catalog_name, "intermediate"
-            )
-        else:
-            self.tmp_path = file_io.append_paths_to_pointer(
-                self.catalog_path, "intermediate"
-            )
-        if not self.resume:
-            if file_io.directory_has_contents(self.tmp_path):
-                raise ValueError(
-                    f"tmp_path ({self.tmp_path}) contains intermediate files."
-                    " choose a different directory or use --resume flag"
-                )
-        file_io.make_directory(self.tmp_path, exist_ok=True)
-
-    def to_catalog_parameters(self) -> CatalogParameters:
-        """Convert importing arguments into hipscat catalog parameters.
-
-        Returns:
-            CatalogParameters for catalog being created.
-        """
-        return CatalogParameters(
-            catalog_name=self.catalog_name,
-            input_paths=self.input_paths,
-            input_format=self.input_format,
-            output_path=self._output_path,
-            highest_healpix_order=self.highest_healpix_order,
-            pixel_threshold=self.pixel_threshold,
-            epoch=self.epoch,
-            ra_column=self.ra_column,
-            dec_column=self.dec_column,
-        )
-
-    def provenance_info(self) -> dict:
-        """Fill all known information in a dictionary for provenance tracking.
-
-        Returns:
-            dictionary with all argument_name -> argument_value as key -> value pairs.
-        """
-        runtime_args = {
-            "catalog_name": self.catalog_name,
-            "epoch": self.epoch,
-            "input_path": str(self._input_path),
-            "input_paths": self.input_paths,
-            "input_format": self.input_format,
-            "input_file_list": self._input_file_list,
-            "ra_column": self.ra_column,
-            "dec_column": self.dec_column,
-            "id_column": self.id_column,
-            "output_path": str(self._output_path),
-            "overwrite": self.overwrite,
-            "resume": self.resume,
-            "highest_healpix_order": self.highest_healpix_order,
-            "pixel_threshold": self.pixel_threshold,
-            "debug_stats_only": self.debug_stats_only,
-            "catalog_path": self.catalog_path,
-            "tmp_path": str(self.tmp_path),
-            "progress_bar": self.progress_bar,
-            "dask_tmp": str(self.dask_tmp),
-            "dask_n_workers": self.dask_n_workers,
-            "dask_threads_per_worker": self.dask_threads_per_worker,
-            "file_reader_info": self.file_reader.provenance_info(),
-        }
-        runtime_args["uses_filter_function"] = (
-            self.filter_function != passthrough_filter_function
-        )
-        provenance_info = {
-            "tool_name": "hipscat_import",
-            "version": version("hipscat-import"),
-            "runtime_args": runtime_args,
-        }
-
-        return provenance_info
-
-    def __str__(self):
-        formatted_string = (
-            f"  catalog_name {self.catalog_name}\n"
-            f"  input_path {self._input_path}\n"
-            f"  input format {self.input_format}\n"
-            f"  num input_paths {len(self.input_paths)}\n"
-            f"  ra_column {self.ra_column}\n"
-            f"  dec_column {self.dec_column}\n"
-            f"  id_column {self.id_column}\n"
-            f"  output_path {self._output_path}\n"
-            f"  overwrite {self.overwrite}\n"
-            f"  highest_healpix_order {self.highest_healpix_order}\n"
-            f"  pixel_threshold {self.pixel_threshold}\n"
-            f"  debug_stats_only {self.debug_stats_only}\n"
-            f"  progress_bar {self.progress_bar}\n"
-            f"  dask_tmp {self.dask_tmp}\n"
-            f"  dask_n_workers {self.dask_n_workers}\n"
-            f"  dask_threads_per_worker {self.dask_threads_per_worker}\n"
-            f"  tmp_path {self.tmp_path}\n"
-        )
-        return formatted_string
-
-
-def passthrough_filter_function(data: pd.DataFrame) -> pd.DataFrame:
-    """No-op filter function to be used when no user-defined filter is provided"""
-    return data
+        output_path=tmp_path,
+        dask_tmp=tmp_path,
+        highest_healpix_order=1,
+        progress_bar=False,
+    )
+
+    runner.run(args, dask_client)
+
+    # Check that the catalog parquet file exists
+    output_file = os.path.join(
+        args.catalog_path, "Norder=0", "Dir=0", "Npix=11.parquet"
+    )
+
+    data_frame = pd.read_parquet(output_file, engine="pyarrow")
+    assert data_frame.index.name == "_hipscat_index"
+    npt.assert_array_equal(
+        data_frame.columns,
+        ["obs_id", "obj_id", "band", "ra", "dec", "mag", "Norder", "Dir", "Npix"],
+    )
+    assert_parquet_file_ids(output_file, "obs_id", expected_indexes)
+
+
+@pytest.mark.dask
+def test_import_multiindex(
+    dask_client,
+    formats_multiindex,
+    assert_parquet_file_ids,
+    assert_parquet_file_index,
+    tmp_path,
+):
+    """Test basic execution, with input with pandas metadata
+    - this is *similar* to the above test
+    - the input file is a parquet file with a multi-level pandas index.
+        this verifies that the parquet file at the end also has pandas
+        metadata, and the user's preferred id is retained as the index,
+        when requested.
+    """
+
+    index_arrays = [
+        [
+            "star1",
+            "star1",
+            "star1",
+            "star1",
+            "galaxy1",
+            "galaxy1",
+            "galaxy2",
+            "galaxy2",
+        ],
+        ["r", "r", "i", "i", "r", "r", "r", "r"],
+    ]
+    expected_indexes = list(zip(index_arrays[0], index_arrays[1]))
+    assert_parquet_file_index(formats_multiindex, expected_indexes)
+    data_frame = pd.read_parquet(formats_multiindex, engine="pyarrow")
+    assert data_frame.index.names == ["obj_id", "band"]
+    npt.assert_array_equal(
+        data_frame.columns,
+        ["ra", "dec", "mag"],
+    )
+
+    ## Don't generate a hipscat index. Verify that the original index remains.
+    args = ImportArguments(
+        output_catalog_name="multiindex",
+        input_file_list=[formats_multiindex],
+        input_format="parquet",
+        id_column=["obj_id", "band"],
+        add_hipscat_index=False,
+        output_path=tmp_path,
+        dask_tmp=tmp_path,
+        highest_healpix_order=1,
+        progress_bar=False,
+    )
+
+    runner.run(args, dask_client)
+
+    # Check that the catalog parquet file exists
+    output_file = os.path.join(
+        args.catalog_path, "Norder=0", "Dir=0", "Npix=11.parquet"
+    )
+
+    assert_parquet_file_index(output_file, expected_indexes)
+    data_frame = pd.read_parquet(output_file, engine="pyarrow")
+    assert data_frame.index.names == ["obj_id", "band"]
+    npt.assert_array_equal(
+        data_frame.columns,
+        ["ra", "dec", "mag", "Norder", "Dir", "Npix"],
+    )
+
+    ## DO generate a hipscat index. Verify that the original index is preserved in a column.
+    args = ImportArguments(
+        output_catalog_name="multiindex_preserve",
+        input_file_list=[formats_multiindex],
+        input_format="parquet",
+        id_column=["obj_id", "band"],
+        add_hipscat_index=True,
+        output_path=tmp_path,
+        dask_tmp=tmp_path,
+        highest_healpix_order=1,
+        progress_bar=False,
+    )
+
+    runner.run(args, dask_client)
+
+    # Check that the catalog parquet file exists
+    output_file = os.path.join(
+        args.catalog_path, "Norder=0", "Dir=0", "Npix=11.parquet"
+    )
+
+    data_frame = pd.read_parquet(output_file, engine="pyarrow")
+    assert data_frame.index.name == "_hipscat_index"
+    npt.assert_array_equal(
+        data_frame.columns,
+        ["obj_id", "band", "ra", "dec", "mag", "Norder", "Dir", "Npix"],
+    )
+    assert_parquet_file_ids(output_file, "obj_id", index_arrays[0])
+
+
+@pytest.mark.dask
+def test_import_constant_healpix_order(
+    dask_client,
+    small_sky_parts_dir,
+    tmp_path,
+):
+    """Test basic execution.
+    - tests that all the final tiles are at the same healpix order,
+        and that we don't create tiles where there is no data.
+    """
+    args = ImportArguments(
+        output_catalog_name="small_sky_object_catalog",
+        input_path=small_sky_parts_dir,
+        input_format="csv",
+        output_path=tmp_path,
+        dask_tmp=tmp_path,
+        constant_healpix_order=2,
+        progress_bar=False,
+    )
+
+    runner.run(args, dask_client)
+
+    # Check that the catalog metadata file exists
+    catalog = Catalog.read_from_hipscat(args.catalog_path)
+    assert catalog.on_disk
+    assert catalog.catalog_path == args.catalog_path
+    # Check that the partition info file exists - all pixels at order 2!
+    assert all(
+        pixel.order == 2 for pixel in catalog.partition_info.get_healpix_pixels()
+    )
+
+    # Pick a parquet file and make sure it contains as many rows as we expect
+    output_file = os.path.join(
+        args.catalog_path, "Norder=2", "Dir=0", "Npix=178.parquet"
+    )
+
+    data_frame = pd.read_parquet(output_file, engine="pyarrow")
+    assert len(data_frame) == 14
+    ids = data_frame["id"]
+    assert np.logical_and(ids >= 700, ids < 832).all()
+
+@pytest.mark.dask
+def test_import_starr_file(
+    dask_client,
+    formats_dir,
+    assert_parquet_file_ids,
+    tmp_path,
+):
+    """Test basic execution.
+    - tests that we can run pipeline with a totally unknown file type, so long
+      as a valid InputReader implementation is provided.
+    """
+
+    class StarrReader(CsvReader):
+        """Shallow subclass"""
+
+    args = ImportArguments(
+        output_catalog_name="starr",
+        input_path=formats_dir,
+        input_format="starr",
+        file_reader=StarrReader(),
+        output_path=tmp_path,
+        dask_tmp=tmp_path,
+        highest_healpix_order=2,
+        pixel_threshold=3_000,
+        progress_bar=False,
+    )
+
+    runner.run(args, dask_client)
+
+    # Check that the catalog metadata file exists
+    catalog = Catalog.read_from_hipscat(args.catalog_path)
+    assert catalog.on_disk
+    assert catalog.catalog_path == args.catalog_path
+    assert catalog.catalog_info.total_rows == 131
+    assert len(catalog.get_pixels()) == 1
+
+    # Check that the catalog parquet file exists and contains correct object IDs
+    output_file = os.path.join(
+        args.catalog_path, "Norder=0", "Dir=0", "Npix=11.parquet"
+    )
+
+    expected_ids = [*range(700, 831)]
+    assert_parquet_file_ids(output_file, "id", expected_ids)
```

### Comparing `hipscat-import-0.0.3/src/hipscat_import/file_readers.py` & `hipscat-import-0.0.4/src/hipscat_import/catalog/file_readers.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,67 +15,70 @@
     chunksize=500_000,
     header="infer",
     schema_file=None,
     column_names=None,
     skip_column_names=None,
     type_map=None,
     separator=",",
+    **kwargs,
 ):
     """Get a generator file reader for common file types
-    
+
     Args:
         file_format (str): specifier for the file type and extension.
-            Currently supported formats include: 
+            Currently supported formats include:
 
             - `csv`, comma separated values. may also be tab- or pipe-delimited
-                    includes `.csv.gz` and other compressed csv files
+              includes `.csv.gz` and other compressed csv files
             - `fits`, flexible image transport system. often used for astropy tables.
             - `parquet`, compressed columnar data format
 
         chunksize (int): number of rows to read in a single iteration.
         header (int, list of int, None, default 'infer'): for CSV files, rows to
             use as the header with column names
         schema_file (str): path to a parquet schema file. if provided, header names
             and column types will be pulled from the parquet schema metadata.
         column_names (list[str]): for CSV files, the names of columns if no header
             is available. for fits files, a list of columns to *keep*.
         skip_column_names (list[str]): for fits files, a list of columns to remove.
         type_map (dict): for CSV files, the data types to use for columns
-        separator (str): for CSV files, the character used for separation. 
+        separator (str): for CSV files, the character used for separation.
     """
     if "csv" in file_format:
         return CsvReader(
             chunksize=chunksize,
             header=header,
             schema_file=schema_file,
             column_names=column_names,
             type_map=type_map,
             separator=separator,
+            **kwargs,
         )
     if file_format == "fits":
         return FitsReader(
             chunksize=chunksize,
             column_names=column_names,
             skip_column_names=skip_column_names,
+            **kwargs,
         )
     if file_format == "parquet":
-        return ParquetReader(chunksize=chunksize)
+        return ParquetReader(chunksize=chunksize, **kwargs)
 
     raise NotImplementedError(f"File Format: {file_format} not supported")
 
 
 class InputReader(abc.ABC):
     """Base class for chunking file readers."""
 
     @abc.abstractmethod
     def read(self, input_file):
         """Read the input file, or chunk of the input file.
 
         Args:
-            input_file(str) path to the input file.
+            input_file(str): path to the input file.
         Yields:
             DataFrame containing chunk of file info.
         """
 
     @abc.abstractmethod
     def provenance_info(self) -> dict:
         """Create dictionary of parameters for provenance tracking.
@@ -84,49 +87,52 @@
             dictionary with all argument_name -> argument_value as key -> value pairs.
         """
 
 
 class CsvReader(InputReader):
     """CSV reader for the most common CSV reading arguments.
 
-    This uses `pandas.read_csv`, and you can find more information on 
+    This uses `pandas.read_csv`, and you can find more information on
     additional arguments in the pandas documentation:
     https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html
-    
+
     Attributes:
         chunksize (int): number of rows to read in a single iteration.
         header (int, list of int, None, default 'infer'): rows to
             use as the header with column names
         schema_file (str): path to a parquet schema file. if provided, header names
             and column types will be pulled from the parquet schema metadata.
         column_names (list[str]): the names of columns if no header is available
         type_map (dict): the data types to use for columns
-        separator (str): the character used for separation. 
+        separator (str): the character used for separation.
     """
 
     def __init__(
         self,
         chunksize=500_000,
         header="infer",
         schema_file=None,
         column_names=None,
         type_map=None,
         separator=",",
+        **kwargs,
     ):
         self.chunksize = chunksize
         self.header = header
         self.schema_file = schema_file
         self.column_names = column_names
         self.type_map = type_map
         self.separator = separator
+        self.kwargs = kwargs
 
     def read(self, input_file):
-        """Read CSV using chunked file reader"""
         if self.schema_file:
-            schema_parquet = pd.read_parquet(self.schema_file, use_nullable_dtypes=True)
+            schema_parquet = pd.read_parquet(
+                self.schema_file, dtype_backend="numpy_nullable"
+            )
 
         use_column_names = None
         if self.column_names:
             use_column_names = self.column_names
         elif not self.header and self.schema_file:
             use_column_names = schema_parquet.columns
 
@@ -139,14 +145,15 @@
         with pd.read_csv(
             input_file,
             chunksize=self.chunksize,
             sep=self.separator,
             header=self.header,
             names=use_column_names,
             dtype=use_type_map,
+            **self.kwargs,
         ) as reader:
             for chunk in reader:
                 yield chunk
 
     def provenance_info(self) -> dict:
         str_type_map = {}
         if self.type_map:
@@ -164,48 +171,46 @@
 
 
 class FitsReader(InputReader):
     """Chunked FITS file reader.
 
     There are two column-level arguments for reading fits files:
     `column_names` and `skip_column_names`.
-    
+
         - If neither is provided, we will read and process all columns in the fits file.
         - If `column_names` is given, we will use *only* those names, and
           `skip_column_names` will be ignored.
         - If `skip_column_names` is provided, we will remove those columns from processing stages.
 
+    NB:
+        Uses astropy table memmap to avoid reading the entire file into memory.
+
+        See: https://docs.astropy.org/en/stable/io/fits/index.html#working-with-large-files
+
+
     Attributes:
         chunksize (int): number of rows of the file to process at once.
             For large files, this can prevent loading the entire file
             into memory at once.
         column_names (list[str]): list of column names to keep. only use
             one of `column_names` or `skip_column_names`
         skip_column_names (list[str]): list of column names to skip. only use
             one of `column_names` or `skip_column_names`
     """
 
     def __init__(
-        self,
-        chunksize=500_000,
-        column_names=None,
-        skip_column_names=None,
+        self, chunksize=500_000, column_names=None, skip_column_names=None, **kwargs
     ):
         self.chunksize = chunksize
         self.column_names = column_names
         self.skip_column_names = skip_column_names
+        self.kwargs = kwargs
 
     def read(self, input_file):
-        """Read chunks of rows in a fits file.
-
-        Uses astropy table memmap to avoid reading the entire file into memory.
-
-        See: https://docs.astropy.org/en/stable/io/fits/index.html#working-with-large-files
-        """
-        table = Table.read(input_file, memmap=True)
+        table = Table.read(input_file, memmap=True, **self.kwargs)
         if self.column_names:
             table.keep_columns(self.column_names)
         elif self.skip_column_names:
             table.remove_columns(self.skip_column_names)
 
         total_rows = len(table)
         read_rows = 0
@@ -222,30 +227,27 @@
             "skip_column_names": self.skip_column_names,
         }
         return provenance_info
 
 
 class ParquetReader(InputReader):
     """Parquet reader for the most common Parquet reading arguments.
-    
+
     Attributes:
         chunksize (int): number of rows of the file to process at once.
             For large files, this can prevent loading the entire file
             into memory at once.
     """
 
-    def __init__(
-        self,
-        chunksize=500_000,
-    ):
+    def __init__(self, chunksize=500_000, **kwargs):
         self.chunksize = chunksize
+        self.kwargs = kwargs
 
     def read(self, input_file):
-        """Read chunks of rows in a parquet file."""
-        parquet_file = pq.read_table(input_file)
+        parquet_file = pq.read_table(input_file, **self.kwargs)
         for smaller_table in parquet_file.to_batches(max_chunksize=self.chunksize):
             yield pa.Table.from_batches([smaller_table]).to_pandas()
 
     def provenance_info(self) -> dict:
         provenance_info = {
             "input_reader_type": "ParquetReader",
             "chunksize": self.chunksize,
```

### Comparing `hipscat-import-0.0.3/src/hipscat_import/map_reduce.py` & `hipscat-import-0.0.4/src/hipscat_import/catalog/map_reduce.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,191 +1,301 @@
 """Import a set of non-hipscat files using dask for parallelization"""
 
 import healpy as hp
 import numpy as np
-import pandas as pd
+import pyarrow as pa
+import pyarrow.parquet as pq
 from hipscat import pixel_math
 from hipscat.io import FilePointer, file_io, paths
 
+from hipscat_import.catalog.file_readers import InputReader
+
 # pylint: disable=too-many-locals,too-many-arguments
 
 
-def _get_pixel_directory(cache_path: FilePointer, pixel: np.int64):
+def _get_pixel_directory(cache_path: FilePointer, order: np.int64, pixel: np.int64):
     """Create a path for intermediate pixel data.
-    
+
     This will take the form:
 
         <cache_path>/dir_<directory separator>/pixel_<pixel>
 
     where the directory separator is calculated using integer division:
 
         (pixel/10000)*10000
 
     and exists to mitigate problems on file systems that don't support
     more than 10_000 children nodes.
     """
     dir_number = int(pixel / 10_000) * 10_000
     return file_io.append_paths_to_pointer(
-        cache_path, f"dir_{dir_number}", f"pixel_{pixel}"
+        cache_path, f"order_{order}", f"dir_{dir_number}", f"pixel_{pixel}"
     )
 
 
-def map_to_pixels(
+def _has_named_index(dataframe):
+    """Heuristic to determine if a dataframe has some meaningful index.
+
+    This will reject dataframes with no index name for a single index,
+    or empty names for multi-index (e.g. [] or [None]).
+    """
+    if dataframe.index.name is not None:
+        ## Single index with a given name.
+        return True
+    if len(dataframe.index.names) == 0 or all(
+        name is None for name in dataframe.index.names
+    ):
+        return False
+    return True
+
+
+def _iterate_input_file(
     input_file: FilePointer,
-    file_reader,
-    shard_suffix,
+    file_reader: InputReader,
     highest_order,
     ra_column,
     dec_column,
-    cache_path: FilePointer = None,
     filter_function=None,
 ):
-    """Map a file of input objects to their healpix pixels.
-    
-    Args:
-        input_file (FilePointer): file to read for catalog data.
-        file_reader (InputReader): instance of input reader that
-            specifies arguments necessary for reading from the input file.
-        shard_suffix (str): unique counter for this input file, used
-            when creating intermediate files
-        highest_order (int): healpix order to use when mapping
-        ra_column (str): where to find right ascension data in the dataframe
-        dec_column (str): where to find declation in the dataframe
-        cache_path (FilePointer): where to write intermediate files.
-            if None, no intermediate files will be written, but healpix
-            stats will be returned
-        filter_function (function pointer): method to perform some filtering
-            or transformation of the input data
-    Returns:
-        one-dimensional numpy array of long integers where the value at each index corresponds
-        to the number of objects found at the healpix pixel.
-    Raises:
-        ValueError: if the `ra_column` or `dec_column` cannot be found in the input file.
-        FileNotFoundError: if the file does not exist, or is a directory
-    """
-
-    # Perform checks on the provided path
+    """Helper function to handle input file reading and healpix pixel calculation"""
     if not file_io.does_file_or_directory_exist(input_file):
         raise FileNotFoundError(f"File not found at path: {input_file}")
     if not file_io.is_regular_file(input_file):
         raise FileNotFoundError(
             f"Directory found at path - requires regular file: {input_file}"
         )
     if not file_reader:
         raise NotImplementedError("No file reader implemented")
 
     required_columns = [ra_column, dec_column]
-    histo = pixel_math.empty_histogram(highest_order)
 
     for chunk_number, data in enumerate(file_reader.read(input_file)):
-        data.reset_index(inplace=True)
         if not all(x in data.columns for x in required_columns):
             raise ValueError(
                 f"Invalid column names in input file: {ra_column}, {dec_column} not in {input_file}"
             )
         # Set up the data we want (filter and find pixel)
         if filter_function:
             data = filter_function(data)
-            data.reset_index(inplace=True)
         mapped_pixels = hp.ang2pix(
             2**highest_order,
             data[ra_column].values,
             data[dec_column].values,
             lonlat=True,
             nest=True,
         )
+        yield chunk_number, data, mapped_pixels
+
+
+def map_to_pixels(
+    input_file: FilePointer,
+    file_reader: InputReader,
+    highest_order,
+    ra_column,
+    dec_column,
+    filter_function=None,
+):
+    """Map a file of input objects to their healpix pixels.
+
+    Args:
+        input_file (FilePointer): file to read for catalog data.
+        file_reader (hipscat_import.catalog.file_readers.InputReader): instance of input
+            reader that specifies arguments necessary for reading from the input file.
+        shard_suffix (str): unique counter for this input file, used
+            when creating intermediate files
+        highest_order (int): healpix order to use when mapping
+        ra_column (str): where to find right ascension data in the dataframe
+        dec_column (str): where to find declation in the dataframe
+
+    Returns:
+        one-dimensional numpy array of long integers where the value at each index corresponds
+        to the number of objects found at the healpix pixel.
+    Raises:
+        ValueError: if the `ra_column` or `dec_column` cannot be found in the input file.
+        FileNotFoundError: if the file does not exist, or is a directory
+    """
+    histo = pixel_math.empty_histogram(highest_order)
+    for _, _, mapped_pixels in _iterate_input_file(
+        input_file, file_reader, highest_order, ra_column, dec_column, filter_function
+    ):
         mapped_pixel, count_at_pixel = np.unique(mapped_pixels, return_counts=True)
         histo[mapped_pixel] += count_at_pixel.astype(np.int64)
+    return histo
 
-        if cache_path:
-            for pixel in mapped_pixel:
-                data_indexes = np.where(mapped_pixels == pixel)
-                filtered_data = data.filter(items=data_indexes[0].tolist(), axis=0)
-
-                pixel_dir = _get_pixel_directory(cache_path, pixel)
-                file_io.make_directory(pixel_dir, exist_ok=True)
-                output_file = file_io.append_paths_to_pointer(
-                    pixel_dir, f"shard_{shard_suffix}_{chunk_number}.parquet"
-                )
-                filtered_data.to_parquet(output_file)
-            del filtered_data, data_indexes
 
-        ## Pesky memory!
-        del mapped_pixels, mapped_pixel, count_at_pixel
-    return histo
+def split_pixels(
+    input_file: FilePointer,
+    file_reader: InputReader,
+    shard_suffix,
+    highest_order,
+    ra_column,
+    dec_column,
+    cache_path: FilePointer,
+    alignment=None,
+    filter_function=None,
+):
+    """Map a file of input objects to their healpix pixels and split into shards.
+
+    Args:
+        input_file (FilePointer): file to read for catalog data.
+        file_reader (hipscat_import.catalog.file_readers.InputReader): instance
+            of input reader that specifies arguments necessary for reading from the input file.
+        shard_suffix (str): unique counter for this input file, used
+            when creating intermediate files
+        highest_order (int): healpix order to use when mapping
+        ra_column (str): where to find right ascension data in the dataframe
+        dec_column (str): where to find declation in the dataframe
+        cache_path (FilePointer): where to write intermediate files.
+        filter_function (function pointer): method to perform some filtering
+            or transformation of the input data
+
+    Raises:
+        ValueError: if the `ra_column` or `dec_column` cannot be found in the input file.
+        FileNotFoundError: if the file does not exist, or is a directory
+    """
+    for chunk_number, data, mapped_pixels in _iterate_input_file(
+        input_file, file_reader, highest_order, ra_column, dec_column, filter_function
+    ):
+        aligned_pixels = alignment[mapped_pixels]
+        unique_pixels, unique_inverse = np.unique(aligned_pixels, return_inverse=True)
+
+        for unique_index, [order, pixel, _] in enumerate(unique_pixels):
+            mapped_indexes = np.where(unique_inverse == unique_index)
+            data_indexes = data.index[mapped_indexes[0].tolist()]
+
+            filtered_data = data.filter(items=data_indexes, axis=0)
+
+            pixel_dir = _get_pixel_directory(cache_path, order, pixel)
+            file_io.make_directory(pixel_dir, exist_ok=True)
+            output_file = file_io.append_paths_to_pointer(
+                pixel_dir, f"shard_{shard_suffix}_{chunk_number}.parquet"
+            )
+            if _has_named_index(filtered_data):
+                filtered_data.to_parquet(output_file, index=True)
+            else:
+                filtered_data.to_parquet(output_file, index=False)
+        del filtered_data, data_indexes
 
 
 def reduce_pixel_shards(
     cache_path,
-    origin_pixel_numbers,
     destination_pixel_order,
     destination_pixel_number,
     destination_pixel_size,
     output_path,
     ra_column,
     dec_column,
     id_column,
     add_hipscat_index=True,
     delete_input_files=True,
+    use_schema_file="",
 ):
     """Reduce sharded source pixels into destination pixels.
-    
+
+    In addition to combining multiple shards of data into a single
+    parquet file, this method will add a few new columns:
+
+        - ``Norder`` - the healpix order for the pixel
+        - ``Dir`` - the directory part, corresponding to the pixel
+        - ``Npix`` - the healpix pixel
+        - ``_hipscat_index`` - optional - a spatially-correlated
+          64-bit index field.
+
+    Notes on ``_hipscat_index``:
+
+        - if we generate the field, we will promote any previous
+          *named* pandas index field(s) to a column with
+          that name.
+        - see ``hipscat.pixel_math.hipscat_id``
+          for more in-depth discussion of this field.
+
     Args:
         cache_path (str): where to read intermediate files
         origin_pixel_numbers (list[int]): high order pixels, with object
             data written to intermediate directories.
         destination_pixel_order (int): order of the final catalog pixel
         destination_pixel_number (int): pixel number at the above order
         destination_pixel_size (int): expected number of rows to write
             for the catalog's final pixel
         output_path (str): where to write the final catalog pixel data
         id_column (str): column for survey identifier, or other sortable column
+        add_hipscat_index (bool): should we add a _hipscat_index column to
+            the resulting parquet file?
         delete_input_files (bool): should we delete the intermediate files
             used as input for this method.
+        use_schema_file (str): use the parquet schema from the indicated
+            parquet file.
 
     Raises:
         ValueError: if the number of rows written doesn't equal provided
-            `destination_pixel_size`    
+            `destination_pixel_size`
     """
     destination_dir = paths.pixel_directory(
         output_path, destination_pixel_order, destination_pixel_number
     )
     file_io.make_directory(destination_dir, exist_ok=True)
 
     destination_file = paths.pixel_catalog_file(
         output_path, destination_pixel_order, destination_pixel_number
     )
 
+    schema = None
+    if use_schema_file:
+        schema = file_io.read_parquet_metadata(use_schema_file).schema.to_arrow_schema()
+
     tables = []
-    for pixel in origin_pixel_numbers:
-        pixel_dir = _get_pixel_directory(cache_path, pixel)
+    pixel_dir = _get_pixel_directory(
+        cache_path, destination_pixel_order, destination_pixel_number
+    )
 
-        for file in file_io.get_directory_contents(pixel_dir):
-            tables.append(pd.read_parquet(file, engine="pyarrow"))
+    if schema:
+        tables.append(pq.read_table(pixel_dir, schema=schema))
+    else:
+        tables.append(pq.read_table(pixel_dir))
 
-    merged_table = pd.concat(tables, ignore_index=True, sort=False)
-    if id_column:
-        merged_table = merged_table.sort_values(by=id_column)
-    if add_hipscat_index:
-        merged_table["_hipscat_index"] = pixel_math.compute_hipscat_id(
-            merged_table[ra_column].values, merged_table[dec_column].values
-        )
-        merged_table.set_index("_hipscat_index").sort_index()
+    merged_table = pa.concat_tables(tables)
 
     rows_written = len(merged_table)
 
     if rows_written != destination_pixel_size:
         raise ValueError(
             "Unexpected number of objects at pixel "
             f"({destination_pixel_order}, {destination_pixel_number})."
             f" Expected {destination_pixel_size}, wrote {rows_written}"
         )
 
-    merged_table.to_parquet(destination_file)
+    dataframe = merged_table.to_pandas()
+    if id_column:
+        dataframe = dataframe.sort_values(id_column)
+    if add_hipscat_index:
+        dataframe["_hipscat_index"] = pixel_math.compute_hipscat_id(
+            dataframe[ra_column].values,
+            dataframe[dec_column].values,
+        )
+
+    dataframe["Norder"] = np.full(
+        rows_written, fill_value=destination_pixel_order, dtype=np.int32
+    )
+    dataframe["Dir"] = np.full(
+        rows_written,
+        fill_value=int(destination_pixel_number / 10_000) * 10_000,
+        dtype=np.int32,
+    )
+    dataframe["Npix"] = np.full(
+        rows_written, fill_value=destination_pixel_number, dtype=np.int32
+    )
 
-    del merged_table, tables
+    if add_hipscat_index:
+        ## If we had a meaningful index before, preserve it as a column.
+        if _has_named_index(dataframe):
+            dataframe = dataframe.reset_index()
+        dataframe = dataframe.set_index("_hipscat_index").sort_index()
+    dataframe.to_parquet(destination_file)
+
+    del dataframe, merged_table, tables
 
     if delete_input_files:
-        for pixel in origin_pixel_numbers:
-            pixel_dir = _get_pixel_directory(cache_path=cache_path, pixel=pixel)
+        pixel_dir = _get_pixel_directory(
+            cache_path, destination_pixel_order, destination_pixel_number
+        )
 
-            file_io.remove_directory(pixel_dir, ignore_errors=True)
+        file_io.remove_directory(pixel_dir, ignore_errors=True)
```

### Comparing `hipscat-import-0.0.3/src/hipscat_import/resume_files.py` & `hipscat-import-0.0.4/src/hipscat_import/catalog/resume_files.py`

 * *Files 21% similar despite different names*

```diff
@@ -35,14 +35,26 @@
 
 
 def set_mapping_done(tmp_path: FilePointer):
     """Touch (create) a done file"""
     Path(file_io.append_paths_to_pointer(tmp_path, "mapping_done")).touch()
 
 
+def is_splitting_done(tmp_path: FilePointer):
+    """Check for existence of done file"""
+    return file_io.does_file_or_directory_exist(
+        file_io.append_paths_to_pointer(tmp_path, "splitting_done")
+    )
+
+
+def set_splitting_done(tmp_path: FilePointer):
+    """Touch (create) a done file"""
+    Path(file_io.append_paths_to_pointer(tmp_path, "splitting_done")).touch()
+
+
 def is_reducing_done(tmp_path: FilePointer):
     """Check for existence of done file"""
     return file_io.does_file_or_directory_exist(
         file_io.append_paths_to_pointer(tmp_path, "reducing_done")
     )
 
 
@@ -62,14 +74,21 @@
     if len(mapping_done_keys) != len(mapping_start_keys):
         raise ValueError(
             "Resume logs are corrupted. Delete temp directory and restart import pipeline."
         )
     return mapping_start_keys
 
 
+def read_splitting_keys(tmp_path: FilePointer):
+    """Read keys from splitting log file"""
+    return _read_log_keys(
+        file_io.append_paths_to_pointer(tmp_path, "splitting_done_log.txt")
+    )
+
+
 def read_reducing_keys(tmp_path: FilePointer):
     """Read keys from reducing log file"""
     return _read_log_keys(file_io.append_paths_to_pointer(tmp_path, "reducing_log.txt"))
 
 
 def _read_log_keys(file_name):
     """Read a resume log file, containing timestamp and keys."""
@@ -94,14 +113,21 @@
 def write_mapping_done_key(tmp_path: FilePointer, key):
     """Append single key to mapping log file"""
     _write_log_key(
         file_io.append_paths_to_pointer(tmp_path, "mapping_done_log.txt"), key
     )
 
 
+def write_splitting_done_key(tmp_path: FilePointer, key):
+    """Append single key to splitting log file"""
+    _write_log_key(
+        file_io.append_paths_to_pointer(tmp_path, "splitting_done_log.txt"), key
+    )
+
+
 def write_reducing_key(tmp_path: FilePointer, key):
     """Append single key to reducing log file"""
     _write_log_key(file_io.append_paths_to_pointer(tmp_path, "reducing_log.txt"), key)
 
 
 def _write_log_key(file_name, key):
     """Append a tab-delimited line to the file with the current timestamp and provided key"""
```

### Comparing `hipscat-import-0.0.3/src/hipscat_import/run_import.py` & `hipscat-import-0.0.4/src/hipscat_import/catalog/run_import.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,151 +3,224 @@
 Methods in this file set up a dask pipeline using futures. 
 The actual logic of the map reduce is in the `map_reduce.py` file.
 """
 
 
 import hipscat.io.write_metadata as io
 import numpy as np
-from dask.distributed import Client, as_completed
+from dask.distributed import as_completed
 from hipscat import pixel_math
 from tqdm import tqdm
 
-import hipscat_import.map_reduce as mr
-import hipscat_import.resume_files as resume
-from hipscat_import.arguments import ImportArguments
+import hipscat_import.catalog.map_reduce as mr
+import hipscat_import.catalog.resume_files as resume
+from hipscat_import.catalog.arguments import ImportArguments
 
 
 def _map_pixels(args, client):
     """Generate a raw histogram of object counts in each healpix pixel"""
 
-    raw_histogram = resume.read_histogram(args.tmp_path, args.highest_healpix_order)
+    raw_histogram = resume.read_histogram(args.tmp_path, args.mapping_healpix_order)
     if resume.is_mapping_done(args.tmp_path):
         return raw_histogram
 
     mapped_paths = set(resume.read_mapping_keys(args.tmp_path))
 
     futures = []
-    for i, file_path in enumerate(args.input_paths):
-        if file_path in mapped_paths:
+    for file_path in args.input_paths:
+        map_key = f"map_{file_path}"
+        if map_key in mapped_paths:
             continue
         futures.append(
             client.submit(
                 mr.map_to_pixels,
-                key=file_path,
+                key=map_key,
                 input_file=file_path,
                 file_reader=args.file_reader,
                 filter_function=args.filter_function,
-                highest_order=args.highest_healpix_order,
+                highest_order=args.mapping_healpix_order,
                 ra_column=args.ra_column,
                 dec_column=args.dec_column,
-                shard_suffix=i,
-                cache_path=None if args.debug_stats_only else args.tmp_path,
             )
         )
 
+    some_error = False
     for future, result in tqdm(
         as_completed(futures, with_results=True),
         desc="Mapping  ",
         total=len(futures),
         disable=(not args.progress_bar),
     ):
+        if future.status == "error":  # pragma: no cover
+            some_error = True
+            continue
         raw_histogram = np.add(raw_histogram, result)
         resume.write_mapping_start_key(args.tmp_path, future.key)
         resume.write_histogram(args.tmp_path, raw_histogram)
         resume.write_mapping_done_key(args.tmp_path, future.key)
+    if some_error:  # pragma: no cover
+        raise RuntimeError("Some mapping stages failed. See logs for details.")
     resume.set_mapping_done(args.tmp_path)
     return raw_histogram
 
 
+def _split_pixels(args, alignment_future, client):
+    """Generate a raw histogram of object counts in each healpix pixel"""
+
+    if resume.is_splitting_done(args.tmp_path):
+        return
+
+    split_paths = set(resume.read_splitting_keys(args.tmp_path))
+
+    futures = []
+    for i, file_path in enumerate(args.input_paths):
+        split_key = f"split_{file_path}"
+        if split_key in split_paths:
+            continue
+        futures.append(
+            client.submit(
+                mr.split_pixels,
+                key=split_key,
+                input_file=file_path,
+                file_reader=args.file_reader,
+                filter_function=args.filter_function,
+                highest_order=args.mapping_healpix_order,
+                ra_column=args.ra_column,
+                dec_column=args.dec_column,
+                shard_suffix=i,
+                cache_path=args.tmp_path,
+                alignment=alignment_future,
+            )
+        )
+
+    some_error = False
+    for future in tqdm(
+        as_completed(futures),
+        desc="Splitting",
+        total=len(futures),
+        disable=(not args.progress_bar),
+    ):
+        if future.status == "error":  # pragma: no cover
+            some_error = True
+            continue
+        resume.write_splitting_done_key(args.tmp_path, future.key)
+    if some_error:  # pragma: no cover
+        raise RuntimeError("Some splitting stages failed. See logs for details.")
+    resume.set_splitting_done(args.tmp_path)
+
+
 def _reduce_pixels(args, destination_pixel_map, client):
     """Loop over destination pixels and merge into parquet files"""
 
     if resume.is_reducing_done(args.tmp_path):
         return
 
     reduced_keys = set(resume.read_reducing_keys(args.tmp_path))
 
     futures = []
     for destination_pixel, source_pixels in destination_pixel_map.items():
-        destination_pixel_key = f"{destination_pixel[0]}_{destination_pixel[1]}"
+        destination_pixel_key = f"{destination_pixel.order}_{destination_pixel.pixel}"
         if destination_pixel_key in reduced_keys:
             continue
         futures.append(
             client.submit(
                 mr.reduce_pixel_shards,
                 key=destination_pixel_key,
                 cache_path=args.tmp_path,
-                origin_pixel_numbers=source_pixels,
-                destination_pixel_order=destination_pixel[0],
-                destination_pixel_number=destination_pixel[1],
-                destination_pixel_size=destination_pixel[2],
+                destination_pixel_order=destination_pixel.order,
+                destination_pixel_number=destination_pixel.pixel,
+                destination_pixel_size=source_pixels[0],
                 output_path=args.catalog_path,
                 ra_column=args.ra_column,
                 dec_column=args.dec_column,
                 id_column=args.id_column,
                 add_hipscat_index=args.add_hipscat_index,
+                use_schema_file=args.use_schema_file,
             )
         )
+
+    some_error = False
     for future in tqdm(
         as_completed(futures),
         desc="Reducing ",
         total=len(futures),
         disable=(not args.progress_bar),
     ):
+        if future.status == "error":  # pragma: no cover
+            some_error = True
+            continue
         resume.write_reducing_key(args.tmp_path, future.key)
+    if some_error:  # pragma: no cover
+        raise RuntimeError("Some reducing stages failed. See logs for details.")
     resume.set_reducing_done(args.tmp_path)
 
 
-def _validate_args(args):
+def run(args, client):
+    """Run catalog creation pipeline."""
     if not args:
         raise ValueError("args is required and should be type ImportArguments")
     if not isinstance(args, ImportArguments):
         raise ValueError("args must be type ImportArguments")
-
-
-def run(args):
-    """Importer that creates a dask client from the arguments"""
-    _validate_args(args)
-
-    with Client(
-        local_directory=args.dask_tmp,
-        n_workers=args.dask_n_workers,
-        threads_per_worker=args.dask_threads_per_worker,
-    ) as client:  # pragma: no cover
-        run_with_client(args, client)
-
-
-def run_with_client(args, client):
-    """Importer, where the client context may out-live the runner"""
-    _validate_args(args)
     raw_histogram = _map_pixels(args, client)
 
-    step_progress = tqdm(total=2, desc="Binning  ", disable=not args.progress_bar)
-    pixel_map = pixel_math.generate_alignment(
-        raw_histogram, args.highest_healpix_order, args.pixel_threshold
-    )
-    step_progress.update(1)
-    destination_pixel_map = pixel_math.generate_destination_pixel_map(
-        raw_histogram, pixel_map
-    )
-    step_progress.update(1)
-    step_progress.close()
+    with tqdm(
+        total=1, desc="Binning  ", disable=not args.progress_bar
+    ) as step_progress:
+        if args.constant_healpix_order >= 0:
+            alignment = np.full(len(raw_histogram), None)
+            for pixel_num, pixel_sum in enumerate(raw_histogram):
+                alignment[pixel_num] = (
+                    args.constant_healpix_order,
+                    pixel_num,
+                    pixel_sum,
+                )
+
+            destination_pixel_map = pixel_math.generate_constant_pixel_map(
+                histogram=raw_histogram,
+                constant_healpix_order=args.constant_healpix_order,
+            )
+        else:
+            alignment = pixel_math.generate_alignment(
+                raw_histogram,
+                highest_order=args.highest_healpix_order,
+                threshold=args.pixel_threshold,
+            )
+            destination_pixel_map = pixel_math.compute_pixel_map(
+                raw_histogram,
+                highest_order=args.highest_healpix_order,
+                threshold=args.pixel_threshold,
+            )
+        step_progress.update(1)
 
     if not args.debug_stats_only:
+        alignment_future = client.scatter(alignment)
+        _split_pixels(args, alignment_future, client)
         _reduce_pixels(args, destination_pixel_map, client)
 
     # All done - write out the metadata
-    step_progress = tqdm(total=6, desc="Finishing", disable=not args.progress_bar)
-    io.write_provenance_info(args.to_catalog_parameters(), args.provenance_info())
-    step_progress.update(1)
-    io.write_catalog_info(args.to_catalog_parameters(), raw_histogram)
-    step_progress.update(1)
-    if not args.debug_stats_only:
-        io.write_parquet_metadata(args.catalog_path)
-    step_progress.update(1)
-    io.write_fits_map(args.catalog_path, raw_histogram)
-    step_progress.update(1)
-    io.write_partition_info(args.to_catalog_parameters(), destination_pixel_map)
-    step_progress.update(1)
-    resume.clean_resume_files(args.tmp_path)
-    step_progress.update(1)
-    step_progress.close()
+    with tqdm(
+        total=6, desc="Finishing", disable=not args.progress_bar
+    ) as step_progress:
+        catalog_info = args.to_catalog_info(int(raw_histogram.sum()))
+        io.write_provenance_info(
+            catalog_base_dir=args.catalog_path,
+            dataset_info=catalog_info,
+            tool_args=args.provenance_info(),
+        )
+        step_progress.update(1)
+
+        io.write_catalog_info(
+            catalog_base_dir=args.catalog_path, dataset_info=catalog_info
+        )
+        step_progress.update(1)
+        if not args.debug_stats_only:
+            io.write_parquet_metadata(args.catalog_path)
+        step_progress.update(1)
+        io.write_fits_map(args.catalog_path, raw_histogram)
+        step_progress.update(1)
+        io.write_partition_info(
+            catalog_base_dir=args.catalog_path,
+            destination_healpix_pixel_map=destination_pixel_map,
+        )
+        step_progress.update(1)
+        resume.clean_resume_files(args.tmp_path)
+        step_progress.update(1)
```

### Comparing `hipscat-import-0.0.3/src/hipscat_import.egg-info/PKG-INFO` & `hipscat-import-0.0.4/src/hipscat_import.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: hipscat-import
-Version: 0.0.3
+Version: 0.0.4
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
-        Copyright (c) 2023, Astronomy Data Commons
+        Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
         
@@ -26,14 +26,15 @@
         DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -64,7 +65,13 @@
 
 ## Contributing
 
 [![GitHub issue custom search in repo](https://img.shields.io/github/issues-search/astronomy-commons/hipscat-import?color=purple&label=Good%20first%20issues&query=is%3Aopen%20label%3A%22good%20first%20issue%22)](https://github.com/astronomy-commons/hipscat-import/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
 
 See the [contribution guide](https://hipscat-import.readthedocs.io/en/latest/overview/contributing.html)
 for complete installation instructions and contribution best practices.
+
+## Acknowledgements
+
+LINCC Frameworks is supported by Schmidt Futures, a philanthropic initiative
+founded by Eric and Wendy Schmidt, as part of the Virtual Institute of 
+Astrophysics (VIA).
```

### Comparing `hipscat-import-0.0.3/tests/.pylintrc` & `hipscat-import-0.0.4/tests/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # Always return a 0 (non-error) status code, even if lint errors are found.
 # This is primarily useful in continuous integration scripts.
 #exit-zero=
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code.
-extension-pkg-allow-list=
+extension-pkg-allow-list=pyarrow.lib
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code. (This is an alternative name to extension-pkg-allow-list
 # for backward compatibility.)
 extension-pkg-whitelist=
 
@@ -273,15 +273,15 @@
 exclude-too-few-public-methods=
 
 # List of qualified class names to ignore when counting class parents (see
 # R0901)
 ignored-parents=
 
 # Maximum number of arguments for function / method.
-max-args=5
+max-args=10
 
 # Maximum number of attributes for a class (see R0902).
 max-attributes=7
 
 # Maximum number of boolean expressions in an if statement (see R0916).
 max-bool-expr=5
 
@@ -328,15 +328,15 @@
 # tab).
 indent-string='    '
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module.
-max-module-lines=1000
+max-module-lines=500
 
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
@@ -440,16 +440,15 @@
 timeout-methods=requests.api.delete,requests.api.get,requests.api.head,requests.api.options,requests.api.patch,requests.api.post,requests.api.put,requests.api.request
 
 
 [MISCELLANEOUS]
 
 # List of note tags to take in consideration, separated by a comma.
 notes=FIXME,
-      XXX,
-      TODO
+      XXX
 
 # Regular expression of note tags to take in consideration.
 notes-rgx=
 
 
 [REFACTORING]
 
@@ -499,15 +498,15 @@
 # Imports are removed from the similarity computation
 ignore-imports=yes
 
 # Signatures are removed from the similarity computation
 ignore-signatures=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=10
 
 
 [SPELLING]
 
 # Limits count of emitted suggestions for spelling mistakes.
 max-spelling-suggestions=4
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/mixed_schema/schema.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/mixed_schema/schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_44/shard_0.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet`

 * *Files 12% similar despite different names*

```diff
@@ -60,247 +60,182 @@
 000003b0: 0000 0000 0000 0009 2002 0000 000e 0101  ........ .......
 000003c0: 0e00 2684 0f1c 1504 1935 1000 0619 1809  ..&......5......
 000003d0: 6465 635f 6572 726f 7215 0216 0e16 b801  dec_error.......
 000003e0: 16c0 0126 f40d 26c4 0d1c 1808 0000 0000  ...&..&.........
 000003f0: 0000 0000 1808 0000 0000 0000 0000 1600  ................
 00000400: 2808 0000 0000 0000 0000 1808 0000 0000  (...............
 00000410: 0000 0000 0019 2c15 0415 0015 0200 1500  ......,.........
-00000420: 1510 1502 0000 0015 0415 7015 504c 150e  ..........p.PL..
-00000430: 1500 1200 0038 0403 0009 0100 0a09 0704  .....8..........
-00000440: 000f 0d08 0011 0d08 0012 0d08 3c14 0000  ............<...
-00000450: 0000 0000 0018 0000 0000 0000 0015 0015  ................
-00000460: 1615 1a2c 150e 1510 1506 1506 1c18 0818  ...,............
-00000470: 0000 0000 0000 0018 0803 0000 0000 0000  ................
-00000480: 0016 0028 0818 0000 0000 0000 0018 0803  ...(............
-00000490: 0000 0000 0000 0000 0000 0b28 0200 0000  ...........(....
-000004a0: 0e01 0303 88c6 1a26 ce12 1c15 0419 3510  .......&......5.
-000004b0: 0006 1918 115f 5f69 6e64 6578 5f6c 6576  .....__index_lev
-000004c0: 656c 5f30 5f5f 1502 160e 169c 0216 8002  el_0__..........
-000004d0: 26ba 1126 ce10 1c18 0818 0000 0000 0000  &..&............
-000004e0: 0018 0803 0000 0000 0000 0016 0028 0818  .............(..
-000004f0: 0000 0000 0000 0018 0803 0000 0000 0000  ................
-00000500: 0000 192c 1504 1500 1502 0015 0015 1015  ...,............
-00000510: 0200 0000 1504 197c 3500 1806 7363 6865  .......|5...sche
-00000520: 6d61 150c 0015 0425 0218 0269 6400 150a  ma.....%...id...
-00000530: 2502 1802 7261 0015 0a25 0218 0364 6563  %...ra...%...dec
-00000540: 0015 0425 0218 0872 615f 6572 726f 7200  ...%...ra_error.
-00000550: 1504 2502 1809 6465 635f 6572 726f 7200  ..%...dec_error.
-00000560: 1504 2502 1811 5f5f 696e 6465 785f 6c65  ..%...__index_le
-00000570: 7665 6c5f 305f 5f00 160e 191c 196c 2688  vel_0__......l&.
-00000580: 021c 1504 1935 1000 0619 1802 6964 1502  .....5......id..
-00000590: 160e 169c 0216 8002 2674 2608 1c18 0821  ........&t&....!
-000005a0: 0300 0000 0000 0018 080c 0300 0000 0000  ................
-000005b0: 0016 0028 0821 0300 0000 0000 0018 080c  ...(.!..........
-000005c0: 0300 0000 0000 0000 192c 1504 1500 1502  .........,......
-000005d0: 0015 0015 1015 0200 0000 26bc 051c 150a  ..........&.....
-000005e0: 1935 1000 0619 1802 7261 1502 160e 168c  .5......ra......
-000005f0: 0216 fc01 26a8 0426 c003 1c18 0800 0000  ....&..&........
-00000600: 0000 6874 4018 0800 0000 0000 c872 4016  ..ht@........r@.
-00000610: 0028 0800 0000 0000 6874 4018 0800 0000  .(......ht@.....
-00000620: 0000 c872 4000 192c 1504 1500 1502 0015  ...r@..,........
-00000630: 0015 1015 0200 0000 26fe 081c 150a 1935  ........&......5
-00000640: 1000 0619 1803 6465 6315 0216 0e16 9c02  ......dec.......
-00000650: 1686 0226 ea07 26f8 061c 1808 0000 0000  ...&..&.........
-00000660: 00c0 47c0 1808 0000 0000 0060 51c0 1600  ..G........`Q...
-00000670: 2808 0000 0000 00c0 47c0 1808 0000 0000  (.......G.......
-00000680: 0060 51c0 0019 2c15 0415 0015 0200 1500  .`Q...,.........
-00000690: 1510 1502 0000 0026 fc0b 1c15 0419 3510  .......&......5.
-000006a0: 0006 1918 0872 615f 6572 726f 7215 0216  .....ra_error...
-000006b0: 0e16 b801 16c0 0126 ec0a 26bc 0a1c 1808  .......&..&.....
-000006c0: 0000 0000 0000 0000 1808 0000 0000 0000  ................
-000006d0: 0000 1600 2808 0000 0000 0000 0000 1808  ....(...........
-000006e0: 0000 0000 0000 0000 0019 2c15 0415 0015  ..........,.....
-000006f0: 0200 1500 1510 1502 0000 0026 840f 1c15  ...........&....
-00000700: 0419 3510 0006 1918 0964 6563 5f65 7272  ..5......dec_err
-00000710: 6f72 1502 160e 16b8 0116 c001 26f4 0d26  or..........&..&
-00000720: c40d 1c18 0800 0000 0000 0000 0018 0800  ................
-00000730: 0000 0000 0000 0016 0028 0800 0000 0000  .........(......
-00000740: 0000 0018 0800 0000 0000 0000 0000 192c  ...............,
-00000750: 1504 1500 1502 0015 0015 1015 0200 0000  ................
-00000760: 26ce 121c 1504 1935 1000 0619 1811 5f5f  &......5......__
-00000770: 696e 6465 785f 6c65 7665 6c5f 305f 5f15  index_level_0__.
-00000780: 0216 0e16 9c02 1680 0226 ba11 26ce 101c  .........&..&...
-00000790: 1808 1800 0000 0000 0000 1808 0300 0000  ................
-000007a0: 0000 0000 1600 2808 1800 0000 0000 0000  ......(.........
-000007b0: 1808 0300 0000 0000 0000 0019 2c15 0415  ............,...
-000007c0: 0015 0200 1500 1510 1502 0000 0016 d00b  ................
-000007d0: 160e 2608 1682 0b14 0000 192c 1806 7061  ..&........,..pa
-000007e0: 6e64 6173 18a5 077b 2269 6e64 6578 5f63  ndas...{"index_c
-000007f0: 6f6c 756d 6e73 223a 205b 225f 5f69 6e64  olumns": ["__ind
-00000800: 6578 5f6c 6576 656c 5f30 5f5f 225d 2c20  ex_level_0__"], 
-00000810: 2263 6f6c 756d 6e5f 696e 6465 7865 7322  "column_indexes"
-00000820: 3a20 5b7b 226e 616d 6522 3a20 6e75 6c6c  : [{"name": null
-00000830: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
-00000840: 6e75 6c6c 2c20 2270 616e 6461 735f 7479  null, "pandas_ty
-00000850: 7065 223a 2022 756e 6963 6f64 6522 2c20  pe": "unicode", 
-00000860: 226e 756d 7079 5f74 7970 6522 3a20 226f  "numpy_type": "o
-00000870: 626a 6563 7422 2c20 226d 6574 6164 6174  bject", "metadat
-00000880: 6122 3a20 7b22 656e 636f 6469 6e67 223a  a": {"encoding":
-00000890: 2022 5554 462d 3822 7d7d 5d2c 2022 636f   "UTF-8"}}], "co
-000008a0: 6c75 6d6e 7322 3a20 5b7b 226e 616d 6522  lumns": [{"name"
-000008b0: 3a20 2269 6422 2c20 2266 6965 6c64 5f6e  : "id", "field_n
-000008c0: 616d 6522 3a20 2269 6422 2c20 2270 616e  ame": "id", "pan
-000008d0: 6461 735f 7479 7065 223a 2022 696e 7436  das_type": "int6
-000008e0: 3422 2c20 226e 756d 7079 5f74 7970 6522  4", "numpy_type"
-000008f0: 3a20 2269 6e74 3634 222c 2022 6d65 7461  : "int64", "meta
-00000900: 6461 7461 223a 206e 756c 6c7d 2c20 7b22  data": null}, {"
-00000910: 6e61 6d65 223a 2022 7261 222c 2022 6669  name": "ra", "fi
-00000920: 656c 645f 6e61 6d65 223a 2022 7261 222c  eld_name": "ra",
-00000930: 2022 7061 6e64 6173 5f74 7970 6522 3a20   "pandas_type": 
-00000940: 2266 6c6f 6174 3634 222c 2022 6e75 6d70  "float64", "nump
-00000950: 795f 7479 7065 223a 2022 666c 6f61 7436  y_type": "float6
-00000960: 3422 2c20 226d 6574 6164 6174 6122 3a20  4", "metadata": 
-00000970: 6e75 6c6c 7d2c 207b 226e 616d 6522 3a20  null}, {"name": 
-00000980: 2264 6563 222c 2022 6669 656c 645f 6e61  "dec", "field_na
-00000990: 6d65 223a 2022 6465 6322 2c20 2270 616e  me": "dec", "pan
-000009a0: 6461 735f 7479 7065 223a 2022 666c 6f61  das_type": "floa
-000009b0: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
-000009c0: 6522 3a20 2266 6c6f 6174 3634 222c 2022  e": "float64", "
-000009d0: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
-000009e0: 2c20 7b22 6e61 6d65 223a 2022 7261 5f65  , {"name": "ra_e
-000009f0: 7272 6f72 222c 2022 6669 656c 645f 6e61  rror", "field_na
-00000a00: 6d65 223a 2022 7261 5f65 7272 6f72 222c  me": "ra_error",
-00000a10: 2022 7061 6e64 6173 5f74 7970 6522 3a20   "pandas_type": 
-00000a20: 2269 6e74 3634 222c 2022 6e75 6d70 795f  "int64", "numpy_
-00000a30: 7479 7065 223a 2022 696e 7436 3422 2c20  type": "int64", 
-00000a40: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
-00000a50: 7d2c 207b 226e 616d 6522 3a20 2264 6563  }, {"name": "dec
-00000a60: 5f65 7272 6f72 222c 2022 6669 656c 645f  _error", "field_
-00000a70: 6e61 6d65 223a 2022 6465 635f 6572 726f  name": "dec_erro
-00000a80: 7222 2c20 2270 616e 6461 735f 7479 7065  r", "pandas_type
-00000a90: 223a 2022 696e 7436 3422 2c20 226e 756d  ": "int64", "num
-00000aa0: 7079 5f74 7970 6522 3a20 2269 6e74 3634  py_type": "int64
-00000ab0: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
-00000ac0: 756c 6c7d 2c20 7b22 6e61 6d65 223a 206e  ull}, {"name": n
-00000ad0: 756c 6c2c 2022 6669 656c 645f 6e61 6d65  ull, "field_name
-00000ae0: 223a 2022 5f5f 696e 6465 785f 6c65 7665  ": "__index_leve
-00000af0: 6c5f 305f 5f22 2c20 2270 616e 6461 735f  l_0__", "pandas_
-00000b00: 7479 7065 223a 2022 696e 7436 3422 2c20  type": "int64", 
-00000b10: 226e 756d 7079 5f74 7970 6522 3a20 2269  "numpy_type": "i
-00000b20: 6e74 3634 222c 2022 6d65 7461 6461 7461  nt64", "metadata
-00000b30: 223a 206e 756c 6c7d 5d2c 2022 6372 6561  ": null}], "crea
-00000b40: 746f 7222 3a20 7b22 6c69 6272 6172 7922  tor": {"library"
-00000b50: 3a20 2270 7961 7272 6f77 222c 2022 7665  : "pyarrow", "ve
-00000b60: 7273 696f 6e22 3a20 2239 2e30 2e30 227d  rsion": "9.0.0"}
-00000b70: 2c20 2270 616e 6461 735f 7665 7273 696f  , "pandas_versio
-00000b80: 6e22 3a20 2231 2e33 2e35 227d 0018 0c41  n": "1.3.5"}...A
-00000b90: 5252 4f57 3a73 6368 656d 6118 c00e 2f2f  RROW:schema...//
-00000ba0: 2f2f 2f32 6746 4141 4151 4141 4141 4141  ///2gFAAAQAAAAAA
-00000bb0: 414b 4141 3441 4267 4146 4141 6741 4367  AKAA4ABgAFAAgACg
-00000bc0: 4141 4141 4142 4241 4151 4141 4141 4141  AAAAABBAAQAAAAAA
-00000bd0: 414b 4141 7741 4141 4145 4141 6741 4367  AKAAwAAAAEAAgACg
-00000be0: 4141 414e 7744 4141 4145 4141 4141 4151  AAANwDAAAEAAAAAQ
-00000bf0: 4141 4141 7741 4141 4149 4141 7741 4241  AAAAwAAAAIAAwABA
-00000c00: 4149 4141 6741 4141 4149 4141 4141 4541  AIAAgAAAAIAAAAEA
-00000c10: 4141 4141 5941 4141 4277 5957 356b 5958  AAAAYAAABwYW5kYX
-00000c20: 4d41 414b 5544 4141 4237 496d 6c75 5a47  MAAKUDAAB7ImluZG
-00000c30: 5634 5832 4e76 6248 5674 626e 4d69 4f69  V4X2NvbHVtbnMiOi
-00000c40: 4262 496c 3966 6157 356b 5a58 6866 6247  BbIl9faW5kZXhfbG
-00000c50: 5632 5a57 7866 4d46 3966 496c 3073 4943  V2ZWxfMF9fIl0sIC
-00000c60: 4a6a 6232 7831 6257 3566 6157 356b 5a58  Jjb2x1bW5faW5kZX
-00000c70: 686c 6379 4936 4946 7437 496d 3568 6257  hlcyI6IFt7Im5hbW
-00000c80: 5569 4f69 4275 6457 7873 4c43 4169 5a6d  UiOiBudWxsLCAiZm
-00000c90: 6c6c 6247 5266 626d 4674 5a53 4936 4947  llbGRfbmFtZSI6IG
-00000ca0: 3531 6247 7773 4943 4a77 5957 356b 5958  51bGwsICJwYW5kYX
-00000cb0: 4e66 6448 6c77 5a53 4936 4943 4a31 626d  NfdHlwZSI6ICJ1bm
-00000cc0: 6c6a 6232 526c 4969 7767 496d 3531 6258  ljb2RlIiwgIm51bX
-00000cd0: 4235 5833 5235 6347 5569 4f69 4169 6232  B5X3R5cGUiOiAib2
-00000ce0: 4a71 5a57 4e30 4969 7767 496d 316c 6447  JqZWN0IiwgIm1ldG
-00000cf0: 466b 5958 5268 496a 6f67 6579 4a6c 626d  FkYXRhIjogeyJlbm
-00000d00: 4e76 5a47 6c75 5a79 4936 4943 4a56 5645  NvZGluZyI6ICJVVE
-00000d10: 5974 4f43 4a39 6656 3073 4943 4a6a 6232  YtOCJ9fV0sICJjb2
-00000d20: 7831 6257 357a 496a 6f67 5733 7369 626d  x1bW5zIjogW3sibm
-00000d30: 4674 5a53 4936 4943 4a70 5a43 4973 4943  FtZSI6ICJpZCIsIC
-00000d40: 4a6d 6157 5673 5a46 3975 5957 316c 496a  JmaWVsZF9uYW1lIj
-00000d50: 6f67 496d 6c6b 4969 7767 496e 4268 626d  ogImlkIiwgInBhbm
-00000d60: 5268 6331 3930 6558 426c 496a 6f67 496d  Rhc190eXBlIjogIm
-00000d70: 6c75 6444 5930 4969 7767 496d 3531 6258  ludDY0IiwgIm51bX
-00000d80: 4235 5833 5235 6347 5569 4f69 4169 6157  B5X3R5cGUiOiAiaW
-00000d90: 3530 4e6a 5169 4c43 4169 6257 5630 5957  50NjQiLCAibWV0YW
-00000da0: 5268 6447 4569 4f69 4275 6457 7873 6653  RhdGEiOiBudWxsfS
-00000db0: 7767 6579 4a75 5957 316c 496a 6f67 496e  wgeyJuYW1lIjogIn
-00000dc0: 4a68 4969 7767 496d 5a70 5a57 786b 5832  JhIiwgImZpZWxkX2
-00000dd0: 3568 6257 5569 4f69 4169 636d 4569 4c43  5hbWUiOiAicmEiLC
-00000de0: 4169 6347 4675 5a47 467a 5833 5235 6347  AicGFuZGFzX3R5cG
-00000df0: 5569 4f69 4169 5a6d 7876 5958 5132 4e43  UiOiAiZmxvYXQ2NC
-00000e00: 4973 4943 4a75 6457 3177 6556 3930 6558  IsICJudW1weV90eX
-00000e10: 426c 496a 6f67 496d 5a73 6232 4630 4e6a  BlIjogImZsb2F0Nj
-00000e20: 5169 4c43 4169 6257 5630 5957 5268 6447  QiLCAibWV0YWRhdG
-00000e30: 4569 4f69 4275 6457 7873 6653 7767 6579  EiOiBudWxsfSwgey
-00000e40: 4a75 5957 316c 496a 6f67 496d 526c 5979  JuYW1lIjogImRlYy
-00000e50: 4973 4943 4a6d 6157 5673 5a46 3975 5957  IsICJmaWVsZF9uYW
-00000e60: 316c 496a 6f67 496d 526c 5979 4973 4943  1lIjogImRlYyIsIC
-00000e70: 4a77 5957 356b 5958 4e66 6448 6c77 5a53  JwYW5kYXNfdHlwZS
-00000e80: 4936 4943 4a6d 6247 3968 6444 5930 4969  I6ICJmbG9hdDY0Ii
-00000e90: 7767 496d 3531 6258 4235 5833 5235 6347  wgIm51bXB5X3R5cG
-00000ea0: 5569 4f69 4169 5a6d 7876 5958 5132 4e43  UiOiAiZmxvYXQ2NC
-00000eb0: 4973 4943 4a74 5a58 5268 5a47 4630 5953  IsICJtZXRhZGF0YS
-00000ec0: 4936 4947 3531 6247 7839 4c43 4237 496d  I6IG51bGx9LCB7Im
-00000ed0: 3568 6257 5569 4f69 4169 636d 4666 5a58  5hbWUiOiAicmFfZX
-00000ee0: 4a79 6233 4969 4c43 4169 5a6d 6c6c 6247  Jyb3IiLCAiZmllbG
-00000ef0: 5266 626d 4674 5a53 4936 4943 4a79 5956  RfbmFtZSI6ICJyYV
-00000f00: 396c 636e 4a76 6369 4973 4943 4a77 5957  9lcnJvciIsICJwYW
-00000f10: 356b 5958 4e66 6448 6c77 5a53 4936 4943  5kYXNfdHlwZSI6IC
-00000f20: 4a70 626e 5132 4e43 4973 4943 4a75 6457  JpbnQ2NCIsICJudW
-00000f30: 3177 6556 3930 6558 426c 496a 6f67 496d  1weV90eXBlIjogIm
-00000f40: 6c75 6444 5930 4969 7767 496d 316c 6447  ludDY0IiwgIm1ldG
-00000f50: 466b 5958 5268 496a 6f67 626e 5673 6248  FkYXRhIjogbnVsbH
-00000f60: 3073 4948 7369 626d 4674 5a53 4936 4943  0sIHsibmFtZSI6IC
-00000f70: 4a6b 5a57 4e66 5a58 4a79 6233 4969 4c43  JkZWNfZXJyb3IiLC
-00000f80: 4169 5a6d 6c6c 6247 5266 626d 4674 5a53  AiZmllbGRfbmFtZS
-00000f90: 4936 4943 4a6b 5a57 4e66 5a58 4a79 6233  I6ICJkZWNfZXJyb3
-00000fa0: 4969 4c43 4169 6347 4675 5a47 467a 5833  IiLCAicGFuZGFzX3
-00000fb0: 5235 6347 5569 4f69 4169 6157 3530 4e6a  R5cGUiOiAiaW50Nj
-00000fc0: 5169 4c43 4169 626e 5674 6348 6c66 6448  QiLCAibnVtcHlfdH
-00000fd0: 6c77 5a53 4936 4943 4a70 626e 5132 4e43  lwZSI6ICJpbnQ2NC
-00000fe0: 4973 4943 4a74 5a58 5268 5a47 4630 5953  IsICJtZXRhZGF0YS
-00000ff0: 4936 4947 3531 6247 7839 4c43 4237 496d  I6IG51bGx9LCB7Im
-00001000: 3568 6257 5569 4f69 4275 6457 7873 4c43  5hbWUiOiBudWxsLC
-00001010: 4169 5a6d 6c6c 6247 5266 626d 4674 5a53  AiZmllbGRfbmFtZS
-00001020: 4936 4943 4a66 5832 6c75 5a47 5634 5832  I6ICJfX2luZGV4X2
-00001030: 786c 646d 5673 587a 4266 5879 4973 4943  xldmVsXzBfXyIsIC
-00001040: 4a77 5957 356b 5958 4e66 6448 6c77 5a53  JwYW5kYXNfdHlwZS
-00001050: 4936 4943 4a70 626e 5132 4e43 4973 4943  I6ICJpbnQ2NCIsIC
-00001060: 4a75 6457 3177 6556 3930 6558 426c 496a  JudW1weV90eXBlIj
-00001070: 6f67 496d 6c75 6444 5930 4969 7767 496d  ogImludDY0IiwgIm
-00001080: 316c 6447 466b 5958 5268 496a 6f67 626e  1ldGFkYXRhIjogbn
-00001090: 5673 6248 3164 4c43 4169 5933 4a6c 5958  VsbH1dLCAiY3JlYX
-000010a0: 5276 6369 4936 4948 7369 6247 6c69 636d  RvciI6IHsibGlicm
-000010b0: 4679 6553 4936 4943 4a77 6557 4679 636d  FyeSI6ICJweWFycm
-000010c0: 3933 4969 7767 496e 5a6c 636e 4e70 6232  93IiwgInZlcnNpb2
-000010d0: 3469 4f69 4169 4f53 3477 4c6a 4169 6653  4iOiAiOS4wLjAifS
-000010e0: 7767 496e 4268 626d 5268 6331 3932 5a58  wgInBhbmRhc192ZX
-000010f0: 4a7a 6157 3975 496a 6f67 496a 4575 4d79  JzaW9uIjogIjEuMy
-00001100: 3431 496e 3041 4141 4147 4141 4141 4a41  41In0AAAAGAAAAJA
-00001110: 4541 414f 4141 4141 4330 4141 4141 6641  EAAOAAAAC0AAAAfA
-00001120: 4141 4145 5141 4141 4145 4141 4141 4250  AAAEQAAAAEAAAABP
-00001130: 2f2f 2f77 4141 4151 4951 4141 4141 4a41  ///wAAAQIQAAAAJA
-00001140: 4141 4141 5141 4141 4141 4141 4141 4551  AAAAQAAAAAAAAAEQ
-00001150: 4141 4146 3966 6157 356b 5a58 6866 6247  AAAF9faW5kZXhfbG
-00001160: 5632 5a57 7866 4d46 3966 4141 4141 4250  V2ZWxfMF9fAAAABP
-00001170: 2f2f 2f77 4141 4141 4641 4141 4141 5150  ///wAAAAFAAAAAQP
-00001180: 2f2f 2f77 4141 4151 4951 4141 4141 4841  ///wAAAQIQAAAAHA
-00001190: 4141 4141 5141 4141 4141 4141 4141 4351  AAAAQAAAAAAAAACQ
-000011a0: 4141 4147 526c 5931 396c 636e 4a76 6367  AAAGRlY19lcnJvcg
-000011b0: 4141 4144 6a2f 2f2f 3841 4141 4142 5141  AAADj///8AAAABQA
-000011c0: 4141 4148 542f 2f2f 3841 4141 4543 4541  AAAHT///8AAAECEA
-000011d0: 4141 4142 7741 4141 4145 4141 4141 4141  AAABwAAAAEAAAAAA
-000011e0: 4141 4141 6741 4141 4279 5956 396c 636e  AAAAgAAAByYV9lcn
-000011f0: 4a76 6367 4141 4141 4273 2f2f 2f2f 4141  JvcgAAAABs////AA
-00001200: 4141 4155 4141 4141 436f 2f2f 2f2f 4141  AAAUAAAACo////AA
-00001210: 4142 4178 4141 4141 4155 4141 4141 4241  ABAxAAAAAUAAAABA
-00001220: 4141 4141 4141 4141 4144 4141 4141 5a47  AAAAAAAAADAAAAZG
-00001230: 566a 414e 622f 2f2f 3841 4141 4941 3050  VjANb///8AAAIA0P
-00001240: 2f2f 2f77 4141 4151 4d51 4141 4141 4841  ///wAAAQMQAAAAHA
-00001250: 4141 4141 5141 4141 4141 4141 4141 4167  AAAAQAAAAAAAAAAg
-00001260: 4141 4148 4a68 4141 4141 4141 5941 4341  AAAHJhAAAAAAYACA
-00001270: 4147 4141 5941 4141 4141 4141 4941 4541  AGAAYAAAAAAAIAEA
-00001280: 4155 4141 6741 4267 4148 4141 7741 4141  AUAAgABgAHAAwAAA
-00001290: 4151 4142 4141 4141 4141 4141 4543 4541  AQABAAAAAAAAECEA
-000012a0: 4141 4142 7741 4141 4145 4141 4141 4141  AAABwAAAAEAAAAAA
-000012b0: 4141 4141 4941 4141 4270 5a41 4141 4341  AAAAIAAABpZAAACA
-000012c0: 414d 4141 6741 4277 4149 4141 4141 4141  AMAAgABwAIAAAAAA
-000012d0: 4141 4155 4141 4141 4141 4141 4141 0018  AAAUAAAAAAAAAA..
-000012e0: 1f70 6172 7175 6574 2d63 7070 2d61 7272  .parquet-cpp-arr
-000012f0: 6f77 2076 6572 7369 6f6e 2039 2e30 2e30  ow version 9.0.0
-00001300: 196c 1c00 001c 0000 1c00 001c 0000 1c00  .l..............
-00001310: 001c 0000 0001 0e00 0050 4152 31         .........PAR1
+00000420: 1510 1502 0000 0015 0419 6c35 0018 0673  ..........l5...s
+00000430: 6368 656d 6115 0a00 1504 2502 1802 6964  chema.....%...id
+00000440: 0015 0a25 0218 0272 6100 150a 2502 1803  ...%...ra...%...
+00000450: 6465 6300 1504 2502 1808 7261 5f65 7272  dec...%...ra_err
+00000460: 6f72 0015 0425 0218 0964 6563 5f65 7272  or...%...dec_err
+00000470: 6f72 0016 0e19 1c19 5c26 8802 1c15 0419  or......\&......
+00000480: 3510 0006 1918 0269 6415 0216 0e16 9c02  5......id.......
+00000490: 1680 0226 7426 081c 1808 2103 0000 0000  ...&t&....!.....
+000004a0: 0000 1808 0c03 0000 0000 0000 1600 2808  ..............(.
+000004b0: 2103 0000 0000 0000 1808 0c03 0000 0000  !...............
+000004c0: 0000 0019 2c15 0415 0015 0200 1500 1510  ....,...........
+000004d0: 1502 0000 0026 bc05 1c15 0a19 3510 0006  .....&......5...
+000004e0: 1918 0272 6115 0216 0e16 8c02 16fc 0126  ...ra..........&
+000004f0: a804 26c0 031c 1808 0000 0000 0068 7440  ..&..........ht@
+00000500: 1808 0000 0000 00c8 7240 1600 2808 0000  ........r@..(...
+00000510: 0000 0068 7440 1808 0000 0000 00c8 7240  ...ht@........r@
+00000520: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
+00000530: 0000 0026 fe08 1c15 0a19 3510 0006 1918  ...&......5.....
+00000540: 0364 6563 1502 160e 169c 0216 8602 26ea  .dec..........&.
+00000550: 0726 f806 1c18 0800 0000 0000 c047 c018  .&...........G..
+00000560: 0800 0000 0000 6051 c016 0028 0800 0000  ......`Q...(....
+00000570: 0000 c047 c018 0800 0000 0000 6051 c000  ...G........`Q..
+00000580: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
+00000590: 0000 26fc 0b1c 1504 1935 1000 0619 1808  ..&......5......
+000005a0: 7261 5f65 7272 6f72 1502 160e 16b8 0116  ra_error........
+000005b0: c001 26ec 0a26 bc0a 1c18 0800 0000 0000  ..&..&..........
+000005c0: 0000 0018 0800 0000 0000 0000 0016 0028  ...............(
+000005d0: 0800 0000 0000 0000 0018 0800 0000 0000  ................
+000005e0: 0000 0000 192c 1504 1500 1502 0015 0015  .....,..........
+000005f0: 1015 0200 0000 2684 0f1c 1504 1935 1000  ......&......5..
+00000600: 0619 1809 6465 635f 6572 726f 7215 0216  ....dec_error...
+00000610: 0e16 b801 16c0 0126 f40d 26c4 0d1c 1808  .......&..&.....
+00000620: 0000 0000 0000 0000 1808 0000 0000 0000  ................
+00000630: 0000 1600 2808 0000 0000 0000 0000 1808  ....(...........
+00000640: 0000 0000 0000 0000 0019 2c15 0415 0015  ..........,.....
+00000650: 0200 1500 1510 1502 0000 0016 b409 160e  ................
+00000660: 2608 1682 0914 0000 192c 1806 7061 6e64  &........,..pand
+00000670: 6173 18a7 057b 2269 6e64 6578 5f63 6f6c  as...{"index_col
+00000680: 756d 6e73 223a 205b 5d2c 2022 636f 6c75  umns": [], "colu
+00000690: 6d6e 5f69 6e64 6578 6573 223a 205b 5d2c  mn_indexes": [],
+000006a0: 2022 636f 6c75 6d6e 7322 3a20 5b7b 226e   "columns": [{"n
+000006b0: 616d 6522 3a20 2269 6422 2c20 2266 6965  ame": "id", "fie
+000006c0: 6c64 5f6e 616d 6522 3a20 2269 6422 2c20  ld_name": "id", 
+000006d0: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
+000006e0: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
+000006f0: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
+00000700: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
+00000710: 2c20 7b22 6e61 6d65 223a 2022 7261 222c  , {"name": "ra",
+00000720: 2022 6669 656c 645f 6e61 6d65 223a 2022   "field_name": "
+00000730: 7261 222c 2022 7061 6e64 6173 5f74 7970  ra", "pandas_typ
+00000740: 6522 3a20 2266 6c6f 6174 3634 222c 2022  e": "float64", "
+00000750: 6e75 6d70 795f 7479 7065 223a 2022 666c  numpy_type": "fl
+00000760: 6f61 7436 3422 2c20 226d 6574 6164 6174  oat64", "metadat
+00000770: 6122 3a20 6e75 6c6c 7d2c 207b 226e 616d  a": null}, {"nam
+00000780: 6522 3a20 2264 6563 222c 2022 6669 656c  e": "dec", "fiel
+00000790: 645f 6e61 6d65 223a 2022 6465 6322 2c20  d_name": "dec", 
+000007a0: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
+000007b0: 666c 6f61 7436 3422 2c20 226e 756d 7079  float64", "numpy
+000007c0: 5f74 7970 6522 3a20 2266 6c6f 6174 3634  _type": "float64
+000007d0: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
+000007e0: 756c 6c7d 2c20 7b22 6e61 6d65 223a 2022  ull}, {"name": "
+000007f0: 7261 5f65 7272 6f72 222c 2022 6669 656c  ra_error", "fiel
+00000800: 645f 6e61 6d65 223a 2022 7261 5f65 7272  d_name": "ra_err
+00000810: 6f72 222c 2022 7061 6e64 6173 5f74 7970  or", "pandas_typ
+00000820: 6522 3a20 2269 6e74 3634 222c 2022 6e75  e": "int64", "nu
+00000830: 6d70 795f 7479 7065 223a 2022 696e 7436  mpy_type": "int6
+00000840: 3422 2c20 226d 6574 6164 6174 6122 3a20  4", "metadata": 
+00000850: 6e75 6c6c 7d2c 207b 226e 616d 6522 3a20  null}, {"name": 
+00000860: 2264 6563 5f65 7272 6f72 222c 2022 6669  "dec_error", "fi
+00000870: 656c 645f 6e61 6d65 223a 2022 6465 635f  eld_name": "dec_
+00000880: 6572 726f 7222 2c20 2270 616e 6461 735f  error", "pandas_
+00000890: 7479 7065 223a 2022 696e 7436 3422 2c20  type": "int64", 
+000008a0: 226e 756d 7079 5f74 7970 6522 3a20 2269  "numpy_type": "i
+000008b0: 6e74 3634 222c 2022 6d65 7461 6461 7461  nt64", "metadata
+000008c0: 223a 206e 756c 6c7d 5d2c 2022 6372 6561  ": null}], "crea
+000008d0: 746f 7222 3a20 7b22 6c69 6272 6172 7922  tor": {"library"
+000008e0: 3a20 2270 7961 7272 6f77 222c 2022 7665  : "pyarrow", "ve
+000008f0: 7273 696f 6e22 3a20 2239 2e30 2e30 227d  rsion": "9.0.0"}
+00000900: 2c20 2270 616e 6461 735f 7665 7273 696f  , "pandas_versio
+00000910: 6e22 3a20 2232 2e30 2e30 227d 0018 0c41  n": "2.0.0"}...A
+00000920: 5252 4f57 3a73 6368 656d 6118 980b 2f2f  RROW:schema...//
+00000930: 2f2f 2f79 6745 4141 4151 4141 4141 4141  ///ygEAAAQAAAAAA
+00000940: 414b 4141 3441 4267 4146 4141 6741 4367  AKAA4ABgAFAAgACg
+00000950: 4141 4141 4142 4241 4151 4141 4141 4141  AAAAABBAAQAAAAAA
+00000960: 414b 4141 7741 4141 4145 4141 6741 4367  AKAAwAAAAEAAgACg
+00000970: 4141 414e 7743 4141 4145 4141 4141 4151  AAANwCAAAEAAAAAQ
+00000980: 4141 4141 7741 4141 4149 4141 7741 4241  AAAAwAAAAIAAwABA
+00000990: 4149 4141 6741 4141 4149 4141 4141 4541  AIAAgAAAAIAAAAEA
+000009a0: 4141 4141 5941 4141 4277 5957 356b 5958  AAAAYAAABwYW5kYX
+000009b0: 4d41 414b 6343 4141 4237 496d 6c75 5a47  MAAKcCAAB7ImluZG
+000009c0: 5634 5832 4e76 6248 5674 626e 4d69 4f69  V4X2NvbHVtbnMiOi
+000009d0: 4262 5853 7767 496d 4e76 6248 5674 626c  BbXSwgImNvbHVtbl
+000009e0: 3970 626d 526c 6547 567a 496a 6f67 5731  9pbmRleGVzIjogW1
+000009f0: 3073 4943 4a6a 6232 7831 6257 357a 496a  0sICJjb2x1bW5zIj
+00000a00: 6f67 5733 7369 626d 4674 5a53 4936 4943  ogW3sibmFtZSI6IC
+00000a10: 4a70 5a43 4973 4943 4a6d 6157 5673 5a46  JpZCIsICJmaWVsZF
+00000a20: 3975 5957 316c 496a 6f67 496d 6c6b 4969  9uYW1lIjogImlkIi
+00000a30: 7767 496e 4268 626d 5268 6331 3930 6558  wgInBhbmRhc190eX
+00000a40: 426c 496a 6f67 496d 6c75 6444 5930 4969  BlIjogImludDY0Ii
+00000a50: 7767 496d 3531 6258 4235 5833 5235 6347  wgIm51bXB5X3R5cG
+00000a60: 5569 4f69 4169 6157 3530 4e6a 5169 4c43  UiOiAiaW50NjQiLC
+00000a70: 4169 6257 5630 5957 5268 6447 4569 4f69  AibWV0YWRhdGEiOi
+00000a80: 4275 6457 7873 6653 7767 6579 4a75 5957  BudWxsfSwgeyJuYW
+00000a90: 316c 496a 6f67 496e 4a68 4969 7767 496d  1lIjogInJhIiwgIm
+00000aa0: 5a70 5a57 786b 5832 3568 6257 5569 4f69  ZpZWxkX25hbWUiOi
+00000ab0: 4169 636d 4569 4c43 4169 6347 4675 5a47  AicmEiLCAicGFuZG
+00000ac0: 467a 5833 5235 6347 5569 4f69 4169 5a6d  FzX3R5cGUiOiAiZm
+00000ad0: 7876 5958 5132 4e43 4973 4943 4a75 6457  xvYXQ2NCIsICJudW
+00000ae0: 3177 6556 3930 6558 426c 496a 6f67 496d  1weV90eXBlIjogIm
+00000af0: 5a73 6232 4630 4e6a 5169 4c43 4169 6257  Zsb2F0NjQiLCAibW
+00000b00: 5630 5957 5268 6447 4569 4f69 4275 6457  V0YWRhdGEiOiBudW
+00000b10: 7873 6653 7767 6579 4a75 5957 316c 496a  xsfSwgeyJuYW1lIj
+00000b20: 6f67 496d 526c 5979 4973 4943 4a6d 6157  ogImRlYyIsICJmaW
+00000b30: 5673 5a46 3975 5957 316c 496a 6f67 496d  VsZF9uYW1lIjogIm
+00000b40: 526c 5979 4973 4943 4a77 5957 356b 5958  RlYyIsICJwYW5kYX
+00000b50: 4e66 6448 6c77 5a53 4936 4943 4a6d 6247  NfdHlwZSI6ICJmbG
+00000b60: 3968 6444 5930 4969 7767 496d 3531 6258  9hdDY0IiwgIm51bX
+00000b70: 4235 5833 5235 6347 5569 4f69 4169 5a6d  B5X3R5cGUiOiAiZm
+00000b80: 7876 5958 5132 4e43 4973 4943 4a74 5a58  xvYXQ2NCIsICJtZX
+00000b90: 5268 5a47 4630 5953 4936 4947 3531 6247  RhZGF0YSI6IG51bG
+00000ba0: 7839 4c43 4237 496d 3568 6257 5569 4f69  x9LCB7Im5hbWUiOi
+00000bb0: 4169 636d 4666 5a58 4a79 6233 4969 4c43  AicmFfZXJyb3IiLC
+00000bc0: 4169 5a6d 6c6c 6247 5266 626d 4674 5a53  AiZmllbGRfbmFtZS
+00000bd0: 4936 4943 4a79 5956 396c 636e 4a76 6369  I6ICJyYV9lcnJvci
+00000be0: 4973 4943 4a77 5957 356b 5958 4e66 6448  IsICJwYW5kYXNfdH
+00000bf0: 6c77 5a53 4936 4943 4a70 626e 5132 4e43  lwZSI6ICJpbnQ2NC
+00000c00: 4973 4943 4a75 6457 3177 6556 3930 6558  IsICJudW1weV90eX
+00000c10: 426c 496a 6f67 496d 6c75 6444 5930 4969  BlIjogImludDY0Ii
+00000c20: 7767 496d 316c 6447 466b 5958 5268 496a  wgIm1ldGFkYXRhIj
+00000c30: 6f67 626e 5673 6248 3073 4948 7369 626d  ogbnVsbH0sIHsibm
+00000c40: 4674 5a53 4936 4943 4a6b 5a57 4e66 5a58  FtZSI6ICJkZWNfZX
+00000c50: 4a79 6233 4969 4c43 4169 5a6d 6c6c 6247  Jyb3IiLCAiZmllbG
+00000c60: 5266 626d 4674 5a53 4936 4943 4a6b 5a57  RfbmFtZSI6ICJkZW
+00000c70: 4e66 5a58 4a79 6233 4969 4c43 4169 6347  NfZXJyb3IiLCAicG
+00000c80: 4675 5a47 467a 5833 5235 6347 5569 4f69  FuZGFzX3R5cGUiOi
+00000c90: 4169 6157 3530 4e6a 5169 4c43 4169 626e  AiaW50NjQiLCAibn
+00000ca0: 5674 6348 6c66 6448 6c77 5a53 4936 4943  VtcHlfdHlwZSI6IC
+00000cb0: 4a70 626e 5132 4e43 4973 4943 4a74 5a58  JpbnQ2NCIsICJtZX
+00000cc0: 5268 5a47 4630 5953 4936 4947 3531 6247  RhZGF0YSI6IG51bG
+00000cd0: 7839 5853 7767 496d 4e79 5a57 4630 6233  x9XSwgImNyZWF0b3
+00000ce0: 4969 4f69 4237 496d 7870 596e 4a68 636e  IiOiB7ImxpYnJhcn
+00000cf0: 6b69 4f69 4169 6348 6c68 636e 4a76 6479  kiOiAicHlhcnJvdy
+00000d00: 4973 4943 4a32 5a58 4a7a 6157 3975 496a  IsICJ2ZXJzaW9uIj
+00000d10: 6f67 496a 6b75 4d43 3477 496e 3073 4943  ogIjkuMC4wIn0sIC
+00000d20: 4a77 5957 356b 5958 4e66 646d 5679 6332  JwYW5kYXNfdmVyc2
+00000d30: 6c76 6269 4936 4943 4979 4c6a 4175 4d43  lvbiI6ICIyLjAuMC
+00000d40: 4a39 4141 5541 4141 446b 4141 4141 6f41  J9AAUAAADkAAAAoA
+00000d50: 4141 4148 5141 4141 4138 4141 4141 4241  AAAHQAAAA8AAAABA
+00000d60: 4141 4145 442f 2f2f 3841 4141 4543 4541  AAAED///8AAAECEA
+00000d70: 4141 4142 7741 4141 4145 4141 4141 4141  AAABwAAAAEAAAAAA
+00000d80: 4141 4141 6b41 4141 426b 5a57 4e66 5a58  AAAAkAAABkZWNfZX
+00000d90: 4a79 6233 4941 4141 4134 2f2f 2f2f 4141  Jyb3IAAAA4////AA
+00000da0: 4141 4155 4141 4141 4230 2f2f 2f2f 4141  AAAUAAAAB0////AA
+00000db0: 4142 4168 4141 4141 4163 4141 4141 4241  ABAhAAAAAcAAAABA
+00000dc0: 4141 4141 4141 4141 4149 4141 4141 636d  AAAAAAAAAIAAAAcm
+00000dd0: 4666 5a58 4a79 6233 4941 4141 4141 6250  FfZXJyb3IAAAAAbP
+00000de0: 2f2f 2f77 4141 4141 4641 4141 4141 7150  ///wAAAAFAAAAAqP
+00000df0: 2f2f 2f77 4141 4151 4d51 4141 4141 4641  ///wAAAQMQAAAAFA
+00000e00: 4141 4141 5141 4141 4141 4141 4141 4177  AAAAQAAAAAAAAAAw
+00000e10: 4141 4147 526c 5977 4457 2f2f 2f2f 4141  AAAGRlYwDW////AA
+00000e20: 4143 414e 442f 2f2f 3841 4141 4544 4541  ACAND///8AAAEDEA
+00000e30: 4141 4142 7741 4141 4145 4141 4141 4141  AAABwAAAAEAAAAAA
+00000e40: 4141 4141 4941 4141 4279 5951 4141 4141  AAAAIAAAByYQAAAA
+00000e50: 4147 4141 6741 4267 4147 4141 4141 4141  AGAAgABgAGAAAAAA
+00000e60: 4143 4142 4141 4641 4149 4141 5941 4277  ACABAAFAAIAAYABw
+00000e70: 414d 4141 4141 4541 4151 4141 4141 4141  AMAAAAEAAQAAAAAA
+00000e80: 4142 4168 4141 4141 4163 4141 4141 4241  ABAhAAAAAcAAAABA
+00000e90: 4141 4141 4141 4141 4143 4141 4141 6157  AAAAAAAAACAAAAaW
+00000ea0: 5141 4141 6741 4441 4149 4141 6341 4341  QAAAgADAAIAAcACA
+00000eb0: 4141 4141 4141 4141 4641 4141 4141 4141  AAAAAAAAFAAAAAAA
+00000ec0: 4141 4141 3d3d 0018 1f70 6172 7175 6574  AAAA==...parquet
+00000ed0: 2d63 7070 2d61 7272 6f77 2076 6572 7369  -cpp-arrow versi
+00000ee0: 6f6e 2039 2e30 2e30 195c 1c00 001c 0000  on 9.0.0.\......
+00000ef0: 1c00 001c 0000 1c00 0000 d30a 0000 5041  ..............PA
+00000f00: 5231                                     R1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_44/shard_1.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet`

 * *Files 16% similar despite different names*

```diff
@@ -58,247 +58,182 @@
 00000390: 0000 0000 0000 0920 0200 0000 0a01 010a  ....... ........
 000003a0: 0026 c20e 1c15 0419 3510 0006 1918 0964  .&......5......d
 000003b0: 6563 5f65 7272 6f72 1502 160a 16b8 0116  ec_error........
 000003c0: c001 26b2 0d26 820d 1c18 0800 0000 0000  ..&..&..........
 000003d0: 0000 0018 0800 0000 0000 0000 0016 0028  ...............(
 000003e0: 0800 0000 0000 0000 0018 0800 0000 0000  ................
 000003f0: 0000 0000 192c 1504 1500 1502 0015 0015  .....,..........
-00000400: 1015 0200 0000 1504 1550 1540 4c15 0a15  .........P.@L...
-00000410: 0012 0000 2804 0300 0901 0007 0907 0400  ....(...........
-00000420: 100d 083c 1200 0000 0000 0000 1700 0000  ...<............
-00000430: 0000 0000 1500 1516 151a 2c15 0a15 1015  ..........,.....
-00000440: 0615 061c 1808 1700 0000 0000 0000 1808  ................
-00000450: 0300 0000 0000 0000 1600 2808 1700 0000  ..........(.....
-00000460: 0000 0000 1808 0300 0000 0000 0000 0000  ................
-00000470: 000b 2802 0000 000a 0103 0388 4600 26fc  ..(.........F.&.
-00000480: 111c 1504 1935 1000 0619 1811 5f5f 696e  .....5......__in
-00000490: 6465 785f 6c65 7665 6c5f 305f 5f15 0216  dex_level_0__...
-000004a0: 0a16 fc01 16f0 0126 e810 268c 101c 1808  .......&..&.....
-000004b0: 1700 0000 0000 0000 1808 0300 0000 0000  ................
-000004c0: 0000 1600 2808 1700 0000 0000 0000 1808  ....(...........
-000004d0: 0300 0000 0000 0000 0019 2c15 0415 0015  ..........,.....
-000004e0: 0200 1500 1510 1502 0000 0015 0419 7c35  ..............|5
-000004f0: 0018 0673 6368 656d 6115 0c00 1504 2502  ...schema.....%.
-00000500: 1802 6964 0015 0a25 0218 0272 6100 150a  ..id...%...ra...
-00000510: 2502 1803 6465 6300 1504 2502 1808 7261  %...dec...%...ra
-00000520: 5f65 7272 6f72 0015 0425 0218 0964 6563  _error...%...dec
-00000530: 5f65 7272 6f72 0015 0425 0218 115f 5f69  _error...%...__i
-00000540: 6e64 6578 5f6c 6576 656c 5f30 5f5f 0016  ndex_level_0__..
-00000550: 0a19 1c19 6c26 f801 1c15 0419 3510 0006  ....l&......5...
-00000560: 1918 0269 6415 0216 0a16 fc01 16f0 0126  ...id..........&
-00000570: 6426 081c 1808 d302 0000 0000 0000 1808  d&..............
-00000580: bf02 0000 0000 0000 1600 2808 d302 0000  ..........(.....
-00000590: 0000 0000 1808 bf02 0000 0000 0000 0019  ................
-000005a0: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
-000005b0: 0026 a205 1c15 0a19 3510 0006 1918 0272  .&......5......r
-000005c0: 6115 0216 0a16 fc01 16f2 0126 8e04 26b0  a..........&..&.
-000005d0: 031c 1808 0000 0000 00b8 7340 1808 0000  ..........s@....
-000005e0: 0000 00e8 7140 1600 2808 0000 0000 00b8  ....q@..(.......
-000005f0: 7340 1808 0000 0000 00e8 7140 0019 2c15  s@........q@..,.
-00000600: 0415 0015 0200 1500 1510 1502 0000 0026  ...............&
-00000610: bc08 1c15 0a19 3510 0006 1918 0364 6563  ......5......dec
-00000620: 1502 160a 16da 0116 de01 26aa 0726 de06  ..........&..&..
-00000630: 1c18 0800 0000 0000 404e c018 0800 0000  ........@N......
-00000640: 0000 6051 c016 0028 0800 0000 0000 404e  ..`Q...(......@N
-00000650: c018 0800 0000 0000 6051 c000 192c 1504  ........`Q...,..
-00000660: 1500 1502 0015 0015 1015 0200 0000 26ba  ..............&.
-00000670: 0b1c 1504 1935 1000 0619 1808 7261 5f65  .....5......ra_e
-00000680: 7272 6f72 1502 160a 16b8 0116 c001 26aa  rror..........&.
-00000690: 0a26 fa09 1c18 0800 0000 0000 0000 0018  .&..............
-000006a0: 0800 0000 0000 0000 0016 0028 0800 0000  ...........(....
-000006b0: 0000 0000 0018 0800 0000 0000 0000 0000  ................
-000006c0: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
-000006d0: 0000 26c2 0e1c 1504 1935 1000 0619 1809  ..&......5......
-000006e0: 6465 635f 6572 726f 7215 0216 0a16 b801  dec_error.......
-000006f0: 16c0 0126 b20d 2682 0d1c 1808 0000 0000  ...&..&.........
-00000700: 0000 0000 1808 0000 0000 0000 0000 1600  ................
-00000710: 2808 0000 0000 0000 0000 1808 0000 0000  (...............
-00000720: 0000 0000 0019 2c15 0415 0015 0200 1500  ......,.........
-00000730: 1510 1502 0000 0026 fc11 1c15 0419 3510  .......&......5.
-00000740: 0006 1918 115f 5f69 6e64 6578 5f6c 6576  .....__index_lev
-00000750: 656c 5f30 5f5f 1502 160a 16fc 0116 f001  el_0__..........
-00000760: 26e8 1026 8c10 1c18 0817 0000 0000 0000  &..&............
-00000770: 0018 0803 0000 0000 0000 0016 0028 0817  .............(..
-00000780: 0000 0000 0000 0018 0803 0000 0000 0000  ................
-00000790: 0000 192c 1504 1500 1502 0015 0015 1015  ...,............
-000007a0: 0200 0000 16be 0a16 0a26 0816 b00a 1400  .........&......
-000007b0: 0019 2c18 0670 616e 6461 7318 a507 7b22  ..,..pandas...{"
-000007c0: 696e 6465 785f 636f 6c75 6d6e 7322 3a20  index_columns": 
-000007d0: 5b22 5f5f 696e 6465 785f 6c65 7665 6c5f  ["__index_level_
-000007e0: 305f 5f22 5d2c 2022 636f 6c75 6d6e 5f69  0__"], "column_i
-000007f0: 6e64 6578 6573 223a 205b 7b22 6e61 6d65  ndexes": [{"name
-00000800: 223a 206e 756c 6c2c 2022 6669 656c 645f  ": null, "field_
-00000810: 6e61 6d65 223a 206e 756c 6c2c 2022 7061  name": null, "pa
-00000820: 6e64 6173 5f74 7970 6522 3a20 2275 6e69  ndas_type": "uni
-00000830: 636f 6465 222c 2022 6e75 6d70 795f 7479  code", "numpy_ty
-00000840: 7065 223a 2022 6f62 6a65 6374 222c 2022  pe": "object", "
-00000850: 6d65 7461 6461 7461 223a 207b 2265 6e63  metadata": {"enc
-00000860: 6f64 696e 6722 3a20 2255 5446 2d38 227d  oding": "UTF-8"}
-00000870: 7d5d 2c20 2263 6f6c 756d 6e73 223a 205b  }], "columns": [
-00000880: 7b22 6e61 6d65 223a 2022 6964 222c 2022  {"name": "id", "
-00000890: 6669 656c 645f 6e61 6d65 223a 2022 6964  field_name": "id
-000008a0: 222c 2022 7061 6e64 6173 5f74 7970 6522  ", "pandas_type"
-000008b0: 3a20 2269 6e74 3634 222c 2022 6e75 6d70  : "int64", "nump
-000008c0: 795f 7479 7065 223a 2022 696e 7436 3422  y_type": "int64"
-000008d0: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
-000008e0: 6c6c 7d2c 207b 226e 616d 6522 3a20 2272  ll}, {"name": "r
-000008f0: 6122 2c20 2266 6965 6c64 5f6e 616d 6522  a", "field_name"
-00000900: 3a20 2272 6122 2c20 2270 616e 6461 735f  : "ra", "pandas_
-00000910: 7479 7065 223a 2022 666c 6f61 7436 3422  type": "float64"
-00000920: 2c20 226e 756d 7079 5f74 7970 6522 3a20  , "numpy_type": 
-00000930: 2266 6c6f 6174 3634 222c 2022 6d65 7461  "float64", "meta
-00000940: 6461 7461 223a 206e 756c 6c7d 2c20 7b22  data": null}, {"
-00000950: 6e61 6d65 223a 2022 6465 6322 2c20 2266  name": "dec", "f
-00000960: 6965 6c64 5f6e 616d 6522 3a20 2264 6563  ield_name": "dec
-00000970: 222c 2022 7061 6e64 6173 5f74 7970 6522  ", "pandas_type"
-00000980: 3a20 2266 6c6f 6174 3634 222c 2022 6e75  : "float64", "nu
-00000990: 6d70 795f 7479 7065 223a 2022 666c 6f61  mpy_type": "floa
-000009a0: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
-000009b0: 3a20 6e75 6c6c 7d2c 207b 226e 616d 6522  : null}, {"name"
-000009c0: 3a20 2272 615f 6572 726f 7222 2c20 2266  : "ra_error", "f
-000009d0: 6965 6c64 5f6e 616d 6522 3a20 2272 615f  ield_name": "ra_
-000009e0: 6572 726f 7222 2c20 2270 616e 6461 735f  error", "pandas_
-000009f0: 7479 7065 223a 2022 696e 7436 3422 2c20  type": "int64", 
-00000a00: 226e 756d 7079 5f74 7970 6522 3a20 2269  "numpy_type": "i
-00000a10: 6e74 3634 222c 2022 6d65 7461 6461 7461  nt64", "metadata
-00000a20: 223a 206e 756c 6c7d 2c20 7b22 6e61 6d65  ": null}, {"name
-00000a30: 223a 2022 6465 635f 6572 726f 7222 2c20  ": "dec_error", 
-00000a40: 2266 6965 6c64 5f6e 616d 6522 3a20 2264  "field_name": "d
-00000a50: 6563 5f65 7272 6f72 222c 2022 7061 6e64  ec_error", "pand
-00000a60: 6173 5f74 7970 6522 3a20 2269 6e74 3634  as_type": "int64
-00000a70: 222c 2022 6e75 6d70 795f 7479 7065 223a  ", "numpy_type":
-00000a80: 2022 696e 7436 3422 2c20 226d 6574 6164   "int64", "metad
-00000a90: 6174 6122 3a20 6e75 6c6c 7d2c 207b 226e  ata": null}, {"n
-00000aa0: 616d 6522 3a20 6e75 6c6c 2c20 2266 6965  ame": null, "fie
-00000ab0: 6c64 5f6e 616d 6522 3a20 225f 5f69 6e64  ld_name": "__ind
-00000ac0: 6578 5f6c 6576 656c 5f30 5f5f 222c 2022  ex_level_0__", "
-00000ad0: 7061 6e64 6173 5f74 7970 6522 3a20 2269  pandas_type": "i
-00000ae0: 6e74 3634 222c 2022 6e75 6d70 795f 7479  nt64", "numpy_ty
-00000af0: 7065 223a 2022 696e 7436 3422 2c20 226d  pe": "int64", "m
-00000b00: 6574 6164 6174 6122 3a20 6e75 6c6c 7d5d  etadata": null}]
-00000b10: 2c20 2263 7265 6174 6f72 223a 207b 226c  , "creator": {"l
-00000b20: 6962 7261 7279 223a 2022 7079 6172 726f  ibrary": "pyarro
-00000b30: 7722 2c20 2276 6572 7369 6f6e 223a 2022  w", "version": "
-00000b40: 392e 302e 3022 7d2c 2022 7061 6e64 6173  9.0.0"}, "pandas
-00000b50: 5f76 6572 7369 6f6e 223a 2022 312e 332e  _version": "1.3.
-00000b60: 3522 7d00 180c 4152 524f 573a 7363 6865  5"}...ARROW:sche
-00000b70: 6d61 18c0 0e2f 2f2f 2f2f 3267 4641 4141  ma.../////2gFAAA
-00000b80: 5141 4141 4141 4141 4b41 4134 4142 6741  QAAAAAAAKAA4ABgA
-00000b90: 4641 4167 4143 6741 4141 4141 4242 4141  FAAgACgAAAAABBAA
-00000ba0: 5141 4141 4141 4141 4b41 4177 4141 4141  QAAAAAAAKAAwAAAA
-00000bb0: 4541 4167 4143 6741 4141 4e77 4441 4141  EAAgACgAAANwDAAA
-00000bc0: 4541 4141 4141 5141 4141 4177 4141 4141  EAAAAAQAAAAwAAAA
-00000bd0: 4941 4177 4142 4141 4941 4167 4141 4141  IAAwABAAIAAgAAAA
-00000be0: 4941 4141 4145 4141 4141 4159 4141 4142  IAAAAEAAAAAYAAAB
-00000bf0: 7759 5735 6b59 584d 4141 4b55 4441 4142  wYW5kYXMAAKUDAAB
-00000c00: 3749 6d6c 755a 4756 3458 324e 7662 4856  7ImluZGV4X2NvbHV
-00000c10: 7462 6e4d 694f 6942 6249 6c39 6661 5735  tbnMiOiBbIl9faW5
-00000c20: 6b5a 5868 6662 4756 325a 5778 664d 4639  kZXhfbGV2ZWxfMF9
-00000c30: 6649 6c30 7349 434a 6a62 3278 3162 5735  fIl0sICJjb2x1bW5
-00000c40: 6661 5735 6b5a 5868 6c63 7949 3649 4674  faW5kZXhlcyI6IFt
-00000c50: 3749 6d35 6862 5755 694f 6942 7564 5778  7Im5hbWUiOiBudWx
-00000c60: 734c 4341 695a 6d6c 6c62 4752 6662 6d46  sLCAiZmllbGRfbmF
-00000c70: 745a 5349 3649 4735 3162 4777 7349 434a  tZSI6IG51bGwsICJ
-00000c80: 7759 5735 6b59 584e 6664 486c 775a 5349  wYW5kYXNfdHlwZSI
-00000c90: 3649 434a 3162 6d6c 6a62 3252 6c49 6977  6ICJ1bmljb2RlIiw
-00000ca0: 6749 6d35 3162 5842 3558 3352 3563 4755  gIm51bXB5X3R5cGU
-00000cb0: 694f 6941 6962 324a 715a 574e 3049 6977  iOiAib2JqZWN0Iiw
-00000cc0: 6749 6d31 6c64 4746 6b59 5852 6849 6a6f  gIm1ldGFkYXRhIjo
-00000cd0: 6765 794a 6c62 6d4e 765a 476c 755a 7949  geyJlbmNvZGluZyI
-00000ce0: 3649 434a 5656 4559 744f 434a 3966 5630  6ICJVVEYtOCJ9fV0
-00000cf0: 7349 434a 6a62 3278 3162 5735 7a49 6a6f  sICJjb2x1bW5zIjo
-00000d00: 6757 3373 6962 6d46 745a 5349 3649 434a  gW3sibmFtZSI6ICJ
-00000d10: 705a 4349 7349 434a 6d61 5756 735a 4639  pZCIsICJmaWVsZF9
-00000d20: 7559 5731 6c49 6a6f 6749 6d6c 6b49 6977  uYW1lIjogImlkIiw
-00000d30: 6749 6e42 6862 6d52 6863 3139 3065 5842  gInBhbmRhc190eXB
-00000d40: 6c49 6a6f 6749 6d6c 7564 4459 3049 6977  lIjogImludDY0Iiw
-00000d50: 6749 6d35 3162 5842 3558 3352 3563 4755  gIm51bXB5X3R5cGU
-00000d60: 694f 6941 6961 5735 304e 6a51 694c 4341  iOiAiaW50NjQiLCA
-00000d70: 6962 5756 3059 5752 6864 4745 694f 6942  ibWV0YWRhdGEiOiB
-00000d80: 7564 5778 7366 5377 6765 794a 7559 5731  udWxsfSwgeyJuYW1
-00000d90: 6c49 6a6f 6749 6e4a 6849 6977 6749 6d5a  lIjogInJhIiwgImZ
-00000da0: 705a 5778 6b58 3235 6862 5755 694f 6941  pZWxkX25hbWUiOiA
-00000db0: 6963 6d45 694c 4341 6963 4746 755a 4746  icmEiLCAicGFuZGF
-00000dc0: 7a58 3352 3563 4755 694f 6941 695a 6d78  zX3R5cGUiOiAiZmx
-00000dd0: 7659 5851 324e 4349 7349 434a 7564 5731  vYXQ2NCIsICJudW1
-00000de0: 7765 5639 3065 5842 6c49 6a6f 6749 6d5a  weV90eXBlIjogImZ
-00000df0: 7362 3246 304e 6a51 694c 4341 6962 5756  sb2F0NjQiLCAibWV
-00000e00: 3059 5752 6864 4745 694f 6942 7564 5778  0YWRhdGEiOiBudWx
-00000e10: 7366 5377 6765 794a 7559 5731 6c49 6a6f  sfSwgeyJuYW1lIjo
-00000e20: 6749 6d52 6c59 7949 7349 434a 6d61 5756  gImRlYyIsICJmaWV
-00000e30: 735a 4639 7559 5731 6c49 6a6f 6749 6d52  sZF9uYW1lIjogImR
-00000e40: 6c59 7949 7349 434a 7759 5735 6b59 584e  lYyIsICJwYW5kYXN
-00000e50: 6664 486c 775a 5349 3649 434a 6d62 4739  fdHlwZSI6ICJmbG9
-00000e60: 6864 4459 3049 6977 6749 6d35 3162 5842  hdDY0IiwgIm51bXB
-00000e70: 3558 3352 3563 4755 694f 6941 695a 6d78  5X3R5cGUiOiAiZmx
-00000e80: 7659 5851 324e 4349 7349 434a 745a 5852  vYXQ2NCIsICJtZXR
-00000e90: 685a 4746 3059 5349 3649 4735 3162 4778  hZGF0YSI6IG51bGx
-00000ea0: 394c 4342 3749 6d35 6862 5755 694f 6941  9LCB7Im5hbWUiOiA
-00000eb0: 6963 6d46 665a 584a 7962 3349 694c 4341  icmFfZXJyb3IiLCA
-00000ec0: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
-00000ed0: 3649 434a 7959 5639 6c63 6e4a 7663 6949  6ICJyYV9lcnJvciI
-00000ee0: 7349 434a 7759 5735 6b59 584e 6664 486c  sICJwYW5kYXNfdHl
-00000ef0: 775a 5349 3649 434a 7062 6e51 324e 4349  wZSI6ICJpbnQ2NCI
-00000f00: 7349 434a 7564 5731 7765 5639 3065 5842  sICJudW1weV90eXB
-00000f10: 6c49 6a6f 6749 6d6c 7564 4459 3049 6977  lIjogImludDY0Iiw
-00000f20: 6749 6d31 6c64 4746 6b59 5852 6849 6a6f  gIm1ldGFkYXRhIjo
-00000f30: 6762 6e56 7362 4830 7349 4873 6962 6d46  gbnVsbH0sIHsibmF
-00000f40: 745a 5349 3649 434a 6b5a 574e 665a 584a  tZSI6ICJkZWNfZXJ
-00000f50: 7962 3349 694c 4341 695a 6d6c 6c62 4752  yb3IiLCAiZmllbGR
-00000f60: 6662 6d46 745a 5349 3649 434a 6b5a 574e  fbmFtZSI6ICJkZWN
-00000f70: 665a 584a 7962 3349 694c 4341 6963 4746  fZXJyb3IiLCAicGF
-00000f80: 755a 4746 7a58 3352 3563 4755 694f 6941  uZGFzX3R5cGUiOiA
-00000f90: 6961 5735 304e 6a51 694c 4341 6962 6e56  iaW50NjQiLCAibnV
-00000fa0: 7463 486c 6664 486c 775a 5349 3649 434a  tcHlfdHlwZSI6ICJ
-00000fb0: 7062 6e51 324e 4349 7349 434a 745a 5852  pbnQ2NCIsICJtZXR
-00000fc0: 685a 4746 3059 5349 3649 4735 3162 4778  hZGF0YSI6IG51bGx
-00000fd0: 394c 4342 3749 6d35 6862 5755 694f 6942  9LCB7Im5hbWUiOiB
-00000fe0: 7564 5778 734c 4341 695a 6d6c 6c62 4752  udWxsLCAiZmllbGR
-00000ff0: 6662 6d46 745a 5349 3649 434a 6658 326c  fbmFtZSI6ICJfX2l
-00001000: 755a 4756 3458 3278 6c64 6d56 7358 7a42  uZGV4X2xldmVsXzB
-00001010: 6658 7949 7349 434a 7759 5735 6b59 584e  fXyIsICJwYW5kYXN
-00001020: 6664 486c 775a 5349 3649 434a 7062 6e51  fdHlwZSI6ICJpbnQ
-00001030: 324e 4349 7349 434a 7564 5731 7765 5639  2NCIsICJudW1weV9
-00001040: 3065 5842 6c49 6a6f 6749 6d6c 7564 4459  0eXBlIjogImludDY
-00001050: 3049 6977 6749 6d31 6c64 4746 6b59 5852  0IiwgIm1ldGFkYXR
-00001060: 6849 6a6f 6762 6e56 7362 4831 644c 4341  hIjogbnVsbH1dLCA
-00001070: 6959 334a 6c59 5852 7663 6949 3649 4873  iY3JlYXRvciI6IHs
-00001080: 6962 476c 6963 6d46 7965 5349 3649 434a  ibGlicmFyeSI6ICJ
-00001090: 7765 5746 7963 6d39 3349 6977 6749 6e5a  weWFycm93IiwgInZ
-000010a0: 6c63 6e4e 7062 3234 694f 6941 694f 5334  lcnNpb24iOiAiOS4
-000010b0: 774c 6a41 6966 5377 6749 6e42 6862 6d52  wLjAifSwgInBhbmR
-000010c0: 6863 3139 325a 584a 7a61 5739 7549 6a6f  hc192ZXJzaW9uIjo
-000010d0: 6749 6a45 754d 7934 3149 6e30 4141 4141  gIjEuMy41In0AAAA
-000010e0: 4741 4141 414a 4145 4141 4f41 4141 4143  GAAAAJAEAAOAAAAC
-000010f0: 3041 4141 4166 4141 4141 4551 4141 4141  0AAAAfAAAAEQAAAA
-00001100: 4541 4141 4142 502f 2f2f 7741 4141 5149  EAAAABP///wAAAQI
-00001110: 5141 4141 414a 4141 4141 4151 4141 4141  QAAAAJAAAAAQAAAA
-00001120: 4141 4141 4145 5141 4141 4639 6661 5735  AAAAAEQAAAF9faW5
-00001130: 6b5a 5868 6662 4756 325a 5778 664d 4639  kZXhfbGV2ZWxfMF9
-00001140: 6641 4141 4142 502f 2f2f 7741 4141 4146  fAAAABP///wAAAAF
-00001150: 4141 4141 4151 502f 2f2f 7741 4141 5149  AAAAAQP///wAAAQI
-00001160: 5141 4141 4148 4141 4141 4151 4141 4141  QAAAAHAAAAAQAAAA
-00001170: 4141 4141 4143 5141 4141 4752 6c59 3139  AAAAACQAAAGRlY19
-00001180: 6c63 6e4a 7663 6741 4141 446a 2f2f 2f38  lcnJvcgAAADj///8
-00001190: 4141 4141 4251 4141 4141 4854 2f2f 2f38  AAAABQAAAAHT///8
-000011a0: 4141 4145 4345 4141 4141 4277 4141 4141  AAAECEAAAABwAAAA
-000011b0: 4541 4141 4141 4141 4141 4167 4141 4142  EAAAAAAAAAAgAAAB
-000011c0: 7959 5639 6c63 6e4a 7663 6741 4141 4142  yYV9lcnJvcgAAAAB
-000011d0: 732f 2f2f 2f41 4141 4141 5541 4141 4143  s////AAAAAUAAAAC
-000011e0: 6f2f 2f2f 2f41 4141 4241 7841 4141 4141  o////AAABAxAAAAA
-000011f0: 5541 4141 4142 4141 4141 4141 4141 4141  UAAAABAAAAAAAAAA
-00001200: 4441 4141 415a 4756 6a41 4e62 2f2f 2f38  DAAAAZGVjANb///8
-00001210: 4141 4149 4130 502f 2f2f 7741 4141 514d  AAAIA0P///wAAAQM
-00001220: 5141 4141 4148 4141 4141 4151 4141 4141  QAAAAHAAAAAQAAAA
-00001230: 4141 4141 4141 6741 4141 484a 6841 4141  AAAAAAgAAAHJhAAA
-00001240: 4141 4159 4143 4141 4741 4159 4141 4141  AAAYACAAGAAYAAAA
-00001250: 4141 4149 4145 4141 5541 4167 4142 6741  AAAIAEAAUAAgABgA
-00001260: 4841 4177 4141 4141 5141 4241 4141 4141  HAAwAAAAQABAAAAA
-00001270: 4141 4145 4345 4141 4141 4277 4141 4141  AAAECEAAAABwAAAA
-00001280: 4541 4141 4141 4141 4141 4149 4141 4142  EAAAAAAAAAAIAAAB
-00001290: 705a 4141 4143 4141 4d41 4167 4142 7741  pZAAACAAMAAgABwA
-000012a0: 4941 4141 4141 4141 4141 5541 4141 4141  IAAAAAAAAAUAAAAA
-000012b0: 4141 4141 4100 181f 7061 7271 7565 742d  AAAAA...parquet-
-000012c0: 6370 702d 6172 726f 7720 7665 7273 696f  cpp-arrow versio
-000012d0: 6e20 392e 302e 3019 6c1c 0000 1c00 001c  n 9.0.0.l.......
-000012e0: 0000 1c00 001c 0000 1c00 0000 010e 0000  ................
-000012f0: 5041 5231                                PAR1
+00000400: 1015 0200 0000 1504 196c 3500 1806 7363  .........l5...sc
+00000410: 6865 6d61 150a 0015 0425 0218 0269 6400  hema.....%...id.
+00000420: 150a 2502 1802 7261 0015 0a25 0218 0364  ..%...ra...%...d
+00000430: 6563 0015 0425 0218 0872 615f 6572 726f  ec...%...ra_erro
+00000440: 7200 1504 2502 1809 6465 635f 6572 726f  r...%...dec_erro
+00000450: 7200 160a 191c 195c 26f8 011c 1504 1935  r......\&......5
+00000460: 1000 0619 1802 6964 1502 160a 16fc 0116  ......id........
+00000470: f001 2664 2608 1c18 08d3 0200 0000 0000  ..&d&...........
+00000480: 0018 08bf 0200 0000 0000 0016 0028 08d3  .............(..
+00000490: 0200 0000 0000 0018 08bf 0200 0000 0000  ................
+000004a0: 0000 192c 1504 1500 1502 0015 0015 1015  ...,............
+000004b0: 0200 0000 26a2 051c 150a 1935 1000 0619  ....&......5....
+000004c0: 1802 7261 1502 160a 16fc 0116 f201 268e  ..ra..........&.
+000004d0: 0426 b003 1c18 0800 0000 0000 b873 4018  .&...........s@.
+000004e0: 0800 0000 0000 e871 4016 0028 0800 0000  .......q@..(....
+000004f0: 0000 b873 4018 0800 0000 0000 e871 4000  ...s@........q@.
+00000500: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
+00000510: 0000 26bc 081c 150a 1935 1000 0619 1803  ..&......5......
+00000520: 6465 6315 0216 0a16 da01 16de 0126 aa07  dec..........&..
+00000530: 26de 061c 1808 0000 0000 0040 4ec0 1808  &..........@N...
+00000540: 0000 0000 0060 51c0 1600 2808 0000 0000  .....`Q...(.....
+00000550: 0040 4ec0 1808 0000 0000 0060 51c0 0019  .@N........`Q...
+00000560: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
+00000570: 0026 ba0b 1c15 0419 3510 0006 1918 0872  .&......5......r
+00000580: 615f 6572 726f 7215 0216 0a16 b801 16c0  a_error.........
+00000590: 0126 aa0a 26fa 091c 1808 0000 0000 0000  .&..&...........
+000005a0: 0000 1808 0000 0000 0000 0000 1600 2808  ..............(.
+000005b0: 0000 0000 0000 0000 1808 0000 0000 0000  ................
+000005c0: 0000 0019 2c15 0415 0015 0200 1500 1510  ....,...........
+000005d0: 1502 0000 0026 c20e 1c15 0419 3510 0006  .....&......5...
+000005e0: 1918 0964 6563 5f65 7272 6f72 1502 160a  ...dec_error....
+000005f0: 16b8 0116 c001 26b2 0d26 820d 1c18 0800  ......&..&......
+00000600: 0000 0000 0000 0018 0800 0000 0000 0000  ................
+00000610: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
+00000620: 0000 0000 0000 0000 192c 1504 1500 1502  .........,......
+00000630: 0015 0015 1015 0200 0000 16c2 0816 0a26  ...............&
+00000640: 0816 c008 1400 0019 2c18 0670 616e 6461  ........,..panda
+00000650: 7318 a705 7b22 696e 6465 785f 636f 6c75  s...{"index_colu
+00000660: 6d6e 7322 3a20 5b5d 2c20 2263 6f6c 756d  mns": [], "colum
+00000670: 6e5f 696e 6465 7865 7322 3a20 5b5d 2c20  n_indexes": [], 
+00000680: 2263 6f6c 756d 6e73 223a 205b 7b22 6e61  "columns": [{"na
+00000690: 6d65 223a 2022 6964 222c 2022 6669 656c  me": "id", "fiel
+000006a0: 645f 6e61 6d65 223a 2022 6964 222c 2022  d_name": "id", "
+000006b0: 7061 6e64 6173 5f74 7970 6522 3a20 2269  pandas_type": "i
+000006c0: 6e74 3634 222c 2022 6e75 6d70 795f 7479  nt64", "numpy_ty
+000006d0: 7065 223a 2022 696e 7436 3422 2c20 226d  pe": "int64", "m
+000006e0: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
+000006f0: 207b 226e 616d 6522 3a20 2272 6122 2c20   {"name": "ra", 
+00000700: 2266 6965 6c64 5f6e 616d 6522 3a20 2272  "field_name": "r
+00000710: 6122 2c20 2270 616e 6461 735f 7479 7065  a", "pandas_type
+00000720: 223a 2022 666c 6f61 7436 3422 2c20 226e  ": "float64", "n
+00000730: 756d 7079 5f74 7970 6522 3a20 2266 6c6f  umpy_type": "flo
+00000740: 6174 3634 222c 2022 6d65 7461 6461 7461  at64", "metadata
+00000750: 223a 206e 756c 6c7d 2c20 7b22 6e61 6d65  ": null}, {"name
+00000760: 223a 2022 6465 6322 2c20 2266 6965 6c64  ": "dec", "field
+00000770: 5f6e 616d 6522 3a20 2264 6563 222c 2022  _name": "dec", "
+00000780: 7061 6e64 6173 5f74 7970 6522 3a20 2266  pandas_type": "f
+00000790: 6c6f 6174 3634 222c 2022 6e75 6d70 795f  loat64", "numpy_
+000007a0: 7479 7065 223a 2022 666c 6f61 7436 3422  type": "float64"
+000007b0: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
+000007c0: 6c6c 7d2c 207b 226e 616d 6522 3a20 2272  ll}, {"name": "r
+000007d0: 615f 6572 726f 7222 2c20 2266 6965 6c64  a_error", "field
+000007e0: 5f6e 616d 6522 3a20 2272 615f 6572 726f  _name": "ra_erro
+000007f0: 7222 2c20 2270 616e 6461 735f 7479 7065  r", "pandas_type
+00000800: 223a 2022 696e 7436 3422 2c20 226e 756d  ": "int64", "num
+00000810: 7079 5f74 7970 6522 3a20 2269 6e74 3634  py_type": "int64
+00000820: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
+00000830: 756c 6c7d 2c20 7b22 6e61 6d65 223a 2022  ull}, {"name": "
+00000840: 6465 635f 6572 726f 7222 2c20 2266 6965  dec_error", "fie
+00000850: 6c64 5f6e 616d 6522 3a20 2264 6563 5f65  ld_name": "dec_e
+00000860: 7272 6f72 222c 2022 7061 6e64 6173 5f74  rror", "pandas_t
+00000870: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
+00000880: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
+00000890: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
+000008a0: 3a20 6e75 6c6c 7d5d 2c20 2263 7265 6174  : null}], "creat
+000008b0: 6f72 223a 207b 226c 6962 7261 7279 223a  or": {"library":
+000008c0: 2022 7079 6172 726f 7722 2c20 2276 6572   "pyarrow", "ver
+000008d0: 7369 6f6e 223a 2022 392e 302e 3022 7d2c  sion": "9.0.0"},
+000008e0: 2022 7061 6e64 6173 5f76 6572 7369 6f6e   "pandas_version
+000008f0: 223a 2022 322e 302e 3022 7d00 180c 4152  ": "2.0.0"}...AR
+00000900: 524f 573a 7363 6865 6d61 1898 0b2f 2f2f  ROW:schema...///
+00000910: 2f2f 7967 4541 4141 5141 4141 4141 4141  //ygEAAAQAAAAAAA
+00000920: 4b41 4134 4142 6741 4641 4167 4143 6741  KAA4ABgAFAAgACgA
+00000930: 4141 4141 4242 4141 5141 4141 4141 4141  AAAABBAAQAAAAAAA
+00000940: 4b41 4177 4141 4141 4541 4167 4143 6741  KAAwAAAAEAAgACgA
+00000950: 4141 4e77 4341 4141 4541 4141 4141 5141  AANwCAAAEAAAAAQA
+00000960: 4141 4177 4141 4141 4941 4177 4142 4141  AAAwAAAAIAAwABAA
+00000970: 4941 4167 4141 4141 4941 4141 4145 4141  IAAgAAAAIAAAAEAA
+00000980: 4141 4159 4141 4142 7759 5735 6b59 584d  AAAYAAABwYW5kYXM
+00000990: 4141 4b63 4341 4142 3749 6d6c 755a 4756  AAKcCAAB7ImluZGV
+000009a0: 3458 324e 7662 4856 7462 6e4d 694f 6942  4X2NvbHVtbnMiOiB
+000009b0: 6258 5377 6749 6d4e 7662 4856 7462 6c39  bXSwgImNvbHVtbl9
+000009c0: 7062 6d52 6c65 4756 7a49 6a6f 6757 3130  pbmRleGVzIjogW10
+000009d0: 7349 434a 6a62 3278 3162 5735 7a49 6a6f  sICJjb2x1bW5zIjo
+000009e0: 6757 3373 6962 6d46 745a 5349 3649 434a  gW3sibmFtZSI6ICJ
+000009f0: 705a 4349 7349 434a 6d61 5756 735a 4639  pZCIsICJmaWVsZF9
+00000a00: 7559 5731 6c49 6a6f 6749 6d6c 6b49 6977  uYW1lIjogImlkIiw
+00000a10: 6749 6e42 6862 6d52 6863 3139 3065 5842  gInBhbmRhc190eXB
+00000a20: 6c49 6a6f 6749 6d6c 7564 4459 3049 6977  lIjogImludDY0Iiw
+00000a30: 6749 6d35 3162 5842 3558 3352 3563 4755  gIm51bXB5X3R5cGU
+00000a40: 694f 6941 6961 5735 304e 6a51 694c 4341  iOiAiaW50NjQiLCA
+00000a50: 6962 5756 3059 5752 6864 4745 694f 6942  ibWV0YWRhdGEiOiB
+00000a60: 7564 5778 7366 5377 6765 794a 7559 5731  udWxsfSwgeyJuYW1
+00000a70: 6c49 6a6f 6749 6e4a 6849 6977 6749 6d5a  lIjogInJhIiwgImZ
+00000a80: 705a 5778 6b58 3235 6862 5755 694f 6941  pZWxkX25hbWUiOiA
+00000a90: 6963 6d45 694c 4341 6963 4746 755a 4746  icmEiLCAicGFuZGF
+00000aa0: 7a58 3352 3563 4755 694f 6941 695a 6d78  zX3R5cGUiOiAiZmx
+00000ab0: 7659 5851 324e 4349 7349 434a 7564 5731  vYXQ2NCIsICJudW1
+00000ac0: 7765 5639 3065 5842 6c49 6a6f 6749 6d5a  weV90eXBlIjogImZ
+00000ad0: 7362 3246 304e 6a51 694c 4341 6962 5756  sb2F0NjQiLCAibWV
+00000ae0: 3059 5752 6864 4745 694f 6942 7564 5778  0YWRhdGEiOiBudWx
+00000af0: 7366 5377 6765 794a 7559 5731 6c49 6a6f  sfSwgeyJuYW1lIjo
+00000b00: 6749 6d52 6c59 7949 7349 434a 6d61 5756  gImRlYyIsICJmaWV
+00000b10: 735a 4639 7559 5731 6c49 6a6f 6749 6d52  sZF9uYW1lIjogImR
+00000b20: 6c59 7949 7349 434a 7759 5735 6b59 584e  lYyIsICJwYW5kYXN
+00000b30: 6664 486c 775a 5349 3649 434a 6d62 4739  fdHlwZSI6ICJmbG9
+00000b40: 6864 4459 3049 6977 6749 6d35 3162 5842  hdDY0IiwgIm51bXB
+00000b50: 3558 3352 3563 4755 694f 6941 695a 6d78  5X3R5cGUiOiAiZmx
+00000b60: 7659 5851 324e 4349 7349 434a 745a 5852  vYXQ2NCIsICJtZXR
+00000b70: 685a 4746 3059 5349 3649 4735 3162 4778  hZGF0YSI6IG51bGx
+00000b80: 394c 4342 3749 6d35 6862 5755 694f 6941  9LCB7Im5hbWUiOiA
+00000b90: 6963 6d46 665a 584a 7962 3349 694c 4341  icmFfZXJyb3IiLCA
+00000ba0: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
+00000bb0: 3649 434a 7959 5639 6c63 6e4a 7663 6949  6ICJyYV9lcnJvciI
+00000bc0: 7349 434a 7759 5735 6b59 584e 6664 486c  sICJwYW5kYXNfdHl
+00000bd0: 775a 5349 3649 434a 7062 6e51 324e 4349  wZSI6ICJpbnQ2NCI
+00000be0: 7349 434a 7564 5731 7765 5639 3065 5842  sICJudW1weV90eXB
+00000bf0: 6c49 6a6f 6749 6d6c 7564 4459 3049 6977  lIjogImludDY0Iiw
+00000c00: 6749 6d31 6c64 4746 6b59 5852 6849 6a6f  gIm1ldGFkYXRhIjo
+00000c10: 6762 6e56 7362 4830 7349 4873 6962 6d46  gbnVsbH0sIHsibmF
+00000c20: 745a 5349 3649 434a 6b5a 574e 665a 584a  tZSI6ICJkZWNfZXJ
+00000c30: 7962 3349 694c 4341 695a 6d6c 6c62 4752  yb3IiLCAiZmllbGR
+00000c40: 6662 6d46 745a 5349 3649 434a 6b5a 574e  fbmFtZSI6ICJkZWN
+00000c50: 665a 584a 7962 3349 694c 4341 6963 4746  fZXJyb3IiLCAicGF
+00000c60: 755a 4746 7a58 3352 3563 4755 694f 6941  uZGFzX3R5cGUiOiA
+00000c70: 6961 5735 304e 6a51 694c 4341 6962 6e56  iaW50NjQiLCAibnV
+00000c80: 7463 486c 6664 486c 775a 5349 3649 434a  tcHlfdHlwZSI6ICJ
+00000c90: 7062 6e51 324e 4349 7349 434a 745a 5852  pbnQ2NCIsICJtZXR
+00000ca0: 685a 4746 3059 5349 3649 4735 3162 4778  hZGF0YSI6IG51bGx
+00000cb0: 3958 5377 6749 6d4e 795a 5746 3062 3349  9XSwgImNyZWF0b3I
+00000cc0: 694f 6942 3749 6d78 7059 6e4a 6863 6e6b  iOiB7ImxpYnJhcnk
+00000cd0: 694f 6941 6963 486c 6863 6e4a 7664 7949  iOiAicHlhcnJvdyI
+00000ce0: 7349 434a 325a 584a 7a61 5739 7549 6a6f  sICJ2ZXJzaW9uIjo
+00000cf0: 6749 6a6b 754d 4334 7749 6e30 7349 434a  gIjkuMC4wIn0sICJ
+00000d00: 7759 5735 6b59 584e 6664 6d56 7963 326c  wYW5kYXNfdmVyc2l
+00000d10: 7662 6949 3649 4349 794c 6a41 754d 434a  vbiI6ICIyLjAuMCJ
+00000d20: 3941 4155 4141 4144 6b41 4141 416f 4141  9AAUAAADkAAAAoAA
+00000d30: 4141 4851 4141 4141 3841 4141 4142 4141  AAHQAAAA8AAAABAA
+00000d40: 4141 4544 2f2f 2f38 4141 4145 4345 4141  AAED///8AAAECEAA
+00000d50: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
+00000d60: 4141 416b 4141 4142 6b5a 574e 665a 584a  AAAkAAABkZWNfZXJ
+00000d70: 7962 3349 4141 4141 342f 2f2f 2f41 4141  yb3IAAAA4////AAA
+00000d80: 4141 5541 4141 4142 302f 2f2f 2f41 4141  AAUAAAAB0////AAA
+00000d90: 4241 6841 4141 4141 6341 4141 4142 4141  BAhAAAAAcAAAABAA
+00000da0: 4141 4141 4141 4141 4941 4141 4163 6d46  AAAAAAAAIAAAAcmF
+00000db0: 665a 584a 7962 3349 4141 4141 4162 502f  fZXJyb3IAAAAAbP/
+00000dc0: 2f2f 7741 4141 4146 4141 4141 4171 502f  //wAAAAFAAAAAqP/
+00000dd0: 2f2f 7741 4141 514d 5141 4141 4146 4141  //wAAAQMQAAAAFAA
+00000de0: 4141 4151 4141 4141 4141 4141 4141 7741  AAAQAAAAAAAAAAwA
+00000df0: 4141 4752 6c59 7744 572f 2f2f 2f41 4141  AAGRlYwDW////AAA
+00000e00: 4341 4e44 2f2f 2f38 4141 4145 4445 4141  CAND///8AAAEDEAA
+00000e10: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
+00000e20: 4141 4149 4141 4142 7959 5141 4141 4141  AAAIAAAByYQAAAAA
+00000e30: 4741 4167 4142 6741 4741 4141 4141 4141  GAAgABgAGAAAAAAA
+00000e40: 4341 4241 4146 4141 4941 4159 4142 7741  CABAAFAAIAAYABwA
+00000e50: 4d41 4141 4145 4141 5141 4141 4141 4141  MAAAAEAAQAAAAAAA
+00000e60: 4241 6841 4141 4141 6341 4141 4142 4141  BAhAAAAAcAAAABAA
+00000e70: 4141 4141 4141 4141 4341 4141 4161 5751  AAAAAAAACAAAAaWQ
+00000e80: 4141 4167 4144 4141 4941 4163 4143 4141  AAAgADAAIAAcACAA
+00000e90: 4141 4141 4141 4146 4141 4141 4141 4141  AAAAAAAFAAAAAAAA
+00000ea0: 4141 413d 3d00 181f 7061 7271 7565 742d  AAA==...parquet-
+00000eb0: 6370 702d 6172 726f 7720 7665 7273 696f  cpp-arrow versio
+00000ec0: 6e20 392e 302e 3019 5c1c 0000 1c00 001c  n 9.0.0.\.......
+00000ed0: 0000 1c00 001c 0000 00d3 0a00 0050 4152  .............PAR
+00000ee0: 31                                       1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_44/shard_2.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet`

 * *Files 16% similar despite different names*

```diff
@@ -1,307 +1,241 @@
-00000000: 5041 5231 1504 1580 0115 5c4c 1510 1500  PAR1......\L....
-00000010: 1200 0040 08f6 0200 0501 00f8 0d08 00fe  ...@............
-00000020: 0d08 0400 0305 1704 0003 0d08 0004 0d08  ................
-00000030: 3c07 0300 0000 0000 0008 0300 0000 0000  <...............
-00000040: 0015 0015 1615 1a2c 1510 1510 1506 1506  .......,........
-00000050: 1c18 0808 0300 0000 0000 0018 08f6 0200  ................
-00000060: 0000 0000 0016 0028 0808 0300 0000 0000  .......(........
-00000070: 0018 08f6 0200 0000 0000 0000 0000 0b28  ...............(
-00000080: 0200 0000 1001 0303 88c6 fa26 9602 1c15  ...........&....
-00000090: 0419 3510 0006 1918 0269 6415 0216 1016  ..5......id.....
-000000a0: ae02 168e 0226 8201 2608 1c18 0808 0300  .....&..&.......
-000000b0: 0000 0000 0018 08f6 0200 0000 0000 0016  ................
-000000c0: 0028 0808 0300 0000 0000 0018 08f6 0200  .(..............
-000000d0: 0000 0000 0000 192c 1504 1500 1502 0015  .......,........
-000000e0: 0015 1015 0200 0000 1504 1570 1556 4c15  ...........p.VL.
-000000f0: 0e15 0012 0000 3800 0001 0108 5874 4001  ......8.....Xt@.
-00000100: 0704 0008 0d08 0468 7309 1004 9872 0908  .......hs....r..
-00000110: 04c8 7509 0828 1874 4000 0000 0000 8875  ..u..(.t@......u
-00000120: 4015 0015 1615 1a2c 1510 1510 1506 1506  @......,........
-00000130: 1c18 0800 0000 0000 c875 4018 0800 0000  .........u@.....
-00000140: 0000 9872 4016 0028 0800 0000 0000 c875  ...r@..(.......u
-00000150: 4018 0800 0000 0000 9872 4000 0000 0b28  @........r@....(
-00000160: 0200 0000 1001 0303 8846 d626 d605 1c15  .........F.&....
-00000170: 0a19 3510 0006 1918 0272 6115 0216 1016  ..5......ra.....
-00000180: 9c02 1686 0226 c204 26d0 031c 1808 0000  .....&..&.......
-00000190: 0000 00c8 7540 1808 0000 0000 0098 7240  ....u@........r@
-000001a0: 1600 2808 0000 0000 00c8 7540 1808 0000  ..(.......u@....
-000001b0: 0000 0098 7240 0019 2c15 0415 0015 0200  ....r@..,.......
-000001c0: 1500 1510 1502 0000 0015 0415 6015 4e4c  ............`.NL
-000001d0: 150c 1500 1200 0030 0000 0101 08c0 4ac0  .......0......J.
-000001e0: 0107 0800 c04f 0908 0440 4e09 0804 e050  .....O...@N....P
-000001f0: 0908 2820 50c0 0000 0000 0040 4bc0 1500  ..( P......@K...
-00000200: 1516 151a 2c15 1015 1015 0615 061c 1808  ....,...........
-00000210: 0000 0000 00c0 4ac0 1808 0000 0000 00e0  ......J.........
-00000220: 50c0 1600 2808 0000 0000 00c0 4ac0 1808  P...(.......J...
-00000230: 0000 0000 00e0 50c0 0000 000b 2802 0000  ......P.....(...
-00000240: 0010 0103 0340 3436 2690 091c 150a 1935  .....@46&......5
-00000250: 1000 0619 1803 6465 6315 0216 1016 8c02  ......dec.......
-00000260: 16fe 0126 fc07 2692 071c 1808 0000 0000  ...&..&.........
-00000270: 00c0 4ac0 1808 0000 0000 00e0 50c0 1600  ..J.........P...
-00000280: 2808 0000 0000 00c0 4ac0 1808 0000 0000  (.......J.......
-00000290: 00e0 50c0 0019 2c15 0415 0015 0200 1500  ..P...,.........
-000002a0: 1510 1502 0000 0015 0415 1015 144c 1502  .............L..
-000002b0: 1500 1200 0008 1c00 0000 0000 0000 0015  ................
-000002c0: 0015 1215 162c 1510 1510 1506 1506 1c18  .....,..........
-000002d0: 0800 0000 0000 0000 0018 0800 0000 0000  ................
-000002e0: 0000 0016 0028 0800 0000 0000 0000 0018  .....(..........
-000002f0: 0800 0000 0000 0000 0000 0000 0920 0200  ............. ..
-00000300: 0000 1001 0110 0026 8e0c 1c15 0419 3510  .......&......5.
-00000310: 0006 1918 0872 615f 6572 726f 7215 0216  .....ra_error...
-00000320: 1016 b801 16c0 0126 fe0a 26ce 0a1c 1808  .......&..&.....
-00000330: 0000 0000 0000 0000 1808 0000 0000 0000  ................
-00000340: 0000 1600 2808 0000 0000 0000 0000 1808  ....(...........
-00000350: 0000 0000 0000 0000 0019 2c15 0415 0015  ..........,.....
-00000360: 0200 1500 1510 1502 0000 0015 0415 1015  ................
-00000370: 144c 1502 1500 1200 0008 1c00 0000 0000  .L..............
-00000380: 0000 0015 0015 1215 162c 1510 1510 1506  .........,......
-00000390: 1506 1c18 0800 0000 0000 0000 0018 0800  ................
-000003a0: 0000 0000 0000 0016 0028 0800 0000 0000  .........(......
-000003b0: 0000 0018 0800 0000 0000 0000 0000 0000  ................
-000003c0: 0920 0200 0000 1001 0110 0026 960f 1c15  . .........&....
-000003d0: 0419 3510 0006 1918 0964 6563 5f65 7272  ..5......dec_err
-000003e0: 6f72 1502 1610 16b8 0116 c001 2686 0e26  or..........&..&
-000003f0: d60d 1c18 0800 0000 0000 0000 0018 0800  ................
-00000400: 0000 0000 0000 0016 0028 0800 0000 0000  .........(......
-00000410: 0000 0018 0800 0000 0000 0000 0000 192c  ...............,
-00000420: 1504 1500 1502 0015 0015 1015 0200 0000  ................
-00000430: 1504 1580 0115 584c 1510 1500 1200 0040  ......XL.......@
-00000440: 0407 0009 0100 0909 0704 000f 0d08 0011  ................
-00000450: 0d08 0014 0d08 0015 0d08 3c18 0000 0000  ..........<.....
-00000460: 0000 0019 0000 0000 0000 0015 0015 1615  ................
-00000470: 1a2c 1510 1510 1506 1506 1c18 0819 0000  .,..............
-00000480: 0000 0000 0018 0807 0000 0000 0000 0016  ................
-00000490: 0028 0819 0000 0000 0000 0018 0807 0000  .(..............
-000004a0: 0000 0000 0000 0000 0b28 0200 0000 1001  .........(......
-000004b0: 0303 88c6 fa26 ea12 1c15 0419 3510 0006  .....&......5...
-000004c0: 1918 115f 5f69 6e64 6578 5f6c 6576 656c  ...__index_level
-000004d0: 5f30 5f5f 1502 1610 16ae 0216 8a02 26d6  _0__..........&.
-000004e0: 1126 e010 1c18 0819 0000 0000 0000 0018  .&..............
-000004f0: 0807 0000 0000 0000 0016 0028 0819 0000  ...........(....
-00000500: 0000 0000 0018 0807 0000 0000 0000 0000  ................
-00000510: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
-00000520: 0000 1504 197c 3500 1806 7363 6865 6d61  .....|5...schema
-00000530: 150c 0015 0425 0218 0269 6400 150a 2502  .....%...id...%.
-00000540: 1802 7261 0015 0a25 0218 0364 6563 0015  ..ra...%...dec..
-00000550: 0425 0218 0872 615f 6572 726f 7200 1504  .%...ra_error...
-00000560: 2502 1809 6465 635f 6572 726f 7200 1504  %...dec_error...
-00000570: 2502 1811 5f5f 696e 6465 785f 6c65 7665  %...__index_leve
-00000580: 6c5f 305f 5f00 1610 191c 196c 2696 021c  l_0__......l&...
-00000590: 1504 1935 1000 0619 1802 6964 1502 1610  ...5......id....
-000005a0: 16ae 0216 8e02 2682 0126 081c 1808 0803  ......&..&......
-000005b0: 0000 0000 0000 1808 f602 0000 0000 0000  ................
-000005c0: 1600 2808 0803 0000 0000 0000 1808 f602  ..(.............
-000005d0: 0000 0000 0000 0019 2c15 0415 0015 0200  ........,.......
-000005e0: 1500 1510 1502 0000 0026 d605 1c15 0a19  .........&......
-000005f0: 3510 0006 1918 0272 6115 0216 1016 9c02  5......ra.......
-00000600: 1686 0226 c204 26d0 031c 1808 0000 0000  ...&..&.........
-00000610: 00c8 7540 1808 0000 0000 0098 7240 1600  ..u@........r@..
-00000620: 2808 0000 0000 00c8 7540 1808 0000 0000  (.......u@......
-00000630: 0098 7240 0019 2c15 0415 0015 0200 1500  ..r@..,.........
-00000640: 1510 1502 0000 0026 9009 1c15 0a19 3510  .......&......5.
-00000650: 0006 1918 0364 6563 1502 1610 168c 0216  .....dec........
-00000660: fe01 26fc 0726 9207 1c18 0800 0000 0000  ..&..&..........
-00000670: c04a c018 0800 0000 0000 e050 c016 0028  .J.........P...(
-00000680: 0800 0000 0000 c04a c018 0800 0000 0000  .......J........
-00000690: e050 c000 192c 1504 1500 1502 0015 0015  .P...,..........
-000006a0: 1015 0200 0000 268e 0c1c 1504 1935 1000  ......&......5..
-000006b0: 0619 1808 7261 5f65 7272 6f72 1502 1610  ....ra_error....
-000006c0: 16b8 0116 c001 26fe 0a26 ce0a 1c18 0800  ......&..&......
-000006d0: 0000 0000 0000 0018 0800 0000 0000 0000  ................
-000006e0: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
-000006f0: 0000 0000 0000 0000 192c 1504 1500 1502  .........,......
-00000700: 0015 0015 1015 0200 0000 2696 0f1c 1504  ..........&.....
-00000710: 1935 1000 0619 1809 6465 635f 6572 726f  .5......dec_erro
-00000720: 7215 0216 1016 b801 16c0 0126 860e 26d6  r..........&..&.
-00000730: 0d1c 1808 0000 0000 0000 0000 1808 0000  ................
-00000740: 0000 0000 0000 1600 2808 0000 0000 0000  ........(.......
-00000750: 0000 1808 0000 0000 0000 0000 0019 2c15  ..............,.
-00000760: 0415 0015 0200 1500 1510 1502 0000 0026  ...............&
-00000770: ea12 1c15 0419 3510 0006 1918 115f 5f69  ......5......__i
-00000780: 6e64 6578 5f6c 6576 656c 5f30 5f5f 1502  ndex_level_0__..
-00000790: 1610 16ae 0216 8a02 26d6 1126 e010 1c18  ........&..&....
-000007a0: 0819 0000 0000 0000 0018 0807 0000 0000  ................
-000007b0: 0000 0016 0028 0819 0000 0000 0000 0018  .....(..........
-000007c0: 0807 0000 0000 0000 0000 192c 1504 1500  ...........,....
-000007d0: 1502 0015 0015 1015 0200 0000 16f4 0b16  ................
-000007e0: 1026 0816 9c0b 1400 0019 2c18 0670 616e  .&........,..pan
-000007f0: 6461 7318 a507 7b22 696e 6465 785f 636f  das...{"index_co
-00000800: 6c75 6d6e 7322 3a20 5b22 5f5f 696e 6465  lumns": ["__inde
-00000810: 785f 6c65 7665 6c5f 305f 5f22 5d2c 2022  x_level_0__"], "
-00000820: 636f 6c75 6d6e 5f69 6e64 6578 6573 223a  column_indexes":
-00000830: 205b 7b22 6e61 6d65 223a 206e 756c 6c2c   [{"name": null,
-00000840: 2022 6669 656c 645f 6e61 6d65 223a 206e   "field_name": n
-00000850: 756c 6c2c 2022 7061 6e64 6173 5f74 7970  ull, "pandas_typ
-00000860: 6522 3a20 2275 6e69 636f 6465 222c 2022  e": "unicode", "
-00000870: 6e75 6d70 795f 7479 7065 223a 2022 6f62  numpy_type": "ob
-00000880: 6a65 6374 222c 2022 6d65 7461 6461 7461  ject", "metadata
-00000890: 223a 207b 2265 6e63 6f64 696e 6722 3a20  ": {"encoding": 
-000008a0: 2255 5446 2d38 227d 7d5d 2c20 2263 6f6c  "UTF-8"}}], "col
-000008b0: 756d 6e73 223a 205b 7b22 6e61 6d65 223a  umns": [{"name":
-000008c0: 2022 6964 222c 2022 6669 656c 645f 6e61   "id", "field_na
-000008d0: 6d65 223a 2022 6964 222c 2022 7061 6e64  me": "id", "pand
-000008e0: 6173 5f74 7970 6522 3a20 2269 6e74 3634  as_type": "int64
-000008f0: 222c 2022 6e75 6d70 795f 7479 7065 223a  ", "numpy_type":
-00000900: 2022 696e 7436 3422 2c20 226d 6574 6164   "int64", "metad
-00000910: 6174 6122 3a20 6e75 6c6c 7d2c 207b 226e  ata": null}, {"n
-00000920: 616d 6522 3a20 2272 6122 2c20 2266 6965  ame": "ra", "fie
-00000930: 6c64 5f6e 616d 6522 3a20 2272 6122 2c20  ld_name": "ra", 
-00000940: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
-00000950: 666c 6f61 7436 3422 2c20 226e 756d 7079  float64", "numpy
-00000960: 5f74 7970 6522 3a20 2266 6c6f 6174 3634  _type": "float64
-00000970: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
-00000980: 756c 6c7d 2c20 7b22 6e61 6d65 223a 2022  ull}, {"name": "
-00000990: 6465 6322 2c20 2266 6965 6c64 5f6e 616d  dec", "field_nam
-000009a0: 6522 3a20 2264 6563 222c 2022 7061 6e64  e": "dec", "pand
-000009b0: 6173 5f74 7970 6522 3a20 2266 6c6f 6174  as_type": "float
-000009c0: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
-000009d0: 223a 2022 666c 6f61 7436 3422 2c20 226d  ": "float64", "m
-000009e0: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
-000009f0: 207b 226e 616d 6522 3a20 2272 615f 6572   {"name": "ra_er
-00000a00: 726f 7222 2c20 2266 6965 6c64 5f6e 616d  ror", "field_nam
-00000a10: 6522 3a20 2272 615f 6572 726f 7222 2c20  e": "ra_error", 
-00000a20: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
-00000a30: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
-00000a40: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
-00000a50: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
-00000a60: 2c20 7b22 6e61 6d65 223a 2022 6465 635f  , {"name": "dec_
-00000a70: 6572 726f 7222 2c20 2266 6965 6c64 5f6e  error", "field_n
-00000a80: 616d 6522 3a20 2264 6563 5f65 7272 6f72  ame": "dec_error
-00000a90: 222c 2022 7061 6e64 6173 5f74 7970 6522  ", "pandas_type"
-00000aa0: 3a20 2269 6e74 3634 222c 2022 6e75 6d70  : "int64", "nump
-00000ab0: 795f 7479 7065 223a 2022 696e 7436 3422  y_type": "int64"
-00000ac0: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
-00000ad0: 6c6c 7d2c 207b 226e 616d 6522 3a20 6e75  ll}, {"name": nu
-00000ae0: 6c6c 2c20 2266 6965 6c64 5f6e 616d 6522  ll, "field_name"
-00000af0: 3a20 225f 5f69 6e64 6578 5f6c 6576 656c  : "__index_level
-00000b00: 5f30 5f5f 222c 2022 7061 6e64 6173 5f74  _0__", "pandas_t
-00000b10: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
-00000b20: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
-00000b30: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
-00000b40: 3a20 6e75 6c6c 7d5d 2c20 2263 7265 6174  : null}], "creat
-00000b50: 6f72 223a 207b 226c 6962 7261 7279 223a  or": {"library":
-00000b60: 2022 7079 6172 726f 7722 2c20 2276 6572   "pyarrow", "ver
-00000b70: 7369 6f6e 223a 2022 392e 302e 3022 7d2c  sion": "9.0.0"},
-00000b80: 2022 7061 6e64 6173 5f76 6572 7369 6f6e   "pandas_version
-00000b90: 223a 2022 312e 332e 3522 7d00 180c 4152  ": "1.3.5"}...AR
-00000ba0: 524f 573a 7363 6865 6d61 18c0 0e2f 2f2f  ROW:schema...///
-00000bb0: 2f2f 3267 4641 4141 5141 4141 4141 4141  //2gFAAAQAAAAAAA
-00000bc0: 4b41 4134 4142 6741 4641 4167 4143 6741  KAA4ABgAFAAgACgA
-00000bd0: 4141 4141 4242 4141 5141 4141 4141 4141  AAAABBAAQAAAAAAA
-00000be0: 4b41 4177 4141 4141 4541 4167 4143 6741  KAAwAAAAEAAgACgA
-00000bf0: 4141 4e77 4441 4141 4541 4141 4141 5141  AANwDAAAEAAAAAQA
-00000c00: 4141 4177 4141 4141 4941 4177 4142 4141  AAAwAAAAIAAwABAA
-00000c10: 4941 4167 4141 4141 4941 4141 4145 4141  IAAgAAAAIAAAAEAA
-00000c20: 4141 4159 4141 4142 7759 5735 6b59 584d  AAAYAAABwYW5kYXM
-00000c30: 4141 4b55 4441 4142 3749 6d6c 755a 4756  AAKUDAAB7ImluZGV
-00000c40: 3458 324e 7662 4856 7462 6e4d 694f 6942  4X2NvbHVtbnMiOiB
-00000c50: 6249 6c39 6661 5735 6b5a 5868 6662 4756  bIl9faW5kZXhfbGV
-00000c60: 325a 5778 664d 4639 6649 6c30 7349 434a  2ZWxfMF9fIl0sICJ
-00000c70: 6a62 3278 3162 5735 6661 5735 6b5a 5868  jb2x1bW5faW5kZXh
-00000c80: 6c63 7949 3649 4674 3749 6d35 6862 5755  lcyI6IFt7Im5hbWU
-00000c90: 694f 6942 7564 5778 734c 4341 695a 6d6c  iOiBudWxsLCAiZml
-00000ca0: 6c62 4752 6662 6d46 745a 5349 3649 4735  lbGRfbmFtZSI6IG5
-00000cb0: 3162 4777 7349 434a 7759 5735 6b59 584e  1bGwsICJwYW5kYXN
-00000cc0: 6664 486c 775a 5349 3649 434a 3162 6d6c  fdHlwZSI6ICJ1bml
-00000cd0: 6a62 3252 6c49 6977 6749 6d35 3162 5842  jb2RlIiwgIm51bXB
-00000ce0: 3558 3352 3563 4755 694f 6941 6962 324a  5X3R5cGUiOiAib2J
-00000cf0: 715a 574e 3049 6977 6749 6d31 6c64 4746  qZWN0IiwgIm1ldGF
-00000d00: 6b59 5852 6849 6a6f 6765 794a 6c62 6d4e  kYXRhIjogeyJlbmN
-00000d10: 765a 476c 755a 7949 3649 434a 5656 4559  vZGluZyI6ICJVVEY
-00000d20: 744f 434a 3966 5630 7349 434a 6a62 3278  tOCJ9fV0sICJjb2x
-00000d30: 3162 5735 7a49 6a6f 6757 3373 6962 6d46  1bW5zIjogW3sibmF
-00000d40: 745a 5349 3649 434a 705a 4349 7349 434a  tZSI6ICJpZCIsICJ
-00000d50: 6d61 5756 735a 4639 7559 5731 6c49 6a6f  maWVsZF9uYW1lIjo
-00000d60: 6749 6d6c 6b49 6977 6749 6e42 6862 6d52  gImlkIiwgInBhbmR
-00000d70: 6863 3139 3065 5842 6c49 6a6f 6749 6d6c  hc190eXBlIjogIml
-00000d80: 7564 4459 3049 6977 6749 6d35 3162 5842  udDY0IiwgIm51bXB
-00000d90: 3558 3352 3563 4755 694f 6941 6961 5735  5X3R5cGUiOiAiaW5
-00000da0: 304e 6a51 694c 4341 6962 5756 3059 5752  0NjQiLCAibWV0YWR
-00000db0: 6864 4745 694f 6942 7564 5778 7366 5377  hdGEiOiBudWxsfSw
-00000dc0: 6765 794a 7559 5731 6c49 6a6f 6749 6e4a  geyJuYW1lIjogInJ
-00000dd0: 6849 6977 6749 6d5a 705a 5778 6b58 3235  hIiwgImZpZWxkX25
-00000de0: 6862 5755 694f 6941 6963 6d45 694c 4341  hbWUiOiAicmEiLCA
-00000df0: 6963 4746 755a 4746 7a58 3352 3563 4755  icGFuZGFzX3R5cGU
-00000e00: 694f 6941 695a 6d78 7659 5851 324e 4349  iOiAiZmxvYXQ2NCI
-00000e10: 7349 434a 7564 5731 7765 5639 3065 5842  sICJudW1weV90eXB
-00000e20: 6c49 6a6f 6749 6d5a 7362 3246 304e 6a51  lIjogImZsb2F0NjQ
-00000e30: 694c 4341 6962 5756 3059 5752 6864 4745  iLCAibWV0YWRhdGE
-00000e40: 694f 6942 7564 5778 7366 5377 6765 794a  iOiBudWxsfSwgeyJ
-00000e50: 7559 5731 6c49 6a6f 6749 6d52 6c59 7949  uYW1lIjogImRlYyI
-00000e60: 7349 434a 6d61 5756 735a 4639 7559 5731  sICJmaWVsZF9uYW1
-00000e70: 6c49 6a6f 6749 6d52 6c59 7949 7349 434a  lIjogImRlYyIsICJ
-00000e80: 7759 5735 6b59 584e 6664 486c 775a 5349  wYW5kYXNfdHlwZSI
-00000e90: 3649 434a 6d62 4739 6864 4459 3049 6977  6ICJmbG9hdDY0Iiw
-00000ea0: 6749 6d35 3162 5842 3558 3352 3563 4755  gIm51bXB5X3R5cGU
-00000eb0: 694f 6941 695a 6d78 7659 5851 324e 4349  iOiAiZmxvYXQ2NCI
-00000ec0: 7349 434a 745a 5852 685a 4746 3059 5349  sICJtZXRhZGF0YSI
-00000ed0: 3649 4735 3162 4778 394c 4342 3749 6d35  6IG51bGx9LCB7Im5
-00000ee0: 6862 5755 694f 6941 6963 6d46 665a 584a  hbWUiOiAicmFfZXJ
-00000ef0: 7962 3349 694c 4341 695a 6d6c 6c62 4752  yb3IiLCAiZmllbGR
-00000f00: 6662 6d46 745a 5349 3649 434a 7959 5639  fbmFtZSI6ICJyYV9
-00000f10: 6c63 6e4a 7663 6949 7349 434a 7759 5735  lcnJvciIsICJwYW5
-00000f20: 6b59 584e 6664 486c 775a 5349 3649 434a  kYXNfdHlwZSI6ICJ
-00000f30: 7062 6e51 324e 4349 7349 434a 7564 5731  pbnQ2NCIsICJudW1
-00000f40: 7765 5639 3065 5842 6c49 6a6f 6749 6d6c  weV90eXBlIjogIml
-00000f50: 7564 4459 3049 6977 6749 6d31 6c64 4746  udDY0IiwgIm1ldGF
-00000f60: 6b59 5852 6849 6a6f 6762 6e56 7362 4830  kYXRhIjogbnVsbH0
-00000f70: 7349 4873 6962 6d46 745a 5349 3649 434a  sIHsibmFtZSI6ICJ
-00000f80: 6b5a 574e 665a 584a 7962 3349 694c 4341  kZWNfZXJyb3IiLCA
-00000f90: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
-00000fa0: 3649 434a 6b5a 574e 665a 584a 7962 3349  6ICJkZWNfZXJyb3I
-00000fb0: 694c 4341 6963 4746 755a 4746 7a58 3352  iLCAicGFuZGFzX3R
-00000fc0: 3563 4755 694f 6941 6961 5735 304e 6a51  5cGUiOiAiaW50NjQ
-00000fd0: 694c 4341 6962 6e56 7463 486c 6664 486c  iLCAibnVtcHlfdHl
-00000fe0: 775a 5349 3649 434a 7062 6e51 324e 4349  wZSI6ICJpbnQ2NCI
-00000ff0: 7349 434a 745a 5852 685a 4746 3059 5349  sICJtZXRhZGF0YSI
-00001000: 3649 4735 3162 4778 394c 4342 3749 6d35  6IG51bGx9LCB7Im5
-00001010: 6862 5755 694f 6942 7564 5778 734c 4341  hbWUiOiBudWxsLCA
-00001020: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
-00001030: 3649 434a 6658 326c 755a 4756 3458 3278  6ICJfX2luZGV4X2x
-00001040: 6c64 6d56 7358 7a42 6658 7949 7349 434a  ldmVsXzBfXyIsICJ
-00001050: 7759 5735 6b59 584e 6664 486c 775a 5349  wYW5kYXNfdHlwZSI
-00001060: 3649 434a 7062 6e51 324e 4349 7349 434a  6ICJpbnQ2NCIsICJ
-00001070: 7564 5731 7765 5639 3065 5842 6c49 6a6f  udW1weV90eXBlIjo
-00001080: 6749 6d6c 7564 4459 3049 6977 6749 6d31  gImludDY0IiwgIm1
-00001090: 6c64 4746 6b59 5852 6849 6a6f 6762 6e56  ldGFkYXRhIjogbnV
-000010a0: 7362 4831 644c 4341 6959 334a 6c59 5852  sbH1dLCAiY3JlYXR
-000010b0: 7663 6949 3649 4873 6962 476c 6963 6d46  vciI6IHsibGlicmF
-000010c0: 7965 5349 3649 434a 7765 5746 7963 6d39  yeSI6ICJweWFycm9
-000010d0: 3349 6977 6749 6e5a 6c63 6e4e 7062 3234  3IiwgInZlcnNpb24
-000010e0: 694f 6941 694f 5334 774c 6a41 6966 5377  iOiAiOS4wLjAifSw
-000010f0: 6749 6e42 6862 6d52 6863 3139 325a 584a  gInBhbmRhc192ZXJ
-00001100: 7a61 5739 7549 6a6f 6749 6a45 754d 7934  zaW9uIjogIjEuMy4
-00001110: 3149 6e30 4141 4141 4741 4141 414a 4145  1In0AAAAGAAAAJAE
-00001120: 4141 4f41 4141 4143 3041 4141 4166 4141  AAOAAAAC0AAAAfAA
-00001130: 4141 4551 4141 4141 4541 4141 4142 502f  AAEQAAAAEAAAABP/
-00001140: 2f2f 7741 4141 5149 5141 4141 414a 4141  //wAAAQIQAAAAJAA
-00001150: 4141 4151 4141 4141 4141 4141 4145 5141  AAAQAAAAAAAAAEQA
-00001160: 4141 4639 6661 5735 6b5a 5868 6662 4756  AAF9faW5kZXhfbGV
-00001170: 325a 5778 664d 4639 6641 4141 4142 502f  2ZWxfMF9fAAAABP/
-00001180: 2f2f 7741 4141 4146 4141 4141 4151 502f  //wAAAAFAAAAAQP/
-00001190: 2f2f 7741 4141 5149 5141 4141 4148 4141  //wAAAQIQAAAAHAA
-000011a0: 4141 4151 4141 4141 4141 4141 4143 5141  AAAQAAAAAAAAACQA
-000011b0: 4141 4752 6c59 3139 6c63 6e4a 7663 6741  AAGRlY19lcnJvcgA
-000011c0: 4141 446a 2f2f 2f38 4141 4141 4251 4141  AADj///8AAAABQAA
-000011d0: 4141 4854 2f2f 2f38 4141 4145 4345 4141  AAHT///8AAAECEAA
-000011e0: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
-000011f0: 4141 4167 4141 4142 7959 5639 6c63 6e4a  AAAgAAAByYV9lcnJ
-00001200: 7663 6741 4141 4142 732f 2f2f 2f41 4141  vcgAAAABs////AAA
-00001210: 4141 5541 4141 4143 6f2f 2f2f 2f41 4141  AAUAAAACo////AAA
-00001220: 4241 7841 4141 4141 5541 4141 4142 4141  BAxAAAAAUAAAABAA
-00001230: 4141 4141 4141 4141 4441 4141 415a 4756  AAAAAAAADAAAAZGV
-00001240: 6a41 4e62 2f2f 2f38 4141 4149 4130 502f  jANb///8AAAIA0P/
-00001250: 2f2f 7741 4141 514d 5141 4141 4148 4141  //wAAAQMQAAAAHAA
-00001260: 4141 4151 4141 4141 4141 4141 4141 6741  AAAQAAAAAAAAAAgA
-00001270: 4141 484a 6841 4141 4141 4159 4143 4141  AAHJhAAAAAAYACAA
-00001280: 4741 4159 4141 4141 4141 4149 4145 4141  GAAYAAAAAAAIAEAA
-00001290: 5541 4167 4142 6741 4841 4177 4141 4141  UAAgABgAHAAwAAAA
-000012a0: 5141 4241 4141 4141 4141 4145 4345 4141  QABAAAAAAAAECEAA
-000012b0: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
-000012c0: 4141 4149 4141 4142 705a 4141 4143 4141  AAAIAAABpZAAACAA
-000012d0: 4d41 4167 4142 7741 4941 4141 4141 4141  MAAgABwAIAAAAAAA
-000012e0: 4141 5541 4141 4141 4141 4141 4100 181f  AAUAAAAAAAAAA...
-000012f0: 7061 7271 7565 742d 6370 702d 6172 726f  parquet-cpp-arro
-00001300: 7720 7665 7273 696f 6e20 392e 302e 3019  w version 9.0.0.
-00001310: 6c1c 0000 1c00 001c 0000 1c00 001c 0000  l...............
-00001320: 1c00 0000 020e 0000 5041 5231            ........PAR1
+00000000: 5041 5231 1504 1570 1550 4c15 0e15 0012  PAR1...p.PL.....
+00000010: 0000 3808 2303 0005 0100 280d 0800 2c0d  ..8.#.....(...,.
+00000020: 0800 2d0d 0800 350d 083c 3703 0000 0000  ..-...5..<7.....
+00000030: 0000 3c03 0000 0000 0000 1500 1516 151a  ..<.............
+00000040: 2c15 0e15 1015 0615 061c 1808 3c03 0000  ,...........<...
+00000050: 0000 0000 1808 2303 0000 0000 0000 1600  ......#.........
+00000060: 2808 3c03 0000 0000 0000 1808 2303 0000  (.<.........#...
+00000070: 0000 0000 0000 000b 2802 0000 000e 0103  ........(.......
+00000080: 0388 c61a 2688 021c 1504 1935 1000 0619  ....&......5....
+00000090: 1802 6964 1502 160e 169c 0216 8002 2674  ..id..........&t
+000000a0: 2608 1c18 083c 0300 0000 0000 0018 0823  &....<.........#
+000000b0: 0300 0000 0000 0016 0028 083c 0300 0000  .........(.<....
+000000c0: 0000 0018 0823 0300 0000 0000 0000 192c  .....#.........,
+000000d0: 1504 1500 1502 0015 0015 1015 0200 0000  ................
+000000e0: 1504 1560 154a 4c15 0c15 0012 0000 3000  ...`.JL.......0.
+000000f0: 0001 0108 0875 4001 0708 0008 7409 0800  .....u@.....t...
+00000100: a80d 1000 d80d 0828 a874 4000 0000 0000  .......(.t@.....
+00000110: 2875 4015 0015 1615 1a2c 150e 1510 1506  (u@......,......
+00000120: 1506 1c18 0800 0000 0000 d875 4018 0800  ...........u@...
+00000130: 0000 0000 0874 4016 0028 0800 0000 0000  .....t@..(......
+00000140: d875 4018 0800 0000 0000 0874 4000 0000  .u@........t@...
+00000150: 0b28 0200 0000 0e01 0303 88c6 1226 ba05  .(...........&..
+00000160: 1c15 0a19 3510 0006 1918 0272 6115 0216  ....5......ra...
+00000170: 0e16 8c02 16fa 0126 a604 26c0 031c 1808  .......&..&.....
+00000180: 0000 0000 00d8 7540 1808 0000 0000 0008  ......u@........
+00000190: 7440 1600 2808 0000 0000 00d8 7540 1808  t@..(.......u@..
+000001a0: 0000 0000 0008 7440 0019 2c15 0415 0015  ......t@..,.....
+000001b0: 0200 1500 1510 1502 0000 0015 0415 7015  ..............p.
+000001c0: 564c 150e 1500 1200 0038 0000 0101 0880  VL.......8......
+000001d0: 39c0 0107 0800 4044 0d08 004e 0908 04c0  9.....@D...N....
+000001e0: 4209 0804 404a 0908 28c0 46c0 0000 0000  B...@J..(.F.....
+000001f0: 0080 3ac0 1500 1516 151a 2c15 0e15 1015  ..:.......,.....
+00000200: 0615 061c 1808 0000 0000 0080 39c0 1808  ............9...
+00000210: 0000 0000 0040 4ec0 1600 2808 0000 0000  .....@N...(.....
+00000220: 0080 39c0 1808 0000 0000 0040 4ec0 0000  ..9........@N...
+00000230: 000b 2802 0000 000e 0103 0388 c61a 26fc  ..(...........&.
+00000240: 081c 150a 1935 1000 0619 1803 6465 6315  .....5......dec.
+00000250: 0216 0e16 9c02 1686 0226 e807 26f6 061c  .........&..&...
+00000260: 1808 0000 0000 0080 39c0 1808 0000 0000  ........9.......
+00000270: 0040 4ec0 1600 2808 0000 0000 0080 39c0  .@N...(.......9.
+00000280: 1808 0000 0000 0040 4ec0 0019 2c15 0415  .......@N...,...
+00000290: 0015 0200 1500 1510 1502 0000 0015 0415  ................
+000002a0: 1015 144c 1502 1500 1200 0008 1c00 0000  ...L............
+000002b0: 0000 0000 0015 0015 1215 162c 150e 1510  ...........,....
+000002c0: 1506 1506 1c18 0800 0000 0000 0000 0018  ................
+000002d0: 0800 0000 0000 0000 0016 0028 0800 0000  ...........(....
+000002e0: 0000 0000 0018 0800 0000 0000 0000 0000  ................
+000002f0: 0000 0920 0200 0000 0e01 010e 0026 fa0b  ... .........&..
+00000300: 1c15 0419 3510 0006 1918 0872 615f 6572  ....5......ra_er
+00000310: 726f 7215 0216 0e16 b801 16c0 0126 ea0a  ror..........&..
+00000320: 26ba 0a1c 1808 0000 0000 0000 0000 1808  &...............
+00000330: 0000 0000 0000 0000 1600 2808 0000 0000  ..........(.....
+00000340: 0000 0000 1808 0000 0000 0000 0000 0019  ................
+00000350: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
+00000360: 0015 0415 1015 144c 1502 1500 1200 0008  .......L........
+00000370: 1c00 0000 0000 0000 0015 0015 1215 162c  ...............,
+00000380: 150e 1510 1506 1506 1c18 0800 0000 0000  ................
+00000390: 0000 0018 0800 0000 0000 0000 0016 0028  ...............(
+000003a0: 0800 0000 0000 0000 0018 0800 0000 0000  ................
+000003b0: 0000 0000 0000 0920 0200 0000 0e01 010e  ....... ........
+000003c0: 0026 820f 1c15 0419 3510 0006 1918 0964  .&......5......d
+000003d0: 6563 5f65 7272 6f72 1502 160e 16b8 0116  ec_error........
+000003e0: c001 26f2 0d26 c20d 1c18 0800 0000 0000  ..&..&..........
+000003f0: 0000 0018 0800 0000 0000 0000 0016 0028  ...............(
+00000400: 0800 0000 0000 0000 0018 0800 0000 0000  ................
+00000410: 0000 0000 192c 1504 1500 1502 0015 0015  .....,..........
+00000420: 1015 0200 0000 1504 196c 3500 1806 7363  .........l5...sc
+00000430: 6865 6d61 150a 0015 0425 0218 0269 6400  hema.....%...id.
+00000440: 150a 2502 1802 7261 0015 0a25 0218 0364  ..%...ra...%...d
+00000450: 6563 0015 0425 0218 0872 615f 6572 726f  ec...%...ra_erro
+00000460: 7200 1504 2502 1809 6465 635f 6572 726f  r...%...dec_erro
+00000470: 7200 160e 191c 195c 2688 021c 1504 1935  r......\&......5
+00000480: 1000 0619 1802 6964 1502 160e 169c 0216  ......id........
+00000490: 8002 2674 2608 1c18 083c 0300 0000 0000  ..&t&....<......
+000004a0: 0018 0823 0300 0000 0000 0016 0028 083c  ...#.........(.<
+000004b0: 0300 0000 0000 0018 0823 0300 0000 0000  .........#......
+000004c0: 0000 192c 1504 1500 1502 0015 0015 1015  ...,............
+000004d0: 0200 0000 26ba 051c 150a 1935 1000 0619  ....&......5....
+000004e0: 1802 7261 1502 160e 168c 0216 fa01 26a6  ..ra..........&.
+000004f0: 0426 c003 1c18 0800 0000 0000 d875 4018  .&...........u@.
+00000500: 0800 0000 0000 0874 4016 0028 0800 0000  .......t@..(....
+00000510: 0000 d875 4018 0800 0000 0000 0874 4000  ...u@........t@.
+00000520: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
+00000530: 0000 26fc 081c 150a 1935 1000 0619 1803  ..&......5......
+00000540: 6465 6315 0216 0e16 9c02 1686 0226 e807  dec..........&..
+00000550: 26f6 061c 1808 0000 0000 0080 39c0 1808  &...........9...
+00000560: 0000 0000 0040 4ec0 1600 2808 0000 0000  .....@N...(.....
+00000570: 0080 39c0 1808 0000 0000 0040 4ec0 0019  ..9........@N...
+00000580: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
+00000590: 0026 fa0b 1c15 0419 3510 0006 1918 0872  .&......5......r
+000005a0: 615f 6572 726f 7215 0216 0e16 b801 16c0  a_error.........
+000005b0: 0126 ea0a 26ba 0a1c 1808 0000 0000 0000  .&..&...........
+000005c0: 0000 1808 0000 0000 0000 0000 1600 2808  ..............(.
+000005d0: 0000 0000 0000 0000 1808 0000 0000 0000  ................
+000005e0: 0000 0019 2c15 0415 0015 0200 1500 1510  ....,...........
+000005f0: 1502 0000 0026 820f 1c15 0419 3510 0006  .....&......5...
+00000600: 1918 0964 6563 5f65 7272 6f72 1502 160e  ...dec_error....
+00000610: 16b8 0116 c001 26f2 0d26 c20d 1c18 0800  ......&..&......
+00000620: 0000 0000 0000 0018 0800 0000 0000 0000  ................
+00000630: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
+00000640: 0000 0000 0000 0000 192c 1504 1500 1502  .........,......
+00000650: 0015 0015 1015 0200 0000 16b4 0916 0e26  ...............&
+00000660: 0816 8009 1400 0019 2c18 0670 616e 6461  ........,..panda
+00000670: 7318 a705 7b22 696e 6465 785f 636f 6c75  s...{"index_colu
+00000680: 6d6e 7322 3a20 5b5d 2c20 2263 6f6c 756d  mns": [], "colum
+00000690: 6e5f 696e 6465 7865 7322 3a20 5b5d 2c20  n_indexes": [], 
+000006a0: 2263 6f6c 756d 6e73 223a 205b 7b22 6e61  "columns": [{"na
+000006b0: 6d65 223a 2022 6964 222c 2022 6669 656c  me": "id", "fiel
+000006c0: 645f 6e61 6d65 223a 2022 6964 222c 2022  d_name": "id", "
+000006d0: 7061 6e64 6173 5f74 7970 6522 3a20 2269  pandas_type": "i
+000006e0: 6e74 3634 222c 2022 6e75 6d70 795f 7479  nt64", "numpy_ty
+000006f0: 7065 223a 2022 696e 7436 3422 2c20 226d  pe": "int64", "m
+00000700: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
+00000710: 207b 226e 616d 6522 3a20 2272 6122 2c20   {"name": "ra", 
+00000720: 2266 6965 6c64 5f6e 616d 6522 3a20 2272  "field_name": "r
+00000730: 6122 2c20 2270 616e 6461 735f 7479 7065  a", "pandas_type
+00000740: 223a 2022 666c 6f61 7436 3422 2c20 226e  ": "float64", "n
+00000750: 756d 7079 5f74 7970 6522 3a20 2266 6c6f  umpy_type": "flo
+00000760: 6174 3634 222c 2022 6d65 7461 6461 7461  at64", "metadata
+00000770: 223a 206e 756c 6c7d 2c20 7b22 6e61 6d65  ": null}, {"name
+00000780: 223a 2022 6465 6322 2c20 2266 6965 6c64  ": "dec", "field
+00000790: 5f6e 616d 6522 3a20 2264 6563 222c 2022  _name": "dec", "
+000007a0: 7061 6e64 6173 5f74 7970 6522 3a20 2266  pandas_type": "f
+000007b0: 6c6f 6174 3634 222c 2022 6e75 6d70 795f  loat64", "numpy_
+000007c0: 7479 7065 223a 2022 666c 6f61 7436 3422  type": "float64"
+000007d0: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
+000007e0: 6c6c 7d2c 207b 226e 616d 6522 3a20 2272  ll}, {"name": "r
+000007f0: 615f 6572 726f 7222 2c20 2266 6965 6c64  a_error", "field
+00000800: 5f6e 616d 6522 3a20 2272 615f 6572 726f  _name": "ra_erro
+00000810: 7222 2c20 2270 616e 6461 735f 7479 7065  r", "pandas_type
+00000820: 223a 2022 696e 7436 3422 2c20 226e 756d  ": "int64", "num
+00000830: 7079 5f74 7970 6522 3a20 2269 6e74 3634  py_type": "int64
+00000840: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
+00000850: 756c 6c7d 2c20 7b22 6e61 6d65 223a 2022  ull}, {"name": "
+00000860: 6465 635f 6572 726f 7222 2c20 2266 6965  dec_error", "fie
+00000870: 6c64 5f6e 616d 6522 3a20 2264 6563 5f65  ld_name": "dec_e
+00000880: 7272 6f72 222c 2022 7061 6e64 6173 5f74  rror", "pandas_t
+00000890: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
+000008a0: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
+000008b0: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
+000008c0: 3a20 6e75 6c6c 7d5d 2c20 2263 7265 6174  : null}], "creat
+000008d0: 6f72 223a 207b 226c 6962 7261 7279 223a  or": {"library":
+000008e0: 2022 7079 6172 726f 7722 2c20 2276 6572   "pyarrow", "ver
+000008f0: 7369 6f6e 223a 2022 392e 302e 3022 7d2c  sion": "9.0.0"},
+00000900: 2022 7061 6e64 6173 5f76 6572 7369 6f6e   "pandas_version
+00000910: 223a 2022 322e 302e 3022 7d00 180c 4152  ": "2.0.0"}...AR
+00000920: 524f 573a 7363 6865 6d61 1898 0b2f 2f2f  ROW:schema...///
+00000930: 2f2f 7967 4541 4141 5141 4141 4141 4141  //ygEAAAQAAAAAAA
+00000940: 4b41 4134 4142 6741 4641 4167 4143 6741  KAA4ABgAFAAgACgA
+00000950: 4141 4141 4242 4141 5141 4141 4141 4141  AAAABBAAQAAAAAAA
+00000960: 4b41 4177 4141 4141 4541 4167 4143 6741  KAAwAAAAEAAgACgA
+00000970: 4141 4e77 4341 4141 4541 4141 4141 5141  AANwCAAAEAAAAAQA
+00000980: 4141 4177 4141 4141 4941 4177 4142 4141  AAAwAAAAIAAwABAA
+00000990: 4941 4167 4141 4141 4941 4141 4145 4141  IAAgAAAAIAAAAEAA
+000009a0: 4141 4159 4141 4142 7759 5735 6b59 584d  AAAYAAABwYW5kYXM
+000009b0: 4141 4b63 4341 4142 3749 6d6c 755a 4756  AAKcCAAB7ImluZGV
+000009c0: 3458 324e 7662 4856 7462 6e4d 694f 6942  4X2NvbHVtbnMiOiB
+000009d0: 6258 5377 6749 6d4e 7662 4856 7462 6c39  bXSwgImNvbHVtbl9
+000009e0: 7062 6d52 6c65 4756 7a49 6a6f 6757 3130  pbmRleGVzIjogW10
+000009f0: 7349 434a 6a62 3278 3162 5735 7a49 6a6f  sICJjb2x1bW5zIjo
+00000a00: 6757 3373 6962 6d46 745a 5349 3649 434a  gW3sibmFtZSI6ICJ
+00000a10: 705a 4349 7349 434a 6d61 5756 735a 4639  pZCIsICJmaWVsZF9
+00000a20: 7559 5731 6c49 6a6f 6749 6d6c 6b49 6977  uYW1lIjogImlkIiw
+00000a30: 6749 6e42 6862 6d52 6863 3139 3065 5842  gInBhbmRhc190eXB
+00000a40: 6c49 6a6f 6749 6d6c 7564 4459 3049 6977  lIjogImludDY0Iiw
+00000a50: 6749 6d35 3162 5842 3558 3352 3563 4755  gIm51bXB5X3R5cGU
+00000a60: 694f 6941 6961 5735 304e 6a51 694c 4341  iOiAiaW50NjQiLCA
+00000a70: 6962 5756 3059 5752 6864 4745 694f 6942  ibWV0YWRhdGEiOiB
+00000a80: 7564 5778 7366 5377 6765 794a 7559 5731  udWxsfSwgeyJuYW1
+00000a90: 6c49 6a6f 6749 6e4a 6849 6977 6749 6d5a  lIjogInJhIiwgImZ
+00000aa0: 705a 5778 6b58 3235 6862 5755 694f 6941  pZWxkX25hbWUiOiA
+00000ab0: 6963 6d45 694c 4341 6963 4746 755a 4746  icmEiLCAicGFuZGF
+00000ac0: 7a58 3352 3563 4755 694f 6941 695a 6d78  zX3R5cGUiOiAiZmx
+00000ad0: 7659 5851 324e 4349 7349 434a 7564 5731  vYXQ2NCIsICJudW1
+00000ae0: 7765 5639 3065 5842 6c49 6a6f 6749 6d5a  weV90eXBlIjogImZ
+00000af0: 7362 3246 304e 6a51 694c 4341 6962 5756  sb2F0NjQiLCAibWV
+00000b00: 3059 5752 6864 4745 694f 6942 7564 5778  0YWRhdGEiOiBudWx
+00000b10: 7366 5377 6765 794a 7559 5731 6c49 6a6f  sfSwgeyJuYW1lIjo
+00000b20: 6749 6d52 6c59 7949 7349 434a 6d61 5756  gImRlYyIsICJmaWV
+00000b30: 735a 4639 7559 5731 6c49 6a6f 6749 6d52  sZF9uYW1lIjogImR
+00000b40: 6c59 7949 7349 434a 7759 5735 6b59 584e  lYyIsICJwYW5kYXN
+00000b50: 6664 486c 775a 5349 3649 434a 6d62 4739  fdHlwZSI6ICJmbG9
+00000b60: 6864 4459 3049 6977 6749 6d35 3162 5842  hdDY0IiwgIm51bXB
+00000b70: 3558 3352 3563 4755 694f 6941 695a 6d78  5X3R5cGUiOiAiZmx
+00000b80: 7659 5851 324e 4349 7349 434a 745a 5852  vYXQ2NCIsICJtZXR
+00000b90: 685a 4746 3059 5349 3649 4735 3162 4778  hZGF0YSI6IG51bGx
+00000ba0: 394c 4342 3749 6d35 6862 5755 694f 6941  9LCB7Im5hbWUiOiA
+00000bb0: 6963 6d46 665a 584a 7962 3349 694c 4341  icmFfZXJyb3IiLCA
+00000bc0: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
+00000bd0: 3649 434a 7959 5639 6c63 6e4a 7663 6949  6ICJyYV9lcnJvciI
+00000be0: 7349 434a 7759 5735 6b59 584e 6664 486c  sICJwYW5kYXNfdHl
+00000bf0: 775a 5349 3649 434a 7062 6e51 324e 4349  wZSI6ICJpbnQ2NCI
+00000c00: 7349 434a 7564 5731 7765 5639 3065 5842  sICJudW1weV90eXB
+00000c10: 6c49 6a6f 6749 6d6c 7564 4459 3049 6977  lIjogImludDY0Iiw
+00000c20: 6749 6d31 6c64 4746 6b59 5852 6849 6a6f  gIm1ldGFkYXRhIjo
+00000c30: 6762 6e56 7362 4830 7349 4873 6962 6d46  gbnVsbH0sIHsibmF
+00000c40: 745a 5349 3649 434a 6b5a 574e 665a 584a  tZSI6ICJkZWNfZXJ
+00000c50: 7962 3349 694c 4341 695a 6d6c 6c62 4752  yb3IiLCAiZmllbGR
+00000c60: 6662 6d46 745a 5349 3649 434a 6b5a 574e  fbmFtZSI6ICJkZWN
+00000c70: 665a 584a 7962 3349 694c 4341 6963 4746  fZXJyb3IiLCAicGF
+00000c80: 755a 4746 7a58 3352 3563 4755 694f 6941  uZGFzX3R5cGUiOiA
+00000c90: 6961 5735 304e 6a51 694c 4341 6962 6e56  iaW50NjQiLCAibnV
+00000ca0: 7463 486c 6664 486c 775a 5349 3649 434a  tcHlfdHlwZSI6ICJ
+00000cb0: 7062 6e51 324e 4349 7349 434a 745a 5852  pbnQ2NCIsICJtZXR
+00000cc0: 685a 4746 3059 5349 3649 4735 3162 4778  hZGF0YSI6IG51bGx
+00000cd0: 3958 5377 6749 6d4e 795a 5746 3062 3349  9XSwgImNyZWF0b3I
+00000ce0: 694f 6942 3749 6d78 7059 6e4a 6863 6e6b  iOiB7ImxpYnJhcnk
+00000cf0: 694f 6941 6963 486c 6863 6e4a 7664 7949  iOiAicHlhcnJvdyI
+00000d00: 7349 434a 325a 584a 7a61 5739 7549 6a6f  sICJ2ZXJzaW9uIjo
+00000d10: 6749 6a6b 754d 4334 7749 6e30 7349 434a  gIjkuMC4wIn0sICJ
+00000d20: 7759 5735 6b59 584e 6664 6d56 7963 326c  wYW5kYXNfdmVyc2l
+00000d30: 7662 6949 3649 4349 794c 6a41 754d 434a  vbiI6ICIyLjAuMCJ
+00000d40: 3941 4155 4141 4144 6b41 4141 416f 4141  9AAUAAADkAAAAoAA
+00000d50: 4141 4851 4141 4141 3841 4141 4142 4141  AAHQAAAA8AAAABAA
+00000d60: 4141 4544 2f2f 2f38 4141 4145 4345 4141  AAED///8AAAECEAA
+00000d70: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
+00000d80: 4141 416b 4141 4142 6b5a 574e 665a 584a  AAAkAAABkZWNfZXJ
+00000d90: 7962 3349 4141 4141 342f 2f2f 2f41 4141  yb3IAAAA4////AAA
+00000da0: 4141 5541 4141 4142 302f 2f2f 2f41 4141  AAUAAAAB0////AAA
+00000db0: 4241 6841 4141 4141 6341 4141 4142 4141  BAhAAAAAcAAAABAA
+00000dc0: 4141 4141 4141 4141 4941 4141 4163 6d46  AAAAAAAAIAAAAcmF
+00000dd0: 665a 584a 7962 3349 4141 4141 4162 502f  fZXJyb3IAAAAAbP/
+00000de0: 2f2f 7741 4141 4146 4141 4141 4171 502f  //wAAAAFAAAAAqP/
+00000df0: 2f2f 7741 4141 514d 5141 4141 4146 4141  //wAAAQMQAAAAFAA
+00000e00: 4141 4151 4141 4141 4141 4141 4141 7741  AAAQAAAAAAAAAAwA
+00000e10: 4141 4752 6c59 7744 572f 2f2f 2f41 4141  AAGRlYwDW////AAA
+00000e20: 4341 4e44 2f2f 2f38 4141 4145 4445 4141  CAND///8AAAEDEAA
+00000e30: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
+00000e40: 4141 4149 4141 4142 7959 5141 4141 4141  AAAIAAAByYQAAAAA
+00000e50: 4741 4167 4142 6741 4741 4141 4141 4141  GAAgABgAGAAAAAAA
+00000e60: 4341 4241 4146 4141 4941 4159 4142 7741  CABAAFAAIAAYABwA
+00000e70: 4d41 4141 4145 4141 5141 4141 4141 4141  MAAAAEAAQAAAAAAA
+00000e80: 4241 6841 4141 4141 6341 4141 4142 4141  BAhAAAAAcAAAABAA
+00000e90: 4141 4141 4141 4141 4341 4141 4161 5751  AAAAAAAACAAAAaWQ
+00000ea0: 4141 4167 4144 4141 4941 4163 4143 4141  AAAgADAAIAAcACAA
+00000eb0: 4141 4141 4141 4146 4141 4141 4141 4141  AAAAAAAFAAAAAAAA
+00000ec0: 4141 413d 3d00 181f 7061 7271 7565 742d  AAA==...parquet-
+00000ed0: 6370 702d 6172 726f 7720 7665 7273 696f  cpp-arrow versio
+00000ee0: 6e20 392e 302e 3019 5c1c 0000 1c00 001c  n 9.0.0.\.......
+00000ef0: 0000 1c00 001c 0000 00d3 0a00 0050 4152  .............PAR
+00000f00: 31                                       1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_44/shard_3.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet`

 * *Files 13% similar despite different names*

```diff
@@ -64,248 +64,181 @@
 000003f0: 0000 0009 2002 0000 0016 0101 1600 26fc  .... .........&.
 00000400: 0f1c 1504 1935 1000 0619 1809 6465 635f  .....5......dec_
 00000410: 6572 726f 7215 0216 1616 b801 16c0 0126  error..........&
 00000420: ec0e 26bc 0e1c 1808 0000 0000 0000 0000  ..&.............
 00000430: 1808 0000 0000 0000 0000 1600 2808 0000  ............(...
 00000440: 0000 0000 0000 1808 0000 0000 0000 0000  ................
 00000450: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
-00000460: 0000 0015 0415 b001 1570 4c15 1615 0012  .........pL.....
-00000470: 0000 5804 0400 0901 0005 0907 0400 080d  ..X.............
-00000480: 0800 090d 0800 0a0d 0800 0b0d 0800 0d0d  ................
-00000490: 0800 0e0d 0800 160d 083c 1700 0000 0000  .........<......
-000004a0: 0000 1900 0000 0000 0000 1500 1520 1524  ............. .$
-000004b0: 2c15 1615 1015 0615 061c 1808 1900 0000  ,...............
-000004c0: 0000 0000 1808 0400 0000 0000 0000 1600  ................
-000004d0: 2808 1900 0000 0000 0000 1808 0400 0000  (...............
-000004e0: 0000 0000 0000 0010 3c02 0000 0016 0104  ........<.......
-000004f0: 0510 3254 7698 0a00 0026 f213 1c15 0419  ..2Tv....&......
-00000500: 3510 0006 1918 115f 5f69 6e64 6578 5f6c  5......__index_l
-00000510: 6576 656c 5f30 5f5f 1502 1616 16e8 0216  evel_0__........
-00000520: ac02 26d4 1226 c611 1c18 0819 0000 0000  ..&..&..........
-00000530: 0000 0018 0804 0000 0000 0000 0016 0028  ...............(
-00000540: 0819 0000 0000 0000 0018 0804 0000 0000  ................
-00000550: 0000 0000 192c 1504 1500 1502 0015 0015  .....,..........
-00000560: 1015 0200 0000 1504 197c 3500 1806 7363  .........|5...sc
-00000570: 6865 6d61 150c 0015 0425 0218 0269 6400  hema.....%...id.
-00000580: 150a 2502 1802 7261 0015 0a25 0218 0364  ..%...ra...%...d
-00000590: 6563 0015 0425 0218 0872 615f 6572 726f  ec...%...ra_erro
-000005a0: 7200 1504 2502 1809 6465 635f 6572 726f  r...%...dec_erro
-000005b0: 7200 1504 2502 1811 5f5f 696e 6465 785f  r...%...__index_
-000005c0: 6c65 7665 6c5f 305f 5f00 1616 191c 196c  level_0__......l
-000005d0: 26b4 021c 1504 1935 1000 0619 1802 6964  &......5......id
-000005e0: 1502 1616 16e8 0216 ac02 2696 0126 081c  ..........&..&..
-000005f0: 1808 ee02 0000 0000 0000 1808 d902 0000  ................
-00000600: 0000 0000 1600 2808 ee02 0000 0000 0000  ......(.........
-00000610: 1808 d902 0000 0000 0000 0019 2c15 0415  ............,...
-00000620: 0015 0200 1500 1510 1502 0000 0026 9606  .............&..
-00000630: 1c15 0a19 3510 0006 1918 0272 6115 0216  ....5......ra...
-00000640: 1616 d802 16a8 0226 f804 26ee 031c 1808  .......&..&.....
-00000650: 0000 0000 00c8 7540 1808 0000 0000 0088  ......u@........
-00000660: 7240 1600 2808 0000 0000 00c8 7540 1808  r@..(.......u@..
-00000670: 0000 0000 0088 7240 0019 2c15 0415 0015  ......r@..,.....
-00000680: 0200 1500 1510 1502 0000 0026 f609 1c15  ...........&....
-00000690: 0a19 3510 0006 1918 0364 6563 1502 1616  ..5......dec....
-000006a0: 16c8 0216 a402 26d8 0826 d207 1c18 0800  ......&..&......
-000006b0: 0000 0000 404a c018 0800 0000 0000 e050  ....@J.........P
-000006c0: c016 0028 0800 0000 0000 404a c018 0800  ...(......@J....
-000006d0: 0000 0000 e050 c000 192c 1504 1500 1502  .....P...,......
-000006e0: 0015 0015 1015 0200 0000 26f4 0c1c 1504  ..........&.....
-000006f0: 1935 1000 0619 1808 7261 5f65 7272 6f72  .5......ra_error
-00000700: 1502 1616 16b8 0116 c001 26e4 0b26 b40b  ..........&..&..
-00000710: 1c18 0800 0000 0000 0000 0018 0800 0000  ................
-00000720: 0000 0000 0016 0028 0800 0000 0000 0000  .......(........
-00000730: 0018 0800 0000 0000 0000 0000 192c 1504  .............,..
-00000740: 1500 1502 0015 0015 1015 0200 0000 26fc  ..............&.
-00000750: 0f1c 1504 1935 1000 0619 1809 6465 635f  .....5......dec_
-00000760: 6572 726f 7215 0216 1616 b801 16c0 0126  error..........&
-00000770: ec0e 26bc 0e1c 1808 0000 0000 0000 0000  ..&.............
-00000780: 1808 0000 0000 0000 0000 1600 2808 0000  ............(...
-00000790: 0000 0000 0000 1808 0000 0000 0000 0000  ................
-000007a0: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
-000007b0: 0000 0026 f213 1c15 0419 3510 0006 1918  ...&......5.....
-000007c0: 115f 5f69 6e64 6578 5f6c 6576 656c 5f30  .__index_level_0
-000007d0: 5f5f 1502 1616 16e8 0216 ac02 26d4 1226  __..........&..&
-000007e0: c611 1c18 0819 0000 0000 0000 0018 0804  ................
-000007f0: 0000 0000 0000 0016 0028 0819 0000 0000  .........(......
-00000800: 0000 0018 0804 0000 0000 0000 0000 192c  ...............,
-00000810: 1504 1500 1502 0015 0015 1015 0200 0000  ................
-00000820: 16e0 0d16 1626 0816 a40c 1400 0019 2c18  .....&........,.
-00000830: 0670 616e 6461 7318 a507 7b22 696e 6465  .pandas...{"inde
-00000840: 785f 636f 6c75 6d6e 7322 3a20 5b22 5f5f  x_columns": ["__
-00000850: 696e 6465 785f 6c65 7665 6c5f 305f 5f22  index_level_0__"
-00000860: 5d2c 2022 636f 6c75 6d6e 5f69 6e64 6578  ], "column_index
-00000870: 6573 223a 205b 7b22 6e61 6d65 223a 206e  es": [{"name": n
-00000880: 756c 6c2c 2022 6669 656c 645f 6e61 6d65  ull, "field_name
-00000890: 223a 206e 756c 6c2c 2022 7061 6e64 6173  ": null, "pandas
-000008a0: 5f74 7970 6522 3a20 2275 6e69 636f 6465  _type": "unicode
-000008b0: 222c 2022 6e75 6d70 795f 7479 7065 223a  ", "numpy_type":
-000008c0: 2022 6f62 6a65 6374 222c 2022 6d65 7461   "object", "meta
-000008d0: 6461 7461 223a 207b 2265 6e63 6f64 696e  data": {"encodin
-000008e0: 6722 3a20 2255 5446 2d38 227d 7d5d 2c20  g": "UTF-8"}}], 
-000008f0: 2263 6f6c 756d 6e73 223a 205b 7b22 6e61  "columns": [{"na
-00000900: 6d65 223a 2022 6964 222c 2022 6669 656c  me": "id", "fiel
-00000910: 645f 6e61 6d65 223a 2022 6964 222c 2022  d_name": "id", "
-00000920: 7061 6e64 6173 5f74 7970 6522 3a20 2269  pandas_type": "i
-00000930: 6e74 3634 222c 2022 6e75 6d70 795f 7479  nt64", "numpy_ty
-00000940: 7065 223a 2022 696e 7436 3422 2c20 226d  pe": "int64", "m
-00000950: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
-00000960: 207b 226e 616d 6522 3a20 2272 6122 2c20   {"name": "ra", 
-00000970: 2266 6965 6c64 5f6e 616d 6522 3a20 2272  "field_name": "r
-00000980: 6122 2c20 2270 616e 6461 735f 7479 7065  a", "pandas_type
-00000990: 223a 2022 666c 6f61 7436 3422 2c20 226e  ": "float64", "n
-000009a0: 756d 7079 5f74 7970 6522 3a20 2266 6c6f  umpy_type": "flo
-000009b0: 6174 3634 222c 2022 6d65 7461 6461 7461  at64", "metadata
-000009c0: 223a 206e 756c 6c7d 2c20 7b22 6e61 6d65  ": null}, {"name
-000009d0: 223a 2022 6465 6322 2c20 2266 6965 6c64  ": "dec", "field
-000009e0: 5f6e 616d 6522 3a20 2264 6563 222c 2022  _name": "dec", "
-000009f0: 7061 6e64 6173 5f74 7970 6522 3a20 2266  pandas_type": "f
-00000a00: 6c6f 6174 3634 222c 2022 6e75 6d70 795f  loat64", "numpy_
-00000a10: 7479 7065 223a 2022 666c 6f61 7436 3422  type": "float64"
-00000a20: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
-00000a30: 6c6c 7d2c 207b 226e 616d 6522 3a20 2272  ll}, {"name": "r
-00000a40: 615f 6572 726f 7222 2c20 2266 6965 6c64  a_error", "field
-00000a50: 5f6e 616d 6522 3a20 2272 615f 6572 726f  _name": "ra_erro
-00000a60: 7222 2c20 2270 616e 6461 735f 7479 7065  r", "pandas_type
-00000a70: 223a 2022 696e 7436 3422 2c20 226e 756d  ": "int64", "num
-00000a80: 7079 5f74 7970 6522 3a20 2269 6e74 3634  py_type": "int64
-00000a90: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
-00000aa0: 756c 6c7d 2c20 7b22 6e61 6d65 223a 2022  ull}, {"name": "
-00000ab0: 6465 635f 6572 726f 7222 2c20 2266 6965  dec_error", "fie
-00000ac0: 6c64 5f6e 616d 6522 3a20 2264 6563 5f65  ld_name": "dec_e
-00000ad0: 7272 6f72 222c 2022 7061 6e64 6173 5f74  rror", "pandas_t
-00000ae0: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
-00000af0: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
-00000b00: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
-00000b10: 3a20 6e75 6c6c 7d2c 207b 226e 616d 6522  : null}, {"name"
-00000b20: 3a20 6e75 6c6c 2c20 2266 6965 6c64 5f6e  : null, "field_n
-00000b30: 616d 6522 3a20 225f 5f69 6e64 6578 5f6c  ame": "__index_l
-00000b40: 6576 656c 5f30 5f5f 222c 2022 7061 6e64  evel_0__", "pand
-00000b50: 6173 5f74 7970 6522 3a20 2269 6e74 3634  as_type": "int64
-00000b60: 222c 2022 6e75 6d70 795f 7479 7065 223a  ", "numpy_type":
-00000b70: 2022 696e 7436 3422 2c20 226d 6574 6164   "int64", "metad
-00000b80: 6174 6122 3a20 6e75 6c6c 7d5d 2c20 2263  ata": null}], "c
-00000b90: 7265 6174 6f72 223a 207b 226c 6962 7261  reator": {"libra
-00000ba0: 7279 223a 2022 7079 6172 726f 7722 2c20  ry": "pyarrow", 
-00000bb0: 2276 6572 7369 6f6e 223a 2022 392e 302e  "version": "9.0.
-00000bc0: 3022 7d2c 2022 7061 6e64 6173 5f76 6572  0"}, "pandas_ver
-00000bd0: 7369 6f6e 223a 2022 312e 332e 3522 7d00  sion": "1.3.5"}.
-00000be0: 180c 4152 524f 573a 7363 6865 6d61 18c0  ..ARROW:schema..
-00000bf0: 0e2f 2f2f 2f2f 3267 4641 4141 5141 4141  ./////2gFAAAQAAA
-00000c00: 4141 4141 4b41 4134 4142 6741 4641 4167  AAAAKAA4ABgAFAAg
-00000c10: 4143 6741 4141 4141 4242 4141 5141 4141  ACgAAAAABBAAQAAA
-00000c20: 4141 4141 4b41 4177 4141 4141 4541 4167  AAAAKAAwAAAAEAAg
-00000c30: 4143 6741 4141 4e77 4441 4141 4541 4141  ACgAAANwDAAAEAAA
-00000c40: 4141 5141 4141 4177 4141 4141 4941 4177  AAQAAAAwAAAAIAAw
-00000c50: 4142 4141 4941 4167 4141 4141 4941 4141  ABAAIAAgAAAAIAAA
-00000c60: 4145 4141 4141 4159 4141 4142 7759 5735  AEAAAAAYAAABwYW5
-00000c70: 6b59 584d 4141 4b55 4441 4142 3749 6d6c  kYXMAAKUDAAB7Iml
-00000c80: 755a 4756 3458 324e 7662 4856 7462 6e4d  uZGV4X2NvbHVtbnM
-00000c90: 694f 6942 6249 6c39 6661 5735 6b5a 5868  iOiBbIl9faW5kZXh
-00000ca0: 6662 4756 325a 5778 664d 4639 6649 6c30  fbGV2ZWxfMF9fIl0
-00000cb0: 7349 434a 6a62 3278 3162 5735 6661 5735  sICJjb2x1bW5faW5
-00000cc0: 6b5a 5868 6c63 7949 3649 4674 3749 6d35  kZXhlcyI6IFt7Im5
-00000cd0: 6862 5755 694f 6942 7564 5778 734c 4341  hbWUiOiBudWxsLCA
-00000ce0: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
-00000cf0: 3649 4735 3162 4777 7349 434a 7759 5735  6IG51bGwsICJwYW5
-00000d00: 6b59 584e 6664 486c 775a 5349 3649 434a  kYXNfdHlwZSI6ICJ
-00000d10: 3162 6d6c 6a62 3252 6c49 6977 6749 6d35  1bmljb2RlIiwgIm5
-00000d20: 3162 5842 3558 3352 3563 4755 694f 6941  1bXB5X3R5cGUiOiA
-00000d30: 6962 324a 715a 574e 3049 6977 6749 6d31  ib2JqZWN0IiwgIm1
-00000d40: 6c64 4746 6b59 5852 6849 6a6f 6765 794a  ldGFkYXRhIjogeyJ
-00000d50: 6c62 6d4e 765a 476c 755a 7949 3649 434a  lbmNvZGluZyI6ICJ
-00000d60: 5656 4559 744f 434a 3966 5630 7349 434a  VVEYtOCJ9fV0sICJ
-00000d70: 6a62 3278 3162 5735 7a49 6a6f 6757 3373  jb2x1bW5zIjogW3s
-00000d80: 6962 6d46 745a 5349 3649 434a 705a 4349  ibmFtZSI6ICJpZCI
-00000d90: 7349 434a 6d61 5756 735a 4639 7559 5731  sICJmaWVsZF9uYW1
-00000da0: 6c49 6a6f 6749 6d6c 6b49 6977 6749 6e42  lIjogImlkIiwgInB
-00000db0: 6862 6d52 6863 3139 3065 5842 6c49 6a6f  hbmRhc190eXBlIjo
-00000dc0: 6749 6d6c 7564 4459 3049 6977 6749 6d35  gImludDY0IiwgIm5
-00000dd0: 3162 5842 3558 3352 3563 4755 694f 6941  1bXB5X3R5cGUiOiA
-00000de0: 6961 5735 304e 6a51 694c 4341 6962 5756  iaW50NjQiLCAibWV
-00000df0: 3059 5752 6864 4745 694f 6942 7564 5778  0YWRhdGEiOiBudWx
-00000e00: 7366 5377 6765 794a 7559 5731 6c49 6a6f  sfSwgeyJuYW1lIjo
-00000e10: 6749 6e4a 6849 6977 6749 6d5a 705a 5778  gInJhIiwgImZpZWx
-00000e20: 6b58 3235 6862 5755 694f 6941 6963 6d45  kX25hbWUiOiAicmE
-00000e30: 694c 4341 6963 4746 755a 4746 7a58 3352  iLCAicGFuZGFzX3R
-00000e40: 3563 4755 694f 6941 695a 6d78 7659 5851  5cGUiOiAiZmxvYXQ
-00000e50: 324e 4349 7349 434a 7564 5731 7765 5639  2NCIsICJudW1weV9
-00000e60: 3065 5842 6c49 6a6f 6749 6d5a 7362 3246  0eXBlIjogImZsb2F
-00000e70: 304e 6a51 694c 4341 6962 5756 3059 5752  0NjQiLCAibWV0YWR
-00000e80: 6864 4745 694f 6942 7564 5778 7366 5377  hdGEiOiBudWxsfSw
-00000e90: 6765 794a 7559 5731 6c49 6a6f 6749 6d52  geyJuYW1lIjogImR
-00000ea0: 6c59 7949 7349 434a 6d61 5756 735a 4639  lYyIsICJmaWVsZF9
-00000eb0: 7559 5731 6c49 6a6f 6749 6d52 6c59 7949  uYW1lIjogImRlYyI
-00000ec0: 7349 434a 7759 5735 6b59 584e 6664 486c  sICJwYW5kYXNfdHl
-00000ed0: 775a 5349 3649 434a 6d62 4739 6864 4459  wZSI6ICJmbG9hdDY
-00000ee0: 3049 6977 6749 6d35 3162 5842 3558 3352  0IiwgIm51bXB5X3R
-00000ef0: 3563 4755 694f 6941 695a 6d78 7659 5851  5cGUiOiAiZmxvYXQ
-00000f00: 324e 4349 7349 434a 745a 5852 685a 4746  2NCIsICJtZXRhZGF
-00000f10: 3059 5349 3649 4735 3162 4778 394c 4342  0YSI6IG51bGx9LCB
-00000f20: 3749 6d35 6862 5755 694f 6941 6963 6d46  7Im5hbWUiOiAicmF
-00000f30: 665a 584a 7962 3349 694c 4341 695a 6d6c  fZXJyb3IiLCAiZml
-00000f40: 6c62 4752 6662 6d46 745a 5349 3649 434a  lbGRfbmFtZSI6ICJ
-00000f50: 7959 5639 6c63 6e4a 7663 6949 7349 434a  yYV9lcnJvciIsICJ
-00000f60: 7759 5735 6b59 584e 6664 486c 775a 5349  wYW5kYXNfdHlwZSI
-00000f70: 3649 434a 7062 6e51 324e 4349 7349 434a  6ICJpbnQ2NCIsICJ
-00000f80: 7564 5731 7765 5639 3065 5842 6c49 6a6f  udW1weV90eXBlIjo
-00000f90: 6749 6d6c 7564 4459 3049 6977 6749 6d31  gImludDY0IiwgIm1
-00000fa0: 6c64 4746 6b59 5852 6849 6a6f 6762 6e56  ldGFkYXRhIjogbnV
-00000fb0: 7362 4830 7349 4873 6962 6d46 745a 5349  sbH0sIHsibmFtZSI
-00000fc0: 3649 434a 6b5a 574e 665a 584a 7962 3349  6ICJkZWNfZXJyb3I
-00000fd0: 694c 4341 695a 6d6c 6c62 4752 6662 6d46  iLCAiZmllbGRfbmF
-00000fe0: 745a 5349 3649 434a 6b5a 574e 665a 584a  tZSI6ICJkZWNfZXJ
-00000ff0: 7962 3349 694c 4341 6963 4746 755a 4746  yb3IiLCAicGFuZGF
-00001000: 7a58 3352 3563 4755 694f 6941 6961 5735  zX3R5cGUiOiAiaW5
-00001010: 304e 6a51 694c 4341 6962 6e56 7463 486c  0NjQiLCAibnVtcHl
-00001020: 6664 486c 775a 5349 3649 434a 7062 6e51  fdHlwZSI6ICJpbnQ
-00001030: 324e 4349 7349 434a 745a 5852 685a 4746  2NCIsICJtZXRhZGF
-00001040: 3059 5349 3649 4735 3162 4778 394c 4342  0YSI6IG51bGx9LCB
-00001050: 3749 6d35 6862 5755 694f 6942 7564 5778  7Im5hbWUiOiBudWx
-00001060: 734c 4341 695a 6d6c 6c62 4752 6662 6d46  sLCAiZmllbGRfbmF
-00001070: 745a 5349 3649 434a 6658 326c 755a 4756  tZSI6ICJfX2luZGV
-00001080: 3458 3278 6c64 6d56 7358 7a42 6658 7949  4X2xldmVsXzBfXyI
-00001090: 7349 434a 7759 5735 6b59 584e 6664 486c  sICJwYW5kYXNfdHl
-000010a0: 775a 5349 3649 434a 7062 6e51 324e 4349  wZSI6ICJpbnQ2NCI
-000010b0: 7349 434a 7564 5731 7765 5639 3065 5842  sICJudW1weV90eXB
-000010c0: 6c49 6a6f 6749 6d6c 7564 4459 3049 6977  lIjogImludDY0Iiw
-000010d0: 6749 6d31 6c64 4746 6b59 5852 6849 6a6f  gIm1ldGFkYXRhIjo
-000010e0: 6762 6e56 7362 4831 644c 4341 6959 334a  gbnVsbH1dLCAiY3J
-000010f0: 6c59 5852 7663 6949 3649 4873 6962 476c  lYXRvciI6IHsibGl
-00001100: 6963 6d46 7965 5349 3649 434a 7765 5746  icmFyeSI6ICJweWF
-00001110: 7963 6d39 3349 6977 6749 6e5a 6c63 6e4e  ycm93IiwgInZlcnN
-00001120: 7062 3234 694f 6941 694f 5334 774c 6a41  pb24iOiAiOS4wLjA
-00001130: 6966 5377 6749 6e42 6862 6d52 6863 3139  ifSwgInBhbmRhc19
-00001140: 325a 584a 7a61 5739 7549 6a6f 6749 6a45  2ZXJzaW9uIjogIjE
-00001150: 754d 7934 3149 6e30 4141 4141 4741 4141  uMy41In0AAAAGAAA
-00001160: 414a 4145 4141 4f41 4141 4143 3041 4141  AJAEAAOAAAAC0AAA
-00001170: 4166 4141 4141 4551 4141 4141 4541 4141  AfAAAAEQAAAAEAAA
-00001180: 4142 502f 2f2f 7741 4141 5149 5141 4141  ABP///wAAAQIQAAA
-00001190: 414a 4141 4141 4151 4141 4141 4141 4141  AJAAAAAQAAAAAAAA
-000011a0: 4145 5141 4141 4639 6661 5735 6b5a 5868  AEQAAAF9faW5kZXh
-000011b0: 6662 4756 325a 5778 664d 4639 6641 4141  fbGV2ZWxfMF9fAAA
-000011c0: 4142 502f 2f2f 7741 4141 4146 4141 4141  ABP///wAAAAFAAAA
-000011d0: 4151 502f 2f2f 7741 4141 5149 5141 4141  AQP///wAAAQIQAAA
-000011e0: 4148 4141 4141 4151 4141 4141 4141 4141  AHAAAAAQAAAAAAAA
-000011f0: 4143 5141 4141 4752 6c59 3139 6c63 6e4a  ACQAAAGRlY19lcnJ
-00001200: 7663 6741 4141 446a 2f2f 2f38 4141 4141  vcgAAADj///8AAAA
-00001210: 4251 4141 4141 4854 2f2f 2f38 4141 4145  BQAAAAHT///8AAAE
-00001220: 4345 4141 4141 4277 4141 4141 4541 4141  CEAAAABwAAAAEAAA
-00001230: 4141 4141 4141 4167 4141 4142 7959 5639  AAAAAAAgAAAByYV9
-00001240: 6c63 6e4a 7663 6741 4141 4142 732f 2f2f  lcnJvcgAAAABs///
-00001250: 2f41 4141 4141 5541 4141 4143 6f2f 2f2f  /AAAAAUAAAACo///
-00001260: 2f41 4141 4241 7841 4141 4141 5541 4141  /AAABAxAAAAAUAAA
-00001270: 4142 4141 4141 4141 4141 4141 4441 4141  ABAAAAAAAAAADAAA
-00001280: 415a 4756 6a41 4e62 2f2f 2f38 4141 4149  AZGVjANb///8AAAI
-00001290: 4130 502f 2f2f 7741 4141 514d 5141 4141  A0P///wAAAQMQAAA
-000012a0: 4148 4141 4141 4151 4141 4141 4141 4141  AHAAAAAQAAAAAAAA
-000012b0: 4141 6741 4141 484a 6841 4141 4141 4159  AAgAAAHJhAAAAAAY
-000012c0: 4143 4141 4741 4159 4141 4141 4141 4149  ACAAGAAYAAAAAAAI
-000012d0: 4145 4141 5541 4167 4142 6741 4841 4177  AEAAUAAgABgAHAAw
-000012e0: 4141 4141 5141 4241 4141 4141 4141 4145  AAAAQABAAAAAAAAE
-000012f0: 4345 4141 4141 4277 4141 4141 4541 4141  CEAAAABwAAAAEAAA
-00001300: 4141 4141 4141 4149 4141 4142 705a 4141  AAAAAAAIAAABpZAA
-00001310: 4143 4141 4d41 4167 4142 7741 4941 4141  ACAAMAAgABwAIAAA
-00001320: 4141 4141 4141 5541 4141 4141 4141 4141  AAAAAAUAAAAAAAAA
-00001330: 4100 181f 7061 7271 7565 742d 6370 702d  A...parquet-cpp-
-00001340: 6172 726f 7720 7665 7273 696f 6e20 392e  arrow version 9.
-00001350: 302e 3019 6c1c 0000 1c00 001c 0000 1c00  0.0.l...........
-00001360: 001c 0000 1c00 0000 020e 0000 5041 5231  ............PAR1
+00000460: 0000 0015 0419 6c35 0018 0673 6368 656d  ......l5...schem
+00000470: 6115 0a00 1504 2502 1802 6964 0015 0a25  a.....%...id...%
+00000480: 0218 0272 6100 150a 2502 1803 6465 6300  ...ra...%...dec.
+00000490: 1504 2502 1808 7261 5f65 7272 6f72 0015  ..%...ra_error..
+000004a0: 0425 0218 0964 6563 5f65 7272 6f72 0016  .%...dec_error..
+000004b0: 1619 1c19 5c26 b402 1c15 0419 3510 0006  ....\&......5...
+000004c0: 1918 0269 6415 0216 1616 e802 16ac 0226  ...id..........&
+000004d0: 9601 2608 1c18 08ee 0200 0000 0000 0018  ..&.............
+000004e0: 08d9 0200 0000 0000 0016 0028 08ee 0200  ...........(....
+000004f0: 0000 0000 0018 08d9 0200 0000 0000 0000  ................
+00000500: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
+00000510: 0000 2696 061c 150a 1935 1000 0619 1802  ..&......5......
+00000520: 7261 1502 1616 16d8 0216 a802 26f8 0426  ra..........&..&
+00000530: ee03 1c18 0800 0000 0000 c875 4018 0800  ...........u@...
+00000540: 0000 0000 8872 4016 0028 0800 0000 0000  .....r@..(......
+00000550: c875 4018 0800 0000 0000 8872 4000 192c  .u@........r@..,
+00000560: 1504 1500 1502 0015 0015 1015 0200 0000  ................
+00000570: 26f6 091c 150a 1935 1000 0619 1803 6465  &......5......de
+00000580: 6315 0216 1616 c802 16a4 0226 d808 26d2  c..........&..&.
+00000590: 071c 1808 0000 0000 0040 4ac0 1808 0000  .........@J.....
+000005a0: 0000 00e0 50c0 1600 2808 0000 0000 0040  ....P...(......@
+000005b0: 4ac0 1808 0000 0000 00e0 50c0 0019 2c15  J.........P...,.
+000005c0: 0415 0015 0200 1500 1510 1502 0000 0026  ...............&
+000005d0: f40c 1c15 0419 3510 0006 1918 0872 615f  ......5......ra_
+000005e0: 6572 726f 7215 0216 1616 b801 16c0 0126  error..........&
+000005f0: e40b 26b4 0b1c 1808 0000 0000 0000 0000  ..&.............
+00000600: 1808 0000 0000 0000 0000 1600 2808 0000  ............(...
+00000610: 0000 0000 0000 1808 0000 0000 0000 0000  ................
+00000620: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
+00000630: 0000 0026 fc0f 1c15 0419 3510 0006 1918  ...&......5.....
+00000640: 0964 6563 5f65 7272 6f72 1502 1616 16b8  .dec_error......
+00000650: 0116 c001 26ec 0e26 bc0e 1c18 0800 0000  ....&..&........
+00000660: 0000 0000 0018 0800 0000 0000 0000 0016  ................
+00000670: 0028 0800 0000 0000 0000 0018 0800 0000  .(..............
+00000680: 0000 0000 0000 192c 1504 1500 1502 0015  .......,........
+00000690: 0015 1015 0200 0000 16f8 0a16 1626 0816  .............&..
+000006a0: f809 1400 0019 2c18 0670 616e 6461 7318  ......,..pandas.
+000006b0: a705 7b22 696e 6465 785f 636f 6c75 6d6e  ..{"index_column
+000006c0: 7322 3a20 5b5d 2c20 2263 6f6c 756d 6e5f  s": [], "column_
+000006d0: 696e 6465 7865 7322 3a20 5b5d 2c20 2263  indexes": [], "c
+000006e0: 6f6c 756d 6e73 223a 205b 7b22 6e61 6d65  olumns": [{"name
+000006f0: 223a 2022 6964 222c 2022 6669 656c 645f  ": "id", "field_
+00000700: 6e61 6d65 223a 2022 6964 222c 2022 7061  name": "id", "pa
+00000710: 6e64 6173 5f74 7970 6522 3a20 2269 6e74  ndas_type": "int
+00000720: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
+00000730: 223a 2022 696e 7436 3422 2c20 226d 6574  ": "int64", "met
+00000740: 6164 6174 6122 3a20 6e75 6c6c 7d2c 207b  adata": null}, {
+00000750: 226e 616d 6522 3a20 2272 6122 2c20 2266  "name": "ra", "f
+00000760: 6965 6c64 5f6e 616d 6522 3a20 2272 6122  ield_name": "ra"
+00000770: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
+00000780: 2022 666c 6f61 7436 3422 2c20 226e 756d   "float64", "num
+00000790: 7079 5f74 7970 6522 3a20 2266 6c6f 6174  py_type": "float
+000007a0: 3634 222c 2022 6d65 7461 6461 7461 223a  64", "metadata":
+000007b0: 206e 756c 6c7d 2c20 7b22 6e61 6d65 223a   null}, {"name":
+000007c0: 2022 6465 6322 2c20 2266 6965 6c64 5f6e   "dec", "field_n
+000007d0: 616d 6522 3a20 2264 6563 222c 2022 7061  ame": "dec", "pa
+000007e0: 6e64 6173 5f74 7970 6522 3a20 2266 6c6f  ndas_type": "flo
+000007f0: 6174 3634 222c 2022 6e75 6d70 795f 7479  at64", "numpy_ty
+00000800: 7065 223a 2022 666c 6f61 7436 3422 2c20  pe": "float64", 
+00000810: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
+00000820: 7d2c 207b 226e 616d 6522 3a20 2272 615f  }, {"name": "ra_
+00000830: 6572 726f 7222 2c20 2266 6965 6c64 5f6e  error", "field_n
+00000840: 616d 6522 3a20 2272 615f 6572 726f 7222  ame": "ra_error"
+00000850: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
+00000860: 2022 696e 7436 3422 2c20 226e 756d 7079   "int64", "numpy
+00000870: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
+00000880: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
+00000890: 6c7d 2c20 7b22 6e61 6d65 223a 2022 6465  l}, {"name": "de
+000008a0: 635f 6572 726f 7222 2c20 2266 6965 6c64  c_error", "field
+000008b0: 5f6e 616d 6522 3a20 2264 6563 5f65 7272  _name": "dec_err
+000008c0: 6f72 222c 2022 7061 6e64 6173 5f74 7970  or", "pandas_typ
+000008d0: 6522 3a20 2269 6e74 3634 222c 2022 6e75  e": "int64", "nu
+000008e0: 6d70 795f 7479 7065 223a 2022 696e 7436  mpy_type": "int6
+000008f0: 3422 2c20 226d 6574 6164 6174 6122 3a20  4", "metadata": 
+00000900: 6e75 6c6c 7d5d 2c20 2263 7265 6174 6f72  null}], "creator
+00000910: 223a 207b 226c 6962 7261 7279 223a 2022  ": {"library": "
+00000920: 7079 6172 726f 7722 2c20 2276 6572 7369  pyarrow", "versi
+00000930: 6f6e 223a 2022 392e 302e 3022 7d2c 2022  on": "9.0.0"}, "
+00000940: 7061 6e64 6173 5f76 6572 7369 6f6e 223a  pandas_version":
+00000950: 2022 322e 302e 3022 7d00 180c 4152 524f   "2.0.0"}...ARRO
+00000960: 573a 7363 6865 6d61 1898 0b2f 2f2f 2f2f  W:schema.../////
+00000970: 7967 4541 4141 5141 4141 4141 4141 4b41  ygEAAAQAAAAAAAKA
+00000980: 4134 4142 6741 4641 4167 4143 6741 4141  A4ABgAFAAgACgAAA
+00000990: 4141 4242 4141 5141 4141 4141 4141 4b41  AABBAAQAAAAAAAKA
+000009a0: 4177 4141 4141 4541 4167 4143 6741 4141  AwAAAAEAAgACgAAA
+000009b0: 4e77 4341 4141 4541 4141 4141 5141 4141  NwCAAAEAAAAAQAAA
+000009c0: 4177 4141 4141 4941 4177 4142 4141 4941  AwAAAAIAAwABAAIA
+000009d0: 4167 4141 4141 4941 4141 4145 4141 4141  AgAAAAIAAAAEAAAA
+000009e0: 4159 4141 4142 7759 5735 6b59 584d 4141  AYAAABwYW5kYXMAA
+000009f0: 4b63 4341 4142 3749 6d6c 755a 4756 3458  KcCAAB7ImluZGV4X
+00000a00: 324e 7662 4856 7462 6e4d 694f 6942 6258  2NvbHVtbnMiOiBbX
+00000a10: 5377 6749 6d4e 7662 4856 7462 6c39 7062  SwgImNvbHVtbl9pb
+00000a20: 6d52 6c65 4756 7a49 6a6f 6757 3130 7349  mRleGVzIjogW10sI
+00000a30: 434a 6a62 3278 3162 5735 7a49 6a6f 6757  CJjb2x1bW5zIjogW
+00000a40: 3373 6962 6d46 745a 5349 3649 434a 705a  3sibmFtZSI6ICJpZ
+00000a50: 4349 7349 434a 6d61 5756 735a 4639 7559  CIsICJmaWVsZF9uY
+00000a60: 5731 6c49 6a6f 6749 6d6c 6b49 6977 6749  W1lIjogImlkIiwgI
+00000a70: 6e42 6862 6d52 6863 3139 3065 5842 6c49  nBhbmRhc190eXBlI
+00000a80: 6a6f 6749 6d6c 7564 4459 3049 6977 6749  jogImludDY0IiwgI
+00000a90: 6d35 3162 5842 3558 3352 3563 4755 694f  m51bXB5X3R5cGUiO
+00000aa0: 6941 6961 5735 304e 6a51 694c 4341 6962  iAiaW50NjQiLCAib
+00000ab0: 5756 3059 5752 6864 4745 694f 6942 7564  WV0YWRhdGEiOiBud
+00000ac0: 5778 7366 5377 6765 794a 7559 5731 6c49  WxsfSwgeyJuYW1lI
+00000ad0: 6a6f 6749 6e4a 6849 6977 6749 6d5a 705a  jogInJhIiwgImZpZ
+00000ae0: 5778 6b58 3235 6862 5755 694f 6941 6963  WxkX25hbWUiOiAic
+00000af0: 6d45 694c 4341 6963 4746 755a 4746 7a58  mEiLCAicGFuZGFzX
+00000b00: 3352 3563 4755 694f 6941 695a 6d78 7659  3R5cGUiOiAiZmxvY
+00000b10: 5851 324e 4349 7349 434a 7564 5731 7765  XQ2NCIsICJudW1we
+00000b20: 5639 3065 5842 6c49 6a6f 6749 6d5a 7362  V90eXBlIjogImZsb
+00000b30: 3246 304e 6a51 694c 4341 6962 5756 3059  2F0NjQiLCAibWV0Y
+00000b40: 5752 6864 4745 694f 6942 7564 5778 7366  WRhdGEiOiBudWxsf
+00000b50: 5377 6765 794a 7559 5731 6c49 6a6f 6749  SwgeyJuYW1lIjogI
+00000b60: 6d52 6c59 7949 7349 434a 6d61 5756 735a  mRlYyIsICJmaWVsZ
+00000b70: 4639 7559 5731 6c49 6a6f 6749 6d52 6c59  F9uYW1lIjogImRlY
+00000b80: 7949 7349 434a 7759 5735 6b59 584e 6664  yIsICJwYW5kYXNfd
+00000b90: 486c 775a 5349 3649 434a 6d62 4739 6864  HlwZSI6ICJmbG9hd
+00000ba0: 4459 3049 6977 6749 6d35 3162 5842 3558  DY0IiwgIm51bXB5X
+00000bb0: 3352 3563 4755 694f 6941 695a 6d78 7659  3R5cGUiOiAiZmxvY
+00000bc0: 5851 324e 4349 7349 434a 745a 5852 685a  XQ2NCIsICJtZXRhZ
+00000bd0: 4746 3059 5349 3649 4735 3162 4778 394c  GF0YSI6IG51bGx9L
+00000be0: 4342 3749 6d35 6862 5755 694f 6941 6963  CB7Im5hbWUiOiAic
+00000bf0: 6d46 665a 584a 7962 3349 694c 4341 695a  mFfZXJyb3IiLCAiZ
+00000c00: 6d6c 6c62 4752 6662 6d46 745a 5349 3649  mllbGRfbmFtZSI6I
+00000c10: 434a 7959 5639 6c63 6e4a 7663 6949 7349  CJyYV9lcnJvciIsI
+00000c20: 434a 7759 5735 6b59 584e 6664 486c 775a  CJwYW5kYXNfdHlwZ
+00000c30: 5349 3649 434a 7062 6e51 324e 4349 7349  SI6ICJpbnQ2NCIsI
+00000c40: 434a 7564 5731 7765 5639 3065 5842 6c49  CJudW1weV90eXBlI
+00000c50: 6a6f 6749 6d6c 7564 4459 3049 6977 6749  jogImludDY0IiwgI
+00000c60: 6d31 6c64 4746 6b59 5852 6849 6a6f 6762  m1ldGFkYXRhIjogb
+00000c70: 6e56 7362 4830 7349 4873 6962 6d46 745a  nVsbH0sIHsibmFtZ
+00000c80: 5349 3649 434a 6b5a 574e 665a 584a 7962  SI6ICJkZWNfZXJyb
+00000c90: 3349 694c 4341 695a 6d6c 6c62 4752 6662  3IiLCAiZmllbGRfb
+00000ca0: 6d46 745a 5349 3649 434a 6b5a 574e 665a  mFtZSI6ICJkZWNfZ
+00000cb0: 584a 7962 3349 694c 4341 6963 4746 755a  XJyb3IiLCAicGFuZ
+00000cc0: 4746 7a58 3352 3563 4755 694f 6941 6961  GFzX3R5cGUiOiAia
+00000cd0: 5735 304e 6a51 694c 4341 6962 6e56 7463  W50NjQiLCAibnVtc
+00000ce0: 486c 6664 486c 775a 5349 3649 434a 7062  HlfdHlwZSI6ICJpb
+00000cf0: 6e51 324e 4349 7349 434a 745a 5852 685a  nQ2NCIsICJtZXRhZ
+00000d00: 4746 3059 5349 3649 4735 3162 4778 3958  GF0YSI6IG51bGx9X
+00000d10: 5377 6749 6d4e 795a 5746 3062 3349 694f  SwgImNyZWF0b3IiO
+00000d20: 6942 3749 6d78 7059 6e4a 6863 6e6b 694f  iB7ImxpYnJhcnkiO
+00000d30: 6941 6963 486c 6863 6e4a 7664 7949 7349  iAicHlhcnJvdyIsI
+00000d40: 434a 325a 584a 7a61 5739 7549 6a6f 6749  CJ2ZXJzaW9uIjogI
+00000d50: 6a6b 754d 4334 7749 6e30 7349 434a 7759  jkuMC4wIn0sICJwY
+00000d60: 5735 6b59 584e 6664 6d56 7963 326c 7662  W5kYXNfdmVyc2lvb
+00000d70: 6949 3649 4349 794c 6a41 754d 434a 3941  iI6ICIyLjAuMCJ9A
+00000d80: 4155 4141 4144 6b41 4141 416f 4141 4141  AUAAADkAAAAoAAAA
+00000d90: 4851 4141 4141 3841 4141 4142 4141 4141  HQAAAA8AAAABAAAA
+00000da0: 4544 2f2f 2f38 4141 4145 4345 4141 4141  ED///8AAAECEAAAA
+00000db0: 4277 4141 4141 4541 4141 4141 4141 4141  BwAAAAEAAAAAAAAA
+00000dc0: 416b 4141 4142 6b5a 574e 665a 584a 7962  AkAAABkZWNfZXJyb
+00000dd0: 3349 4141 4141 342f 2f2f 2f41 4141 4141  3IAAAA4////AAAAA
+00000de0: 5541 4141 4142 302f 2f2f 2f41 4141 4241  UAAAAB0////AAABA
+00000df0: 6841 4141 4141 6341 4141 4142 4141 4141  hAAAAAcAAAABAAAA
+00000e00: 4141 4141 4141 4941 4141 4163 6d46 665a  AAAAAAIAAAAcmFfZ
+00000e10: 584a 7962 3349 4141 4141 4162 502f 2f2f  XJyb3IAAAAAbP///
+00000e20: 7741 4141 4146 4141 4141 4171 502f 2f2f  wAAAAFAAAAAqP///
+00000e30: 7741 4141 514d 5141 4141 4146 4141 4141  wAAAQMQAAAAFAAAA
+00000e40: 4151 4141 4141 4141 4141 4141 7741 4141  AQAAAAAAAAAAwAAA
+00000e50: 4752 6c59 7744 572f 2f2f 2f41 4141 4341  GRlYwDW////AAACA
+00000e60: 4e44 2f2f 2f38 4141 4145 4445 4141 4141  ND///8AAAEDEAAAA
+00000e70: 4277 4141 4141 4541 4141 4141 4141 4141  BwAAAAEAAAAAAAAA
+00000e80: 4149 4141 4142 7959 5141 4141 4141 4741  AIAAAByYQAAAAAGA
+00000e90: 4167 4142 6741 4741 4141 4141 4141 4341  AgABgAGAAAAAAACA
+00000ea0: 4241 4146 4141 4941 4159 4142 7741 4d41  BAAFAAIAAYABwAMA
+00000eb0: 4141 4145 4141 5141 4141 4141 4141 4241  AAAEAAQAAAAAAABA
+00000ec0: 6841 4141 4141 6341 4141 4142 4141 4141  hAAAAAcAAAABAAAA
+00000ed0: 4141 4141 4141 4341 4141 4161 5751 4141  AAAAAACAAAAaWQAA
+00000ee0: 4167 4144 4141 4941 4163 4143 4141 4141  AgADAAIAAcACAAAA
+00000ef0: 4141 4141 4146 4141 4141 4141 4141 4141  AAAAAFAAAAAAAAAA
+00000f00: 413d 3d00 181f 7061 7271 7565 742d 6370  A==...parquet-cp
+00000f10: 702d 6172 726f 7720 7665 7273 696f 6e20  p-arrow version 
+00000f20: 392e 302e 3019 5c1c 0000 1c00 001c 0000  9.0.0.\.........
+00000f30: 1c00 001c 0000 00d4 0a00 0050 4152 31    ...........PAR1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_44/shard_4.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet`

 * *Files 16% similar despite different names*

```diff
@@ -64,249 +64,182 @@
 000003f0: 0000 0000 0009 2002 0000 0016 0101 1600  ...... .........
 00000400: 2680 101c 1504 1935 1000 0619 1809 6465  &......5......de
 00000410: 635f 6572 726f 7215 0216 1616 b801 16c0  c_error.........
 00000420: 0126 f00e 26c0 0e1c 1808 0000 0000 0000  .&..&...........
 00000430: 0000 1808 0000 0000 0000 0000 1600 2808  ..............(.
 00000440: 0000 0000 0000 0000 1808 0000 0000 0000  ................
 00000450: 0000 0019 2c15 0415 0015 0200 1500 1510  ....,...........
-00000460: 1502 0000 0015 0415 b001 1570 4c15 1615  ...........pL...
-00000470: 0012 0000 5804 0100 0901 0004 0907 0400  ....X...........
-00000480: 070d 0800 080d 0800 0c0d 0800 0d0d 0800  ................
-00000490: 0e0d 0800 0f0d 0800 130d 083c 1700 0000  ...........<....
-000004a0: 0000 0000 1b00 0000 0000 0000 1500 1520  ............... 
-000004b0: 1524 2c15 1615 1015 0615 061c 1808 1b00  .$,.............
-000004c0: 0000 0000 0000 1808 0100 0000 0000 0000  ................
-000004d0: 1600 2808 1b00 0000 0000 0000 1808 0100  ..(.............
-000004e0: 0000 0000 0000 0000 0010 3c02 0000 0016  ..........<.....
-000004f0: 0104 0510 3254 7698 0a00 0026 f613 1c15  ....2Tv....&....
-00000500: 0419 3510 0006 1918 115f 5f69 6e64 6578  ..5......__index
-00000510: 5f6c 6576 656c 5f30 5f5f 1502 1616 16e8  _level_0__......
-00000520: 0216 ac02 26d8 1226 ca11 1c18 081b 0000  ....&..&........
-00000530: 0000 0000 0018 0801 0000 0000 0000 0016  ................
-00000540: 0028 081b 0000 0000 0000 0018 0801 0000  .(..............
-00000550: 0000 0000 0000 192c 1504 1500 1502 0015  .......,........
-00000560: 0015 1015 0200 0000 1504 197c 3500 1806  ...........|5...
-00000570: 7363 6865 6d61 150c 0015 0425 0218 0269  schema.....%...i
-00000580: 6400 150a 2502 1802 7261 0015 0a25 0218  d...%...ra...%..
-00000590: 0364 6563 0015 0425 0218 0872 615f 6572  .dec...%...ra_er
-000005a0: 726f 7200 1504 2502 1809 6465 635f 6572  ror...%...dec_er
-000005b0: 726f 7200 1504 2502 1811 5f5f 696e 6465  ror...%...__inde
-000005c0: 785f 6c65 7665 6c5f 305f 5f00 1616 191c  x_level_0__.....
-000005d0: 196c 26b4 021c 1504 1935 1000 0619 1802  .l&......5......
-000005e0: 6964 1502 1616 16e8 0216 ac02 2696 0126  id..........&..&
-000005f0: 081c 1808 3e03 0000 0000 0000 1808 2403  ....>.........$.
-00000600: 0000 0000 0000 1600 2808 3e03 0000 0000  ........(.>.....
-00000610: 0000 1808 2403 0000 0000 0000 0019 2c15  ....$.........,.
-00000620: 0415 0015 0200 1500 1510 1502 0000 0026  ...............&
-00000630: 9806 1c15 0a19 3510 0006 1918 0272 6115  ......5......ra.
-00000640: 0216 1616 d802 16aa 0226 fa04 26ee 031c  .........&..&...
-00000650: 1808 0000 0000 00f8 7440 1808 0000 0000  ........t@......
-00000660: 00b8 7140 1600 2808 0000 0000 00f8 7440  ..q@..(.......t@
-00000670: 1808 0000 0000 00b8 7140 0019 2c15 0415  ........q@..,...
-00000680: 0015 0200 1500 1510 1502 0000 0026 fa09  .............&..
-00000690: 1c15 0a19 3510 0006 1918 0364 6563 1502  ....5......dec..
-000006a0: 1616 16c8 0216 a602 26dc 0826 d407 1c18  ........&..&....
-000006b0: 0800 0000 0000 4048 c018 0800 0000 0000  ......@H........
-000006c0: 6051 c016 0028 0800 0000 0000 4048 c018  `Q...(......@H..
-000006d0: 0800 0000 0000 6051 c000 192c 1504 1500  ......`Q...,....
-000006e0: 1502 0015 0015 1015 0200 0000 26f8 0c1c  ............&...
-000006f0: 1504 1935 1000 0619 1808 7261 5f65 7272  ...5......ra_err
-00000700: 6f72 1502 1616 16b8 0116 c001 26e8 0b26  or..........&..&
-00000710: b80b 1c18 0800 0000 0000 0000 0018 0800  ................
-00000720: 0000 0000 0000 0016 0028 0800 0000 0000  .........(......
-00000730: 0000 0018 0800 0000 0000 0000 0000 192c  ...............,
-00000740: 1504 1500 1502 0015 0015 1015 0200 0000  ................
-00000750: 2680 101c 1504 1935 1000 0619 1809 6465  &......5......de
-00000760: 635f 6572 726f 7215 0216 1616 b801 16c0  c_error.........
-00000770: 0126 f00e 26c0 0e1c 1808 0000 0000 0000  .&..&...........
-00000780: 0000 1808 0000 0000 0000 0000 1600 2808  ..............(.
-00000790: 0000 0000 0000 0000 1808 0000 0000 0000  ................
-000007a0: 0000 0019 2c15 0415 0015 0200 1500 1510  ....,...........
-000007b0: 1502 0000 0026 f613 1c15 0419 3510 0006  .....&......5...
-000007c0: 1918 115f 5f69 6e64 6578 5f6c 6576 656c  ...__index_level
-000007d0: 5f30 5f5f 1502 1616 16e8 0216 ac02 26d8  _0__..........&.
-000007e0: 1226 ca11 1c18 081b 0000 0000 0000 0018  .&..............
-000007f0: 0801 0000 0000 0000 0016 0028 081b 0000  ...........(....
-00000800: 0000 0000 0018 0801 0000 0000 0000 0000  ................
-00000810: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
-00000820: 0000 16e0 0d16 1626 0816 a80c 1400 0019  .......&........
-00000830: 2c18 0670 616e 6461 7318 a507 7b22 696e  ,..pandas...{"in
-00000840: 6465 785f 636f 6c75 6d6e 7322 3a20 5b22  dex_columns": ["
-00000850: 5f5f 696e 6465 785f 6c65 7665 6c5f 305f  __index_level_0_
-00000860: 5f22 5d2c 2022 636f 6c75 6d6e 5f69 6e64  _"], "column_ind
-00000870: 6578 6573 223a 205b 7b22 6e61 6d65 223a  exes": [{"name":
-00000880: 206e 756c 6c2c 2022 6669 656c 645f 6e61   null, "field_na
-00000890: 6d65 223a 206e 756c 6c2c 2022 7061 6e64  me": null, "pand
-000008a0: 6173 5f74 7970 6522 3a20 2275 6e69 636f  as_type": "unico
-000008b0: 6465 222c 2022 6e75 6d70 795f 7479 7065  de", "numpy_type
-000008c0: 223a 2022 6f62 6a65 6374 222c 2022 6d65  ": "object", "me
-000008d0: 7461 6461 7461 223a 207b 2265 6e63 6f64  tadata": {"encod
-000008e0: 696e 6722 3a20 2255 5446 2d38 227d 7d5d  ing": "UTF-8"}}]
-000008f0: 2c20 2263 6f6c 756d 6e73 223a 205b 7b22  , "columns": [{"
-00000900: 6e61 6d65 223a 2022 6964 222c 2022 6669  name": "id", "fi
-00000910: 656c 645f 6e61 6d65 223a 2022 6964 222c  eld_name": "id",
-00000920: 2022 7061 6e64 6173 5f74 7970 6522 3a20   "pandas_type": 
-00000930: 2269 6e74 3634 222c 2022 6e75 6d70 795f  "int64", "numpy_
-00000940: 7479 7065 223a 2022 696e 7436 3422 2c20  type": "int64", 
-00000950: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
-00000960: 7d2c 207b 226e 616d 6522 3a20 2272 6122  }, {"name": "ra"
-00000970: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
-00000980: 2272 6122 2c20 2270 616e 6461 735f 7479  "ra", "pandas_ty
-00000990: 7065 223a 2022 666c 6f61 7436 3422 2c20  pe": "float64", 
-000009a0: 226e 756d 7079 5f74 7970 6522 3a20 2266  "numpy_type": "f
-000009b0: 6c6f 6174 3634 222c 2022 6d65 7461 6461  loat64", "metada
-000009c0: 7461 223a 206e 756c 6c7d 2c20 7b22 6e61  ta": null}, {"na
-000009d0: 6d65 223a 2022 6465 6322 2c20 2266 6965  me": "dec", "fie
-000009e0: 6c64 5f6e 616d 6522 3a20 2264 6563 222c  ld_name": "dec",
-000009f0: 2022 7061 6e64 6173 5f74 7970 6522 3a20   "pandas_type": 
-00000a00: 2266 6c6f 6174 3634 222c 2022 6e75 6d70  "float64", "nump
-00000a10: 795f 7479 7065 223a 2022 666c 6f61 7436  y_type": "float6
-00000a20: 3422 2c20 226d 6574 6164 6174 6122 3a20  4", "metadata": 
-00000a30: 6e75 6c6c 7d2c 207b 226e 616d 6522 3a20  null}, {"name": 
-00000a40: 2272 615f 6572 726f 7222 2c20 2266 6965  "ra_error", "fie
-00000a50: 6c64 5f6e 616d 6522 3a20 2272 615f 6572  ld_name": "ra_er
-00000a60: 726f 7222 2c20 2270 616e 6461 735f 7479  ror", "pandas_ty
-00000a70: 7065 223a 2022 696e 7436 3422 2c20 226e  pe": "int64", "n
-00000a80: 756d 7079 5f74 7970 6522 3a20 2269 6e74  umpy_type": "int
-00000a90: 3634 222c 2022 6d65 7461 6461 7461 223a  64", "metadata":
-00000aa0: 206e 756c 6c7d 2c20 7b22 6e61 6d65 223a   null}, {"name":
-00000ab0: 2022 6465 635f 6572 726f 7222 2c20 2266   "dec_error", "f
-00000ac0: 6965 6c64 5f6e 616d 6522 3a20 2264 6563  ield_name": "dec
-00000ad0: 5f65 7272 6f72 222c 2022 7061 6e64 6173  _error", "pandas
-00000ae0: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
-00000af0: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
-00000b00: 696e 7436 3422 2c20 226d 6574 6164 6174  int64", "metadat
-00000b10: 6122 3a20 6e75 6c6c 7d2c 207b 226e 616d  a": null}, {"nam
-00000b20: 6522 3a20 6e75 6c6c 2c20 2266 6965 6c64  e": null, "field
-00000b30: 5f6e 616d 6522 3a20 225f 5f69 6e64 6578  _name": "__index
-00000b40: 5f6c 6576 656c 5f30 5f5f 222c 2022 7061  _level_0__", "pa
-00000b50: 6e64 6173 5f74 7970 6522 3a20 2269 6e74  ndas_type": "int
-00000b60: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
-00000b70: 223a 2022 696e 7436 3422 2c20 226d 6574  ": "int64", "met
-00000b80: 6164 6174 6122 3a20 6e75 6c6c 7d5d 2c20  adata": null}], 
-00000b90: 2263 7265 6174 6f72 223a 207b 226c 6962  "creator": {"lib
-00000ba0: 7261 7279 223a 2022 7079 6172 726f 7722  rary": "pyarrow"
-00000bb0: 2c20 2276 6572 7369 6f6e 223a 2022 392e  , "version": "9.
-00000bc0: 302e 3022 7d2c 2022 7061 6e64 6173 5f76  0.0"}, "pandas_v
-00000bd0: 6572 7369 6f6e 223a 2022 312e 332e 3522  ersion": "1.3.5"
-00000be0: 7d00 180c 4152 524f 573a 7363 6865 6d61  }...ARROW:schema
-00000bf0: 18c0 0e2f 2f2f 2f2f 3267 4641 4141 5141  .../////2gFAAAQA
-00000c00: 4141 4141 4141 4b41 4134 4142 6741 4641  AAAAAAKAA4ABgAFA
-00000c10: 4167 4143 6741 4141 4141 4242 4141 5141  AgACgAAAAABBAAQA
-00000c20: 4141 4141 4141 4b41 4177 4141 4141 4541  AAAAAAKAAwAAAAEA
-00000c30: 4167 4143 6741 4141 4e77 4441 4141 4541  AgACgAAANwDAAAEA
-00000c40: 4141 4141 5141 4141 4177 4141 4141 4941  AAAAQAAAAwAAAAIA
-00000c50: 4177 4142 4141 4941 4167 4141 4141 4941  AwABAAIAAgAAAAIA
-00000c60: 4141 4145 4141 4141 4159 4141 4142 7759  AAAEAAAAAYAAABwY
-00000c70: 5735 6b59 584d 4141 4b55 4441 4142 3749  W5kYXMAAKUDAAB7I
-00000c80: 6d6c 755a 4756 3458 324e 7662 4856 7462  mluZGV4X2NvbHVtb
-00000c90: 6e4d 694f 6942 6249 6c39 6661 5735 6b5a  nMiOiBbIl9faW5kZ
-00000ca0: 5868 6662 4756 325a 5778 664d 4639 6649  XhfbGV2ZWxfMF9fI
-00000cb0: 6c30 7349 434a 6a62 3278 3162 5735 6661  l0sICJjb2x1bW5fa
-00000cc0: 5735 6b5a 5868 6c63 7949 3649 4674 3749  W5kZXhlcyI6IFt7I
-00000cd0: 6d35 6862 5755 694f 6942 7564 5778 734c  m5hbWUiOiBudWxsL
-00000ce0: 4341 695a 6d6c 6c62 4752 6662 6d46 745a  CAiZmllbGRfbmFtZ
-00000cf0: 5349 3649 4735 3162 4777 7349 434a 7759  SI6IG51bGwsICJwY
-00000d00: 5735 6b59 584e 6664 486c 775a 5349 3649  W5kYXNfdHlwZSI6I
-00000d10: 434a 3162 6d6c 6a62 3252 6c49 6977 6749  CJ1bmljb2RlIiwgI
-00000d20: 6d35 3162 5842 3558 3352 3563 4755 694f  m51bXB5X3R5cGUiO
-00000d30: 6941 6962 324a 715a 574e 3049 6977 6749  iAib2JqZWN0IiwgI
-00000d40: 6d31 6c64 4746 6b59 5852 6849 6a6f 6765  m1ldGFkYXRhIjoge
-00000d50: 794a 6c62 6d4e 765a 476c 755a 7949 3649  yJlbmNvZGluZyI6I
-00000d60: 434a 5656 4559 744f 434a 3966 5630 7349  CJVVEYtOCJ9fV0sI
-00000d70: 434a 6a62 3278 3162 5735 7a49 6a6f 6757  CJjb2x1bW5zIjogW
-00000d80: 3373 6962 6d46 745a 5349 3649 434a 705a  3sibmFtZSI6ICJpZ
-00000d90: 4349 7349 434a 6d61 5756 735a 4639 7559  CIsICJmaWVsZF9uY
-00000da0: 5731 6c49 6a6f 6749 6d6c 6b49 6977 6749  W1lIjogImlkIiwgI
-00000db0: 6e42 6862 6d52 6863 3139 3065 5842 6c49  nBhbmRhc190eXBlI
-00000dc0: 6a6f 6749 6d6c 7564 4459 3049 6977 6749  jogImludDY0IiwgI
-00000dd0: 6d35 3162 5842 3558 3352 3563 4755 694f  m51bXB5X3R5cGUiO
-00000de0: 6941 6961 5735 304e 6a51 694c 4341 6962  iAiaW50NjQiLCAib
-00000df0: 5756 3059 5752 6864 4745 694f 6942 7564  WV0YWRhdGEiOiBud
-00000e00: 5778 7366 5377 6765 794a 7559 5731 6c49  WxsfSwgeyJuYW1lI
-00000e10: 6a6f 6749 6e4a 6849 6977 6749 6d5a 705a  jogInJhIiwgImZpZ
-00000e20: 5778 6b58 3235 6862 5755 694f 6941 6963  WxkX25hbWUiOiAic
-00000e30: 6d45 694c 4341 6963 4746 755a 4746 7a58  mEiLCAicGFuZGFzX
-00000e40: 3352 3563 4755 694f 6941 695a 6d78 7659  3R5cGUiOiAiZmxvY
-00000e50: 5851 324e 4349 7349 434a 7564 5731 7765  XQ2NCIsICJudW1we
-00000e60: 5639 3065 5842 6c49 6a6f 6749 6d5a 7362  V90eXBlIjogImZsb
-00000e70: 3246 304e 6a51 694c 4341 6962 5756 3059  2F0NjQiLCAibWV0Y
-00000e80: 5752 6864 4745 694f 6942 7564 5778 7366  WRhdGEiOiBudWxsf
-00000e90: 5377 6765 794a 7559 5731 6c49 6a6f 6749  SwgeyJuYW1lIjogI
-00000ea0: 6d52 6c59 7949 7349 434a 6d61 5756 735a  mRlYyIsICJmaWVsZ
-00000eb0: 4639 7559 5731 6c49 6a6f 6749 6d52 6c59  F9uYW1lIjogImRlY
-00000ec0: 7949 7349 434a 7759 5735 6b59 584e 6664  yIsICJwYW5kYXNfd
-00000ed0: 486c 775a 5349 3649 434a 6d62 4739 6864  HlwZSI6ICJmbG9hd
-00000ee0: 4459 3049 6977 6749 6d35 3162 5842 3558  DY0IiwgIm51bXB5X
-00000ef0: 3352 3563 4755 694f 6941 695a 6d78 7659  3R5cGUiOiAiZmxvY
-00000f00: 5851 324e 4349 7349 434a 745a 5852 685a  XQ2NCIsICJtZXRhZ
-00000f10: 4746 3059 5349 3649 4735 3162 4778 394c  GF0YSI6IG51bGx9L
-00000f20: 4342 3749 6d35 6862 5755 694f 6941 6963  CB7Im5hbWUiOiAic
-00000f30: 6d46 665a 584a 7962 3349 694c 4341 695a  mFfZXJyb3IiLCAiZ
-00000f40: 6d6c 6c62 4752 6662 6d46 745a 5349 3649  mllbGRfbmFtZSI6I
-00000f50: 434a 7959 5639 6c63 6e4a 7663 6949 7349  CJyYV9lcnJvciIsI
-00000f60: 434a 7759 5735 6b59 584e 6664 486c 775a  CJwYW5kYXNfdHlwZ
-00000f70: 5349 3649 434a 7062 6e51 324e 4349 7349  SI6ICJpbnQ2NCIsI
-00000f80: 434a 7564 5731 7765 5639 3065 5842 6c49  CJudW1weV90eXBlI
-00000f90: 6a6f 6749 6d6c 7564 4459 3049 6977 6749  jogImludDY0IiwgI
-00000fa0: 6d31 6c64 4746 6b59 5852 6849 6a6f 6762  m1ldGFkYXRhIjogb
-00000fb0: 6e56 7362 4830 7349 4873 6962 6d46 745a  nVsbH0sIHsibmFtZ
-00000fc0: 5349 3649 434a 6b5a 574e 665a 584a 7962  SI6ICJkZWNfZXJyb
-00000fd0: 3349 694c 4341 695a 6d6c 6c62 4752 6662  3IiLCAiZmllbGRfb
-00000fe0: 6d46 745a 5349 3649 434a 6b5a 574e 665a  mFtZSI6ICJkZWNfZ
-00000ff0: 584a 7962 3349 694c 4341 6963 4746 755a  XJyb3IiLCAicGFuZ
-00001000: 4746 7a58 3352 3563 4755 694f 6941 6961  GFzX3R5cGUiOiAia
-00001010: 5735 304e 6a51 694c 4341 6962 6e56 7463  W50NjQiLCAibnVtc
-00001020: 486c 6664 486c 775a 5349 3649 434a 7062  HlfdHlwZSI6ICJpb
-00001030: 6e51 324e 4349 7349 434a 745a 5852 685a  nQ2NCIsICJtZXRhZ
-00001040: 4746 3059 5349 3649 4735 3162 4778 394c  GF0YSI6IG51bGx9L
-00001050: 4342 3749 6d35 6862 5755 694f 6942 7564  CB7Im5hbWUiOiBud
-00001060: 5778 734c 4341 695a 6d6c 6c62 4752 6662  WxsLCAiZmllbGRfb
-00001070: 6d46 745a 5349 3649 434a 6658 326c 755a  mFtZSI6ICJfX2luZ
-00001080: 4756 3458 3278 6c64 6d56 7358 7a42 6658  GV4X2xldmVsXzBfX
-00001090: 7949 7349 434a 7759 5735 6b59 584e 6664  yIsICJwYW5kYXNfd
-000010a0: 486c 775a 5349 3649 434a 7062 6e51 324e  HlwZSI6ICJpbnQ2N
-000010b0: 4349 7349 434a 7564 5731 7765 5639 3065  CIsICJudW1weV90e
-000010c0: 5842 6c49 6a6f 6749 6d6c 7564 4459 3049  XBlIjogImludDY0I
-000010d0: 6977 6749 6d31 6c64 4746 6b59 5852 6849  iwgIm1ldGFkYXRhI
-000010e0: 6a6f 6762 6e56 7362 4831 644c 4341 6959  jogbnVsbH1dLCAiY
-000010f0: 334a 6c59 5852 7663 6949 3649 4873 6962  3JlYXRvciI6IHsib
-00001100: 476c 6963 6d46 7965 5349 3649 434a 7765  GlicmFyeSI6ICJwe
-00001110: 5746 7963 6d39 3349 6977 6749 6e5a 6c63  WFycm93IiwgInZlc
-00001120: 6e4e 7062 3234 694f 6941 694f 5334 774c  nNpb24iOiAiOS4wL
-00001130: 6a41 6966 5377 6749 6e42 6862 6d52 6863  jAifSwgInBhbmRhc
-00001140: 3139 325a 584a 7a61 5739 7549 6a6f 6749  192ZXJzaW9uIjogI
-00001150: 6a45 754d 7934 3149 6e30 4141 4141 4741  jEuMy41In0AAAAGA
-00001160: 4141 414a 4145 4141 4f41 4141 4143 3041  AAAJAEAAOAAAAC0A
-00001170: 4141 4166 4141 4141 4551 4141 4141 4541  AAAfAAAAEQAAAAEA
-00001180: 4141 4142 502f 2f2f 7741 4141 5149 5141  AAABP///wAAAQIQA
-00001190: 4141 414a 4141 4141 4151 4141 4141 4141  AAAJAAAAAQAAAAAA
-000011a0: 4141 4145 5141 4141 4639 6661 5735 6b5a  AAAEQAAAF9faW5kZ
-000011b0: 5868 6662 4756 325a 5778 664d 4639 6641  XhfbGV2ZWxfMF9fA
-000011c0: 4141 4142 502f 2f2f 7741 4141 4146 4141  AAABP///wAAAAFAA
-000011d0: 4141 4151 502f 2f2f 7741 4141 5149 5141  AAAQP///wAAAQIQA
-000011e0: 4141 4148 4141 4141 4151 4141 4141 4141  AAAHAAAAAQAAAAAA
-000011f0: 4141 4143 5141 4141 4752 6c59 3139 6c63  AAACQAAAGRlY19lc
-00001200: 6e4a 7663 6741 4141 446a 2f2f 2f38 4141  nJvcgAAADj///8AA
-00001210: 4141 4251 4141 4141 4854 2f2f 2f38 4141  AABQAAAAHT///8AA
-00001220: 4145 4345 4141 4141 4277 4141 4141 4541  AECEAAAABwAAAAEA
-00001230: 4141 4141 4141 4141 4167 4141 4142 7959  AAAAAAAAAgAAAByY
-00001240: 5639 6c63 6e4a 7663 6741 4141 4142 732f  V9lcnJvcgAAAABs/
-00001250: 2f2f 2f41 4141 4141 5541 4141 4143 6f2f  ///AAAAAUAAAACo/
-00001260: 2f2f 2f41 4141 4241 7841 4141 4141 5541  ///AAABAxAAAAAUA
-00001270: 4141 4142 4141 4141 4141 4141 4141 4441  AAABAAAAAAAAAADA
-00001280: 4141 415a 4756 6a41 4e62 2f2f 2f38 4141  AAAZGVjANb///8AA
-00001290: 4149 4130 502f 2f2f 7741 4141 514d 5141  AIA0P///wAAAQMQA
-000012a0: 4141 4148 4141 4141 4151 4141 4141 4141  AAAHAAAAAQAAAAAA
-000012b0: 4141 4141 6741 4141 484a 6841 4141 4141  AAAAgAAAHJhAAAAA
-000012c0: 4159 4143 4141 4741 4159 4141 4141 4141  AYACAAGAAYAAAAAA
-000012d0: 4149 4145 4141 5541 4167 4142 6741 4841  AIAEAAUAAgABgAHA
-000012e0: 4177 4141 4141 5141 4241 4141 4141 4141  AwAAAAQABAAAAAAA
-000012f0: 4145 4345 4141 4141 4277 4141 4141 4541  AECEAAAABwAAAAEA
-00001300: 4141 4141 4141 4141 4149 4141 4142 705a  AAAAAAAAAIAAABpZ
-00001310: 4141 4143 4141 4d41 4167 4142 7741 4941  AAACAAMAAgABwAIA
-00001320: 4141 4141 4141 4141 5541 4141 4141 4141  AAAAAAAAUAAAAAAA
-00001330: 4141 4100 181f 7061 7271 7565 742d 6370  AAA...parquet-cp
-00001340: 702d 6172 726f 7720 7665 7273 696f 6e20  p-arrow version 
-00001350: 392e 302e 3019 6c1c 0000 1c00 001c 0000  9.0.0.l.........
-00001360: 1c00 001c 0000 1c00 0000 020e 0000 5041  ..............PA
-00001370: 5231                                     R1
+00000460: 1502 0000 0015 0419 6c35 0018 0673 6368  ........l5...sch
+00000470: 656d 6115 0a00 1504 2502 1802 6964 0015  ema.....%...id..
+00000480: 0a25 0218 0272 6100 150a 2502 1803 6465  .%...ra...%...de
+00000490: 6300 1504 2502 1808 7261 5f65 7272 6f72  c...%...ra_error
+000004a0: 0015 0425 0218 0964 6563 5f65 7272 6f72  ...%...dec_error
+000004b0: 0016 1619 1c19 5c26 b402 1c15 0419 3510  ......\&......5.
+000004c0: 0006 1918 0269 6415 0216 1616 e802 16ac  .....id.........
+000004d0: 0226 9601 2608 1c18 083e 0300 0000 0000  .&..&....>......
+000004e0: 0018 0824 0300 0000 0000 0016 0028 083e  ...$.........(.>
+000004f0: 0300 0000 0000 0018 0824 0300 0000 0000  .........$......
+00000500: 0000 192c 1504 1500 1502 0015 0015 1015  ...,............
+00000510: 0200 0000 2698 061c 150a 1935 1000 0619  ....&......5....
+00000520: 1802 7261 1502 1616 16d8 0216 aa02 26fa  ..ra..........&.
+00000530: 0426 ee03 1c18 0800 0000 0000 f874 4018  .&...........t@.
+00000540: 0800 0000 0000 b871 4016 0028 0800 0000  .......q@..(....
+00000550: 0000 f874 4018 0800 0000 0000 b871 4000  ...t@........q@.
+00000560: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
+00000570: 0000 26fa 091c 150a 1935 1000 0619 1803  ..&......5......
+00000580: 6465 6315 0216 1616 c802 16a6 0226 dc08  dec..........&..
+00000590: 26d4 071c 1808 0000 0000 0040 48c0 1808  &..........@H...
+000005a0: 0000 0000 0060 51c0 1600 2808 0000 0000  .....`Q...(.....
+000005b0: 0040 48c0 1808 0000 0000 0060 51c0 0019  .@H........`Q...
+000005c0: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
+000005d0: 0026 f80c 1c15 0419 3510 0006 1918 0872  .&......5......r
+000005e0: 615f 6572 726f 7215 0216 1616 b801 16c0  a_error.........
+000005f0: 0126 e80b 26b8 0b1c 1808 0000 0000 0000  .&..&...........
+00000600: 0000 1808 0000 0000 0000 0000 1600 2808  ..............(.
+00000610: 0000 0000 0000 0000 1808 0000 0000 0000  ................
+00000620: 0000 0019 2c15 0415 0015 0200 1500 1510  ....,...........
+00000630: 1502 0000 0026 8010 1c15 0419 3510 0006  .....&......5...
+00000640: 1918 0964 6563 5f65 7272 6f72 1502 1616  ...dec_error....
+00000650: 16b8 0116 c001 26f0 0e26 c00e 1c18 0800  ......&..&......
+00000660: 0000 0000 0000 0018 0800 0000 0000 0000  ................
+00000670: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
+00000680: 0000 0000 0000 0000 192c 1504 1500 1502  .........,......
+00000690: 0015 0015 1015 0200 0000 16f8 0a16 1626  ...............&
+000006a0: 0816 fc09 1400 0019 2c18 0670 616e 6461  ........,..panda
+000006b0: 7318 a705 7b22 696e 6465 785f 636f 6c75  s...{"index_colu
+000006c0: 6d6e 7322 3a20 5b5d 2c20 2263 6f6c 756d  mns": [], "colum
+000006d0: 6e5f 696e 6465 7865 7322 3a20 5b5d 2c20  n_indexes": [], 
+000006e0: 2263 6f6c 756d 6e73 223a 205b 7b22 6e61  "columns": [{"na
+000006f0: 6d65 223a 2022 6964 222c 2022 6669 656c  me": "id", "fiel
+00000700: 645f 6e61 6d65 223a 2022 6964 222c 2022  d_name": "id", "
+00000710: 7061 6e64 6173 5f74 7970 6522 3a20 2269  pandas_type": "i
+00000720: 6e74 3634 222c 2022 6e75 6d70 795f 7479  nt64", "numpy_ty
+00000730: 7065 223a 2022 696e 7436 3422 2c20 226d  pe": "int64", "m
+00000740: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
+00000750: 207b 226e 616d 6522 3a20 2272 6122 2c20   {"name": "ra", 
+00000760: 2266 6965 6c64 5f6e 616d 6522 3a20 2272  "field_name": "r
+00000770: 6122 2c20 2270 616e 6461 735f 7479 7065  a", "pandas_type
+00000780: 223a 2022 666c 6f61 7436 3422 2c20 226e  ": "float64", "n
+00000790: 756d 7079 5f74 7970 6522 3a20 2266 6c6f  umpy_type": "flo
+000007a0: 6174 3634 222c 2022 6d65 7461 6461 7461  at64", "metadata
+000007b0: 223a 206e 756c 6c7d 2c20 7b22 6e61 6d65  ": null}, {"name
+000007c0: 223a 2022 6465 6322 2c20 2266 6965 6c64  ": "dec", "field
+000007d0: 5f6e 616d 6522 3a20 2264 6563 222c 2022  _name": "dec", "
+000007e0: 7061 6e64 6173 5f74 7970 6522 3a20 2266  pandas_type": "f
+000007f0: 6c6f 6174 3634 222c 2022 6e75 6d70 795f  loat64", "numpy_
+00000800: 7479 7065 223a 2022 666c 6f61 7436 3422  type": "float64"
+00000810: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
+00000820: 6c6c 7d2c 207b 226e 616d 6522 3a20 2272  ll}, {"name": "r
+00000830: 615f 6572 726f 7222 2c20 2266 6965 6c64  a_error", "field
+00000840: 5f6e 616d 6522 3a20 2272 615f 6572 726f  _name": "ra_erro
+00000850: 7222 2c20 2270 616e 6461 735f 7479 7065  r", "pandas_type
+00000860: 223a 2022 696e 7436 3422 2c20 226e 756d  ": "int64", "num
+00000870: 7079 5f74 7970 6522 3a20 2269 6e74 3634  py_type": "int64
+00000880: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
+00000890: 756c 6c7d 2c20 7b22 6e61 6d65 223a 2022  ull}, {"name": "
+000008a0: 6465 635f 6572 726f 7222 2c20 2266 6965  dec_error", "fie
+000008b0: 6c64 5f6e 616d 6522 3a20 2264 6563 5f65  ld_name": "dec_e
+000008c0: 7272 6f72 222c 2022 7061 6e64 6173 5f74  rror", "pandas_t
+000008d0: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
+000008e0: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
+000008f0: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
+00000900: 3a20 6e75 6c6c 7d5d 2c20 2263 7265 6174  : null}], "creat
+00000910: 6f72 223a 207b 226c 6962 7261 7279 223a  or": {"library":
+00000920: 2022 7079 6172 726f 7722 2c20 2276 6572   "pyarrow", "ver
+00000930: 7369 6f6e 223a 2022 392e 302e 3022 7d2c  sion": "9.0.0"},
+00000940: 2022 7061 6e64 6173 5f76 6572 7369 6f6e   "pandas_version
+00000950: 223a 2022 322e 302e 3022 7d00 180c 4152  ": "2.0.0"}...AR
+00000960: 524f 573a 7363 6865 6d61 1898 0b2f 2f2f  ROW:schema...///
+00000970: 2f2f 7967 4541 4141 5141 4141 4141 4141  //ygEAAAQAAAAAAA
+00000980: 4b41 4134 4142 6741 4641 4167 4143 6741  KAA4ABgAFAAgACgA
+00000990: 4141 4141 4242 4141 5141 4141 4141 4141  AAAABBAAQAAAAAAA
+000009a0: 4b41 4177 4141 4141 4541 4167 4143 6741  KAAwAAAAEAAgACgA
+000009b0: 4141 4e77 4341 4141 4541 4141 4141 5141  AANwCAAAEAAAAAQA
+000009c0: 4141 4177 4141 4141 4941 4177 4142 4141  AAAwAAAAIAAwABAA
+000009d0: 4941 4167 4141 4141 4941 4141 4145 4141  IAAgAAAAIAAAAEAA
+000009e0: 4141 4159 4141 4142 7759 5735 6b59 584d  AAAYAAABwYW5kYXM
+000009f0: 4141 4b63 4341 4142 3749 6d6c 755a 4756  AAKcCAAB7ImluZGV
+00000a00: 3458 324e 7662 4856 7462 6e4d 694f 6942  4X2NvbHVtbnMiOiB
+00000a10: 6258 5377 6749 6d4e 7662 4856 7462 6c39  bXSwgImNvbHVtbl9
+00000a20: 7062 6d52 6c65 4756 7a49 6a6f 6757 3130  pbmRleGVzIjogW10
+00000a30: 7349 434a 6a62 3278 3162 5735 7a49 6a6f  sICJjb2x1bW5zIjo
+00000a40: 6757 3373 6962 6d46 745a 5349 3649 434a  gW3sibmFtZSI6ICJ
+00000a50: 705a 4349 7349 434a 6d61 5756 735a 4639  pZCIsICJmaWVsZF9
+00000a60: 7559 5731 6c49 6a6f 6749 6d6c 6b49 6977  uYW1lIjogImlkIiw
+00000a70: 6749 6e42 6862 6d52 6863 3139 3065 5842  gInBhbmRhc190eXB
+00000a80: 6c49 6a6f 6749 6d6c 7564 4459 3049 6977  lIjogImludDY0Iiw
+00000a90: 6749 6d35 3162 5842 3558 3352 3563 4755  gIm51bXB5X3R5cGU
+00000aa0: 694f 6941 6961 5735 304e 6a51 694c 4341  iOiAiaW50NjQiLCA
+00000ab0: 6962 5756 3059 5752 6864 4745 694f 6942  ibWV0YWRhdGEiOiB
+00000ac0: 7564 5778 7366 5377 6765 794a 7559 5731  udWxsfSwgeyJuYW1
+00000ad0: 6c49 6a6f 6749 6e4a 6849 6977 6749 6d5a  lIjogInJhIiwgImZ
+00000ae0: 705a 5778 6b58 3235 6862 5755 694f 6941  pZWxkX25hbWUiOiA
+00000af0: 6963 6d45 694c 4341 6963 4746 755a 4746  icmEiLCAicGFuZGF
+00000b00: 7a58 3352 3563 4755 694f 6941 695a 6d78  zX3R5cGUiOiAiZmx
+00000b10: 7659 5851 324e 4349 7349 434a 7564 5731  vYXQ2NCIsICJudW1
+00000b20: 7765 5639 3065 5842 6c49 6a6f 6749 6d5a  weV90eXBlIjogImZ
+00000b30: 7362 3246 304e 6a51 694c 4341 6962 5756  sb2F0NjQiLCAibWV
+00000b40: 3059 5752 6864 4745 694f 6942 7564 5778  0YWRhdGEiOiBudWx
+00000b50: 7366 5377 6765 794a 7559 5731 6c49 6a6f  sfSwgeyJuYW1lIjo
+00000b60: 6749 6d52 6c59 7949 7349 434a 6d61 5756  gImRlYyIsICJmaWV
+00000b70: 735a 4639 7559 5731 6c49 6a6f 6749 6d52  sZF9uYW1lIjogImR
+00000b80: 6c59 7949 7349 434a 7759 5735 6b59 584e  lYyIsICJwYW5kYXN
+00000b90: 6664 486c 775a 5349 3649 434a 6d62 4739  fdHlwZSI6ICJmbG9
+00000ba0: 6864 4459 3049 6977 6749 6d35 3162 5842  hdDY0IiwgIm51bXB
+00000bb0: 3558 3352 3563 4755 694f 6941 695a 6d78  5X3R5cGUiOiAiZmx
+00000bc0: 7659 5851 324e 4349 7349 434a 745a 5852  vYXQ2NCIsICJtZXR
+00000bd0: 685a 4746 3059 5349 3649 4735 3162 4778  hZGF0YSI6IG51bGx
+00000be0: 394c 4342 3749 6d35 6862 5755 694f 6941  9LCB7Im5hbWUiOiA
+00000bf0: 6963 6d46 665a 584a 7962 3349 694c 4341  icmFfZXJyb3IiLCA
+00000c00: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
+00000c10: 3649 434a 7959 5639 6c63 6e4a 7663 6949  6ICJyYV9lcnJvciI
+00000c20: 7349 434a 7759 5735 6b59 584e 6664 486c  sICJwYW5kYXNfdHl
+00000c30: 775a 5349 3649 434a 7062 6e51 324e 4349  wZSI6ICJpbnQ2NCI
+00000c40: 7349 434a 7564 5731 7765 5639 3065 5842  sICJudW1weV90eXB
+00000c50: 6c49 6a6f 6749 6d6c 7564 4459 3049 6977  lIjogImludDY0Iiw
+00000c60: 6749 6d31 6c64 4746 6b59 5852 6849 6a6f  gIm1ldGFkYXRhIjo
+00000c70: 6762 6e56 7362 4830 7349 4873 6962 6d46  gbnVsbH0sIHsibmF
+00000c80: 745a 5349 3649 434a 6b5a 574e 665a 584a  tZSI6ICJkZWNfZXJ
+00000c90: 7962 3349 694c 4341 695a 6d6c 6c62 4752  yb3IiLCAiZmllbGR
+00000ca0: 6662 6d46 745a 5349 3649 434a 6b5a 574e  fbmFtZSI6ICJkZWN
+00000cb0: 665a 584a 7962 3349 694c 4341 6963 4746  fZXJyb3IiLCAicGF
+00000cc0: 755a 4746 7a58 3352 3563 4755 694f 6941  uZGFzX3R5cGUiOiA
+00000cd0: 6961 5735 304e 6a51 694c 4341 6962 6e56  iaW50NjQiLCAibnV
+00000ce0: 7463 486c 6664 486c 775a 5349 3649 434a  tcHlfdHlwZSI6ICJ
+00000cf0: 7062 6e51 324e 4349 7349 434a 745a 5852  pbnQ2NCIsICJtZXR
+00000d00: 685a 4746 3059 5349 3649 4735 3162 4778  hZGF0YSI6IG51bGx
+00000d10: 3958 5377 6749 6d4e 795a 5746 3062 3349  9XSwgImNyZWF0b3I
+00000d20: 694f 6942 3749 6d78 7059 6e4a 6863 6e6b  iOiB7ImxpYnJhcnk
+00000d30: 694f 6941 6963 486c 6863 6e4a 7664 7949  iOiAicHlhcnJvdyI
+00000d40: 7349 434a 325a 584a 7a61 5739 7549 6a6f  sICJ2ZXJzaW9uIjo
+00000d50: 6749 6a6b 754d 4334 7749 6e30 7349 434a  gIjkuMC4wIn0sICJ
+00000d60: 7759 5735 6b59 584e 6664 6d56 7963 326c  wYW5kYXNfdmVyc2l
+00000d70: 7662 6949 3649 4349 794c 6a41 754d 434a  vbiI6ICIyLjAuMCJ
+00000d80: 3941 4155 4141 4144 6b41 4141 416f 4141  9AAUAAADkAAAAoAA
+00000d90: 4141 4851 4141 4141 3841 4141 4142 4141  AAHQAAAA8AAAABAA
+00000da0: 4141 4544 2f2f 2f38 4141 4145 4345 4141  AAED///8AAAECEAA
+00000db0: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
+00000dc0: 4141 416b 4141 4142 6b5a 574e 665a 584a  AAAkAAABkZWNfZXJ
+00000dd0: 7962 3349 4141 4141 342f 2f2f 2f41 4141  yb3IAAAA4////AAA
+00000de0: 4141 5541 4141 4142 302f 2f2f 2f41 4141  AAUAAAAB0////AAA
+00000df0: 4241 6841 4141 4141 6341 4141 4142 4141  BAhAAAAAcAAAABAA
+00000e00: 4141 4141 4141 4141 4941 4141 4163 6d46  AAAAAAAAIAAAAcmF
+00000e10: 665a 584a 7962 3349 4141 4141 4162 502f  fZXJyb3IAAAAAbP/
+00000e20: 2f2f 7741 4141 4146 4141 4141 4171 502f  //wAAAAFAAAAAqP/
+00000e30: 2f2f 7741 4141 514d 5141 4141 4146 4141  //wAAAQMQAAAAFAA
+00000e40: 4141 4151 4141 4141 4141 4141 4141 7741  AAAQAAAAAAAAAAwA
+00000e50: 4141 4752 6c59 7744 572f 2f2f 2f41 4141  AAGRlYwDW////AAA
+00000e60: 4341 4e44 2f2f 2f38 4141 4145 4445 4141  CAND///8AAAEDEAA
+00000e70: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
+00000e80: 4141 4149 4141 4142 7959 5141 4141 4141  AAAIAAAByYQAAAAA
+00000e90: 4741 4167 4142 6741 4741 4141 4141 4141  GAAgABgAGAAAAAAA
+00000ea0: 4341 4241 4146 4141 4941 4159 4142 7741  CABAAFAAIAAYABwA
+00000eb0: 4d41 4141 4145 4141 5141 4141 4141 4141  MAAAAEAAQAAAAAAA
+00000ec0: 4241 6841 4141 4141 6341 4141 4142 4141  BAhAAAAAcAAAABAA
+00000ed0: 4141 4141 4141 4141 4341 4141 4161 5751  AAAAAAAACAAAAaWQ
+00000ee0: 4141 4167 4144 4141 4941 4163 4143 4141  AAAgADAAIAAcACAA
+00000ef0: 4141 4141 4141 4146 4141 4141 4141 4141  AAAAAAAFAAAAAAAA
+00000f00: 4141 413d 3d00 181f 7061 7271 7565 742d  AAA==...parquet-
+00000f10: 6370 702d 6172 726f 7720 7665 7273 696f  cpp-arrow versio
+00000f20: 6e20 392e 302e 3019 5c1c 0000 1c00 001c  n 9.0.0.\.......
+00000f30: 0000 1c00 001c 0000 00d4 0a00 0050 4152  .............PAR
+00000f40: 31                                       1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_45/shard_0.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet`

 * *Files 19% similar despite different names*

```diff
@@ -1,303 +1,240 @@
-00000000: 5041 5231 1504 1540 1538 4c15 0815 0012  PAR1...@.8L.....
-00000010: 0000 2008 0b03 0005 0100 0d0d 083c 1003  .. ..........<..
-00000020: 0000 0000 0000 1203 0000 0000 0000 1500  ................
-00000030: 1514 1518 2c15 0815 1015 0615 061c 1808  ....,...........
-00000040: 1203 0000 0000 0000 1808 0b03 0000 0000  ................
-00000050: 0000 1600 2808 1203 0000 0000 0000 1808  ....(...........
-00000060: 0b03 0000 0000 0000 0000 000a 2402 0000  ............$...
-00000070: 0008 0102 03e4 0026 ee01 1c15 0419 3510  .......&......5.
-00000080: 0006 1918 0269 6415 0216 0816 ea01 16e6  .....id.........
-00000090: 0126 5c26 081c 1808 1203 0000 0000 0000  .&\&............
-000000a0: 1808 0b03 0000 0000 0000 1600 2808 1203  ............(...
-000000b0: 0000 0000 0000 1808 0b03 0000 0000 0000  ................
-000000c0: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
-000000d0: 0000 0015 0415 4015 3a4c 1508 1500 1200  ......@.:L......
-000000e0: 0020 0000 0101 08b8 7540 0107 0800 a874  . ......u@.....t
-000000f0: 0908 2828 7540 0000 0000 0008 7540 1500  ..((u@......u@..
-00000100: 1514 1518 2c15 0815 1015 0615 061c 1808  ....,...........
-00000110: 0000 0000 00b8 7540 1808 0000 0000 00a8  ......u@........
-00000120: 7440 1600 2808 0000 0000 00b8 7540 1808  t@..(.......u@..
-00000130: 0000 0000 00a8 7440 0000 000a 2402 0000  ......t@....$...
-00000140: 0008 0102 03e4 0026 8e05 1c15 0a19 3510  .......&......5.
-00000150: 0006 1918 0272 6115 0216 0816 ea01 16e8  .....ra.........
-00000160: 0126 fc03 26a6 031c 1808 0000 0000 00b8  .&..&...........
-00000170: 7540 1808 0000 0000 00a8 7440 1600 2808  u@........t@..(.
-00000180: 0000 0000 00b8 7540 1808 0000 0000 00a8  ......u@........
-00000190: 7440 0019 2c15 0415 0015 0200 1500 1510  t@..,...........
-000001a0: 1502 0000 0015 0415 4015 384c 1508 1500  ........@.8L....
-000001b0: 1200 0020 0000 0101 0880 3dc0 0107 0800  ... ......=.....
-000001c0: 4047 0d08 2444 c000 0000 0000 c040 c015  @G..$D.......@..
-000001d0: 0015 1415 182c 1508 1510 1506 1506 1c18  .....,..........
-000001e0: 0800 0000 0000 803d c018 0800 0000 0000  .......=........
-000001f0: 4047 c016 0028 0800 0000 0000 803d c018  @G...(.......=..
-00000200: 0800 0000 0000 4047 c000 0000 0a24 0200  ......@G.....$..
-00000210: 0000 0801 0203 e400 26b0 081c 150a 1935  ........&......5
-00000220: 1000 0619 1803 6465 6315 0216 0816 ea01  ......dec.......
-00000230: 16e6 0126 9e07 26ca 061c 1808 0000 0000  ...&..&.........
-00000240: 0080 3dc0 1808 0000 0000 0040 47c0 1600  ..=........@G...
-00000250: 2808 0000 0000 0080 3dc0 1808 0000 0000  (.......=.......
-00000260: 0040 47c0 0019 2c15 0415 0015 0200 1500  .@G...,.........
-00000270: 1510 1502 0000 0015 0415 1015 144c 1502  .............L..
-00000280: 1500 1200 0008 1c00 0000 0000 0000 0015  ................
-00000290: 0015 1215 162c 1508 1510 1506 1506 1c18  .....,..........
-000002a0: 0800 0000 0000 0000 0018 0800 0000 0000  ................
-000002b0: 0000 0016 0028 0800 0000 0000 0000 0018  .....(..........
-000002c0: 0800 0000 0000 0000 0000 0000 0920 0200  ............. ..
-000002d0: 0000 0801 0108 0026 ae0b 1c15 0419 3510  .......&......5.
-000002e0: 0006 1918 0872 615f 6572 726f 7215 0216  .....ra_error...
-000002f0: 0816 b801 16c0 0126 9e0a 26ee 091c 1808  .......&..&.....
-00000300: 0000 0000 0000 0000 1808 0000 0000 0000  ................
-00000310: 0000 1600 2808 0000 0000 0000 0000 1808  ....(...........
-00000320: 0000 0000 0000 0000 0019 2c15 0415 0015  ..........,.....
-00000330: 0200 1500 1510 1502 0000 0015 0415 1015  ................
-00000340: 144c 1502 1500 1200 0008 1c00 0000 0000  .L..............
-00000350: 0000 0015 0015 1215 162c 1508 1510 1506  .........,......
-00000360: 1506 1c18 0800 0000 0000 0000 0018 0800  ................
-00000370: 0000 0000 0000 0016 0028 0800 0000 0000  .........(......
-00000380: 0000 0018 0800 0000 0000 0000 0000 0000  ................
-00000390: 0920 0200 0000 0801 0108 0026 b60e 1c15  . .........&....
-000003a0: 0419 3510 0006 1918 0964 6563 5f65 7272  ..5......dec_err
-000003b0: 6f72 1502 1608 16b8 0116 c001 26a6 0d26  or..........&..&
-000003c0: f60c 1c18 0800 0000 0000 0000 0018 0800  ................
-000003d0: 0000 0000 0000 0016 0028 0800 0000 0000  .........(......
-000003e0: 0000 0018 0800 0000 0000 0000 0000 192c  ...............,
-000003f0: 1504 1500 1502 0015 0015 1015 0200 0000  ................
-00000400: 1504 1540 1538 4c15 0815 0012 0000 2004  ...@.8L....... .
-00000410: 0200 0901 0004 0907 4000 0700 0000 0000  ........@.......
-00000420: 0000 0900 0000 0000 0000 1500 1514 1518  ................
-00000430: 2c15 0815 1015 0615 061c 1808 0900 0000  ,...............
-00000440: 0000 0000 1808 0200 0000 0000 0000 1600  ................
-00000450: 2808 0900 0000 0000 0000 1808 0200 0000  (...............
-00000460: 0000 0000 0000 000a 2402 0000 0008 0102  ........$.......
-00000470: 03e4 0026 e611 1c15 0419 3510 0006 1918  ...&......5.....
-00000480: 115f 5f69 6e64 6578 5f6c 6576 656c 5f30  .__index_level_0
-00000490: 5f5f 1502 1608 16ea 0116 e601 26d4 1026  __..........&..&
-000004a0: 8010 1c18 0809 0000 0000 0000 0018 0802  ................
-000004b0: 0000 0000 0000 0016 0028 0809 0000 0000  .........(......
-000004c0: 0000 0018 0802 0000 0000 0000 0000 192c  ...............,
-000004d0: 1504 1500 1502 0015 0015 1015 0200 0000  ................
-000004e0: 1504 197c 3500 1806 7363 6865 6d61 150c  ...|5...schema..
-000004f0: 0015 0425 0218 0269 6400 150a 2502 1802  ...%...id...%...
-00000500: 7261 0015 0a25 0218 0364 6563 0015 0425  ra...%...dec...%
-00000510: 0218 0872 615f 6572 726f 7200 1504 2502  ...ra_error...%.
-00000520: 1809 6465 635f 6572 726f 7200 1504 2502  ..dec_error...%.
-00000530: 1811 5f5f 696e 6465 785f 6c65 7665 6c5f  ..__index_level_
-00000540: 305f 5f00 1608 191c 196c 26ee 011c 1504  0__......l&.....
-00000550: 1935 1000 0619 1802 6964 1502 1608 16ea  .5......id......
-00000560: 0116 e601 265c 2608 1c18 0812 0300 0000  ....&\&.........
-00000570: 0000 0018 080b 0300 0000 0000 0016 0028  ...............(
-00000580: 0812 0300 0000 0000 0018 080b 0300 0000  ................
-00000590: 0000 0000 192c 1504 1500 1502 0015 0015  .....,..........
-000005a0: 1015 0200 0000 268e 051c 150a 1935 1000  ......&......5..
-000005b0: 0619 1802 7261 1502 1608 16ea 0116 e801  ....ra..........
-000005c0: 26fc 0326 a603 1c18 0800 0000 0000 b875  &..&...........u
-000005d0: 4018 0800 0000 0000 a874 4016 0028 0800  @........t@..(..
-000005e0: 0000 0000 b875 4018 0800 0000 0000 a874  .....u@........t
-000005f0: 4000 192c 1504 1500 1502 0015 0015 1015  @..,............
-00000600: 0200 0000 26b0 081c 150a 1935 1000 0619  ....&......5....
-00000610: 1803 6465 6315 0216 0816 ea01 16e6 0126  ..dec..........&
-00000620: 9e07 26ca 061c 1808 0000 0000 0080 3dc0  ..&...........=.
-00000630: 1808 0000 0000 0040 47c0 1600 2808 0000  .......@G...(...
-00000640: 0000 0080 3dc0 1808 0000 0000 0040 47c0  ....=........@G.
-00000650: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
-00000660: 0000 0026 ae0b 1c15 0419 3510 0006 1918  ...&......5.....
-00000670: 0872 615f 6572 726f 7215 0216 0816 b801  .ra_error.......
-00000680: 16c0 0126 9e0a 26ee 091c 1808 0000 0000  ...&..&.........
-00000690: 0000 0000 1808 0000 0000 0000 0000 1600  ................
-000006a0: 2808 0000 0000 0000 0000 1808 0000 0000  (...............
-000006b0: 0000 0000 0019 2c15 0415 0015 0200 1500  ......,.........
-000006c0: 1510 1502 0000 0026 b60e 1c15 0419 3510  .......&......5.
-000006d0: 0006 1918 0964 6563 5f65 7272 6f72 1502  .....dec_error..
-000006e0: 1608 16b8 0116 c001 26a6 0d26 f60c 1c18  ........&..&....
-000006f0: 0800 0000 0000 0000 0018 0800 0000 0000  ................
-00000700: 0000 0016 0028 0800 0000 0000 0000 0018  .....(..........
-00000710: 0800 0000 0000 0000 0000 192c 1504 1500  ...........,....
-00000720: 1502 0015 0015 1015 0200 0000 26e6 111c  ............&...
-00000730: 1504 1935 1000 0619 1811 5f5f 696e 6465  ...5......__inde
-00000740: 785f 6c65 7665 6c5f 305f 5f15 0216 0816  x_level_0__.....
-00000750: ea01 16e6 0126 d410 2680 101c 1808 0900  .....&..&.......
-00000760: 0000 0000 0000 1808 0200 0000 0000 0000  ................
-00000770: 1600 2808 0900 0000 0000 0000 1808 0200  ..(.............
-00000780: 0000 0000 0000 0019 2c15 0415 0015 0200  ........,.......
-00000790: 1500 1510 1502 0000 0016 980a 1608 2608  ..............&.
-000007a0: 169a 0a14 0000 192c 1806 7061 6e64 6173  .......,..pandas
-000007b0: 18a5 077b 2269 6e64 6578 5f63 6f6c 756d  ...{"index_colum
-000007c0: 6e73 223a 205b 225f 5f69 6e64 6578 5f6c  ns": ["__index_l
-000007d0: 6576 656c 5f30 5f5f 225d 2c20 2263 6f6c  evel_0__"], "col
-000007e0: 756d 6e5f 696e 6465 7865 7322 3a20 5b7b  umn_indexes": [{
-000007f0: 226e 616d 6522 3a20 6e75 6c6c 2c20 2266  "name": null, "f
-00000800: 6965 6c64 5f6e 616d 6522 3a20 6e75 6c6c  ield_name": null
-00000810: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
-00000820: 2022 756e 6963 6f64 6522 2c20 226e 756d   "unicode", "num
-00000830: 7079 5f74 7970 6522 3a20 226f 626a 6563  py_type": "objec
-00000840: 7422 2c20 226d 6574 6164 6174 6122 3a20  t", "metadata": 
-00000850: 7b22 656e 636f 6469 6e67 223a 2022 5554  {"encoding": "UT
-00000860: 462d 3822 7d7d 5d2c 2022 636f 6c75 6d6e  F-8"}}], "column
-00000870: 7322 3a20 5b7b 226e 616d 6522 3a20 2269  s": [{"name": "i
-00000880: 6422 2c20 2266 6965 6c64 5f6e 616d 6522  d", "field_name"
-00000890: 3a20 2269 6422 2c20 2270 616e 6461 735f  : "id", "pandas_
-000008a0: 7479 7065 223a 2022 696e 7436 3422 2c20  type": "int64", 
-000008b0: 226e 756d 7079 5f74 7970 6522 3a20 2269  "numpy_type": "i
-000008c0: 6e74 3634 222c 2022 6d65 7461 6461 7461  nt64", "metadata
-000008d0: 223a 206e 756c 6c7d 2c20 7b22 6e61 6d65  ": null}, {"name
-000008e0: 223a 2022 7261 222c 2022 6669 656c 645f  ": "ra", "field_
-000008f0: 6e61 6d65 223a 2022 7261 222c 2022 7061  name": "ra", "pa
-00000900: 6e64 6173 5f74 7970 6522 3a20 2266 6c6f  ndas_type": "flo
-00000910: 6174 3634 222c 2022 6e75 6d70 795f 7479  at64", "numpy_ty
-00000920: 7065 223a 2022 666c 6f61 7436 3422 2c20  pe": "float64", 
-00000930: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
-00000940: 7d2c 207b 226e 616d 6522 3a20 2264 6563  }, {"name": "dec
-00000950: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
-00000960: 2022 6465 6322 2c20 2270 616e 6461 735f   "dec", "pandas_
-00000970: 7479 7065 223a 2022 666c 6f61 7436 3422  type": "float64"
-00000980: 2c20 226e 756d 7079 5f74 7970 6522 3a20  , "numpy_type": 
-00000990: 2266 6c6f 6174 3634 222c 2022 6d65 7461  "float64", "meta
-000009a0: 6461 7461 223a 206e 756c 6c7d 2c20 7b22  data": null}, {"
-000009b0: 6e61 6d65 223a 2022 7261 5f65 7272 6f72  name": "ra_error
-000009c0: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
-000009d0: 2022 7261 5f65 7272 6f72 222c 2022 7061   "ra_error", "pa
-000009e0: 6e64 6173 5f74 7970 6522 3a20 2269 6e74  ndas_type": "int
-000009f0: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
-00000a00: 223a 2022 696e 7436 3422 2c20 226d 6574  ": "int64", "met
-00000a10: 6164 6174 6122 3a20 6e75 6c6c 7d2c 207b  adata": null}, {
-00000a20: 226e 616d 6522 3a20 2264 6563 5f65 7272  "name": "dec_err
-00000a30: 6f72 222c 2022 6669 656c 645f 6e61 6d65  or", "field_name
-00000a40: 223a 2022 6465 635f 6572 726f 7222 2c20  ": "dec_error", 
-00000a50: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
-00000a60: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
-00000a70: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
-00000a80: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
-00000a90: 2c20 7b22 6e61 6d65 223a 206e 756c 6c2c  , {"name": null,
-00000aa0: 2022 6669 656c 645f 6e61 6d65 223a 2022   "field_name": "
-00000ab0: 5f5f 696e 6465 785f 6c65 7665 6c5f 305f  __index_level_0_
-00000ac0: 5f22 2c20 2270 616e 6461 735f 7479 7065  _", "pandas_type
-00000ad0: 223a 2022 696e 7436 3422 2c20 226e 756d  ": "int64", "num
-00000ae0: 7079 5f74 7970 6522 3a20 2269 6e74 3634  py_type": "int64
-00000af0: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
-00000b00: 756c 6c7d 5d2c 2022 6372 6561 746f 7222  ull}], "creator"
-00000b10: 3a20 7b22 6c69 6272 6172 7922 3a20 2270  : {"library": "p
-00000b20: 7961 7272 6f77 222c 2022 7665 7273 696f  yarrow", "versio
-00000b30: 6e22 3a20 2239 2e30 2e30 227d 2c20 2270  n": "9.0.0"}, "p
-00000b40: 616e 6461 735f 7665 7273 696f 6e22 3a20  andas_version": 
-00000b50: 2231 2e33 2e35 227d 0018 0c41 5252 4f57  "1.3.5"}...ARROW
-00000b60: 3a73 6368 656d 6118 c00e 2f2f 2f2f 2f32  :schema.../////2
-00000b70: 6746 4141 4151 4141 4141 4141 414b 4141  gFAAAQAAAAAAAKAA
-00000b80: 3441 4267 4146 4141 6741 4367 4141 4141  4ABgAFAAgACgAAAA
-00000b90: 4142 4241 4151 4141 4141 4141 414b 4141  ABBAAQAAAAAAAKAA
-00000ba0: 7741 4141 4145 4141 6741 4367 4141 414e  wAAAAEAAgACgAAAN
-00000bb0: 7744 4141 4145 4141 4141 4151 4141 4141  wDAAAEAAAAAQAAAA
-00000bc0: 7741 4141 4149 4141 7741 4241 4149 4141  wAAAAIAAwABAAIAA
-00000bd0: 6741 4141 4149 4141 4141 4541 4141 4141  gAAAAIAAAAEAAAAA
-00000be0: 5941 4141 4277 5957 356b 5958 4d41 414b  YAAABwYW5kYXMAAK
-00000bf0: 5544 4141 4237 496d 6c75 5a47 5634 5832  UDAAB7ImluZGV4X2
-00000c00: 4e76 6248 5674 626e 4d69 4f69 4262 496c  NvbHVtbnMiOiBbIl
-00000c10: 3966 6157 356b 5a58 6866 6247 5632 5a57  9faW5kZXhfbGV2ZW
-00000c20: 7866 4d46 3966 496c 3073 4943 4a6a 6232  xfMF9fIl0sICJjb2
-00000c30: 7831 6257 3566 6157 356b 5a58 686c 6379  x1bW5faW5kZXhlcy
-00000c40: 4936 4946 7437 496d 3568 6257 5569 4f69  I6IFt7Im5hbWUiOi
-00000c50: 4275 6457 7873 4c43 4169 5a6d 6c6c 6247  BudWxsLCAiZmllbG
-00000c60: 5266 626d 4674 5a53 4936 4947 3531 6247  RfbmFtZSI6IG51bG
-00000c70: 7773 4943 4a77 5957 356b 5958 4e66 6448  wsICJwYW5kYXNfdH
-00000c80: 6c77 5a53 4936 4943 4a31 626d 6c6a 6232  lwZSI6ICJ1bmljb2
-00000c90: 526c 4969 7767 496d 3531 6258 4235 5833  RlIiwgIm51bXB5X3
-00000ca0: 5235 6347 5569 4f69 4169 6232 4a71 5a57  R5cGUiOiAib2JqZW
-00000cb0: 4e30 4969 7767 496d 316c 6447 466b 5958  N0IiwgIm1ldGFkYX
-00000cc0: 5268 496a 6f67 6579 4a6c 626d 4e76 5a47  RhIjogeyJlbmNvZG
-00000cd0: 6c75 5a79 4936 4943 4a56 5645 5974 4f43  luZyI6ICJVVEYtOC
-00000ce0: 4a39 6656 3073 4943 4a6a 6232 7831 6257  J9fV0sICJjb2x1bW
-00000cf0: 357a 496a 6f67 5733 7369 626d 4674 5a53  5zIjogW3sibmFtZS
-00000d00: 4936 4943 4a70 5a43 4973 4943 4a6d 6157  I6ICJpZCIsICJmaW
-00000d10: 5673 5a46 3975 5957 316c 496a 6f67 496d  VsZF9uYW1lIjogIm
-00000d20: 6c6b 4969 7767 496e 4268 626d 5268 6331  lkIiwgInBhbmRhc1
-00000d30: 3930 6558 426c 496a 6f67 496d 6c75 6444  90eXBlIjogImludD
-00000d40: 5930 4969 7767 496d 3531 6258 4235 5833  Y0IiwgIm51bXB5X3
-00000d50: 5235 6347 5569 4f69 4169 6157 3530 4e6a  R5cGUiOiAiaW50Nj
-00000d60: 5169 4c43 4169 6257 5630 5957 5268 6447  QiLCAibWV0YWRhdG
-00000d70: 4569 4f69 4275 6457 7873 6653 7767 6579  EiOiBudWxsfSwgey
-00000d80: 4a75 5957 316c 496a 6f67 496e 4a68 4969  JuYW1lIjogInJhIi
-00000d90: 7767 496d 5a70 5a57 786b 5832 3568 6257  wgImZpZWxkX25hbW
-00000da0: 5569 4f69 4169 636d 4569 4c43 4169 6347  UiOiAicmEiLCAicG
-00000db0: 4675 5a47 467a 5833 5235 6347 5569 4f69  FuZGFzX3R5cGUiOi
-00000dc0: 4169 5a6d 7876 5958 5132 4e43 4973 4943  AiZmxvYXQ2NCIsIC
-00000dd0: 4a75 6457 3177 6556 3930 6558 426c 496a  JudW1weV90eXBlIj
-00000de0: 6f67 496d 5a73 6232 4630 4e6a 5169 4c43  ogImZsb2F0NjQiLC
-00000df0: 4169 6257 5630 5957 5268 6447 4569 4f69  AibWV0YWRhdGEiOi
-00000e00: 4275 6457 7873 6653 7767 6579 4a75 5957  BudWxsfSwgeyJuYW
-00000e10: 316c 496a 6f67 496d 526c 5979 4973 4943  1lIjogImRlYyIsIC
-00000e20: 4a6d 6157 5673 5a46 3975 5957 316c 496a  JmaWVsZF9uYW1lIj
-00000e30: 6f67 496d 526c 5979 4973 4943 4a77 5957  ogImRlYyIsICJwYW
-00000e40: 356b 5958 4e66 6448 6c77 5a53 4936 4943  5kYXNfdHlwZSI6IC
-00000e50: 4a6d 6247 3968 6444 5930 4969 7767 496d  JmbG9hdDY0IiwgIm
-00000e60: 3531 6258 4235 5833 5235 6347 5569 4f69  51bXB5X3R5cGUiOi
-00000e70: 4169 5a6d 7876 5958 5132 4e43 4973 4943  AiZmxvYXQ2NCIsIC
-00000e80: 4a74 5a58 5268 5a47 4630 5953 4936 4947  JtZXRhZGF0YSI6IG
-00000e90: 3531 6247 7839 4c43 4237 496d 3568 6257  51bGx9LCB7Im5hbW
-00000ea0: 5569 4f69 4169 636d 4666 5a58 4a79 6233  UiOiAicmFfZXJyb3
-00000eb0: 4969 4c43 4169 5a6d 6c6c 6247 5266 626d  IiLCAiZmllbGRfbm
-00000ec0: 4674 5a53 4936 4943 4a79 5956 396c 636e  FtZSI6ICJyYV9lcn
-00000ed0: 4a76 6369 4973 4943 4a77 5957 356b 5958  JvciIsICJwYW5kYX
-00000ee0: 4e66 6448 6c77 5a53 4936 4943 4a70 626e  NfdHlwZSI6ICJpbn
-00000ef0: 5132 4e43 4973 4943 4a75 6457 3177 6556  Q2NCIsICJudW1weV
-00000f00: 3930 6558 426c 496a 6f67 496d 6c75 6444  90eXBlIjogImludD
-00000f10: 5930 4969 7767 496d 316c 6447 466b 5958  Y0IiwgIm1ldGFkYX
-00000f20: 5268 496a 6f67 626e 5673 6248 3073 4948  RhIjogbnVsbH0sIH
-00000f30: 7369 626d 4674 5a53 4936 4943 4a6b 5a57  sibmFtZSI6ICJkZW
-00000f40: 4e66 5a58 4a79 6233 4969 4c43 4169 5a6d  NfZXJyb3IiLCAiZm
-00000f50: 6c6c 6247 5266 626d 4674 5a53 4936 4943  llbGRfbmFtZSI6IC
-00000f60: 4a6b 5a57 4e66 5a58 4a79 6233 4969 4c43  JkZWNfZXJyb3IiLC
-00000f70: 4169 6347 4675 5a47 467a 5833 5235 6347  AicGFuZGFzX3R5cG
-00000f80: 5569 4f69 4169 6157 3530 4e6a 5169 4c43  UiOiAiaW50NjQiLC
-00000f90: 4169 626e 5674 6348 6c66 6448 6c77 5a53  AibnVtcHlfdHlwZS
-00000fa0: 4936 4943 4a70 626e 5132 4e43 4973 4943  I6ICJpbnQ2NCIsIC
-00000fb0: 4a74 5a58 5268 5a47 4630 5953 4936 4947  JtZXRhZGF0YSI6IG
-00000fc0: 3531 6247 7839 4c43 4237 496d 3568 6257  51bGx9LCB7Im5hbW
-00000fd0: 5569 4f69 4275 6457 7873 4c43 4169 5a6d  UiOiBudWxsLCAiZm
-00000fe0: 6c6c 6247 5266 626d 4674 5a53 4936 4943  llbGRfbmFtZSI6IC
-00000ff0: 4a66 5832 6c75 5a47 5634 5832 786c 646d  JfX2luZGV4X2xldm
-00001000: 5673 587a 4266 5879 4973 4943 4a77 5957  VsXzBfXyIsICJwYW
-00001010: 356b 5958 4e66 6448 6c77 5a53 4936 4943  5kYXNfdHlwZSI6IC
-00001020: 4a70 626e 5132 4e43 4973 4943 4a75 6457  JpbnQ2NCIsICJudW
-00001030: 3177 6556 3930 6558 426c 496a 6f67 496d  1weV90eXBlIjogIm
-00001040: 6c75 6444 5930 4969 7767 496d 316c 6447  ludDY0IiwgIm1ldG
-00001050: 466b 5958 5268 496a 6f67 626e 5673 6248  FkYXRhIjogbnVsbH
-00001060: 3164 4c43 4169 5933 4a6c 5958 5276 6369  1dLCAiY3JlYXRvci
-00001070: 4936 4948 7369 6247 6c69 636d 4679 6553  I6IHsibGlicmFyeS
-00001080: 4936 4943 4a77 6557 4679 636d 3933 4969  I6ICJweWFycm93Ii
-00001090: 7767 496e 5a6c 636e 4e70 6232 3469 4f69  wgInZlcnNpb24iOi
-000010a0: 4169 4f53 3477 4c6a 4169 6653 7767 496e  AiOS4wLjAifSwgIn
-000010b0: 4268 626d 5268 6331 3932 5a58 4a7a 6157  BhbmRhc192ZXJzaW
-000010c0: 3975 496a 6f67 496a 4575 4d79 3431 496e  9uIjogIjEuMy41In
-000010d0: 3041 4141 4147 4141 4141 4a41 4541 414f  0AAAAGAAAAJAEAAO
-000010e0: 4141 4141 4330 4141 4141 6641 4141 4145  AAAAC0AAAAfAAAAE
-000010f0: 5141 4141 4145 4141 4141 4250 2f2f 2f77  QAAAAEAAAABP///w
-00001100: 4141 4151 4951 4141 4141 4a41 4141 4141  AAAQIQAAAAJAAAAA
-00001110: 5141 4141 4141 4141 4141 4551 4141 4146  QAAAAAAAAAEQAAAF
-00001120: 3966 6157 356b 5a58 6866 6247 5632 5a57  9faW5kZXhfbGV2ZW
-00001130: 7866 4d46 3966 4141 4141 4250 2f2f 2f77  xfMF9fAAAABP///w
-00001140: 4141 4141 4641 4141 4141 5150 2f2f 2f77  AAAAFAAAAAQP///w
-00001150: 4141 4151 4951 4141 4141 4841 4141 4141  AAAQIQAAAAHAAAAA
-00001160: 5141 4141 4141 4141 4141 4351 4141 4147  QAAAAAAAAACQAAAG
-00001170: 526c 5931 396c 636e 4a76 6367 4141 4144  RlY19lcnJvcgAAAD
-00001180: 6a2f 2f2f 3841 4141 4142 5141 4141 4148  j///8AAAABQAAAAH
-00001190: 542f 2f2f 3841 4141 4543 4541 4141 4142  T///8AAAECEAAAAB
-000011a0: 7741 4141 4145 4141 4141 4141 4141 4141  wAAAAEAAAAAAAAAA
-000011b0: 6741 4141 4279 5956 396c 636e 4a76 6367  gAAAByYV9lcnJvcg
-000011c0: 4141 4141 4273 2f2f 2f2f 4141 4141 4155  AAAABs////AAAAAU
-000011d0: 4141 4141 436f 2f2f 2f2f 4141 4142 4178  AAAACo////AAABAx
-000011e0: 4141 4141 4155 4141 4141 4241 4141 4141  AAAAAUAAAABAAAAA
-000011f0: 4141 4141 4144 4141 4141 5a47 566a 414e  AAAAADAAAAZGVjAN
-00001200: 622f 2f2f 3841 4141 4941 3050 2f2f 2f77  b///8AAAIA0P///w
-00001210: 4141 4151 4d51 4141 4141 4841 4141 4141  AAAQMQAAAAHAAAAA
-00001220: 5141 4141 4141 4141 4141 4167 4141 4148  QAAAAAAAAAAgAAAH
-00001230: 4a68 4141 4141 4141 5941 4341 4147 4141  JhAAAAAAYACAAGAA
-00001240: 5941 4141 4141 4141 4941 4541 4155 4141  YAAAAAAAIAEAAUAA
-00001250: 6741 4267 4148 4141 7741 4141 4151 4142  gABgAHAAwAAAAQAB
-00001260: 4141 4141 4141 4141 4543 4541 4141 4142  AAAAAAAAECEAAAAB
-00001270: 7741 4141 4145 4141 4141 4141 4141 4141  wAAAAEAAAAAAAAAA
-00001280: 4941 4141 4270 5a41 4141 4341 414d 4141  IAAABpZAAACAAMAA
-00001290: 6741 4277 4149 4141 4141 4141 4141 4155  gABwAIAAAAAAAAAU
-000012a0: 4141 4141 4141 4141 4141 0018 1f70 6172  AAAAAAAAAA...par
-000012b0: 7175 6574 2d63 7070 2d61 7272 6f77 2076  quet-cpp-arrow v
-000012c0: 6572 7369 6f6e 2039 2e30 2e30 196c 1c00  ersion 9.0.0.l..
-000012d0: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
-000012e0: 0001 0e00 0050 4152 31                   .....PAR1
+00000000: 5041 5231 1504 1570 1550 4c15 0e15 0012  PAR1...p.PL.....
+00000010: 0000 3808 c002 0005 0100 c10d 0800 c60d  ..8.............
+00000020: 0800 cf0d 0800 d00d 083c d202 0000 0000  .........<......
+00000030: 0000 d402 0000 0000 0000 1500 1516 151a  ................
+00000040: 2c15 0e15 1015 0615 061c 1808 d402 0000  ,...............
+00000050: 0000 0000 1808 c002 0000 0000 0000 1600  ................
+00000060: 2808 d402 0000 0000 0000 1808 c002 0000  (...............
+00000070: 0000 0000 0000 000b 2802 0000 000e 0103  ........(.......
+00000080: 0388 c61a 2688 021c 1504 1935 1000 0619  ....&......5....
+00000090: 1802 6964 1502 160e 169c 0216 8002 2674  ..id..........&t
+000000a0: 2608 1c18 08d4 0200 0000 0000 0018 08c0  &...............
+000000b0: 0200 0000 0000 0016 0028 08d4 0200 0000  .........(......
+000000c0: 0000 0018 08c0 0200 0000 0000 0000 192c  ...............,
+000000d0: 1504 1500 1502 0015 0015 1015 0200 0000  ................
+000000e0: 1504 1560 154a 4c15 0c15 0012 0000 3000  ...`.JL.......0.
+000000f0: 0001 0108 6874 4001 0704 00f8 0d08 0458  ....ht@........X
+00000100: 7509 1000 880d 0828 e875 4000 0000 0000  u......(.u@.....
+00000110: 3874 4015 0015 1615 1a2c 150e 1510 1506  8t@......,......
+00000120: 1506 1c18 0800 0000 0000 e875 4018 0800  ...........u@...
+00000130: 0000 0000 3874 4016 0028 0800 0000 0000  ....8t@..(......
+00000140: e875 4018 0800 0000 0000 3874 4000 0000  .u@.......8t@...
+00000150: 0b28 0200 0000 0e01 0303 8836 1626 ba05  .(.........6.&..
+00000160: 1c15 0a19 3510 0006 1918 0272 6115 0216  ....5......ra...
+00000170: 0e16 8c02 16fa 0126 a604 26c0 031c 1808  .......&..&.....
+00000180: 0000 0000 00e8 7540 1808 0000 0000 0038  ......u@.......8
+00000190: 7440 1600 2808 0000 0000 00e8 7540 1808  t@..(.......u@..
+000001a0: 0000 0000 0038 7440 0019 2c15 0415 0015  .....8t@..,.....
+000001b0: 0200 1500 1510 1502 0000 0015 0415 6015  ..............`.
+000001c0: 4c4c 150c 1500 1200 0030 0000 0101 08c0  LL.......0......
+000001d0: 46c0 0107 0800 4040 0908 04c0 430d 0800  F.....@@....C...
+000001e0: 4709 0828 404d c000 0000 0000 c044 c015  G..(@M.......D..
+000001f0: 0015 1615 1a2c 150e 1510 1506 1506 1c18  .....,..........
+00000200: 0800 0000 0000 4040 c018 0800 0000 0000  ......@@........
+00000210: 404d c016 0028 0800 0000 0000 4040 c018  @M...(......@@..
+00000220: 0800 0000 0000 404d c000 0000 0b28 0200  ......@M.....(..
+00000230: 0000 0e01 0303 8834 1626 f208 1c15 0a19  .......4.&......
+00000240: 3510 0006 1918 0364 6563 1502 160e 168c  5......dec......
+00000250: 0216 fc01 26de 0726 f606 1c18 0800 0000  ....&..&........
+00000260: 0000 4040 c018 0800 0000 0000 404d c016  ..@@........@M..
+00000270: 0028 0800 0000 0000 4040 c018 0800 0000  .(......@@......
+00000280: 0000 404d c000 192c 1504 1500 1502 0015  ..@M...,........
+00000290: 0015 1015 0200 0000 1504 1510 1514 4c15  ..............L.
+000002a0: 0215 0012 0000 081c 0000 0000 0000 0000  ................
+000002b0: 1500 1512 1516 2c15 0e15 1015 0615 061c  ......,.........
+000002c0: 1808 0000 0000 0000 0000 1808 0000 0000  ................
+000002d0: 0000 0000 1600 2808 0000 0000 0000 0000  ......(.........
+000002e0: 1808 0000 0000 0000 0000 0000 0009 2002  .............. .
+000002f0: 0000 000e 0101 0e00 26f0 0b1c 1504 1935  ........&......5
+00000300: 1000 0619 1808 7261 5f65 7272 6f72 1502  ......ra_error..
+00000310: 160e 16b8 0116 c001 26e0 0a26 b00a 1c18  ........&..&....
+00000320: 0800 0000 0000 0000 0018 0800 0000 0000  ................
+00000330: 0000 0016 0028 0800 0000 0000 0000 0018  .....(..........
+00000340: 0800 0000 0000 0000 0000 192c 1504 1500  ...........,....
+00000350: 1502 0015 0015 1015 0200 0000 1504 1510  ................
+00000360: 1514 4c15 0215 0012 0000 081c 0000 0000  ..L.............
+00000370: 0000 0000 1500 1512 1516 2c15 0e15 1015  ..........,.....
+00000380: 0615 061c 1808 0000 0000 0000 0000 1808  ................
+00000390: 0000 0000 0000 0000 1600 2808 0000 0000  ..........(.....
+000003a0: 0000 0000 1808 0000 0000 0000 0000 0000  ................
+000003b0: 0009 2002 0000 000e 0101 0e00 26f8 0e1c  .. .........&...
+000003c0: 1504 1935 1000 0619 1809 6465 635f 6572  ...5......dec_er
+000003d0: 726f 7215 0216 0e16 b801 16c0 0126 e80d  ror..........&..
+000003e0: 26b8 0d1c 1808 0000 0000 0000 0000 1808  &...............
+000003f0: 0000 0000 0000 0000 1600 2808 0000 0000  ..........(.....
+00000400: 0000 0000 1808 0000 0000 0000 0000 0019  ................
+00000410: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
+00000420: 0015 0419 6c35 0018 0673 6368 656d 6115  ....l5...schema.
+00000430: 0a00 1504 2502 1802 6964 0015 0a25 0218  ....%...id...%..
+00000440: 0272 6100 150a 2502 1803 6465 6300 1504  .ra...%...dec...
+00000450: 2502 1808 7261 5f65 7272 6f72 0015 0425  %...ra_error...%
+00000460: 0218 0964 6563 5f65 7272 6f72 0016 0e19  ...dec_error....
+00000470: 1c19 5c26 8802 1c15 0419 3510 0006 1918  ..\&......5.....
+00000480: 0269 6415 0216 0e16 9c02 1680 0226 7426  .id..........&t&
+00000490: 081c 1808 d402 0000 0000 0000 1808 c002  ................
+000004a0: 0000 0000 0000 1600 2808 d402 0000 0000  ........(.......
+000004b0: 0000 1808 c002 0000 0000 0000 0019 2c15  ..............,.
+000004c0: 0415 0015 0200 1500 1510 1502 0000 0026  ...............&
+000004d0: ba05 1c15 0a19 3510 0006 1918 0272 6115  ......5......ra.
+000004e0: 0216 0e16 8c02 16fa 0126 a604 26c0 031c  .........&..&...
+000004f0: 1808 0000 0000 00e8 7540 1808 0000 0000  ........u@......
+00000500: 0038 7440 1600 2808 0000 0000 00e8 7540  .8t@..(.......u@
+00000510: 1808 0000 0000 0038 7440 0019 2c15 0415  .......8t@..,...
+00000520: 0015 0200 1500 1510 1502 0000 0026 f208  .............&..
+00000530: 1c15 0a19 3510 0006 1918 0364 6563 1502  ....5......dec..
+00000540: 160e 168c 0216 fc01 26de 0726 f606 1c18  ........&..&....
+00000550: 0800 0000 0000 4040 c018 0800 0000 0000  ......@@........
+00000560: 404d c016 0028 0800 0000 0000 4040 c018  @M...(......@@..
+00000570: 0800 0000 0000 404d c000 192c 1504 1500  ......@M...,....
+00000580: 1502 0015 0015 1015 0200 0000 26f0 0b1c  ............&...
+00000590: 1504 1935 1000 0619 1808 7261 5f65 7272  ...5......ra_err
+000005a0: 6f72 1502 160e 16b8 0116 c001 26e0 0a26  or..........&..&
+000005b0: b00a 1c18 0800 0000 0000 0000 0018 0800  ................
+000005c0: 0000 0000 0000 0016 0028 0800 0000 0000  .........(......
+000005d0: 0000 0018 0800 0000 0000 0000 0000 192c  ...............,
+000005e0: 1504 1500 1502 0015 0015 1015 0200 0000  ................
+000005f0: 26f8 0e1c 1504 1935 1000 0619 1809 6465  &......5......de
+00000600: 635f 6572 726f 7215 0216 0e16 b801 16c0  c_error.........
+00000610: 0126 e80d 26b8 0d1c 1808 0000 0000 0000  .&..&...........
+00000620: 0000 1808 0000 0000 0000 0000 1600 2808  ..............(.
+00000630: 0000 0000 0000 0000 1808 0000 0000 0000  ................
+00000640: 0000 0019 2c15 0415 0015 0200 1500 1510  ....,...........
+00000650: 1502 0000 0016 a409 160e 2608 16f6 0814  ..........&.....
+00000660: 0000 192c 1806 7061 6e64 6173 18a7 057b  ...,..pandas...{
+00000670: 2269 6e64 6578 5f63 6f6c 756d 6e73 223a  "index_columns":
+00000680: 205b 5d2c 2022 636f 6c75 6d6e 5f69 6e64   [], "column_ind
+00000690: 6578 6573 223a 205b 5d2c 2022 636f 6c75  exes": [], "colu
+000006a0: 6d6e 7322 3a20 5b7b 226e 616d 6522 3a20  mns": [{"name": 
+000006b0: 2269 6422 2c20 2266 6965 6c64 5f6e 616d  "id", "field_nam
+000006c0: 6522 3a20 2269 6422 2c20 2270 616e 6461  e": "id", "panda
+000006d0: 735f 7479 7065 223a 2022 696e 7436 3422  s_type": "int64"
+000006e0: 2c20 226e 756d 7079 5f74 7970 6522 3a20  , "numpy_type": 
+000006f0: 2269 6e74 3634 222c 2022 6d65 7461 6461  "int64", "metada
+00000700: 7461 223a 206e 756c 6c7d 2c20 7b22 6e61  ta": null}, {"na
+00000710: 6d65 223a 2022 7261 222c 2022 6669 656c  me": "ra", "fiel
+00000720: 645f 6e61 6d65 223a 2022 7261 222c 2022  d_name": "ra", "
+00000730: 7061 6e64 6173 5f74 7970 6522 3a20 2266  pandas_type": "f
+00000740: 6c6f 6174 3634 222c 2022 6e75 6d70 795f  loat64", "numpy_
+00000750: 7479 7065 223a 2022 666c 6f61 7436 3422  type": "float64"
+00000760: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
+00000770: 6c6c 7d2c 207b 226e 616d 6522 3a20 2264  ll}, {"name": "d
+00000780: 6563 222c 2022 6669 656c 645f 6e61 6d65  ec", "field_name
+00000790: 223a 2022 6465 6322 2c20 2270 616e 6461  ": "dec", "panda
+000007a0: 735f 7479 7065 223a 2022 666c 6f61 7436  s_type": "float6
+000007b0: 3422 2c20 226e 756d 7079 5f74 7970 6522  4", "numpy_type"
+000007c0: 3a20 2266 6c6f 6174 3634 222c 2022 6d65  : "float64", "me
+000007d0: 7461 6461 7461 223a 206e 756c 6c7d 2c20  tadata": null}, 
+000007e0: 7b22 6e61 6d65 223a 2022 7261 5f65 7272  {"name": "ra_err
+000007f0: 6f72 222c 2022 6669 656c 645f 6e61 6d65  or", "field_name
+00000800: 223a 2022 7261 5f65 7272 6f72 222c 2022  ": "ra_error", "
+00000810: 7061 6e64 6173 5f74 7970 6522 3a20 2269  pandas_type": "i
+00000820: 6e74 3634 222c 2022 6e75 6d70 795f 7479  nt64", "numpy_ty
+00000830: 7065 223a 2022 696e 7436 3422 2c20 226d  pe": "int64", "m
+00000840: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
+00000850: 207b 226e 616d 6522 3a20 2264 6563 5f65   {"name": "dec_e
+00000860: 7272 6f72 222c 2022 6669 656c 645f 6e61  rror", "field_na
+00000870: 6d65 223a 2022 6465 635f 6572 726f 7222  me": "dec_error"
+00000880: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
+00000890: 2022 696e 7436 3422 2c20 226e 756d 7079   "int64", "numpy
+000008a0: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
+000008b0: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
+000008c0: 6c7d 5d2c 2022 6372 6561 746f 7222 3a20  l}], "creator": 
+000008d0: 7b22 6c69 6272 6172 7922 3a20 2270 7961  {"library": "pya
+000008e0: 7272 6f77 222c 2022 7665 7273 696f 6e22  rrow", "version"
+000008f0: 3a20 2239 2e30 2e30 227d 2c20 2270 616e  : "9.0.0"}, "pan
+00000900: 6461 735f 7665 7273 696f 6e22 3a20 2232  das_version": "2
+00000910: 2e30 2e30 227d 0018 0c41 5252 4f57 3a73  .0.0"}...ARROW:s
+00000920: 6368 656d 6118 980b 2f2f 2f2f 2f79 6745  chema.../////ygE
+00000930: 4141 4151 4141 4141 4141 414b 4141 3441  AAAQAAAAAAAKAA4A
+00000940: 4267 4146 4141 6741 4367 4141 4141 4142  BgAFAAgACgAAAAAB
+00000950: 4241 4151 4141 4141 4141 414b 4141 7741  BAAQAAAAAAAKAAwA
+00000960: 4141 4145 4141 6741 4367 4141 414e 7743  AAAEAAgACgAAANwC
+00000970: 4141 4145 4141 4141 4151 4141 4141 7741  AAAEAAAAAQAAAAwA
+00000980: 4141 4149 4141 7741 4241 4149 4141 6741  AAAIAAwABAAIAAgA
+00000990: 4141 4149 4141 4141 4541 4141 4141 5941  AAAIAAAAEAAAAAYA
+000009a0: 4141 4277 5957 356b 5958 4d41 414b 6343  AABwYW5kYXMAAKcC
+000009b0: 4141 4237 496d 6c75 5a47 5634 5832 4e76  AAB7ImluZGV4X2Nv
+000009c0: 6248 5674 626e 4d69 4f69 4262 5853 7767  bHVtbnMiOiBbXSwg
+000009d0: 496d 4e76 6248 5674 626c 3970 626d 526c  ImNvbHVtbl9pbmRl
+000009e0: 6547 567a 496a 6f67 5731 3073 4943 4a6a  eGVzIjogW10sICJj
+000009f0: 6232 7831 6257 357a 496a 6f67 5733 7369  b2x1bW5zIjogW3si
+00000a00: 626d 4674 5a53 4936 4943 4a70 5a43 4973  bmFtZSI6ICJpZCIs
+00000a10: 4943 4a6d 6157 5673 5a46 3975 5957 316c  ICJmaWVsZF9uYW1l
+00000a20: 496a 6f67 496d 6c6b 4969 7767 496e 4268  IjogImlkIiwgInBh
+00000a30: 626d 5268 6331 3930 6558 426c 496a 6f67  bmRhc190eXBlIjog
+00000a40: 496d 6c75 6444 5930 4969 7767 496d 3531  ImludDY0IiwgIm51
+00000a50: 6258 4235 5833 5235 6347 5569 4f69 4169  bXB5X3R5cGUiOiAi
+00000a60: 6157 3530 4e6a 5169 4c43 4169 6257 5630  aW50NjQiLCAibWV0
+00000a70: 5957 5268 6447 4569 4f69 4275 6457 7873  YWRhdGEiOiBudWxs
+00000a80: 6653 7767 6579 4a75 5957 316c 496a 6f67  fSwgeyJuYW1lIjog
+00000a90: 496e 4a68 4969 7767 496d 5a70 5a57 786b  InJhIiwgImZpZWxk
+00000aa0: 5832 3568 6257 5569 4f69 4169 636d 4569  X25hbWUiOiAicmEi
+00000ab0: 4c43 4169 6347 4675 5a47 467a 5833 5235  LCAicGFuZGFzX3R5
+00000ac0: 6347 5569 4f69 4169 5a6d 7876 5958 5132  cGUiOiAiZmxvYXQ2
+00000ad0: 4e43 4973 4943 4a75 6457 3177 6556 3930  NCIsICJudW1weV90
+00000ae0: 6558 426c 496a 6f67 496d 5a73 6232 4630  eXBlIjogImZsb2F0
+00000af0: 4e6a 5169 4c43 4169 6257 5630 5957 5268  NjQiLCAibWV0YWRh
+00000b00: 6447 4569 4f69 4275 6457 7873 6653 7767  dGEiOiBudWxsfSwg
+00000b10: 6579 4a75 5957 316c 496a 6f67 496d 526c  eyJuYW1lIjogImRl
+00000b20: 5979 4973 4943 4a6d 6157 5673 5a46 3975  YyIsICJmaWVsZF9u
+00000b30: 5957 316c 496a 6f67 496d 526c 5979 4973  YW1lIjogImRlYyIs
+00000b40: 4943 4a77 5957 356b 5958 4e66 6448 6c77  ICJwYW5kYXNfdHlw
+00000b50: 5a53 4936 4943 4a6d 6247 3968 6444 5930  ZSI6ICJmbG9hdDY0
+00000b60: 4969 7767 496d 3531 6258 4235 5833 5235  IiwgIm51bXB5X3R5
+00000b70: 6347 5569 4f69 4169 5a6d 7876 5958 5132  cGUiOiAiZmxvYXQ2
+00000b80: 4e43 4973 4943 4a74 5a58 5268 5a47 4630  NCIsICJtZXRhZGF0
+00000b90: 5953 4936 4947 3531 6247 7839 4c43 4237  YSI6IG51bGx9LCB7
+00000ba0: 496d 3568 6257 5569 4f69 4169 636d 4666  Im5hbWUiOiAicmFf
+00000bb0: 5a58 4a79 6233 4969 4c43 4169 5a6d 6c6c  ZXJyb3IiLCAiZmll
+00000bc0: 6247 5266 626d 4674 5a53 4936 4943 4a79  bGRfbmFtZSI6ICJy
+00000bd0: 5956 396c 636e 4a76 6369 4973 4943 4a77  YV9lcnJvciIsICJw
+00000be0: 5957 356b 5958 4e66 6448 6c77 5a53 4936  YW5kYXNfdHlwZSI6
+00000bf0: 4943 4a70 626e 5132 4e43 4973 4943 4a75  ICJpbnQ2NCIsICJu
+00000c00: 6457 3177 6556 3930 6558 426c 496a 6f67  dW1weV90eXBlIjog
+00000c10: 496d 6c75 6444 5930 4969 7767 496d 316c  ImludDY0IiwgIm1l
+00000c20: 6447 466b 5958 5268 496a 6f67 626e 5673  dGFkYXRhIjogbnVs
+00000c30: 6248 3073 4948 7369 626d 4674 5a53 4936  bH0sIHsibmFtZSI6
+00000c40: 4943 4a6b 5a57 4e66 5a58 4a79 6233 4969  ICJkZWNfZXJyb3Ii
+00000c50: 4c43 4169 5a6d 6c6c 6247 5266 626d 4674  LCAiZmllbGRfbmFt
+00000c60: 5a53 4936 4943 4a6b 5a57 4e66 5a58 4a79  ZSI6ICJkZWNfZXJy
+00000c70: 6233 4969 4c43 4169 6347 4675 5a47 467a  b3IiLCAicGFuZGFz
+00000c80: 5833 5235 6347 5569 4f69 4169 6157 3530  X3R5cGUiOiAiaW50
+00000c90: 4e6a 5169 4c43 4169 626e 5674 6348 6c66  NjQiLCAibnVtcHlf
+00000ca0: 6448 6c77 5a53 4936 4943 4a70 626e 5132  dHlwZSI6ICJpbnQ2
+00000cb0: 4e43 4973 4943 4a74 5a58 5268 5a47 4630  NCIsICJtZXRhZGF0
+00000cc0: 5953 4936 4947 3531 6247 7839 5853 7767  YSI6IG51bGx9XSwg
+00000cd0: 496d 4e79 5a57 4630 6233 4969 4f69 4237  ImNyZWF0b3IiOiB7
+00000ce0: 496d 7870 596e 4a68 636e 6b69 4f69 4169  ImxpYnJhcnkiOiAi
+00000cf0: 6348 6c68 636e 4a76 6479 4973 4943 4a32  cHlhcnJvdyIsICJ2
+00000d00: 5a58 4a7a 6157 3975 496a 6f67 496a 6b75  ZXJzaW9uIjogIjku
+00000d10: 4d43 3477 496e 3073 4943 4a77 5957 356b  MC4wIn0sICJwYW5k
+00000d20: 5958 4e66 646d 5679 6332 6c76 6269 4936  YXNfdmVyc2lvbiI6
+00000d30: 4943 4979 4c6a 4175 4d43 4a39 4141 5541  ICIyLjAuMCJ9AAUA
+00000d40: 4141 446b 4141 4141 6f41 4141 4148 5141  AADkAAAAoAAAAHQA
+00000d50: 4141 4138 4141 4141 4241 4141 4145 442f  AAA8AAAABAAAAED/
+00000d60: 2f2f 3841 4141 4543 4541 4141 4142 7741  //8AAAECEAAAABwA
+00000d70: 4141 4145 4141 4141 4141 4141 4141 6b41  AAAEAAAAAAAAAAkA
+00000d80: 4141 426b 5a57 4e66 5a58 4a79 6233 4941  AABkZWNfZXJyb3IA
+00000d90: 4141 4134 2f2f 2f2f 4141 4141 4155 4141  AAA4////AAAAAUAA
+00000da0: 4141 4230 2f2f 2f2f 4141 4142 4168 4141  AAB0////AAABAhAA
+00000db0: 4141 4163 4141 4141 4241 4141 4141 4141  AAAcAAAABAAAAAAA
+00000dc0: 4141 4149 4141 4141 636d 4666 5a58 4a79  AAAIAAAAcmFfZXJy
+00000dd0: 6233 4941 4141 4141 6250 2f2f 2f77 4141  b3IAAAAAbP///wAA
+00000de0: 4141 4641 4141 4141 7150 2f2f 2f77 4141  AAFAAAAAqP///wAA
+00000df0: 4151 4d51 4141 4141 4641 4141 4141 5141  AQMQAAAAFAAAAAQA
+00000e00: 4141 4141 4141 4141 4177 4141 4147 526c  AAAAAAAAAwAAAGRl
+00000e10: 5977 4457 2f2f 2f2f 4141 4143 414e 442f  YwDW////AAACAND/
+00000e20: 2f2f 3841 4141 4544 4541 4141 4142 7741  //8AAAEDEAAAABwA
+00000e30: 4141 4145 4141 4141 4141 4141 4141 4941  AAAEAAAAAAAAAAIA
+00000e40: 4141 4279 5951 4141 4141 4147 4141 6741  AAByYQAAAAAGAAgA
+00000e50: 4267 4147 4141 4141 4141 4143 4142 4141  BgAGAAAAAAACABAA
+00000e60: 4641 4149 4141 5941 4277 414d 4141 4141  FAAIAAYABwAMAAAA
+00000e70: 4541 4151 4141 4141 4141 4142 4168 4141  EAAQAAAAAAABAhAA
+00000e80: 4141 4163 4141 4141 4241 4141 4141 4141  AAAcAAAABAAAAAAA
+00000e90: 4141 4143 4141 4141 6157 5141 4141 6741  AAACAAAAaWQAAAgA
+00000ea0: 4441 4149 4141 6341 4341 4141 4141 4141  DAAIAAcACAAAAAAA
+00000eb0: 4141 4641 4141 4141 4141 4141 4141 3d3d  AAFAAAAAAAAAAA==
+00000ec0: 0018 1f70 6172 7175 6574 2d63 7070 2d61  ...parquet-cpp-a
+00000ed0: 7272 6f77 2076 6572 7369 6f6e 2039 2e30  rrow version 9.0
+00000ee0: 2e30 195c 1c00 001c 0000 1c00 001c 0000  .0.\............
+00000ef0: 1c00 0000 d30a 0000 5041 5231            ........PAR1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_45/shard_1.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet`

 * *Files 16% similar despite different names*

```diff
@@ -1,306 +1,241 @@
-00000000: 5041 5231 1504 1570 1550 4c15 0e15 0012  PAR1...p.PL.....
-00000010: 0000 3808 c002 0005 0100 c10d 0800 c60d  ..8.............
-00000020: 0800 cf0d 0800 d00d 083c d202 0000 0000  .........<......
-00000030: 0000 d402 0000 0000 0000 1500 1516 151a  ................
-00000040: 2c15 0e15 1015 0615 061c 1808 d402 0000  ,...............
-00000050: 0000 0000 1808 c002 0000 0000 0000 1600  ................
-00000060: 2808 d402 0000 0000 0000 1808 c002 0000  (...............
-00000070: 0000 0000 0000 000b 2802 0000 000e 0103  ........(.......
-00000080: 0388 c61a 2688 021c 1504 1935 1000 0619  ....&......5....
-00000090: 1802 6964 1502 160e 169c 0216 8002 2674  ..id..........&t
-000000a0: 2608 1c18 08d4 0200 0000 0000 0018 08c0  &...............
-000000b0: 0200 0000 0000 0016 0028 08d4 0200 0000  .........(......
-000000c0: 0000 0018 08c0 0200 0000 0000 0000 192c  ...............,
-000000d0: 1504 1500 1502 0015 0015 1015 0200 0000  ................
-000000e0: 1504 1560 154a 4c15 0c15 0012 0000 3000  ...`.JL.......0.
-000000f0: 0001 0108 6874 4001 0704 00f8 0d08 0458  ....ht@........X
-00000100: 7509 1000 880d 0828 e875 4000 0000 0000  u......(.u@.....
-00000110: 3874 4015 0015 1615 1a2c 150e 1510 1506  8t@......,......
-00000120: 1506 1c18 0800 0000 0000 e875 4018 0800  ...........u@...
-00000130: 0000 0000 3874 4016 0028 0800 0000 0000  ....8t@..(......
-00000140: e875 4018 0800 0000 0000 3874 4000 0000  .u@.......8t@...
-00000150: 0b28 0200 0000 0e01 0303 8836 1626 ba05  .(.........6.&..
-00000160: 1c15 0a19 3510 0006 1918 0272 6115 0216  ....5......ra...
-00000170: 0e16 8c02 16fa 0126 a604 26c0 031c 1808  .......&..&.....
-00000180: 0000 0000 00e8 7540 1808 0000 0000 0038  ......u@.......8
-00000190: 7440 1600 2808 0000 0000 00e8 7540 1808  t@..(.......u@..
-000001a0: 0000 0000 0038 7440 0019 2c15 0415 0015  .....8t@..,.....
-000001b0: 0200 1500 1510 1502 0000 0015 0415 6015  ..............`.
-000001c0: 4c4c 150c 1500 1200 0030 0000 0101 08c0  LL.......0......
-000001d0: 46c0 0107 0800 4040 0908 04c0 430d 0800  F.....@@....C...
-000001e0: 4709 0828 404d c000 0000 0000 c044 c015  G..(@M.......D..
-000001f0: 0015 1615 1a2c 150e 1510 1506 1506 1c18  .....,..........
-00000200: 0800 0000 0000 4040 c018 0800 0000 0000  ......@@........
-00000210: 404d c016 0028 0800 0000 0000 4040 c018  @M...(......@@..
-00000220: 0800 0000 0000 404d c000 0000 0b28 0200  ......@M.....(..
-00000230: 0000 0e01 0303 8834 1626 f208 1c15 0a19  .......4.&......
-00000240: 3510 0006 1918 0364 6563 1502 160e 168c  5......dec......
-00000250: 0216 fc01 26de 0726 f606 1c18 0800 0000  ....&..&........
-00000260: 0000 4040 c018 0800 0000 0000 404d c016  ..@@........@M..
-00000270: 0028 0800 0000 0000 4040 c018 0800 0000  .(......@@......
-00000280: 0000 404d c000 192c 1504 1500 1502 0015  ..@M...,........
-00000290: 0015 1015 0200 0000 1504 1510 1514 4c15  ..............L.
-000002a0: 0215 0012 0000 081c 0000 0000 0000 0000  ................
-000002b0: 1500 1512 1516 2c15 0e15 1015 0615 061c  ......,.........
-000002c0: 1808 0000 0000 0000 0000 1808 0000 0000  ................
-000002d0: 0000 0000 1600 2808 0000 0000 0000 0000  ......(.........
-000002e0: 1808 0000 0000 0000 0000 0000 0009 2002  .............. .
-000002f0: 0000 000e 0101 0e00 26f0 0b1c 1504 1935  ........&......5
-00000300: 1000 0619 1808 7261 5f65 7272 6f72 1502  ......ra_error..
-00000310: 160e 16b8 0116 c001 26e0 0a26 b00a 1c18  ........&..&....
-00000320: 0800 0000 0000 0000 0018 0800 0000 0000  ................
-00000330: 0000 0016 0028 0800 0000 0000 0000 0018  .....(..........
-00000340: 0800 0000 0000 0000 0000 192c 1504 1500  ...........,....
-00000350: 1502 0015 0015 1015 0200 0000 1504 1510  ................
-00000360: 1514 4c15 0215 0012 0000 081c 0000 0000  ..L.............
-00000370: 0000 0000 1500 1512 1516 2c15 0e15 1015  ..........,.....
-00000380: 0615 061c 1808 0000 0000 0000 0000 1808  ................
-00000390: 0000 0000 0000 0000 1600 2808 0000 0000  ..........(.....
-000003a0: 0000 0000 1808 0000 0000 0000 0000 0000  ................
-000003b0: 0009 2002 0000 000e 0101 0e00 26f8 0e1c  .. .........&...
-000003c0: 1504 1935 1000 0619 1809 6465 635f 6572  ...5......dec_er
-000003d0: 726f 7215 0216 0e16 b801 16c0 0126 e80d  ror..........&..
-000003e0: 26b8 0d1c 1808 0000 0000 0000 0000 1808  &...............
-000003f0: 0000 0000 0000 0000 1600 2808 0000 0000  ..........(.....
-00000400: 0000 0000 1808 0000 0000 0000 0000 0019  ................
-00000410: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
-00000420: 0015 0415 7015 504c 150e 1500 1200 0038  ....p.PL.......8
-00000430: 0404 0009 0100 0509 0704 000a 0d08 0013  ................
-00000440: 0d08 0014 0d08 3c16 0000 0000 0000 0018  ......<.........
-00000450: 0000 0000 0000 0015 0015 1615 1a2c 150e  .............,..
-00000460: 1510 1506 1506 1c18 0818 0000 0000 0000  ................
-00000470: 0018 0804 0000 0000 0000 0016 0028 0818  .............(..
-00000480: 0000 0000 0000 0018 0804 0000 0000 0000  ................
-00000490: 0000 0000 0b28 0200 0000 0e01 0303 88c6  .....(..........
-000004a0: 1a26 c212 1c15 0419 3510 0006 1918 115f  .&......5......_
-000004b0: 5f69 6e64 6578 5f6c 6576 656c 5f30 5f5f  _index_level_0__
-000004c0: 1502 160e 169c 0216 8002 26ae 1126 c210  ..........&..&..
-000004d0: 1c18 0818 0000 0000 0000 0018 0804 0000  ................
-000004e0: 0000 0000 0016 0028 0818 0000 0000 0000  .......(........
-000004f0: 0018 0804 0000 0000 0000 0000 192c 1504  .............,..
-00000500: 1500 1502 0015 0015 1015 0200 0000 1504  ................
-00000510: 197c 3500 1806 7363 6865 6d61 150c 0015  .|5...schema....
-00000520: 0425 0218 0269 6400 150a 2502 1802 7261  .%...id...%...ra
-00000530: 0015 0a25 0218 0364 6563 0015 0425 0218  ...%...dec...%..
-00000540: 0872 615f 6572 726f 7200 1504 2502 1809  .ra_error...%...
-00000550: 6465 635f 6572 726f 7200 1504 2502 1811  dec_error...%...
-00000560: 5f5f 696e 6465 785f 6c65 7665 6c5f 305f  __index_level_0_
-00000570: 5f00 160e 191c 196c 2688 021c 1504 1935  _......l&......5
-00000580: 1000 0619 1802 6964 1502 160e 169c 0216  ......id........
-00000590: 8002 2674 2608 1c18 08d4 0200 0000 0000  ..&t&...........
-000005a0: 0018 08c0 0200 0000 0000 0016 0028 08d4  .............(..
-000005b0: 0200 0000 0000 0018 08c0 0200 0000 0000  ................
-000005c0: 0000 192c 1504 1500 1502 0015 0015 1015  ...,............
-000005d0: 0200 0000 26ba 051c 150a 1935 1000 0619  ....&......5....
-000005e0: 1802 7261 1502 160e 168c 0216 fa01 26a6  ..ra..........&.
-000005f0: 0426 c003 1c18 0800 0000 0000 e875 4018  .&...........u@.
-00000600: 0800 0000 0000 3874 4016 0028 0800 0000  ......8t@..(....
-00000610: 0000 e875 4018 0800 0000 0000 3874 4000  ...u@.......8t@.
-00000620: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
-00000630: 0000 26f2 081c 150a 1935 1000 0619 1803  ..&......5......
-00000640: 6465 6315 0216 0e16 8c02 16fc 0126 de07  dec..........&..
-00000650: 26f6 061c 1808 0000 0000 0040 40c0 1808  &..........@@...
-00000660: 0000 0000 0040 4dc0 1600 2808 0000 0000  .....@M...(.....
-00000670: 0040 40c0 1808 0000 0000 0040 4dc0 0019  .@@........@M...
-00000680: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
-00000690: 0026 f00b 1c15 0419 3510 0006 1918 0872  .&......5......r
-000006a0: 615f 6572 726f 7215 0216 0e16 b801 16c0  a_error.........
-000006b0: 0126 e00a 26b0 0a1c 1808 0000 0000 0000  .&..&...........
-000006c0: 0000 1808 0000 0000 0000 0000 1600 2808  ..............(.
-000006d0: 0000 0000 0000 0000 1808 0000 0000 0000  ................
-000006e0: 0000 0019 2c15 0415 0015 0200 1500 1510  ....,...........
-000006f0: 1502 0000 0026 f80e 1c15 0419 3510 0006  .....&......5...
-00000700: 1918 0964 6563 5f65 7272 6f72 1502 160e  ...dec_error....
-00000710: 16b8 0116 c001 26e8 0d26 b80d 1c18 0800  ......&..&......
-00000720: 0000 0000 0000 0018 0800 0000 0000 0000  ................
-00000730: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
-00000740: 0000 0000 0000 0000 192c 1504 1500 1502  .........,......
-00000750: 0015 0015 1015 0200 0000 26c2 121c 1504  ..........&.....
-00000760: 1935 1000 0619 1811 5f5f 696e 6465 785f  .5......__index_
-00000770: 6c65 7665 6c5f 305f 5f15 0216 0e16 9c02  level_0__.......
-00000780: 1680 0226 ae11 26c2 101c 1808 1800 0000  ...&..&.........
-00000790: 0000 0000 1808 0400 0000 0000 0000 1600  ................
-000007a0: 2808 1800 0000 0000 0000 1808 0400 0000  (...............
-000007b0: 0000 0000 0019 2c15 0415 0015 0200 1500  ......,.........
-000007c0: 1510 1502 0000 0016 c00b 160e 2608 16f6  ............&...
-000007d0: 0a14 0000 192c 1806 7061 6e64 6173 18a5  .....,..pandas..
-000007e0: 077b 2269 6e64 6578 5f63 6f6c 756d 6e73  .{"index_columns
-000007f0: 223a 205b 225f 5f69 6e64 6578 5f6c 6576  ": ["__index_lev
-00000800: 656c 5f30 5f5f 225d 2c20 2263 6f6c 756d  el_0__"], "colum
-00000810: 6e5f 696e 6465 7865 7322 3a20 5b7b 226e  n_indexes": [{"n
-00000820: 616d 6522 3a20 6e75 6c6c 2c20 2266 6965  ame": null, "fie
-00000830: 6c64 5f6e 616d 6522 3a20 6e75 6c6c 2c20  ld_name": null, 
-00000840: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
-00000850: 756e 6963 6f64 6522 2c20 226e 756d 7079  unicode", "numpy
-00000860: 5f74 7970 6522 3a20 226f 626a 6563 7422  _type": "object"
-00000870: 2c20 226d 6574 6164 6174 6122 3a20 7b22  , "metadata": {"
-00000880: 656e 636f 6469 6e67 223a 2022 5554 462d  encoding": "UTF-
-00000890: 3822 7d7d 5d2c 2022 636f 6c75 6d6e 7322  8"}}], "columns"
-000008a0: 3a20 5b7b 226e 616d 6522 3a20 2269 6422  : [{"name": "id"
-000008b0: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
-000008c0: 2269 6422 2c20 2270 616e 6461 735f 7479  "id", "pandas_ty
-000008d0: 7065 223a 2022 696e 7436 3422 2c20 226e  pe": "int64", "n
-000008e0: 756d 7079 5f74 7970 6522 3a20 2269 6e74  umpy_type": "int
-000008f0: 3634 222c 2022 6d65 7461 6461 7461 223a  64", "metadata":
-00000900: 206e 756c 6c7d 2c20 7b22 6e61 6d65 223a   null}, {"name":
-00000910: 2022 7261 222c 2022 6669 656c 645f 6e61   "ra", "field_na
-00000920: 6d65 223a 2022 7261 222c 2022 7061 6e64  me": "ra", "pand
-00000930: 6173 5f74 7970 6522 3a20 2266 6c6f 6174  as_type": "float
-00000940: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
-00000950: 223a 2022 666c 6f61 7436 3422 2c20 226d  ": "float64", "m
-00000960: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
-00000970: 207b 226e 616d 6522 3a20 2264 6563 222c   {"name": "dec",
-00000980: 2022 6669 656c 645f 6e61 6d65 223a 2022   "field_name": "
-00000990: 6465 6322 2c20 2270 616e 6461 735f 7479  dec", "pandas_ty
-000009a0: 7065 223a 2022 666c 6f61 7436 3422 2c20  pe": "float64", 
-000009b0: 226e 756d 7079 5f74 7970 6522 3a20 2266  "numpy_type": "f
-000009c0: 6c6f 6174 3634 222c 2022 6d65 7461 6461  loat64", "metada
-000009d0: 7461 223a 206e 756c 6c7d 2c20 7b22 6e61  ta": null}, {"na
-000009e0: 6d65 223a 2022 7261 5f65 7272 6f72 222c  me": "ra_error",
-000009f0: 2022 6669 656c 645f 6e61 6d65 223a 2022   "field_name": "
-00000a00: 7261 5f65 7272 6f72 222c 2022 7061 6e64  ra_error", "pand
-00000a10: 6173 5f74 7970 6522 3a20 2269 6e74 3634  as_type": "int64
-00000a20: 222c 2022 6e75 6d70 795f 7479 7065 223a  ", "numpy_type":
-00000a30: 2022 696e 7436 3422 2c20 226d 6574 6164   "int64", "metad
-00000a40: 6174 6122 3a20 6e75 6c6c 7d2c 207b 226e  ata": null}, {"n
-00000a50: 616d 6522 3a20 2264 6563 5f65 7272 6f72  ame": "dec_error
-00000a60: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
-00000a70: 2022 6465 635f 6572 726f 7222 2c20 2270   "dec_error", "p
-00000a80: 616e 6461 735f 7479 7065 223a 2022 696e  andas_type": "in
-00000a90: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
-00000aa0: 6522 3a20 2269 6e74 3634 222c 2022 6d65  e": "int64", "me
-00000ab0: 7461 6461 7461 223a 206e 756c 6c7d 2c20  tadata": null}, 
-00000ac0: 7b22 6e61 6d65 223a 206e 756c 6c2c 2022  {"name": null, "
-00000ad0: 6669 656c 645f 6e61 6d65 223a 2022 5f5f  field_name": "__
-00000ae0: 696e 6465 785f 6c65 7665 6c5f 305f 5f22  index_level_0__"
-00000af0: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
-00000b00: 2022 696e 7436 3422 2c20 226e 756d 7079   "int64", "numpy
-00000b10: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
-00000b20: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
-00000b30: 6c7d 5d2c 2022 6372 6561 746f 7222 3a20  l}], "creator": 
-00000b40: 7b22 6c69 6272 6172 7922 3a20 2270 7961  {"library": "pya
-00000b50: 7272 6f77 222c 2022 7665 7273 696f 6e22  rrow", "version"
-00000b60: 3a20 2239 2e30 2e30 227d 2c20 2270 616e  : "9.0.0"}, "pan
-00000b70: 6461 735f 7665 7273 696f 6e22 3a20 2231  das_version": "1
-00000b80: 2e33 2e35 227d 0018 0c41 5252 4f57 3a73  .3.5"}...ARROW:s
-00000b90: 6368 656d 6118 c00e 2f2f 2f2f 2f32 6746  chema.../////2gF
-00000ba0: 4141 4151 4141 4141 4141 414b 4141 3441  AAAQAAAAAAAKAA4A
-00000bb0: 4267 4146 4141 6741 4367 4141 4141 4142  BgAFAAgACgAAAAAB
-00000bc0: 4241 4151 4141 4141 4141 414b 4141 7741  BAAQAAAAAAAKAAwA
-00000bd0: 4141 4145 4141 6741 4367 4141 414e 7744  AAAEAAgACgAAANwD
-00000be0: 4141 4145 4141 4141 4151 4141 4141 7741  AAAEAAAAAQAAAAwA
-00000bf0: 4141 4149 4141 7741 4241 4149 4141 6741  AAAIAAwABAAIAAgA
-00000c00: 4141 4149 4141 4141 4541 4141 4141 5941  AAAIAAAAEAAAAAYA
-00000c10: 4141 4277 5957 356b 5958 4d41 414b 5544  AABwYW5kYXMAAKUD
-00000c20: 4141 4237 496d 6c75 5a47 5634 5832 4e76  AAB7ImluZGV4X2Nv
-00000c30: 6248 5674 626e 4d69 4f69 4262 496c 3966  bHVtbnMiOiBbIl9f
-00000c40: 6157 356b 5a58 6866 6247 5632 5a57 7866  aW5kZXhfbGV2ZWxf
-00000c50: 4d46 3966 496c 3073 4943 4a6a 6232 7831  MF9fIl0sICJjb2x1
-00000c60: 6257 3566 6157 356b 5a58 686c 6379 4936  bW5faW5kZXhlcyI6
-00000c70: 4946 7437 496d 3568 6257 5569 4f69 4275  IFt7Im5hbWUiOiBu
-00000c80: 6457 7873 4c43 4169 5a6d 6c6c 6247 5266  dWxsLCAiZmllbGRf
-00000c90: 626d 4674 5a53 4936 4947 3531 6247 7773  bmFtZSI6IG51bGws
-00000ca0: 4943 4a77 5957 356b 5958 4e66 6448 6c77  ICJwYW5kYXNfdHlw
-00000cb0: 5a53 4936 4943 4a31 626d 6c6a 6232 526c  ZSI6ICJ1bmljb2Rl
-00000cc0: 4969 7767 496d 3531 6258 4235 5833 5235  IiwgIm51bXB5X3R5
-00000cd0: 6347 5569 4f69 4169 6232 4a71 5a57 4e30  cGUiOiAib2JqZWN0
-00000ce0: 4969 7767 496d 316c 6447 466b 5958 5268  IiwgIm1ldGFkYXRh
-00000cf0: 496a 6f67 6579 4a6c 626d 4e76 5a47 6c75  IjogeyJlbmNvZGlu
-00000d00: 5a79 4936 4943 4a56 5645 5974 4f43 4a39  ZyI6ICJVVEYtOCJ9
-00000d10: 6656 3073 4943 4a6a 6232 7831 6257 357a  fV0sICJjb2x1bW5z
-00000d20: 496a 6f67 5733 7369 626d 4674 5a53 4936  IjogW3sibmFtZSI6
-00000d30: 4943 4a70 5a43 4973 4943 4a6d 6157 5673  ICJpZCIsICJmaWVs
-00000d40: 5a46 3975 5957 316c 496a 6f67 496d 6c6b  ZF9uYW1lIjogImlk
-00000d50: 4969 7767 496e 4268 626d 5268 6331 3930  IiwgInBhbmRhc190
-00000d60: 6558 426c 496a 6f67 496d 6c75 6444 5930  eXBlIjogImludDY0
-00000d70: 4969 7767 496d 3531 6258 4235 5833 5235  IiwgIm51bXB5X3R5
-00000d80: 6347 5569 4f69 4169 6157 3530 4e6a 5169  cGUiOiAiaW50NjQi
-00000d90: 4c43 4169 6257 5630 5957 5268 6447 4569  LCAibWV0YWRhdGEi
-00000da0: 4f69 4275 6457 7873 6653 7767 6579 4a75  OiBudWxsfSwgeyJu
-00000db0: 5957 316c 496a 6f67 496e 4a68 4969 7767  YW1lIjogInJhIiwg
-00000dc0: 496d 5a70 5a57 786b 5832 3568 6257 5569  ImZpZWxkX25hbWUi
-00000dd0: 4f69 4169 636d 4569 4c43 4169 6347 4675  OiAicmEiLCAicGFu
-00000de0: 5a47 467a 5833 5235 6347 5569 4f69 4169  ZGFzX3R5cGUiOiAi
-00000df0: 5a6d 7876 5958 5132 4e43 4973 4943 4a75  ZmxvYXQ2NCIsICJu
-00000e00: 6457 3177 6556 3930 6558 426c 496a 6f67  dW1weV90eXBlIjog
-00000e10: 496d 5a73 6232 4630 4e6a 5169 4c43 4169  ImZsb2F0NjQiLCAi
-00000e20: 6257 5630 5957 5268 6447 4569 4f69 4275  bWV0YWRhdGEiOiBu
-00000e30: 6457 7873 6653 7767 6579 4a75 5957 316c  dWxsfSwgeyJuYW1l
-00000e40: 496a 6f67 496d 526c 5979 4973 4943 4a6d  IjogImRlYyIsICJm
-00000e50: 6157 5673 5a46 3975 5957 316c 496a 6f67  aWVsZF9uYW1lIjog
-00000e60: 496d 526c 5979 4973 4943 4a77 5957 356b  ImRlYyIsICJwYW5k
-00000e70: 5958 4e66 6448 6c77 5a53 4936 4943 4a6d  YXNfdHlwZSI6ICJm
-00000e80: 6247 3968 6444 5930 4969 7767 496d 3531  bG9hdDY0IiwgIm51
-00000e90: 6258 4235 5833 5235 6347 5569 4f69 4169  bXB5X3R5cGUiOiAi
-00000ea0: 5a6d 7876 5958 5132 4e43 4973 4943 4a74  ZmxvYXQ2NCIsICJt
-00000eb0: 5a58 5268 5a47 4630 5953 4936 4947 3531  ZXRhZGF0YSI6IG51
-00000ec0: 6247 7839 4c43 4237 496d 3568 6257 5569  bGx9LCB7Im5hbWUi
-00000ed0: 4f69 4169 636d 4666 5a58 4a79 6233 4969  OiAicmFfZXJyb3Ii
-00000ee0: 4c43 4169 5a6d 6c6c 6247 5266 626d 4674  LCAiZmllbGRfbmFt
-00000ef0: 5a53 4936 4943 4a79 5956 396c 636e 4a76  ZSI6ICJyYV9lcnJv
-00000f00: 6369 4973 4943 4a77 5957 356b 5958 4e66  ciIsICJwYW5kYXNf
-00000f10: 6448 6c77 5a53 4936 4943 4a70 626e 5132  dHlwZSI6ICJpbnQ2
-00000f20: 4e43 4973 4943 4a75 6457 3177 6556 3930  NCIsICJudW1weV90
-00000f30: 6558 426c 496a 6f67 496d 6c75 6444 5930  eXBlIjogImludDY0
-00000f40: 4969 7767 496d 316c 6447 466b 5958 5268  IiwgIm1ldGFkYXRh
-00000f50: 496a 6f67 626e 5673 6248 3073 4948 7369  IjogbnVsbH0sIHsi
-00000f60: 626d 4674 5a53 4936 4943 4a6b 5a57 4e66  bmFtZSI6ICJkZWNf
-00000f70: 5a58 4a79 6233 4969 4c43 4169 5a6d 6c6c  ZXJyb3IiLCAiZmll
-00000f80: 6247 5266 626d 4674 5a53 4936 4943 4a6b  bGRfbmFtZSI6ICJk
-00000f90: 5a57 4e66 5a58 4a79 6233 4969 4c43 4169  ZWNfZXJyb3IiLCAi
-00000fa0: 6347 4675 5a47 467a 5833 5235 6347 5569  cGFuZGFzX3R5cGUi
-00000fb0: 4f69 4169 6157 3530 4e6a 5169 4c43 4169  OiAiaW50NjQiLCAi
-00000fc0: 626e 5674 6348 6c66 6448 6c77 5a53 4936  bnVtcHlfdHlwZSI6
-00000fd0: 4943 4a70 626e 5132 4e43 4973 4943 4a74  ICJpbnQ2NCIsICJt
-00000fe0: 5a58 5268 5a47 4630 5953 4936 4947 3531  ZXRhZGF0YSI6IG51
-00000ff0: 6247 7839 4c43 4237 496d 3568 6257 5569  bGx9LCB7Im5hbWUi
-00001000: 4f69 4275 6457 7873 4c43 4169 5a6d 6c6c  OiBudWxsLCAiZmll
-00001010: 6247 5266 626d 4674 5a53 4936 4943 4a66  bGRfbmFtZSI6ICJf
-00001020: 5832 6c75 5a47 5634 5832 786c 646d 5673  X2luZGV4X2xldmVs
-00001030: 587a 4266 5879 4973 4943 4a77 5957 356b  XzBfXyIsICJwYW5k
-00001040: 5958 4e66 6448 6c77 5a53 4936 4943 4a70  YXNfdHlwZSI6ICJp
-00001050: 626e 5132 4e43 4973 4943 4a75 6457 3177  bnQ2NCIsICJudW1w
-00001060: 6556 3930 6558 426c 496a 6f67 496d 6c75  eV90eXBlIjogImlu
-00001070: 6444 5930 4969 7767 496d 316c 6447 466b  dDY0IiwgIm1ldGFk
-00001080: 5958 5268 496a 6f67 626e 5673 6248 3164  YXRhIjogbnVsbH1d
-00001090: 4c43 4169 5933 4a6c 5958 5276 6369 4936  LCAiY3JlYXRvciI6
-000010a0: 4948 7369 6247 6c69 636d 4679 6553 4936  IHsibGlicmFyeSI6
-000010b0: 4943 4a77 6557 4679 636d 3933 4969 7767  ICJweWFycm93Iiwg
-000010c0: 496e 5a6c 636e 4e70 6232 3469 4f69 4169  InZlcnNpb24iOiAi
-000010d0: 4f53 3477 4c6a 4169 6653 7767 496e 4268  OS4wLjAifSwgInBh
-000010e0: 626d 5268 6331 3932 5a58 4a7a 6157 3975  bmRhc192ZXJzaW9u
-000010f0: 496a 6f67 496a 4575 4d79 3431 496e 3041  IjogIjEuMy41In0A
-00001100: 4141 4147 4141 4141 4a41 4541 414f 4141  AAAGAAAAJAEAAOAA
-00001110: 4141 4330 4141 4141 6641 4141 4145 5141  AAC0AAAAfAAAAEQA
-00001120: 4141 4145 4141 4141 4250 2f2f 2f77 4141  AAAEAAAABP///wAA
-00001130: 4151 4951 4141 4141 4a41 4141 4141 5141  AQIQAAAAJAAAAAQA
-00001140: 4141 4141 4141 4141 4551 4141 4146 3966  AAAAAAAAEQAAAF9f
-00001150: 6157 356b 5a58 6866 6247 5632 5a57 7866  aW5kZXhfbGV2ZWxf
-00001160: 4d46 3966 4141 4141 4250 2f2f 2f77 4141  MF9fAAAABP///wAA
-00001170: 4141 4641 4141 4141 5150 2f2f 2f77 4141  AAFAAAAAQP///wAA
-00001180: 4151 4951 4141 4141 4841 4141 4141 5141  AQIQAAAAHAAAAAQA
-00001190: 4141 4141 4141 4141 4351 4141 4147 526c  AAAAAAAACQAAAGRl
-000011a0: 5931 396c 636e 4a76 6367 4141 4144 6a2f  Y19lcnJvcgAAADj/
-000011b0: 2f2f 3841 4141 4142 5141 4141 4148 542f  //8AAAABQAAAAHT/
-000011c0: 2f2f 3841 4141 4543 4541 4141 4142 7741  //8AAAECEAAAABwA
-000011d0: 4141 4145 4141 4141 4141 4141 4141 6741  AAAEAAAAAAAAAAgA
-000011e0: 4141 4279 5956 396c 636e 4a76 6367 4141  AAByYV9lcnJvcgAA
-000011f0: 4141 4273 2f2f 2f2f 4141 4141 4155 4141  AABs////AAAAAUAA
-00001200: 4141 436f 2f2f 2f2f 4141 4142 4178 4141  AACo////AAABAxAA
-00001210: 4141 4155 4141 4141 4241 4141 4141 4141  AAAUAAAABAAAAAAA
-00001220: 4141 4144 4141 4141 5a47 566a 414e 622f  AAADAAAAZGVjANb/
-00001230: 2f2f 3841 4141 4941 3050 2f2f 2f77 4141  //8AAAIA0P///wAA
-00001240: 4151 4d51 4141 4141 4841 4141 4141 5141  AQMQAAAAHAAAAAQA
-00001250: 4141 4141 4141 4141 4167 4141 4148 4a68  AAAAAAAAAgAAAHJh
-00001260: 4141 4141 4141 5941 4341 4147 4141 5941  AAAAAAYACAAGAAYA
-00001270: 4141 4141 4141 4941 4541 4155 4141 6741  AAAAAAIAEAAUAAgA
-00001280: 4267 4148 4141 7741 4141 4151 4142 4141  BgAHAAwAAAAQABAA
-00001290: 4141 4141 4141 4543 4541 4141 4142 7741  AAAAAAECEAAAABwA
-000012a0: 4141 4145 4141 4141 4141 4141 4141 4941  AAAEAAAAAAAAAAIA
-000012b0: 4141 4270 5a41 4141 4341 414d 4141 6741  AABpZAAACAAMAAgA
-000012c0: 4277 4149 4141 4141 4141 4141 4155 4141  BwAIAAAAAAAAAUAA
-000012d0: 4141 4141 4141 4141 0018 1f70 6172 7175  AAAAAAAA...parqu
-000012e0: 6574 2d63 7070 2d61 7272 6f77 2076 6572  et-cpp-arrow ver
-000012f0: 7369 6f6e 2039 2e30 2e30 196c 1c00 001c  sion 9.0.0.l....
-00001300: 0000 1c00 001c 0000 1c00 001c 0000 0001  ................
-00001310: 0e00 0050 4152 31                        ...PAR1
+00000000: 5041 5231 1504 1580 0115 5c4c 1510 1500  PAR1......\L....
+00000010: 1200 0040 08f6 0200 0501 00f8 0d08 00fe  ...@............
+00000020: 0d08 0400 0305 1704 0003 0d08 0004 0d08  ................
+00000030: 3c07 0300 0000 0000 0008 0300 0000 0000  <...............
+00000040: 0015 0015 1615 1a2c 1510 1510 1506 1506  .......,........
+00000050: 1c18 0808 0300 0000 0000 0018 08f6 0200  ................
+00000060: 0000 0000 0016 0028 0808 0300 0000 0000  .......(........
+00000070: 0018 08f6 0200 0000 0000 0000 0000 0b28  ...............(
+00000080: 0200 0000 1001 0303 88c6 fa26 9602 1c15  ...........&....
+00000090: 0419 3510 0006 1918 0269 6415 0216 1016  ..5......id.....
+000000a0: ae02 168e 0226 8201 2608 1c18 0808 0300  .....&..&.......
+000000b0: 0000 0000 0018 08f6 0200 0000 0000 0016  ................
+000000c0: 0028 0808 0300 0000 0000 0018 08f6 0200  .(..............
+000000d0: 0000 0000 0000 192c 1504 1500 1502 0015  .......,........
+000000e0: 0015 1015 0200 0000 1504 1570 1556 4c15  ...........p.VL.
+000000f0: 0e15 0012 0000 3800 0001 0108 5874 4001  ......8.....Xt@.
+00000100: 0704 0008 0d08 0468 7309 1004 9872 0908  .......hs....r..
+00000110: 04c8 7509 0828 1874 4000 0000 0000 8875  ..u..(.t@......u
+00000120: 4015 0015 1615 1a2c 1510 1510 1506 1506  @......,........
+00000130: 1c18 0800 0000 0000 c875 4018 0800 0000  .........u@.....
+00000140: 0000 9872 4016 0028 0800 0000 0000 c875  ...r@..(.......u
+00000150: 4018 0800 0000 0000 9872 4000 0000 0b28  @........r@....(
+00000160: 0200 0000 1001 0303 8846 d626 d605 1c15  .........F.&....
+00000170: 0a19 3510 0006 1918 0272 6115 0216 1016  ..5......ra.....
+00000180: 9c02 1686 0226 c204 26d0 031c 1808 0000  .....&..&.......
+00000190: 0000 00c8 7540 1808 0000 0000 0098 7240  ....u@........r@
+000001a0: 1600 2808 0000 0000 00c8 7540 1808 0000  ..(.......u@....
+000001b0: 0000 0098 7240 0019 2c15 0415 0015 0200  ....r@..,.......
+000001c0: 1500 1510 1502 0000 0015 0415 6015 4e4c  ............`.NL
+000001d0: 150c 1500 1200 0030 0000 0101 08c0 4ac0  .......0......J.
+000001e0: 0107 0800 c04f 0908 0440 4e09 0804 e050  .....O...@N....P
+000001f0: 0908 2820 50c0 0000 0000 0040 4bc0 1500  ..( P......@K...
+00000200: 1516 151a 2c15 1015 1015 0615 061c 1808  ....,...........
+00000210: 0000 0000 00c0 4ac0 1808 0000 0000 00e0  ......J.........
+00000220: 50c0 1600 2808 0000 0000 00c0 4ac0 1808  P...(.......J...
+00000230: 0000 0000 00e0 50c0 0000 000b 2802 0000  ......P.....(...
+00000240: 0010 0103 0340 3436 2690 091c 150a 1935  .....@46&......5
+00000250: 1000 0619 1803 6465 6315 0216 1016 8c02  ......dec.......
+00000260: 16fe 0126 fc07 2692 071c 1808 0000 0000  ...&..&.........
+00000270: 00c0 4ac0 1808 0000 0000 00e0 50c0 1600  ..J.........P...
+00000280: 2808 0000 0000 00c0 4ac0 1808 0000 0000  (.......J.......
+00000290: 00e0 50c0 0019 2c15 0415 0015 0200 1500  ..P...,.........
+000002a0: 1510 1502 0000 0015 0415 1015 144c 1502  .............L..
+000002b0: 1500 1200 0008 1c00 0000 0000 0000 0015  ................
+000002c0: 0015 1215 162c 1510 1510 1506 1506 1c18  .....,..........
+000002d0: 0800 0000 0000 0000 0018 0800 0000 0000  ................
+000002e0: 0000 0016 0028 0800 0000 0000 0000 0018  .....(..........
+000002f0: 0800 0000 0000 0000 0000 0000 0920 0200  ............. ..
+00000300: 0000 1001 0110 0026 8e0c 1c15 0419 3510  .......&......5.
+00000310: 0006 1918 0872 615f 6572 726f 7215 0216  .....ra_error...
+00000320: 1016 b801 16c0 0126 fe0a 26ce 0a1c 1808  .......&..&.....
+00000330: 0000 0000 0000 0000 1808 0000 0000 0000  ................
+00000340: 0000 1600 2808 0000 0000 0000 0000 1808  ....(...........
+00000350: 0000 0000 0000 0000 0019 2c15 0415 0015  ..........,.....
+00000360: 0200 1500 1510 1502 0000 0015 0415 1015  ................
+00000370: 144c 1502 1500 1200 0008 1c00 0000 0000  .L..............
+00000380: 0000 0015 0015 1215 162c 1510 1510 1506  .........,......
+00000390: 1506 1c18 0800 0000 0000 0000 0018 0800  ................
+000003a0: 0000 0000 0000 0016 0028 0800 0000 0000  .........(......
+000003b0: 0000 0018 0800 0000 0000 0000 0000 0000  ................
+000003c0: 0920 0200 0000 1001 0110 0026 960f 1c15  . .........&....
+000003d0: 0419 3510 0006 1918 0964 6563 5f65 7272  ..5......dec_err
+000003e0: 6f72 1502 1610 16b8 0116 c001 2686 0e26  or..........&..&
+000003f0: d60d 1c18 0800 0000 0000 0000 0018 0800  ................
+00000400: 0000 0000 0000 0016 0028 0800 0000 0000  .........(......
+00000410: 0000 0018 0800 0000 0000 0000 0000 192c  ...............,
+00000420: 1504 1500 1502 0015 0015 1015 0200 0000  ................
+00000430: 1504 196c 3500 1806 7363 6865 6d61 150a  ...l5...schema..
+00000440: 0015 0425 0218 0269 6400 150a 2502 1802  ...%...id...%...
+00000450: 7261 0015 0a25 0218 0364 6563 0015 0425  ra...%...dec...%
+00000460: 0218 0872 615f 6572 726f 7200 1504 2502  ...ra_error...%.
+00000470: 1809 6465 635f 6572 726f 7200 1610 191c  ..dec_error.....
+00000480: 195c 2696 021c 1504 1935 1000 0619 1802  .\&......5......
+00000490: 6964 1502 1610 16ae 0216 8e02 2682 0126  id..........&..&
+000004a0: 081c 1808 0803 0000 0000 0000 1808 f602  ................
+000004b0: 0000 0000 0000 1600 2808 0803 0000 0000  ........(.......
+000004c0: 0000 1808 f602 0000 0000 0000 0019 2c15  ..............,.
+000004d0: 0415 0015 0200 1500 1510 1502 0000 0026  ...............&
+000004e0: d605 1c15 0a19 3510 0006 1918 0272 6115  ......5......ra.
+000004f0: 0216 1016 9c02 1686 0226 c204 26d0 031c  .........&..&...
+00000500: 1808 0000 0000 00c8 7540 1808 0000 0000  ........u@......
+00000510: 0098 7240 1600 2808 0000 0000 00c8 7540  ..r@..(.......u@
+00000520: 1808 0000 0000 0098 7240 0019 2c15 0415  ........r@..,...
+00000530: 0015 0200 1500 1510 1502 0000 0026 9009  .............&..
+00000540: 1c15 0a19 3510 0006 1918 0364 6563 1502  ....5......dec..
+00000550: 1610 168c 0216 fe01 26fc 0726 9207 1c18  ........&..&....
+00000560: 0800 0000 0000 c04a c018 0800 0000 0000  .......J........
+00000570: e050 c016 0028 0800 0000 0000 c04a c018  .P...(.......J..
+00000580: 0800 0000 0000 e050 c000 192c 1504 1500  .......P...,....
+00000590: 1502 0015 0015 1015 0200 0000 268e 0c1c  ............&...
+000005a0: 1504 1935 1000 0619 1808 7261 5f65 7272  ...5......ra_err
+000005b0: 6f72 1502 1610 16b8 0116 c001 26fe 0a26  or..........&..&
+000005c0: ce0a 1c18 0800 0000 0000 0000 0018 0800  ................
+000005d0: 0000 0000 0000 0016 0028 0800 0000 0000  .........(......
+000005e0: 0000 0018 0800 0000 0000 0000 0000 192c  ...............,
+000005f0: 1504 1500 1502 0015 0015 1015 0200 0000  ................
+00000600: 2696 0f1c 1504 1935 1000 0619 1809 6465  &......5......de
+00000610: 635f 6572 726f 7215 0216 1016 b801 16c0  c_error.........
+00000620: 0126 860e 26d6 0d1c 1808 0000 0000 0000  .&..&...........
+00000630: 0000 1808 0000 0000 0000 0000 1600 2808  ..............(.
+00000640: 0000 0000 0000 0000 1808 0000 0000 0000  ................
+00000650: 0000 0019 2c15 0415 0015 0200 1500 1510  ....,...........
+00000660: 1502 0000 0016 c609 1610 2608 1692 0914  ..........&.....
+00000670: 0000 192c 1806 7061 6e64 6173 18a7 057b  ...,..pandas...{
+00000680: 2269 6e64 6578 5f63 6f6c 756d 6e73 223a  "index_columns":
+00000690: 205b 5d2c 2022 636f 6c75 6d6e 5f69 6e64   [], "column_ind
+000006a0: 6578 6573 223a 205b 5d2c 2022 636f 6c75  exes": [], "colu
+000006b0: 6d6e 7322 3a20 5b7b 226e 616d 6522 3a20  mns": [{"name": 
+000006c0: 2269 6422 2c20 2266 6965 6c64 5f6e 616d  "id", "field_nam
+000006d0: 6522 3a20 2269 6422 2c20 2270 616e 6461  e": "id", "panda
+000006e0: 735f 7479 7065 223a 2022 696e 7436 3422  s_type": "int64"
+000006f0: 2c20 226e 756d 7079 5f74 7970 6522 3a20  , "numpy_type": 
+00000700: 2269 6e74 3634 222c 2022 6d65 7461 6461  "int64", "metada
+00000710: 7461 223a 206e 756c 6c7d 2c20 7b22 6e61  ta": null}, {"na
+00000720: 6d65 223a 2022 7261 222c 2022 6669 656c  me": "ra", "fiel
+00000730: 645f 6e61 6d65 223a 2022 7261 222c 2022  d_name": "ra", "
+00000740: 7061 6e64 6173 5f74 7970 6522 3a20 2266  pandas_type": "f
+00000750: 6c6f 6174 3634 222c 2022 6e75 6d70 795f  loat64", "numpy_
+00000760: 7479 7065 223a 2022 666c 6f61 7436 3422  type": "float64"
+00000770: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
+00000780: 6c6c 7d2c 207b 226e 616d 6522 3a20 2264  ll}, {"name": "d
+00000790: 6563 222c 2022 6669 656c 645f 6e61 6d65  ec", "field_name
+000007a0: 223a 2022 6465 6322 2c20 2270 616e 6461  ": "dec", "panda
+000007b0: 735f 7479 7065 223a 2022 666c 6f61 7436  s_type": "float6
+000007c0: 3422 2c20 226e 756d 7079 5f74 7970 6522  4", "numpy_type"
+000007d0: 3a20 2266 6c6f 6174 3634 222c 2022 6d65  : "float64", "me
+000007e0: 7461 6461 7461 223a 206e 756c 6c7d 2c20  tadata": null}, 
+000007f0: 7b22 6e61 6d65 223a 2022 7261 5f65 7272  {"name": "ra_err
+00000800: 6f72 222c 2022 6669 656c 645f 6e61 6d65  or", "field_name
+00000810: 223a 2022 7261 5f65 7272 6f72 222c 2022  ": "ra_error", "
+00000820: 7061 6e64 6173 5f74 7970 6522 3a20 2269  pandas_type": "i
+00000830: 6e74 3634 222c 2022 6e75 6d70 795f 7479  nt64", "numpy_ty
+00000840: 7065 223a 2022 696e 7436 3422 2c20 226d  pe": "int64", "m
+00000850: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
+00000860: 207b 226e 616d 6522 3a20 2264 6563 5f65   {"name": "dec_e
+00000870: 7272 6f72 222c 2022 6669 656c 645f 6e61  rror", "field_na
+00000880: 6d65 223a 2022 6465 635f 6572 726f 7222  me": "dec_error"
+00000890: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
+000008a0: 2022 696e 7436 3422 2c20 226e 756d 7079   "int64", "numpy
+000008b0: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
+000008c0: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
+000008d0: 6c7d 5d2c 2022 6372 6561 746f 7222 3a20  l}], "creator": 
+000008e0: 7b22 6c69 6272 6172 7922 3a20 2270 7961  {"library": "pya
+000008f0: 7272 6f77 222c 2022 7665 7273 696f 6e22  rrow", "version"
+00000900: 3a20 2239 2e30 2e30 227d 2c20 2270 616e  : "9.0.0"}, "pan
+00000910: 6461 735f 7665 7273 696f 6e22 3a20 2232  das_version": "2
+00000920: 2e30 2e30 227d 0018 0c41 5252 4f57 3a73  .0.0"}...ARROW:s
+00000930: 6368 656d 6118 980b 2f2f 2f2f 2f79 6745  chema.../////ygE
+00000940: 4141 4151 4141 4141 4141 414b 4141 3441  AAAQAAAAAAAKAA4A
+00000950: 4267 4146 4141 6741 4367 4141 4141 4142  BgAFAAgACgAAAAAB
+00000960: 4241 4151 4141 4141 4141 414b 4141 7741  BAAQAAAAAAAKAAwA
+00000970: 4141 4145 4141 6741 4367 4141 414e 7743  AAAEAAgACgAAANwC
+00000980: 4141 4145 4141 4141 4151 4141 4141 7741  AAAEAAAAAQAAAAwA
+00000990: 4141 4149 4141 7741 4241 4149 4141 6741  AAAIAAwABAAIAAgA
+000009a0: 4141 4149 4141 4141 4541 4141 4141 5941  AAAIAAAAEAAAAAYA
+000009b0: 4141 4277 5957 356b 5958 4d41 414b 6343  AABwYW5kYXMAAKcC
+000009c0: 4141 4237 496d 6c75 5a47 5634 5832 4e76  AAB7ImluZGV4X2Nv
+000009d0: 6248 5674 626e 4d69 4f69 4262 5853 7767  bHVtbnMiOiBbXSwg
+000009e0: 496d 4e76 6248 5674 626c 3970 626d 526c  ImNvbHVtbl9pbmRl
+000009f0: 6547 567a 496a 6f67 5731 3073 4943 4a6a  eGVzIjogW10sICJj
+00000a00: 6232 7831 6257 357a 496a 6f67 5733 7369  b2x1bW5zIjogW3si
+00000a10: 626d 4674 5a53 4936 4943 4a70 5a43 4973  bmFtZSI6ICJpZCIs
+00000a20: 4943 4a6d 6157 5673 5a46 3975 5957 316c  ICJmaWVsZF9uYW1l
+00000a30: 496a 6f67 496d 6c6b 4969 7767 496e 4268  IjogImlkIiwgInBh
+00000a40: 626d 5268 6331 3930 6558 426c 496a 6f67  bmRhc190eXBlIjog
+00000a50: 496d 6c75 6444 5930 4969 7767 496d 3531  ImludDY0IiwgIm51
+00000a60: 6258 4235 5833 5235 6347 5569 4f69 4169  bXB5X3R5cGUiOiAi
+00000a70: 6157 3530 4e6a 5169 4c43 4169 6257 5630  aW50NjQiLCAibWV0
+00000a80: 5957 5268 6447 4569 4f69 4275 6457 7873  YWRhdGEiOiBudWxs
+00000a90: 6653 7767 6579 4a75 5957 316c 496a 6f67  fSwgeyJuYW1lIjog
+00000aa0: 496e 4a68 4969 7767 496d 5a70 5a57 786b  InJhIiwgImZpZWxk
+00000ab0: 5832 3568 6257 5569 4f69 4169 636d 4569  X25hbWUiOiAicmEi
+00000ac0: 4c43 4169 6347 4675 5a47 467a 5833 5235  LCAicGFuZGFzX3R5
+00000ad0: 6347 5569 4f69 4169 5a6d 7876 5958 5132  cGUiOiAiZmxvYXQ2
+00000ae0: 4e43 4973 4943 4a75 6457 3177 6556 3930  NCIsICJudW1weV90
+00000af0: 6558 426c 496a 6f67 496d 5a73 6232 4630  eXBlIjogImZsb2F0
+00000b00: 4e6a 5169 4c43 4169 6257 5630 5957 5268  NjQiLCAibWV0YWRh
+00000b10: 6447 4569 4f69 4275 6457 7873 6653 7767  dGEiOiBudWxsfSwg
+00000b20: 6579 4a75 5957 316c 496a 6f67 496d 526c  eyJuYW1lIjogImRl
+00000b30: 5979 4973 4943 4a6d 6157 5673 5a46 3975  YyIsICJmaWVsZF9u
+00000b40: 5957 316c 496a 6f67 496d 526c 5979 4973  YW1lIjogImRlYyIs
+00000b50: 4943 4a77 5957 356b 5958 4e66 6448 6c77  ICJwYW5kYXNfdHlw
+00000b60: 5a53 4936 4943 4a6d 6247 3968 6444 5930  ZSI6ICJmbG9hdDY0
+00000b70: 4969 7767 496d 3531 6258 4235 5833 5235  IiwgIm51bXB5X3R5
+00000b80: 6347 5569 4f69 4169 5a6d 7876 5958 5132  cGUiOiAiZmxvYXQ2
+00000b90: 4e43 4973 4943 4a74 5a58 5268 5a47 4630  NCIsICJtZXRhZGF0
+00000ba0: 5953 4936 4947 3531 6247 7839 4c43 4237  YSI6IG51bGx9LCB7
+00000bb0: 496d 3568 6257 5569 4f69 4169 636d 4666  Im5hbWUiOiAicmFf
+00000bc0: 5a58 4a79 6233 4969 4c43 4169 5a6d 6c6c  ZXJyb3IiLCAiZmll
+00000bd0: 6247 5266 626d 4674 5a53 4936 4943 4a79  bGRfbmFtZSI6ICJy
+00000be0: 5956 396c 636e 4a76 6369 4973 4943 4a77  YV9lcnJvciIsICJw
+00000bf0: 5957 356b 5958 4e66 6448 6c77 5a53 4936  YW5kYXNfdHlwZSI6
+00000c00: 4943 4a70 626e 5132 4e43 4973 4943 4a75  ICJpbnQ2NCIsICJu
+00000c10: 6457 3177 6556 3930 6558 426c 496a 6f67  dW1weV90eXBlIjog
+00000c20: 496d 6c75 6444 5930 4969 7767 496d 316c  ImludDY0IiwgIm1l
+00000c30: 6447 466b 5958 5268 496a 6f67 626e 5673  dGFkYXRhIjogbnVs
+00000c40: 6248 3073 4948 7369 626d 4674 5a53 4936  bH0sIHsibmFtZSI6
+00000c50: 4943 4a6b 5a57 4e66 5a58 4a79 6233 4969  ICJkZWNfZXJyb3Ii
+00000c60: 4c43 4169 5a6d 6c6c 6247 5266 626d 4674  LCAiZmllbGRfbmFt
+00000c70: 5a53 4936 4943 4a6b 5a57 4e66 5a58 4a79  ZSI6ICJkZWNfZXJy
+00000c80: 6233 4969 4c43 4169 6347 4675 5a47 467a  b3IiLCAicGFuZGFz
+00000c90: 5833 5235 6347 5569 4f69 4169 6157 3530  X3R5cGUiOiAiaW50
+00000ca0: 4e6a 5169 4c43 4169 626e 5674 6348 6c66  NjQiLCAibnVtcHlf
+00000cb0: 6448 6c77 5a53 4936 4943 4a70 626e 5132  dHlwZSI6ICJpbnQ2
+00000cc0: 4e43 4973 4943 4a74 5a58 5268 5a47 4630  NCIsICJtZXRhZGF0
+00000cd0: 5953 4936 4947 3531 6247 7839 5853 7767  YSI6IG51bGx9XSwg
+00000ce0: 496d 4e79 5a57 4630 6233 4969 4f69 4237  ImNyZWF0b3IiOiB7
+00000cf0: 496d 7870 596e 4a68 636e 6b69 4f69 4169  ImxpYnJhcnkiOiAi
+00000d00: 6348 6c68 636e 4a76 6479 4973 4943 4a32  cHlhcnJvdyIsICJ2
+00000d10: 5a58 4a7a 6157 3975 496a 6f67 496a 6b75  ZXJzaW9uIjogIjku
+00000d20: 4d43 3477 496e 3073 4943 4a77 5957 356b  MC4wIn0sICJwYW5k
+00000d30: 5958 4e66 646d 5679 6332 6c76 6269 4936  YXNfdmVyc2lvbiI6
+00000d40: 4943 4979 4c6a 4175 4d43 4a39 4141 5541  ICIyLjAuMCJ9AAUA
+00000d50: 4141 446b 4141 4141 6f41 4141 4148 5141  AADkAAAAoAAAAHQA
+00000d60: 4141 4138 4141 4141 4241 4141 4145 442f  AAA8AAAABAAAAED/
+00000d70: 2f2f 3841 4141 4543 4541 4141 4142 7741  //8AAAECEAAAABwA
+00000d80: 4141 4145 4141 4141 4141 4141 4141 6b41  AAAEAAAAAAAAAAkA
+00000d90: 4141 426b 5a57 4e66 5a58 4a79 6233 4941  AABkZWNfZXJyb3IA
+00000da0: 4141 4134 2f2f 2f2f 4141 4141 4155 4141  AAA4////AAAAAUAA
+00000db0: 4141 4230 2f2f 2f2f 4141 4142 4168 4141  AAB0////AAABAhAA
+00000dc0: 4141 4163 4141 4141 4241 4141 4141 4141  AAAcAAAABAAAAAAA
+00000dd0: 4141 4149 4141 4141 636d 4666 5a58 4a79  AAAIAAAAcmFfZXJy
+00000de0: 6233 4941 4141 4141 6250 2f2f 2f77 4141  b3IAAAAAbP///wAA
+00000df0: 4141 4641 4141 4141 7150 2f2f 2f77 4141  AAFAAAAAqP///wAA
+00000e00: 4151 4d51 4141 4141 4641 4141 4141 5141  AQMQAAAAFAAAAAQA
+00000e10: 4141 4141 4141 4141 4177 4141 4147 526c  AAAAAAAAAwAAAGRl
+00000e20: 5977 4457 2f2f 2f2f 4141 4143 414e 442f  YwDW////AAACAND/
+00000e30: 2f2f 3841 4141 4544 4541 4141 4142 7741  //8AAAEDEAAAABwA
+00000e40: 4141 4145 4141 4141 4141 4141 4141 4941  AAAEAAAAAAAAAAIA
+00000e50: 4141 4279 5951 4141 4141 4147 4141 6741  AAByYQAAAAAGAAgA
+00000e60: 4267 4147 4141 4141 4141 4143 4142 4141  BgAGAAAAAAACABAA
+00000e70: 4641 4149 4141 5941 4277 414d 4141 4141  FAAIAAYABwAMAAAA
+00000e80: 4541 4151 4141 4141 4141 4142 4168 4141  EAAQAAAAAAABAhAA
+00000e90: 4141 4163 4141 4141 4241 4141 4141 4141  AAAcAAAABAAAAAAA
+00000ea0: 4141 4143 4141 4141 6157 5141 4141 6741  AAACAAAAaWQAAAgA
+00000eb0: 4441 4149 4141 6341 4341 4141 4141 4141  DAAIAAcACAAAAAAA
+00000ec0: 4141 4641 4141 4141 4141 4141 4141 3d3d  AAFAAAAAAAAAAA==
+00000ed0: 0018 1f70 6172 7175 6574 2d63 7070 2d61  ...parquet-cpp-a
+00000ee0: 7272 6f77 2076 6572 7369 6f6e 2039 2e30  rrow version 9.0
+00000ef0: 2e30 195c 1c00 001c 0000 1c00 001c 0000  .0.\............
+00000f00: 1c00 0000 d40a 0000 5041 5231            ........PAR1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_45/shard_2.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet`

 * *Files 19% similar despite different names*

```diff
@@ -1,303 +1,244 @@
-00000000: 5041 5231 1504 1540 1538 4c15 0815 0012  PAR1...@.8L.....
-00000010: 0000 2008 ef02 0005 0100 f50d 083c f902  .. ..........<..
-00000020: 0000 0000 0000 fa02 0000 0000 0000 1500  ................
-00000030: 1514 1518 2c15 0815 1015 0615 061c 1808  ....,...........
-00000040: fa02 0000 0000 0000 1808 ef02 0000 0000  ................
-00000050: 0000 1600 2808 fa02 0000 0000 0000 1808  ....(...........
-00000060: ef02 0000 0000 0000 0000 000a 2402 0000  ............$...
-00000070: 0008 0102 03e4 0026 ee01 1c15 0419 3510  .......&......5.
-00000080: 0006 1918 0269 6415 0216 0816 ea01 16e6  .....id.........
-00000090: 0126 5c26 081c 1808 fa02 0000 0000 0000  .&\&............
-000000a0: 1808 ef02 0000 0000 0000 1600 2808 fa02  ............(...
-000000b0: 0000 0000 0000 1808 ef02 0000 0000 0000  ................
-000000c0: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
-000000d0: 0000 0015 0415 4015 3a4c 1508 1500 1200  ......@.:L......
-000000e0: 0020 0000 0101 08a8 7440 0107 0800 a875  . ......t@.....u
-000000f0: 0908 2898 7440 0000 0000 0078 7440 1500  ..(.t@.....xt@..
-00000100: 1514 1518 2c15 0815 1015 0615 061c 1808  ....,...........
-00000110: 0000 0000 00a8 7540 1808 0000 0000 0078  ......u@.......x
-00000120: 7440 1600 2808 0000 0000 00a8 7540 1808  t@..(.......u@..
-00000130: 0000 0000 0078 7440 0000 000a 2402 0000  .....xt@....$...
-00000140: 0008 0102 03e4 0026 8e05 1c15 0a19 3510  .......&......5.
-00000150: 0006 1918 0272 6115 0216 0816 ea01 16e8  .....ra.........
-00000160: 0126 fc03 26a6 031c 1808 0000 0000 00a8  .&..&...........
-00000170: 7540 1808 0000 0000 0078 7440 1600 2808  u@.......xt@..(.
-00000180: 0000 0000 00a8 7540 1808 0000 0000 0078  ......u@.......x
-00000190: 7440 0019 2c15 0415 0015 0200 1500 1510  t@..,...........
-000001a0: 1502 0000 0015 0415 4015 3a4c 1508 1500  ........@.:L....
-000001b0: 1200 0020 0000 0101 0840 46c0 0107 0800  ... .....@F.....
-000001c0: 4041 0908 2880 3dc0 0000 0000 00c0 49c0  @A..(.=.......I.
-000001d0: 1500 1514 1518 2c15 0815 1015 0615 061c  ......,.........
-000001e0: 1808 0000 0000 0080 3dc0 1808 0000 0000  ........=.......
-000001f0: 00c0 49c0 1600 2808 0000 0000 0080 3dc0  ..I...(.......=.
-00000200: 1808 0000 0000 00c0 49c0 0000 000a 2402  ........I.....$.
-00000210: 0000 0008 0102 03e4 0026 b208 1c15 0a19  .........&......
-00000220: 3510 0006 1918 0364 6563 1502 1608 16ea  5......dec......
-00000230: 0116 e801 26a0 0726 ca06 1c18 0800 0000  ....&..&........
-00000240: 0000 803d c018 0800 0000 0000 c049 c016  ...=.........I..
-00000250: 0028 0800 0000 0000 803d c018 0800 0000  .(.......=......
-00000260: 0000 c049 c000 192c 1504 1500 1502 0015  ...I...,........
-00000270: 0015 1015 0200 0000 1504 1510 1514 4c15  ..............L.
-00000280: 0215 0012 0000 081c 0000 0000 0000 0000  ................
-00000290: 1500 1512 1516 2c15 0815 1015 0615 061c  ......,.........
-000002a0: 1808 0000 0000 0000 0000 1808 0000 0000  ................
-000002b0: 0000 0000 1600 2808 0000 0000 0000 0000  ......(.........
-000002c0: 1808 0000 0000 0000 0000 0000 0009 2002  .............. .
-000002d0: 0000 0008 0101 0800 26b0 0b1c 1504 1935  ........&......5
-000002e0: 1000 0619 1808 7261 5f65 7272 6f72 1502  ......ra_error..
-000002f0: 1608 16b8 0116 c001 26a0 0a26 f009 1c18  ........&..&....
-00000300: 0800 0000 0000 0000 0018 0800 0000 0000  ................
-00000310: 0000 0016 0028 0800 0000 0000 0000 0018  .....(..........
-00000320: 0800 0000 0000 0000 0000 192c 1504 1500  ...........,....
-00000330: 1502 0015 0015 1015 0200 0000 1504 1510  ................
-00000340: 1514 4c15 0215 0012 0000 081c 0000 0000  ..L.............
-00000350: 0000 0000 1500 1512 1516 2c15 0815 1015  ..........,.....
-00000360: 0615 061c 1808 0000 0000 0000 0000 1808  ................
-00000370: 0000 0000 0000 0000 1600 2808 0000 0000  ..........(.....
-00000380: 0000 0000 1808 0000 0000 0000 0000 0000  ................
-00000390: 0009 2002 0000 0008 0101 0800 26b8 0e1c  .. .........&...
-000003a0: 1504 1935 1000 0619 1809 6465 635f 6572  ...5......dec_er
-000003b0: 726f 7215 0216 0816 b801 16c0 0126 a80d  ror..........&..
-000003c0: 26f8 0c1c 1808 0000 0000 0000 0000 1808  &...............
-000003d0: 0000 0000 0000 0000 1600 2808 0000 0000  ..........(.....
-000003e0: 0000 0000 1808 0000 0000 0000 0000 0019  ................
-000003f0: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
-00000400: 0015 0415 4015 344c 1508 1500 1200 0020  ....@.4L....... 
-00000410: 0000 0d01 0006 0d08 3c0a 0000 0000 0000  ........<.......
-00000420: 000b 0000 0000 0000 0015 0015 1415 182c  ...............,
-00000430: 1508 1510 1506 1506 1c18 080b 0000 0000  ................
-00000440: 0000 0018 0800 0000 0000 0000 0016 0028  ...............(
-00000450: 080b 0000 0000 0000 0018 0800 0000 0000  ................
-00000460: 0000 0000 0000 0a24 0200 0000 0801 0203  .......$........
-00000470: e400 26e4 111c 1504 1935 1000 0619 1811  ..&......5......
-00000480: 5f5f 696e 6465 785f 6c65 7665 6c5f 305f  __index_level_0_
-00000490: 5f15 0216 0816 ea01 16e2 0126 d210 2682  _..........&..&.
-000004a0: 101c 1808 0b00 0000 0000 0000 1808 0000  ................
-000004b0: 0000 0000 0000 1600 2808 0b00 0000 0000  ........(.......
-000004c0: 0000 1808 0000 0000 0000 0000 0019 2c15  ..............,.
-000004d0: 0415 0015 0200 1500 1510 1502 0000 0015  ................
-000004e0: 0419 7c35 0018 0673 6368 656d 6115 0c00  ..|5...schema...
-000004f0: 1504 2502 1802 6964 0015 0a25 0218 0272  ..%...id...%...r
-00000500: 6100 150a 2502 1803 6465 6300 1504 2502  a...%...dec...%.
-00000510: 1808 7261 5f65 7272 6f72 0015 0425 0218  ..ra_error...%..
-00000520: 0964 6563 5f65 7272 6f72 0015 0425 0218  .dec_error...%..
-00000530: 115f 5f69 6e64 6578 5f6c 6576 656c 5f30  .__index_level_0
-00000540: 5f5f 0016 0819 1c19 6c26 ee01 1c15 0419  __......l&......
-00000550: 3510 0006 1918 0269 6415 0216 0816 ea01  5......id.......
-00000560: 16e6 0126 5c26 081c 1808 fa02 0000 0000  ...&\&..........
-00000570: 0000 1808 ef02 0000 0000 0000 1600 2808  ..............(.
-00000580: fa02 0000 0000 0000 1808 ef02 0000 0000  ................
-00000590: 0000 0019 2c15 0415 0015 0200 1500 1510  ....,...........
-000005a0: 1502 0000 0026 8e05 1c15 0a19 3510 0006  .....&......5...
-000005b0: 1918 0272 6115 0216 0816 ea01 16e8 0126  ...ra..........&
-000005c0: fc03 26a6 031c 1808 0000 0000 00a8 7540  ..&...........u@
-000005d0: 1808 0000 0000 0078 7440 1600 2808 0000  .......xt@..(...
-000005e0: 0000 00a8 7540 1808 0000 0000 0078 7440  ....u@.......xt@
-000005f0: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
-00000600: 0000 0026 b208 1c15 0a19 3510 0006 1918  ...&......5.....
-00000610: 0364 6563 1502 1608 16ea 0116 e801 26a0  .dec..........&.
-00000620: 0726 ca06 1c18 0800 0000 0000 803d c018  .&...........=..
-00000630: 0800 0000 0000 c049 c016 0028 0800 0000  .......I...(....
-00000640: 0000 803d c018 0800 0000 0000 c049 c000  ...=.........I..
-00000650: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
-00000660: 0000 26b0 0b1c 1504 1935 1000 0619 1808  ..&......5......
-00000670: 7261 5f65 7272 6f72 1502 1608 16b8 0116  ra_error........
-00000680: c001 26a0 0a26 f009 1c18 0800 0000 0000  ..&..&..........
-00000690: 0000 0018 0800 0000 0000 0000 0016 0028  ...............(
-000006a0: 0800 0000 0000 0000 0018 0800 0000 0000  ................
-000006b0: 0000 0000 192c 1504 1500 1502 0015 0015  .....,..........
-000006c0: 1015 0200 0000 26b8 0e1c 1504 1935 1000  ......&......5..
-000006d0: 0619 1809 6465 635f 6572 726f 7215 0216  ....dec_error...
-000006e0: 0816 b801 16c0 0126 a80d 26f8 0c1c 1808  .......&..&.....
-000006f0: 0000 0000 0000 0000 1808 0000 0000 0000  ................
-00000700: 0000 1600 2808 0000 0000 0000 0000 1808  ....(...........
-00000710: 0000 0000 0000 0000 0019 2c15 0415 0015  ..........,.....
-00000720: 0200 1500 1510 1502 0000 0026 e411 1c15  ...........&....
-00000730: 0419 3510 0006 1918 115f 5f69 6e64 6578  ..5......__index
-00000740: 5f6c 6576 656c 5f30 5f5f 1502 1608 16ea  _level_0__......
-00000750: 0116 e201 26d2 1026 8210 1c18 080b 0000  ....&..&........
-00000760: 0000 0000 0018 0800 0000 0000 0000 0016  ................
-00000770: 0028 080b 0000 0000 0000 0018 0800 0000  .(..............
-00000780: 0000 0000 0000 192c 1504 1500 1502 0015  .......,........
-00000790: 0015 1015 0200 0000 1698 0a16 0826 0816  .............&..
-000007a0: 980a 1400 0019 2c18 0670 616e 6461 7318  ......,..pandas.
-000007b0: a507 7b22 696e 6465 785f 636f 6c75 6d6e  ..{"index_column
-000007c0: 7322 3a20 5b22 5f5f 696e 6465 785f 6c65  s": ["__index_le
-000007d0: 7665 6c5f 305f 5f22 5d2c 2022 636f 6c75  vel_0__"], "colu
-000007e0: 6d6e 5f69 6e64 6578 6573 223a 205b 7b22  mn_indexes": [{"
-000007f0: 6e61 6d65 223a 206e 756c 6c2c 2022 6669  name": null, "fi
-00000800: 656c 645f 6e61 6d65 223a 206e 756c 6c2c  eld_name": null,
-00000810: 2022 7061 6e64 6173 5f74 7970 6522 3a20   "pandas_type": 
-00000820: 2275 6e69 636f 6465 222c 2022 6e75 6d70  "unicode", "nump
-00000830: 795f 7479 7065 223a 2022 6f62 6a65 6374  y_type": "object
-00000840: 222c 2022 6d65 7461 6461 7461 223a 207b  ", "metadata": {
-00000850: 2265 6e63 6f64 696e 6722 3a20 2255 5446  "encoding": "UTF
-00000860: 2d38 227d 7d5d 2c20 2263 6f6c 756d 6e73  -8"}}], "columns
-00000870: 223a 205b 7b22 6e61 6d65 223a 2022 6964  ": [{"name": "id
-00000880: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
-00000890: 2022 6964 222c 2022 7061 6e64 6173 5f74   "id", "pandas_t
-000008a0: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
-000008b0: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
-000008c0: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
-000008d0: 3a20 6e75 6c6c 7d2c 207b 226e 616d 6522  : null}, {"name"
-000008e0: 3a20 2272 6122 2c20 2266 6965 6c64 5f6e  : "ra", "field_n
-000008f0: 616d 6522 3a20 2272 6122 2c20 2270 616e  ame": "ra", "pan
-00000900: 6461 735f 7479 7065 223a 2022 666c 6f61  das_type": "floa
-00000910: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
-00000920: 6522 3a20 2266 6c6f 6174 3634 222c 2022  e": "float64", "
-00000930: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
-00000940: 2c20 7b22 6e61 6d65 223a 2022 6465 6322  , {"name": "dec"
-00000950: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
-00000960: 2264 6563 222c 2022 7061 6e64 6173 5f74  "dec", "pandas_t
-00000970: 7970 6522 3a20 2266 6c6f 6174 3634 222c  ype": "float64",
-00000980: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
-00000990: 666c 6f61 7436 3422 2c20 226d 6574 6164  float64", "metad
-000009a0: 6174 6122 3a20 6e75 6c6c 7d2c 207b 226e  ata": null}, {"n
-000009b0: 616d 6522 3a20 2272 615f 6572 726f 7222  ame": "ra_error"
-000009c0: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
-000009d0: 2272 615f 6572 726f 7222 2c20 2270 616e  "ra_error", "pan
-000009e0: 6461 735f 7479 7065 223a 2022 696e 7436  das_type": "int6
-000009f0: 3422 2c20 226e 756d 7079 5f74 7970 6522  4", "numpy_type"
-00000a00: 3a20 2269 6e74 3634 222c 2022 6d65 7461  : "int64", "meta
-00000a10: 6461 7461 223a 206e 756c 6c7d 2c20 7b22  data": null}, {"
-00000a20: 6e61 6d65 223a 2022 6465 635f 6572 726f  name": "dec_erro
-00000a30: 7222 2c20 2266 6965 6c64 5f6e 616d 6522  r", "field_name"
-00000a40: 3a20 2264 6563 5f65 7272 6f72 222c 2022  : "dec_error", "
-00000a50: 7061 6e64 6173 5f74 7970 6522 3a20 2269  pandas_type": "i
-00000a60: 6e74 3634 222c 2022 6e75 6d70 795f 7479  nt64", "numpy_ty
-00000a70: 7065 223a 2022 696e 7436 3422 2c20 226d  pe": "int64", "m
-00000a80: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
-00000a90: 207b 226e 616d 6522 3a20 6e75 6c6c 2c20   {"name": null, 
-00000aa0: 2266 6965 6c64 5f6e 616d 6522 3a20 225f  "field_name": "_
-00000ab0: 5f69 6e64 6578 5f6c 6576 656c 5f30 5f5f  _index_level_0__
-00000ac0: 222c 2022 7061 6e64 6173 5f74 7970 6522  ", "pandas_type"
-00000ad0: 3a20 2269 6e74 3634 222c 2022 6e75 6d70  : "int64", "nump
-00000ae0: 795f 7479 7065 223a 2022 696e 7436 3422  y_type": "int64"
-00000af0: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
-00000b00: 6c6c 7d5d 2c20 2263 7265 6174 6f72 223a  ll}], "creator":
-00000b10: 207b 226c 6962 7261 7279 223a 2022 7079   {"library": "py
-00000b20: 6172 726f 7722 2c20 2276 6572 7369 6f6e  arrow", "version
-00000b30: 223a 2022 392e 302e 3022 7d2c 2022 7061  ": "9.0.0"}, "pa
-00000b40: 6e64 6173 5f76 6572 7369 6f6e 223a 2022  ndas_version": "
-00000b50: 312e 332e 3522 7d00 180c 4152 524f 573a  1.3.5"}...ARROW:
-00000b60: 7363 6865 6d61 18c0 0e2f 2f2f 2f2f 3267  schema.../////2g
-00000b70: 4641 4141 5141 4141 4141 4141 4b41 4134  FAAAQAAAAAAAKAA4
-00000b80: 4142 6741 4641 4167 4143 6741 4141 4141  ABgAFAAgACgAAAAA
-00000b90: 4242 4141 5141 4141 4141 4141 4b41 4177  BBAAQAAAAAAAKAAw
-00000ba0: 4141 4141 4541 4167 4143 6741 4141 4e77  AAAAEAAgACgAAANw
-00000bb0: 4441 4141 4541 4141 4141 5141 4141 4177  DAAAEAAAAAQAAAAw
-00000bc0: 4141 4141 4941 4177 4142 4141 4941 4167  AAAAIAAwABAAIAAg
-00000bd0: 4141 4141 4941 4141 4145 4141 4141 4159  AAAAIAAAAEAAAAAY
-00000be0: 4141 4142 7759 5735 6b59 584d 4141 4b55  AAABwYW5kYXMAAKU
-00000bf0: 4441 4142 3749 6d6c 755a 4756 3458 324e  DAAB7ImluZGV4X2N
-00000c00: 7662 4856 7462 6e4d 694f 6942 6249 6c39  vbHVtbnMiOiBbIl9
-00000c10: 6661 5735 6b5a 5868 6662 4756 325a 5778  faW5kZXhfbGV2ZWx
-00000c20: 664d 4639 6649 6c30 7349 434a 6a62 3278  fMF9fIl0sICJjb2x
-00000c30: 3162 5735 6661 5735 6b5a 5868 6c63 7949  1bW5faW5kZXhlcyI
-00000c40: 3649 4674 3749 6d35 6862 5755 694f 6942  6IFt7Im5hbWUiOiB
-00000c50: 7564 5778 734c 4341 695a 6d6c 6c62 4752  udWxsLCAiZmllbGR
-00000c60: 6662 6d46 745a 5349 3649 4735 3162 4777  fbmFtZSI6IG51bGw
-00000c70: 7349 434a 7759 5735 6b59 584e 6664 486c  sICJwYW5kYXNfdHl
-00000c80: 775a 5349 3649 434a 3162 6d6c 6a62 3252  wZSI6ICJ1bmljb2R
-00000c90: 6c49 6977 6749 6d35 3162 5842 3558 3352  lIiwgIm51bXB5X3R
-00000ca0: 3563 4755 694f 6941 6962 324a 715a 574e  5cGUiOiAib2JqZWN
-00000cb0: 3049 6977 6749 6d31 6c64 4746 6b59 5852  0IiwgIm1ldGFkYXR
-00000cc0: 6849 6a6f 6765 794a 6c62 6d4e 765a 476c  hIjogeyJlbmNvZGl
-00000cd0: 755a 7949 3649 434a 5656 4559 744f 434a  uZyI6ICJVVEYtOCJ
-00000ce0: 3966 5630 7349 434a 6a62 3278 3162 5735  9fV0sICJjb2x1bW5
-00000cf0: 7a49 6a6f 6757 3373 6962 6d46 745a 5349  zIjogW3sibmFtZSI
-00000d00: 3649 434a 705a 4349 7349 434a 6d61 5756  6ICJpZCIsICJmaWV
-00000d10: 735a 4639 7559 5731 6c49 6a6f 6749 6d6c  sZF9uYW1lIjogIml
-00000d20: 6b49 6977 6749 6e42 6862 6d52 6863 3139  kIiwgInBhbmRhc19
-00000d30: 3065 5842 6c49 6a6f 6749 6d6c 7564 4459  0eXBlIjogImludDY
-00000d40: 3049 6977 6749 6d35 3162 5842 3558 3352  0IiwgIm51bXB5X3R
-00000d50: 3563 4755 694f 6941 6961 5735 304e 6a51  5cGUiOiAiaW50NjQ
-00000d60: 694c 4341 6962 5756 3059 5752 6864 4745  iLCAibWV0YWRhdGE
-00000d70: 694f 6942 7564 5778 7366 5377 6765 794a  iOiBudWxsfSwgeyJ
-00000d80: 7559 5731 6c49 6a6f 6749 6e4a 6849 6977  uYW1lIjogInJhIiw
-00000d90: 6749 6d5a 705a 5778 6b58 3235 6862 5755  gImZpZWxkX25hbWU
-00000da0: 694f 6941 6963 6d45 694c 4341 6963 4746  iOiAicmEiLCAicGF
-00000db0: 755a 4746 7a58 3352 3563 4755 694f 6941  uZGFzX3R5cGUiOiA
-00000dc0: 695a 6d78 7659 5851 324e 4349 7349 434a  iZmxvYXQ2NCIsICJ
-00000dd0: 7564 5731 7765 5639 3065 5842 6c49 6a6f  udW1weV90eXBlIjo
-00000de0: 6749 6d5a 7362 3246 304e 6a51 694c 4341  gImZsb2F0NjQiLCA
-00000df0: 6962 5756 3059 5752 6864 4745 694f 6942  ibWV0YWRhdGEiOiB
-00000e00: 7564 5778 7366 5377 6765 794a 7559 5731  udWxsfSwgeyJuYW1
-00000e10: 6c49 6a6f 6749 6d52 6c59 7949 7349 434a  lIjogImRlYyIsICJ
-00000e20: 6d61 5756 735a 4639 7559 5731 6c49 6a6f  maWVsZF9uYW1lIjo
-00000e30: 6749 6d52 6c59 7949 7349 434a 7759 5735  gImRlYyIsICJwYW5
-00000e40: 6b59 584e 6664 486c 775a 5349 3649 434a  kYXNfdHlwZSI6ICJ
-00000e50: 6d62 4739 6864 4459 3049 6977 6749 6d35  mbG9hdDY0IiwgIm5
-00000e60: 3162 5842 3558 3352 3563 4755 694f 6941  1bXB5X3R5cGUiOiA
-00000e70: 695a 6d78 7659 5851 324e 4349 7349 434a  iZmxvYXQ2NCIsICJ
-00000e80: 745a 5852 685a 4746 3059 5349 3649 4735  tZXRhZGF0YSI6IG5
-00000e90: 3162 4778 394c 4342 3749 6d35 6862 5755  1bGx9LCB7Im5hbWU
-00000ea0: 694f 6941 6963 6d46 665a 584a 7962 3349  iOiAicmFfZXJyb3I
-00000eb0: 694c 4341 695a 6d6c 6c62 4752 6662 6d46  iLCAiZmllbGRfbmF
-00000ec0: 745a 5349 3649 434a 7959 5639 6c63 6e4a  tZSI6ICJyYV9lcnJ
-00000ed0: 7663 6949 7349 434a 7759 5735 6b59 584e  vciIsICJwYW5kYXN
-00000ee0: 6664 486c 775a 5349 3649 434a 7062 6e51  fdHlwZSI6ICJpbnQ
-00000ef0: 324e 4349 7349 434a 7564 5731 7765 5639  2NCIsICJudW1weV9
-00000f00: 3065 5842 6c49 6a6f 6749 6d6c 7564 4459  0eXBlIjogImludDY
-00000f10: 3049 6977 6749 6d31 6c64 4746 6b59 5852  0IiwgIm1ldGFkYXR
-00000f20: 6849 6a6f 6762 6e56 7362 4830 7349 4873  hIjogbnVsbH0sIHs
-00000f30: 6962 6d46 745a 5349 3649 434a 6b5a 574e  ibmFtZSI6ICJkZWN
-00000f40: 665a 584a 7962 3349 694c 4341 695a 6d6c  fZXJyb3IiLCAiZml
-00000f50: 6c62 4752 6662 6d46 745a 5349 3649 434a  lbGRfbmFtZSI6ICJ
-00000f60: 6b5a 574e 665a 584a 7962 3349 694c 4341  kZWNfZXJyb3IiLCA
-00000f70: 6963 4746 755a 4746 7a58 3352 3563 4755  icGFuZGFzX3R5cGU
-00000f80: 694f 6941 6961 5735 304e 6a51 694c 4341  iOiAiaW50NjQiLCA
-00000f90: 6962 6e56 7463 486c 6664 486c 775a 5349  ibnVtcHlfdHlwZSI
-00000fa0: 3649 434a 7062 6e51 324e 4349 7349 434a  6ICJpbnQ2NCIsICJ
-00000fb0: 745a 5852 685a 4746 3059 5349 3649 4735  tZXRhZGF0YSI6IG5
-00000fc0: 3162 4778 394c 4342 3749 6d35 6862 5755  1bGx9LCB7Im5hbWU
-00000fd0: 694f 6942 7564 5778 734c 4341 695a 6d6c  iOiBudWxsLCAiZml
-00000fe0: 6c62 4752 6662 6d46 745a 5349 3649 434a  lbGRfbmFtZSI6ICJ
-00000ff0: 6658 326c 755a 4756 3458 3278 6c64 6d56  fX2luZGV4X2xldmV
-00001000: 7358 7a42 6658 7949 7349 434a 7759 5735  sXzBfXyIsICJwYW5
-00001010: 6b59 584e 6664 486c 775a 5349 3649 434a  kYXNfdHlwZSI6ICJ
-00001020: 7062 6e51 324e 4349 7349 434a 7564 5731  pbnQ2NCIsICJudW1
-00001030: 7765 5639 3065 5842 6c49 6a6f 6749 6d6c  weV90eXBlIjogIml
-00001040: 7564 4459 3049 6977 6749 6d31 6c64 4746  udDY0IiwgIm1ldGF
-00001050: 6b59 5852 6849 6a6f 6762 6e56 7362 4831  kYXRhIjogbnVsbH1
-00001060: 644c 4341 6959 334a 6c59 5852 7663 6949  dLCAiY3JlYXRvciI
-00001070: 3649 4873 6962 476c 6963 6d46 7965 5349  6IHsibGlicmFyeSI
-00001080: 3649 434a 7765 5746 7963 6d39 3349 6977  6ICJweWFycm93Iiw
-00001090: 6749 6e5a 6c63 6e4e 7062 3234 694f 6941  gInZlcnNpb24iOiA
-000010a0: 694f 5334 774c 6a41 6966 5377 6749 6e42  iOS4wLjAifSwgInB
-000010b0: 6862 6d52 6863 3139 325a 584a 7a61 5739  hbmRhc192ZXJzaW9
-000010c0: 7549 6a6f 6749 6a45 754d 7934 3149 6e30  uIjogIjEuMy41In0
-000010d0: 4141 4141 4741 4141 414a 4145 4141 4f41  AAAAGAAAAJAEAAOA
-000010e0: 4141 4143 3041 4141 4166 4141 4141 4551  AAAC0AAAAfAAAAEQ
-000010f0: 4141 4141 4541 4141 4142 502f 2f2f 7741  AAAAEAAAABP///wA
-00001100: 4141 5149 5141 4141 414a 4141 4141 4151  AAQIQAAAAJAAAAAQ
-00001110: 4141 4141 4141 4141 4145 5141 4141 4639  AAAAAAAAAEQAAAF9
-00001120: 6661 5735 6b5a 5868 6662 4756 325a 5778  faW5kZXhfbGV2ZWx
-00001130: 664d 4639 6641 4141 4142 502f 2f2f 7741  fMF9fAAAABP///wA
-00001140: 4141 4146 4141 4141 4151 502f 2f2f 7741  AAAFAAAAAQP///wA
-00001150: 4141 5149 5141 4141 4148 4141 4141 4151  AAQIQAAAAHAAAAAQ
-00001160: 4141 4141 4141 4141 4143 5141 4141 4752  AAAAAAAAACQAAAGR
-00001170: 6c59 3139 6c63 6e4a 7663 6741 4141 446a  lY19lcnJvcgAAADj
-00001180: 2f2f 2f38 4141 4141 4251 4141 4141 4854  ///8AAAABQAAAAHT
-00001190: 2f2f 2f38 4141 4145 4345 4141 4141 4277  ///8AAAECEAAAABw
-000011a0: 4141 4141 4541 4141 4141 4141 4141 4167  AAAAEAAAAAAAAAAg
-000011b0: 4141 4142 7959 5639 6c63 6e4a 7663 6741  AAAByYV9lcnJvcgA
-000011c0: 4141 4142 732f 2f2f 2f41 4141 4141 5541  AAABs////AAAAAUA
-000011d0: 4141 4143 6f2f 2f2f 2f41 4141 4241 7841  AAACo////AAABAxA
-000011e0: 4141 4141 5541 4141 4142 4141 4141 4141  AAAAUAAAABAAAAAA
-000011f0: 4141 4141 4441 4141 415a 4756 6a41 4e62  AAAADAAAAZGVjANb
-00001200: 2f2f 2f38 4141 4149 4130 502f 2f2f 7741  ///8AAAIA0P///wA
-00001210: 4141 514d 5141 4141 4148 4141 4141 4151  AAQMQAAAAHAAAAAQ
-00001220: 4141 4141 4141 4141 4141 6741 4141 484a  AAAAAAAAAAgAAAHJ
-00001230: 6841 4141 4141 4159 4143 4141 4741 4159  hAAAAAAYACAAGAAY
-00001240: 4141 4141 4141 4149 4145 4141 5541 4167  AAAAAAAIAEAAUAAg
-00001250: 4142 6741 4841 4177 4141 4141 5141 4241  ABgAHAAwAAAAQABA
-00001260: 4141 4141 4141 4145 4345 4141 4141 4277  AAAAAAAECEAAAABw
-00001270: 4141 4141 4541 4141 4141 4141 4141 4149  AAAAEAAAAAAAAAAI
-00001280: 4141 4142 705a 4141 4143 4141 4d41 4167  AAABpZAAACAAMAAg
-00001290: 4142 7741 4941 4141 4141 4141 4141 5541  ABwAIAAAAAAAAAUA
-000012a0: 4141 4141 4141 4141 4100 181f 7061 7271  AAAAAAAAA...parq
-000012b0: 7565 742d 6370 702d 6172 726f 7720 7665  uet-cpp-arrow ve
-000012c0: 7273 696f 6e20 392e 302e 3019 6c1c 0000  rsion 9.0.0.l...
-000012d0: 1c00 001c 0000 1c00 001c 0000 1c00 0000  ................
-000012e0: 010e 0000 5041 5231                      ....PAR1
+00000000: 5041 5231 1504 15b0 0115 744c 1516 1500  PAR1......tL....
+00000010: 1200 0058 08f0 0200 0501 00f1 0d08 00f3  ...X............
+00000020: 0d08 00f7 0d08 00fb 0d08 00fc 0d08 00fd  ................
+00000030: 0d08 0401 0305 3704 0002 0d08 3c05 0300  ......7.....<...
+00000040: 0000 0000 0006 0300 0000 0000 0015 0015  ................
+00000050: 2015 242c 1516 1510 1506 1506 1c18 0806   .$,............
+00000060: 0300 0000 0000 0018 08f0 0200 0000 0000  ................
+00000070: 0016 0028 0806 0300 0000 0000 0018 08f0  ...(............
+00000080: 0200 0000 0000 0000 0000 103c 0200 0000  ...........<....
+00000090: 1601 0405 1032 5476 980a 0000 26b8 021c  .....2Tv....&...
+000000a0: 1504 1935 1000 0619 1802 6964 1502 1616  ...5......id....
+000000b0: 16e8 0216 b002 269a 0126 081c 1808 0603  ......&..&......
+000000c0: 0000 0000 0000 1808 f002 0000 0000 0000  ................
+000000d0: 1600 2808 0603 0000 0000 0000 1808 f002  ..(.............
+000000e0: 0000 0000 0000 0019 2c15 0415 0015 0200  ........,.......
+000000f0: 1500 1510 1502 0000 0015 0415 9001 1560  ...............`
+00000100: 4c15 1215 0012 0000 4800 0001 0108 3872  L.......H.....8r
+00000110: 4001 0708 0038 7309 0800 f80d 1000 2811  @....8s.......(.
+00000120: 080d 1800 980d 1004 d871 0928 2858 7240  .........q.((Xr@
+00000130: 0000 0000 0098 7140 1500 1520 1524 2c15  ......q@... .$,.
+00000140: 1615 1015 0615 061c 1808 0000 0000 0038  ...............8
+00000150: 7340 1808 0000 0000 0098 7140 1600 2808  s@........q@..(.
+00000160: 0000 0000 0038 7340 1808 0000 0000 0098  .....8s@........
+00000170: 7140 0000 0010 3c02 0000 0016 0104 0510  q@....<.........
+00000180: 3254 1476 0800 0026 8e06 1c15 0a19 3510  2T.v...&......5.
+00000190: 0006 1918 0272 6115 0216 1616 c802 169c  .....ra.........
+000001a0: 0226 f004 26f2 031c 1808 0000 0000 0038  .&..&..........8
+000001b0: 7340 1808 0000 0000 0098 7140 1600 2808  s@........q@..(.
+000001c0: 0000 0000 0038 7340 1808 0000 0000 0098  .....8s@........
+000001d0: 7140 0019 2c15 0415 0015 0200 1500 1510  q@..,...........
+000001e0: 1502 0000 0015 0415 9001 1568 4c15 1215  ...........hL...
+000001f0: 0012 0000 4800 0001 0108 4041 c001 0708  ....H.....@A....
+00000200: 00c0 4609 0804 4043 0d08 0048 0908 00c0  ..F...@C...H....
+00000210: 0d20 0440 4509 1004 803d 0908 2840 49c0  . .@E....=..(@I.
+00000220: 0000 0000 0040 4bc0 1500 1520 1524 2c15  .....@K.... .$,.
+00000230: 1615 1015 0615 061c 1808 0000 0000 0080  ................
+00000240: 3dc0 1808 0000 0000 0040 4bc0 1600 2808  =........@K...(.
+00000250: 0000 0000 0080 3dc0 1808 0000 0000 0040  ......=........@
+00000260: 4bc0 0000 0010 3c02 0000 0016 0104 0510  K.....<.........
+00000270: 3212 5476 0800 0026 ee09 1c15 0a19 3510  2.Tv...&......5.
+00000280: 0006 1918 0364 6563 1502 1616 16c8 0216  .....dec........
+00000290: a402 26d0 0826 ca07 1c18 0800 0000 0000  ..&..&..........
+000002a0: 803d c018 0800 0000 0000 404b c016 0028  .=........@K...(
+000002b0: 0800 0000 0000 803d c018 0800 0000 0000  .......=........
+000002c0: 404b c000 192c 1504 1500 1502 0015 0015  @K...,..........
+000002d0: 1015 0200 0000 1504 1510 1514 4c15 0215  ............L...
+000002e0: 0012 0000 081c 0000 0000 0000 0000 1500  ................
+000002f0: 1512 1516 2c15 1615 1015 0615 061c 1808  ....,...........
+00000300: 0000 0000 0000 0000 1808 0000 0000 0000  ................
+00000310: 0000 1600 2808 0000 0000 0000 0000 1808  ....(...........
+00000320: 0000 0000 0000 0000 0000 0009 2002 0000  ............ ...
+00000330: 0016 0101 1600 26ec 0c1c 1504 1935 1000  ......&......5..
+00000340: 0619 1808 7261 5f65 7272 6f72 1502 1616  ....ra_error....
+00000350: 16b8 0116 c001 26dc 0b26 ac0b 1c18 0800  ......&..&......
+00000360: 0000 0000 0000 0018 0800 0000 0000 0000  ................
+00000370: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
+00000380: 0000 0000 0000 0000 192c 1504 1500 1502  .........,......
+00000390: 0015 0015 1015 0200 0000 1504 1510 1514  ................
+000003a0: 4c15 0215 0012 0000 081c 0000 0000 0000  L...............
+000003b0: 0000 1500 1512 1516 2c15 1615 1015 0615  ........,.......
+000003c0: 061c 1808 0000 0000 0000 0000 1808 0000  ................
+000003d0: 0000 0000 0000 1600 2808 0000 0000 0000  ........(.......
+000003e0: 0000 1808 0000 0000 0000 0000 0000 0009  ................
+000003f0: 2002 0000 0016 0101 1600 26f4 0f1c 1504   .........&.....
+00000400: 1935 1000 0619 1809 6465 635f 6572 726f  .5......dec_erro
+00000410: 7215 0216 1616 b801 16c0 0126 e40e 26b4  r..........&..&.
+00000420: 0e1c 1808 0000 0000 0000 0000 1808 0000  ................
+00000430: 0000 0000 0000 1600 2808 0000 0000 0000  ........(.......
+00000440: 0000 1808 0000 0000 0000 0000 0019 2c15  ..............,.
+00000450: 0415 0015 0200 1500 1510 1502 0000 0015  ................
+00000460: 0419 6c35 0018 0673 6368 656d 6115 0a00  ..l5...schema...
+00000470: 1504 2502 1802 6964 0015 0a25 0218 0272  ..%...id...%...r
+00000480: 6100 150a 2502 1803 6465 6300 1504 2502  a...%...dec...%.
+00000490: 1808 7261 5f65 7272 6f72 0015 0425 0218  ..ra_error...%..
+000004a0: 0964 6563 5f65 7272 6f72 0016 1619 1c19  .dec_error......
+000004b0: 5c26 b802 1c15 0419 3510 0006 1918 0269  \&......5......i
+000004c0: 6415 0216 1616 e802 16b0 0226 9a01 2608  d..........&..&.
+000004d0: 1c18 0806 0300 0000 0000 0018 08f0 0200  ................
+000004e0: 0000 0000 0016 0028 0806 0300 0000 0000  .......(........
+000004f0: 0018 08f0 0200 0000 0000 0000 192c 1504  .............,..
+00000500: 1500 1502 0015 0015 1015 0200 0000 268e  ..............&.
+00000510: 061c 150a 1935 1000 0619 1802 7261 1502  .....5......ra..
+00000520: 1616 16c8 0216 9c02 26f0 0426 f203 1c18  ........&..&....
+00000530: 0800 0000 0000 3873 4018 0800 0000 0000  ......8s@.......
+00000540: 9871 4016 0028 0800 0000 0000 3873 4018  .q@..(......8s@.
+00000550: 0800 0000 0000 9871 4000 192c 1504 1500  .......q@..,....
+00000560: 1502 0015 0015 1015 0200 0000 26ee 091c  ............&...
+00000570: 150a 1935 1000 0619 1803 6465 6315 0216  ...5......dec...
+00000580: 1616 c802 16a4 0226 d008 26ca 071c 1808  .......&..&.....
+00000590: 0000 0000 0080 3dc0 1808 0000 0000 0040  ......=........@
+000005a0: 4bc0 1600 2808 0000 0000 0080 3dc0 1808  K...(.......=...
+000005b0: 0000 0000 0040 4bc0 0019 2c15 0415 0015  .....@K...,.....
+000005c0: 0200 1500 1510 1502 0000 0026 ec0c 1c15  ...........&....
+000005d0: 0419 3510 0006 1918 0872 615f 6572 726f  ..5......ra_erro
+000005e0: 7215 0216 1616 b801 16c0 0126 dc0b 26ac  r..........&..&.
+000005f0: 0b1c 1808 0000 0000 0000 0000 1808 0000  ................
+00000600: 0000 0000 0000 1600 2808 0000 0000 0000  ........(.......
+00000610: 0000 1808 0000 0000 0000 0000 0019 2c15  ..............,.
+00000620: 0415 0015 0200 1500 1510 1502 0000 0026  ...............&
+00000630: f40f 1c15 0419 3510 0006 1918 0964 6563  ......5......dec
+00000640: 5f65 7272 6f72 1502 1616 16b8 0116 c001  _error..........
+00000650: 26e4 0e26 b40e 1c18 0800 0000 0000 0000  &..&............
+00000660: 0018 0800 0000 0000 0000 0016 0028 0800  .............(..
+00000670: 0000 0000 0000 0018 0800 0000 0000 0000  ................
+00000680: 0000 192c 1504 1500 1502 0015 0015 1015  ...,............
+00000690: 0200 0000 16e8 0a16 1626 0816 f009 1400  .........&......
+000006a0: 0019 2c18 0670 616e 6461 7318 a705 7b22  ..,..pandas...{"
+000006b0: 696e 6465 785f 636f 6c75 6d6e 7322 3a20  index_columns": 
+000006c0: 5b5d 2c20 2263 6f6c 756d 6e5f 696e 6465  [], "column_inde
+000006d0: 7865 7322 3a20 5b5d 2c20 2263 6f6c 756d  xes": [], "colum
+000006e0: 6e73 223a 205b 7b22 6e61 6d65 223a 2022  ns": [{"name": "
+000006f0: 6964 222c 2022 6669 656c 645f 6e61 6d65  id", "field_name
+00000700: 223a 2022 6964 222c 2022 7061 6e64 6173  ": "id", "pandas
+00000710: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
+00000720: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
+00000730: 696e 7436 3422 2c20 226d 6574 6164 6174  int64", "metadat
+00000740: 6122 3a20 6e75 6c6c 7d2c 207b 226e 616d  a": null}, {"nam
+00000750: 6522 3a20 2272 6122 2c20 2266 6965 6c64  e": "ra", "field
+00000760: 5f6e 616d 6522 3a20 2272 6122 2c20 2270  _name": "ra", "p
+00000770: 616e 6461 735f 7479 7065 223a 2022 666c  andas_type": "fl
+00000780: 6f61 7436 3422 2c20 226e 756d 7079 5f74  oat64", "numpy_t
+00000790: 7970 6522 3a20 2266 6c6f 6174 3634 222c  ype": "float64",
+000007a0: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
+000007b0: 6c7d 2c20 7b22 6e61 6d65 223a 2022 6465  l}, {"name": "de
+000007c0: 6322 2c20 2266 6965 6c64 5f6e 616d 6522  c", "field_name"
+000007d0: 3a20 2264 6563 222c 2022 7061 6e64 6173  : "dec", "pandas
+000007e0: 5f74 7970 6522 3a20 2266 6c6f 6174 3634  _type": "float64
+000007f0: 222c 2022 6e75 6d70 795f 7479 7065 223a  ", "numpy_type":
+00000800: 2022 666c 6f61 7436 3422 2c20 226d 6574   "float64", "met
+00000810: 6164 6174 6122 3a20 6e75 6c6c 7d2c 207b  adata": null}, {
+00000820: 226e 616d 6522 3a20 2272 615f 6572 726f  "name": "ra_erro
+00000830: 7222 2c20 2266 6965 6c64 5f6e 616d 6522  r", "field_name"
+00000840: 3a20 2272 615f 6572 726f 7222 2c20 2270  : "ra_error", "p
+00000850: 616e 6461 735f 7479 7065 223a 2022 696e  andas_type": "in
+00000860: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
+00000870: 6522 3a20 2269 6e74 3634 222c 2022 6d65  e": "int64", "me
+00000880: 7461 6461 7461 223a 206e 756c 6c7d 2c20  tadata": null}, 
+00000890: 7b22 6e61 6d65 223a 2022 6465 635f 6572  {"name": "dec_er
+000008a0: 726f 7222 2c20 2266 6965 6c64 5f6e 616d  ror", "field_nam
+000008b0: 6522 3a20 2264 6563 5f65 7272 6f72 222c  e": "dec_error",
+000008c0: 2022 7061 6e64 6173 5f74 7970 6522 3a20   "pandas_type": 
+000008d0: 2269 6e74 3634 222c 2022 6e75 6d70 795f  "int64", "numpy_
+000008e0: 7479 7065 223a 2022 696e 7436 3422 2c20  type": "int64", 
+000008f0: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
+00000900: 7d5d 2c20 2263 7265 6174 6f72 223a 207b  }], "creator": {
+00000910: 226c 6962 7261 7279 223a 2022 7079 6172  "library": "pyar
+00000920: 726f 7722 2c20 2276 6572 7369 6f6e 223a  row", "version":
+00000930: 2022 392e 302e 3022 7d2c 2022 7061 6e64   "9.0.0"}, "pand
+00000940: 6173 5f76 6572 7369 6f6e 223a 2022 322e  as_version": "2.
+00000950: 302e 3022 7d00 180c 4152 524f 573a 7363  0.0"}...ARROW:sc
+00000960: 6865 6d61 1898 0b2f 2f2f 2f2f 7967 4541  hema.../////ygEA
+00000970: 4141 5141 4141 4141 4141 4b41 4134 4142  AAQAAAAAAAKAA4AB
+00000980: 6741 4641 4167 4143 6741 4141 4141 4242  gAFAAgACgAAAAABB
+00000990: 4141 5141 4141 4141 4141 4b41 4177 4141  AAQAAAAAAAKAAwAA
+000009a0: 4141 4541 4167 4143 6741 4141 4e77 4341  AAEAAgACgAAANwCA
+000009b0: 4141 4541 4141 4141 5141 4141 4177 4141  AAEAAAAAQAAAAwAA
+000009c0: 4141 4941 4177 4142 4141 4941 4167 4141  AAIAAwABAAIAAgAA
+000009d0: 4141 4941 4141 4145 4141 4141 4159 4141  AAIAAAAEAAAAAYAA
+000009e0: 4142 7759 5735 6b59 584d 4141 4b63 4341  ABwYW5kYXMAAKcCA
+000009f0: 4142 3749 6d6c 755a 4756 3458 324e 7662  AB7ImluZGV4X2Nvb
+00000a00: 4856 7462 6e4d 694f 6942 6258 5377 6749  HVtbnMiOiBbXSwgI
+00000a10: 6d4e 7662 4856 7462 6c39 7062 6d52 6c65  mNvbHVtbl9pbmRle
+00000a20: 4756 7a49 6a6f 6757 3130 7349 434a 6a62  GVzIjogW10sICJjb
+00000a30: 3278 3162 5735 7a49 6a6f 6757 3373 6962  2x1bW5zIjogW3sib
+00000a40: 6d46 745a 5349 3649 434a 705a 4349 7349  mFtZSI6ICJpZCIsI
+00000a50: 434a 6d61 5756 735a 4639 7559 5731 6c49  CJmaWVsZF9uYW1lI
+00000a60: 6a6f 6749 6d6c 6b49 6977 6749 6e42 6862  jogImlkIiwgInBhb
+00000a70: 6d52 6863 3139 3065 5842 6c49 6a6f 6749  mRhc190eXBlIjogI
+00000a80: 6d6c 7564 4459 3049 6977 6749 6d35 3162  mludDY0IiwgIm51b
+00000a90: 5842 3558 3352 3563 4755 694f 6941 6961  XB5X3R5cGUiOiAia
+00000aa0: 5735 304e 6a51 694c 4341 6962 5756 3059  W50NjQiLCAibWV0Y
+00000ab0: 5752 6864 4745 694f 6942 7564 5778 7366  WRhdGEiOiBudWxsf
+00000ac0: 5377 6765 794a 7559 5731 6c49 6a6f 6749  SwgeyJuYW1lIjogI
+00000ad0: 6e4a 6849 6977 6749 6d5a 705a 5778 6b58  nJhIiwgImZpZWxkX
+00000ae0: 3235 6862 5755 694f 6941 6963 6d45 694c  25hbWUiOiAicmEiL
+00000af0: 4341 6963 4746 755a 4746 7a58 3352 3563  CAicGFuZGFzX3R5c
+00000b00: 4755 694f 6941 695a 6d78 7659 5851 324e  GUiOiAiZmxvYXQ2N
+00000b10: 4349 7349 434a 7564 5731 7765 5639 3065  CIsICJudW1weV90e
+00000b20: 5842 6c49 6a6f 6749 6d5a 7362 3246 304e  XBlIjogImZsb2F0N
+00000b30: 6a51 694c 4341 6962 5756 3059 5752 6864  jQiLCAibWV0YWRhd
+00000b40: 4745 694f 6942 7564 5778 7366 5377 6765  GEiOiBudWxsfSwge
+00000b50: 794a 7559 5731 6c49 6a6f 6749 6d52 6c59  yJuYW1lIjogImRlY
+00000b60: 7949 7349 434a 6d61 5756 735a 4639 7559  yIsICJmaWVsZF9uY
+00000b70: 5731 6c49 6a6f 6749 6d52 6c59 7949 7349  W1lIjogImRlYyIsI
+00000b80: 434a 7759 5735 6b59 584e 6664 486c 775a  CJwYW5kYXNfdHlwZ
+00000b90: 5349 3649 434a 6d62 4739 6864 4459 3049  SI6ICJmbG9hdDY0I
+00000ba0: 6977 6749 6d35 3162 5842 3558 3352 3563  iwgIm51bXB5X3R5c
+00000bb0: 4755 694f 6941 695a 6d78 7659 5851 324e  GUiOiAiZmxvYXQ2N
+00000bc0: 4349 7349 434a 745a 5852 685a 4746 3059  CIsICJtZXRhZGF0Y
+00000bd0: 5349 3649 4735 3162 4778 394c 4342 3749  SI6IG51bGx9LCB7I
+00000be0: 6d35 6862 5755 694f 6941 6963 6d46 665a  m5hbWUiOiAicmFfZ
+00000bf0: 584a 7962 3349 694c 4341 695a 6d6c 6c62  XJyb3IiLCAiZmllb
+00000c00: 4752 6662 6d46 745a 5349 3649 434a 7959  GRfbmFtZSI6ICJyY
+00000c10: 5639 6c63 6e4a 7663 6949 7349 434a 7759  V9lcnJvciIsICJwY
+00000c20: 5735 6b59 584e 6664 486c 775a 5349 3649  W5kYXNfdHlwZSI6I
+00000c30: 434a 7062 6e51 324e 4349 7349 434a 7564  CJpbnQ2NCIsICJud
+00000c40: 5731 7765 5639 3065 5842 6c49 6a6f 6749  W1weV90eXBlIjogI
+00000c50: 6d6c 7564 4459 3049 6977 6749 6d31 6c64  mludDY0IiwgIm1ld
+00000c60: 4746 6b59 5852 6849 6a6f 6762 6e56 7362  GFkYXRhIjogbnVsb
+00000c70: 4830 7349 4873 6962 6d46 745a 5349 3649  H0sIHsibmFtZSI6I
+00000c80: 434a 6b5a 574e 665a 584a 7962 3349 694c  CJkZWNfZXJyb3IiL
+00000c90: 4341 695a 6d6c 6c62 4752 6662 6d46 745a  CAiZmllbGRfbmFtZ
+00000ca0: 5349 3649 434a 6b5a 574e 665a 584a 7962  SI6ICJkZWNfZXJyb
+00000cb0: 3349 694c 4341 6963 4746 755a 4746 7a58  3IiLCAicGFuZGFzX
+00000cc0: 3352 3563 4755 694f 6941 6961 5735 304e  3R5cGUiOiAiaW50N
+00000cd0: 6a51 694c 4341 6962 6e56 7463 486c 6664  jQiLCAibnVtcHlfd
+00000ce0: 486c 775a 5349 3649 434a 7062 6e51 324e  HlwZSI6ICJpbnQ2N
+00000cf0: 4349 7349 434a 745a 5852 685a 4746 3059  CIsICJtZXRhZGF0Y
+00000d00: 5349 3649 4735 3162 4778 3958 5377 6749  SI6IG51bGx9XSwgI
+00000d10: 6d4e 795a 5746 3062 3349 694f 6942 3749  mNyZWF0b3IiOiB7I
+00000d20: 6d78 7059 6e4a 6863 6e6b 694f 6941 6963  mxpYnJhcnkiOiAic
+00000d30: 486c 6863 6e4a 7664 7949 7349 434a 325a  HlhcnJvdyIsICJ2Z
+00000d40: 584a 7a61 5739 7549 6a6f 6749 6a6b 754d  XJzaW9uIjogIjkuM
+00000d50: 4334 7749 6e30 7349 434a 7759 5735 6b59  C4wIn0sICJwYW5kY
+00000d60: 584e 6664 6d56 7963 326c 7662 6949 3649  XNfdmVyc2lvbiI6I
+00000d70: 4349 794c 6a41 754d 434a 3941 4155 4141  CIyLjAuMCJ9AAUAA
+00000d80: 4144 6b41 4141 416f 4141 4141 4851 4141  ADkAAAAoAAAAHQAA
+00000d90: 4141 3841 4141 4142 4141 4141 4544 2f2f  AA8AAAABAAAAED//
+00000da0: 2f38 4141 4145 4345 4141 4141 4277 4141  /8AAAECEAAAABwAA
+00000db0: 4141 4541 4141 4141 4141 4141 416b 4141  AAEAAAAAAAAAAkAA
+00000dc0: 4142 6b5a 574e 665a 584a 7962 3349 4141  ABkZWNfZXJyb3IAA
+00000dd0: 4141 342f 2f2f 2f41 4141 4141 5541 4141  AA4////AAAAAUAAA
+00000de0: 4142 302f 2f2f 2f41 4141 4241 6841 4141  AB0////AAABAhAAA
+00000df0: 4141 6341 4141 4142 4141 4141 4141 4141  AAcAAAABAAAAAAAA
+00000e00: 4141 4941 4141 4163 6d46 665a 584a 7962  AAIAAAAcmFfZXJyb
+00000e10: 3349 4141 4141 4162 502f 2f2f 7741 4141  3IAAAAAbP///wAAA
+00000e20: 4146 4141 4141 4171 502f 2f2f 7741 4141  AFAAAAAqP///wAAA
+00000e30: 514d 5141 4141 4146 4141 4141 4151 4141  QMQAAAAFAAAAAQAA
+00000e40: 4141 4141 4141 4141 7741 4141 4752 6c59  AAAAAAAAwAAAGRlY
+00000e50: 7744 572f 2f2f 2f41 4141 4341 4e44 2f2f  wDW////AAACAND//
+00000e60: 2f38 4141 4145 4445 4141 4141 4277 4141  /8AAAEDEAAAABwAA
+00000e70: 4141 4541 4141 4141 4141 4141 4149 4141  AAEAAAAAAAAAAIAA
+00000e80: 4142 7959 5141 4141 4141 4741 4167 4142  AByYQAAAAAGAAgAB
+00000e90: 6741 4741 4141 4141 4141 4341 4241 4146  gAGAAAAAAACABAAF
+00000ea0: 4141 4941 4159 4142 7741 4d41 4141 4145  AAIAAYABwAMAAAAE
+00000eb0: 4141 5141 4141 4141 4141 4241 6841 4141  AAQAAAAAAABAhAAA
+00000ec0: 4141 6341 4141 4142 4141 4141 4141 4141  AAcAAAABAAAAAAAA
+00000ed0: 4141 4341 4141 4161 5751 4141 4167 4144  AACAAAAaWQAAAgAD
+00000ee0: 4141 4941 4163 4143 4141 4141 4141 4141  AAIAAcACAAAAAAAA
+00000ef0: 4146 4141 4141 4141 4141 4141 413d 3d00  AFAAAAAAAAAAA==.
+00000f00: 181f 7061 7271 7565 742d 6370 702d 6172  ..parquet-cpp-ar
+00000f10: 726f 7720 7665 7273 696f 6e20 392e 302e  row version 9.0.
+00000f20: 3019 5c1c 0000 1c00 001c 0000 1c00 001c  0.\.............
+00000f30: 0000 00d4 0a00 0050 4152 31              .......PAR1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_45/shard_3.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet`

 * *Files 14% similar despite different names*

```diff
@@ -60,247 +60,181 @@
 000003b0: 0009 2002 0000 000e 0101 0e00 26f8 0e1c  .. .........&...
 000003c0: 1504 1935 1000 0619 1809 6465 635f 6572  ...5......dec_er
 000003d0: 726f 7215 0216 0e16 b801 16c0 0126 e80d  ror..........&..
 000003e0: 26b8 0d1c 1808 0000 0000 0000 0000 1808  &...............
 000003f0: 0000 0000 0000 0000 1600 2808 0000 0000  ..........(.....
 00000400: 0000 0000 1808 0000 0000 0000 0000 0019  ................
 00000410: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
-00000420: 0015 0415 7015 504c 150e 1500 1200 0038  ....p.PL.......8
-00000430: 0401 0009 0100 0309 0704 0006 0d08 0007  ................
-00000440: 0d08 0011 0d08 3c13 0000 0000 0000 0014  ......<.........
-00000450: 0000 0000 0000 0015 0015 1615 1a2c 150e  .............,..
-00000460: 1510 1506 1506 1c18 0814 0000 0000 0000  ................
-00000470: 0018 0801 0000 0000 0000 0016 0028 0814  .............(..
-00000480: 0000 0000 0000 0018 0801 0000 0000 0000  ................
-00000490: 0000 0000 0b28 0200 0000 0e01 0303 88c6  .....(..........
-000004a0: 1a26 c212 1c15 0419 3510 0006 1918 115f  .&......5......_
-000004b0: 5f69 6e64 6578 5f6c 6576 656c 5f30 5f5f  _index_level_0__
-000004c0: 1502 160e 169c 0216 8002 26ae 1126 c210  ..........&..&..
-000004d0: 1c18 0814 0000 0000 0000 0018 0801 0000  ................
-000004e0: 0000 0000 0016 0028 0814 0000 0000 0000  .......(........
-000004f0: 0018 0801 0000 0000 0000 0000 192c 1504  .............,..
-00000500: 1500 1502 0015 0015 1015 0200 0000 1504  ................
-00000510: 197c 3500 1806 7363 6865 6d61 150c 0015  .|5...schema....
-00000520: 0425 0218 0269 6400 150a 2502 1802 7261  .%...id...%...ra
-00000530: 0015 0a25 0218 0364 6563 0015 0425 0218  ...%...dec...%..
-00000540: 0872 615f 6572 726f 7200 1504 2502 1809  .ra_error...%...
-00000550: 6465 635f 6572 726f 7200 1504 2502 1811  dec_error...%...
-00000560: 5f5f 696e 6465 785f 6c65 7665 6c5f 305f  __index_level_0_
-00000570: 5f00 160e 191c 196c 2688 021c 1504 1935  _......l&......5
-00000580: 1000 0619 1802 6964 1502 160e 169c 0216  ......id........
-00000590: 8002 2674 2608 1c18 08e9 0200 0000 0000  ..&t&...........
-000005a0: 0018 08d6 0200 0000 0000 0016 0028 08e9  .............(..
-000005b0: 0200 0000 0000 0018 08d6 0200 0000 0000  ................
-000005c0: 0000 192c 1504 1500 1502 0015 0015 1015  ...,............
-000005d0: 0200 0000 26ba 051c 150a 1935 1000 0619  ....&......5....
-000005e0: 1802 7261 1502 160e 168c 0216 fa01 26a6  ..ra..........&.
-000005f0: 0426 c003 1c18 0800 0000 0000 d875 4018  .&...........u@.
-00000600: 0800 0000 0000 8874 4016 0028 0800 0000  .......t@..(....
-00000610: 0000 d875 4018 0800 0000 0000 8874 4000  ...u@........t@.
-00000620: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
-00000630: 0000 26f2 081c 150a 1935 1000 0619 1803  ..&......5......
-00000640: 6465 6315 0216 0e16 8c02 16fc 0126 de07  dec..........&..
-00000650: 26f6 061c 1808 0000 0000 00c0 42c0 1808  &...........B...
-00000660: 0000 0000 0040 4ac0 1600 2808 0000 0000  .....@J...(.....
-00000670: 00c0 42c0 1808 0000 0000 0040 4ac0 0019  ..B........@J...
-00000680: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
-00000690: 0026 f00b 1c15 0419 3510 0006 1918 0872  .&......5......r
-000006a0: 615f 6572 726f 7215 0216 0e16 b801 16c0  a_error.........
-000006b0: 0126 e00a 26b0 0a1c 1808 0000 0000 0000  .&..&...........
-000006c0: 0000 1808 0000 0000 0000 0000 1600 2808  ..............(.
-000006d0: 0000 0000 0000 0000 1808 0000 0000 0000  ................
-000006e0: 0000 0019 2c15 0415 0015 0200 1500 1510  ....,...........
-000006f0: 1502 0000 0026 f80e 1c15 0419 3510 0006  .....&......5...
-00000700: 1918 0964 6563 5f65 7272 6f72 1502 160e  ...dec_error....
-00000710: 16b8 0116 c001 26e8 0d26 b80d 1c18 0800  ......&..&......
-00000720: 0000 0000 0000 0018 0800 0000 0000 0000  ................
-00000730: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
-00000740: 0000 0000 0000 0000 192c 1504 1500 1502  .........,......
-00000750: 0015 0015 1015 0200 0000 26c2 121c 1504  ..........&.....
-00000760: 1935 1000 0619 1811 5f5f 696e 6465 785f  .5......__index_
-00000770: 6c65 7665 6c5f 305f 5f15 0216 0e16 9c02  level_0__.......
-00000780: 1680 0226 ae11 26c2 101c 1808 1400 0000  ...&..&.........
-00000790: 0000 0000 1808 0100 0000 0000 0000 1600  ................
-000007a0: 2808 1400 0000 0000 0000 1808 0100 0000  (...............
-000007b0: 0000 0000 0019 2c15 0415 0015 0200 1500  ......,.........
-000007c0: 1510 1502 0000 0016 c00b 160e 2608 16f6  ............&...
-000007d0: 0a14 0000 192c 1806 7061 6e64 6173 18a5  .....,..pandas..
-000007e0: 077b 2269 6e64 6578 5f63 6f6c 756d 6e73  .{"index_columns
-000007f0: 223a 205b 225f 5f69 6e64 6578 5f6c 6576  ": ["__index_lev
-00000800: 656c 5f30 5f5f 225d 2c20 2263 6f6c 756d  el_0__"], "colum
-00000810: 6e5f 696e 6465 7865 7322 3a20 5b7b 226e  n_indexes": [{"n
-00000820: 616d 6522 3a20 6e75 6c6c 2c20 2266 6965  ame": null, "fie
-00000830: 6c64 5f6e 616d 6522 3a20 6e75 6c6c 2c20  ld_name": null, 
-00000840: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
-00000850: 756e 6963 6f64 6522 2c20 226e 756d 7079  unicode", "numpy
-00000860: 5f74 7970 6522 3a20 226f 626a 6563 7422  _type": "object"
-00000870: 2c20 226d 6574 6164 6174 6122 3a20 7b22  , "metadata": {"
-00000880: 656e 636f 6469 6e67 223a 2022 5554 462d  encoding": "UTF-
-00000890: 3822 7d7d 5d2c 2022 636f 6c75 6d6e 7322  8"}}], "columns"
-000008a0: 3a20 5b7b 226e 616d 6522 3a20 2269 6422  : [{"name": "id"
-000008b0: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
-000008c0: 2269 6422 2c20 2270 616e 6461 735f 7479  "id", "pandas_ty
-000008d0: 7065 223a 2022 696e 7436 3422 2c20 226e  pe": "int64", "n
-000008e0: 756d 7079 5f74 7970 6522 3a20 2269 6e74  umpy_type": "int
-000008f0: 3634 222c 2022 6d65 7461 6461 7461 223a  64", "metadata":
-00000900: 206e 756c 6c7d 2c20 7b22 6e61 6d65 223a   null}, {"name":
-00000910: 2022 7261 222c 2022 6669 656c 645f 6e61   "ra", "field_na
-00000920: 6d65 223a 2022 7261 222c 2022 7061 6e64  me": "ra", "pand
-00000930: 6173 5f74 7970 6522 3a20 2266 6c6f 6174  as_type": "float
-00000940: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
-00000950: 223a 2022 666c 6f61 7436 3422 2c20 226d  ": "float64", "m
-00000960: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
-00000970: 207b 226e 616d 6522 3a20 2264 6563 222c   {"name": "dec",
-00000980: 2022 6669 656c 645f 6e61 6d65 223a 2022   "field_name": "
-00000990: 6465 6322 2c20 2270 616e 6461 735f 7479  dec", "pandas_ty
-000009a0: 7065 223a 2022 666c 6f61 7436 3422 2c20  pe": "float64", 
-000009b0: 226e 756d 7079 5f74 7970 6522 3a20 2266  "numpy_type": "f
-000009c0: 6c6f 6174 3634 222c 2022 6d65 7461 6461  loat64", "metada
-000009d0: 7461 223a 206e 756c 6c7d 2c20 7b22 6e61  ta": null}, {"na
-000009e0: 6d65 223a 2022 7261 5f65 7272 6f72 222c  me": "ra_error",
-000009f0: 2022 6669 656c 645f 6e61 6d65 223a 2022   "field_name": "
-00000a00: 7261 5f65 7272 6f72 222c 2022 7061 6e64  ra_error", "pand
-00000a10: 6173 5f74 7970 6522 3a20 2269 6e74 3634  as_type": "int64
-00000a20: 222c 2022 6e75 6d70 795f 7479 7065 223a  ", "numpy_type":
-00000a30: 2022 696e 7436 3422 2c20 226d 6574 6164   "int64", "metad
-00000a40: 6174 6122 3a20 6e75 6c6c 7d2c 207b 226e  ata": null}, {"n
-00000a50: 616d 6522 3a20 2264 6563 5f65 7272 6f72  ame": "dec_error
-00000a60: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
-00000a70: 2022 6465 635f 6572 726f 7222 2c20 2270   "dec_error", "p
-00000a80: 616e 6461 735f 7479 7065 223a 2022 696e  andas_type": "in
-00000a90: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
-00000aa0: 6522 3a20 2269 6e74 3634 222c 2022 6d65  e": "int64", "me
-00000ab0: 7461 6461 7461 223a 206e 756c 6c7d 2c20  tadata": null}, 
-00000ac0: 7b22 6e61 6d65 223a 206e 756c 6c2c 2022  {"name": null, "
-00000ad0: 6669 656c 645f 6e61 6d65 223a 2022 5f5f  field_name": "__
-00000ae0: 696e 6465 785f 6c65 7665 6c5f 305f 5f22  index_level_0__"
-00000af0: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
-00000b00: 2022 696e 7436 3422 2c20 226e 756d 7079   "int64", "numpy
-00000b10: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
-00000b20: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
-00000b30: 6c7d 5d2c 2022 6372 6561 746f 7222 3a20  l}], "creator": 
-00000b40: 7b22 6c69 6272 6172 7922 3a20 2270 7961  {"library": "pya
-00000b50: 7272 6f77 222c 2022 7665 7273 696f 6e22  rrow", "version"
-00000b60: 3a20 2239 2e30 2e30 227d 2c20 2270 616e  : "9.0.0"}, "pan
-00000b70: 6461 735f 7665 7273 696f 6e22 3a20 2231  das_version": "1
-00000b80: 2e33 2e35 227d 0018 0c41 5252 4f57 3a73  .3.5"}...ARROW:s
-00000b90: 6368 656d 6118 c00e 2f2f 2f2f 2f32 6746  chema.../////2gF
-00000ba0: 4141 4151 4141 4141 4141 414b 4141 3441  AAAQAAAAAAAKAA4A
-00000bb0: 4267 4146 4141 6741 4367 4141 4141 4142  BgAFAAgACgAAAAAB
-00000bc0: 4241 4151 4141 4141 4141 414b 4141 7741  BAAQAAAAAAAKAAwA
-00000bd0: 4141 4145 4141 6741 4367 4141 414e 7744  AAAEAAgACgAAANwD
-00000be0: 4141 4145 4141 4141 4151 4141 4141 7741  AAAEAAAAAQAAAAwA
-00000bf0: 4141 4149 4141 7741 4241 4149 4141 6741  AAAIAAwABAAIAAgA
-00000c00: 4141 4149 4141 4141 4541 4141 4141 5941  AAAIAAAAEAAAAAYA
-00000c10: 4141 4277 5957 356b 5958 4d41 414b 5544  AABwYW5kYXMAAKUD
-00000c20: 4141 4237 496d 6c75 5a47 5634 5832 4e76  AAB7ImluZGV4X2Nv
-00000c30: 6248 5674 626e 4d69 4f69 4262 496c 3966  bHVtbnMiOiBbIl9f
-00000c40: 6157 356b 5a58 6866 6247 5632 5a57 7866  aW5kZXhfbGV2ZWxf
-00000c50: 4d46 3966 496c 3073 4943 4a6a 6232 7831  MF9fIl0sICJjb2x1
-00000c60: 6257 3566 6157 356b 5a58 686c 6379 4936  bW5faW5kZXhlcyI6
-00000c70: 4946 7437 496d 3568 6257 5569 4f69 4275  IFt7Im5hbWUiOiBu
-00000c80: 6457 7873 4c43 4169 5a6d 6c6c 6247 5266  dWxsLCAiZmllbGRf
-00000c90: 626d 4674 5a53 4936 4947 3531 6247 7773  bmFtZSI6IG51bGws
-00000ca0: 4943 4a77 5957 356b 5958 4e66 6448 6c77  ICJwYW5kYXNfdHlw
-00000cb0: 5a53 4936 4943 4a31 626d 6c6a 6232 526c  ZSI6ICJ1bmljb2Rl
-00000cc0: 4969 7767 496d 3531 6258 4235 5833 5235  IiwgIm51bXB5X3R5
-00000cd0: 6347 5569 4f69 4169 6232 4a71 5a57 4e30  cGUiOiAib2JqZWN0
-00000ce0: 4969 7767 496d 316c 6447 466b 5958 5268  IiwgIm1ldGFkYXRh
-00000cf0: 496a 6f67 6579 4a6c 626d 4e76 5a47 6c75  IjogeyJlbmNvZGlu
-00000d00: 5a79 4936 4943 4a56 5645 5974 4f43 4a39  ZyI6ICJVVEYtOCJ9
-00000d10: 6656 3073 4943 4a6a 6232 7831 6257 357a  fV0sICJjb2x1bW5z
-00000d20: 496a 6f67 5733 7369 626d 4674 5a53 4936  IjogW3sibmFtZSI6
-00000d30: 4943 4a70 5a43 4973 4943 4a6d 6157 5673  ICJpZCIsICJmaWVs
-00000d40: 5a46 3975 5957 316c 496a 6f67 496d 6c6b  ZF9uYW1lIjogImlk
-00000d50: 4969 7767 496e 4268 626d 5268 6331 3930  IiwgInBhbmRhc190
-00000d60: 6558 426c 496a 6f67 496d 6c75 6444 5930  eXBlIjogImludDY0
-00000d70: 4969 7767 496d 3531 6258 4235 5833 5235  IiwgIm51bXB5X3R5
-00000d80: 6347 5569 4f69 4169 6157 3530 4e6a 5169  cGUiOiAiaW50NjQi
-00000d90: 4c43 4169 6257 5630 5957 5268 6447 4569  LCAibWV0YWRhdGEi
-00000da0: 4f69 4275 6457 7873 6653 7767 6579 4a75  OiBudWxsfSwgeyJu
-00000db0: 5957 316c 496a 6f67 496e 4a68 4969 7767  YW1lIjogInJhIiwg
-00000dc0: 496d 5a70 5a57 786b 5832 3568 6257 5569  ImZpZWxkX25hbWUi
-00000dd0: 4f69 4169 636d 4569 4c43 4169 6347 4675  OiAicmEiLCAicGFu
-00000de0: 5a47 467a 5833 5235 6347 5569 4f69 4169  ZGFzX3R5cGUiOiAi
-00000df0: 5a6d 7876 5958 5132 4e43 4973 4943 4a75  ZmxvYXQ2NCIsICJu
-00000e00: 6457 3177 6556 3930 6558 426c 496a 6f67  dW1weV90eXBlIjog
-00000e10: 496d 5a73 6232 4630 4e6a 5169 4c43 4169  ImZsb2F0NjQiLCAi
-00000e20: 6257 5630 5957 5268 6447 4569 4f69 4275  bWV0YWRhdGEiOiBu
-00000e30: 6457 7873 6653 7767 6579 4a75 5957 316c  dWxsfSwgeyJuYW1l
-00000e40: 496a 6f67 496d 526c 5979 4973 4943 4a6d  IjogImRlYyIsICJm
-00000e50: 6157 5673 5a46 3975 5957 316c 496a 6f67  aWVsZF9uYW1lIjog
-00000e60: 496d 526c 5979 4973 4943 4a77 5957 356b  ImRlYyIsICJwYW5k
-00000e70: 5958 4e66 6448 6c77 5a53 4936 4943 4a6d  YXNfdHlwZSI6ICJm
-00000e80: 6247 3968 6444 5930 4969 7767 496d 3531  bG9hdDY0IiwgIm51
-00000e90: 6258 4235 5833 5235 6347 5569 4f69 4169  bXB5X3R5cGUiOiAi
-00000ea0: 5a6d 7876 5958 5132 4e43 4973 4943 4a74  ZmxvYXQ2NCIsICJt
-00000eb0: 5a58 5268 5a47 4630 5953 4936 4947 3531  ZXRhZGF0YSI6IG51
-00000ec0: 6247 7839 4c43 4237 496d 3568 6257 5569  bGx9LCB7Im5hbWUi
-00000ed0: 4f69 4169 636d 4666 5a58 4a79 6233 4969  OiAicmFfZXJyb3Ii
-00000ee0: 4c43 4169 5a6d 6c6c 6247 5266 626d 4674  LCAiZmllbGRfbmFt
-00000ef0: 5a53 4936 4943 4a79 5956 396c 636e 4a76  ZSI6ICJyYV9lcnJv
-00000f00: 6369 4973 4943 4a77 5957 356b 5958 4e66  ciIsICJwYW5kYXNf
-00000f10: 6448 6c77 5a53 4936 4943 4a70 626e 5132  dHlwZSI6ICJpbnQ2
-00000f20: 4e43 4973 4943 4a75 6457 3177 6556 3930  NCIsICJudW1weV90
-00000f30: 6558 426c 496a 6f67 496d 6c75 6444 5930  eXBlIjogImludDY0
-00000f40: 4969 7767 496d 316c 6447 466b 5958 5268  IiwgIm1ldGFkYXRh
-00000f50: 496a 6f67 626e 5673 6248 3073 4948 7369  IjogbnVsbH0sIHsi
-00000f60: 626d 4674 5a53 4936 4943 4a6b 5a57 4e66  bmFtZSI6ICJkZWNf
-00000f70: 5a58 4a79 6233 4969 4c43 4169 5a6d 6c6c  ZXJyb3IiLCAiZmll
-00000f80: 6247 5266 626d 4674 5a53 4936 4943 4a6b  bGRfbmFtZSI6ICJk
-00000f90: 5a57 4e66 5a58 4a79 6233 4969 4c43 4169  ZWNfZXJyb3IiLCAi
-00000fa0: 6347 4675 5a47 467a 5833 5235 6347 5569  cGFuZGFzX3R5cGUi
-00000fb0: 4f69 4169 6157 3530 4e6a 5169 4c43 4169  OiAiaW50NjQiLCAi
-00000fc0: 626e 5674 6348 6c66 6448 6c77 5a53 4936  bnVtcHlfdHlwZSI6
-00000fd0: 4943 4a70 626e 5132 4e43 4973 4943 4a74  ICJpbnQ2NCIsICJt
-00000fe0: 5a58 5268 5a47 4630 5953 4936 4947 3531  ZXRhZGF0YSI6IG51
-00000ff0: 6247 7839 4c43 4237 496d 3568 6257 5569  bGx9LCB7Im5hbWUi
-00001000: 4f69 4275 6457 7873 4c43 4169 5a6d 6c6c  OiBudWxsLCAiZmll
-00001010: 6247 5266 626d 4674 5a53 4936 4943 4a66  bGRfbmFtZSI6ICJf
-00001020: 5832 6c75 5a47 5634 5832 786c 646d 5673  X2luZGV4X2xldmVs
-00001030: 587a 4266 5879 4973 4943 4a77 5957 356b  XzBfXyIsICJwYW5k
-00001040: 5958 4e66 6448 6c77 5a53 4936 4943 4a70  YXNfdHlwZSI6ICJp
-00001050: 626e 5132 4e43 4973 4943 4a75 6457 3177  bnQ2NCIsICJudW1w
-00001060: 6556 3930 6558 426c 496a 6f67 496d 6c75  eV90eXBlIjogImlu
-00001070: 6444 5930 4969 7767 496d 316c 6447 466b  dDY0IiwgIm1ldGFk
-00001080: 5958 5268 496a 6f67 626e 5673 6248 3164  YXRhIjogbnVsbH1d
-00001090: 4c43 4169 5933 4a6c 5958 5276 6369 4936  LCAiY3JlYXRvciI6
-000010a0: 4948 7369 6247 6c69 636d 4679 6553 4936  IHsibGlicmFyeSI6
-000010b0: 4943 4a77 6557 4679 636d 3933 4969 7767  ICJweWFycm93Iiwg
-000010c0: 496e 5a6c 636e 4e70 6232 3469 4f69 4169  InZlcnNpb24iOiAi
-000010d0: 4f53 3477 4c6a 4169 6653 7767 496e 4268  OS4wLjAifSwgInBh
-000010e0: 626d 5268 6331 3932 5a58 4a7a 6157 3975  bmRhc192ZXJzaW9u
-000010f0: 496a 6f67 496a 4575 4d79 3431 496e 3041  IjogIjEuMy41In0A
-00001100: 4141 4147 4141 4141 4a41 4541 414f 4141  AAAGAAAAJAEAAOAA
-00001110: 4141 4330 4141 4141 6641 4141 4145 5141  AAC0AAAAfAAAAEQA
-00001120: 4141 4145 4141 4141 4250 2f2f 2f77 4141  AAAEAAAABP///wAA
-00001130: 4151 4951 4141 4141 4a41 4141 4141 5141  AQIQAAAAJAAAAAQA
-00001140: 4141 4141 4141 4141 4551 4141 4146 3966  AAAAAAAAEQAAAF9f
-00001150: 6157 356b 5a58 6866 6247 5632 5a57 7866  aW5kZXhfbGV2ZWxf
-00001160: 4d46 3966 4141 4141 4250 2f2f 2f77 4141  MF9fAAAABP///wAA
-00001170: 4141 4641 4141 4141 5150 2f2f 2f77 4141  AAFAAAAAQP///wAA
-00001180: 4151 4951 4141 4141 4841 4141 4141 5141  AQIQAAAAHAAAAAQA
-00001190: 4141 4141 4141 4141 4351 4141 4147 526c  AAAAAAAACQAAAGRl
-000011a0: 5931 396c 636e 4a76 6367 4141 4144 6a2f  Y19lcnJvcgAAADj/
-000011b0: 2f2f 3841 4141 4142 5141 4141 4148 542f  //8AAAABQAAAAHT/
-000011c0: 2f2f 3841 4141 4543 4541 4141 4142 7741  //8AAAECEAAAABwA
-000011d0: 4141 4145 4141 4141 4141 4141 4141 6741  AAAEAAAAAAAAAAgA
-000011e0: 4141 4279 5956 396c 636e 4a76 6367 4141  AAByYV9lcnJvcgAA
-000011f0: 4141 4273 2f2f 2f2f 4141 4141 4155 4141  AABs////AAAAAUAA
-00001200: 4141 436f 2f2f 2f2f 4141 4142 4178 4141  AACo////AAABAxAA
-00001210: 4141 4155 4141 4141 4241 4141 4141 4141  AAAUAAAABAAAAAAA
-00001220: 4141 4144 4141 4141 5a47 566a 414e 622f  AAADAAAAZGVjANb/
-00001230: 2f2f 3841 4141 4941 3050 2f2f 2f77 4141  //8AAAIA0P///wAA
-00001240: 4151 4d51 4141 4141 4841 4141 4141 5141  AQMQAAAAHAAAAAQA
-00001250: 4141 4141 4141 4141 4167 4141 4148 4a68  AAAAAAAAAgAAAHJh
-00001260: 4141 4141 4141 5941 4341 4147 4141 5941  AAAAAAYACAAGAAYA
-00001270: 4141 4141 4141 4941 4541 4155 4141 6741  AAAAAAIAEAAUAAgA
-00001280: 4267 4148 4141 7741 4141 4151 4142 4141  BgAHAAwAAAAQABAA
-00001290: 4141 4141 4141 4543 4541 4141 4142 7741  AAAAAAECEAAAABwA
-000012a0: 4141 4145 4141 4141 4141 4141 4141 4941  AAAEAAAAAAAAAAIA
-000012b0: 4141 4270 5a41 4141 4341 414d 4141 6741  AABpZAAACAAMAAgA
-000012c0: 4277 4149 4141 4141 4141 4141 4155 4141  BwAIAAAAAAAAAUAA
-000012d0: 4141 4141 4141 4141 0018 1f70 6172 7175  AAAAAAAA...parqu
-000012e0: 6574 2d63 7070 2d61 7272 6f77 2076 6572  et-cpp-arrow ver
-000012f0: 7369 6f6e 2039 2e30 2e30 196c 1c00 001c  sion 9.0.0.l....
-00001300: 0000 1c00 001c 0000 1c00 001c 0000 0001  ................
-00001310: 0e00 0050 4152 31                        ...PAR1
+00000420: 0015 0419 6c35 0018 0673 6368 656d 6115  ....l5...schema.
+00000430: 0a00 1504 2502 1802 6964 0015 0a25 0218  ....%...id...%..
+00000440: 0272 6100 150a 2502 1803 6465 6300 1504  .ra...%...dec...
+00000450: 2502 1808 7261 5f65 7272 6f72 0015 0425  %...ra_error...%
+00000460: 0218 0964 6563 5f65 7272 6f72 0016 0e19  ...dec_error....
+00000470: 1c19 5c26 8802 1c15 0419 3510 0006 1918  ..\&......5.....
+00000480: 0269 6415 0216 0e16 9c02 1680 0226 7426  .id..........&t&
+00000490: 081c 1808 e902 0000 0000 0000 1808 d602  ................
+000004a0: 0000 0000 0000 1600 2808 e902 0000 0000  ........(.......
+000004b0: 0000 1808 d602 0000 0000 0000 0019 2c15  ..............,.
+000004c0: 0415 0015 0200 1500 1510 1502 0000 0026  ...............&
+000004d0: ba05 1c15 0a19 3510 0006 1918 0272 6115  ......5......ra.
+000004e0: 0216 0e16 8c02 16fa 0126 a604 26c0 031c  .........&..&...
+000004f0: 1808 0000 0000 00d8 7540 1808 0000 0000  ........u@......
+00000500: 0088 7440 1600 2808 0000 0000 00d8 7540  ..t@..(.......u@
+00000510: 1808 0000 0000 0088 7440 0019 2c15 0415  ........t@..,...
+00000520: 0015 0200 1500 1510 1502 0000 0026 f208  .............&..
+00000530: 1c15 0a19 3510 0006 1918 0364 6563 1502  ....5......dec..
+00000540: 160e 168c 0216 fc01 26de 0726 f606 1c18  ........&..&....
+00000550: 0800 0000 0000 c042 c018 0800 0000 0000  .......B........
+00000560: 404a c016 0028 0800 0000 0000 c042 c018  @J...(.......B..
+00000570: 0800 0000 0000 404a c000 192c 1504 1500  ......@J...,....
+00000580: 1502 0015 0015 1015 0200 0000 26f0 0b1c  ............&...
+00000590: 1504 1935 1000 0619 1808 7261 5f65 7272  ...5......ra_err
+000005a0: 6f72 1502 160e 16b8 0116 c001 26e0 0a26  or..........&..&
+000005b0: b00a 1c18 0800 0000 0000 0000 0018 0800  ................
+000005c0: 0000 0000 0000 0016 0028 0800 0000 0000  .........(......
+000005d0: 0000 0018 0800 0000 0000 0000 0000 192c  ...............,
+000005e0: 1504 1500 1502 0015 0015 1015 0200 0000  ................
+000005f0: 26f8 0e1c 1504 1935 1000 0619 1809 6465  &......5......de
+00000600: 635f 6572 726f 7215 0216 0e16 b801 16c0  c_error.........
+00000610: 0126 e80d 26b8 0d1c 1808 0000 0000 0000  .&..&...........
+00000620: 0000 1808 0000 0000 0000 0000 1600 2808  ..............(.
+00000630: 0000 0000 0000 0000 1808 0000 0000 0000  ................
+00000640: 0000 0019 2c15 0415 0015 0200 1500 1510  ....,...........
+00000650: 1502 0000 0016 a409 160e 2608 16f6 0814  ..........&.....
+00000660: 0000 192c 1806 7061 6e64 6173 18a7 057b  ...,..pandas...{
+00000670: 2269 6e64 6578 5f63 6f6c 756d 6e73 223a  "index_columns":
+00000680: 205b 5d2c 2022 636f 6c75 6d6e 5f69 6e64   [], "column_ind
+00000690: 6578 6573 223a 205b 5d2c 2022 636f 6c75  exes": [], "colu
+000006a0: 6d6e 7322 3a20 5b7b 226e 616d 6522 3a20  mns": [{"name": 
+000006b0: 2269 6422 2c20 2266 6965 6c64 5f6e 616d  "id", "field_nam
+000006c0: 6522 3a20 2269 6422 2c20 2270 616e 6461  e": "id", "panda
+000006d0: 735f 7479 7065 223a 2022 696e 7436 3422  s_type": "int64"
+000006e0: 2c20 226e 756d 7079 5f74 7970 6522 3a20  , "numpy_type": 
+000006f0: 2269 6e74 3634 222c 2022 6d65 7461 6461  "int64", "metada
+00000700: 7461 223a 206e 756c 6c7d 2c20 7b22 6e61  ta": null}, {"na
+00000710: 6d65 223a 2022 7261 222c 2022 6669 656c  me": "ra", "fiel
+00000720: 645f 6e61 6d65 223a 2022 7261 222c 2022  d_name": "ra", "
+00000730: 7061 6e64 6173 5f74 7970 6522 3a20 2266  pandas_type": "f
+00000740: 6c6f 6174 3634 222c 2022 6e75 6d70 795f  loat64", "numpy_
+00000750: 7479 7065 223a 2022 666c 6f61 7436 3422  type": "float64"
+00000760: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
+00000770: 6c6c 7d2c 207b 226e 616d 6522 3a20 2264  ll}, {"name": "d
+00000780: 6563 222c 2022 6669 656c 645f 6e61 6d65  ec", "field_name
+00000790: 223a 2022 6465 6322 2c20 2270 616e 6461  ": "dec", "panda
+000007a0: 735f 7479 7065 223a 2022 666c 6f61 7436  s_type": "float6
+000007b0: 3422 2c20 226e 756d 7079 5f74 7970 6522  4", "numpy_type"
+000007c0: 3a20 2266 6c6f 6174 3634 222c 2022 6d65  : "float64", "me
+000007d0: 7461 6461 7461 223a 206e 756c 6c7d 2c20  tadata": null}, 
+000007e0: 7b22 6e61 6d65 223a 2022 7261 5f65 7272  {"name": "ra_err
+000007f0: 6f72 222c 2022 6669 656c 645f 6e61 6d65  or", "field_name
+00000800: 223a 2022 7261 5f65 7272 6f72 222c 2022  ": "ra_error", "
+00000810: 7061 6e64 6173 5f74 7970 6522 3a20 2269  pandas_type": "i
+00000820: 6e74 3634 222c 2022 6e75 6d70 795f 7479  nt64", "numpy_ty
+00000830: 7065 223a 2022 696e 7436 3422 2c20 226d  pe": "int64", "m
+00000840: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
+00000850: 207b 226e 616d 6522 3a20 2264 6563 5f65   {"name": "dec_e
+00000860: 7272 6f72 222c 2022 6669 656c 645f 6e61  rror", "field_na
+00000870: 6d65 223a 2022 6465 635f 6572 726f 7222  me": "dec_error"
+00000880: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
+00000890: 2022 696e 7436 3422 2c20 226e 756d 7079   "int64", "numpy
+000008a0: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
+000008b0: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
+000008c0: 6c7d 5d2c 2022 6372 6561 746f 7222 3a20  l}], "creator": 
+000008d0: 7b22 6c69 6272 6172 7922 3a20 2270 7961  {"library": "pya
+000008e0: 7272 6f77 222c 2022 7665 7273 696f 6e22  rrow", "version"
+000008f0: 3a20 2239 2e30 2e30 227d 2c20 2270 616e  : "9.0.0"}, "pan
+00000900: 6461 735f 7665 7273 696f 6e22 3a20 2232  das_version": "2
+00000910: 2e30 2e30 227d 0018 0c41 5252 4f57 3a73  .0.0"}...ARROW:s
+00000920: 6368 656d 6118 980b 2f2f 2f2f 2f79 6745  chema.../////ygE
+00000930: 4141 4151 4141 4141 4141 414b 4141 3441  AAAQAAAAAAAKAA4A
+00000940: 4267 4146 4141 6741 4367 4141 4141 4142  BgAFAAgACgAAAAAB
+00000950: 4241 4151 4141 4141 4141 414b 4141 7741  BAAQAAAAAAAKAAwA
+00000960: 4141 4145 4141 6741 4367 4141 414e 7743  AAAEAAgACgAAANwC
+00000970: 4141 4145 4141 4141 4151 4141 4141 7741  AAAEAAAAAQAAAAwA
+00000980: 4141 4149 4141 7741 4241 4149 4141 6741  AAAIAAwABAAIAAgA
+00000990: 4141 4149 4141 4141 4541 4141 4141 5941  AAAIAAAAEAAAAAYA
+000009a0: 4141 4277 5957 356b 5958 4d41 414b 6343  AABwYW5kYXMAAKcC
+000009b0: 4141 4237 496d 6c75 5a47 5634 5832 4e76  AAB7ImluZGV4X2Nv
+000009c0: 6248 5674 626e 4d69 4f69 4262 5853 7767  bHVtbnMiOiBbXSwg
+000009d0: 496d 4e76 6248 5674 626c 3970 626d 526c  ImNvbHVtbl9pbmRl
+000009e0: 6547 567a 496a 6f67 5731 3073 4943 4a6a  eGVzIjogW10sICJj
+000009f0: 6232 7831 6257 357a 496a 6f67 5733 7369  b2x1bW5zIjogW3si
+00000a00: 626d 4674 5a53 4936 4943 4a70 5a43 4973  bmFtZSI6ICJpZCIs
+00000a10: 4943 4a6d 6157 5673 5a46 3975 5957 316c  ICJmaWVsZF9uYW1l
+00000a20: 496a 6f67 496d 6c6b 4969 7767 496e 4268  IjogImlkIiwgInBh
+00000a30: 626d 5268 6331 3930 6558 426c 496a 6f67  bmRhc190eXBlIjog
+00000a40: 496d 6c75 6444 5930 4969 7767 496d 3531  ImludDY0IiwgIm51
+00000a50: 6258 4235 5833 5235 6347 5569 4f69 4169  bXB5X3R5cGUiOiAi
+00000a60: 6157 3530 4e6a 5169 4c43 4169 6257 5630  aW50NjQiLCAibWV0
+00000a70: 5957 5268 6447 4569 4f69 4275 6457 7873  YWRhdGEiOiBudWxs
+00000a80: 6653 7767 6579 4a75 5957 316c 496a 6f67  fSwgeyJuYW1lIjog
+00000a90: 496e 4a68 4969 7767 496d 5a70 5a57 786b  InJhIiwgImZpZWxk
+00000aa0: 5832 3568 6257 5569 4f69 4169 636d 4569  X25hbWUiOiAicmEi
+00000ab0: 4c43 4169 6347 4675 5a47 467a 5833 5235  LCAicGFuZGFzX3R5
+00000ac0: 6347 5569 4f69 4169 5a6d 7876 5958 5132  cGUiOiAiZmxvYXQ2
+00000ad0: 4e43 4973 4943 4a75 6457 3177 6556 3930  NCIsICJudW1weV90
+00000ae0: 6558 426c 496a 6f67 496d 5a73 6232 4630  eXBlIjogImZsb2F0
+00000af0: 4e6a 5169 4c43 4169 6257 5630 5957 5268  NjQiLCAibWV0YWRh
+00000b00: 6447 4569 4f69 4275 6457 7873 6653 7767  dGEiOiBudWxsfSwg
+00000b10: 6579 4a75 5957 316c 496a 6f67 496d 526c  eyJuYW1lIjogImRl
+00000b20: 5979 4973 4943 4a6d 6157 5673 5a46 3975  YyIsICJmaWVsZF9u
+00000b30: 5957 316c 496a 6f67 496d 526c 5979 4973  YW1lIjogImRlYyIs
+00000b40: 4943 4a77 5957 356b 5958 4e66 6448 6c77  ICJwYW5kYXNfdHlw
+00000b50: 5a53 4936 4943 4a6d 6247 3968 6444 5930  ZSI6ICJmbG9hdDY0
+00000b60: 4969 7767 496d 3531 6258 4235 5833 5235  IiwgIm51bXB5X3R5
+00000b70: 6347 5569 4f69 4169 5a6d 7876 5958 5132  cGUiOiAiZmxvYXQ2
+00000b80: 4e43 4973 4943 4a74 5a58 5268 5a47 4630  NCIsICJtZXRhZGF0
+00000b90: 5953 4936 4947 3531 6247 7839 4c43 4237  YSI6IG51bGx9LCB7
+00000ba0: 496d 3568 6257 5569 4f69 4169 636d 4666  Im5hbWUiOiAicmFf
+00000bb0: 5a58 4a79 6233 4969 4c43 4169 5a6d 6c6c  ZXJyb3IiLCAiZmll
+00000bc0: 6247 5266 626d 4674 5a53 4936 4943 4a79  bGRfbmFtZSI6ICJy
+00000bd0: 5956 396c 636e 4a76 6369 4973 4943 4a77  YV9lcnJvciIsICJw
+00000be0: 5957 356b 5958 4e66 6448 6c77 5a53 4936  YW5kYXNfdHlwZSI6
+00000bf0: 4943 4a70 626e 5132 4e43 4973 4943 4a75  ICJpbnQ2NCIsICJu
+00000c00: 6457 3177 6556 3930 6558 426c 496a 6f67  dW1weV90eXBlIjog
+00000c10: 496d 6c75 6444 5930 4969 7767 496d 316c  ImludDY0IiwgIm1l
+00000c20: 6447 466b 5958 5268 496a 6f67 626e 5673  dGFkYXRhIjogbnVs
+00000c30: 6248 3073 4948 7369 626d 4674 5a53 4936  bH0sIHsibmFtZSI6
+00000c40: 4943 4a6b 5a57 4e66 5a58 4a79 6233 4969  ICJkZWNfZXJyb3Ii
+00000c50: 4c43 4169 5a6d 6c6c 6247 5266 626d 4674  LCAiZmllbGRfbmFt
+00000c60: 5a53 4936 4943 4a6b 5a57 4e66 5a58 4a79  ZSI6ICJkZWNfZXJy
+00000c70: 6233 4969 4c43 4169 6347 4675 5a47 467a  b3IiLCAicGFuZGFz
+00000c80: 5833 5235 6347 5569 4f69 4169 6157 3530  X3R5cGUiOiAiaW50
+00000c90: 4e6a 5169 4c43 4169 626e 5674 6348 6c66  NjQiLCAibnVtcHlf
+00000ca0: 6448 6c77 5a53 4936 4943 4a70 626e 5132  dHlwZSI6ICJpbnQ2
+00000cb0: 4e43 4973 4943 4a74 5a58 5268 5a47 4630  NCIsICJtZXRhZGF0
+00000cc0: 5953 4936 4947 3531 6247 7839 5853 7767  YSI6IG51bGx9XSwg
+00000cd0: 496d 4e79 5a57 4630 6233 4969 4f69 4237  ImNyZWF0b3IiOiB7
+00000ce0: 496d 7870 596e 4a68 636e 6b69 4f69 4169  ImxpYnJhcnkiOiAi
+00000cf0: 6348 6c68 636e 4a76 6479 4973 4943 4a32  cHlhcnJvdyIsICJ2
+00000d00: 5a58 4a7a 6157 3975 496a 6f67 496a 6b75  ZXJzaW9uIjogIjku
+00000d10: 4d43 3477 496e 3073 4943 4a77 5957 356b  MC4wIn0sICJwYW5k
+00000d20: 5958 4e66 646d 5679 6332 6c76 6269 4936  YXNfdmVyc2lvbiI6
+00000d30: 4943 4979 4c6a 4175 4d43 4a39 4141 5541  ICIyLjAuMCJ9AAUA
+00000d40: 4141 446b 4141 4141 6f41 4141 4148 5141  AADkAAAAoAAAAHQA
+00000d50: 4141 4138 4141 4141 4241 4141 4145 442f  AAA8AAAABAAAAED/
+00000d60: 2f2f 3841 4141 4543 4541 4141 4142 7741  //8AAAECEAAAABwA
+00000d70: 4141 4145 4141 4141 4141 4141 4141 6b41  AAAEAAAAAAAAAAkA
+00000d80: 4141 426b 5a57 4e66 5a58 4a79 6233 4941  AABkZWNfZXJyb3IA
+00000d90: 4141 4134 2f2f 2f2f 4141 4141 4155 4141  AAA4////AAAAAUAA
+00000da0: 4141 4230 2f2f 2f2f 4141 4142 4168 4141  AAB0////AAABAhAA
+00000db0: 4141 4163 4141 4141 4241 4141 4141 4141  AAAcAAAABAAAAAAA
+00000dc0: 4141 4149 4141 4141 636d 4666 5a58 4a79  AAAIAAAAcmFfZXJy
+00000dd0: 6233 4941 4141 4141 6250 2f2f 2f77 4141  b3IAAAAAbP///wAA
+00000de0: 4141 4641 4141 4141 7150 2f2f 2f77 4141  AAFAAAAAqP///wAA
+00000df0: 4151 4d51 4141 4141 4641 4141 4141 5141  AQMQAAAAFAAAAAQA
+00000e00: 4141 4141 4141 4141 4177 4141 4147 526c  AAAAAAAAAwAAAGRl
+00000e10: 5977 4457 2f2f 2f2f 4141 4143 414e 442f  YwDW////AAACAND/
+00000e20: 2f2f 3841 4141 4544 4541 4141 4142 7741  //8AAAEDEAAAABwA
+00000e30: 4141 4145 4141 4141 4141 4141 4141 4941  AAAEAAAAAAAAAAIA
+00000e40: 4141 4279 5951 4141 4141 4147 4141 6741  AAByYQAAAAAGAAgA
+00000e50: 4267 4147 4141 4141 4141 4143 4142 4141  BgAGAAAAAAACABAA
+00000e60: 4641 4149 4141 5941 4277 414d 4141 4141  FAAIAAYABwAMAAAA
+00000e70: 4541 4151 4141 4141 4141 4142 4168 4141  EAAQAAAAAAABAhAA
+00000e80: 4141 4163 4141 4141 4241 4141 4141 4141  AAAcAAAABAAAAAAA
+00000e90: 4141 4143 4141 4141 6157 5141 4141 6741  AAACAAAAaWQAAAgA
+00000ea0: 4441 4149 4141 6341 4341 4141 4141 4141  DAAIAAcACAAAAAAA
+00000eb0: 4141 4641 4141 4141 4141 4141 4141 3d3d  AAFAAAAAAAAAAA==
+00000ec0: 0018 1f70 6172 7175 6574 2d63 7070 2d61  ...parquet-cpp-a
+00000ed0: 7272 6f77 2076 6572 7369 6f6e 2039 2e30  rrow version 9.0
+00000ee0: 2e30 195c 1c00 001c 0000 1c00 001c 0000  .0.\............
+00000ef0: 1c00 0000 d30a 0000 5041 5231            ........PAR1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_45/shard_4.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet`

 * *Files 21% similar despite different names*

```diff
@@ -1,306 +1,244 @@
-00000000: 5041 5231 1504 1570 1550 4c15 0e15 0012  PAR1...p.PL.....
-00000010: 0000 3808 2303 0005 0100 280d 0800 2c0d  ..8.#.....(...,.
-00000020: 0800 2d0d 0800 350d 083c 3703 0000 0000  ..-...5..<7.....
-00000030: 0000 3c03 0000 0000 0000 1500 1516 151a  ..<.............
-00000040: 2c15 0e15 1015 0615 061c 1808 3c03 0000  ,...........<...
-00000050: 0000 0000 1808 2303 0000 0000 0000 1600  ......#.........
-00000060: 2808 3c03 0000 0000 0000 1808 2303 0000  (.<.........#...
-00000070: 0000 0000 0000 000b 2802 0000 000e 0103  ........(.......
-00000080: 0388 c61a 2688 021c 1504 1935 1000 0619  ....&......5....
-00000090: 1802 6964 1502 160e 169c 0216 8002 2674  ..id..........&t
-000000a0: 2608 1c18 083c 0300 0000 0000 0018 0823  &....<.........#
-000000b0: 0300 0000 0000 0016 0028 083c 0300 0000  .........(.<....
-000000c0: 0000 0018 0823 0300 0000 0000 0000 192c  .....#.........,
-000000d0: 1504 1500 1502 0015 0015 1015 0200 0000  ................
-000000e0: 1504 1560 154a 4c15 0c15 0012 0000 3000  ...`.JL.......0.
-000000f0: 0001 0108 0875 4001 0708 0008 7409 0800  .....u@.....t...
-00000100: a80d 1000 d80d 0828 a874 4000 0000 0000  .......(.t@.....
-00000110: 2875 4015 0015 1615 1a2c 150e 1510 1506  (u@......,......
-00000120: 1506 1c18 0800 0000 0000 d875 4018 0800  ...........u@...
-00000130: 0000 0000 0874 4016 0028 0800 0000 0000  .....t@..(......
-00000140: d875 4018 0800 0000 0000 0874 4000 0000  .u@........t@...
-00000150: 0b28 0200 0000 0e01 0303 88c6 1226 ba05  .(...........&..
-00000160: 1c15 0a19 3510 0006 1918 0272 6115 0216  ....5......ra...
-00000170: 0e16 8c02 16fa 0126 a604 26c0 031c 1808  .......&..&.....
-00000180: 0000 0000 00d8 7540 1808 0000 0000 0008  ......u@........
-00000190: 7440 1600 2808 0000 0000 00d8 7540 1808  t@..(.......u@..
-000001a0: 0000 0000 0008 7440 0019 2c15 0415 0015  ......t@..,.....
-000001b0: 0200 1500 1510 1502 0000 0015 0415 7015  ..............p.
-000001c0: 564c 150e 1500 1200 0038 0000 0101 0880  VL.......8......
-000001d0: 39c0 0107 0800 4044 0d08 004e 0908 04c0  9.....@D...N....
-000001e0: 4209 0804 404a 0908 28c0 46c0 0000 0000  B...@J..(.F.....
-000001f0: 0080 3ac0 1500 1516 151a 2c15 0e15 1015  ..:.......,.....
-00000200: 0615 061c 1808 0000 0000 0080 39c0 1808  ............9...
-00000210: 0000 0000 0040 4ec0 1600 2808 0000 0000  .....@N...(.....
-00000220: 0080 39c0 1808 0000 0000 0040 4ec0 0000  ..9........@N...
-00000230: 000b 2802 0000 000e 0103 0388 c61a 26fc  ..(...........&.
-00000240: 081c 150a 1935 1000 0619 1803 6465 6315  .....5......dec.
-00000250: 0216 0e16 9c02 1686 0226 e807 26f6 061c  .........&..&...
-00000260: 1808 0000 0000 0080 39c0 1808 0000 0000  ........9.......
-00000270: 0040 4ec0 1600 2808 0000 0000 0080 39c0  .@N...(.......9.
-00000280: 1808 0000 0000 0040 4ec0 0019 2c15 0415  .......@N...,...
-00000290: 0015 0200 1500 1510 1502 0000 0015 0415  ................
-000002a0: 1015 144c 1502 1500 1200 0008 1c00 0000  ...L............
-000002b0: 0000 0000 0015 0015 1215 162c 150e 1510  ...........,....
-000002c0: 1506 1506 1c18 0800 0000 0000 0000 0018  ................
-000002d0: 0800 0000 0000 0000 0016 0028 0800 0000  ...........(....
-000002e0: 0000 0000 0018 0800 0000 0000 0000 0000  ................
-000002f0: 0000 0920 0200 0000 0e01 010e 0026 fa0b  ... .........&..
-00000300: 1c15 0419 3510 0006 1918 0872 615f 6572  ....5......ra_er
-00000310: 726f 7215 0216 0e16 b801 16c0 0126 ea0a  ror..........&..
-00000320: 26ba 0a1c 1808 0000 0000 0000 0000 1808  &...............
-00000330: 0000 0000 0000 0000 1600 2808 0000 0000  ..........(.....
-00000340: 0000 0000 1808 0000 0000 0000 0000 0019  ................
-00000350: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
-00000360: 0015 0415 1015 144c 1502 1500 1200 0008  .......L........
-00000370: 1c00 0000 0000 0000 0015 0015 1215 162c  ...............,
-00000380: 150e 1510 1506 1506 1c18 0800 0000 0000  ................
-00000390: 0000 0018 0800 0000 0000 0000 0016 0028  ...............(
-000003a0: 0800 0000 0000 0000 0018 0800 0000 0000  ................
-000003b0: 0000 0000 0000 0920 0200 0000 0e01 010e  ....... ........
-000003c0: 0026 820f 1c15 0419 3510 0006 1918 0964  .&......5......d
-000003d0: 6563 5f65 7272 6f72 1502 160e 16b8 0116  ec_error........
-000003e0: c001 26f2 0d26 c20d 1c18 0800 0000 0000  ..&..&..........
-000003f0: 0000 0018 0800 0000 0000 0000 0016 0028  ...............(
-00000400: 0800 0000 0000 0000 0018 0800 0000 0000  ................
-00000410: 0000 0000 192c 1504 1500 1502 0015 0015  .....,..........
-00000420: 1015 0200 0000 1504 1570 154c 4c15 0e15  .........p.LL...
-00000430: 0012 0000 3800 000d 0100 050d 0800 090d  ....8...........
-00000440: 0800 0a0d 0800 120d 083c 1400 0000 0000  .........<......
-00000450: 0000 1900 0000 0000 0000 1500 1516 151a  ................
-00000460: 2c15 0e15 1015 0615 061c 1808 1900 0000  ,...............
-00000470: 0000 0000 1808 0000 0000 0000 0000 1600  ................
-00000480: 2808 1900 0000 0000 0000 1808 0000 0000  (...............
-00000490: 0000 0000 0000 000b 2802 0000 000e 0103  ........(.......
-000004a0: 0388 c61a 26c8 121c 1504 1935 1000 0619  ....&......5....
-000004b0: 1811 5f5f 696e 6465 785f 6c65 7665 6c5f  ..__index_level_
-000004c0: 305f 5f15 0216 0e16 9c02 16fc 0126 b411  0__..........&..
-000004d0: 26cc 101c 1808 1900 0000 0000 0000 1808  &...............
-000004e0: 0000 0000 0000 0000 1600 2808 1900 0000  ..........(.....
-000004f0: 0000 0000 1808 0000 0000 0000 0000 0019  ................
-00000500: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
-00000510: 0015 0419 7c35 0018 0673 6368 656d 6115  ....|5...schema.
-00000520: 0c00 1504 2502 1802 6964 0015 0a25 0218  ....%...id...%..
-00000530: 0272 6100 150a 2502 1803 6465 6300 1504  .ra...%...dec...
-00000540: 2502 1808 7261 5f65 7272 6f72 0015 0425  %...ra_error...%
-00000550: 0218 0964 6563 5f65 7272 6f72 0015 0425  ...dec_error...%
-00000560: 0218 115f 5f69 6e64 6578 5f6c 6576 656c  ...__index_level
-00000570: 5f30 5f5f 0016 0e19 1c19 6c26 8802 1c15  _0__......l&....
-00000580: 0419 3510 0006 1918 0269 6415 0216 0e16  ..5......id.....
-00000590: 9c02 1680 0226 7426 081c 1808 3c03 0000  .....&t&....<...
-000005a0: 0000 0000 1808 2303 0000 0000 0000 1600  ......#.........
-000005b0: 2808 3c03 0000 0000 0000 1808 2303 0000  (.<.........#...
-000005c0: 0000 0000 0019 2c15 0415 0015 0200 1500  ......,.........
-000005d0: 1510 1502 0000 0026 ba05 1c15 0a19 3510  .......&......5.
-000005e0: 0006 1918 0272 6115 0216 0e16 8c02 16fa  .....ra.........
-000005f0: 0126 a604 26c0 031c 1808 0000 0000 00d8  .&..&...........
-00000600: 7540 1808 0000 0000 0008 7440 1600 2808  u@........t@..(.
-00000610: 0000 0000 00d8 7540 1808 0000 0000 0008  ......u@........
-00000620: 7440 0019 2c15 0415 0015 0200 1500 1510  t@..,...........
-00000630: 1502 0000 0026 fc08 1c15 0a19 3510 0006  .....&......5...
-00000640: 1918 0364 6563 1502 160e 169c 0216 8602  ...dec..........
-00000650: 26e8 0726 f606 1c18 0800 0000 0000 8039  &..&...........9
-00000660: c018 0800 0000 0000 404e c016 0028 0800  ........@N...(..
-00000670: 0000 0000 8039 c018 0800 0000 0000 404e  .....9........@N
-00000680: c000 192c 1504 1500 1502 0015 0015 1015  ...,............
-00000690: 0200 0000 26fa 0b1c 1504 1935 1000 0619  ....&......5....
-000006a0: 1808 7261 5f65 7272 6f72 1502 160e 16b8  ..ra_error......
-000006b0: 0116 c001 26ea 0a26 ba0a 1c18 0800 0000  ....&..&........
-000006c0: 0000 0000 0018 0800 0000 0000 0000 0016  ................
-000006d0: 0028 0800 0000 0000 0000 0018 0800 0000  .(..............
-000006e0: 0000 0000 0000 192c 1504 1500 1502 0015  .......,........
-000006f0: 0015 1015 0200 0000 2682 0f1c 1504 1935  ........&......5
-00000700: 1000 0619 1809 6465 635f 6572 726f 7215  ......dec_error.
-00000710: 0216 0e16 b801 16c0 0126 f20d 26c2 0d1c  .........&..&...
-00000720: 1808 0000 0000 0000 0000 1808 0000 0000  ................
-00000730: 0000 0000 1600 2808 0000 0000 0000 0000  ......(.........
-00000740: 1808 0000 0000 0000 0000 0019 2c15 0415  ............,...
-00000750: 0015 0200 1500 1510 1502 0000 0026 c812  .............&..
-00000760: 1c15 0419 3510 0006 1918 115f 5f69 6e64  ....5......__ind
-00000770: 6578 5f6c 6576 656c 5f30 5f5f 1502 160e  ex_level_0__....
-00000780: 169c 0216 fc01 26b4 1126 cc10 1c18 0819  ......&..&......
-00000790: 0000 0000 0000 0018 0800 0000 0000 0000  ................
-000007a0: 0016 0028 0819 0000 0000 0000 0018 0800  ...(............
-000007b0: 0000 0000 0000 0000 192c 1504 1500 1502  .........,......
-000007c0: 0015 0015 1015 0200 0000 16d0 0b16 0e26  ...............&
-000007d0: 0816 fc0a 1400 0019 2c18 0670 616e 6461  ........,..panda
-000007e0: 7318 a507 7b22 696e 6465 785f 636f 6c75  s...{"index_colu
-000007f0: 6d6e 7322 3a20 5b22 5f5f 696e 6465 785f  mns": ["__index_
-00000800: 6c65 7665 6c5f 305f 5f22 5d2c 2022 636f  level_0__"], "co
-00000810: 6c75 6d6e 5f69 6e64 6578 6573 223a 205b  lumn_indexes": [
-00000820: 7b22 6e61 6d65 223a 206e 756c 6c2c 2022  {"name": null, "
-00000830: 6669 656c 645f 6e61 6d65 223a 206e 756c  field_name": nul
-00000840: 6c2c 2022 7061 6e64 6173 5f74 7970 6522  l, "pandas_type"
-00000850: 3a20 2275 6e69 636f 6465 222c 2022 6e75  : "unicode", "nu
-00000860: 6d70 795f 7479 7065 223a 2022 6f62 6a65  mpy_type": "obje
-00000870: 6374 222c 2022 6d65 7461 6461 7461 223a  ct", "metadata":
-00000880: 207b 2265 6e63 6f64 696e 6722 3a20 2255   {"encoding": "U
-00000890: 5446 2d38 227d 7d5d 2c20 2263 6f6c 756d  TF-8"}}], "colum
-000008a0: 6e73 223a 205b 7b22 6e61 6d65 223a 2022  ns": [{"name": "
-000008b0: 6964 222c 2022 6669 656c 645f 6e61 6d65  id", "field_name
-000008c0: 223a 2022 6964 222c 2022 7061 6e64 6173  ": "id", "pandas
-000008d0: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
-000008e0: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
-000008f0: 696e 7436 3422 2c20 226d 6574 6164 6174  int64", "metadat
-00000900: 6122 3a20 6e75 6c6c 7d2c 207b 226e 616d  a": null}, {"nam
-00000910: 6522 3a20 2272 6122 2c20 2266 6965 6c64  e": "ra", "field
-00000920: 5f6e 616d 6522 3a20 2272 6122 2c20 2270  _name": "ra", "p
-00000930: 616e 6461 735f 7479 7065 223a 2022 666c  andas_type": "fl
-00000940: 6f61 7436 3422 2c20 226e 756d 7079 5f74  oat64", "numpy_t
-00000950: 7970 6522 3a20 2266 6c6f 6174 3634 222c  ype": "float64",
-00000960: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
-00000970: 6c7d 2c20 7b22 6e61 6d65 223a 2022 6465  l}, {"name": "de
-00000980: 6322 2c20 2266 6965 6c64 5f6e 616d 6522  c", "field_name"
-00000990: 3a20 2264 6563 222c 2022 7061 6e64 6173  : "dec", "pandas
-000009a0: 5f74 7970 6522 3a20 2266 6c6f 6174 3634  _type": "float64
-000009b0: 222c 2022 6e75 6d70 795f 7479 7065 223a  ", "numpy_type":
-000009c0: 2022 666c 6f61 7436 3422 2c20 226d 6574   "float64", "met
-000009d0: 6164 6174 6122 3a20 6e75 6c6c 7d2c 207b  adata": null}, {
-000009e0: 226e 616d 6522 3a20 2272 615f 6572 726f  "name": "ra_erro
-000009f0: 7222 2c20 2266 6965 6c64 5f6e 616d 6522  r", "field_name"
-00000a00: 3a20 2272 615f 6572 726f 7222 2c20 2270  : "ra_error", "p
-00000a10: 616e 6461 735f 7479 7065 223a 2022 696e  andas_type": "in
-00000a20: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
-00000a30: 6522 3a20 2269 6e74 3634 222c 2022 6d65  e": "int64", "me
-00000a40: 7461 6461 7461 223a 206e 756c 6c7d 2c20  tadata": null}, 
-00000a50: 7b22 6e61 6d65 223a 2022 6465 635f 6572  {"name": "dec_er
-00000a60: 726f 7222 2c20 2266 6965 6c64 5f6e 616d  ror", "field_nam
-00000a70: 6522 3a20 2264 6563 5f65 7272 6f72 222c  e": "dec_error",
-00000a80: 2022 7061 6e64 6173 5f74 7970 6522 3a20   "pandas_type": 
-00000a90: 2269 6e74 3634 222c 2022 6e75 6d70 795f  "int64", "numpy_
-00000aa0: 7479 7065 223a 2022 696e 7436 3422 2c20  type": "int64", 
-00000ab0: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
-00000ac0: 7d2c 207b 226e 616d 6522 3a20 6e75 6c6c  }, {"name": null
-00000ad0: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
-00000ae0: 225f 5f69 6e64 6578 5f6c 6576 656c 5f30  "__index_level_0
-00000af0: 5f5f 222c 2022 7061 6e64 6173 5f74 7970  __", "pandas_typ
-00000b00: 6522 3a20 2269 6e74 3634 222c 2022 6e75  e": "int64", "nu
-00000b10: 6d70 795f 7479 7065 223a 2022 696e 7436  mpy_type": "int6
-00000b20: 3422 2c20 226d 6574 6164 6174 6122 3a20  4", "metadata": 
-00000b30: 6e75 6c6c 7d5d 2c20 2263 7265 6174 6f72  null}], "creator
-00000b40: 223a 207b 226c 6962 7261 7279 223a 2022  ": {"library": "
-00000b50: 7079 6172 726f 7722 2c20 2276 6572 7369  pyarrow", "versi
-00000b60: 6f6e 223a 2022 392e 302e 3022 7d2c 2022  on": "9.0.0"}, "
-00000b70: 7061 6e64 6173 5f76 6572 7369 6f6e 223a  pandas_version":
-00000b80: 2022 312e 332e 3522 7d00 180c 4152 524f   "1.3.5"}...ARRO
-00000b90: 573a 7363 6865 6d61 18c0 0e2f 2f2f 2f2f  W:schema.../////
-00000ba0: 3267 4641 4141 5141 4141 4141 4141 4b41  2gFAAAQAAAAAAAKA
-00000bb0: 4134 4142 6741 4641 4167 4143 6741 4141  A4ABgAFAAgACgAAA
-00000bc0: 4141 4242 4141 5141 4141 4141 4141 4b41  AABBAAQAAAAAAAKA
-00000bd0: 4177 4141 4141 4541 4167 4143 6741 4141  AwAAAAEAAgACgAAA
-00000be0: 4e77 4441 4141 4541 4141 4141 5141 4141  NwDAAAEAAAAAQAAA
-00000bf0: 4177 4141 4141 4941 4177 4142 4141 4941  AwAAAAIAAwABAAIA
-00000c00: 4167 4141 4141 4941 4141 4145 4141 4141  AgAAAAIAAAAEAAAA
-00000c10: 4159 4141 4142 7759 5735 6b59 584d 4141  AYAAABwYW5kYXMAA
-00000c20: 4b55 4441 4142 3749 6d6c 755a 4756 3458  KUDAAB7ImluZGV4X
-00000c30: 324e 7662 4856 7462 6e4d 694f 6942 6249  2NvbHVtbnMiOiBbI
-00000c40: 6c39 6661 5735 6b5a 5868 6662 4756 325a  l9faW5kZXhfbGV2Z
-00000c50: 5778 664d 4639 6649 6c30 7349 434a 6a62  WxfMF9fIl0sICJjb
-00000c60: 3278 3162 5735 6661 5735 6b5a 5868 6c63  2x1bW5faW5kZXhlc
-00000c70: 7949 3649 4674 3749 6d35 6862 5755 694f  yI6IFt7Im5hbWUiO
-00000c80: 6942 7564 5778 734c 4341 695a 6d6c 6c62  iBudWxsLCAiZmllb
-00000c90: 4752 6662 6d46 745a 5349 3649 4735 3162  GRfbmFtZSI6IG51b
-00000ca0: 4777 7349 434a 7759 5735 6b59 584e 6664  GwsICJwYW5kYXNfd
-00000cb0: 486c 775a 5349 3649 434a 3162 6d6c 6a62  HlwZSI6ICJ1bmljb
-00000cc0: 3252 6c49 6977 6749 6d35 3162 5842 3558  2RlIiwgIm51bXB5X
-00000cd0: 3352 3563 4755 694f 6941 6962 324a 715a  3R5cGUiOiAib2JqZ
-00000ce0: 574e 3049 6977 6749 6d31 6c64 4746 6b59  WN0IiwgIm1ldGFkY
-00000cf0: 5852 6849 6a6f 6765 794a 6c62 6d4e 765a  XRhIjogeyJlbmNvZ
-00000d00: 476c 755a 7949 3649 434a 5656 4559 744f  GluZyI6ICJVVEYtO
-00000d10: 434a 3966 5630 7349 434a 6a62 3278 3162  CJ9fV0sICJjb2x1b
-00000d20: 5735 7a49 6a6f 6757 3373 6962 6d46 745a  W5zIjogW3sibmFtZ
-00000d30: 5349 3649 434a 705a 4349 7349 434a 6d61  SI6ICJpZCIsICJma
-00000d40: 5756 735a 4639 7559 5731 6c49 6a6f 6749  WVsZF9uYW1lIjogI
-00000d50: 6d6c 6b49 6977 6749 6e42 6862 6d52 6863  mlkIiwgInBhbmRhc
-00000d60: 3139 3065 5842 6c49 6a6f 6749 6d6c 7564  190eXBlIjogImlud
-00000d70: 4459 3049 6977 6749 6d35 3162 5842 3558  DY0IiwgIm51bXB5X
-00000d80: 3352 3563 4755 694f 6941 6961 5735 304e  3R5cGUiOiAiaW50N
-00000d90: 6a51 694c 4341 6962 5756 3059 5752 6864  jQiLCAibWV0YWRhd
-00000da0: 4745 694f 6942 7564 5778 7366 5377 6765  GEiOiBudWxsfSwge
-00000db0: 794a 7559 5731 6c49 6a6f 6749 6e4a 6849  yJuYW1lIjogInJhI
-00000dc0: 6977 6749 6d5a 705a 5778 6b58 3235 6862  iwgImZpZWxkX25hb
-00000dd0: 5755 694f 6941 6963 6d45 694c 4341 6963  WUiOiAicmEiLCAic
-00000de0: 4746 755a 4746 7a58 3352 3563 4755 694f  GFuZGFzX3R5cGUiO
-00000df0: 6941 695a 6d78 7659 5851 324e 4349 7349  iAiZmxvYXQ2NCIsI
-00000e00: 434a 7564 5731 7765 5639 3065 5842 6c49  CJudW1weV90eXBlI
-00000e10: 6a6f 6749 6d5a 7362 3246 304e 6a51 694c  jogImZsb2F0NjQiL
-00000e20: 4341 6962 5756 3059 5752 6864 4745 694f  CAibWV0YWRhdGEiO
-00000e30: 6942 7564 5778 7366 5377 6765 794a 7559  iBudWxsfSwgeyJuY
-00000e40: 5731 6c49 6a6f 6749 6d52 6c59 7949 7349  W1lIjogImRlYyIsI
-00000e50: 434a 6d61 5756 735a 4639 7559 5731 6c49  CJmaWVsZF9uYW1lI
-00000e60: 6a6f 6749 6d52 6c59 7949 7349 434a 7759  jogImRlYyIsICJwY
-00000e70: 5735 6b59 584e 6664 486c 775a 5349 3649  W5kYXNfdHlwZSI6I
-00000e80: 434a 6d62 4739 6864 4459 3049 6977 6749  CJmbG9hdDY0IiwgI
-00000e90: 6d35 3162 5842 3558 3352 3563 4755 694f  m51bXB5X3R5cGUiO
-00000ea0: 6941 695a 6d78 7659 5851 324e 4349 7349  iAiZmxvYXQ2NCIsI
-00000eb0: 434a 745a 5852 685a 4746 3059 5349 3649  CJtZXRhZGF0YSI6I
-00000ec0: 4735 3162 4778 394c 4342 3749 6d35 6862  G51bGx9LCB7Im5hb
-00000ed0: 5755 694f 6941 6963 6d46 665a 584a 7962  WUiOiAicmFfZXJyb
-00000ee0: 3349 694c 4341 695a 6d6c 6c62 4752 6662  3IiLCAiZmllbGRfb
-00000ef0: 6d46 745a 5349 3649 434a 7959 5639 6c63  mFtZSI6ICJyYV9lc
-00000f00: 6e4a 7663 6949 7349 434a 7759 5735 6b59  nJvciIsICJwYW5kY
-00000f10: 584e 6664 486c 775a 5349 3649 434a 7062  XNfdHlwZSI6ICJpb
-00000f20: 6e51 324e 4349 7349 434a 7564 5731 7765  nQ2NCIsICJudW1we
-00000f30: 5639 3065 5842 6c49 6a6f 6749 6d6c 7564  V90eXBlIjogImlud
-00000f40: 4459 3049 6977 6749 6d31 6c64 4746 6b59  DY0IiwgIm1ldGFkY
-00000f50: 5852 6849 6a6f 6762 6e56 7362 4830 7349  XRhIjogbnVsbH0sI
-00000f60: 4873 6962 6d46 745a 5349 3649 434a 6b5a  HsibmFtZSI6ICJkZ
-00000f70: 574e 665a 584a 7962 3349 694c 4341 695a  WNfZXJyb3IiLCAiZ
-00000f80: 6d6c 6c62 4752 6662 6d46 745a 5349 3649  mllbGRfbmFtZSI6I
-00000f90: 434a 6b5a 574e 665a 584a 7962 3349 694c  CJkZWNfZXJyb3IiL
-00000fa0: 4341 6963 4746 755a 4746 7a58 3352 3563  CAicGFuZGFzX3R5c
-00000fb0: 4755 694f 6941 6961 5735 304e 6a51 694c  GUiOiAiaW50NjQiL
-00000fc0: 4341 6962 6e56 7463 486c 6664 486c 775a  CAibnVtcHlfdHlwZ
-00000fd0: 5349 3649 434a 7062 6e51 324e 4349 7349  SI6ICJpbnQ2NCIsI
-00000fe0: 434a 745a 5852 685a 4746 3059 5349 3649  CJtZXRhZGF0YSI6I
-00000ff0: 4735 3162 4778 394c 4342 3749 6d35 6862  G51bGx9LCB7Im5hb
-00001000: 5755 694f 6942 7564 5778 734c 4341 695a  WUiOiBudWxsLCAiZ
-00001010: 6d6c 6c62 4752 6662 6d46 745a 5349 3649  mllbGRfbmFtZSI6I
-00001020: 434a 6658 326c 755a 4756 3458 3278 6c64  CJfX2luZGV4X2xld
-00001030: 6d56 7358 7a42 6658 7949 7349 434a 7759  mVsXzBfXyIsICJwY
-00001040: 5735 6b59 584e 6664 486c 775a 5349 3649  W5kYXNfdHlwZSI6I
-00001050: 434a 7062 6e51 324e 4349 7349 434a 7564  CJpbnQ2NCIsICJud
-00001060: 5731 7765 5639 3065 5842 6c49 6a6f 6749  W1weV90eXBlIjogI
-00001070: 6d6c 7564 4459 3049 6977 6749 6d31 6c64  mludDY0IiwgIm1ld
-00001080: 4746 6b59 5852 6849 6a6f 6762 6e56 7362  GFkYXRhIjogbnVsb
-00001090: 4831 644c 4341 6959 334a 6c59 5852 7663  H1dLCAiY3JlYXRvc
-000010a0: 6949 3649 4873 6962 476c 6963 6d46 7965  iI6IHsibGlicmFye
-000010b0: 5349 3649 434a 7765 5746 7963 6d39 3349  SI6ICJweWFycm93I
-000010c0: 6977 6749 6e5a 6c63 6e4e 7062 3234 694f  iwgInZlcnNpb24iO
-000010d0: 6941 694f 5334 774c 6a41 6966 5377 6749  iAiOS4wLjAifSwgI
-000010e0: 6e42 6862 6d52 6863 3139 325a 584a 7a61  nBhbmRhc192ZXJza
-000010f0: 5739 7549 6a6f 6749 6a45 754d 7934 3149  W9uIjogIjEuMy41I
-00001100: 6e30 4141 4141 4741 4141 414a 4145 4141  n0AAAAGAAAAJAEAA
-00001110: 4f41 4141 4143 3041 4141 4166 4141 4141  OAAAAC0AAAAfAAAA
-00001120: 4551 4141 4141 4541 4141 4142 502f 2f2f  EQAAAAEAAAABP///
-00001130: 7741 4141 5149 5141 4141 414a 4141 4141  wAAAQIQAAAAJAAAA
-00001140: 4151 4141 4141 4141 4141 4145 5141 4141  AQAAAAAAAAAEQAAA
-00001150: 4639 6661 5735 6b5a 5868 6662 4756 325a  F9faW5kZXhfbGV2Z
-00001160: 5778 664d 4639 6641 4141 4142 502f 2f2f  WxfMF9fAAAABP///
-00001170: 7741 4141 4146 4141 4141 4151 502f 2f2f  wAAAAFAAAAAQP///
-00001180: 7741 4141 5149 5141 4141 4148 4141 4141  wAAAQIQAAAAHAAAA
-00001190: 4151 4141 4141 4141 4141 4143 5141 4141  AQAAAAAAAAACQAAA
-000011a0: 4752 6c59 3139 6c63 6e4a 7663 6741 4141  GRlY19lcnJvcgAAA
-000011b0: 446a 2f2f 2f38 4141 4141 4251 4141 4141  Dj///8AAAABQAAAA
-000011c0: 4854 2f2f 2f38 4141 4145 4345 4141 4141  HT///8AAAECEAAAA
-000011d0: 4277 4141 4141 4541 4141 4141 4141 4141  BwAAAAEAAAAAAAAA
-000011e0: 4167 4141 4142 7959 5639 6c63 6e4a 7663  AgAAAByYV9lcnJvc
-000011f0: 6741 4141 4142 732f 2f2f 2f41 4141 4141  gAAAABs////AAAAA
-00001200: 5541 4141 4143 6f2f 2f2f 2f41 4141 4241  UAAAACo////AAABA
-00001210: 7841 4141 4141 5541 4141 4142 4141 4141  xAAAAAUAAAABAAAA
-00001220: 4141 4141 4141 4441 4141 415a 4756 6a41  AAAAAADAAAAZGVjA
-00001230: 4e62 2f2f 2f38 4141 4149 4130 502f 2f2f  Nb///8AAAIA0P///
-00001240: 7741 4141 514d 5141 4141 4148 4141 4141  wAAAQMQAAAAHAAAA
-00001250: 4151 4141 4141 4141 4141 4141 6741 4141  AQAAAAAAAAAAgAAA
-00001260: 484a 6841 4141 4141 4159 4143 4141 4741  HJhAAAAAAYACAAGA
-00001270: 4159 4141 4141 4141 4149 4145 4141 5541  AYAAAAAAAIAEAAUA
-00001280: 4167 4142 6741 4841 4177 4141 4141 5141  AgABgAHAAwAAAAQA
-00001290: 4241 4141 4141 4141 4145 4345 4141 4141  BAAAAAAAAECEAAAA
-000012a0: 4277 4141 4141 4541 4141 4141 4141 4141  BwAAAAEAAAAAAAAA
-000012b0: 4149 4141 4142 705a 4141 4143 4141 4d41  AIAAABpZAAACAAMA
-000012c0: 4167 4142 7741 4941 4141 4141 4141 4141  AgABwAIAAAAAAAAA
-000012d0: 5541 4141 4141 4141 4141 4100 181f 7061  UAAAAAAAAAA...pa
-000012e0: 7271 7565 742d 6370 702d 6172 726f 7720  rquet-cpp-arrow 
-000012f0: 7665 7273 696f 6e20 392e 302e 3019 6c1c  version 9.0.0.l.
-00001300: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
-00001310: 0000 010e 0000 5041 5231                 ......PAR1
+00000000: 5041 5231 1504 15b0 0115 704c 1516 1500  PAR1......pL....
+00000010: 1200 0058 08bc 0200 0501 00bd 0d08 00c2  ...X............
+00000020: 0d08 00c4 0d08 00c5 0d08 00c7 0d08 00c8  ................
+00000030: 0d08 00c9 0d08 00ca 0d08 3ccb 0200 0000  ..........<.....
+00000040: 0000 00cd 0200 0000 0000 0015 0015 2015  .............. .
+00000050: 242c 1516 1510 1506 1506 1c18 08cd 0200  $,..............
+00000060: 0000 0000 0018 08bc 0200 0000 0000 0016  ................
+00000070: 0028 08cd 0200 0000 0000 0018 08bc 0200  .(..............
+00000080: 0000 0000 0000 0000 103c 0200 0000 1601  .........<......
+00000090: 0405 1032 5476 980a 0000 26b4 021c 1504  ...2Tv....&.....
+000000a0: 1935 1000 0619 1802 6964 1502 1616 16e8  .5......id......
+000000b0: 0216 ac02 2696 0126 081c 1808 cd02 0000  ....&..&........
+000000c0: 0000 0000 1808 bc02 0000 0000 0000 1600  ................
+000000d0: 2808 cd02 0000 0000 0000 1808 bc02 0000  (...............
+000000e0: 0000 0000 0019 2c15 0415 0015 0200 1500  ......,.........
+000000f0: 1510 1502 0000 0015 0415 a001 156c 4c15  .............lL.
+00000100: 1415 0012 0000 5000 0001 0108 a871 4001  ......P......q@.
+00000110: 0708 00b8 7209 0800 980d 0804 3873 0910  ....r.......8s..
+00000120: 0068 0d10 0018 0d10 0008 0d10 00a8 0d08  .h..............
+00000130: 28f8 7240 0000 0000 0088 7140 1500 1520  (.r@......q@... 
+00000140: 1524 2c15 1615 1015 0615 061c 1808 0000  .$,.............
+00000150: 0000 0038 7340 1808 0000 0000 0088 7140  ...8s@........q@
+00000160: 1600 2808 0000 0000 0038 7340 1808 0000  ..(......8s@....
+00000170: 0000 0088 7140 0000 0010 3c02 0000 0016  ....q@....<.....
+00000180: 0104 0510 3254 7698 0800 0026 9606 1c15  ....2Tv....&....
+00000190: 0a19 3510 0006 1918 0272 6115 0216 1616  ..5......ra.....
+000001a0: d802 16a8 0226 f804 26ee 031c 1808 0000  .....&..&.......
+000001b0: 0000 0038 7340 1808 0000 0000 0088 7140  ...8s@........q@
+000001c0: 1600 2808 0000 0000 0038 7340 1808 0000  ..(......8s@....
+000001d0: 0000 0088 7140 0019 2c15 0415 0015 0200  ....q@..,.......
+000001e0: 1500 1510 1502 0000 0015 0415 9001 155e  ...............^
+000001f0: 4c15 1215 0012 0000 4800 0001 0108 404d  L.......H.....@M
+00000200: c001 0708 0040 480d 0800 4209 0800 c011  .....@H...B.....
+00000210: 0800 460d 100d 2004 c044 0d10 2441 c000  ..F... ..D..$A..
+00000220: 0000 0000 c045 c015 0015 2015 242c 1516  .....E.... .$,..
+00000230: 1510 1506 1506 1c18 0800 0000 0000 c041  ...............A
+00000240: c018 0800 0000 0000 404d c016 0028 0800  ........@M...(..
+00000250: 0000 0000 c041 c018 0800 0000 0000 404d  .....A........@M
+00000260: c000 0000 103c 0200 0000 1601 0405 1032  .....<.........2
+00000270: 5465 7308 0000 26ec 091c 150a 1935 1000  Tes...&......5..
+00000280: 0619 1803 6465 6315 0216 1616 c802 169a  ....dec.........
+00000290: 0226 ce08 26d2 071c 1808 0000 0000 00c0  .&..&...........
+000002a0: 41c0 1808 0000 0000 0040 4dc0 1600 2808  A........@M...(.
+000002b0: 0000 0000 00c0 41c0 1808 0000 0000 0040  ......A........@
+000002c0: 4dc0 0019 2c15 0415 0015 0200 1500 1510  M...,...........
+000002d0: 1502 0000 0015 0415 1015 144c 1502 1500  ...........L....
+000002e0: 1200 0008 1c00 0000 0000 0000 0015 0015  ................
+000002f0: 1215 162c 1516 1510 1506 1506 1c18 0800  ...,............
+00000300: 0000 0000 0000 0018 0800 0000 0000 0000  ................
+00000310: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
+00000320: 0000 0000 0000 0000 0000 0920 0200 0000  ........... ....
+00000330: 1601 0116 0026 ea0c 1c15 0419 3510 0006  .....&......5...
+00000340: 1918 0872 615f 6572 726f 7215 0216 1616  ...ra_error.....
+00000350: b801 16c0 0126 da0b 26aa 0b1c 1808 0000  .....&..&.......
+00000360: 0000 0000 0000 1808 0000 0000 0000 0000  ................
+00000370: 1600 2808 0000 0000 0000 0000 1808 0000  ..(.............
+00000380: 0000 0000 0000 0019 2c15 0415 0015 0200  ........,.......
+00000390: 1500 1510 1502 0000 0015 0415 1015 144c  ...............L
+000003a0: 1502 1500 1200 0008 1c00 0000 0000 0000  ................
+000003b0: 0015 0015 1215 162c 1516 1510 1506 1506  .......,........
+000003c0: 1c18 0800 0000 0000 0000 0018 0800 0000  ................
+000003d0: 0000 0000 0016 0028 0800 0000 0000 0000  .......(........
+000003e0: 0018 0800 0000 0000 0000 0000 0000 0920  ............... 
+000003f0: 0200 0000 1601 0116 0026 f20f 1c15 0419  .........&......
+00000400: 3510 0006 1918 0964 6563 5f65 7272 6f72  5......dec_error
+00000410: 1502 1616 16b8 0116 c001 26e2 0e26 b20e  ..........&..&..
+00000420: 1c18 0800 0000 0000 0000 0018 0800 0000  ................
+00000430: 0000 0000 0016 0028 0800 0000 0000 0000  .......(........
+00000440: 0018 0800 0000 0000 0000 0000 192c 1504  .............,..
+00000450: 1500 1502 0015 0015 1015 0200 0000 1504  ................
+00000460: 196c 3500 1806 7363 6865 6d61 150a 0015  .l5...schema....
+00000470: 0425 0218 0269 6400 150a 2502 1802 7261  .%...id...%...ra
+00000480: 0015 0a25 0218 0364 6563 0015 0425 0218  ...%...dec...%..
+00000490: 0872 615f 6572 726f 7200 1504 2502 1809  .ra_error...%...
+000004a0: 6465 635f 6572 726f 7200 1616 191c 195c  dec_error......\
+000004b0: 26b4 021c 1504 1935 1000 0619 1802 6964  &......5......id
+000004c0: 1502 1616 16e8 0216 ac02 2696 0126 081c  ..........&..&..
+000004d0: 1808 cd02 0000 0000 0000 1808 bc02 0000  ................
+000004e0: 0000 0000 1600 2808 cd02 0000 0000 0000  ......(.........
+000004f0: 1808 bc02 0000 0000 0000 0019 2c15 0415  ............,...
+00000500: 0015 0200 1500 1510 1502 0000 0026 9606  .............&..
+00000510: 1c15 0a19 3510 0006 1918 0272 6115 0216  ....5......ra...
+00000520: 1616 d802 16a8 0226 f804 26ee 031c 1808  .......&..&.....
+00000530: 0000 0000 0038 7340 1808 0000 0000 0088  .....8s@........
+00000540: 7140 1600 2808 0000 0000 0038 7340 1808  q@..(......8s@..
+00000550: 0000 0000 0088 7140 0019 2c15 0415 0015  ......q@..,.....
+00000560: 0200 1500 1510 1502 0000 0026 ec09 1c15  ...........&....
+00000570: 0a19 3510 0006 1918 0364 6563 1502 1616  ..5......dec....
+00000580: 16c8 0216 9a02 26ce 0826 d207 1c18 0800  ......&..&......
+00000590: 0000 0000 c041 c018 0800 0000 0000 404d  .....A........@M
+000005a0: c016 0028 0800 0000 0000 c041 c018 0800  ...(.......A....
+000005b0: 0000 0000 404d c000 192c 1504 1500 1502  ....@M...,......
+000005c0: 0015 0015 1015 0200 0000 26ea 0c1c 1504  ..........&.....
+000005d0: 1935 1000 0619 1808 7261 5f65 7272 6f72  .5......ra_error
+000005e0: 1502 1616 16b8 0116 c001 26da 0b26 aa0b  ..........&..&..
+000005f0: 1c18 0800 0000 0000 0000 0018 0800 0000  ................
+00000600: 0000 0000 0016 0028 0800 0000 0000 0000  .......(........
+00000610: 0018 0800 0000 0000 0000 0000 192c 1504  .............,..
+00000620: 1500 1502 0015 0015 1015 0200 0000 26f2  ..............&.
+00000630: 0f1c 1504 1935 1000 0619 1809 6465 635f  .....5......dec_
+00000640: 6572 726f 7215 0216 1616 b801 16c0 0126  error..........&
+00000650: e20e 26b2 0e1c 1808 0000 0000 0000 0000  ..&.............
+00000660: 1808 0000 0000 0000 0000 1600 2808 0000  ............(...
+00000670: 0000 0000 0000 1808 0000 0000 0000 0000  ................
+00000680: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
+00000690: 0000 0016 f80a 1616 2608 16ee 0914 0000  ........&.......
+000006a0: 192c 1806 7061 6e64 6173 18a7 057b 2269  .,..pandas...{"i
+000006b0: 6e64 6578 5f63 6f6c 756d 6e73 223a 205b  ndex_columns": [
+000006c0: 5d2c 2022 636f 6c75 6d6e 5f69 6e64 6578  ], "column_index
+000006d0: 6573 223a 205b 5d2c 2022 636f 6c75 6d6e  es": [], "column
+000006e0: 7322 3a20 5b7b 226e 616d 6522 3a20 2269  s": [{"name": "i
+000006f0: 6422 2c20 2266 6965 6c64 5f6e 616d 6522  d", "field_name"
+00000700: 3a20 2269 6422 2c20 2270 616e 6461 735f  : "id", "pandas_
+00000710: 7479 7065 223a 2022 696e 7436 3422 2c20  type": "int64", 
+00000720: 226e 756d 7079 5f74 7970 6522 3a20 2269  "numpy_type": "i
+00000730: 6e74 3634 222c 2022 6d65 7461 6461 7461  nt64", "metadata
+00000740: 223a 206e 756c 6c7d 2c20 7b22 6e61 6d65  ": null}, {"name
+00000750: 223a 2022 7261 222c 2022 6669 656c 645f  ": "ra", "field_
+00000760: 6e61 6d65 223a 2022 7261 222c 2022 7061  name": "ra", "pa
+00000770: 6e64 6173 5f74 7970 6522 3a20 2266 6c6f  ndas_type": "flo
+00000780: 6174 3634 222c 2022 6e75 6d70 795f 7479  at64", "numpy_ty
+00000790: 7065 223a 2022 666c 6f61 7436 3422 2c20  pe": "float64", 
+000007a0: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
+000007b0: 7d2c 207b 226e 616d 6522 3a20 2264 6563  }, {"name": "dec
+000007c0: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
+000007d0: 2022 6465 6322 2c20 2270 616e 6461 735f   "dec", "pandas_
+000007e0: 7479 7065 223a 2022 666c 6f61 7436 3422  type": "float64"
+000007f0: 2c20 226e 756d 7079 5f74 7970 6522 3a20  , "numpy_type": 
+00000800: 2266 6c6f 6174 3634 222c 2022 6d65 7461  "float64", "meta
+00000810: 6461 7461 223a 206e 756c 6c7d 2c20 7b22  data": null}, {"
+00000820: 6e61 6d65 223a 2022 7261 5f65 7272 6f72  name": "ra_error
+00000830: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
+00000840: 2022 7261 5f65 7272 6f72 222c 2022 7061   "ra_error", "pa
+00000850: 6e64 6173 5f74 7970 6522 3a20 2269 6e74  ndas_type": "int
+00000860: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
+00000870: 223a 2022 696e 7436 3422 2c20 226d 6574  ": "int64", "met
+00000880: 6164 6174 6122 3a20 6e75 6c6c 7d2c 207b  adata": null}, {
+00000890: 226e 616d 6522 3a20 2264 6563 5f65 7272  "name": "dec_err
+000008a0: 6f72 222c 2022 6669 656c 645f 6e61 6d65  or", "field_name
+000008b0: 223a 2022 6465 635f 6572 726f 7222 2c20  ": "dec_error", 
+000008c0: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
+000008d0: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
+000008e0: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
+000008f0: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
+00000900: 5d2c 2022 6372 6561 746f 7222 3a20 7b22  ], "creator": {"
+00000910: 6c69 6272 6172 7922 3a20 2270 7961 7272  library": "pyarr
+00000920: 6f77 222c 2022 7665 7273 696f 6e22 3a20  ow", "version": 
+00000930: 2239 2e30 2e30 227d 2c20 2270 616e 6461  "9.0.0"}, "panda
+00000940: 735f 7665 7273 696f 6e22 3a20 2232 2e30  s_version": "2.0
+00000950: 2e30 227d 0018 0c41 5252 4f57 3a73 6368  .0"}...ARROW:sch
+00000960: 656d 6118 980b 2f2f 2f2f 2f79 6745 4141  ema.../////ygEAA
+00000970: 4151 4141 4141 4141 414b 4141 3441 4267  AQAAAAAAAKAA4ABg
+00000980: 4146 4141 6741 4367 4141 4141 4142 4241  AFAAgACgAAAAABBA
+00000990: 4151 4141 4141 4141 414b 4141 7741 4141  AQAAAAAAAKAAwAAA
+000009a0: 4145 4141 6741 4367 4141 414e 7743 4141  AEAAgACgAAANwCAA
+000009b0: 4145 4141 4141 4151 4141 4141 7741 4141  AEAAAAAQAAAAwAAA
+000009c0: 4149 4141 7741 4241 4149 4141 6741 4141  AIAAwABAAIAAgAAA
+000009d0: 4149 4141 4141 4541 4141 4141 5941 4141  AIAAAAEAAAAAYAAA
+000009e0: 4277 5957 356b 5958 4d41 414b 6343 4141  BwYW5kYXMAAKcCAA
+000009f0: 4237 496d 6c75 5a47 5634 5832 4e76 6248  B7ImluZGV4X2NvbH
+00000a00: 5674 626e 4d69 4f69 4262 5853 7767 496d  VtbnMiOiBbXSwgIm
+00000a10: 4e76 6248 5674 626c 3970 626d 526c 6547  NvbHVtbl9pbmRleG
+00000a20: 567a 496a 6f67 5731 3073 4943 4a6a 6232  VzIjogW10sICJjb2
+00000a30: 7831 6257 357a 496a 6f67 5733 7369 626d  x1bW5zIjogW3sibm
+00000a40: 4674 5a53 4936 4943 4a70 5a43 4973 4943  FtZSI6ICJpZCIsIC
+00000a50: 4a6d 6157 5673 5a46 3975 5957 316c 496a  JmaWVsZF9uYW1lIj
+00000a60: 6f67 496d 6c6b 4969 7767 496e 4268 626d  ogImlkIiwgInBhbm
+00000a70: 5268 6331 3930 6558 426c 496a 6f67 496d  Rhc190eXBlIjogIm
+00000a80: 6c75 6444 5930 4969 7767 496d 3531 6258  ludDY0IiwgIm51bX
+00000a90: 4235 5833 5235 6347 5569 4f69 4169 6157  B5X3R5cGUiOiAiaW
+00000aa0: 3530 4e6a 5169 4c43 4169 6257 5630 5957  50NjQiLCAibWV0YW
+00000ab0: 5268 6447 4569 4f69 4275 6457 7873 6653  RhdGEiOiBudWxsfS
+00000ac0: 7767 6579 4a75 5957 316c 496a 6f67 496e  wgeyJuYW1lIjogIn
+00000ad0: 4a68 4969 7767 496d 5a70 5a57 786b 5832  JhIiwgImZpZWxkX2
+00000ae0: 3568 6257 5569 4f69 4169 636d 4569 4c43  5hbWUiOiAicmEiLC
+00000af0: 4169 6347 4675 5a47 467a 5833 5235 6347  AicGFuZGFzX3R5cG
+00000b00: 5569 4f69 4169 5a6d 7876 5958 5132 4e43  UiOiAiZmxvYXQ2NC
+00000b10: 4973 4943 4a75 6457 3177 6556 3930 6558  IsICJudW1weV90eX
+00000b20: 426c 496a 6f67 496d 5a73 6232 4630 4e6a  BlIjogImZsb2F0Nj
+00000b30: 5169 4c43 4169 6257 5630 5957 5268 6447  QiLCAibWV0YWRhdG
+00000b40: 4569 4f69 4275 6457 7873 6653 7767 6579  EiOiBudWxsfSwgey
+00000b50: 4a75 5957 316c 496a 6f67 496d 526c 5979  JuYW1lIjogImRlYy
+00000b60: 4973 4943 4a6d 6157 5673 5a46 3975 5957  IsICJmaWVsZF9uYW
+00000b70: 316c 496a 6f67 496d 526c 5979 4973 4943  1lIjogImRlYyIsIC
+00000b80: 4a77 5957 356b 5958 4e66 6448 6c77 5a53  JwYW5kYXNfdHlwZS
+00000b90: 4936 4943 4a6d 6247 3968 6444 5930 4969  I6ICJmbG9hdDY0Ii
+00000ba0: 7767 496d 3531 6258 4235 5833 5235 6347  wgIm51bXB5X3R5cG
+00000bb0: 5569 4f69 4169 5a6d 7876 5958 5132 4e43  UiOiAiZmxvYXQ2NC
+00000bc0: 4973 4943 4a74 5a58 5268 5a47 4630 5953  IsICJtZXRhZGF0YS
+00000bd0: 4936 4947 3531 6247 7839 4c43 4237 496d  I6IG51bGx9LCB7Im
+00000be0: 3568 6257 5569 4f69 4169 636d 4666 5a58  5hbWUiOiAicmFfZX
+00000bf0: 4a79 6233 4969 4c43 4169 5a6d 6c6c 6247  Jyb3IiLCAiZmllbG
+00000c00: 5266 626d 4674 5a53 4936 4943 4a79 5956  RfbmFtZSI6ICJyYV
+00000c10: 396c 636e 4a76 6369 4973 4943 4a77 5957  9lcnJvciIsICJwYW
+00000c20: 356b 5958 4e66 6448 6c77 5a53 4936 4943  5kYXNfdHlwZSI6IC
+00000c30: 4a70 626e 5132 4e43 4973 4943 4a75 6457  JpbnQ2NCIsICJudW
+00000c40: 3177 6556 3930 6558 426c 496a 6f67 496d  1weV90eXBlIjogIm
+00000c50: 6c75 6444 5930 4969 7767 496d 316c 6447  ludDY0IiwgIm1ldG
+00000c60: 466b 5958 5268 496a 6f67 626e 5673 6248  FkYXRhIjogbnVsbH
+00000c70: 3073 4948 7369 626d 4674 5a53 4936 4943  0sIHsibmFtZSI6IC
+00000c80: 4a6b 5a57 4e66 5a58 4a79 6233 4969 4c43  JkZWNfZXJyb3IiLC
+00000c90: 4169 5a6d 6c6c 6247 5266 626d 4674 5a53  AiZmllbGRfbmFtZS
+00000ca0: 4936 4943 4a6b 5a57 4e66 5a58 4a79 6233  I6ICJkZWNfZXJyb3
+00000cb0: 4969 4c43 4169 6347 4675 5a47 467a 5833  IiLCAicGFuZGFzX3
+00000cc0: 5235 6347 5569 4f69 4169 6157 3530 4e6a  R5cGUiOiAiaW50Nj
+00000cd0: 5169 4c43 4169 626e 5674 6348 6c66 6448  QiLCAibnVtcHlfdH
+00000ce0: 6c77 5a53 4936 4943 4a70 626e 5132 4e43  lwZSI6ICJpbnQ2NC
+00000cf0: 4973 4943 4a74 5a58 5268 5a47 4630 5953  IsICJtZXRhZGF0YS
+00000d00: 4936 4947 3531 6247 7839 5853 7767 496d  I6IG51bGx9XSwgIm
+00000d10: 4e79 5a57 4630 6233 4969 4f69 4237 496d  NyZWF0b3IiOiB7Im
+00000d20: 7870 596e 4a68 636e 6b69 4f69 4169 6348  xpYnJhcnkiOiAicH
+00000d30: 6c68 636e 4a76 6479 4973 4943 4a32 5a58  lhcnJvdyIsICJ2ZX
+00000d40: 4a7a 6157 3975 496a 6f67 496a 6b75 4d43  JzaW9uIjogIjkuMC
+00000d50: 3477 496e 3073 4943 4a77 5957 356b 5958  4wIn0sICJwYW5kYX
+00000d60: 4e66 646d 5679 6332 6c76 6269 4936 4943  NfdmVyc2lvbiI6IC
+00000d70: 4979 4c6a 4175 4d43 4a39 4141 5541 4141  IyLjAuMCJ9AAUAAA
+00000d80: 446b 4141 4141 6f41 4141 4148 5141 4141  DkAAAAoAAAAHQAAA
+00000d90: 4138 4141 4141 4241 4141 4145 442f 2f2f  A8AAAABAAAAED///
+00000da0: 3841 4141 4543 4541 4141 4142 7741 4141  8AAAECEAAAABwAAA
+00000db0: 4145 4141 4141 4141 4141 4141 6b41 4141  AEAAAAAAAAAAkAAA
+00000dc0: 426b 5a57 4e66 5a58 4a79 6233 4941 4141  BkZWNfZXJyb3IAAA
+00000dd0: 4134 2f2f 2f2f 4141 4141 4155 4141 4141  A4////AAAAAUAAAA
+00000de0: 4230 2f2f 2f2f 4141 4142 4168 4141 4141  B0////AAABAhAAAA
+00000df0: 4163 4141 4141 4241 4141 4141 4141 4141  AcAAAABAAAAAAAAA
+00000e00: 4149 4141 4141 636d 4666 5a58 4a79 6233  AIAAAAcmFfZXJyb3
+00000e10: 4941 4141 4141 6250 2f2f 2f77 4141 4141  IAAAAAbP///wAAAA
+00000e20: 4641 4141 4141 7150 2f2f 2f77 4141 4151  FAAAAAqP///wAAAQ
+00000e30: 4d51 4141 4141 4641 4141 4141 5141 4141  MQAAAAFAAAAAQAAA
+00000e40: 4141 4141 4141 4177 4141 4147 526c 5977  AAAAAAAwAAAGRlYw
+00000e50: 4457 2f2f 2f2f 4141 4143 414e 442f 2f2f  DW////AAACAND///
+00000e60: 3841 4141 4544 4541 4141 4142 7741 4141  8AAAEDEAAAABwAAA
+00000e70: 4145 4141 4141 4141 4141 4141 4941 4141  AEAAAAAAAAAAIAAA
+00000e80: 4279 5951 4141 4141 4147 4141 6741 4267  ByYQAAAAAGAAgABg
+00000e90: 4147 4141 4141 4141 4143 4142 4141 4641  AGAAAAAAACABAAFA
+00000ea0: 4149 4141 5941 4277 414d 4141 4141 4541  AIAAYABwAMAAAAEA
+00000eb0: 4151 4141 4141 4141 4142 4168 4141 4141  AQAAAAAAABAhAAAA
+00000ec0: 4163 4141 4141 4241 4141 4141 4141 4141  AcAAAABAAAAAAAAA
+00000ed0: 4143 4141 4141 6157 5141 4141 6741 4441  ACAAAAaWQAAAgADA
+00000ee0: 4149 4141 6341 4341 4141 4141 4141 4141  AIAAcACAAAAAAAAA
+00000ef0: 4641 4141 4141 4141 4141 4141 3d3d 0018  FAAAAAAAAAAA==..
+00000f00: 1f70 6172 7175 6574 2d63 7070 2d61 7272  .parquet-cpp-arr
+00000f10: 6f77 2076 6572 7369 6f6e 2039 2e30 2e30  ow version 9.0.0
+00000f20: 195c 1c00 001c 0000 1c00 001c 0000 1c00  .\..............
+00000f30: 0000 d40a 0000 5041 5231                 ......PAR1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_46/shard_0.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet`

 * *Files 12% similar despite different names*

```diff
@@ -63,248 +63,182 @@
 000003e0: 0000 0000 0000 0009 2002 0000 0014 0101  ........ .......
 000003f0: 1400 26e4 0f1c 1504 1935 1000 0619 1809  ..&......5......
 00000400: 6465 635f 6572 726f 7215 0216 1416 b801  dec_error.......
 00000410: 16c0 0126 d40e 26a4 0e1c 1808 0000 0000  ...&..&.........
 00000420: 0000 0000 1808 0000 0000 0000 0000 1600  ................
 00000430: 2808 0000 0000 0000 0000 1808 0000 0000  (...............
 00000440: 0000 0000 0019 2c15 0415 0015 0200 1500  ......,.........
-00000450: 1510 1502 0000 0015 0415 a001 1564 4c15  .............dL.
-00000460: 1415 0012 0000 5000 000d 0100 050d 0800  ......P.........
-00000470: 060d 0800 080d 0800 0b0d 0800 0c0d 0800  ................
-00000480: 0d0d 0800 100d 083c 1700 0000 0000 0000  .......<........
-00000490: 1900 0000 0000 0000 1500 1520 1524 2c15  ........... .$,.
-000004a0: 1415 1015 0615 061c 1808 1900 0000 0000  ................
-000004b0: 0000 1808 0000 0000 0000 0000 1600 2808  ..............(.
-000004c0: 1900 0000 0000 0000 1808 0000 0000 0000  ................
-000004d0: 0000 0000 0010 3c02 0000 0014 0104 0510  ......<.........
-000004e0: 3254 7698 0000 0026 ce13 1c15 0419 3510  2Tv....&......5.
-000004f0: 0006 1918 115f 5f69 6e64 6578 5f6c 6576  .....__index_lev
-00000500: 656c 5f30 5f5f 1502 1614 16d8 0216 a002  el_0__..........
-00000510: 26b0 1226 ae11 1c18 0819 0000 0000 0000  &..&............
-00000520: 0018 0800 0000 0000 0000 0016 0028 0819  .............(..
-00000530: 0000 0000 0000 0018 0800 0000 0000 0000  ................
-00000540: 0000 192c 1504 1500 1502 0015 0015 1015  ...,............
-00000550: 0200 0000 1504 197c 3500 1806 7363 6865  .......|5...sche
-00000560: 6d61 150c 0015 0425 0218 0269 6400 150a  ma.....%...id...
-00000570: 2502 1802 7261 0015 0a25 0218 0364 6563  %...ra...%...dec
-00000580: 0015 0425 0218 0872 615f 6572 726f 7200  ...%...ra_error.
-00000590: 1504 2502 1809 6465 635f 6572 726f 7200  ..%...dec_error.
-000005a0: 1504 2502 1811 5f5f 696e 6465 785f 6c65  ..%...__index_le
-000005b0: 7665 6c5f 305f 5f00 1614 191c 196c 26ac  vel_0__......l&.
-000005c0: 021c 1504 1935 1000 0619 1802 6964 1502  .....5......id..
-000005d0: 1614 16d8 0216 a402 268e 0126 081c 1808  ........&..&....
-000005e0: 2203 0000 0000 0000 1808 0903 0000 0000  "...............
-000005f0: 0000 1600 2808 2203 0000 0000 0000 1808  ....(.".........
-00000600: 0903 0000 0000 0000 0019 2c15 0415 0015  ..........,.....
-00000610: 0200 1500 1510 1502 0000 0026 8406 1c15  ...........&....
-00000620: 0a19 3510 0006 1918 0272 6115 0216 1416  ..5......ra.....
-00000630: c802 169e 0226 e604 26e6 031c 1808 0000  .....&..&.......
-00000640: 0000 0038 7340 1808 0000 0000 00b8 7140  ...8s@........q@
-00000650: 1600 2808 0000 0000 0038 7340 1808 0000  ..(......8s@....
-00000660: 0000 00b8 7140 0019 2c15 0415 0015 0200  ....q@..,.......
-00000670: 1500 1510 1502 0000 0026 de09 1c15 0a19  .........&......
-00000680: 3510 0006 1918 0364 6563 1502 1614 16c8  5......dec......
-00000690: 0216 9e02 26c0 0826 c007 1c18 0800 0000  ....&..&........
-000006a0: 0000 c041 c018 0800 0000 0000 c04e c016  ...A.........N..
-000006b0: 0028 0800 0000 0000 c041 c018 0800 0000  .(.......A......
-000006c0: 0000 c04e c000 192c 1504 1500 1502 0015  ...N...,........
-000006d0: 0015 1015 0200 0000 26dc 0c1c 1504 1935  ........&......5
-000006e0: 1000 0619 1808 7261 5f65 7272 6f72 1502  ......ra_error..
-000006f0: 1614 16b8 0116 c001 26cc 0b26 9c0b 1c18  ........&..&....
-00000700: 0800 0000 0000 0000 0018 0800 0000 0000  ................
-00000710: 0000 0016 0028 0800 0000 0000 0000 0018  .....(..........
-00000720: 0800 0000 0000 0000 0000 192c 1504 1500  ...........,....
-00000730: 1502 0015 0015 1015 0200 0000 26e4 0f1c  ............&...
-00000740: 1504 1935 1000 0619 1809 6465 635f 6572  ...5......dec_er
-00000750: 726f 7215 0216 1416 b801 16c0 0126 d40e  ror..........&..
-00000760: 26a4 0e1c 1808 0000 0000 0000 0000 1808  &...............
-00000770: 0000 0000 0000 0000 1600 2808 0000 0000  ..........(.....
-00000780: 0000 0000 1808 0000 0000 0000 0000 0019  ................
-00000790: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
-000007a0: 0026 ce13 1c15 0419 3510 0006 1918 115f  .&......5......_
-000007b0: 5f69 6e64 6578 5f6c 6576 656c 5f30 5f5f  _index_level_0__
-000007c0: 1502 1614 16d8 0216 a002 26b0 1226 ae11  ..........&..&..
-000007d0: 1c18 0819 0000 0000 0000 0018 0800 0000  ................
-000007e0: 0000 0000 0016 0028 0819 0000 0000 0000  .......(........
-000007f0: 0018 0800 0000 0000 0000 0000 192c 1504  .............,..
-00000800: 1500 1502 0015 0015 1015 0200 0000 16b0  ................
-00000810: 0d16 1426 0816 800c 1400 0019 2c18 0670  ...&........,..p
-00000820: 616e 6461 7318 a507 7b22 696e 6465 785f  andas...{"index_
-00000830: 636f 6c75 6d6e 7322 3a20 5b22 5f5f 696e  columns": ["__in
-00000840: 6465 785f 6c65 7665 6c5f 305f 5f22 5d2c  dex_level_0__"],
-00000850: 2022 636f 6c75 6d6e 5f69 6e64 6578 6573   "column_indexes
-00000860: 223a 205b 7b22 6e61 6d65 223a 206e 756c  ": [{"name": nul
-00000870: 6c2c 2022 6669 656c 645f 6e61 6d65 223a  l, "field_name":
-00000880: 206e 756c 6c2c 2022 7061 6e64 6173 5f74   null, "pandas_t
-00000890: 7970 6522 3a20 2275 6e69 636f 6465 222c  ype": "unicode",
-000008a0: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
-000008b0: 6f62 6a65 6374 222c 2022 6d65 7461 6461  object", "metada
-000008c0: 7461 223a 207b 2265 6e63 6f64 696e 6722  ta": {"encoding"
-000008d0: 3a20 2255 5446 2d38 227d 7d5d 2c20 2263  : "UTF-8"}}], "c
-000008e0: 6f6c 756d 6e73 223a 205b 7b22 6e61 6d65  olumns": [{"name
-000008f0: 223a 2022 6964 222c 2022 6669 656c 645f  ": "id", "field_
-00000900: 6e61 6d65 223a 2022 6964 222c 2022 7061  name": "id", "pa
-00000910: 6e64 6173 5f74 7970 6522 3a20 2269 6e74  ndas_type": "int
-00000920: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
-00000930: 223a 2022 696e 7436 3422 2c20 226d 6574  ": "int64", "met
-00000940: 6164 6174 6122 3a20 6e75 6c6c 7d2c 207b  adata": null}, {
-00000950: 226e 616d 6522 3a20 2272 6122 2c20 2266  "name": "ra", "f
-00000960: 6965 6c64 5f6e 616d 6522 3a20 2272 6122  ield_name": "ra"
-00000970: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
-00000980: 2022 666c 6f61 7436 3422 2c20 226e 756d   "float64", "num
-00000990: 7079 5f74 7970 6522 3a20 2266 6c6f 6174  py_type": "float
-000009a0: 3634 222c 2022 6d65 7461 6461 7461 223a  64", "metadata":
-000009b0: 206e 756c 6c7d 2c20 7b22 6e61 6d65 223a   null}, {"name":
-000009c0: 2022 6465 6322 2c20 2266 6965 6c64 5f6e   "dec", "field_n
-000009d0: 616d 6522 3a20 2264 6563 222c 2022 7061  ame": "dec", "pa
-000009e0: 6e64 6173 5f74 7970 6522 3a20 2266 6c6f  ndas_type": "flo
-000009f0: 6174 3634 222c 2022 6e75 6d70 795f 7479  at64", "numpy_ty
-00000a00: 7065 223a 2022 666c 6f61 7436 3422 2c20  pe": "float64", 
-00000a10: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
-00000a20: 7d2c 207b 226e 616d 6522 3a20 2272 615f  }, {"name": "ra_
-00000a30: 6572 726f 7222 2c20 2266 6965 6c64 5f6e  error", "field_n
-00000a40: 616d 6522 3a20 2272 615f 6572 726f 7222  ame": "ra_error"
-00000a50: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
-00000a60: 2022 696e 7436 3422 2c20 226e 756d 7079   "int64", "numpy
-00000a70: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
-00000a80: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
-00000a90: 6c7d 2c20 7b22 6e61 6d65 223a 2022 6465  l}, {"name": "de
-00000aa0: 635f 6572 726f 7222 2c20 2266 6965 6c64  c_error", "field
-00000ab0: 5f6e 616d 6522 3a20 2264 6563 5f65 7272  _name": "dec_err
-00000ac0: 6f72 222c 2022 7061 6e64 6173 5f74 7970  or", "pandas_typ
-00000ad0: 6522 3a20 2269 6e74 3634 222c 2022 6e75  e": "int64", "nu
-00000ae0: 6d70 795f 7479 7065 223a 2022 696e 7436  mpy_type": "int6
-00000af0: 3422 2c20 226d 6574 6164 6174 6122 3a20  4", "metadata": 
-00000b00: 6e75 6c6c 7d2c 207b 226e 616d 6522 3a20  null}, {"name": 
-00000b10: 6e75 6c6c 2c20 2266 6965 6c64 5f6e 616d  null, "field_nam
-00000b20: 6522 3a20 225f 5f69 6e64 6578 5f6c 6576  e": "__index_lev
-00000b30: 656c 5f30 5f5f 222c 2022 7061 6e64 6173  el_0__", "pandas
-00000b40: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
-00000b50: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
-00000b60: 696e 7436 3422 2c20 226d 6574 6164 6174  int64", "metadat
-00000b70: 6122 3a20 6e75 6c6c 7d5d 2c20 2263 7265  a": null}], "cre
-00000b80: 6174 6f72 223a 207b 226c 6962 7261 7279  ator": {"library
-00000b90: 223a 2022 7079 6172 726f 7722 2c20 2276  ": "pyarrow", "v
-00000ba0: 6572 7369 6f6e 223a 2022 392e 302e 3022  ersion": "9.0.0"
-00000bb0: 7d2c 2022 7061 6e64 6173 5f76 6572 7369  }, "pandas_versi
-00000bc0: 6f6e 223a 2022 312e 332e 3522 7d00 180c  on": "1.3.5"}...
-00000bd0: 4152 524f 573a 7363 6865 6d61 18c0 0e2f  ARROW:schema.../
-00000be0: 2f2f 2f2f 3267 4641 4141 5141 4141 4141  ////2gFAAAQAAAAA
-00000bf0: 4141 4b41 4134 4142 6741 4641 4167 4143  AAKAA4ABgAFAAgAC
-00000c00: 6741 4141 4141 4242 4141 5141 4141 4141  gAAAAABBAAQAAAAA
-00000c10: 4141 4b41 4177 4141 4141 4541 4167 4143  AAKAAwAAAAEAAgAC
-00000c20: 6741 4141 4e77 4441 4141 4541 4141 4141  gAAANwDAAAEAAAAA
-00000c30: 5141 4141 4177 4141 4141 4941 4177 4142  QAAAAwAAAAIAAwAB
-00000c40: 4141 4941 4167 4141 4141 4941 4141 4145  AAIAAgAAAAIAAAAE
-00000c50: 4141 4141 4159 4141 4142 7759 5735 6b59  AAAAAYAAABwYW5kY
-00000c60: 584d 4141 4b55 4441 4142 3749 6d6c 755a  XMAAKUDAAB7ImluZ
-00000c70: 4756 3458 324e 7662 4856 7462 6e4d 694f  GV4X2NvbHVtbnMiO
-00000c80: 6942 6249 6c39 6661 5735 6b5a 5868 6662  iBbIl9faW5kZXhfb
-00000c90: 4756 325a 5778 664d 4639 6649 6c30 7349  GV2ZWxfMF9fIl0sI
-00000ca0: 434a 6a62 3278 3162 5735 6661 5735 6b5a  CJjb2x1bW5faW5kZ
-00000cb0: 5868 6c63 7949 3649 4674 3749 6d35 6862  XhlcyI6IFt7Im5hb
-00000cc0: 5755 694f 6942 7564 5778 734c 4341 695a  WUiOiBudWxsLCAiZ
-00000cd0: 6d6c 6c62 4752 6662 6d46 745a 5349 3649  mllbGRfbmFtZSI6I
-00000ce0: 4735 3162 4777 7349 434a 7759 5735 6b59  G51bGwsICJwYW5kY
-00000cf0: 584e 6664 486c 775a 5349 3649 434a 3162  XNfdHlwZSI6ICJ1b
-00000d00: 6d6c 6a62 3252 6c49 6977 6749 6d35 3162  mljb2RlIiwgIm51b
-00000d10: 5842 3558 3352 3563 4755 694f 6941 6962  XB5X3R5cGUiOiAib
-00000d20: 324a 715a 574e 3049 6977 6749 6d31 6c64  2JqZWN0IiwgIm1ld
-00000d30: 4746 6b59 5852 6849 6a6f 6765 794a 6c62  GFkYXRhIjogeyJlb
-00000d40: 6d4e 765a 476c 755a 7949 3649 434a 5656  mNvZGluZyI6ICJVV
-00000d50: 4559 744f 434a 3966 5630 7349 434a 6a62  EYtOCJ9fV0sICJjb
-00000d60: 3278 3162 5735 7a49 6a6f 6757 3373 6962  2x1bW5zIjogW3sib
-00000d70: 6d46 745a 5349 3649 434a 705a 4349 7349  mFtZSI6ICJpZCIsI
-00000d80: 434a 6d61 5756 735a 4639 7559 5731 6c49  CJmaWVsZF9uYW1lI
-00000d90: 6a6f 6749 6d6c 6b49 6977 6749 6e42 6862  jogImlkIiwgInBhb
-00000da0: 6d52 6863 3139 3065 5842 6c49 6a6f 6749  mRhc190eXBlIjogI
-00000db0: 6d6c 7564 4459 3049 6977 6749 6d35 3162  mludDY0IiwgIm51b
-00000dc0: 5842 3558 3352 3563 4755 694f 6941 6961  XB5X3R5cGUiOiAia
-00000dd0: 5735 304e 6a51 694c 4341 6962 5756 3059  W50NjQiLCAibWV0Y
-00000de0: 5752 6864 4745 694f 6942 7564 5778 7366  WRhdGEiOiBudWxsf
-00000df0: 5377 6765 794a 7559 5731 6c49 6a6f 6749  SwgeyJuYW1lIjogI
-00000e00: 6e4a 6849 6977 6749 6d5a 705a 5778 6b58  nJhIiwgImZpZWxkX
-00000e10: 3235 6862 5755 694f 6941 6963 6d45 694c  25hbWUiOiAicmEiL
-00000e20: 4341 6963 4746 755a 4746 7a58 3352 3563  CAicGFuZGFzX3R5c
-00000e30: 4755 694f 6941 695a 6d78 7659 5851 324e  GUiOiAiZmxvYXQ2N
-00000e40: 4349 7349 434a 7564 5731 7765 5639 3065  CIsICJudW1weV90e
-00000e50: 5842 6c49 6a6f 6749 6d5a 7362 3246 304e  XBlIjogImZsb2F0N
-00000e60: 6a51 694c 4341 6962 5756 3059 5752 6864  jQiLCAibWV0YWRhd
-00000e70: 4745 694f 6942 7564 5778 7366 5377 6765  GEiOiBudWxsfSwge
-00000e80: 794a 7559 5731 6c49 6a6f 6749 6d52 6c59  yJuYW1lIjogImRlY
-00000e90: 7949 7349 434a 6d61 5756 735a 4639 7559  yIsICJmaWVsZF9uY
-00000ea0: 5731 6c49 6a6f 6749 6d52 6c59 7949 7349  W1lIjogImRlYyIsI
-00000eb0: 434a 7759 5735 6b59 584e 6664 486c 775a  CJwYW5kYXNfdHlwZ
-00000ec0: 5349 3649 434a 6d62 4739 6864 4459 3049  SI6ICJmbG9hdDY0I
-00000ed0: 6977 6749 6d35 3162 5842 3558 3352 3563  iwgIm51bXB5X3R5c
-00000ee0: 4755 694f 6941 695a 6d78 7659 5851 324e  GUiOiAiZmxvYXQ2N
-00000ef0: 4349 7349 434a 745a 5852 685a 4746 3059  CIsICJtZXRhZGF0Y
-00000f00: 5349 3649 4735 3162 4778 394c 4342 3749  SI6IG51bGx9LCB7I
-00000f10: 6d35 6862 5755 694f 6941 6963 6d46 665a  m5hbWUiOiAicmFfZ
-00000f20: 584a 7962 3349 694c 4341 695a 6d6c 6c62  XJyb3IiLCAiZmllb
-00000f30: 4752 6662 6d46 745a 5349 3649 434a 7959  GRfbmFtZSI6ICJyY
-00000f40: 5639 6c63 6e4a 7663 6949 7349 434a 7759  V9lcnJvciIsICJwY
-00000f50: 5735 6b59 584e 6664 486c 775a 5349 3649  W5kYXNfdHlwZSI6I
-00000f60: 434a 7062 6e51 324e 4349 7349 434a 7564  CJpbnQ2NCIsICJud
-00000f70: 5731 7765 5639 3065 5842 6c49 6a6f 6749  W1weV90eXBlIjogI
-00000f80: 6d6c 7564 4459 3049 6977 6749 6d31 6c64  mludDY0IiwgIm1ld
-00000f90: 4746 6b59 5852 6849 6a6f 6762 6e56 7362  GFkYXRhIjogbnVsb
-00000fa0: 4830 7349 4873 6962 6d46 745a 5349 3649  H0sIHsibmFtZSI6I
-00000fb0: 434a 6b5a 574e 665a 584a 7962 3349 694c  CJkZWNfZXJyb3IiL
-00000fc0: 4341 695a 6d6c 6c62 4752 6662 6d46 745a  CAiZmllbGRfbmFtZ
-00000fd0: 5349 3649 434a 6b5a 574e 665a 584a 7962  SI6ICJkZWNfZXJyb
-00000fe0: 3349 694c 4341 6963 4746 755a 4746 7a58  3IiLCAicGFuZGFzX
-00000ff0: 3352 3563 4755 694f 6941 6961 5735 304e  3R5cGUiOiAiaW50N
-00001000: 6a51 694c 4341 6962 6e56 7463 486c 6664  jQiLCAibnVtcHlfd
-00001010: 486c 775a 5349 3649 434a 7062 6e51 324e  HlwZSI6ICJpbnQ2N
-00001020: 4349 7349 434a 745a 5852 685a 4746 3059  CIsICJtZXRhZGF0Y
-00001030: 5349 3649 4735 3162 4778 394c 4342 3749  SI6IG51bGx9LCB7I
-00001040: 6d35 6862 5755 694f 6942 7564 5778 734c  m5hbWUiOiBudWxsL
-00001050: 4341 695a 6d6c 6c62 4752 6662 6d46 745a  CAiZmllbGRfbmFtZ
-00001060: 5349 3649 434a 6658 326c 755a 4756 3458  SI6ICJfX2luZGV4X
-00001070: 3278 6c64 6d56 7358 7a42 6658 7949 7349  2xldmVsXzBfXyIsI
-00001080: 434a 7759 5735 6b59 584e 6664 486c 775a  CJwYW5kYXNfdHlwZ
-00001090: 5349 3649 434a 7062 6e51 324e 4349 7349  SI6ICJpbnQ2NCIsI
-000010a0: 434a 7564 5731 7765 5639 3065 5842 6c49  CJudW1weV90eXBlI
-000010b0: 6a6f 6749 6d6c 7564 4459 3049 6977 6749  jogImludDY0IiwgI
-000010c0: 6d31 6c64 4746 6b59 5852 6849 6a6f 6762  m1ldGFkYXRhIjogb
-000010d0: 6e56 7362 4831 644c 4341 6959 334a 6c59  nVsbH1dLCAiY3JlY
-000010e0: 5852 7663 6949 3649 4873 6962 476c 6963  XRvciI6IHsibGlic
-000010f0: 6d46 7965 5349 3649 434a 7765 5746 7963  mFyeSI6ICJweWFyc
-00001100: 6d39 3349 6977 6749 6e5a 6c63 6e4e 7062  m93IiwgInZlcnNpb
-00001110: 3234 694f 6941 694f 5334 774c 6a41 6966  24iOiAiOS4wLjAif
-00001120: 5377 6749 6e42 6862 6d52 6863 3139 325a  SwgInBhbmRhc192Z
-00001130: 584a 7a61 5739 7549 6a6f 6749 6a45 754d  XJzaW9uIjogIjEuM
-00001140: 7934 3149 6e30 4141 4141 4741 4141 414a  y41In0AAAAGAAAAJ
-00001150: 4145 4141 4f41 4141 4143 3041 4141 4166  AEAAOAAAAC0AAAAf
-00001160: 4141 4141 4551 4141 4141 4541 4141 4142  AAAAEQAAAAEAAAAB
-00001170: 502f 2f2f 7741 4141 5149 5141 4141 414a  P///wAAAQIQAAAAJ
-00001180: 4141 4141 4151 4141 4141 4141 4141 4145  AAAAAQAAAAAAAAAE
-00001190: 5141 4141 4639 6661 5735 6b5a 5868 6662  QAAAF9faW5kZXhfb
-000011a0: 4756 325a 5778 664d 4639 6641 4141 4142  GV2ZWxfMF9fAAAAB
-000011b0: 502f 2f2f 7741 4141 4146 4141 4141 4151  P///wAAAAFAAAAAQ
-000011c0: 502f 2f2f 7741 4141 5149 5141 4141 4148  P///wAAAQIQAAAAH
-000011d0: 4141 4141 4151 4141 4141 4141 4141 4143  AAAAAQAAAAAAAAAC
-000011e0: 5141 4141 4752 6c59 3139 6c63 6e4a 7663  QAAAGRlY19lcnJvc
-000011f0: 6741 4141 446a 2f2f 2f38 4141 4141 4251  gAAADj///8AAAABQ
-00001200: 4141 4141 4854 2f2f 2f38 4141 4145 4345  AAAAHT///8AAAECE
-00001210: 4141 4141 4277 4141 4141 4541 4141 4141  AAAABwAAAAEAAAAA
-00001220: 4141 4141 4167 4141 4142 7959 5639 6c63  AAAAAgAAAByYV9lc
-00001230: 6e4a 7663 6741 4141 4142 732f 2f2f 2f41  nJvcgAAAABs////A
-00001240: 4141 4141 5541 4141 4143 6f2f 2f2f 2f41  AAAAUAAAACo////A
-00001250: 4141 4241 7841 4141 4141 5541 4141 4142  AABAxAAAAAUAAAAB
-00001260: 4141 4141 4141 4141 4141 4441 4141 415a  AAAAAAAAAADAAAAZ
-00001270: 4756 6a41 4e62 2f2f 2f38 4141 4149 4130  GVjANb///8AAAIA0
-00001280: 502f 2f2f 7741 4141 514d 5141 4141 4148  P///wAAAQMQAAAAH
-00001290: 4141 4141 4151 4141 4141 4141 4141 4141  AAAAAQAAAAAAAAAA
-000012a0: 6741 4141 484a 6841 4141 4141 4159 4143  gAAAHJhAAAAAAYAC
-000012b0: 4141 4741 4159 4141 4141 4141 4149 4145  AAGAAYAAAAAAAIAE
-000012c0: 4141 5541 4167 4142 6741 4841 4177 4141  AAUAAgABgAHAAwAA
-000012d0: 4141 5141 4241 4141 4141 4141 4145 4345  AAQABAAAAAAAAECE
-000012e0: 4141 4141 4277 4141 4141 4541 4141 4141  AAAABwAAAAEAAAAA
-000012f0: 4141 4141 4149 4141 4142 705a 4141 4143  AAAAAIAAABpZAAAC
-00001300: 4141 4d41 4167 4142 7741 4941 4141 4141  AAMAAgABwAIAAAAA
-00001310: 4141 4141 5541 4141 4141 4141 4141 4100  AAAAUAAAAAAAAAA.
-00001320: 181f 7061 7271 7565 742d 6370 702d 6172  ..parquet-cpp-ar
-00001330: 726f 7720 7665 7273 696f 6e20 392e 302e  row version 9.0.
-00001340: 3019 6c1c 0000 1c00 001c 0000 1c00 001c  0.l.............
-00001350: 0000 1c00 0000 020e 0000 5041 5231       ..........PAR1
+00000450: 1510 1502 0000 0015 0419 6c35 0018 0673  ..........l5...s
+00000460: 6368 656d 6115 0a00 1504 2502 1802 6964  chema.....%...id
+00000470: 0015 0a25 0218 0272 6100 150a 2502 1803  ...%...ra...%...
+00000480: 6465 6300 1504 2502 1808 7261 5f65 7272  dec...%...ra_err
+00000490: 6f72 0015 0425 0218 0964 6563 5f65 7272  or...%...dec_err
+000004a0: 6f72 0016 1419 1c19 5c26 ac02 1c15 0419  or......\&......
+000004b0: 3510 0006 1918 0269 6415 0216 1416 d802  5......id.......
+000004c0: 16a4 0226 8e01 2608 1c18 0822 0300 0000  ...&..&...."....
+000004d0: 0000 0018 0809 0300 0000 0000 0016 0028  ...............(
+000004e0: 0822 0300 0000 0000 0018 0809 0300 0000  ."..............
+000004f0: 0000 0000 192c 1504 1500 1502 0015 0015  .....,..........
+00000500: 1015 0200 0000 2684 061c 150a 1935 1000  ......&......5..
+00000510: 0619 1802 7261 1502 1614 16c8 0216 9e02  ....ra..........
+00000520: 26e6 0426 e603 1c18 0800 0000 0000 3873  &..&..........8s
+00000530: 4018 0800 0000 0000 b871 4016 0028 0800  @........q@..(..
+00000540: 0000 0000 3873 4018 0800 0000 0000 b871  ....8s@........q
+00000550: 4000 192c 1504 1500 1502 0015 0015 1015  @..,............
+00000560: 0200 0000 26de 091c 150a 1935 1000 0619  ....&......5....
+00000570: 1803 6465 6315 0216 1416 c802 169e 0226  ..dec..........&
+00000580: c008 26c0 071c 1808 0000 0000 00c0 41c0  ..&...........A.
+00000590: 1808 0000 0000 00c0 4ec0 1600 2808 0000  ........N...(...
+000005a0: 0000 00c0 41c0 1808 0000 0000 00c0 4ec0  ....A.........N.
+000005b0: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
+000005c0: 0000 0026 dc0c 1c15 0419 3510 0006 1918  ...&......5.....
+000005d0: 0872 615f 6572 726f 7215 0216 1416 b801  .ra_error.......
+000005e0: 16c0 0126 cc0b 269c 0b1c 1808 0000 0000  ...&..&.........
+000005f0: 0000 0000 1808 0000 0000 0000 0000 1600  ................
+00000600: 2808 0000 0000 0000 0000 1808 0000 0000  (...............
+00000610: 0000 0000 0019 2c15 0415 0015 0200 1500  ......,.........
+00000620: 1510 1502 0000 0026 e40f 1c15 0419 3510  .......&......5.
+00000630: 0006 1918 0964 6563 5f65 7272 6f72 1502  .....dec_error..
+00000640: 1614 16b8 0116 c001 26d4 0e26 a40e 1c18  ........&..&....
+00000650: 0800 0000 0000 0000 0018 0800 0000 0000  ................
+00000660: 0000 0016 0028 0800 0000 0000 0000 0018  .....(..........
+00000670: 0800 0000 0000 0000 0000 192c 1504 1500  ...........,....
+00000680: 1502 0015 0015 1015 0200 0000 16d8 0a16  ................
+00000690: 1426 0816 e009 1400 0019 2c18 0670 616e  .&........,..pan
+000006a0: 6461 7318 a705 7b22 696e 6465 785f 636f  das...{"index_co
+000006b0: 6c75 6d6e 7322 3a20 5b5d 2c20 2263 6f6c  lumns": [], "col
+000006c0: 756d 6e5f 696e 6465 7865 7322 3a20 5b5d  umn_indexes": []
+000006d0: 2c20 2263 6f6c 756d 6e73 223a 205b 7b22  , "columns": [{"
+000006e0: 6e61 6d65 223a 2022 6964 222c 2022 6669  name": "id", "fi
+000006f0: 656c 645f 6e61 6d65 223a 2022 6964 222c  eld_name": "id",
+00000700: 2022 7061 6e64 6173 5f74 7970 6522 3a20   "pandas_type": 
+00000710: 2269 6e74 3634 222c 2022 6e75 6d70 795f  "int64", "numpy_
+00000720: 7479 7065 223a 2022 696e 7436 3422 2c20  type": "int64", 
+00000730: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
+00000740: 7d2c 207b 226e 616d 6522 3a20 2272 6122  }, {"name": "ra"
+00000750: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
+00000760: 2272 6122 2c20 2270 616e 6461 735f 7479  "ra", "pandas_ty
+00000770: 7065 223a 2022 666c 6f61 7436 3422 2c20  pe": "float64", 
+00000780: 226e 756d 7079 5f74 7970 6522 3a20 2266  "numpy_type": "f
+00000790: 6c6f 6174 3634 222c 2022 6d65 7461 6461  loat64", "metada
+000007a0: 7461 223a 206e 756c 6c7d 2c20 7b22 6e61  ta": null}, {"na
+000007b0: 6d65 223a 2022 6465 6322 2c20 2266 6965  me": "dec", "fie
+000007c0: 6c64 5f6e 616d 6522 3a20 2264 6563 222c  ld_name": "dec",
+000007d0: 2022 7061 6e64 6173 5f74 7970 6522 3a20   "pandas_type": 
+000007e0: 2266 6c6f 6174 3634 222c 2022 6e75 6d70  "float64", "nump
+000007f0: 795f 7479 7065 223a 2022 666c 6f61 7436  y_type": "float6
+00000800: 3422 2c20 226d 6574 6164 6174 6122 3a20  4", "metadata": 
+00000810: 6e75 6c6c 7d2c 207b 226e 616d 6522 3a20  null}, {"name": 
+00000820: 2272 615f 6572 726f 7222 2c20 2266 6965  "ra_error", "fie
+00000830: 6c64 5f6e 616d 6522 3a20 2272 615f 6572  ld_name": "ra_er
+00000840: 726f 7222 2c20 2270 616e 6461 735f 7479  ror", "pandas_ty
+00000850: 7065 223a 2022 696e 7436 3422 2c20 226e  pe": "int64", "n
+00000860: 756d 7079 5f74 7970 6522 3a20 2269 6e74  umpy_type": "int
+00000870: 3634 222c 2022 6d65 7461 6461 7461 223a  64", "metadata":
+00000880: 206e 756c 6c7d 2c20 7b22 6e61 6d65 223a   null}, {"name":
+00000890: 2022 6465 635f 6572 726f 7222 2c20 2266   "dec_error", "f
+000008a0: 6965 6c64 5f6e 616d 6522 3a20 2264 6563  ield_name": "dec
+000008b0: 5f65 7272 6f72 222c 2022 7061 6e64 6173  _error", "pandas
+000008c0: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
+000008d0: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
+000008e0: 696e 7436 3422 2c20 226d 6574 6164 6174  int64", "metadat
+000008f0: 6122 3a20 6e75 6c6c 7d5d 2c20 2263 7265  a": null}], "cre
+00000900: 6174 6f72 223a 207b 226c 6962 7261 7279  ator": {"library
+00000910: 223a 2022 7079 6172 726f 7722 2c20 2276  ": "pyarrow", "v
+00000920: 6572 7369 6f6e 223a 2022 392e 302e 3022  ersion": "9.0.0"
+00000930: 7d2c 2022 7061 6e64 6173 5f76 6572 7369  }, "pandas_versi
+00000940: 6f6e 223a 2022 322e 302e 3022 7d00 180c  on": "2.0.0"}...
+00000950: 4152 524f 573a 7363 6865 6d61 1898 0b2f  ARROW:schema.../
+00000960: 2f2f 2f2f 7967 4541 4141 5141 4141 4141  ////ygEAAAQAAAAA
+00000970: 4141 4b41 4134 4142 6741 4641 4167 4143  AAKAA4ABgAFAAgAC
+00000980: 6741 4141 4141 4242 4141 5141 4141 4141  gAAAAABBAAQAAAAA
+00000990: 4141 4b41 4177 4141 4141 4541 4167 4143  AAKAAwAAAAEAAgAC
+000009a0: 6741 4141 4e77 4341 4141 4541 4141 4141  gAAANwCAAAEAAAAA
+000009b0: 5141 4141 4177 4141 4141 4941 4177 4142  QAAAAwAAAAIAAwAB
+000009c0: 4141 4941 4167 4141 4141 4941 4141 4145  AAIAAgAAAAIAAAAE
+000009d0: 4141 4141 4159 4141 4142 7759 5735 6b59  AAAAAYAAABwYW5kY
+000009e0: 584d 4141 4b63 4341 4142 3749 6d6c 755a  XMAAKcCAAB7ImluZ
+000009f0: 4756 3458 324e 7662 4856 7462 6e4d 694f  GV4X2NvbHVtbnMiO
+00000a00: 6942 6258 5377 6749 6d4e 7662 4856 7462  iBbXSwgImNvbHVtb
+00000a10: 6c39 7062 6d52 6c65 4756 7a49 6a6f 6757  l9pbmRleGVzIjogW
+00000a20: 3130 7349 434a 6a62 3278 3162 5735 7a49  10sICJjb2x1bW5zI
+00000a30: 6a6f 6757 3373 6962 6d46 745a 5349 3649  jogW3sibmFtZSI6I
+00000a40: 434a 705a 4349 7349 434a 6d61 5756 735a  CJpZCIsICJmaWVsZ
+00000a50: 4639 7559 5731 6c49 6a6f 6749 6d6c 6b49  F9uYW1lIjogImlkI
+00000a60: 6977 6749 6e42 6862 6d52 6863 3139 3065  iwgInBhbmRhc190e
+00000a70: 5842 6c49 6a6f 6749 6d6c 7564 4459 3049  XBlIjogImludDY0I
+00000a80: 6977 6749 6d35 3162 5842 3558 3352 3563  iwgIm51bXB5X3R5c
+00000a90: 4755 694f 6941 6961 5735 304e 6a51 694c  GUiOiAiaW50NjQiL
+00000aa0: 4341 6962 5756 3059 5752 6864 4745 694f  CAibWV0YWRhdGEiO
+00000ab0: 6942 7564 5778 7366 5377 6765 794a 7559  iBudWxsfSwgeyJuY
+00000ac0: 5731 6c49 6a6f 6749 6e4a 6849 6977 6749  W1lIjogInJhIiwgI
+00000ad0: 6d5a 705a 5778 6b58 3235 6862 5755 694f  mZpZWxkX25hbWUiO
+00000ae0: 6941 6963 6d45 694c 4341 6963 4746 755a  iAicmEiLCAicGFuZ
+00000af0: 4746 7a58 3352 3563 4755 694f 6941 695a  GFzX3R5cGUiOiAiZ
+00000b00: 6d78 7659 5851 324e 4349 7349 434a 7564  mxvYXQ2NCIsICJud
+00000b10: 5731 7765 5639 3065 5842 6c49 6a6f 6749  W1weV90eXBlIjogI
+00000b20: 6d5a 7362 3246 304e 6a51 694c 4341 6962  mZsb2F0NjQiLCAib
+00000b30: 5756 3059 5752 6864 4745 694f 6942 7564  WV0YWRhdGEiOiBud
+00000b40: 5778 7366 5377 6765 794a 7559 5731 6c49  WxsfSwgeyJuYW1lI
+00000b50: 6a6f 6749 6d52 6c59 7949 7349 434a 6d61  jogImRlYyIsICJma
+00000b60: 5756 735a 4639 7559 5731 6c49 6a6f 6749  WVsZF9uYW1lIjogI
+00000b70: 6d52 6c59 7949 7349 434a 7759 5735 6b59  mRlYyIsICJwYW5kY
+00000b80: 584e 6664 486c 775a 5349 3649 434a 6d62  XNfdHlwZSI6ICJmb
+00000b90: 4739 6864 4459 3049 6977 6749 6d35 3162  G9hdDY0IiwgIm51b
+00000ba0: 5842 3558 3352 3563 4755 694f 6941 695a  XB5X3R5cGUiOiAiZ
+00000bb0: 6d78 7659 5851 324e 4349 7349 434a 745a  mxvYXQ2NCIsICJtZ
+00000bc0: 5852 685a 4746 3059 5349 3649 4735 3162  XRhZGF0YSI6IG51b
+00000bd0: 4778 394c 4342 3749 6d35 6862 5755 694f  Gx9LCB7Im5hbWUiO
+00000be0: 6941 6963 6d46 665a 584a 7962 3349 694c  iAicmFfZXJyb3IiL
+00000bf0: 4341 695a 6d6c 6c62 4752 6662 6d46 745a  CAiZmllbGRfbmFtZ
+00000c00: 5349 3649 434a 7959 5639 6c63 6e4a 7663  SI6ICJyYV9lcnJvc
+00000c10: 6949 7349 434a 7759 5735 6b59 584e 6664  iIsICJwYW5kYXNfd
+00000c20: 486c 775a 5349 3649 434a 7062 6e51 324e  HlwZSI6ICJpbnQ2N
+00000c30: 4349 7349 434a 7564 5731 7765 5639 3065  CIsICJudW1weV90e
+00000c40: 5842 6c49 6a6f 6749 6d6c 7564 4459 3049  XBlIjogImludDY0I
+00000c50: 6977 6749 6d31 6c64 4746 6b59 5852 6849  iwgIm1ldGFkYXRhI
+00000c60: 6a6f 6762 6e56 7362 4830 7349 4873 6962  jogbnVsbH0sIHsib
+00000c70: 6d46 745a 5349 3649 434a 6b5a 574e 665a  mFtZSI6ICJkZWNfZ
+00000c80: 584a 7962 3349 694c 4341 695a 6d6c 6c62  XJyb3IiLCAiZmllb
+00000c90: 4752 6662 6d46 745a 5349 3649 434a 6b5a  GRfbmFtZSI6ICJkZ
+00000ca0: 574e 665a 584a 7962 3349 694c 4341 6963  WNfZXJyb3IiLCAic
+00000cb0: 4746 755a 4746 7a58 3352 3563 4755 694f  GFuZGFzX3R5cGUiO
+00000cc0: 6941 6961 5735 304e 6a51 694c 4341 6962  iAiaW50NjQiLCAib
+00000cd0: 6e56 7463 486c 6664 486c 775a 5349 3649  nVtcHlfdHlwZSI6I
+00000ce0: 434a 7062 6e51 324e 4349 7349 434a 745a  CJpbnQ2NCIsICJtZ
+00000cf0: 5852 685a 4746 3059 5349 3649 4735 3162  XRhZGF0YSI6IG51b
+00000d00: 4778 3958 5377 6749 6d4e 795a 5746 3062  Gx9XSwgImNyZWF0b
+00000d10: 3349 694f 6942 3749 6d78 7059 6e4a 6863  3IiOiB7ImxpYnJhc
+00000d20: 6e6b 694f 6941 6963 486c 6863 6e4a 7664  nkiOiAicHlhcnJvd
+00000d30: 7949 7349 434a 325a 584a 7a61 5739 7549  yIsICJ2ZXJzaW9uI
+00000d40: 6a6f 6749 6a6b 754d 4334 7749 6e30 7349  jogIjkuMC4wIn0sI
+00000d50: 434a 7759 5735 6b59 584e 6664 6d56 7963  CJwYW5kYXNfdmVyc
+00000d60: 326c 7662 6949 3649 4349 794c 6a41 754d  2lvbiI6ICIyLjAuM
+00000d70: 434a 3941 4155 4141 4144 6b41 4141 416f  CJ9AAUAAADkAAAAo
+00000d80: 4141 4141 4851 4141 4141 3841 4141 4142  AAAAHQAAAA8AAAAB
+00000d90: 4141 4141 4544 2f2f 2f38 4141 4145 4345  AAAAED///8AAAECE
+00000da0: 4141 4141 4277 4141 4141 4541 4141 4141  AAAABwAAAAEAAAAA
+00000db0: 4141 4141 416b 4141 4142 6b5a 574e 665a  AAAAAkAAABkZWNfZ
+00000dc0: 584a 7962 3349 4141 4141 342f 2f2f 2f41  XJyb3IAAAA4////A
+00000dd0: 4141 4141 5541 4141 4142 302f 2f2f 2f41  AAAAUAAAAB0////A
+00000de0: 4141 4241 6841 4141 4141 6341 4141 4142  AABAhAAAAAcAAAAB
+00000df0: 4141 4141 4141 4141 4141 4941 4141 4163  AAAAAAAAAAIAAAAc
+00000e00: 6d46 665a 584a 7962 3349 4141 4141 4162  mFfZXJyb3IAAAAAb
+00000e10: 502f 2f2f 7741 4141 4146 4141 4141 4171  P///wAAAAFAAAAAq
+00000e20: 502f 2f2f 7741 4141 514d 5141 4141 4146  P///wAAAQMQAAAAF
+00000e30: 4141 4141 4151 4141 4141 4141 4141 4141  AAAAAQAAAAAAAAAA
+00000e40: 7741 4141 4752 6c59 7744 572f 2f2f 2f41  wAAAGRlYwDW////A
+00000e50: 4141 4341 4e44 2f2f 2f38 4141 4145 4445  AACAND///8AAAEDE
+00000e60: 4141 4141 4277 4141 4141 4541 4141 4141  AAAABwAAAAEAAAAA
+00000e70: 4141 4141 4149 4141 4142 7959 5141 4141  AAAAAIAAAByYQAAA
+00000e80: 4141 4741 4167 4142 6741 4741 4141 4141  AAGAAgABgAGAAAAA
+00000e90: 4141 4341 4241 4146 4141 4941 4159 4142  AACABAAFAAIAAYAB
+00000ea0: 7741 4d41 4141 4145 4141 5141 4141 4141  wAMAAAAEAAQAAAAA
+00000eb0: 4141 4241 6841 4141 4141 6341 4141 4142  AABAhAAAAAcAAAAB
+00000ec0: 4141 4141 4141 4141 4141 4341 4141 4161  AAAAAAAAAACAAAAa
+00000ed0: 5751 4141 4167 4144 4141 4941 4163 4143  WQAAAgADAAIAAcAC
+00000ee0: 4141 4141 4141 4141 4146 4141 4141 4141  AAAAAAAAAFAAAAAA
+00000ef0: 4141 4141 413d 3d00 181f 7061 7271 7565  AAAAA==...parque
+00000f00: 742d 6370 702d 6172 726f 7720 7665 7273  t-cpp-arrow vers
+00000f10: 696f 6e20 392e 302e 3019 5c1c 0000 1c00  ion 9.0.0.\.....
+00000f20: 001c 0000 1c00 001c 0000 00d4 0a00 0050  ...............P
+00000f30: 4152 31                                  AR1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_46/shard_1.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet`

 * *Files 17% similar despite different names*

```diff
@@ -1,311 +1,240 @@
-00000000: 5041 5231 1504 15b0 0115 704c 1516 1500  PAR1......pL....
-00000010: 1200 0058 08bc 0200 0501 00bd 0d08 00c2  ...X............
-00000020: 0d08 00c4 0d08 00c5 0d08 00c7 0d08 00c8  ................
-00000030: 0d08 00c9 0d08 00ca 0d08 3ccb 0200 0000  ..........<.....
-00000040: 0000 00cd 0200 0000 0000 0015 0015 2015  .............. .
-00000050: 242c 1516 1510 1506 1506 1c18 08cd 0200  $,..............
-00000060: 0000 0000 0018 08bc 0200 0000 0000 0016  ................
-00000070: 0028 08cd 0200 0000 0000 0018 08bc 0200  .(..............
-00000080: 0000 0000 0000 0000 103c 0200 0000 1601  .........<......
-00000090: 0405 1032 5476 980a 0000 26b4 021c 1504  ...2Tv....&.....
-000000a0: 1935 1000 0619 1802 6964 1502 1616 16e8  .5......id......
-000000b0: 0216 ac02 2696 0126 081c 1808 cd02 0000  ....&..&........
-000000c0: 0000 0000 1808 bc02 0000 0000 0000 1600  ................
-000000d0: 2808 cd02 0000 0000 0000 1808 bc02 0000  (...............
-000000e0: 0000 0000 0019 2c15 0415 0015 0200 1500  ......,.........
-000000f0: 1510 1502 0000 0015 0415 a001 156c 4c15  .............lL.
-00000100: 1415 0012 0000 5000 0001 0108 a871 4001  ......P......q@.
-00000110: 0708 00b8 7209 0800 980d 0804 3873 0910  ....r.......8s..
-00000120: 0068 0d10 0018 0d10 0008 0d10 00a8 0d08  .h..............
-00000130: 28f8 7240 0000 0000 0088 7140 1500 1520  (.r@......q@... 
-00000140: 1524 2c15 1615 1015 0615 061c 1808 0000  .$,.............
-00000150: 0000 0038 7340 1808 0000 0000 0088 7140  ...8s@........q@
-00000160: 1600 2808 0000 0000 0038 7340 1808 0000  ..(......8s@....
-00000170: 0000 0088 7140 0000 0010 3c02 0000 0016  ....q@....<.....
-00000180: 0104 0510 3254 7698 0800 0026 9606 1c15  ....2Tv....&....
-00000190: 0a19 3510 0006 1918 0272 6115 0216 1616  ..5......ra.....
-000001a0: d802 16a8 0226 f804 26ee 031c 1808 0000  .....&..&.......
-000001b0: 0000 0038 7340 1808 0000 0000 0088 7140  ...8s@........q@
-000001c0: 1600 2808 0000 0000 0038 7340 1808 0000  ..(......8s@....
-000001d0: 0000 0088 7140 0019 2c15 0415 0015 0200  ....q@..,.......
-000001e0: 1500 1510 1502 0000 0015 0415 9001 155e  ...............^
-000001f0: 4c15 1215 0012 0000 4800 0001 0108 404d  L.......H.....@M
-00000200: c001 0708 0040 480d 0800 4209 0800 c011  .....@H...B.....
-00000210: 0800 460d 100d 2004 c044 0d10 2441 c000  ..F... ..D..$A..
-00000220: 0000 0000 c045 c015 0015 2015 242c 1516  .....E.... .$,..
-00000230: 1510 1506 1506 1c18 0800 0000 0000 c041  ...............A
-00000240: c018 0800 0000 0000 404d c016 0028 0800  ........@M...(..
-00000250: 0000 0000 c041 c018 0800 0000 0000 404d  .....A........@M
-00000260: c000 0000 103c 0200 0000 1601 0405 1032  .....<.........2
-00000270: 5465 7308 0000 26ec 091c 150a 1935 1000  Tes...&......5..
-00000280: 0619 1803 6465 6315 0216 1616 c802 169a  ....dec.........
-00000290: 0226 ce08 26d2 071c 1808 0000 0000 00c0  .&..&...........
-000002a0: 41c0 1808 0000 0000 0040 4dc0 1600 2808  A........@M...(.
-000002b0: 0000 0000 00c0 41c0 1808 0000 0000 0040  ......A........@
-000002c0: 4dc0 0019 2c15 0415 0015 0200 1500 1510  M...,...........
-000002d0: 1502 0000 0015 0415 1015 144c 1502 1500  ...........L....
-000002e0: 1200 0008 1c00 0000 0000 0000 0015 0015  ................
-000002f0: 1215 162c 1516 1510 1506 1506 1c18 0800  ...,............
-00000300: 0000 0000 0000 0018 0800 0000 0000 0000  ................
-00000310: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
-00000320: 0000 0000 0000 0000 0000 0920 0200 0000  ........... ....
-00000330: 1601 0116 0026 ea0c 1c15 0419 3510 0006  .....&......5...
-00000340: 1918 0872 615f 6572 726f 7215 0216 1616  ...ra_error.....
-00000350: b801 16c0 0126 da0b 26aa 0b1c 1808 0000  .....&..&.......
-00000360: 0000 0000 0000 1808 0000 0000 0000 0000  ................
-00000370: 1600 2808 0000 0000 0000 0000 1808 0000  ..(.............
-00000380: 0000 0000 0000 0019 2c15 0415 0015 0200  ........,.......
-00000390: 1500 1510 1502 0000 0015 0415 1015 144c  ...............L
-000003a0: 1502 1500 1200 0008 1c00 0000 0000 0000  ................
-000003b0: 0015 0015 1215 162c 1516 1510 1506 1506  .......,........
-000003c0: 1c18 0800 0000 0000 0000 0018 0800 0000  ................
-000003d0: 0000 0000 0016 0028 0800 0000 0000 0000  .......(........
-000003e0: 0018 0800 0000 0000 0000 0000 0000 0920  ............... 
-000003f0: 0200 0000 1601 0116 0026 f20f 1c15 0419  .........&......
-00000400: 3510 0006 1918 0964 6563 5f65 7272 6f72  5......dec_error
-00000410: 1502 1616 16b8 0116 c001 26e2 0e26 b20e  ..........&..&..
-00000420: 1c18 0800 0000 0000 0000 0018 0800 0000  ................
-00000430: 0000 0000 0016 0028 0800 0000 0000 0000  .......(........
-00000440: 0018 0800 0000 0000 0000 0000 192c 1504  .............,..
-00000450: 1500 1502 0015 0015 1015 0200 0000 1504  ................
-00000460: 15b0 0115 6c4c 1516 1500 1200 0058 0000  ....lL.......X..
-00000470: 0d01 0001 0d08 0006 0d08 0008 0d08 0009  ................
-00000480: 0d08 000b 0d08 000c 0d08 000d 0d08 000e  ................
-00000490: 0d08 3c0f 0000 0000 0000 0011 0000 0000  ..<.............
-000004a0: 0000 0015 0015 2015 242c 1516 1510 1506  ...... .$,......
-000004b0: 1506 1c18 0811 0000 0000 0000 0018 0800  ................
-000004c0: 0000 0000 0000 0016 0028 0811 0000 0000  .........(......
-000004d0: 0000 0018 0800 0000 0000 0000 0000 0000  ................
-000004e0: 103c 0200 0000 1601 0405 1032 5476 980a  .<.........2Tv..
-000004f0: 0000 26e4 131c 1504 1935 1000 0619 1811  ..&......5......
-00000500: 5f5f 696e 6465 785f 6c65 7665 6c5f 305f  __index_level_0_
-00000510: 5f15 0216 1616 e802 16a8 0226 c612 26bc  _..........&..&.
-00000520: 111c 1808 1100 0000 0000 0000 1808 0000  ................
-00000530: 0000 0000 0000 1600 2808 1100 0000 0000  ........(.......
-00000540: 0000 1808 0000 0000 0000 0000 0019 2c15  ..............,.
-00000550: 0415 0015 0200 1500 1510 1502 0000 0015  ................
-00000560: 0419 7c35 0018 0673 6368 656d 6115 0c00  ..|5...schema...
-00000570: 1504 2502 1802 6964 0015 0a25 0218 0272  ..%...id...%...r
-00000580: 6100 150a 2502 1803 6465 6300 1504 2502  a...%...dec...%.
-00000590: 1808 7261 5f65 7272 6f72 0015 0425 0218  ..ra_error...%..
-000005a0: 0964 6563 5f65 7272 6f72 0015 0425 0218  .dec_error...%..
-000005b0: 115f 5f69 6e64 6578 5f6c 6576 656c 5f30  .__index_level_0
-000005c0: 5f5f 0016 1619 1c19 6c26 b402 1c15 0419  __......l&......
-000005d0: 3510 0006 1918 0269 6415 0216 1616 e802  5......id.......
-000005e0: 16ac 0226 9601 2608 1c18 08cd 0200 0000  ...&..&.........
-000005f0: 0000 0018 08bc 0200 0000 0000 0016 0028  ...............(
-00000600: 08cd 0200 0000 0000 0018 08bc 0200 0000  ................
-00000610: 0000 0000 192c 1504 1500 1502 0015 0015  .....,..........
-00000620: 1015 0200 0000 2696 061c 150a 1935 1000  ......&......5..
-00000630: 0619 1802 7261 1502 1616 16d8 0216 a802  ....ra..........
-00000640: 26f8 0426 ee03 1c18 0800 0000 0000 3873  &..&..........8s
-00000650: 4018 0800 0000 0000 8871 4016 0028 0800  @........q@..(..
-00000660: 0000 0000 3873 4018 0800 0000 0000 8871  ....8s@........q
-00000670: 4000 192c 1504 1500 1502 0015 0015 1015  @..,............
-00000680: 0200 0000 26ec 091c 150a 1935 1000 0619  ....&......5....
-00000690: 1803 6465 6315 0216 1616 c802 169a 0226  ..dec..........&
-000006a0: ce08 26d2 071c 1808 0000 0000 00c0 41c0  ..&...........A.
-000006b0: 1808 0000 0000 0040 4dc0 1600 2808 0000  .......@M...(...
-000006c0: 0000 00c0 41c0 1808 0000 0000 0040 4dc0  ....A........@M.
-000006d0: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
-000006e0: 0000 0026 ea0c 1c15 0419 3510 0006 1918  ...&......5.....
-000006f0: 0872 615f 6572 726f 7215 0216 1616 b801  .ra_error.......
-00000700: 16c0 0126 da0b 26aa 0b1c 1808 0000 0000  ...&..&.........
-00000710: 0000 0000 1808 0000 0000 0000 0000 1600  ................
-00000720: 2808 0000 0000 0000 0000 1808 0000 0000  (...............
-00000730: 0000 0000 0019 2c15 0415 0015 0200 1500  ......,.........
-00000740: 1510 1502 0000 0026 f20f 1c15 0419 3510  .......&......5.
-00000750: 0006 1918 0964 6563 5f65 7272 6f72 1502  .....dec_error..
-00000760: 1616 16b8 0116 c001 26e2 0e26 b20e 1c18  ........&..&....
-00000770: 0800 0000 0000 0000 0018 0800 0000 0000  ................
-00000780: 0000 0016 0028 0800 0000 0000 0000 0018  .....(..........
-00000790: 0800 0000 0000 0000 0000 192c 1504 1500  ...........,....
-000007a0: 1502 0015 0015 1015 0200 0000 26e4 131c  ............&...
-000007b0: 1504 1935 1000 0619 1811 5f5f 696e 6465  ...5......__inde
-000007c0: 785f 6c65 7665 6c5f 305f 5f15 0216 1616  x_level_0__.....
-000007d0: e802 16a8 0226 c612 26bc 111c 1808 1100  .....&..&.......
-000007e0: 0000 0000 0000 1808 0000 0000 0000 0000  ................
-000007f0: 1600 2808 1100 0000 0000 0000 1808 0000  ..(.............
-00000800: 0000 0000 0000 0019 2c15 0415 0015 0200  ........,.......
-00000810: 1500 1510 1502 0000 0016 e00d 1616 2608  ..............&.
-00000820: 1696 0c14 0000 192c 1806 7061 6e64 6173  .......,..pandas
-00000830: 18a5 077b 2269 6e64 6578 5f63 6f6c 756d  ...{"index_colum
-00000840: 6e73 223a 205b 225f 5f69 6e64 6578 5f6c  ns": ["__index_l
-00000850: 6576 656c 5f30 5f5f 225d 2c20 2263 6f6c  evel_0__"], "col
-00000860: 756d 6e5f 696e 6465 7865 7322 3a20 5b7b  umn_indexes": [{
-00000870: 226e 616d 6522 3a20 6e75 6c6c 2c20 2266  "name": null, "f
-00000880: 6965 6c64 5f6e 616d 6522 3a20 6e75 6c6c  ield_name": null
-00000890: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
-000008a0: 2022 756e 6963 6f64 6522 2c20 226e 756d   "unicode", "num
-000008b0: 7079 5f74 7970 6522 3a20 226f 626a 6563  py_type": "objec
-000008c0: 7422 2c20 226d 6574 6164 6174 6122 3a20  t", "metadata": 
-000008d0: 7b22 656e 636f 6469 6e67 223a 2022 5554  {"encoding": "UT
-000008e0: 462d 3822 7d7d 5d2c 2022 636f 6c75 6d6e  F-8"}}], "column
-000008f0: 7322 3a20 5b7b 226e 616d 6522 3a20 2269  s": [{"name": "i
-00000900: 6422 2c20 2266 6965 6c64 5f6e 616d 6522  d", "field_name"
-00000910: 3a20 2269 6422 2c20 2270 616e 6461 735f  : "id", "pandas_
-00000920: 7479 7065 223a 2022 696e 7436 3422 2c20  type": "int64", 
-00000930: 226e 756d 7079 5f74 7970 6522 3a20 2269  "numpy_type": "i
-00000940: 6e74 3634 222c 2022 6d65 7461 6461 7461  nt64", "metadata
-00000950: 223a 206e 756c 6c7d 2c20 7b22 6e61 6d65  ": null}, {"name
-00000960: 223a 2022 7261 222c 2022 6669 656c 645f  ": "ra", "field_
-00000970: 6e61 6d65 223a 2022 7261 222c 2022 7061  name": "ra", "pa
-00000980: 6e64 6173 5f74 7970 6522 3a20 2266 6c6f  ndas_type": "flo
-00000990: 6174 3634 222c 2022 6e75 6d70 795f 7479  at64", "numpy_ty
-000009a0: 7065 223a 2022 666c 6f61 7436 3422 2c20  pe": "float64", 
-000009b0: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
-000009c0: 7d2c 207b 226e 616d 6522 3a20 2264 6563  }, {"name": "dec
-000009d0: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
-000009e0: 2022 6465 6322 2c20 2270 616e 6461 735f   "dec", "pandas_
-000009f0: 7479 7065 223a 2022 666c 6f61 7436 3422  type": "float64"
-00000a00: 2c20 226e 756d 7079 5f74 7970 6522 3a20  , "numpy_type": 
-00000a10: 2266 6c6f 6174 3634 222c 2022 6d65 7461  "float64", "meta
-00000a20: 6461 7461 223a 206e 756c 6c7d 2c20 7b22  data": null}, {"
-00000a30: 6e61 6d65 223a 2022 7261 5f65 7272 6f72  name": "ra_error
-00000a40: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
-00000a50: 2022 7261 5f65 7272 6f72 222c 2022 7061   "ra_error", "pa
-00000a60: 6e64 6173 5f74 7970 6522 3a20 2269 6e74  ndas_type": "int
-00000a70: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
-00000a80: 223a 2022 696e 7436 3422 2c20 226d 6574  ": "int64", "met
-00000a90: 6164 6174 6122 3a20 6e75 6c6c 7d2c 207b  adata": null}, {
-00000aa0: 226e 616d 6522 3a20 2264 6563 5f65 7272  "name": "dec_err
-00000ab0: 6f72 222c 2022 6669 656c 645f 6e61 6d65  or", "field_name
-00000ac0: 223a 2022 6465 635f 6572 726f 7222 2c20  ": "dec_error", 
-00000ad0: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
-00000ae0: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
-00000af0: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
-00000b00: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
-00000b10: 2c20 7b22 6e61 6d65 223a 206e 756c 6c2c  , {"name": null,
-00000b20: 2022 6669 656c 645f 6e61 6d65 223a 2022   "field_name": "
-00000b30: 5f5f 696e 6465 785f 6c65 7665 6c5f 305f  __index_level_0_
-00000b40: 5f22 2c20 2270 616e 6461 735f 7479 7065  _", "pandas_type
-00000b50: 223a 2022 696e 7436 3422 2c20 226e 756d  ": "int64", "num
-00000b60: 7079 5f74 7970 6522 3a20 2269 6e74 3634  py_type": "int64
-00000b70: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
-00000b80: 756c 6c7d 5d2c 2022 6372 6561 746f 7222  ull}], "creator"
-00000b90: 3a20 7b22 6c69 6272 6172 7922 3a20 2270  : {"library": "p
-00000ba0: 7961 7272 6f77 222c 2022 7665 7273 696f  yarrow", "versio
-00000bb0: 6e22 3a20 2239 2e30 2e30 227d 2c20 2270  n": "9.0.0"}, "p
-00000bc0: 616e 6461 735f 7665 7273 696f 6e22 3a20  andas_version": 
-00000bd0: 2231 2e33 2e35 227d 0018 0c41 5252 4f57  "1.3.5"}...ARROW
-00000be0: 3a73 6368 656d 6118 c00e 2f2f 2f2f 2f32  :schema.../////2
-00000bf0: 6746 4141 4151 4141 4141 4141 414b 4141  gFAAAQAAAAAAAKAA
-00000c00: 3441 4267 4146 4141 6741 4367 4141 4141  4ABgAFAAgACgAAAA
-00000c10: 4142 4241 4151 4141 4141 4141 414b 4141  ABBAAQAAAAAAAKAA
-00000c20: 7741 4141 4145 4141 6741 4367 4141 414e  wAAAAEAAgACgAAAN
-00000c30: 7744 4141 4145 4141 4141 4151 4141 4141  wDAAAEAAAAAQAAAA
-00000c40: 7741 4141 4149 4141 7741 4241 4149 4141  wAAAAIAAwABAAIAA
-00000c50: 6741 4141 4149 4141 4141 4541 4141 4141  gAAAAIAAAAEAAAAA
-00000c60: 5941 4141 4277 5957 356b 5958 4d41 414b  YAAABwYW5kYXMAAK
-00000c70: 5544 4141 4237 496d 6c75 5a47 5634 5832  UDAAB7ImluZGV4X2
-00000c80: 4e76 6248 5674 626e 4d69 4f69 4262 496c  NvbHVtbnMiOiBbIl
-00000c90: 3966 6157 356b 5a58 6866 6247 5632 5a57  9faW5kZXhfbGV2ZW
-00000ca0: 7866 4d46 3966 496c 3073 4943 4a6a 6232  xfMF9fIl0sICJjb2
-00000cb0: 7831 6257 3566 6157 356b 5a58 686c 6379  x1bW5faW5kZXhlcy
-00000cc0: 4936 4946 7437 496d 3568 6257 5569 4f69  I6IFt7Im5hbWUiOi
-00000cd0: 4275 6457 7873 4c43 4169 5a6d 6c6c 6247  BudWxsLCAiZmllbG
-00000ce0: 5266 626d 4674 5a53 4936 4947 3531 6247  RfbmFtZSI6IG51bG
-00000cf0: 7773 4943 4a77 5957 356b 5958 4e66 6448  wsICJwYW5kYXNfdH
-00000d00: 6c77 5a53 4936 4943 4a31 626d 6c6a 6232  lwZSI6ICJ1bmljb2
-00000d10: 526c 4969 7767 496d 3531 6258 4235 5833  RlIiwgIm51bXB5X3
-00000d20: 5235 6347 5569 4f69 4169 6232 4a71 5a57  R5cGUiOiAib2JqZW
-00000d30: 4e30 4969 7767 496d 316c 6447 466b 5958  N0IiwgIm1ldGFkYX
-00000d40: 5268 496a 6f67 6579 4a6c 626d 4e76 5a47  RhIjogeyJlbmNvZG
-00000d50: 6c75 5a79 4936 4943 4a56 5645 5974 4f43  luZyI6ICJVVEYtOC
-00000d60: 4a39 6656 3073 4943 4a6a 6232 7831 6257  J9fV0sICJjb2x1bW
-00000d70: 357a 496a 6f67 5733 7369 626d 4674 5a53  5zIjogW3sibmFtZS
-00000d80: 4936 4943 4a70 5a43 4973 4943 4a6d 6157  I6ICJpZCIsICJmaW
-00000d90: 5673 5a46 3975 5957 316c 496a 6f67 496d  VsZF9uYW1lIjogIm
-00000da0: 6c6b 4969 7767 496e 4268 626d 5268 6331  lkIiwgInBhbmRhc1
-00000db0: 3930 6558 426c 496a 6f67 496d 6c75 6444  90eXBlIjogImludD
-00000dc0: 5930 4969 7767 496d 3531 6258 4235 5833  Y0IiwgIm51bXB5X3
-00000dd0: 5235 6347 5569 4f69 4169 6157 3530 4e6a  R5cGUiOiAiaW50Nj
-00000de0: 5169 4c43 4169 6257 5630 5957 5268 6447  QiLCAibWV0YWRhdG
-00000df0: 4569 4f69 4275 6457 7873 6653 7767 6579  EiOiBudWxsfSwgey
-00000e00: 4a75 5957 316c 496a 6f67 496e 4a68 4969  JuYW1lIjogInJhIi
-00000e10: 7767 496d 5a70 5a57 786b 5832 3568 6257  wgImZpZWxkX25hbW
-00000e20: 5569 4f69 4169 636d 4569 4c43 4169 6347  UiOiAicmEiLCAicG
-00000e30: 4675 5a47 467a 5833 5235 6347 5569 4f69  FuZGFzX3R5cGUiOi
-00000e40: 4169 5a6d 7876 5958 5132 4e43 4973 4943  AiZmxvYXQ2NCIsIC
-00000e50: 4a75 6457 3177 6556 3930 6558 426c 496a  JudW1weV90eXBlIj
-00000e60: 6f67 496d 5a73 6232 4630 4e6a 5169 4c43  ogImZsb2F0NjQiLC
-00000e70: 4169 6257 5630 5957 5268 6447 4569 4f69  AibWV0YWRhdGEiOi
-00000e80: 4275 6457 7873 6653 7767 6579 4a75 5957  BudWxsfSwgeyJuYW
-00000e90: 316c 496a 6f67 496d 526c 5979 4973 4943  1lIjogImRlYyIsIC
-00000ea0: 4a6d 6157 5673 5a46 3975 5957 316c 496a  JmaWVsZF9uYW1lIj
-00000eb0: 6f67 496d 526c 5979 4973 4943 4a77 5957  ogImRlYyIsICJwYW
-00000ec0: 356b 5958 4e66 6448 6c77 5a53 4936 4943  5kYXNfdHlwZSI6IC
-00000ed0: 4a6d 6247 3968 6444 5930 4969 7767 496d  JmbG9hdDY0IiwgIm
-00000ee0: 3531 6258 4235 5833 5235 6347 5569 4f69  51bXB5X3R5cGUiOi
-00000ef0: 4169 5a6d 7876 5958 5132 4e43 4973 4943  AiZmxvYXQ2NCIsIC
-00000f00: 4a74 5a58 5268 5a47 4630 5953 4936 4947  JtZXRhZGF0YSI6IG
-00000f10: 3531 6247 7839 4c43 4237 496d 3568 6257  51bGx9LCB7Im5hbW
-00000f20: 5569 4f69 4169 636d 4666 5a58 4a79 6233  UiOiAicmFfZXJyb3
-00000f30: 4969 4c43 4169 5a6d 6c6c 6247 5266 626d  IiLCAiZmllbGRfbm
-00000f40: 4674 5a53 4936 4943 4a79 5956 396c 636e  FtZSI6ICJyYV9lcn
-00000f50: 4a76 6369 4973 4943 4a77 5957 356b 5958  JvciIsICJwYW5kYX
-00000f60: 4e66 6448 6c77 5a53 4936 4943 4a70 626e  NfdHlwZSI6ICJpbn
-00000f70: 5132 4e43 4973 4943 4a75 6457 3177 6556  Q2NCIsICJudW1weV
-00000f80: 3930 6558 426c 496a 6f67 496d 6c75 6444  90eXBlIjogImludD
-00000f90: 5930 4969 7767 496d 316c 6447 466b 5958  Y0IiwgIm1ldGFkYX
-00000fa0: 5268 496a 6f67 626e 5673 6248 3073 4948  RhIjogbnVsbH0sIH
-00000fb0: 7369 626d 4674 5a53 4936 4943 4a6b 5a57  sibmFtZSI6ICJkZW
-00000fc0: 4e66 5a58 4a79 6233 4969 4c43 4169 5a6d  NfZXJyb3IiLCAiZm
-00000fd0: 6c6c 6247 5266 626d 4674 5a53 4936 4943  llbGRfbmFtZSI6IC
-00000fe0: 4a6b 5a57 4e66 5a58 4a79 6233 4969 4c43  JkZWNfZXJyb3IiLC
-00000ff0: 4169 6347 4675 5a47 467a 5833 5235 6347  AicGFuZGFzX3R5cG
-00001000: 5569 4f69 4169 6157 3530 4e6a 5169 4c43  UiOiAiaW50NjQiLC
-00001010: 4169 626e 5674 6348 6c66 6448 6c77 5a53  AibnVtcHlfdHlwZS
-00001020: 4936 4943 4a70 626e 5132 4e43 4973 4943  I6ICJpbnQ2NCIsIC
-00001030: 4a74 5a58 5268 5a47 4630 5953 4936 4947  JtZXRhZGF0YSI6IG
-00001040: 3531 6247 7839 4c43 4237 496d 3568 6257  51bGx9LCB7Im5hbW
-00001050: 5569 4f69 4275 6457 7873 4c43 4169 5a6d  UiOiBudWxsLCAiZm
-00001060: 6c6c 6247 5266 626d 4674 5a53 4936 4943  llbGRfbmFtZSI6IC
-00001070: 4a66 5832 6c75 5a47 5634 5832 786c 646d  JfX2luZGV4X2xldm
-00001080: 5673 587a 4266 5879 4973 4943 4a77 5957  VsXzBfXyIsICJwYW
-00001090: 356b 5958 4e66 6448 6c77 5a53 4936 4943  5kYXNfdHlwZSI6IC
-000010a0: 4a70 626e 5132 4e43 4973 4943 4a75 6457  JpbnQ2NCIsICJudW
-000010b0: 3177 6556 3930 6558 426c 496a 6f67 496d  1weV90eXBlIjogIm
-000010c0: 6c75 6444 5930 4969 7767 496d 316c 6447  ludDY0IiwgIm1ldG
-000010d0: 466b 5958 5268 496a 6f67 626e 5673 6248  FkYXRhIjogbnVsbH
-000010e0: 3164 4c43 4169 5933 4a6c 5958 5276 6369  1dLCAiY3JlYXRvci
-000010f0: 4936 4948 7369 6247 6c69 636d 4679 6553  I6IHsibGlicmFyeS
-00001100: 4936 4943 4a77 6557 4679 636d 3933 4969  I6ICJweWFycm93Ii
-00001110: 7767 496e 5a6c 636e 4e70 6232 3469 4f69  wgInZlcnNpb24iOi
-00001120: 4169 4f53 3477 4c6a 4169 6653 7767 496e  AiOS4wLjAifSwgIn
-00001130: 4268 626d 5268 6331 3932 5a58 4a7a 6157  BhbmRhc192ZXJzaW
-00001140: 3975 496a 6f67 496a 4575 4d79 3431 496e  9uIjogIjEuMy41In
-00001150: 3041 4141 4147 4141 4141 4a41 4541 414f  0AAAAGAAAAJAEAAO
-00001160: 4141 4141 4330 4141 4141 6641 4141 4145  AAAAC0AAAAfAAAAE
-00001170: 5141 4141 4145 4141 4141 4250 2f2f 2f77  QAAAAEAAAABP///w
-00001180: 4141 4151 4951 4141 4141 4a41 4141 4141  AAAQIQAAAAJAAAAA
-00001190: 5141 4141 4141 4141 4141 4551 4141 4146  QAAAAAAAAAEQAAAF
-000011a0: 3966 6157 356b 5a58 6866 6247 5632 5a57  9faW5kZXhfbGV2ZW
-000011b0: 7866 4d46 3966 4141 4141 4250 2f2f 2f77  xfMF9fAAAABP///w
-000011c0: 4141 4141 4641 4141 4141 5150 2f2f 2f77  AAAAFAAAAAQP///w
-000011d0: 4141 4151 4951 4141 4141 4841 4141 4141  AAAQIQAAAAHAAAAA
-000011e0: 5141 4141 4141 4141 4141 4351 4141 4147  QAAAAAAAAACQAAAG
-000011f0: 526c 5931 396c 636e 4a76 6367 4141 4144  RlY19lcnJvcgAAAD
-00001200: 6a2f 2f2f 3841 4141 4142 5141 4141 4148  j///8AAAABQAAAAH
-00001210: 542f 2f2f 3841 4141 4543 4541 4141 4142  T///8AAAECEAAAAB
-00001220: 7741 4141 4145 4141 4141 4141 4141 4141  wAAAAEAAAAAAAAAA
-00001230: 6741 4141 4279 5956 396c 636e 4a76 6367  gAAAByYV9lcnJvcg
-00001240: 4141 4141 4273 2f2f 2f2f 4141 4141 4155  AAAABs////AAAAAU
-00001250: 4141 4141 436f 2f2f 2f2f 4141 4142 4178  AAAACo////AAABAx
-00001260: 4141 4141 4155 4141 4141 4241 4141 4141  AAAAAUAAAABAAAAA
-00001270: 4141 4141 4144 4141 4141 5a47 566a 414e  AAAAADAAAAZGVjAN
-00001280: 622f 2f2f 3841 4141 4941 3050 2f2f 2f77  b///8AAAIA0P///w
-00001290: 4141 4151 4d51 4141 4141 4841 4141 4141  AAAQMQAAAAHAAAAA
-000012a0: 5141 4141 4141 4141 4141 4167 4141 4148  QAAAAAAAAAAgAAAH
-000012b0: 4a68 4141 4141 4141 5941 4341 4147 4141  JhAAAAAAYACAAGAA
-000012c0: 5941 4141 4141 4141 4941 4541 4155 4141  YAAAAAAAIAEAAUAA
-000012d0: 6741 4267 4148 4141 7741 4141 4151 4142  gABgAHAAwAAAAQAB
-000012e0: 4141 4141 4141 4141 4543 4541 4141 4142  AAAAAAAAECEAAAAB
-000012f0: 7741 4141 4145 4141 4141 4141 4141 4141  wAAAAEAAAAAAAAAA
-00001300: 4941 4141 4270 5a41 4141 4341 414d 4141  IAAABpZAAACAAMAA
-00001310: 6741 4277 4149 4141 4141 4141 4141 4155  gABwAIAAAAAAAAAU
-00001320: 4141 4141 4141 4141 4141 0018 1f70 6172  AAAAAAAAAA...par
-00001330: 7175 6574 2d63 7070 2d61 7272 6f77 2076  quet-cpp-arrow v
-00001340: 6572 7369 6f6e 2039 2e30 2e30 196c 1c00  ersion 9.0.0.l..
-00001350: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
-00001360: 0002 0e00 0050 4152 31                   .....PAR1
+00000000: 5041 5231 1504 1560 1548 4c15 0c15 0012  PAR1...`.HL.....
+00000010: 0000 3008 d502 0005 0100 d70d 0800 e40d  ..0.............
+00000020: 0800 e50d 083c ea02 0000 0000 0000 ed02  .....<..........
+00000030: 0000 0000 0000 1500 1516 151a 2c15 0c15  ............,...
+00000040: 1015 0615 061c 1808 ed02 0000 0000 0000  ................
+00000050: 1808 d502 0000 0000 0000 1600 2808 ed02  ............(...
+00000060: 0000 0000 0000 1808 d502 0000 0000 0000  ................
+00000070: 0000 000b 2802 0000 000c 0103 0388 c602  ....(...........
+00000080: 2680 021c 1504 1935 1000 0619 1802 6964  &......5......id
+00000090: 1502 160c 168c 0216 f801 266c 2608 1c18  ..........&l&...
+000000a0: 08ed 0200 0000 0000 0018 08d5 0200 0000  ................
+000000b0: 0000 0016 0028 08ed 0200 0000 0000 0018  .....(..........
+000000c0: 08d5 0200 0000 0000 0000 192c 1504 1500  ...........,....
+000000d0: 1502 0015 0015 1015 0200 0000 1504 1560  ...............`
+000000e0: 154a 4c15 0c15 0012 0000 3000 0001 0108  .JL.......0.....
+000000f0: 4873 4001 0708 00d8 7209 0800 280d 1000  Hs@.....r...(...
+00000100: f80d 1028 b871 4000 0000 0000 5872 4015  ...(.q@.....Xr@.
+00000110: 0015 1615 1a2c 150c 1510 1506 1506 1c18  .....,..........
+00000120: 0800 0000 0000 4873 4018 0800 0000 0000  ......Hs@.......
+00000130: b871 4016 0028 0800 0000 0000 4873 4018  .q@..(......Hs@.
+00000140: 0800 0000 0000 b871 4000 0000 0b28 0200  .......q@....(..
+00000150: 0000 0c01 0303 88c6 0226 b205 1c15 0a19  .........&......
+00000160: 3510 0006 1918 0272 6115 0216 0c16 8c02  5......ra.......
+00000170: 16fa 0126 9e04 26b8 031c 1808 0000 0000  ...&..&.........
+00000180: 0048 7340 1808 0000 0000 00b8 7140 1600  .Hs@........q@..
+00000190: 2808 0000 0000 0048 7340 1808 0000 0000  (......Hs@......
+000001a0: 00b8 7140 0019 2c15 0415 0015 0200 1500  ..q@..,.........
+000001b0: 1510 1502 0000 0015 0415 6015 4e4c 150c  ..........`.NL..
+000001c0: 1500 1200 0030 0000 0101 0cc0 44c0 0001  .....0......D...
+000001d0: 0104 4046 0908 04c0 4009 0804 4043 0908  ..@F....@...@C..
+000001e0: 2880 3fc0 0000 0000 00c0 4bc0 1500 1516  (.?.......K.....
+000001f0: 151a 2c15 0c15 1015 0615 061c 1808 0000  ..,.............
+00000200: 0000 0080 3fc0 1808 0000 0000 00c0 4bc0  ....?.........K.
+00000210: 1600 2808 0000 0000 0080 3fc0 1808 0000  ..(.......?.....
+00000220: 0000 00c0 4bc0 0000 000b 2802 0000 000c  ....K.....(.....
+00000230: 0103 0388 c602 26ec 081c 150a 1935 1000  ......&......5..
+00000240: 0619 1803 6465 6315 0216 0c16 8c02 16fe  ....dec.........
+00000250: 0126 d807 26ee 061c 1808 0000 0000 0080  .&..&...........
+00000260: 3fc0 1808 0000 0000 00c0 4bc0 1600 2808  ?.........K...(.
+00000270: 0000 0000 0080 3fc0 1808 0000 0000 00c0  ......?.........
+00000280: 4bc0 0019 2c15 0415 0015 0200 1500 1510  K...,...........
+00000290: 1502 0000 0015 0415 1015 144c 1502 1500  ...........L....
+000002a0: 1200 0008 1c00 0000 0000 0000 0015 0015  ................
+000002b0: 1215 162c 150c 1510 1506 1506 1c18 0800  ...,............
+000002c0: 0000 0000 0000 0018 0800 0000 0000 0000  ................
+000002d0: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
+000002e0: 0000 0000 0000 0000 0000 0920 0200 0000  ........... ....
+000002f0: 0c01 010c 0026 ea0b 1c15 0419 3510 0006  .....&......5...
+00000300: 1918 0872 615f 6572 726f 7215 0216 0c16  ...ra_error.....
+00000310: b801 16c0 0126 da0a 26aa 0a1c 1808 0000  .....&..&.......
+00000320: 0000 0000 0000 1808 0000 0000 0000 0000  ................
+00000330: 1600 2808 0000 0000 0000 0000 1808 0000  ..(.............
+00000340: 0000 0000 0000 0019 2c15 0415 0015 0200  ........,.......
+00000350: 1500 1510 1502 0000 0015 0415 1015 144c  ...............L
+00000360: 1502 1500 1200 0008 1c00 0000 0000 0000  ................
+00000370: 0015 0015 1215 162c 150c 1510 1506 1506  .......,........
+00000380: 1c18 0800 0000 0000 0000 0018 0800 0000  ................
+00000390: 0000 0000 0016 0028 0800 0000 0000 0000  .......(........
+000003a0: 0018 0800 0000 0000 0000 0000 0000 0920  ............... 
+000003b0: 0200 0000 0c01 010c 0026 f20e 1c15 0419  .........&......
+000003c0: 3510 0006 1918 0964 6563 5f65 7272 6f72  5......dec_error
+000003d0: 1502 160c 16b8 0116 c001 26e2 0d26 b20d  ..........&..&..
+000003e0: 1c18 0800 0000 0000 0000 0018 0800 0000  ................
+000003f0: 0000 0000 0016 0028 0800 0000 0000 0000  .......(........
+00000400: 0018 0800 0000 0000 0000 0000 192c 1504  .............,..
+00000410: 1500 1502 0015 0015 1015 0200 0000 1504  ................
+00000420: 196c 3500 1806 7363 6865 6d61 150a 0015  .l5...schema....
+00000430: 0425 0218 0269 6400 150a 2502 1802 7261  .%...id...%...ra
+00000440: 0015 0a25 0218 0364 6563 0015 0425 0218  ...%...dec...%..
+00000450: 0872 615f 6572 726f 7200 1504 2502 1809  .ra_error...%...
+00000460: 6465 635f 6572 726f 7200 160c 191c 195c  dec_error......\
+00000470: 2680 021c 1504 1935 1000 0619 1802 6964  &......5......id
+00000480: 1502 160c 168c 0216 f801 266c 2608 1c18  ..........&l&...
+00000490: 08ed 0200 0000 0000 0018 08d5 0200 0000  ................
+000004a0: 0000 0016 0028 08ed 0200 0000 0000 0018  .....(..........
+000004b0: 08d5 0200 0000 0000 0000 192c 1504 1500  ...........,....
+000004c0: 1502 0015 0015 1015 0200 0000 26b2 051c  ............&...
+000004d0: 150a 1935 1000 0619 1802 7261 1502 160c  ...5......ra....
+000004e0: 168c 0216 fa01 269e 0426 b803 1c18 0800  ......&..&......
+000004f0: 0000 0000 4873 4018 0800 0000 0000 b871  ....Hs@........q
+00000500: 4016 0028 0800 0000 0000 4873 4018 0800  @..(......Hs@...
+00000510: 0000 0000 b871 4000 192c 1504 1500 1502  .....q@..,......
+00000520: 0015 0015 1015 0200 0000 26ec 081c 150a  ..........&.....
+00000530: 1935 1000 0619 1803 6465 6315 0216 0c16  .5......dec.....
+00000540: 8c02 16fe 0126 d807 26ee 061c 1808 0000  .....&..&.......
+00000550: 0000 0080 3fc0 1808 0000 0000 00c0 4bc0  ....?.........K.
+00000560: 1600 2808 0000 0000 0080 3fc0 1808 0000  ..(.......?.....
+00000570: 0000 00c0 4bc0 0019 2c15 0415 0015 0200  ....K...,.......
+00000580: 1500 1510 1502 0000 0026 ea0b 1c15 0419  .........&......
+00000590: 3510 0006 1918 0872 615f 6572 726f 7215  5......ra_error.
+000005a0: 0216 0c16 b801 16c0 0126 da0a 26aa 0a1c  .........&..&...
+000005b0: 1808 0000 0000 0000 0000 1808 0000 0000  ................
+000005c0: 0000 0000 1600 2808 0000 0000 0000 0000  ......(.........
+000005d0: 1808 0000 0000 0000 0000 0019 2c15 0415  ............,...
+000005e0: 0015 0200 1500 1510 1502 0000 0026 f20e  .............&..
+000005f0: 1c15 0419 3510 0006 1918 0964 6563 5f65  ....5......dec_e
+00000600: 7272 6f72 1502 160c 16b8 0116 c001 26e2  rror..........&.
+00000610: 0d26 b20d 1c18 0800 0000 0000 0000 0018  .&..............
+00000620: 0800 0000 0000 0000 0016 0028 0800 0000  ...........(....
+00000630: 0000 0000 0018 0800 0000 0000 0000 0000  ................
+00000640: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
+00000650: 0000 1694 0916 0c26 0816 f008 1400 0019  .......&........
+00000660: 2c18 0670 616e 6461 7318 a705 7b22 696e  ,..pandas...{"in
+00000670: 6465 785f 636f 6c75 6d6e 7322 3a20 5b5d  dex_columns": []
+00000680: 2c20 2263 6f6c 756d 6e5f 696e 6465 7865  , "column_indexe
+00000690: 7322 3a20 5b5d 2c20 2263 6f6c 756d 6e73  s": [], "columns
+000006a0: 223a 205b 7b22 6e61 6d65 223a 2022 6964  ": [{"name": "id
+000006b0: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
+000006c0: 2022 6964 222c 2022 7061 6e64 6173 5f74   "id", "pandas_t
+000006d0: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
+000006e0: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
+000006f0: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
+00000700: 3a20 6e75 6c6c 7d2c 207b 226e 616d 6522  : null}, {"name"
+00000710: 3a20 2272 6122 2c20 2266 6965 6c64 5f6e  : "ra", "field_n
+00000720: 616d 6522 3a20 2272 6122 2c20 2270 616e  ame": "ra", "pan
+00000730: 6461 735f 7479 7065 223a 2022 666c 6f61  das_type": "floa
+00000740: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
+00000750: 6522 3a20 2266 6c6f 6174 3634 222c 2022  e": "float64", "
+00000760: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
+00000770: 2c20 7b22 6e61 6d65 223a 2022 6465 6322  , {"name": "dec"
+00000780: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
+00000790: 2264 6563 222c 2022 7061 6e64 6173 5f74  "dec", "pandas_t
+000007a0: 7970 6522 3a20 2266 6c6f 6174 3634 222c  ype": "float64",
+000007b0: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
+000007c0: 666c 6f61 7436 3422 2c20 226d 6574 6164  float64", "metad
+000007d0: 6174 6122 3a20 6e75 6c6c 7d2c 207b 226e  ata": null}, {"n
+000007e0: 616d 6522 3a20 2272 615f 6572 726f 7222  ame": "ra_error"
+000007f0: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
+00000800: 2272 615f 6572 726f 7222 2c20 2270 616e  "ra_error", "pan
+00000810: 6461 735f 7479 7065 223a 2022 696e 7436  das_type": "int6
+00000820: 3422 2c20 226e 756d 7079 5f74 7970 6522  4", "numpy_type"
+00000830: 3a20 2269 6e74 3634 222c 2022 6d65 7461  : "int64", "meta
+00000840: 6461 7461 223a 206e 756c 6c7d 2c20 7b22  data": null}, {"
+00000850: 6e61 6d65 223a 2022 6465 635f 6572 726f  name": "dec_erro
+00000860: 7222 2c20 2266 6965 6c64 5f6e 616d 6522  r", "field_name"
+00000870: 3a20 2264 6563 5f65 7272 6f72 222c 2022  : "dec_error", "
+00000880: 7061 6e64 6173 5f74 7970 6522 3a20 2269  pandas_type": "i
+00000890: 6e74 3634 222c 2022 6e75 6d70 795f 7479  nt64", "numpy_ty
+000008a0: 7065 223a 2022 696e 7436 3422 2c20 226d  pe": "int64", "m
+000008b0: 6574 6164 6174 6122 3a20 6e75 6c6c 7d5d  etadata": null}]
+000008c0: 2c20 2263 7265 6174 6f72 223a 207b 226c  , "creator": {"l
+000008d0: 6962 7261 7279 223a 2022 7079 6172 726f  ibrary": "pyarro
+000008e0: 7722 2c20 2276 6572 7369 6f6e 223a 2022  w", "version": "
+000008f0: 392e 302e 3022 7d2c 2022 7061 6e64 6173  9.0.0"}, "pandas
+00000900: 5f76 6572 7369 6f6e 223a 2022 322e 302e  _version": "2.0.
+00000910: 3022 7d00 180c 4152 524f 573a 7363 6865  0"}...ARROW:sche
+00000920: 6d61 1898 0b2f 2f2f 2f2f 7967 4541 4141  ma.../////ygEAAA
+00000930: 5141 4141 4141 4141 4b41 4134 4142 6741  QAAAAAAAKAA4ABgA
+00000940: 4641 4167 4143 6741 4141 4141 4242 4141  FAAgACgAAAAABBAA
+00000950: 5141 4141 4141 4141 4b41 4177 4141 4141  QAAAAAAAKAAwAAAA
+00000960: 4541 4167 4143 6741 4141 4e77 4341 4141  EAAgACgAAANwCAAA
+00000970: 4541 4141 4141 5141 4141 4177 4141 4141  EAAAAAQAAAAwAAAA
+00000980: 4941 4177 4142 4141 4941 4167 4141 4141  IAAwABAAIAAgAAAA
+00000990: 4941 4141 4145 4141 4141 4159 4141 4142  IAAAAEAAAAAYAAAB
+000009a0: 7759 5735 6b59 584d 4141 4b63 4341 4142  wYW5kYXMAAKcCAAB
+000009b0: 3749 6d6c 755a 4756 3458 324e 7662 4856  7ImluZGV4X2NvbHV
+000009c0: 7462 6e4d 694f 6942 6258 5377 6749 6d4e  tbnMiOiBbXSwgImN
+000009d0: 7662 4856 7462 6c39 7062 6d52 6c65 4756  vbHVtbl9pbmRleGV
+000009e0: 7a49 6a6f 6757 3130 7349 434a 6a62 3278  zIjogW10sICJjb2x
+000009f0: 3162 5735 7a49 6a6f 6757 3373 6962 6d46  1bW5zIjogW3sibmF
+00000a00: 745a 5349 3649 434a 705a 4349 7349 434a  tZSI6ICJpZCIsICJ
+00000a10: 6d61 5756 735a 4639 7559 5731 6c49 6a6f  maWVsZF9uYW1lIjo
+00000a20: 6749 6d6c 6b49 6977 6749 6e42 6862 6d52  gImlkIiwgInBhbmR
+00000a30: 6863 3139 3065 5842 6c49 6a6f 6749 6d6c  hc190eXBlIjogIml
+00000a40: 7564 4459 3049 6977 6749 6d35 3162 5842  udDY0IiwgIm51bXB
+00000a50: 3558 3352 3563 4755 694f 6941 6961 5735  5X3R5cGUiOiAiaW5
+00000a60: 304e 6a51 694c 4341 6962 5756 3059 5752  0NjQiLCAibWV0YWR
+00000a70: 6864 4745 694f 6942 7564 5778 7366 5377  hdGEiOiBudWxsfSw
+00000a80: 6765 794a 7559 5731 6c49 6a6f 6749 6e4a  geyJuYW1lIjogInJ
+00000a90: 6849 6977 6749 6d5a 705a 5778 6b58 3235  hIiwgImZpZWxkX25
+00000aa0: 6862 5755 694f 6941 6963 6d45 694c 4341  hbWUiOiAicmEiLCA
+00000ab0: 6963 4746 755a 4746 7a58 3352 3563 4755  icGFuZGFzX3R5cGU
+00000ac0: 694f 6941 695a 6d78 7659 5851 324e 4349  iOiAiZmxvYXQ2NCI
+00000ad0: 7349 434a 7564 5731 7765 5639 3065 5842  sICJudW1weV90eXB
+00000ae0: 6c49 6a6f 6749 6d5a 7362 3246 304e 6a51  lIjogImZsb2F0NjQ
+00000af0: 694c 4341 6962 5756 3059 5752 6864 4745  iLCAibWV0YWRhdGE
+00000b00: 694f 6942 7564 5778 7366 5377 6765 794a  iOiBudWxsfSwgeyJ
+00000b10: 7559 5731 6c49 6a6f 6749 6d52 6c59 7949  uYW1lIjogImRlYyI
+00000b20: 7349 434a 6d61 5756 735a 4639 7559 5731  sICJmaWVsZF9uYW1
+00000b30: 6c49 6a6f 6749 6d52 6c59 7949 7349 434a  lIjogImRlYyIsICJ
+00000b40: 7759 5735 6b59 584e 6664 486c 775a 5349  wYW5kYXNfdHlwZSI
+00000b50: 3649 434a 6d62 4739 6864 4459 3049 6977  6ICJmbG9hdDY0Iiw
+00000b60: 6749 6d35 3162 5842 3558 3352 3563 4755  gIm51bXB5X3R5cGU
+00000b70: 694f 6941 695a 6d78 7659 5851 324e 4349  iOiAiZmxvYXQ2NCI
+00000b80: 7349 434a 745a 5852 685a 4746 3059 5349  sICJtZXRhZGF0YSI
+00000b90: 3649 4735 3162 4778 394c 4342 3749 6d35  6IG51bGx9LCB7Im5
+00000ba0: 6862 5755 694f 6941 6963 6d46 665a 584a  hbWUiOiAicmFfZXJ
+00000bb0: 7962 3349 694c 4341 695a 6d6c 6c62 4752  yb3IiLCAiZmllbGR
+00000bc0: 6662 6d46 745a 5349 3649 434a 7959 5639  fbmFtZSI6ICJyYV9
+00000bd0: 6c63 6e4a 7663 6949 7349 434a 7759 5735  lcnJvciIsICJwYW5
+00000be0: 6b59 584e 6664 486c 775a 5349 3649 434a  kYXNfdHlwZSI6ICJ
+00000bf0: 7062 6e51 324e 4349 7349 434a 7564 5731  pbnQ2NCIsICJudW1
+00000c00: 7765 5639 3065 5842 6c49 6a6f 6749 6d6c  weV90eXBlIjogIml
+00000c10: 7564 4459 3049 6977 6749 6d31 6c64 4746  udDY0IiwgIm1ldGF
+00000c20: 6b59 5852 6849 6a6f 6762 6e56 7362 4830  kYXRhIjogbnVsbH0
+00000c30: 7349 4873 6962 6d46 745a 5349 3649 434a  sIHsibmFtZSI6ICJ
+00000c40: 6b5a 574e 665a 584a 7962 3349 694c 4341  kZWNfZXJyb3IiLCA
+00000c50: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
+00000c60: 3649 434a 6b5a 574e 665a 584a 7962 3349  6ICJkZWNfZXJyb3I
+00000c70: 694c 4341 6963 4746 755a 4746 7a58 3352  iLCAicGFuZGFzX3R
+00000c80: 3563 4755 694f 6941 6961 5735 304e 6a51  5cGUiOiAiaW50NjQ
+00000c90: 694c 4341 6962 6e56 7463 486c 6664 486c  iLCAibnVtcHlfdHl
+00000ca0: 775a 5349 3649 434a 7062 6e51 324e 4349  wZSI6ICJpbnQ2NCI
+00000cb0: 7349 434a 745a 5852 685a 4746 3059 5349  sICJtZXRhZGF0YSI
+00000cc0: 3649 4735 3162 4778 3958 5377 6749 6d4e  6IG51bGx9XSwgImN
+00000cd0: 795a 5746 3062 3349 694f 6942 3749 6d78  yZWF0b3IiOiB7Imx
+00000ce0: 7059 6e4a 6863 6e6b 694f 6941 6963 486c  pYnJhcnkiOiAicHl
+00000cf0: 6863 6e4a 7664 7949 7349 434a 325a 584a  hcnJvdyIsICJ2ZXJ
+00000d00: 7a61 5739 7549 6a6f 6749 6a6b 754d 4334  zaW9uIjogIjkuMC4
+00000d10: 7749 6e30 7349 434a 7759 5735 6b59 584e  wIn0sICJwYW5kYXN
+00000d20: 6664 6d56 7963 326c 7662 6949 3649 4349  fdmVyc2lvbiI6ICI
+00000d30: 794c 6a41 754d 434a 3941 4155 4141 4144  yLjAuMCJ9AAUAAAD
+00000d40: 6b41 4141 416f 4141 4141 4851 4141 4141  kAAAAoAAAAHQAAAA
+00000d50: 3841 4141 4142 4141 4141 4544 2f2f 2f38  8AAAABAAAAED///8
+00000d60: 4141 4145 4345 4141 4141 4277 4141 4141  AAAECEAAAABwAAAA
+00000d70: 4541 4141 4141 4141 4141 416b 4141 4142  EAAAAAAAAAAkAAAB
+00000d80: 6b5a 574e 665a 584a 7962 3349 4141 4141  kZWNfZXJyb3IAAAA
+00000d90: 342f 2f2f 2f41 4141 4141 5541 4141 4142  4////AAAAAUAAAAB
+00000da0: 302f 2f2f 2f41 4141 4241 6841 4141 4141  0////AAABAhAAAAA
+00000db0: 6341 4141 4142 4141 4141 4141 4141 4141  cAAAABAAAAAAAAAA
+00000dc0: 4941 4141 4163 6d46 665a 584a 7962 3349  IAAAAcmFfZXJyb3I
+00000dd0: 4141 4141 4162 502f 2f2f 7741 4141 4146  AAAAAbP///wAAAAF
+00000de0: 4141 4141 4171 502f 2f2f 7741 4141 514d  AAAAAqP///wAAAQM
+00000df0: 5141 4141 4146 4141 4141 4151 4141 4141  QAAAAFAAAAAQAAAA
+00000e00: 4141 4141 4141 7741 4141 4752 6c59 7744  AAAAAAwAAAGRlYwD
+00000e10: 572f 2f2f 2f41 4141 4341 4e44 2f2f 2f38  W////AAACAND///8
+00000e20: 4141 4145 4445 4141 4141 4277 4141 4141  AAAEDEAAAABwAAAA
+00000e30: 4541 4141 4141 4141 4141 4149 4141 4142  EAAAAAAAAAAIAAAB
+00000e40: 7959 5141 4141 4141 4741 4167 4142 6741  yYQAAAAAGAAgABgA
+00000e50: 4741 4141 4141 4141 4341 4241 4146 4141  GAAAAAAACABAAFAA
+00000e60: 4941 4159 4142 7741 4d41 4141 4145 4141  IAAYABwAMAAAAEAA
+00000e70: 5141 4141 4141 4141 4241 6841 4141 4141  QAAAAAAABAhAAAAA
+00000e80: 6341 4141 4142 4141 4141 4141 4141 4141  cAAAABAAAAAAAAAA
+00000e90: 4341 4141 4161 5751 4141 4167 4144 4141  CAAAAaWQAAAgADAA
+00000ea0: 4941 4163 4143 4141 4141 4141 4141 4146  IAAcACAAAAAAAAAF
+00000eb0: 4141 4141 4141 4141 4141 413d 3d00 181f  AAAAAAAAAAA==...
+00000ec0: 7061 7271 7565 742d 6370 702d 6172 726f  parquet-cpp-arro
+00000ed0: 7720 7665 7273 696f 6e20 392e 302e 3019  w version 9.0.0.
+00000ee0: 5c1c 0000 1c00 001c 0000 1c00 001c 0000  \...............
+00000ef0: 00d3 0a00 0050 4152 31                   .....PAR1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_46/shard_2.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet`

 * *Files 19% similar despite different names*

```diff
@@ -1,311 +1,256 @@
-00000000: 5041 5231 1504 15b0 0115 744c 1516 1500  PAR1......tL....
-00000010: 1200 0058 08f0 0200 0501 00f1 0d08 00f3  ...X............
-00000020: 0d08 00f7 0d08 00fb 0d08 00fc 0d08 00fd  ................
-00000030: 0d08 0401 0305 3704 0002 0d08 3c05 0300  ......7.....<...
-00000040: 0000 0000 0006 0300 0000 0000 0015 0015  ................
-00000050: 2015 242c 1516 1510 1506 1506 1c18 0806   .$,............
-00000060: 0300 0000 0000 0018 08f0 0200 0000 0000  ................
-00000070: 0016 0028 0806 0300 0000 0000 0018 08f0  ...(............
-00000080: 0200 0000 0000 0000 0000 103c 0200 0000  ...........<....
-00000090: 1601 0405 1032 5476 980a 0000 26b8 021c  .....2Tv....&...
-000000a0: 1504 1935 1000 0619 1802 6964 1502 1616  ...5......id....
-000000b0: 16e8 0216 b002 269a 0126 081c 1808 0603  ......&..&......
-000000c0: 0000 0000 0000 1808 f002 0000 0000 0000  ................
-000000d0: 1600 2808 0603 0000 0000 0000 1808 f002  ..(.............
-000000e0: 0000 0000 0000 0019 2c15 0415 0015 0200  ........,.......
-000000f0: 1500 1510 1502 0000 0015 0415 9001 1560  ...............`
-00000100: 4c15 1215 0012 0000 4800 0001 0108 3872  L.......H.....8r
-00000110: 4001 0708 0038 7309 0800 f80d 1000 2811  @....8s.......(.
-00000120: 080d 1800 980d 1004 d871 0928 2858 7240  .........q.((Xr@
-00000130: 0000 0000 0098 7140 1500 1520 1524 2c15  ......q@... .$,.
-00000140: 1615 1015 0615 061c 1808 0000 0000 0038  ...............8
-00000150: 7340 1808 0000 0000 0098 7140 1600 2808  s@........q@..(.
-00000160: 0000 0000 0038 7340 1808 0000 0000 0098  .....8s@........
-00000170: 7140 0000 0010 3c02 0000 0016 0104 0510  q@....<.........
-00000180: 3254 1476 0800 0026 8e06 1c15 0a19 3510  2T.v...&......5.
-00000190: 0006 1918 0272 6115 0216 1616 c802 169c  .....ra.........
-000001a0: 0226 f004 26f2 031c 1808 0000 0000 0038  .&..&..........8
-000001b0: 7340 1808 0000 0000 0098 7140 1600 2808  s@........q@..(.
-000001c0: 0000 0000 0038 7340 1808 0000 0000 0098  .....8s@........
-000001d0: 7140 0019 2c15 0415 0015 0200 1500 1510  q@..,...........
-000001e0: 1502 0000 0015 0415 9001 1568 4c15 1215  ...........hL...
-000001f0: 0012 0000 4800 0001 0108 4041 c001 0708  ....H.....@A....
-00000200: 00c0 4609 0804 4043 0d08 0048 0908 00c0  ..F...@C...H....
-00000210: 0d20 0440 4509 1004 803d 0908 2840 49c0  . .@E....=..(@I.
-00000220: 0000 0000 0040 4bc0 1500 1520 1524 2c15  .....@K.... .$,.
-00000230: 1615 1015 0615 061c 1808 0000 0000 0080  ................
-00000240: 3dc0 1808 0000 0000 0040 4bc0 1600 2808  =........@K...(.
-00000250: 0000 0000 0080 3dc0 1808 0000 0000 0040  ......=........@
-00000260: 4bc0 0000 0010 3c02 0000 0016 0104 0510  K.....<.........
-00000270: 3212 5476 0800 0026 ee09 1c15 0a19 3510  2.Tv...&......5.
-00000280: 0006 1918 0364 6563 1502 1616 16c8 0216  .....dec........
-00000290: a402 26d0 0826 ca07 1c18 0800 0000 0000  ..&..&..........
-000002a0: 803d c018 0800 0000 0000 404b c016 0028  .=........@K...(
-000002b0: 0800 0000 0000 803d c018 0800 0000 0000  .......=........
-000002c0: 404b c000 192c 1504 1500 1502 0015 0015  @K...,..........
-000002d0: 1015 0200 0000 1504 1510 1514 4c15 0215  ............L...
-000002e0: 0012 0000 081c 0000 0000 0000 0000 1500  ................
-000002f0: 1512 1516 2c15 1615 1015 0615 061c 1808  ....,...........
-00000300: 0000 0000 0000 0000 1808 0000 0000 0000  ................
-00000310: 0000 1600 2808 0000 0000 0000 0000 1808  ....(...........
-00000320: 0000 0000 0000 0000 0000 0009 2002 0000  ............ ...
-00000330: 0016 0101 1600 26ec 0c1c 1504 1935 1000  ......&......5..
-00000340: 0619 1808 7261 5f65 7272 6f72 1502 1616  ....ra_error....
-00000350: 16b8 0116 c001 26dc 0b26 ac0b 1c18 0800  ......&..&......
-00000360: 0000 0000 0000 0018 0800 0000 0000 0000  ................
-00000370: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
-00000380: 0000 0000 0000 0000 192c 1504 1500 1502  .........,......
-00000390: 0015 0015 1015 0200 0000 1504 1510 1514  ................
-000003a0: 4c15 0215 0012 0000 081c 0000 0000 0000  L...............
-000003b0: 0000 1500 1512 1516 2c15 1615 1015 0615  ........,.......
-000003c0: 061c 1808 0000 0000 0000 0000 1808 0000  ................
-000003d0: 0000 0000 0000 1600 2808 0000 0000 0000  ........(.......
-000003e0: 0000 1808 0000 0000 0000 0000 0000 0009  ................
-000003f0: 2002 0000 0016 0101 1600 26f4 0f1c 1504   .........&.....
-00000400: 1935 1000 0619 1809 6465 635f 6572 726f  .5......dec_erro
-00000410: 7215 0216 1616 b801 16c0 0126 e40e 26b4  r..........&..&.
-00000420: 0e1c 1808 0000 0000 0000 0000 1808 0000  ................
-00000430: 0000 0000 0000 1600 2808 0000 0000 0000  ........(.......
-00000440: 0000 1808 0000 0000 0000 0000 0019 2c15  ..............,.
-00000450: 0415 0015 0200 1500 1510 1502 0000 0015  ................
-00000460: 0415 b001 1570 4c15 1615 0012 0000 5804  .....pL.......X.
-00000470: 0100 0901 0002 0907 0400 040d 0800 080d  ................
-00000480: 0800 0c0d 0800 0d0d 0800 0e0d 0800 120d  ................
-00000490: 0800 130d 083c 1600 0000 0000 0000 1700  .....<..........
-000004a0: 0000 0000 0000 1500 1520 1524 2c15 1615  ......... .$,...
-000004b0: 1015 0615 061c 1808 1700 0000 0000 0000  ................
-000004c0: 1808 0100 0000 0000 0000 1600 2808 1700  ............(...
-000004d0: 0000 0000 0000 1808 0100 0000 0000 0000  ................
-000004e0: 0000 0010 3c02 0000 0016 0104 0510 3254  ....<.........2T
-000004f0: 7698 0a00 0026 ea13 1c15 0419 3510 0006  v....&......5...
-00000500: 1918 115f 5f69 6e64 6578 5f6c 6576 656c  ...__index_level
-00000510: 5f30 5f5f 1502 1616 16e8 0216 ac02 26cc  _0__..........&.
-00000520: 1226 be11 1c18 0817 0000 0000 0000 0018  .&..............
-00000530: 0801 0000 0000 0000 0016 0028 0817 0000  ...........(....
-00000540: 0000 0000 0018 0801 0000 0000 0000 0000  ................
-00000550: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
-00000560: 0000 1504 197c 3500 1806 7363 6865 6d61  .....|5...schema
-00000570: 150c 0015 0425 0218 0269 6400 150a 2502  .....%...id...%.
-00000580: 1802 7261 0015 0a25 0218 0364 6563 0015  ..ra...%...dec..
-00000590: 0425 0218 0872 615f 6572 726f 7200 1504  .%...ra_error...
-000005a0: 2502 1809 6465 635f 6572 726f 7200 1504  %...dec_error...
-000005b0: 2502 1811 5f5f 696e 6465 785f 6c65 7665  %...__index_leve
-000005c0: 6c5f 305f 5f00 1616 191c 196c 26b8 021c  l_0__......l&...
-000005d0: 1504 1935 1000 0619 1802 6964 1502 1616  ...5......id....
-000005e0: 16e8 0216 b002 269a 0126 081c 1808 0603  ......&..&......
-000005f0: 0000 0000 0000 1808 f002 0000 0000 0000  ................
-00000600: 1600 2808 0603 0000 0000 0000 1808 f002  ..(.............
-00000610: 0000 0000 0000 0019 2c15 0415 0015 0200  ........,.......
-00000620: 1500 1510 1502 0000 0026 8e06 1c15 0a19  .........&......
-00000630: 3510 0006 1918 0272 6115 0216 1616 c802  5......ra.......
-00000640: 169c 0226 f004 26f2 031c 1808 0000 0000  ...&..&.........
-00000650: 0038 7340 1808 0000 0000 0098 7140 1600  .8s@........q@..
-00000660: 2808 0000 0000 0038 7340 1808 0000 0000  (......8s@......
-00000670: 0098 7140 0019 2c15 0415 0015 0200 1500  ..q@..,.........
-00000680: 1510 1502 0000 0026 ee09 1c15 0a19 3510  .......&......5.
-00000690: 0006 1918 0364 6563 1502 1616 16c8 0216  .....dec........
-000006a0: a402 26d0 0826 ca07 1c18 0800 0000 0000  ..&..&..........
-000006b0: 803d c018 0800 0000 0000 404b c016 0028  .=........@K...(
-000006c0: 0800 0000 0000 803d c018 0800 0000 0000  .......=........
-000006d0: 404b c000 192c 1504 1500 1502 0015 0015  @K...,..........
-000006e0: 1015 0200 0000 26ec 0c1c 1504 1935 1000  ......&......5..
-000006f0: 0619 1808 7261 5f65 7272 6f72 1502 1616  ....ra_error....
-00000700: 16b8 0116 c001 26dc 0b26 ac0b 1c18 0800  ......&..&......
-00000710: 0000 0000 0000 0018 0800 0000 0000 0000  ................
-00000720: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
-00000730: 0000 0000 0000 0000 192c 1504 1500 1502  .........,......
-00000740: 0015 0015 1015 0200 0000 26f4 0f1c 1504  ..........&.....
-00000750: 1935 1000 0619 1809 6465 635f 6572 726f  .5......dec_erro
-00000760: 7215 0216 1616 b801 16c0 0126 e40e 26b4  r..........&..&.
-00000770: 0e1c 1808 0000 0000 0000 0000 1808 0000  ................
-00000780: 0000 0000 0000 1600 2808 0000 0000 0000  ........(.......
-00000790: 0000 1808 0000 0000 0000 0000 0019 2c15  ..............,.
-000007a0: 0415 0015 0200 1500 1510 1502 0000 0026  ...............&
-000007b0: ea13 1c15 0419 3510 0006 1918 115f 5f69  ......5......__i
-000007c0: 6e64 6578 5f6c 6576 656c 5f30 5f5f 1502  ndex_level_0__..
-000007d0: 1616 16e8 0216 ac02 26cc 1226 be11 1c18  ........&..&....
-000007e0: 0817 0000 0000 0000 0018 0801 0000 0000  ................
-000007f0: 0000 0016 0028 0817 0000 0000 0000 0018  .....(..........
-00000800: 0801 0000 0000 0000 0000 192c 1504 1500  ...........,....
-00000810: 1502 0015 0015 1015 0200 0000 16d0 0d16  ................
-00000820: 1626 0816 9c0c 1400 0019 2c18 0670 616e  .&........,..pan
-00000830: 6461 7318 a507 7b22 696e 6465 785f 636f  das...{"index_co
-00000840: 6c75 6d6e 7322 3a20 5b22 5f5f 696e 6465  lumns": ["__inde
-00000850: 785f 6c65 7665 6c5f 305f 5f22 5d2c 2022  x_level_0__"], "
-00000860: 636f 6c75 6d6e 5f69 6e64 6578 6573 223a  column_indexes":
-00000870: 205b 7b22 6e61 6d65 223a 206e 756c 6c2c   [{"name": null,
-00000880: 2022 6669 656c 645f 6e61 6d65 223a 206e   "field_name": n
-00000890: 756c 6c2c 2022 7061 6e64 6173 5f74 7970  ull, "pandas_typ
-000008a0: 6522 3a20 2275 6e69 636f 6465 222c 2022  e": "unicode", "
-000008b0: 6e75 6d70 795f 7479 7065 223a 2022 6f62  numpy_type": "ob
-000008c0: 6a65 6374 222c 2022 6d65 7461 6461 7461  ject", "metadata
-000008d0: 223a 207b 2265 6e63 6f64 696e 6722 3a20  ": {"encoding": 
-000008e0: 2255 5446 2d38 227d 7d5d 2c20 2263 6f6c  "UTF-8"}}], "col
-000008f0: 756d 6e73 223a 205b 7b22 6e61 6d65 223a  umns": [{"name":
-00000900: 2022 6964 222c 2022 6669 656c 645f 6e61   "id", "field_na
-00000910: 6d65 223a 2022 6964 222c 2022 7061 6e64  me": "id", "pand
-00000920: 6173 5f74 7970 6522 3a20 2269 6e74 3634  as_type": "int64
-00000930: 222c 2022 6e75 6d70 795f 7479 7065 223a  ", "numpy_type":
-00000940: 2022 696e 7436 3422 2c20 226d 6574 6164   "int64", "metad
-00000950: 6174 6122 3a20 6e75 6c6c 7d2c 207b 226e  ata": null}, {"n
-00000960: 616d 6522 3a20 2272 6122 2c20 2266 6965  ame": "ra", "fie
-00000970: 6c64 5f6e 616d 6522 3a20 2272 6122 2c20  ld_name": "ra", 
-00000980: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
-00000990: 666c 6f61 7436 3422 2c20 226e 756d 7079  float64", "numpy
-000009a0: 5f74 7970 6522 3a20 2266 6c6f 6174 3634  _type": "float64
-000009b0: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
-000009c0: 756c 6c7d 2c20 7b22 6e61 6d65 223a 2022  ull}, {"name": "
-000009d0: 6465 6322 2c20 2266 6965 6c64 5f6e 616d  dec", "field_nam
-000009e0: 6522 3a20 2264 6563 222c 2022 7061 6e64  e": "dec", "pand
-000009f0: 6173 5f74 7970 6522 3a20 2266 6c6f 6174  as_type": "float
-00000a00: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
-00000a10: 223a 2022 666c 6f61 7436 3422 2c20 226d  ": "float64", "m
-00000a20: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
-00000a30: 207b 226e 616d 6522 3a20 2272 615f 6572   {"name": "ra_er
-00000a40: 726f 7222 2c20 2266 6965 6c64 5f6e 616d  ror", "field_nam
-00000a50: 6522 3a20 2272 615f 6572 726f 7222 2c20  e": "ra_error", 
-00000a60: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
-00000a70: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
-00000a80: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
-00000a90: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
-00000aa0: 2c20 7b22 6e61 6d65 223a 2022 6465 635f  , {"name": "dec_
-00000ab0: 6572 726f 7222 2c20 2266 6965 6c64 5f6e  error", "field_n
-00000ac0: 616d 6522 3a20 2264 6563 5f65 7272 6f72  ame": "dec_error
-00000ad0: 222c 2022 7061 6e64 6173 5f74 7970 6522  ", "pandas_type"
-00000ae0: 3a20 2269 6e74 3634 222c 2022 6e75 6d70  : "int64", "nump
-00000af0: 795f 7479 7065 223a 2022 696e 7436 3422  y_type": "int64"
-00000b00: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
-00000b10: 6c6c 7d2c 207b 226e 616d 6522 3a20 6e75  ll}, {"name": nu
-00000b20: 6c6c 2c20 2266 6965 6c64 5f6e 616d 6522  ll, "field_name"
-00000b30: 3a20 225f 5f69 6e64 6578 5f6c 6576 656c  : "__index_level
-00000b40: 5f30 5f5f 222c 2022 7061 6e64 6173 5f74  _0__", "pandas_t
-00000b50: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
-00000b60: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
-00000b70: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
-00000b80: 3a20 6e75 6c6c 7d5d 2c20 2263 7265 6174  : null}], "creat
-00000b90: 6f72 223a 207b 226c 6962 7261 7279 223a  or": {"library":
-00000ba0: 2022 7079 6172 726f 7722 2c20 2276 6572   "pyarrow", "ver
-00000bb0: 7369 6f6e 223a 2022 392e 302e 3022 7d2c  sion": "9.0.0"},
-00000bc0: 2022 7061 6e64 6173 5f76 6572 7369 6f6e   "pandas_version
-00000bd0: 223a 2022 312e 332e 3522 7d00 180c 4152  ": "1.3.5"}...AR
-00000be0: 524f 573a 7363 6865 6d61 18c0 0e2f 2f2f  ROW:schema...///
-00000bf0: 2f2f 3267 4641 4141 5141 4141 4141 4141  //2gFAAAQAAAAAAA
-00000c00: 4b41 4134 4142 6741 4641 4167 4143 6741  KAA4ABgAFAAgACgA
-00000c10: 4141 4141 4242 4141 5141 4141 4141 4141  AAAABBAAQAAAAAAA
-00000c20: 4b41 4177 4141 4141 4541 4167 4143 6741  KAAwAAAAEAAgACgA
-00000c30: 4141 4e77 4441 4141 4541 4141 4141 5141  AANwDAAAEAAAAAQA
-00000c40: 4141 4177 4141 4141 4941 4177 4142 4141  AAAwAAAAIAAwABAA
-00000c50: 4941 4167 4141 4141 4941 4141 4145 4141  IAAgAAAAIAAAAEAA
-00000c60: 4141 4159 4141 4142 7759 5735 6b59 584d  AAAYAAABwYW5kYXM
-00000c70: 4141 4b55 4441 4142 3749 6d6c 755a 4756  AAKUDAAB7ImluZGV
-00000c80: 3458 324e 7662 4856 7462 6e4d 694f 6942  4X2NvbHVtbnMiOiB
-00000c90: 6249 6c39 6661 5735 6b5a 5868 6662 4756  bIl9faW5kZXhfbGV
-00000ca0: 325a 5778 664d 4639 6649 6c30 7349 434a  2ZWxfMF9fIl0sICJ
-00000cb0: 6a62 3278 3162 5735 6661 5735 6b5a 5868  jb2x1bW5faW5kZXh
-00000cc0: 6c63 7949 3649 4674 3749 6d35 6862 5755  lcyI6IFt7Im5hbWU
-00000cd0: 694f 6942 7564 5778 734c 4341 695a 6d6c  iOiBudWxsLCAiZml
-00000ce0: 6c62 4752 6662 6d46 745a 5349 3649 4735  lbGRfbmFtZSI6IG5
-00000cf0: 3162 4777 7349 434a 7759 5735 6b59 584e  1bGwsICJwYW5kYXN
-00000d00: 6664 486c 775a 5349 3649 434a 3162 6d6c  fdHlwZSI6ICJ1bml
-00000d10: 6a62 3252 6c49 6977 6749 6d35 3162 5842  jb2RlIiwgIm51bXB
-00000d20: 3558 3352 3563 4755 694f 6941 6962 324a  5X3R5cGUiOiAib2J
-00000d30: 715a 574e 3049 6977 6749 6d31 6c64 4746  qZWN0IiwgIm1ldGF
-00000d40: 6b59 5852 6849 6a6f 6765 794a 6c62 6d4e  kYXRhIjogeyJlbmN
-00000d50: 765a 476c 755a 7949 3649 434a 5656 4559  vZGluZyI6ICJVVEY
-00000d60: 744f 434a 3966 5630 7349 434a 6a62 3278  tOCJ9fV0sICJjb2x
-00000d70: 3162 5735 7a49 6a6f 6757 3373 6962 6d46  1bW5zIjogW3sibmF
-00000d80: 745a 5349 3649 434a 705a 4349 7349 434a  tZSI6ICJpZCIsICJ
-00000d90: 6d61 5756 735a 4639 7559 5731 6c49 6a6f  maWVsZF9uYW1lIjo
-00000da0: 6749 6d6c 6b49 6977 6749 6e42 6862 6d52  gImlkIiwgInBhbmR
-00000db0: 6863 3139 3065 5842 6c49 6a6f 6749 6d6c  hc190eXBlIjogIml
-00000dc0: 7564 4459 3049 6977 6749 6d35 3162 5842  udDY0IiwgIm51bXB
-00000dd0: 3558 3352 3563 4755 694f 6941 6961 5735  5X3R5cGUiOiAiaW5
-00000de0: 304e 6a51 694c 4341 6962 5756 3059 5752  0NjQiLCAibWV0YWR
-00000df0: 6864 4745 694f 6942 7564 5778 7366 5377  hdGEiOiBudWxsfSw
-00000e00: 6765 794a 7559 5731 6c49 6a6f 6749 6e4a  geyJuYW1lIjogInJ
-00000e10: 6849 6977 6749 6d5a 705a 5778 6b58 3235  hIiwgImZpZWxkX25
-00000e20: 6862 5755 694f 6941 6963 6d45 694c 4341  hbWUiOiAicmEiLCA
-00000e30: 6963 4746 755a 4746 7a58 3352 3563 4755  icGFuZGFzX3R5cGU
-00000e40: 694f 6941 695a 6d78 7659 5851 324e 4349  iOiAiZmxvYXQ2NCI
-00000e50: 7349 434a 7564 5731 7765 5639 3065 5842  sICJudW1weV90eXB
-00000e60: 6c49 6a6f 6749 6d5a 7362 3246 304e 6a51  lIjogImZsb2F0NjQ
-00000e70: 694c 4341 6962 5756 3059 5752 6864 4745  iLCAibWV0YWRhdGE
-00000e80: 694f 6942 7564 5778 7366 5377 6765 794a  iOiBudWxsfSwgeyJ
-00000e90: 7559 5731 6c49 6a6f 6749 6d52 6c59 7949  uYW1lIjogImRlYyI
-00000ea0: 7349 434a 6d61 5756 735a 4639 7559 5731  sICJmaWVsZF9uYW1
-00000eb0: 6c49 6a6f 6749 6d52 6c59 7949 7349 434a  lIjogImRlYyIsICJ
-00000ec0: 7759 5735 6b59 584e 6664 486c 775a 5349  wYW5kYXNfdHlwZSI
-00000ed0: 3649 434a 6d62 4739 6864 4459 3049 6977  6ICJmbG9hdDY0Iiw
-00000ee0: 6749 6d35 3162 5842 3558 3352 3563 4755  gIm51bXB5X3R5cGU
-00000ef0: 694f 6941 695a 6d78 7659 5851 324e 4349  iOiAiZmxvYXQ2NCI
-00000f00: 7349 434a 745a 5852 685a 4746 3059 5349  sICJtZXRhZGF0YSI
-00000f10: 3649 4735 3162 4778 394c 4342 3749 6d35  6IG51bGx9LCB7Im5
-00000f20: 6862 5755 694f 6941 6963 6d46 665a 584a  hbWUiOiAicmFfZXJ
-00000f30: 7962 3349 694c 4341 695a 6d6c 6c62 4752  yb3IiLCAiZmllbGR
-00000f40: 6662 6d46 745a 5349 3649 434a 7959 5639  fbmFtZSI6ICJyYV9
-00000f50: 6c63 6e4a 7663 6949 7349 434a 7759 5735  lcnJvciIsICJwYW5
-00000f60: 6b59 584e 6664 486c 775a 5349 3649 434a  kYXNfdHlwZSI6ICJ
-00000f70: 7062 6e51 324e 4349 7349 434a 7564 5731  pbnQ2NCIsICJudW1
-00000f80: 7765 5639 3065 5842 6c49 6a6f 6749 6d6c  weV90eXBlIjogIml
-00000f90: 7564 4459 3049 6977 6749 6d31 6c64 4746  udDY0IiwgIm1ldGF
-00000fa0: 6b59 5852 6849 6a6f 6762 6e56 7362 4830  kYXRhIjogbnVsbH0
-00000fb0: 7349 4873 6962 6d46 745a 5349 3649 434a  sIHsibmFtZSI6ICJ
-00000fc0: 6b5a 574e 665a 584a 7962 3349 694c 4341  kZWNfZXJyb3IiLCA
-00000fd0: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
-00000fe0: 3649 434a 6b5a 574e 665a 584a 7962 3349  6ICJkZWNfZXJyb3I
-00000ff0: 694c 4341 6963 4746 755a 4746 7a58 3352  iLCAicGFuZGFzX3R
-00001000: 3563 4755 694f 6941 6961 5735 304e 6a51  5cGUiOiAiaW50NjQ
-00001010: 694c 4341 6962 6e56 7463 486c 6664 486c  iLCAibnVtcHlfdHl
-00001020: 775a 5349 3649 434a 7062 6e51 324e 4349  wZSI6ICJpbnQ2NCI
-00001030: 7349 434a 745a 5852 685a 4746 3059 5349  sICJtZXRhZGF0YSI
-00001040: 3649 4735 3162 4778 394c 4342 3749 6d35  6IG51bGx9LCB7Im5
-00001050: 6862 5755 694f 6942 7564 5778 734c 4341  hbWUiOiBudWxsLCA
-00001060: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
-00001070: 3649 434a 6658 326c 755a 4756 3458 3278  6ICJfX2luZGV4X2x
-00001080: 6c64 6d56 7358 7a42 6658 7949 7349 434a  ldmVsXzBfXyIsICJ
-00001090: 7759 5735 6b59 584e 6664 486c 775a 5349  wYW5kYXNfdHlwZSI
-000010a0: 3649 434a 7062 6e51 324e 4349 7349 434a  6ICJpbnQ2NCIsICJ
-000010b0: 7564 5731 7765 5639 3065 5842 6c49 6a6f  udW1weV90eXBlIjo
-000010c0: 6749 6d6c 7564 4459 3049 6977 6749 6d31  gImludDY0IiwgIm1
-000010d0: 6c64 4746 6b59 5852 6849 6a6f 6762 6e56  ldGFkYXRhIjogbnV
-000010e0: 7362 4831 644c 4341 6959 334a 6c59 5852  sbH1dLCAiY3JlYXR
-000010f0: 7663 6949 3649 4873 6962 476c 6963 6d46  vciI6IHsibGlicmF
-00001100: 7965 5349 3649 434a 7765 5746 7963 6d39  yeSI6ICJweWFycm9
-00001110: 3349 6977 6749 6e5a 6c63 6e4e 7062 3234  3IiwgInZlcnNpb24
-00001120: 694f 6941 694f 5334 774c 6a41 6966 5377  iOiAiOS4wLjAifSw
-00001130: 6749 6e42 6862 6d52 6863 3139 325a 584a  gInBhbmRhc192ZXJ
-00001140: 7a61 5739 7549 6a6f 6749 6a45 754d 7934  zaW9uIjogIjEuMy4
-00001150: 3149 6e30 4141 4141 4741 4141 414a 4145  1In0AAAAGAAAAJAE
-00001160: 4141 4f41 4141 4143 3041 4141 4166 4141  AAOAAAAC0AAAAfAA
-00001170: 4141 4551 4141 4141 4541 4141 4142 502f  AAEQAAAAEAAAABP/
-00001180: 2f2f 7741 4141 5149 5141 4141 414a 4141  //wAAAQIQAAAAJAA
-00001190: 4141 4151 4141 4141 4141 4141 4145 5141  AAAQAAAAAAAAAEQA
-000011a0: 4141 4639 6661 5735 6b5a 5868 6662 4756  AAF9faW5kZXhfbGV
-000011b0: 325a 5778 664d 4639 6641 4141 4142 502f  2ZWxfMF9fAAAABP/
-000011c0: 2f2f 7741 4141 4146 4141 4141 4151 502f  //wAAAAFAAAAAQP/
-000011d0: 2f2f 7741 4141 5149 5141 4141 4148 4141  //wAAAQIQAAAAHAA
-000011e0: 4141 4151 4141 4141 4141 4141 4143 5141  AAAQAAAAAAAAACQA
-000011f0: 4141 4752 6c59 3139 6c63 6e4a 7663 6741  AAGRlY19lcnJvcgA
-00001200: 4141 446a 2f2f 2f38 4141 4141 4251 4141  AADj///8AAAABQAA
-00001210: 4141 4854 2f2f 2f38 4141 4145 4345 4141  AAHT///8AAAECEAA
-00001220: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
-00001230: 4141 4167 4141 4142 7959 5639 6c63 6e4a  AAAgAAAByYV9lcnJ
-00001240: 7663 6741 4141 4142 732f 2f2f 2f41 4141  vcgAAAABs////AAA
-00001250: 4141 5541 4141 4143 6f2f 2f2f 2f41 4141  AAUAAAACo////AAA
-00001260: 4241 7841 4141 4141 5541 4141 4142 4141  BAxAAAAAUAAAABAA
-00001270: 4141 4141 4141 4141 4441 4141 415a 4756  AAAAAAAADAAAAZGV
-00001280: 6a41 4e62 2f2f 2f38 4141 4149 4130 502f  jANb///8AAAIA0P/
-00001290: 2f2f 7741 4141 514d 5141 4141 4148 4141  //wAAAQMQAAAAHAA
-000012a0: 4141 4151 4141 4141 4141 4141 4141 6741  AAAQAAAAAAAAAAgA
-000012b0: 4141 484a 6841 4141 4141 4159 4143 4141  AAHJhAAAAAAYACAA
-000012c0: 4741 4159 4141 4141 4141 4149 4145 4141  GAAYAAAAAAAIAEAA
-000012d0: 5541 4167 4142 6741 4841 4177 4141 4141  UAAgABgAHAAwAAAA
-000012e0: 5141 4241 4141 4141 4141 4145 4345 4141  QABAAAAAAAAECEAA
-000012f0: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
-00001300: 4141 4149 4141 4142 705a 4141 4143 4141  AAAIAAABpZAAACAA
-00001310: 4d41 4167 4142 7741 4941 4141 4141 4141  MAAgABwAIAAAAAAA
-00001320: 4141 5541 4141 4141 4141 4141 4100 181f  AAUAAAAAAAAAA...
-00001330: 7061 7271 7565 742d 6370 702d 6172 726f  parquet-cpp-arro
-00001340: 7720 7665 7273 696f 6e20 392e 302e 3019  w version 9.0.0.
-00001350: 6c1c 0000 1c00 001c 0000 1c00 001c 0000  l...............
-00001360: 1c00 0000 020e 0000 5041 5231            ........PAR1
+00000000: 5041 5231 1504 1590 0315 e201 4c15 3215  PAR1........L.2.
+00000010: 0012 0000 c801 08bc 0200 0501 00bd 0d08  ................
+00000020: 00be 0d08 00bf 0d08 00c0 0d08 00c1 0d08  ................
+00000030: 00c2 0d08 00c3 0d08 00c4 0d08 00c5 0d08  ................
+00000040: 00c6 0d08 00c7 0d08 00c8 0d08 00c9 0d08  ................
+00000050: 00ca 0d08 00cb 0d08 00cc 0d08 00cd 0d08  ................
+00000060: 00ce 0d08 00cf 0d08 00d0 0d08 00d1 0d08  ................
+00000070: 00d2 0d08 3cd3 0200 0000 0000 00d4 0200  ....<...........
+00000080: 0000 0000 0015 0015 3815 3c2c 1532 1510  ........8.<,.2..
+00000090: 1506 1506 1c18 08d4 0200 0000 0000 0018  ................
+000000a0: 08bc 0200 0000 0000 0016 0028 08d4 0200  ...........(....
+000000b0: 0000 0000 0018 08bc 0200 0000 0000 0000  ................
+000000c0: 0000 1c6c 0200 0000 3201 0509 2088 418a  ...l....2... .A.
+000000d0: 3928 a9c5 9a7b 30ca 49ab bd18 0000 0000  9(...{0.I.......
+000000e0: 26c0 031c 1504 1935 1000 0619 1802 6964  &......5......id
+000000f0: 1502 1632 16e2 0416 b803 268a 0226 081c  ...2......&..&..
+00000100: 1808 d402 0000 0000 0000 1808 bc02 0000  ................
+00000110: 0000 0000 1600 2808 d402 0000 0000 0000  ......(.........
+00000120: 1808 bc02 0000 0000 0000 0019 2c15 0415  ............,...
+00000130: 0015 0200 1500 1510 1502 0000 0015 0415  ................
+00000140: e002 15ce 014c 152c 1500 1200 00b0 0100  .....L.,........
+00000150: 0001 0108 a871 4001 0708 00b8 7209 0804  .....q@.....r...
+00000160: 6873 0908 00e8 0d18 0468 7409 1000 f80d  hs.......ht.....
+00000170: 0800 980d 2800 480d 2800 380d 0800 680d  ....(.H.(.8...h.
+00000180: 1804 5875 0930 0018 0d18 0008 0d18 00a8  ..Xu.0..........
+00000190: 0d08 00f8 0d08 0088 0d60 0048 1110 0d38  .........`.H...8
+000001a0: 00a8 0d38 00e8 0d10 28b8 7340 0000 0000  ...8....(.s@....
+000001b0: 0038 7440 1500 1538 153c 2c15 3215 1015  .8t@...8.<,.2...
+000001c0: 0615 061c 1808 0000 0000 00e8 7540 1808  ............u@..
+000001d0: 0000 0000 0088 7140 1600 2808 0000 0000  ......q@..(.....
+000001e0: 00e8 7540 1808 0000 0000 0088 7140 0000  ..u@........q@..
+000001f0: 001c 6c02 0000 0032 0105 0920 8841 8a39  ..l....2... .A.9
+00000200: 28a9 c59a 7bcb c118 e5a4 1500 0000 0026  (...{..........&
+00000210: 9e08 1c15 0a19 3510 0006 1918 0272 6115  ......5......ra.
+00000220: 0216 3216 b204 16a4 0326 e806 26fa 041c  ..2......&..&...
+00000230: 1808 0000 0000 00e8 7540 1808 0000 0000  ........u@......
+00000240: 0088 7140 1600 2808 0000 0000 00e8 7540  ..q@..(.......u@
+00000250: 1808 0000 0000 0088 7140 0019 2c15 0415  ........q@..,...
+00000260: 0015 0200 1500 1510 1502 0000 0015 0415  ................
+00000270: 9002 15b0 014c 1522 1500 1200 0088 0100  .....L."........
+00000280: 0001 0108 404d c001 0708 0040 4809 0804  ....@M.....@H...
+00000290: 803b 0908 0460 5109 0804 c046 0908 0440  .;...`Q....F...@
+000002a0: 400d 0800 4209 0800 c011 0800 430d 1000  @...B.......C...
+000002b0: 480d 0800 440d 0800 4109 0804 404e 0908  H...D...A...@N..
+000002c0: 04c0 450d 0800 4709 0828 4041 c000 0000  ..E...G..(@A....
+000002d0: 0000 2051 c015 0015 3815 3c2c 1532 1510  .. Q....8.<,.2..
+000002e0: 1506 1506 1c18 0800 0000 0000 803b c018  .............;..
+000002f0: 0800 0000 0000 6051 c016 0028 0800 0000  ......`Q...(....
+00000300: 0000 803b c018 0800 0000 0000 6051 c000  ...;........`Q..
+00000310: 0000 1c6c 0200 0000 3201 0509 2088 418a  ...l....2... .A.
+00000320: 1987 a094 d459 ac31 e41e 800a 0000 0000  .....Y.1........
+00000330: 26e0 0c1c 150a 1935 1000 0619 1803 6465  &......5......de
+00000340: 6315 0216 3216 e203 1686 0326 aa0b 26da  c...2......&..&.
+00000350: 091c 1808 0000 0000 0080 3bc0 1808 0000  ..........;.....
+00000360: 0000 0060 51c0 1600 2808 0000 0000 0080  ...`Q...(.......
+00000370: 3bc0 1808 0000 0000 0060 51c0 0019 2c15  ;........`Q...,.
+00000380: 0415 0015 0200 1500 1510 1502 0000 0015  ................
+00000390: 0415 1015 144c 1502 1500 1200 0008 1c00  .....L..........
+000003a0: 0000 0000 0000 0015 0015 1215 162c 1532  .............,.2
+000003b0: 1510 1506 1506 1c18 0800 0000 0000 0000  ................
+000003c0: 0018 0800 0000 0000 0000 0016 0028 0800  .............(..
+000003d0: 0000 0000 0000 0018 0800 0000 0000 0000  ................
+000003e0: 0000 0000 0920 0200 0000 3201 0132 0026  ..... ....2..2.&
+000003f0: de0f 1c15 0419 3510 0006 1918 0872 615f  ......5......ra_
+00000400: 6572 726f 7215 0216 3216 b801 16c0 0126  error...2......&
+00000410: ce0e 269e 0e1c 1808 0000 0000 0000 0000  ..&.............
+00000420: 1808 0000 0000 0000 0000 1600 2808 0000  ............(...
+00000430: 0000 0000 0000 1808 0000 0000 0000 0000  ................
+00000440: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
+00000450: 0000 0015 0415 1015 144c 1502 1500 1200  .........L......
+00000460: 0008 1c00 0000 0000 0000 0015 0015 1215  ................
+00000470: 162c 1532 1510 1506 1506 1c18 0800 0000  .,.2............
+00000480: 0000 0000 0018 0800 0000 0000 0000 0016  ................
+00000490: 0028 0800 0000 0000 0000 0018 0800 0000  .(..............
+000004a0: 0000 0000 0000 0000 0920 0200 0000 3201  ......... ....2.
+000004b0: 0132 0026 e612 1c15 0419 3510 0006 1918  .2.&......5.....
+000004c0: 0964 6563 5f65 7272 6f72 1502 1632 16b8  .dec_error...2..
+000004d0: 0116 c001 26d6 1126 a611 1c18 0800 0000  ....&..&........
+000004e0: 0000 0000 0018 0800 0000 0000 0000 0016  ................
+000004f0: 0028 0800 0000 0000 0000 0018 0800 0000  .(..............
+00000500: 0000 0000 0000 192c 1504 1500 1502 0015  .......,........
+00000510: 0015 1015 0200 0000 1504 196c 3500 1806  ...........l5...
+00000520: 7363 6865 6d61 150a 0015 0425 0218 0269  schema.....%...i
+00000530: 6400 150a 2502 1802 7261 0015 0a25 0218  d...%...ra...%..
+00000540: 0364 6563 0015 0425 0218 0872 615f 6572  .dec...%...ra_er
+00000550: 726f 7200 1504 2502 1809 6465 635f 6572  ror...%...dec_er
+00000560: 726f 7200 1632 191c 195c 26c0 031c 1504  ror..2...\&.....
+00000570: 1935 1000 0619 1802 6964 1502 1632 16e2  .5......id...2..
+00000580: 0416 b803 268a 0226 081c 1808 d402 0000  ....&..&........
+00000590: 0000 0000 1808 bc02 0000 0000 0000 1600  ................
+000005a0: 2808 d402 0000 0000 0000 1808 bc02 0000  (...............
+000005b0: 0000 0000 0019 2c15 0415 0015 0200 1500  ......,.........
+000005c0: 1510 1502 0000 0026 9e08 1c15 0a19 3510  .......&......5.
+000005d0: 0006 1918 0272 6115 0216 3216 b204 16a4  .....ra...2.....
+000005e0: 0326 e806 26fa 041c 1808 0000 0000 00e8  .&..&...........
+000005f0: 7540 1808 0000 0000 0088 7140 1600 2808  u@........q@..(.
+00000600: 0000 0000 00e8 7540 1808 0000 0000 0088  ......u@........
+00000610: 7140 0019 2c15 0415 0015 0200 1500 1510  q@..,...........
+00000620: 1502 0000 0026 e00c 1c15 0a19 3510 0006  .....&......5...
+00000630: 1918 0364 6563 1502 1632 16e2 0316 8603  ...dec...2......
+00000640: 26aa 0b26 da09 1c18 0800 0000 0000 803b  &..&...........;
+00000650: c018 0800 0000 0000 6051 c016 0028 0800  ........`Q...(..
+00000660: 0000 0000 803b c018 0800 0000 0000 6051  .....;........`Q
+00000670: c000 192c 1504 1500 1502 0015 0015 1015  ...,............
+00000680: 0200 0000 26de 0f1c 1504 1935 1000 0619  ....&......5....
+00000690: 1808 7261 5f65 7272 6f72 1502 1632 16b8  ..ra_error...2..
+000006a0: 0116 c001 26ce 0e26 9e0e 1c18 0800 0000  ....&..&........
+000006b0: 0000 0000 0018 0800 0000 0000 0000 0016  ................
+000006c0: 0028 0800 0000 0000 0000 0018 0800 0000  .(..............
+000006d0: 0000 0000 0000 192c 1504 1500 1502 0015  .......,........
+000006e0: 0015 1015 0200 0000 26e6 121c 1504 1935  ........&......5
+000006f0: 1000 0619 1809 6465 635f 6572 726f 7215  ......dec_error.
+00000700: 0216 3216 b801 16c0 0126 d611 26a6 111c  ..2......&..&...
+00000710: 1808 0000 0000 0000 0000 1808 0000 0000  ................
+00000720: 0000 0000 1600 2808 0000 0000 0000 0000  ......(.........
+00000730: 1808 0000 0000 0000 0000 0019 2c15 0415  ............,...
+00000740: 0015 0200 1500 1510 1502 0000 0016 e60f  ................
+00000750: 1632 2608 16e2 0c14 0000 192c 1806 7061  .2&........,..pa
+00000760: 6e64 6173 18a7 057b 2269 6e64 6578 5f63  ndas...{"index_c
+00000770: 6f6c 756d 6e73 223a 205b 5d2c 2022 636f  olumns": [], "co
+00000780: 6c75 6d6e 5f69 6e64 6578 6573 223a 205b  lumn_indexes": [
+00000790: 5d2c 2022 636f 6c75 6d6e 7322 3a20 5b7b  ], "columns": [{
+000007a0: 226e 616d 6522 3a20 2269 6422 2c20 2266  "name": "id", "f
+000007b0: 6965 6c64 5f6e 616d 6522 3a20 2269 6422  ield_name": "id"
+000007c0: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
+000007d0: 2022 696e 7436 3422 2c20 226e 756d 7079   "int64", "numpy
+000007e0: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
+000007f0: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
+00000800: 6c7d 2c20 7b22 6e61 6d65 223a 2022 7261  l}, {"name": "ra
+00000810: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
+00000820: 2022 7261 222c 2022 7061 6e64 6173 5f74   "ra", "pandas_t
+00000830: 7970 6522 3a20 2266 6c6f 6174 3634 222c  ype": "float64",
+00000840: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
+00000850: 666c 6f61 7436 3422 2c20 226d 6574 6164  float64", "metad
+00000860: 6174 6122 3a20 6e75 6c6c 7d2c 207b 226e  ata": null}, {"n
+00000870: 616d 6522 3a20 2264 6563 222c 2022 6669  ame": "dec", "fi
+00000880: 656c 645f 6e61 6d65 223a 2022 6465 6322  eld_name": "dec"
+00000890: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
+000008a0: 2022 666c 6f61 7436 3422 2c20 226e 756d   "float64", "num
+000008b0: 7079 5f74 7970 6522 3a20 2266 6c6f 6174  py_type": "float
+000008c0: 3634 222c 2022 6d65 7461 6461 7461 223a  64", "metadata":
+000008d0: 206e 756c 6c7d 2c20 7b22 6e61 6d65 223a   null}, {"name":
+000008e0: 2022 7261 5f65 7272 6f72 222c 2022 6669   "ra_error", "fi
+000008f0: 656c 645f 6e61 6d65 223a 2022 7261 5f65  eld_name": "ra_e
+00000900: 7272 6f72 222c 2022 7061 6e64 6173 5f74  rror", "pandas_t
+00000910: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
+00000920: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
+00000930: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
+00000940: 3a20 6e75 6c6c 7d2c 207b 226e 616d 6522  : null}, {"name"
+00000950: 3a20 2264 6563 5f65 7272 6f72 222c 2022  : "dec_error", "
+00000960: 6669 656c 645f 6e61 6d65 223a 2022 6465  field_name": "de
+00000970: 635f 6572 726f 7222 2c20 2270 616e 6461  c_error", "panda
+00000980: 735f 7479 7065 223a 2022 696e 7436 3422  s_type": "int64"
+00000990: 2c20 226e 756d 7079 5f74 7970 6522 3a20  , "numpy_type": 
+000009a0: 2269 6e74 3634 222c 2022 6d65 7461 6461  "int64", "metada
+000009b0: 7461 223a 206e 756c 6c7d 5d2c 2022 6372  ta": null}], "cr
+000009c0: 6561 746f 7222 3a20 7b22 6c69 6272 6172  eator": {"librar
+000009d0: 7922 3a20 2270 7961 7272 6f77 222c 2022  y": "pyarrow", "
+000009e0: 7665 7273 696f 6e22 3a20 2239 2e30 2e30  version": "9.0.0
+000009f0: 227d 2c20 2270 616e 6461 735f 7665 7273  "}, "pandas_vers
+00000a00: 696f 6e22 3a20 2232 2e30 2e30 227d 0018  ion": "2.0.0"}..
+00000a10: 0c41 5252 4f57 3a73 6368 656d 6118 980b  .ARROW:schema...
+00000a20: 2f2f 2f2f 2f79 6745 4141 4151 4141 4141  /////ygEAAAQAAAA
+00000a30: 4141 414b 4141 3441 4267 4146 4141 6741  AAAKAA4ABgAFAAgA
+00000a40: 4367 4141 4141 4142 4241 4151 4141 4141  CgAAAAABBAAQAAAA
+00000a50: 4141 414b 4141 7741 4141 4145 4141 6741  AAAKAAwAAAAEAAgA
+00000a60: 4367 4141 414e 7743 4141 4145 4141 4141  CgAAANwCAAAEAAAA
+00000a70: 4151 4141 4141 7741 4141 4149 4141 7741  AQAAAAwAAAAIAAwA
+00000a80: 4241 4149 4141 6741 4141 4149 4141 4141  BAAIAAgAAAAIAAAA
+00000a90: 4541 4141 4141 5941 4141 4277 5957 356b  EAAAAAYAAABwYW5k
+00000aa0: 5958 4d41 414b 6343 4141 4237 496d 6c75  YXMAAKcCAAB7Imlu
+00000ab0: 5a47 5634 5832 4e76 6248 5674 626e 4d69  ZGV4X2NvbHVtbnMi
+00000ac0: 4f69 4262 5853 7767 496d 4e76 6248 5674  OiBbXSwgImNvbHVt
+00000ad0: 626c 3970 626d 526c 6547 567a 496a 6f67  bl9pbmRleGVzIjog
+00000ae0: 5731 3073 4943 4a6a 6232 7831 6257 357a  W10sICJjb2x1bW5z
+00000af0: 496a 6f67 5733 7369 626d 4674 5a53 4936  IjogW3sibmFtZSI6
+00000b00: 4943 4a70 5a43 4973 4943 4a6d 6157 5673  ICJpZCIsICJmaWVs
+00000b10: 5a46 3975 5957 316c 496a 6f67 496d 6c6b  ZF9uYW1lIjogImlk
+00000b20: 4969 7767 496e 4268 626d 5268 6331 3930  IiwgInBhbmRhc190
+00000b30: 6558 426c 496a 6f67 496d 6c75 6444 5930  eXBlIjogImludDY0
+00000b40: 4969 7767 496d 3531 6258 4235 5833 5235  IiwgIm51bXB5X3R5
+00000b50: 6347 5569 4f69 4169 6157 3530 4e6a 5169  cGUiOiAiaW50NjQi
+00000b60: 4c43 4169 6257 5630 5957 5268 6447 4569  LCAibWV0YWRhdGEi
+00000b70: 4f69 4275 6457 7873 6653 7767 6579 4a75  OiBudWxsfSwgeyJu
+00000b80: 5957 316c 496a 6f67 496e 4a68 4969 7767  YW1lIjogInJhIiwg
+00000b90: 496d 5a70 5a57 786b 5832 3568 6257 5569  ImZpZWxkX25hbWUi
+00000ba0: 4f69 4169 636d 4569 4c43 4169 6347 4675  OiAicmEiLCAicGFu
+00000bb0: 5a47 467a 5833 5235 6347 5569 4f69 4169  ZGFzX3R5cGUiOiAi
+00000bc0: 5a6d 7876 5958 5132 4e43 4973 4943 4a75  ZmxvYXQ2NCIsICJu
+00000bd0: 6457 3177 6556 3930 6558 426c 496a 6f67  dW1weV90eXBlIjog
+00000be0: 496d 5a73 6232 4630 4e6a 5169 4c43 4169  ImZsb2F0NjQiLCAi
+00000bf0: 6257 5630 5957 5268 6447 4569 4f69 4275  bWV0YWRhdGEiOiBu
+00000c00: 6457 7873 6653 7767 6579 4a75 5957 316c  dWxsfSwgeyJuYW1l
+00000c10: 496a 6f67 496d 526c 5979 4973 4943 4a6d  IjogImRlYyIsICJm
+00000c20: 6157 5673 5a46 3975 5957 316c 496a 6f67  aWVsZF9uYW1lIjog
+00000c30: 496d 526c 5979 4973 4943 4a77 5957 356b  ImRlYyIsICJwYW5k
+00000c40: 5958 4e66 6448 6c77 5a53 4936 4943 4a6d  YXNfdHlwZSI6ICJm
+00000c50: 6247 3968 6444 5930 4969 7767 496d 3531  bG9hdDY0IiwgIm51
+00000c60: 6258 4235 5833 5235 6347 5569 4f69 4169  bXB5X3R5cGUiOiAi
+00000c70: 5a6d 7876 5958 5132 4e43 4973 4943 4a74  ZmxvYXQ2NCIsICJt
+00000c80: 5a58 5268 5a47 4630 5953 4936 4947 3531  ZXRhZGF0YSI6IG51
+00000c90: 6247 7839 4c43 4237 496d 3568 6257 5569  bGx9LCB7Im5hbWUi
+00000ca0: 4f69 4169 636d 4666 5a58 4a79 6233 4969  OiAicmFfZXJyb3Ii
+00000cb0: 4c43 4169 5a6d 6c6c 6247 5266 626d 4674  LCAiZmllbGRfbmFt
+00000cc0: 5a53 4936 4943 4a79 5956 396c 636e 4a76  ZSI6ICJyYV9lcnJv
+00000cd0: 6369 4973 4943 4a77 5957 356b 5958 4e66  ciIsICJwYW5kYXNf
+00000ce0: 6448 6c77 5a53 4936 4943 4a70 626e 5132  dHlwZSI6ICJpbnQ2
+00000cf0: 4e43 4973 4943 4a75 6457 3177 6556 3930  NCIsICJudW1weV90
+00000d00: 6558 426c 496a 6f67 496d 6c75 6444 5930  eXBlIjogImludDY0
+00000d10: 4969 7767 496d 316c 6447 466b 5958 5268  IiwgIm1ldGFkYXRh
+00000d20: 496a 6f67 626e 5673 6248 3073 4948 7369  IjogbnVsbH0sIHsi
+00000d30: 626d 4674 5a53 4936 4943 4a6b 5a57 4e66  bmFtZSI6ICJkZWNf
+00000d40: 5a58 4a79 6233 4969 4c43 4169 5a6d 6c6c  ZXJyb3IiLCAiZmll
+00000d50: 6247 5266 626d 4674 5a53 4936 4943 4a6b  bGRfbmFtZSI6ICJk
+00000d60: 5a57 4e66 5a58 4a79 6233 4969 4c43 4169  ZWNfZXJyb3IiLCAi
+00000d70: 6347 4675 5a47 467a 5833 5235 6347 5569  cGFuZGFzX3R5cGUi
+00000d80: 4f69 4169 6157 3530 4e6a 5169 4c43 4169  OiAiaW50NjQiLCAi
+00000d90: 626e 5674 6348 6c66 6448 6c77 5a53 4936  bnVtcHlfdHlwZSI6
+00000da0: 4943 4a70 626e 5132 4e43 4973 4943 4a74  ICJpbnQ2NCIsICJt
+00000db0: 5a58 5268 5a47 4630 5953 4936 4947 3531  ZXRhZGF0YSI6IG51
+00000dc0: 6247 7839 5853 7767 496d 4e79 5a57 4630  bGx9XSwgImNyZWF0
+00000dd0: 6233 4969 4f69 4237 496d 7870 596e 4a68  b3IiOiB7ImxpYnJh
+00000de0: 636e 6b69 4f69 4169 6348 6c68 636e 4a76  cnkiOiAicHlhcnJv
+00000df0: 6479 4973 4943 4a32 5a58 4a7a 6157 3975  dyIsICJ2ZXJzaW9u
+00000e00: 496a 6f67 496a 6b75 4d43 3477 496e 3073  IjogIjkuMC4wIn0s
+00000e10: 4943 4a77 5957 356b 5958 4e66 646d 5679  ICJwYW5kYXNfdmVy
+00000e20: 6332 6c76 6269 4936 4943 4979 4c6a 4175  c2lvbiI6ICIyLjAu
+00000e30: 4d43 4a39 4141 5541 4141 446b 4141 4141  MCJ9AAUAAADkAAAA
+00000e40: 6f41 4141 4148 5141 4141 4138 4141 4141  oAAAAHQAAAA8AAAA
+00000e50: 4241 4141 4145 442f 2f2f 3841 4141 4543  BAAAAED///8AAAEC
+00000e60: 4541 4141 4142 7741 4141 4145 4141 4141  EAAAABwAAAAEAAAA
+00000e70: 4141 4141 4141 6b41 4141 426b 5a57 4e66  AAAAAAkAAABkZWNf
+00000e80: 5a58 4a79 6233 4941 4141 4134 2f2f 2f2f  ZXJyb3IAAAA4////
+00000e90: 4141 4141 4155 4141 4141 4230 2f2f 2f2f  AAAAAUAAAAB0////
+00000ea0: 4141 4142 4168 4141 4141 4163 4141 4141  AAABAhAAAAAcAAAA
+00000eb0: 4241 4141 4141 4141 4141 4149 4141 4141  BAAAAAAAAAAIAAAA
+00000ec0: 636d 4666 5a58 4a79 6233 4941 4141 4141  cmFfZXJyb3IAAAAA
+00000ed0: 6250 2f2f 2f77 4141 4141 4641 4141 4141  bP///wAAAAFAAAAA
+00000ee0: 7150 2f2f 2f77 4141 4151 4d51 4141 4141  qP///wAAAQMQAAAA
+00000ef0: 4641 4141 4141 5141 4141 4141 4141 4141  FAAAAAQAAAAAAAAA
+00000f00: 4177 4141 4147 526c 5977 4457 2f2f 2f2f  AwAAAGRlYwDW////
+00000f10: 4141 4143 414e 442f 2f2f 3841 4141 4544  AAACAND///8AAAED
+00000f20: 4541 4141 4142 7741 4141 4145 4141 4141  EAAAABwAAAAEAAAA
+00000f30: 4141 4141 4141 4941 4141 4279 5951 4141  AAAAAAIAAAByYQAA
+00000f40: 4141 4147 4141 6741 4267 4147 4141 4141  AAAGAAgABgAGAAAA
+00000f50: 4141 4143 4142 4141 4641 4149 4141 5941  AAACABAAFAAIAAYA
+00000f60: 4277 414d 4141 4141 4541 4151 4141 4141  BwAMAAAAEAAQAAAA
+00000f70: 4141 4142 4168 4141 4141 4163 4141 4141  AAABAhAAAAAcAAAA
+00000f80: 4241 4141 4141 4141 4141 4143 4141 4141  BAAAAAAAAAACAAAA
+00000f90: 6157 5141 4141 6741 4441 4149 4141 6341  aWQAAAgADAAIAAcA
+00000fa0: 4341 4141 4141 4141 4141 4641 4141 4141  CAAAAAAAAAFAAAAA
+00000fb0: 4141 4141 4141 3d3d 0018 1f70 6172 7175  AAAAAA==...parqu
+00000fc0: 6574 2d63 7070 2d61 7272 6f77 2076 6572  et-cpp-arrow ver
+00000fd0: 7369 6f6e 2039 2e30 2e30 195c 1c00 001c  sion 9.0.0.\....
+00000fe0: 0000 1c00 001c 0000 1c00 0000 d40a 0000  ................
+00000ff0: 5041 5231                                PAR1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_46/shard_3.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_object_catalog/_metadata`

 * *Files 19% similar despite different names*

```diff
@@ -1,305 +1,321 @@
-00000000: 5041 5231 1504 1560 1548 4c15 0c15 0012  PAR1...`.HL.....
-00000010: 0000 3008 d502 0005 0100 d70d 0800 e40d  ..0.............
-00000020: 0800 e50d 083c ea02 0000 0000 0000 ed02  .....<..........
-00000030: 0000 0000 0000 1500 1516 151a 2c15 0c15  ............,...
-00000040: 1015 0615 061c 1808 ed02 0000 0000 0000  ................
-00000050: 1808 d502 0000 0000 0000 1600 2808 ed02  ............(...
-00000060: 0000 0000 0000 1808 d502 0000 0000 0000  ................
-00000070: 0000 000b 2802 0000 000c 0103 0388 c602  ....(...........
-00000080: 2680 021c 1504 1935 1000 0619 1802 6964  &......5......id
-00000090: 1502 160c 168c 0216 f801 266c 2608 1c18  ..........&l&...
-000000a0: 08ed 0200 0000 0000 0018 08d5 0200 0000  ................
-000000b0: 0000 0016 0028 08ed 0200 0000 0000 0018  .....(..........
-000000c0: 08d5 0200 0000 0000 0000 192c 1504 1500  ...........,....
-000000d0: 1502 0015 0015 1015 0200 0000 1504 1560  ...............`
-000000e0: 154a 4c15 0c15 0012 0000 3000 0001 0108  .JL.......0.....
-000000f0: 4873 4001 0708 00d8 7209 0800 280d 1000  Hs@.....r...(...
-00000100: f80d 1028 b871 4000 0000 0000 5872 4015  ...(.q@.....Xr@.
-00000110: 0015 1615 1a2c 150c 1510 1506 1506 1c18  .....,..........
-00000120: 0800 0000 0000 4873 4018 0800 0000 0000  ......Hs@.......
-00000130: b871 4016 0028 0800 0000 0000 4873 4018  .q@..(......Hs@.
-00000140: 0800 0000 0000 b871 4000 0000 0b28 0200  .......q@....(..
-00000150: 0000 0c01 0303 88c6 0226 b205 1c15 0a19  .........&......
-00000160: 3510 0006 1918 0272 6115 0216 0c16 8c02  5......ra.......
-00000170: 16fa 0126 9e04 26b8 031c 1808 0000 0000  ...&..&.........
-00000180: 0048 7340 1808 0000 0000 00b8 7140 1600  .Hs@........q@..
-00000190: 2808 0000 0000 0048 7340 1808 0000 0000  (......Hs@......
-000001a0: 00b8 7140 0019 2c15 0415 0015 0200 1500  ..q@..,.........
-000001b0: 1510 1502 0000 0015 0415 6015 4e4c 150c  ..........`.NL..
-000001c0: 1500 1200 0030 0000 0101 0cc0 44c0 0001  .....0......D...
-000001d0: 0104 4046 0908 04c0 4009 0804 4043 0908  ..@F....@...@C..
-000001e0: 2880 3fc0 0000 0000 00c0 4bc0 1500 1516  (.?.......K.....
-000001f0: 151a 2c15 0c15 1015 0615 061c 1808 0000  ..,.............
-00000200: 0000 0080 3fc0 1808 0000 0000 00c0 4bc0  ....?.........K.
-00000210: 1600 2808 0000 0000 0080 3fc0 1808 0000  ..(.......?.....
-00000220: 0000 00c0 4bc0 0000 000b 2802 0000 000c  ....K.....(.....
-00000230: 0103 0388 c602 26ec 081c 150a 1935 1000  ......&......5..
-00000240: 0619 1803 6465 6315 0216 0c16 8c02 16fe  ....dec.........
-00000250: 0126 d807 26ee 061c 1808 0000 0000 0080  .&..&...........
-00000260: 3fc0 1808 0000 0000 00c0 4bc0 1600 2808  ?.........K...(.
-00000270: 0000 0000 0080 3fc0 1808 0000 0000 00c0  ......?.........
-00000280: 4bc0 0019 2c15 0415 0015 0200 1500 1510  K...,...........
-00000290: 1502 0000 0015 0415 1015 144c 1502 1500  ...........L....
-000002a0: 1200 0008 1c00 0000 0000 0000 0015 0015  ................
-000002b0: 1215 162c 150c 1510 1506 1506 1c18 0800  ...,............
-000002c0: 0000 0000 0000 0018 0800 0000 0000 0000  ................
-000002d0: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
-000002e0: 0000 0000 0000 0000 0000 0920 0200 0000  ........... ....
-000002f0: 0c01 010c 0026 ea0b 1c15 0419 3510 0006  .....&......5...
-00000300: 1918 0872 615f 6572 726f 7215 0216 0c16  ...ra_error.....
-00000310: b801 16c0 0126 da0a 26aa 0a1c 1808 0000  .....&..&.......
-00000320: 0000 0000 0000 1808 0000 0000 0000 0000  ................
-00000330: 1600 2808 0000 0000 0000 0000 1808 0000  ..(.............
-00000340: 0000 0000 0000 0019 2c15 0415 0015 0200  ........,.......
-00000350: 1500 1510 1502 0000 0015 0415 1015 144c  ...............L
-00000360: 1502 1500 1200 0008 1c00 0000 0000 0000  ................
-00000370: 0015 0015 1215 162c 150c 1510 1506 1506  .......,........
-00000380: 1c18 0800 0000 0000 0000 0018 0800 0000  ................
-00000390: 0000 0000 0016 0028 0800 0000 0000 0000  .......(........
-000003a0: 0018 0800 0000 0000 0000 0000 0000 0920  ............... 
-000003b0: 0200 0000 0c01 010c 0026 f20e 1c15 0419  .........&......
-000003c0: 3510 0006 1918 0964 6563 5f65 7272 6f72  5......dec_error
-000003d0: 1502 160c 16b8 0116 c001 26e2 0d26 b20d  ..........&..&..
-000003e0: 1c18 0800 0000 0000 0000 0018 0800 0000  ................
-000003f0: 0000 0000 0016 0028 0800 0000 0000 0000  .......(........
-00000400: 0018 0800 0000 0000 0000 0000 192c 1504  .............,..
-00000410: 1500 1502 0015 0015 1015 0200 0000 1504  ................
-00000420: 1560 1544 4c15 0c15 0012 0000 3000 000d  .`.DL.......0...
-00000430: 0100 020d 0800 0f0d 0800 100d 083c 1500  .............<..
-00000440: 0000 0000 0000 1800 0000 0000 0000 1500  ................
-00000450: 1516 151a 2c15 0c15 1015 0615 061c 1808  ....,...........
-00000460: 1800 0000 0000 0000 1808 0000 0000 0000  ................
-00000470: 0000 1600 2808 1800 0000 0000 0000 1808  ....(...........
-00000480: 0000 0000 0000 0000 0000 000b 2802 0000  ............(...
-00000490: 000c 0103 0388 c602 26b0 121c 1504 1935  ........&......5
-000004a0: 1000 0619 1811 5f5f 696e 6465 785f 6c65  ......__index_le
-000004b0: 7665 6c5f 305f 5f15 0216 0c16 8c02 16f4  vel_0__.........
-000004c0: 0126 9c11 26bc 101c 1808 1800 0000 0000  .&..&...........
-000004d0: 0000 1808 0000 0000 0000 0000 1600 2808  ..............(.
-000004e0: 1800 0000 0000 0000 1808 0000 0000 0000  ................
-000004f0: 0000 0019 2c15 0415 0015 0200 1500 1510  ....,...........
-00000500: 1502 0000 0015 0419 7c35 0018 0673 6368  ........|5...sch
-00000510: 656d 6115 0c00 1504 2502 1802 6964 0015  ema.....%...id..
-00000520: 0a25 0218 0272 6100 150a 2502 1803 6465  .%...ra...%...de
-00000530: 6300 1504 2502 1808 7261 5f65 7272 6f72  c...%...ra_error
-00000540: 0015 0425 0218 0964 6563 5f65 7272 6f72  ...%...dec_error
-00000550: 0015 0425 0218 115f 5f69 6e64 6578 5f6c  ...%...__index_l
-00000560: 6576 656c 5f30 5f5f 0016 0c19 1c19 6c26  evel_0__......l&
-00000570: 8002 1c15 0419 3510 0006 1918 0269 6415  ......5......id.
-00000580: 0216 0c16 8c02 16f8 0126 6c26 081c 1808  .........&l&....
-00000590: ed02 0000 0000 0000 1808 d502 0000 0000  ................
-000005a0: 0000 1600 2808 ed02 0000 0000 0000 1808  ....(...........
-000005b0: d502 0000 0000 0000 0019 2c15 0415 0015  ..........,.....
-000005c0: 0200 1500 1510 1502 0000 0026 b205 1c15  ...........&....
-000005d0: 0a19 3510 0006 1918 0272 6115 0216 0c16  ..5......ra.....
-000005e0: 8c02 16fa 0126 9e04 26b8 031c 1808 0000  .....&..&.......
-000005f0: 0000 0048 7340 1808 0000 0000 00b8 7140  ...Hs@........q@
-00000600: 1600 2808 0000 0000 0048 7340 1808 0000  ..(......Hs@....
-00000610: 0000 00b8 7140 0019 2c15 0415 0015 0200  ....q@..,.......
-00000620: 1500 1510 1502 0000 0026 ec08 1c15 0a19  .........&......
-00000630: 3510 0006 1918 0364 6563 1502 160c 168c  5......dec......
-00000640: 0216 fe01 26d8 0726 ee06 1c18 0800 0000  ....&..&........
-00000650: 0000 803f c018 0800 0000 0000 c04b c016  ...?.........K..
-00000660: 0028 0800 0000 0000 803f c018 0800 0000  .(.......?......
-00000670: 0000 c04b c000 192c 1504 1500 1502 0015  ...K...,........
-00000680: 0015 1015 0200 0000 26ea 0b1c 1504 1935  ........&......5
-00000690: 1000 0619 1808 7261 5f65 7272 6f72 1502  ......ra_error..
-000006a0: 160c 16b8 0116 c001 26da 0a26 aa0a 1c18  ........&..&....
-000006b0: 0800 0000 0000 0000 0018 0800 0000 0000  ................
-000006c0: 0000 0016 0028 0800 0000 0000 0000 0018  .....(..........
-000006d0: 0800 0000 0000 0000 0000 192c 1504 1500  ...........,....
-000006e0: 1502 0015 0015 1015 0200 0000 26f2 0e1c  ............&...
-000006f0: 1504 1935 1000 0619 1809 6465 635f 6572  ...5......dec_er
-00000700: 726f 7215 0216 0c16 b801 16c0 0126 e20d  ror..........&..
-00000710: 26b2 0d1c 1808 0000 0000 0000 0000 1808  &...............
-00000720: 0000 0000 0000 0000 1600 2808 0000 0000  ..........(.....
-00000730: 0000 0000 1808 0000 0000 0000 0000 0019  ................
-00000740: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
-00000750: 0026 b012 1c15 0419 3510 0006 1918 115f  .&......5......_
-00000760: 5f69 6e64 6578 5f6c 6576 656c 5f30 5f5f  _index_level_0__
-00000770: 1502 160c 168c 0216 f401 269c 1126 bc10  ..........&..&..
-00000780: 1c18 0818 0000 0000 0000 0018 0800 0000  ................
-00000790: 0000 0000 0016 0028 0818 0000 0000 0000  .......(........
-000007a0: 0018 0800 0000 0000 0000 0000 192c 1504  .............,..
-000007b0: 1500 1502 0015 0015 1015 0200 0000 16a0  ................
-000007c0: 0b16 0c26 0816 e40a 1400 0019 2c18 0670  ...&........,..p
-000007d0: 616e 6461 7318 a507 7b22 696e 6465 785f  andas...{"index_
-000007e0: 636f 6c75 6d6e 7322 3a20 5b22 5f5f 696e  columns": ["__in
-000007f0: 6465 785f 6c65 7665 6c5f 305f 5f22 5d2c  dex_level_0__"],
-00000800: 2022 636f 6c75 6d6e 5f69 6e64 6578 6573   "column_indexes
-00000810: 223a 205b 7b22 6e61 6d65 223a 206e 756c  ": [{"name": nul
-00000820: 6c2c 2022 6669 656c 645f 6e61 6d65 223a  l, "field_name":
-00000830: 206e 756c 6c2c 2022 7061 6e64 6173 5f74   null, "pandas_t
-00000840: 7970 6522 3a20 2275 6e69 636f 6465 222c  ype": "unicode",
-00000850: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
-00000860: 6f62 6a65 6374 222c 2022 6d65 7461 6461  object", "metada
-00000870: 7461 223a 207b 2265 6e63 6f64 696e 6722  ta": {"encoding"
-00000880: 3a20 2255 5446 2d38 227d 7d5d 2c20 2263  : "UTF-8"}}], "c
-00000890: 6f6c 756d 6e73 223a 205b 7b22 6e61 6d65  olumns": [{"name
-000008a0: 223a 2022 6964 222c 2022 6669 656c 645f  ": "id", "field_
-000008b0: 6e61 6d65 223a 2022 6964 222c 2022 7061  name": "id", "pa
-000008c0: 6e64 6173 5f74 7970 6522 3a20 2269 6e74  ndas_type": "int
-000008d0: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
-000008e0: 223a 2022 696e 7436 3422 2c20 226d 6574  ": "int64", "met
-000008f0: 6164 6174 6122 3a20 6e75 6c6c 7d2c 207b  adata": null}, {
-00000900: 226e 616d 6522 3a20 2272 6122 2c20 2266  "name": "ra", "f
-00000910: 6965 6c64 5f6e 616d 6522 3a20 2272 6122  ield_name": "ra"
-00000920: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
-00000930: 2022 666c 6f61 7436 3422 2c20 226e 756d   "float64", "num
-00000940: 7079 5f74 7970 6522 3a20 2266 6c6f 6174  py_type": "float
-00000950: 3634 222c 2022 6d65 7461 6461 7461 223a  64", "metadata":
-00000960: 206e 756c 6c7d 2c20 7b22 6e61 6d65 223a   null}, {"name":
-00000970: 2022 6465 6322 2c20 2266 6965 6c64 5f6e   "dec", "field_n
-00000980: 616d 6522 3a20 2264 6563 222c 2022 7061  ame": "dec", "pa
-00000990: 6e64 6173 5f74 7970 6522 3a20 2266 6c6f  ndas_type": "flo
-000009a0: 6174 3634 222c 2022 6e75 6d70 795f 7479  at64", "numpy_ty
-000009b0: 7065 223a 2022 666c 6f61 7436 3422 2c20  pe": "float64", 
-000009c0: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
-000009d0: 7d2c 207b 226e 616d 6522 3a20 2272 615f  }, {"name": "ra_
-000009e0: 6572 726f 7222 2c20 2266 6965 6c64 5f6e  error", "field_n
-000009f0: 616d 6522 3a20 2272 615f 6572 726f 7222  ame": "ra_error"
-00000a00: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
-00000a10: 2022 696e 7436 3422 2c20 226e 756d 7079   "int64", "numpy
-00000a20: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
-00000a30: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
-00000a40: 6c7d 2c20 7b22 6e61 6d65 223a 2022 6465  l}, {"name": "de
-00000a50: 635f 6572 726f 7222 2c20 2266 6965 6c64  c_error", "field
-00000a60: 5f6e 616d 6522 3a20 2264 6563 5f65 7272  _name": "dec_err
-00000a70: 6f72 222c 2022 7061 6e64 6173 5f74 7970  or", "pandas_typ
-00000a80: 6522 3a20 2269 6e74 3634 222c 2022 6e75  e": "int64", "nu
-00000a90: 6d70 795f 7479 7065 223a 2022 696e 7436  mpy_type": "int6
-00000aa0: 3422 2c20 226d 6574 6164 6174 6122 3a20  4", "metadata": 
-00000ab0: 6e75 6c6c 7d2c 207b 226e 616d 6522 3a20  null}, {"name": 
-00000ac0: 6e75 6c6c 2c20 2266 6965 6c64 5f6e 616d  null, "field_nam
-00000ad0: 6522 3a20 225f 5f69 6e64 6578 5f6c 6576  e": "__index_lev
-00000ae0: 656c 5f30 5f5f 222c 2022 7061 6e64 6173  el_0__", "pandas
-00000af0: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
-00000b00: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
-00000b10: 696e 7436 3422 2c20 226d 6574 6164 6174  int64", "metadat
-00000b20: 6122 3a20 6e75 6c6c 7d5d 2c20 2263 7265  a": null}], "cre
-00000b30: 6174 6f72 223a 207b 226c 6962 7261 7279  ator": {"library
-00000b40: 223a 2022 7079 6172 726f 7722 2c20 2276  ": "pyarrow", "v
-00000b50: 6572 7369 6f6e 223a 2022 392e 302e 3022  ersion": "9.0.0"
-00000b60: 7d2c 2022 7061 6e64 6173 5f76 6572 7369  }, "pandas_versi
-00000b70: 6f6e 223a 2022 312e 332e 3522 7d00 180c  on": "1.3.5"}...
-00000b80: 4152 524f 573a 7363 6865 6d61 18c0 0e2f  ARROW:schema.../
-00000b90: 2f2f 2f2f 3267 4641 4141 5141 4141 4141  ////2gFAAAQAAAAA
-00000ba0: 4141 4b41 4134 4142 6741 4641 4167 4143  AAKAA4ABgAFAAgAC
-00000bb0: 6741 4141 4141 4242 4141 5141 4141 4141  gAAAAABBAAQAAAAA
-00000bc0: 4141 4b41 4177 4141 4141 4541 4167 4143  AAKAAwAAAAEAAgAC
-00000bd0: 6741 4141 4e77 4441 4141 4541 4141 4141  gAAANwDAAAEAAAAA
-00000be0: 5141 4141 4177 4141 4141 4941 4177 4142  QAAAAwAAAAIAAwAB
-00000bf0: 4141 4941 4167 4141 4141 4941 4141 4145  AAIAAgAAAAIAAAAE
-00000c00: 4141 4141 4159 4141 4142 7759 5735 6b59  AAAAAYAAABwYW5kY
-00000c10: 584d 4141 4b55 4441 4142 3749 6d6c 755a  XMAAKUDAAB7ImluZ
-00000c20: 4756 3458 324e 7662 4856 7462 6e4d 694f  GV4X2NvbHVtbnMiO
-00000c30: 6942 6249 6c39 6661 5735 6b5a 5868 6662  iBbIl9faW5kZXhfb
-00000c40: 4756 325a 5778 664d 4639 6649 6c30 7349  GV2ZWxfMF9fIl0sI
-00000c50: 434a 6a62 3278 3162 5735 6661 5735 6b5a  CJjb2x1bW5faW5kZ
-00000c60: 5868 6c63 7949 3649 4674 3749 6d35 6862  XhlcyI6IFt7Im5hb
-00000c70: 5755 694f 6942 7564 5778 734c 4341 695a  WUiOiBudWxsLCAiZ
-00000c80: 6d6c 6c62 4752 6662 6d46 745a 5349 3649  mllbGRfbmFtZSI6I
-00000c90: 4735 3162 4777 7349 434a 7759 5735 6b59  G51bGwsICJwYW5kY
-00000ca0: 584e 6664 486c 775a 5349 3649 434a 3162  XNfdHlwZSI6ICJ1b
-00000cb0: 6d6c 6a62 3252 6c49 6977 6749 6d35 3162  mljb2RlIiwgIm51b
-00000cc0: 5842 3558 3352 3563 4755 694f 6941 6962  XB5X3R5cGUiOiAib
-00000cd0: 324a 715a 574e 3049 6977 6749 6d31 6c64  2JqZWN0IiwgIm1ld
-00000ce0: 4746 6b59 5852 6849 6a6f 6765 794a 6c62  GFkYXRhIjogeyJlb
-00000cf0: 6d4e 765a 476c 755a 7949 3649 434a 5656  mNvZGluZyI6ICJVV
-00000d00: 4559 744f 434a 3966 5630 7349 434a 6a62  EYtOCJ9fV0sICJjb
-00000d10: 3278 3162 5735 7a49 6a6f 6757 3373 6962  2x1bW5zIjogW3sib
-00000d20: 6d46 745a 5349 3649 434a 705a 4349 7349  mFtZSI6ICJpZCIsI
-00000d30: 434a 6d61 5756 735a 4639 7559 5731 6c49  CJmaWVsZF9uYW1lI
-00000d40: 6a6f 6749 6d6c 6b49 6977 6749 6e42 6862  jogImlkIiwgInBhb
-00000d50: 6d52 6863 3139 3065 5842 6c49 6a6f 6749  mRhc190eXBlIjogI
-00000d60: 6d6c 7564 4459 3049 6977 6749 6d35 3162  mludDY0IiwgIm51b
-00000d70: 5842 3558 3352 3563 4755 694f 6941 6961  XB5X3R5cGUiOiAia
-00000d80: 5735 304e 6a51 694c 4341 6962 5756 3059  W50NjQiLCAibWV0Y
-00000d90: 5752 6864 4745 694f 6942 7564 5778 7366  WRhdGEiOiBudWxsf
-00000da0: 5377 6765 794a 7559 5731 6c49 6a6f 6749  SwgeyJuYW1lIjogI
-00000db0: 6e4a 6849 6977 6749 6d5a 705a 5778 6b58  nJhIiwgImZpZWxkX
-00000dc0: 3235 6862 5755 694f 6941 6963 6d45 694c  25hbWUiOiAicmEiL
-00000dd0: 4341 6963 4746 755a 4746 7a58 3352 3563  CAicGFuZGFzX3R5c
-00000de0: 4755 694f 6941 695a 6d78 7659 5851 324e  GUiOiAiZmxvYXQ2N
-00000df0: 4349 7349 434a 7564 5731 7765 5639 3065  CIsICJudW1weV90e
-00000e00: 5842 6c49 6a6f 6749 6d5a 7362 3246 304e  XBlIjogImZsb2F0N
-00000e10: 6a51 694c 4341 6962 5756 3059 5752 6864  jQiLCAibWV0YWRhd
-00000e20: 4745 694f 6942 7564 5778 7366 5377 6765  GEiOiBudWxsfSwge
-00000e30: 794a 7559 5731 6c49 6a6f 6749 6d52 6c59  yJuYW1lIjogImRlY
-00000e40: 7949 7349 434a 6d61 5756 735a 4639 7559  yIsICJmaWVsZF9uY
-00000e50: 5731 6c49 6a6f 6749 6d52 6c59 7949 7349  W1lIjogImRlYyIsI
-00000e60: 434a 7759 5735 6b59 584e 6664 486c 775a  CJwYW5kYXNfdHlwZ
-00000e70: 5349 3649 434a 6d62 4739 6864 4459 3049  SI6ICJmbG9hdDY0I
-00000e80: 6977 6749 6d35 3162 5842 3558 3352 3563  iwgIm51bXB5X3R5c
-00000e90: 4755 694f 6941 695a 6d78 7659 5851 324e  GUiOiAiZmxvYXQ2N
-00000ea0: 4349 7349 434a 745a 5852 685a 4746 3059  CIsICJtZXRhZGF0Y
-00000eb0: 5349 3649 4735 3162 4778 394c 4342 3749  SI6IG51bGx9LCB7I
-00000ec0: 6d35 6862 5755 694f 6941 6963 6d46 665a  m5hbWUiOiAicmFfZ
-00000ed0: 584a 7962 3349 694c 4341 695a 6d6c 6c62  XJyb3IiLCAiZmllb
-00000ee0: 4752 6662 6d46 745a 5349 3649 434a 7959  GRfbmFtZSI6ICJyY
-00000ef0: 5639 6c63 6e4a 7663 6949 7349 434a 7759  V9lcnJvciIsICJwY
-00000f00: 5735 6b59 584e 6664 486c 775a 5349 3649  W5kYXNfdHlwZSI6I
-00000f10: 434a 7062 6e51 324e 4349 7349 434a 7564  CJpbnQ2NCIsICJud
-00000f20: 5731 7765 5639 3065 5842 6c49 6a6f 6749  W1weV90eXBlIjogI
-00000f30: 6d6c 7564 4459 3049 6977 6749 6d31 6c64  mludDY0IiwgIm1ld
-00000f40: 4746 6b59 5852 6849 6a6f 6762 6e56 7362  GFkYXRhIjogbnVsb
-00000f50: 4830 7349 4873 6962 6d46 745a 5349 3649  H0sIHsibmFtZSI6I
-00000f60: 434a 6b5a 574e 665a 584a 7962 3349 694c  CJkZWNfZXJyb3IiL
-00000f70: 4341 695a 6d6c 6c62 4752 6662 6d46 745a  CAiZmllbGRfbmFtZ
-00000f80: 5349 3649 434a 6b5a 574e 665a 584a 7962  SI6ICJkZWNfZXJyb
-00000f90: 3349 694c 4341 6963 4746 755a 4746 7a58  3IiLCAicGFuZGFzX
-00000fa0: 3352 3563 4755 694f 6941 6961 5735 304e  3R5cGUiOiAiaW50N
-00000fb0: 6a51 694c 4341 6962 6e56 7463 486c 6664  jQiLCAibnVtcHlfd
-00000fc0: 486c 775a 5349 3649 434a 7062 6e51 324e  HlwZSI6ICJpbnQ2N
-00000fd0: 4349 7349 434a 745a 5852 685a 4746 3059  CIsICJtZXRhZGF0Y
-00000fe0: 5349 3649 4735 3162 4778 394c 4342 3749  SI6IG51bGx9LCB7I
-00000ff0: 6d35 6862 5755 694f 6942 7564 5778 734c  m5hbWUiOiBudWxsL
-00001000: 4341 695a 6d6c 6c62 4752 6662 6d46 745a  CAiZmllbGRfbmFtZ
-00001010: 5349 3649 434a 6658 326c 755a 4756 3458  SI6ICJfX2luZGV4X
-00001020: 3278 6c64 6d56 7358 7a42 6658 7949 7349  2xldmVsXzBfXyIsI
-00001030: 434a 7759 5735 6b59 584e 6664 486c 775a  CJwYW5kYXNfdHlwZ
-00001040: 5349 3649 434a 7062 6e51 324e 4349 7349  SI6ICJpbnQ2NCIsI
-00001050: 434a 7564 5731 7765 5639 3065 5842 6c49  CJudW1weV90eXBlI
-00001060: 6a6f 6749 6d6c 7564 4459 3049 6977 6749  jogImludDY0IiwgI
-00001070: 6d31 6c64 4746 6b59 5852 6849 6a6f 6762  m1ldGFkYXRhIjogb
-00001080: 6e56 7362 4831 644c 4341 6959 334a 6c59  nVsbH1dLCAiY3JlY
-00001090: 5852 7663 6949 3649 4873 6962 476c 6963  XRvciI6IHsibGlic
-000010a0: 6d46 7965 5349 3649 434a 7765 5746 7963  mFyeSI6ICJweWFyc
-000010b0: 6d39 3349 6977 6749 6e5a 6c63 6e4e 7062  m93IiwgInZlcnNpb
-000010c0: 3234 694f 6941 694f 5334 774c 6a41 6966  24iOiAiOS4wLjAif
-000010d0: 5377 6749 6e42 6862 6d52 6863 3139 325a  SwgInBhbmRhc192Z
-000010e0: 584a 7a61 5739 7549 6a6f 6749 6a45 754d  XJzaW9uIjogIjEuM
-000010f0: 7934 3149 6e30 4141 4141 4741 4141 414a  y41In0AAAAGAAAAJ
-00001100: 4145 4141 4f41 4141 4143 3041 4141 4166  AEAAOAAAAC0AAAAf
-00001110: 4141 4141 4551 4141 4141 4541 4141 4142  AAAAEQAAAAEAAAAB
-00001120: 502f 2f2f 7741 4141 5149 5141 4141 414a  P///wAAAQIQAAAAJ
-00001130: 4141 4141 4151 4141 4141 4141 4141 4145  AAAAAQAAAAAAAAAE
-00001140: 5141 4141 4639 6661 5735 6b5a 5868 6662  QAAAF9faW5kZXhfb
-00001150: 4756 325a 5778 664d 4639 6641 4141 4142  GV2ZWxfMF9fAAAAB
-00001160: 502f 2f2f 7741 4141 4146 4141 4141 4151  P///wAAAAFAAAAAQ
-00001170: 502f 2f2f 7741 4141 5149 5141 4141 4148  P///wAAAQIQAAAAH
-00001180: 4141 4141 4151 4141 4141 4141 4141 4143  AAAAAQAAAAAAAAAC
-00001190: 5141 4141 4752 6c59 3139 6c63 6e4a 7663  QAAAGRlY19lcnJvc
-000011a0: 6741 4141 446a 2f2f 2f38 4141 4141 4251  gAAADj///8AAAABQ
-000011b0: 4141 4141 4854 2f2f 2f38 4141 4145 4345  AAAAHT///8AAAECE
-000011c0: 4141 4141 4277 4141 4141 4541 4141 4141  AAAABwAAAAEAAAAA
-000011d0: 4141 4141 4167 4141 4142 7959 5639 6c63  AAAAAgAAAByYV9lc
-000011e0: 6e4a 7663 6741 4141 4142 732f 2f2f 2f41  nJvcgAAAABs////A
-000011f0: 4141 4141 5541 4141 4143 6f2f 2f2f 2f41  AAAAUAAAACo////A
-00001200: 4141 4241 7841 4141 4141 5541 4141 4142  AABAxAAAAAUAAAAB
-00001210: 4141 4141 4141 4141 4141 4441 4141 415a  AAAAAAAAAADAAAAZ
-00001220: 4756 6a41 4e62 2f2f 2f38 4141 4149 4130  GVjANb///8AAAIA0
-00001230: 502f 2f2f 7741 4141 514d 5141 4141 4148  P///wAAAQMQAAAAH
-00001240: 4141 4141 4151 4141 4141 4141 4141 4141  AAAAAQAAAAAAAAAA
-00001250: 6741 4141 484a 6841 4141 4141 4159 4143  gAAAHJhAAAAAAYAC
-00001260: 4141 4741 4159 4141 4141 4141 4149 4145  AAGAAYAAAAAAAIAE
-00001270: 4141 5541 4167 4142 6741 4841 4177 4141  AAUAAgABgAHAAwAA
-00001280: 4141 5141 4241 4141 4141 4141 4145 4345  AAQABAAAAAAAAECE
-00001290: 4141 4141 4277 4141 4141 4541 4141 4141  AAAABwAAAAEAAAAA
-000012a0: 4141 4141 4149 4141 4142 705a 4141 4143  AAAAAIAAABpZAAAC
-000012b0: 4141 4d41 4167 4142 7741 4941 4141 4141  AAMAAgABwAIAAAAA
-000012c0: 4141 4141 5541 4141 4141 4141 4141 4100  AAAAUAAAAAAAAAA.
-000012d0: 181f 7061 7271 7565 742d 6370 702d 6172  ..parquet-cpp-ar
-000012e0: 726f 7720 7665 7273 696f 6e20 392e 302e  row version 9.0.
-000012f0: 3019 6c1c 0000 1c00 001c 0000 1c00 001c  0.l.............
-00001300: 0000 1c00 0000 010e 0000 5041 5231       ..........PAR1
+00000000: 5041 5231 1504 19ac 3500 1806 7363 6865  PAR1....5...sche
+00000010: 6d61 1512 0015 0425 0218 0269 6400 150a  ma.....%...id...
+00000020: 2502 1802 7261 0015 0a25 0218 0364 6563  %...ra...%...dec
+00000030: 0015 0425 0218 0872 615f 6572 726f 7200  ...%...ra_error.
+00000040: 1504 2502 1809 6465 635f 6572 726f 7200  ..%...dec_error.
+00000050: 1502 2502 1806 4e6f 7264 6572 0015 0225  ..%...Norder...%
+00000060: 0218 0344 6972 0015 0225 0218 044e 7069  ...Dir...%...Npi
+00000070: 7800 1504 2502 180e 5f68 6970 7363 6174  x...%..._hipscat
+00000080: 5f69 6e64 6578 251c 4cac 1340 1200 0000  _index%.L..@....
+00000090: 1686 0219 1c19 9c18 1f2f 4e6f 7264 6572  ........./Norder
+000000a0: 3d30 2f44 6972 3d30 2f4e 7069 783d 3131  =0/Dir=0/Npix=11
+000000b0: 2e70 6172 7175 6574 168a 0c1c 1504 1935  .parquet.......5
+000000c0: 1000 0619 1802 6964 1502 1686 0216 f413  ......id........
+000000d0: 1682 0c26 e008 2608 1c18 083e 0300 0000  ...&..&....>....
+000000e0: 0000 0018 08bc 0200 0000 0000 0016 0028  ...............(
+000000f0: 083e 0300 0000 0000 0018 08bc 0200 0000  .>..............
+00000100: 0000 0000 192c 1504 1500 1502 0015 0015  .....,..........
+00000110: 1015 0200 0000 181f 2f4e 6f72 6465 723d  ......../Norder=
+00000120: 302f 4469 723d 302f 4e70 6978 3d31 312e  0/Dir=0/Npix=11.
+00000130: 7061 7271 7565 7416 b814 1c15 0a19 3510  parquet.......5.
+00000140: 0006 1918 0272 6115 0216 8602 16ae 0a16  .....ra.........
+00000150: f206 26d4 1126 c60d 1c18 0800 0000 0000  ..&..&..........
+00000160: e875 4018 0800 0000 0000 8871 4016 0028  .u@........q@..(
+00000170: 0800 0000 0000 e875 4018 0800 0000 0000  .......u@.......
+00000180: 8871 4000 192c 1504 1500 1502 0015 0015  .q@..,..........
+00000190: 1015 0200 0000 181f 2f4e 6f72 6465 723d  ......../Norder=
+000001a0: 302f 4469 723d 302f 4e70 6978 3d31 312e  0/Dir=0/Npix=11.
+000001b0: 7061 7271 7565 7416 f41b 1c15 0a19 3510  parquet.......5.
+000001c0: 0006 1918 0364 6563 1502 1686 0216 be08  .....dec........
+000001d0: 16fe 0526 9019 26f6 151c 1808 0000 0000  ...&..&.........
+000001e0: 0080 39c0 1808 0000 0000 0060 51c0 1600  ..9........`Q...
+000001f0: 2808 0000 0000 0080 39c0 1808 0000 0000  (.......9.......
+00000200: 0060 51c0 0019 2c15 0415 0015 0200 1500  .`Q...,.........
+00000210: 1510 1502 0000 0018 1f2f 4e6f 7264 6572  ........./Norder
+00000220: 3d30 2f44 6972 3d30 2f4e 7069 783d 3131  =0/Dir=0/Npix=11
+00000230: 2e70 6172 7175 6574 16fa 1e1c 1504 1935  .parquet.......5
+00000240: 1000 0619 1808 7261 5f65 7272 6f72 1502  ......ra_error..
+00000250: 1686 0216 be01 16c6 0126 e41d 26b4 1d1c  .........&..&...
+00000260: 1808 0000 0000 0000 0000 1808 0000 0000  ................
+00000270: 0000 0000 1600 2808 0000 0000 0000 0000  ......(.........
+00000280: 1808 0000 0000 0000 0000 0019 2c15 0415  ............,...
+00000290: 0015 0200 1500 1510 1502 0000 0018 1f2f  .............../
+000002a0: 4e6f 7264 6572 3d30 2f44 6972 3d30 2f4e  Norder=0/Dir=0/N
+000002b0: 7069 783d 3131 2e70 6172 7175 6574 168a  pix=11.parquet..
+000002c0: 221c 1504 1935 1000 0619 1809 6465 635f  "....5......dec_
+000002d0: 6572 726f 7215 0216 8602 16be 0116 c601  error...........
+000002e0: 26f4 2026 c420 1c18 0800 0000 0000 0000  &. &. ..........
+000002f0: 0018 0800 0000 0000 0000 0016 0028 0800  .............(..
+00000300: 0000 0000 0000 0018 0800 0000 0000 0000  ................
+00000310: 0000 192c 1504 1500 1502 0015 0015 1015  ...,............
+00000320: 0200 0000 181f 2f4e 6f72 6465 723d 302f  ....../Norder=0/
+00000330: 4469 723d 302f 4e70 6978 3d31 312e 7061  Dir=0/Npix=11.pa
+00000340: 7271 7565 7416 f424 1c15 0219 3510 0006  rquet..$....5...
+00000350: 1918 064e 6f72 6465 7215 0216 8602 1696  ...Norder.......
+00000360: 0116 9e01 26fe 2326 d623 1c18 0400 0000  ....&.#&.#......
+00000370: 0018 0400 0000 0016 0028 0400 0000 0018  .........(......
+00000380: 0400 0000 0000 192c 1504 1500 1502 0015  .......,........
+00000390: 0015 1015 0200 0000 181f 2f4e 6f72 6465  ........../Norde
+000003a0: 723d 302f 4469 723d 302f 4e70 6978 3d31  r=0/Dir=0/Npix=1
+000003b0: 312e 7061 7271 7565 7416 b827 1c15 0219  1.parquet..'....
+000003c0: 3510 0006 1918 0344 6972 1502 1686 0216  5......Dir......
+000003d0: 9601 169e 0126 c226 269a 261c 1804 0000  .....&.&&.&.....
+000003e0: 0000 1804 0000 0000 1600 2804 0000 0000  ..........(.....
+000003f0: 1804 0000 0000 0019 2c15 0415 0015 0200  ........,.......
+00000400: 1500 1510 1502 0000 0018 1f2f 4e6f 7264  .........../Nord
+00000410: 6572 3d30 2f44 6972 3d30 2f4e 7069 783d  er=0/Dir=0/Npix=
+00000420: 3131 2e70 6172 7175 6574 16f6 291c 1502  11.parquet..)...
+00000430: 1935 1000 0619 1804 4e70 6978 1502 1686  .5......Npix....
+00000440: 0216 9601 169e 0126 8029 26d8 281c 1804  .......&.)&.(...
+00000450: 0b00 0000 1804 0b00 0000 1600 2804 0b00  ............(...
+00000460: 0000 1804 0b00 0000 0019 2c15 0415 0015  ..........,.....
+00000470: 0200 1500 1510 1502 0000 0018 1f2f 4e6f  ............./No
+00000480: 7264 6572 3d30 2f44 6972 3d30 2f4e 7069  rder=0/Dir=0/Npi
+00000490: 783d 3131 2e70 6172 7175 6574 16ba 3e1c  x=11.parquet..>.
+000004a0: 1504 1935 1000 0619 180e 5f68 6970 7363  ...5......_hipsc
+000004b0: 6174 5f69 6e64 6578 1502 1686 0216 cc13  at_index........
+000004c0: 16a2 1326 b83b 2698 2b1c 3600 2808 0000  ...&.;&.+.6.(...
+000004d0: 404a 8a88 14be 1808 0000 807c 7cfe efb0  @J.........||...
+000004e0: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
+000004f0: 0000 0016 ea40 1686 0226 0816 fa32 1400  .....@...&...2..
+00000500: 0019 2c18 0670 616e 6461 7318 ea09 7b22  ..,..pandas...{"
+00000510: 696e 6465 785f 636f 6c75 6d6e 7322 3a20  index_columns": 
+00000520: 5b22 5f68 6970 7363 6174 5f69 6e64 6578  ["_hipscat_index
+00000530: 225d 2c20 2263 6f6c 756d 6e5f 696e 6465  "], "column_inde
+00000540: 7865 7322 3a20 5b7b 226e 616d 6522 3a20  xes": [{"name": 
+00000550: 6e75 6c6c 2c20 2266 6965 6c64 5f6e 616d  null, "field_nam
+00000560: 6522 3a20 6e75 6c6c 2c20 2270 616e 6461  e": null, "panda
+00000570: 735f 7479 7065 223a 2022 756e 6963 6f64  s_type": "unicod
+00000580: 6522 2c20 226e 756d 7079 5f74 7970 6522  e", "numpy_type"
+00000590: 3a20 226f 626a 6563 7422 2c20 226d 6574  : "object", "met
+000005a0: 6164 6174 6122 3a20 7b22 656e 636f 6469  adata": {"encodi
+000005b0: 6e67 223a 2022 5554 462d 3822 7d7d 5d2c  ng": "UTF-8"}}],
+000005c0: 2022 636f 6c75 6d6e 7322 3a20 5b7b 226e   "columns": [{"n
+000005d0: 616d 6522 3a20 2269 6422 2c20 2266 6965  ame": "id", "fie
+000005e0: 6c64 5f6e 616d 6522 3a20 2269 6422 2c20  ld_name": "id", 
+000005f0: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
+00000600: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
+00000610: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
+00000620: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
+00000630: 2c20 7b22 6e61 6d65 223a 2022 7261 222c  , {"name": "ra",
+00000640: 2022 6669 656c 645f 6e61 6d65 223a 2022   "field_name": "
+00000650: 7261 222c 2022 7061 6e64 6173 5f74 7970  ra", "pandas_typ
+00000660: 6522 3a20 2266 6c6f 6174 3634 222c 2022  e": "float64", "
+00000670: 6e75 6d70 795f 7479 7065 223a 2022 666c  numpy_type": "fl
+00000680: 6f61 7436 3422 2c20 226d 6574 6164 6174  oat64", "metadat
+00000690: 6122 3a20 6e75 6c6c 7d2c 207b 226e 616d  a": null}, {"nam
+000006a0: 6522 3a20 2264 6563 222c 2022 6669 656c  e": "dec", "fiel
+000006b0: 645f 6e61 6d65 223a 2022 6465 6322 2c20  d_name": "dec", 
+000006c0: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
+000006d0: 666c 6f61 7436 3422 2c20 226e 756d 7079  float64", "numpy
+000006e0: 5f74 7970 6522 3a20 2266 6c6f 6174 3634  _type": "float64
+000006f0: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
+00000700: 756c 6c7d 2c20 7b22 6e61 6d65 223a 2022  ull}, {"name": "
+00000710: 7261 5f65 7272 6f72 222c 2022 6669 656c  ra_error", "fiel
+00000720: 645f 6e61 6d65 223a 2022 7261 5f65 7272  d_name": "ra_err
+00000730: 6f72 222c 2022 7061 6e64 6173 5f74 7970  or", "pandas_typ
+00000740: 6522 3a20 2269 6e74 3634 222c 2022 6e75  e": "int64", "nu
+00000750: 6d70 795f 7479 7065 223a 2022 696e 7436  mpy_type": "int6
+00000760: 3422 2c20 226d 6574 6164 6174 6122 3a20  4", "metadata": 
+00000770: 6e75 6c6c 7d2c 207b 226e 616d 6522 3a20  null}, {"name": 
+00000780: 2264 6563 5f65 7272 6f72 222c 2022 6669  "dec_error", "fi
+00000790: 656c 645f 6e61 6d65 223a 2022 6465 635f  eld_name": "dec_
+000007a0: 6572 726f 7222 2c20 2270 616e 6461 735f  error", "pandas_
+000007b0: 7479 7065 223a 2022 696e 7436 3422 2c20  type": "int64", 
+000007c0: 226e 756d 7079 5f74 7970 6522 3a20 2269  "numpy_type": "i
+000007d0: 6e74 3634 222c 2022 6d65 7461 6461 7461  nt64", "metadata
+000007e0: 223a 206e 756c 6c7d 2c20 7b22 6e61 6d65  ": null}, {"name
+000007f0: 223a 2022 4e6f 7264 6572 222c 2022 6669  ": "Norder", "fi
+00000800: 656c 645f 6e61 6d65 223a 2022 4e6f 7264  eld_name": "Nord
+00000810: 6572 222c 2022 7061 6e64 6173 5f74 7970  er", "pandas_typ
+00000820: 6522 3a20 2269 6e74 3332 222c 2022 6e75  e": "int32", "nu
+00000830: 6d70 795f 7479 7065 223a 2022 696e 7433  mpy_type": "int3
+00000840: 3222 2c20 226d 6574 6164 6174 6122 3a20  2", "metadata": 
+00000850: 6e75 6c6c 7d2c 207b 226e 616d 6522 3a20  null}, {"name": 
+00000860: 2244 6972 222c 2022 6669 656c 645f 6e61  "Dir", "field_na
+00000870: 6d65 223a 2022 4469 7222 2c20 2270 616e  me": "Dir", "pan
+00000880: 6461 735f 7479 7065 223a 2022 696e 7433  das_type": "int3
+00000890: 3222 2c20 226e 756d 7079 5f74 7970 6522  2", "numpy_type"
+000008a0: 3a20 2269 6e74 3332 222c 2022 6d65 7461  : "int32", "meta
+000008b0: 6461 7461 223a 206e 756c 6c7d 2c20 7b22  data": null}, {"
+000008c0: 6e61 6d65 223a 2022 4e70 6978 222c 2022  name": "Npix", "
+000008d0: 6669 656c 645f 6e61 6d65 223a 2022 4e70  field_name": "Np
+000008e0: 6978 222c 2022 7061 6e64 6173 5f74 7970  ix", "pandas_typ
+000008f0: 6522 3a20 2269 6e74 3332 222c 2022 6e75  e": "int32", "nu
+00000900: 6d70 795f 7479 7065 223a 2022 696e 7433  mpy_type": "int3
+00000910: 3222 2c20 226d 6574 6164 6174 6122 3a20  2", "metadata": 
+00000920: 6e75 6c6c 7d2c 207b 226e 616d 6522 3a20  null}, {"name": 
+00000930: 225f 6869 7073 6361 745f 696e 6465 7822  "_hipscat_index"
+00000940: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
+00000950: 225f 6869 7073 6361 745f 696e 6465 7822  "_hipscat_index"
+00000960: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
+00000970: 2022 7569 6e74 3634 222c 2022 6e75 6d70   "uint64", "nump
+00000980: 795f 7479 7065 223a 2022 7569 6e74 3634  y_type": "uint64
+00000990: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
+000009a0: 756c 6c7d 5d2c 2022 6372 6561 746f 7222  ull}], "creator"
+000009b0: 3a20 7b22 6c69 6272 6172 7922 3a20 2270  : {"library": "p
+000009c0: 7961 7272 6f77 222c 2022 7665 7273 696f  yarrow", "versio
+000009d0: 6e22 3a20 2239 2e30 2e30 227d 2c20 2270  n": "9.0.0"}, "p
+000009e0: 616e 6461 735f 7665 7273 696f 6e22 3a20  andas_version": 
+000009f0: 2232 2e30 2e30 227d 0018 0c41 5252 4f57  "2.0.0"}...ARROW
+00000a00: 3a73 6368 656d 6118 b813 2f2f 2f2f 2f30  :schema.../////0
+00000a10: 4148 4141 4151 4141 4141 4141 414b 4141  AHAAAQAAAAAAAKAA
+00000a20: 3441 4267 4146 4141 6741 4367 4141 4141  4ABgAFAAgACgAAAA
+00000a30: 4142 4241 4151 4141 4141 4141 414b 4141  ABBAAQAAAAAAAKAA
+00000a40: 7741 4141 4145 4141 6741 4367 4141 4143  wAAAAEAAgACgAAAC
+00000a50: 4146 4141 4145 4141 4141 4151 4141 4141  AFAAAEAAAAAQAAAA
+00000a60: 7741 4141 4149 4141 7741 4241 4149 4141  wAAAAIAAwABAAIAA
+00000a70: 6741 4141 4149 4141 4141 4541 4141 4141  gAAAAIAAAAEAAAAA
+00000a80: 5941 4141 4277 5957 356b 5958 4d41 414f  YAAABwYW5kYXMAAO
+00000a90: 6f45 4141 4237 496d 6c75 5a47 5634 5832  oEAAB7ImluZGV4X2
+00000aa0: 4e76 6248 5674 626e 4d69 4f69 4262 496c  NvbHVtbnMiOiBbIl
+00000ab0: 396f 6158 427a 5932 4630 5832 6c75 5a47  9oaXBzY2F0X2luZG
+00000ac0: 5634 496c 3073 4943 4a6a 6232 7831 6257  V4Il0sICJjb2x1bW
+00000ad0: 3566 6157 356b 5a58 686c 6379 4936 4946  5faW5kZXhlcyI6IF
+00000ae0: 7437 496d 3568 6257 5569 4f69 4275 6457  t7Im5hbWUiOiBudW
+00000af0: 7873 4c43 4169 5a6d 6c6c 6247 5266 626d  xsLCAiZmllbGRfbm
+00000b00: 4674 5a53 4936 4947 3531 6247 7773 4943  FtZSI6IG51bGwsIC
+00000b10: 4a77 5957 356b 5958 4e66 6448 6c77 5a53  JwYW5kYXNfdHlwZS
+00000b20: 4936 4943 4a31 626d 6c6a 6232 526c 4969  I6ICJ1bmljb2RlIi
+00000b30: 7767 496d 3531 6258 4235 5833 5235 6347  wgIm51bXB5X3R5cG
+00000b40: 5569 4f69 4169 6232 4a71 5a57 4e30 4969  UiOiAib2JqZWN0Ii
+00000b50: 7767 496d 316c 6447 466b 5958 5268 496a  wgIm1ldGFkYXRhIj
+00000b60: 6f67 6579 4a6c 626d 4e76 5a47 6c75 5a79  ogeyJlbmNvZGluZy
+00000b70: 4936 4943 4a56 5645 5974 4f43 4a39 6656  I6ICJVVEYtOCJ9fV
+00000b80: 3073 4943 4a6a 6232 7831 6257 357a 496a  0sICJjb2x1bW5zIj
+00000b90: 6f67 5733 7369 626d 4674 5a53 4936 4943  ogW3sibmFtZSI6IC
+00000ba0: 4a70 5a43 4973 4943 4a6d 6157 5673 5a46  JpZCIsICJmaWVsZF
+00000bb0: 3975 5957 316c 496a 6f67 496d 6c6b 4969  9uYW1lIjogImlkIi
+00000bc0: 7767 496e 4268 626d 5268 6331 3930 6558  wgInBhbmRhc190eX
+00000bd0: 426c 496a 6f67 496d 6c75 6444 5930 4969  BlIjogImludDY0Ii
+00000be0: 7767 496d 3531 6258 4235 5833 5235 6347  wgIm51bXB5X3R5cG
+00000bf0: 5569 4f69 4169 6157 3530 4e6a 5169 4c43  UiOiAiaW50NjQiLC
+00000c00: 4169 6257 5630 5957 5268 6447 4569 4f69  AibWV0YWRhdGEiOi
+00000c10: 4275 6457 7873 6653 7767 6579 4a75 5957  BudWxsfSwgeyJuYW
+00000c20: 316c 496a 6f67 496e 4a68 4969 7767 496d  1lIjogInJhIiwgIm
+00000c30: 5a70 5a57 786b 5832 3568 6257 5569 4f69  ZpZWxkX25hbWUiOi
+00000c40: 4169 636d 4569 4c43 4169 6347 4675 5a47  AicmEiLCAicGFuZG
+00000c50: 467a 5833 5235 6347 5569 4f69 4169 5a6d  FzX3R5cGUiOiAiZm
+00000c60: 7876 5958 5132 4e43 4973 4943 4a75 6457  xvYXQ2NCIsICJudW
+00000c70: 3177 6556 3930 6558 426c 496a 6f67 496d  1weV90eXBlIjogIm
+00000c80: 5a73 6232 4630 4e6a 5169 4c43 4169 6257  Zsb2F0NjQiLCAibW
+00000c90: 5630 5957 5268 6447 4569 4f69 4275 6457  V0YWRhdGEiOiBudW
+00000ca0: 7873 6653 7767 6579 4a75 5957 316c 496a  xsfSwgeyJuYW1lIj
+00000cb0: 6f67 496d 526c 5979 4973 4943 4a6d 6157  ogImRlYyIsICJmaW
+00000cc0: 5673 5a46 3975 5957 316c 496a 6f67 496d  VsZF9uYW1lIjogIm
+00000cd0: 526c 5979 4973 4943 4a77 5957 356b 5958  RlYyIsICJwYW5kYX
+00000ce0: 4e66 6448 6c77 5a53 4936 4943 4a6d 6247  NfdHlwZSI6ICJmbG
+00000cf0: 3968 6444 5930 4969 7767 496d 3531 6258  9hdDY0IiwgIm51bX
+00000d00: 4235 5833 5235 6347 5569 4f69 4169 5a6d  B5X3R5cGUiOiAiZm
+00000d10: 7876 5958 5132 4e43 4973 4943 4a74 5a58  xvYXQ2NCIsICJtZX
+00000d20: 5268 5a47 4630 5953 4936 4947 3531 6247  RhZGF0YSI6IG51bG
+00000d30: 7839 4c43 4237 496d 3568 6257 5569 4f69  x9LCB7Im5hbWUiOi
+00000d40: 4169 636d 4666 5a58 4a79 6233 4969 4c43  AicmFfZXJyb3IiLC
+00000d50: 4169 5a6d 6c6c 6247 5266 626d 4674 5a53  AiZmllbGRfbmFtZS
+00000d60: 4936 4943 4a79 5956 396c 636e 4a76 6369  I6ICJyYV9lcnJvci
+00000d70: 4973 4943 4a77 5957 356b 5958 4e66 6448  IsICJwYW5kYXNfdH
+00000d80: 6c77 5a53 4936 4943 4a70 626e 5132 4e43  lwZSI6ICJpbnQ2NC
+00000d90: 4973 4943 4a75 6457 3177 6556 3930 6558  IsICJudW1weV90eX
+00000da0: 426c 496a 6f67 496d 6c75 6444 5930 4969  BlIjogImludDY0Ii
+00000db0: 7767 496d 316c 6447 466b 5958 5268 496a  wgIm1ldGFkYXRhIj
+00000dc0: 6f67 626e 5673 6248 3073 4948 7369 626d  ogbnVsbH0sIHsibm
+00000dd0: 4674 5a53 4936 4943 4a6b 5a57 4e66 5a58  FtZSI6ICJkZWNfZX
+00000de0: 4a79 6233 4969 4c43 4169 5a6d 6c6c 6247  Jyb3IiLCAiZmllbG
+00000df0: 5266 626d 4674 5a53 4936 4943 4a6b 5a57  RfbmFtZSI6ICJkZW
+00000e00: 4e66 5a58 4a79 6233 4969 4c43 4169 6347  NfZXJyb3IiLCAicG
+00000e10: 4675 5a47 467a 5833 5235 6347 5569 4f69  FuZGFzX3R5cGUiOi
+00000e20: 4169 6157 3530 4e6a 5169 4c43 4169 626e  AiaW50NjQiLCAibn
+00000e30: 5674 6348 6c66 6448 6c77 5a53 4936 4943  VtcHlfdHlwZSI6IC
+00000e40: 4a70 626e 5132 4e43 4973 4943 4a74 5a58  JpbnQ2NCIsICJtZX
+00000e50: 5268 5a47 4630 5953 4936 4947 3531 6247  RhZGF0YSI6IG51bG
+00000e60: 7839 4c43 4237 496d 3568 6257 5569 4f69  x9LCB7Im5hbWUiOi
+00000e70: 4169 546d 3979 5a47 5679 4969 7767 496d  AiTm9yZGVyIiwgIm
+00000e80: 5a70 5a57 786b 5832 3568 6257 5569 4f69  ZpZWxkX25hbWUiOi
+00000e90: 4169 546d 3979 5a47 5679 4969 7767 496e  AiTm9yZGVyIiwgIn
+00000ea0: 4268 626d 5268 6331 3930 6558 426c 496a  BhbmRhc190eXBlIj
+00000eb0: 6f67 496d 6c75 6444 4d79 4969 7767 496d  ogImludDMyIiwgIm
+00000ec0: 3531 6258 4235 5833 5235 6347 5569 4f69  51bXB5X3R5cGUiOi
+00000ed0: 4169 6157 3530 4d7a 4969 4c43 4169 6257  AiaW50MzIiLCAibW
+00000ee0: 5630 5957 5268 6447 4569 4f69 4275 6457  V0YWRhdGEiOiBudW
+00000ef0: 7873 6653 7767 6579 4a75 5957 316c 496a  xsfSwgeyJuYW1lIj
+00000f00: 6f67 496b 5270 6369 4973 4943 4a6d 6157  ogIkRpciIsICJmaW
+00000f10: 5673 5a46 3975 5957 316c 496a 6f67 496b  VsZF9uYW1lIjogIk
+00000f20: 5270 6369 4973 4943 4a77 5957 356b 5958  RpciIsICJwYW5kYX
+00000f30: 4e66 6448 6c77 5a53 4936 4943 4a70 626e  NfdHlwZSI6ICJpbn
+00000f40: 517a 4d69 4973 4943 4a75 6457 3177 6556  QzMiIsICJudW1weV
+00000f50: 3930 6558 426c 496a 6f67 496d 6c75 6444  90eXBlIjogImludD
+00000f60: 4d79 4969 7767 496d 316c 6447 466b 5958  MyIiwgIm1ldGFkYX
+00000f70: 5268 496a 6f67 626e 5673 6248 3073 4948  RhIjogbnVsbH0sIH
+00000f80: 7369 626d 4674 5a53 4936 4943 4a4f 6347  sibmFtZSI6ICJOcG
+00000f90: 6c34 4969 7767 496d 5a70 5a57 786b 5832  l4IiwgImZpZWxkX2
+00000fa0: 3568 6257 5569 4f69 4169 546e 4270 6543  5hbWUiOiAiTnBpeC
+00000fb0: 4973 4943 4a77 5957 356b 5958 4e66 6448  IsICJwYW5kYXNfdH
+00000fc0: 6c77 5a53 4936 4943 4a70 626e 517a 4d69  lwZSI6ICJpbnQzMi
+00000fd0: 4973 4943 4a75 6457 3177 6556 3930 6558  IsICJudW1weV90eX
+00000fe0: 426c 496a 6f67 496d 6c75 6444 4d79 4969  BlIjogImludDMyIi
+00000ff0: 7767 496d 316c 6447 466b 5958 5268 496a  wgIm1ldGFkYXRhIj
+00001000: 6f67 626e 5673 6248 3073 4948 7369 626d  ogbnVsbH0sIHsibm
+00001010: 4674 5a53 4936 4943 4a66 6147 6c77 6332  FtZSI6ICJfaGlwc2
+00001020: 4e68 6446 3970 626d 526c 6543 4973 4943  NhdF9pbmRleCIsIC
+00001030: 4a6d 6157 5673 5a46 3975 5957 316c 496a  JmaWVsZF9uYW1lIj
+00001040: 6f67 496c 396f 6158 427a 5932 4630 5832  ogIl9oaXBzY2F0X2
+00001050: 6c75 5a47 5634 4969 7767 496e 4268 626d  luZGV4IiwgInBhbm
+00001060: 5268 6331 3930 6558 426c 496a 6f67 496e  Rhc190eXBlIjogIn
+00001070: 5670 626e 5132 4e43 4973 4943 4a75 6457  VpbnQ2NCIsICJudW
+00001080: 3177 6556 3930 6558 426c 496a 6f67 496e  1weV90eXBlIjogIn
+00001090: 5670 626e 5132 4e43 4973 4943 4a74 5a58  VpbnQ2NCIsICJtZX
+000010a0: 5268 5a47 4630 5953 4936 4947 3531 6247  RhZGF0YSI6IG51bG
+000010b0: 7839 5853 7767 496d 4e79 5a57 4630 6233  x9XSwgImNyZWF0b3
+000010c0: 4969 4f69 4237 496d 7870 596e 4a68 636e  IiOiB7ImxpYnJhcn
+000010d0: 6b69 4f69 4169 6348 6c68 636e 4a76 6479  kiOiAicHlhcnJvdy
+000010e0: 4973 4943 4a32 5a58 4a7a 6157 3975 496a  IsICJ2ZXJzaW9uIj
+000010f0: 6f67 496a 6b75 4d43 3477 496e 3073 4943  ogIjkuMC4wIn0sIC
+00001100: 4a77 5957 356b 5958 4e66 646d 5679 6332  JwYW5kYXNfdmVyc2
+00001110: 6c76 6269 4936 4943 4979 4c6a 4175 4d43  lvbiI6ICIyLjAuMC
+00001120: 4a39 4141 414a 4141 4141 7641 4541 4148  J9AAAJAAAAvAEAAH
+00001130: 6742 4141 424d 4151 4141 4641 4541 414e  gBAABMAQAAFAEAAN
+00001140: 7741 4141 436f 4141 4141 6541 4141 4145  wAAACoAAAAeAAAAE
+00001150: 5141 4141 4145 4141 4141 6550 372f 2f77  QAAAAEAAAAeP7//w
+00001160: 4141 4151 4951 4141 4141 4b41 4141 4141  AAAQIQAAAAKAAAAA
+00001170: 5141 4141 4141 4141 4141 4467 4141 4146  QAAAAAAAAADgAAAF
+00001180: 396f 6158 427a 5932 4630 5832 6c75 5a47  9oaXBzY2F0X2luZG
+00001190: 5634 4141 4141 4141 5941 4341 4145 4141  V4AAAAAAYACAAEAA
+000011a0: 5941 4141 4241 4141 4141 7450 372f 2f77  YAAABAAAAAtP7//w
+000011b0: 4141 4151 4951 4141 4141 4741 4141 4141  AAAQIQAAAAGAAAAA
+000011c0: 5141 4141 4141 4141 4141 4241 4141 4145  QAAAAAAAAABAAAAE
+000011d0: 3577 6158 6741 4141 4141 7150 372f 2f77  5waXgAAAAAqP7//w
+000011e0: 4141 4141 4567 4141 4141 3550 372f 2f77  AAAAEgAAAA5P7//w
+000011f0: 4141 4151 4951 4141 4141 4641 4141 4141  AAAQIQAAAAFAAAAA
+00001200: 5141 4141 4141 4141 4141 4177 4141 4145  QAAAAAAAAAAwAAAE
+00001210: 5270 6367 4455 2f76 2f2f 4141 4141 4153  RpcgDU/v//AAAAAS
+00001220: 4141 4141 4151 2f2f 2f2f 4141 4142 4168  AAAAAQ////AAABAh
+00001230: 4141 4141 4159 4141 4141 4241 4141 4141  AAAAAYAAAABAAAAA
+00001240: 4141 4141 4147 4141 4141 546d 3979 5a47  AAAAAGAAAATm9yZG
+00001250: 5679 4141 4145 2f2f 2f2f 4141 4141 4153  VyAAAE////AAAAAS
+00001260: 4141 4141 4241 2f2f 2f2f 4141 4142 4168  AAAABA////AAABAh
+00001270: 4141 4141 4163 4141 4141 4241 4141 4141  AAAAAcAAAABAAAAA
+00001280: 4141 4141 414a 4141 4141 5a47 566a 5832  AAAAAJAAAAZGVjX2
+00001290: 5679 636d 3979 4141 4141 4f50 2f2f 2f77  Vycm9yAAAAOP///w
+000012a0: 4141 4141 4641 4141 4141 6450 2f2f 2f77  AAAAFAAAAAdP///w
+000012b0: 4141 4151 4951 4141 4141 4841 4141 4141  AAAQIQAAAAHAAAAA
+000012c0: 5141 4141 4141 4141 4141 4341 4141 4148  QAAAAAAAAACAAAAH
+000012d0: 4a68 5832 5679 636d 3979 4141 4141 4147  JhX2Vycm9yAAAAAG
+000012e0: 7a2f 2f2f 3841 4141 4142 5141 4141 414b  z///8AAAABQAAAAK
+000012f0: 6a2f 2f2f 3841 4141 4544 4541 4141 4142  j///8AAAEDEAAAAB
+00001300: 5141 4141 4145 4141 4141 4141 4141 4141  QAAAAEAAAAAAAAAA
+00001310: 4d41 4141 426b 5a57 4d41 3176 2f2f 2f77  MAAABkZWMA1v///w
+00001320: 4141 4167 4451 2f2f 2f2f 4141 4142 4178  AAAgDQ////AAABAx
+00001330: 4141 4141 4163 4141 4141 4241 4141 4141  AAAAAcAAAABAAAAA
+00001340: 4141 4141 4143 4141 4141 636d 4541 4141  AAAAACAAAAcmEAAA
+00001350: 4141 4267 4149 4141 5941 4267 4141 4141  AABgAIAAYABgAAAA
+00001360: 4141 4167 4151 4142 5141 4341 4147 4141  AAAgAQABQACAAGAA
+00001370: 6341 4441 4141 4142 4141 4541 4141 4141  cADAAAABAAEAAAAA
+00001380: 4141 4151 4951 4141 4141 4841 4141 4141  AAAQIQAAAAHAAAAA
+00001390: 5141 4141 4141 4141 4141 4167 4141 4147  QAAAAAAAAAAgAAAG
+000013a0: 6c6b 4141 4149 4141 7741 4341 4148 4141  lkAAAIAAwACAAHAA
+000013b0: 6741 4141 4141 4141 4142 5141 4141 4141  gAAAAAAAABQAAAAA
+000013c0: 3d3d 0018 1f70 6172 7175 6574 2d63 7070  ==...parquet-cpp
+000013d0: 2d61 7272 6f77 2076 6572 7369 6f6e 2039  -arrow version 9
+000013e0: 2e30 2e30 199c 1c00 001c 0000 1c00 001c  .0.0............
+000013f0: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
+00001400: 0000 fe13 0000 5041 5231                 ......PAR1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_46/shard_4.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 00000000: 5041 5231 1504 1540 1538 4c15 0815 0012  PAR1...@.8L.....
-00000010: 0000 2008 2503 0005 0100 290d 083c 3403  .. .%.....)..<4.
-00000020: 0000 0000 0000 3b03 0000 0000 0000 1500  ......;.........
+00000010: 0000 2008 0b03 0005 0100 0d0d 083c 1003  .. ..........<..
+00000020: 0000 0000 0000 1203 0000 0000 0000 1500  ................
 00000030: 1514 1518 2c15 0815 1015 0615 061c 1808  ....,...........
-00000040: 3b03 0000 0000 0000 1808 2503 0000 0000  ;.........%.....
-00000050: 0000 1600 2808 3b03 0000 0000 0000 1808  ....(.;.........
-00000060: 2503 0000 0000 0000 0000 000a 2402 0000  %...........$...
+00000040: 1203 0000 0000 0000 1808 0b03 0000 0000  ................
+00000050: 0000 1600 2808 1203 0000 0000 0000 1808  ....(...........
+00000060: 0b03 0000 0000 0000 0000 000a 2402 0000  ............$...
 00000070: 0008 0102 03e4 0026 ee01 1c15 0419 3510  .......&......5.
 00000080: 0006 1918 0269 6415 0216 0816 ea01 16e6  .....id.........
-00000090: 0126 5c26 081c 1808 3b03 0000 0000 0000  .&\&....;.......
-000000a0: 1808 2503 0000 0000 0000 1600 2808 3b03  ..%.........(.;.
-000000b0: 0000 0000 0000 1808 2503 0000 0000 0000  ........%.......
+00000090: 0126 5c26 081c 1808 1203 0000 0000 0000  .&\&............
+000000a0: 1808 0b03 0000 0000 0000 1600 2808 1203  ............(...
+000000b0: 0000 0000 0000 1808 0b03 0000 0000 0000  ................
 000000c0: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
 000000d0: 0000 0015 0415 4015 3a4c 1508 1500 1200  ......@.:L......
-000000e0: 0020 0000 0101 0898 7240 0107 0800 b871  . ......r@.....q
-000000f0: 0908 28e8 7140 0000 0000 0068 7340 1500  ..(.q@.....hs@..
+000000e0: 0020 0000 0101 08b8 7540 0107 0800 a874  . ......u@.....t
+000000f0: 0908 2828 7540 0000 0000 0008 7540 1500  ..((u@......u@..
 00000100: 1514 1518 2c15 0815 1015 0615 061c 1808  ....,...........
-00000110: 0000 0000 0068 7340 1808 0000 0000 00b8  .....hs@........
-00000120: 7140 1600 2808 0000 0000 0068 7340 1808  q@..(......hs@..
-00000130: 0000 0000 00b8 7140 0000 000a 2402 0000  ......q@....$...
+00000110: 0000 0000 00b8 7540 1808 0000 0000 00a8  ......u@........
+00000120: 7440 1600 2808 0000 0000 00b8 7540 1808  t@..(.......u@..
+00000130: 0000 0000 00a8 7440 0000 000a 2402 0000  ......t@....$...
 00000140: 0008 0102 03e4 0026 8e05 1c15 0a19 3510  .......&......5.
 00000150: 0006 1918 0272 6115 0216 0816 ea01 16e8  .....ra.........
-00000160: 0126 fc03 26a6 031c 1808 0000 0000 0068  .&..&..........h
-00000170: 7340 1808 0000 0000 00b8 7140 1600 2808  s@........q@..(.
-00000180: 0000 0000 0068 7340 1808 0000 0000 00b8  .....hs@........
-00000190: 7140 0019 2c15 0415 0015 0200 1500 1510  q@..,...........
+00000160: 0126 fc03 26a6 031c 1808 0000 0000 00b8  .&..&...........
+00000170: 7540 1808 0000 0000 00a8 7440 1600 2808  u@........t@..(.
+00000180: 0000 0000 00b8 7540 1808 0000 0000 00a8  ......u@........
+00000190: 7440 0019 2c15 0415 0015 0200 1500 1510  t@..,...........
 000001a0: 1502 0000 0015 0415 4015 384c 1508 1500  ........@.8L....
-000001b0: 1200 0020 0000 0101 0840 4ac0 0107 0800  ... .....@J.....
-000001c0: 4041 0d08 2447 c000 0000 0000 4044 c015  @A..$G......@D..
+000001b0: 1200 0020 0000 0101 0880 3dc0 0107 0800  ... ......=.....
+000001c0: 4047 0d08 2444 c000 0000 0000 c040 c015  @G..$D.......@..
 000001d0: 0015 1415 182c 1508 1510 1506 1506 1c18  .....,..........
-000001e0: 0800 0000 0000 4041 c018 0800 0000 0000  ......@A........
-000001f0: 404a c016 0028 0800 0000 0000 4041 c018  @J...(......@A..
-00000200: 0800 0000 0000 404a c000 0000 0a24 0200  ......@J.....$..
+000001e0: 0800 0000 0000 803d c018 0800 0000 0000  .......=........
+000001f0: 4047 c016 0028 0800 0000 0000 803d c018  @G...(.......=..
+00000200: 0800 0000 0000 4047 c000 0000 0a24 0200  ......@G.....$..
 00000210: 0000 0801 0203 e400 26b0 081c 150a 1935  ........&......5
 00000220: 1000 0619 1803 6465 6315 0216 0816 ea01  ......dec.......
 00000230: 16e6 0126 9e07 26ca 061c 1808 0000 0000  ...&..&.........
-00000240: 0040 41c0 1808 0000 0000 0040 4ac0 1600  .@A........@J...
-00000250: 2808 0000 0000 0040 41c0 1808 0000 0000  (......@A.......
-00000260: 0040 4ac0 0019 2c15 0415 0015 0200 1500  .@J...,.........
+00000240: 0080 3dc0 1808 0000 0000 0040 47c0 1600  ..=........@G...
+00000250: 2808 0000 0000 0080 3dc0 1808 0000 0000  (.......=.......
+00000260: 0040 47c0 0019 2c15 0415 0015 0200 1500  .@G...,.........
 00000270: 1510 1502 0000 0015 0415 1015 144c 1502  .............L..
 00000280: 1500 1200 0008 1c00 0000 0000 0000 0015  ................
 00000290: 0015 1215 162c 1508 1510 1506 1506 1c18  .....,..........
 000002a0: 0800 0000 0000 0000 0018 0800 0000 0000  ................
 000002b0: 0000 0016 0028 0800 0000 0000 0000 0018  .....(..........
 000002c0: 0800 0000 0000 0000 0000 0000 0920 0200  ............. ..
 000002d0: 0000 0801 0108 0026 ae0b 1c15 0419 3510  .......&......5.
@@ -58,246 +58,181 @@
 00000390: 0920 0200 0000 0801 0108 0026 b60e 1c15  . .........&....
 000003a0: 0419 3510 0006 1918 0964 6563 5f65 7272  ..5......dec_err
 000003b0: 6f72 1502 1608 16b8 0116 c001 26a6 0d26  or..........&..&
 000003c0: f60c 1c18 0800 0000 0000 0000 0018 0800  ................
 000003d0: 0000 0000 0000 0016 0028 0800 0000 0000  .........(......
 000003e0: 0000 0018 0800 0000 0000 0000 0000 192c  ...............,
 000003f0: 1504 1500 1502 0015 0015 1015 0200 0000  ................
-00000400: 1504 1540 1538 4c15 0815 0012 0000 2004  ...@.8L....... .
-00000410: 0200 0901 0006 0907 4000 1100 0000 0000  ........@.......
-00000420: 0000 1800 0000 0000 0000 1500 1514 1518  ................
-00000430: 2c15 0815 1015 0615 061c 1808 1800 0000  ,...............
-00000440: 0000 0000 1808 0200 0000 0000 0000 1600  ................
-00000450: 2808 1800 0000 0000 0000 1808 0200 0000  (...............
-00000460: 0000 0000 0000 000a 2402 0000 0008 0102  ........$.......
-00000470: 03e4 0026 e611 1c15 0419 3510 0006 1918  ...&......5.....
-00000480: 115f 5f69 6e64 6578 5f6c 6576 656c 5f30  .__index_level_0
-00000490: 5f5f 1502 1608 16ea 0116 e601 26d4 1026  __..........&..&
-000004a0: 8010 1c18 0818 0000 0000 0000 0018 0802  ................
-000004b0: 0000 0000 0000 0016 0028 0818 0000 0000  .........(......
-000004c0: 0000 0018 0802 0000 0000 0000 0000 192c  ...............,
-000004d0: 1504 1500 1502 0015 0015 1015 0200 0000  ................
-000004e0: 1504 197c 3500 1806 7363 6865 6d61 150c  ...|5...schema..
-000004f0: 0015 0425 0218 0269 6400 150a 2502 1802  ...%...id...%...
-00000500: 7261 0015 0a25 0218 0364 6563 0015 0425  ra...%...dec...%
-00000510: 0218 0872 615f 6572 726f 7200 1504 2502  ...ra_error...%.
-00000520: 1809 6465 635f 6572 726f 7200 1504 2502  ..dec_error...%.
-00000530: 1811 5f5f 696e 6465 785f 6c65 7665 6c5f  ..__index_level_
-00000540: 305f 5f00 1608 191c 196c 26ee 011c 1504  0__......l&.....
-00000550: 1935 1000 0619 1802 6964 1502 1608 16ea  .5......id......
-00000560: 0116 e601 265c 2608 1c18 083b 0300 0000  ....&\&....;....
-00000570: 0000 0018 0825 0300 0000 0000 0016 0028  .....%.........(
-00000580: 083b 0300 0000 0000 0018 0825 0300 0000  .;.........%....
-00000590: 0000 0000 192c 1504 1500 1502 0015 0015  .....,..........
-000005a0: 1015 0200 0000 268e 051c 150a 1935 1000  ......&......5..
-000005b0: 0619 1802 7261 1502 1608 16ea 0116 e801  ....ra..........
-000005c0: 26fc 0326 a603 1c18 0800 0000 0000 6873  &..&..........hs
-000005d0: 4018 0800 0000 0000 b871 4016 0028 0800  @........q@..(..
-000005e0: 0000 0000 6873 4018 0800 0000 0000 b871  ....hs@........q
-000005f0: 4000 192c 1504 1500 1502 0015 0015 1015  @..,............
-00000600: 0200 0000 26b0 081c 150a 1935 1000 0619  ....&......5....
-00000610: 1803 6465 6315 0216 0816 ea01 16e6 0126  ..dec..........&
-00000620: 9e07 26ca 061c 1808 0000 0000 0040 41c0  ..&..........@A.
-00000630: 1808 0000 0000 0040 4ac0 1600 2808 0000  .......@J...(...
-00000640: 0000 0040 41c0 1808 0000 0000 0040 4ac0  ...@A........@J.
-00000650: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
-00000660: 0000 0026 ae0b 1c15 0419 3510 0006 1918  ...&......5.....
-00000670: 0872 615f 6572 726f 7215 0216 0816 b801  .ra_error.......
-00000680: 16c0 0126 9e0a 26ee 091c 1808 0000 0000  ...&..&.........
-00000690: 0000 0000 1808 0000 0000 0000 0000 1600  ................
-000006a0: 2808 0000 0000 0000 0000 1808 0000 0000  (...............
-000006b0: 0000 0000 0019 2c15 0415 0015 0200 1500  ......,.........
-000006c0: 1510 1502 0000 0026 b60e 1c15 0419 3510  .......&......5.
-000006d0: 0006 1918 0964 6563 5f65 7272 6f72 1502  .....dec_error..
-000006e0: 1608 16b8 0116 c001 26a6 0d26 f60c 1c18  ........&..&....
-000006f0: 0800 0000 0000 0000 0018 0800 0000 0000  ................
-00000700: 0000 0016 0028 0800 0000 0000 0000 0018  .....(..........
-00000710: 0800 0000 0000 0000 0000 192c 1504 1500  ...........,....
-00000720: 1502 0015 0015 1015 0200 0000 26e6 111c  ............&...
-00000730: 1504 1935 1000 0619 1811 5f5f 696e 6465  ...5......__inde
-00000740: 785f 6c65 7665 6c5f 305f 5f15 0216 0816  x_level_0__.....
-00000750: ea01 16e6 0126 d410 2680 101c 1808 1800  .....&..&.......
-00000760: 0000 0000 0000 1808 0200 0000 0000 0000  ................
-00000770: 1600 2808 1800 0000 0000 0000 1808 0200  ..(.............
-00000780: 0000 0000 0000 0019 2c15 0415 0015 0200  ........,.......
-00000790: 1500 1510 1502 0000 0016 980a 1608 2608  ..............&.
-000007a0: 169a 0a14 0000 192c 1806 7061 6e64 6173  .......,..pandas
-000007b0: 18a5 077b 2269 6e64 6578 5f63 6f6c 756d  ...{"index_colum
-000007c0: 6e73 223a 205b 225f 5f69 6e64 6578 5f6c  ns": ["__index_l
-000007d0: 6576 656c 5f30 5f5f 225d 2c20 2263 6f6c  evel_0__"], "col
-000007e0: 756d 6e5f 696e 6465 7865 7322 3a20 5b7b  umn_indexes": [{
-000007f0: 226e 616d 6522 3a20 6e75 6c6c 2c20 2266  "name": null, "f
-00000800: 6965 6c64 5f6e 616d 6522 3a20 6e75 6c6c  ield_name": null
-00000810: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
-00000820: 2022 756e 6963 6f64 6522 2c20 226e 756d   "unicode", "num
-00000830: 7079 5f74 7970 6522 3a20 226f 626a 6563  py_type": "objec
-00000840: 7422 2c20 226d 6574 6164 6174 6122 3a20  t", "metadata": 
-00000850: 7b22 656e 636f 6469 6e67 223a 2022 5554  {"encoding": "UT
-00000860: 462d 3822 7d7d 5d2c 2022 636f 6c75 6d6e  F-8"}}], "column
-00000870: 7322 3a20 5b7b 226e 616d 6522 3a20 2269  s": [{"name": "i
-00000880: 6422 2c20 2266 6965 6c64 5f6e 616d 6522  d", "field_name"
-00000890: 3a20 2269 6422 2c20 2270 616e 6461 735f  : "id", "pandas_
-000008a0: 7479 7065 223a 2022 696e 7436 3422 2c20  type": "int64", 
-000008b0: 226e 756d 7079 5f74 7970 6522 3a20 2269  "numpy_type": "i
-000008c0: 6e74 3634 222c 2022 6d65 7461 6461 7461  nt64", "metadata
-000008d0: 223a 206e 756c 6c7d 2c20 7b22 6e61 6d65  ": null}, {"name
-000008e0: 223a 2022 7261 222c 2022 6669 656c 645f  ": "ra", "field_
-000008f0: 6e61 6d65 223a 2022 7261 222c 2022 7061  name": "ra", "pa
-00000900: 6e64 6173 5f74 7970 6522 3a20 2266 6c6f  ndas_type": "flo
-00000910: 6174 3634 222c 2022 6e75 6d70 795f 7479  at64", "numpy_ty
-00000920: 7065 223a 2022 666c 6f61 7436 3422 2c20  pe": "float64", 
-00000930: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
-00000940: 7d2c 207b 226e 616d 6522 3a20 2264 6563  }, {"name": "dec
-00000950: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
-00000960: 2022 6465 6322 2c20 2270 616e 6461 735f   "dec", "pandas_
-00000970: 7479 7065 223a 2022 666c 6f61 7436 3422  type": "float64"
-00000980: 2c20 226e 756d 7079 5f74 7970 6522 3a20  , "numpy_type": 
-00000990: 2266 6c6f 6174 3634 222c 2022 6d65 7461  "float64", "meta
-000009a0: 6461 7461 223a 206e 756c 6c7d 2c20 7b22  data": null}, {"
-000009b0: 6e61 6d65 223a 2022 7261 5f65 7272 6f72  name": "ra_error
-000009c0: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
-000009d0: 2022 7261 5f65 7272 6f72 222c 2022 7061   "ra_error", "pa
-000009e0: 6e64 6173 5f74 7970 6522 3a20 2269 6e74  ndas_type": "int
-000009f0: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
-00000a00: 223a 2022 696e 7436 3422 2c20 226d 6574  ": "int64", "met
-00000a10: 6164 6174 6122 3a20 6e75 6c6c 7d2c 207b  adata": null}, {
-00000a20: 226e 616d 6522 3a20 2264 6563 5f65 7272  "name": "dec_err
-00000a30: 6f72 222c 2022 6669 656c 645f 6e61 6d65  or", "field_name
-00000a40: 223a 2022 6465 635f 6572 726f 7222 2c20  ": "dec_error", 
-00000a50: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
-00000a60: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
-00000a70: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
-00000a80: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
-00000a90: 2c20 7b22 6e61 6d65 223a 206e 756c 6c2c  , {"name": null,
-00000aa0: 2022 6669 656c 645f 6e61 6d65 223a 2022   "field_name": "
-00000ab0: 5f5f 696e 6465 785f 6c65 7665 6c5f 305f  __index_level_0_
-00000ac0: 5f22 2c20 2270 616e 6461 735f 7479 7065  _", "pandas_type
-00000ad0: 223a 2022 696e 7436 3422 2c20 226e 756d  ": "int64", "num
-00000ae0: 7079 5f74 7970 6522 3a20 2269 6e74 3634  py_type": "int64
-00000af0: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
-00000b00: 756c 6c7d 5d2c 2022 6372 6561 746f 7222  ull}], "creator"
-00000b10: 3a20 7b22 6c69 6272 6172 7922 3a20 2270  : {"library": "p
-00000b20: 7961 7272 6f77 222c 2022 7665 7273 696f  yarrow", "versio
-00000b30: 6e22 3a20 2239 2e30 2e30 227d 2c20 2270  n": "9.0.0"}, "p
-00000b40: 616e 6461 735f 7665 7273 696f 6e22 3a20  andas_version": 
-00000b50: 2231 2e33 2e35 227d 0018 0c41 5252 4f57  "1.3.5"}...ARROW
-00000b60: 3a73 6368 656d 6118 c00e 2f2f 2f2f 2f32  :schema.../////2
-00000b70: 6746 4141 4151 4141 4141 4141 414b 4141  gFAAAQAAAAAAAKAA
-00000b80: 3441 4267 4146 4141 6741 4367 4141 4141  4ABgAFAAgACgAAAA
-00000b90: 4142 4241 4151 4141 4141 4141 414b 4141  ABBAAQAAAAAAAKAA
-00000ba0: 7741 4141 4145 4141 6741 4367 4141 414e  wAAAAEAAgACgAAAN
-00000bb0: 7744 4141 4145 4141 4141 4151 4141 4141  wDAAAEAAAAAQAAAA
-00000bc0: 7741 4141 4149 4141 7741 4241 4149 4141  wAAAAIAAwABAAIAA
-00000bd0: 6741 4141 4149 4141 4141 4541 4141 4141  gAAAAIAAAAEAAAAA
-00000be0: 5941 4141 4277 5957 356b 5958 4d41 414b  YAAABwYW5kYXMAAK
-00000bf0: 5544 4141 4237 496d 6c75 5a47 5634 5832  UDAAB7ImluZGV4X2
-00000c00: 4e76 6248 5674 626e 4d69 4f69 4262 496c  NvbHVtbnMiOiBbIl
-00000c10: 3966 6157 356b 5a58 6866 6247 5632 5a57  9faW5kZXhfbGV2ZW
-00000c20: 7866 4d46 3966 496c 3073 4943 4a6a 6232  xfMF9fIl0sICJjb2
-00000c30: 7831 6257 3566 6157 356b 5a58 686c 6379  x1bW5faW5kZXhlcy
-00000c40: 4936 4946 7437 496d 3568 6257 5569 4f69  I6IFt7Im5hbWUiOi
-00000c50: 4275 6457 7873 4c43 4169 5a6d 6c6c 6247  BudWxsLCAiZmllbG
-00000c60: 5266 626d 4674 5a53 4936 4947 3531 6247  RfbmFtZSI6IG51bG
-00000c70: 7773 4943 4a77 5957 356b 5958 4e66 6448  wsICJwYW5kYXNfdH
-00000c80: 6c77 5a53 4936 4943 4a31 626d 6c6a 6232  lwZSI6ICJ1bmljb2
-00000c90: 526c 4969 7767 496d 3531 6258 4235 5833  RlIiwgIm51bXB5X3
-00000ca0: 5235 6347 5569 4f69 4169 6232 4a71 5a57  R5cGUiOiAib2JqZW
-00000cb0: 4e30 4969 7767 496d 316c 6447 466b 5958  N0IiwgIm1ldGFkYX
-00000cc0: 5268 496a 6f67 6579 4a6c 626d 4e76 5a47  RhIjogeyJlbmNvZG
-00000cd0: 6c75 5a79 4936 4943 4a56 5645 5974 4f43  luZyI6ICJVVEYtOC
-00000ce0: 4a39 6656 3073 4943 4a6a 6232 7831 6257  J9fV0sICJjb2x1bW
-00000cf0: 357a 496a 6f67 5733 7369 626d 4674 5a53  5zIjogW3sibmFtZS
-00000d00: 4936 4943 4a70 5a43 4973 4943 4a6d 6157  I6ICJpZCIsICJmaW
-00000d10: 5673 5a46 3975 5957 316c 496a 6f67 496d  VsZF9uYW1lIjogIm
-00000d20: 6c6b 4969 7767 496e 4268 626d 5268 6331  lkIiwgInBhbmRhc1
-00000d30: 3930 6558 426c 496a 6f67 496d 6c75 6444  90eXBlIjogImludD
-00000d40: 5930 4969 7767 496d 3531 6258 4235 5833  Y0IiwgIm51bXB5X3
-00000d50: 5235 6347 5569 4f69 4169 6157 3530 4e6a  R5cGUiOiAiaW50Nj
-00000d60: 5169 4c43 4169 6257 5630 5957 5268 6447  QiLCAibWV0YWRhdG
-00000d70: 4569 4f69 4275 6457 7873 6653 7767 6579  EiOiBudWxsfSwgey
-00000d80: 4a75 5957 316c 496a 6f67 496e 4a68 4969  JuYW1lIjogInJhIi
-00000d90: 7767 496d 5a70 5a57 786b 5832 3568 6257  wgImZpZWxkX25hbW
-00000da0: 5569 4f69 4169 636d 4569 4c43 4169 6347  UiOiAicmEiLCAicG
-00000db0: 4675 5a47 467a 5833 5235 6347 5569 4f69  FuZGFzX3R5cGUiOi
-00000dc0: 4169 5a6d 7876 5958 5132 4e43 4973 4943  AiZmxvYXQ2NCIsIC
-00000dd0: 4a75 6457 3177 6556 3930 6558 426c 496a  JudW1weV90eXBlIj
-00000de0: 6f67 496d 5a73 6232 4630 4e6a 5169 4c43  ogImZsb2F0NjQiLC
-00000df0: 4169 6257 5630 5957 5268 6447 4569 4f69  AibWV0YWRhdGEiOi
-00000e00: 4275 6457 7873 6653 7767 6579 4a75 5957  BudWxsfSwgeyJuYW
-00000e10: 316c 496a 6f67 496d 526c 5979 4973 4943  1lIjogImRlYyIsIC
-00000e20: 4a6d 6157 5673 5a46 3975 5957 316c 496a  JmaWVsZF9uYW1lIj
-00000e30: 6f67 496d 526c 5979 4973 4943 4a77 5957  ogImRlYyIsICJwYW
-00000e40: 356b 5958 4e66 6448 6c77 5a53 4936 4943  5kYXNfdHlwZSI6IC
-00000e50: 4a6d 6247 3968 6444 5930 4969 7767 496d  JmbG9hdDY0IiwgIm
-00000e60: 3531 6258 4235 5833 5235 6347 5569 4f69  51bXB5X3R5cGUiOi
-00000e70: 4169 5a6d 7876 5958 5132 4e43 4973 4943  AiZmxvYXQ2NCIsIC
-00000e80: 4a74 5a58 5268 5a47 4630 5953 4936 4947  JtZXRhZGF0YSI6IG
-00000e90: 3531 6247 7839 4c43 4237 496d 3568 6257  51bGx9LCB7Im5hbW
-00000ea0: 5569 4f69 4169 636d 4666 5a58 4a79 6233  UiOiAicmFfZXJyb3
-00000eb0: 4969 4c43 4169 5a6d 6c6c 6247 5266 626d  IiLCAiZmllbGRfbm
-00000ec0: 4674 5a53 4936 4943 4a79 5956 396c 636e  FtZSI6ICJyYV9lcn
-00000ed0: 4a76 6369 4973 4943 4a77 5957 356b 5958  JvciIsICJwYW5kYX
-00000ee0: 4e66 6448 6c77 5a53 4936 4943 4a70 626e  NfdHlwZSI6ICJpbn
-00000ef0: 5132 4e43 4973 4943 4a75 6457 3177 6556  Q2NCIsICJudW1weV
-00000f00: 3930 6558 426c 496a 6f67 496d 6c75 6444  90eXBlIjogImludD
-00000f10: 5930 4969 7767 496d 316c 6447 466b 5958  Y0IiwgIm1ldGFkYX
-00000f20: 5268 496a 6f67 626e 5673 6248 3073 4948  RhIjogbnVsbH0sIH
-00000f30: 7369 626d 4674 5a53 4936 4943 4a6b 5a57  sibmFtZSI6ICJkZW
-00000f40: 4e66 5a58 4a79 6233 4969 4c43 4169 5a6d  NfZXJyb3IiLCAiZm
-00000f50: 6c6c 6247 5266 626d 4674 5a53 4936 4943  llbGRfbmFtZSI6IC
-00000f60: 4a6b 5a57 4e66 5a58 4a79 6233 4969 4c43  JkZWNfZXJyb3IiLC
-00000f70: 4169 6347 4675 5a47 467a 5833 5235 6347  AicGFuZGFzX3R5cG
-00000f80: 5569 4f69 4169 6157 3530 4e6a 5169 4c43  UiOiAiaW50NjQiLC
-00000f90: 4169 626e 5674 6348 6c66 6448 6c77 5a53  AibnVtcHlfdHlwZS
-00000fa0: 4936 4943 4a70 626e 5132 4e43 4973 4943  I6ICJpbnQ2NCIsIC
-00000fb0: 4a74 5a58 5268 5a47 4630 5953 4936 4947  JtZXRhZGF0YSI6IG
-00000fc0: 3531 6247 7839 4c43 4237 496d 3568 6257  51bGx9LCB7Im5hbW
-00000fd0: 5569 4f69 4275 6457 7873 4c43 4169 5a6d  UiOiBudWxsLCAiZm
-00000fe0: 6c6c 6247 5266 626d 4674 5a53 4936 4943  llbGRfbmFtZSI6IC
-00000ff0: 4a66 5832 6c75 5a47 5634 5832 786c 646d  JfX2luZGV4X2xldm
-00001000: 5673 587a 4266 5879 4973 4943 4a77 5957  VsXzBfXyIsICJwYW
-00001010: 356b 5958 4e66 6448 6c77 5a53 4936 4943  5kYXNfdHlwZSI6IC
-00001020: 4a70 626e 5132 4e43 4973 4943 4a75 6457  JpbnQ2NCIsICJudW
-00001030: 3177 6556 3930 6558 426c 496a 6f67 496d  1weV90eXBlIjogIm
-00001040: 6c75 6444 5930 4969 7767 496d 316c 6447  ludDY0IiwgIm1ldG
-00001050: 466b 5958 5268 496a 6f67 626e 5673 6248  FkYXRhIjogbnVsbH
-00001060: 3164 4c43 4169 5933 4a6c 5958 5276 6369  1dLCAiY3JlYXRvci
-00001070: 4936 4948 7369 6247 6c69 636d 4679 6553  I6IHsibGlicmFyeS
-00001080: 4936 4943 4a77 6557 4679 636d 3933 4969  I6ICJweWFycm93Ii
-00001090: 7767 496e 5a6c 636e 4e70 6232 3469 4f69  wgInZlcnNpb24iOi
-000010a0: 4169 4f53 3477 4c6a 4169 6653 7767 496e  AiOS4wLjAifSwgIn
-000010b0: 4268 626d 5268 6331 3932 5a58 4a7a 6157  BhbmRhc192ZXJzaW
-000010c0: 3975 496a 6f67 496a 4575 4d79 3431 496e  9uIjogIjEuMy41In
-000010d0: 3041 4141 4147 4141 4141 4a41 4541 414f  0AAAAGAAAAJAEAAO
-000010e0: 4141 4141 4330 4141 4141 6641 4141 4145  AAAAC0AAAAfAAAAE
-000010f0: 5141 4141 4145 4141 4141 4250 2f2f 2f77  QAAAAEAAAABP///w
-00001100: 4141 4151 4951 4141 4141 4a41 4141 4141  AAAQIQAAAAJAAAAA
-00001110: 5141 4141 4141 4141 4141 4551 4141 4146  QAAAAAAAAAEQAAAF
-00001120: 3966 6157 356b 5a58 6866 6247 5632 5a57  9faW5kZXhfbGV2ZW
-00001130: 7866 4d46 3966 4141 4141 4250 2f2f 2f77  xfMF9fAAAABP///w
-00001140: 4141 4141 4641 4141 4141 5150 2f2f 2f77  AAAAFAAAAAQP///w
-00001150: 4141 4151 4951 4141 4141 4841 4141 4141  AAAQIQAAAAHAAAAA
-00001160: 5141 4141 4141 4141 4141 4351 4141 4147  QAAAAAAAAACQAAAG
-00001170: 526c 5931 396c 636e 4a76 6367 4141 4144  RlY19lcnJvcgAAAD
-00001180: 6a2f 2f2f 3841 4141 4142 5141 4141 4148  j///8AAAABQAAAAH
-00001190: 542f 2f2f 3841 4141 4543 4541 4141 4142  T///8AAAECEAAAAB
-000011a0: 7741 4141 4145 4141 4141 4141 4141 4141  wAAAAEAAAAAAAAAA
-000011b0: 6741 4141 4279 5956 396c 636e 4a76 6367  gAAAByYV9lcnJvcg
-000011c0: 4141 4141 4273 2f2f 2f2f 4141 4141 4155  AAAABs////AAAAAU
-000011d0: 4141 4141 436f 2f2f 2f2f 4141 4142 4178  AAAACo////AAABAx
-000011e0: 4141 4141 4155 4141 4141 4241 4141 4141  AAAAAUAAAABAAAAA
-000011f0: 4141 4141 4144 4141 4141 5a47 566a 414e  AAAAADAAAAZGVjAN
-00001200: 622f 2f2f 3841 4141 4941 3050 2f2f 2f77  b///8AAAIA0P///w
-00001210: 4141 4151 4d51 4141 4141 4841 4141 4141  AAAQMQAAAAHAAAAA
-00001220: 5141 4141 4141 4141 4141 4167 4141 4148  QAAAAAAAAAAgAAAH
-00001230: 4a68 4141 4141 4141 5941 4341 4147 4141  JhAAAAAAYACAAGAA
-00001240: 5941 4141 4141 4141 4941 4541 4155 4141  YAAAAAAAIAEAAUAA
-00001250: 6741 4267 4148 4141 7741 4141 4151 4142  gABgAHAAwAAAAQAB
-00001260: 4141 4141 4141 4141 4543 4541 4141 4142  AAAAAAAAECEAAAAB
-00001270: 7741 4141 4145 4141 4141 4141 4141 4141  wAAAAEAAAAAAAAAA
-00001280: 4941 4141 4270 5a41 4141 4341 414d 4141  IAAABpZAAACAAMAA
-00001290: 6741 4277 4149 4141 4141 4141 4141 4155  gABwAIAAAAAAAAAU
-000012a0: 4141 4141 4141 4141 4141 0018 1f70 6172  AAAAAAAAAA...par
-000012b0: 7175 6574 2d63 7070 2d61 7272 6f77 2076  quet-cpp-arrow v
-000012c0: 6572 7369 6f6e 2039 2e30 2e30 196c 1c00  ersion 9.0.0.l..
-000012d0: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
-000012e0: 0001 0e00 0050 4152 31                   .....PAR1
+00000400: 1504 196c 3500 1806 7363 6865 6d61 150a  ...l5...schema..
+00000410: 0015 0425 0218 0269 6400 150a 2502 1802  ...%...id...%...
+00000420: 7261 0015 0a25 0218 0364 6563 0015 0425  ra...%...dec...%
+00000430: 0218 0872 615f 6572 726f 7200 1504 2502  ...ra_error...%.
+00000440: 1809 6465 635f 6572 726f 7200 1608 191c  ..dec_error.....
+00000450: 195c 26ee 011c 1504 1935 1000 0619 1802  .\&......5......
+00000460: 6964 1502 1608 16ea 0116 e601 265c 2608  id..........&\&.
+00000470: 1c18 0812 0300 0000 0000 0018 080b 0300  ................
+00000480: 0000 0000 0016 0028 0812 0300 0000 0000  .......(........
+00000490: 0018 080b 0300 0000 0000 0000 192c 1504  .............,..
+000004a0: 1500 1502 0015 0015 1015 0200 0000 268e  ..............&.
+000004b0: 051c 150a 1935 1000 0619 1802 7261 1502  .....5......ra..
+000004c0: 1608 16ea 0116 e801 26fc 0326 a603 1c18  ........&..&....
+000004d0: 0800 0000 0000 b875 4018 0800 0000 0000  .......u@.......
+000004e0: a874 4016 0028 0800 0000 0000 b875 4018  .t@..(.......u@.
+000004f0: 0800 0000 0000 a874 4000 192c 1504 1500  .......t@..,....
+00000500: 1502 0015 0015 1015 0200 0000 26b0 081c  ............&...
+00000510: 150a 1935 1000 0619 1803 6465 6315 0216  ...5......dec...
+00000520: 0816 ea01 16e6 0126 9e07 26ca 061c 1808  .......&..&.....
+00000530: 0000 0000 0080 3dc0 1808 0000 0000 0040  ......=........@
+00000540: 47c0 1600 2808 0000 0000 0080 3dc0 1808  G...(.......=...
+00000550: 0000 0000 0040 47c0 0019 2c15 0415 0015  .....@G...,.....
+00000560: 0200 1500 1510 1502 0000 0026 ae0b 1c15  ...........&....
+00000570: 0419 3510 0006 1918 0872 615f 6572 726f  ..5......ra_erro
+00000580: 7215 0216 0816 b801 16c0 0126 9e0a 26ee  r..........&..&.
+00000590: 091c 1808 0000 0000 0000 0000 1808 0000  ................
+000005a0: 0000 0000 0000 1600 2808 0000 0000 0000  ........(.......
+000005b0: 0000 1808 0000 0000 0000 0000 0019 2c15  ..............,.
+000005c0: 0415 0015 0200 1500 1510 1502 0000 0026  ...............&
+000005d0: b60e 1c15 0419 3510 0006 1918 0964 6563  ......5......dec
+000005e0: 5f65 7272 6f72 1502 1608 16b8 0116 c001  _error..........
+000005f0: 26a6 0d26 f60c 1c18 0800 0000 0000 0000  &..&............
+00000600: 0018 0800 0000 0000 0000 0016 0028 0800  .............(..
+00000610: 0000 0000 0000 0018 0800 0000 0000 0000  ................
+00000620: 0000 192c 1504 1500 1502 0015 0015 1015  ...,............
+00000630: 0200 0000 16ae 0816 0826 0816 b408 1400  .........&......
+00000640: 0019 2c18 0670 616e 6461 7318 a705 7b22  ..,..pandas...{"
+00000650: 696e 6465 785f 636f 6c75 6d6e 7322 3a20  index_columns": 
+00000660: 5b5d 2c20 2263 6f6c 756d 6e5f 696e 6465  [], "column_inde
+00000670: 7865 7322 3a20 5b5d 2c20 2263 6f6c 756d  xes": [], "colum
+00000680: 6e73 223a 205b 7b22 6e61 6d65 223a 2022  ns": [{"name": "
+00000690: 6964 222c 2022 6669 656c 645f 6e61 6d65  id", "field_name
+000006a0: 223a 2022 6964 222c 2022 7061 6e64 6173  ": "id", "pandas
+000006b0: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
+000006c0: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
+000006d0: 696e 7436 3422 2c20 226d 6574 6164 6174  int64", "metadat
+000006e0: 6122 3a20 6e75 6c6c 7d2c 207b 226e 616d  a": null}, {"nam
+000006f0: 6522 3a20 2272 6122 2c20 2266 6965 6c64  e": "ra", "field
+00000700: 5f6e 616d 6522 3a20 2272 6122 2c20 2270  _name": "ra", "p
+00000710: 616e 6461 735f 7479 7065 223a 2022 666c  andas_type": "fl
+00000720: 6f61 7436 3422 2c20 226e 756d 7079 5f74  oat64", "numpy_t
+00000730: 7970 6522 3a20 2266 6c6f 6174 3634 222c  ype": "float64",
+00000740: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
+00000750: 6c7d 2c20 7b22 6e61 6d65 223a 2022 6465  l}, {"name": "de
+00000760: 6322 2c20 2266 6965 6c64 5f6e 616d 6522  c", "field_name"
+00000770: 3a20 2264 6563 222c 2022 7061 6e64 6173  : "dec", "pandas
+00000780: 5f74 7970 6522 3a20 2266 6c6f 6174 3634  _type": "float64
+00000790: 222c 2022 6e75 6d70 795f 7479 7065 223a  ", "numpy_type":
+000007a0: 2022 666c 6f61 7436 3422 2c20 226d 6574   "float64", "met
+000007b0: 6164 6174 6122 3a20 6e75 6c6c 7d2c 207b  adata": null}, {
+000007c0: 226e 616d 6522 3a20 2272 615f 6572 726f  "name": "ra_erro
+000007d0: 7222 2c20 2266 6965 6c64 5f6e 616d 6522  r", "field_name"
+000007e0: 3a20 2272 615f 6572 726f 7222 2c20 2270  : "ra_error", "p
+000007f0: 616e 6461 735f 7479 7065 223a 2022 696e  andas_type": "in
+00000800: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
+00000810: 6522 3a20 2269 6e74 3634 222c 2022 6d65  e": "int64", "me
+00000820: 7461 6461 7461 223a 206e 756c 6c7d 2c20  tadata": null}, 
+00000830: 7b22 6e61 6d65 223a 2022 6465 635f 6572  {"name": "dec_er
+00000840: 726f 7222 2c20 2266 6965 6c64 5f6e 616d  ror", "field_nam
+00000850: 6522 3a20 2264 6563 5f65 7272 6f72 222c  e": "dec_error",
+00000860: 2022 7061 6e64 6173 5f74 7970 6522 3a20   "pandas_type": 
+00000870: 2269 6e74 3634 222c 2022 6e75 6d70 795f  "int64", "numpy_
+00000880: 7479 7065 223a 2022 696e 7436 3422 2c20  type": "int64", 
+00000890: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
+000008a0: 7d5d 2c20 2263 7265 6174 6f72 223a 207b  }], "creator": {
+000008b0: 226c 6962 7261 7279 223a 2022 7079 6172  "library": "pyar
+000008c0: 726f 7722 2c20 2276 6572 7369 6f6e 223a  row", "version":
+000008d0: 2022 392e 302e 3022 7d2c 2022 7061 6e64   "9.0.0"}, "pand
+000008e0: 6173 5f76 6572 7369 6f6e 223a 2022 322e  as_version": "2.
+000008f0: 302e 3022 7d00 180c 4152 524f 573a 7363  0.0"}...ARROW:sc
+00000900: 6865 6d61 1898 0b2f 2f2f 2f2f 7967 4541  hema.../////ygEA
+00000910: 4141 5141 4141 4141 4141 4b41 4134 4142  AAQAAAAAAAKAA4AB
+00000920: 6741 4641 4167 4143 6741 4141 4141 4242  gAFAAgACgAAAAABB
+00000930: 4141 5141 4141 4141 4141 4b41 4177 4141  AAQAAAAAAAKAAwAA
+00000940: 4141 4541 4167 4143 6741 4141 4e77 4341  AAEAAgACgAAANwCA
+00000950: 4141 4541 4141 4141 5141 4141 4177 4141  AAEAAAAAQAAAAwAA
+00000960: 4141 4941 4177 4142 4141 4941 4167 4141  AAIAAwABAAIAAgAA
+00000970: 4141 4941 4141 4145 4141 4141 4159 4141  AAIAAAAEAAAAAYAA
+00000980: 4142 7759 5735 6b59 584d 4141 4b63 4341  ABwYW5kYXMAAKcCA
+00000990: 4142 3749 6d6c 755a 4756 3458 324e 7662  AB7ImluZGV4X2Nvb
+000009a0: 4856 7462 6e4d 694f 6942 6258 5377 6749  HVtbnMiOiBbXSwgI
+000009b0: 6d4e 7662 4856 7462 6c39 7062 6d52 6c65  mNvbHVtbl9pbmRle
+000009c0: 4756 7a49 6a6f 6757 3130 7349 434a 6a62  GVzIjogW10sICJjb
+000009d0: 3278 3162 5735 7a49 6a6f 6757 3373 6962  2x1bW5zIjogW3sib
+000009e0: 6d46 745a 5349 3649 434a 705a 4349 7349  mFtZSI6ICJpZCIsI
+000009f0: 434a 6d61 5756 735a 4639 7559 5731 6c49  CJmaWVsZF9uYW1lI
+00000a00: 6a6f 6749 6d6c 6b49 6977 6749 6e42 6862  jogImlkIiwgInBhb
+00000a10: 6d52 6863 3139 3065 5842 6c49 6a6f 6749  mRhc190eXBlIjogI
+00000a20: 6d6c 7564 4459 3049 6977 6749 6d35 3162  mludDY0IiwgIm51b
+00000a30: 5842 3558 3352 3563 4755 694f 6941 6961  XB5X3R5cGUiOiAia
+00000a40: 5735 304e 6a51 694c 4341 6962 5756 3059  W50NjQiLCAibWV0Y
+00000a50: 5752 6864 4745 694f 6942 7564 5778 7366  WRhdGEiOiBudWxsf
+00000a60: 5377 6765 794a 7559 5731 6c49 6a6f 6749  SwgeyJuYW1lIjogI
+00000a70: 6e4a 6849 6977 6749 6d5a 705a 5778 6b58  nJhIiwgImZpZWxkX
+00000a80: 3235 6862 5755 694f 6941 6963 6d45 694c  25hbWUiOiAicmEiL
+00000a90: 4341 6963 4746 755a 4746 7a58 3352 3563  CAicGFuZGFzX3R5c
+00000aa0: 4755 694f 6941 695a 6d78 7659 5851 324e  GUiOiAiZmxvYXQ2N
+00000ab0: 4349 7349 434a 7564 5731 7765 5639 3065  CIsICJudW1weV90e
+00000ac0: 5842 6c49 6a6f 6749 6d5a 7362 3246 304e  XBlIjogImZsb2F0N
+00000ad0: 6a51 694c 4341 6962 5756 3059 5752 6864  jQiLCAibWV0YWRhd
+00000ae0: 4745 694f 6942 7564 5778 7366 5377 6765  GEiOiBudWxsfSwge
+00000af0: 794a 7559 5731 6c49 6a6f 6749 6d52 6c59  yJuYW1lIjogImRlY
+00000b00: 7949 7349 434a 6d61 5756 735a 4639 7559  yIsICJmaWVsZF9uY
+00000b10: 5731 6c49 6a6f 6749 6d52 6c59 7949 7349  W1lIjogImRlYyIsI
+00000b20: 434a 7759 5735 6b59 584e 6664 486c 775a  CJwYW5kYXNfdHlwZ
+00000b30: 5349 3649 434a 6d62 4739 6864 4459 3049  SI6ICJmbG9hdDY0I
+00000b40: 6977 6749 6d35 3162 5842 3558 3352 3563  iwgIm51bXB5X3R5c
+00000b50: 4755 694f 6941 695a 6d78 7659 5851 324e  GUiOiAiZmxvYXQ2N
+00000b60: 4349 7349 434a 745a 5852 685a 4746 3059  CIsICJtZXRhZGF0Y
+00000b70: 5349 3649 4735 3162 4778 394c 4342 3749  SI6IG51bGx9LCB7I
+00000b80: 6d35 6862 5755 694f 6941 6963 6d46 665a  m5hbWUiOiAicmFfZ
+00000b90: 584a 7962 3349 694c 4341 695a 6d6c 6c62  XJyb3IiLCAiZmllb
+00000ba0: 4752 6662 6d46 745a 5349 3649 434a 7959  GRfbmFtZSI6ICJyY
+00000bb0: 5639 6c63 6e4a 7663 6949 7349 434a 7759  V9lcnJvciIsICJwY
+00000bc0: 5735 6b59 584e 6664 486c 775a 5349 3649  W5kYXNfdHlwZSI6I
+00000bd0: 434a 7062 6e51 324e 4349 7349 434a 7564  CJpbnQ2NCIsICJud
+00000be0: 5731 7765 5639 3065 5842 6c49 6a6f 6749  W1weV90eXBlIjogI
+00000bf0: 6d6c 7564 4459 3049 6977 6749 6d31 6c64  mludDY0IiwgIm1ld
+00000c00: 4746 6b59 5852 6849 6a6f 6762 6e56 7362  GFkYXRhIjogbnVsb
+00000c10: 4830 7349 4873 6962 6d46 745a 5349 3649  H0sIHsibmFtZSI6I
+00000c20: 434a 6b5a 574e 665a 584a 7962 3349 694c  CJkZWNfZXJyb3IiL
+00000c30: 4341 695a 6d6c 6c62 4752 6662 6d46 745a  CAiZmllbGRfbmFtZ
+00000c40: 5349 3649 434a 6b5a 574e 665a 584a 7962  SI6ICJkZWNfZXJyb
+00000c50: 3349 694c 4341 6963 4746 755a 4746 7a58  3IiLCAicGFuZGFzX
+00000c60: 3352 3563 4755 694f 6941 6961 5735 304e  3R5cGUiOiAiaW50N
+00000c70: 6a51 694c 4341 6962 6e56 7463 486c 6664  jQiLCAibnVtcHlfd
+00000c80: 486c 775a 5349 3649 434a 7062 6e51 324e  HlwZSI6ICJpbnQ2N
+00000c90: 4349 7349 434a 745a 5852 685a 4746 3059  CIsICJtZXRhZGF0Y
+00000ca0: 5349 3649 4735 3162 4778 3958 5377 6749  SI6IG51bGx9XSwgI
+00000cb0: 6d4e 795a 5746 3062 3349 694f 6942 3749  mNyZWF0b3IiOiB7I
+00000cc0: 6d78 7059 6e4a 6863 6e6b 694f 6941 6963  mxpYnJhcnkiOiAic
+00000cd0: 486c 6863 6e4a 7664 7949 7349 434a 325a  HlhcnJvdyIsICJ2Z
+00000ce0: 584a 7a61 5739 7549 6a6f 6749 6a6b 754d  XJzaW9uIjogIjkuM
+00000cf0: 4334 7749 6e30 7349 434a 7759 5735 6b59  C4wIn0sICJwYW5kY
+00000d00: 584e 6664 6d56 7963 326c 7662 6949 3649  XNfdmVyc2lvbiI6I
+00000d10: 4349 794c 6a41 754d 434a 3941 4155 4141  CIyLjAuMCJ9AAUAA
+00000d20: 4144 6b41 4141 416f 4141 4141 4851 4141  ADkAAAAoAAAAHQAA
+00000d30: 4141 3841 4141 4142 4141 4141 4544 2f2f  AA8AAAABAAAAED//
+00000d40: 2f38 4141 4145 4345 4141 4141 4277 4141  /8AAAECEAAAABwAA
+00000d50: 4141 4541 4141 4141 4141 4141 416b 4141  AAEAAAAAAAAAAkAA
+00000d60: 4142 6b5a 574e 665a 584a 7962 3349 4141  ABkZWNfZXJyb3IAA
+00000d70: 4141 342f 2f2f 2f41 4141 4141 5541 4141  AA4////AAAAAUAAA
+00000d80: 4142 302f 2f2f 2f41 4141 4241 6841 4141  AB0////AAABAhAAA
+00000d90: 4141 6341 4141 4142 4141 4141 4141 4141  AAcAAAABAAAAAAAA
+00000da0: 4141 4941 4141 4163 6d46 665a 584a 7962  AAIAAAAcmFfZXJyb
+00000db0: 3349 4141 4141 4162 502f 2f2f 7741 4141  3IAAAAAbP///wAAA
+00000dc0: 4146 4141 4141 4171 502f 2f2f 7741 4141  AFAAAAAqP///wAAA
+00000dd0: 514d 5141 4141 4146 4141 4141 4151 4141  QMQAAAAFAAAAAQAA
+00000de0: 4141 4141 4141 4141 7741 4141 4752 6c59  AAAAAAAAwAAAGRlY
+00000df0: 7744 572f 2f2f 2f41 4141 4341 4e44 2f2f  wDW////AAACAND//
+00000e00: 2f38 4141 4145 4445 4141 4141 4277 4141  /8AAAEDEAAAABwAA
+00000e10: 4141 4541 4141 4141 4141 4141 4149 4141  AAEAAAAAAAAAAIAA
+00000e20: 4142 7959 5141 4141 4141 4741 4167 4142  AByYQAAAAAGAAgAB
+00000e30: 6741 4741 4141 4141 4141 4341 4241 4146  gAGAAAAAAACABAAF
+00000e40: 4141 4941 4159 4142 7741 4d41 4141 4145  AAIAAYABwAMAAAAE
+00000e50: 4141 5141 4141 4141 4141 4241 6841 4141  AAQAAAAAAABAhAAA
+00000e60: 4141 6341 4141 4142 4141 4141 4141 4141  AAcAAAABAAAAAAAA
+00000e70: 4141 4341 4141 4161 5751 4141 4167 4144  AACAAAAaWQAAAgAD
+00000e80: 4141 4941 4163 4143 4141 4141 4141 4141  AAIAAcACAAAAAAAA
+00000e90: 4146 4141 4141 4141 4141 4141 413d 3d00  AFAAAAAAAAAAA==.
+00000ea0: 181f 7061 7271 7565 742d 6370 702d 6172  ..parquet-cpp-ar
+00000eb0: 726f 7720 7665 7273 696f 6e20 392e 302e  row version 9.0.
+00000ec0: 3019 5c1c 0000 1c00 001c 0000 1c00 001c  0.\.............
+00000ed0: 0000 00d3 0a00 0050 4152 31              .......PAR1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_47/shard_0.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet`

 * *Files 15% similar despite different names*

```diff
@@ -58,247 +58,181 @@
 00000390: 0000 0000 0009 2002 0000 000a 0101 0a00  ...... .........
 000003a0: 26c0 0e1c 1504 1935 1000 0619 1809 6465  &......5......de
 000003b0: 635f 6572 726f 7215 0216 0a16 b801 16c0  c_error.........
 000003c0: 0126 b00d 2680 0d1c 1808 0000 0000 0000  .&..&...........
 000003d0: 0000 1808 0000 0000 0000 0000 1600 2808  ..............(.
 000003e0: 0000 0000 0000 0000 1808 0000 0000 0000  ................
 000003f0: 0000 0019 2c15 0415 0015 0200 1500 1510  ....,...........
-00000400: 1502 0000 0015 0415 5015 404c 150a 1500  ........P.@L....
-00000410: 1200 0028 0401 0009 0100 0e09 0704 0013  ...(............
-00000420: 0d08 3c15 0000 0000 0000 0016 0000 0000  ..<.............
-00000430: 0000 0015 0015 1615 1a2c 150a 1510 1506  .........,......
-00000440: 1506 1c18 0816 0000 0000 0000 0018 0801  ................
-00000450: 0000 0000 0000 0016 0028 0816 0000 0000  .........(......
-00000460: 0000 0018 0801 0000 0000 0000 0000 0000  ................
-00000470: 0b28 0200 0000 0a01 0303 8846 0026 fa11  .(.........F.&..
-00000480: 1c15 0419 3510 0006 1918 115f 5f69 6e64  ....5......__ind
-00000490: 6578 5f6c 6576 656c 5f30 5f5f 1502 160a  ex_level_0__....
-000004a0: 16fc 0116 f001 26e6 1026 8a10 1c18 0816  ......&..&......
-000004b0: 0000 0000 0000 0018 0801 0000 0000 0000  ................
-000004c0: 0016 0028 0816 0000 0000 0000 0018 0801  ...(............
-000004d0: 0000 0000 0000 0000 192c 1504 1500 1502  .........,......
-000004e0: 0015 0015 1015 0200 0000 1504 197c 3500  .............|5.
-000004f0: 1806 7363 6865 6d61 150c 0015 0425 0218  ..schema.....%..
-00000500: 0269 6400 150a 2502 1802 7261 0015 0a25  .id...%...ra...%
-00000510: 0218 0364 6563 0015 0425 0218 0872 615f  ...dec...%...ra_
-00000520: 6572 726f 7200 1504 2502 1809 6465 635f  error...%...dec_
-00000530: 6572 726f 7200 1504 2502 1811 5f5f 696e  error...%...__in
-00000540: 6465 785f 6c65 7665 6c5f 305f 5f00 160a  dex_level_0__...
-00000550: 191c 196c 26f8 011c 1504 1935 1000 0619  ...l&......5....
-00000560: 1802 6964 1502 160a 16fc 0116 f001 2664  ..id..........&d
-00000570: 2608 1c18 081f 0300 0000 0000 0018 080a  &...............
-00000580: 0300 0000 0000 0016 0028 081f 0300 0000  .........(......
-00000590: 0000 0018 080a 0300 0000 0000 0000 192c  ...............,
-000005a0: 1504 1500 1502 0015 0015 1015 0200 0000  ................
-000005b0: 2696 051c 150a 1935 1000 0619 1802 7261  &......5......ra
-000005c0: 1502 160a 16ea 0116 e601 2684 0426 b003  ..........&..&..
-000005d0: 1c18 0800 0000 0000 0874 4018 0800 0000  .........t@.....
-000005e0: 0000 8873 4016 0028 0800 0000 0000 0874  ...s@..(.......t
-000005f0: 4018 0800 0000 0000 8873 4000 192c 1504  @........s@..,..
-00000600: 1500 1502 0015 0015 1015 0200 0000 26ba  ..............&.
-00000610: 081c 150a 1935 1000 0619 1803 6465 6315  .....5......dec.
-00000620: 0216 0a16 ea01 16e8 0126 a807 26d2 061c  .........&..&...
-00000630: 1808 0000 0000 0080 3cc0 1808 0000 0000  ........<.......
-00000640: 0040 42c0 1600 2808 0000 0000 0080 3cc0  .@B...(.......<.
-00000650: 1808 0000 0000 0040 42c0 0019 2c15 0415  .......@B...,...
-00000660: 0015 0200 1500 1510 1502 0000 0026 b80b  .............&..
-00000670: 1c15 0419 3510 0006 1918 0872 615f 6572  ....5......ra_er
-00000680: 726f 7215 0216 0a16 b801 16c0 0126 a80a  ror..........&..
-00000690: 26f8 091c 1808 0000 0000 0000 0000 1808  &...............
-000006a0: 0000 0000 0000 0000 1600 2808 0000 0000  ..........(.....
-000006b0: 0000 0000 1808 0000 0000 0000 0000 0019  ................
-000006c0: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
-000006d0: 0026 c00e 1c15 0419 3510 0006 1918 0964  .&......5......d
-000006e0: 6563 5f65 7272 6f72 1502 160a 16b8 0116  ec_error........
-000006f0: c001 26b0 0d26 800d 1c18 0800 0000 0000  ..&..&..........
-00000700: 0000 0018 0800 0000 0000 0000 0016 0028  ...............(
-00000710: 0800 0000 0000 0000 0018 0800 0000 0000  ................
-00000720: 0000 0000 192c 1504 1500 1502 0015 0015  .....,..........
-00000730: 1015 0200 0000 26fa 111c 1504 1935 1000  ......&......5..
-00000740: 0619 1811 5f5f 696e 6465 785f 6c65 7665  ....__index_leve
-00000750: 6c5f 305f 5f15 0216 0a16 fc01 16f0 0126  l_0__..........&
-00000760: e610 268a 101c 1808 1600 0000 0000 0000  ..&.............
-00000770: 1808 0100 0000 0000 0000 1600 2808 1600  ............(...
-00000780: 0000 0000 0000 1808 0100 0000 0000 0000  ................
-00000790: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
-000007a0: 0000 0016 bc0a 160a 2608 16ae 0a14 0000  ........&.......
-000007b0: 192c 1806 7061 6e64 6173 18a5 077b 2269  .,..pandas...{"i
-000007c0: 6e64 6578 5f63 6f6c 756d 6e73 223a 205b  ndex_columns": [
-000007d0: 225f 5f69 6e64 6578 5f6c 6576 656c 5f30  "__index_level_0
-000007e0: 5f5f 225d 2c20 2263 6f6c 756d 6e5f 696e  __"], "column_in
-000007f0: 6465 7865 7322 3a20 5b7b 226e 616d 6522  dexes": [{"name"
-00000800: 3a20 6e75 6c6c 2c20 2266 6965 6c64 5f6e  : null, "field_n
-00000810: 616d 6522 3a20 6e75 6c6c 2c20 2270 616e  ame": null, "pan
-00000820: 6461 735f 7479 7065 223a 2022 756e 6963  das_type": "unic
-00000830: 6f64 6522 2c20 226e 756d 7079 5f74 7970  ode", "numpy_typ
-00000840: 6522 3a20 226f 626a 6563 7422 2c20 226d  e": "object", "m
-00000850: 6574 6164 6174 6122 3a20 7b22 656e 636f  etadata": {"enco
-00000860: 6469 6e67 223a 2022 5554 462d 3822 7d7d  ding": "UTF-8"}}
-00000870: 5d2c 2022 636f 6c75 6d6e 7322 3a20 5b7b  ], "columns": [{
-00000880: 226e 616d 6522 3a20 2269 6422 2c20 2266  "name": "id", "f
-00000890: 6965 6c64 5f6e 616d 6522 3a20 2269 6422  ield_name": "id"
-000008a0: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
-000008b0: 2022 696e 7436 3422 2c20 226e 756d 7079   "int64", "numpy
-000008c0: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
-000008d0: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
-000008e0: 6c7d 2c20 7b22 6e61 6d65 223a 2022 7261  l}, {"name": "ra
-000008f0: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
-00000900: 2022 7261 222c 2022 7061 6e64 6173 5f74   "ra", "pandas_t
-00000910: 7970 6522 3a20 2266 6c6f 6174 3634 222c  ype": "float64",
-00000920: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
-00000930: 666c 6f61 7436 3422 2c20 226d 6574 6164  float64", "metad
-00000940: 6174 6122 3a20 6e75 6c6c 7d2c 207b 226e  ata": null}, {"n
-00000950: 616d 6522 3a20 2264 6563 222c 2022 6669  ame": "dec", "fi
-00000960: 656c 645f 6e61 6d65 223a 2022 6465 6322  eld_name": "dec"
-00000970: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
-00000980: 2022 666c 6f61 7436 3422 2c20 226e 756d   "float64", "num
-00000990: 7079 5f74 7970 6522 3a20 2266 6c6f 6174  py_type": "float
-000009a0: 3634 222c 2022 6d65 7461 6461 7461 223a  64", "metadata":
-000009b0: 206e 756c 6c7d 2c20 7b22 6e61 6d65 223a   null}, {"name":
-000009c0: 2022 7261 5f65 7272 6f72 222c 2022 6669   "ra_error", "fi
-000009d0: 656c 645f 6e61 6d65 223a 2022 7261 5f65  eld_name": "ra_e
-000009e0: 7272 6f72 222c 2022 7061 6e64 6173 5f74  rror", "pandas_t
-000009f0: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
-00000a00: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
-00000a10: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
-00000a20: 3a20 6e75 6c6c 7d2c 207b 226e 616d 6522  : null}, {"name"
-00000a30: 3a20 2264 6563 5f65 7272 6f72 222c 2022  : "dec_error", "
-00000a40: 6669 656c 645f 6e61 6d65 223a 2022 6465  field_name": "de
-00000a50: 635f 6572 726f 7222 2c20 2270 616e 6461  c_error", "panda
-00000a60: 735f 7479 7065 223a 2022 696e 7436 3422  s_type": "int64"
-00000a70: 2c20 226e 756d 7079 5f74 7970 6522 3a20  , "numpy_type": 
-00000a80: 2269 6e74 3634 222c 2022 6d65 7461 6461  "int64", "metada
-00000a90: 7461 223a 206e 756c 6c7d 2c20 7b22 6e61  ta": null}, {"na
-00000aa0: 6d65 223a 206e 756c 6c2c 2022 6669 656c  me": null, "fiel
-00000ab0: 645f 6e61 6d65 223a 2022 5f5f 696e 6465  d_name": "__inde
-00000ac0: 785f 6c65 7665 6c5f 305f 5f22 2c20 2270  x_level_0__", "p
-00000ad0: 616e 6461 735f 7479 7065 223a 2022 696e  andas_type": "in
-00000ae0: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
-00000af0: 6522 3a20 2269 6e74 3634 222c 2022 6d65  e": "int64", "me
-00000b00: 7461 6461 7461 223a 206e 756c 6c7d 5d2c  tadata": null}],
-00000b10: 2022 6372 6561 746f 7222 3a20 7b22 6c69   "creator": {"li
-00000b20: 6272 6172 7922 3a20 2270 7961 7272 6f77  brary": "pyarrow
-00000b30: 222c 2022 7665 7273 696f 6e22 3a20 2239  ", "version": "9
-00000b40: 2e30 2e30 227d 2c20 2270 616e 6461 735f  .0.0"}, "pandas_
-00000b50: 7665 7273 696f 6e22 3a20 2231 2e33 2e35  version": "1.3.5
-00000b60: 227d 0018 0c41 5252 4f57 3a73 6368 656d  "}...ARROW:schem
-00000b70: 6118 c00e 2f2f 2f2f 2f32 6746 4141 4151  a.../////2gFAAAQ
-00000b80: 4141 4141 4141 414b 4141 3441 4267 4146  AAAAAAAKAA4ABgAF
-00000b90: 4141 6741 4367 4141 4141 4142 4241 4151  AAgACgAAAAABBAAQ
-00000ba0: 4141 4141 4141 414b 4141 7741 4141 4145  AAAAAAAKAAwAAAAE
-00000bb0: 4141 6741 4367 4141 414e 7744 4141 4145  AAgACgAAANwDAAAE
-00000bc0: 4141 4141 4151 4141 4141 7741 4141 4149  AAAAAQAAAAwAAAAI
-00000bd0: 4141 7741 4241 4149 4141 6741 4141 4149  AAwABAAIAAgAAAAI
-00000be0: 4141 4141 4541 4141 4141 5941 4141 4277  AAAAEAAAAAYAAABw
-00000bf0: 5957 356b 5958 4d41 414b 5544 4141 4237  YW5kYXMAAKUDAAB7
-00000c00: 496d 6c75 5a47 5634 5832 4e76 6248 5674  ImluZGV4X2NvbHVt
-00000c10: 626e 4d69 4f69 4262 496c 3966 6157 356b  bnMiOiBbIl9faW5k
-00000c20: 5a58 6866 6247 5632 5a57 7866 4d46 3966  ZXhfbGV2ZWxfMF9f
-00000c30: 496c 3073 4943 4a6a 6232 7831 6257 3566  Il0sICJjb2x1bW5f
-00000c40: 6157 356b 5a58 686c 6379 4936 4946 7437  aW5kZXhlcyI6IFt7
-00000c50: 496d 3568 6257 5569 4f69 4275 6457 7873  Im5hbWUiOiBudWxs
-00000c60: 4c43 4169 5a6d 6c6c 6247 5266 626d 4674  LCAiZmllbGRfbmFt
-00000c70: 5a53 4936 4947 3531 6247 7773 4943 4a77  ZSI6IG51bGwsICJw
-00000c80: 5957 356b 5958 4e66 6448 6c77 5a53 4936  YW5kYXNfdHlwZSI6
-00000c90: 4943 4a31 626d 6c6a 6232 526c 4969 7767  ICJ1bmljb2RlIiwg
-00000ca0: 496d 3531 6258 4235 5833 5235 6347 5569  Im51bXB5X3R5cGUi
-00000cb0: 4f69 4169 6232 4a71 5a57 4e30 4969 7767  OiAib2JqZWN0Iiwg
-00000cc0: 496d 316c 6447 466b 5958 5268 496a 6f67  Im1ldGFkYXRhIjog
-00000cd0: 6579 4a6c 626d 4e76 5a47 6c75 5a79 4936  eyJlbmNvZGluZyI6
-00000ce0: 4943 4a56 5645 5974 4f43 4a39 6656 3073  ICJVVEYtOCJ9fV0s
-00000cf0: 4943 4a6a 6232 7831 6257 357a 496a 6f67  ICJjb2x1bW5zIjog
-00000d00: 5733 7369 626d 4674 5a53 4936 4943 4a70  W3sibmFtZSI6ICJp
-00000d10: 5a43 4973 4943 4a6d 6157 5673 5a46 3975  ZCIsICJmaWVsZF9u
-00000d20: 5957 316c 496a 6f67 496d 6c6b 4969 7767  YW1lIjogImlkIiwg
-00000d30: 496e 4268 626d 5268 6331 3930 6558 426c  InBhbmRhc190eXBl
-00000d40: 496a 6f67 496d 6c75 6444 5930 4969 7767  IjogImludDY0Iiwg
-00000d50: 496d 3531 6258 4235 5833 5235 6347 5569  Im51bXB5X3R5cGUi
-00000d60: 4f69 4169 6157 3530 4e6a 5169 4c43 4169  OiAiaW50NjQiLCAi
-00000d70: 6257 5630 5957 5268 6447 4569 4f69 4275  bWV0YWRhdGEiOiBu
-00000d80: 6457 7873 6653 7767 6579 4a75 5957 316c  dWxsfSwgeyJuYW1l
-00000d90: 496a 6f67 496e 4a68 4969 7767 496d 5a70  IjogInJhIiwgImZp
-00000da0: 5a57 786b 5832 3568 6257 5569 4f69 4169  ZWxkX25hbWUiOiAi
-00000db0: 636d 4569 4c43 4169 6347 4675 5a47 467a  cmEiLCAicGFuZGFz
-00000dc0: 5833 5235 6347 5569 4f69 4169 5a6d 7876  X3R5cGUiOiAiZmxv
-00000dd0: 5958 5132 4e43 4973 4943 4a75 6457 3177  YXQ2NCIsICJudW1w
-00000de0: 6556 3930 6558 426c 496a 6f67 496d 5a73  eV90eXBlIjogImZs
-00000df0: 6232 4630 4e6a 5169 4c43 4169 6257 5630  b2F0NjQiLCAibWV0
-00000e00: 5957 5268 6447 4569 4f69 4275 6457 7873  YWRhdGEiOiBudWxs
-00000e10: 6653 7767 6579 4a75 5957 316c 496a 6f67  fSwgeyJuYW1lIjog
-00000e20: 496d 526c 5979 4973 4943 4a6d 6157 5673  ImRlYyIsICJmaWVs
-00000e30: 5a46 3975 5957 316c 496a 6f67 496d 526c  ZF9uYW1lIjogImRl
-00000e40: 5979 4973 4943 4a77 5957 356b 5958 4e66  YyIsICJwYW5kYXNf
-00000e50: 6448 6c77 5a53 4936 4943 4a6d 6247 3968  dHlwZSI6ICJmbG9h
-00000e60: 6444 5930 4969 7767 496d 3531 6258 4235  dDY0IiwgIm51bXB5
-00000e70: 5833 5235 6347 5569 4f69 4169 5a6d 7876  X3R5cGUiOiAiZmxv
-00000e80: 5958 5132 4e43 4973 4943 4a74 5a58 5268  YXQ2NCIsICJtZXRh
-00000e90: 5a47 4630 5953 4936 4947 3531 6247 7839  ZGF0YSI6IG51bGx9
-00000ea0: 4c43 4237 496d 3568 6257 5569 4f69 4169  LCB7Im5hbWUiOiAi
-00000eb0: 636d 4666 5a58 4a79 6233 4969 4c43 4169  cmFfZXJyb3IiLCAi
-00000ec0: 5a6d 6c6c 6247 5266 626d 4674 5a53 4936  ZmllbGRfbmFtZSI6
-00000ed0: 4943 4a79 5956 396c 636e 4a76 6369 4973  ICJyYV9lcnJvciIs
-00000ee0: 4943 4a77 5957 356b 5958 4e66 6448 6c77  ICJwYW5kYXNfdHlw
-00000ef0: 5a53 4936 4943 4a70 626e 5132 4e43 4973  ZSI6ICJpbnQ2NCIs
-00000f00: 4943 4a75 6457 3177 6556 3930 6558 426c  ICJudW1weV90eXBl
-00000f10: 496a 6f67 496d 6c75 6444 5930 4969 7767  IjogImludDY0Iiwg
-00000f20: 496d 316c 6447 466b 5958 5268 496a 6f67  Im1ldGFkYXRhIjog
-00000f30: 626e 5673 6248 3073 4948 7369 626d 4674  bnVsbH0sIHsibmFt
-00000f40: 5a53 4936 4943 4a6b 5a57 4e66 5a58 4a79  ZSI6ICJkZWNfZXJy
-00000f50: 6233 4969 4c43 4169 5a6d 6c6c 6247 5266  b3IiLCAiZmllbGRf
-00000f60: 626d 4674 5a53 4936 4943 4a6b 5a57 4e66  bmFtZSI6ICJkZWNf
-00000f70: 5a58 4a79 6233 4969 4c43 4169 6347 4675  ZXJyb3IiLCAicGFu
-00000f80: 5a47 467a 5833 5235 6347 5569 4f69 4169  ZGFzX3R5cGUiOiAi
-00000f90: 6157 3530 4e6a 5169 4c43 4169 626e 5674  aW50NjQiLCAibnVt
-00000fa0: 6348 6c66 6448 6c77 5a53 4936 4943 4a70  cHlfdHlwZSI6ICJp
-00000fb0: 626e 5132 4e43 4973 4943 4a74 5a58 5268  bnQ2NCIsICJtZXRh
-00000fc0: 5a47 4630 5953 4936 4947 3531 6247 7839  ZGF0YSI6IG51bGx9
-00000fd0: 4c43 4237 496d 3568 6257 5569 4f69 4275  LCB7Im5hbWUiOiBu
-00000fe0: 6457 7873 4c43 4169 5a6d 6c6c 6247 5266  dWxsLCAiZmllbGRf
-00000ff0: 626d 4674 5a53 4936 4943 4a66 5832 6c75  bmFtZSI6ICJfX2lu
-00001000: 5a47 5634 5832 786c 646d 5673 587a 4266  ZGV4X2xldmVsXzBf
-00001010: 5879 4973 4943 4a77 5957 356b 5958 4e66  XyIsICJwYW5kYXNf
-00001020: 6448 6c77 5a53 4936 4943 4a70 626e 5132  dHlwZSI6ICJpbnQ2
-00001030: 4e43 4973 4943 4a75 6457 3177 6556 3930  NCIsICJudW1weV90
-00001040: 6558 426c 496a 6f67 496d 6c75 6444 5930  eXBlIjogImludDY0
-00001050: 4969 7767 496d 316c 6447 466b 5958 5268  IiwgIm1ldGFkYXRh
-00001060: 496a 6f67 626e 5673 6248 3164 4c43 4169  IjogbnVsbH1dLCAi
-00001070: 5933 4a6c 5958 5276 6369 4936 4948 7369  Y3JlYXRvciI6IHsi
-00001080: 6247 6c69 636d 4679 6553 4936 4943 4a77  bGlicmFyeSI6ICJw
-00001090: 6557 4679 636d 3933 4969 7767 496e 5a6c  eWFycm93IiwgInZl
-000010a0: 636e 4e70 6232 3469 4f69 4169 4f53 3477  cnNpb24iOiAiOS4w
-000010b0: 4c6a 4169 6653 7767 496e 4268 626d 5268  LjAifSwgInBhbmRh
-000010c0: 6331 3932 5a58 4a7a 6157 3975 496a 6f67  c192ZXJzaW9uIjog
-000010d0: 496a 4575 4d79 3431 496e 3041 4141 4147  IjEuMy41In0AAAAG
-000010e0: 4141 4141 4a41 4541 414f 4141 4141 4330  AAAAJAEAAOAAAAC0
-000010f0: 4141 4141 6641 4141 4145 5141 4141 4145  AAAAfAAAAEQAAAAE
-00001100: 4141 4141 4250 2f2f 2f77 4141 4151 4951  AAAABP///wAAAQIQ
-00001110: 4141 4141 4a41 4141 4141 5141 4141 4141  AAAAJAAAAAQAAAAA
-00001120: 4141 4141 4551 4141 4146 3966 6157 356b  AAAAEQAAAF9faW5k
-00001130: 5a58 6866 6247 5632 5a57 7866 4d46 3966  ZXhfbGV2ZWxfMF9f
-00001140: 4141 4141 4250 2f2f 2f77 4141 4141 4641  AAAABP///wAAAAFA
-00001150: 4141 4141 5150 2f2f 2f77 4141 4151 4951  AAAAQP///wAAAQIQ
-00001160: 4141 4141 4841 4141 4141 5141 4141 4141  AAAAHAAAAAQAAAAA
-00001170: 4141 4141 4351 4141 4147 526c 5931 396c  AAAACQAAAGRlY19l
-00001180: 636e 4a76 6367 4141 4144 6a2f 2f2f 3841  cnJvcgAAADj///8A
-00001190: 4141 4142 5141 4141 4148 542f 2f2f 3841  AAABQAAAAHT///8A
-000011a0: 4141 4543 4541 4141 4142 7741 4141 4145  AAECEAAAABwAAAAE
-000011b0: 4141 4141 4141 4141 4141 6741 4141 4279  AAAAAAAAAAgAAABy
-000011c0: 5956 396c 636e 4a76 6367 4141 4141 4273  YV9lcnJvcgAAAABs
-000011d0: 2f2f 2f2f 4141 4141 4155 4141 4141 436f  ////AAAAAUAAAACo
-000011e0: 2f2f 2f2f 4141 4142 4178 4141 4141 4155  ////AAABAxAAAAAU
-000011f0: 4141 4141 4241 4141 4141 4141 4141 4144  AAAABAAAAAAAAAAD
-00001200: 4141 4141 5a47 566a 414e 622f 2f2f 3841  AAAAZGVjANb///8A
-00001210: 4141 4941 3050 2f2f 2f77 4141 4151 4d51  AAIA0P///wAAAQMQ
-00001220: 4141 4141 4841 4141 4141 5141 4141 4141  AAAAHAAAAAQAAAAA
-00001230: 4141 4141 4167 4141 4148 4a68 4141 4141  AAAAAgAAAHJhAAAA
-00001240: 4141 5941 4341 4147 4141 5941 4141 4141  AAYACAAGAAYAAAAA
-00001250: 4141 4941 4541 4155 4141 6741 4267 4148  AAIAEAAUAAgABgAH
-00001260: 4141 7741 4141 4151 4142 4141 4141 4141  AAwAAAAQABAAAAAA
-00001270: 4141 4543 4541 4141 4142 7741 4141 4145  AAECEAAAABwAAAAE
-00001280: 4141 4141 4141 4141 4141 4941 4141 4270  AAAAAAAAAAIAAABp
-00001290: 5a41 4141 4341 414d 4141 6741 4277 4149  ZAAACAAMAAgABwAI
-000012a0: 4141 4141 4141 4141 4155 4141 4141 4141  AAAAAAAAAUAAAAAA
-000012b0: 4141 4141 0018 1f70 6172 7175 6574 2d63  AAAA...parquet-c
-000012c0: 7070 2d61 7272 6f77 2076 6572 7369 6f6e  pp-arrow version
-000012d0: 2039 2e30 2e30 196c 1c00 001c 0000 1c00   9.0.0.l........
-000012e0: 001c 0000 1c00 001c 0000 0001 0e00 0050  ...............P
-000012f0: 4152 31                                  AR1
+00000400: 1502 0000 0015 0419 6c35 0018 0673 6368  ........l5...sch
+00000410: 656d 6115 0a00 1504 2502 1802 6964 0015  ema.....%...id..
+00000420: 0a25 0218 0272 6100 150a 2502 1803 6465  .%...ra...%...de
+00000430: 6300 1504 2502 1808 7261 5f65 7272 6f72  c...%...ra_error
+00000440: 0015 0425 0218 0964 6563 5f65 7272 6f72  ...%...dec_error
+00000450: 0016 0a19 1c19 5c26 f801 1c15 0419 3510  ......\&......5.
+00000460: 0006 1918 0269 6415 0216 0a16 fc01 16f0  .....id.........
+00000470: 0126 6426 081c 1808 1f03 0000 0000 0000  .&d&............
+00000480: 1808 0a03 0000 0000 0000 1600 2808 1f03  ............(...
+00000490: 0000 0000 0000 1808 0a03 0000 0000 0000  ................
+000004a0: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
+000004b0: 0000 0026 9605 1c15 0a19 3510 0006 1918  ...&......5.....
+000004c0: 0272 6115 0216 0a16 ea01 16e6 0126 8404  .ra..........&..
+000004d0: 26b0 031c 1808 0000 0000 0008 7440 1808  &...........t@..
+000004e0: 0000 0000 0088 7340 1600 2808 0000 0000  ......s@..(.....
+000004f0: 0008 7440 1808 0000 0000 0088 7340 0019  ..t@........s@..
+00000500: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
+00000510: 0026 ba08 1c15 0a19 3510 0006 1918 0364  .&......5......d
+00000520: 6563 1502 160a 16ea 0116 e801 26a8 0726  ec..........&..&
+00000530: d206 1c18 0800 0000 0000 803c c018 0800  ...........<....
+00000540: 0000 0000 4042 c016 0028 0800 0000 0000  ....@B...(......
+00000550: 803c c018 0800 0000 0000 4042 c000 192c  .<........@B...,
+00000560: 1504 1500 1502 0015 0015 1015 0200 0000  ................
+00000570: 26b8 0b1c 1504 1935 1000 0619 1808 7261  &......5......ra
+00000580: 5f65 7272 6f72 1502 160a 16b8 0116 c001  _error..........
+00000590: 26a8 0a26 f809 1c18 0800 0000 0000 0000  &..&............
+000005a0: 0018 0800 0000 0000 0000 0016 0028 0800  .............(..
+000005b0: 0000 0000 0000 0018 0800 0000 0000 0000  ................
+000005c0: 0000 192c 1504 1500 1502 0015 0015 1015  ...,............
+000005d0: 0200 0000 26c0 0e1c 1504 1935 1000 0619  ....&......5....
+000005e0: 1809 6465 635f 6572 726f 7215 0216 0a16  ..dec_error.....
+000005f0: b801 16c0 0126 b00d 2680 0d1c 1808 0000  .....&..&.......
+00000600: 0000 0000 0000 1808 0000 0000 0000 0000  ................
+00000610: 1600 2808 0000 0000 0000 0000 1808 0000  ..(.............
+00000620: 0000 0000 0000 0019 2c15 0415 0015 0200  ........,.......
+00000630: 1500 1510 1502 0000 0016 c008 160a 2608  ..............&.
+00000640: 16be 0814 0000 192c 1806 7061 6e64 6173  .......,..pandas
+00000650: 18a7 057b 2269 6e64 6578 5f63 6f6c 756d  ...{"index_colum
+00000660: 6e73 223a 205b 5d2c 2022 636f 6c75 6d6e  ns": [], "column
+00000670: 5f69 6e64 6578 6573 223a 205b 5d2c 2022  _indexes": [], "
+00000680: 636f 6c75 6d6e 7322 3a20 5b7b 226e 616d  columns": [{"nam
+00000690: 6522 3a20 2269 6422 2c20 2266 6965 6c64  e": "id", "field
+000006a0: 5f6e 616d 6522 3a20 2269 6422 2c20 2270  _name": "id", "p
+000006b0: 616e 6461 735f 7479 7065 223a 2022 696e  andas_type": "in
+000006c0: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
+000006d0: 6522 3a20 2269 6e74 3634 222c 2022 6d65  e": "int64", "me
+000006e0: 7461 6461 7461 223a 206e 756c 6c7d 2c20  tadata": null}, 
+000006f0: 7b22 6e61 6d65 223a 2022 7261 222c 2022  {"name": "ra", "
+00000700: 6669 656c 645f 6e61 6d65 223a 2022 7261  field_name": "ra
+00000710: 222c 2022 7061 6e64 6173 5f74 7970 6522  ", "pandas_type"
+00000720: 3a20 2266 6c6f 6174 3634 222c 2022 6e75  : "float64", "nu
+00000730: 6d70 795f 7479 7065 223a 2022 666c 6f61  mpy_type": "floa
+00000740: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
+00000750: 3a20 6e75 6c6c 7d2c 207b 226e 616d 6522  : null}, {"name"
+00000760: 3a20 2264 6563 222c 2022 6669 656c 645f  : "dec", "field_
+00000770: 6e61 6d65 223a 2022 6465 6322 2c20 2270  name": "dec", "p
+00000780: 616e 6461 735f 7479 7065 223a 2022 666c  andas_type": "fl
+00000790: 6f61 7436 3422 2c20 226e 756d 7079 5f74  oat64", "numpy_t
+000007a0: 7970 6522 3a20 2266 6c6f 6174 3634 222c  ype": "float64",
+000007b0: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
+000007c0: 6c7d 2c20 7b22 6e61 6d65 223a 2022 7261  l}, {"name": "ra
+000007d0: 5f65 7272 6f72 222c 2022 6669 656c 645f  _error", "field_
+000007e0: 6e61 6d65 223a 2022 7261 5f65 7272 6f72  name": "ra_error
+000007f0: 222c 2022 7061 6e64 6173 5f74 7970 6522  ", "pandas_type"
+00000800: 3a20 2269 6e74 3634 222c 2022 6e75 6d70  : "int64", "nump
+00000810: 795f 7479 7065 223a 2022 696e 7436 3422  y_type": "int64"
+00000820: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
+00000830: 6c6c 7d2c 207b 226e 616d 6522 3a20 2264  ll}, {"name": "d
+00000840: 6563 5f65 7272 6f72 222c 2022 6669 656c  ec_error", "fiel
+00000850: 645f 6e61 6d65 223a 2022 6465 635f 6572  d_name": "dec_er
+00000860: 726f 7222 2c20 2270 616e 6461 735f 7479  ror", "pandas_ty
+00000870: 7065 223a 2022 696e 7436 3422 2c20 226e  pe": "int64", "n
+00000880: 756d 7079 5f74 7970 6522 3a20 2269 6e74  umpy_type": "int
+00000890: 3634 222c 2022 6d65 7461 6461 7461 223a  64", "metadata":
+000008a0: 206e 756c 6c7d 5d2c 2022 6372 6561 746f   null}], "creato
+000008b0: 7222 3a20 7b22 6c69 6272 6172 7922 3a20  r": {"library": 
+000008c0: 2270 7961 7272 6f77 222c 2022 7665 7273  "pyarrow", "vers
+000008d0: 696f 6e22 3a20 2239 2e30 2e30 227d 2c20  ion": "9.0.0"}, 
+000008e0: 2270 616e 6461 735f 7665 7273 696f 6e22  "pandas_version"
+000008f0: 3a20 2232 2e30 2e30 227d 0018 0c41 5252  : "2.0.0"}...ARR
+00000900: 4f57 3a73 6368 656d 6118 980b 2f2f 2f2f  OW:schema...////
+00000910: 2f79 6745 4141 4151 4141 4141 4141 414b  /ygEAAAQAAAAAAAK
+00000920: 4141 3441 4267 4146 4141 6741 4367 4141  AA4ABgAFAAgACgAA
+00000930: 4141 4142 4241 4151 4141 4141 4141 414b  AAABBAAQAAAAAAAK
+00000940: 4141 7741 4141 4145 4141 6741 4367 4141  AAwAAAAEAAgACgAA
+00000950: 414e 7743 4141 4145 4141 4141 4151 4141  ANwCAAAEAAAAAQAA
+00000960: 4141 7741 4141 4149 4141 7741 4241 4149  AAwAAAAIAAwABAAI
+00000970: 4141 6741 4141 4149 4141 4141 4541 4141  AAgAAAAIAAAAEAAA
+00000980: 4141 5941 4141 4277 5957 356b 5958 4d41  AAYAAABwYW5kYXMA
+00000990: 414b 6343 4141 4237 496d 6c75 5a47 5634  AKcCAAB7ImluZGV4
+000009a0: 5832 4e76 6248 5674 626e 4d69 4f69 4262  X2NvbHVtbnMiOiBb
+000009b0: 5853 7767 496d 4e76 6248 5674 626c 3970  XSwgImNvbHVtbl9p
+000009c0: 626d 526c 6547 567a 496a 6f67 5731 3073  bmRleGVzIjogW10s
+000009d0: 4943 4a6a 6232 7831 6257 357a 496a 6f67  ICJjb2x1bW5zIjog
+000009e0: 5733 7369 626d 4674 5a53 4936 4943 4a70  W3sibmFtZSI6ICJp
+000009f0: 5a43 4973 4943 4a6d 6157 5673 5a46 3975  ZCIsICJmaWVsZF9u
+00000a00: 5957 316c 496a 6f67 496d 6c6b 4969 7767  YW1lIjogImlkIiwg
+00000a10: 496e 4268 626d 5268 6331 3930 6558 426c  InBhbmRhc190eXBl
+00000a20: 496a 6f67 496d 6c75 6444 5930 4969 7767  IjogImludDY0Iiwg
+00000a30: 496d 3531 6258 4235 5833 5235 6347 5569  Im51bXB5X3R5cGUi
+00000a40: 4f69 4169 6157 3530 4e6a 5169 4c43 4169  OiAiaW50NjQiLCAi
+00000a50: 6257 5630 5957 5268 6447 4569 4f69 4275  bWV0YWRhdGEiOiBu
+00000a60: 6457 7873 6653 7767 6579 4a75 5957 316c  dWxsfSwgeyJuYW1l
+00000a70: 496a 6f67 496e 4a68 4969 7767 496d 5a70  IjogInJhIiwgImZp
+00000a80: 5a57 786b 5832 3568 6257 5569 4f69 4169  ZWxkX25hbWUiOiAi
+00000a90: 636d 4569 4c43 4169 6347 4675 5a47 467a  cmEiLCAicGFuZGFz
+00000aa0: 5833 5235 6347 5569 4f69 4169 5a6d 7876  X3R5cGUiOiAiZmxv
+00000ab0: 5958 5132 4e43 4973 4943 4a75 6457 3177  YXQ2NCIsICJudW1w
+00000ac0: 6556 3930 6558 426c 496a 6f67 496d 5a73  eV90eXBlIjogImZs
+00000ad0: 6232 4630 4e6a 5169 4c43 4169 6257 5630  b2F0NjQiLCAibWV0
+00000ae0: 5957 5268 6447 4569 4f69 4275 6457 7873  YWRhdGEiOiBudWxs
+00000af0: 6653 7767 6579 4a75 5957 316c 496a 6f67  fSwgeyJuYW1lIjog
+00000b00: 496d 526c 5979 4973 4943 4a6d 6157 5673  ImRlYyIsICJmaWVs
+00000b10: 5a46 3975 5957 316c 496a 6f67 496d 526c  ZF9uYW1lIjogImRl
+00000b20: 5979 4973 4943 4a77 5957 356b 5958 4e66  YyIsICJwYW5kYXNf
+00000b30: 6448 6c77 5a53 4936 4943 4a6d 6247 3968  dHlwZSI6ICJmbG9h
+00000b40: 6444 5930 4969 7767 496d 3531 6258 4235  dDY0IiwgIm51bXB5
+00000b50: 5833 5235 6347 5569 4f69 4169 5a6d 7876  X3R5cGUiOiAiZmxv
+00000b60: 5958 5132 4e43 4973 4943 4a74 5a58 5268  YXQ2NCIsICJtZXRh
+00000b70: 5a47 4630 5953 4936 4947 3531 6247 7839  ZGF0YSI6IG51bGx9
+00000b80: 4c43 4237 496d 3568 6257 5569 4f69 4169  LCB7Im5hbWUiOiAi
+00000b90: 636d 4666 5a58 4a79 6233 4969 4c43 4169  cmFfZXJyb3IiLCAi
+00000ba0: 5a6d 6c6c 6247 5266 626d 4674 5a53 4936  ZmllbGRfbmFtZSI6
+00000bb0: 4943 4a79 5956 396c 636e 4a76 6369 4973  ICJyYV9lcnJvciIs
+00000bc0: 4943 4a77 5957 356b 5958 4e66 6448 6c77  ICJwYW5kYXNfdHlw
+00000bd0: 5a53 4936 4943 4a70 626e 5132 4e43 4973  ZSI6ICJpbnQ2NCIs
+00000be0: 4943 4a75 6457 3177 6556 3930 6558 426c  ICJudW1weV90eXBl
+00000bf0: 496a 6f67 496d 6c75 6444 5930 4969 7767  IjogImludDY0Iiwg
+00000c00: 496d 316c 6447 466b 5958 5268 496a 6f67  Im1ldGFkYXRhIjog
+00000c10: 626e 5673 6248 3073 4948 7369 626d 4674  bnVsbH0sIHsibmFt
+00000c20: 5a53 4936 4943 4a6b 5a57 4e66 5a58 4a79  ZSI6ICJkZWNfZXJy
+00000c30: 6233 4969 4c43 4169 5a6d 6c6c 6247 5266  b3IiLCAiZmllbGRf
+00000c40: 626d 4674 5a53 4936 4943 4a6b 5a57 4e66  bmFtZSI6ICJkZWNf
+00000c50: 5a58 4a79 6233 4969 4c43 4169 6347 4675  ZXJyb3IiLCAicGFu
+00000c60: 5a47 467a 5833 5235 6347 5569 4f69 4169  ZGFzX3R5cGUiOiAi
+00000c70: 6157 3530 4e6a 5169 4c43 4169 626e 5674  aW50NjQiLCAibnVt
+00000c80: 6348 6c66 6448 6c77 5a53 4936 4943 4a70  cHlfdHlwZSI6ICJp
+00000c90: 626e 5132 4e43 4973 4943 4a74 5a58 5268  bnQ2NCIsICJtZXRh
+00000ca0: 5a47 4630 5953 4936 4947 3531 6247 7839  ZGF0YSI6IG51bGx9
+00000cb0: 5853 7767 496d 4e79 5a57 4630 6233 4969  XSwgImNyZWF0b3Ii
+00000cc0: 4f69 4237 496d 7870 596e 4a68 636e 6b69  OiB7ImxpYnJhcnki
+00000cd0: 4f69 4169 6348 6c68 636e 4a76 6479 4973  OiAicHlhcnJvdyIs
+00000ce0: 4943 4a32 5a58 4a7a 6157 3975 496a 6f67  ICJ2ZXJzaW9uIjog
+00000cf0: 496a 6b75 4d43 3477 496e 3073 4943 4a77  IjkuMC4wIn0sICJw
+00000d00: 5957 356b 5958 4e66 646d 5679 6332 6c76  YW5kYXNfdmVyc2lv
+00000d10: 6269 4936 4943 4979 4c6a 4175 4d43 4a39  biI6ICIyLjAuMCJ9
+00000d20: 4141 5541 4141 446b 4141 4141 6f41 4141  AAUAAADkAAAAoAAA
+00000d30: 4148 5141 4141 4138 4141 4141 4241 4141  AHQAAAA8AAAABAAA
+00000d40: 4145 442f 2f2f 3841 4141 4543 4541 4141  AED///8AAAECEAAA
+00000d50: 4142 7741 4141 4145 4141 4141 4141 4141  ABwAAAAEAAAAAAAA
+00000d60: 4141 6b41 4141 426b 5a57 4e66 5a58 4a79  AAkAAABkZWNfZXJy
+00000d70: 6233 4941 4141 4134 2f2f 2f2f 4141 4141  b3IAAAA4////AAAA
+00000d80: 4155 4141 4141 4230 2f2f 2f2f 4141 4142  AUAAAAB0////AAAB
+00000d90: 4168 4141 4141 4163 4141 4141 4241 4141  AhAAAAAcAAAABAAA
+00000da0: 4141 4141 4141 4149 4141 4141 636d 4666  AAAAAAAIAAAAcmFf
+00000db0: 5a58 4a79 6233 4941 4141 4141 6250 2f2f  ZXJyb3IAAAAAbP//
+00000dc0: 2f77 4141 4141 4641 4141 4141 7150 2f2f  /wAAAAFAAAAAqP//
+00000dd0: 2f77 4141 4151 4d51 4141 4141 4641 4141  /wAAAQMQAAAAFAAA
+00000de0: 4141 5141 4141 4141 4141 4141 4177 4141  AAQAAAAAAAAAAwAA
+00000df0: 4147 526c 5977 4457 2f2f 2f2f 4141 4143  AGRlYwDW////AAAC
+00000e00: 414e 442f 2f2f 3841 4141 4544 4541 4141  AND///8AAAEDEAAA
+00000e10: 4142 7741 4141 4145 4141 4141 4141 4141  ABwAAAAEAAAAAAAA
+00000e20: 4141 4941 4141 4279 5951 4141 4141 4147  AAIAAAByYQAAAAAG
+00000e30: 4141 6741 4267 4147 4141 4141 4141 4143  AAgABgAGAAAAAAAC
+00000e40: 4142 4141 4641 4149 4141 5941 4277 414d  ABAAFAAIAAYABwAM
+00000e50: 4141 4141 4541 4151 4141 4141 4141 4142  AAAAEAAQAAAAAAAB
+00000e60: 4168 4141 4141 4163 4141 4141 4241 4141  AhAAAAAcAAAABAAA
+00000e70: 4141 4141 4141 4143 4141 4141 6157 5141  AAAAAAACAAAAaWQA
+00000e80: 4141 6741 4441 4149 4141 6341 4341 4141  AAgADAAIAAcACAAA
+00000e90: 4141 4141 4141 4641 4141 4141 4141 4141  AAAAAAFAAAAAAAAA
+00000ea0: 4141 3d3d 0018 1f70 6172 7175 6574 2d63  AA==...parquet-c
+00000eb0: 7070 2d61 7272 6f77 2076 6572 7369 6f6e  pp-arrow version
+00000ec0: 2039 2e30 2e30 195c 1c00 001c 0000 1c00   9.0.0.\........
+00000ed0: 001c 0000 1c00 0000 d30a 0000 5041 5231  ............PAR1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_47/shard_1.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet`

 * *Files 16% similar despite different names*

```diff
@@ -56,245 +56,181 @@
 00000370: 0200 0000 0401 0104 0026 f20d 1c15 0419  .........&......
 00000380: 3510 0006 1918 0964 6563 5f65 7272 6f72  5......dec_error
 00000390: 1502 1604 16b8 0116 c001 26e2 0c26 b20c  ..........&..&..
 000003a0: 1c18 0800 0000 0000 0000 0018 0800 0000  ................
 000003b0: 0000 0000 0016 0028 0800 0000 0000 0000  .......(........
 000003c0: 0018 0800 0000 0000 0000 0000 192c 1504  .............,..
 000003d0: 1500 1502 0015 0015 1015 0200 0000 1504  ................
-000003e0: 1520 1524 4c15 0415 0012 0000 103c 0200  . .$L........<..
-000003f0: 0000 0000 0000 1500 0000 0000 0000 1500  ................
-00000400: 1512 1516 2c15 0415 1015 0615 061c 1808  ....,...........
-00000410: 1500 0000 0000 0000 1808 0200 0000 0000  ................
-00000420: 0000 1600 2808 1500 0000 0000 0000 1808  ....(...........
-00000430: 0200 0000 0000 0000 0000 0009 2002 0000  ............ ...
-00000440: 0004 0101 0302 268c 111c 1504 1935 1000  ......&......5..
-00000450: 0619 1811 5f5f 696e 6465 785f 6c65 7665  ....__index_leve
-00000460: 6c5f 305f 5f15 0216 0416 c801 16d0 0126  l_0__..........&
-00000470: fc0f 26bc 0f1c 1808 1500 0000 0000 0000  ..&.............
-00000480: 1808 0200 0000 0000 0000 1600 2808 1500  ............(...
-00000490: 0000 0000 0000 1808 0200 0000 0000 0000  ................
-000004a0: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
-000004b0: 0000 0015 0419 7c35 0018 0673 6368 656d  ......|5...schem
-000004c0: 6115 0c00 1504 2502 1802 6964 0015 0a25  a.....%...id...%
-000004d0: 0218 0272 6100 150a 2502 1803 6465 6300  ...ra...%...dec.
-000004e0: 1504 2502 1808 7261 5f65 7272 6f72 0015  ..%...ra_error..
-000004f0: 0425 0218 0964 6563 5f65 7272 6f72 0015  .%...dec_error..
-00000500: 0425 0218 115f 5f69 6e64 6578 5f6c 6576  .%...__index_lev
-00000510: 656c 5f30 5f5f 0016 0419 1c19 6c26 d801  el_0__......l&..
-00000520: 1c15 0419 3510 0006 1918 0269 6415 0216  ....5......id...
-00000530: 0416 c801 16d0 0126 4826 081c 1808 d102  .......&H&......
-00000540: 0000 0000 0000 1808 be02 0000 0000 0000  ................
-00000550: 1600 2808 d102 0000 0000 0000 1808 be02  ..(.............
-00000560: 0000 0000 0000 0019 2c15 0415 0015 0200  ........,.......
-00000570: 1500 1510 1502 0000 0026 e004 1c15 0a19  .........&......
-00000580: 3510 0006 1918 0272 6115 0216 0416 c801  5......ra.......
-00000590: 16d0 0126 d003 2690 031c 1808 0000 0000  ...&..&.........
-000005a0: 00a8 7340 1808 0000 0000 0068 7340 1600  ..s@.......hs@..
-000005b0: 2808 0000 0000 00a8 7340 1808 0000 0000  (.......s@......
-000005c0: 0068 7340 0019 2c15 0415 0015 0200 1500  .hs@..,.........
-000005d0: 1510 1502 0000 0026 ec07 1c15 0a19 3510  .......&......5.
-000005e0: 0006 1918 0364 6563 1502 1604 16c8 0116  .....dec........
-000005f0: d001 26dc 0626 9c06 1c18 0800 0000 0000  ..&..&..........
-00000600: 803b c018 0800 0000 0000 4041 c016 0028  .;........@A...(
-00000610: 0800 0000 0000 803b c018 0800 0000 0000  .......;........
-00000620: 4041 c000 192c 1504 1500 1502 0015 0015  @A...,..........
-00000630: 1015 0200 0000 26ea 0a1c 1504 1935 1000  ......&......5..
-00000640: 0619 1808 7261 5f65 7272 6f72 1502 1604  ....ra_error....
-00000650: 16b8 0116 c001 26da 0926 aa09 1c18 0800  ......&..&......
-00000660: 0000 0000 0000 0018 0800 0000 0000 0000  ................
-00000670: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
-00000680: 0000 0000 0000 0000 192c 1504 1500 1502  .........,......
-00000690: 0015 0015 1015 0200 0000 26f2 0d1c 1504  ..........&.....
-000006a0: 1935 1000 0619 1809 6465 635f 6572 726f  .5......dec_erro
-000006b0: 7215 0216 0416 b801 16c0 0126 e20c 26b2  r..........&..&.
-000006c0: 0c1c 1808 0000 0000 0000 0000 1808 0000  ................
-000006d0: 0000 0000 0000 1600 2808 0000 0000 0000  ........(.......
-000006e0: 0000 1808 0000 0000 0000 0000 0019 2c15  ..............,.
-000006f0: 0415 0015 0200 1500 1510 1502 0000 0026  ...............&
-00000700: 8c11 1c15 0419 3510 0006 1918 115f 5f69  ......5......__i
-00000710: 6e64 6578 5f6c 6576 656c 5f30 5f5f 1502  ndex_level_0__..
-00000720: 1604 16c8 0116 d001 26fc 0f26 bc0f 1c18  ........&..&....
-00000730: 0815 0000 0000 0000 0018 0802 0000 0000  ................
-00000740: 0000 0016 0028 0815 0000 0000 0000 0018  .....(..........
-00000750: 0802 0000 0000 0000 0000 192c 1504 1500  ...........,....
-00000760: 1502 0015 0015 1015 0200 0000 1690 0916  ................
-00000770: 0426 0816 c009 1400 0019 2c18 0670 616e  .&........,..pan
-00000780: 6461 7318 a507 7b22 696e 6465 785f 636f  das...{"index_co
-00000790: 6c75 6d6e 7322 3a20 5b22 5f5f 696e 6465  lumns": ["__inde
-000007a0: 785f 6c65 7665 6c5f 305f 5f22 5d2c 2022  x_level_0__"], "
-000007b0: 636f 6c75 6d6e 5f69 6e64 6578 6573 223a  column_indexes":
-000007c0: 205b 7b22 6e61 6d65 223a 206e 756c 6c2c   [{"name": null,
-000007d0: 2022 6669 656c 645f 6e61 6d65 223a 206e   "field_name": n
-000007e0: 756c 6c2c 2022 7061 6e64 6173 5f74 7970  ull, "pandas_typ
-000007f0: 6522 3a20 2275 6e69 636f 6465 222c 2022  e": "unicode", "
-00000800: 6e75 6d70 795f 7479 7065 223a 2022 6f62  numpy_type": "ob
-00000810: 6a65 6374 222c 2022 6d65 7461 6461 7461  ject", "metadata
-00000820: 223a 207b 2265 6e63 6f64 696e 6722 3a20  ": {"encoding": 
-00000830: 2255 5446 2d38 227d 7d5d 2c20 2263 6f6c  "UTF-8"}}], "col
-00000840: 756d 6e73 223a 205b 7b22 6e61 6d65 223a  umns": [{"name":
-00000850: 2022 6964 222c 2022 6669 656c 645f 6e61   "id", "field_na
-00000860: 6d65 223a 2022 6964 222c 2022 7061 6e64  me": "id", "pand
-00000870: 6173 5f74 7970 6522 3a20 2269 6e74 3634  as_type": "int64
-00000880: 222c 2022 6e75 6d70 795f 7479 7065 223a  ", "numpy_type":
-00000890: 2022 696e 7436 3422 2c20 226d 6574 6164   "int64", "metad
-000008a0: 6174 6122 3a20 6e75 6c6c 7d2c 207b 226e  ata": null}, {"n
-000008b0: 616d 6522 3a20 2272 6122 2c20 2266 6965  ame": "ra", "fie
-000008c0: 6c64 5f6e 616d 6522 3a20 2272 6122 2c20  ld_name": "ra", 
-000008d0: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
-000008e0: 666c 6f61 7436 3422 2c20 226e 756d 7079  float64", "numpy
-000008f0: 5f74 7970 6522 3a20 2266 6c6f 6174 3634  _type": "float64
-00000900: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
-00000910: 756c 6c7d 2c20 7b22 6e61 6d65 223a 2022  ull}, {"name": "
-00000920: 6465 6322 2c20 2266 6965 6c64 5f6e 616d  dec", "field_nam
-00000930: 6522 3a20 2264 6563 222c 2022 7061 6e64  e": "dec", "pand
-00000940: 6173 5f74 7970 6522 3a20 2266 6c6f 6174  as_type": "float
-00000950: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
-00000960: 223a 2022 666c 6f61 7436 3422 2c20 226d  ": "float64", "m
-00000970: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
-00000980: 207b 226e 616d 6522 3a20 2272 615f 6572   {"name": "ra_er
-00000990: 726f 7222 2c20 2266 6965 6c64 5f6e 616d  ror", "field_nam
-000009a0: 6522 3a20 2272 615f 6572 726f 7222 2c20  e": "ra_error", 
-000009b0: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
-000009c0: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
-000009d0: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
-000009e0: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
-000009f0: 2c20 7b22 6e61 6d65 223a 2022 6465 635f  , {"name": "dec_
-00000a00: 6572 726f 7222 2c20 2266 6965 6c64 5f6e  error", "field_n
-00000a10: 616d 6522 3a20 2264 6563 5f65 7272 6f72  ame": "dec_error
-00000a20: 222c 2022 7061 6e64 6173 5f74 7970 6522  ", "pandas_type"
-00000a30: 3a20 2269 6e74 3634 222c 2022 6e75 6d70  : "int64", "nump
-00000a40: 795f 7479 7065 223a 2022 696e 7436 3422  y_type": "int64"
-00000a50: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
-00000a60: 6c6c 7d2c 207b 226e 616d 6522 3a20 6e75  ll}, {"name": nu
-00000a70: 6c6c 2c20 2266 6965 6c64 5f6e 616d 6522  ll, "field_name"
-00000a80: 3a20 225f 5f69 6e64 6578 5f6c 6576 656c  : "__index_level
-00000a90: 5f30 5f5f 222c 2022 7061 6e64 6173 5f74  _0__", "pandas_t
-00000aa0: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
-00000ab0: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
-00000ac0: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
-00000ad0: 3a20 6e75 6c6c 7d5d 2c20 2263 7265 6174  : null}], "creat
-00000ae0: 6f72 223a 207b 226c 6962 7261 7279 223a  or": {"library":
-00000af0: 2022 7079 6172 726f 7722 2c20 2276 6572   "pyarrow", "ver
-00000b00: 7369 6f6e 223a 2022 392e 302e 3022 7d2c  sion": "9.0.0"},
-00000b10: 2022 7061 6e64 6173 5f76 6572 7369 6f6e   "pandas_version
-00000b20: 223a 2022 312e 332e 3522 7d00 180c 4152  ": "1.3.5"}...AR
-00000b30: 524f 573a 7363 6865 6d61 18c0 0e2f 2f2f  ROW:schema...///
-00000b40: 2f2f 3267 4641 4141 5141 4141 4141 4141  //2gFAAAQAAAAAAA
-00000b50: 4b41 4134 4142 6741 4641 4167 4143 6741  KAA4ABgAFAAgACgA
-00000b60: 4141 4141 4242 4141 5141 4141 4141 4141  AAAABBAAQAAAAAAA
-00000b70: 4b41 4177 4141 4141 4541 4167 4143 6741  KAAwAAAAEAAgACgA
-00000b80: 4141 4e77 4441 4141 4541 4141 4141 5141  AANwDAAAEAAAAAQA
-00000b90: 4141 4177 4141 4141 4941 4177 4142 4141  AAAwAAAAIAAwABAA
-00000ba0: 4941 4167 4141 4141 4941 4141 4145 4141  IAAgAAAAIAAAAEAA
-00000bb0: 4141 4159 4141 4142 7759 5735 6b59 584d  AAAYAAABwYW5kYXM
-00000bc0: 4141 4b55 4441 4142 3749 6d6c 755a 4756  AAKUDAAB7ImluZGV
-00000bd0: 3458 324e 7662 4856 7462 6e4d 694f 6942  4X2NvbHVtbnMiOiB
-00000be0: 6249 6c39 6661 5735 6b5a 5868 6662 4756  bIl9faW5kZXhfbGV
-00000bf0: 325a 5778 664d 4639 6649 6c30 7349 434a  2ZWxfMF9fIl0sICJ
-00000c00: 6a62 3278 3162 5735 6661 5735 6b5a 5868  jb2x1bW5faW5kZXh
-00000c10: 6c63 7949 3649 4674 3749 6d35 6862 5755  lcyI6IFt7Im5hbWU
-00000c20: 694f 6942 7564 5778 734c 4341 695a 6d6c  iOiBudWxsLCAiZml
-00000c30: 6c62 4752 6662 6d46 745a 5349 3649 4735  lbGRfbmFtZSI6IG5
-00000c40: 3162 4777 7349 434a 7759 5735 6b59 584e  1bGwsICJwYW5kYXN
-00000c50: 6664 486c 775a 5349 3649 434a 3162 6d6c  fdHlwZSI6ICJ1bml
-00000c60: 6a62 3252 6c49 6977 6749 6d35 3162 5842  jb2RlIiwgIm51bXB
-00000c70: 3558 3352 3563 4755 694f 6941 6962 324a  5X3R5cGUiOiAib2J
-00000c80: 715a 574e 3049 6977 6749 6d31 6c64 4746  qZWN0IiwgIm1ldGF
-00000c90: 6b59 5852 6849 6a6f 6765 794a 6c62 6d4e  kYXRhIjogeyJlbmN
-00000ca0: 765a 476c 755a 7949 3649 434a 5656 4559  vZGluZyI6ICJVVEY
-00000cb0: 744f 434a 3966 5630 7349 434a 6a62 3278  tOCJ9fV0sICJjb2x
-00000cc0: 3162 5735 7a49 6a6f 6757 3373 6962 6d46  1bW5zIjogW3sibmF
-00000cd0: 745a 5349 3649 434a 705a 4349 7349 434a  tZSI6ICJpZCIsICJ
-00000ce0: 6d61 5756 735a 4639 7559 5731 6c49 6a6f  maWVsZF9uYW1lIjo
-00000cf0: 6749 6d6c 6b49 6977 6749 6e42 6862 6d52  gImlkIiwgInBhbmR
-00000d00: 6863 3139 3065 5842 6c49 6a6f 6749 6d6c  hc190eXBlIjogIml
-00000d10: 7564 4459 3049 6977 6749 6d35 3162 5842  udDY0IiwgIm51bXB
-00000d20: 3558 3352 3563 4755 694f 6941 6961 5735  5X3R5cGUiOiAiaW5
-00000d30: 304e 6a51 694c 4341 6962 5756 3059 5752  0NjQiLCAibWV0YWR
-00000d40: 6864 4745 694f 6942 7564 5778 7366 5377  hdGEiOiBudWxsfSw
-00000d50: 6765 794a 7559 5731 6c49 6a6f 6749 6e4a  geyJuYW1lIjogInJ
-00000d60: 6849 6977 6749 6d5a 705a 5778 6b58 3235  hIiwgImZpZWxkX25
-00000d70: 6862 5755 694f 6941 6963 6d45 694c 4341  hbWUiOiAicmEiLCA
-00000d80: 6963 4746 755a 4746 7a58 3352 3563 4755  icGFuZGFzX3R5cGU
-00000d90: 694f 6941 695a 6d78 7659 5851 324e 4349  iOiAiZmxvYXQ2NCI
-00000da0: 7349 434a 7564 5731 7765 5639 3065 5842  sICJudW1weV90eXB
-00000db0: 6c49 6a6f 6749 6d5a 7362 3246 304e 6a51  lIjogImZsb2F0NjQ
-00000dc0: 694c 4341 6962 5756 3059 5752 6864 4745  iLCAibWV0YWRhdGE
-00000dd0: 694f 6942 7564 5778 7366 5377 6765 794a  iOiBudWxsfSwgeyJ
-00000de0: 7559 5731 6c49 6a6f 6749 6d52 6c59 7949  uYW1lIjogImRlYyI
-00000df0: 7349 434a 6d61 5756 735a 4639 7559 5731  sICJmaWVsZF9uYW1
-00000e00: 6c49 6a6f 6749 6d52 6c59 7949 7349 434a  lIjogImRlYyIsICJ
-00000e10: 7759 5735 6b59 584e 6664 486c 775a 5349  wYW5kYXNfdHlwZSI
-00000e20: 3649 434a 6d62 4739 6864 4459 3049 6977  6ICJmbG9hdDY0Iiw
-00000e30: 6749 6d35 3162 5842 3558 3352 3563 4755  gIm51bXB5X3R5cGU
-00000e40: 694f 6941 695a 6d78 7659 5851 324e 4349  iOiAiZmxvYXQ2NCI
-00000e50: 7349 434a 745a 5852 685a 4746 3059 5349  sICJtZXRhZGF0YSI
-00000e60: 3649 4735 3162 4778 394c 4342 3749 6d35  6IG51bGx9LCB7Im5
-00000e70: 6862 5755 694f 6941 6963 6d46 665a 584a  hbWUiOiAicmFfZXJ
-00000e80: 7962 3349 694c 4341 695a 6d6c 6c62 4752  yb3IiLCAiZmllbGR
-00000e90: 6662 6d46 745a 5349 3649 434a 7959 5639  fbmFtZSI6ICJyYV9
-00000ea0: 6c63 6e4a 7663 6949 7349 434a 7759 5735  lcnJvciIsICJwYW5
-00000eb0: 6b59 584e 6664 486c 775a 5349 3649 434a  kYXNfdHlwZSI6ICJ
-00000ec0: 7062 6e51 324e 4349 7349 434a 7564 5731  pbnQ2NCIsICJudW1
-00000ed0: 7765 5639 3065 5842 6c49 6a6f 6749 6d6c  weV90eXBlIjogIml
-00000ee0: 7564 4459 3049 6977 6749 6d31 6c64 4746  udDY0IiwgIm1ldGF
-00000ef0: 6b59 5852 6849 6a6f 6762 6e56 7362 4830  kYXRhIjogbnVsbH0
-00000f00: 7349 4873 6962 6d46 745a 5349 3649 434a  sIHsibmFtZSI6ICJ
-00000f10: 6b5a 574e 665a 584a 7962 3349 694c 4341  kZWNfZXJyb3IiLCA
-00000f20: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
-00000f30: 3649 434a 6b5a 574e 665a 584a 7962 3349  6ICJkZWNfZXJyb3I
-00000f40: 694c 4341 6963 4746 755a 4746 7a58 3352  iLCAicGFuZGFzX3R
-00000f50: 3563 4755 694f 6941 6961 5735 304e 6a51  5cGUiOiAiaW50NjQ
-00000f60: 694c 4341 6962 6e56 7463 486c 6664 486c  iLCAibnVtcHlfdHl
-00000f70: 775a 5349 3649 434a 7062 6e51 324e 4349  wZSI6ICJpbnQ2NCI
-00000f80: 7349 434a 745a 5852 685a 4746 3059 5349  sICJtZXRhZGF0YSI
-00000f90: 3649 4735 3162 4778 394c 4342 3749 6d35  6IG51bGx9LCB7Im5
-00000fa0: 6862 5755 694f 6942 7564 5778 734c 4341  hbWUiOiBudWxsLCA
-00000fb0: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
-00000fc0: 3649 434a 6658 326c 755a 4756 3458 3278  6ICJfX2luZGV4X2x
-00000fd0: 6c64 6d56 7358 7a42 6658 7949 7349 434a  ldmVsXzBfXyIsICJ
-00000fe0: 7759 5735 6b59 584e 6664 486c 775a 5349  wYW5kYXNfdHlwZSI
-00000ff0: 3649 434a 7062 6e51 324e 4349 7349 434a  6ICJpbnQ2NCIsICJ
-00001000: 7564 5731 7765 5639 3065 5842 6c49 6a6f  udW1weV90eXBlIjo
-00001010: 6749 6d6c 7564 4459 3049 6977 6749 6d31  gImludDY0IiwgIm1
-00001020: 6c64 4746 6b59 5852 6849 6a6f 6762 6e56  ldGFkYXRhIjogbnV
-00001030: 7362 4831 644c 4341 6959 334a 6c59 5852  sbH1dLCAiY3JlYXR
-00001040: 7663 6949 3649 4873 6962 476c 6963 6d46  vciI6IHsibGlicmF
-00001050: 7965 5349 3649 434a 7765 5746 7963 6d39  yeSI6ICJweWFycm9
-00001060: 3349 6977 6749 6e5a 6c63 6e4e 7062 3234  3IiwgInZlcnNpb24
-00001070: 694f 6941 694f 5334 774c 6a41 6966 5377  iOiAiOS4wLjAifSw
-00001080: 6749 6e42 6862 6d52 6863 3139 325a 584a  gInBhbmRhc192ZXJ
-00001090: 7a61 5739 7549 6a6f 6749 6a45 754d 7934  zaW9uIjogIjEuMy4
-000010a0: 3149 6e30 4141 4141 4741 4141 414a 4145  1In0AAAAGAAAAJAE
-000010b0: 4141 4f41 4141 4143 3041 4141 4166 4141  AAOAAAAC0AAAAfAA
-000010c0: 4141 4551 4141 4141 4541 4141 4142 502f  AAEQAAAAEAAAABP/
-000010d0: 2f2f 7741 4141 5149 5141 4141 414a 4141  //wAAAQIQAAAAJAA
-000010e0: 4141 4151 4141 4141 4141 4141 4145 5141  AAAQAAAAAAAAAEQA
-000010f0: 4141 4639 6661 5735 6b5a 5868 6662 4756  AAF9faW5kZXhfbGV
-00001100: 325a 5778 664d 4639 6641 4141 4142 502f  2ZWxfMF9fAAAABP/
-00001110: 2f2f 7741 4141 4146 4141 4141 4151 502f  //wAAAAFAAAAAQP/
-00001120: 2f2f 7741 4141 5149 5141 4141 4148 4141  //wAAAQIQAAAAHAA
-00001130: 4141 4151 4141 4141 4141 4141 4143 5141  AAAQAAAAAAAAACQA
-00001140: 4141 4752 6c59 3139 6c63 6e4a 7663 6741  AAGRlY19lcnJvcgA
-00001150: 4141 446a 2f2f 2f38 4141 4141 4251 4141  AADj///8AAAABQAA
-00001160: 4141 4854 2f2f 2f38 4141 4145 4345 4141  AAHT///8AAAECEAA
-00001170: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
-00001180: 4141 4167 4141 4142 7959 5639 6c63 6e4a  AAAgAAAByYV9lcnJ
-00001190: 7663 6741 4141 4142 732f 2f2f 2f41 4141  vcgAAAABs////AAA
-000011a0: 4141 5541 4141 4143 6f2f 2f2f 2f41 4141  AAUAAAACo////AAA
-000011b0: 4241 7841 4141 4141 5541 4141 4142 4141  BAxAAAAAUAAAABAA
-000011c0: 4141 4141 4141 4141 4441 4141 415a 4756  AAAAAAAADAAAAZGV
-000011d0: 6a41 4e62 2f2f 2f38 4141 4149 4130 502f  jANb///8AAAIA0P/
-000011e0: 2f2f 7741 4141 514d 5141 4141 4148 4141  //wAAAQMQAAAAHAA
-000011f0: 4141 4151 4141 4141 4141 4141 4141 6741  AAAQAAAAAAAAAAgA
-00001200: 4141 484a 6841 4141 4141 4159 4143 4141  AAHJhAAAAAAYACAA
-00001210: 4741 4159 4141 4141 4141 4149 4145 4141  GAAYAAAAAAAIAEAA
-00001220: 5541 4167 4142 6741 4841 4177 4141 4141  UAAgABgAHAAwAAAA
-00001230: 5141 4241 4141 4141 4141 4145 4345 4141  QABAAAAAAAAECEAA
-00001240: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
-00001250: 4141 4149 4141 4142 705a 4141 4143 4141  AAAIAAABpZAAACAA
-00001260: 4d41 4167 4142 7741 4941 4141 4141 4141  MAAgABwAIAAAAAAA
-00001270: 4141 5541 4141 4141 4141 4141 4100 181f  AAUAAAAAAAAAA...
-00001280: 7061 7271 7565 742d 6370 702d 6172 726f  parquet-cpp-arro
-00001290: 7720 7665 7273 696f 6e20 392e 302e 3019  w version 9.0.0.
-000012a0: 6c1c 0000 1c00 001c 0000 1c00 001c 0000  l...............
-000012b0: 1c00 0000 010e 0000 5041 5231            ........PAR1
+000003e0: 196c 3500 1806 7363 6865 6d61 150a 0015  .l5...schema....
+000003f0: 0425 0218 0269 6400 150a 2502 1802 7261  .%...id...%...ra
+00000400: 0015 0a25 0218 0364 6563 0015 0425 0218  ...%...dec...%..
+00000410: 0872 615f 6572 726f 7200 1504 2502 1809  .ra_error...%...
+00000420: 6465 635f 6572 726f 7200 1604 191c 195c  dec_error......\
+00000430: 26d8 011c 1504 1935 1000 0619 1802 6964  &......5......id
+00000440: 1502 1604 16c8 0116 d001 2648 2608 1c18  ..........&H&...
+00000450: 08d1 0200 0000 0000 0018 08be 0200 0000  ................
+00000460: 0000 0016 0028 08d1 0200 0000 0000 0018  .....(..........
+00000470: 08be 0200 0000 0000 0000 192c 1504 1500  ...........,....
+00000480: 1502 0015 0015 1015 0200 0000 26e0 041c  ............&...
+00000490: 150a 1935 1000 0619 1802 7261 1502 1604  ...5......ra....
+000004a0: 16c8 0116 d001 26d0 0326 9003 1c18 0800  ......&..&......
+000004b0: 0000 0000 a873 4018 0800 0000 0000 6873  .....s@.......hs
+000004c0: 4016 0028 0800 0000 0000 a873 4018 0800  @..(.......s@...
+000004d0: 0000 0000 6873 4000 192c 1504 1500 1502  ....hs@..,......
+000004e0: 0015 0015 1015 0200 0000 26ec 071c 150a  ..........&.....
+000004f0: 1935 1000 0619 1803 6465 6315 0216 0416  .5......dec.....
+00000500: c801 16d0 0126 dc06 269c 061c 1808 0000  .....&..&.......
+00000510: 0000 0080 3bc0 1808 0000 0000 0040 41c0  ....;........@A.
+00000520: 1600 2808 0000 0000 0080 3bc0 1808 0000  ..(.......;.....
+00000530: 0000 0040 41c0 0019 2c15 0415 0015 0200  ...@A...,.......
+00000540: 1500 1510 1502 0000 0026 ea0a 1c15 0419  .........&......
+00000550: 3510 0006 1918 0872 615f 6572 726f 7215  5......ra_error.
+00000560: 0216 0416 b801 16c0 0126 da09 26aa 091c  .........&..&...
+00000570: 1808 0000 0000 0000 0000 1808 0000 0000  ................
+00000580: 0000 0000 1600 2808 0000 0000 0000 0000  ......(.........
+00000590: 1808 0000 0000 0000 0000 0019 2c15 0415  ............,...
+000005a0: 0015 0200 1500 1510 1502 0000 0026 f20d  .............&..
+000005b0: 1c15 0419 3510 0006 1918 0964 6563 5f65  ....5......dec_e
+000005c0: 7272 6f72 1502 1604 16b8 0116 c001 26e2  rror..........&.
+000005d0: 0c26 b20c 1c18 0800 0000 0000 0000 0018  .&..............
+000005e0: 0800 0000 0000 0000 0016 0028 0800 0000  ...........(....
+000005f0: 0000 0000 0018 0800 0000 0000 0000 0000  ................
+00000600: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
+00000610: 0000 16c8 0716 0426 0816 f007 1400 0019  .......&........
+00000620: 2c18 0670 616e 6461 7318 a705 7b22 696e  ,..pandas...{"in
+00000630: 6465 785f 636f 6c75 6d6e 7322 3a20 5b5d  dex_columns": []
+00000640: 2c20 2263 6f6c 756d 6e5f 696e 6465 7865  , "column_indexe
+00000650: 7322 3a20 5b5d 2c20 2263 6f6c 756d 6e73  s": [], "columns
+00000660: 223a 205b 7b22 6e61 6d65 223a 2022 6964  ": [{"name": "id
+00000670: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
+00000680: 2022 6964 222c 2022 7061 6e64 6173 5f74   "id", "pandas_t
+00000690: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
+000006a0: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
+000006b0: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
+000006c0: 3a20 6e75 6c6c 7d2c 207b 226e 616d 6522  : null}, {"name"
+000006d0: 3a20 2272 6122 2c20 2266 6965 6c64 5f6e  : "ra", "field_n
+000006e0: 616d 6522 3a20 2272 6122 2c20 2270 616e  ame": "ra", "pan
+000006f0: 6461 735f 7479 7065 223a 2022 666c 6f61  das_type": "floa
+00000700: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
+00000710: 6522 3a20 2266 6c6f 6174 3634 222c 2022  e": "float64", "
+00000720: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
+00000730: 2c20 7b22 6e61 6d65 223a 2022 6465 6322  , {"name": "dec"
+00000740: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
+00000750: 2264 6563 222c 2022 7061 6e64 6173 5f74  "dec", "pandas_t
+00000760: 7970 6522 3a20 2266 6c6f 6174 3634 222c  ype": "float64",
+00000770: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
+00000780: 666c 6f61 7436 3422 2c20 226d 6574 6164  float64", "metad
+00000790: 6174 6122 3a20 6e75 6c6c 7d2c 207b 226e  ata": null}, {"n
+000007a0: 616d 6522 3a20 2272 615f 6572 726f 7222  ame": "ra_error"
+000007b0: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
+000007c0: 2272 615f 6572 726f 7222 2c20 2270 616e  "ra_error", "pan
+000007d0: 6461 735f 7479 7065 223a 2022 696e 7436  das_type": "int6
+000007e0: 3422 2c20 226e 756d 7079 5f74 7970 6522  4", "numpy_type"
+000007f0: 3a20 2269 6e74 3634 222c 2022 6d65 7461  : "int64", "meta
+00000800: 6461 7461 223a 206e 756c 6c7d 2c20 7b22  data": null}, {"
+00000810: 6e61 6d65 223a 2022 6465 635f 6572 726f  name": "dec_erro
+00000820: 7222 2c20 2266 6965 6c64 5f6e 616d 6522  r", "field_name"
+00000830: 3a20 2264 6563 5f65 7272 6f72 222c 2022  : "dec_error", "
+00000840: 7061 6e64 6173 5f74 7970 6522 3a20 2269  pandas_type": "i
+00000850: 6e74 3634 222c 2022 6e75 6d70 795f 7479  nt64", "numpy_ty
+00000860: 7065 223a 2022 696e 7436 3422 2c20 226d  pe": "int64", "m
+00000870: 6574 6164 6174 6122 3a20 6e75 6c6c 7d5d  etadata": null}]
+00000880: 2c20 2263 7265 6174 6f72 223a 207b 226c  , "creator": {"l
+00000890: 6962 7261 7279 223a 2022 7079 6172 726f  ibrary": "pyarro
+000008a0: 7722 2c20 2276 6572 7369 6f6e 223a 2022  w", "version": "
+000008b0: 392e 302e 3022 7d2c 2022 7061 6e64 6173  9.0.0"}, "pandas
+000008c0: 5f76 6572 7369 6f6e 223a 2022 322e 302e  _version": "2.0.
+000008d0: 3022 7d00 180c 4152 524f 573a 7363 6865  0"}...ARROW:sche
+000008e0: 6d61 1898 0b2f 2f2f 2f2f 7967 4541 4141  ma.../////ygEAAA
+000008f0: 5141 4141 4141 4141 4b41 4134 4142 6741  QAAAAAAAKAA4ABgA
+00000900: 4641 4167 4143 6741 4141 4141 4242 4141  FAAgACgAAAAABBAA
+00000910: 5141 4141 4141 4141 4b41 4177 4141 4141  QAAAAAAAKAAwAAAA
+00000920: 4541 4167 4143 6741 4141 4e77 4341 4141  EAAgACgAAANwCAAA
+00000930: 4541 4141 4141 5141 4141 4177 4141 4141  EAAAAAQAAAAwAAAA
+00000940: 4941 4177 4142 4141 4941 4167 4141 4141  IAAwABAAIAAgAAAA
+00000950: 4941 4141 4145 4141 4141 4159 4141 4142  IAAAAEAAAAAYAAAB
+00000960: 7759 5735 6b59 584d 4141 4b63 4341 4142  wYW5kYXMAAKcCAAB
+00000970: 3749 6d6c 755a 4756 3458 324e 7662 4856  7ImluZGV4X2NvbHV
+00000980: 7462 6e4d 694f 6942 6258 5377 6749 6d4e  tbnMiOiBbXSwgImN
+00000990: 7662 4856 7462 6c39 7062 6d52 6c65 4756  vbHVtbl9pbmRleGV
+000009a0: 7a49 6a6f 6757 3130 7349 434a 6a62 3278  zIjogW10sICJjb2x
+000009b0: 3162 5735 7a49 6a6f 6757 3373 6962 6d46  1bW5zIjogW3sibmF
+000009c0: 745a 5349 3649 434a 705a 4349 7349 434a  tZSI6ICJpZCIsICJ
+000009d0: 6d61 5756 735a 4639 7559 5731 6c49 6a6f  maWVsZF9uYW1lIjo
+000009e0: 6749 6d6c 6b49 6977 6749 6e42 6862 6d52  gImlkIiwgInBhbmR
+000009f0: 6863 3139 3065 5842 6c49 6a6f 6749 6d6c  hc190eXBlIjogIml
+00000a00: 7564 4459 3049 6977 6749 6d35 3162 5842  udDY0IiwgIm51bXB
+00000a10: 3558 3352 3563 4755 694f 6941 6961 5735  5X3R5cGUiOiAiaW5
+00000a20: 304e 6a51 694c 4341 6962 5756 3059 5752  0NjQiLCAibWV0YWR
+00000a30: 6864 4745 694f 6942 7564 5778 7366 5377  hdGEiOiBudWxsfSw
+00000a40: 6765 794a 7559 5731 6c49 6a6f 6749 6e4a  geyJuYW1lIjogInJ
+00000a50: 6849 6977 6749 6d5a 705a 5778 6b58 3235  hIiwgImZpZWxkX25
+00000a60: 6862 5755 694f 6941 6963 6d45 694c 4341  hbWUiOiAicmEiLCA
+00000a70: 6963 4746 755a 4746 7a58 3352 3563 4755  icGFuZGFzX3R5cGU
+00000a80: 694f 6941 695a 6d78 7659 5851 324e 4349  iOiAiZmxvYXQ2NCI
+00000a90: 7349 434a 7564 5731 7765 5639 3065 5842  sICJudW1weV90eXB
+00000aa0: 6c49 6a6f 6749 6d5a 7362 3246 304e 6a51  lIjogImZsb2F0NjQ
+00000ab0: 694c 4341 6962 5756 3059 5752 6864 4745  iLCAibWV0YWRhdGE
+00000ac0: 694f 6942 7564 5778 7366 5377 6765 794a  iOiBudWxsfSwgeyJ
+00000ad0: 7559 5731 6c49 6a6f 6749 6d52 6c59 7949  uYW1lIjogImRlYyI
+00000ae0: 7349 434a 6d61 5756 735a 4639 7559 5731  sICJmaWVsZF9uYW1
+00000af0: 6c49 6a6f 6749 6d52 6c59 7949 7349 434a  lIjogImRlYyIsICJ
+00000b00: 7759 5735 6b59 584e 6664 486c 775a 5349  wYW5kYXNfdHlwZSI
+00000b10: 3649 434a 6d62 4739 6864 4459 3049 6977  6ICJmbG9hdDY0Iiw
+00000b20: 6749 6d35 3162 5842 3558 3352 3563 4755  gIm51bXB5X3R5cGU
+00000b30: 694f 6941 695a 6d78 7659 5851 324e 4349  iOiAiZmxvYXQ2NCI
+00000b40: 7349 434a 745a 5852 685a 4746 3059 5349  sICJtZXRhZGF0YSI
+00000b50: 3649 4735 3162 4778 394c 4342 3749 6d35  6IG51bGx9LCB7Im5
+00000b60: 6862 5755 694f 6941 6963 6d46 665a 584a  hbWUiOiAicmFfZXJ
+00000b70: 7962 3349 694c 4341 695a 6d6c 6c62 4752  yb3IiLCAiZmllbGR
+00000b80: 6662 6d46 745a 5349 3649 434a 7959 5639  fbmFtZSI6ICJyYV9
+00000b90: 6c63 6e4a 7663 6949 7349 434a 7759 5735  lcnJvciIsICJwYW5
+00000ba0: 6b59 584e 6664 486c 775a 5349 3649 434a  kYXNfdHlwZSI6ICJ
+00000bb0: 7062 6e51 324e 4349 7349 434a 7564 5731  pbnQ2NCIsICJudW1
+00000bc0: 7765 5639 3065 5842 6c49 6a6f 6749 6d6c  weV90eXBlIjogIml
+00000bd0: 7564 4459 3049 6977 6749 6d31 6c64 4746  udDY0IiwgIm1ldGF
+00000be0: 6b59 5852 6849 6a6f 6762 6e56 7362 4830  kYXRhIjogbnVsbH0
+00000bf0: 7349 4873 6962 6d46 745a 5349 3649 434a  sIHsibmFtZSI6ICJ
+00000c00: 6b5a 574e 665a 584a 7962 3349 694c 4341  kZWNfZXJyb3IiLCA
+00000c10: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
+00000c20: 3649 434a 6b5a 574e 665a 584a 7962 3349  6ICJkZWNfZXJyb3I
+00000c30: 694c 4341 6963 4746 755a 4746 7a58 3352  iLCAicGFuZGFzX3R
+00000c40: 3563 4755 694f 6941 6961 5735 304e 6a51  5cGUiOiAiaW50NjQ
+00000c50: 694c 4341 6962 6e56 7463 486c 6664 486c  iLCAibnVtcHlfdHl
+00000c60: 775a 5349 3649 434a 7062 6e51 324e 4349  wZSI6ICJpbnQ2NCI
+00000c70: 7349 434a 745a 5852 685a 4746 3059 5349  sICJtZXRhZGF0YSI
+00000c80: 3649 4735 3162 4778 3958 5377 6749 6d4e  6IG51bGx9XSwgImN
+00000c90: 795a 5746 3062 3349 694f 6942 3749 6d78  yZWF0b3IiOiB7Imx
+00000ca0: 7059 6e4a 6863 6e6b 694f 6941 6963 486c  pYnJhcnkiOiAicHl
+00000cb0: 6863 6e4a 7664 7949 7349 434a 325a 584a  hcnJvdyIsICJ2ZXJ
+00000cc0: 7a61 5739 7549 6a6f 6749 6a6b 754d 4334  zaW9uIjogIjkuMC4
+00000cd0: 7749 6e30 7349 434a 7759 5735 6b59 584e  wIn0sICJwYW5kYXN
+00000ce0: 6664 6d56 7963 326c 7662 6949 3649 4349  fdmVyc2lvbiI6ICI
+00000cf0: 794c 6a41 754d 434a 3941 4155 4141 4144  yLjAuMCJ9AAUAAAD
+00000d00: 6b41 4141 416f 4141 4141 4851 4141 4141  kAAAAoAAAAHQAAAA
+00000d10: 3841 4141 4142 4141 4141 4544 2f2f 2f38  8AAAABAAAAED///8
+00000d20: 4141 4145 4345 4141 4141 4277 4141 4141  AAAECEAAAABwAAAA
+00000d30: 4541 4141 4141 4141 4141 416b 4141 4142  EAAAAAAAAAAkAAAB
+00000d40: 6b5a 574e 665a 584a 7962 3349 4141 4141  kZWNfZXJyb3IAAAA
+00000d50: 342f 2f2f 2f41 4141 4141 5541 4141 4142  4////AAAAAUAAAAB
+00000d60: 302f 2f2f 2f41 4141 4241 6841 4141 4141  0////AAABAhAAAAA
+00000d70: 6341 4141 4142 4141 4141 4141 4141 4141  cAAAABAAAAAAAAAA
+00000d80: 4941 4141 4163 6d46 665a 584a 7962 3349  IAAAAcmFfZXJyb3I
+00000d90: 4141 4141 4162 502f 2f2f 7741 4141 4146  AAAAAbP///wAAAAF
+00000da0: 4141 4141 4171 502f 2f2f 7741 4141 514d  AAAAAqP///wAAAQM
+00000db0: 5141 4141 4146 4141 4141 4151 4141 4141  QAAAAFAAAAAQAAAA
+00000dc0: 4141 4141 4141 7741 4141 4752 6c59 7744  AAAAAAwAAAGRlYwD
+00000dd0: 572f 2f2f 2f41 4141 4341 4e44 2f2f 2f38  W////AAACAND///8
+00000de0: 4141 4145 4445 4141 4141 4277 4141 4141  AAAEDEAAAABwAAAA
+00000df0: 4541 4141 4141 4141 4141 4149 4141 4142  EAAAAAAAAAAIAAAB
+00000e00: 7959 5141 4141 4141 4741 4167 4142 6741  yYQAAAAAGAAgABgA
+00000e10: 4741 4141 4141 4141 4341 4241 4146 4141  GAAAAAAACABAAFAA
+00000e20: 4941 4159 4142 7741 4d41 4141 4145 4141  IAAYABwAMAAAAEAA
+00000e30: 5141 4141 4141 4141 4241 6841 4141 4141  QAAAAAAABAhAAAAA
+00000e40: 6341 4141 4142 4141 4141 4141 4141 4141  cAAAABAAAAAAAAAA
+00000e50: 4341 4141 4161 5751 4141 4167 4144 4141  CAAAAaWQAAAgADAA
+00000e60: 4941 4163 4143 4141 4141 4141 4141 4146  IAAcACAAAAAAAAAF
+00000e70: 4141 4141 4141 4141 4141 413d 3d00 181f  AAAAAAAAAAA==...
+00000e80: 7061 7271 7565 742d 6370 702d 6172 726f  parquet-cpp-arro
+00000e90: 7720 7665 7273 696f 6e20 392e 302e 3019  w version 9.0.0.
+00000ea0: 5c1c 0000 1c00 001c 0000 1c00 001c 0000  \...............
+00000eb0: 00d3 0a00 0050 4152 31                   .....PAR1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_47/shard_2.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet`

 * *Files 18% similar despite different names*

```diff
@@ -57,246 +57,181 @@
 00000380: 0000 0009 2002 0000 0006 0101 0600 269c  .... .........&.
 00000390: 0e1c 1504 1935 1000 0619 1809 6465 635f  .....5......dec_
 000003a0: 6572 726f 7215 0216 0616 b801 16c0 0126  error..........&
 000003b0: 8c0d 26dc 0c1c 1808 0000 0000 0000 0000  ..&.............
 000003c0: 1808 0000 0000 0000 0000 1600 2808 0000  ............(...
 000003d0: 0000 0000 0000 1808 0000 0000 0000 0000  ................
 000003e0: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
-000003f0: 0000 0015 0415 3015 2e4c 1506 1500 1200  ......0..L......
-00000400: 0018 0403 0009 013c 0500 0000 0000 0000  .......<........
-00000410: 1000 0000 0000 0000 1500 1514 1518 2c15  ..............,.
-00000420: 0615 1015 0615 061c 1808 1000 0000 0000  ................
-00000430: 0000 1808 0300 0000 0000 0000 1600 2808  ..............(.
-00000440: 1000 0000 0000 0000 1808 0300 0000 0000  ................
-00000450: 0000 0000 000a 2402 0000 0006 0102 0324  ......$........$
-00000460: 0026 c211 1c15 0419 3510 0006 1918 115f  .&......5......_
-00000470: 5f69 6e64 6578 5f6c 6576 656c 5f30 5f5f  _index_level_0__
-00000480: 1502 1606 16da 0116 dc01 26b0 1026 e60f  ..........&..&..
-00000490: 1c18 0810 0000 0000 0000 0018 0803 0000  ................
-000004a0: 0000 0000 0016 0028 0810 0000 0000 0000  .......(........
-000004b0: 0018 0803 0000 0000 0000 0000 192c 1504  .............,..
-000004c0: 1500 1502 0015 0015 1015 0200 0000 1504  ................
-000004d0: 197c 3500 1806 7363 6865 6d61 150c 0015  .|5...schema....
-000004e0: 0425 0218 0269 6400 150a 2502 1802 7261  .%...id...%...ra
-000004f0: 0015 0a25 0218 0364 6563 0015 0425 0218  ...%...dec...%..
-00000500: 0872 615f 6572 726f 7200 1504 2502 1809  .ra_error...%...
-00000510: 6465 635f 6572 726f 7200 1504 2502 1811  dec_error...%...
-00000520: 5f5f 696e 6465 785f 6c65 7665 6c5f 305f  __index_level_0_
-00000530: 5f00 1606 191c 196c 26e6 011c 1504 1935  _......l&......5
-00000540: 1000 0619 1802 6964 1502 1606 16da 0116  ......id........
-00000550: de01 2654 2608 1c18 08ff 0200 0000 0000  ..&T&...........
-00000560: 0018 08f2 0200 0000 0000 0016 0028 08ff  .............(..
-00000570: 0200 0000 0000 0018 08f2 0200 0000 0000  ................
-00000580: 0000 192c 1504 1500 1502 0015 0015 1015  ...,............
-00000590: 0200 0000 26fc 041c 150a 1935 1000 0619  ....&......5....
-000005a0: 1802 7261 1502 1606 16da 0116 de01 26ea  ..ra..........&.
-000005b0: 0326 9e03 1c18 0800 0000 0000 f873 4018  .&...........s@.
-000005c0: 0800 0000 0000 9873 4016 0028 0800 0000  .......s@..(....
-000005d0: 0000 f873 4018 0800 0000 0000 9873 4000  ...s@........s@.
-000005e0: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
-000005f0: 0000 2696 081c 150a 1935 1000 0619 1803  ..&......5......
-00000600: 6465 6315 0216 0616 da01 16de 0126 8407  dec..........&..
-00000610: 26b8 061c 1808 0000 0000 0080 3dc0 1808  &...........=...
-00000620: 0000 0000 00c0 41c0 1600 2808 0000 0000  ......A...(.....
-00000630: 0080 3dc0 1808 0000 0000 00c0 41c0 0019  ..=.........A...
-00000640: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
-00000650: 0026 940b 1c15 0419 3510 0006 1918 0872  .&......5......r
-00000660: 615f 6572 726f 7215 0216 0616 b801 16c0  a_error.........
-00000670: 0126 840a 26d4 091c 1808 0000 0000 0000  .&..&...........
-00000680: 0000 1808 0000 0000 0000 0000 1600 2808  ..............(.
-00000690: 0000 0000 0000 0000 1808 0000 0000 0000  ................
-000006a0: 0000 0019 2c15 0415 0015 0200 1500 1510  ....,...........
-000006b0: 1502 0000 0026 9c0e 1c15 0419 3510 0006  .....&......5...
-000006c0: 1918 0964 6563 5f65 7272 6f72 1502 1606  ...dec_error....
-000006d0: 16b8 0116 c001 268c 0d26 dc0c 1c18 0800  ......&..&......
-000006e0: 0000 0000 0000 0018 0800 0000 0000 0000  ................
-000006f0: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
-00000700: 0000 0000 0000 0000 192c 1504 1500 1502  .........,......
-00000710: 0015 0015 1015 0200 0000 26c2 111c 1504  ..........&.....
-00000720: 1935 1000 0619 1811 5f5f 696e 6465 785f  .5......__index_
-00000730: 6c65 7665 6c5f 305f 5f15 0216 0616 da01  level_0__.......
-00000740: 16dc 0126 b010 26e6 0f1c 1808 1000 0000  ...&..&.........
-00000750: 0000 0000 1808 0300 0000 0000 0000 1600  ................
-00000760: 2808 1000 0000 0000 0000 1808 0300 0000  (...............
-00000770: 0000 0000 0019 2c15 0415 0015 0200 1500  ......,.........
-00000780: 1510 1502 0000 0016 d809 1606 2608 16f6  ............&...
-00000790: 0914 0000 192c 1806 7061 6e64 6173 18a5  .....,..pandas..
-000007a0: 077b 2269 6e64 6578 5f63 6f6c 756d 6e73  .{"index_columns
-000007b0: 223a 205b 225f 5f69 6e64 6578 5f6c 6576  ": ["__index_lev
-000007c0: 656c 5f30 5f5f 225d 2c20 2263 6f6c 756d  el_0__"], "colum
-000007d0: 6e5f 696e 6465 7865 7322 3a20 5b7b 226e  n_indexes": [{"n
-000007e0: 616d 6522 3a20 6e75 6c6c 2c20 2266 6965  ame": null, "fie
-000007f0: 6c64 5f6e 616d 6522 3a20 6e75 6c6c 2c20  ld_name": null, 
-00000800: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
-00000810: 756e 6963 6f64 6522 2c20 226e 756d 7079  unicode", "numpy
-00000820: 5f74 7970 6522 3a20 226f 626a 6563 7422  _type": "object"
-00000830: 2c20 226d 6574 6164 6174 6122 3a20 7b22  , "metadata": {"
-00000840: 656e 636f 6469 6e67 223a 2022 5554 462d  encoding": "UTF-
-00000850: 3822 7d7d 5d2c 2022 636f 6c75 6d6e 7322  8"}}], "columns"
-00000860: 3a20 5b7b 226e 616d 6522 3a20 2269 6422  : [{"name": "id"
-00000870: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
-00000880: 2269 6422 2c20 2270 616e 6461 735f 7479  "id", "pandas_ty
-00000890: 7065 223a 2022 696e 7436 3422 2c20 226e  pe": "int64", "n
-000008a0: 756d 7079 5f74 7970 6522 3a20 2269 6e74  umpy_type": "int
-000008b0: 3634 222c 2022 6d65 7461 6461 7461 223a  64", "metadata":
-000008c0: 206e 756c 6c7d 2c20 7b22 6e61 6d65 223a   null}, {"name":
-000008d0: 2022 7261 222c 2022 6669 656c 645f 6e61   "ra", "field_na
-000008e0: 6d65 223a 2022 7261 222c 2022 7061 6e64  me": "ra", "pand
-000008f0: 6173 5f74 7970 6522 3a20 2266 6c6f 6174  as_type": "float
-00000900: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
-00000910: 223a 2022 666c 6f61 7436 3422 2c20 226d  ": "float64", "m
-00000920: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
-00000930: 207b 226e 616d 6522 3a20 2264 6563 222c   {"name": "dec",
-00000940: 2022 6669 656c 645f 6e61 6d65 223a 2022   "field_name": "
-00000950: 6465 6322 2c20 2270 616e 6461 735f 7479  dec", "pandas_ty
-00000960: 7065 223a 2022 666c 6f61 7436 3422 2c20  pe": "float64", 
-00000970: 226e 756d 7079 5f74 7970 6522 3a20 2266  "numpy_type": "f
-00000980: 6c6f 6174 3634 222c 2022 6d65 7461 6461  loat64", "metada
-00000990: 7461 223a 206e 756c 6c7d 2c20 7b22 6e61  ta": null}, {"na
-000009a0: 6d65 223a 2022 7261 5f65 7272 6f72 222c  me": "ra_error",
-000009b0: 2022 6669 656c 645f 6e61 6d65 223a 2022   "field_name": "
-000009c0: 7261 5f65 7272 6f72 222c 2022 7061 6e64  ra_error", "pand
-000009d0: 6173 5f74 7970 6522 3a20 2269 6e74 3634  as_type": "int64
-000009e0: 222c 2022 6e75 6d70 795f 7479 7065 223a  ", "numpy_type":
-000009f0: 2022 696e 7436 3422 2c20 226d 6574 6164   "int64", "metad
-00000a00: 6174 6122 3a20 6e75 6c6c 7d2c 207b 226e  ata": null}, {"n
-00000a10: 616d 6522 3a20 2264 6563 5f65 7272 6f72  ame": "dec_error
-00000a20: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
-00000a30: 2022 6465 635f 6572 726f 7222 2c20 2270   "dec_error", "p
-00000a40: 616e 6461 735f 7479 7065 223a 2022 696e  andas_type": "in
-00000a50: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
-00000a60: 6522 3a20 2269 6e74 3634 222c 2022 6d65  e": "int64", "me
-00000a70: 7461 6461 7461 223a 206e 756c 6c7d 2c20  tadata": null}, 
-00000a80: 7b22 6e61 6d65 223a 206e 756c 6c2c 2022  {"name": null, "
-00000a90: 6669 656c 645f 6e61 6d65 223a 2022 5f5f  field_name": "__
-00000aa0: 696e 6465 785f 6c65 7665 6c5f 305f 5f22  index_level_0__"
-00000ab0: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
-00000ac0: 2022 696e 7436 3422 2c20 226e 756d 7079   "int64", "numpy
-00000ad0: 5f74 7970 6522 3a20 2269 6e74 3634 222c  _type": "int64",
-00000ae0: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
-00000af0: 6c7d 5d2c 2022 6372 6561 746f 7222 3a20  l}], "creator": 
-00000b00: 7b22 6c69 6272 6172 7922 3a20 2270 7961  {"library": "pya
-00000b10: 7272 6f77 222c 2022 7665 7273 696f 6e22  rrow", "version"
-00000b20: 3a20 2239 2e30 2e30 227d 2c20 2270 616e  : "9.0.0"}, "pan
-00000b30: 6461 735f 7665 7273 696f 6e22 3a20 2231  das_version": "1
-00000b40: 2e33 2e35 227d 0018 0c41 5252 4f57 3a73  .3.5"}...ARROW:s
-00000b50: 6368 656d 6118 c00e 2f2f 2f2f 2f32 6746  chema.../////2gF
-00000b60: 4141 4151 4141 4141 4141 414b 4141 3441  AAAQAAAAAAAKAA4A
-00000b70: 4267 4146 4141 6741 4367 4141 4141 4142  BgAFAAgACgAAAAAB
-00000b80: 4241 4151 4141 4141 4141 414b 4141 7741  BAAQAAAAAAAKAAwA
-00000b90: 4141 4145 4141 6741 4367 4141 414e 7744  AAAEAAgACgAAANwD
-00000ba0: 4141 4145 4141 4141 4151 4141 4141 7741  AAAEAAAAAQAAAAwA
-00000bb0: 4141 4149 4141 7741 4241 4149 4141 6741  AAAIAAwABAAIAAgA
-00000bc0: 4141 4149 4141 4141 4541 4141 4141 5941  AAAIAAAAEAAAAAYA
-00000bd0: 4141 4277 5957 356b 5958 4d41 414b 5544  AABwYW5kYXMAAKUD
-00000be0: 4141 4237 496d 6c75 5a47 5634 5832 4e76  AAB7ImluZGV4X2Nv
-00000bf0: 6248 5674 626e 4d69 4f69 4262 496c 3966  bHVtbnMiOiBbIl9f
-00000c00: 6157 356b 5a58 6866 6247 5632 5a57 7866  aW5kZXhfbGV2ZWxf
-00000c10: 4d46 3966 496c 3073 4943 4a6a 6232 7831  MF9fIl0sICJjb2x1
-00000c20: 6257 3566 6157 356b 5a58 686c 6379 4936  bW5faW5kZXhlcyI6
-00000c30: 4946 7437 496d 3568 6257 5569 4f69 4275  IFt7Im5hbWUiOiBu
-00000c40: 6457 7873 4c43 4169 5a6d 6c6c 6247 5266  dWxsLCAiZmllbGRf
-00000c50: 626d 4674 5a53 4936 4947 3531 6247 7773  bmFtZSI6IG51bGws
-00000c60: 4943 4a77 5957 356b 5958 4e66 6448 6c77  ICJwYW5kYXNfdHlw
-00000c70: 5a53 4936 4943 4a31 626d 6c6a 6232 526c  ZSI6ICJ1bmljb2Rl
-00000c80: 4969 7767 496d 3531 6258 4235 5833 5235  IiwgIm51bXB5X3R5
-00000c90: 6347 5569 4f69 4169 6232 4a71 5a57 4e30  cGUiOiAib2JqZWN0
-00000ca0: 4969 7767 496d 316c 6447 466b 5958 5268  IiwgIm1ldGFkYXRh
-00000cb0: 496a 6f67 6579 4a6c 626d 4e76 5a47 6c75  IjogeyJlbmNvZGlu
-00000cc0: 5a79 4936 4943 4a56 5645 5974 4f43 4a39  ZyI6ICJVVEYtOCJ9
-00000cd0: 6656 3073 4943 4a6a 6232 7831 6257 357a  fV0sICJjb2x1bW5z
-00000ce0: 496a 6f67 5733 7369 626d 4674 5a53 4936  IjogW3sibmFtZSI6
-00000cf0: 4943 4a70 5a43 4973 4943 4a6d 6157 5673  ICJpZCIsICJmaWVs
-00000d00: 5a46 3975 5957 316c 496a 6f67 496d 6c6b  ZF9uYW1lIjogImlk
-00000d10: 4969 7767 496e 4268 626d 5268 6331 3930  IiwgInBhbmRhc190
-00000d20: 6558 426c 496a 6f67 496d 6c75 6444 5930  eXBlIjogImludDY0
-00000d30: 4969 7767 496d 3531 6258 4235 5833 5235  IiwgIm51bXB5X3R5
-00000d40: 6347 5569 4f69 4169 6157 3530 4e6a 5169  cGUiOiAiaW50NjQi
-00000d50: 4c43 4169 6257 5630 5957 5268 6447 4569  LCAibWV0YWRhdGEi
-00000d60: 4f69 4275 6457 7873 6653 7767 6579 4a75  OiBudWxsfSwgeyJu
-00000d70: 5957 316c 496a 6f67 496e 4a68 4969 7767  YW1lIjogInJhIiwg
-00000d80: 496d 5a70 5a57 786b 5832 3568 6257 5569  ImZpZWxkX25hbWUi
-00000d90: 4f69 4169 636d 4569 4c43 4169 6347 4675  OiAicmEiLCAicGFu
-00000da0: 5a47 467a 5833 5235 6347 5569 4f69 4169  ZGFzX3R5cGUiOiAi
-00000db0: 5a6d 7876 5958 5132 4e43 4973 4943 4a75  ZmxvYXQ2NCIsICJu
-00000dc0: 6457 3177 6556 3930 6558 426c 496a 6f67  dW1weV90eXBlIjog
-00000dd0: 496d 5a73 6232 4630 4e6a 5169 4c43 4169  ImZsb2F0NjQiLCAi
-00000de0: 6257 5630 5957 5268 6447 4569 4f69 4275  bWV0YWRhdGEiOiBu
-00000df0: 6457 7873 6653 7767 6579 4a75 5957 316c  dWxsfSwgeyJuYW1l
-00000e00: 496a 6f67 496d 526c 5979 4973 4943 4a6d  IjogImRlYyIsICJm
-00000e10: 6157 5673 5a46 3975 5957 316c 496a 6f67  aWVsZF9uYW1lIjog
-00000e20: 496d 526c 5979 4973 4943 4a77 5957 356b  ImRlYyIsICJwYW5k
-00000e30: 5958 4e66 6448 6c77 5a53 4936 4943 4a6d  YXNfdHlwZSI6ICJm
-00000e40: 6247 3968 6444 5930 4969 7767 496d 3531  bG9hdDY0IiwgIm51
-00000e50: 6258 4235 5833 5235 6347 5569 4f69 4169  bXB5X3R5cGUiOiAi
-00000e60: 5a6d 7876 5958 5132 4e43 4973 4943 4a74  ZmxvYXQ2NCIsICJt
-00000e70: 5a58 5268 5a47 4630 5953 4936 4947 3531  ZXRhZGF0YSI6IG51
-00000e80: 6247 7839 4c43 4237 496d 3568 6257 5569  bGx9LCB7Im5hbWUi
-00000e90: 4f69 4169 636d 4666 5a58 4a79 6233 4969  OiAicmFfZXJyb3Ii
-00000ea0: 4c43 4169 5a6d 6c6c 6247 5266 626d 4674  LCAiZmllbGRfbmFt
-00000eb0: 5a53 4936 4943 4a79 5956 396c 636e 4a76  ZSI6ICJyYV9lcnJv
-00000ec0: 6369 4973 4943 4a77 5957 356b 5958 4e66  ciIsICJwYW5kYXNf
-00000ed0: 6448 6c77 5a53 4936 4943 4a70 626e 5132  dHlwZSI6ICJpbnQ2
-00000ee0: 4e43 4973 4943 4a75 6457 3177 6556 3930  NCIsICJudW1weV90
-00000ef0: 6558 426c 496a 6f67 496d 6c75 6444 5930  eXBlIjogImludDY0
-00000f00: 4969 7767 496d 316c 6447 466b 5958 5268  IiwgIm1ldGFkYXRh
-00000f10: 496a 6f67 626e 5673 6248 3073 4948 7369  IjogbnVsbH0sIHsi
-00000f20: 626d 4674 5a53 4936 4943 4a6b 5a57 4e66  bmFtZSI6ICJkZWNf
-00000f30: 5a58 4a79 6233 4969 4c43 4169 5a6d 6c6c  ZXJyb3IiLCAiZmll
-00000f40: 6247 5266 626d 4674 5a53 4936 4943 4a6b  bGRfbmFtZSI6ICJk
-00000f50: 5a57 4e66 5a58 4a79 6233 4969 4c43 4169  ZWNfZXJyb3IiLCAi
-00000f60: 6347 4675 5a47 467a 5833 5235 6347 5569  cGFuZGFzX3R5cGUi
-00000f70: 4f69 4169 6157 3530 4e6a 5169 4c43 4169  OiAiaW50NjQiLCAi
-00000f80: 626e 5674 6348 6c66 6448 6c77 5a53 4936  bnVtcHlfdHlwZSI6
-00000f90: 4943 4a70 626e 5132 4e43 4973 4943 4a74  ICJpbnQ2NCIsICJt
-00000fa0: 5a58 5268 5a47 4630 5953 4936 4947 3531  ZXRhZGF0YSI6IG51
-00000fb0: 6247 7839 4c43 4237 496d 3568 6257 5569  bGx9LCB7Im5hbWUi
-00000fc0: 4f69 4275 6457 7873 4c43 4169 5a6d 6c6c  OiBudWxsLCAiZmll
-00000fd0: 6247 5266 626d 4674 5a53 4936 4943 4a66  bGRfbmFtZSI6ICJf
-00000fe0: 5832 6c75 5a47 5634 5832 786c 646d 5673  X2luZGV4X2xldmVs
-00000ff0: 587a 4266 5879 4973 4943 4a77 5957 356b  XzBfXyIsICJwYW5k
-00001000: 5958 4e66 6448 6c77 5a53 4936 4943 4a70  YXNfdHlwZSI6ICJp
-00001010: 626e 5132 4e43 4973 4943 4a75 6457 3177  bnQ2NCIsICJudW1w
-00001020: 6556 3930 6558 426c 496a 6f67 496d 6c75  eV90eXBlIjogImlu
-00001030: 6444 5930 4969 7767 496d 316c 6447 466b  dDY0IiwgIm1ldGFk
-00001040: 5958 5268 496a 6f67 626e 5673 6248 3164  YXRhIjogbnVsbH1d
-00001050: 4c43 4169 5933 4a6c 5958 5276 6369 4936  LCAiY3JlYXRvciI6
-00001060: 4948 7369 6247 6c69 636d 4679 6553 4936  IHsibGlicmFyeSI6
-00001070: 4943 4a77 6557 4679 636d 3933 4969 7767  ICJweWFycm93Iiwg
-00001080: 496e 5a6c 636e 4e70 6232 3469 4f69 4169  InZlcnNpb24iOiAi
-00001090: 4f53 3477 4c6a 4169 6653 7767 496e 4268  OS4wLjAifSwgInBh
-000010a0: 626d 5268 6331 3932 5a58 4a7a 6157 3975  bmRhc192ZXJzaW9u
-000010b0: 496a 6f67 496a 4575 4d79 3431 496e 3041  IjogIjEuMy41In0A
-000010c0: 4141 4147 4141 4141 4a41 4541 414f 4141  AAAGAAAAJAEAAOAA
-000010d0: 4141 4330 4141 4141 6641 4141 4145 5141  AAC0AAAAfAAAAEQA
-000010e0: 4141 4145 4141 4141 4250 2f2f 2f77 4141  AAAEAAAABP///wAA
-000010f0: 4151 4951 4141 4141 4a41 4141 4141 5141  AQIQAAAAJAAAAAQA
-00001100: 4141 4141 4141 4141 4551 4141 4146 3966  AAAAAAAAEQAAAF9f
-00001110: 6157 356b 5a58 6866 6247 5632 5a57 7866  aW5kZXhfbGV2ZWxf
-00001120: 4d46 3966 4141 4141 4250 2f2f 2f77 4141  MF9fAAAABP///wAA
-00001130: 4141 4641 4141 4141 5150 2f2f 2f77 4141  AAFAAAAAQP///wAA
-00001140: 4151 4951 4141 4141 4841 4141 4141 5141  AQIQAAAAHAAAAAQA
-00001150: 4141 4141 4141 4141 4351 4141 4147 526c  AAAAAAAACQAAAGRl
-00001160: 5931 396c 636e 4a76 6367 4141 4144 6a2f  Y19lcnJvcgAAADj/
-00001170: 2f2f 3841 4141 4142 5141 4141 4148 542f  //8AAAABQAAAAHT/
-00001180: 2f2f 3841 4141 4543 4541 4141 4142 7741  //8AAAECEAAAABwA
-00001190: 4141 4145 4141 4141 4141 4141 4141 6741  AAAEAAAAAAAAAAgA
-000011a0: 4141 4279 5956 396c 636e 4a76 6367 4141  AAByYV9lcnJvcgAA
-000011b0: 4141 4273 2f2f 2f2f 4141 4141 4155 4141  AABs////AAAAAUAA
-000011c0: 4141 436f 2f2f 2f2f 4141 4142 4178 4141  AACo////AAABAxAA
-000011d0: 4141 4155 4141 4141 4241 4141 4141 4141  AAAUAAAABAAAAAAA
-000011e0: 4141 4144 4141 4141 5a47 566a 414e 622f  AAADAAAAZGVjANb/
-000011f0: 2f2f 3841 4141 4941 3050 2f2f 2f77 4141  //8AAAIA0P///wAA
-00001200: 4151 4d51 4141 4141 4841 4141 4141 5141  AQMQAAAAHAAAAAQA
-00001210: 4141 4141 4141 4141 4167 4141 4148 4a68  AAAAAAAAAgAAAHJh
-00001220: 4141 4141 4141 5941 4341 4147 4141 5941  AAAAAAYACAAGAAYA
-00001230: 4141 4141 4141 4941 4541 4155 4141 6741  AAAAAAIAEAAUAAgA
-00001240: 4267 4148 4141 7741 4141 4151 4142 4141  BgAHAAwAAAAQABAA
-00001250: 4141 4141 4141 4543 4541 4141 4142 7741  AAAAAAECEAAAABwA
-00001260: 4141 4145 4141 4141 4141 4141 4141 4941  AAAEAAAAAAAAAAIA
-00001270: 4141 4270 5a41 4141 4341 414d 4141 6741  AABpZAAACAAMAAgA
-00001280: 4277 4149 4141 4141 4141 4141 4155 4141  BwAIAAAAAAAAAUAA
-00001290: 4141 4141 4141 4141 0018 1f70 6172 7175  AAAAAAAA...parqu
-000012a0: 6574 2d63 7070 2d61 7272 6f77 2076 6572  et-cpp-arrow ver
-000012b0: 7369 6f6e 2039 2e30 2e30 196c 1c00 001c  sion 9.0.0.l....
-000012c0: 0000 1c00 001c 0000 1c00 001c 0000 0001  ................
-000012d0: 0e00 0050 4152 31                        ...PAR1
+000003f0: 0000 0015 0419 6c35 0018 0673 6368 656d  ......l5...schem
+00000400: 6115 0a00 1504 2502 1802 6964 0015 0a25  a.....%...id...%
+00000410: 0218 0272 6100 150a 2502 1803 6465 6300  ...ra...%...dec.
+00000420: 1504 2502 1808 7261 5f65 7272 6f72 0015  ..%...ra_error..
+00000430: 0425 0218 0964 6563 5f65 7272 6f72 0016  .%...dec_error..
+00000440: 0619 1c19 5c26 e601 1c15 0419 3510 0006  ....\&......5...
+00000450: 1918 0269 6415 0216 0616 da01 16de 0126  ...id..........&
+00000460: 5426 081c 1808 ff02 0000 0000 0000 1808  T&..............
+00000470: f202 0000 0000 0000 1600 2808 ff02 0000  ..........(.....
+00000480: 0000 0000 1808 f202 0000 0000 0000 0019  ................
+00000490: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
+000004a0: 0026 fc04 1c15 0a19 3510 0006 1918 0272  .&......5......r
+000004b0: 6115 0216 0616 da01 16de 0126 ea03 269e  a..........&..&.
+000004c0: 031c 1808 0000 0000 00f8 7340 1808 0000  ..........s@....
+000004d0: 0000 0098 7340 1600 2808 0000 0000 00f8  ....s@..(.......
+000004e0: 7340 1808 0000 0000 0098 7340 0019 2c15  s@........s@..,.
+000004f0: 0415 0015 0200 1500 1510 1502 0000 0026  ...............&
+00000500: 9608 1c15 0a19 3510 0006 1918 0364 6563  ......5......dec
+00000510: 1502 1606 16da 0116 de01 2684 0726 b806  ..........&..&..
+00000520: 1c18 0800 0000 0000 803d c018 0800 0000  .........=......
+00000530: 0000 c041 c016 0028 0800 0000 0000 803d  ...A...(.......=
+00000540: c018 0800 0000 0000 c041 c000 192c 1504  .........A...,..
+00000550: 1500 1502 0015 0015 1015 0200 0000 2694  ..............&.
+00000560: 0b1c 1504 1935 1000 0619 1808 7261 5f65  .....5......ra_e
+00000570: 7272 6f72 1502 1606 16b8 0116 c001 2684  rror..........&.
+00000580: 0a26 d409 1c18 0800 0000 0000 0000 0018  .&..............
+00000590: 0800 0000 0000 0000 0016 0028 0800 0000  ...........(....
+000005a0: 0000 0000 0018 0800 0000 0000 0000 0000  ................
+000005b0: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
+000005c0: 0000 269c 0e1c 1504 1935 1000 0619 1809  ..&......5......
+000005d0: 6465 635f 6572 726f 7215 0216 0616 b801  dec_error.......
+000005e0: 16c0 0126 8c0d 26dc 0c1c 1808 0000 0000  ...&..&.........
+000005f0: 0000 0000 1808 0000 0000 0000 0000 1600  ................
+00000600: 2808 0000 0000 0000 0000 1808 0000 0000  (...............
+00000610: 0000 0000 0019 2c15 0415 0015 0200 1500  ......,.........
+00000620: 1510 1502 0000 0016 fe07 1606 2608 169a  ............&...
+00000630: 0814 0000 192c 1806 7061 6e64 6173 18a7  .....,..pandas..
+00000640: 057b 2269 6e64 6578 5f63 6f6c 756d 6e73  .{"index_columns
+00000650: 223a 205b 5d2c 2022 636f 6c75 6d6e 5f69  ": [], "column_i
+00000660: 6e64 6578 6573 223a 205b 5d2c 2022 636f  ndexes": [], "co
+00000670: 6c75 6d6e 7322 3a20 5b7b 226e 616d 6522  lumns": [{"name"
+00000680: 3a20 2269 6422 2c20 2266 6965 6c64 5f6e  : "id", "field_n
+00000690: 616d 6522 3a20 2269 6422 2c20 2270 616e  ame": "id", "pan
+000006a0: 6461 735f 7479 7065 223a 2022 696e 7436  das_type": "int6
+000006b0: 3422 2c20 226e 756d 7079 5f74 7970 6522  4", "numpy_type"
+000006c0: 3a20 2269 6e74 3634 222c 2022 6d65 7461  : "int64", "meta
+000006d0: 6461 7461 223a 206e 756c 6c7d 2c20 7b22  data": null}, {"
+000006e0: 6e61 6d65 223a 2022 7261 222c 2022 6669  name": "ra", "fi
+000006f0: 656c 645f 6e61 6d65 223a 2022 7261 222c  eld_name": "ra",
+00000700: 2022 7061 6e64 6173 5f74 7970 6522 3a20   "pandas_type": 
+00000710: 2266 6c6f 6174 3634 222c 2022 6e75 6d70  "float64", "nump
+00000720: 795f 7479 7065 223a 2022 666c 6f61 7436  y_type": "float6
+00000730: 3422 2c20 226d 6574 6164 6174 6122 3a20  4", "metadata": 
+00000740: 6e75 6c6c 7d2c 207b 226e 616d 6522 3a20  null}, {"name": 
+00000750: 2264 6563 222c 2022 6669 656c 645f 6e61  "dec", "field_na
+00000760: 6d65 223a 2022 6465 6322 2c20 2270 616e  me": "dec", "pan
+00000770: 6461 735f 7479 7065 223a 2022 666c 6f61  das_type": "floa
+00000780: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
+00000790: 6522 3a20 2266 6c6f 6174 3634 222c 2022  e": "float64", "
+000007a0: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
+000007b0: 2c20 7b22 6e61 6d65 223a 2022 7261 5f65  , {"name": "ra_e
+000007c0: 7272 6f72 222c 2022 6669 656c 645f 6e61  rror", "field_na
+000007d0: 6d65 223a 2022 7261 5f65 7272 6f72 222c  me": "ra_error",
+000007e0: 2022 7061 6e64 6173 5f74 7970 6522 3a20   "pandas_type": 
+000007f0: 2269 6e74 3634 222c 2022 6e75 6d70 795f  "int64", "numpy_
+00000800: 7479 7065 223a 2022 696e 7436 3422 2c20  type": "int64", 
+00000810: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
+00000820: 7d2c 207b 226e 616d 6522 3a20 2264 6563  }, {"name": "dec
+00000830: 5f65 7272 6f72 222c 2022 6669 656c 645f  _error", "field_
+00000840: 6e61 6d65 223a 2022 6465 635f 6572 726f  name": "dec_erro
+00000850: 7222 2c20 2270 616e 6461 735f 7479 7065  r", "pandas_type
+00000860: 223a 2022 696e 7436 3422 2c20 226e 756d  ": "int64", "num
+00000870: 7079 5f74 7970 6522 3a20 2269 6e74 3634  py_type": "int64
+00000880: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
+00000890: 756c 6c7d 5d2c 2022 6372 6561 746f 7222  ull}], "creator"
+000008a0: 3a20 7b22 6c69 6272 6172 7922 3a20 2270  : {"library": "p
+000008b0: 7961 7272 6f77 222c 2022 7665 7273 696f  yarrow", "versio
+000008c0: 6e22 3a20 2239 2e30 2e30 227d 2c20 2270  n": "9.0.0"}, "p
+000008d0: 616e 6461 735f 7665 7273 696f 6e22 3a20  andas_version": 
+000008e0: 2232 2e30 2e30 227d 0018 0c41 5252 4f57  "2.0.0"}...ARROW
+000008f0: 3a73 6368 656d 6118 980b 2f2f 2f2f 2f79  :schema.../////y
+00000900: 6745 4141 4151 4141 4141 4141 414b 4141  gEAAAQAAAAAAAKAA
+00000910: 3441 4267 4146 4141 6741 4367 4141 4141  4ABgAFAAgACgAAAA
+00000920: 4142 4241 4151 4141 4141 4141 414b 4141  ABBAAQAAAAAAAKAA
+00000930: 7741 4141 4145 4141 6741 4367 4141 414e  wAAAAEAAgACgAAAN
+00000940: 7743 4141 4145 4141 4141 4151 4141 4141  wCAAAEAAAAAQAAAA
+00000950: 7741 4141 4149 4141 7741 4241 4149 4141  wAAAAIAAwABAAIAA
+00000960: 6741 4141 4149 4141 4141 4541 4141 4141  gAAAAIAAAAEAAAAA
+00000970: 5941 4141 4277 5957 356b 5958 4d41 414b  YAAABwYW5kYXMAAK
+00000980: 6343 4141 4237 496d 6c75 5a47 5634 5832  cCAAB7ImluZGV4X2
+00000990: 4e76 6248 5674 626e 4d69 4f69 4262 5853  NvbHVtbnMiOiBbXS
+000009a0: 7767 496d 4e76 6248 5674 626c 3970 626d  wgImNvbHVtbl9pbm
+000009b0: 526c 6547 567a 496a 6f67 5731 3073 4943  RleGVzIjogW10sIC
+000009c0: 4a6a 6232 7831 6257 357a 496a 6f67 5733  Jjb2x1bW5zIjogW3
+000009d0: 7369 626d 4674 5a53 4936 4943 4a70 5a43  sibmFtZSI6ICJpZC
+000009e0: 4973 4943 4a6d 6157 5673 5a46 3975 5957  IsICJmaWVsZF9uYW
+000009f0: 316c 496a 6f67 496d 6c6b 4969 7767 496e  1lIjogImlkIiwgIn
+00000a00: 4268 626d 5268 6331 3930 6558 426c 496a  BhbmRhc190eXBlIj
+00000a10: 6f67 496d 6c75 6444 5930 4969 7767 496d  ogImludDY0IiwgIm
+00000a20: 3531 6258 4235 5833 5235 6347 5569 4f69  51bXB5X3R5cGUiOi
+00000a30: 4169 6157 3530 4e6a 5169 4c43 4169 6257  AiaW50NjQiLCAibW
+00000a40: 5630 5957 5268 6447 4569 4f69 4275 6457  V0YWRhdGEiOiBudW
+00000a50: 7873 6653 7767 6579 4a75 5957 316c 496a  xsfSwgeyJuYW1lIj
+00000a60: 6f67 496e 4a68 4969 7767 496d 5a70 5a57  ogInJhIiwgImZpZW
+00000a70: 786b 5832 3568 6257 5569 4f69 4169 636d  xkX25hbWUiOiAicm
+00000a80: 4569 4c43 4169 6347 4675 5a47 467a 5833  EiLCAicGFuZGFzX3
+00000a90: 5235 6347 5569 4f69 4169 5a6d 7876 5958  R5cGUiOiAiZmxvYX
+00000aa0: 5132 4e43 4973 4943 4a75 6457 3177 6556  Q2NCIsICJudW1weV
+00000ab0: 3930 6558 426c 496a 6f67 496d 5a73 6232  90eXBlIjogImZsb2
+00000ac0: 4630 4e6a 5169 4c43 4169 6257 5630 5957  F0NjQiLCAibWV0YW
+00000ad0: 5268 6447 4569 4f69 4275 6457 7873 6653  RhdGEiOiBudWxsfS
+00000ae0: 7767 6579 4a75 5957 316c 496a 6f67 496d  wgeyJuYW1lIjogIm
+00000af0: 526c 5979 4973 4943 4a6d 6157 5673 5a46  RlYyIsICJmaWVsZF
+00000b00: 3975 5957 316c 496a 6f67 496d 526c 5979  9uYW1lIjogImRlYy
+00000b10: 4973 4943 4a77 5957 356b 5958 4e66 6448  IsICJwYW5kYXNfdH
+00000b20: 6c77 5a53 4936 4943 4a6d 6247 3968 6444  lwZSI6ICJmbG9hdD
+00000b30: 5930 4969 7767 496d 3531 6258 4235 5833  Y0IiwgIm51bXB5X3
+00000b40: 5235 6347 5569 4f69 4169 5a6d 7876 5958  R5cGUiOiAiZmxvYX
+00000b50: 5132 4e43 4973 4943 4a74 5a58 5268 5a47  Q2NCIsICJtZXRhZG
+00000b60: 4630 5953 4936 4947 3531 6247 7839 4c43  F0YSI6IG51bGx9LC
+00000b70: 4237 496d 3568 6257 5569 4f69 4169 636d  B7Im5hbWUiOiAicm
+00000b80: 4666 5a58 4a79 6233 4969 4c43 4169 5a6d  FfZXJyb3IiLCAiZm
+00000b90: 6c6c 6247 5266 626d 4674 5a53 4936 4943  llbGRfbmFtZSI6IC
+00000ba0: 4a79 5956 396c 636e 4a76 6369 4973 4943  JyYV9lcnJvciIsIC
+00000bb0: 4a77 5957 356b 5958 4e66 6448 6c77 5a53  JwYW5kYXNfdHlwZS
+00000bc0: 4936 4943 4a70 626e 5132 4e43 4973 4943  I6ICJpbnQ2NCIsIC
+00000bd0: 4a75 6457 3177 6556 3930 6558 426c 496a  JudW1weV90eXBlIj
+00000be0: 6f67 496d 6c75 6444 5930 4969 7767 496d  ogImludDY0IiwgIm
+00000bf0: 316c 6447 466b 5958 5268 496a 6f67 626e  1ldGFkYXRhIjogbn
+00000c00: 5673 6248 3073 4948 7369 626d 4674 5a53  VsbH0sIHsibmFtZS
+00000c10: 4936 4943 4a6b 5a57 4e66 5a58 4a79 6233  I6ICJkZWNfZXJyb3
+00000c20: 4969 4c43 4169 5a6d 6c6c 6247 5266 626d  IiLCAiZmllbGRfbm
+00000c30: 4674 5a53 4936 4943 4a6b 5a57 4e66 5a58  FtZSI6ICJkZWNfZX
+00000c40: 4a79 6233 4969 4c43 4169 6347 4675 5a47  Jyb3IiLCAicGFuZG
+00000c50: 467a 5833 5235 6347 5569 4f69 4169 6157  FzX3R5cGUiOiAiaW
+00000c60: 3530 4e6a 5169 4c43 4169 626e 5674 6348  50NjQiLCAibnVtcH
+00000c70: 6c66 6448 6c77 5a53 4936 4943 4a70 626e  lfdHlwZSI6ICJpbn
+00000c80: 5132 4e43 4973 4943 4a74 5a58 5268 5a47  Q2NCIsICJtZXRhZG
+00000c90: 4630 5953 4936 4947 3531 6247 7839 5853  F0YSI6IG51bGx9XS
+00000ca0: 7767 496d 4e79 5a57 4630 6233 4969 4f69  wgImNyZWF0b3IiOi
+00000cb0: 4237 496d 7870 596e 4a68 636e 6b69 4f69  B7ImxpYnJhcnkiOi
+00000cc0: 4169 6348 6c68 636e 4a76 6479 4973 4943  AicHlhcnJvdyIsIC
+00000cd0: 4a32 5a58 4a7a 6157 3975 496a 6f67 496a  J2ZXJzaW9uIjogIj
+00000ce0: 6b75 4d43 3477 496e 3073 4943 4a77 5957  kuMC4wIn0sICJwYW
+00000cf0: 356b 5958 4e66 646d 5679 6332 6c76 6269  5kYXNfdmVyc2lvbi
+00000d00: 4936 4943 4979 4c6a 4175 4d43 4a39 4141  I6ICIyLjAuMCJ9AA
+00000d10: 5541 4141 446b 4141 4141 6f41 4141 4148  UAAADkAAAAoAAAAH
+00000d20: 5141 4141 4138 4141 4141 4241 4141 4145  QAAAA8AAAABAAAAE
+00000d30: 442f 2f2f 3841 4141 4543 4541 4141 4142  D///8AAAECEAAAAB
+00000d40: 7741 4141 4145 4141 4141 4141 4141 4141  wAAAAEAAAAAAAAAA
+00000d50: 6b41 4141 426b 5a57 4e66 5a58 4a79 6233  kAAABkZWNfZXJyb3
+00000d60: 4941 4141 4134 2f2f 2f2f 4141 4141 4155  IAAAA4////AAAAAU
+00000d70: 4141 4141 4230 2f2f 2f2f 4141 4142 4168  AAAAB0////AAABAh
+00000d80: 4141 4141 4163 4141 4141 4241 4141 4141  AAAAAcAAAABAAAAA
+00000d90: 4141 4141 4149 4141 4141 636d 4666 5a58  AAAAAIAAAAcmFfZX
+00000da0: 4a79 6233 4941 4141 4141 6250 2f2f 2f77  Jyb3IAAAAAbP///w
+00000db0: 4141 4141 4641 4141 4141 7150 2f2f 2f77  AAAAFAAAAAqP///w
+00000dc0: 4141 4151 4d51 4141 4141 4641 4141 4141  AAAQMQAAAAFAAAAA
+00000dd0: 5141 4141 4141 4141 4141 4177 4141 4147  QAAAAAAAAAAwAAAG
+00000de0: 526c 5977 4457 2f2f 2f2f 4141 4143 414e  RlYwDW////AAACAN
+00000df0: 442f 2f2f 3841 4141 4544 4541 4141 4142  D///8AAAEDEAAAAB
+00000e00: 7741 4141 4145 4141 4141 4141 4141 4141  wAAAAEAAAAAAAAAA
+00000e10: 4941 4141 4279 5951 4141 4141 4147 4141  IAAAByYQAAAAAGAA
+00000e20: 6741 4267 4147 4141 4141 4141 4143 4142  gABgAGAAAAAAACAB
+00000e30: 4141 4641 4149 4141 5941 4277 414d 4141  AAFAAIAAYABwAMAA
+00000e40: 4141 4541 4151 4141 4141 4141 4142 4168  AAEAAQAAAAAAABAh
+00000e50: 4141 4141 4163 4141 4141 4241 4141 4141  AAAAAcAAAABAAAAA
+00000e60: 4141 4141 4143 4141 4141 6157 5141 4141  AAAAACAAAAaWQAAA
+00000e70: 6741 4441 4149 4141 6341 4341 4141 4141  gADAAIAAcACAAAAA
+00000e80: 4141 4141 4641 4141 4141 4141 4141 4141  AAAAFAAAAAAAAAAA
+00000e90: 3d3d 0018 1f70 6172 7175 6574 2d63 7070  ==...parquet-cpp
+00000ea0: 2d61 7272 6f77 2076 6572 7369 6f6e 2039  -arrow version 9
+00000eb0: 2e30 2e30 195c 1c00 001c 0000 1c00 001c  .0.0.\..........
+00000ec0: 0000 1c00 0000 d30a 0000 5041 5231       ..........PAR1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/parquet_shards/dir_0/pixel_47/shard_3.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet`

 * *Files 20% similar despite different names*

```diff
@@ -56,245 +56,181 @@
 00000370: 0200 0000 0401 0104 0026 f20d 1c15 0419  .........&......
 00000380: 3510 0006 1918 0964 6563 5f65 7272 6f72  5......dec_error
 00000390: 1502 1604 16b8 0116 c001 26e2 0c26 b20c  ..........&..&..
 000003a0: 1c18 0800 0000 0000 0000 0018 0800 0000  ................
 000003b0: 0000 0000 0016 0028 0800 0000 0000 0000  .......(........
 000003c0: 0018 0800 0000 0000 0000 0000 192c 1504  .............,..
 000003d0: 1500 1502 0015 0015 1015 0200 0000 1504  ................
-000003e0: 1520 1524 4c15 0415 0012 0000 103c 0c00  . .$L........<..
-000003f0: 0000 0000 0000 1200 0000 0000 0000 1500  ................
-00000400: 1512 1516 2c15 0415 1015 0615 061c 1808  ....,...........
-00000410: 1200 0000 0000 0000 1808 0c00 0000 0000  ................
-00000420: 0000 1600 2808 1200 0000 0000 0000 1808  ....(...........
-00000430: 0c00 0000 0000 0000 0000 0009 2002 0000  ............ ...
-00000440: 0004 0101 0302 268c 111c 1504 1935 1000  ......&......5..
-00000450: 0619 1811 5f5f 696e 6465 785f 6c65 7665  ....__index_leve
-00000460: 6c5f 305f 5f15 0216 0416 c801 16d0 0126  l_0__..........&
-00000470: fc0f 26bc 0f1c 1808 1200 0000 0000 0000  ..&.............
-00000480: 1808 0c00 0000 0000 0000 1600 2808 1200  ............(...
-00000490: 0000 0000 0000 1808 0c00 0000 0000 0000  ................
-000004a0: 0019 2c15 0415 0015 0200 1500 1510 1502  ..,.............
-000004b0: 0000 0015 0419 7c35 0018 0673 6368 656d  ......|5...schem
-000004c0: 6115 0c00 1504 2502 1802 6964 0015 0a25  a.....%...id...%
-000004d0: 0218 0272 6100 150a 2502 1803 6465 6300  ...ra...%...dec.
-000004e0: 1504 2502 1808 7261 5f65 7272 6f72 0015  ..%...ra_error..
-000004f0: 0425 0218 0964 6563 5f65 7272 6f72 0015  .%...dec_error..
-00000500: 0425 0218 115f 5f69 6e64 6578 5f6c 6576  .%...__index_lev
-00000510: 656c 5f30 5f5f 0016 0419 1c19 6c26 d801  el_0__......l&..
-00000520: 1c15 0419 3510 0006 1918 0269 6415 0216  ....5......id...
-00000530: 0416 c801 16d0 0126 4826 081c 1808 e702  .......&H&......
-00000540: 0000 0000 0000 1808 e102 0000 0000 0000  ................
-00000550: 1600 2808 e702 0000 0000 0000 1808 e102  ..(.............
-00000560: 0000 0000 0000 0019 2c15 0415 0015 0200  ........,.......
-00000570: 1500 1510 1502 0000 0026 e004 1c15 0a19  .........&......
-00000580: 3510 0006 1918 0272 6115 0216 0416 c801  5......ra.......
-00000590: 16d0 0126 d003 2690 031c 1808 0000 0000  ...&..&.........
-000005a0: 00c8 7340 1808 0000 0000 0038 7340 1600  ..s@.......8s@..
-000005b0: 2808 0000 0000 00c8 7340 1808 0000 0000  (.......s@......
-000005c0: 0038 7340 0019 2c15 0415 0015 0200 1500  .8s@..,.........
-000005d0: 1510 1502 0000 0026 ec07 1c15 0a19 3510  .......&......5.
-000005e0: 0006 1918 0364 6563 1502 1604 16c8 0116  .....dec........
-000005f0: d001 26dc 0626 9c06 1c18 0800 0000 0000  ..&..&..........
-00000600: 8039 c018 0800 0000 0000 c040 c016 0028  .9.........@...(
-00000610: 0800 0000 0000 8039 c018 0800 0000 0000  .......9........
-00000620: c040 c000 192c 1504 1500 1502 0015 0015  .@...,..........
-00000630: 1015 0200 0000 26ea 0a1c 1504 1935 1000  ......&......5..
-00000640: 0619 1808 7261 5f65 7272 6f72 1502 1604  ....ra_error....
-00000650: 16b8 0116 c001 26da 0926 aa09 1c18 0800  ......&..&......
-00000660: 0000 0000 0000 0018 0800 0000 0000 0000  ................
-00000670: 0016 0028 0800 0000 0000 0000 0018 0800  ...(............
-00000680: 0000 0000 0000 0000 192c 1504 1500 1502  .........,......
-00000690: 0015 0015 1015 0200 0000 26f2 0d1c 1504  ..........&.....
-000006a0: 1935 1000 0619 1809 6465 635f 6572 726f  .5......dec_erro
-000006b0: 7215 0216 0416 b801 16c0 0126 e20c 26b2  r..........&..&.
-000006c0: 0c1c 1808 0000 0000 0000 0000 1808 0000  ................
-000006d0: 0000 0000 0000 1600 2808 0000 0000 0000  ........(.......
-000006e0: 0000 1808 0000 0000 0000 0000 0019 2c15  ..............,.
-000006f0: 0415 0015 0200 1500 1510 1502 0000 0026  ...............&
-00000700: 8c11 1c15 0419 3510 0006 1918 115f 5f69  ......5......__i
-00000710: 6e64 6578 5f6c 6576 656c 5f30 5f5f 1502  ndex_level_0__..
-00000720: 1604 16c8 0116 d001 26fc 0f26 bc0f 1c18  ........&..&....
-00000730: 0812 0000 0000 0000 0018 080c 0000 0000  ................
-00000740: 0000 0016 0028 0812 0000 0000 0000 0018  .....(..........
-00000750: 080c 0000 0000 0000 0000 192c 1504 1500  ...........,....
-00000760: 1502 0015 0015 1015 0200 0000 1690 0916  ................
-00000770: 0426 0816 c009 1400 0019 2c18 0670 616e  .&........,..pan
-00000780: 6461 7318 a507 7b22 696e 6465 785f 636f  das...{"index_co
-00000790: 6c75 6d6e 7322 3a20 5b22 5f5f 696e 6465  lumns": ["__inde
-000007a0: 785f 6c65 7665 6c5f 305f 5f22 5d2c 2022  x_level_0__"], "
-000007b0: 636f 6c75 6d6e 5f69 6e64 6578 6573 223a  column_indexes":
-000007c0: 205b 7b22 6e61 6d65 223a 206e 756c 6c2c   [{"name": null,
-000007d0: 2022 6669 656c 645f 6e61 6d65 223a 206e   "field_name": n
-000007e0: 756c 6c2c 2022 7061 6e64 6173 5f74 7970  ull, "pandas_typ
-000007f0: 6522 3a20 2275 6e69 636f 6465 222c 2022  e": "unicode", "
-00000800: 6e75 6d70 795f 7479 7065 223a 2022 6f62  numpy_type": "ob
-00000810: 6a65 6374 222c 2022 6d65 7461 6461 7461  ject", "metadata
-00000820: 223a 207b 2265 6e63 6f64 696e 6722 3a20  ": {"encoding": 
-00000830: 2255 5446 2d38 227d 7d5d 2c20 2263 6f6c  "UTF-8"}}], "col
-00000840: 756d 6e73 223a 205b 7b22 6e61 6d65 223a  umns": [{"name":
-00000850: 2022 6964 222c 2022 6669 656c 645f 6e61   "id", "field_na
-00000860: 6d65 223a 2022 6964 222c 2022 7061 6e64  me": "id", "pand
-00000870: 6173 5f74 7970 6522 3a20 2269 6e74 3634  as_type": "int64
-00000880: 222c 2022 6e75 6d70 795f 7479 7065 223a  ", "numpy_type":
-00000890: 2022 696e 7436 3422 2c20 226d 6574 6164   "int64", "metad
-000008a0: 6174 6122 3a20 6e75 6c6c 7d2c 207b 226e  ata": null}, {"n
-000008b0: 616d 6522 3a20 2272 6122 2c20 2266 6965  ame": "ra", "fie
-000008c0: 6c64 5f6e 616d 6522 3a20 2272 6122 2c20  ld_name": "ra", 
-000008d0: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
-000008e0: 666c 6f61 7436 3422 2c20 226e 756d 7079  float64", "numpy
-000008f0: 5f74 7970 6522 3a20 2266 6c6f 6174 3634  _type": "float64
-00000900: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
-00000910: 756c 6c7d 2c20 7b22 6e61 6d65 223a 2022  ull}, {"name": "
-00000920: 6465 6322 2c20 2266 6965 6c64 5f6e 616d  dec", "field_nam
-00000930: 6522 3a20 2264 6563 222c 2022 7061 6e64  e": "dec", "pand
-00000940: 6173 5f74 7970 6522 3a20 2266 6c6f 6174  as_type": "float
-00000950: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
-00000960: 223a 2022 666c 6f61 7436 3422 2c20 226d  ": "float64", "m
-00000970: 6574 6164 6174 6122 3a20 6e75 6c6c 7d2c  etadata": null},
-00000980: 207b 226e 616d 6522 3a20 2272 615f 6572   {"name": "ra_er
-00000990: 726f 7222 2c20 2266 6965 6c64 5f6e 616d  ror", "field_nam
-000009a0: 6522 3a20 2272 615f 6572 726f 7222 2c20  e": "ra_error", 
-000009b0: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
-000009c0: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
-000009d0: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
-000009e0: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
-000009f0: 2c20 7b22 6e61 6d65 223a 2022 6465 635f  , {"name": "dec_
-00000a00: 6572 726f 7222 2c20 2266 6965 6c64 5f6e  error", "field_n
-00000a10: 616d 6522 3a20 2264 6563 5f65 7272 6f72  ame": "dec_error
-00000a20: 222c 2022 7061 6e64 6173 5f74 7970 6522  ", "pandas_type"
-00000a30: 3a20 2269 6e74 3634 222c 2022 6e75 6d70  : "int64", "nump
-00000a40: 795f 7479 7065 223a 2022 696e 7436 3422  y_type": "int64"
-00000a50: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
-00000a60: 6c6c 7d2c 207b 226e 616d 6522 3a20 6e75  ll}, {"name": nu
-00000a70: 6c6c 2c20 2266 6965 6c64 5f6e 616d 6522  ll, "field_name"
-00000a80: 3a20 225f 5f69 6e64 6578 5f6c 6576 656c  : "__index_level
-00000a90: 5f30 5f5f 222c 2022 7061 6e64 6173 5f74  _0__", "pandas_t
-00000aa0: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
-00000ab0: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
-00000ac0: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
-00000ad0: 3a20 6e75 6c6c 7d5d 2c20 2263 7265 6174  : null}], "creat
-00000ae0: 6f72 223a 207b 226c 6962 7261 7279 223a  or": {"library":
-00000af0: 2022 7079 6172 726f 7722 2c20 2276 6572   "pyarrow", "ver
-00000b00: 7369 6f6e 223a 2022 392e 302e 3022 7d2c  sion": "9.0.0"},
-00000b10: 2022 7061 6e64 6173 5f76 6572 7369 6f6e   "pandas_version
-00000b20: 223a 2022 312e 332e 3522 7d00 180c 4152  ": "1.3.5"}...AR
-00000b30: 524f 573a 7363 6865 6d61 18c0 0e2f 2f2f  ROW:schema...///
-00000b40: 2f2f 3267 4641 4141 5141 4141 4141 4141  //2gFAAAQAAAAAAA
-00000b50: 4b41 4134 4142 6741 4641 4167 4143 6741  KAA4ABgAFAAgACgA
-00000b60: 4141 4141 4242 4141 5141 4141 4141 4141  AAAABBAAQAAAAAAA
-00000b70: 4b41 4177 4141 4141 4541 4167 4143 6741  KAAwAAAAEAAgACgA
-00000b80: 4141 4e77 4441 4141 4541 4141 4141 5141  AANwDAAAEAAAAAQA
-00000b90: 4141 4177 4141 4141 4941 4177 4142 4141  AAAwAAAAIAAwABAA
-00000ba0: 4941 4167 4141 4141 4941 4141 4145 4141  IAAgAAAAIAAAAEAA
-00000bb0: 4141 4159 4141 4142 7759 5735 6b59 584d  AAAYAAABwYW5kYXM
-00000bc0: 4141 4b55 4441 4142 3749 6d6c 755a 4756  AAKUDAAB7ImluZGV
-00000bd0: 3458 324e 7662 4856 7462 6e4d 694f 6942  4X2NvbHVtbnMiOiB
-00000be0: 6249 6c39 6661 5735 6b5a 5868 6662 4756  bIl9faW5kZXhfbGV
-00000bf0: 325a 5778 664d 4639 6649 6c30 7349 434a  2ZWxfMF9fIl0sICJ
-00000c00: 6a62 3278 3162 5735 6661 5735 6b5a 5868  jb2x1bW5faW5kZXh
-00000c10: 6c63 7949 3649 4674 3749 6d35 6862 5755  lcyI6IFt7Im5hbWU
-00000c20: 694f 6942 7564 5778 734c 4341 695a 6d6c  iOiBudWxsLCAiZml
-00000c30: 6c62 4752 6662 6d46 745a 5349 3649 4735  lbGRfbmFtZSI6IG5
-00000c40: 3162 4777 7349 434a 7759 5735 6b59 584e  1bGwsICJwYW5kYXN
-00000c50: 6664 486c 775a 5349 3649 434a 3162 6d6c  fdHlwZSI6ICJ1bml
-00000c60: 6a62 3252 6c49 6977 6749 6d35 3162 5842  jb2RlIiwgIm51bXB
-00000c70: 3558 3352 3563 4755 694f 6941 6962 324a  5X3R5cGUiOiAib2J
-00000c80: 715a 574e 3049 6977 6749 6d31 6c64 4746  qZWN0IiwgIm1ldGF
-00000c90: 6b59 5852 6849 6a6f 6765 794a 6c62 6d4e  kYXRhIjogeyJlbmN
-00000ca0: 765a 476c 755a 7949 3649 434a 5656 4559  vZGluZyI6ICJVVEY
-00000cb0: 744f 434a 3966 5630 7349 434a 6a62 3278  tOCJ9fV0sICJjb2x
-00000cc0: 3162 5735 7a49 6a6f 6757 3373 6962 6d46  1bW5zIjogW3sibmF
-00000cd0: 745a 5349 3649 434a 705a 4349 7349 434a  tZSI6ICJpZCIsICJ
-00000ce0: 6d61 5756 735a 4639 7559 5731 6c49 6a6f  maWVsZF9uYW1lIjo
-00000cf0: 6749 6d6c 6b49 6977 6749 6e42 6862 6d52  gImlkIiwgInBhbmR
-00000d00: 6863 3139 3065 5842 6c49 6a6f 6749 6d6c  hc190eXBlIjogIml
-00000d10: 7564 4459 3049 6977 6749 6d35 3162 5842  udDY0IiwgIm51bXB
-00000d20: 3558 3352 3563 4755 694f 6941 6961 5735  5X3R5cGUiOiAiaW5
-00000d30: 304e 6a51 694c 4341 6962 5756 3059 5752  0NjQiLCAibWV0YWR
-00000d40: 6864 4745 694f 6942 7564 5778 7366 5377  hdGEiOiBudWxsfSw
-00000d50: 6765 794a 7559 5731 6c49 6a6f 6749 6e4a  geyJuYW1lIjogInJ
-00000d60: 6849 6977 6749 6d5a 705a 5778 6b58 3235  hIiwgImZpZWxkX25
-00000d70: 6862 5755 694f 6941 6963 6d45 694c 4341  hbWUiOiAicmEiLCA
-00000d80: 6963 4746 755a 4746 7a58 3352 3563 4755  icGFuZGFzX3R5cGU
-00000d90: 694f 6941 695a 6d78 7659 5851 324e 4349  iOiAiZmxvYXQ2NCI
-00000da0: 7349 434a 7564 5731 7765 5639 3065 5842  sICJudW1weV90eXB
-00000db0: 6c49 6a6f 6749 6d5a 7362 3246 304e 6a51  lIjogImZsb2F0NjQ
-00000dc0: 694c 4341 6962 5756 3059 5752 6864 4745  iLCAibWV0YWRhdGE
-00000dd0: 694f 6942 7564 5778 7366 5377 6765 794a  iOiBudWxsfSwgeyJ
-00000de0: 7559 5731 6c49 6a6f 6749 6d52 6c59 7949  uYW1lIjogImRlYyI
-00000df0: 7349 434a 6d61 5756 735a 4639 7559 5731  sICJmaWVsZF9uYW1
-00000e00: 6c49 6a6f 6749 6d52 6c59 7949 7349 434a  lIjogImRlYyIsICJ
-00000e10: 7759 5735 6b59 584e 6664 486c 775a 5349  wYW5kYXNfdHlwZSI
-00000e20: 3649 434a 6d62 4739 6864 4459 3049 6977  6ICJmbG9hdDY0Iiw
-00000e30: 6749 6d35 3162 5842 3558 3352 3563 4755  gIm51bXB5X3R5cGU
-00000e40: 694f 6941 695a 6d78 7659 5851 324e 4349  iOiAiZmxvYXQ2NCI
-00000e50: 7349 434a 745a 5852 685a 4746 3059 5349  sICJtZXRhZGF0YSI
-00000e60: 3649 4735 3162 4778 394c 4342 3749 6d35  6IG51bGx9LCB7Im5
-00000e70: 6862 5755 694f 6941 6963 6d46 665a 584a  hbWUiOiAicmFfZXJ
-00000e80: 7962 3349 694c 4341 695a 6d6c 6c62 4752  yb3IiLCAiZmllbGR
-00000e90: 6662 6d46 745a 5349 3649 434a 7959 5639  fbmFtZSI6ICJyYV9
-00000ea0: 6c63 6e4a 7663 6949 7349 434a 7759 5735  lcnJvciIsICJwYW5
-00000eb0: 6b59 584e 6664 486c 775a 5349 3649 434a  kYXNfdHlwZSI6ICJ
-00000ec0: 7062 6e51 324e 4349 7349 434a 7564 5731  pbnQ2NCIsICJudW1
-00000ed0: 7765 5639 3065 5842 6c49 6a6f 6749 6d6c  weV90eXBlIjogIml
-00000ee0: 7564 4459 3049 6977 6749 6d31 6c64 4746  udDY0IiwgIm1ldGF
-00000ef0: 6b59 5852 6849 6a6f 6762 6e56 7362 4830  kYXRhIjogbnVsbH0
-00000f00: 7349 4873 6962 6d46 745a 5349 3649 434a  sIHsibmFtZSI6ICJ
-00000f10: 6b5a 574e 665a 584a 7962 3349 694c 4341  kZWNfZXJyb3IiLCA
-00000f20: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
-00000f30: 3649 434a 6b5a 574e 665a 584a 7962 3349  6ICJkZWNfZXJyb3I
-00000f40: 694c 4341 6963 4746 755a 4746 7a58 3352  iLCAicGFuZGFzX3R
-00000f50: 3563 4755 694f 6941 6961 5735 304e 6a51  5cGUiOiAiaW50NjQ
-00000f60: 694c 4341 6962 6e56 7463 486c 6664 486c  iLCAibnVtcHlfdHl
-00000f70: 775a 5349 3649 434a 7062 6e51 324e 4349  wZSI6ICJpbnQ2NCI
-00000f80: 7349 434a 745a 5852 685a 4746 3059 5349  sICJtZXRhZGF0YSI
-00000f90: 3649 4735 3162 4778 394c 4342 3749 6d35  6IG51bGx9LCB7Im5
-00000fa0: 6862 5755 694f 6942 7564 5778 734c 4341  hbWUiOiBudWxsLCA
-00000fb0: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
-00000fc0: 3649 434a 6658 326c 755a 4756 3458 3278  6ICJfX2luZGV4X2x
-00000fd0: 6c64 6d56 7358 7a42 6658 7949 7349 434a  ldmVsXzBfXyIsICJ
-00000fe0: 7759 5735 6b59 584e 6664 486c 775a 5349  wYW5kYXNfdHlwZSI
-00000ff0: 3649 434a 7062 6e51 324e 4349 7349 434a  6ICJpbnQ2NCIsICJ
-00001000: 7564 5731 7765 5639 3065 5842 6c49 6a6f  udW1weV90eXBlIjo
-00001010: 6749 6d6c 7564 4459 3049 6977 6749 6d31  gImludDY0IiwgIm1
-00001020: 6c64 4746 6b59 5852 6849 6a6f 6762 6e56  ldGFkYXRhIjogbnV
-00001030: 7362 4831 644c 4341 6959 334a 6c59 5852  sbH1dLCAiY3JlYXR
-00001040: 7663 6949 3649 4873 6962 476c 6963 6d46  vciI6IHsibGlicmF
-00001050: 7965 5349 3649 434a 7765 5746 7963 6d39  yeSI6ICJweWFycm9
-00001060: 3349 6977 6749 6e5a 6c63 6e4e 7062 3234  3IiwgInZlcnNpb24
-00001070: 694f 6941 694f 5334 774c 6a41 6966 5377  iOiAiOS4wLjAifSw
-00001080: 6749 6e42 6862 6d52 6863 3139 325a 584a  gInBhbmRhc192ZXJ
-00001090: 7a61 5739 7549 6a6f 6749 6a45 754d 7934  zaW9uIjogIjEuMy4
-000010a0: 3149 6e30 4141 4141 4741 4141 414a 4145  1In0AAAAGAAAAJAE
-000010b0: 4141 4f41 4141 4143 3041 4141 4166 4141  AAOAAAAC0AAAAfAA
-000010c0: 4141 4551 4141 4141 4541 4141 4142 502f  AAEQAAAAEAAAABP/
-000010d0: 2f2f 7741 4141 5149 5141 4141 414a 4141  //wAAAQIQAAAAJAA
-000010e0: 4141 4151 4141 4141 4141 4141 4145 5141  AAAQAAAAAAAAAEQA
-000010f0: 4141 4639 6661 5735 6b5a 5868 6662 4756  AAF9faW5kZXhfbGV
-00001100: 325a 5778 664d 4639 6641 4141 4142 502f  2ZWxfMF9fAAAABP/
-00001110: 2f2f 7741 4141 4146 4141 4141 4151 502f  //wAAAAFAAAAAQP/
-00001120: 2f2f 7741 4141 5149 5141 4141 4148 4141  //wAAAQIQAAAAHAA
-00001130: 4141 4151 4141 4141 4141 4141 4143 5141  AAAQAAAAAAAAACQA
-00001140: 4141 4752 6c59 3139 6c63 6e4a 7663 6741  AAGRlY19lcnJvcgA
-00001150: 4141 446a 2f2f 2f38 4141 4141 4251 4141  AADj///8AAAABQAA
-00001160: 4141 4854 2f2f 2f38 4141 4145 4345 4141  AAHT///8AAAECEAA
-00001170: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
-00001180: 4141 4167 4141 4142 7959 5639 6c63 6e4a  AAAgAAAByYV9lcnJ
-00001190: 7663 6741 4141 4142 732f 2f2f 2f41 4141  vcgAAAABs////AAA
-000011a0: 4141 5541 4141 4143 6f2f 2f2f 2f41 4141  AAUAAAACo////AAA
-000011b0: 4241 7841 4141 4141 5541 4141 4142 4141  BAxAAAAAUAAAABAA
-000011c0: 4141 4141 4141 4141 4441 4141 415a 4756  AAAAAAAADAAAAZGV
-000011d0: 6a41 4e62 2f2f 2f38 4141 4149 4130 502f  jANb///8AAAIA0P/
-000011e0: 2f2f 7741 4141 514d 5141 4141 4148 4141  //wAAAQMQAAAAHAA
-000011f0: 4141 4151 4141 4141 4141 4141 4141 6741  AAAQAAAAAAAAAAgA
-00001200: 4141 484a 6841 4141 4141 4159 4143 4141  AAHJhAAAAAAYACAA
-00001210: 4741 4159 4141 4141 4141 4149 4145 4141  GAAYAAAAAAAIAEAA
-00001220: 5541 4167 4142 6741 4841 4177 4141 4141  UAAgABgAHAAwAAAA
-00001230: 5141 4241 4141 4141 4141 4145 4345 4141  QABAAAAAAAAECEAA
-00001240: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
-00001250: 4141 4149 4141 4142 705a 4141 4143 4141  AAAIAAABpZAAACAA
-00001260: 4d41 4167 4142 7741 4941 4141 4141 4141  MAAgABwAIAAAAAAA
-00001270: 4141 5541 4141 4141 4141 4141 4100 181f  AAUAAAAAAAAAA...
-00001280: 7061 7271 7565 742d 6370 702d 6172 726f  parquet-cpp-arro
-00001290: 7720 7665 7273 696f 6e20 392e 302e 3019  w version 9.0.0.
-000012a0: 6c1c 0000 1c00 001c 0000 1c00 001c 0000  l...............
-000012b0: 1c00 0000 010e 0000 5041 5231            ........PAR1
+000003e0: 196c 3500 1806 7363 6865 6d61 150a 0015  .l5...schema....
+000003f0: 0425 0218 0269 6400 150a 2502 1802 7261  .%...id...%...ra
+00000400: 0015 0a25 0218 0364 6563 0015 0425 0218  ...%...dec...%..
+00000410: 0872 615f 6572 726f 7200 1504 2502 1809  .ra_error...%...
+00000420: 6465 635f 6572 726f 7200 1604 191c 195c  dec_error......\
+00000430: 26d8 011c 1504 1935 1000 0619 1802 6964  &......5......id
+00000440: 1502 1604 16c8 0116 d001 2648 2608 1c18  ..........&H&...
+00000450: 08e7 0200 0000 0000 0018 08e1 0200 0000  ................
+00000460: 0000 0016 0028 08e7 0200 0000 0000 0018  .....(..........
+00000470: 08e1 0200 0000 0000 0000 192c 1504 1500  ...........,....
+00000480: 1502 0015 0015 1015 0200 0000 26e0 041c  ............&...
+00000490: 150a 1935 1000 0619 1802 7261 1502 1604  ...5......ra....
+000004a0: 16c8 0116 d001 26d0 0326 9003 1c18 0800  ......&..&......
+000004b0: 0000 0000 c873 4018 0800 0000 0000 3873  .....s@.......8s
+000004c0: 4016 0028 0800 0000 0000 c873 4018 0800  @..(.......s@...
+000004d0: 0000 0000 3873 4000 192c 1504 1500 1502  ....8s@..,......
+000004e0: 0015 0015 1015 0200 0000 26ec 071c 150a  ..........&.....
+000004f0: 1935 1000 0619 1803 6465 6315 0216 0416  .5......dec.....
+00000500: c801 16d0 0126 dc06 269c 061c 1808 0000  .....&..&.......
+00000510: 0000 0080 39c0 1808 0000 0000 00c0 40c0  ....9.........@.
+00000520: 1600 2808 0000 0000 0080 39c0 1808 0000  ..(.......9.....
+00000530: 0000 00c0 40c0 0019 2c15 0415 0015 0200  ....@...,.......
+00000540: 1500 1510 1502 0000 0026 ea0a 1c15 0419  .........&......
+00000550: 3510 0006 1918 0872 615f 6572 726f 7215  5......ra_error.
+00000560: 0216 0416 b801 16c0 0126 da09 26aa 091c  .........&..&...
+00000570: 1808 0000 0000 0000 0000 1808 0000 0000  ................
+00000580: 0000 0000 1600 2808 0000 0000 0000 0000  ......(.........
+00000590: 1808 0000 0000 0000 0000 0019 2c15 0415  ............,...
+000005a0: 0015 0200 1500 1510 1502 0000 0026 f20d  .............&..
+000005b0: 1c15 0419 3510 0006 1918 0964 6563 5f65  ....5......dec_e
+000005c0: 7272 6f72 1502 1604 16b8 0116 c001 26e2  rror..........&.
+000005d0: 0c26 b20c 1c18 0800 0000 0000 0000 0018  .&..............
+000005e0: 0800 0000 0000 0000 0016 0028 0800 0000  ...........(....
+000005f0: 0000 0000 0018 0800 0000 0000 0000 0000  ................
+00000600: 192c 1504 1500 1502 0015 0015 1015 0200  .,..............
+00000610: 0000 16c8 0716 0426 0816 f007 1400 0019  .......&........
+00000620: 2c18 0670 616e 6461 7318 a705 7b22 696e  ,..pandas...{"in
+00000630: 6465 785f 636f 6c75 6d6e 7322 3a20 5b5d  dex_columns": []
+00000640: 2c20 2263 6f6c 756d 6e5f 696e 6465 7865  , "column_indexe
+00000650: 7322 3a20 5b5d 2c20 2263 6f6c 756d 6e73  s": [], "columns
+00000660: 223a 205b 7b22 6e61 6d65 223a 2022 6964  ": [{"name": "id
+00000670: 222c 2022 6669 656c 645f 6e61 6d65 223a  ", "field_name":
+00000680: 2022 6964 222c 2022 7061 6e64 6173 5f74   "id", "pandas_t
+00000690: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
+000006a0: 6e75 6d70 795f 7479 7065 223a 2022 696e  numpy_type": "in
+000006b0: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
+000006c0: 3a20 6e75 6c6c 7d2c 207b 226e 616d 6522  : null}, {"name"
+000006d0: 3a20 2272 6122 2c20 2266 6965 6c64 5f6e  : "ra", "field_n
+000006e0: 616d 6522 3a20 2272 6122 2c20 2270 616e  ame": "ra", "pan
+000006f0: 6461 735f 7479 7065 223a 2022 666c 6f61  das_type": "floa
+00000700: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
+00000710: 6522 3a20 2266 6c6f 6174 3634 222c 2022  e": "float64", "
+00000720: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
+00000730: 2c20 7b22 6e61 6d65 223a 2022 6465 6322  , {"name": "dec"
+00000740: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
+00000750: 2264 6563 222c 2022 7061 6e64 6173 5f74  "dec", "pandas_t
+00000760: 7970 6522 3a20 2266 6c6f 6174 3634 222c  ype": "float64",
+00000770: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
+00000780: 666c 6f61 7436 3422 2c20 226d 6574 6164  float64", "metad
+00000790: 6174 6122 3a20 6e75 6c6c 7d2c 207b 226e  ata": null}, {"n
+000007a0: 616d 6522 3a20 2272 615f 6572 726f 7222  ame": "ra_error"
+000007b0: 2c20 2266 6965 6c64 5f6e 616d 6522 3a20  , "field_name": 
+000007c0: 2272 615f 6572 726f 7222 2c20 2270 616e  "ra_error", "pan
+000007d0: 6461 735f 7479 7065 223a 2022 696e 7436  das_type": "int6
+000007e0: 3422 2c20 226e 756d 7079 5f74 7970 6522  4", "numpy_type"
+000007f0: 3a20 2269 6e74 3634 222c 2022 6d65 7461  : "int64", "meta
+00000800: 6461 7461 223a 206e 756c 6c7d 2c20 7b22  data": null}, {"
+00000810: 6e61 6d65 223a 2022 6465 635f 6572 726f  name": "dec_erro
+00000820: 7222 2c20 2266 6965 6c64 5f6e 616d 6522  r", "field_name"
+00000830: 3a20 2264 6563 5f65 7272 6f72 222c 2022  : "dec_error", "
+00000840: 7061 6e64 6173 5f74 7970 6522 3a20 2269  pandas_type": "i
+00000850: 6e74 3634 222c 2022 6e75 6d70 795f 7479  nt64", "numpy_ty
+00000860: 7065 223a 2022 696e 7436 3422 2c20 226d  pe": "int64", "m
+00000870: 6574 6164 6174 6122 3a20 6e75 6c6c 7d5d  etadata": null}]
+00000880: 2c20 2263 7265 6174 6f72 223a 207b 226c  , "creator": {"l
+00000890: 6962 7261 7279 223a 2022 7079 6172 726f  ibrary": "pyarro
+000008a0: 7722 2c20 2276 6572 7369 6f6e 223a 2022  w", "version": "
+000008b0: 392e 302e 3022 7d2c 2022 7061 6e64 6173  9.0.0"}, "pandas
+000008c0: 5f76 6572 7369 6f6e 223a 2022 322e 302e  _version": "2.0.
+000008d0: 3022 7d00 180c 4152 524f 573a 7363 6865  0"}...ARROW:sche
+000008e0: 6d61 1898 0b2f 2f2f 2f2f 7967 4541 4141  ma.../////ygEAAA
+000008f0: 5141 4141 4141 4141 4b41 4134 4142 6741  QAAAAAAAKAA4ABgA
+00000900: 4641 4167 4143 6741 4141 4141 4242 4141  FAAgACgAAAAABBAA
+00000910: 5141 4141 4141 4141 4b41 4177 4141 4141  QAAAAAAAKAAwAAAA
+00000920: 4541 4167 4143 6741 4141 4e77 4341 4141  EAAgACgAAANwCAAA
+00000930: 4541 4141 4141 5141 4141 4177 4141 4141  EAAAAAQAAAAwAAAA
+00000940: 4941 4177 4142 4141 4941 4167 4141 4141  IAAwABAAIAAgAAAA
+00000950: 4941 4141 4145 4141 4141 4159 4141 4142  IAAAAEAAAAAYAAAB
+00000960: 7759 5735 6b59 584d 4141 4b63 4341 4142  wYW5kYXMAAKcCAAB
+00000970: 3749 6d6c 755a 4756 3458 324e 7662 4856  7ImluZGV4X2NvbHV
+00000980: 7462 6e4d 694f 6942 6258 5377 6749 6d4e  tbnMiOiBbXSwgImN
+00000990: 7662 4856 7462 6c39 7062 6d52 6c65 4756  vbHVtbl9pbmRleGV
+000009a0: 7a49 6a6f 6757 3130 7349 434a 6a62 3278  zIjogW10sICJjb2x
+000009b0: 3162 5735 7a49 6a6f 6757 3373 6962 6d46  1bW5zIjogW3sibmF
+000009c0: 745a 5349 3649 434a 705a 4349 7349 434a  tZSI6ICJpZCIsICJ
+000009d0: 6d61 5756 735a 4639 7559 5731 6c49 6a6f  maWVsZF9uYW1lIjo
+000009e0: 6749 6d6c 6b49 6977 6749 6e42 6862 6d52  gImlkIiwgInBhbmR
+000009f0: 6863 3139 3065 5842 6c49 6a6f 6749 6d6c  hc190eXBlIjogIml
+00000a00: 7564 4459 3049 6977 6749 6d35 3162 5842  udDY0IiwgIm51bXB
+00000a10: 3558 3352 3563 4755 694f 6941 6961 5735  5X3R5cGUiOiAiaW5
+00000a20: 304e 6a51 694c 4341 6962 5756 3059 5752  0NjQiLCAibWV0YWR
+00000a30: 6864 4745 694f 6942 7564 5778 7366 5377  hdGEiOiBudWxsfSw
+00000a40: 6765 794a 7559 5731 6c49 6a6f 6749 6e4a  geyJuYW1lIjogInJ
+00000a50: 6849 6977 6749 6d5a 705a 5778 6b58 3235  hIiwgImZpZWxkX25
+00000a60: 6862 5755 694f 6941 6963 6d45 694c 4341  hbWUiOiAicmEiLCA
+00000a70: 6963 4746 755a 4746 7a58 3352 3563 4755  icGFuZGFzX3R5cGU
+00000a80: 694f 6941 695a 6d78 7659 5851 324e 4349  iOiAiZmxvYXQ2NCI
+00000a90: 7349 434a 7564 5731 7765 5639 3065 5842  sICJudW1weV90eXB
+00000aa0: 6c49 6a6f 6749 6d5a 7362 3246 304e 6a51  lIjogImZsb2F0NjQ
+00000ab0: 694c 4341 6962 5756 3059 5752 6864 4745  iLCAibWV0YWRhdGE
+00000ac0: 694f 6942 7564 5778 7366 5377 6765 794a  iOiBudWxsfSwgeyJ
+00000ad0: 7559 5731 6c49 6a6f 6749 6d52 6c59 7949  uYW1lIjogImRlYyI
+00000ae0: 7349 434a 6d61 5756 735a 4639 7559 5731  sICJmaWVsZF9uYW1
+00000af0: 6c49 6a6f 6749 6d52 6c59 7949 7349 434a  lIjogImRlYyIsICJ
+00000b00: 7759 5735 6b59 584e 6664 486c 775a 5349  wYW5kYXNfdHlwZSI
+00000b10: 3649 434a 6d62 4739 6864 4459 3049 6977  6ICJmbG9hdDY0Iiw
+00000b20: 6749 6d35 3162 5842 3558 3352 3563 4755  gIm51bXB5X3R5cGU
+00000b30: 694f 6941 695a 6d78 7659 5851 324e 4349  iOiAiZmxvYXQ2NCI
+00000b40: 7349 434a 745a 5852 685a 4746 3059 5349  sICJtZXRhZGF0YSI
+00000b50: 3649 4735 3162 4778 394c 4342 3749 6d35  6IG51bGx9LCB7Im5
+00000b60: 6862 5755 694f 6941 6963 6d46 665a 584a  hbWUiOiAicmFfZXJ
+00000b70: 7962 3349 694c 4341 695a 6d6c 6c62 4752  yb3IiLCAiZmllbGR
+00000b80: 6662 6d46 745a 5349 3649 434a 7959 5639  fbmFtZSI6ICJyYV9
+00000b90: 6c63 6e4a 7663 6949 7349 434a 7759 5735  lcnJvciIsICJwYW5
+00000ba0: 6b59 584e 6664 486c 775a 5349 3649 434a  kYXNfdHlwZSI6ICJ
+00000bb0: 7062 6e51 324e 4349 7349 434a 7564 5731  pbnQ2NCIsICJudW1
+00000bc0: 7765 5639 3065 5842 6c49 6a6f 6749 6d6c  weV90eXBlIjogIml
+00000bd0: 7564 4459 3049 6977 6749 6d31 6c64 4746  udDY0IiwgIm1ldGF
+00000be0: 6b59 5852 6849 6a6f 6762 6e56 7362 4830  kYXRhIjogbnVsbH0
+00000bf0: 7349 4873 6962 6d46 745a 5349 3649 434a  sIHsibmFtZSI6ICJ
+00000c00: 6b5a 574e 665a 584a 7962 3349 694c 4341  kZWNfZXJyb3IiLCA
+00000c10: 695a 6d6c 6c62 4752 6662 6d46 745a 5349  iZmllbGRfbmFtZSI
+00000c20: 3649 434a 6b5a 574e 665a 584a 7962 3349  6ICJkZWNfZXJyb3I
+00000c30: 694c 4341 6963 4746 755a 4746 7a58 3352  iLCAicGFuZGFzX3R
+00000c40: 3563 4755 694f 6941 6961 5735 304e 6a51  5cGUiOiAiaW50NjQ
+00000c50: 694c 4341 6962 6e56 7463 486c 6664 486c  iLCAibnVtcHlfdHl
+00000c60: 775a 5349 3649 434a 7062 6e51 324e 4349  wZSI6ICJpbnQ2NCI
+00000c70: 7349 434a 745a 5852 685a 4746 3059 5349  sICJtZXRhZGF0YSI
+00000c80: 3649 4735 3162 4778 3958 5377 6749 6d4e  6IG51bGx9XSwgImN
+00000c90: 795a 5746 3062 3349 694f 6942 3749 6d78  yZWF0b3IiOiB7Imx
+00000ca0: 7059 6e4a 6863 6e6b 694f 6941 6963 486c  pYnJhcnkiOiAicHl
+00000cb0: 6863 6e4a 7664 7949 7349 434a 325a 584a  hcnJvdyIsICJ2ZXJ
+00000cc0: 7a61 5739 7549 6a6f 6749 6a6b 754d 4334  zaW9uIjogIjkuMC4
+00000cd0: 7749 6e30 7349 434a 7759 5735 6b59 584e  wIn0sICJwYW5kYXN
+00000ce0: 6664 6d56 7963 326c 7662 6949 3649 4349  fdmVyc2lvbiI6ICI
+00000cf0: 794c 6a41 754d 434a 3941 4155 4141 4144  yLjAuMCJ9AAUAAAD
+00000d00: 6b41 4141 416f 4141 4141 4851 4141 4141  kAAAAoAAAAHQAAAA
+00000d10: 3841 4141 4142 4141 4141 4544 2f2f 2f38  8AAAABAAAAED///8
+00000d20: 4141 4145 4345 4141 4141 4277 4141 4141  AAAECEAAAABwAAAA
+00000d30: 4541 4141 4141 4141 4141 416b 4141 4142  EAAAAAAAAAAkAAAB
+00000d40: 6b5a 574e 665a 584a 7962 3349 4141 4141  kZWNfZXJyb3IAAAA
+00000d50: 342f 2f2f 2f41 4141 4141 5541 4141 4142  4////AAAAAUAAAAB
+00000d60: 302f 2f2f 2f41 4141 4241 6841 4141 4141  0////AAABAhAAAAA
+00000d70: 6341 4141 4142 4141 4141 4141 4141 4141  cAAAABAAAAAAAAAA
+00000d80: 4941 4141 4163 6d46 665a 584a 7962 3349  IAAAAcmFfZXJyb3I
+00000d90: 4141 4141 4162 502f 2f2f 7741 4141 4146  AAAAAbP///wAAAAF
+00000da0: 4141 4141 4171 502f 2f2f 7741 4141 514d  AAAAAqP///wAAAQM
+00000db0: 5141 4141 4146 4141 4141 4151 4141 4141  QAAAAFAAAAAQAAAA
+00000dc0: 4141 4141 4141 7741 4141 4752 6c59 7744  AAAAAAwAAAGRlYwD
+00000dd0: 572f 2f2f 2f41 4141 4341 4e44 2f2f 2f38  W////AAACAND///8
+00000de0: 4141 4145 4445 4141 4141 4277 4141 4141  AAAEDEAAAABwAAAA
+00000df0: 4541 4141 4141 4141 4141 4149 4141 4142  EAAAAAAAAAAIAAAB
+00000e00: 7959 5141 4141 4141 4741 4167 4142 6741  yYQAAAAAGAAgABgA
+00000e10: 4741 4141 4141 4141 4341 4241 4146 4141  GAAAAAAACABAAFAA
+00000e20: 4941 4159 4142 7741 4d41 4141 4145 4141  IAAYABwAMAAAAEAA
+00000e30: 5141 4141 4141 4141 4241 6841 4141 4141  QAAAAAAABAhAAAAA
+00000e40: 6341 4141 4142 4141 4141 4141 4141 4141  cAAAABAAAAAAAAAA
+00000e50: 4341 4141 4161 5751 4141 4167 4144 4141  CAAAAaWQAAAgADAA
+00000e60: 4941 4163 4143 4141 4141 4141 4141 4146  IAAcACAAAAAAAAAF
+00000e70: 4141 4141 4141 4141 4141 413d 3d00 181f  AAAAAAAAAAA==...
+00000e80: 7061 7271 7565 742d 6370 702d 6172 726f  parquet-cpp-arro
+00000e90: 7720 7665 7273 696f 6e20 392e 302e 3019  w version 9.0.0.
+00000ea0: 5c1c 0000 1c00 001c 0000 1c00 001c 0000  \...............
+00000eb0: 00d3 0a00 0050 4152 31                   .....PAR1
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet` & `hipscat-import-0.0.4/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/small_sky/catalog.csv` & `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky/catalog.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv` & `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv` & `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv` & `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv` & `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv` & `hipscat-import-0.0.4/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/data/test_formats/small_sky.fits` & `hipscat-import-0.0.4/tests/hipscat_import/data/test_formats/small_sky.fits`

 * *Files identical despite different names*

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/test_file_readers.py` & `hipscat-import-0.0.4/tests/hipscat_import/catalog/test_file_readers.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,37 @@
 
 import hipscat.io.write_metadata as io
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 import pytest
-from hipscat.catalog import CatalogParameters
+from hipscat.catalog.catalog import CatalogInfo
 
-from hipscat_import.file_readers import (
+from hipscat_import.catalog.file_readers import (
     CsvReader,
     FitsReader,
     ParquetReader,
     get_file_reader,
 )
 
 
+# pylint: disable=redefined-outer-name
+@pytest.fixture
+def basic_catalog_info():
+    info = {
+        "catalog_name": "test_catalog",
+        "catalog_type": "object",
+        "total_rows": 100,
+        "ra_column": "ra",
+        "dec_column": "dec",
+    }
+    return CatalogInfo(**info)
+
+
 def test_unknown_file_type():
     """File reader factory method should fail for unknown file types"""
     with pytest.raises(NotImplementedError):
         get_file_reader("")
     with pytest.raises(NotImplementedError):
         get_file_reader("unknown")
 
@@ -90,14 +103,25 @@
         "dec": pd.Float64Dtype(),
         "ra_error": pd.Float64Dtype(),
         "dec_error": pd.Float64Dtype(),
     }
     assert np.all(column_types == expected_column_types)
 
 
+def test_csv_reader_kwargs(small_sky_single_file):
+    """Verify we can read the csv file using kwargs passed to read_csv call."""
+
+    ## Input file has 5 columns: ["id", "ra", "dec", "ra_error", "dec_error"]
+    frame = next(CsvReader(usecols=["id", "ra", "dec"]).read(small_sky_single_file))
+    assert len(frame) == 131
+
+    assert len(frame.columns) == 3
+    assert np.all(frame.columns == ["id", "ra", "dec"])
+
+
 def test_csv_reader_pipe_delimited(formats_pipe_csv, tmp_path):
     """Verify we can read a pipe-delimited csv file without a header row."""
     total_chunks = 0
     for frame in CsvReader(header=None, separator="|").read(formats_pipe_csv):
         total_chunks += 1
         assert len(frame) == 3
         assert np.all(frame[0] == ["AA", "BB", "CC"])
@@ -172,32 +196,31 @@
         "ints": pd.Int64Dtype(),
         "empty": pd.Int64Dtype(),
         "numeric": pd.Int64Dtype(),
     }
     assert np.all(column_types == expected_column_types)
 
 
-def test_csv_reader_provenance_info(tmp_path):
+def test_csv_reader_provenance_info(tmp_path, basic_catalog_info):
     """Test that we get some provenance info and it is parseable into JSON."""
     reader = CsvReader(
         header=None,
         separator="|",
         column_names=["letters", "ints", "empty", "numeric"],
         type_map={
             "letters": object,
             "ints": int,
             "empty": "Int64",
             "numeric": int,
         },
     )
     provenance_info = reader.provenance_info()
-    base_catalog_parameters = CatalogParameters(
-        output_path=tmp_path, catalog_name="empty"
-    )
-    io.write_provenance_info(base_catalog_parameters, provenance_info)
+    catalog_base_dir = os.path.join(tmp_path, "test_catalog")
+    os.makedirs(catalog_base_dir)
+    io.write_provenance_info(catalog_base_dir, basic_catalog_info, provenance_info)
 
 
 def test_parquet_reader(parquet_shards_shard_44_0):
     """Verify we can read the parquet file into a single data frame."""
     total_chunks = 0
     for frame in ParquetReader().read(parquet_shards_shard_44_0):
         total_chunks += 1
@@ -211,22 +234,21 @@
     total_chunks = 0
     for frame in ParquetReader(chunksize=1).read(parquet_shards_shard_44_0):
         total_chunks += 1
         assert len(frame) == 1
     assert total_chunks == 7
 
 
-def test_parquet_reader_provenance_info(tmp_path):
+def test_parquet_reader_provenance_info(tmp_path, basic_catalog_info):
     """Test that we get some provenance info and it is parseable into JSON."""
     reader = ParquetReader(chunksize=1)
     provenance_info = reader.provenance_info()
-    base_catalog_parameters = CatalogParameters(
-        output_path=tmp_path, catalog_name="empty"
-    )
-    io.write_provenance_info(base_catalog_parameters, provenance_info)
+    catalog_base_dir = os.path.join(tmp_path, "test_catalog")
+    os.makedirs(catalog_base_dir)
+    io.write_provenance_info(catalog_base_dir, basic_catalog_info, provenance_info)
 
 
 def test_read_fits(formats_fits):
     """Success case - fits file that exists being read as fits"""
     total_chunks = 0
     for frame in FitsReader().read(formats_fits):
         total_chunks += 1
@@ -252,15 +274,14 @@
 
     frame = next(
         FitsReader(skip_column_names=["ra_error", "dec_error"]).read(formats_fits)
     )
     assert list(frame.columns) == ["id", "ra", "dec"]
 
 
-def test_fits_reader_provenance_info(tmp_path):
+def test_fits_reader_provenance_info(tmp_path, basic_catalog_info):
     """Test that we get some provenance info and it is parseable into JSON."""
     reader = FitsReader()
     provenance_info = reader.provenance_info()
-    base_catalog_parameters = CatalogParameters(
-        output_path=tmp_path, catalog_name="empty"
-    )
-    io.write_provenance_info(base_catalog_parameters, provenance_info)
+    catalog_base_dir = os.path.join(tmp_path, "test_catalog")
+    os.makedirs(catalog_base_dir)
+    io.write_provenance_info(catalog_base_dir, basic_catalog_info, provenance_info)
```

### Comparing `hipscat-import-0.0.3/tests/hipscat_import/test_resume_files.py` & `hipscat-import-0.0.4/tests/hipscat_import/catalog/test_resume_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Test resume file operations"""
 
 import hipscat.pixel_math as hist
 import numpy.testing as npt
 import pytest
 
-from hipscat_import.resume_files import (
+from hipscat_import.catalog.resume_files import (
     clean_resume_files,
     is_mapping_done,
     is_reducing_done,
     read_histogram,
     read_mapping_keys,
     read_reducing_keys,
     set_mapping_done,
@@ -88,15 +88,15 @@
     write_mapping_start_key(tmp_path, "key1")
     write_mapping_done_key(tmp_path, "key1")
     mapping_keys = read_mapping_keys(tmp_path)
     assert len(mapping_keys) == 1
     assert mapping_keys[0] == "key1"
 
     write_mapping_start_key(tmp_path, "key2")
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="logs are corrupted"):
         read_mapping_keys(tmp_path)
 
     clean_resume_files(tmp_path)
     mapping_keys = read_mapping_keys(tmp_path)
     assert len(mapping_keys) == 0
```

