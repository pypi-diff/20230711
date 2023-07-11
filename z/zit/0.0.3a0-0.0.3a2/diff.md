# Comparing `tmp/zit-0.0.3a0.tar.gz` & `tmp/zit-0.0.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zit-0.0.3a0.tar", max compression
+gzip compressed data, was "zit-0.0.3a2.tar", max compression
```

## Comparing `zit-0.0.3a0.tar` & `zit-0.0.3a2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1018 2023-07-10 18:29:27.055868 zit-0.0.3a0/pyproject.toml
--rw-r--r--   0        0        0       72 2022-01-10 03:44:16.795928 zit-0.0.3a0/zit/__init__.py
--rw-r--r--   0        0        0     1544 2023-04-14 12:30:48.576605 zit-0.0.3a0/zit/auth.py
--rw-r--r--   0        0        0      582 2023-07-07 04:26:24.431211 zit-0.0.3a0/zit/config.py
--rw-r--r--   0        0        0     9138 2023-07-07 12:56:08.546696 zit-0.0.3a0/zit/dashboard.py
--rw-r--r--   0        0        0       60 2023-06-15 21:58:13.307052 zit-0.0.3a0/zit/dataset/__init__.py
--rw-r--r--   0        0        0      407 2023-05-11 08:42:13.675272 zit-0.0.3a0/zit/dataset/build.py
--rw-r--r--   0        0        0        0 2023-06-15 21:56:33.152907 zit-0.0.3a0/zit/dataset/classification.py
--rw-r--r--   0        0        0     2029 2023-06-15 17:30:11.785818 zit-0.0.3a0/zit/dataset/convert.py
--rw-r--r--   0        0        0     1577 2023-07-10 11:08:29.567160 zit-0.0.3a0/zit/dataset/detection.py
--rw-r--r--   0        0        0      427 2023-05-11 07:24:56.576494 zit-0.0.3a0/zit/dataset/factory.py
--rw-r--r--   0        0        0        0 2023-05-11 05:37:14.408208 zit-0.0.3a0/zit/dataset/keypoints.py
--rw-r--r--   0        0        0    15732 2023-07-10 11:03:37.537197 zit-0.0.3a0/zit/dataset/manager.py
--rw-r--r--   0        0        0        0 2023-05-11 05:37:56.638196 zit-0.0.3a0/zit/dataset/multilabel_classification.py
--rw-r--r--   0        0        0        0 2023-05-11 05:36:54.588213 zit-0.0.3a0/zit/dataset/segmentation.py
--rw-r--r--   0        0        0    12010 2023-07-07 20:00:48.386764 zit-0.0.3a0/zit/formula.py
--rw-r--r--   0        0        0      617 2023-04-16 19:16:58.258259 zit-0.0.3a0/zit/main.py
--rw-r--r--   0        0        0      712 2023-07-10 11:09:05.807157 zit-0.0.3a0/zit/routes/__init__.py
--rw-r--r--   0        0        0      520 2023-06-18 22:26:38.078376 zit-0.0.3a0/zit/routes/dataset/annotations.py
--rw-r--r--   0        0        0      831 2023-06-18 22:58:55.749634 zit-0.0.3a0/zit/routes/dataset/categories.py
--rw-r--r--   0        0        0     3214 2023-06-18 21:57:11.118740 zit-0.0.3a0/zit/routes/dataset/images.py
--rw-r--r--   0        0        0     2346 2023-07-10 18:27:33.457549 zit-0.0.3a0/zit/routes/dataset/queries.py
--rw-r--r--   0        0        0      402 2023-06-16 09:25:23.231629 zit-0.0.3a0/zit/utils.py
--rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 zit-0.0.3a0/setup.py
--rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 zit-0.0.3a0/PKG-INFO
+-rw-r--r--   0        0        0     1018 2023-07-10 19:39:11.582000 zit-0.0.3a2/pyproject.toml
+-rw-r--r--   0        0        0       72 2022-01-10 03:44:16.795928 zit-0.0.3a2/zit/__init__.py
+-rw-r--r--   0        0        0     1544 2023-04-14 12:30:48.576605 zit-0.0.3a2/zit/auth.py
+-rw-r--r--   0        0        0      582 2023-07-07 04:26:24.431211 zit-0.0.3a2/zit/config.py
+-rw-r--r--   0        0        0     8607 2023-07-10 18:46:59.264897 zit-0.0.3a2/zit/dashboard.py
+-rw-r--r--   0        0        0       60 2023-06-15 21:58:13.307052 zit-0.0.3a2/zit/dataset/__init__.py
+-rw-r--r--   0        0        0      407 2023-05-11 08:42:13.675272 zit-0.0.3a2/zit/dataset/build.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:56:33.152907 zit-0.0.3a2/zit/dataset/classification.py
+-rw-r--r--   0        0        0     2029 2023-06-15 17:30:11.785818 zit-0.0.3a2/zit/dataset/convert.py
+-rw-r--r--   0        0        0     1577 2023-07-10 11:08:29.567160 zit-0.0.3a2/zit/dataset/detection.py
+-rw-r--r--   0        0        0      427 2023-05-11 07:24:56.576494 zit-0.0.3a2/zit/dataset/factory.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:37:14.408208 zit-0.0.3a2/zit/dataset/keypoints.py
+-rw-r--r--   0        0        0    15732 2023-07-10 11:03:37.537197 zit-0.0.3a2/zit/dataset/manager.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:37:56.638196 zit-0.0.3a2/zit/dataset/multilabel_classification.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:36:54.588213 zit-0.0.3a2/zit/dataset/segmentation.py
+-rw-r--r--   0        0        0    12010 2023-07-07 20:00:48.386764 zit-0.0.3a2/zit/formula.py
+-rw-r--r--   0        0        0      617 2023-04-16 19:16:58.258259 zit-0.0.3a2/zit/main.py
+-rw-r--r--   0        0        0      712 2023-07-10 11:09:05.807157 zit-0.0.3a2/zit/routes/__init__.py
+-rw-r--r--   0        0        0      520 2023-06-18 22:26:38.078376 zit-0.0.3a2/zit/routes/dataset/annotations.py
+-rw-r--r--   0        0        0      831 2023-06-18 22:58:55.749634 zit-0.0.3a2/zit/routes/dataset/categories.py
+-rw-r--r--   0        0        0     3214 2023-06-18 21:57:11.118740 zit-0.0.3a2/zit/routes/dataset/images.py
+-rw-r--r--   0        0        0     2312 2023-07-10 19:28:08.018745 zit-0.0.3a2/zit/routes/dataset/queries.py
+-rw-r--r--   0        0        0      402 2023-06-16 09:25:23.231629 zit-0.0.3a2/zit/utils.py
+-rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 zit-0.0.3a2/setup.py
+-rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 zit-0.0.3a2/PKG-INFO
```

### Comparing `zit-0.0.3a0/pyproject.toml` & `zit-0.0.3a2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zit"
-version = "0.0.3a0"
+version = "0.0.3a2"
 description = "ZitySpace CLI tool"
 authors = ["Rui Zheng <rui@zityspace.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 PyYAML = "^6.0"
@@ -46,10 +46,10 @@
 
 [tool.isort]
 profile = "black"
 skip = ["dist"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.0.3a0"
+version = "0.0.3a2"
 version_files = ["pyproject.toml:version"]
 tag_format = "v$version"
```

### Comparing `zit-0.0.3a0/zit/auth.py` & `zit-0.0.3a2/zit/auth.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a0/zit/config.py` & `zit-0.0.3a2/zit/config.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a0/zit/dashboard.py` & `zit-0.0.3a2/zit/dashboard.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,22 +72,14 @@
     try:
         run_subprocess(["npm", "-v"], capture_stdout=False)
         return True
     except FileNotFoundError:
         return False
 
 
-def has_rabbitmq():
-    try:
-        run_subprocess(["rabbitmqctl", "status"], capture_stdout=False)
-        return True
-    except FileNotFoundError:
-        return False
-
-
 def check_and_install_poetry():
     try:
         # Check if poetry is already installed
         run_subprocess(["poetry", "--version"], cwd=None, capture_stdout=False)
         logger.info("Poetry is already installed.")
     except FileNotFoundError:
         yes = typer.prompt("Poetry not found. Do you want to install it?", type=bool)
@@ -126,26 +118,14 @@
             run_subprocess(install_command, cwd=None, shell=True)
             logger.info("pnpm has been installed successfully.")
         except SubprocessError as e:
             logger.error("Error installing pnpm:")
             logger.error(e.stderr)
 
 
-def check_rabbitmq_service():
-    if not has_rabbitmq():
-        logger.info(
-            "RabbitMQ is not installed. Please install RabbitMQ manually, start rabbitmq-server service and re-run 'zit"
-            " dashboard install'."
-        )
-        return
-
-    # need a way to check if rabbitmq-server is running
-    pass
-
-
 def install_zlens_dependencies(path: Path):
     api_path = path / "api"
     ui_path = path / "ui"
 
     check_and_install_poetry()
     logger.info("Installing zlens API dependencies...")
     try:
@@ -163,16 +143,14 @@
     try:
         run_subprocess(["pnpm", "install"], cwd=str(ui_path))
     except SubprocessError as e:
         logger.error("Error installing zlens UI dependencies:")
         logger.error(e.stderr)
         sys.exit(1)
 
-    check_rabbitmq_service()
-
 
 def create_database_tables(path: Path):
     api_path = path / "api"
     venv_path = api_path / ".venv"
     python_executable = (
         venv_path / "bin" / "python" if sys.platform != "win32" else venv_path / "Scripts" / "python.exe"
     )
```

### Comparing `zit-0.0.3a0/zit/dataset/convert.py` & `zit-0.0.3a2/zit/dataset/convert.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a0/zit/dataset/detection.py` & `zit-0.0.3a2/zit/dataset/detection.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a0/zit/dataset/manager.py` & `zit-0.0.3a2/zit/dataset/manager.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a0/zit/formula.py` & `zit-0.0.3a2/zit/formula.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a0/zit/main.py` & `zit-0.0.3a2/zit/main.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a0/zit/routes/__init__.py` & `zit-0.0.3a2/zit/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a0/zit/routes/dataset/annotations.py` & `zit-0.0.3a2/zit/routes/dataset/annotations.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a0/zit/routes/dataset/categories.py` & `zit-0.0.3a2/zit/routes/dataset/categories.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a0/zit/routes/dataset/images.py` & `zit-0.0.3a2/zit/routes/dataset/images.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.3a0/zit/routes/dataset/queries.py` & `zit-0.0.3a2/zit/routes/dataset/queries.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         df["type"] = "keypoints"
 
     gdict = {"pd": pd, "ast": ast}
     ldict = {"df": df}
 
     if meta_serving:
         meta_df = manager.meta_df.copy()
-        meta_df["image_hash"] = meta_df["file_name"].apply(lambda fname: fname.split(".")[0])
+        meta_df.rename(columns={"file_name": "image_hash"})
         ldict["meta_df"] = meta_df
 
     @r.post("/queries", summary="Query the annotation dataframe")
     async def query_r(query: Query):
         with capture() as out:
             try:
                 exec(query.code, gdict, ldict)
```

### Comparing `zit-0.0.3a0/setup.py` & `zit-0.0.3a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'websocket-client>=1.5.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['zit = zit.main:app']}
 
 setup_kwargs = {
     'name': 'zit',
-    'version': '0.0.3a0',
+    'version': '0.0.3a2',
     'description': 'ZitySpace CLI tool',
     'long_description': 'None',
     'author': 'Rui Zheng',
     'author_email': 'rui@zityspace.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `zit-0.0.3a0/PKG-INFO` & `zit-0.0.3a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zit
-Version: 0.0.3a0
+Version: 0.0.3a2
 Summary: ZitySpace CLI tool
 License: MIT
 Author: Rui Zheng
 Author-email: rui@zityspace.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

