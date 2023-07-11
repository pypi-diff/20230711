# Comparing `tmp/matchmaps-0.3.1.tar.gz` & `tmp/matchmaps-0.3.1.2.tar.gz`

## Comparing `matchmaps-0.3.1.tar` & `matchmaps-0.3.1.2.tar`

### file list

```diff
@@ -1,28 +1,32 @@
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.github_changelog_generator
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 matchmaps-0.3.1/setup.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 matchmaps-0.3.1/tox.ini
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.github/workflows/cron.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 matchmaps-0.3.1/docs/Makefile
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 matchmaps-0.3.1/docs/about.md
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 matchmaps-0.3.1/docs/cli.md
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 matchmaps-0.3.1/docs/conf.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 matchmaps-0.3.1/docs/index.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 matchmaps-0.3.1/docs/make.bat
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 matchmaps-0.3.1/docs/_static/custom.css
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 matchmaps-0.3.1/src/matchmaps/__init__.py
--rw-r--r--   0        0        0    13918 2020-02-02 00:00:00.000000 matchmaps-0.3.1/src/matchmaps/_compute_mr_diff.py
--rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 matchmaps-0.3.1/src/matchmaps/_compute_ncs_diff.py
--rwxr-xr-x   0        0        0    12085 2020-02-02 00:00:00.000000 matchmaps-0.3.1/src/matchmaps/_compute_realspace_diff.py
--rw-r--r--   0        0        0    26064 2020-02-02 00:00:00.000000 matchmaps-0.3.1/src/matchmaps/_utils.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 matchmaps-0.3.1/tests/test_matchmaps.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 matchmaps-0.3.1/LICENSE
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 matchmaps-0.3.1/README.md
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 matchmaps-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 matchmaps-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/.github_changelog_generator
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/setup.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/tox.ini
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/.github/workflows/cron.yml
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/.github/workflows/test_docs.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/docs/Makefile
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/docs/about.md
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/docs/cli.md
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/docs/conf.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/docs/index.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/docs/make.bat
+-rw-r--r--   0        0        0     8971 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/docs/quickstart.md
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/docs/_static/custom.css
+-rw-r--r--   0        0        0   217883 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/docs/images/isdifferencemap.png
+-rw-r--r--   0        0        0   116988 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/docs/images/openmap.png
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/src/matchmaps/__init__.py
+-rw-r--r--   0        0        0    13918 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/src/matchmaps/_compute_mr_diff.py
+-rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/src/matchmaps/_compute_ncs_diff.py
+-rwxr-xr-x   0        0        0    12085 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/src/matchmaps/_compute_realspace_diff.py
+-rw-r--r--   0        0        0    26064 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/src/matchmaps/_utils.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/tests/test_matchmaps.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/LICENSE
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/README.md
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 matchmaps-0.3.1.2/PKG-INFO
```

### Comparing `matchmaps-0.3.1/.pre-commit-config.yaml` & `matchmaps-0.3.1.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   autofix_commit_msg: "style(pre-commit.ci): auto fixes [...]"
   autoupdate_commit_msg: "ci(pre-commit.ci): autoupdate"
 
 default_install_hook_types: [pre-commit, commit-msg]
 
 repos:
   - repo: https://github.com/compilerla/conventional-pre-commit
-    rev: v2.2.0
+    rev: v2.3.0
     hooks:
       - id: conventional-pre-commit
         stages: [commit-msg]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
@@ -27,15 +27,15 @@
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.2
+    rev: v0.13
     hooks:
       - id: validate-pyproject
 
 #   - repo: https://github.com/pre-commit/mirrors-mypy
 #     rev: v0.991
 #     hooks:
 #       - id: mypy
```

### Comparing `matchmaps-0.3.1/setup.py` & `matchmaps-0.3.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.1/tox.ini` & `matchmaps-0.3.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.1/.github/workflows/build_docs.yml` & `matchmaps-0.3.1.2/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.1/.github/workflows/ci.yml` & `matchmaps-0.3.1.2/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
   test:
     name: ${{ matrix.platform }} (${{ matrix.python-version }})
     runs-on: ${{ matrix.platform }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.9', '3.10', '3.11']
+        python-version: ['3.9', '3.10']
         platform: [ubuntu-latest]
 
     steps:
       - name: Cancel Previous Runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           access_token: ${{ github.token }}
```

### Comparing `matchmaps-0.3.1/.github/workflows/cron.yml` & `matchmaps-0.3.1.2/.github/workflows/cron.yml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
   test:
     name: ${{ matrix.platform }} (${{ matrix.python-version }})
     runs-on: ${{ matrix.platform }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.9', '3.10', '3.11']
+        python-version: ['3.9', '3.10']
         platform: [ubuntu-latest, macos-latest, windows-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
```

### Comparing `matchmaps-0.3.1/docs/Makefile` & `matchmaps-0.3.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.1/docs/conf.py` & `matchmaps-0.3.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.1/docs/make.bat` & `matchmaps-0.3.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.1/src/matchmaps/_compute_mr_diff.py` & `matchmaps-0.3.1.2/src/matchmaps/_compute_mr_diff.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.1/src/matchmaps/_compute_ncs_diff.py` & `matchmaps-0.3.1.2/src/matchmaps/_compute_ncs_diff.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.1/src/matchmaps/_compute_realspace_diff.py` & `matchmaps-0.3.1.2/src/matchmaps/_compute_realspace_diff.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.1/src/matchmaps/_utils.py` & `matchmaps-0.3.1.2/src/matchmaps/_utils.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.1/.gitignore` & `matchmaps-0.3.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.1/LICENSE` & `matchmaps-0.3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.1/README.md` & `matchmaps-0.3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.1/PKG-INFO` & `matchmaps-0.3.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: matchmaps
-Version: 0.3.1
+Version: 0.3.1.2
 Summary: Make unbiased difference maps even for non-isomorphous inputs
-Project-URL: homepage, https://dennisbrookner.github.io/matchmaps/
-Project-URL: repository, https://github.com/dennisbrookner/matchmaps
+Project-URL: homepage, https://rs-station.github.io/matchmaps/
+Project-URL: repository, https://github.com/rs-station/matchmaps
 Author-email: Dennis Brookner <debrookner@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

