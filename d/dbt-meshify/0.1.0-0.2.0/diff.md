# Comparing `tmp/dbt_meshify-0.1.0.tar.gz` & `tmp/dbt_meshify-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_meshify-0.1.0.tar", max compression
+gzip compressed data, was "dbt_meshify-0.2.0.tar", max compression
```

## Comparing `dbt_meshify-0.1.0.tar` & `dbt_meshify-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    11356 2023-06-13 20:19:11.610541 dbt_meshify-0.1.0/LICENSE
--rw-r--r--   0        0        0     1346 2023-06-13 20:19:11.610541 dbt_meshify-0.1.0/README.md
--rw-r--r--   0        0        0       11 2023-06-13 20:19:11.610541 dbt_meshify-0.1.0/dbt_meshify/.gitignore
--rw-r--r--   0        0        0        0 2023-06-13 20:19:11.610541 dbt_meshify-0.1.0/dbt_meshify/__init__.py
--rw-r--r--   0        0        0       92 2023-06-13 20:19:11.610541 dbt_meshify-0.1.0/dbt_meshify/cli.py
--rw-r--r--   0        0        0     1762 2023-06-13 20:19:11.610541 dbt_meshify-0.1.0/dbt_meshify/dbt.py
--rw-r--r--   0        0        0    10456 2023-06-13 20:19:11.610541 dbt_meshify-0.1.0/dbt_meshify/dbt_projects.py
--rw-r--r--   0        0        0     5224 2023-06-13 20:19:11.610541 dbt_meshify-0.1.0/dbt_meshify/linker.py
--rw-r--r--   0        0        0     7197 2023-06-13 20:19:11.610541 dbt_meshify-0.1.0/dbt_meshify/main.py
--rw-r--r--   0        0        0        0 2023-06-13 20:19:11.610541 dbt_meshify-0.1.0/dbt_meshify/storage/__init__.py
--rw-r--r--   0        0        0     2098 2023-06-13 20:19:11.610541 dbt_meshify-0.1.0/dbt_meshify/storage/file_manager.py
--rw-r--r--   0        0        0    11349 2023-06-13 20:19:11.610541 dbt_meshify-0.1.0/dbt_meshify/storage/yaml_editors.py
--rw-r--r--   0        0        0        0 2023-06-13 20:19:11.610541 dbt_meshify-0.1.0/dbt_meshify/utilities/__init__.py
--rw-r--r--   0        0        0     5592 2023-06-13 20:19:11.610541 dbt_meshify-0.1.0/dbt_meshify/utilities/grouper.py
--rw-r--r--   0        0        0     1115 2023-06-13 20:19:11.610541 dbt_meshify-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2097 1970-01-01 00:00:00.000000 dbt_meshify-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-07-11 00:33:03.838344 dbt_meshify-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1348 2023-07-11 00:33:03.838344 dbt_meshify-0.2.0/README.md
+-rw-r--r--   0        0        0       11 2023-07-11 00:33:03.838344 dbt_meshify-0.2.0/dbt_meshify/.gitignore
+-rw-r--r--   0        0        0        0 2023-07-11 00:33:03.838344 dbt_meshify-0.2.0/dbt_meshify/__init__.py
+-rw-r--r--   0        0        0     2282 2023-07-11 00:33:03.838344 dbt_meshify-0.2.0/dbt_meshify/cli.py
+-rw-r--r--   0        0        0     1902 2023-07-11 00:33:03.838344 dbt_meshify-0.2.0/dbt_meshify/dbt.py
+-rw-r--r--   0        0        0    14329 2023-07-11 00:33:03.838344 dbt_meshify-0.2.0/dbt_meshify/dbt_projects.py
+-rw-r--r--   0        0        0     5224 2023-07-11 00:33:03.838344 dbt_meshify-0.2.0/dbt_meshify/linker.py
+-rw-r--r--   0        0        0     8814 2023-07-11 00:33:03.838344 dbt_meshify-0.2.0/dbt_meshify/main.py
+-rw-r--r--   0        0        0        0 2023-07-11 00:33:03.838344 dbt_meshify-0.2.0/dbt_meshify/storage/__init__.py
+-rw-r--r--   0        0        0    10781 2023-07-11 00:33:03.838344 dbt_meshify-0.2.0/dbt_meshify/storage/dbt_project_creator.py
+-rw-r--r--   0        0        0    20063 2023-07-11 00:33:03.838344 dbt_meshify-0.2.0/dbt_meshify/storage/file_content_editors.py
+-rw-r--r--   0        0        0     3206 2023-07-11 00:33:03.838344 dbt_meshify-0.2.0/dbt_meshify/storage/file_manager.py
+-rw-r--r--   0        0        0        0 2023-07-11 00:33:03.838344 dbt_meshify-0.2.0/dbt_meshify/utilities/__init__.py
+-rw-r--r--   0        0        0     6788 2023-07-11 00:33:03.838344 dbt_meshify-0.2.0/dbt_meshify/utilities/grouper.py
+-rw-r--r--   0        0        0     1133 2023-07-11 00:33:03.842344 dbt_meshify-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 dbt_meshify-0.2.0/PKG-INFO
```

### Comparing `dbt_meshify-0.1.0/LICENSE` & `dbt_meshify-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_meshify-0.1.0/README.md` & `dbt_meshify-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 
 ## Basic Usage
 
 ```bash
 # create a group of all models tagged with "finance"
 # leaf nodes and nodes with cross-group dependencies will be `public`
 # public nodes will also have contracts added to them
-dbt-meshify group finance --owner name Monopoly Man -s +tag:finance
+dbt-meshify group finance --owner-name "Monopoly Man" -s +tag:finance
 
 # optionally use the add-version operation to add a new version to a model
 dbt-meshify operation add-version -s fct_orders
 ```
```

### Comparing `dbt_meshify-0.1.0/dbt_meshify/dbt.py` & `dbt_meshify-0.2.0/dbt_meshify/dbt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # third party
 import os
 from typing import List, Optional
 
 from dbt.cli.main import dbtRunner
 from dbt.contracts.graph.manifest import Manifest
 from dbt.contracts.results import CatalogArtifact
+from loguru import logger
 
 
 class Dbt:
     def __init__(self, manifest: Optional[Manifest] = None):
         self.dbt_runner = dbtRunner(manifest=manifest)  # type: ignore
 
     def invoke(
@@ -21,14 +22,15 @@
         os.chdir(starting_directory)
 
         if not result.success and result.exception:
             raise result.exception
         return result.result
 
     def parse(self, directory: os.PathLike):
+        logger.info("Executing dbt parse...")
         return self.invoke(directory, ["--quiet", "parse"])
 
     def ls(
         self,
         directory: os.PathLike,
         arguments: Optional[List[str]] = None,
         output_key: Optional[str] = None,
@@ -46,9 +48,10 @@
 
         return self.invoke(directory, args)
 
     def docs_generate(self, directory: os.PathLike) -> CatalogArtifact:
         """
         Excute dbt docs generate with the given arguments
         """
+        logger.info("Generating catalog with dbt docs generate...")
         args = ["--quiet", "docs", "generate"]
         return self.invoke(directory, args)
```

### Comparing `dbt_meshify-0.1.0/dbt_meshify/dbt_projects.py` & `dbt_meshify-0.2.0/dbt_meshify/dbt_projects.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,38 @@
 import copy
 import hashlib
 import json
-import logging
 import os
 from pathlib import Path
 from typing import Any, Dict, MutableMapping, Optional, Set, Union
 
 import yaml
 from dbt.contracts.graph.manifest import Manifest
-from dbt.contracts.graph.nodes import ManifestNode, ModelNode, SourceDefinition
+from dbt.contracts.graph.nodes import (
+    Documentation,
+    Exposure,
+    Group,
+    Macro,
+    ManifestNode,
+    ModelNode,
+    Resource,
+    SourceDefinition,
+)
 from dbt.contracts.project import Project
 from dbt.contracts.results import CatalogArtifact, CatalogTable
 from dbt.graph import Graph
+from dbt.node_types import NodeType
+from loguru import logger
 
 from dbt_meshify.dbt import Dbt
-
-logger = logging.getLogger()
+from dbt_meshify.storage.file_content_editors import (
+    DbtMeshConstructor,
+    filter_empty_dict_items,
+)
+from dbt_meshify.storage.file_manager import DbtFileManager
 
 
 class BaseDbtProject:
     """A base-level representation of a dbt project."""
 
     def __init__(
         self,
@@ -96,15 +109,16 @@
         project_packages = []
         for key in ["nodes", "sources", "exposures", "metrics", "sources", "macros"]:
             items = getattr(self.manifest, key)
             for key, item in items.items():
                 if item.package_name:
                     _hash = hashlib.md5()
                     _hash.update(item.package_name.encode("utf-8"))
-                    project_packages.append(_hash.hexdigest())
+                    if _hash.hexdigest() != self.manifest.metadata.project_id:
+                        project_packages.append(_hash.hexdigest())
         return set(project_packages)
 
     @property
     def project_id(self) -> Optional[str]:
         return self.manifest.metadata.project_id
 
     def installs(self, other) -> bool:
@@ -146,36 +160,61 @@
         """
         return self.installs(other) or self.shares_source_metadata(other)
 
     def get_catalog_entry(self, unique_id: str) -> Optional[CatalogTable]:
         """Returns the catalog entry for a model in the dbt project's catalog"""
         return self.catalog.nodes.get(unique_id)
 
-    def get_manifest_node(self, unique_id: str) -> Optional[ManifestNode]:
-        """Returns the catalog entry for a model in the dbt project's catalog"""
-        return self.manifest.nodes.get(unique_id)
+    def get_manifest_node(self, unique_id: str) -> Optional[Resource]:
+        """Returns the manifest entry for a resource in the dbt project's manifest"""
+        if unique_id.split(".")[0] in [
+            "model",
+            "seed",
+            "snapshot",
+            "test",
+            "analysis",
+            "snapshot",
+        ]:
+            return self.manifest.nodes.get(unique_id)
+        pluralized = NodeType(unique_id.split(".")[0]).pluralize()
+        resources = getattr(self.manifest, pluralized)
+        return resources.get(unique_id)
 
 
 class DbtProject(BaseDbtProject):
     @staticmethod
     def _load_project(path) -> Project:
         """Load a dbt Project configuration"""
         project_dict = yaml.load(open(os.path.join(path, "dbt_project.yml")), Loader=yaml.Loader)
         return Project.from_dict(project_dict)
 
     @classmethod
-    def from_directory(cls, directory: os.PathLike) -> "DbtProject":
+    def from_directory(cls, directory: os.PathLike, read_catalog: bool) -> "DbtProject":
         """Create a new DbtProject using a dbt project directory"""
 
         dbt = Dbt()
+        project = cls._load_project(directory)
+
+        def get_catalog(directory: os.PathLike, read_catalog: bool) -> CatalogArtifact:
+            catalog_path = Path(directory) / (project.target_path or "target") / "catalog.json"
+            if read_catalog:
+                logger.info(f"Reading catalog from {catalog_path}")
+                try:
+                    catalog_dict = json.loads(catalog_path.read_text())
+                    return CatalogArtifact.from_dict(catalog_dict)
+                except FileNotFoundError:
+                    logger.info(f"Catalog not found at {catalog_path}, running dbt docs generate")
+                    return dbt.docs_generate(directory)
+            else:
+                return dbt.docs_generate(directory)
 
         return DbtProject(
             manifest=dbt.parse(directory),
-            project=cls._load_project(directory),
-            catalog=dbt.docs_generate(directory),
+            project=project,
+            catalog=get_catalog(directory, read_catalog),
             dbt=dbt,
             path=Path(directory),
         )
 
     def __init__(
         self,
         manifest: Manifest,
@@ -212,18 +251,21 @@
         return set(results)
 
     def split(
         self,
         project_name: str,
         select: str,
         exclude: Optional[str] = None,
+        selector: Optional[str] = None,
     ) -> "DbtSubProject":
         """Create a new DbtSubProject using NodeSelection syntax."""
 
-        subproject_resources = self.select_resources(select, exclude)
+        subproject_resources = self.select_resources(
+            select=select, exclude=exclude, selector=selector, output_key="unique_id"
+        )
 
         # Construct a new project and inject the new manifest
         subproject = DbtSubProject(
             name=project_name, parent_project=copy.deepcopy(self), resources=subproject_resources
         )
 
         # Record the subproject to create a cross-project dependency edge list
@@ -238,32 +280,94 @@
     a parent DbtProject for their manifest and project definitions until a real DbtProject
     is created on disk.
     """
 
     def __init__(self, name: str, parent_project: DbtProject, resources: Set[str]):
         self.name = name
         self.resources = resources
-        self.parent = parent_project
+        self.parent_project = parent_project
+        self.path = parent_project.path / Path(name)
 
-        self.manifest = parent_project.manifest.deepcopy()
+        # self.manifest = parent_project.manifest.deepcopy()
+        # i am running into a bug with the core deepcopy -- checking with michelle
+        self.manifest = copy.deepcopy(parent_project.manifest)
         self.project = copy.deepcopy(parent_project.project)
         self.catalog = parent_project.catalog
+        self.custom_macros = self._get_custom_macros()
+        self.groups = self._get_indirect_groups()
 
-        super().__init__(self.manifest, self.project, self.catalog)
+        self._rename_project()
 
-    def select_resources(self, select: str, exclude: Optional[str] = None) -> Set[str]:
+        super().__init__(self.manifest, self.project, self.catalog, self.name)
+
+    def _rename_project(self) -> None:
+        """
+        edits the project yml to take any instance of the parent project name and update it to the subproject name
+        """
+        project_dict = self.project.to_dict()
+        for key in [resource.pluralize() for resource in NodeType]:
+            if self.parent_project.name in project_dict.get(key, {}).keys():
+                project_dict[key][self.name] = project_dict[key].pop(self.parent_project.name)
+        project_dict["name"] = self.name
+        self.project = Project.from_dict(project_dict)
+
+    def _get_custom_macros(self) -> Set[str]:
+        """
+        get a set of macro unique_ids for all the selected resources
+        """
+        macros_set = set()
+        for unique_id in self.resources:
+            resource = self.get_manifest_node(unique_id)
+            if not resource or any(
+                isinstance(resource, class_) for class_ in [Documentation, Group]
+            ):
+                continue
+            macros = resource.depends_on.macros  # type: ignore
+            project_macros = [
+                macro
+                for macro in macros
+                if hashlib.md5((macro.split(".")[1]).encode()).hexdigest()
+                == self.manifest.metadata.project_id
+            ]
+            macros_set.update(project_macros)
+        return macros_set
+
+    def _get_indirect_groups(self) -> Set[str]:
+        """
+        get a set of group unique_ids for all the selected resources
+        """
+        groups = set()
+        for unique_id in self.resources:
+            resource = self.get_manifest_node(unique_id)  # type: ignore
+            if not resource or any(
+                isinstance(resource, class_)
+                for class_ in [Documentation, Group, Exposure, SourceDefinition, Macro]
+            ):
+                continue
+            group = resource.group  # type: ignore
+            if group:
+                group_unique_id = f"group.{self.parent_project.name}.{group}"
+                groups.update({group_unique_id})
+        return groups
+
+    def select_resources(
+        self,
+        select: str,
+        exclude: Optional[str] = None,
+        selector: Optional[str] = None,
+        output_key: Optional[str] = None,
+    ) -> Set[str]:
         """
         Select resources using the parent DbtProject and filtering down to only include resources in this
         subproject.
         """
-        args = ["--select", select]
-        if exclude:
-            args.extend(["--exclude", exclude])
 
-        results = self.parent.dbt.ls(self.parent.path, args)
+        results = self.parent_project.select_resources(
+            select=select, exclude=exclude, selector=selector, output_key=output_key
+        )
 
         return set(results) - self.resources
 
     def split(
         self,
         project_name: str,
         select: str,
@@ -272,30 +376,23 @@
         """Create a new DbtSubProject using NodeSelection syntax."""
 
         subproject_resources = self.select_resources(select, exclude)
 
         # Construct a new project and inject the new manifest
         subproject = DbtSubProject(
             name=project_name,
-            parent_project=copy.deepcopy(self.parent),
+            parent_project=copy.deepcopy(self.parent_project),
             resources=subproject_resources,
         )
 
         # Record the subproject to create a cross-project dependency edge list
         self.register_relationship(project_name, subproject_resources)
 
         return subproject
 
-    def initialize(self, target_directory: os.PathLike):
-        """Initialize this subproject as a full dbt project at the provided `target_directory`."""
-
-        # TODO: Implement project initialization
-
-        raise NotImplementedError
-
 
 class DbtProjectHolder:
     def __init__(self) -> None:
         self.projects: Dict[str, BaseDbtProject] = {}
 
     def project_map(self) -> dict:
         return self.projects
```

### Comparing `dbt_meshify-0.1.0/dbt_meshify/linker.py` & `dbt_meshify-0.2.0/dbt_meshify/linker.py`

 * *Files identical despite different names*

### Comparing `dbt_meshify-0.1.0/dbt_meshify/main.py` & `dbt_meshify-0.2.0/dbt_meshify/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,48 @@
 import os
+import sys
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Optional
 
 import click
+import yaml
 from dbt.contracts.graph.unparsed import Owner
+from loguru import logger
 
-from .dbt_projects import DbtProject, DbtProjectHolder, DbtSubProject
-from .storage.yaml_editors import DbtMeshModelConstructor
+from dbt_meshify.storage.dbt_project_creator import DbtSubprojectCreator
 
-# define common parameters
-project_path = click.option(
-    "--project-path",
-    type=click.Path(exists=True),
-    default=".",
-    help="The path to the dbt project to operate on. Defaults to the current directory.",
+from .cli import (
+    create_path,
+    exclude,
+    group_yml_path,
+    owner,
+    owner_email,
+    owner_name,
+    owner_properties,
+    project_path,
+    read_catalog,
+    select,
+    selector,
 )
+from .dbt_projects import DbtProject, DbtProjectHolder, DbtSubProject
+from .storage.file_content_editors import DbtMeshConstructor
 
-exclude = click.option(
-    "--exclude",
-    "-e",
-    default=None,
-    help="The dbt selection syntax specifying the resources to exclude in the operation",
-)
+log_format = "<white>{time:HH:mm:ss}</white> | <level>{level}</level> | <level>{message}</level>"
+logger.remove()  # Remove the default sink added by Loguru
+logger.add(sys.stdout, format=log_format)
 
-group_yml_path = click.option(
-    "--group-yml-path",
-    type=click.Path(exists=False),
-    help="An optional path to store the new group YAML definition.",
-)
 
-select = click.option(
-    "--select",
-    "-s",
-    default=None,
-    help="The dbt selection syntax specifying the resources to include in the operation",
-)
+class FatalMeshifyException(click.ClickException):
+    def __init__(self, message):
+        super().__init__(message)
 
-owner = click.option(
-    "--owner",
-    nargs=2,
-    multiple=True,
-    type=click.Tuple([str, str]),
-    help="A tuple of Owner information for the group. For example " "`--owner name example`",
-)
-
-selector = click.option(
-    "--selector",
-    default=None,
-    help="The name of the YML selector specifying the resources to include in the operation",
-)
+    def show(self):
+        logger.error(self.message)
+        if self.__cause__ is not None:
+            logger.exception(self.__cause__)
 
 
 # define cli group
 @click.group()
 def cli():
     pass
 
@@ -78,177 +68,213 @@
 
     while True:
         path_string = input("Enter the relative path to a dbt project (enter 'done' to finish): ")
         if path_string == "done":
             break
 
         path = Path(path_string).expanduser().resolve()
-        project = DbtProject.from_directory(path)
+        project = DbtProject.from_directory(path, read_catalog)
         holder.register_project(project)
 
     print(holder.project_map())
 
 
 @cli.command(name="split")
+@create_path
+@click.argument("project_name")
 @exclude
 @project_path
+@read_catalog
 @select
 @selector
-def split():
+def split(project_name, select, exclude, project_path, selector, create_path, read_catalog):
     """
-    !!! info
-        This command is not yet implemented
-
-    Splits dbt projects apart by adding all necessary dbt Mesh constructs based on the selection syntax.
+    Splits out a new subproject from a dbt project by adding all necessary dbt Mesh constructs to the resources based on the selected resources.
 
     """
-    path_string = input("Enter the relative path to a dbt project you'd like to split: ")
-
-    holder = DbtProjectHolder()
-
-    path = Path(path_string).expanduser().resolve()
-    project = DbtProject.from_directory(path)
-    holder.register_project(project)
-
-    while True:
-        subproject_name = input("Enter the name for your subproject ('done' to finish): ")
-        if subproject_name == "done":
-            break
-        subproject_selector = input(
-            f"Enter the selector that represents the subproject {subproject_name}: "
-        )
-
-        subproject: DbtSubProject = project.split(
-            project_name=subproject_name, select=subproject_selector
-        )
-        holder.register_project(subproject)
+    path = Path(project_path).expanduser().resolve()
+    project = DbtProject.from_directory(path, read_catalog)
 
-    print(holder.project_map())
+    subproject = project.split(
+        project_name=project_name, select=select, exclude=exclude, selector=selector
+    )
+    logger.info(f"Selected {len(subproject.resources)} resources: {subproject.resources}")
+    target_directory = Path(create_path) if create_path else None
+    subproject_creator = DbtSubprojectCreator(
+        subproject=subproject, target_directory=target_directory
+    )
+    logger.info(f"Creating subproject {subproject.name}...")
+    try:
+        subproject_creator.initialize()
+        logger.success(f"Successfully created subproject {subproject.name}")
+    except Exception as e:
+        raise FatalMeshifyException(f"Error creating subproject {subproject.name}")
 
 
 @operation.command(name="add-contract")
 @exclude
 @project_path
+@read_catalog
 @select
 @selector
-def add_contract(select, exclude, project_path, selector, public_only=False):
+def add_contract(select, exclude, project_path, selector, read_catalog, public_only=False):
     """
     Adds a contract to all selected models.
     """
     path = Path(project_path).expanduser().resolve()
-    project = DbtProject.from_directory(path)
+    logger.info(f"Reading dbt project at {path}")
+    project = DbtProject.from_directory(path, read_catalog)
     resources = list(
         project.select_resources(
             select=select, exclude=exclude, selector=selector, output_key="unique_id"
         )
     )
+
+    logger.info(f"Selected {len(resources)} resources: {resources}")
     models = filter(lambda x: x.startswith("model"), resources)
     if public_only:
         models = filter(lambda x: project.get_manifest_node(x).access == "public", models)
+    logger.info(f"Adding contracts to models in selected resources...")
     for model_unique_id in models:
         model_node = project.get_manifest_node(model_unique_id)
         model_catalog = project.get_catalog_entry(model_unique_id)
-        meshify_constructor = DbtMeshModelConstructor(
-            project_path=project_path, model_node=model_node, model_catalog=model_catalog
+        meshify_constructor = DbtMeshConstructor(
+            project_path=project_path, node=model_node, catalog=model_catalog
         )
-        meshify_constructor.add_model_contract()
+        logger.info(f"Adding contract to model: {model_unique_id}")
+        try:
+            meshify_constructor.add_model_contract()
+            logger.success(f"Successfully added contract to model: {model_unique_id}")
+        except Exception as e:
+            raise FatalMeshifyException(f"Error adding contract to model: {model_unique_id}")
 
 
 @operation.command(name="add-version")
 @exclude
 @project_path
+@read_catalog
 @select
 @selector
 @click.option("--prerelease", "--pre", default=False, is_flag=True)
 @click.option("--defined-in", default=None)
-def add_version(select, exclude, project_path, selector, prerelease, defined_in):
+def add_version(select, exclude, project_path, selector, prerelease, defined_in, read_catalog):
     """
     Adds/increments model versions for all selected models.
     """
     path = Path(project_path).expanduser().resolve()
-    project = DbtProject.from_directory(path)
+
+    logger.info(f"Reading dbt project at {path}")
+    project = DbtProject.from_directory(path, read_catalog)
     resources = list(
         project.select_resources(
             select=select, exclude=exclude, selector=selector, output_key="unique_id"
         )
     )
     models = filter(lambda x: x.startswith("model"), resources)
+    logger.info(f"Selected {len(resources)} resources: {resources}")
+    logger.info(f"Adding version to models in selected resources...")
     for model_unique_id in models:
         model_node = project.get_manifest_node(model_unique_id)
         if model_node.version == model_node.latest_version:
-            meshify_constructor = DbtMeshModelConstructor(
-                project_path=project_path, model_node=model_node
-            )
-            meshify_constructor.add_model_version(prerelease=prerelease, defined_in=defined_in)
+            meshify_constructor = DbtMeshConstructor(project_path=project_path, node=model_node)
+            try:
+                meshify_constructor.add_model_version(prerelease=prerelease, defined_in=defined_in)
+                logger.success(f"Successfully added version to model: {model_unique_id}")
+            except Exception as e:
+                raise FatalMeshifyException(
+                    f"Error adding version to model: {model_unique_id}"
+                ) from e
 
 
 @operation.command(name="create-group")
+@click.argument("name")
 @exclude
+@group_yml_path
+@owner
+@owner_email
+@owner_name
+@owner_properties
 @project_path
+@read_catalog
 @select
 @selector
-@click.argument("name")
-@owner
-@group_yml_path
 def create_group(
     name,
     project_path: os.PathLike,
-    owner: List[Tuple[str, str]],
     group_yml_path: os.PathLike,
     select: str,
+    read_catalog: bool,
+    owner_name: Optional[str] = None,
+    owner_email: Optional[str] = None,
+    owner_properties: Optional[str] = None,
     exclude: Optional[str] = None,
     selector: Optional[str] = None,
 ):
     """
     Create a group and add selected resources to the group.
     """
     from dbt_meshify.utilities.grouper import ResourceGrouper
 
     path = Path(project_path).expanduser().resolve()
-    project = DbtProject.from_directory(path)
+    logger.info(f"Reading dbt project at {path}")
+    project = DbtProject.from_directory(path, read_catalog)
 
     if group_yml_path is None:
         group_yml_path = (path / Path("models/_groups.yml")).resolve()
     else:
         group_yml_path = Path(group_yml_path).resolve()
+    logger.info(f"Creating new model group in file {group_yml_path.name}")
 
     if not str(os.path.commonpath([group_yml_path, path])) == str(path):
         raise Exception(
             "The provided group-yml-path is not contained within the provided dbt project."
         )
 
-    owner: Owner = Owner(**{key: value for key, value in owner})
+    group_owner: Owner = Owner(
+        name=owner_name, email=owner_email, _extra=yaml.safe_load(owner_properties or '{}')
+    )
 
     grouper = ResourceGrouper(project)
-    grouper.add_group(
-        name=name,
-        owner=owner,
-        select=select,
-        exclude=exclude,
-        selector=selector,
-        path=group_yml_path,
-    )
+    try:
+        grouper.add_group(
+            name=name,
+            owner=group_owner,
+            select=select,
+            exclude=exclude,
+            selector=selector,
+            path=group_yml_path,
+        )
+        logger.success(f"Successfully created group: {name}")
+    except Exception as e:
+        raise FatalMeshifyException(f"Error creating group: {name}")
 
 
 @cli.command(name="group")
+@click.argument("name")
 @exclude
+@group_yml_path
+@owner
+@owner_email
+@owner_name
+@owner_properties
 @project_path
+@read_catalog
 @select
 @selector
-@click.argument("name")
-@owner
-@group_yml_path
 @click.pass_context
 def group(
     ctx,
     name,
     project_path: os.PathLike,
-    owner: List[Tuple[str, str]],
     group_yml_path: os.PathLike,
     select: str,
+    read_catalog: bool,
+    owner_name: Optional[str] = None,
+    owner_email: Optional[str] = None,
+    owner_properties: Optional[str] = None,
     exclude: Optional[str] = None,
     selector: Optional[str] = None,
 ):
     """
     Creates a new dbt group based on the selection syntax
     Detects the edges of the group, makes their access public, and adds contracts to them
     """
```

### Comparing `dbt_meshify-0.1.0/dbt_meshify/utilities/grouper.py` & `dbt_meshify-0.2.0/dbt_meshify/utilities/grouper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import os
 from pathlib import Path
-from typing import Any, Dict, Optional, Set, Tuple
+from typing import Any, Dict, Optional, Set, Tuple, Union
 
 import networkx
 from dbt.contracts.graph.nodes import Group, ModelNode
 from dbt.contracts.graph.unparsed import Owner
 from dbt.node_types import AccessType, NodeType
+from loguru import logger
 
-from dbt_meshify.dbt_projects import DbtProject
+from dbt_meshify.dbt_projects import DbtProject, DbtSubProject
+from dbt_meshify.storage.file_content_editors import DbtMeshFileEditor
 from dbt_meshify.storage.file_manager import DbtFileManager
-from dbt_meshify.storage.yaml_editors import DbtMeshModelYmlEditor
 
 
 class ResourceGroupingException(BaseException):
     """Exceptions relating to grouping of resources."""
 
 
 class ResourceGrouper:
     """
     The ResourceGrouper is responsible for generating a dbt-core Group for a
     collection of resources in a DbtProject, and for providing access control
     recommendations based on the reference characteristics for each resource.
     """
 
-    def __init__(self, project: DbtProject):
+    def __init__(self, project: Union[DbtProject, DbtSubProject]):
         self.project = project
-        self.meshify = DbtMeshModelYmlEditor()
+        self.meshify = DbtMeshFileEditor()
         self.file_manager = DbtFileManager(read_project_path=project.path)
 
     @classmethod
     def identify_interface(cls, graph: networkx.Graph, selected_bunch: Set[str]) -> Set[str]:
         """
         Given a graph, find the interface nodes, where interface nodes are the nodes that
         either have downstream consumers outside the selected bunch OR are nodes
@@ -49,16 +50,23 @@
         whereas nodes that are not a referenced are safe for a private access level.
         """
         boundary_nodes = cls.identify_interface(graph, nodes)
         resources = {
             node: AccessType.Public if node in boundary_nodes else AccessType.Private
             for node in nodes
         }
+        logger.info(f"Identified resource access types based on the graph: {resources}")
         return resources
 
+    @classmethod
+    def clean_subgraph(cls, graph: networkx.DiGraph) -> networkx.DiGraph:
+        """Generate a subgraph that does not contain test resource types."""
+        test_nodes = set(node for node in graph.nodes if node.startswith('test'))
+        return graph.subgraph(set(graph.nodes) - test_nodes)
+
     def _generate_resource_group(
         self,
         name: str,
         owner: Owner,
         path: os.PathLike,
         select: str,
         exclude: Optional[str] = None,
@@ -72,32 +80,37 @@
             package_name=self.project.name,
             original_file_path=os.path.relpath(path, self.project.path),
             unique_id=f"group.{self.project.name}.{name}",
             path=os.path.relpath(path, self.project.path / Path("models")),
             resource_type=NodeType.Group,
         )
 
-        nodes = self.project.select_resources(
-            select=select, exclude=exclude, selector=selector, output_key="unique_id"
-        )
+        if not (select or exclude or selector):
+            nodes = set()
+        else:
+            nodes = self.project.select_resources(
+                select=select, exclude=exclude, selector=selector, output_key="unique_id"
+            )
 
+        logger.info(f"Selected {len(nodes)} resources: {nodes}")
         # Check if any of the selected nodes are already in a group of a different name. If so, raise an exception.
         nodes = set(filter(lambda x: not x.startswith("source"), nodes))
         for node in nodes:
             existing_group = self.project.manifest.nodes[node].config.group
 
             if existing_group is None or existing_group == group.name:
                 continue
 
             raise ResourceGroupingException(
                 f"The node {node} has been selected for addition to a new group, however {node} is already part "
                 f"of the {existing_group} group. Please remove {node} from its group and try again."
             )
 
-        resources = self.classify_resource_access(self.project.graph.graph, nodes)
+        cleaned_subgraph = self.clean_subgraph(self.project.graph.graph)
+        resources = self.classify_resource_access(cleaned_subgraph, nodes)
 
         return group, resources
 
     def add_group(
         self,
         name: str,
         owner: Owner,
@@ -117,14 +130,15 @@
             group_yml: Dict[str, str] = self.file_manager.read_file(group_path)  # type: ignore
         except FileNotFoundError:
             group_yml = {}
 
         output_yml = self.meshify.add_group_to_yml(group, group_yml)
         self.file_manager.write_file(group_path, output_yml)
 
+        logger.info(f"Adding resources to group '{group.name}'...")
         for resource, access_type in resources.items():
             # TODO: revisit this logic other resource types
             if not resource.startswith("model"):
                 continue
             model: ModelNode = self.project.models[resource]
             if model.patch_path:
                 path = Path(model.patch_path.split("://")[1])
@@ -135,12 +149,20 @@
                 path = Path(model.original_file_path).parent / '_models.yml'
 
             try:
                 file_yml: Dict[str, Any] = self.file_manager.read_file(path)  # type: ignore
             except FileNotFoundError:
                 file_yml = {}
 
-            output_yml = self.meshify.add_group_and_access_to_model_yml(
-                model.name, group, access_type, file_yml
+            logger.info(
+                f"Adding model '{model.name}' to group '{group.name}' in file '{path.name}'"
             )
-
-            self.file_manager.write_file(path, output_yml)
+            try:
+                output_yml = self.meshify.add_group_and_access_to_model_yml(
+                    model.name, group, access_type, file_yml
+                )
+
+                self.file_manager.write_file(path, output_yml)
+                logger.success(f"Successfully added model '{model.name}' to group '{group.name}'")
+            except Exception as e:
+                logger.error(f"Failed to add model '{model.name}' to group '{group.name}'")
+                logger.exception(e)
```

### Comparing `dbt_meshify-0.1.0/pyproject.toml` & `dbt_meshify-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.black]
 line-length = 99
 target-version = ['py38']
 
 [tool.poetry]
 name = "dbt-meshify"
-version = "0.1.0"
+version = "0.2.0"
 description = "a package to upgrade dbt packages to the dbt mesh framework"
 authors = [
     "Dave Connors <dave.connors@fishtownanalytics.com>",
     "Grace Goheen <grace.goheen@dbtlabs.com>"
 ]
 license = "Apache 2.0"
 readme = "README.md"
@@ -23,14 +23,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 dbt-core = "^1.5.0"
 click = "^8.1.3"
 dbt-postgres = { version = "^1.5.0", optional = true }
 ruamel-yaml = "^0.17.31"
+loguru = "^0.7.0"
 
 [tool.poetry.extras]
 postgres = ['dbt-postgres']
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 dbt-duckdb = "^1.5.0"
```

### Comparing `dbt_meshify-0.1.0/PKG-INFO` & `dbt_meshify-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dbt-meshify
-Version: 0.1.0
+Version: 0.2.0
 Summary: a package to upgrade dbt packages to the dbt mesh framework
 License: Apache 2.0
 Author: Dave Connors
 Author-email: dave.connors@fishtownanalytics.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: postgres
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dbt-core (>=1.5.0,<2.0.0)
 Requires-Dist: dbt-postgres (>=1.5.0,<2.0.0) ; extra == "postgres"
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: ruamel-yaml (>=0.17.31,<0.18.0)
 Description-Content-Type: text/markdown
 
 # dbt-meshify
 
 EXPERIMENTAL
 
@@ -45,13 +46,13 @@
 
 ## Basic Usage
 
 ```bash
 # create a group of all models tagged with "finance"
 # leaf nodes and nodes with cross-group dependencies will be `public`
 # public nodes will also have contracts added to them
-dbt-meshify group finance --owner name Monopoly Man -s +tag:finance
+dbt-meshify group finance --owner-name "Monopoly Man" -s +tag:finance
 
 # optionally use the add-version operation to add a new version to a model
 dbt-meshify operation add-version -s fct_orders
 ```
```

