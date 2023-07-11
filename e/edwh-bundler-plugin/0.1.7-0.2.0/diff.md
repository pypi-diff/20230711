# Comparing `tmp/edwh_bundler_plugin-0.1.7.tar.gz` & `tmp/edwh_bundler_plugin-0.2.0.tar.gz`

## Comparing `edwh_bundler_plugin-0.1.7.tar` & `edwh_bundler_plugin-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/CHANGELOG.md
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/bundle.yaml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/__init__.py
--rw-r--r--   0        0        0    20717 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/bundler_plugin.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/css.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/js.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/shared.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/README.md
--rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.2.0/bundle.toml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.2.0/bundle.yaml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.2.0/src/edwh_bundler_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.2.0/src/edwh_bundler_plugin/__init__.py
+-rw-r--r--   0        0        0    23843 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.2.0/src/edwh_bundler_plugin/bundler_plugin.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.2.0/src/edwh_bundler_plugin/css.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.2.0/src/edwh_bundler_plugin/js.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.2.0/src/edwh_bundler_plugin/shared.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.2.0/README.md
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.2.0/PKG-INFO
```

### Comparing `edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/bundler_plugin.py` & `edwh_bundler_plugin-0.2.0/src/edwh_bundler_plugin/bundler_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import warnings
 from contextlib import contextmanager
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 
 import invoke
+import tomlkit
 import yaml
 from invoke import task, Context
 from dotenv import load_dotenv
 from shutil import rmtree
 
 from .css import extract_contents_for_css
 from .js import extract_contents_for_js
@@ -35,25 +36,79 @@
 DEFAULT_OUTPUT_CSS = "bundle.css"
 TEMP_OUTPUT_DIR = "/tmp/bundle-build/"
 TEMP_OUTPUT = ".bundle_tmp"
 DEFAULT_ASSETS_DB = "/tmp/lts_assets.db"
 DEFAULT_ASSETS_SQL = "py4web/apps/lts/databases/lts_assets.sql"
 
 
-def load_config(fname: str = DEFAULT_INPUT, strict=False) -> dict:
+def convert_data(data: dict[str, typing.Any] | list[typing.Any] | typing.Any):
+    """
+    Recursively replace "-" in keys to "_"
+    """
+    if isinstance(data, dict):
+        return {key.replace("-", "_"): convert_data(value) for key, value in data.items()}
+    elif isinstance(data, list):
+        return [convert_data(value) for value in data]
+    else:
+        # normal value, don't change!
+        return data
+
+
+def _load_config_yaml(fname: str):
+    with open(fname) as f:
+        data = yaml.load(f, yaml.Loader)
+
+    return convert_data(data)
+
+
+def _load_config_toml(fname: str, key: str = ""):
+    with open(fname) as f:
+        data = tomlkit.load(f)
+
+    if key:
+        for part in key.split("."):
+            data = data.get(part)
+            if data is None:
+                # key not found in toml!
+                return {}
+
+    return convert_data(data)
+
+
+def _load_config(fname: str = DEFAULT_INPUT, strict=False) -> tuple[str, dict]:
     """
     Load yaml config from file name, default to empty or error if strict
     """
-    if os.path.exists(fname):
-        with open(fname) as f:
-            return yaml.load(f, yaml.Loader)
+    if os.path.exists(fname) and fname.endswith((".yml", ".yaml")):
+        # load default or user-defined yaml
+        return fname, _load_config_yaml(fname)
+    elif os.path.exists(fname) and fname.endswith(".toml"):
+        # load user defined toml
+        return fname, _load_config_toml(fname)
+    elif fname == DEFAULT_INPUT and (altname := DEFAULT_INPUT.replace(".yaml", ".toml")) and os.path.exists(altname):
+        # try bundle.toml
+        return altname, _load_config_toml(altname)
+    elif (altname := "pyproject.toml") and os.path.exists(altname):
+        # look in pyproject
+        return altname, _load_config_toml(altname, key="tool.edwh.bundle")
     elif strict:
+        # err !
         raise FileNotFoundError(fname)
     else:
-        return {}
+        # fallback to empty config
+        return "", {}
+
+
+def load_config(fname: str = DEFAULT_INPUT, strict=True) -> dict:
+    file_used, data = _load_config(fname, strict=strict)
+    if not data and strict:
+        # empty config!
+        raise ValueError(f"Config data found for `{file_used}` was empty!")
+
+    return data or {}
 
 
 @contextmanager
 def start_buffer(temp: str | typing.IO = TEMP_OUTPUT) -> typing.IO:
     """
     Open a temp buffer file in append mode and first remove old version if that exists
     """
@@ -74,19 +129,19 @@
     try:
         yield f
     finally:
         f.close()
 
 
 def cli_or_config(
-    value: typing.Any,
-    config: dict,
-    key: typing.Hashable,
-    bool: bool = True,
-    default: typing.Any = None,
+        value: typing.Any,
+        config: dict,
+        key: typing.Hashable,
+        bool: bool = True,
+        default: typing.Any = None,
 ) -> bool | typing.Any:
     """
     Get a setting from either the config yaml or the cli (used to override config)
     cli > config > default
 
     Args:
         value: the value from cli, will override config if anything other than None
@@ -135,22 +190,33 @@
 def _regexify_settings(setting_dict: dict[str, typing.Any]) -> dict[re.Pattern, typing.Any]:
     """
     Convert a dict keys from string to a compiled regex pattern (/$string/)
     """
     return {re.compile(rf"\${key}"): value for key, value in setting_dict.items()}
 
 
+def store_file_hash(input_filename: str, output_filename: str = None):
+    if output_filename is None:
+        output_filename = f"{input_filename}.hash"
+    c = Context()
+    file_hash = calculate_file_hash(c, input_filename)
+    with open(output_filename, "w") as f:
+        f.write(file_hash)
+    return output_filename
+
+
 def _handle_files(
-    files: list,
-    callback: typing.Callable,
-    output: str | typing.IO,
-    verbose: bool,
-    cache: bool,
-    minify: bool,
-    settings: dict,
+        files: list,
+        callback: typing.Callable,
+        output: str | typing.IO,
+        verbose: bool,
+        cache: bool,
+        minify: bool,
+        hash: bool,
+        settings: dict,
 ):
     """
     Execute 'callback' (js or css specific) on all 'files'
 
     Args:
         files: list of files from the 'css' or 'js' section in the config yaml
         callback: method to execute to gather and process file contents
@@ -166,14 +232,15 @@
     files = [_fill_variables(f, re_settings) for f in files]
 
     if verbose:
         print(
             f"Building {callback.__name__.split('_')[-1]} [verbose]\n" f"{output=}\n",
             f"{minify=}\n",
             f"{cache=}\n",
+            f"{hash=}\n",
             f"{files=}\n",
             file=sys.stderr,
         )
 
     if not files:
         if verbose:
             print("No files supplied, quitting", file=sys.stderr)
@@ -196,29 +263,34 @@
                 print(f"Handled {inf}", file=sys.stderr)
 
     if not isinstance(output, io.IOBase):
         os.rename(bufferf.name, output)
     if verbose:
         print(f"Written final bundle to {output}", file=sys.stderr)
 
+    if hash:
+        hash_file = store_file_hash(output)
+        return (output, hash_file)
+
     return output
 
 
 @task(iterable=["files"])
 def build_js(
-    c,
-    files=None,
-    input=DEFAULT_INPUT,
-    verbose=False,
-    # overrule config:
-    output=None,  # DEFAULT_OUTPUT_JS
-    minify=None,
-    cache=None,
-    version=None,
-    stdout=False,  # overrides output
+        c,
+        files=None,
+        input=DEFAULT_INPUT,
+        verbose=False,
+        # overrule config:
+        output=None,  # DEFAULT_OUTPUT_JS
+        minify=None,
+        cache=None,
+        hash=None,
+        version=None,
+        stdout=False,  # overrides output
 ):
     """
     Build the JS bundle (cli only)
     """
     config = load_config(input)
 
     files = files or config.get("js")
@@ -226,37 +298,41 @@
     if not files:
         raise NotFound("js")
 
     settings = config.get("config", {})
 
     minify = cli_or_config(minify, settings, "minify")
     cache = cli_or_config(cache, settings, "cache", default=True)
+    hash = cli_or_config(hash, settings, "hash")
+
     output = sys.stdout if stdout else cli_or_config(output, settings, "output_js", bool=False) or DEFAULT_OUTPUT_JS
 
     settings["version"] = cli_or_config(version, settings, "version", bool=False, default="latest")
 
     return _handle_files(
         files,
         extract_contents_for_js,
         output,
         verbose=verbose,
         cache=cache,
+        hash=hash,
         minify=minify,
         settings=settings,
     )
 
 
 # import version:
 def bundle_js(
-    files: list = None,
-    verbose: bool = False,
-    output: str | typing.IO = None,
-    minify: bool = True,
-    cache: bool = True,
-    **settings,
+        files: list = None,
+        verbose: bool = False,
+        output: str | typing.IO = None,
+        minify: bool = True,
+        cache: bool = True,
+        hash: bool = False,
+        **settings,
 ) -> typing.Optional[str]:
     """
     Importable version of 'build_js'.
     If output is left as None, the bundled code will be returned as a string
 
     Args:
         files: list of things to bundle
@@ -272,14 +348,15 @@
 
     _handle_files(
         files,
         extract_contents_for_js,
         output,
         verbose=verbose,
         cache=cache,
+        hash=hash,
         minify=minify,
         settings=settings,
     )
 
     if not isinstance(output, io.StringIO):
         return output
 
@@ -291,125 +368,138 @@
 class NotFound(Exception):
     type: typing.Literal["js", "css"]
 
     def __str__(self):
         return f"Please specify either --files or the {self.type} key in a config yaml (e.g. bundle.yaml)"
 
 
-@task(iterable=["files"])
+@task(iterable=["files"], )
 def build_css(
-    c,
-    files=None,
-    input=DEFAULT_INPUT,
-    verbose=False,
-    # overrule config:
-    output=None,  # DEFAULT_OUTPUT_CSS
-    minify=None,
-    cache=None,
-    version=None,
-    stdout=False,  # overrides output
+        c,
+        files=None,
+        input=DEFAULT_INPUT,
+        verbose=False,
+        # overrule config:
+        output=None,  # DEFAULT_OUTPUT_CSS
+        minify=None,
+        cache=None,
+        hash=None,
+        version=None,
+        stdout=False,  # overrides output
 ):
     """
     Build the CSS bundle (cli only)
     """
     config = load_config(input)
     settings = config.get("config", {})
 
     minify = cli_or_config(minify, settings, "minify")
     cache = cli_or_config(cache, settings, "cache", default=True)
+    hash = cli_or_config(hash, settings, "hash")
 
     settings["version"] = cli_or_config(version, settings, "version", bool=False, default="latest")
 
     output = sys.stdout if stdout else cli_or_config(output, settings, "output_css", bool=False) or DEFAULT_OUTPUT_CSS
 
     if not (files := (files or config.get("css"))):
         raise NotFound("css")
 
     return _handle_files(
         files,
         extract_contents_for_css,
         output,
         verbose=verbose,
         cache=cache,
+        hash=hash,
         minify=minify,
         settings=settings,
     )
 
 
 # import version:
 def bundle_css(
-    files: list = None,
-    verbose: bool = False,
-    output: str | typing.IO = None,
-    minify: bool = True,
-    cache: bool = True,
-    **settings,
+        files: list = None,
+        verbose: bool = False,
+        output: str | typing.IO = None,
+        minify: bool = True,
+        cache: bool = True,
+        hash: bool = False,
+        **settings,
 ) -> typing.Optional[str]:
     """
     Importable version of 'build_css'.
     If output is left as None, the bundled code will be returned as a string
 
     Args:
         files: list of things to bundle
         verbose: print some info to stderr?
         output: filepath or IO to write to
         minify: minify files?
         cache: save external files to disk for re-use?
+        hash: should an additional .hash file be stored after generating the bundle?
 
     Returns: bundle of CSS
     """
     if output is None:
         output = io.StringIO()
 
     _handle_files(
         files,
         extract_contents_for_css,
         output,
         verbose=verbose,
         cache=cache,
+        hash=hash,
         minify=minify,
         settings=settings,
     )
 
     if not isinstance(output, io.StringIO):
         return output
 
     output.seek(0)
     return output.read()
 
 
 @task(iterable=["files"])
 def build(
-    c,
-    input=DEFAULT_INPUT,
-    verbose=False,
-    # defaults from config, can be overwritten:
-    output_js=None,  # DEFAULT_OUTPUT_JS
-    output_css=None,  # DEFAULT_OUTPUT_CSS
-    minify=None,
-    cache=None,
-    version=None,
+        c,
+        input=DEFAULT_INPUT,
+        verbose=False,
+        # defaults from config, can be overwritten:
+        output_js=None,  # DEFAULT_OUTPUT_JS
+        output_css=None,  # DEFAULT_OUTPUT_CSS
+        minify=None,
+        cache=None,
+        hash=None,
+        version=None,
 ):
     """
     Build the JS and CSS bundle
     """
     # invoke build
 
+    settings = load_config(input).get("config", {})
+
+    minify = cli_or_config(minify, settings, "minify")
+    cache = cli_or_config(cache, settings, "cache", default=True)
+    hash = cli_or_config(hash, settings, "hash")
+
     # second argument of build_ is None, so files will be loaded from config.
     # --files can be supplied for the build-js or build-css methods, but not for normal build
     # since it would be too ambiguous to determine whether the files should be compiled as JS or CSS.
     result = []
     try:
-        result.append(build_js(c, None, input, verbose, output_js, minify, cache, version))
+        result.append(build_js(c, None, input, verbose, output_js, minify, cache, hash, version))
     except NotFound as e:
         warnings.warn(str(e), source=e)
 
     try:
         result.append(
-            build_css(c, None, input, verbose, output_css, minify, cache, version),
+            build_css(c, None, input, verbose, output_css, minify, cache, hash, version),
         )
     except NotFound as e:
         warnings.warn(str(e), source=e)
 
     print(result)
     return result
 
@@ -571,25 +661,25 @@
 
 def calculate_file_hash(c: Context, filename: str):
     return c.run(f"sha1sum {filename}", hide=True).stdout.split(" ")[0]
 
 
 @task()
 def publish(
-    c,
-    version=None,
-    major=False,
-    minor=False,
-    patch=False,
-    filename=None,
-    js=True,
-    css=True,
-    verbose=False,
-    config=DEFAULT_INPUT_LTS,
-    force=False,
+        c,
+        version=None,
+        major=False,
+        minor=False,
+        patch=False,
+        filename=None,
+        js=True,
+        css=True,
+        verbose=False,
+        config=DEFAULT_INPUT_LTS,
+        force=False,
 ):
     c: invoke.context.Context
     db = setup_db(c)
     previous = get_latest_version(db, "js")
 
     if not os.path.exists(TEMP_OUTPUT_DIR):
         os.mkdir(TEMP_OUTPUT_DIR)
@@ -686,15 +776,15 @@
     return True, file_hash, filename, file_contents
 
 
 @task(name="list")
 def list_versions(c):
     db = setup_db(c)
     for row in db.execute(
-        "SELECT filetype, version FROM bundle_version ORDER BY major DESC, minor DESC, patch DESC"
+            "SELECT filetype, version FROM bundle_version ORDER BY major DESC, minor DESC, patch DESC"
     ).fetchall():
         print(row)
 
 
 @task()
 def reset(c):
     db = setup_db(c)
@@ -706,15 +796,14 @@
     # ^ that's the whole point of 'reset'.
     db.execute("DELETE FROM bundle_version;")
     db.commit()
     _update_assets_sql(c)
 
     assert db.execute("SELECT COUNT(*) as c FROM bundle_version;").fetchone()["c"] == 0
 
-
 # DEV:
 
 #
 # @task
 # def update_dependencies(c):
 #     # invoke update-dependencies
 #     c.run("pip-compile requirements.in")
```

### Comparing `edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/css.py` & `edwh_bundler_plugin-0.2.0/src/edwh_bundler_plugin/css.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/js.py` & `edwh_bundler_plugin-0.2.0/src/edwh_bundler_plugin/js.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/shared.py` & `edwh_bundler_plugin-0.2.0/src/edwh_bundler_plugin/shared.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.7/LICENSE.txt` & `edwh_bundler_plugin-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.7/README.md` & `edwh_bundler_plugin-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.7/pyproject.toml` & `edwh_bundler_plugin-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -7,44 +7,61 @@
 dynamic = ["version"]
 description = 'Python-only static file (js, css) bundler for `edwh`'
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
 keywords = []
 authors = [
-  { name = "Robin van der Noord", email = "robin.vdn@educationwarehouse.nl" },
-  { name = "Remco Boerma", email = "remco.b@educationwarehouse.nl" },
+    { name = "Robin van der Noord", email = "robin.vdn@educationwarehouse.nl" },
+    { name = "Remco Boerma", email = "remco.b@educationwarehouse.nl" },
 ]
 classifiers = [
-  "Development Status :: 4 - Beta",
-  "Programming Language :: Python",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: 3.12",
-  "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
+    "Development Status :: 4 - Beta",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ['invoke', 'python-dotenv', 'pysass', 'rjsmin', 'httpx', 'pyyaml']
 
 [project.optional-dependencies]
 dev = [
-  "hatch",
-  # "python-semantic-release",
-  "black",
+    "hatch",
+    # "python-semantic-release",
+    "black",
 ]
 
 [project.urls]
 Documentation = "https://github.com/educationwarehouse/edwh-bundler-plugin#readme"
 Issues = "https://github.com/educationwarehouse/edwh-bundler-plugin/issues"
 Source = "https://github.com/educationwarehouse/edwh-bundler-plugin"
 
 # https://packaging.python.org/en/latest/guides/creating-and-discovering-plugins/#using-package-metadata
 [project.entry-points."edwh.tasks"]
 bundle = "edwh_bundler_plugin.bundler_plugin"
 
+[tool.edwh.bundle]
+js = [
+    "https://unpkg.com/htmx.org@1.9.2/dist/htmx.min.js"
+]
+
+css = [
+    "https://cdn.jsdelivr.net/npm/bulma@0.9.4/css/bulma.min.css"
+]
+
+[tool.edwh.bundle.config]
+minify = true
+filename = "bundled"
+output-css = "static/css/$filename-$version.css"
+output_js = "static/js/$filename-$version.js"
+hash = true
+
+
 [tool.hatch.version]
 path = "src/edwh_bundler_plugin/__about__.py"
 
 [tool.semantic_release]
 branch = "master"
 version_variable = "src/edwh_bundler_plugin/__about__.py:__version__"
 change_log = "CHANGELOG.md"
@@ -53,109 +70,109 @@
 build_command = "hatch build"
 
 parser_angular_minor_types = "feat,minor"
 parser_angular_patch_types = "fix,perf,refactor,build,chore,patch"
 
 [tool.hatch.envs.default]
 dependencies = [
-  "coverage[toml]>=6.5",
-  "pytest",
+    "coverage[toml]>=6.5",
+    "pytest",
 ]
 [tool.hatch.envs.default.scripts]
 publish = [
-  'semantic-release publish',
-  'hatch build -c',
-  'hatch publish',
+    'semantic-release publish',
+    'hatch build -c',
+    'hatch publish',
 ]
 
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
-  "- coverage combine",
-  "coverage report",
+    "- coverage combine",
+    "coverage report",
 ]
 cov = [
-  "test-cov",
-  "cov-report",
+    "test-cov",
+    "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
-  "black>=23.1.0",
-  "mypy>=1.0.0",
-  "ruff>=0.0.243",
+    "black>=23.1.0",
+    "mypy>=1.0.0",
+    "ruff>=0.0.243",
 ]
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:src/edwh_bundler_plugin tests}"
 style = [
-  "ruff {args:.}",
-  "black --check --diff {args:.}",
+    "ruff {args:.}",
+    "black --check --diff {args:.}",
 ]
 fmt = [
-  "black {args:.}",
-  "ruff --fix {args:.}",
-  "style",
+    "black {args:.}",
+    "ruff --fix {args:.}",
+    "style",
 ]
 all = [
-  "style",
-  "typing",
+    "style",
+    "typing",
 ]
 
 [tool.black]
 target-version = ["py37"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
 target-version = "py37"
 line-length = 120
 select = [
-  "A",
-  "ARG",
-  "B",
-  "C",
-  "DTZ",
-  "E",
-  "EM",
-  "F",
-  "FBT",
-  "I",
-  "ICN",
-  "ISC",
-  "N",
-  "PLC",
-  "PLE",
-  "PLR",
-  "PLW",
-  "Q",
-  "RUF",
-  "S",
-  "T",
-  "TID",
-  "UP",
-  "W",
-  "YTT",
+    "A",
+    "ARG",
+    "B",
+    "C",
+    "DTZ",
+    "E",
+    "EM",
+    "F",
+    "FBT",
+    "I",
+    "ICN",
+    "ISC",
+    "N",
+    "PLC",
+    "PLE",
+    "PLR",
+    "PLW",
+    "Q",
+    "RUF",
+    "S",
+    "T",
+    "TID",
+    "UP",
+    "W",
+    "YTT",
 ]
 ignore = [
-  # Allow non-abstract empty methods in abstract base classes
-  "B027",
-  # Allow boolean positional values in function calls, like `dict.get(... True)`
-  "FBT003",
-  # Ignore checks for possible passwords
-  "S105", "S106", "S107",
-  # Ignore complexity
-  "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
+    # Allow non-abstract empty methods in abstract base classes
+    "B027",
+    # Allow boolean positional values in function calls, like `dict.get(... True)`
+    "FBT003",
+    # Ignore checks for possible passwords
+    "S105", "S106", "S107",
+    # Ignore complexity
+    "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
 ]
 unfixable = [
-  # Don't touch unused imports
-  "F401",
+    # Don't touch unused imports
+    "F401",
 ]
 
 [tool.ruff.isort]
 known-first-party = ["edwh_bundler_plugin"]
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
@@ -165,20 +182,20 @@
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
 source_pkgs = ["edwh_bundler_plugin", "tests"]
 branch = true
 parallel = true
 omit = [
-  "src/edwh_bundler_plugin/__about__.py",
+    "src/edwh_bundler_plugin/__about__.py",
 ]
 
 [tool.coverage.paths]
 edwh_bundler_plugin = ["src/edwh_bundler_plugin", "*/edwh-bundler-plugin/src/edwh_bundler_plugin"]
 tests = ["tests", "*/edwh-bundler-plugin/tests"]
 
 [tool.coverage.report]
 exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
+    "no cov",
+    "if __name__ == .__main__.:",
+    "if TYPE_CHECKING:",
 ]
```

### Comparing `edwh_bundler_plugin-0.1.7/PKG-INFO` & `edwh_bundler_plugin-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-bundler-plugin
-Version: 0.1.7
+Version: 0.2.0
 Summary: Python-only static file (js, css) bundler for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-bundler-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-bundler-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-bundler-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

