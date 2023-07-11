# Comparing `tmp/poetry-dynamic-versioning-1.0.0b2.tar.gz` & `tmp/poetry-dynamic-versioning-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry-dynamic-versioning-1.0.0b2.tar", max compression
+gzip compressed data, was "poetry-dynamic-versioning-1.0.0b3.tar", max compression
```

## Comparing `poetry-dynamic-versioning-1.0.0b2.tar` & `poetry-dynamic-versioning-1.0.0b3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1089 2021-12-24 01:49:41.427292 poetry-dynamic-versioning-1.0.0b2/LICENSE
--rw-r--r--   0        0        0     7545 2022-04-14 16:01:55.635465 poetry-dynamic-versioning-1.0.0b2/poetry_dynamic_versioning/__init__.py
--rw-r--r--   0        0        0     2978 2022-04-14 16:07:56.308341 poetry-dynamic-versioning-1.0.0b2/poetry_dynamic_versioning/plugin.py
--rw-r--r--   0        0        0     1622 2022-04-14 16:25:52.259591 poetry-dynamic-versioning-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0    10457 2022-04-14 15:59:29.183993 poetry-dynamic-versioning-1.0.0b2/README.md
--rw-r--r--   0        0        0    11828 1970-01-01 00:00:00.000000 poetry-dynamic-versioning-1.0.0b2/setup.py
--rw-r--r--   0        0        0    11949 1970-01-01 00:00:00.000000 poetry-dynamic-versioning-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2021-12-24 01:49:41.427292 poetry-dynamic-versioning-1.0.0b3/LICENSE
+-rw-r--r--   0        0        0     7566 2022-04-24 10:58:12.278980 poetry-dynamic-versioning-1.0.0b3/poetry_dynamic_versioning/__init__.py
+-rw-r--r--   0        0        0     4036 2022-04-24 11:33:30.859916 poetry-dynamic-versioning-1.0.0b3/poetry_dynamic_versioning/plugin.py
+-rw-r--r--   0        0        0     1529 2022-04-24 12:42:47.490024 poetry-dynamic-versioning-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0    10457 2022-04-24 10:50:25.065710 poetry-dynamic-versioning-1.0.0b3/README.md
+-rw-r--r--   0        0        0    11711 1970-01-01 00:00:00.000000 poetry-dynamic-versioning-1.0.0b3/setup.py
+-rw-r--r--   0        0        0    11949 1970-01-01 00:00:00.000000 poetry-dynamic-versioning-1.0.0b3/PKG-INFO
```

### Comparing `poetry-dynamic-versioning-1.0.0b2/LICENSE` & `poetry-dynamic-versioning-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry-dynamic-versioning-1.0.0b2/poetry_dynamic_versioning/__init__.py` & `poetry-dynamic-versioning-1.0.0b3/poetry_dynamic_versioning/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,19 +24,17 @@
         self.path = path
         self.original_version = original_version
         self.version = version
         self.substitutions = {} if substitutions is None else substitutions
 
 
 class _State:
-    def __init__(self, projects: MutableMapping[str, _ProjectState] = None) -> None:
-        if projects is None:
-            self.projects = {}  # type: MutableMapping[str, _ProjectState]
-        else:
-            self.projects = projects
+    def __init__(self) -> None:
+        self.patched = False
+        self.projects = {}  # type: MutableMapping[str, _ProjectState]
 
 
 _state = _State()
 
 
 def _default_config() -> Mapping:
     return {
@@ -188,46 +186,47 @@
             file.write_text(new_content, encoding="utf-8")
 
 
 def _apply_version(
     version: str, config: Mapping, pyproject_path: Path, retain: bool = False
 ) -> str:
     pyproject = tomlkit.parse(pyproject_path.read_text(encoding="utf-8"))
-    if pyproject["tool"]["poetry"]["version"] != version:
-        pyproject["tool"]["poetry"]["version"] = version
+
+    if pyproject["tool"]["poetry"]["version"] != version:  # type: ignore
+        pyproject["tool"]["poetry"]["version"] = version  # type: ignore
 
         # Disable the plugin in case we're building a source distribution,
         # which won't have access to the VCS info at install time.
         # We revert this later when we deactivate.
         if not retain:
-            pyproject["tool"]["poetry-dynamic-versioning"]["enable"] = False
+            pyproject["tool"]["poetry-dynamic-versioning"]["enable"] = False  # type: ignore
 
         pyproject_path.write_text(tomlkit.dumps(pyproject), encoding="utf-8")
 
-    name = pyproject["tool"]["poetry"]["name"]
+    name = pyproject["tool"]["poetry"]["name"]  # type: ignore
 
     _substitute_version(
-        name,
+        name,  # type: ignore
         pyproject_path.parent,
         config["substitution"]["files"],
         config["substitution"]["patterns"],
         version,
     )
 
-    return name
+    return name  # type: ignore
 
 
 def _revert_version(retain: bool = False) -> None:
     for project, state in _state.projects.items():
         if state.original_version != state.version:
             pyproject = tomlkit.parse(state.path.read_text(encoding="utf-8"))
-            pyproject["tool"]["poetry"]["version"] = state.original_version
+            pyproject["tool"]["poetry"]["version"] = state.original_version  # type: ignore
 
             if not retain:
-                pyproject["tool"]["poetry-dynamic-versioning"]["enable"] = True
+                pyproject["tool"]["poetry-dynamic-versioning"]["enable"] = True  # type: ignore
 
             state.path.write_text(tomlkit.dumps(pyproject), encoding="utf-8")
 
         if state.substitutions:
             for file, content in state.substitutions.items():
                 file.write_text(content, encoding="utf-8")
```

### Comparing `poetry-dynamic-versioning-1.0.0b2/pyproject.toml` & `poetry-dynamic-versioning-1.0.0b3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-dynamic-versioning"
-version = "1.0.0b2"
+version = "1.0.0b3"
 description = "Plugin for Poetry to enable dynamic versioning based on VCS tags"
 license = "MIT"
 authors = ["Matthew T. Kennerly <mtkennerly@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/mtkennerly/poetry-dynamic-versioning"
 keywords = ["poetry", "plugin", "version", "versioning", "dynamic"]
 classifiers = [
@@ -34,16 +34,13 @@
 flake8 = "^3.7"
 mypy = "^0.740"
 pep8-naming = "^0.8.2"
 
 [tool.poetry.plugins."poetry.application.plugin"]
 poetry-dynamic-versioning = "poetry_dynamic_versioning.plugin:DynamicVersioningPlugin"
 
-[tool.poetry.scripts]
-poetry-dynamic-versioning = 'poetry_dynamic_versioning.__main__:main'
-
 [tool.black]
 line-length = 100
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `poetry-dynamic-versioning-1.0.0b2/README.md` & `poetry-dynamic-versioning-1.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `poetry-dynamic-versioning-1.0.0b2/setup.py` & `poetry-dynamic-versioning-1.0.0b3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,20 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['dunamai>=1.11.1,<2.0.0', 'jinja2>=2.11.1,<4', 'poetry>=1.2.0a2,<2.0.0']
 
 entry_points = \
-{'console_scripts': ['poetry-dynamic-versioning = '
-                     'poetry_dynamic_versioning.__main__:main'],
- 'poetry.application.plugin': ['poetry-dynamic-versioning = '
+{'poetry.application.plugin': ['poetry-dynamic-versioning = '
                                'poetry_dynamic_versioning.plugin:DynamicVersioningPlugin']}
 
 setup_kwargs = {
     'name': 'poetry-dynamic-versioning',
-    'version': '1.0.0b2',
+    'version': '1.0.0b3',
     'description': 'Plugin for Poetry to enable dynamic versioning based on VCS tags',
     'long_description': '# Dynamic versioning plugin for Poetry\n[![Version](https://img.shields.io/pypi/v/poetry-dynamic-versioning)](https://pypi.org/project/poetry-dynamic-versioning)\n[![License: MIT](https://img.shields.io/badge/license-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n\nThis package is a plugin for [Poetry](https://github.com/sdispater/poetry)\nto enable dynamic versioning based on tags in your version control system,\npowered by [Dunamai](https://github.com/mtkennerly/dunamai). Many different\nversion control systems are supported, including Git and Mercurial; please\nrefer to the Dunamai page for the full list (and minimum supported version\nwhere applicable).\n\nThis is using the experimental plugin interface from Poetry 1.2.0a2 and newer\npre-releases. Until the final Poetry 1.2.0 release, the design of this plugin\nis subject to change.\n\n## Installation\nPython 3.6+ and Poetry 1.2.0a2+ are required.\n\nInstall by running `poetry plugin add poetry-dynamic-versioning`.\n\n* Add this section to your pyproject.toml:\n  ```toml\n  [tool.poetry-dynamic-versioning]\n  enable = true\n  ```\n* Include the plugin in the `build-system` section of pyproject.toml\n  for interoperability with PEP 517 build frontends.\n  * Example using `poetry` as the build system:\n    ```toml\n    [build-system]\n    requires = ["poetry>=1.2.0a2", "poetry-dynamic-versioning>=1.0.0b1"]\n    build-backend = "poetry.masonry.api"\n    ```\n\nPoetry\'s typical `version` setting is still required in `[tool.poetry]`,\nbut you are encouraged to use `version = "0.0.0"` as a standard placeholder.\n\nWith the minimal configuration above, the plugin will automatically take effect\nwhen you run commands such as `poetry build`. It will update the version in\npyproject.toml, then revert the change when the plugin deactivates. If you want\nto include a `__version__` variable in your code, just put a placeholder in the\nappropriate file and configure the plugin to update it (see below) if it isn\'t\none of the defaults. You are encouraged to use `__version__ = "0.0.0"` as a\nstandard placeholder.\n\n## Configuration\nIn your pyproject.toml file, you may configure the following options:\n\n* `[tool.poetry-dynamic-versioning]`: General options.\n  * `enable`: Boolean. Default: false. Since the plugin has to be installed\n    globally, this setting is an opt-in per project. This setting will likely\n    be removed once plugins are officially supported.\n  * `vcs`: String. This is the version control system to check for a version.\n    One of: `any` (default), `git`, `mercurial`, `darcs`, `bazaar`,\n    `subversion`, `fossil`.\n  * `metadata`: Boolean. Default: unset. If true, include the commit hash in\n    the version, and also include a dirty flag if `dirty` is true. If unset,\n    metadata will only be included if you are on a commit without a version tag.\n    This is ignored when `format` or `format-jinja` is used.\n  * `tagged-metadata`: Boolean. Default: false. If true, include any tagged\n    metadata discovered as the first part of the metadata segment.\n    Has no effect when `metadata` is set to false.\n    This is ignored when `format` or `format-jinja` is used.\n  * `dirty`: Boolean. Default: false. If true, include a dirty flag in the\n    metadata, indicating whether there are any uncommitted changes.\n    Has no effect when `metadata` is set to false.\n    This is ignored when `format` or `format-jinja` is used.\n  * `pattern`: String. This is a regular expression which will be used to find\n    a tag representing a version. There must be a capture group named `base`\n    with the main part of the version. Optionally, it may contain another two\n    groups named `stage` and `revision` for prereleases, and it may contain a\n    group named `tagged_metadata` to be used with the `tagged-metadata` option.\n    There may also be a group named `epoch` for the PEP 440 concept.\n\n    The default is to use Dunamai\'s `VERSION_SOURCE_PATTERN`. You can check it\n    for your installed version of Dunamai by running this command:\n    ```\n    poetry run python -c "import dunamai; print(dunamai.VERSION_SOURCE_PATTERN)"\n    ```\n    Or you can check [the latest definition in Dunamai](https://github.com/mtkennerly/dunamai/blob/master/dunamai/__init__.py).\n\n    Remember that backslashes must be escaped (`\\\\`) in the TOML file.\n  * `format`: String. Default: unset. This defines a custom output format for\n    the version. Available substitutions:\n\n    * `{base}`\n    * `{stage}`\n    * `{revision}`\n    * `{distance}`\n    * `{commit}`\n    * `{dirty}`\n    * `{tagged_metadata}`\n    * `{branch}`\n    * `{branch_escaped}` which omits any non-letter/number characters\n    * `{timestamp}` of the current commit, which expands to YYYYmmddHHMMSS as UTC\n\n    Example: `v{base}+{distance}.{commit}`\n  * `format-jinja`: String. Default: unset. This defines a custom output format\n    for the version, using a [Jinja](https://pypi.org/project/Jinja2) template.\n    When this is set, `format` is ignored.\n\n    Available variables:\n\n    * `base` (string)\n    * `stage` (string or None)\n    * `revision` (integer or None)\n    * `distance` (integer)\n    * `commit` (string)\n    * `dirty` (boolean)\n    * `tagged_metadata` (string or None)\n    * `version` (dunumai.Version)\n    * `env` (dictionary of environment variables)\n    * `branch` (string or None)\n    * `branch_escaped` (string or None)\n    * `timestamp` (string or None)\n\n    Available functions:\n\n    * `bump_version` ([from Dunamai](https://github.com/mtkennerly/dunamai/blob/dc2777cdcc5eeff61c10602e33b1a0dc0bb0357b/dunamai/__init__.py#L786-L797))\n    * `serialize_pep440` ([from Dunamai](https://github.com/mtkennerly/dunamai/blob/dc2777cdcc5eeff61c10602e33b1a0dc0bb0357b/dunamai/__init__.py#L687-L710))\n    * `serialize_semver` ([from Dunamai](https://github.com/mtkennerly/dunamai/blob/dc2777cdcc5eeff61c10602e33b1a0dc0bb0357b/dunamai/__init__.py#L740-L752))\n    * `serialize_pvp` ([from Dunamai](https://github.com/mtkennerly/dunamai/blob/dc2777cdcc5eeff61c10602e33b1a0dc0bb0357b/dunamai/__init__.py#L766-L775))\n\n    Simple example:\n\n    ```toml\n    format-jinja = "{% if distance == 0 %}{{ base }}{% else %}{{ base }}+{{ distance }}.{{ commit }}{% endif %}"\n    ```\n\n    Complex example:\n\n    ```toml\n    format-jinja = """\n        {%- if distance == 0 -%}\n            {{ serialize_pep440(base, stage, revision) }}\n        {%- elif revision is not none -%}\n            {{ serialize_pep440(base, stage, revision + 1, dev=distance, metadata=[commit]) }}\n        {%- else -%}\n            {{ serialize_pep440(bump_version(base), stage, revision, dev=distance, metadata=[commit]) }}\n        {%- endif -%}\n    """\n    ```\n  * `format-jinja-imports`: Array of tables. Default: empty. This defines\n    additional things to import and make available to the `format-jinja`\n    template. Each table must contain a `module` key and may also contain an\n    `item` key. Consider this example:\n\n    ```toml\n    format-jinja-imports = [\n        { module = "foo" },\n        { module = "bar", item = "baz" },\n    ]\n    ```\n\n    This is roughly equivalent to:\n\n    ```python\n    import foo\n    from bar import baz\n    ```\n\n    `foo` and `baz` would then become available in the Jinja formatting.\n  * `style`: String. Default: unset. One of: `pep440`, `semver`, `pvp`.\n    These are preconfigured output formats. If you set both a `style` and\n    a `format`, then the format will be validated against the style\'s rules.\n    If `style` is unset, the default output format will follow PEP 440,\n    but a custom `format` will only be validated if `style` is set explicitly.\n  * `latest-tag`: Boolean. Default: false. If true, then only check the latest\n    tag for a version, rather than looking through all the tags until a suitable\n    one is found to match the `pattern`.\n  * `bump`: Boolean. Default: false. If true, then increment the last part of\n    the version `base` by 1, unless the `stage` is set, in which case increment\n    the `revision` by 1 or set it to a default of 2 if there was no `revision`.\n    Does nothing when on a commit with a version tag.\n\n    Example, if there have been 3 commits since the `v1.3.1` tag:\n    * PEP 440 with `bump = false`: `1.3.1.post3.dev0+28c1684`\n    * PEP 440 with `bump = true`: `1.3.2.dev3+28c1684`\n* `[tool.poetry-dynamic-versioning.subversion]`: Options specific to Subversion.\n  * `tag-dir`: String. Default: `tags`. This is the location of tags relative\n    to the root.\n* `[tool.poetry-dynamic-versioning.substitution]`: Insert the dynamic version\n  into additional files other than just pyproject.toml. These changes will be\n  reverted when the plugin deactivates.\n  * `files`: List of globs for any files that need substitutions. Default:\n    `["*.py", "*/__init__.py", "*/__version__.py", "*/_version.py"]`.\n    To disable substitution, set this to an empty list.\n  * `patterns`: List of regular expressions for the text to replace.\n    Each regular expression must have two capture groups, which are any\n    text to preserve before and after the replaced text. Default:\n    `["(^__version__\\s*(?::.*?)?=\\s*[\'\\"])[^\'\\"]*([\'\\"])"]`.\n\n    Remember that the backslashes must be escaped (`\\\\`) in the TOML file.\n\nSimple example:\n\n```toml\n[tool.poetry-dynamic-versioning]\nenable = true\nvcs = "git"\nstyle = "semver"\n```\n\n## Command line mode\nThe plugin also has a command line mode for execution on demand.\nThis mode applies the dynamic version to all relevant files and leaves\nthe changes in-place, allowing you to inspect the result.\nYour configuration will be detected from pyproject.toml as normal,\nbut the `enable` option is not necessary.\n\nTo activate this mode, run the `poetry dynamic-versioning` command\nin your console.\n\n## Caveats\n* The dynamic version is not available during `poetry run` or `poetry shell`.\n* Regarding PEP 517 support:\n\n  `pip wheel .` will not work, because Pip creates an isolated copy of the\n  source code, which does not contain the Git history and therefore cannot\n  determine the dynamic version.\n\n  If you want to build wheels of your dependencies, you **can** do the following,\n  but it won\'t work with path dependencies for the same reason as above:\n\n  ```\n  poetry export -f requirements.txt -o requirements.txt --without-hashes\n  pip wheel -r requirements.txt\n  ```\n\n  With newer versions of Pip, you can pass `--use-feature=in-tree-build`\n  to make the `pip wheel .` and `pip install .` commands work.\n\n## Development\nPlease refer to [CONTRIBUTING.md](CONTRIBUTING.md).\n',
     'author': 'Matthew T. Kennerly',
     'author_email': 'mtkennerly@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mtkennerly/poetry-dynamic-versioning',
```

### Comparing `poetry-dynamic-versioning-1.0.0b2/PKG-INFO` & `poetry-dynamic-versioning-1.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-dynamic-versioning
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Plugin for Poetry to enable dynamic versioning based on VCS tags
 Home-page: https://github.com/mtkennerly/poetry-dynamic-versioning
 License: MIT
 Keywords: poetry,plugin,version,versioning,dynamic
 Author: Matthew T. Kennerly
 Author-email: mtkennerly@gmail.com
 Requires-Python: >=3.6,<4.0
```

