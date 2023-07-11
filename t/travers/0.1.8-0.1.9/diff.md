# Comparing `tmp/travers-0.1.8.tar.gz` & `tmp/travers-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "travers-0.1.8.tar", last modified: Mon Jan 30 21:52:53 2023, max compression
+gzip compressed data, was "travers-0.1.9.tar", last modified: Tue Jul 11 16:51:19 2023, max compression
```

## Comparing `travers-0.1.8.tar` & `travers-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:52:53.613494 travers-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-01-30 21:52:41.000000 travers-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-01-30 21:52:41.000000 travers-0.1.8/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-30 21:52:53.613494 travers-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-01-30 21:52:41.000000 travers-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 21:52:53.613494 travers-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-01-30 21:52:41.000000 travers-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:52:53.609494 travers-0.1.8/travers/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-01-30 21:52:41.000000 travers-0.1.8/travers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-01-30 21:52:41.000000 travers-0.1.8/travers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:52:53.613494 travers-0.1.8/travers/graphs/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-30 21:52:41.000000 travers-0.1.8/travers/graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-01-30 21:52:41.000000 travers-0.1.8/travers/graphs/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-01-30 21:52:41.000000 travers-0.1.8/travers/graphs/graph_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-01-30 21:52:41.000000 travers-0.1.8/travers/graphs/internals.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-30 21:52:41.000000 travers-0.1.8/travers/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-01-30 21:52:41.000000 travers-0.1.8/travers/xmler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:52:53.609494 travers-0.1.8/travers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-30 21:52:53.000000 travers-0.1.8/travers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-30 21:52:53.000000 travers-0.1.8/travers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 21:52:53.000000 travers-0.1.8/travers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-30 21:52:53.000000 travers-0.1.8/travers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-30 21:52:53.000000 travers-0.1.8/travers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:51:19.242886 travers-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-11 16:51:08.000000 travers-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-11 16:51:08.000000 travers-0.1.9/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-11 16:51:19.242886 travers-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-11 16:51:08.000000 travers-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-11 16:51:08.000000 travers-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:51:19.242886 travers-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 16:51:08.000000 travers-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:51:19.242886 travers-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-11 16:51:08.000000 travers-0.1.9/tests/test_data_formats_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-11 16:51:08.000000 travers-0.1.9/tests/test_data_formats_graph_traverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-11 16:51:08.000000 travers-0.1.9/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-11 16:51:08.000000 travers-0.1.9/tests/test_graph_dag_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-11 16:51:08.000000 travers-0.1.9/tests/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-11 16:51:08.000000 travers-0.1.9/tests/test_utils_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-11 16:51:08.000000 travers-0.1.9/tests/test_walk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:51:19.242886 travers-0.1.9/travers/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-11 16:51:08.000000 travers-0.1.9/travers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-11 16:51:08.000000 travers-0.1.9/travers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-11 16:51:08.000000 travers-0.1.9/travers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:51:19.242886 travers-0.1.9/travers/graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-11 16:51:08.000000 travers-0.1.9/travers/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-07-11 16:51:08.000000 travers-0.1.9/travers/graphs/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-11 16:51:08.000000 travers-0.1.9/travers/graphs/graph_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-11 16:51:08.000000 travers-0.1.9/travers/graphs/internals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-11 16:51:08.000000 travers-0.1.9/travers/xmler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:51:19.242886 travers-0.1.9/travers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-11 16:51:19.000000 travers-0.1.9/travers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-11 16:51:19.000000 travers-0.1.9/travers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:51:19.000000 travers-0.1.9/travers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 16:51:19.000000 travers-0.1.9/travers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 16:51:19.000000 travers-0.1.9/travers.egg-info/top_level.txt
```

### Comparing `travers-0.1.8/LICENSE` & `travers-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `travers-0.1.8/NOTICE.md` & `travers-0.1.9/NOTICE.md`

 * *Files identical despite different names*

### Comparing `travers-0.1.8/setup.py` & `travers-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # python setup.py build_ext --inplace
 
-from setuptools import setup, find_packages  # type:ignore
+from setuptools import find_packages  # type:ignore
+from setuptools import setup
 
-with open("travers/version.py", "r") as v:
+with open("travers/__version__.py", "r") as v:
     vers = v.read()
 exec(vers)  # nosec
 
 with open("README.md", "r") as rm:
     long_description = rm.read()
 
 with open("requirements.txt") as f:
```

### Comparing `travers-0.1.8/travers/__init__.py` & `travers-0.1.9/travers/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,10 +12,12 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from travers.__version__ import __author__
+from travers.__version__ import __version__
 from travers.graphs.graph import Graph
-from travers.graphs.internals import load, read_graphml
-from travers.version import __author__, __version__
+from travers.graphs.internals import load
+from travers.graphs.internals import read_graphml
```

### Comparing `travers-0.1.8/travers/graphs/graph.py` & `travers-0.1.9/travers/graphs/graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,21 +13,45 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from pathlib import Path
-from typing import List, Optional, Tuple
+from typing import List
+from typing import Optional
+from typing import Tuple
 
 import orjson
 
 from travers.errors import MissingDependencyError
 
 
+def print_tree_inner(tree, prefix="", last=True):
+    """
+    Prints a nested dictionary as an ascii tree
+    """
+
+    yield prefix
+    if last:
+        yield "└─ "
+        prefix += "   "
+    else:
+        yield "├─ "
+        prefix += "│  "
+
+    yield str(tree["node"]) + "\n"
+
+    # Recursively print the children
+    count = len(tree["children"])
+    for i, child in enumerate(tree["children"]):
+        last = i == count - 1
+        yield from print_tree_inner(child, prefix, last)
+
+
 class Graph(object):
     """
     Graph object, optimized for traversal.
 
     Edges are stored in a dictionary, the key is the source node to speed up
     finding outgoing edges. The Edges only have three pieces of data:
         - the source node (the key)
@@ -142,17 +166,15 @@
         """
         The edges which comprise the graph
 
         Returns:
             Generator of Tuples of (Source, Target and Relationship)
         """
         for source, records in self._edges.items():
-            yield from (
-                (source, target, relationship) for target, relationship in records
-            )
+            yield from ((source, target, relationship) for target, relationship in records)
 
     def breadth_first_search(self, source: str, depth: int = 100):  # pragma: nocover
         """
         Search a tree for nodes we can walk to from a given node.
 
         Parameters:
             source: string
@@ -197,27 +219,56 @@
                                 node_distance + 1,
                                 self.outgoing_edges(t),
                             )
                         )
             queue.popleft()
         return new_edges
 
+    def depth_first_search(
+        self, node: Optional[str] = None, visited: Optional[set] = None, depth: int = 0
+    ):
+        """
+        Returns a nested dictionary representing the graph as a tree
+        """
+        if node is None:
+            node = self.get_exit_points()[0]
+
+        if visited is None:
+            visited = set()
+
+        visited.add(node)
+
+        tree: dict = {
+            "type": str(self[node].node_type),
+            "node": str(self[node]),
+            "name": node,
+            "depth": depth,
+            "children": [],
+        }
+
+        for neighbor, _, relationship in self.ingoing_edges(node):
+            if neighbor not in visited:
+                child = self.depth_first_search(neighbor, visited, depth + 1)
+                child["relationship"] = relationship
+                tree["children"].append(child)  # type:ignore
+
+        return tree
+
     def outgoing_edges(self, source) -> List[Tuple]:
         """
         Get the list of edges traversable from a given node.
 
         Parameters:
             source: string
                 The node to get the outgoing edges for
 
         Returns:
             Set of Tuples (Source, Target, Relationship)
         """
-        targets = self._edges.get(source) or []
-        return [(source, t, r) for t, r in targets]
+        return [(source, t, r) for t, r in self._edges.get(source, [])]
 
     def ingoing_edges(self, target) -> List[Tuple]:
         """
         Get the list of edges which can traverse to a given node.
 
         Parameters:
             target: string
@@ -237,19 +288,15 @@
 
         # rebuild the edge information
         my_edges = list(self.edges())
 
         while len(my_edges) > 0:
             # find all of the exits
             sources = {source for source, target, direction in my_edges}
-            exits = {
-                target
-                for source, target, direction in my_edges
-                if target not in sources
-            }
+            exits = {target for source, target, direction in my_edges if target not in sources}
 
             if len(exits) == 0:
                 return False
 
             # remove the exits
             new_edges = [
                 (source, target, direction)
@@ -262,33 +309,25 @@
     def get_entry_points(self):
         """
         Get nodes in the Graph with no incoming edges.
         """
         if len(self._nodes) == 1:
             return list(self._nodes.keys())
         targets = {target for source, target, direction in self.edges()}
-        retval = (
-            source
-            for source, target, direction in self.edges()
-            if source not in targets
-        )
+        retval = (source for source, target, direction in self.edges() if source not in targets)
         return sorted(retval)
 
     def get_exit_points(self):
         """
         Get nodes in the Graph with no outgoing edges.
         """
         if len(self._nodes) == 1:  # pragma: no cover
             return list(self._nodes.keys())
         sources = self._edges.keys()
-        retval = (
-            target
-            for source, target, direction in self.edges()
-            if target not in sources
-        )
+        retval = {target for source, target, direction in self.edges() if target not in sources}
         return sorted(retval)
 
     def remove_node(self, nid, heal: bool = False):
         """
         Remove a node.
 
         Parameters:
@@ -308,17 +347,15 @@
             # remove edges where the node is the source
             if nid in self._edges:
                 del self._edges[nid]
 
             # remove the edges where the node is the target
             for source, records in self._edges.items():
                 self._edges[source] = [
-                    (target, relationship)
-                    for target, relationship in records
-                    if target != nid
+                    (target, relationship) for target, relationship in records if target != nid
                 ]
             self._edges = {k: v for k, v in self._edges.items() if len(v) > 0}
 
             # wire up the old incoming and outgoing nodes, cartesian style
             for out_nid in out_going:
                 for in_nid in in_coming:
                     self.add_edge(in_nid[0], out_nid[1], in_nid[1])  # type:ignore
@@ -368,18 +405,16 @@
 
     def to_networkx(self):  # pragma: nocover
         """
         Convert a travers graph to a NetworkX graph
         """
         try:
             import networkx as nx  # type:ignore
-        except ImportError:  # pragma: no cover
-            raise MissingDependencyError(
-                "`networx` is missing, please install or include in requirements.txt"
-            )
+        except ImportError as err:  # pragma: no cover
+            raise MissingDependencyError(err.name) from err
 
         g = nx.DiGraph()
         for s, t, r in self.edges():
             g.add_edge(s, t, relationship=r)
         for node, attribs in self.nodes(True):
             g.add_node(node, **attribs)
         return g
@@ -391,26 +426,34 @@
         g = Graph()
         for s, t, r in self.edges():
             node1 = self[s]
             node2 = self[t]
             if node1 and node2:
                 g.add_edge(node1.get("node_type"), node2.get("node_type"), r)
             if node1:
-                g.add_node(
-                    node1.get("node_type"), {"node_type": node1.get("node_type")}
-                )
+                g.add_node(node1.get("node_type"), {"node_type": node1.get("node_type")})
             if node2:
-                g.add_node(
-                    node2.get("node_type"), {"node_type": node2.get("node_type")}
-                )
+                g.add_node(node2.get("node_type"), {"node_type": node2.get("node_type")})
         return g
 
     def __repr__(self):
-        return (
-            f"Graph - {len(list(self.nodes()))} nodes, {len(list(self.edges()))} edges"
-        )
+        return f"Graph - {len(list(self.nodes()))} nodes, {len(list(self.edges()))} edges"
 
     def __len__(self):
         return len(list(self.nodes()))
 
     def __getitem__(self, nid):
         return self._nodes.get(nid, None)
+
+    def __setitem__(self, nid, node):
+        if not nid in self._nodes:
+            raise ValueError("Cannot create nodes with [] syntax")
+        self._nodes[nid] = node
+
+    def __add__(self, other):
+        self._edges.update(other._edges)
+        self._nodes.update(other._nodes)
+        return self
+
+    def draw(self):
+        tree = self.depth_first_search()
+        return "".join(print_tree_inner(tree))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `travers-0.1.8/travers/graphs/graph_traversal.py` & `travers-0.1.9/travers/graphs/graph_traversal.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from typing import Callable
 
 
 class GraphTraversal:
-
     __slots__ = ("graph", "_active_nodes", "_active_nodes_cache")
 
     def __init__(self, graph, active_nodes: set = set()):
         """
         Graph Traversal
 
         Parameters:
@@ -70,46 +69,34 @@
         Parameters:
             filter: Callable
                 node attribute name to filter on
 
         Returns:
             GraphTraversal
         """
-        active_nodes = {
-            nid for nid, attrib in self.active_nodes(data=True) if filter(attrib)
-        }
+        active_nodes = {nid for nid, attrib in self.active_nodes(data=True) if filter(attrib)}
         return GraphTraversal(graph=self.graph, active_nodes=active_nodes)
 
     def has(self, key, value):
         """
         Filters the active nodes by a key/value match
         """
         active_nodes = [
-            nid
-            for nid, attrib in self.active_nodes(data=True)
-            if attrib.get(key) == value
+            nid for nid, attrib in self.active_nodes(data=True) if attrib.get(key) == value
         ]
         return GraphTraversal(graph=self.graph, active_nodes=active_nodes)
 
     def values(self, key):
-        return list(
-            {
-                attrib[key]
-                for nid, attrib in self.active_nodes(data=True)
-                if key in attrib
-            }
-        )
+        return list({attrib[key] for nid, attrib in self.active_nodes(data=True) if key in attrib})
 
     def active_nodes(self, data=False):
         if not data:
             return self._active_nodes
         if not self._active_nodes_cache:
-            self._active_nodes_cache = [
-                (nid, self.graph[nid]) for nid in self._active_nodes
-            ]
+            self._active_nodes_cache = [(nid, self.graph[nid]) for nid in self._active_nodes]
         return self._active_nodes_cache
 
     def list_relationships(self):
         relationships = []
         for node in self._active_nodes:
             relationships += {r for (s, t, r) in self.graph.outgoing_edges(node)}
         return set(relationships)
```

### Comparing `travers-0.1.8/travers/graphs/internals.py` & `travers-0.1.9/travers/graphs/internals.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import types
-
 from pathlib import Path
 
 import orjson
 
 from travers import xmler
 from travers.graphs.graph import Graph
 from travers.graphs.graph_traversal import GraphTraversal
```

### Comparing `travers-0.1.8/travers/version.py` & `travers-0.1.9/travers/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 __author__ = "joocer"
```

### Comparing `travers-0.1.8/travers/xmler.py` & `travers-0.1.9/travers/xmler.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from xml.etree import cElementTree as ElementTree  # nosec
 from collections import defaultdict
+from xml.etree import cElementTree as ElementTree  # nosec
 
 
 def _strip_namespace(entry):
     if isinstance(entry, dict):
-        for k in [k for k in entry.keys() if k.startswith("{")]:
+        for k in (k for k in entry.keys() if k.startswith("{")):
             k2 = k.split("}", 1)[1]
             entry[k2] = entry.pop(k)
-        for k in [k for k in entry.keys() if k.startswith("@{")]:
+        for k in (k for k in entry.keys() if k.startswith("@{")):
             k2 = k.split("}", 1)[1]
             entry[f"@{k2}"] = entry.pop(k)
         for child in entry:
             if isinstance(entry[child], (list, dict)):
                 _strip_namespace(entry[child])
     if isinstance(entry, list):
         for child in entry:
```

