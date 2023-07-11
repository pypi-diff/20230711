# Comparing `tmp/cacholote-0.3.1.tar.gz` & `tmp/cacholote-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cacholote-0.3.1.tar", last modified: Thu May  4 15:02:22 2023, max compression
+gzip compressed data, was "cacholote-0.3.2.tar", last modified: Tue Jul 11 10:19:17 2023, max compression
```

## Comparing `cacholote-0.3.1.tar` & `cacholote-0.3.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.366105 cacholote-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-04 15:02:04.000000 cacholote-0.3.1/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.358105 cacholote-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.362105 cacholote-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-05-04 15:02:04.000000 cacholote-0.3.1/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-04 15:02:04.000000 cacholote-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-04 15:02:04.000000 cacholote-0.3.1/.pre-commit-config-cruft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-04 15:02:04.000000 cacholote-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-04 15:02:04.000000 cacholote-0.3.1/DESIGN.rst
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 15:02:04.000000 cacholote-0.3.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-05-04 15:02:04.000000 cacholote-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-04 15:02:04.000000 cacholote-0.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-04 15:02:04.000000 cacholote-0.3.1/OBJECT-STORAGE-DESIGN.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-05-04 15:02:22.366105 cacholote-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-04 15:02:04.000000 cacholote-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.362105 cacholote-0.3.1/cacholote/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/extra_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 15:02:22.000000 cacholote-0.3.1/cacholote/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.362105 cacholote-0.3.1/cacholote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-05-04 15:02:22.000000 cacholote-0.3.1/cacholote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-04 15:02:22.000000 cacholote-0.3.1/cacholote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:02:22.000000 cacholote-0.3.1/cacholote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 15:02:22.000000 cacholote-0.3.1/cacholote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 15:02:22.000000 cacholote-0.3.1/cacholote.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.362105 cacholote-0.3.1/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-04 15:02:04.000000 cacholote-0.3.1/ci/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-04 15:02:04.000000 cacholote-0.3.1/ci/environment-integration.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.366105 cacholote-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-04 15:02:04.000000 cacholote-0.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.366105 cacholote-0.3.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:04.000000 cacholote-0.3.1/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.366105 cacholote-0.3.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:04.000000 cacholote-0.3.1/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-04 15:02:04.000000 cacholote-0.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-04 15:02:04.000000 cacholote-0.3.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-04 15:02:04.000000 cacholote-0.3.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 15:02:04.000000 cacholote-0.3.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-04 15:02:04.000000 cacholote-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:02:22.366105 cacholote-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.366105 cacholote-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_01_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_02_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_10_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_20_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_30_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_40_xarray_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_50_io_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_60_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:19:17.130490 cacholote-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-11 10:18:58.000000 cacholote-0.3.2/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:19:17.122491 cacholote-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:19:17.126490 cacholote-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-11 10:18:58.000000 cacholote-0.3.2/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-11 10:18:58.000000 cacholote-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-11 10:18:58.000000 cacholote-0.3.2/.pre-commit-config-cruft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-11 10:18:58.000000 cacholote-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-11 10:18:58.000000 cacholote-0.3.2/DESIGN.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-11 10:18:58.000000 cacholote-0.3.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-07-11 10:18:58.000000 cacholote-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-11 10:18:58.000000 cacholote-0.3.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-11 10:18:58.000000 cacholote-0.3.2/OBJECT-STORAGE-DESIGN.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-07-11 10:19:17.130490 cacholote-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-11 10:18:58.000000 cacholote-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:19:17.126490 cacholote-0.3.2/cacholote/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-11 10:18:58.000000 cacholote-0.3.2/cacholote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-11 10:18:58.000000 cacholote-0.3.2/cacholote/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-07-11 10:18:58.000000 cacholote-0.3.2/cacholote/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-07-11 10:18:58.000000 cacholote-0.3.2/cacholote/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-11 10:18:58.000000 cacholote-0.3.2/cacholote/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-11 10:18:58.000000 cacholote-0.3.2/cacholote/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-11 10:18:58.000000 cacholote-0.3.2/cacholote/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-07-11 10:18:58.000000 cacholote-0.3.2/cacholote/extra_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:58.000000 cacholote-0.3.2/cacholote/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-11 10:18:58.000000 cacholote-0.3.2/cacholote/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 10:19:17.000000 cacholote-0.3.2/cacholote/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:19:17.126490 cacholote-0.3.2/cacholote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-07-11 10:19:17.000000 cacholote-0.3.2/cacholote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-11 10:19:17.000000 cacholote-0.3.2/cacholote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:19:17.000000 cacholote-0.3.2/cacholote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 10:19:17.000000 cacholote-0.3.2/cacholote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 10:19:17.000000 cacholote-0.3.2/cacholote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:19:17.126490 cacholote-0.3.2/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-11 10:18:58.000000 cacholote-0.3.2/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-11 10:18:58.000000 cacholote-0.3.2/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:19:17.126490 cacholote-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-11 10:18:58.000000 cacholote-0.3.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:19:17.126490 cacholote-0.3.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:58.000000 cacholote-0.3.2/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:19:17.126490 cacholote-0.3.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:58.000000 cacholote-0.3.2/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-11 10:18:58.000000 cacholote-0.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-11 10:18:58.000000 cacholote-0.3.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-11 10:18:58.000000 cacholote-0.3.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-11 10:18:58.000000 cacholote-0.3.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-11 10:18:58.000000 cacholote-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 10:19:17.130490 cacholote-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:19:17.130490 cacholote-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-11 10:18:58.000000 cacholote-0.3.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 10:18:58.000000 cacholote-0.3.2/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-11 10:18:58.000000 cacholote-0.3.2/tests/test_01_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-11 10:18:58.000000 cacholote-0.3.2/tests/test_02_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-11 10:18:58.000000 cacholote-0.3.2/tests/test_10_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-11 10:18:58.000000 cacholote-0.3.2/tests/test_20_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-11 10:18:58.000000 cacholote-0.3.2/tests/test_30_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-11 10:18:58.000000 cacholote-0.3.2/tests/test_40_xarray_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-11 10:18:58.000000 cacholote-0.3.2/tests/test_50_io_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-11 10:18:58.000000 cacholote-0.3.2/tests/test_60_clean.py
```

### Comparing `cacholote-0.3.1/.cruft.json` & `cacholote-0.3.2/.cruft.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'9627920059b31038e1bb8a978921806cb835fde7'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "abe10924d34c36556d1767e1833b88ea93df0e13",
+    "commit": "9627920059b31038e1bb8a978921806cb835fde7",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/ecmwf-projects/cookiecutter-conda-package",
             "copyright_holder": "B-Open Solutions srl",
             "copyright_year": "2019",
             "integration_tests": "True",
             "mypy_strict": "True",
```

### Comparing `cacholote-0.3.1/.github/workflows/on-push.yml` & `cacholote-0.3.2/.github/workflows/on-push.yml`

 * *Files 9% similar despite different names*

```diff
@@ -44,34 +44,36 @@
     - name: Archive combined environments
       uses: actions/upload-artifact@v3
       with:
         name: combined-environments
         path: ci/combined-environment-*.yml
 
   unit-tests:
-    name: unit-tests (3.10)
+    name: unit-tests
     needs: combine-environments
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: ['3.10', '3.11']
 
     steps:
     - uses: actions/checkout@v3
     - name: Download combined environments
       uses: actions/download-artifact@v3
       with:
         name: combined-environments
         path: ci
     - name: Install Conda environment with Micromamba
-      uses: mamba-org/provision-with-micromamba@v15
+      uses: mamba-org/setup-micromamba@v1
       with:
         environment-file: ci/combined-environment-ci.yml
         environment-name: DEVELOP
-        channels: conda-forge
-        cache-env: true
-        extra-specs: |
-          python=3.10
+        cache-environment: true
+        create-args: >-
+          python=${{ matrix.python-version }}
     - name: Install package
       run: |
         python -m pip install --no-deps -e .
     - name: Run tests
       run: |
         make unit-tests COV_REPORT=xml
 
@@ -83,21 +85,20 @@
     - uses: actions/checkout@v3
     - name: Download combined environments
       uses: actions/download-artifact@v3
       with:
         name: combined-environments
         path: ci
     - name: Install Conda environment with Micromamba
-      uses: mamba-org/provision-with-micromamba@v15
+      uses: mamba-org/setup-micromamba@v1
       with:
         environment-file: ci/combined-environment-ci.yml
         environment-name: DEVELOP
-        channels: conda-forge
-        cache-env: true
-        extra-specs: |
+        cache-environment: true
+        create-args: >-
           python=3.10
     - name: Install package
       run: |
         python -m pip install --no-deps -e .
     - name: Run code quality checks
       run: |
         make type-check
@@ -110,21 +111,20 @@
     - uses: actions/checkout@v3
     - name: Download combined environments
       uses: actions/download-artifact@v3
       with:
         name: combined-environments
         path: ci
     - name: Install Conda environment with Micromamba
-      uses: mamba-org/provision-with-micromamba@v15
+      uses: mamba-org/setup-micromamba@v1
       with:
         environment-file: ci/combined-environment-ci.yml
         environment-name: DEVELOP
-        channels: conda-forge
-        cache-env: true
-        extra-specs: |
+        cache-environment: true
+        create-args: >-
           python=3.10
     - name: Install package
       run: |
         python -m pip install --no-deps -e .
     - name: Build documentation
       run: |
         make docs-build
@@ -133,35 +133,34 @@
     needs: [combine-environments, unit-tests]
     if: |
       success() && true
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        python-version: [3.8, 3.11]
-        extra: [-ci]
         include:
+        - python-version: '3.8'
+          extra: -ci
         - python-version: '3.10'
           extra: -integration
 
     steps:
     - uses: actions/checkout@v3
     - name: Download combined environments
       uses: actions/download-artifact@v3
       with:
         name: combined-environments
         path: ci
     - name: Install Conda environment with Micromamba
-      uses: mamba-org/provision-with-micromamba@v15
+      uses: mamba-org/setup-micromamba@v1
       with:
         environment-file: ci/combined-environment${{ matrix.extra }}.yml
         environment-name: DEVELOP${{ matrix.extra }}
-        channels: conda-forge
-        cache-env: true
-        extra-specs: |
+        cache-environment: true
+        create-args: >-
           python=${{ matrix.python-version }}
     - name: Install package
       run: |
         python -m pip install --no-deps -e .
     - name: Run tests
       run: |
         make unit-tests COV_REPORT=xml
```

### Comparing `cacholote-0.3.1/.gitignore` & `cacholote-0.3.2/.gitignore`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,66 @@
 # setuptools-scm
 version.py
 
 # Sphinx automatic generation of API
 docs/_api/
 
-# Created by https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks,vim,visualstudiocode,pycharm
-# Edit at https://www.toptal.com/developers/gitignore?templates=python,jupyternotebooks,vim,visualstudiocode,pycharm
+# Created by https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks,vim,visualstudiocode,pycharm,emacs,linux,macos,windows
+# Edit at https://www.toptal.com/developers/gitignore?templates=python,jupyternotebooks,vim,visualstudiocode,pycharm,emacs,linux,macos,windows
+
+### Emacs ###
+# -*- mode: gitignore; -*-
+*~
+\#*\#
+/.emacs.desktop
+/.emacs.desktop.lock
+*.elc
+auto-save-list
+tramp
+.\#*
+
+# Org-mode
+.org-id-locations
+*_archive
+
+# flymake-mode
+*_flymake.*
+
+# eshell files
+/eshell/history
+/eshell/lastdir
+
+# elpa packages
+/elpa/
+
+# reftex files
+*.rel
+
+# AUCTeX auto folder
+/auto/
+
+# cask packages
+.cask/
+dist/
+
+# Flycheck
+flycheck_*.el
+
+# server auth directory
+/server/
+
+# projectiles files
+.projectile
+
+# directory configuration
+.dir-locals.el
+
+# network security
+/network-security.data
+
 
 ### JupyterNotebooks ###
 # gitignore template for Jupyter Notebooks
 # website: http://jupyter.org/
 
 .ipynb_checkpoints
 */.ipynb_checkpoints/*
@@ -17,14 +68,60 @@
 # IPython
 profile_default/
 ipython_config.py
 
 # Remove previous ipynb_checkpoints
 #   git rm -r .ipynb_checkpoints/
 
+### Linux ###
+
+# temporary files which can be created if a process still has a handle open of a deleted file
+.fuse_hidden*
+
+# KDE directory preferences
+.directory
+
+# Linux trash folder which might appear on any partition or disk
+.Trash-*
+
+# .nfs files are created when an open file is removed but is still being accessed
+.nfs*
+
+### macOS ###
+# General
+.DS_Store
+.AppleDouble
+.LSOverride
+
+# Icon must end with two \r
+Icon
+
+# Thumbnails
+._*
+
+# Files that might appear in the root of a volume
+.DocumentRevisions-V100
+.fseventsd
+.Spotlight-V100
+.TemporaryItems
+.Trashes
+.VolumeIcon.icns
+.com.apple.timemachine.donotpresent
+
+# Directories potentially created on remote AFP share
+.AppleDB
+.AppleDesktop
+Network Trash Folder
+Temporary Items
+.apdisk
+
+### macOS Patch ###
+# iCloud generated files
+*.icloud
+
 ### PyCharm ###
 # Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio, WebStorm and Rider
 # Reference: https://intellij-support.jetbrains.com/hc/en-us/articles/206544839
 
 # User-specific stuff
 .idea/**/workspace.xml
 .idea/**/tasks.xml
@@ -143,15 +240,14 @@
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
-dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
@@ -314,15 +410,14 @@
 
 # Session
 Session.vim
 Sessionx.vim
 
 # Temporary
 .netrwhist
-*~
 # Auto-generated tag files
 tags
 # Persistent undo
 [._]*.un~
 
 ### VisualStudioCode ###
 .vscode/
@@ -340,11 +435,34 @@
 *.vsix
 
 ### VisualStudioCode Patch ###
 # Ignore all local history of files
 .history
 .ionide
 
-# Ignore code-workspaces
-*.code-workspace
+### Windows ###
+# Windows thumbnail cache files
+Thumbs.db
+Thumbs.db:encryptable
+ehthumbs.db
+ehthumbs_vista.db
+
+# Dump file
+*.stackdump
+
+# Folder config file
+[Dd]esktop.ini
+
+# Recycle Bin used on file shares
+$RECYCLE.BIN/
+
+# Windows Installer files
+*.cab
+*.msi
+*.msix
+*.msm
+*.msp
+
+# Windows shortcuts
+*.lnk
 
-# End of https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks,vim,visualstudiocode,pycharm
+# End of https://www.toptal.com/developers/gitignore/api/python,jupyternotebooks,vim,visualstudiocode,pycharm,emacs,linux,macos,windows
```

### Comparing `cacholote-0.3.1/.pre-commit-config.yaml` & `cacholote-0.3.2/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -15,23 +15,23 @@
   hooks:
   - id: black
 - repo: https://github.com/keewis/blackdoc
   rev: v0.3.8
   hooks:
   - id: blackdoc
     additional_dependencies: [black==22.3.0]
-- repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: v0.0.263
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  rev: v0.0.277
   hooks:
   - id: ruff
-    args: [--fix]
+    args: [--fix, --show-fixes]
 - repo: https://github.com/executablebooks/mdformat
   rev: 0.7.16
   hooks:
   - id: mdformat
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.8.0
+  rev: v2.9.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --preserve-quotes]
   - id: pretty-format-toml
     args: [--autofix]
```

### Comparing `cacholote-0.3.1/DESIGN.rst` & `cacholote-0.3.2/DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/LICENSE` & `cacholote-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/Makefile` & `cacholote-0.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/OBJECT-STORAGE-DESIGN.rst` & `cacholote-0.3.2/OBJECT-STORAGE-DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/PKG-INFO` & `cacholote-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 0.3.1
+Version: 0.3.2
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -207,14 +207,15 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cacholote
 
 Efficiently cache calls to functions
```

### Comparing `cacholote-0.3.1/README.md` & `cacholote-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/cacholote/__init__.py` & `cacholote-0.3.2/cacholote/__init__.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/cacholote/cache.py` & `cacholote-0.3.2/cacholote/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import datetime
 import functools
 import json
 import warnings
 from typing import Any, Callable, TypeVar, cast
 
 import sqlalchemy as sa
 import sqlalchemy.orm
 
-from . import clean, config, database, decode, encode
+from . import clean, config, database, decode, encode, utils
 
 F = TypeVar("F", bound=Callable[..., Any])
 
 
 def _decode_and_update(
     session: sa.orm.Session,
     cache_entry: Any,
@@ -61,15 +60,15 @@
             if settings.return_cache_entry:
                 raise ex
             warnings.warn(f"can NOT encode python call: {ex!r}", UserWarning)
             return func(*args, **kwargs)
 
         filters = [
             database.CacheEntry.key == hexdigest,
-            database.CacheEntry.expiration > datetime.datetime.utcnow(),
+            database.CacheEntry.expiration > utils.utcnow(),
         ]
         if settings.expiration:
             # When expiration is provided, only get entries with matching expiration
             filters.append(database.CacheEntry.expiration == settings.expiration)
 
         with settings.sessionmaker() as session:
             for cache_entry in session.scalars(
```

### Comparing `cacholote-0.3.1/cacholote/clean.py` & `cacholote-0.3.2/cacholote/clean.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,56 +19,52 @@
 import functools
 import json
 import posixpath
 from typing import Any, Callable, Dict, List, Literal, Optional, Sequence, Set, Union
 
 import sqlalchemy as sa
 import sqlalchemy.orm
-import structlog
 
 from . import config, database, encode, extra_encoders, utils
 
-LOGGER = structlog.get_logger()
-
 
 def _delete_cache_file(
     obj: Dict[str, Any],
     session: Optional[sa.orm.Session] = None,
     cache_entry: Optional[database.CacheEntry] = None,
     sizes: Optional[Dict[str, int]] = None,
     dry_run: bool = False,
-    logger: Optional[structlog.stdlib.BoundLogger] = None,
 ) -> Any:
-    logger = logger or LOGGER
+    logger = config.get().logger
 
     if {"type", "callable", "args", "kwargs"} == set(obj) and obj["callable"] in (
         "cacholote.extra_encoders:decode_xr_dataset",
         "cacholote.extra_encoders:decode_io_object",
     ):
         sizes = sizes or {}
         cache_fs, cache_dirname = utils.get_cache_files_fs_dirname()
         cache_dirname = cache_fs.unstrip_protocol(cache_dirname)
 
         fs, urlpath = extra_encoders._get_fs_and_urlpath(*obj["args"][:2])
         urlpath = fs.unstrip_protocol(urlpath)
 
         if posixpath.dirname(urlpath) == cache_dirname:
             sizes.pop(urlpath, None)
-            if session and cache_entry and not dry_run:
-                logger.info("Delete cache entry", cache_entry=cache_entry)
-                session.delete(cache_entry)
-                database._commit_or_rollback(session)
             if not dry_run:
-                with utils._Locker(fs, urlpath) as file_exists:
-                    if file_exists:
-                        logger.info("Delete cache file", urlpath=urlpath)
-                        fs.rm(
-                            urlpath,
-                            recursive=obj["args"][0]["type"] == "application/vnd+zarr",
-                        )
+                if session and cache_entry:
+                    logger.info("delete cache entry", cache_entry=cache_entry)
+                    session.delete(cache_entry)
+                    database._commit_or_rollback(session)
+
+                if fs.exists(urlpath):
+                    logger.info("delete cache file", urlpath=urlpath)
+                    fs.rm(
+                        urlpath,
+                        recursive=obj["args"][0]["type"] == "application/vnd+zarr",
+                    )
 
     return obj
 
 
 def _delete_cache_entry(
     session: sa.orm.Session, cache_entry: database.CacheEntry
 ) -> None:
@@ -98,43 +94,40 @@
         for cache_entry in session.scalars(
             sa.select(database.CacheEntry).filter(database.CacheEntry.key == hexdigest)
         ):
             _delete_cache_entry(session, cache_entry)
 
 
 class _Cleaner:
-    def __init__(self, logger: structlog.stdlib.BoundLogger) -> None:
-        fs, dirname = utils.get_cache_files_fs_dirname()
-        urldir = fs.unstrip_protocol(dirname)
-
-        logger.info("Get disk usage of cache files")
-        sizes: Dict[str, int] = collections.defaultdict(lambda: 0)
-        for path, size in fs.du(dirname, total=False).items():
+    def __init__(self) -> None:
+        self.logger = config.get().logger
+        self.fs, self.dirname = utils.get_cache_files_fs_dirname()
+
+        urldir = self.fs.unstrip_protocol(self.dirname)
+
+        self.logger.info("get disk usage of cache files")
+        self.sizes: Dict[str, int] = collections.defaultdict(lambda: 0)
+        for path, size in self.fs.du(self.dirname, total=False).items():
             # Group dirs
-            urlpath = fs.unstrip_protocol(path)
+            urlpath = self.fs.unstrip_protocol(path)
             basename, *_ = urlpath.replace(urldir, "", 1).strip("/").split("/")
             if basename:
-                sizes[posixpath.join(urldir, basename)] += size
-
-        self.logger = logger
-        self.fs = fs
-        self.dirname = dirname
-        self.sizes = sizes
+                self.sizes[posixpath.join(urldir, basename)] += size
 
     @property
     def size(self) -> int:
         sum_sizes = sum(self.sizes.values())
-        self.logger.info("Check cache files total size", size=sum_sizes)
+        self.logger.info("check cache files total size", size=sum_sizes)
         return sum_sizes
 
     def stop_cleaning(self, maxsize: int) -> bool:
         return self.size <= maxsize
 
     def get_unknown_files(self, lock_validity_period: Optional[float]) -> Set[str]:
-        self.logger.info("Get unknown files")
+        self.logger.info("get unknown files")
         now = datetime.datetime.now()
         files_to_skip = []
         for urlpath in self.sizes:
             if urlpath.endswith(".lock"):
                 delta = now - self.fs.modified(urlpath)
                 if lock_validity_period is None or delta < datetime.timedelta(
                     seconds=lock_validity_period
@@ -148,30 +141,26 @@
                 for cache_entry in session.scalars(sa.select(database.CacheEntry)):
                     json.loads(
                         cache_entry._result_as_string,
                         object_hook=functools.partial(
                             _delete_cache_file,
                             sizes=unknown_sizes,
                             dry_run=True,
-                            logger=self.logger,
                         ),
                     )
         return set(unknown_sizes)
 
     def delete_unknown_files(
         self, lock_validity_period: Optional[float], recursive: bool
     ) -> None:
         for urlpath in self.get_unknown_files(lock_validity_period):
             self.sizes.pop(urlpath)
-            with utils._Locker(self.fs, urlpath, lock_validity_period) as file_exists:
-                if file_exists:
-                    self.logger.info(
-                        "Delete unknown", urlpath=urlpath, recursive=recursive
-                    )
-                    self.fs.rm(urlpath, recursive=recursive)
+            if self.fs.exists(urlpath):
+                self.logger.info("delete unknown", urlpath=urlpath, recursive=recursive)
+                self.fs.rm(urlpath, recursive=recursive)
 
     @staticmethod
     def check_tags(*args: Any) -> None:
         if None not in args:
             raise ValueError("tags_to_clean/keep are mutually exclusive.")
         for tags in args:
             if tags is not None and (
@@ -232,15 +221,14 @@
                 json.loads(
                     cache_entry._result_as_string,
                     object_hook=functools.partial(
                         _delete_cache_file,
                         session=session,
                         cache_entry=cache_entry,
                         sizes=self.sizes,
-                        logger=self.logger,
                     ),
                 )
                 if self.stop_cleaning(maxsize):
                     return
 
         raise ValueError(
             f"Unable to clean {self.dirname!r}. Final size: {self.size!r}. Expected size: {maxsize!r}"
@@ -251,15 +239,14 @@
     maxsize: int,
     method: Literal["LRU", "LFU"] = "LRU",
     delete_unknown_files: bool = False,
     recursive: bool = False,
     lock_validity_period: Optional[float] = None,
     tags_to_clean: Optional[Sequence[Optional[str]]] = None,
     tags_to_keep: Optional[Sequence[Optional[str]]] = None,
-    logger: Optional[structlog.stdlib.BoundLogger] = None,
 ) -> None:
     """Clean cache files.
 
     Parameters
     ----------
     maxsize: int
         Maximum total size of cache files (bytes).
@@ -272,18 +259,16 @@
         Whether to delete unknown directories or not
     lock_validity_period: float, optional, default: None
         Validity period of lock files in seconds. Expired locks will be deleted.
     tags_to_clean, tags_to_keep: sequence of strings/None, optional, default: None
         Tags to clean/keep. If None, delete all cache entries.
         To delete/keep untagged entries, add None in the sequence (e.g., [None, 'tag1', ...]).
         tags_to_clean and tags_to_keep are mutually exclusive.
-    logger: optional
-        Python object use to produce logs.
     """
-    cleaner = _Cleaner(logger=logger or LOGGER)
+    cleaner = _Cleaner()
 
     if delete_unknown_files:
         cleaner.delete_unknown_files(lock_validity_period, recursive)
 
     cleaner.delete_cache_files(
         maxsize=maxsize,
         method=method,
```

### Comparing `cacholote-0.3.1/cacholote/config.py` & `cacholote-0.3.2/cacholote/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,31 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import datetime
+import logging
 import pathlib
 import tempfile
 from types import TracebackType
 from typing import Any, Dict, Literal, Optional, Tuple, Type, Union
 
 import fsspec
 import pydantic
 import sqlalchemy as sa
 import sqlalchemy.orm
+import structlog
 
 from . import database
 
+_LOGGER = structlog.get_logger(
+    wrapper_class=structlog.make_filtering_bound_logger(logging.WARNING)
+)
 _SETTINGS: Optional[Settings] = None
 _DEFAULT_CACHE_DIR = pathlib.Path(tempfile.gettempdir()) / "cacholote"
 _DEFAULT_CACHE_DIR.mkdir(exist_ok=True)
 
 _CONFIG_NOT_SET_MSG = (
     "Configuration settings have not been set. Run `cacholote.config.reset()`."
 )
@@ -48,14 +53,17 @@
         "application/netcdf", "application/x-grib", "application/vnd+zarr"
     ] = "application/netcdf"
     io_delete_original: bool = False
     raise_all_encoding_errors: bool = False
     expiration: Optional[datetime.datetime] = None
     tag: Optional[str] = None
     return_cache_entry: bool = False
+    logger: Union[
+        structlog.BoundLogger, structlog._config.BoundLoggerLazyProxy
+    ] = _LOGGER
 
     @pydantic.validator("create_engine_kwargs", allow_reuse=True)
     def validate_create_engine_kwargs(
         cls: pydantic.BaseSettings, create_engine_kwargs: Dict[str, Any]
     ) -> Dict[str, Any]:
         poolclass = create_engine_kwargs.get("poolclass")
         if isinstance(poolclass, str):
@@ -68,14 +76,22 @@
     ) -> bool:
         if return_cache_entry is True and values["use_cache"] is False:
             raise ValueError(
                 "`use_cache` must be True when `return_cache_entry` is True"
             )
         return return_cache_entry
 
+    @pydantic.validator("expiration", allow_reuse=True)
+    def validate_expiration(
+        cls: pydantic.BaseSettings, expiration: Optional[datetime.datetime]
+    ) -> Optional[datetime.datetime]:
+        if expiration is not None and expiration.tzinfo is None:
+            raise ValueError(f"Expiration is missing the timezone info. {expiration=}")
+        return expiration
+
     def make_cache_dir(self) -> None:
         fs, _, (urlpath, *_) = fsspec.get_fs_token_paths(
             self.cache_files_urlpath,
             storage_options=self.cache_files_storage_options,
         )
         fs.mkdirs(urlpath, exist_ok=True)
```

### Comparing `cacholote-0.3.1/cacholote/database.py` & `cacholote-0.3.2/cacholote/database.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,31 +17,37 @@
 import datetime
 import json
 from typing import Any, Dict, Optional
 
 import sqlalchemy as sa
 import sqlalchemy.orm
 
+from . import utils
+
+_DATETIME_MAX = datetime.datetime(
+    datetime.MAXYEAR, 12, 31, tzinfo=datetime.timezone.utc
+)
+
 ENGINE: Optional[sa.engine.Engine] = None
 SESSIONMAKER: Optional[sa.orm.sessionmaker] = None  # type: ignore[type-arg]
 
 Base = sa.orm.declarative_base()
 
 
 class CacheEntry(Base):
     __tablename__ = "cache_entries"
 
     id = sa.Column(sa.Integer(), primary_key=True)
     key = sa.Column(sa.String(32))
-    expiration = sa.Column(sa.DateTime, default=datetime.datetime.max)
+    expiration = sa.Column(sa.DateTime, default=_DATETIME_MAX)
     result = sa.Column(sa.JSON)
     timestamp = sa.Column(
         sa.DateTime,
-        default=datetime.datetime.utcnow,
-        onupdate=datetime.datetime.utcnow,
+        default=utils.utcnow,
+        onupdate=utils.utcnow,
     )
     counter = sa.Column(sa.Integer)
     tag = sa.Column(sa.String)
 
     @property
     def _result_as_string(self) -> str:
         return json.dumps(self.result)
@@ -52,17 +58,17 @@
 
 @sa.event.listens_for(CacheEntry, "before_insert")
 def set_expiration_to_max(
     mapper: sa.orm.Mapper[CacheEntry],
     connection: sa.Connection,
     target: CacheEntry,
 ) -> None:
-    target.expiration = target.expiration or datetime.datetime.max
-    if target.expiration < datetime.datetime.utcnow():
-        raise ValueError("Expiration date has passed.")
+    target.expiration = target.expiration or _DATETIME_MAX
+    if target.expiration < utils.utcnow():
+        raise ValueError(f"Expiration date has passed. {target.expiration=}")
 
 
 def _commit_or_rollback(session: sa.orm.Session) -> None:
     try:
         session.commit()
     finally:
         session.rollback()
```

### Comparing `cacholote-0.3.1/cacholote/decode.py` & `cacholote-0.3.2/cacholote/decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/cacholote/encode.py` & `cacholote-0.3.2/cacholote/encode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/cacholote/extra_encoders.py` & `cacholote-0.3.2/cacholote/extra_encoders.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+import contextlib
 import functools
 import hashlib
 import inspect
 import io
 import mimetypes
 import pathlib
 import posixpath
 import tempfile
-from typing import Any, Callable, Dict, Optional, Tuple, TypeVar, Union, cast
+import time
+from typing import Any, Callable, Dict, Generator, Optional, Tuple, TypeVar, Union, cast
 
 import fsspec
 import fsspec.implementations.local
 import pydantic
 
 from . import config, encode, utils
 
@@ -92,31 +93,42 @@
         if not _HAS_XARRAY_AND_DASK:
             raise ValueError("please install 'xarray' and 'dask'")
         return func(*args, **kwargs)
 
     return cast(F, wrapper)
 
 
+@contextlib.contextmanager
+def _logging_timer(event: str, **kwargs: Any) -> Generator[float, None, None]:
+    logger = config.get().logger
+    logger.info(f"start {event}", **kwargs)
+    tic = time.perf_counter()
+    yield tic
+    toc = time.perf_counter()
+    kwargs["_".join(event.split() + ["time"])] = toc - tic  # elapsed time
+    logger.info(f"end {event}", **kwargs)
+
+
 class FileInfoModel(pydantic.BaseModel):
     type: str
     href: str
-    file_checksum: int = pydantic.Field(..., alias="file:checksum")
+    file_checksum: str = pydantic.Field(..., alias="file:checksum")
     file_size: int = pydantic.Field(..., alias="file:size")
     file_local_path: str = pydantic.Field(..., alias="file:local_path")
 
 
 def _dictify_file(fs: fsspec.AbstractFileSystem, local_path: str) -> Dict[str, Any]:
     href = posixpath.join(
         config.get().cache_files_urlpath_readonly or config.get().cache_files_urlpath,
         posixpath.basename(local_path),
     )
     file_dict = {
         "type": _guess_type(fs, local_path),
         "href": href,
-        "file:checksum": fs.checksum(local_path),
+        "file:checksum": f"{fs.checksum(local_path):x}",
         "file:size": fs.size(local_path),
         "file:local_path": local_path,
     }
 
     return FileInfoModel(**file_dict).dict(by_alias=True)
 
 
@@ -136,17 +148,23 @@
     # Attempt to read from local_path
     try:
         fs, *_ = fsspec.get_fs_token_paths(urlpath, storage_options=storage_options)
     except:  # noqa: E722
         pass
     else:
         if fs.exists(urlpath):
-            if fs.checksum(urlpath) == file_json["file:checksum"]:
-                return (fs, urlpath)
-            raise ValueError("checksum mismatch")
+            expected = file_json["file:checksum"]
+            actual = (
+                fs.checksum(urlpath)  # Just for backward compatibility.
+                if isinstance(expected, int)
+                else f"{fs.checksum(urlpath):x}"
+            )
+            if expected != actual:
+                raise ValueError(f"checksum mismatch: {expected=} {actual=}")
+            return (fs, urlpath)
 
     # Attempt to read from href
     urlpath = file_json["href"]
     fs, *_ = fsspec.get_fs_token_paths(urlpath)
     if fs.exists(urlpath):
         return (fs, urlpath)
 
@@ -193,29 +211,31 @@
 @_requires_xarray_and_dask
 def _maybe_store_xr_dataset(
     obj: "xr.Dataset", fs: fsspec.AbstractFileSystem, urlpath: str, filetype: str
 ) -> None:
     if filetype == "application/vnd+zarr":
         # Write directly on any filesystem
         mapper = fs.get_mapper(urlpath)
-        obj.to_zarr(mapper, consolidated=True)
+        with _logging_timer("upload", urlpath=fs.unstrip_protocol(urlpath)):
+            obj.to_zarr(mapper, consolidated=True)
     else:
         # Need a tmp local copy to write on a different filesystem
         with tempfile.TemporaryDirectory() as tmpdirname:
             tmpfilename = str(pathlib.Path(tmpdirname) / pathlib.Path(urlpath).name)
 
-            if filetype == "application/netcdf":
-                obj.to_netcdf(tmpfilename)
-            elif filetype == "application/x-grib":
-                import cfgrib.xarray_to_grib
-
-                cfgrib.xarray_to_grib.to_grib(obj, tmpfilename)
-            else:
-                # Should never get here! xarray_cache_type is checked in config.py
-                raise ValueError(f"type {filetype!r} is NOT supported.")
+            with _logging_timer("download", urlpath=tmpfilename):
+                if filetype == "application/netcdf":
+                    obj.to_netcdf(tmpfilename)
+                elif filetype == "application/x-grib":
+                    import cfgrib.xarray_to_grib
+
+                    cfgrib.xarray_to_grib.to_grib(obj, tmpfilename)
+                else:
+                    # Should never get here! xarray_cache_type is checked in config.py
+                    raise ValueError(f"type {filetype!r} is NOT supported.")
 
             _maybe_store_file_object(
                 fsspec.filesystem("file"), tmpfilename, fs, urlpath
             )
 
 
 @_requires_xarray_and_dask
@@ -255,39 +275,49 @@
 ) -> None:
     with utils._Locker(fs_out, urlpath_out) as file_exists:
         if not file_exists:
             kwargs = {}
             content_type = _guess_type(fs_in, urlpath_in)
             if content_type:
                 kwargs["ContentType"] = content_type
-            if fs_in == fs_out:
-                if config.get().io_delete_original:
-                    fs_in.mv(urlpath_in, urlpath_out, **kwargs)
+            with _logging_timer(
+                "upload",
+                urlpath=fs_out.unstrip_protocol(urlpath_out),
+                size=fs_in.size(urlpath_in),
+            ):
+                if fs_in == fs_out:
+                    if config.get().io_delete_original:
+                        fs_in.mv(urlpath_in, urlpath_out, **kwargs)
+                    else:
+                        fs_in.cp(urlpath_in, urlpath_out, **kwargs)
+                elif fs_in.protocol == "file":
+                    fs_out.put(urlpath_in, urlpath_out, **kwargs)
                 else:
-                    fs_in.cp(urlpath_in, urlpath_out, **kwargs)
-            elif fs_in.protocol == "file":
-                fs_out.put(urlpath_in, urlpath_out, **kwargs)
-            else:
-                with fs_in.open(urlpath_in, "rb") as f_in, fs_out.open(
-                    urlpath_out, "wb"
-                ) as f_out:
-                    utils.copy_buffered_file(f_in, f_out)
+                    with fs_in.open(urlpath_in, "rb") as f_in:
+                        with fs_out.open(urlpath_out, "wb") as f_out:
+                            utils.copy_buffered_file(f_in, f_out)
     if config.get().io_delete_original and fs_in.exists(urlpath_in):
-        fs_in.rm(urlpath_in)
+        with _logging_timer(
+            "remove",
+            urlpath=fs_in.unstrip_protocol(urlpath_in),
+            size=fs_in.size(urlpath_in),
+        ):
+            fs_in.rm(urlpath_in)
 
 
 def _maybe_store_io_object(
     f_in: _UNION_IO_TYPES,
     fs_out: fsspec.AbstractFileSystem,
     urlpath_out: str,
 ) -> None:
     with utils._Locker(fs_out, urlpath_out) as file_exists:
         if not file_exists:
             f_out = fs_out.open(urlpath_out, "wb")
-            utils.copy_buffered_file(f_in, f_out)
+            with _logging_timer("upload", urlpath=fs_out.unstrip_protocol(urlpath_out)):
+                utils.copy_buffered_file(f_in, f_out)
 
 
 def dictify_io_object(obj: _UNION_IO_TYPES) -> Dict[str, Any]:
     """Encode a file object to JSON deserialized data (``dict``)."""
     cache_files_urlpath = config.get().cache_files_urlpath
     fs_out, *_ = fsspec.get_fs_token_paths(
         cache_files_urlpath,
```

### Comparing `cacholote-0.3.1/cacholote/utils.py` & `cacholote-0.3.2/cacholote/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -122,7 +122,12 @@
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
         self.release()
+
+
+def utcnow() -> datetime.datetime:
+    """See https://discuss.python.org/t/deprecating-utcnow-and-utcfromtimestamp/26221."""
+    return datetime.datetime.now(tz=datetime.timezone.utc)
```

### Comparing `cacholote-0.3.1/cacholote.egg-info/PKG-INFO` & `cacholote-0.3.2/cacholote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 0.3.1
+Version: 0.3.2
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -207,14 +207,15 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cacholote
 
 Efficiently cache calls to functions
```

### Comparing `cacholote-0.3.1/cacholote.egg-info/SOURCES.txt` & `cacholote-0.3.2/cacholote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/docs/Makefile` & `cacholote-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/docs/conf.py` & `cacholote-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/docs/make.bat` & `cacholote-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/pyproject.toml` & `cacholote-0.3.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,20 @@
   "Development Status :: 2 - Pre-Alpha",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering"
 ]
 dependencies = [
   "fsspec",
-  "pydantic[dotenv]",
+  "pydantic[dotenv]==1.*",
   "sqlalchemy>=2.0.9",
   "structlog"
 ]
 description = "Efficiently cache calls to functions"
 dynamic = ["version"]
 license = {file = "LICENSE"}
 name = "cacholote"
```

### Comparing `cacholote-0.3.1/tests/conftest.py` & `cacholote-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/tests/test_01_settings.py` & `cacholote-0.3.2/tests/test_01_settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+import contextlib
+import datetime
 import os
 import pathlib
 from typing import Any, Dict, Union
 
 import pytest
 import sqlalchemy as sa
 
 from cacholote import config
 
+does_not_raise = contextlib.nullcontext
+
 
 def test_change_cache_db_urlpath(tmpdir: pathlib.Path) -> None:
     old_db = config.get().cache_db_urlpath
     new_db = "sqlite:///" + str(tmpdir / "dummy.db")
 
     with config.set(cache_db_urlpath=new_db):
         assert str(config.get().engine.url) == config.get().cache_db_urlpath == new_db
@@ -86,7 +90,29 @@
 
 @pytest.mark.parametrize("poolclass", ("NullPool", sa.pool.NullPool))
 def test_set_poolclass(poolclass: Union[str, sa.pool.Pool]) -> None:
     config.set(create_engine_kwargs={"poolclass": poolclass})
     settings = config.get()
     assert settings.create_engine_kwargs["poolclass"] == sa.pool.NullPool
     assert isinstance(settings.engine.pool, sa.pool.NullPool)
+
+
+@pytest.mark.parametrize(
+    "expiration,raises",
+    [
+        (
+            datetime.datetime.now(),
+            pytest.raises(ValueError, match="Expiration is missing the timezone info."),
+        ),
+        (
+            datetime.datetime.now().isoformat(),
+            pytest.raises(ValueError, match="Expiration is missing the timezone info."),
+        ),
+        (datetime.datetime.now(tz=datetime.timezone.utc), does_not_raise()),
+        (datetime.datetime.now(tz=datetime.timezone.utc).isoformat(), does_not_raise()),
+    ],
+)
+def test_set_expiration(
+    expiration: Union[datetime.datetime, str], raises: contextlib.nullcontext  # type: ignore[type-arg]
+) -> None:
+    with raises:
+        config.set(expiration=expiration)
```

### Comparing `cacholote-0.3.1/tests/test_02_utils.py` & `cacholote-0.3.2/tests/test_02_utils.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/tests/test_10_decode.py` & `cacholote-0.3.2/tests/test_10_decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/tests/test_20_encode.py` & `cacholote-0.3.2/tests/test_20_encode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.1/tests/test_30_cache.py` & `cacholote-0.3.2/tests/test_30_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,35 +32,35 @@
 def test_cacheable(tmpdir: pathlib.Path) -> None:
     con = config.get().engine.raw_connection()
     cur = con.cursor()
 
     cfunc = cache.cacheable(func)
 
     for counter in range(1, 3):
-        before = datetime.datetime.utcnow()
+        before = datetime.datetime.now(tz=datetime.timezone.utc)
         res = cfunc("test")
-        after = datetime.datetime.utcnow()
+        after = datetime.datetime.now(tz=datetime.timezone.utc)
         assert res == {"a": "test", "args": [], "b": None, "kwargs": {}}
 
         cur.execute(
             "SELECT id, key, expiration, result, counter FROM cache_entries", ()
         )
         assert cur.fetchall() == [
             (
                 1,
                 "a8260ac3cdc1404aa64a6fb71e853049",
-                "9999-12-31 23:59:59.999999",
+                "9999-12-31 00:00:00.000000",
                 '{"a": "test", "b": null, "args": [], "kwargs": {}}',
                 counter,
             )
         ]
 
         cur.execute("SELECT timestamp FROM cache_entries", ())
         (timestamp,) = cur.fetchone() or []
-        assert before < datetime.datetime.fromisoformat(timestamp) < after
+        assert before < datetime.datetime.fromisoformat(timestamp + "+00:00") < after
 
 
 @pytest.mark.parametrize("raise_all_encoding_errors", [True, False])
 def test_encode_errors(tmpdir: pathlib.Path, raise_all_encoding_errors: bool) -> None:
     config.set(raise_all_encoding_errors=raise_all_encoding_errors)
 
     cfunc = cache.cacheable(func)
@@ -119,30 +119,34 @@
 
 
 def test_expiration_and_return_cache_entry() -> None:
     config.set(return_cache_entry=True)
     first: database.CacheEntry = cached_now()  # type: ignore[assignment]
     assert first.id == 1
     assert first.key == "c3d9e414d0d32337c3672cb29b1b3cc9"
-    assert first.expiration == datetime.datetime(9999, 12, 31, 23, 59, 59, 999999)
+    assert first.expiration == datetime.datetime(9999, 12, 31)
 
-    expiration = datetime.datetime.utcnow() + datetime.timedelta(seconds=0.1)
+    dt = datetime.timedelta(seconds=0.1)
+    expiration = datetime.datetime.now(tz=datetime.timezone.utc) + dt
     with config.set(expiration=expiration):
         second: database.CacheEntry = cached_now()  # type: ignore[assignment]
         assert second.result != first.result
         assert second.id == 2
         assert second.key == "c3d9e414d0d32337c3672cb29b1b3cc9"
-        assert second.expiration == expiration
+        assert (
+            second.expiration is not None
+            and second.expiration.isoformat() + "+00:00" == expiration.isoformat()
+        )
 
     time.sleep(0.1)
     third: database.CacheEntry = cached_now()  # type: ignore[assignment]
     assert third.result == first.result
     assert third.id == 1
     assert third.key == "c3d9e414d0d32337c3672cb29b1b3cc9"
-    assert third.expiration == datetime.datetime(9999, 12, 31, 23, 59, 59, 999999)
+    assert third.expiration == datetime.datetime(9999, 12, 31)
 
 
 def test_tag(tmpdir: pathlib.Path) -> None:
     con = config.get().engine.raw_connection()
     cur = con.cursor()
 
     cached_now()
```

### Comparing `cacholote-0.3.1/tests/test_40_xarray_encoder.py` & `cacholote-0.3.2/tests/test_40_xarray_encoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pathlib
 
 import fsspec
 import pytest
+import structlog
 
 from cacholote import cache, config, decode, encode, extra_encoders, utils
 
 try:
     import xarray as xr
 except ImportError:
     pytest.importorskip("xarray")
@@ -41,15 +42,15 @@
     expected = {
         "type": "python_call",
         "callable": "cacholote.extra_encoders:decode_xr_dataset",
         "args": (
             {
                 "type": "application/netcdf",
                 "href": href,
-                "file:checksum": fsspec.filesystem("file").checksum(local_path),
+                "file:checksum": f"{fsspec.filesystem('file').checksum(local_path):x}",
                 "file:size": 669,
                 "file:local_path": local_path,
             },
             {},
         ),
         "kwargs": {"chunks": {}},
     }
@@ -149,7 +150,36 @@
 
     # Warn if file is deleted
     fs.rm(cached_path, recursive=True)
     with pytest.warns(UserWarning, match="No such file or directory"):
         actual = cfunc()
     xr.testing.assert_identical(actual, expected)
     assert fs.exists(cached_path)
+
+
+def test_xr_logging(capsys: pytest.CaptureFixture[str]) -> None:
+    config.set(logger=structlog.get_logger())
+
+    # Cache dataset
+    cfunc = cache.cacheable(get_grib_ds)
+    cached_ds = cfunc()
+    captured = iter(capsys.readouterr().out.splitlines())
+
+    line = next(captured)
+    assert "start download" in line
+    assert "urlpath=" in line
+
+    line = next(captured)
+    assert "end download" in line
+    assert "urlpath=" in line
+    assert "download_time=" in line
+
+    line = next(captured)
+    assert "start upload" in line
+    assert f"urlpath=file://{cached_ds.encoding['source']}" in line
+    assert "size=22597" in line
+
+    line = next(captured)
+    assert "end upload" in line
+    assert f"urlpath=file://{cached_ds.encoding['source']}" in line
+    assert "upload_time=" in line
+    assert "size=22597" in line
```

### Comparing `cacholote-0.3.1/tests/test_50_io_encoder.py` & `cacholote-0.3.2/tests/test_50_io_encoder.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pathlib
 import threading
 from typing import Any, Dict, Tuple, Union
 
 import fsspec
 import pytest
 import pytest_httpserver
+import structlog
 
 from cacholote import cache, config, decode, encode, extra_encoders, utils
 
 
 @cache.cacheable
 def cached_open(*args: Any, **kwargs: Any) -> fsspec.spec.AbstractBufferedFile:
     with fsspec.open(*args, **kwargs) as f:
@@ -32,23 +33,22 @@
     fsspec.filesystem("file").pipe_file(tmpfile, b"test")
     tmp_hash = f"{fsspec.filesystem('file').checksum(tmpfile):x}"
 
     # Check dict and cached file
     actual = extra_encoders.dictify_io_object(open(tmpfile, "rb"))
     href = f"{readonly_dir}/{tmp_hash}.txt"
     local_path = f"{tmpdir}/cache_files/{tmp_hash}.txt"
-    checksum = fsspec.filesystem("file").checksum(local_path)
     expected = {
         "type": "python_call",
         "callable": "cacholote.extra_encoders:decode_io_object",
         "args": (
             {
                 "type": "text/plain",
                 "href": href,
-                "file:checksum": checksum,
+                "file:checksum": f"{fsspec.filesystem('file').checksum(local_path):x}",
                 "file:size": 4,
                 "file:local_path": local_path,
             },
             {},
         ),
         "kwargs": {"mode": "rb"},
     }
@@ -63,25 +63,24 @@
 @pytest.mark.parametrize("obj", [io.BytesIO(b"test"), io.StringIO("test")])
 def test_dictify_bytes_io_object(
     tmpdir: pathlib.Path, obj: Union[io.BytesIO, io.StringIO]
 ) -> None:
     actual = extra_encoders.dictify_io_object(obj)["args"]
     obj_hash = hashlib.md5(f"{hash(obj)}".encode()).hexdigest()
     local_path = f"{tmpdir}/cache_files/{obj_hash}"
-    checksum = fsspec.filesystem("file").checksum(local_path)
     type = (
         "text/plain"
         if importlib.util.find_spec("magic")
         else "application/octet-stream"
     )
     expected: Tuple[Dict[str, Any], ...] = (
         {
             "type": type,
             "href": local_path,
-            "file:checksum": checksum,
+            "file:checksum": f"{fsspec.filesystem('file').checksum(local_path):x}",
             "file:size": 4,
             "file:local_path": local_path,
         },
         {},
     )
     assert actual == expected
     assert open(local_path).read() == "test"
@@ -144,16 +143,14 @@
     with pytest.warns(UserWarning, match="No such file or directory"):
         result = cached_open(url)
     assert result.read() == b"test"
     assert fs.exists(f"{dirname}/{cached_basename}")
 
 
 def test_io_locker_warning(tmpdir: pathlib.Path) -> None:
-    cached_open = cache.cacheable(open)
-
     # Create tmpfile
     tmpfile = tmpdir / "test.txt"
     fsspec.filesystem("file").touch(tmpfile)
 
     # Acquire lock
     fs, dirname = utils.get_cache_files_fs_dirname()
     file_hash = f"{fsspec.filesystem('file').checksum(tmpfile):x}"
@@ -178,7 +175,40 @@
 @pytest.mark.parametrize("set_cache", ["cads"], indirect=True)
 def test_content_type(tmpdir: pathlib.Path, set_cache: str) -> None:
     tmpfile = str(tmpdir / "test.grib")
     fsspec.filesystem("file").touch(tmpfile)
     fs, _ = utils.get_cache_files_fs_dirname()
     cached_grib = cached_open(tmpfile)
     assert fs.info(cached_grib)["ContentType"] == "application/x-grib"
+
+
+@pytest.mark.parametrize("set_cache", ["cads"], indirect=True)
+def test_io_logging(capsys: pytest.CaptureFixture[str], tmpdir: pathlib.Path) -> None:
+    config.set(logger=structlog.get_logger(), io_delete_original=True)
+
+    # Cache file
+    tmpfile = tmpdir / "test.txt"
+    fsspec.filesystem("file").touch(tmpfile)
+    cached_file = cached_open(tmpfile)
+    captured = iter(capsys.readouterr().out.splitlines())
+
+    line = next(captured)
+    assert "start upload" in line
+    assert f"urlpath=s3://{cached_file.path}" in line
+    assert "size=0" in line
+
+    line = next(captured)
+    assert "end upload" in line
+    assert f"urlpath=s3://{cached_file.path}" in line
+    assert "upload_time=" in line
+    assert "size=0" in line
+
+    line = next(captured)
+    assert "start remove" in line
+    assert f"urlpath=file://{tmpfile}" in line
+    assert "size=0" in line
+
+    line = next(captured)
+    assert "end remove" in line
+    assert f"urlpath=file://{tmpfile}" in line
+    assert "remove_time=" in line
+    assert "size=0" in line
```

### Comparing `cacholote-0.3.1/tests/test_60_clean.py` & `cacholote-0.3.2/tests/test_60_clean.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import contextlib
 import pathlib
 from typing import Any, Literal, Optional, Sequence
 
 import fsspec
 import pytest
+import structlog
 
 from cacholote import cache, clean, config, utils
 
 does_not_raise = contextlib.nullcontext
 
 
 @cache.cacheable
@@ -73,15 +74,15 @@
         assert fs.ls(dirname) == [f"{dirname}/unknown.txt"]
 
 
 @pytest.mark.parametrize(
     "recursive,raises,final_size",
     [
         (True, does_not_raise(), 0),
-        (False, pytest.raises((PermissionError, IsADirectoryError)), 1),
+        (False, pytest.raises((PermissionError, IsADirectoryError, ValueError)), 1),
     ],
 )
 def test_delete_unknown_dirs(
     recursive: bool, raises: contextlib.nullcontext, final_size: int  # type: ignore[type-arg]
 ) -> None:
     fs, dirname = utils.get_cache_files_fs_dirname()
     fs.mkdir(f"{dirname}/unknown")
@@ -190,7 +191,50 @@
     # Delete cache entry
     clean.delete(open_url, tmpfile)
     assert fs.ls(dirname) == []
 
     # Cache again
     assert open_url(tmpfile).read() == b"new"
     assert len(fs.ls(dirname)) == 1
+
+
+def test_cleaner_logging(
+    capsys: pytest.CaptureFixture[str], tmpdir: pathlib.Path
+) -> None:
+    # Cache file and create unknown
+    tmpfile = tmpdir / "test.txt"
+    fsspec.filesystem("file").pipe_file(tmpfile, b"1")
+    cached_file = open_url(tmpfile)
+    fs, dirname = utils.get_cache_files_fs_dirname()
+    fs.pipe_file(f"{dirname}/unknown.txt", b"1")
+
+    # Clean
+    config.set(logger=structlog.get_logger())
+    clean.clean_cache_files(0, delete_unknown_files=True)
+    captured = iter(capsys.readouterr().out.splitlines())
+
+    line = next(captured)
+    assert "get disk usage of cache files" in line
+
+    line = next(captured)
+    assert "get unknown files" in line
+
+    line = next(captured)
+    assert "delete unknown" in line
+    assert "recursive=False" in line
+    assert f"urlpath=file://{dirname}/unknown.txt" in line
+
+    line = next(captured)
+    assert "check cache files total size" in line
+    assert "size=1" in line
+
+    line = next(captured)
+    assert "delete cache entry" in line
+    assert "cache_entry=" in line
+
+    line = next(captured)
+    assert "delete cache file" in line
+    assert f"urlpath=file://{cached_file.path}" in line
+
+    line = next(captured)
+    assert "check cache files total size" in line
+    assert "size=0" in line
```

