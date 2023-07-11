# Comparing `tmp/grai_source_metabase-0.1.1a2.tar.gz` & `tmp/grai_source_metabase-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_metabase-0.1.1a2.tar", max compression
+gzip compressed data, was "grai_source_metabase-0.2.0a1.tar", max compression
```

## Comparing `grai_source_metabase-0.1.1a2.tar` & `grai_source_metabase-0.2.0a1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       29 2023-07-06 18:33:54.210141 grai_source_metabase-0.1.1a2/README.md
--rw-r--r--   0        0        0      784 2023-07-06 21:31:42.320460 grai_source_metabase-0.1.1a2/pyproject.toml
--rw-r--r--   0        0        0      156 2023-07-06 21:31:58.229774 grai_source_metabase-0.1.1a2/src/grai_source_metabase/__init__.py
--rw-r--r--   0        0        0    10225 2023-07-06 21:31:58.236058 grai_source_metabase-0.1.1a2/src/grai_source_metabase/adapters.py
--rw-r--r--   0        0        0     1618 2023-07-06 21:31:58.233939 grai_source_metabase-0.1.1a2/src/grai_source_metabase/base.py
--rw-r--r--   0        0        0     9818 2023-07-06 21:31:58.231680 grai_source_metabase-0.1.1a2/src/grai_source_metabase/loader.py
--rw-r--r--   0        0        0     3223 2023-07-06 21:31:58.228203 grai_source_metabase-0.1.1a2/src/grai_source_metabase/mock_tools.py
--rw-r--r--   0        0        0      783 2023-07-06 18:33:54.212995 grai_source_metabase-0.1.1a2/src/grai_source_metabase/models.py
--rw-r--r--   0        0        0      186 2023-07-06 18:33:54.213324 grai_source_metabase-0.1.1a2/src/grai_source_metabase/package_definitions.py
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 grai_source_metabase-0.1.1a2/PKG-INFO
+-rw-r--r--   0        0        0       28 2023-07-11 08:47:36.897894 grai_source_metabase-0.2.0a1/README.md
+-rw-r--r--   0        0        0      797 2023-07-11 08:47:41.694392 grai_source_metabase-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-07-11 08:47:41.694537 grai_source_metabase-0.2.0a1/src/grai_source_metabase/__init__.py
+-rw-r--r--   0        0        0    11025 2023-07-11 08:47:41.694755 grai_source_metabase-0.2.0a1/src/grai_source_metabase/adapters.py
+-rw-r--r--   0        0        0     1730 2023-07-11 08:47:41.694831 grai_source_metabase-0.2.0a1/src/grai_source_metabase/base.py
+-rw-r--r--   0        0        0    10353 2023-07-11 08:47:41.694941 grai_source_metabase-0.2.0a1/src/grai_source_metabase/loader.py
+-rw-r--r--   0        0        0     3223 2023-07-11 08:47:41.695259 grai_source_metabase-0.2.0a1/src/grai_source_metabase/mock_tools.py
+-rw-r--r--   0        0        0      783 2023-07-11 08:47:41.695829 grai_source_metabase-0.2.0a1/src/grai_source_metabase/models.py
+-rw-r--r--   0        0        0      186 2023-07-11 08:47:41.697283 grai_source_metabase-0.2.0a1/src/grai_source_metabase/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:47:41.697516 grai_source_metabase-0.2.0a1/src/grai_source_metabase/py.typed
+-rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 grai_source_metabase-0.2.0a1/PKG-INFO
```

### Comparing `grai_source_metabase-0.1.1a2/pyproject.toml` & `grai_source_metabase-0.2.0a1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "grai-source-metabase"
-version = "0.1.1-alpha2"
+version = "0.2.0-alpha1"
 description = ""
 authors = ["Elseagle <dowolebolu@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "grai_source_metabase", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^1.10.9"
 requests = "^2.31.0"
-grai-schemas = "^0.1.16"
-grai-client = "^0.2.19"
+grai-schemas = "^0.2.0-alpha4"
+grai-client = "^0.3.0-alpha18"
 multimethod = "^1.9.1"
 retrying = "^1.3.4"
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.0"
 faker = "^18.11.2"
 black = "^23.3.0"
```

### Comparing `grai_source_metabase-0.1.1a2/src/grai_source_metabase/adapters.py` & `grai_source_metabase-0.2.0a1/src/grai_source_metabase/adapters.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-from typing import Any, Dict, List, Literal, Sequence, Union
+from typing import Any, Dict, List, Literal, Sequence, TypeVar, Union
 
 from grai_schemas import config as base_config
 from grai_schemas.schema import Schema
-from grai_schemas.v1 import EdgeV1, NodeV1
+from grai_schemas.v1 import EdgeV1, NodeV1, SourcedEdgeV1, SourcedNodeV1, SourceV1
 from grai_schemas.v1.metadata.edges import EdgeMetadataTypeLabels, GenericEdgeMetadataV1
 from grai_schemas.v1.metadata.nodes import (
     GenericNodeMetadataV1,
     NodeMetadataTypeLabels,
     QueryMetadata,
     TableMetadata,
 )
+from grai_schemas.v1.source import SourceSpec
 from multimethod import multimethod
 from pydantic import BaseModel
 
 from grai_source_metabase.models import Edge, NodeTypes, Question, Table
 from grai_source_metabase.package_definitions import config
 
+T = TypeVar("T")
+
 
 @multimethod
 def build_grai_metadata(current: Any, desired: Any) -> None:
     """
     Build grai metadata for a given object.
 
     Args:
@@ -179,15 +182,15 @@
         "metadata": current.metadata if current.metadata is not None else {},
         "raw_object": current.dict(),
     }
 
     return data
 
 
-def build_metadata(obj, version):
+def build_metadata(obj, version) -> Dict[str, Dict]:
     """
     Build metadata for a given object.
 
     Args:
         obj: The object to build metadata from.
         version: The version of the metadata to build.
 
@@ -221,67 +224,69 @@
 
     """
 
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)}")
 
 
 @adapt_to_client.register
-def adapt_table_to_client(current: Table, version: Literal["v1"] = "v1") -> NodeV1:
+def adapt_table_to_client(current: Table, source: SourceSpec, version: Literal["v1"] = "v1") -> SourcedNodeV1:
     """
     Adapt a Table object to the desired client format.
 
     Args:
-        current (Table): The Table object to adapt.
-        version (Literal["v1"], optional): The version of the client format to adapt to. Defaults to "v1".
+        current: The Table object to adapt.
+        source: The Source associated with the Table
+        version: The version of the client format to adapt to. Defaults to "v1".
 
     Returns:
         NodeV1: Adapted Table object in the desired client format.
 
     Raises:
         None.
 
     """
 
     spec_dict = {
         "name": current.full_name,
         "namespace": current.namespace,
         "display_name": current.name,
-        "data_source": config.integration_name,
+        "data_source": source,
         "metadata": build_metadata(current, version),
     }
 
-    return NodeV1.from_spec(spec_dict)
+    return SourcedNodeV1.from_spec(spec_dict)
 
 
 @adapt_to_client.register
-def adapt_question_to_client(current: Question, version: Literal["v1"] = "v1") -> NodeV1:
+def adapt_question_to_client(current: Question, source: SourceSpec, version: Literal["v1"] = "v1") -> SourcedNodeV1:
     """
     Adapt a Question object to the desired client format.
 
     Args:
-        current (Question): The Question object to adapt.
-        version (Literal["v1"], optional): The version of the client format to adapt to. Defaults to "v1".
+        current: The Question object to adapt.
+        source: The source associated with the Question
+        version: The version of the client format to adapt to. Defaults to "v1".
 
     Returns:
         NodeV1: Adapted Question object in the desired client format.
 
     Raises:
         None.
 
     """
 
     spec_dict = {
         "name": current.full_name,
         "namespace": current.namespace,
         "display_name": current.name,
-        "data_source": config.integration_name,
+        "data_source": source,
         "metadata": build_metadata(current, version),
     }
 
-    return NodeV1.from_spec(spec_dict)
+    return SourcedNodeV1.from_spec(spec_dict)
 
 
 def make_name(node1: NodeTypes, node2: NodeTypes) -> str:
     """
     Creates a name for an edge based on the given nodes.
 
     Args:
@@ -298,82 +303,104 @@
     node1_name = f"{node1.namespace}:{node1.full_name}"
     node2_name = f"{node2.namespace}:{node2.full_name}"
 
     return f"{node1_name} -> {node2_name}"
 
 
 @adapt_to_client.register
-def adapt_edge_to_client(current: Edge, version: Literal["v1"] = "v1") -> EdgeV1:
+def adapt_edge_to_client(current: Edge, source: SourceSpec, version: Literal["v1"] = "v1") -> SourcedEdgeV1:
     """
     Adapt an Edge object to the desired client format.
 
     Args:
-        current (Edge): The Edge object to adapt.
-        version (Literal["v1"], optional): The version of the client format to adapt to. Defaults to "v1".
+        current: The Edge object to adapt.
+        source: The data source associated with the Edge
+        version: The version of the client format to adapt to. Defaults to "v1".
 
     Returns:
         EdgeV1: Adapted Edge object in the desired client format.
 
     Raises:
         None.
 
     """
 
     spec_dict = {
-        "data_source": config.integration_name,
+        "data_source": source,
         "name": make_name(current.source, current.destination),
         "namespace": current.source.namespace,
         "source": {
             "name": current.source.full_name,
             "namespace": current.source.namespace,
         },
         "destination": {
             "name": current.destination.full_name,
             "namespace": current.destination.namespace,
         },
         "metadata": build_metadata(current, version),
     }
 
-    return EdgeV1.from_spec(spec_dict)
+    return SourcedEdgeV1.from_spec(spec_dict)
 
 
 @adapt_to_client.register
-def adapt_seq_to_client(objs: Sequence, version: Literal["v1"]) -> List[Union[NodeV1, EdgeV1]]:
+def adapt_seq_to_client(objs: Sequence, source: SourceSpec, version: Literal["v1"]) -> List[T]:
     """
     Adapt a sequence of objects to the desired client format.
 
     Args:
-        objs (Sequence): The sequence of objects to adapt.
-        version (Literal["v1"]): The version of the client format to adapt to.
+        objs: The sequence of objects to adapt.
+        source: The source associated with each object in objs
+        version: The version of the client format to adapt to.
 
     Returns:
         List[Union[NodeV1, EdgeV1]]: Adapted sequence of objects in the desired client format.
 
     Raises:
         None.
 
     """
-    entities = [adapt_to_client(item, version) for item in objs]
-    entities = {entity for entity in entities}
+    entities = [adapt_to_client(item, source, version) for item in objs]
     return list(entities)
 
 
 @adapt_to_client.register
-def adapt_list_to_client(objs: List, version: Literal["v1"]) -> List[Union[NodeV1, EdgeV1]]:
+def adapt_list_to_client(objs: List, source: SourceSpec, version: Literal["v1"]) -> List[T]:
     """
     Adapt a list of objects to the desired client format.
 
     Args:
-        objs (List): The list of objects to adapt.
-        version (Literal["v1"]): The version of the client format to adapt to.
+        objs: The list of objects to adapt.
+        source: The source associated with each object in objs
+        version: The version of the client format to adapt to.
 
     Returns:
         List[Union[NodeV1, EdgeV1]]: Adapted list of objects in the desired client format.
 
     Raises:
         None.
 
     """
 
-    entities = [adapt_to_client(item, version) for item in objs]
-    entities = {entity for entity in entities}
+    entities = [adapt_to_client(item, source, version) for item in objs]
     return list(entities)
+
+
+@adapt_to_client.register
+def adapt_source_v1_to_client(objs: Any, source: SourceV1, version: Any) -> List[T]:
+    """
+    Adapt a list of objects to the desired client format.
+
+    Args:
+        objs: The list of objects to adapt.
+        source: The source associated with each object in objs
+        version: The version of the client format to adapt to.
+
+    Returns:
+        List[Union[NodeV1, EdgeV1]]: Adapted list of objects in the desired client format.
+
+    Raises:
+        None.
+
+    """
+
+    return adapt_to_client(objs, source.spec, version)
```

### Comparing `grai_source_metabase-0.1.1a2/src/grai_source_metabase/base.py` & `grai_source_metabase-0.2.0a1/src/grai_source_metabase/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,50 @@
-from typing import List, Literal, Optional, Tuple
+from typing import Dict, List, Literal, Optional, Tuple, Union
 
 from grai_client.endpoints.client import BaseClient
+from grai_client.integrations.base import GraiIntegrationImplementation
 from grai_client.update import update
-from grai_schemas.base import Edge, Node
+from grai_schemas.base import Edge, Node, SourcedEdge, SourcedNode
+from grai_schemas.v1.source import SourceV1
 
 from grai_source_metabase.adapters import adapt_to_client
 from grai_source_metabase.loader import MetabaseConnector
 
 
-def get_nodes_and_edges(connector: MetabaseConnector, version: Literal["v1"]) -> Tuple[List[Node], List[Edge]]:
-    """
+class MetabaseIntegration(GraiIntegrationImplementation):
+    def __init__(
+        self,
+        source: SourceV1,
+        version: Optional[str] = None,
+        metabase_namespace: Optional[str] = None,
+        namespace_map: Optional[Union[str, Dict[int, str]]] = None,
+        endpoint: Optional[str] = None,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+    ):
+        super().__init__(source, version)
+
+        self.connector = MetabaseConnector(
+            metabase_namespace=metabase_namespace,
+            namespace_map=namespace_map,
+            username=username,
+            password=password,
+            endpoint=endpoint,
+        )
+
+    def ready(self) -> bool:
+        try:
+            self.connector.authenticate()
+            return True
+        except Exception as e:
+            return False
+
+    def nodes(self) -> List[SourcedNode]:
+        nodes = adapt_to_client(self.connector.get_nodes(), self.source, self.version)
+        return nodes
+
+    def edges(self) -> List[SourcedEdge]:
+        edges = adapt_to_client(self.connector.get_edges(), self.source, self.version)
+        return edges
 
-    Args:
-        connector (MetabaseConnector):
-        version (Literal["v1"]):
-
-    Returns:
-
-    Raises:
-
-    """
-    nodes = connector.get_nodes()
-    edges = connector.get_edges()
-
-    nodes = adapt_to_client(nodes, version)
-    edges = adapt_to_client(edges, version)
-    return nodes, edges
-
-
-def update_server(
-    client: BaseClient,
-    namespaces: Optional = None,
-    metabase_namespace: Optional[str] = None,
-    username: Optional[str] = None,
-    password: Optional[str] = None,
-    endpoint: Optional[str] = None,
-):
-    """
-
-    Args:
-        password:
-        username: Optional[str]
-        client:
-        namespaces:  (Default value = None)
-        metabase_namespace:  (Default value = None)
-        endpoint:  (Default value = None)
-
-    Returns:
-
-    Raises:
-
-    """
-    kwargs = {
-        "namespaces": namespaces,
-        "metabase_namespace": metabase_namespace,
-        "username": username,
-        "password": password,
-        "endpoint": endpoint,
-    }
-    kwargs = {k: v for k, v in kwargs.items() if v is not None}
-
-    conn = MetabaseConnector(**kwargs)
-    nodes, edges = get_nodes_and_edges(conn, "v1")
-
-    update(client, nodes)
-    update(client, edges)
+    def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
+        return self.nodes(), self.edges()
```

### Comparing `grai_source_metabase-0.1.1a2/src/grai_source_metabase/loader.py` & `grai_source_metabase-0.2.0a1/src/grai_source_metabase/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,36 @@
-import json
+from functools import cached_property
 from itertools import chain
-from typing import Callable, Dict, List, Optional, Union
+from typing import Callable, Dict, List, Optional, TypedDict, Union
 
 import requests
-from pydantic import BaseSettings, SecretStr, validator
+from pydantic import (
+    BaseModel,
+    BaseSettings,
+    HttpUrl,
+    Json,
+    SecretStr,
+    parse_obj_as,
+    validator,
+)
 from requests.exceptions import ConnectionError
 from retrying import retry
 
 from grai_source_metabase.models import Edge, NodeTypes, Question, Table
 
 
 class MetabaseConfig(BaseSettings):
-    endpoint: str
+    endpoint: HttpUrl
     username: SecretStr
     password: SecretStr
 
     @validator("endpoint")
     def validate_endpoint(cls, endpoint: str):
         endpoint = endpoint.rstrip("/")
-        return endpoint
+        return parse_obj_as(HttpUrl, endpoint)
 
     class Config:
         env_prefix = "grai_metabase_"
         env_file = ".env"
 
 
 class MetabaseAPI:
@@ -144,27 +152,28 @@
             dict: The JSON response containing the list of collections.
 
         """
 
         pass
 
 
-def build_namespace_map(dbs: Dict, namespace_map: Union[str, Dict, None], metabase_namespace: str) -> Dict:
-    if isinstance(namespace_map, str):
-        namespace_map = json.loads(namespace_map)
-    elif namespace_map is None:
-        namespace_map = {}
+def build_namespace_map(default_map: Dict[int, str], dbs: Dict, metabase_namespace: str) -> Dict[int, str]:
+    namespace_map = default_map.copy()
 
     for k, v in dbs.items():
         db_id_ns = f"{metabase_namespace}.{k}.{v['name']}"
         namespace_map.setdefault(k, db_id_ns)
 
     return namespace_map
 
 
+class NamespaceMapJsonModel(BaseModel):
+    json_obj: Json[Dict[int, str]]
+
+
 class MetabaseConnector(MetabaseAPI):
     """
     Connector class for interacting with Metabase API and building lineage information.
 
     Args:
         namespaces (Dict, optional): A mapping of database IDs to their corresponding namespace names. Defaults to None.
         default_namespace (str, optional): The default namespace to be used when a table or question does not have a specific namespace. Defaults to None.
@@ -183,76 +192,84 @@
         question_db_map (Dict[int, int]): A mapping of question IDs to their corresponding database IDs.
 
     """
 
     def __init__(
         self,
         metabase_namespace: str,
-        namespaces: Optional[Dict] = None,
+        namespace_map: Optional[Union[str, Dict[int, str]]] = None,
         *args,
         **kwargs,
     ):
+        if namespace_map is None:
+            namespace_map = {}
+        elif isinstance(namespace_map, str):
+            try:
+                namespace_map = NamespaceMapJsonModel(json_obj=namespace_map).json_obj
+            except Exception as e:
+                message = (
+                    f"There was an error parsing the value provided in namespace_map. When providing namespace_map "
+                    f"it must be either a dictionary whose keys are database id's in metabase and values are namespace "
+                    f"strings in Grai for the corresponding database or a JSON string of the same. "
+                    f"In this case we received a JSON string but it did not parse to Dict[int, str] as expected."
+                )
+                raise ValueError(message) from e
+
         super().__init__(*args, **kwargs)
-        self._lineage_ready = False
+        self.base_namespace_map = namespace_map
         self.metabase_namespace = metabase_namespace
 
+    @cached_property
+    def namespace_map(self):
+        return build_namespace_map(self.base_namespace_map, self.dbs_map, self.metabase_namespace)
+
+    @cached_property
+    def tables(self) -> List[Dict]:
         # This line creates a list of tables by modifying each table dictionary obtained from the get_tables() method.
         # It replaces the "schema" key with a new key "schema_name" while preserving the other key-value pairs.
         # this is because the "schema" key is a reserved keyword in the pydantic.
-        self.tables = [{**table, "schema_name": table.pop("schema")} for table in self.get_tables()]
-        self.tables_map = {table["id"]: table for table in self.tables if table["active"]}
-        self.dbs_map = {db["id"]: db for db in self.get_dbs()["data"]}
-
-        self.questions_map = {
-            question["id"]: question for question in self.get_questions() if question["archived"] is False
-        }
-        self.namespace_map = build_namespace_map(self.dbs_map, namespaces, self.metabase_namespace)
-
-        self.question_table_map = {}
-        self.table_db_map = {}
-        # self.question_db_map = {}
-
-    def build_lineage(self):
-        """
-        Builds the lineage information by updating the mappings and maps.
+        return [{**table, "schema_name": table.pop("schema")} for table in self.get_tables()]
 
-        This method updates the `tables_map`, `dbs_map`, `questions_map`, `question_table_map`, `table_db_map`,
-        and `question_db_map` attributes.
-
-        """
-
-        self.question_table_map = {
+    @cached_property
+    def tables_map(self) -> Dict:
+        return {table["id"]: table for table in self.tables if table["active"]}
+
+    @cached_property
+    def dbs_map(self) -> Dict:
+        return {db["id"]: db for db in self.get_dbs()["data"]}
+
+    @cached_property
+    def questions_map(self) -> Dict:
+        return {question["id"]: question for question in self.get_questions() if question["archived"] is False}
+
+    @cached_property
+    def question_table_map(self) -> Dict:
+        return {
             question["id"]: question["table_id"]
             for question in self.questions_map.values()
             if question["table_id"] and self.tables_map.get(question["table_id"]) is not None
         }
 
-        self.table_db_map = {
+    @cached_property
+    def table_db_map(self) -> Dict:
+        return {
             table["id"]: table["db_id"]
             for table in self.tables
             if table["id"] is not None and table["db_id"] is not None
         }
 
-        # for question, table in self.question_table_map.items():
-        #     self.question_db_map[question] = self.table_db_map[table]
-
-        self._lineage_ready = True
-
     def get_nodes(self) -> List[NodeTypes]:
         """
         Retrieves the list of nodes representing tables and questions.
 
         Returns:
             List[NodeTypes]: The list of nodes.
 
         """
 
-        if not self._lineage_ready:
-            self.build_lineage()
-
         for question in self.questions_map.values():
             question["namespace"] = self.metabase_namespace
 
         for table in self.tables_map.values():
             table["namespace"] = self.namespace_map[self.table_db_map[table["id"]]]
 
         verified_questions = [Question(**question) for question in self.questions_map.values()]
@@ -265,18 +282,14 @@
         """
         Retrieves the list of edges representing the relationships between questions and tables.
 
         Returns:
             List[Edge]: The list of edges.
 
         """
-
-        if not self._lineage_ready:
-            self.build_lineage()
-
         edges = (
             Edge(
                 source=Question(**self.questions_map[question]),
                 destination=Table(**self.tables_map[table]),
                 namespace=self.questions_map[question]["namespace"],
             )
             for question, table in self.question_table_map.items()
```

### Comparing `grai_source_metabase-0.1.1a2/src/grai_source_metabase/mock_tools.py` & `grai_source_metabase-0.2.0a1/src/grai_source_metabase/mock_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_metabase-0.1.1a2/src/grai_source_metabase/models.py` & `grai_source_metabase-0.2.0a1/src/grai_source_metabase/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_metabase-0.1.1a2/PKG-INFO` & `grai_source_metabase-0.2.0a1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: grai-source-metabase
-Version: 0.1.1a2
+Version: 0.2.0a1
 Summary: 
 Author: Elseagle
 Author-email: dowolebolu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: grai-client (>=0.2.19,<0.3.0)
-Requires-Dist: grai-schemas (>=0.1.16,<0.2.0)
+Requires-Dist: grai-client (>=0.3.0-alpha18,<0.4.0)
+Requires-Dist: grai-schemas (>=0.2.0-alpha4,<0.3.0)
 Requires-Dist: multimethod (>=1.9.1,<2.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: retrying (>=1.3.4,<2.0.0)
 Description-Content-Type: text/markdown
 
-"# Grai Metabase Integration"
+# Grai Metabase Integration
+
```

