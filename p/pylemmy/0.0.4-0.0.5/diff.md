# Comparing `tmp/pylemmy-0.0.4.tar.gz` & `tmp/pylemmy-0.0.5.tar.gz`

## Comparing `pylemmy-0.0.4.tar` & `pylemmy-0.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 pylemmy-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 pylemmy-0.0.4/mkdocs.yml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pylemmy-0.0.4/.github/workflows/docs.yaml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pylemmy-0.0.4/.github/workflows/integration.yml
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pylemmy-0.0.4/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 pylemmy-0.0.4/.github/workflows/run.yaml
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pylemmy-0.0.4/docs/index.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.4/docs/api/lemmy.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.4/docs/api/utils.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pylemmy-0.0.4/docs/api/models/comment.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pylemmy-0.0.4/docs/api/models/community.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pylemmy-0.0.4/docs/api/models/post.md
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pylemmy-0.0.4/examples/lmgtfy.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/__about__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/__init__.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/endpoints.py
--rw-r--r--   0        0        0    10222 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/lemmy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/py.typed
--rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/auth.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/comment.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/community.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/listing.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/person.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/post.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/site.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/api/utils.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/models/__init__.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/models/comment.py
--rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/models/community.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pylemmy/models/post.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylemmy-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pylemmy-0.0.4/tests/integration/__init__.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pylemmy-0.0.4/tests/integration/docker-compose.yml
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pylemmy-0.0.4/tests/integration/lemmy.hjson
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 pylemmy-0.0.4/tests/integration/test_api.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 pylemmy-0.0.4/tests/integration/test_lemmy.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 pylemmy-0.0.4/tests/unit/test_utils.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pylemmy-0.0.4/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pylemmy-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 pylemmy-0.0.4/README.md
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 pylemmy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 pylemmy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 pylemmy-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 pylemmy-0.0.5/mkdocs.yml
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pylemmy-0.0.5/.github/workflows/docs.yaml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pylemmy-0.0.5/.github/workflows/integration.yml
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pylemmy-0.0.5/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 pylemmy-0.0.5/.github/workflows/run.yaml
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pylemmy-0.0.5/docs/index.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.5/docs/api/lemmy.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.5/docs/api/utils.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pylemmy-0.0.5/docs/api/models/comment.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pylemmy-0.0.5/docs/api/models/community.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pylemmy-0.0.5/docs/api/models/post.md
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pylemmy-0.0.5/examples/lmgtfy.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/__about__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/endpoints.py
+-rw-r--r--   0        0        0    10222 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/lemmy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/py.typed
+-rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/auth.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/comment.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/community.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/listing.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/person.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/post.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/site.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/utils.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/models/__init__.py
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/models/comment.py
+-rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/models/community.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/models/post.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylemmy-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pylemmy-0.0.5/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pylemmy-0.0.5/tests/integration/docker-compose.yml
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pylemmy-0.0.5/tests/integration/lemmy.hjson
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 pylemmy-0.0.5/tests/integration/test_api.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 pylemmy-0.0.5/tests/integration/test_lemmy.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 pylemmy-0.0.5/tests/unit/test_utils.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pylemmy-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pylemmy-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 pylemmy-0.0.5/README.md
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 pylemmy-0.0.5/PKG-INFO
```

### Comparing `pylemmy-0.0.4/mkdocs.yml` & `pylemmy-0.0.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/.github/workflows/docs.yaml` & `pylemmy-0.0.5/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/.github/workflows/publish.yaml` & `pylemmy-0.0.5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/.github/workflows/run.yaml` & `pylemmy-0.0.5/.github/workflows/run.yaml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/docs/index.md` & `pylemmy-0.0.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/examples/lmgtfy.py` & `pylemmy-0.0.5/examples/lmgtfy.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/pylemmy/endpoints.py` & `pylemmy-0.0.5/pylemmy/endpoints.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/pylemmy/lemmy.py` & `pylemmy-0.0.5/pylemmy/lemmy.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/pylemmy/utils.py` & `pylemmy-0.0.5/pylemmy/utils.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/pylemmy/api/comment.py` & `pylemmy-0.0.5/pylemmy/api/comment.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/pylemmy/api/community.py` & `pylemmy-0.0.5/pylemmy/api/community.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/pylemmy/api/post.py` & `pylemmy-0.0.5/pylemmy/api/post.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/pylemmy/models/comment.py` & `pylemmy-0.0.5/pylemmy/models/comment.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     def create_report(self, reason: str) -> CommentReport:
         """Report this comment.
 
         :param reason: A reason for the report.
         """
         payload = api.comment.CreateCommentReport(
             auth=self.lemmy.get_token(),
-            comment_id=self.comment_view.post.id,
+            comment_id=self.comment_view.comment.id,
             reason=reason,
         )
         result = self.lemmy.post_request(LemmyAPI.CreateCommentReport, params=payload)
         parsed_result = api.comment.CommentReportResponse(**result)
 
         return CommentReport(
             lemmy=self.lemmy, report=parsed_result.comment_report_view, comment=self
```

### Comparing `pylemmy-0.0.4/pylemmy/models/community.py` & `pylemmy-0.0.5/pylemmy/models/community.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/pylemmy/models/post.py` & `pylemmy-0.0.5/pylemmy/models/post.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/tests/integration/docker-compose.yml` & `pylemmy-0.0.5/tests/integration/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/tests/integration/lemmy.hjson` & `pylemmy-0.0.5/tests/integration/lemmy.hjson`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/tests/integration/test_api.py` & `pylemmy-0.0.5/tests/integration/test_api.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/tests/integration/test_lemmy.py` & `pylemmy-0.0.5/tests/integration/test_lemmy.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/tests/unit/test_utils.py` & `pylemmy-0.0.5/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/.gitignore` & `pylemmy-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/LICENSE.txt` & `pylemmy-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/README.md` & `pylemmy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/pyproject.toml` & `pylemmy-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.4/PKG-INFO` & `pylemmy-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylemmy
-Version: 0.0.4
+Version: 0.0.5
 Summary: pylemmy enables simple access to Lemmy's API with Python
 Project-URL: Documentation, https://dcferreira.com/pylemmy
 Project-URL: Issues, https://github.com/dcferreira/pylemmy/issues
 Project-URL: Source, https://github.com/dcferreira/pylemmy
 Author-email: Daniel Ferreira <daniel.ferreira.1@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

