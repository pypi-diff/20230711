# Comparing `tmp/sumo-wrapper-python-0.3.4.tar.gz` & `tmp/sumo-wrapper-python-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumo-wrapper-python-0.3.4.tar", last modified: Mon Jun 26 07:33:33 2023, max compression
+gzip compressed data, was "sumo-wrapper-python-0.3.5.tar", last modified: Tue Jul 11 11:28:52 2023, max compression
```

## Comparing `sumo-wrapper-python-0.3.4.tar` & `sumo-wrapper-python-0.3.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:33:33.890977 sumo-wrapper-python-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:33:33.882977 sumo-wrapper-python-0.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:33:33.886977 sumo-wrapper-python-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/.github/workflows/publish_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-26 07:33:33.890977 sumo-wrapper-python-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:33:33.886977 sumo-wrapper-python-0.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:33:33.886977 sumo-wrapper-python-0.3.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/requirements/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/requirements/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 07:33:33.890977 sumo-wrapper-python-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:33:33.882977 sumo-wrapper-python-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:33:33.886977 sumo-wrapper-python-0.3.4/src/sumo/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/src/sumo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:33:33.886977 sumo-wrapper-python-0.3.4/src/sumo/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/src/sumo/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/src/sumo/wrapper/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/src/sumo/wrapper/_blob_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/src/sumo/wrapper/_call_azure_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/src/sumo/wrapper/_call_sumo_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/src/sumo/wrapper/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/src/sumo/wrapper/_new_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/src/sumo/wrapper/_request_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/src/sumo/wrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/src/sumo/wrapper/login.py
--rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/src/sumo/wrapper/sumo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 07:33:33.000000 sumo-wrapper-python-0.3.4/src/sumo/wrapper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:33:33.886977 sumo-wrapper-python-0.3.4/src/sumo_wrapper_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-26 07:33:33.000000 sumo-wrapper-python-0.3.4/src/sumo_wrapper_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-26 07:33:33.000000 sumo-wrapper-python-0.3.4/src/sumo_wrapper_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:33:33.000000 sumo-wrapper-python-0.3.4/src/sumo_wrapper_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 07:33:33.000000 sumo-wrapper-python-0.3.4/src/sumo_wrapper_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:33:33.000000 sumo-wrapper-python-0.3.4/src/sumo_wrapper_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-26 07:33:33.000000 sumo-wrapper-python-0.3.4/src/sumo_wrapper_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 07:33:33.000000 sumo-wrapper-python-0.3.4/src/sumo_wrapper_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:33:33.886977 sumo-wrapper-python-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/tests/test_call_sumo_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/tests/test_sumo_thin_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:33:33.886977 sumo-wrapper-python-0.3.4/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/tests/testdata/case.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-06-26 07:33:21.000000 sumo-wrapper-python-0.3.4/tests/testdata/surface.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:28:52.174096 sumo-wrapper-python-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:28:52.166096 sumo-wrapper-python-0.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:28:52.170096 sumo-wrapper-python-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/.github/workflows/publish_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-11 11:28:52.174096 sumo-wrapper-python-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:28:52.170096 sumo-wrapper-python-0.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:28:52.170096 sumo-wrapper-python-0.3.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/requirements/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/requirements/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 11:28:52.174096 sumo-wrapper-python-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:28:52.166096 sumo-wrapper-python-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:28:52.170096 sumo-wrapper-python-0.3.5/src/sumo/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/src/sumo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:28:52.170096 sumo-wrapper-python-0.3.5/src/sumo/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/src/sumo/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/src/sumo/wrapper/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/src/sumo/wrapper/_blob_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/src/sumo/wrapper/_call_azure_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14139 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/src/sumo/wrapper/_call_sumo_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/src/sumo/wrapper/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/src/sumo/wrapper/_new_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/src/sumo/wrapper/_request_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/src/sumo/wrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/src/sumo/wrapper/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/src/sumo/wrapper/sumo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 11:28:52.000000 sumo-wrapper-python-0.3.5/src/sumo/wrapper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:28:52.174096 sumo-wrapper-python-0.3.5/src/sumo_wrapper_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-11 11:28:52.000000 sumo-wrapper-python-0.3.5/src/sumo_wrapper_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-11 11:28:52.000000 sumo-wrapper-python-0.3.5/src/sumo_wrapper_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:28:52.000000 sumo-wrapper-python-0.3.5/src/sumo_wrapper_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 11:28:52.000000 sumo-wrapper-python-0.3.5/src/sumo_wrapper_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:28:51.000000 sumo-wrapper-python-0.3.5/src/sumo_wrapper_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-11 11:28:52.000000 sumo-wrapper-python-0.3.5/src/sumo_wrapper_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 11:28:52.000000 sumo-wrapper-python-0.3.5/src/sumo_wrapper_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:28:52.174096 sumo-wrapper-python-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/tests/test_call_sumo_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/tests/test_sumo_thin_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:28:52.174096 sumo-wrapper-python-0.3.5/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/tests/testdata/case.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-11 11:28:42.000000 sumo-wrapper-python-0.3.5/tests/testdata/surface.yml
```

### Comparing `sumo-wrapper-python-0.3.4/.github/workflows/linting.yml` & `sumo-wrapper-python-0.3.5/.github/workflows/linting.yml`

 * *Files 12% similar despite different names*

```diff
@@ -14,27 +14,27 @@
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v3
         with:
           python-version: ${{ matrix.python-version }}
       - uses: psf/black@stable
         with:
-          options: "--check --verbose --line-length 80"
+          options: "--check --verbose --line-length 79"
           src: "./src/sumo/wrapper"
   flake8:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8"]
     steps:
-    - uses: actions/checkout@v3
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
-      with:
-        python-version: ${{ matrix.python-version }}
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install flake8
-    - name: Analysing the code with flake8
-      run: |
-        flake8 src/sumo/wrapper --config .flake8
+      - uses: actions/checkout@v3
+      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v3
+        with:
+          python-version: ${{ matrix.python-version }}
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install flake8
+      - name: Analysing the code with flake8
+        run: |
+          flake8 src/sumo/wrapper --config .flake8
```

### Comparing `sumo-wrapper-python-0.3.4/.github/workflows/publish_release.yml` & `sumo-wrapper-python-0.3.5/.github/workflows/publish_release.yml`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/.github/workflows/pytest.yml` & `sumo-wrapper-python-0.3.5/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/LICENSE` & `sumo-wrapper-python-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/PKG-INFO` & `sumo-wrapper-python-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumo-wrapper-python
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python wrapper for the Sumo API
 Home-page: https://github.com/equinor/sumo-wrapper-python
 Author: Equinor ASA
 License: Apache 2.0
 Keywords: sumo,python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sumo-wrapper-python-0.3.4/README.md` & `sumo-wrapper-python-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/docs/Makefile` & `sumo-wrapper-python-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/docs/conf.py` & `sumo-wrapper-python-0.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/docs/index.rst` & `sumo-wrapper-python-0.3.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/docs/make.bat` & `sumo-wrapper-python-0.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/setup.py` & `sumo-wrapper-python-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/src/sumo/wrapper/_auth.py` & `sumo-wrapper-python-0.3.5/src/sumo/wrapper/_auth.py`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/src/sumo/wrapper/_blob_client.py` & `sumo-wrapper-python-0.3.5/src/sumo/wrapper/_blob_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import requests
+import httpx
+
 from ._request_error import raise_request_error_exception
 
 
 class BlobClient:
     """Upload blobs to blob store using pre-authorized URLs"""
 
     def upload_blob(self, blob: bytes, url: str):
@@ -16,15 +17,42 @@
         headers = {
             "Content-Type": "application/octet-stream",
             "Content-Length": str(len(blob)),
             "x-ms-blob-type": "BlockBlob",
         }
 
         try:
-            response = requests.put(url, data=blob, headers=headers)
-        except requests.exceptions.ProxyError as err:
+            response = httpx.put(url, data=blob, headers=headers)
+        except httpx.ProxyError as err:
+            raise_request_error_exception(503, err)
+
+        if response.is_error:
+            raise_request_error_exception(response.status_code, response.text)
+
+        return response
+
+    async def upload_blob_async(self, blob: bytes, url: str):
+        """Upload a blob async.
+
+        Parameters:
+            blob: byte string to upload
+            url: pre-authorized URL to blob store
+        """
+
+        headers = {
+            "Content-Type": "application/octet-stream",
+            "Content-Length": str(len(blob)),
+            "x-ms-blob-type": "BlockBlob",
+        }
+
+        try:
+            async with httpx.AsyncClient() as client:
+                response = await client.put(
+                    url=url, data=blob, headers=headers
+                )
+        except httpx.ProxyError as err:
             raise_request_error_exception(503, err)
 
-        if not response.ok:
+        if response.is_error:
             raise_request_error_exception(response.status_code, response.text)
 
         return response
```

### Comparing `sumo-wrapper-python-0.3.4/src/sumo/wrapper/_call_azure_api.py` & `sumo-wrapper-python-0.3.5/src/sumo/wrapper/_call_azure_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import requests
+import httpx
 import logging
 
 from ._auth import Auth
 from ._request_error import AuthenticationError, TransientError, PermanentError
 
 logger = logging.getLogger("sumo.wrapper")
 
@@ -150,17 +150,17 @@
 
         logger.debug("get_json() is starting")
 
         bearer = self._process_token(bearer)
 
         headers = {"Content-Type": "application/json", "Authorization": bearer}
 
-        response = requests.get(url, headers=headers)
+        response = httpx.get(url, headers=headers)
 
-        if not response.ok:
+        if response.is_error:
             _raise_request_error_exception(response.status_code, response.text)
 
         return response.json()
 
     def get_image(self, url, bearer=None):
         """
         Send an request to the url for the image.
@@ -178,17 +178,17 @@
 
         logger.debug("get_image() is starting")
 
         bearer = self._process_token(bearer)
 
         headers = {"Content-Type": "html/text", "Authorization": bearer}
 
-        response = requests.get(url, headers=headers, stream=True)
+        response = httpx.get(url, headers=headers)
 
-        if not response.ok:
+        if response.is_error:
             _raise_request_error_exception(response.status_code, response.text)
 
         return None
 
     def get_content(self, url, bearer=None):
         """
         Send an request to the url.
@@ -206,17 +206,17 @@
 
         logger.debug("get_content() is starting")
 
         bearer = self._process_token(bearer)
 
         headers = {"Content-Type": "application/json", "Authorization": bearer}
 
-        response = requests.get(url, headers=headers)
+        response = httpx.get(url, headers=headers)
 
-        if not response.ok:
+        if response.is_error:
             _raise_request_error_exception(response.status_code, response.text)
 
         return response.content
 
     def post(self, url, blob=None, json=None, bearer=None):
         """
         Post binary or json to the url and return the response as json.
@@ -245,19 +245,19 @@
             if json is not None
             else "application/octet-stream",
             "Authorization": bearer,
             "Content-Length": str(len(json) if json else len(blob)),
         }
 
         try:
-            response = requests.post(url, data=blob, json=json, headers=headers)
-        except requests.exceptions.ProxyError as err:
+            response = httpx.post(url, data=blob, json=json, headers=headers)
+        except httpx.ProxyError as err:
             _raise_request_error_exception(503, err)
 
-        if not response.ok:
+        if response.is_error:
             _raise_request_error_exception(response.status_code, response.text)
 
         return response
 
     def put(self, url, blob=None, json=None, bearer=None):
         """
         Put binary to the url and return the response as json.
@@ -289,19 +289,19 @@
             "x-ms-blob-type": "BlockBlob",
         }
 
         if url.find("sig=") < 0:
             headers["Authorization"] = bearer
 
         try:
-            response = requests.put(url, data=blob, json=json, headers=headers)
-        except requests.exceptions.ProxyError as err:
+            response = httpx.put(url, data=blob, json=json, headers=headers)
+        except httpx.ProxyError as err:
             _raise_request_error_exception(503, err)
 
-        if not response.ok:
+        if response.is_error:
             _raise_request_error_exception(response.status_code, response.text)
 
         return response
 
     def delete_object(self, url, bearer=None):
         """
         Send delete to the url and return the response as json.
@@ -317,13 +317,13 @@
         bearer = self._process_token(bearer)
 
         headers = {
             "Content-Type": "application/json",
             "Authorization": bearer,
         }
 
-        response = requests.delete(url, headers=headers)
+        response = httpx.delete(url, headers=headers)
 
-        if not response.ok:
+        if response.is_error:
             _raise_request_error_exception(response.status_code, response.text)
 
         return response.json()
```

### Comparing `sumo-wrapper-python-0.3.4/src/sumo/wrapper/_call_sumo_api.py` & `sumo-wrapper-python-0.3.5/src/sumo/wrapper/_call_sumo_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 
         if env == "localhost":
             self.base_url = "http://localhost:8084/api/v1"
         else:
             self.base_url = f"https://main-sumo-{env}.radix.equinor.com/api/v1"
 
         resource_id = (
-            resource_id if resource_id else APP_REGISTRATION[env]["RESOURCE_ID"]
+            resource_id
+            if resource_id
+            else APP_REGISTRATION[env]["RESOURCE_ID"]
         )
         client_id = (
             client_id if client_id else APP_REGISTRATION[env]["CLIENT_ID"]
         )
 
         self.callAzureApi = CallAzureApi(
             resource_id, client_id, outside_token, writeback=writeback
@@ -220,15 +222,17 @@
             parent_id: string, the id of the json object that this json document will be attached to.
             json: json, JSON document to save.
             bearer: string, Azure OAuth2 bear token Default: will create one.
 
         Return
             string: The object id of the newly created object, or error message.
         """
-        return self._post_objects(object_id=parent_id, json=json, bearer=bearer)
+        return self._post_objects(
+            object_id=parent_id, json=json, bearer=bearer
+        )
 
     def update_child_level_json(
         self, json, object_id=None, url=None, bearer=None
     ):
         """
         Updates a child-level json object in SUMO.
```

### Comparing `sumo-wrapper-python-0.3.4/src/sumo/wrapper/_logging.py` & `sumo-wrapper-python-0.3.5/src/sumo/wrapper/_logging.py`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/src/sumo/wrapper/_new_auth.py` & `sumo-wrapper-python-0.3.5/src/sumo/wrapper/_new_auth.py`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/src/sumo/wrapper/_request_error.py` & `sumo-wrapper-python-0.3.5/src/sumo/wrapper/_request_error.py`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/src/sumo/wrapper/config.py` & `sumo-wrapper-python-0.3.5/src/sumo/wrapper/config.py`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/src/sumo/wrapper/login.py` & `sumo-wrapper-python-0.3.5/src/sumo/wrapper/login.py`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/src/sumo/wrapper/sumo_client.py` & `sumo-wrapper-python-0.3.5/src/sumo/wrapper/sumo_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import requests
-import jwt
-import time
 import logging
+import time
+
+import httpx
+import jwt
 
-from .config import APP_REGISTRATION, TENANT_ID
-from ._new_auth import NewAuth
-from ._request_error import raise_request_error_exception
 from ._blob_client import BlobClient
 from ._logging import LogHandlerSumo
+from ._new_auth import NewAuth
+from ._request_error import raise_request_error_exception
+from .config import APP_REGISTRATION, TENANT_ID
 
 logger = logging.getLogger("sumo.wrapper")
 
 
 class SumoClient:
     """Authenticate and perform requests to the Sumo API."""
 
@@ -93,14 +94,18 @@
             Uploading blob::
 
                 blob = ...
                 blob_url = ...
                 sumo = SumoClient("dev")
 
                 sumo.blob_client.upload_blob(blob, blob_url)
+
+            Uploading blob async::
+
+                await sumo.blob_client.upload_blob_async(blob, blob_url)
         """
 
         return self._blob_client
 
     def __decode_token(self, token: str) -> dict:
         """
         Decodes a Json Web Token, returns the payload as a dictionary.
@@ -186,35 +191,36 @@
         token = self._retrieve_token()
 
         headers = {
             "Content-Type": "application/json",
             "authorization": f"Bearer {token}",
         }
 
-        response = requests.get(
+        response = httpx.get(
             f"{self.base_url}{path}",
             params=self._process_params(params),
             headers=headers,
+            follow_redirects=True,
         )
 
-        if not response.ok:
+        if response.is_error:
             raise_request_error_exception(response.status_code, response.text)
 
         if "/blob" in path:
             return response.content
 
         return response.json()
 
     def post(
         self,
         path: str,
         blob: bytes = None,
         json: dict = None,
         params: dict = None,
-    ) -> requests.Response:
+    ) -> httpx.Response:
         """Performs a POST-request to the Sumo API.
 
         Takes either blob or json as a payload,
         will raise an error if both are provided.
 
         Args:
             path: Path to a Sumo endpoint
@@ -258,41 +264,41 @@
 
         content_type = (
             "application/octet-stream" if blob else "application/json"
         )
         content_length = 0
 
         if blob or json:
-            content_length = len(json) if json else len(blob)
+            content_length = len(str(json)) if json else len(blob)
 
         headers = {
             "Content-Type": content_type,
             "authorization": f"Bearer {token}",
             "Content-Length": str(content_length),
         }
 
         try:
-            response = requests.post(
+            response = httpx.post(
                 f"{self.base_url}{path}",
                 data=blob,
                 json=json,
                 headers=headers,
                 params=params,
             )
-        except requests.exceptions.ProxyError as err:
+        except httpx.ProxyError as err:
             raise_request_error_exception(503, err)
 
-        if not response.ok:
+        if response.is_error:
             raise_request_error_exception(response.status_code, response.text)
 
         return response
 
     def put(
         self, path: str, blob: bytes = None, json: dict = None
-    ) -> requests.Response:
+    ) -> httpx.Response:
         """Performs a PUT-request to the Sumo API.
 
         Takes either blob or json as a payload,
         will raise an error if both are provided.
 
         Args:
             path: Path to a Sumo endpoint
@@ -313,25 +319,25 @@
             if json is not None
             else "application/octet-stream"
         )
 
         headers = {
             "Content-Type": content_type,
             "authorization": f"Bearer {token}",
-            "Content-Length": str(len(json) if json else len(blob)),
+            "Content-Length": str(len(str(json)) if json else len(blob)),
         }
 
         try:
-            response = requests.put(
+            response = httpx.put(
                 f"{self.base_url}{path}", data=blob, json=json, headers=headers
             )
-        except requests.exceptions.ProxyError as err:
+        except httpx.ProxyError as err:
             raise_request_error_exception(503, err)
 
-        if not response.ok:
+        if response.is_error:
             raise_request_error_exception(response.status_code, response.text)
 
         return response
 
     def delete(self, path: str) -> dict:
         """Performs a DELETE-request to the Sumo API.
 
@@ -353,17 +359,17 @@
         token = self._retrieve_token()
 
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {token}",
         }
 
-        response = requests.delete(f"{self.base_url}{path}", headers=headers)
+        response = httpx.delete(f"{self.base_url}{path}", headers=headers)
 
-        if not response.ok:
+        if response.is_error:
             raise_request_error_exception(response.status_code, response.text)
 
         return response.json()
 
     def getLogger(self, name):
         """Gets a logger object that sends log objects into the message_log
         index for the Sumo instance.
@@ -377,7 +383,225 @@
         See Python documentation for logging.Logger for details.
         """
 
         logger = logging.getLogger(name)
         handler = LogHandlerSumo(self)
         logger.addHandler(handler)
         return logger
+
+    async def get_async(self, path: str, **params):
+        """Performs an async GET-request to the Sumo API.
+
+        Args:
+            path: Path to a Sumo endpoint
+            params: Keyword arguments treated as query parameters
+
+        Returns:
+            Sumo JSON response as a dictionary
+
+        Examples:
+            Retrieving user data from Sumo::
+
+                sumo = SumoClient("dev")
+
+                userdata = await sumo.getAsync(path="/userdata")
+
+            Searching for cases::
+
+                sumo = SuomClient("dev")
+
+                cases = await sumo.getAsync(
+                    path="/search",
+                    query="class:case",
+                    size=3
+                )
+        """
+        token = self._retrieve_token()
+
+        headers = {
+            "Content-Type": "application/json",
+            "authorization": f"Bearer {token}",
+        }
+
+        async with httpx.AsyncClient() as client:
+            response = await client.get(
+                f"{self.base_url}{path}",
+                params=self._process_params(params),
+                headers=headers,
+            )
+
+        if response.is_error:
+            raise_request_error_exception(response.status_code, response.text)
+
+        if "/blob" in path:
+            return response.content
+
+        return response.json()
+
+    async def post_async(
+        self,
+        path: str,
+        blob: bytes = None,
+        json: dict = None,
+        params: dict = None,
+    ) -> httpx.Response:
+        """Performs an async POST-request to the Sumo API.
+
+        Takes either blob or json as a payload,
+        will raise an error if both are provided.
+
+        Args:
+            path: Path to a Sumo endpoint
+            blob: Blob payload
+            json: Json payload
+
+        Returns:
+            Sumo response object
+
+        Raises:
+            ValueError: If both blob and json parameters have been provided
+
+        Examples:
+            Uploading case metadata::
+
+                case_metadata = {...}
+                sumo = SumoClient("dev")
+
+                new_case = await sumo.postAsync(
+                    path="/objects",
+                    json=case_metadata
+                )
+
+                new_case_id = new_case.json()["_id"]
+
+            Uploading object metadata::
+
+                object_metadata = {...}
+                sumo = SumoClient("dev")
+
+                new_objet = await sumo.postAsync(
+                    path=f"/objects('{new_case_id}')",
+                    json=object_metadata
+                )
+        """
+
+        token = self._retrieve_token()
+
+        if blob and json:
+            raise ValueError("Both blob and json given to post.")
+
+        content_type = (
+            "application/octet-stream" if blob else "application/json"
+        )
+        content_length = 0
+
+        if blob or json:
+            content_length = len(str(json)) if json else len(blob)
+
+        headers = {
+            "Content-Type": content_type,
+            "authorization": f"Bearer {token}",
+            "Content-Length": str(content_length),
+        }
+
+        try:
+            async with httpx.AsyncClient() as client:
+                response = await client.post(
+                    url=f"{self.base_url}{path}",
+                    data=blob,
+                    json=json,
+                    headers=headers,
+                    params=params,
+                )
+        except httpx.ProxyError as err:
+            raise_request_error_exception(503, err)
+
+        if response.is_error:
+            raise_request_error_exception(response.status_code, response.text)
+
+        return response
+
+    async def put_async(
+        self, path: str, blob: bytes = None, json: dict = None
+    ) -> httpx.Response:
+        """Performs an async PUT-request to the Sumo API.
+
+        Takes either blob or json as a payload,
+        will raise an error if both are provided.
+
+        Args:
+            path: Path to a Sumo endpoint
+            blob: Blob payload
+            json: Json payload
+
+        Returns:
+            Sumo response object
+        """
+
+        token = self._retrieve_token()
+
+        if blob and json:
+            raise ValueError("Both blob and json given to post")
+
+        content_type = (
+            "application/json"
+            if json is not None
+            else "application/octet-stream"
+        )
+
+        headers = {
+            "Content-Type": content_type,
+            "authorization": f"Bearer {token}",
+            "Content-Length": str(len(str(json)) if json else len(blob)),
+        }
+
+        try:
+            async with httpx.AsyncClient() as client:
+                response = await client.put(
+                    url=f"{self.base_url}{path}",
+                    data=blob,
+                    json=json,
+                    headers=headers,
+                )
+        except httpx.ProxyError as err:
+            raise_request_error_exception(503, err)
+
+        if response.is_error:
+            raise_request_error_exception(response.status_code, response.text)
+
+        return response
+
+    async def delete_async(self, path: str) -> dict:
+        """Performs an async DELETE-request to the Sumo API.
+
+        Args:
+            path: Path to a Sumo endpoint
+
+        Returns:
+            Sumo JSON resposne as a dictionary
+
+        Examples:
+            Deleting object::
+
+                object_id = ...
+                sumo = SumoClient("dev")
+
+                await sumo.deleteAsync(path=f"/objects('{object_id}')")
+        """
+
+        token = self._retrieve_token()
+
+        headers = {
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {token}",
+        }
+
+        async with httpx.AsyncClient() as client:
+            response = await client.delete(
+                url=f"{self.base_url}{path}",
+                headers=headers,
+            )
+
+        if response.is_error:
+            raise_request_error_exception(response.status_code, response.text)
+
+        return response.json()
```

### Comparing `sumo-wrapper-python-0.3.4/src/sumo_wrapper_python.egg-info/PKG-INFO` & `sumo-wrapper-python-0.3.5/src/sumo_wrapper_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumo-wrapper-python
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python wrapper for the Sumo API
 Home-page: https://github.com/equinor/sumo-wrapper-python
 Author: Equinor ASA
 License: Apache 2.0
 Keywords: sumo,python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sumo-wrapper-python-0.3.4/src/sumo_wrapper_python.egg-info/SOURCES.txt` & `sumo-wrapper-python-0.3.5/src/sumo_wrapper_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/tests/test_call_sumo_api.py` & `sumo-wrapper-python-0.3.5/tests/test_call_sumo_api.py`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/tests/test_sumo_thin_client.py` & `sumo-wrapper-python-0.3.5/tests/test_sumo_thin_client.py`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/tests/testdata/case.yml` & `sumo-wrapper-python-0.3.5/tests/testdata/case.yml`

 * *Files identical despite different names*

### Comparing `sumo-wrapper-python-0.3.4/tests/testdata/surface.yml` & `sumo-wrapper-python-0.3.5/tests/testdata/surface.yml`

 * *Files identical despite different names*

