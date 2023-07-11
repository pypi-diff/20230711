# Comparing `tmp/grai_schemas-0.2.0a4.tar.gz` & `tmp/grai_schemas-0.2.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_schemas-0.2.0a4.tar", max compression
+gzip compressed data, was "grai_schemas-0.2.0a5.tar", max compression
```

## Comparing `grai_schemas-0.2.0a4.tar` & `grai_schemas-0.2.0a5.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     3793 2023-02-14 12:06:39.096892 grai_schemas-0.2.0a4/LICENSE
--rw-r--r--   0        0        0      322 2023-05-02 08:01:59.697152 grai_schemas-0.2.0a4/README.md
--rw-r--r--   0        0        0      862 2023-07-05 16:59:28.458708 grai_schemas-0.2.0a4/pyproject.toml
--rw-r--r--   0        0        0      210 2023-07-05 16:59:33.885947 grai_schemas-0.2.0a4/src/grai_schemas/__init__.py
--rw-r--r--   0        0        0      848 2023-06-30 08:46:34.984841 grai_schemas-0.2.0a4/src/grai_schemas/base.py
--rw-r--r--   0        0        0     3757 2023-07-03 12:38:54.726590 grai_schemas-0.2.0a4/src/grai_schemas/generics.py
--rw-r--r--   0        0        0    41788 2023-06-08 08:40:20.862352 grai_schemas-0.2.0a4/src/grai_schemas/human_ids.py
--rw-r--r--   0        0        0      175 2023-06-06 17:35:16.829056 grai_schemas-0.2.0a4/src/grai_schemas/package_definitions.py
--rw-r--r--   0        0        0        0 2023-02-14 12:06:39.097597 grai_schemas-0.2.0a4/src/grai_schemas/py.typed
--rw-r--r--   0        0        0      669 2023-06-30 08:46:34.985057 grai_schemas-0.2.0a4/src/grai_schemas/schema.py
--rw-r--r--   0        0        0     2564 2023-07-03 12:38:54.727678 grai_schemas-0.2.0a4/src/grai_schemas/utilities.py
--rw-r--r--   0        0        0      451 2023-07-03 12:38:54.727777 grai_schemas-0.2.0a4/src/grai_schemas/v1/__init__.py
--rw-r--r--   0        0        0     2786 2023-06-29 08:12:22.805233 grai_schemas-0.2.0a4/src/grai_schemas/v1/edge.py
--rw-r--r--   0        0        0        0 2023-06-29 08:12:22.805263 grai_schemas-0.2.0a4/src/grai_schemas/v1/events
--rw-r--r--   0        0        0      845 2023-06-29 08:12:22.805491 grai_schemas-0.2.0a4/src/grai_schemas/v1/events.py
--rw-r--r--   0        0        0      793 2023-07-03 12:38:54.727867 grai_schemas-0.2.0a4/src/grai_schemas/v1/generics.py
--rw-r--r--   0        0        0     1738 2023-07-03 12:38:54.727925 grai_schemas-0.2.0a4/src/grai_schemas/v1/merge.py
--rw-r--r--   0        0        0      279 2023-06-16 16:15:18.437295 grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/__init__.py
--rw-r--r--   0        0        0     2179 2023-07-03 12:38:54.728133 grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/edges.py
--rw-r--r--   0        0        0      240 2023-07-03 12:38:54.728222 grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/generics.py
--rw-r--r--   0        0        0      784 2023-07-03 12:38:54.728309 grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/metadata.py
--rw-r--r--   0        0        0     1930 2023-07-03 12:38:54.728593 grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/nodes.py
--rw-r--r--   0        0        0     6925 2023-06-29 08:12:22.806053 grai_schemas-0.2.0a4/src/grai_schemas/v1/mock.py
--rw-r--r--   0        0        0     2776 2023-06-29 08:12:22.806146 grai_schemas-0.2.0a4/src/grai_schemas/v1/node.py
--rw-r--r--   0        0        0      940 2023-06-29 08:12:22.806213 grai_schemas-0.2.0a4/src/grai_schemas/v1/organization.py
--rw-r--r--   0        0        0     1254 2023-07-05 16:59:13.277528 grai_schemas-0.2.0a4/src/grai_schemas/v1/source.py
--rw-r--r--   0        0        0     3696 2023-06-30 16:06:45.947383 grai_schemas-0.2.0a4/src/grai_schemas/v1/workspace.py
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 grai_schemas-0.2.0a4/PKG-INFO
+-rw-r--r--   0        0        0     3793 2023-02-14 12:06:39.096892 grai_schemas-0.2.0a5/LICENSE
+-rw-r--r--   0        0        0      322 2023-05-02 08:01:59.697152 grai_schemas-0.2.0a5/README.md
+-rw-r--r--   0        0        0      862 2023-07-11 10:27:21.769257 grai_schemas-0.2.0a5/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-07-11 10:27:28.122212 grai_schemas-0.2.0a5/src/grai_schemas/__init__.py
+-rw-r--r--   0        0        0      848 2023-07-11 08:47:36.928111 grai_schemas-0.2.0a5/src/grai_schemas/base.py
+-rw-r--r--   0        0        0     3757 2023-07-11 08:47:36.928239 grai_schemas-0.2.0a5/src/grai_schemas/generics.py
+-rw-r--r--   0        0        0    41788 2023-06-08 08:40:20.862352 grai_schemas-0.2.0a5/src/grai_schemas/human_ids.py
+-rw-r--r--   0        0        0      175 2023-06-06 17:35:16.829056 grai_schemas-0.2.0a5/src/grai_schemas/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-02-14 12:06:39.097597 grai_schemas-0.2.0a5/src/grai_schemas/py.typed
+-rw-r--r--   0        0        0      669 2023-07-11 08:47:36.929249 grai_schemas-0.2.0a5/src/grai_schemas/schema.py
+-rw-r--r--   0        0        0     2564 2023-07-11 08:47:36.929380 grai_schemas-0.2.0a5/src/grai_schemas/utilities.py
+-rw-r--r--   0        0        0      451 2023-07-11 08:47:36.929506 grai_schemas-0.2.0a5/src/grai_schemas/v1/__init__.py
+-rw-r--r--   0        0        0     2786 2023-07-11 08:47:36.929628 grai_schemas-0.2.0a5/src/grai_schemas/v1/edge.py
+-rw-r--r--   0        0        0      845 2023-07-11 08:47:36.929712 grai_schemas-0.2.0a5/src/grai_schemas/v1/events.py
+-rw-r--r--   0        0        0      793 2023-07-11 08:47:36.929837 grai_schemas-0.2.0a5/src/grai_schemas/v1/generics.py
+-rw-r--r--   0        0        0     1738 2023-07-11 08:47:36.929909 grai_schemas-0.2.0a5/src/grai_schemas/v1/merge.py
+-rw-r--r--   0        0        0      279 2023-06-16 16:15:18.437295 grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/__init__.py
+-rw-r--r--   0        0        0     2179 2023-07-11 08:47:36.930042 grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/edges.py
+-rw-r--r--   0        0        0      240 2023-07-11 08:47:36.930143 grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/generics.py
+-rw-r--r--   0        0        0      784 2023-07-11 08:47:36.930249 grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/metadata.py
+-rw-r--r--   0        0        0     2228 2023-07-11 08:47:41.704120 grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/nodes.py
+-rw-r--r--   0        0        0     6925 2023-07-11 08:47:36.935588 grai_schemas-0.2.0a5/src/grai_schemas/v1/mock.py
+-rw-r--r--   0        0        0     2776 2023-07-11 08:47:36.935745 grai_schemas-0.2.0a5/src/grai_schemas/v1/node.py
+-rw-r--r--   0        0        0      940 2023-07-11 08:47:36.935826 grai_schemas-0.2.0a5/src/grai_schemas/v1/organization.py
+-rw-r--r--   0        0        0     1203 2023-07-11 08:47:36.936153 grai_schemas-0.2.0a5/src/grai_schemas/v1/source.py
+-rw-r--r--   0        0        0     3696 2023-07-11 08:47:36.936896 grai_schemas-0.2.0a5/src/grai_schemas/v1/workspace.py
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 grai_schemas-0.2.0a5/PKG-INFO
```

### Comparing `grai_schemas-0.2.0a4/LICENSE` & `grai_schemas-0.2.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/pyproject.toml` & `grai_schemas-0.2.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_schemas"
-version = "0.2.0-alpha4"
+version = "0.2.0-alpha5"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [{ include = "grai_schemas", from = "src" },]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-schemas"
```

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/base.py` & `grai_schemas-0.2.0a5/src/grai_schemas/base.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/generics.py` & `grai_schemas-0.2.0a5/src/grai_schemas/generics.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/human_ids.py` & `grai_schemas-0.2.0a5/src/grai_schemas/human_ids.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/schema.py` & `grai_schemas-0.2.0a5/src/grai_schemas/schema.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/utilities.py` & `grai_schemas-0.2.0a5/src/grai_schemas/utilities.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/v1/edge.py` & `grai_schemas-0.2.0a5/src/grai_schemas/v1/edge.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/v1/events.py` & `grai_schemas-0.2.0a5/src/grai_schemas/v1/events.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/v1/generics.py` & `grai_schemas-0.2.0a5/src/grai_schemas/v1/generics.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/v1/merge.py` & `grai_schemas-0.2.0a5/src/grai_schemas/v1/merge.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/edges.py` & `grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/edges.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/metadata.py` & `grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/nodes.py` & `grai_schemas-0.2.0a5/src/grai_schemas/v1/metadata/nodes.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 
 class NodeMetadataTypeLabels(Enum):
     """ """
 
     generic: Literal["Generic"] = "Generic"
     table: Literal["Table"] = "Table"
     column: Literal["Column"] = "Column"
+    query: Literal["Query"] = "Query"
 
 
-NodeMetadataTypeLabelLiterals = Literal["Generic", "Table", "Column"]
+NodeMetadataTypeLabelLiterals = Literal["Generic", "Table", "Column", "Query"]
 
 
 class SourceType(Enum):
     """ """
 
     database = "SQL"
 
@@ -76,8 +77,21 @@
 class TableMetadata(BaseNodeMetadataV1):
     """ """
 
     node_type: Literal["Table"]
     node_attributes: TableAttributes = TableAttributes()
 
 
-Metadata = Union[ColumnMetadata, TableMetadata, GenericNodeMetadataV1]
+class QueryAttributes(GenericAttributes):
+    """ """
+
+    version: Literal["v1"] = "v1"
+
+
+class QueryMetadata(BaseNodeMetadataV1):
+    """ """
+
+    node_type: Literal["Query"]
+    node_attributes: QueryAttributes = QueryAttributes()
+
+
+Metadata = Union[ColumnMetadata, TableMetadata, QueryMetadata, GenericNodeMetadataV1]
```

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/v1/mock.py` & `grai_schemas-0.2.0a5/src/grai_schemas/v1/mock.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/v1/node.py` & `grai_schemas-0.2.0a5/src/grai_schemas/v1/node.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/v1/organization.py` & `grai_schemas-0.2.0a5/src/grai_schemas/v1/organization.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/v1/source.py` & `grai_schemas-0.2.0a5/src/grai_schemas/v1/source.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,19 +9,15 @@
 class SourceSpec(GraiBaseModel):
     id: Optional[UUID]
     name: str
     workspace: Union[UUID, WorkspaceSpec, None]
 
     @property
     def workspace_id(self) -> Optional[UUID]:
-        return (
-            self.workspace.id
-            if isinstance(self.workspace, WorkspaceSpec)
-            else self.workspace
-        )
+        return self.workspace.id if isinstance(self.workspace, WorkspaceSpec) else self.workspace
 
     def __hash__(self) -> int:
         return hash(self.name)
 
 
 class DataSourceMixin(GraiBaseModel):
     data_source: SourceSpec
@@ -36,22 +32,22 @@
     version: Literal["v1"] = "v1"
     spec: SourceSpec
 
     def __hash__(self):
         return hash(self.spec)
 
     @classmethod
-    def from_spec(cls, spec_dict: dict) -> "SourceV1":
+    def from_spec(cls, spec: Union[dict, SourceSpec]) -> "SourceV1":
         """
 
         Args:
-            spec_dict (Dict):
+            spec:
 
         Returns:
 
         Raises:
 
         """
-        return cls(version="v1", type="Source", spec=spec_dict)
+        return cls(version="v1", type="Source", spec=spec)
 
 
 __all__ = ["SourceSpec", "SourceV1", "DataSourceMixin", "DataSourcesMixin"]
```

### Comparing `grai_schemas-0.2.0a4/src/grai_schemas/v1/workspace.py` & `grai_schemas-0.2.0a5/src/grai_schemas/v1/workspace.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a4/PKG-INFO` & `grai_schemas-0.2.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-schemas
-Version: 0.2.0a4
+Version: 0.2.0a5
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

