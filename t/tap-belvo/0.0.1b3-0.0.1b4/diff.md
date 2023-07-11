# Comparing `tmp/tap_belvo-0.0.1b3.tar.gz` & `tmp/tap_belvo-0.0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_belvo-0.0.1b3.tar", max compression
+gzip compressed data, was "tap_belvo-0.0.1b4.tar", max compression
```

## Comparing `tap_belvo-0.0.1b3.tar` & `tap_belvo-0.0.1b4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1068 2023-05-24 20:31:02.676639 tap_belvo-0.0.1b3/LICENSE
--rw-r--r--   0        0        0     3135 2023-05-24 20:31:02.676639 tap_belvo-0.0.1b3/README.md
--rw-r--r--   0        0        0     2264 2023-05-24 20:31:22.381863 tap_belvo-0.0.1b3/pyproject.toml
--rw-r--r--   0        0        0       80 2023-05-24 20:31:02.680639 tap_belvo-0.0.1b3/tap_belvo/__init__.py
--rw-r--r--   0        0        0      110 2023-05-24 20:31:02.680639 tap_belvo-0.0.1b3/tap_belvo/__main__.py
--rw-r--r--   0        0        0     4417 2023-05-24 20:31:02.680639 tap_belvo-0.0.1b3/tap_belvo/client.py
--rw-r--r--   0        0        0  1025531 2023-05-24 20:31:02.680639 tap_belvo-0.0.1b3/tap_belvo/openapi/BelvoOpenFinanceApiSpec.json
--rw-r--r--   0        0        0      739 2023-05-24 20:31:02.680639 tap_belvo-0.0.1b3/tap_belvo/openapi/__init__.py
--rw-r--r--   0        0        0      936 2023-05-24 20:31:02.684639 tap_belvo-0.0.1b3/tap_belvo/streams/__init__.py
--rw-r--r--   0        0        0     2438 2023-05-24 20:31:02.684639 tap_belvo-0.0.1b3/tap_belvo/streams/banking.py
--rw-r--r--   0        0        0      758 2023-05-24 20:31:02.684639 tap_belvo-0.0.1b3/tap_belvo/streams/enrichment.py
--rw-r--r--   0        0        0     1591 2023-05-24 20:31:02.684639 tap_belvo-0.0.1b3/tap_belvo/streams/fiscal.py
--rw-r--r--   0        0        0      903 2023-05-24 20:31:02.684639 tap_belvo-0.0.1b3/tap_belvo/streams/links.py
--rw-r--r--   0        0        0     2006 2023-05-24 20:31:02.684639 tap_belvo-0.0.1b3/tap_belvo/tap.py
--rw-r--r--   0        0        0     4063 1970-01-01 00:00:00.000000 tap_belvo-0.0.1b3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-11 20:52:38.847147 tap_belvo-0.0.1b4/LICENSE
+-rw-r--r--   0        0        0     3135 2023-07-11 20:52:38.847147 tap_belvo-0.0.1b4/README.md
+-rw-r--r--   0        0        0     2304 2023-07-11 20:52:55.579237 tap_belvo-0.0.1b4/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-07-11 20:52:38.847147 tap_belvo-0.0.1b4/tap_belvo/__init__.py
+-rw-r--r--   0        0        0      110 2023-07-11 20:52:38.847147 tap_belvo-0.0.1b4/tap_belvo/__main__.py
+-rw-r--r--   0        0        0     4417 2023-07-11 20:52:38.847147 tap_belvo-0.0.1b4/tap_belvo/client.py
+-rw-r--r--   0        0        0  1025531 2023-07-11 20:52:38.851147 tap_belvo-0.0.1b4/tap_belvo/openapi/BelvoOpenFinanceApiSpec.json
+-rw-r--r--   0        0        0      739 2023-07-11 20:52:38.851147 tap_belvo-0.0.1b4/tap_belvo/openapi/__init__.py
+-rw-r--r--   0        0        0      936 2023-07-11 20:52:38.851147 tap_belvo-0.0.1b4/tap_belvo/streams/__init__.py
+-rw-r--r--   0        0        0     2438 2023-07-11 20:52:38.851147 tap_belvo-0.0.1b4/tap_belvo/streams/banking.py
+-rw-r--r--   0        0        0      758 2023-07-11 20:52:38.851147 tap_belvo-0.0.1b4/tap_belvo/streams/enrichment.py
+-rw-r--r--   0        0        0     1591 2023-07-11 20:52:38.851147 tap_belvo-0.0.1b4/tap_belvo/streams/fiscal.py
+-rw-r--r--   0        0        0      903 2023-07-11 20:52:38.851147 tap_belvo-0.0.1b4/tap_belvo/streams/links.py
+-rw-r--r--   0        0        0     2006 2023-07-11 20:52:38.851147 tap_belvo-0.0.1b4/tap_belvo/tap.py
+-rw-r--r--   0        0        0     4058 1970-01-01 00:00:00.000000 tap_belvo-0.0.1b4/PKG-INFO
```

### Comparing `tap_belvo-0.0.1b3/LICENSE` & `tap_belvo-0.0.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b3/README.md` & `tap_belvo-0.0.1b4/README.md`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b3/pyproject.toml` & `tap_belvo-0.0.1b4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,17 @@
+[build-system]
+build-backend = "poetry_dynamic_versioning.backend"
+requires = [
+  "poetry-core>=1",
+  "poetry-dynamic-versioning",
+]
+
 [tool.poetry]
 name = "tap-belvo"
-version = "0.0.1b3"
+version = "0.0.1b4"
 description = "`tap-belvo` is a Singer tap for Belvo, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 keywords = [
   "ELT",
   "singer.io",
   "Belvo",
 ]
@@ -12,19 +19,23 @@
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-belvo"
 repository = "https://github.com/edgarrmondragon/tap-belvo"
 documentation = "https://github.com/edgarrmondragon/tap-belvo#readme"
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
-singer-sdk = "0.27.0"
-requests-cache = ">=0.9.7,<1.1.0"
+singer-sdk = ">=0.28,<0.30"
+requests-cache = "1.*"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.3.1"
+pytest = "^7.4.0"
+
+[tool.poetry.scripts]
+# CLI declaration
+"tap-belvo" = "tap_belvo.tap:TapBelvo.cli"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3 # Vertical Hanging Indent
 use_parentheses = true
 include_trailing_comma = true
 src_paths = "tap_belvo"
@@ -40,25 +51,14 @@
 python_version = "3.10"
 warn_unused_configs = true
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = ["backoff.*"]
 
-[build-system]
-build-backend = "poetry_dynamic_versioning.backend"
-requires = [
-  "poetry-core>=1",
-  "poetry-dynamic-versioning",
-]
-
-[tool.poetry.scripts]
-# CLI declaration
-"tap-belvo" = "tap_belvo.tap:TapBelvo.cli"
-
 [tool.poetry-dynamic-versioning]
 enable = false
 format-jinja = """
     {%- if distance == 0 -%}
         {{ serialize_pep440(base, stage, revision) }}
     {%- elif revision is not none -%}
         {{ serialize_pep440(base, stage, revision + 1, dev=distance, metadata=[commit]) }}
@@ -68,31 +68,32 @@
 """
 metadata = true
 style = "pep440"
 vcs = "git"
 
 [tool.ruff]
 ignore = [
-  "ANN101", # missing-type-self
-  "DJ", # flake8-django
+  "ANN101",  # missing-type-self
+  "DJ",      # flake8-django
+  "FIX002",  # line-contains-todo
 ]
 line-length = 88
 select = ["ALL"]
 src = ["tap_belvo", "tests"]
 target-version = "py37"
 unfixable = [
   "ERA001",  # commented-out-code
 ]
 
 [tool.ruff.per-file-ignores]
 "noxfile.py" = ["ANN"]
 "tests/*" = [
-  "ANN201", # missing-return-type-public-function
-  "S101", # assert
-  "SLF001", # private-member-access
+  "ANN201",  # missing-return-type-public-function
+  "S101",    # assert
+  "SLF001",  # private-member-access
 ]
 
 [tool.ruff.isort]
 known-first-party = ["tap_belvo"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `tap_belvo-0.0.1b3/tap_belvo/client.py` & `tap_belvo-0.0.1b4/tap_belvo/client.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b3/tap_belvo/openapi/BelvoOpenFinanceApiSpec.json` & `tap_belvo-0.0.1b4/tap_belvo/openapi/BelvoOpenFinanceApiSpec.json`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b3/tap_belvo/openapi/__init__.py` & `tap_belvo-0.0.1b4/tap_belvo/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b3/tap_belvo/streams/__init__.py` & `tap_belvo-0.0.1b4/tap_belvo/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b3/tap_belvo/streams/banking.py` & `tap_belvo-0.0.1b4/tap_belvo/streams/banking.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b3/tap_belvo/streams/enrichment.py` & `tap_belvo-0.0.1b4/tap_belvo/streams/enrichment.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b3/tap_belvo/streams/fiscal.py` & `tap_belvo-0.0.1b4/tap_belvo/streams/fiscal.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b3/tap_belvo/streams/links.py` & `tap_belvo-0.0.1b4/tap_belvo/streams/links.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b3/tap_belvo/tap.py` & `tap_belvo-0.0.1b4/tap_belvo/tap.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b3/PKG-INFO` & `tap_belvo-0.0.1b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tap-belvo
-Version: 0.0.1b3
+Version: 0.0.1b4
 Summary: `tap-belvo` is a Singer tap for Belvo, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-belvo
 License: Apache 2.0
 Keywords: ELT,singer.io,Belvo
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: requests-cache (>=0.9.7,<1.1.0)
-Requires-Dist: singer-sdk (==0.27.0)
+Requires-Dist: requests-cache (==1.*)
+Requires-Dist: singer-sdk (>=0.28,<0.30)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-belvo#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-belvo
 Description-Content-Type: text/markdown
 
 # `tap-belvo`
 
 Singer tap for Belvo.
```

