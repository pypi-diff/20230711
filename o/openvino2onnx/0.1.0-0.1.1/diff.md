# Comparing `tmp/openvino2onnx-0.1.0.tar.gz` & `tmp/openvino2onnx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvino2onnx-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openvino2onnx-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openvino2onnx-0.1.0.tar` & `openvino2onnx-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0        0 2023-07-02 03:33:52.165349 openvino2onnx-0.1.0/.github/words_bag.txt
--rw-r--r--   0        0        0     1279 2023-07-02 08:01:15.072831 openvino2onnx-0.1.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      756 2023-07-02 06:32:19.993506 openvino2onnx-0.1.0/.github/workflows/unittests.yml
--rw-r--r--   0        0        0      112 2023-07-02 03:39:49.201424 openvino2onnx-0.1.0/.gitignore
--rw-r--r--   0        0        0      829 2023-07-02 07:03:14.773393 openvino2onnx-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1098 2023-07-02 03:38:31.602066 openvino2onnx-0.1.0/LICENSE
--rw-r--r--   0        0        0      286 2023-07-02 05:49:32.964854 openvino2onnx-0.1.0/README.md
--rw-r--r--   0        0        0      196 2023-07-02 08:01:15.074833 openvino2onnx-0.1.0/openvino2onnx/__init__.py
--rw-r--r--   0        0        0     4971 2023-07-02 06:33:32.684644 openvino2onnx-0.1.0/openvino2onnx/builder.py
--rw-r--r--   0        0        0        0 2023-07-02 08:01:15.075833 openvino2onnx-0.1.0/openvino2onnx/cli/__init__.py
--rw-r--r--   0        0        0     1768 2023-07-02 08:01:15.076831 openvino2onnx-0.1.0/openvino2onnx/cli/main_cli.py
--rw-r--r--   0        0        0     1199 2023-07-02 08:01:15.077831 openvino2onnx-0.1.0/openvino2onnx/cli/omz_download.py
--rw-r--r--   0        0        0     4672 2023-07-02 06:07:42.919880 openvino2onnx-0.1.0/openvino2onnx/ir11.py
--rw-r--r--   0        0        0      207 2023-07-01 03:29:57.962412 openvino2onnx-0.1.0/openvino2onnx/legalize/__init__.py
--rw-r--r--   0        0        0      772 2023-07-02 08:01:15.078832 openvino2onnx-0.1.0/openvino2onnx/legalize/compose.py
--rw-r--r--   0        0        0     3000 2023-07-02 06:24:12.226151 openvino2onnx-0.1.0/openvino2onnx/legalize/fold_const.py
--rw-r--r--   0        0        0      602 2023-07-02 06:24:27.231265 openvino2onnx-0.1.0/openvino2onnx/legalize/mutator.py
--rw-r--r--   0        0        0     5216 2023-07-02 03:51:54.106330 openvino2onnx-0.1.0/openvino2onnx/legalize/single_node.py
--rw-r--r--   0        0        0      523 2023-07-02 06:25:38.153144 openvino2onnx-0.1.0/openvino2onnx/legalize/utils.py
--rw-r--r--   0        0        0      930 2023-07-02 06:09:12.801701 openvino2onnx-0.1.0/openvino2onnx/mapping.py
--rw-r--r--   0        0        0     2634 2023-07-02 06:38:00.401629 openvino2onnx-0.1.0/openvino2onnx/ops/__init__.py
--rw-r--r--   0        0        0      207 2023-06-30 10:50:48.931036 openvino2onnx-0.1.0/openvino2onnx/ops/activation.py
--rw-r--r--   0        0        0      394 2023-07-01 07:14:54.978839 openvino2onnx-0.1.0/openvino2onnx/ops/concat.py
--rw-r--r--   0        0        0     1732 2023-06-30 10:53:59.903857 openvino2onnx-0.1.0/openvino2onnx/ops/conv.py
--rw-r--r--   0        0        0     1228 2023-07-02 06:36:28.024510 openvino2onnx-0.1.0/openvino2onnx/ops/convert.py
--rw-r--r--   0        0        0      304 2023-06-30 14:12:38.077664 openvino2onnx-0.1.0/openvino2onnx/ops/element_wise.py
--rw-r--r--   0        0        0      394 2023-07-01 12:02:25.216027 openvino2onnx-0.1.0/openvino2onnx/ops/gather.py
--rw-r--r--   0        0        0     1475 2023-07-01 12:46:28.795270 openvino2onnx-0.1.0/openvino2onnx/ops/interpolate.py
--rw-r--r--   0        0        0     1581 2023-07-02 03:52:03.790201 openvino2onnx-0.1.0/openvino2onnx/ops/pool.py
--rw-r--r--   0        0        0      494 2023-07-01 06:37:14.021116 openvino2onnx-0.1.0/openvino2onnx/ops/strided_slice.py
--rw-r--r--   0        0        0      542 2023-07-02 03:50:06.140057 openvino2onnx-0.1.0/openvino2onnx/ops/transpose.py
--rw-r--r--   0        0        0     1016 2023-07-02 08:01:15.080832 openvino2onnx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1680 2023-07-02 07:01:11.972278 openvino2onnx-0.1.0/tests/test.py
--rw-r--r--   0        0        0      948 1970-01-01 00:00:00.000000 openvino2onnx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-02 03:33:52.165349 openvino2onnx-0.1.1/.github/words_bag.txt
+-rw-r--r--   0        0        0     1279 2023-07-02 08:01:15.072831 openvino2onnx-0.1.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      756 2023-07-02 06:32:19.993506 openvino2onnx-0.1.1/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0      112 2023-07-02 03:39:49.201424 openvino2onnx-0.1.1/.gitignore
+-rw-r--r--   0        0        0      829 2023-07-02 07:03:14.773393 openvino2onnx-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1098 2023-07-02 03:38:31.602066 openvino2onnx-0.1.1/LICENSE
+-rw-r--r--   0        0        0      286 2023-07-02 05:49:32.964854 openvino2onnx-0.1.1/README.md
+-rw-r--r--   0        0        0      196 2023-07-02 08:48:52.945705 openvino2onnx-0.1.1/openvino2onnx/__init__.py
+-rw-r--r--   0        0        0      167 2023-07-11 04:57:07.412504 openvino2onnx-0.1.1/openvino2onnx/__main__.py
+-rw-r--r--   0        0        0     4971 2023-07-02 06:33:32.684644 openvino2onnx-0.1.1/openvino2onnx/builder.py
+-rw-r--r--   0        0        0        0 2023-07-02 08:01:15.075833 openvino2onnx-0.1.1/openvino2onnx/cli/__init__.py
+-rw-r--r--   0        0        0     1624 2023-07-11 04:57:07.413407 openvino2onnx-0.1.1/openvino2onnx/cli/main_cli.py
+-rw-r--r--   0        0        0     1199 2023-07-02 08:01:15.077831 openvino2onnx-0.1.1/openvino2onnx/cli/omz_download.py
+-rw-r--r--   0        0        0     4672 2023-07-02 06:07:42.919880 openvino2onnx-0.1.1/openvino2onnx/ir11.py
+-rw-r--r--   0        0        0      207 2023-07-01 03:29:57.962412 openvino2onnx-0.1.1/openvino2onnx/legalize/__init__.py
+-rw-r--r--   0        0        0      772 2023-07-02 08:01:15.078832 openvino2onnx-0.1.1/openvino2onnx/legalize/compose.py
+-rw-r--r--   0        0        0     3257 2023-07-02 08:48:52.946741 openvino2onnx-0.1.1/openvino2onnx/legalize/fold_const.py
+-rw-r--r--   0        0        0      602 2023-07-02 06:24:27.231265 openvino2onnx-0.1.1/openvino2onnx/legalize/mutator.py
+-rw-r--r--   0        0        0     9202 2023-07-11 04:57:07.415411 openvino2onnx-0.1.1/openvino2onnx/legalize/single_node.py
+-rw-r--r--   0        0        0      523 2023-07-02 06:25:38.153144 openvino2onnx-0.1.1/openvino2onnx/legalize/utils.py
+-rw-r--r--   0        0        0      930 2023-07-02 06:09:12.801701 openvino2onnx-0.1.1/openvino2onnx/mapping.py
+-rw-r--r--   0        0        0     2634 2023-07-02 06:38:00.401629 openvino2onnx-0.1.1/openvino2onnx/ops/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-30 10:50:48.931036 openvino2onnx-0.1.1/openvino2onnx/ops/activation.py
+-rw-r--r--   0        0        0      394 2023-07-01 07:14:54.978839 openvino2onnx-0.1.1/openvino2onnx/ops/concat.py
+-rw-r--r--   0        0        0     1732 2023-06-30 10:53:59.903857 openvino2onnx-0.1.1/openvino2onnx/ops/conv.py
+-rw-r--r--   0        0        0     1228 2023-07-02 06:36:28.024510 openvino2onnx-0.1.1/openvino2onnx/ops/convert.py
+-rw-r--r--   0        0        0      304 2023-06-30 14:12:38.077664 openvino2onnx-0.1.1/openvino2onnx/ops/element_wise.py
+-rw-r--r--   0        0        0      394 2023-07-01 12:02:25.216027 openvino2onnx-0.1.1/openvino2onnx/ops/gather.py
+-rw-r--r--   0        0        0     1475 2023-07-01 12:46:28.795270 openvino2onnx-0.1.1/openvino2onnx/ops/interpolate.py
+-rw-r--r--   0        0        0     2900 2023-07-11 04:57:07.416409 openvino2onnx-0.1.1/openvino2onnx/ops/pool.py
+-rw-r--r--   0        0        0      232 2023-07-11 04:57:07.417414 openvino2onnx-0.1.1/openvino2onnx/ops/strided_slice.py
+-rw-r--r--   0        0        0      542 2023-07-02 03:50:06.140057 openvino2onnx-0.1.1/openvino2onnx/ops/transpose.py
+-rw-r--r--   0        0        0     1016 2023-07-02 08:01:15.080832 openvino2onnx-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1750 2023-07-02 08:48:52.949708 openvino2onnx-0.1.1/tests/test.py
+-rw-r--r--   0        0        0      948 1970-01-01 00:00:00.000000 openvino2onnx-0.1.1/PKG-INFO
```

### Comparing `openvino2onnx-0.1.0/.github/workflows/lint.yml` & `openvino2onnx-0.1.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/.github/workflows/unittests.yml` & `openvino2onnx-0.1.1/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/.pre-commit-config.yaml` & `openvino2onnx-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/LICENSE` & `openvino2onnx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/openvino2onnx/builder.py` & `openvino2onnx-0.1.1/openvino2onnx/builder.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/openvino2onnx/cli/main_cli.py` & `openvino2onnx-0.1.1/openvino2onnx/cli/main_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 """
 
 import tempfile
 from argparse import ArgumentParser
 from pathlib import Path
 
 import onnx
-from onnx.tools.replace_constants import replace_initializer_by_constant_of_shape
 
 from openvino2onnx import build, ir_to_graph
 from openvino2onnx.legalize import legalize
 
 
 def parse_args():
     """Parse command line"""
@@ -43,14 +42,13 @@
         with tempfile.TemporaryDirectory() as tmpdir:
             model_url = download_from_omz_link(model_url, tmpdir)
             graph = ir_to_graph(model_url)
     else:
         graph = ir_to_graph(model_url, args.model_bin)
     graph = legalize(graph)
     model = build(graph)
-    model = replace_initializer_by_constant_of_shape(model)
     if args.output is None:
         out_file = Path(model_url).stem + ".onnx"
     else:
         out_file = Path(args.output).with_suffix(".onnx")
     onnx.save(model, out_file)
     print(f"onnx file saved at {out_file}")
```

### Comparing `openvino2onnx-0.1.0/openvino2onnx/cli/omz_download.py` & `openvino2onnx-0.1.1/openvino2onnx/cli/omz_download.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/openvino2onnx/ir11.py` & `openvino2onnx-0.1.1/openvino2onnx/ir11.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/openvino2onnx/legalize/compose.py` & `openvino2onnx-0.1.1/openvino2onnx/legalize/compose.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/openvino2onnx/legalize/fold_const.py` & `openvino2onnx-0.1.1/openvino2onnx/legalize/fold_const.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,99 +1,102 @@
-"""
-Copyright Wenyi Tang 2023
-
-:Author: Wenyi Tang
-:Email: wenyitang@outlook.com
-
-"""
-
-import networkx as nx
-import numpy as np
-from onnx.reference import ReferenceEvaluator
-
-from openvino2onnx.builder import build
-from openvino2onnx.mapping import DTYPE2PREC
-
-
-def _make_output_for_node(graph: nx.DiGraph, node, port=None):
-    attrs = graph.nodes[node]
-    if port is None:
-        port = list(attrs["outputs"].keys())[0]
-    result_node = f"{node}_result{port}"
-    input_port = attrs["outputs"][port]
-    input_port.update(id="0", name=result_node)
-    graph.add_node(
-        result_node,
-        name=result_node,
-        type="Result",
-        version="opset1",
-        inputs={"0": input_port},
-    )
-    graph.add_edge(node, result_node, src=port, dst="0")
-    return result_node
-
-
-def fold_const_on_node(graph: nx.DiGraph, node, remove_nodes=True) -> np.ndarray:
-    """Fold the const path to node in the graph.
-
-    Args:
-        graph (nx.DiGraph): the graph
-        node (str): a node in the graph that can be folded
-        remove_nodes (bool, optional): If true, remove the folded node from graph.
-            Defaults to True.
-
-    Returns:
-        ndarray: evaluated const data
-    """
-    attrs = graph.nodes[node]
-    sources = nx.ancestors(graph, node)
-    subg: nx.DiGraph = nx.subgraph(graph, list(sources) + [node]).copy()
-    # all sources in subgraph must be Const
-    for i in nx.topological_sort(subg):
-        if subg.in_degree(i) != 0:
-            break
-        if subg.nodes[i]["type"] != "Const":
-            raise RuntimeError(f"node {attrs['name']} is not constant!")
-    if len(subg) == 1:
-        # quick solution for only 1 Const
-        const = graph.nodes[next(iter(subg))]["data"]
-    else:
-        subg.graph["input"] = []
-        subg.graph["output"] = [_make_output_for_node(subg, node)]
-        folder = ReferenceEvaluator(build(subg))
-        const = folder.run(None, {})[0]
-    if remove_nodes:
-        graph.remove_nodes_from(subg)
-    return const
-
-
-def expand_const_on_node(graph: nx.DiGraph, node, data, port=None):
-    """Add a const node of data to the node input.
-
-    Args:
-        graph (nx.DiGraph): the graph
-        node (str):  a node in graph to expand
-        data (ndarray): const data
-        port (str, optional): specify a input port id. Defaults to None.
-    """
-    attrs = graph.nodes[node]
-    if port is None:
-        port = len(attrs["inputs"])
-    if port in attrs["inputs"]:
-        raise ValueError(f"input:{port} at {attrs['name']} is in use.")
-    # make a Const
-    const_node = f"{node}_const{port}"
-    graph.add_node(
-        const_node,
-        name=const_node,
-        type="Const",
-        version="opset1",
-        shape=",".join(map(str, data.shape)),
-        outputs={
-            "0": dict(
-                precision=DTYPE2PREC[np.dtype(data.dtype).name],
-                dim=",".join(map(str, data.shape)),
-            )
-        },
-        data=data,
-    )
-    graph.add_edge(const_node, node, src="0", dst=port)
+"""
+Copyright Wenyi Tang 2023
+
+:Author: Wenyi Tang
+:Email: wenyitang@outlook.com
+
+"""
+
+import networkx as nx
+import numpy as np
+from onnx.reference import ReferenceEvaluator
+
+from openvino2onnx.builder import build
+from openvino2onnx.mapping import DTYPE2PREC, PREC2DTYPE
+
+
+def _make_output_for_node(graph: nx.DiGraph, node, port=None):
+    attrs = graph.nodes[node]
+    if port is None:
+        port = list(attrs["outputs"].keys())[0]
+    result_node = f"{node}_result{port}"
+    input_port = attrs["outputs"][port]
+    input_port.update(id="0", name=result_node)
+    graph.add_node(
+        result_node,
+        name=result_node,
+        type="Result",
+        version="opset1",
+        inputs={"0": input_port},
+    )
+    graph.add_edge(node, result_node, src=port, dst="0")
+    return result_node
+
+
+def fold_const_on_node(graph: nx.DiGraph, node, remove_nodes=True) -> np.ndarray:
+    """Fold the const path to node in the graph.
+
+    Args:
+        graph (nx.DiGraph): the graph
+        node (str): a node in the graph that can be folded
+        remove_nodes (bool, optional): If true, remove the folded node from graph.
+            Defaults to True.
+
+    Returns:
+        ndarray: evaluated const data
+    """
+    attrs = graph.nodes[node]
+    sources = nx.ancestors(graph, node)
+    subg: nx.DiGraph = nx.subgraph(graph, list(sources) + [node]).copy()
+    # all sources in subgraph must be Const
+    for i in nx.topological_sort(subg):
+        if subg.in_degree(i) != 0:
+            break
+        if subg.nodes[i]["type"] != "Const":
+            raise RuntimeError(f"node {attrs['name']} is not constant!")
+    if len(subg) == 1:
+        # quick solution for only 1 Const
+        const = graph.nodes[next(iter(subg))]["data"]
+    else:
+        subg.graph["input"] = []
+        subg.graph["output"] = [_make_output_for_node(subg, node)]
+        folder = ReferenceEvaluator(build(subg))
+        const = folder.run(None, {})[0]
+    if remove_nodes:
+        graph.remove_nodes_from(subg)
+    for out in attrs["outputs"].values():
+        if prec := out.get("precision"):
+            const = np.array(const, dtype=PREC2DTYPE[prec])
+    return const
+
+
+def expand_const_on_node(graph: nx.DiGraph, node, data, port=None):
+    """Add a const node of data to the node input.
+
+    Args:
+        graph (nx.DiGraph): the graph
+        node (str):  a node in graph to expand
+        data (ndarray): const data
+        port (str, optional): specify a input port id. Defaults to None.
+    """
+    attrs = graph.nodes[node]
+    if port is None:
+        port = len(attrs["inputs"])
+    if port in attrs["inputs"]:
+        raise ValueError(f"input:{port} at {attrs['name']} is in use.")
+    # make a Const
+    const_node = f"{node}_const{port}"
+    graph.add_node(
+        const_node,
+        name=const_node,
+        type="Const",
+        version="opset1",
+        shape=",".join(map(str, data.shape)),
+        outputs={
+            "0": dict(
+                precision=DTYPE2PREC[np.dtype(data.dtype).name],
+                dim=",".join(map(str, data.shape)),
+            )
+        },
+        data=data,
+    )
+    graph.add_edge(const_node, node, src="0", dst=port)
```

### Comparing `openvino2onnx-0.1.0/openvino2onnx/legalize/mutator.py` & `openvino2onnx-0.1.1/openvino2onnx/legalize/mutator.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/openvino2onnx/legalize/utils.py` & `openvino2onnx-0.1.1/openvino2onnx/legalize/utils.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/openvino2onnx/mapping.py` & `openvino2onnx-0.1.1/openvino2onnx/mapping.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/openvino2onnx/ops/__init__.py` & `openvino2onnx-0.1.1/openvino2onnx/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/openvino2onnx/ops/conv.py` & `openvino2onnx-0.1.1/openvino2onnx/ops/conv.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/openvino2onnx/ops/convert.py` & `openvino2onnx-0.1.1/openvino2onnx/ops/convert.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/openvino2onnx/ops/interpolate.py` & `openvino2onnx-0.1.1/openvino2onnx/ops/interpolate.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/openvino2onnx/ops/transpose.py` & `openvino2onnx-0.1.1/openvino2onnx/ops/transpose.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/pyproject.toml` & `openvino2onnx-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.0/tests/test.py` & `openvino2onnx-0.1.1/tests/test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-"""
-Copyright Wenyi Tang 2023
-
-:Author: Wenyi Tang
-:Email: wenyitang@outlook.com
-
-"""
-import tempfile
-import unittest
-from pathlib import Path
-
-import numpy as np
-import onnx
-from openvino import runtime
-
-from openvino2onnx import builder, ir11
-from openvino2onnx.legalize import legalize
-
-
-class TestOpenvinoConvert(unittest.TestCase):
-    def build_model(self, model_path):
-        g = ir11.ir_to_graph(model_path)
-        legalize(g)
-        model = builder.build(g)
-
-        onnx.checker.check_model(model)
-
-        with tempfile.TemporaryDirectory() as tmpdir:
-            onnx.save(model, f"{tmpdir}/test.onnx")
-            test = runtime.compile_model(f"{tmpdir}/test.onnx")
-        ref = runtime.compile_model(model_path)
-
-        inputs = np.empty(test.input().shape, dtype="float32")
-        out_ref = ref(inputs)
-        out_test = test(inputs)
-        name_not_match = False
-        for k in out_ref:
-            if not any(i in out_test for i in k.names):
-                name_not_match = True
-                continue
-            for name in k.names:
-                if name in out_test:
-                    self.assertTrue(np.allclose(out_ref[name], out_test[name]))
-        if name_not_match and len(out_ref) == len(out_test):
-            for x, y in zip(out_ref.values(), out_test.values()):
-                self.assertTrue(np.allclose(x, y))
-            name_not_match = False
-        self.assertFalse(name_not_match)
-
-    def test_build_models(self):
-        cwd = Path(__file__).parent
-        for model in cwd.rglob("*.xml"):
-            with self.subTest(model=model):
-                self.build_model(model)
-
-
-if __name__ == "__main__":
-    unittest.main()
+"""
+Copyright Wenyi Tang 2023
+
+:Author: Wenyi Tang
+:Email: wenyitang@outlook.com
+
+"""
+import tempfile
+import unittest
+from pathlib import Path
+
+import numpy as np
+import onnx
+from openvino import runtime
+
+from openvino2onnx import builder, ir11
+from openvino2onnx.legalize import legalize
+
+
+class TestOpenvinoConvert(unittest.TestCase):
+    def build_model(self, model_path):
+        g = ir11.ir_to_graph(model_path)
+        legalize(g)
+        model = builder.build(g)
+
+        onnx.checker.check_model(model)
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            onnx.save(model, f"{tmpdir}/test.onnx")
+            test = runtime.compile_model(f"{tmpdir}/test.onnx")
+        ref = runtime.compile_model(model_path)
+
+        inputs = [np.empty(i.shape, dtype="float32") for i in test.inputs]
+        out_ref = ref(inputs)
+        out_test = test(inputs)
+        name_not_match = False
+        for k in out_ref:
+            if not any(i in out_test for i in k.names):
+                name_not_match = True
+                continue
+            for name in k.names:
+                if name in out_test:
+                    self.assertTrue(np.allclose(out_ref[name], out_test[name]))
+        if name_not_match and len(out_ref) == len(out_test):
+            for x, y in zip(out_ref.values(), out_test.values()):
+                self.assertTrue(np.allclose(x, y))
+            name_not_match = False
+        self.assertFalse(name_not_match)
+
+    def test_build_models(self):
+        cwd = Path(__file__).parent
+        for model in cwd.rglob("*.xml"):
+            with self.subTest(model=model):
+                self.build_model(model)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `openvino2onnx-0.1.0/PKG-INFO` & `openvino2onnx-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openvino2onnx
-Version: 0.1.0
+Version: 0.1.1
 Summary: openvino2onnx is a tool to convert openvino IR format to ONNX.
 Author-email: Wenyi Tang <wenyitang@outlook.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: onnx >= 1.8.1
 Requires-Dist: networkx
```

