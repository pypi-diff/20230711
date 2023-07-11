# Comparing `tmp/weblodge-0.1.4.tar.gz` & `tmp/weblodge-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weblodge-0.1.4.tar", max compression
+gzip compressed data, was "weblodge-0.1.5.tar", max compression
```

## Comparing `weblodge-0.1.4.tar` & `weblodge-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1074 2023-07-06 14:06:29.155692 weblodge-0.1.4/LICENSE
--rw-r--r--   0        0        0      614 2023-07-09 07:24:40.785912 weblodge-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5608 2023-07-08 22:55:56.371224 weblodge-0.1.4/README.md
--rw-r--r--   0        0        0       98 2023-07-06 14:06:29.174572 weblodge-0.1.4/weblodge/__main__.py
--rw-r--r--   0        0        0      349 2023-07-06 14:06:29.174572 weblodge-0.1.4/weblodge/_azure/__init__.py
--rw-r--r--   0        0        0     3431 2023-07-06 14:06:29.175573 weblodge-0.1.4/weblodge/_azure/appservice.py
--rw-r--r--   0        0        0     2483 2023-07-08 22:51:06.006012 weblodge-0.1.4/weblodge/_azure/cli.py
--rw-r--r--   0        0        0     2209 2023-07-06 14:06:29.177571 weblodge-0.1.4/weblodge/_azure/resource_group.py
--rw-r--r--   0        0        0     1123 2023-07-06 14:06:29.177571 weblodge-0.1.4/weblodge/_azure/subscription.py
--rw-r--r--   0        0        0     4275 2023-07-08 22:43:38.841236 weblodge-0.1.4/weblodge/_azure/web_app.py
--rw-r--r--   0        0        0      147 2023-07-06 14:06:29.178571 weblodge-0.1.4/weblodge/cli/__init__.py
--rw-r--r--   0        0        0     3259 2023-07-08 22:53:08.396787 weblodge-0.1.4/weblodge/cli/main.py
--rw-r--r--   0        0        0      175 2023-07-06 14:06:29.179570 weblodge-0.1.4/weblodge/config/__init__.py
--rw-r--r--   0        0        0      877 2023-07-06 14:06:29.180572 weblodge-0.1.4/weblodge/config/item.py
--rw-r--r--   0        0        0       92 2023-07-08 22:20:03.486153 weblodge-0.1.4/weblodge/parameters/__init__.py
--rw-r--r--   0        0        0     2466 2023-07-08 22:20:03.486153 weblodge-0.1.4/weblodge/parameters/parameters.py
--rw-r--r--   0        0        0      165 2023-07-06 14:06:29.182572 weblodge-0.1.4/weblodge/state/__init__.py
--rw-r--r--   0        0        0      748 2023-07-06 14:06:29.182572 weblodge-0.1.4/weblodge/state/state.py
--rw-r--r--   0        0        0      202 2023-07-08 22:19:02.555640 weblodge-0.1.4/weblodge/web_app/__init__.py
--rw-r--r--   0        0        0     4728 2023-07-08 22:43:56.400491 weblodge-0.1.4/weblodge/web_app/build.py
--rw-r--r--   0        0        0     1320 2023-07-06 14:06:29.184570 weblodge-0.1.4/weblodge/web_app/delete.py
--rw-r--r--   0        0        0     4165 2023-07-09 07:08:56.772160 weblodge-0.1.4/weblodge/web_app/deploy.py
--rw-r--r--   0        0        0      696 2023-07-08 22:19:02.556642 weblodge-0.1.4/weblodge/web_app/logs.py
--rw-r--r--   0        0        0     1692 2023-07-08 12:32:53.895619 weblodge-0.1.4/weblodge/web_app/web_app.py
--rw-r--r--   0        0        0     7364 1970-01-01 00:00:00.000000 weblodge-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-06 14:06:29.155692 weblodge-0.1.5/LICENSE
+-rw-r--r--   0        0        0      713 2023-07-11 21:51:42.521107 weblodge-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5635 2023-07-11 21:26:46.630621 weblodge-0.1.5/README.md
+-rw-r--r--   0        0        0       98 2023-07-06 14:06:29.174572 weblodge-0.1.5/weblodge/__main__.py
+-rw-r--r--   0        0        0      349 2023-07-06 14:06:29.174572 weblodge-0.1.5/weblodge/_azure/__init__.py
+-rw-r--r--   0        0        0     3431 2023-07-06 14:06:29.175573 weblodge-0.1.5/weblodge/_azure/appservice.py
+-rw-r--r--   0        0        0     2483 2023-07-09 19:00:39.100057 weblodge-0.1.5/weblodge/_azure/cli.py
+-rw-r--r--   0        0        0     2209 2023-07-06 14:06:29.177571 weblodge-0.1.5/weblodge/_azure/resource_group.py
+-rw-r--r--   0        0        0     1123 2023-07-06 14:06:29.177571 weblodge-0.1.5/weblodge/_azure/subscription.py
+-rw-r--r--   0        0        0     4275 2023-07-09 19:00:39.101312 weblodge-0.1.5/weblodge/_azure/web_app.py
+-rw-r--r--   0        0        0      147 2023-07-06 14:06:29.178571 weblodge-0.1.5/weblodge/cli/__init__.py
+-rw-r--r--   0        0        0     3509 2023-07-11 20:05:23.730516 weblodge-0.1.5/weblodge/cli/main.py
+-rw-r--r--   0        0        0      175 2023-07-06 14:06:29.179570 weblodge-0.1.5/weblodge/config/__init__.py
+-rw-r--r--   0        0        0      877 2023-07-06 14:06:29.180572 weblodge-0.1.5/weblodge/config/item.py
+-rw-r--r--   0        0        0       92 2023-07-09 19:00:39.102324 weblodge-0.1.5/weblodge/parameters/__init__.py
+-rw-r--r--   0        0        0     3134 2023-07-11 18:58:24.005879 weblodge-0.1.5/weblodge/parameters/parameters.py
+-rw-r--r--   0        0        0      165 2023-07-06 14:06:29.182572 weblodge-0.1.5/weblodge/state/__init__.py
+-rw-r--r--   0        0        0      748 2023-07-06 14:06:29.182572 weblodge-0.1.5/weblodge/state/state.py
+-rw-r--r--   0        0        0      256 2023-07-11 21:05:52.898919 weblodge-0.1.5/weblodge/web_app/__init__.py
+-rw-r--r--   0        0        0     6328 2023-07-11 21:15:35.831949 weblodge-0.1.5/weblodge/web_app/build.py
+-rw-r--r--   0        0        0     1320 2023-07-06 14:06:29.184570 weblodge-0.1.5/weblodge/web_app/delete.py
+-rw-r--r--   0        0        0     4165 2023-07-09 19:00:39.108261 weblodge-0.1.5/weblodge/web_app/deploy.py
+-rw-r--r--   0        0        0      696 2023-07-08 22:19:02.556642 weblodge-0.1.5/weblodge/web_app/logs.py
+-rw-r--r--   0        0        0     1388 2023-07-11 19:24:32.536898 weblodge-0.1.5/weblodge/web_app/web_app.py
+-rw-r--r--   0        0        0     7490 1970-01-01 00:00:00.000000 weblodge-0.1.5/PKG-INFO
```

### Comparing `weblodge-0.1.4/LICENSE` & `weblodge-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.4/README.md` & `weblodge-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # WebLodge
 
 **WebLodge** is a command line aiming to provide anyone with deployment and cloud management capabilities.
 
-## Prerequisite
+## Prerequisites
 
 - Install the command line with `pip install weblodge`.
 - A Python [Flask](https://flask.palletsprojects.com/en/2.3.x/) application.
 - A `requirements.txt` with the application dependencies. 
 - Have an [Azure account](https://azure.microsoft.com/en-us/free).
 
 > Note: By default, **WebLodge** uses **Free** [Azure services](https://azure.microsoft.com/en-us/pricing/free-services) and lets the user specify non-free configurations.
@@ -61,19 +61,19 @@
 ## Build
 
 The *build* operation collects and prepares the application for deployment on a specific platform.
 
 The *build* operation can handle the following options:
 | Option name | Description | Default value |
 |-|-|-|
-| src | Folder containing application sources. | '.' |
-| dist | Folder containing the application built. | 'dist' |
-| entry-point | The application file to be executed with `python`. | 'app.py' |
-| app | The Flask application object in the `entry-point` file. | 'app' |
-| requirements | The **requirements.txt** file path of the application. This file will be put at the root of the application. | 'requirements.txt' |
+| src | Folder containing application sources. | `.` |
+| dist | Folder containing the application built. | `dist` |
+| entry-point | The application file to be executed with `python`. | `app.py` |
+| app | The Flask application object in the `entry-point` file. | `app` |
+| requirements | The **requirements.txt** file path of the application. Ignores if a `requirements.txt` file is located at the root of the application. | `requirements.txt` |
 
 > Note: Here, the platform is implicitly [Azure App Service](https://azure.microsoft.com/en-us/products/app-service/web).
 
 Example:
 ```
 # Build the local application.
 weblodge build
@@ -85,18 +85,18 @@
 ## Deploy
 
 The *deploy* operation creates the necessary infrastructure and uploads the build package - i.e. your code - on the infrastructure.
 
 | Option name | Description | Default value |
 |-|-|-|
 | app-name | The unique name of the application on the Internet. It will be included in the application URL. | `<randomly generated>` |
-| sku | The application [computational power](https://azure.microsoft.com/en-us/pricing/details/app-service/linux/). | 'F1' |
-| location | The physical application location. | 'northeurope' |
-| environment | The environment of your application. | 'development' |
-| dist | Folder containing the application built. | 'dist' |
+| sku | The application [computational power](https://azure.microsoft.com/en-us/pricing/details/app-service/linux/). | `F1` |
+| location | The physical application location. | `northeurope` |
+| environment | The environment of your application. | `development` |
+| dist | Folder containing the application built. | `dist` |
 
 Example:
 ```
 # Deploy the local application.
 weblodge deploy
 
 # Deploy the local application with a custom name.
@@ -106,15 +106,15 @@
 ## Delete
 
 The *delete* operation deletes the infrastructure deployed but keeps the build.
 
 | Option name | Description | Default value |
 |-|-|-|
 | app-name | The name of the application to be deleted. | `<my-app>` |
-| yes | Do not prompt a validation message before deletion. | 'false' |
+| yes | Do not prompt a validation message before deletion. | `false` |
 
 
 Example:
 ```
 # Delete the application previously deployed.
 weblodge delete
 ```
```

### Comparing `weblodge-0.1.4/weblodge/_azure/appservice.py` & `weblodge-0.1.5/weblodge/_azure/appservice.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.4/weblodge/_azure/cli.py` & `weblodge-0.1.5/weblodge/_azure/cli.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.4/weblodge/_azure/resource_group.py` & `weblodge-0.1.5/weblodge/_azure/resource_group.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.4/weblodge/_azure/subscription.py` & `weblodge-0.1.5/weblodge/_azure/subscription.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.4/weblodge/_azure/web_app.py` & `weblodge-0.1.5/weblodge/_azure/web_app.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.4/weblodge/cli/main.py` & `weblodge-0.1.5/weblodge/cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 # pylint: disable=missing-function-docstring
 def main():
     weblodge = parameters.weblodge()
     config_filename = weblodge.config_filename
 
     config = state.load(config_filename)
-
     if weblodge.action == 'build':
         config = build(config)
     elif weblodge.action == 'deploy':
         config = deploy(config)
     elif weblodge.action == 'delete':
         config = delete(config)
     elif weblodge.action == 'logs':
@@ -39,46 +38,55 @@
     state.dump(config_filename, config)
 
 
 def build(config: Dict[str, str]) -> Dict[str, str]:
     """
     Build the application.
     """
-    logger.info('Building...')
     config = parameters.load(
-        web_app.build_config(),
+        web_app.BuildConfig.items,
         config
     )
-    web_app.build(config)
+
+    logger.info('Building...')
+    build_config = web_app.BuildConfig(**config)
+
+    try:
+        web_app.build(build_config)
+    except web_app.RequirementsFileNotFound:
+        logger.critical(f"Requirements file '{build_config.requirements}' not found.")
+        logger.critical('Build failed.')
+        return config
+
     logger.info('Successfully built.')
     return config
 
 
 def deploy(config: Dict[str, str]) -> Dict[str, str]:
     """
     Deploy the application.
     """
     # The application can be built before being deployed.
-    deploy_can_build = [
+    build_too = [
         ConfigItem(
             name='build',
-            description='Build then deploy the application.',
+            description='Build then deploy the application. Parameters are the same as for the `build` command.',
             attending_value=False
         )
     ]
-    must_build = parameters.load(deploy_can_build, config)
-
-    if must_build.pop('build'):
-        config = build(config)
 
-    logger.info('Deploying...')
     config = parameters.load(
-        web_app.deploy_config(),
+        web_app.deploy_config() + build_too,
         config
     )
+
+    if config['build']:
+        build(config)
+
+    logger.info('Deploying...')
     if webapp_url := web_app.deploy(config):
         logger.info(f"The application will soon be available on: https://{webapp_url}")
     else:
         logger.critical(
             'The application may not be deployed, but the infrastructure may be' \
             f' partially created. You can delete it by running: {parameters.CLI_NAME} delete'
         )
@@ -99,29 +107,29 @@
     )
 
     if not do_not_prompt.get('yes'):
         if input('Are you sure you want to delete the application (yes/no.)? ') != 'yes':
             logger.info('Aborting.')
             return config
 
-    logger.info('Deleting...')
     config = parameters.load(
         web_app.delete_config(),
         config
     )
+    logger.info('Deleting...')
     web_app.delete(config)
     logger.info('Successfully deleted.')
 
     return config
 
 
 def logs(config: Dict[str, str]) -> None:
     """
     Stream application logs.
     """
-    logger.warning('Logs will be stream, execute CTRL+C to stop the application.')
-    logger.info('Recovering logs...')
     config = parameters.load(
         web_app.logs_config(),
         config
     )
+    logger.warning('Logs will be stream, execute CTRL+C to stop the application.')
+    logger.info('Recovering logs...')
     web_app.logs(config)
```

### Comparing `weblodge-0.1.4/weblodge/config/item.py` & `weblodge-0.1.5/weblodge/config/item.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.4/weblodge/parameters/parameters.py` & `weblodge-0.1.5/weblodge/parameters/parameters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 """
 User inputs can be provided by command line.
 This package contains the logic to parse the command line arguments for internal
 components based on the configuration items. but also the global arguments that are
 hard coded.
+
+The help method must be adapted to the action to be carried out.
+Examples:
+    `python weblodge.py -h` must print the `help` message of **WebLodge**.
+    `python weblodge.py build -h` must print the `help` message for the `build` action.
 """
 import sys
 import argparse
 from dataclasses import dataclass
 from typing import Dict, List
 
 from weblodge.config import Item as ConfigItem
@@ -27,16 +32,23 @@
     config_filename: str = '.weblodge.json'
 
 
 def weblodge() -> str:
     """
     Return the action to perform.
     """
+    # If run user run: `python weblodge.py -h` or `python weblodge.py --help`
+    # then we want to display the **WebLodge** `help` message.
+    # Otherwise, we want to parse the arguments and better scope the help message.
+    # Example: `python weblodge.py build -h` must print the `help` message for the `build` action.
+    asking_global_help = len(sys.argv) == 2 and '-h' in sys.argv[1]
+
     parser = argparse.ArgumentParser(
-        description='Deploy a Python Flask-based application to Azure.'
+        description='Deploy a Python Flask-based application to Azure.',
+        add_help=asking_global_help
     )
     parser.add_argument(
         'action',
         type=str,
         help='Action to perform.',
         choices=['build', 'deploy', 'delete', 'logs']
     )
```

### Comparing `weblodge-0.1.4/weblodge/state/state.py` & `weblodge-0.1.5/weblodge/state/state.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.4/weblodge/web_app/build.py` & `weblodge-0.1.5/weblodge/web_app/build.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,144 +5,204 @@
 - The user application code.
 - The user application requirements.
 - A generated Kudu deployment configuration file.
 - A generated startup file.
 
 This package is ready to be deployed on an Azure Web App.
 """
-from dataclasses import dataclass
 import os
 from pathlib import Path
 from typing import List
 import zipfile
 
 from weblodge.config import Item as ConfigItem
 
 
-@dataclass(frozen=True)
-class Build:
+class BuildException(Exception):
     """
-    Facade to the build process.
+    Build exception.
+    """
+
+
+class RequirementsFileNotFound(BuildException):
+    """
+    The requirements file was not found.
+    """
+
+
+class BuildConfig:
+    """
+    Build configuration.
 
     User-customizable fields are found in the `config` property. All are optional from the user's
     point of view so build can proceed without any configuration.
     """
-    # Source directory to zip.
-    src: str = '.'
-    # Destination directory to the zip file `name`.
-    dist: str = 'dist'
-    # Application entrypoint.
-    entry_point: str = 'app.py'
-    # Flask application object.
-    app: str = 'app'
-
     # Zip file that contains the user application code.
     package: str = 'azwebapp.zip'
     # Kudu deployment config file.
     kudu_config: str = '.deployment'
     # Startup file.
     # Set in the deployment config too.
     startup_file: str = 'weblodge.startup'
+    # Kudu needs a requirements file at the root of the zip.
+    kudu_requirements_path = 'requirements.txt'
+
+    # pylint: disable=too-many-arguments
+    def __init__(
+        self,
+        src: str,
+        dist: str,
+        entry_point: str,
+        app: str,
+        requirements: str,
+        *_args,
+        **_kwargs
+    ):
+        # Source directory to zip.
+        self.src = src
+        # Destination directory to the zip file `name`.
+        self.dist = dist
+        # Application entrypoint.
+        self.entry_point = entry_point
+        # Flask application object.
+        self.app = app
+        # User requirements file.
+        self.requirements = requirements
 
     @property
     def package_path(self) -> str:
         """
         Return the package path.
         """
         return os.path.join(self.dist, self.package)
 
     @classmethod
     @property
-    def config(cls) -> List[ConfigItem]:
+    def items(cls) -> List[ConfigItem]:
         """
-        Return the build configuration.
+        Items that can be configured.
         """
         return [
             ConfigItem(
                 name='src',
                 description='Application folder.',
-                default=cls.src
+                default='.'
             ),
             ConfigItem(
                 name='dist',
                 description='Build destination.',
-                default=cls.dist
+                default='dist'
             ),
             ConfigItem(
                 name='entry_point',
                 description='Application entry point.',
-                default=cls.entry_point
+                default='app.py'
             ),
             ConfigItem(
                 name='app',
                 description='Flask Application object.',
-                default=cls.app
+                default='app'
+            ),
+            ConfigItem(
+                name='requirements',
+                description='Requirements.txt file path.',
+                default='requirements.txt'
             )
         ]
 
-    def build(self) -> None:
-        """
-        Build an application to a deployable format.
-        """
-        # Create the destination directory.
-        os.makedirs(self.dist, exist_ok=True)
 
-        # Zip all required files together.
-        with zipfile.ZipFile(self.package_path, 'w', zipfile.ZIP_DEFLATED) as zipf:
-            self._zip_user_application(zipf)
-            self._deployment_config(zipf)
-            self._startup_file(zipf)
+def build(config: BuildConfig) -> None:
+    """
+    Build an application to a deployable format.
+    """
+    # Create the destination directory.
+    os.makedirs(config.dist, exist_ok=True)
+
+    # Zip all required files together.
+    with zipfile.ZipFile(config.package_path, 'w', zipfile.ZIP_DEFLATED) as zipf:
+        requirements_file_included = _zip_user_application(config, zipf)
+        _deployment_config(config, zipf)
+        _startup_file(config, zipf)
 
-    def _zip_user_application(self, zipf: zipfile.ZipFile):
-        """
-        Create the zip folder.
-        """
-        for root, _, files in os.walk(self.src):
-            root = Path(root)
-            # Skip hidden files and directories.
-            if root.name.startswith('.'):
-                continue
-            # Skip bytecode files.
-            if '__pycache__' in root.name:
-                continue
-            # Skip the build directory.
-            # Path conversion removes unnecessary slashes.
-            if root.name.startswith(Path(self.dist).name):
-                continue
-            # Zip the files.
-            for file in files:
-                file_path = root / file
-                relative_to = os.path.relpath(file_path, self.src)
-                zipf.write(file_path, relative_to)
+        # Add the requirements file if it was not included in the user application folder.
+        if not requirements_file_included:
+            _requirements(config, zipf)
 
-    def _deployment_config(self, zipf: zipfile.ZipFile):
-        """
-        Add the deployment config file to the zip folder.
-        """
-        # Kudu deployment config file.
-        config = '''\
+
+def _zip_user_application(config: BuildConfig, zipf: zipfile.ZipFile) -> bool:
+    """
+    Create the zip folder.
+
+    Return True if the requirements file was included at the root of the application folder.
+    """
+    requirements_file_included = False
+
+    for root, _, files in os.walk(config.src):
+        root = Path(root)
+        # Skip hidden files and directories.
+        if root.name.startswith('.'):
+            continue
+        # Skip bytecode files.
+        if '__pycache__' in root.name:
+            continue
+        # Skip the build directory.
+        # Path conversion removes unnecessary slashes.
+        if root.name.startswith(Path(config.dist).name):
+            continue
+        # Zip the files.
+        for file in files:
+            file_path = root / file
+            relative_to = os.path.relpath(file_path, config.src)
+
+            zipf.write(file_path, relative_to)
+
+            if not requirements_file_included:
+                # If the requirements file is not already included at the root of the application
+                # folder, check if the current file is that one.
+                requirements_file_included = Path(relative_to) == Path(config.kudu_requirements_path)
+
+    return requirements_file_included
+
+
+def _requirements(config: BuildConfig, zipf: zipfile.ZipFile):
+    """
+    Add the requirements file to the zip folder from the user folder.
+    """
+    if not os.path.exists(config.requirements):
+        raise RequirementsFileNotFound()
+
+    zipf.write(config.requirements, config.kudu_requirements_path)
+
+
+def _deployment_config(config: BuildConfig, zipf: zipfile.ZipFile):
+    """
+    Add the deployment config file to the zip folder.
+    """
+    # Kudu deployment config file.
+    kudu_config = '''\
 [config]
 # Packages must be installed using during the deployment build.
 SCM_DO_BUILD_DURING_DEPLOYMENT = true
 '''
-        # Add the deployment config file to the zip folder.
-        zipf.writestr(self.kudu_config, config)
+    # Add the deployment config file to the zip folder.
+    zipf.writestr(config.kudu_config, kudu_config)
 
-    def _startup_file(self, zipf: zipfile.ZipFile):
-        """
-        Add the startup file to the zip folder.
-        """
-        # Remove potentional .py extension.
-        entrypoint = self.entry_point
-        if entrypoint.endswith('.py'):
-            entrypoint = entrypoint[:-3]
-
-        # Add the application object if it's not already there.
-        if ':' not in entrypoint:
-            entrypoint = f'{entrypoint}:{self.app}'
-
-        # Default application configuration update with the user and entrypoint.
-        # https://learn.microsoft.com/en-us/azure/developer/python/configure-python-web-app-on-app-service
-        startup_file_content = f'gunicorn --bind=0.0.0.0 --timeout 600 {entrypoint}'
 
-        # Add the startup file to the zip folder.
-        zipf.writestr(self.startup_file, startup_file_content)
+def _startup_file(config: BuildConfig, zipf: zipfile.ZipFile):
+    """
+    Add the startup file to the zip folder.
+    """
+    # Remove potentional .py extension.
+    entrypoint = config.entry_point
+    if entrypoint.endswith('.py'):
+        entrypoint = entrypoint[:-3]
+
+    # Add the application object if it's not already there.
+    if ':' not in entrypoint:
+        entrypoint = f'{entrypoint}:{config.app}'
+
+    # Default application configuration update with the user and entrypoint.
+    # https://learn.microsoft.com/en-us/azure/developer/python/configure-python-web-app-on-app-service
+    startup_file_content = f'gunicorn --bind=0.0.0.0 --timeout 600 {entrypoint}'
+
+    # Add the startup file to the zip folder.
+    zipf.writestr(config.startup_file, startup_file_content)
```

### Comparing `weblodge-0.1.4/weblodge/web_app/delete.py` & `weblodge-0.1.5/weblodge/web_app/delete.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.4/weblodge/web_app/deploy.py` & `weblodge-0.1.5/weblodge/web_app/deploy.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.4/weblodge/web_app/logs.py` & `weblodge-0.1.5/weblodge/web_app/logs.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.4/weblodge/web_app/web_app.py` & `weblodge-0.1.5/weblodge/web_app/web_app.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Web App function to simplify the build, deploy and delete process.
 """
 import functools
 from typing import List, Dict
 
 from weblodge.config import Item as ConfigItem
 
-from .build import Build
 from .deploy import Deploy
 from .delete import Delete
 
 
 # pylint: disable=missing-function-docstring
 def filter_config(retrieve_config):
     def _filter_config(func) -> Dict[str, str]:
@@ -20,29 +19,14 @@
                 k: v for k, v in config.items() if k in retrieve_config()
             }
             return func(_config)
         return __filter_config
     return _filter_config
 
 
-def build_config() -> List[ConfigItem]:
-    """
-    Return the build configuration.
-    """
-    return Build.config
-
-
-@filter_config(build_config)
-def build(config: Dict[str, str]) -> None:
-    """
-    Build the application from the config.
-    """
-    Build(**config).build()
-
-
 def deploy_config() -> List[ConfigItem]:
     """
     Return the deployment configuration.
     """
     return Deploy.config
```

### Comparing `weblodge-0.1.4/PKG-INFO` & `weblodge-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: weblodge
-Version: 0.1.4
-Summary: 
+Version: 0.1.5
+Summary: A simple command line aiming to provide anyone with deployment and cloud management capabilities.
 Home-page: https://github.com/florian-vuillemot/weblodge
 Keywords: deployment,azure
 Author: Vuillemot Florian
 Author-email: vuillemot.florian@outlook.fr
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: azure-cli (==2.49)
+Requires-Dist: azure-cli (==2.50.0)
 Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
 Project-URL: Repository, https://github.com/florian-vuillemot/weblodge
 Description-Content-Type: text/markdown
 
 # WebLodge
 
 **WebLodge** is a command line aiming to provide anyone with deployment and cloud management capabilities.
 
-## Prerequisite
+## Prerequisites
 
 - Install the command line with `pip install weblodge`.
 - A Python [Flask](https://flask.palletsprojects.com/en/2.3.x/) application.
 - A `requirements.txt` with the application dependencies. 
 - Have an [Azure account](https://azure.microsoft.com/en-us/free).
 
 > Note: By default, **WebLodge** uses **Free** [Azure services](https://azure.microsoft.com/en-us/pricing/free-services) and lets the user specify non-free configurations.
@@ -80,19 +80,19 @@
 ## Build
 
 The *build* operation collects and prepares the application for deployment on a specific platform.
 
 The *build* operation can handle the following options:
 | Option name | Description | Default value |
 |-|-|-|
-| src | Folder containing application sources. | '.' |
-| dist | Folder containing the application built. | 'dist' |
-| entry-point | The application file to be executed with `python`. | 'app.py' |
-| app | The Flask application object in the `entry-point` file. | 'app' |
-| requirements | The **requirements.txt** file path of the application. This file will be put at the root of the application. | 'requirements.txt' |
+| src | Folder containing application sources. | `.` |
+| dist | Folder containing the application built. | `dist` |
+| entry-point | The application file to be executed with `python`. | `app.py` |
+| app | The Flask application object in the `entry-point` file. | `app` |
+| requirements | The **requirements.txt** file path of the application. Ignores if a `requirements.txt` file is located at the root of the application. | `requirements.txt` |
 
 > Note: Here, the platform is implicitly [Azure App Service](https://azure.microsoft.com/en-us/products/app-service/web).
 
 Example:
 ```
 # Build the local application.
 weblodge build
@@ -104,18 +104,18 @@
 ## Deploy
 
 The *deploy* operation creates the necessary infrastructure and uploads the build package - i.e. your code - on the infrastructure.
 
 | Option name | Description | Default value |
 |-|-|-|
 | app-name | The unique name of the application on the Internet. It will be included in the application URL. | `<randomly generated>` |
-| sku | The application [computational power](https://azure.microsoft.com/en-us/pricing/details/app-service/linux/). | 'F1' |
-| location | The physical application location. | 'northeurope' |
-| environment | The environment of your application. | 'development' |
-| dist | Folder containing the application built. | 'dist' |
+| sku | The application [computational power](https://azure.microsoft.com/en-us/pricing/details/app-service/linux/). | `F1` |
+| location | The physical application location. | `northeurope` |
+| environment | The environment of your application. | `development` |
+| dist | Folder containing the application built. | `dist` |
 
 Example:
 ```
 # Deploy the local application.
 weblodge deploy
 
 # Deploy the local application with a custom name.
@@ -125,15 +125,15 @@
 ## Delete
 
 The *delete* operation deletes the infrastructure deployed but keeps the build.
 
 | Option name | Description | Default value |
 |-|-|-|
 | app-name | The name of the application to be deleted. | `<my-app>` |
-| yes | Do not prompt a validation message before deletion. | 'false' |
+| yes | Do not prompt a validation message before deletion. | `false` |
 
 
 Example:
 ```
 # Delete the application previously deployed.
 weblodge delete
 ```
```

