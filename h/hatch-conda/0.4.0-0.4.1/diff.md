# Comparing `tmp/hatch_conda-0.4.0.tar.gz` & `tmp/hatch_conda-0.4.1.tar.gz`

## Comparing `hatch_conda-0.4.0.tar` & `hatch_conda-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/.flake8
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/.gitattributes
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/HISTORY.md
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/hatch_conda/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/hatch_conda/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/hatch_conda/hooks.py
--rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/hatch_conda/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/tests/test_config.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/tests/utils.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/README.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/hatch.toml
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 hatch_conda-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/.gitattributes
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/HISTORY.md
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/hatch_conda/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/hatch_conda/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/hatch_conda/hooks.py
+-rw-r--r--   0        0        0     8553 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/hatch_conda/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/tests/test_config.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/tests/utils.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/README.md
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/hatch.toml
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 hatch_conda-0.4.1/PKG-INFO
```

### Comparing `hatch_conda-0.4.0/HISTORY.md` & `hatch_conda-0.4.1/HISTORY.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 -----
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.1] - 11/07/2023
+
+### Fixed
+- Default `environment-file` value had the wrong type.
+
 ## [0.4.0] - 02/07/2023
 
 ### Added
 - A conda `environment.yml` file can specified, which will be used to set up the environment. This allows installing packages from, e.g., the `conda-forge` index.
 
 ## [0.3.2] - 09/06/2023
```

### Comparing `hatch_conda-0.4.0/.github/workflows/build.yml` & `hatch_conda-0.4.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.4.0/.github/workflows/test.yml` & `hatch_conda-0.4.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.4.0/hatch_conda/plugin.py` & `hatch_conda-0.4.1/hatch_conda/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,180 +15,180 @@
 
 
 class ShellManager:
     def __init__(self, environment: EnvironmentInterface):
         self.environment = environment
 
     def enter_bash(self, path: str, args: list[str], cmdl: str) -> None:
-        self.spawn_linux_shell(path or 'bash', args or ['-i'], cmdl)
+        self.spawn_linux_shell(path or "bash", args or ["-i"], cmdl)
 
     def enter_zsh(self, path: str, args: list[str], cmdl: str) -> None:
-        self.spawn_linux_shell(path or 'zsh', args or ['-i'], cmdl)
+        self.spawn_linux_shell(path or "zsh", args or ["-i"], cmdl)
 
     def spawn_linux_shell(
-        self, path: str, args: list[str] | None = None, cmdl: str = '', callback: Callable | None = None
+        self, path: str, args: list[str] | None = None, cmdl: str = "", callback: Callable | None = None
     ) -> None:
         columns, lines = shutil.get_terminal_size()
         terminal = pexpect.spawn(path, args=args, dimensions=(lines, columns))
 
         def sigwinch_passthrough(sig: int, data: FrameType | None) -> None:
             new_columns, new_lines = shutil.get_terminal_size()
             terminal.setwinsize(new_lines, new_columns)
 
-        signal.signal(signal.SIGWINCH, sigwinch_passthrough)
+        signal.signal(signal.SIGWINCH, sigwinch_passthrough)  # type: ignore
 
         terminal.sendline(cmdl)
 
         if callback is not None:
             callback(terminal)
 
         terminal.interact(escape_character=None)
         terminal.close()
 
         self.environment.platform.exit_with_code(terminal.exitstatus)
 
 
 class CondaEnvironment(EnvironmentInterface):
-    PLUGIN_NAME = 'conda'
+    PLUGIN_NAME = "conda"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._config_command = None
         self._config_conda_forge = None
         self._config_environment_file = None
         self.__python_version = None
 
-        self.conda_env_name = f'{self.metadata.core.name}_{self.name}_{self.python_version}'
-        self.project_path = '.'
+        self.conda_env_name = f"{self.metadata.core.name}_{self.name}_{self.python_version}"
+        self.project_path = "."
 
         self.shells = ShellManager(self)
 
     @staticmethod
     def get_option_types():
-        return {'command': str, 'conda-forge': bool, 'environment-file': str}
+        return {"command": str, "conda-forge": bool, "environment-file": str}
 
     def _config_value(self, field_name, default, valid=None):
         class_name = f'_config_{field_name.replace("-", "_")}'
         if self.__dict__[class_name] is None:
             value = self.config.get(field_name, default)
             if not isinstance(value, self.get_option_types()[field_name]):
                 raise TypeError(
-                    f'Field `tool.hatch.envs.{self.name}.{field_name}` must be a '
-                    + '`{self.get_option_types()[field_name]}`'
+                    f"Field `tool.hatch.envs.{self.name}.{field_name}` must be a "
+                    + "`{self.get_option_types()[field_name]}`"
                 )
             if valid is not None and value not in valid:
-                raise ValueError(f'Field `tool.hatch.envs.{self.name}.{field_name}` must be any of [{valid}] values.')
+                raise ValueError(f"Field `tool.hatch.envs.{self.name}.{field_name}` must be any of [{valid}] values.")
             self.__dict__[class_name] = value
         return self.__dict__[class_name]
 
     @property
     def config_command(self):
-        return self._config_value('command', 'conda', ['conda', 'mamba', 'micromamba'])
+        return self._config_value("command", "conda", ["conda", "mamba", "micromamba"])
 
     @property
     def config_conda_forge(self):
-        return self._config_value('conda-forge', True)
+        return self._config_value("conda-forge", True)
 
     @property
     def environment_file(self):
-        return self._config_value('environment-file', False)
+        return self._config_value("environment-file", "")
 
     @property
     def python_version(self):
         if self.__python_version is None:
-            python_version = self.config.get('python', '')
+            python_version = self.config.get("python", "")
             if not python_version:
-                python_version = '.'.join(map(str, sys.version_info[:2]))
+                python_version = ".".join(map(str, sys.version_info[:2]))
             elif python_version.isdigit() and len(python_version) > 1:
-                python_version = f'{python_version[0]}.{python_version[1:]}'
+                python_version = f"{python_version[0]}.{python_version[1:]}"
 
             self.__python_version = python_version
 
         return self.__python_version
 
     def _get_conda_env_path(self, name: str):
-        if self.config_command == 'micromamba':
-            output = self.platform.check_command_output([self.config_command, 'info', '--name', name])
+        if self.config_command == "micromamba":
+            output = self.platform.check_command_output([self.config_command, "info", "--name", name])
 
-            match_env_location = r'env location : ([\S]*)\n'
+            match_env_location = r"env location : ([\S]*)\n"
             return re.findall(match_env_location, output)[0]
 
         else:
-            output = self.platform.check_command_output([self.config_command, 'env', 'list'])
+            output = self.platform.check_command_output([self.config_command, "env", "list"])
             env_names, env_paths = zip(
                 *[
-                    (line.split(' ')[0], line.split(' ')[-1])
+                    (line.split(" ")[0], line.split(" ")[-1])
                     for line in output.splitlines()
-                    if len(line.split(' ')[0]) > 1
+                    if len(line.split(" ")[0]) > 1
                 ]
             )
             if name not in env_names:
                 return None
             return env_paths[env_names.index(name)]
 
     def find(self):
         return self._get_conda_env_path(self.conda_env_name)
 
     def create(self):
         if not self.environment_file:
-            command = [self.config_command, 'create', '-y']
+            command = [self.config_command, "create", "-y"]
             if self.config_conda_forge:
-                command += ['-c', 'conda-forge', '--no-channel-priority']
+                command += ["-c", "conda-forge", "--no-channel-priority"]
             command += [
-                f'python={self.python_version}',
-                'pip',
+                f"python={self.python_version}",
+                "pip",
             ]
-        elif self.config_command == 'micromamba':
-            command = ['micromamba', 'create', '-y', '--file', self.environment_file]
+        elif self.config_command == "micromamba":
+            command = ["micromamba", "create", "-y", "--file", self.environment_file]
         else:
-            command = [self.config_command, 'env', 'create', '--file', self.environment_file]
+            command = [self.config_command, "env", "create", "--file", self.environment_file]
 
-        command += ['-n', self.conda_env_name]
+        command += ["-n", self.conda_env_name]
 
         if self.verbosity > 0:  # no cov
             self.platform.check_command(command)
         else:
             self.platform.check_command_output(command)
         self.apply_env_vars()
 
     def remove(self):
-        self.platform.check_command_output([self.config_command, 'env', 'remove', '-y', '--name', self.conda_env_name])
+        self.platform.check_command_output([self.config_command, "env", "remove", "-y", "--name", self.conda_env_name])
 
     def exists(self):
         env_path = self._get_conda_env_path(self.conda_env_name)
         if env_path is not None:
             return Path(self._get_conda_env_path(self.conda_env_name)).exists()
         return False
 
     def construct_conda_run_command(self, command):
-        return [self.config_command, 'run', '-n', self.conda_env_name] + command
+        return [self.config_command, "run", "-n", self.conda_env_name] + command
 
     def construct_pip_install_command(self, *args, **kwargs):
         return self.construct_conda_run_command(super().construct_pip_install_command(*args, **kwargs))
 
     def install_project(self):
         self.apply_env_vars()
         with self:
             self.platform.check_command(self.construct_pip_install_command([self.apply_features(self.project_path)]))
 
     def install_project_dev_mode(self):
         self.apply_env_vars()
         with self:
             self.platform.check_command(
-                self.construct_pip_install_command(['--editable', self.apply_features(self.project_path)])
+                self.construct_pip_install_command(["--editable", self.apply_features(self.project_path)])
             )
 
     def dependencies_in_sync(self):
         if not self.dependencies:
             return True
         self.apply_env_vars()
         with self:
             process = self.platform.run_command(
-                ' '.join(['hatchling', 'dep', 'synced', '-p', 'python', *self.dependencies]),
+                " ".join(["hatchling", "dep", "synced", "-p", "python", *self.dependencies]),
                 capture_output=True,
             )
             return not process.returncode
 
     def sync_dependencies(self):
         self.apply_env_vars()
         with self:
@@ -198,39 +198,39 @@
     def command_context(self):
         with self:
             yield
 
     def run_shell_command(self, command):
         self.apply_env_vars()
         return self.platform.run_command(
-            ' '.join(
+            " ".join(
                 self.construct_conda_run_command(
                     [
                         command,
                     ]
                 )
             )
         )
 
     def enter_shell(self, name, path, args):  # no cov
-        cmdl = f'{self.config_command} activate {self.conda_env_name}'
-        shell_executor = getattr(self.shells, f'enter_{name}', None)
+        cmdl = f"{self.config_command} activate {self.conda_env_name}"
+        shell_executor = getattr(self.shells, f"enter_{name}", None)
         if shell_executor is None:
-            raise NotImplementedError(f'entering {name} shell in not supported yet')
+            raise NotImplementedError(f"entering {name} shell in not supported yet")
         else:
             self.apply_env_vars()
             shell_executor(path, args, cmdl)
 
     def apply_env_vars(self):
-        if self.config_command == 'micromamba':
+        if self.config_command == "micromamba":
             for env_var, value in dict(self.env_vars).items():
                 os.environ[env_var] = value
         else:
             env_vars = []
             for env_var, value in dict(self.env_vars).items():
                 value_fixed = value
-                if sys.platform == 'win32':
-                    value_fixed = value_fixed.replace('%', '%%%%%%%%')
-                env_vars.append(f'{env_var}={value_fixed}')
+                if sys.platform == "win32":
+                    value_fixed = value_fixed.replace("%", "%%%%%%%%")
+                env_vars.append(f"{env_var}={value_fixed}")
             self.platform.check_command(
-                ['conda', 'env', 'config', 'vars', 'set', '-n', self.conda_env_name, '--'] + env_vars
+                ["conda", "env", "config", "vars", "set", "-n", self.conda_env_name, "--"] + env_vars
             )
```

### Comparing `hatch_conda-0.4.0/tests/conftest.py` & `hatch_conda-0.4.1/tests/conftest.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,101 +19,101 @@
 class CliRunner(__CliRunner):
     def __init__(self, command):
         super().__init__()
         self._command = command
 
     def __call__(self, *args, **kwargs):
         # Exceptions should always be handled
-        kwargs.setdefault('catch_exceptions', False)
+        kwargs.setdefault("catch_exceptions", False)
 
         return self.invoke(self._command, args, **kwargs)
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def hatch():
     from hatch import cli
 
     return CliRunner(cli.hatch)
 
 
-@pytest.fixture(scope='session', autouse=True)
+@pytest.fixture(scope="session", autouse=True)
 def isolation() -> Generator[Path, None, None]:
     with temp_directory() as d:
-        data_dir = d / 'data'
+        data_dir = d / "data"
         data_dir.mkdir()
-        cache_dir = d / 'cache'
+        cache_dir = d / "cache"
         cache_dir.mkdir()
 
         default_env_vars = {
-            AppEnvVars.NO_COLOR: '1',
+            AppEnvVars.NO_COLOR: "1",
             ConfigEnvVars.DATA: str(data_dir),
             ConfigEnvVars.CACHE: str(cache_dir),
-            'COLUMNS': '80',
-            'LINES': '24',
+            "COLUMNS": "80",
+            "LINES": "24",
         }
         with d.as_cwd(default_env_vars):
             os.environ.pop(AppEnvVars.ENV_ACTIVE, None)
             yield d
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def data_dir() -> Generator[Path, None, None]:
     yield Path(os.environ[ConfigEnvVars.DATA])
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def platform():
     return PLATFORM
 
 
 @pytest.fixture
 def temp_dir() -> Generator[Path, None, None]:
     with temp_directory() as d:
         yield d
 
 
 @pytest.fixture
 def temp_dir_data(temp_dir) -> Generator[Path, None, None]:
-    data_path = temp_dir / 'data'
+    data_path = temp_dir / "data"
     data_path.mkdir()
 
     with EnvVars({ConfigEnvVars.DATA: str(data_path)}):
         yield temp_dir
 
 
 @pytest.fixture(autouse=True)
 def config_file(tmp_path) -> ConfigFile:
-    path = Path(tmp_path, 'config.toml')
+    path = Path(tmp_path, "config.toml")
     os.environ[ConfigEnvVars.CONFIG] = str(path)
     config = ConfigFile(path)
     config.restore()
     return config
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def default_python_version():
-    return f'{sys.version_info[0]}.{sys.version_info[1]}'
+    return f"{sys.version_info[0]}.{sys.version_info[1]}"
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def project_name():
     return os.urandom(12).hex()
 
 
 @pytest.fixture
 def conda_project(hatch, temp_dir_data, config_file, project_name):
-    config_file.model.template.plugins['default']['tests'] = False
+    config_file.model.template.plugins["default"]["tests"] = False
     config_file.save()
 
     with temp_dir_data.as_cwd():
-        result = hatch('new', project_name)
+        result = hatch("new", project_name)
 
     assert result.exit_code == 0, result.output
 
     project_path = temp_dir_data / project_name
 
     project = Project(project_path)
-    config = dict(project.config.envs['default'])
-    config.update({'type': 'conda'})
-    update_project_environment(project, 'default', config)
+    config = dict(project.config.envs["default"])
+    config.update({"type": "conda"})
+    update_project_environment(project, "default", config)
 
     yield project_path
```

### Comparing `hatch_conda-0.4.0/tests/test_config.py` & `hatch_conda-0.4.1/tests/test_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,71 +5,71 @@
 
 class TestPythonVersion:
     def test_default(self, isolation, data_dir, platform, default_python_version):
         env_config = {}
         project = Project(
             isolation,
             config={
-                'project': {'name': 'my_app', 'version': '0.0.1'},
-                'tool': {'hatch': {'envs': {'default': env_config}}},
+                "project": {"name": "my_app", "version": "0.0.1"},
+                "tool": {"hatch": {"envs": {"default": env_config}}},
             },
         )
         environment = CondaEnvironment(
             root=isolation,
             metadata=project.metadata,
-            name='default',
-            config=project.config.envs['default'],
+            name="default",
+            config=project.config.envs["default"],
             matrix_variables={},
             data_directory=data_dir,
             isolated_data_directory=None,
             platform=platform,
             verbosity=0,
         )
 
         assert environment.python_version == default_python_version
 
     def test_long(self, isolation, data_dir, platform):
-        env_config = {'python': '3.10'}
+        env_config = {"python": "3.10"}
         project = Project(
             isolation,
             config={
-                'project': {'name': 'my_app', 'version': '0.0.1'},
-                'tool': {'hatch': {'envs': {'default': env_config}}},
+                "project": {"name": "my_app", "version": "0.0.1"},
+                "tool": {"hatch": {"envs": {"default": env_config}}},
             },
         )
         environment = CondaEnvironment(
             root=isolation,
             metadata=project.metadata,
-            name='default',
-            config=project.config.envs['default'],
+            name="default",
+            config=project.config.envs["default"],
             matrix_variables={},
             data_directory=data_dir,
             isolated_data_directory=None,
             platform=platform,
             verbosity=0,
         )
 
-        assert environment.python_version == '3.10'
+        assert environment.python_version == "3.10"
 
     def test_short(self, isolation, data_dir, platform):
-        env_config = {'python': '310'}
+        env_config = {"python": "310"}
         project = Project(
             isolation,
             config={
-                'project': {'name': 'my_app', 'version': '0.0.1'},
-                'tool': {'hatch': {'envs': {'default': env_config}}},
+                "project": {"name": "my_app", "version": "0.0.1"},
+                "tool": {"hatch": {"envs": {"default": env_config}}},
             },
         )
 
         environment = CondaEnvironment(
             root=isolation,
             metadata=project.metadata,
-            name='default',
-            config=project.config.envs['default'],
+            name="default",
+            config=project.config.envs["default"],
             matrix_variables={},
             data_directory=data_dir,
             isolated_data_directory=None,
             platform=platform,
             verbosity=0,
         )
 
-        assert environment.python_version == '3.10'
+        assert environment.python_version == "3.10"
```

### Comparing `hatch_conda-0.4.0/LICENSE.txt` & `hatch_conda-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.4.0/README.md` & `hatch_conda-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `hatch_conda-0.4.0/hatch.toml` & `hatch_conda-0.4.1/hatch.toml`

 * *Files 17% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 [envs.lint]
 skip-install = true
 dependencies = [
   "flake8>=4.0.1",
   "flake8-bugbear>=22.3.23",
   "flake8-quotes>=3.3.1",
+  "Flake8-pyproject>=1.2.3",
   "black>=22.3.0",
   "isort>=5.10.1",
   "mypy>=0.942",
 ]
 [envs.lint.scripts]
 typing = "mypy hatch_conda tests --install-types --non-interactive"
 style = [
```

### Comparing `hatch_conda-0.4.0/pyproject.toml` & `hatch_conda-0.4.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -50,37 +50,40 @@
 [tool.mypy]
 disallow_untyped_defs = false
 follow_imports = "normal"
 ignore_missing_imports = true
 pretty = true
 show_column_numbers = true
 warn_no_return = false
-warn_unused_ignores = true
 
 [tool.black]
-include = '\.pyi?$'
-line-length = 120
-skip-string-normalization = true
 target-version = ["py37"]
+line-length = 120
 
 [tool.isort]
-default_section = "THIRDPARTY"
-force_grid_wrap = 0
+py_version = "37"
+profile = "black"
 include_trailing_comma = true
-known_first_party = ["hatch_conda"]
-line_length = 120
-multi_line_output = 3
 use_parentheses = true
+src_paths = ["hatch_conda", "tests"]
+line_length = 120
 
 [tool.coverage.run]
 branch = true
 parallel = true
+source_pkgs = ["hatch_conda", "tests"]
 omit = [
   "hatch_conda/__about__.py",
 ]
 
 [tool.coverage.report]
-exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
-]
+fail_under = 0
+show_missing = true
+skip_covered = true
+skip_empty = true
+exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:", "raise NotImplementedError"]
+
+[tool.flake8]
+exclude = [".direnv", ]
+select = ["B","C","E","F","W","B001","B003","B006","B007","B301","B305","B306","B902","Q001","Q002","Q003"]
+ignore = ["E203","E722","W503"]
+max-line-length = 120
```

### Comparing `hatch_conda-0.4.0/PKG-INFO` & `hatch_conda-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-conda
-Version: 0.4.0
+Version: 0.4.1
 Summary: Hatch plugin for conda environments
 Project-URL: History, https://github.com/OldGrumpyViking/hatch-conda/blob/master/HISTORY.md
 Project-URL: Issues, https://github.com/OldGrumpyViking/hatch-conda/issues
 Project-URL: Source, https://github.com/OldGrumpyViking/hatch-conda
 Author-email: OldGrumpyViking <old.grumpy.viking@hotmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

