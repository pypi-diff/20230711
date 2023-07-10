# Comparing `tmp/making_with_code_cli-1.2.0.tar.gz` & `tmp/making_with_code_cli-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "making_with_code_cli-1.2.0.tar", max compression
+gzip compressed data, was "making_with_code_cli-1.2.1.tar", max compression
```

## Comparing `making_with_code_cli-1.2.0.tar` & `making_with_code_cli-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1342 2023-05-30 14:14:06.604035 making_with_code_cli-1.2.0/README.md
--rw-r--r--   0        0        0     8206 2023-07-10 21:40:44.612254 making_with_code_cli-1.2.0/making_with_code_cli/cli.py
--rw-r--r--   0        0        0    15392 2023-07-10 20:16:58.660240 making_with_code_cli-1.2.0/making_with_code_cli/cli_setup.py
--rw-r--r--   0        0        0      551 2023-07-10 19:39:26.763192 making_with_code_cli-1.2.0/making_with_code_cli/curriculum.py
--rw-r--r--   0        0        0      658 2023-07-10 20:30:48.777211 making_with_code_cli-1.2.0/making_with_code_cli/errors.py
--rw-r--r--   0        0        0      276 2023-06-05 20:21:54.165003 making_with_code_cli-1.2.0/making_with_code_cli/git_backend/__init__.py
--rw-r--r--   0        0        0     1613 2023-07-02 18:57:59.595603 making_with_code_cli-1.2.0/making_with_code_cli/git_backend/base_backend.py
--rw-r--r--   0        0        0     3461 2023-06-05 20:20:21.178737 making_with_code_cli-1.2.0/making_with_code_cli/git_backend/github_backend.py
--rw-r--r--   0        0        0     3845 2023-06-05 20:21:08.636148 making_with_code_cli-1.2.0/making_with_code_cli/git_backend/github_org_backend.py
--rw-r--r--   0        0        0     4024 2023-07-10 20:40:53.894216 making_with_code_cli-1.2.0/making_with_code_cli/git_backend/mwc_backend.py
--rw-r--r--   0        0        0      309 2023-07-10 21:24:34.798346 making_with_code_cli-1.2.0/making_with_code_cli/git_wrapper.py
--rw-r--r--   0        0        0      266 2023-05-30 14:14:06.615290 making_with_code_cli-1.2.0/making_with_code_cli/helpers.py
--rw-r--r--   0        0        0     1526 2023-07-10 20:12:17.374391 making_with_code_cli-1.2.0/making_with_code_cli/mwc_accounts_api.py
--rw-r--r--   0        0        0     1629 2023-05-30 14:14:06.616770 making_with_code_cli-1.2.0/making_with_code_cli/settings.py
--rw-r--r--   0        0        0     1682 2023-05-30 14:14:06.617319 making_with_code_cli-1.2.0/making_with_code_cli/styles.py
--rw-r--r--   0        0        0      663 2023-07-10 21:45:57.855472 making_with_code_cli-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 making_with_code_cli-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1342 2023-05-30 14:14:06.604035 making_with_code_cli-1.2.1/README.md
+-rw-r--r--   0        0        0     8199 2023-07-10 22:17:59.387044 making_with_code_cli-1.2.1/making_with_code_cli/cli.py
+-rw-r--r--   0        0        0    15392 2023-07-10 20:16:58.660240 making_with_code_cli-1.2.1/making_with_code_cli/cli_setup.py
+-rw-r--r--   0        0        0      551 2023-07-10 19:39:26.763192 making_with_code_cli-1.2.1/making_with_code_cli/curriculum.py
+-rw-r--r--   0        0        0      658 2023-07-10 20:30:48.777211 making_with_code_cli-1.2.1/making_with_code_cli/errors.py
+-rw-r--r--   0        0        0      276 2023-06-05 20:21:54.165003 making_with_code_cli-1.2.1/making_with_code_cli/git_backend/__init__.py
+-rw-r--r--   0        0        0     1613 2023-07-02 18:57:59.595603 making_with_code_cli-1.2.1/making_with_code_cli/git_backend/base_backend.py
+-rw-r--r--   0        0        0     3461 2023-06-05 20:20:21.178737 making_with_code_cli-1.2.1/making_with_code_cli/git_backend/github_backend.py
+-rw-r--r--   0        0        0     3845 2023-06-05 20:21:08.636148 making_with_code_cli-1.2.1/making_with_code_cli/git_backend/github_org_backend.py
+-rw-r--r--   0        0        0     4024 2023-07-10 20:40:53.894216 making_with_code_cli-1.2.1/making_with_code_cli/git_backend/mwc_backend.py
+-rw-r--r--   0        0        0      309 2023-07-10 21:24:34.798346 making_with_code_cli-1.2.1/making_with_code_cli/git_wrapper.py
+-rw-r--r--   0        0        0      266 2023-05-30 14:14:06.615290 making_with_code_cli-1.2.1/making_with_code_cli/helpers.py
+-rw-r--r--   0        0        0     1526 2023-07-10 20:12:17.374391 making_with_code_cli-1.2.1/making_with_code_cli/mwc_accounts_api.py
+-rw-r--r--   0        0        0     1629 2023-05-30 14:14:06.616770 making_with_code_cli-1.2.1/making_with_code_cli/settings.py
+-rw-r--r--   0        0        0     1682 2023-05-30 14:14:06.617319 making_with_code_cli-1.2.1/making_with_code_cli/styles.py
+-rw-r--r--   0        0        0      663 2023-07-10 22:18:06.934668 making_with_code_cli-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 making_with_code_cli-1.2.1/PKG-INFO
```

### Comparing `making_with_code_cli-1.2.0/README.md` & `making_with_code_cli-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.0/making_with_code_cli/cli.py` & `making_with_code_cli-1.2.1/making_with_code_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     curriculum = get_curriculum(settings)
     settings['course'] = choose_course(
         [course['name'] for course in curriculum['courses']], 
         default=settings.get('course')
     )
     course = [c for c in curriculum['courses'] if c['name'] == settings['course']][0]
     if Platform.detect() & (Platform.MAC | Platform.UBUNTU):
-        settings['editor'] = choose_editor(settings.get('editor', 'atom'))
+        settings['editor'] = choose_editor(settings.get('editor', 'code'))
     G = get_backend(course['git_backend'])
     settings = G.extend_settings(settings)
     if yes:
         click.echo(info("Updated settings:"))
         click.echo(info(yaml.dump(settings), preformatted=True))
     else:
         click.echo(info(yaml.dump(settings), preformatted=True))
@@ -220,15 +220,12 @@
                 click.echo(address("Nice job! All your work in this module has been submitted."))
             else:
                 click.echo(info("Cancelled the submit for now."))
         except CalledProcessError:
             click.echo(info("Everything is already up to date."))
     else:
         click.echo(error("You are not in a lab, problem set, or project folder."))
-    
-
-
```

### Comparing `making_with_code_cli-1.2.0/making_with_code_cli/cli_setup.py` & `making_with_code_cli-1.2.1/making_with_code_cli/cli_setup.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.0/making_with_code_cli/curriculum.py` & `making_with_code_cli-1.2.1/making_with_code_cli/curriculum.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.0/making_with_code_cli/errors.py` & `making_with_code_cli-1.2.1/making_with_code_cli/errors.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.0/making_with_code_cli/git_backend/base_backend.py` & `making_with_code_cli-1.2.1/making_with_code_cli/git_backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.0/making_with_code_cli/git_backend/github_backend.py` & `making_with_code_cli-1.2.1/making_with_code_cli/git_backend/github_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.0/making_with_code_cli/git_backend/github_org_backend.py` & `making_with_code_cli-1.2.1/making_with_code_cli/git_backend/github_org_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.0/making_with_code_cli/git_backend/mwc_backend.py` & `making_with_code_cli-1.2.1/making_with_code_cli/git_backend/mwc_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.0/making_with_code_cli/mwc_accounts_api.py` & `making_with_code_cli-1.2.1/making_with_code_cli/mwc_accounts_api.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.0/making_with_code_cli/settings.py` & `making_with_code_cli-1.2.1/making_with_code_cli/settings.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.0/making_with_code_cli/styles.py` & `making_with_code_cli-1.2.1/making_with_code_cli/styles.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.0/pyproject.toml` & `making_with_code_cli-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "making-with-code-cli"
-version = "1.2.0"
+version = "1.2.1"
 description = "Courseware for Making With Code"
 authors = ["Chris Proctor <chris@chrisproctor.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/cproctor/making-with-code-courseware"
 
 [tool.poetry.dependencies]
```

### Comparing `making_with_code_cli-1.2.0/PKG-INFO` & `making_with_code_cli-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: making-with-code-cli
-Version: 1.2.0
+Version: 1.2.1
 Summary: Courseware for Making With Code
 Home-page: https://github.com/cproctor/making-with-code-courseware
 License: MIT
 Author: Chris Proctor
 Author-email: chris@chrisproctor.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

