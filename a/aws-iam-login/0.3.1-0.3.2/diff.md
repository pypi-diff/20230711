# Comparing `tmp/aws_iam_login-0.3.1.tar.gz` & `tmp/aws_iam_login-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_iam_login-0.3.1.tar", max compression
+gzip compressed data, was "aws_iam_login-0.3.2.tar", max compression
```

## Comparing `aws_iam_login-0.3.1.tar` & `aws_iam_login-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1052 2023-03-06 09:57:55.101828 aws_iam_login-0.3.1/LICENSE.md
--rw-r--r--   0        0        0     3400 2023-03-06 09:57:55.101828 aws_iam_login-0.3.1/README.md
--rw-r--r--   0        0        0     2685 2023-03-06 09:57:55.101828 aws_iam_login-0.3.1/aws_iam_login/__init__.py
--rw-r--r--   0        0        0     1510 2023-03-06 09:57:55.101828 aws_iam_login-0.3.1/aws_iam_login/access_key.py
--rw-r--r--   0        0        0        0 2023-03-06 09:57:55.101828 aws_iam_login-0.3.1/aws_iam_login/actions/__init__.py
--rw-r--r--   0        0        0     1076 2023-03-06 09:57:55.101828 aws_iam_login-0.3.1/aws_iam_login/actions/action.py
--rw-r--r--   0        0        0     1376 2023-03-06 09:57:55.101828 aws_iam_login-0.3.1/aws_iam_login/actions/initialize_configuration.py
--rw-r--r--   0        0        0     3401 2023-03-06 09:57:55.101828 aws_iam_login-0.3.1/aws_iam_login/actions/rotate_access_keys.py
--rw-r--r--   0        0        0     1486 2023-03-06 09:57:55.101828 aws_iam_login-0.3.1/aws_iam_login/application_context.py
--rw-r--r--   0        0        0     2545 2023-03-06 09:57:55.101828 aws_iam_login-0.3.1/aws_iam_login/aws_config.py
--rw-r--r--   0        0        0     1275 2023-03-06 09:57:55.101828 aws_iam_login-0.3.1/aws_iam_login/credentials.py
--rw-r--r--   0        0        0      428 2023-03-06 09:57:55.101828 aws_iam_login-0.3.1/aws_iam_login/observer.py
--rw-r--r--   0        0        0      895 2023-03-06 09:57:55.101828 aws_iam_login-0.3.1/aws_iam_login/temp_credentials.py
--rw-r--r--   0        0        0      902 2023-03-06 09:57:55.101828 aws_iam_login-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4045 1970-01-01 00:00:00.000000 aws_iam_login-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-07-11 07:30:20.773662 aws_iam_login-0.3.2/LICENSE.md
+-rw-r--r--   0        0        0     3400 2023-07-11 07:30:20.773662 aws_iam_login-0.3.2/README.md
+-rw-r--r--   0        0        0     2710 2023-07-11 07:30:21.701659 aws_iam_login-0.3.2/aws_iam_login/__init__.py
+-rw-r--r--   0        0        0     1510 2023-07-11 07:30:20.773662 aws_iam_login-0.3.2/aws_iam_login/access_key.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:30:20.773662 aws_iam_login-0.3.2/aws_iam_login/actions/__init__.py
+-rw-r--r--   0        0        0     1076 2023-07-11 07:30:20.773662 aws_iam_login-0.3.2/aws_iam_login/actions/action.py
+-rw-r--r--   0        0        0     1376 2023-07-11 07:30:20.773662 aws_iam_login-0.3.2/aws_iam_login/actions/initialize_configuration.py
+-rw-r--r--   0        0        0     3401 2023-07-11 07:30:20.773662 aws_iam_login-0.3.2/aws_iam_login/actions/rotate_access_keys.py
+-rw-r--r--   0        0        0     1486 2023-07-11 07:30:20.773662 aws_iam_login-0.3.2/aws_iam_login/application_context.py
+-rw-r--r--   0        0        0     2545 2023-07-11 07:30:20.773662 aws_iam_login-0.3.2/aws_iam_login/aws_config.py
+-rw-r--r--   0        0        0     1275 2023-07-11 07:30:20.773662 aws_iam_login-0.3.2/aws_iam_login/credentials.py
+-rw-r--r--   0        0        0      428 2023-07-11 07:30:20.773662 aws_iam_login-0.3.2/aws_iam_login/observer.py
+-rw-r--r--   0        0        0      895 2023-07-11 07:30:20.773662 aws_iam_login-0.3.2/aws_iam_login/temp_credentials.py
+-rw-r--r--   0        0        0     1138 2023-07-11 07:30:21.701659 aws_iam_login-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4045 1970-01-01 00:00:00.000000 aws_iam_login-0.3.2/PKG-INFO
```

### Comparing `aws_iam_login-0.3.1/LICENSE.md` & `aws_iam_login-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aws_iam_login-0.3.1/README.md` & `aws_iam_login-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `aws_iam_login-0.3.1/aws_iam_login/__init__.py` & `aws_iam_login-0.3.2/aws_iam_login/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 from aws_iam_login.observer import Observer
 from aws_iam_login.temp_credentials import TempCredentials
 from aws_iam_login.aws_config import AWSConfig
 from aws_iam_login.actions.rotate_access_keys import RotateAccessKeys
 from aws_iam_login.credentials import Credentials
 from aws_iam_login.application_context import ApplicationContext, ApplicationMessages
 
+__version__ = "0.3.2"
 
-@click.group(invoke_without_command=True)
+
+@click.group(invoke_without_command=True)  # type: ignore
 @click.option("--debug/--no-debug")
 @click.argument("profile")
 @click.pass_context
 def main(ctx: Context, debug: bool, profile: str) -> None:
     """
     aws-iam-login
     """
@@ -45,15 +47,15 @@
         click.echo(f"ClientError: {exc}")
         exit(1)
     except ParamValidationError as exc:
         click.echo(f"ValidationError: {exc}")
         exit(1)
 
 
-@main.command()
+@main.command()  # type: ignore
 @click.pass_obj
 def init(ctx: ApplicationContext) -> None:
     """
     Initialize your `.aws/configuration`
     """
     click.echo(f"Looking up additional required data...")
 
@@ -63,15 +65,15 @@
     if not action.execute():
         click.echo(f"Failed to initialize the {ctx.profile} profile")
         exit(1)
 
     click.echo(f"The {ctx.profile} profile has been successfully initialized!")
 
 
-@main.command()
+@main.command()  # type: ignore
 @click.pass_obj
 def rotate(ctx: ApplicationContext) -> None:
     """
     Rotate your IAM User credentials
     """
     click.echo(f"Key rotation process in progress")
 
@@ -79,11 +81,7 @@
     action.subscribe_subject(ctx.subject)
 
     if not action.execute():
         click.echo(f"Failed to rotate the access keys for the {ctx.profile} profile")
         exit(1)
 
     click.echo(f"Keys successfully rotated for the {ctx.profile} profile")
-
-
-if __name__ == "__main__":
-    main(obj={})
```

### Comparing `aws_iam_login-0.3.1/aws_iam_login/access_key.py` & `aws_iam_login-0.3.2/aws_iam_login/access_key.py`

 * *Files identical despite different names*

### Comparing `aws_iam_login-0.3.1/aws_iam_login/actions/action.py` & `aws_iam_login-0.3.2/aws_iam_login/actions/action.py`

 * *Files identical despite different names*

### Comparing `aws_iam_login-0.3.1/aws_iam_login/actions/initialize_configuration.py` & `aws_iam_login-0.3.2/aws_iam_login/actions/initialize_configuration.py`

 * *Files identical despite different names*

### Comparing `aws_iam_login-0.3.1/aws_iam_login/actions/rotate_access_keys.py` & `aws_iam_login-0.3.2/aws_iam_login/actions/rotate_access_keys.py`

 * *Files identical despite different names*

### Comparing `aws_iam_login-0.3.1/aws_iam_login/application_context.py` & `aws_iam_login-0.3.2/aws_iam_login/application_context.py`

 * *Files identical despite different names*

### Comparing `aws_iam_login-0.3.1/aws_iam_login/aws_config.py` & `aws_iam_login-0.3.2/aws_iam_login/aws_config.py`

 * *Files identical despite different names*

### Comparing `aws_iam_login-0.3.1/aws_iam_login/credentials.py` & `aws_iam_login-0.3.2/aws_iam_login/credentials.py`

 * *Files identical despite different names*

### Comparing `aws_iam_login-0.3.1/aws_iam_login/temp_credentials.py` & `aws_iam_login-0.3.2/aws_iam_login/temp_credentials.py`

 * *Files identical despite different names*

### Comparing `aws_iam_login-0.3.1/pyproject.toml` & `aws_iam_login-0.3.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "aws-iam-login"
-version = "0.3.1"
+version = "0.3.2"
 description = "Configures STS credentials using a MFA authenticated session."
 authors = ["Joris Conijn <jorisconijn@binx.io>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.3"
 boto3 = "^1.24.11"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-black = "^22.6.0"
-pytest-cov = "^3.0.0"
-mypy = "^0.961"
+pytest = "^7.4.0"
+black = "^23.3.0"
+pytest-cov = "^4.1.0"
+mypy = "^1.4"
 radon = "^5.1.0"
 xenon = "^0.9.0"
 twine = "^4.0.1"
 
 [tool.poetry.scripts]
 aws-iam-login = "aws_iam_login:main"
 
@@ -38,10 +38,20 @@
 fail_under = 95
 exclude_lines = [
     "pragma: no cover",
     "if __name__ == .__main__.:",
     "@abstract"
 ]
 
+[tool.semantic_release]
+version_variable = [
+    "aws_iam_login/__init__.py:__version__",
+    "pyproject.toml:version"
+]
+branch = "main"
+upload_to_pypi = true
+upload_to_release = true
+build_command = "pip install poetry && poetry build"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aws_iam_login-0.3.1/PKG-INFO` & `aws_iam_login-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-iam-login
-Version: 0.3.1
+Version: 0.3.2
 Summary: Configures STS credentials using a MFA authenticated session.
 License: MIT
 Author: Joris Conijn
 Author-email: jorisconijn@binx.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

