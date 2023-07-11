# Comparing `tmp/pull_request_codecommit-0.5.2.tar.gz` & `tmp/pull_request_codecommit-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pull_request_codecommit-0.5.2.tar", max compression
+gzip compressed data, was "pull_request_codecommit-0.5.3.tar", max compression
```

## Comparing `pull_request_codecommit-0.5.2.tar` & `pull_request_codecommit-0.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1052 2023-06-21 11:18:06.514315 pull_request_codecommit-0.5.2/LICENSE.md
--rw-r--r--   0        0        0     2336 2023-06-21 11:18:07.170313 pull_request_codecommit-0.5.2/pull_request_codecommit/__init__.py
--rw-r--r--   0        0        0       27 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/aws/__init__.py
--rw-r--r--   0        0        0     4645 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/aws/client.py
--rw-r--r--   0        0        0     1513 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/config.py
--rw-r--r--   0        0        0      139 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/git/__init__.py
--rw-r--r--   0        0        0     2033 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/git/client.py
--rw-r--r--   0        0        0      401 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/git/commit.py
--rw-r--r--   0        0        0     1681 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/git/commits.py
--rw-r--r--   0        0        0     1232 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/git/message.py
--rw-r--r--   0        0        0     1571 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/git/remote.py
--rw-r--r--   0        0        0     1452 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/pull_request.py
--rw-r--r--   0        0        0     2826 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/pull_request_codecommit.py
--rw-r--r--   0        0        0     2793 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/pull_request_proposal.py
--rw-r--r--   0        0        0     1495 2023-06-21 11:18:06.518315 pull_request_codecommit-0.5.2/pull_request_codecommit/repository.py
--rw-r--r--   0        0        0      972 2023-06-21 11:18:07.170313 pull_request_codecommit-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 pull_request_codecommit-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-07-11 06:58:09.142934 pull_request_codecommit-0.5.3/LICENSE.md
+-rw-r--r--   0        0        0     2312 2023-07-11 06:58:09.862938 pull_request_codecommit-0.5.3/pull_request_codecommit/__init__.py
+-rw-r--r--   0        0        0       27 2023-07-11 06:58:09.142934 pull_request_codecommit-0.5.3/pull_request_codecommit/aws/__init__.py
+-rw-r--r--   0        0        0     4645 2023-07-11 06:58:09.142934 pull_request_codecommit-0.5.3/pull_request_codecommit/aws/client.py
+-rw-r--r--   0        0        0     1513 2023-07-11 06:58:09.142934 pull_request_codecommit-0.5.3/pull_request_codecommit/config.py
+-rw-r--r--   0        0        0      139 2023-07-11 06:58:09.142934 pull_request_codecommit-0.5.3/pull_request_codecommit/git/__init__.py
+-rw-r--r--   0        0        0     2033 2023-07-11 06:58:09.142934 pull_request_codecommit-0.5.3/pull_request_codecommit/git/client.py
+-rw-r--r--   0        0        0      401 2023-07-11 06:58:09.142934 pull_request_codecommit-0.5.3/pull_request_codecommit/git/commit.py
+-rw-r--r--   0        0        0     1681 2023-07-11 06:58:09.142934 pull_request_codecommit-0.5.3/pull_request_codecommit/git/commits.py
+-rw-r--r--   0        0        0     1232 2023-07-11 06:58:09.142934 pull_request_codecommit-0.5.3/pull_request_codecommit/git/message.py
+-rw-r--r--   0        0        0     1571 2023-07-11 06:58:09.142934 pull_request_codecommit-0.5.3/pull_request_codecommit/git/remote.py
+-rw-r--r--   0        0        0     1452 2023-07-11 06:58:09.142934 pull_request_codecommit-0.5.3/pull_request_codecommit/pull_request.py
+-rw-r--r--   0        0        0     2826 2023-07-11 06:58:09.142934 pull_request_codecommit-0.5.3/pull_request_codecommit/pull_request_codecommit.py
+-rw-r--r--   0        0        0     2793 2023-07-11 06:58:09.142934 pull_request_codecommit-0.5.3/pull_request_codecommit/pull_request_proposal.py
+-rw-r--r--   0        0        0     1495 2023-07-11 06:58:09.142934 pull_request_codecommit-0.5.3/pull_request_codecommit/repository.py
+-rw-r--r--   0        0        0      972 2023-07-11 06:58:09.862938 pull_request_codecommit-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 pull_request_codecommit-0.5.3/PKG-INFO
```

### Comparing `pull_request_codecommit-0.5.2/LICENSE.md` & `pull_request_codecommit-0.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pull_request_codecommit-0.5.2/pull_request_codecommit/__init__.py` & `pull_request_codecommit-0.5.3/pull_request_codecommit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Optional
 
 import click
 
 from .pull_request import PullRequest
 from .repository import Repository
 
-__version__ = "0.5.2"
+__version__ = "0.5.3"
 
 
-@click.command()
+@click.command()  # type: ignore
 @click.option("-r", "--repository-path", default=None)
 @click.option("-b", "--branch", default=None)
 @click.option("--auto-merge/--no-auto-merge", default=False)
 def main(
     repository_path: Optional[str], branch: Optional[str], auto_merge: bool
 ) -> None:
     """
@@ -76,11 +76,7 @@
     if message is None:
         raise click.ClickException("Pull request was not created")
 
     title = message.splitlines()[0]
     description = "\n".join(message.splitlines()[1:]).lstrip("\n")
 
     pr.update(title, description)
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `pull_request_codecommit-0.5.2/pull_request_codecommit/aws/client.py` & `pull_request_codecommit-0.5.3/pull_request_codecommit/aws/client.py`

 * *Files identical despite different names*

### Comparing `pull_request_codecommit-0.5.2/pull_request_codecommit/config.py` & `pull_request_codecommit-0.5.3/pull_request_codecommit/config.py`

 * *Files identical despite different names*

### Comparing `pull_request_codecommit-0.5.2/pull_request_codecommit/git/client.py` & `pull_request_codecommit-0.5.3/pull_request_codecommit/git/client.py`

 * *Files identical despite different names*

### Comparing `pull_request_codecommit-0.5.2/pull_request_codecommit/git/commits.py` & `pull_request_codecommit-0.5.3/pull_request_codecommit/git/commits.py`

 * *Files identical despite different names*

### Comparing `pull_request_codecommit-0.5.2/pull_request_codecommit/git/message.py` & `pull_request_codecommit-0.5.3/pull_request_codecommit/git/message.py`

 * *Files identical despite different names*

### Comparing `pull_request_codecommit-0.5.2/pull_request_codecommit/git/remote.py` & `pull_request_codecommit-0.5.3/pull_request_codecommit/git/remote.py`

 * *Files identical despite different names*

### Comparing `pull_request_codecommit-0.5.2/pull_request_codecommit/pull_request.py` & `pull_request_codecommit-0.5.3/pull_request_codecommit/pull_request.py`

 * *Files identical despite different names*

### Comparing `pull_request_codecommit-0.5.2/pull_request_codecommit/pull_request_codecommit.py` & `pull_request_codecommit-0.5.3/pull_request_codecommit/pull_request_codecommit.py`

 * *Files identical despite different names*

### Comparing `pull_request_codecommit-0.5.2/pull_request_codecommit/pull_request_proposal.py` & `pull_request_codecommit-0.5.3/pull_request_codecommit/pull_request_proposal.py`

 * *Files identical despite different names*

### Comparing `pull_request_codecommit-0.5.2/pull_request_codecommit/repository.py` & `pull_request_codecommit-0.5.3/pull_request_codecommit/repository.py`

 * *Files identical despite different names*

### Comparing `pull_request_codecommit-0.5.2/pyproject.toml` & `pull_request_codecommit-0.5.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "pull-request-codecommit"
-version = "0.5.2"
+version = "0.5.3"
 description = "pull-request-codecommit creates a PR within CodeCommit based on your commit messages."
 authors = ["Joris Conijn <joris@conijnonline.nl>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.0.3"
 
 [tool.poetry.dev-dependencies]
-black = "^23.1"
-mypy = "^1.0"
-pytest = "^7.2.2"
-pytest-cov = "^4.0.0"
+black = "^23.7"
+mypy = "^1.4"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
 pytest-mypy = "^0.10.3"
 toml = "^0.10.2"
 types-toml = "^0.10.8"
 twine = "^4.0.2"
 xenon = "^0.9.0"
 radon = "^5.1.0"
```

### Comparing `pull_request_codecommit-0.5.2/PKG-INFO` & `pull_request_codecommit-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pull-request-codecommit
-Version: 0.5.2
+Version: 0.5.3
 Summary: pull-request-codecommit creates a PR within CodeCommit based on your commit messages.
 License: MIT
 Author: Joris Conijn
 Author-email: joris@conijnonline.nl
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

