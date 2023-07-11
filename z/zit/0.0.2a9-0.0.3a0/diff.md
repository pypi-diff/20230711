# Comparing `tmp/zit-0.0.2a9.tar.gz` & `tmp/zit-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zit-0.0.2a9.tar", max compression
+gzip compressed data, was "zit-0.0.3a0.tar", max compression
```

## Comparing `zit-0.0.2a9.tar` & `zit-0.0.3a0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      986 2023-07-07 09:10:40.605729 zit-0.0.2a9/pyproject.toml
--rw-r--r--   0        0        0       72 2022-01-10 03:44:16.795928 zit-0.0.2a9/zit/__init__.py
--rw-r--r--   0        0        0     1544 2023-04-14 12:30:48.576605 zit-0.0.2a9/zit/auth.py
--rw-r--r--   0        0        0      582 2023-07-07 04:26:24.431211 zit-0.0.2a9/zit/config.py
--rw-r--r--   0        0        0     8184 2023-07-07 09:09:33.325754 zit-0.0.2a9/zit/dashboard.py
--rw-r--r--   0        0        0       60 2023-06-15 21:58:13.307052 zit-0.0.2a9/zit/dataset/__init__.py
--rw-r--r--   0        0        0      407 2023-05-11 08:42:13.675272 zit-0.0.2a9/zit/dataset/build.py
--rw-r--r--   0        0        0        0 2023-06-15 21:56:33.152907 zit-0.0.2a9/zit/dataset/classification.py
--rw-r--r--   0        0        0     2029 2023-06-15 17:30:11.785818 zit-0.0.2a9/zit/dataset/convert.py
--rw-r--r--   0        0        0     1363 2023-07-03 13:39:04.584358 zit-0.0.2a9/zit/dataset/detection.py
--rw-r--r--   0        0        0      427 2023-05-11 07:24:56.576494 zit-0.0.2a9/zit/dataset/factory.py
--rw-r--r--   0        0        0        0 2023-05-11 05:37:14.408208 zit-0.0.2a9/zit/dataset/keypoints.py
--rw-r--r--   0        0        0    15732 2023-06-18 22:35:18.479099 zit-0.0.2a9/zit/dataset/manager.py
--rw-r--r--   0        0        0        0 2023-05-11 05:37:56.638196 zit-0.0.2a9/zit/dataset/multilabel_classification.py
--rw-r--r--   0        0        0        0 2023-05-11 05:36:54.588213 zit-0.0.2a9/zit/dataset/segmentation.py
--rw-r--r--   0        0        0    10862 2023-07-07 05:43:26.259723 zit-0.0.2a9/zit/formula.py
--rw-r--r--   0        0        0      617 2023-04-16 19:16:58.258259 zit-0.0.2a9/zit/main.py
--rw-r--r--   0        0        0      670 2023-06-28 06:34:04.531830 zit-0.0.2a9/zit/routes/__init__.py
--rw-r--r--   0        0        0      520 2023-06-18 22:26:38.078376 zit-0.0.2a9/zit/routes/dataset/annotations.py
--rw-r--r--   0        0        0      831 2023-06-18 22:58:55.749634 zit-0.0.2a9/zit/routes/dataset/categories.py
--rw-r--r--   0        0        0     3214 2023-06-18 21:57:11.118740 zit-0.0.2a9/zit/routes/dataset/images.py
--rw-r--r--   0        0        0     2126 2023-06-28 09:53:59.159211 zit-0.0.2a9/zit/routes/dataset/queries.py
--rw-r--r--   0        0        0      402 2023-06-16 09:25:23.231629 zit-0.0.2a9/zit/utils.py
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 zit-0.0.2a9/setup.py
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 zit-0.0.2a9/PKG-INFO
+-rw-r--r--   0        0        0     1018 2023-07-10 18:29:27.055868 zit-0.0.3a0/pyproject.toml
+-rw-r--r--   0        0        0       72 2022-01-10 03:44:16.795928 zit-0.0.3a0/zit/__init__.py
+-rw-r--r--   0        0        0     1544 2023-04-14 12:30:48.576605 zit-0.0.3a0/zit/auth.py
+-rw-r--r--   0        0        0      582 2023-07-07 04:26:24.431211 zit-0.0.3a0/zit/config.py
+-rw-r--r--   0        0        0     9138 2023-07-07 12:56:08.546696 zit-0.0.3a0/zit/dashboard.py
+-rw-r--r--   0        0        0       60 2023-06-15 21:58:13.307052 zit-0.0.3a0/zit/dataset/__init__.py
+-rw-r--r--   0        0        0      407 2023-05-11 08:42:13.675272 zit-0.0.3a0/zit/dataset/build.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:56:33.152907 zit-0.0.3a0/zit/dataset/classification.py
+-rw-r--r--   0        0        0     2029 2023-06-15 17:30:11.785818 zit-0.0.3a0/zit/dataset/convert.py
+-rw-r--r--   0        0        0     1577 2023-07-10 11:08:29.567160 zit-0.0.3a0/zit/dataset/detection.py
+-rw-r--r--   0        0        0      427 2023-05-11 07:24:56.576494 zit-0.0.3a0/zit/dataset/factory.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:37:14.408208 zit-0.0.3a0/zit/dataset/keypoints.py
+-rw-r--r--   0        0        0    15732 2023-07-10 11:03:37.537197 zit-0.0.3a0/zit/dataset/manager.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:37:56.638196 zit-0.0.3a0/zit/dataset/multilabel_classification.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:36:54.588213 zit-0.0.3a0/zit/dataset/segmentation.py
+-rw-r--r--   0        0        0    12010 2023-07-07 20:00:48.386764 zit-0.0.3a0/zit/formula.py
+-rw-r--r--   0        0        0      617 2023-04-16 19:16:58.258259 zit-0.0.3a0/zit/main.py
+-rw-r--r--   0        0        0      712 2023-07-10 11:09:05.807157 zit-0.0.3a0/zit/routes/__init__.py
+-rw-r--r--   0        0        0      520 2023-06-18 22:26:38.078376 zit-0.0.3a0/zit/routes/dataset/annotations.py
+-rw-r--r--   0        0        0      831 2023-06-18 22:58:55.749634 zit-0.0.3a0/zit/routes/dataset/categories.py
+-rw-r--r--   0        0        0     3214 2023-06-18 21:57:11.118740 zit-0.0.3a0/zit/routes/dataset/images.py
+-rw-r--r--   0        0        0     2346 2023-07-10 18:27:33.457549 zit-0.0.3a0/zit/routes/dataset/queries.py
+-rw-r--r--   0        0        0      402 2023-06-16 09:25:23.231629 zit-0.0.3a0/zit/utils.py
+-rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 zit-0.0.3a0/setup.py
+-rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 zit-0.0.3a0/PKG-INFO
```

### Comparing `zit-0.0.2a9/pyproject.toml` & `zit-0.0.3a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "zit"
-version = "0.0.2a9"
+version = "0.0.3a0"
 description = "ZitySpace CLI tool"
 authors = ["Rui Zheng <rui@zityspace.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 PyYAML = "^6.0"
 typer = {extras = ["all"], version = "^0.7.0"}
-httpx = "^0.24.0"
+httpx = {extras = ["socks"], version = "^0.24.1"}
 websocket-client = "^1.5.1"
 fastapi = "^0.95.1"
 pandas = "^2.0.2"
 duckdb = "^0.8.1"
 pillow = "^9.5.0"
 python-multipart = "^0.0.6"
 
@@ -46,10 +46,10 @@
 
 [tool.isort]
 profile = "black"
 skip = ["dist"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.0.2a9"
+version = "0.0.3a0"
 version_files = ["pyproject.toml:version"]
 tag_format = "v$version"
```

### Comparing `zit-0.0.2a9/zit/auth.py` & `zit-0.0.3a0/zit/auth.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a9/zit/config.py` & `zit-0.0.3a0/zit/config.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a9/zit/dashboard.py` & `zit-0.0.3a0/zit/dashboard.py`

 * *Files 14% similar despite different names*

```diff
@@ -72,14 +72,22 @@
     try:
         run_subprocess(["npm", "-v"], capture_stdout=False)
         return True
     except FileNotFoundError:
         return False
 
 
+def has_rabbitmq():
+    try:
+        run_subprocess(["rabbitmqctl", "status"], capture_stdout=False)
+        return True
+    except FileNotFoundError:
+        return False
+
+
 def check_and_install_poetry():
     try:
         # Check if poetry is already installed
         run_subprocess(["poetry", "--version"], cwd=None, capture_stdout=False)
         logger.info("Poetry is already installed.")
     except FileNotFoundError:
         yes = typer.prompt("Poetry not found. Do you want to install it?", type=bool)
@@ -118,14 +126,26 @@
             run_subprocess(install_command, cwd=None, shell=True)
             logger.info("pnpm has been installed successfully.")
         except SubprocessError as e:
             logger.error("Error installing pnpm:")
             logger.error(e.stderr)
 
 
+def check_rabbitmq_service():
+    if not has_rabbitmq():
+        logger.info(
+            "RabbitMQ is not installed. Please install RabbitMQ manually, start rabbitmq-server service and re-run 'zit"
+            " dashboard install'."
+        )
+        return
+
+    # need a way to check if rabbitmq-server is running
+    pass
+
+
 def install_zlens_dependencies(path: Path):
     api_path = path / "api"
     ui_path = path / "ui"
 
     check_and_install_poetry()
     logger.info("Installing zlens API dependencies...")
     try:
@@ -143,14 +163,16 @@
     try:
         run_subprocess(["pnpm", "install"], cwd=str(ui_path))
     except SubprocessError as e:
         logger.error("Error installing zlens UI dependencies:")
         logger.error(e.stderr)
         sys.exit(1)
 
+    check_rabbitmq_service()
+
 
 def create_database_tables(path: Path):
     api_path = path / "api"
     venv_path = api_path / ".venv"
     python_executable = (
         venv_path / "bin" / "python" if sys.platform != "win32" else venv_path / "Scripts" / "python.exe"
     )
@@ -180,26 +202,35 @@
 
 
 def start_api_service(api_path: Path, port: int):
     venv_path = api_path / ".venv"
     python_executable = (
         venv_path / "bin" / "python" if sys.platform != "win32" else venv_path / "Scripts" / "python.exe"
     )
+
+    env = os.environ.copy()
+    env.pop("http_proxy", None)
+    env.pop("https_proxy", None)
+    env.pop("all_proxy", None)
+    env.pop("HTTP_PROXY", None)
+    env.pop("HTTPS_PROXY", None)
+    env.pop("ALL_PROXY", None)
+
     command = [
         str(python_executable),
         "-m",
         "uvicorn",
         "app.api.serv:app",
         "--host",
         "0.0.0.0",
         "--port",
         str(port),
         "--reload",
     ]
-    return run_subprocess(command, cwd=str(api_path), capture_stdout=True, wait=False)
+    return run_subprocess(command, cwd=str(api_path), capture_stdout=True, env=env, wait=False)
 
 
 def start_ui_service(ui_path: Path, port: int, api_port: Optional[int] = None):
     env = os.environ.copy()
     env["PORT"] = str(port)
 
     if api_port:
@@ -214,14 +245,20 @@
     python_executable = (
         venv_path / "bin" / "python" if sys.platform != "win32" else venv_path / "Scripts" / "python.exe"
     )
 
     # ensure that the python executable used in the subprocess is the one from zlens api venv
     # otherwise, it will be the one from the current activated venv
     env = os.environ.copy()
+    env.pop("http_proxy", None)
+    env.pop("https_proxy", None)
+    env.pop("all_proxy", None)
+    env.pop("HTTP_PROXY", None)
+    env.pop("HTTPS_PROXY", None)
+    env.pop("ALL_PROXY", None)
     env["PATH"] = str(venv_path / "bin") + os.pathsep + env["PATH"]
 
     command = [
         str(python_executable),
         "-m",
         "celery",
         "-A",
```

### Comparing `zit-0.0.2a9/zit/dataset/convert.py` & `zit-0.0.3a0/zit/dataset/convert.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a9/zit/dataset/detection.py` & `zit-0.0.3a0/zit/dataset/detection.py`

 * *Files 19% similar despite different names*

```diff
@@ -29,15 +29,23 @@
         else:
             manage_root = str(zit_root / ".zit" / "manager" / hash_)
             os.makedirs(manage_root, exist_ok=True)
             manager = Manager(manage_root, "detection", dataframe_serving=True)
             manager.add_metas(image_source, for_init=True)
             manager.add_annotations(annotation_source, for_init=True)
 
-            dataset = {"params": params, "router": build_default_router(params, manager)}
+            meta_serving = kwargs.get("meta_serving", False)
+            dataset = {
+                "params": params,
+                "router": build_default_router(
+                    params,
+                    manager,
+                    meta_serving=meta_serving,
+                ),
+            }
 
             self._datasets[hash_] = dataset
 
         return dataset
 
 
 DatasetFactory.register("detection", DetectionDatasetBuilder())
```

### Comparing `zit-0.0.2a9/zit/dataset/manager.py` & `zit-0.0.3a0/zit/dataset/manager.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a9/zit/formula.py` & `zit-0.0.3a0/zit/formula.py`

 * *Files 13% similar despite different names*

```diff
@@ -342,7 +342,48 @@
         else:
             sql = f"UPDATE formulas SET {' = ?, '.join(list(formula.keys()))} = ? WHERE id = ?"
             cur.execute(sql, list(formula.values()) + [rec[0]])
 
     conn.close()
 
     logger.info("done :)")
+
+
+@app.command(name="delete", help="Delete formula")
+def delete(name: str):
+    zit_root = find_zit_root(Path.cwd())
+    formula_path = zit_root / ".zit" / "formulas" / name
+
+    if not formula_path.is_dir():
+        logger.warning(f"{name} not installed.")
+        return
+
+    # confirm deletion
+    if input(f"Are you sure you want to delete {name}? [y/N]: ").lower() != "y":
+        return
+
+    logger.info(f"deleting: {name}")
+
+    # delete formula
+    shutil.rmtree(formula_path)
+
+    # update database
+    db = zit_root / ".zit" / "zit.sqlite"
+    conn = sqlite3.connect(db)
+    creator, slug = name.split("/")
+    with conn:
+        cur = conn.cursor()
+
+        cur.execute("SELECT * FROM formulas WHERE creator=? AND slug=?", (creator, slug))
+        rec = cur.fetchone()
+        if rec is not None:
+            cur.execute("DELETE FROM formulas WHERE id=?", (rec[0],))
+            cur.execute("DELETE FROM instances WHERE formula_id=?", (rec[0],))
+
+    conn.close()
+
+    # delete log
+    log_file = zit_root / ".zit" / "logs" / f"{creator}" / f"{slug}.log"
+    if log_file.exists():
+        os.remove(log_file)
+
+    logger.info("done :)")
```

### Comparing `zit-0.0.2a9/zit/main.py` & `zit-0.0.3a0/zit/main.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a9/zit/routes/__init__.py` & `zit-0.0.3a0/zit/routes/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from ..dataset.manager import Manager
 from .dataset.annotations import build_annotations_router
 from .dataset.categories import build_categories_router
 from .dataset.images import build_images_router
 from .dataset.queries import build_queries_router
 
 
-def build_default_router(params, manager: Manager):
+def build_default_router(params, manager: Manager, meta_serving: bool = False):
     r = APIRouter(prefix="/default")
 
     r.include_router(build_images_router(params, manager))
     r.include_router(build_annotations_router(params, manager))
     r.include_router(build_categories_router(params, manager))
-    r.include_router(build_queries_router(params, manager))
+    r.include_router(build_queries_router(params, manager, meta_serving))
 
     return r
 
 
 __all__ = ["build_default_router"]
```

### Comparing `zit-0.0.2a9/zit/routes/dataset/annotations.py` & `zit-0.0.3a0/zit/routes/dataset/annotations.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a9/zit/routes/dataset/categories.py` & `zit-0.0.3a0/zit/routes/dataset/categories.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a9/zit/routes/dataset/images.py` & `zit-0.0.3a0/zit/routes/dataset/images.py`

 * *Files identical despite different names*

### Comparing `zit-0.0.2a9/zit/routes/dataset/queries.py` & `zit-0.0.3a0/zit/routes/dataset/queries.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         yield out
     finally:
         sys.stdout, sys.stderr = oldout, olderr
         out[0] = out[0].getvalue()
         out[1] = out[1].getvalue()
 
 
-def build_queries_router(params, manager: Manager):
+def build_queries_router(params, manager: Manager, meta_serving: bool = False):
     queries_router = r = APIRouter(tags=["Dataset: Dataframe queries"])
 
     df = manager.anno_df.copy()
 
     if manager.task == "detection":
         df["type"] = "box"
 
@@ -41,14 +41,19 @@
 
     elif manager.task == "keypoints_detection":
         df["type"] = "keypoints"
 
     gdict = {"pd": pd, "ast": ast}
     ldict = {"df": df}
 
+    if meta_serving:
+        meta_df = manager.meta_df.copy()
+        meta_df["image_hash"] = meta_df["file_name"].apply(lambda fname: fname.split(".")[0])
+        ldict["meta_df"] = meta_df
+
     @r.post("/queries", summary="Query the annotation dataframe")
     async def query_r(query: Query):
         with capture() as out:
             try:
                 exec(query.code, gdict, ldict)
             except Exception as e:
                 raise HTTPException(status_code=409, detail=str(e))
```

### Comparing `zit-0.0.2a9/setup.py` & `zit-0.0.3a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'duckdb>=0.8.1,<0.9.0',
  'fastapi>=0.95.1,<0.96.0',
- 'httpx>=0.24.0,<0.25.0',
+ 'httpx[socks]>=0.24.1,<0.25.0',
  'pandas>=2.0.2,<3.0.0',
  'pillow>=9.5.0,<10.0.0',
  'python-multipart>=0.0.6,<0.0.7',
  'typer[all]>=0.7.0,<0.8.0',
  'websocket-client>=1.5.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['zit = zit.main:app']}
 
 setup_kwargs = {
     'name': 'zit',
-    'version': '0.0.2a9',
+    'version': '0.0.3a0',
     'description': 'ZitySpace CLI tool',
     'long_description': 'None',
     'author': 'Rui Zheng',
     'author_email': 'rui@zityspace.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `zit-0.0.2a9/PKG-INFO` & `zit-0.0.3a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: zit
-Version: 0.0.2a9
+Version: 0.0.3a0
 Summary: ZitySpace CLI tool
 License: MIT
 Author: Rui Zheng
 Author-email: rui@zityspace.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: duckdb (>=0.8.1,<0.9.0)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: httpx[socks] (>=0.24.1,<0.25.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Requires-Dist: websocket-client (>=1.5.1,<2.0.0)
```

