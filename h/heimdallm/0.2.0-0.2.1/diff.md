# Comparing `tmp/heimdallm-0.2.0.tar.gz` & `tmp/heimdallm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heimdallm-0.2.0.tar", max compression
+gzip compressed data, was "heimdallm-0.2.1.tar", max compression
```

## Comparing `heimdallm-0.2.0.tar` & `heimdallm-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      750 2023-07-10 01:26:12.880524 heimdallm-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    34523 2023-07-10 01:26:12.880524 heimdallm-0.2.0/LICENSE
--rw-r--r--   0        0        0     6958 2023-07-10 01:26:12.880524 heimdallm-0.2.0/README.md
--rw-r--r--   0        0        0       81 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/__init__.py
--rw-r--r--   0        0        0     6583 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrost.py
--rw-r--r--   0        0        0        0 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/__init__.py
--rw-r--r--   0        0        0     5293 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/bifrost.py
--rw-r--r--   0        0        0     5688 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/common.py
--rw-r--r--   0        0        0     6014 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/envelope.py
--rw-r--r--   0        0        0     1234 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/envelopes/sql/mysql/select.j2
--rw-r--r--   0        0        0     1331 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/envelopes/sql/sqlite/select.j2
--rw-r--r--   0        0        0        0 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/envelopes/sql/test.j2
--rw-r--r--   0        0        0     6668 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/exc.py
--rw-r--r--   0        0        0        0 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/mysql/__init__.py
--rw-r--r--   0        0        0    15919 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/mysql/presets.py
--rw-r--r--   0        0        0        0 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/mysql/select/__init__.py
--rw-r--r--   0        0        0     1545 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/mysql/select/bifrost.py
--rw-r--r--   0        0        0      563 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/mysql/select/envelope.py
--rw-r--r--   0        0        0     6391 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/mysql/select/grammar.lark
--rw-r--r--   0        0        0      685 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/mysql/select/validator.py
--rw-r--r--   0        0        0     5029 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/reconstruct.py
--rw-r--r--   0        0        0        0 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/sqlite/__init__.py
--rw-r--r--   0        0        0     3707 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/sqlite/presets.py
--rw-r--r--   0        0        0        0 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/sqlite/select/__init__.py
--rw-r--r--   0        0        0     1971 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/sqlite/select/bifrost.py
--rw-r--r--   0        0        0      564 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/sqlite/select/envelope.py
--rw-r--r--   0        0        0     6737 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/sqlite/select/grammar.lark
--rw-r--r--   0        0        0      685 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/sqlite/select/validator.py
--rw-r--r--   0        0        0        0 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/utils/__init__.py
--rw-r--r--   0        0        0     1546 2023-07-10 01:26:12.884524 heimdallm-0.2.0/heimdallm/bifrosts/sql/utils/identifier.py
--rw-r--r--   0        0        0    11519 2023-07-10 01:26:12.888524 heimdallm-0.2.0/heimdallm/bifrosts/sql/validator.py
--rw-r--r--   0        0        0        0 2023-07-10 01:26:12.888524 heimdallm-0.2.0/heimdallm/bifrosts/sql/visitors/__Init__.py
--rw-r--r--   0        0        0     3005 2023-07-10 01:26:12.888524 heimdallm-0.2.0/heimdallm/bifrosts/sql/visitors/aliases.py
--rw-r--r--   0        0        0     2947 2023-07-10 01:26:12.888524 heimdallm-0.2.0/heimdallm/bifrosts/sql/visitors/ambiguity.py
--rw-r--r--   0        0        0    14153 2023-07-10 01:26:12.888524 heimdallm-0.2.0/heimdallm/bifrosts/sql/visitors/facets.py
--rw-r--r--   0        0        0     1451 2023-07-10 01:26:12.888524 heimdallm-0.2.0/heimdallm/constraints.py
--rw-r--r--   0        0        0     1643 2023-07-10 01:26:12.888524 heimdallm-0.2.0/heimdallm/envelope.py
--rw-r--r--   0        0        0      734 2023-07-10 01:26:12.888524 heimdallm-0.2.0/heimdallm/llm.py
--rw-r--r--   0        0        0        0 2023-07-10 01:26:12.888524 heimdallm-0.2.0/heimdallm/llm_providers/__init__.py
--rw-r--r--   0        0        0      793 2023-07-10 01:26:12.888524 heimdallm-0.2.0/heimdallm/llm_providers/mock.py
--rw-r--r--   0        0        0     2433 2023-07-10 01:26:12.888524 heimdallm-0.2.0/heimdallm/llm_providers/openai.py
--rw-r--r--   0        0        0        0 2023-07-10 01:26:12.888524 heimdallm-0.2.0/heimdallm/support/__init__.py
--rw-r--r--   0        0        0     1051 2023-07-10 01:26:12.888524 heimdallm-0.2.0/heimdallm/support/github.py
--rw-r--r--   0        0        0     1621 2023-07-10 01:26:12.916525 heimdallm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8268 1970-01-01 00:00:00.000000 heimdallm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      750 2023-07-10 22:01:58.825056 heimdallm-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2023-07-10 22:01:58.825056 heimdallm-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6958 2023-07-10 22:01:58.825056 heimdallm-0.2.1/README.md
+-rw-r--r--   0        0        0       81 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/__init__.py
+-rw-r--r--   0        0        0     6583 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrost.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/__init__.py
+-rw-r--r--   0        0        0     5293 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/bifrost.py
+-rw-r--r--   0        0        0     5688 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/common.py
+-rw-r--r--   0        0        0     6014 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/envelope.py
+-rw-r--r--   0        0        0     1234 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/envelopes/sql/mysql/select.j2
+-rw-r--r--   0        0        0     1331 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/envelopes/sql/sqlite/select.j2
+-rw-r--r--   0        0        0        0 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/envelopes/sql/test.j2
+-rw-r--r--   0        0        0     6668 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/exc.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/__init__.py
+-rw-r--r--   0        0        0    15919 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/presets.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/__init__.py
+-rw-r--r--   0        0        0     1545 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/bifrost.py
+-rw-r--r--   0        0        0      563 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/envelope.py
+-rw-r--r--   0        0        0     6391 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/grammar.lark
+-rw-r--r--   0        0        0      685 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/validator.py
+-rw-r--r--   0        0        0     5029 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/reconstruct.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/__init__.py
+-rw-r--r--   0        0        0     3707 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/presets.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/__init__.py
+-rw-r--r--   0        0        0     1971 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/bifrost.py
+-rw-r--r--   0        0        0      564 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/envelope.py
+-rw-r--r--   0        0        0     6737 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/grammar.lark
+-rw-r--r--   0        0        0      685 2023-07-10 22:01:58.829056 heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/validator.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/bifrosts/sql/utils/__init__.py
+-rw-r--r--   0        0        0     1546 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/bifrosts/sql/utils/identifier.py
+-rw-r--r--   0        0        0    11519 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/bifrosts/sql/validator.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/bifrosts/sql/visitors/__Init__.py
+-rw-r--r--   0        0        0     3005 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/bifrosts/sql/visitors/aliases.py
+-rw-r--r--   0        0        0     2947 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/bifrosts/sql/visitors/ambiguity.py
+-rw-r--r--   0        0        0    14153 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/bifrosts/sql/visitors/facets.py
+-rw-r--r--   0        0        0     1451 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/constraints.py
+-rw-r--r--   0        0        0     1643 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/envelope.py
+-rw-r--r--   0        0        0      734 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/llm.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/llm_providers/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/llm_providers/mock.py
+-rw-r--r--   0        0        0     2433 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/llm_providers/openai.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/support/__init__.py
+-rw-r--r--   0        0        0     1051 2023-07-10 22:01:58.833057 heimdallm-0.2.1/heimdallm/support/github.py
+-rw-r--r--   0        0        0     1621 2023-07-10 22:01:58.865057 heimdallm-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8268 1970-01-01 00:00:00.000000 heimdallm-0.2.1/PKG-INFO
```

### Comparing `heimdallm-0.2.0/CONTRIBUTING.md` & `heimdallm-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/LICENSE` & `heimdallm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/README.md` & `heimdallm-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrost.py` & `heimdallm-0.2.1/heimdallm/bifrost.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/bifrost.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/bifrost.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/common.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/common.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/envelope.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/envelope.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/envelopes/sql/mysql/select.j2` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/envelopes/sql/mysql/select.j2`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/envelopes/sql/sqlite/select.j2` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/envelopes/sql/sqlite/select.j2`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/exc.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/exc.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/mysql/presets.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/presets.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/mysql/select/bifrost.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/bifrost.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/mysql/select/envelope.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/envelope.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/mysql/select/grammar.lark` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/grammar.lark`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/mysql/select/validator.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/mysql/select/validator.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/reconstruct.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/reconstruct.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/sqlite/presets.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/presets.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/sqlite/select/bifrost.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/bifrost.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/sqlite/select/envelope.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/envelope.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/sqlite/select/grammar.lark` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/grammar.lark`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/sqlite/select/validator.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/sqlite/select/validator.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/utils/identifier.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/utils/identifier.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/validator.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/validator.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/visitors/aliases.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/visitors/aliases.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/visitors/ambiguity.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/visitors/ambiguity.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/bifrosts/sql/visitors/facets.py` & `heimdallm-0.2.1/heimdallm/bifrosts/sql/visitors/facets.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/constraints.py` & `heimdallm-0.2.1/heimdallm/constraints.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/envelope.py` & `heimdallm-0.2.1/heimdallm/envelope.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/llm.py` & `heimdallm-0.2.1/heimdallm/llm.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/llm_providers/mock.py` & `heimdallm-0.2.1/heimdallm/llm_providers/mock.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/llm_providers/openai.py` & `heimdallm-0.2.1/heimdallm/llm_providers/openai.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/heimdallm/support/github.py` & `heimdallm-0.2.1/heimdallm/support/github.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.2.0/pyproject.toml` & `heimdallm-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heimdallm"
-version = "0.2.0"
+version = "0.2.1"
 description = "Construct trusted SQL queries from untrusted input"
 homepage = "https://github.com/amoffat/HeimdaLLM"
 repository = "https://github.com/amoffat/HeimdaLLM"
 documentation = "https://heimdallm.readthedocs.io/en/latest/"
 authors = ["Andrew Moffat <arwmoffat@gmail.com>"]
 maintainers = ["Andrew Moffat <arwmoffat@gmail.com>"]
 keywords = ["sql", "llm", "ai"]
```

### Comparing `heimdallm-0.2.0/PKG-INFO` & `heimdallm-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heimdallm
-Version: 0.2.0
+Version: 0.2.1
 Summary: Construct trusted SQL queries from untrusted input
 Home-page: https://github.com/amoffat/HeimdaLLM
 License: AGPL-3.0
 Keywords: sql,llm,ai
 Author: Andrew Moffat
 Author-email: arwmoffat@gmail.com
 Maintainer: Andrew Moffat
```

