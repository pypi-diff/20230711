# Comparing `tmp/making_with_code_cli-1.2.1.tar.gz` & `tmp/making_with_code_cli-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "making_with_code_cli-1.2.1.tar", max compression
+gzip compressed data, was "making_with_code_cli-1.2.2.tar", max compression
```

## Comparing `making_with_code_cli-1.2.1.tar` & `making_with_code_cli-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1342 2023-05-30 14:14:06.604035 making_with_code_cli-1.2.1/README.md
--rw-r--r--   0        0        0     8199 2023-07-10 22:17:59.387044 making_with_code_cli-1.2.1/making_with_code_cli/cli.py
--rw-r--r--   0        0        0    15392 2023-07-10 20:16:58.660240 making_with_code_cli-1.2.1/making_with_code_cli/cli_setup.py
--rw-r--r--   0        0        0      551 2023-07-10 19:39:26.763192 making_with_code_cli-1.2.1/making_with_code_cli/curriculum.py
--rw-r--r--   0        0        0      658 2023-07-10 20:30:48.777211 making_with_code_cli-1.2.1/making_with_code_cli/errors.py
--rw-r--r--   0        0        0      276 2023-06-05 20:21:54.165003 making_with_code_cli-1.2.1/making_with_code_cli/git_backend/__init__.py
--rw-r--r--   0        0        0     1613 2023-07-02 18:57:59.595603 making_with_code_cli-1.2.1/making_with_code_cli/git_backend/base_backend.py
--rw-r--r--   0        0        0     3461 2023-06-05 20:20:21.178737 making_with_code_cli-1.2.1/making_with_code_cli/git_backend/github_backend.py
--rw-r--r--   0        0        0     3845 2023-06-05 20:21:08.636148 making_with_code_cli-1.2.1/making_with_code_cli/git_backend/github_org_backend.py
--rw-r--r--   0        0        0     4024 2023-07-10 20:40:53.894216 making_with_code_cli-1.2.1/making_with_code_cli/git_backend/mwc_backend.py
--rw-r--r--   0        0        0      309 2023-07-10 21:24:34.798346 making_with_code_cli-1.2.1/making_with_code_cli/git_wrapper.py
--rw-r--r--   0        0        0      266 2023-05-30 14:14:06.615290 making_with_code_cli-1.2.1/making_with_code_cli/helpers.py
--rw-r--r--   0        0        0     1526 2023-07-10 20:12:17.374391 making_with_code_cli-1.2.1/making_with_code_cli/mwc_accounts_api.py
--rw-r--r--   0        0        0     1629 2023-05-30 14:14:06.616770 making_with_code_cli-1.2.1/making_with_code_cli/settings.py
--rw-r--r--   0        0        0     1682 2023-05-30 14:14:06.617319 making_with_code_cli-1.2.1/making_with_code_cli/styles.py
--rw-r--r--   0        0        0      663 2023-07-10 22:18:06.934668 making_with_code_cli-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 making_with_code_cli-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1342 2023-05-30 14:14:06.604035 making_with_code_cli-1.2.2/README.md
+-rw-r--r--   0        0        0     8199 2023-07-10 22:17:59.387044 making_with_code_cli-1.2.2/making_with_code_cli/cli.py
+-rw-r--r--   0        0        0    15392 2023-07-10 20:16:58.660240 making_with_code_cli-1.2.2/making_with_code_cli/cli_setup.py
+-rw-r--r--   0        0        0      551 2023-07-10 19:39:26.763192 making_with_code_cli-1.2.2/making_with_code_cli/curriculum.py
+-rw-r--r--   0        0        0      658 2023-07-10 20:30:48.777211 making_with_code_cli-1.2.2/making_with_code_cli/errors.py
+-rw-r--r--   0        0        0      276 2023-06-05 20:21:54.165003 making_with_code_cli-1.2.2/making_with_code_cli/git_backend/__init__.py
+-rw-r--r--   0        0        0     1613 2023-07-02 18:57:59.595603 making_with_code_cli-1.2.2/making_with_code_cli/git_backend/base_backend.py
+-rw-r--r--   0        0        0     3461 2023-06-05 20:20:21.178737 making_with_code_cli-1.2.2/making_with_code_cli/git_backend/github_backend.py
+-rw-r--r--   0        0        0     3845 2023-06-05 20:21:08.636148 making_with_code_cli-1.2.2/making_with_code_cli/git_backend/github_org_backend.py
+-rw-r--r--   0        0        0     4048 2023-07-11 16:15:54.845783 making_with_code_cli-1.2.2/making_with_code_cli/git_backend/mwc_backend.py
+-rw-r--r--   0        0        0      309 2023-07-10 21:24:34.798346 making_with_code_cli-1.2.2/making_with_code_cli/git_wrapper.py
+-rw-r--r--   0        0        0      266 2023-05-30 14:14:06.615290 making_with_code_cli-1.2.2/making_with_code_cli/helpers.py
+-rw-r--r--   0        0        0     1526 2023-07-10 20:12:17.374391 making_with_code_cli-1.2.2/making_with_code_cli/mwc_accounts_api.py
+-rw-r--r--   0        0        0     1629 2023-05-30 14:14:06.616770 making_with_code_cli-1.2.2/making_with_code_cli/settings.py
+-rw-r--r--   0        0        0     1682 2023-05-30 14:14:06.617319 making_with_code_cli-1.2.2/making_with_code_cli/styles.py
+-rw-r--r--   0        0        0      663 2023-07-11 16:16:07.656393 making_with_code_cli-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 making_with_code_cli-1.2.2/PKG-INFO
```

### Comparing `making_with_code_cli-1.2.1/README.md` & `making_with_code_cli-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.1/making_with_code_cli/cli.py` & `making_with_code_cli-1.2.2/making_with_code_cli/cli.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.1/making_with_code_cli/cli_setup.py` & `making_with_code_cli-1.2.2/making_with_code_cli/cli_setup.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.1/making_with_code_cli/curriculum.py` & `making_with_code_cli-1.2.2/making_with_code_cli/curriculum.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.1/making_with_code_cli/errors.py` & `making_with_code_cli-1.2.2/making_with_code_cli/errors.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.1/making_with_code_cli/git_backend/base_backend.py` & `making_with_code_cli-1.2.2/making_with_code_cli/git_backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.1/making_with_code_cli/git_backend/github_backend.py` & `making_with_code_cli-1.2.2/making_with_code_cli/git_backend/github_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.1/making_with_code_cli/git_backend/github_org_backend.py` & `making_with_code_cli-1.2.2/making_with_code_cli/git_backend/github_org_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.1/making_with_code_cli/git_backend/mwc_backend.py` & `making_with_code_cli-1.2.2/making_with_code_cli/git_backend/mwc_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             self.relocate_existing_directory(modpath)
         if not self.user_has_repo(repo_name):
             self.create_from_template(repo_owner, repo_name)
         with cd(modpath.parent):
             self.clone_repo(repo_name)
         if (modpath / COMMIT_TEMPLATE).exists():
             with cd(modpath):
-                run(f"git config commit.template {COMMIT_TEMPLATE}")
+                run(f"git config commit.template {COMMIT_TEMPLATE}", shell=True, check=True)
 
     def user_has_repo(self, repo_name):
         """Checks to see whether a user already has the named repo.
         """
         url = f"/repos/{self.settings['mwc_username']}/{repo_name}"
         response = self.authenticated_mwc_request('get', url)
         return response.ok
```

### Comparing `making_with_code_cli-1.2.1/making_with_code_cli/mwc_accounts_api.py` & `making_with_code_cli-1.2.2/making_with_code_cli/mwc_accounts_api.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.1/making_with_code_cli/settings.py` & `making_with_code_cli-1.2.2/making_with_code_cli/settings.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.1/making_with_code_cli/styles.py` & `making_with_code_cli-1.2.2/making_with_code_cli/styles.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.1/pyproject.toml` & `making_with_code_cli-1.2.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "making-with-code-cli"
-version = "1.2.1"
+version = "1.2.2"
 description = "Courseware for Making With Code"
 authors = ["Chris Proctor <chris@chrisproctor.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/cproctor/making-with-code-courseware"
 
 [tool.poetry.dependencies]
```

### Comparing `making_with_code_cli-1.2.1/PKG-INFO` & `making_with_code_cli-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: making-with-code-cli
-Version: 1.2.1
+Version: 1.2.2
 Summary: Courseware for Making With Code
 Home-page: https://github.com/cproctor/making-with-code-courseware
 License: MIT
 Author: Chris Proctor
 Author-email: chris@chrisproctor.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

