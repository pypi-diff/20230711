# Comparing `tmp/pipdeptree-2.9.4.tar.gz` & `tmp/pipdeptree-2.9.5.tar.gz`

## Comparing `pipdeptree-2.9.4.tar` & `pipdeptree-2.9.5.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/CHANGES.md
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/tox.ini
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/.github/FUNDING.yml
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/.github/dependabot.yml
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/.github/workflows/check.yml
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/.github/workflows/release.yml
--rw-r--r--   0        0        0    39608 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/src/pipdeptree/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/src/pipdeptree/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/src/pipdeptree/version.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/tests/guess_version_setuptools.py
--rw-r--r--   0        0        0    41622 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/tests/test_pipdeptree.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/LICENSE
--rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/pyproject.toml
--rw-r--r--   0        0        0    15717 2020-02-02 00:00:00.000000 pipdeptree-2.9.4/PKG-INFO
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/CHANGES.md
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/tox.ini
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.github/FUNDING.yml
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.github/release.yml
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.github/workflows/check.yml
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.github/workflows/release.yml
+-rw-r--r--   0        0        0    43408 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/src/pipdeptree/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/src/pipdeptree/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/src/pipdeptree/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/src/pipdeptree/version.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/tests/guess_version_setuptools.py
+-rw-r--r--   0        0        0    42899 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/tests/test_pipdeptree.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/LICENSE
+-rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/README.md
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/pyproject.toml
+-rw-r--r--   0        0        0    15717 2020-02-02 00:00:00.000000 pipdeptree-2.9.5/PKG-INFO
```

### Comparing `pipdeptree-2.9.4/.pre-commit-config.yaml` & `pipdeptree-2.9.5/.pre-commit-config.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: end-of-file-fixer
       - id: trailing-whitespace
-  - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.277"
-    hooks:
-      - id: ruff
-        args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/tox-dev/tox-ini-fmt
     rev: "1.3.1"
     hooks:
@@ -24,11 +19,16 @@
       - id: pyproject-fmt
         additional_dependencies: ["tox>=4.6.4"]
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0"
     hooks:
       - id: prettier
         args: ["--print-width=120", "--prose-wrap=always"]
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: "v0.0.277"
+    hooks:
+      - id: ruff
+        args: [--fix, --exit-non-zero-on-fix]
   - repo: meta
     hooks:
       - id: check-hooks-apply
       - id: check-useless-excludes
```

### Comparing `pipdeptree-2.9.4/CHANGES.md` & `pipdeptree-2.9.5/CHANGES.md`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.4/.github/workflows/check.yml` & `pipdeptree-2.9.5/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.4/.github/workflows/release.yml` & `pipdeptree-2.9.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.4/src/pipdeptree/__init__.py` & `pipdeptree-2.9.5/src/pipdeptree/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 from __future__ import annotations
 
-import argparse
 import fnmatch
 import inspect
 import json
 import os
 import shutil
 import subprocess
 import sys
 import tempfile
+from abc import ABC, abstractmethod
+from argparse import ArgumentParser, Namespace
 from collections import defaultdict, deque
-from collections.abc import Mapping
 from importlib import import_module
 from itertools import chain
 from pathlib import Path
 from textwrap import dedent
+from typing import TYPE_CHECKING, Any, Iterator, List, Mapping, TypeVar, cast
 
-from pip._vendor import pkg_resources
+from pip._vendor.pkg_resources import Distribution, Requirement
 
 from .version import version as __version__
 
 try:
     from pip._internal.operations.freeze import FrozenRequirement
 except ImportError:
-    from pip import FrozenRequirement
+    from pip import FrozenRequirement  # type: ignore[attr-defined, no-redef]
 
 
-def sorted_tree(tree):
+if TYPE_CHECKING:
+    from typing import Literal
+
+    from pip._internal.metadata import BaseDistribution
+    from pip._vendor.pkg_resources import DistInfoDistribution
+
+
+def sorted_tree(tree: dict[DistPackage, list[ReqPackage]]) -> dict[DistPackage, list[ReqPackage]]:
     """
     Sorts the dict representation of the tree. The root packages as well as the intermediate packages are sorted in the
     alphabetical order of the package names.
 
-    :param dict tree: the pkg dependency tree obtained by calling `construct_tree` function
+    :param tree: the pkg dependency tree obtained by calling `construct_tree` function
     :returns: sorted tree
-    :rtype: dict
     """
     return {k: sorted(v) for k, v in sorted(tree.items())}
 
 
-def guess_version(pkg_key, default="?"):
+def guess_version(pkg_key: str, default: str = "?") -> str:
     """
     Guess the version of a pkg when pip doesn't provide it.
 
-    :param str pkg_key: key of the package
-    :param str default: default version to return if unable to find
+    :param pkg_key: key of the package
+    :param default: default version to return if unable to find
     :returns: version
-    :rtype: string
     """
     try:
         if sys.version_info >= (3, 8):  # pragma: >=3.8 cover
             import importlib.metadata as importlib_metadata
         else:  # pragma: <3.8 cover
             import importlib_metadata
         return importlib_metadata.version(pkg_key)
@@ -65,189 +71,199 @@
     else:
         v = getattr(m, "__version__", default)
         if inspect.ismodule(v):
             return getattr(v, "__version__", default)
         return v
 
 
-def frozen_req_from_dist(dist):
+def frozen_req_from_dist(dist: Distribution) -> FrozenRequirement:
     # The `pip._internal.metadata` modules were introduced in 21.1.1
     # and the `pip._internal.operations.freeze.FrozenRequirement`
     # class now expects dist to be a subclass of
     # `pip._internal.metadata.BaseDistribution`, however the
     # `pip._internal.utils.misc.get_installed_distributions` continues
     # to return objects of type
     # pip._vendor.pkg_resources.DistInfoDistribution.
     #
     # This is a hacky backward compatible (with older versions of pip)
     # fix.
     try:
         from pip._internal import metadata
     except ImportError:
-        pass
+        our_dist: BaseDistribution = dist  # type: ignore[assignment]
     else:
-        dist = metadata.pkg_resources.Distribution(dist)
+        our_dist = metadata.pkg_resources.Distribution(dist)
 
     try:
-        return FrozenRequirement.from_dist(dist)
+        return FrozenRequirement.from_dist(our_dist)
     except TypeError:
-        return FrozenRequirement.from_dist(dist, [])
+        return FrozenRequirement.from_dist(our_dist, [])  # type: ignore[call-arg]
 
 
-class Package:
+class Package(ABC):
     """
     Abstract class for wrappers around objects that pip returns. This class needs to be subclassed with implementations
     for `render_as_root` and `render_as_branch` methods.
     """
 
-    def __init__(self, obj) -> None:
-        self._obj = obj
-        self.project_name = obj.project_name
-        self.key = obj.key
-
-    def render_as_root(self, frozen):  # noqa: ARG002
-        return NotImplementedError
-
-    def render_as_branch(self, frozen):  # noqa: ARG002
-        return NotImplementedError
-
-    def render(self, parent=None, frozen=False):  # noqa: FBT002
+    def __init__(self, obj: DistInfoDistribution) -> None:
+        self._obj: DistInfoDistribution = obj
+        self.project_name: str = obj.project_name
+        self.key: str = obj.key
+
+    @abstractmethod
+    def render_as_root(self, frozen: bool) -> str:  # noqa: FBT001
+        raise NotImplementedError
+
+    @abstractmethod
+    def render_as_branch(self, frozen: bool) -> str:  # noqa: FBT001
+        raise NotImplementedError
+
+    def render(
+        self,
+        parent: DistPackage | ReqPackage | None = None,
+        frozen: bool = False,  # noqa: FBT001, FBT002
+    ) -> str:
         if not parent:
             return self.render_as_root(frozen)
         return self.render_as_branch(frozen)
 
     @staticmethod
-    def frozen_repr(obj):
+    def frozen_repr(obj: DistInfoDistribution) -> str:
         fr = frozen_req_from_dist(obj)
         return str(fr).strip()
 
-    def __getattr__(self, key):
+    def __getattr__(self, key: str) -> Any:
         return getattr(self._obj, key)
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__}("{self.key}")>'
 
-    def __lt__(self, rhs):
+    def __lt__(self, rhs: Package) -> bool:
         return self.key < rhs.key
 
 
 class DistPackage(Package):
     """
     Wrapper class for pkg_resources.Distribution instances.
 
     :param obj: pkg_resources.Distribution to wrap over
     :param req: optional ReqPackage object to associate this DistPackage with. This is useful for displaying the tree
         in reverse
     """
 
-    def __init__(self, obj, req=None) -> None:
+    def __init__(self, obj: DistInfoDistribution, req: ReqPackage | None = None) -> None:
         super().__init__(obj)
         self.version_spec = None
         self.req = req
 
-    def render_as_root(self, frozen):
+    def render_as_root(self, frozen: bool) -> str:  # noqa: FBT001
         if not frozen:
             return f"{self.project_name}=={self.version}"
         return self.__class__.frozen_repr(self._obj)
 
-    def render_as_branch(self, frozen):
+    def render_as_branch(self, frozen: bool) -> str:  # noqa: FBT001
         assert self.req is not None  # noqa: S101
         if not frozen:
             parent_ver_spec = self.req.version_spec
             parent_str = self.req.project_name
             if parent_ver_spec:
                 parent_str += parent_ver_spec
             return f"{self.project_name}=={self.version} [requires: {parent_str}]"
         return self.render_as_root(frozen)
 
-    def as_requirement(self):
+    def as_requirement(self) -> ReqPackage:
         """Return a ReqPackage representation of this DistPackage."""
-        return ReqPackage(self._obj.as_requirement(), dist=self)
+        return ReqPackage(self._obj.as_requirement(), dist=self)  # type: ignore[no-untyped-call]
 
-    def as_parent_of(self, req):
+    def as_parent_of(self, req: ReqPackage | None) -> DistPackage:
         """
         Return a DistPackage instance associated to a requirement. This association is necessary for reversing the
         PackageDAG.
 
         If `req` is None, and the `req` attribute of the current instance is also None, then the same instance will be
         returned.
 
         :param ReqPackage req: the requirement to associate with
         :returns: DistPackage instance
         """
         if req is None and self.req is None:
             return self
         return self.__class__(self._obj, req)
 
-    def as_dict(self):
+    def as_dict(self) -> dict[str, str]:
         return {"key": self.key, "package_name": self.project_name, "installed_version": self.version}
 
 
 class ReqPackage(Package):
     """
     Wrapper class for Requirements instance.
 
     :param obj: The `Requirements` instance to wrap over
     :param dist: optional `pkg_resources.Distribution` instance for this requirement
     """
 
     UNKNOWN_VERSION = "?"
 
-    def __init__(self, obj, dist=None) -> None:
+    def __init__(self, obj: Requirement, dist: DistPackage | None = None) -> None:
         super().__init__(obj)
         self.dist = dist
 
     @property
-    def version_spec(self):
+    def version_spec(self) -> str | None:
         specs = sorted(self._obj.specs, reverse=True)  # `reverse` makes '>' prior to '<'
         return ",".join(["".join(sp) for sp in specs]) if specs else None
 
     @property
-    def installed_version(self):
+    def installed_version(self) -> str:
         if not self.dist:
             return guess_version(self.key, self.UNKNOWN_VERSION)
-        return self.dist.version
+        return cast(str, self.dist.version)
 
     @property
-    def is_missing(self):
+    def is_missing(self) -> bool:
         return self.installed_version == self.UNKNOWN_VERSION
 
-    def is_conflicting(self):
+    def is_conflicting(self) -> bool:
         """If installed version conflicts with required version."""
         # unknown installed version is also considered conflicting
         if self.installed_version == self.UNKNOWN_VERSION:
             return True
         ver_spec = self.version_spec if self.version_spec else ""
         req_version_str = f"{self.project_name}{ver_spec}"
-        req_obj = pkg_resources.Requirement.parse(req_version_str)
+        req_obj = Requirement.parse(req_version_str)  # type: ignore[no-untyped-call]
         return self.installed_version not in req_obj
 
-    def render_as_root(self, frozen):
+    def render_as_root(self, frozen: bool) -> str:  # noqa: FBT001
         if not frozen:
             return f"{self.project_name}=={self.installed_version}"
         if self.dist:
             return self.__class__.frozen_repr(self.dist._obj)  # noqa: SLF001
         return self.project_name
 
-    def render_as_branch(self, frozen):
+    def render_as_branch(self, frozen: bool) -> str:  # noqa: FBT001
         if not frozen:
             req_ver = self.version_spec if self.version_spec else "Any"
             return f"{self.project_name} [required: {req_ver}, installed: {self.installed_version}]"
         return self.render_as_root(frozen)
 
-    def as_dict(self):
+    def as_dict(self) -> dict[str, str | None]:
         return {
             "key": self.key,
             "package_name": self.project_name,
             "installed_version": self.installed_version,
             "required_version": self.version_spec,
         }
 
 
-class PackageDAG(Mapping):
+_T = TypeVar("_T")
+_V = TypeVar("_V")
+
+
+class PackageDAG(Mapping[DistPackage, List[ReqPackage]]):
     """
     Representation of Package dependencies as directed acyclic graph using a dict (Mapping) as the underlying
     datastructure.
 
     The nodes and their relationships (edges) are internally stored using a map as follows,
 
     {a: [b, c],
@@ -263,81 +279,78 @@
 
     A node is expected to be an instance of a subclass of `Package`. The keys are must be of class `DistPackage` and
     each item in values must be of class `ReqPackage`. (See also ReversedPackageDAG where the key and value types are
     interchanged).
     """
 
     @classmethod
-    def from_pkgs(cls, pkgs):
-        pkgs = [DistPackage(p) for p in pkgs]
-        idx = {p.key: p for p in pkgs}
-        m = {}
-        for p in pkgs:
+    def from_pkgs(cls, pkgs: list[DistInfoDistribution]) -> PackageDAG:
+        dist_pkgs = [DistPackage(p) for p in pkgs]
+        idx = {p.key: p for p in dist_pkgs}
+        m: dict[DistPackage, list[ReqPackage]] = {}
+        for p in dist_pkgs:
             reqs = []
             for r in p.requires():
                 d = idx.get(r.key)
                 # pip's _vendor.packaging.requirements.Requirement uses the exact casing of a dependency's name found in
                 # a project's build config, which is not ideal when rendering.
                 # See https://github.com/tox-dev/pipdeptree/issues/242
                 r.project_name = d.project_name if d is not None else r.project_name
                 pkg = ReqPackage(r, d)
                 reqs.append(pkg)
             m[p] = reqs
 
         return cls(m)
 
-    def __init__(self, m) -> None:
+    def __init__(self, m: dict[DistPackage, list[ReqPackage]]) -> None:
         """
         Initialize the PackageDAG object.
 
         :param dict m: dict of node objects (refer class docstring)
         :returns: None
         :rtype: NoneType
 
         """
-        self._obj = m
-        self._index = {p.key: p for p in list(self._obj)}
+        self._obj: dict[DistPackage, list[ReqPackage]] = m
+        self._index: dict[str, DistPackage] = {p.key: p for p in list(self._obj)}
 
-    def get_node_as_parent(self, node_key):
+    def get_node_as_parent(self, node_key: str) -> DistPackage | None:
         """
         Get the node from the keys of the dict representing the DAG.
 
         This method is useful if the dict representing the DAG contains different kind of objects in keys and values.
         Use this method to look up a node obj as a parent (from the keys of the dict) given a node key.
 
         :param node_key: identifier corresponding to key attr of node obj
         :returns: node obj (as present in the keys of the dict)
-        :rtype: Object
         """
         try:
             return self._index[node_key]
         except KeyError:
             return None
 
-    def get_children(self, node_key):
+    def get_children(self, node_key: str) -> list[ReqPackage]:
         """
         Get child nodes for a node by its key.
 
-        :param str node_key: key of the node to get children of
-        :returns: list of child nodes
-        :rtype: ReqPackage[]
+        :param node_key: key of the node to get children of
+        :returns: child nodes
         """
         node = self.get_node_as_parent(node_key)
         return self._obj[node] if node else []
 
-    def filter_nodes(self, include, exclude):  # noqa: C901, PLR0912
+    def filter_nodes(self, include: set[str] | None, exclude: set[str] | None) -> PackageDAG:  # noqa: C901, PLR0912
         """
         Filters nodes in a graph by given parameters.
 
         If a node is included, then all it's children are also included.
 
-        :param set include: set of node keys to include (or None)
-        :param set exclude: set of node keys to exclude (or None)
+        :param include: set of node keys to include (or None)
+        :param exclude: set of node keys to exclude (or None)
         :returns: filtered version of the graph
-        :rtype: PackageDAG
         """
         # If neither of the filters are specified, short circuit
         if include is None and exclude is None:
             return self
 
         # Note: In following comparisons, we use lower cased values so
         # that user may specify `key` or `project_name`. As per the
@@ -351,16 +364,16 @@
         # Check for mutual exclusion of show_only and exclude sets
         # after normalizing the values to lowercase
         if include and exclude:
             assert not (include & exclude)  # noqa: S101
 
         # Traverse the graph in a depth first manner and filter the
         # nodes according to `show_only` and `exclude` sets
-        stack = deque()
-        m = {}
+        stack: deque[DistPackage] = deque()
+        m: dict[DistPackage, list[ReqPackage]] = {}
         seen = set()
         for node in self._obj:
             if any(fnmatch.fnmatch(node.key, e) for e in exclude):
                 continue
             if include is None or any(fnmatch.fnmatch(node.key, i) for i in include):
                 stack.append(node)
             while True:
@@ -379,58 +392,57 @@
                                 # a dependency is missing
                                 continue
                 else:
                     break
 
         return self.__class__(m)
 
-    def reverse(self):
+    def reverse(self) -> ReversedPackageDAG:
         """
         Reverse the DAG, or turn it upside-down.
 
         In other words, the directions of edges of the nodes in the DAG will be reversed.
 
         Note that this function purely works on the nodes in the graph. This implies that to perform a combination of
         filtering and reversing, the order in which `filter` and `reverse` methods should be applied is important. For
         e.g., if reverse is called on a filtered graph, then only the filtered nodes and it's children will be
         considered when reversing. On the other hand, if filter is called on reversed DAG, then the definition of
         "child" nodes is as per the reversed DAG.
 
         :returns: DAG in the reversed form
-        :rtype: ReversedPackageDAG
         """
-        m = defaultdict(list)
+        m: defaultdict[ReqPackage, list[DistPackage]] = defaultdict(list)
         child_keys = {r.key for r in chain.from_iterable(self._obj.values())}
         for k, vs in self._obj.items():
             for v in vs:
                 # if v is already added to the dict, then ensure that
                 # we are using the same object. This check is required
                 # as we're using array mutation
                 try:
-                    node = [p for p in m if p.key == v.key][0]
+                    node: ReqPackage = [p for p in m if p.key == v.key][0]
                 except IndexError:  # noqa: PERF203
                     node = v
                 m[node].append(k.as_parent_of(v))
             if k.key not in child_keys:
                 m[k.as_requirement()] = []
-        return ReversedPackageDAG(dict(m))
+        return ReversedPackageDAG(dict(m))  # type: ignore[arg-type]
 
-    def sort(self):
+    def sort(self) -> PackageDAG:
         """
         Return sorted tree in which the underlying _obj dict is an dict, sorted alphabetically by the keys.
 
         :returns: Instance of same class with dict
         """
         return self.__class__(sorted_tree(self._obj))
 
     # Methods required by the abstract base class Mapping
-    def __getitem__(self, *args):
-        return self._obj.get(*args)
+    def __getitem__(self, arg: DistPackage) -> list[ReqPackage] | None:  # type: ignore[override]
+        return self._obj.get(arg)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[DistPackage]:
         return self._obj.__iter__()
 
     def __len__(self) -> int:
         return len(self._obj)
 
 
 class ReversedPackageDAG(PackageDAG):
@@ -439,71 +451,81 @@
 
     Similar to it's super class `PackageDAG`, the underlying datastructure is a dict, but here the keys are expected to
     be of type `ReqPackage` and each item in the values of type `DistPackage`.
 
     Typically, this object will be obtained by calling `PackageDAG.reverse`.
     """
 
-    def reverse(self):
+    def reverse(self) -> PackageDAG:  # type: ignore[override]
         """
         Reverse the already reversed DAG to get the PackageDAG again.
 
         :returns: reverse of the reversed DAG
-        :rtype: PackageDAG
         """
-        m = defaultdict(list)
+        m: defaultdict[DistPackage, list[ReqPackage]] = defaultdict(list)
         child_keys = {r.key for r in chain.from_iterable(self._obj.values())}
         for k, vs in self._obj.items():
             for v in vs:
                 try:
                     node = [p for p in m if p.key == v.key][0]
                 except IndexError:  # noqa: PERF203
                     node = v.as_parent_of(None)
-                m[node].append(k)
+                m[node].append(k)  # type: ignore[arg-type]
             if k.key not in child_keys:
                 m[k.dist] = []
         return PackageDAG(dict(m))
 
 
-def render_text(tree, max_depth, encoding, list_all=True, frozen=False):  # noqa: FBT002
+def render_text(
+    tree: PackageDAG,
+    max_depth: float,
+    encoding: str,
+    list_all: bool = True,  # noqa: FBT001, FBT002
+    frozen: bool = False,  # noqa: FBT001, FBT002
+) -> None:
     """
     Print tree as text on console.
 
-    :param dict tree: the package tree
-    :param bool list_all: whether to list all the pgks at the root level or only those that are the sub-dependencies
-    :param bool frozen: show the names of the pkgs in the output that's favourable to pip --freeze
+    :param tree: the package tree
+    :param list_all: whether to list all the pgks at the root level or only those that are the sub-dependencies
+    :param frozen: show the names of the pkgs in the output that's favourable to pip --freeze
     :returns: None
     """
     tree = tree.sort()
-    nodes = tree.keys()
+    nodes = list(tree.keys())
     branch_keys = {r.key for r in chain.from_iterable(tree.values())}
 
     if not list_all:
         nodes = [p for p in nodes if p.key not in branch_keys]
 
     if encoding in ("utf-8", "utf-16", "utf-32"):
         _render_text_with_unicode(tree, nodes, max_depth, frozen)
     else:
         _render_text_without_unicode(tree, nodes, max_depth, frozen)
 
 
-def _render_text_with_unicode(tree, nodes, max_depth, frozen):
+def _render_text_with_unicode(
+    tree: PackageDAG,
+    nodes: list[DistPackage],
+    max_depth: float,
+    frozen: bool,  # noqa: FBT001
+) -> None:
     use_bullets = not frozen
 
     def aux(  # noqa: PLR0913
-        node,
-        parent=None,
-        indent=0,
-        cur_chain=None,
-        prefix="",
-        depth=0,
-        has_grand_parent=False,  # noqa: FBT002
-        is_last_child=False,  # noqa: FBT002
-        parent_is_last_child=False,  # noqa: FBT002
-    ):
+        node: DistPackage | ReqPackage,
+        parent: DistPackage | ReqPackage | None = None,
+        indent: int = 0,
+        cur_chain: list[str] | None = None,
+        prefix: str = "",
+        depth: int = 0,
+        has_grand_parent: bool = False,  # noqa: FBT001, FBT002
+        is_last_child: bool = False,  # noqa: FBT001, FBT002
+        parent_is_last_child: bool = False,  # noqa: FBT001, FBT002
+    ) -> list[Any]:
         cur_chain = cur_chain or []
         node_str = node.render(parent, frozen)
         next_prefix = ""
         next_indent = indent + 2
 
         if parent:
             bullet = "├── "
@@ -549,18 +571,29 @@
         result += list(chain.from_iterable(children_strings))
         return result
 
     lines = chain.from_iterable([aux(p) for p in nodes])
     print("\n".join(lines))  # noqa: T201
 
 
-def _render_text_without_unicode(tree, nodes, max_depth, frozen):
+def _render_text_without_unicode(
+    tree: PackageDAG,
+    nodes: list[DistPackage],
+    max_depth: float,
+    frozen: bool,  # noqa: FBT001
+) -> None:
     use_bullets = not frozen
 
-    def aux(node, parent=None, indent=0, cur_chain=None, depth=0):
+    def aux(
+        node: DistPackage | ReqPackage,
+        parent: DistPackage | ReqPackage | None = None,
+        indent: int = 0,
+        cur_chain: list[str] | None = None,
+        depth: int = 0,
+    ) -> list[Any]:
         cur_chain = cur_chain or []
         node_str = node.render(parent, frozen)
         if parent:
             prefix = " " * indent + ("- " if use_bullets else "")
             node_str = prefix + node_str
         result = [node_str]
         children = [
@@ -571,60 +604,62 @@
         result += list(chain.from_iterable(children))
         return result
 
     lines = chain.from_iterable([aux(p) for p in nodes])
     print("\n".join(lines))  # noqa: T201
 
 
-def render_json(tree, indent):
+def render_json(tree: PackageDAG, indent: int) -> str:
     """
     Converts the tree into a flat json representation.
 
     The json repr will be a list of hashes, each hash having 2 fields:
       - package
       - dependencies: list of dependencies
 
-    :param dict tree: dependency tree
-    :param int indent: no. of spaces to indent json
+    :param tree: dependency tree
+    :param indent: no. of spaces to indent json
     :returns: json representation of the tree
-    :rtype: str
     """
     tree = tree.sort()
     return json.dumps(
         [{"package": k.as_dict(), "dependencies": [v.as_dict() for v in vs]} for k, vs in tree.items()],
         indent=indent,
     )
 
 
-def render_json_tree(tree, indent):
+def render_json_tree(tree: PackageDAG, indent: int) -> str:
     """
     Converts the tree into a nested json representation.
 
     The json repr will be a list of hashes, each hash having the following fields:
 
       - package_name
       - key
       - required_version
       - installed_version
       - dependencies: list of dependencies
 
-    :param dict tree: dependency tree
-    :param int indent: no. of spaces to indent json
+    :param tree: dependency tree
+    :param indent: no. of spaces to indent json
     :returns: json representation of the tree
-    :rtype: str
     """
     tree = tree.sort()
     branch_keys = {r.key for r in chain.from_iterable(tree.values())}
     nodes = [p for p in tree if p.key not in branch_keys]
 
-    def aux(node, parent=None, cur_chain=None):
+    def aux(
+        node: DistPackage | ReqPackage,
+        parent: DistPackage | ReqPackage | None = None,
+        cur_chain: list[str] | None = None,
+    ) -> dict[str, Any]:
         if cur_chain is None:
             cur_chain = [node.project_name]
 
-        d = node.as_dict()
+        d: dict[str, str | list[Any] | None] = node.as_dict()  # type: ignore[assignment]
         if parent:
             d["required_version"] = node.version_spec if node.version_spec else "Any"
         else:
             d["required_version"] = d["installed_version"]
 
         d["dependencies"] = [
             aux(c, parent=node, cur_chain=[*cur_chain, c.project_name])
@@ -633,19 +668,19 @@
         ]
 
         return d
 
     return json.dumps([aux(p) for p in nodes], indent=indent)
 
 
-def render_mermaid(tree) -> str:  # noqa: C901
+def render_mermaid(tree: PackageDAG) -> str:  # noqa: C901
     """
     Produce a Mermaid flowchart from the dependency graph.
 
-    :param dict tree: dependency graph
+    :param tree: dependency graph
     """
     # List of reserved keywords in Mermaid that cannot be used as node names.
     # See: https://github.com/mermaid-js/mermaid/issues/4182#issuecomment-1454787806
     reserved_ids: set[str] = {
         "C4Component",
         "C4Container",
         "C4Deployment",
@@ -663,15 +698,15 @@
         "flowchart-v2",
         "graph",
         "interpolate",
         "linkStyle",
         "style",
         "subgraph",
     }
-    node_ids_map: dict[str:str] = {}
+    node_ids_map: dict[str, str] = {}
 
     def mermaid_id(key: str) -> str:
         """Returns a valid Mermaid node ID from a string."""
         # If we have already seen this key, return the canonical ID.
         canonical_id = node_ids_map.get(key)
         if canonical_id is not None:
             return canonical_id
@@ -731,15 +766,19 @@
     output += f"\n{indent}".join(node for node in sorted(nodes))
     output += "\n" + indent
     output += f"\n{indent}".join(edge for edge in sorted(edges))
     output += "\n"
     return output
 
 
-def dump_graphviz(tree, output_format="dot", is_reverse=False):  # noqa: C901, FBT002, PLR0912
+def dump_graphviz(  # noqa: C901, PLR0912
+    tree: PackageDAG,
+    output_format: str = "dot",
+    is_reverse: bool = False,  # noqa: FBT001, FBT002
+) -> str | bytes:
     """
     Output dependency graph as one of the supported GraphViz output formats.
 
     :param dict tree: dependency graph
     :param string output_format: output format
     :param bool is_reverse: reverse or not
     :returns: representation of tree in the specified output format
@@ -772,54 +811,54 @@
     if output_format not in valid_formats:
         print(f"{output_format} is not a supported output format.", file=sys.stderr)  # noqa: T201
         print(f"Supported formats are: {', '.join(sorted(valid_formats))}", file=sys.stderr)  # noqa: T201
         raise SystemExit(1)
 
     graph = Digraph(format=output_format)
 
-    if not is_reverse:
+    if is_reverse:
+        for dep_rev, parents in tree.items():
+            dep_label = f"{dep_rev.project_name}\\n{dep_rev.installed_version}"
+            graph.node(dep_rev.key, label=dep_label)
+            for parent in parents:
+                # req reference of the dep associated with this
+                # particular parent package
+                req_ref = parent.req
+                edge_label = req_ref.version_spec or "any"
+                graph.edge(dep_rev.key, parent.key, label=edge_label)
+    else:
         for pkg, deps in tree.items():
             pkg_label = f"{pkg.project_name}\\n{pkg.version}"
             graph.node(pkg.key, label=pkg_label)
             for dep in deps:
                 edge_label = dep.version_spec or "any"
                 if dep.is_missing:
                     dep_label = f"{dep.project_name}\\n(missing)"
                     graph.node(dep.key, label=dep_label, style="dashed")
                     graph.edge(pkg.key, dep.key, style="dashed")
                 else:
                     graph.edge(pkg.key, dep.key, label=edge_label)
-    else:
-        for dep, parents in tree.items():
-            dep_label = f"{dep.project_name}\\n{dep.installed_version}"
-            graph.node(dep.key, label=dep_label)
-            for parent in parents:
-                # req reference of the dep associated with this
-                # particular parent package
-                req_ref = parent.req
-                edge_label = req_ref.version_spec or "any"
-                graph.edge(dep.key, parent.key, label=edge_label)
 
     # Allow output of dot format, even if GraphViz isn't installed.
     if output_format == "dot":
         # Emulates graphviz.dot.Dot.__iter__() to force the sorting of graph.body.
         # Fixes https://github.com/tox-dev/pipdeptree/issues/188
         # That way we can guarantee the output of the dot format is deterministic
         # and stable.
         return "".join([tuple(graph)[0], *sorted(graph.body), graph._tail])  # noqa: SLF001
 
     # As it's unknown if the selected output format is binary or not, try to
     # decode it as UTF8 and only print it out in binary if that's not possible.
     try:
-        return graph.pipe().decode("utf-8")
+        return graph.pipe().decode("utf-8")  # type: ignore[no-any-return]
     except UnicodeDecodeError:
-        return graph.pipe()
+        return graph.pipe()  # type: ignore[no-any-return]
 
 
-def print_graphviz(dump_output):
+def print_graphviz(dump_output: str | bytes) -> None:
     """
     Dump the data generated by GraphViz to stdout.
 
     :param dump_output: The output from dump_graphviz
     """
     if hasattr(dump_output, "encode"):
         print(dump_output)  # noqa: T201
@@ -842,57 +881,61 @@
     for package, requires in tree.items():
         for req in requires:
             if req.is_conflicting():
                 conflicting[package].append(req)  # noqa: PERF401
     return conflicting
 
 
-def render_conflicts_text(conflicts):
+def render_conflicts_text(conflicts: dict[DistPackage, list[ReqPackage]]) -> None:
     if conflicts:
         print("Warning!!! Possibly conflicting dependencies found:", file=sys.stderr)  # noqa: T201
         # Enforce alphabetical order when listing conflicts
         pkgs = sorted(conflicts.keys())
         for p in pkgs:
             pkg = p.render_as_root(False)  # noqa: FBT003
             print(f"* {pkg}", file=sys.stderr)  # noqa: T201
             for req in conflicts[p]:
                 req_str = req.render_as_branch(False)  # noqa: FBT003
                 print(f" - {req_str}", file=sys.stderr)  # noqa: T201
 
 
-def cyclic_deps(tree):
+def cyclic_deps(tree: PackageDAG) -> list[tuple[DistPackage, ReqPackage, ReqPackage]]:
     """
     Return cyclic dependencies as list of tuples.
 
-    :param PackageDAG tree: package tree/dag
+    :param  tree: package tree/dag
     :returns: list of tuples representing cyclic dependencies
-    :rtype: list
+
     """
     index = {p.key: {r.key for r in rs} for p, rs in tree.items()}
-    cyclic = []
+    cyclic: list[tuple[DistPackage, ReqPackage, ReqPackage]] = []
     for p, rs in tree.items():
         for r in rs:
             if p.key in index.get(r.key, []):
-                p_as_dep_of_r = [x for x in tree.get(tree.get_node_as_parent(r.key)) if x.key == p.key][0]
-                cyclic.append((p, r, p_as_dep_of_r))
+                val = tree.get_node_as_parent(r.key)
+                if val is not None:
+                    entry = tree.get(val)
+                    if entry is not None:
+                        p_as_dep_of_r = [x for x in entry if x.key == p.key][0]
+                        cyclic.append((p, r, p_as_dep_of_r))
     return cyclic
 
 
-def render_cycles_text(cycles):
+def render_cycles_text(cycles: list[tuple[DistPackage, ReqPackage, ReqPackage]]) -> None:
     if cycles:
         print("Warning!! Cyclic dependencies found:", file=sys.stderr)  # noqa: T201
         # List in alphabetical order of the dependency that's cycling
         # (2nd item in the tuple)
         cycles = sorted(cycles, key=lambda xs: xs[1].key)
         for a, b, c in cycles:
             print(f"* {a.project_name} => {b.project_name} => {c.project_name}", file=sys.stderr)  # noqa: T201
 
 
-def get_parser():
-    parser = argparse.ArgumentParser(description="Dependency tree of the installed python packages")
+def get_parser() -> ArgumentParser:
+    parser = ArgumentParser(description="Dependency tree of the installed python packages")
     parser.add_argument("-v", "--version", action="version", version=f"{__version__}")
     parser.add_argument("-f", "--freeze", action="store_true", help="Print names so as to write freeze files")
     parser.add_argument(
         "--python",
         default=sys.executable,
         help="Python to use to look for packages in it (default: where installed)",
     )
@@ -1002,20 +1045,37 @@
         dest="encoding_type",
         default=sys.stdout.encoding,
         help="Display dependency tree as text using specified encoding",
     )
     return parser
 
 
-def _get_args():
+class Options(Namespace):
+    freeze: bool
+    python: str
+    all: bool  # noqa: A003
+    local_only: bool
+    warn: Literal["silence", "suppress", "fail"]
+    reverse: bool
+    packages: str
+    exclude: str
+    json: bool
+    json_tree: bool
+    mermaid: bool
+    graph_output: str | None
+    depth: float
+    encoding: str
+
+
+def _get_args() -> Options:
     parser = get_parser()
-    return parser.parse_args()
+    return cast(Options, parser.parse_args())
 
 
-def handle_non_host_target(args):
+def handle_non_host_target(args: Options) -> int | None:
     # if target is not current python re-invoke it under the actual host
     py_path = Path(args.python).absolute()
     if py_path != Path(sys.executable).absolute():
         # there's no way to guarantee that graphviz is available, so refuse
         if args.output_format:
             print(  # noqa: T201
                 "graphviz functionality is not supported when querying non-host python",
@@ -1027,45 +1087,53 @@
             if value == "--python":
                 del argv[py_at]
                 del argv[py_at]
             elif value.startswith("--python"):
                 del argv[py_at]
 
         main_file = inspect.getsourcefile(sys.modules[__name__])
+        assert main_file is not None  # noqa: S101
         with tempfile.TemporaryDirectory() as project:
             shutil.copytree(Path(main_file).parent, Path(project) / "pipdeptree")
             # invoke from an empty folder to avoid cwd altering sys.path
             env = os.environ.copy()
             env["PYTHONPATH"] = project
-            cmd = [py_path, "-m", "pipdeptree"]
+            cmd: list[Path | str] = [py_path, "-m", "pipdeptree"]
             cmd.extend(argv)
             return subprocess.call(cmd, cwd=project, env=env)  # noqa: S603
     return None
 
 
-def get_installed_distributions(local_only=False, user_only=False):  # noqa: FBT002
+def get_installed_distributions(
+    local_only: bool = False,  # noqa: FBT001, FBT002
+    user_only: bool = False,  # noqa: FBT001, FBT002
+) -> list[DistInfoDistribution]:
     try:
         from pip._internal.metadata import pkg_resources
     except ImportError:
         # For backward compatibility with python ver. 2.7 and pip
         # version 20.3.4 (the latest pip version that works with python
         # version 2.7)
         from pip._internal.utils import misc
 
-        return misc.get_installed_distributions(local_only=local_only, user_only=user_only)
+        return misc.get_installed_distributions(  # type: ignore[no-any-return,attr-defined]
+            local_only=local_only,
+            user_only=user_only,
+        )
+
     else:
         dists = pkg_resources.Environment.from_paths(None).iter_installed_distributions(
             local_only=local_only,
             skip=(),
             user_only=user_only,
         )
-        return [d._dist for d in dists]  # noqa: SLF001
+        return [d._dist for d in dists]  # type: ignore[attr-defined] # noqa: SLF001
 
 
-def main():
+def main() -> None | int:
     args = _get_args()
     result = handle_non_host_target(args)
     if result is not None:
         return result
 
     pkgs = get_installed_distributions(local_only=args.local_only, user_only=args.user_only)
     tree = PackageDAG.from_pkgs(pkgs)
@@ -1085,15 +1153,15 @@
         tree = tree.filter_nodes(show_only, exclude)
 
     _render(args, tree)
 
     return return_code
 
 
-def _check_cycle_conflict(args, is_text_output, tree):
+def _check_cycle_conflict(args: Options, is_text_output: bool, tree: PackageDAG) -> int:  # noqa: FBT001
     # Before any reversing or filtering, show warnings to console
     # about possibly conflicting or cyclic deps if found and warnings
     # are enabled (i.e. only if output is to be printed to console)
     if is_text_output and args.warn != "silence":
         conflicts = conflicting_deps(tree)
         if conflicts:
             render_conflicts_text(conflicts)
@@ -1105,15 +1173,15 @@
             print("-" * 72, file=sys.stderr)  # noqa: T201
 
         if args.warn == "fail" and (conflicts or cycles):
             return 1
     return 0
 
 
-def _render(args, tree):
+def _render(args: Options, tree: PackageDAG) -> None:
     if args.json:
         print(render_json(tree, indent=4))  # noqa: T201
     elif args.json_tree:
         print(render_json_tree(tree, indent=4))  # noqa: T201
     elif args.mermaid:
         print(render_mermaid(tree))  # noqa: T201
     elif args.output_format:
```

### Comparing `pipdeptree-2.9.4/tests/test_pipdeptree.py` & `pipdeptree-2.9.5/tests/test_pipdeptree.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import platform
 import random
 import subprocess
 import sys
 from itertools import chain
 from pathlib import Path
 from textwrap import dedent, indent
-from typing import TYPE_CHECKING, Any
-from unittest import mock
+from typing import TYPE_CHECKING, Any, Iterator
+from unittest.mock import Mock
 
 import pytest
 import virtualenv
 
 from pipdeptree import (
     DistPackage,
     PackageDAG,
@@ -32,72 +32,76 @@
 
 if TYPE_CHECKING:
     from pytest_mock import MockerFixture
 
 # Tests for DAG classes
 
 
-def mock_pkgs(simple_graph):
+def mock_pkgs(simple_graph: dict[tuple[str, str], list[tuple[str, list[tuple[str, str]]]]]) -> Iterator[Mock]:
     for node, children in simple_graph.items():
         nk, nv = node
-        m = mock.Mock(key=nk.lower(), project_name=nk, version=nv)
-        as_req = mock.Mock(key=nk, project_name=nk, specs=[("==", nv)])
-        m.as_requirement = mock.Mock(return_value=as_req)
+        m = Mock(key=nk.lower(), project_name=nk, version=nv)
+        as_req = Mock(key=nk, project_name=nk, specs=[("==", nv)])
+        m.as_requirement = Mock(return_value=as_req)
         reqs = []
         for child in children:
             ck, cv = child
-            r = mock.Mock(key=ck, project_name=ck, specs=cv)
+            r = Mock(key=ck, project_name=ck, specs=cv)
             reqs.append(r)
-        m.requires = mock.Mock(return_value=reqs)
+        m.requires = Mock(return_value=reqs)
         yield m
 
 
-def mock_package_dag(simple_graph):
+def mock_package_dag(simple_graph: dict[tuple[str, str], list[tuple[str, list[tuple[str, str]]]]]) -> PackageDAG:
     pkgs = list(mock_pkgs(simple_graph))
-    return PackageDAG.from_pkgs(pkgs)
+    return PackageDAG.from_pkgs(pkgs)  # type: ignore[arg-type]
 
 
 # util for comparing tree contents with a simple graph
-def dag_to_dict(g):
+def dag_to_dict(g: PackageDAG) -> dict[str, list[str]]:
     return {k.key: [v.key for v in vs] for k, vs in g._obj.items()}  # noqa: SLF001
 
 
-def sort_map_values(m):
+def sort_map_values(m: dict[str, Any]) -> dict[str, Any]:
     return {k: sorted(v) for k, v in m.items()}
 
 
-t = mock_package_dag(
+t: PackageDAG = mock_package_dag(
     {
         ("a", "3.4.0"): [("b", [(">=", "2.0.0")]), ("c", [(">=", "5.7.1")])],
         ("b", "2.3.1"): [("d", [(">=", "2.30"), ("<", "2.42")])],
         ("c", "5.10.0"): [("d", [(">=", "2.30")]), ("e", [(">=", "0.12.1")])],
         ("d", "2.35"): [("e", [(">=", "0.9.0")])],
         ("e", "0.12.1"): [],
         ("f", "3.1"): [("b", [(">=", "2.1.0")])],
         ("g", "6.8.3rc1"): [("e", [(">=", "0.9.0")]), ("f", [(">=", "3.0.0")])],
     },
 )
 
 
-def test_package_dag_get_node_as_parent():
-    assert t.get_node_as_parent("b").key == "b"
-    assert t.get_node_as_parent("c").key == "c"
+def test_package_dag_get_node_as_parent() -> None:
+    node = t.get_node_as_parent("b")
+    assert node is not None
+    assert node.key == "b"
+    node = t.get_node_as_parent("c")
+    assert node is not None
+    assert node.key == "c"
 
 
-def test_package_dag_filter():
+def test_package_dag_filter() -> None:
     # When both show_only and exclude are not specified, same tree
     assert t.filter_nodes(None, None) is t
 
     # when show_only is specified
     g1 = dag_to_dict(t.filter_nodes({"a", "d"}, None))
     expected = {"a": ["b", "c"], "b": ["d"], "c": ["d", "e"], "d": ["e"], "e": []}
     assert expected == g1
 
     # when exclude is specified
-    g2 = dag_to_dict(t.filter_nodes(None, ["d"]))
+    g2 = dag_to_dict(t.filter_nodes(None, {"d"}))
     expected = {"a": ["b", "c"], "b": [], "c": ["e"], "e": [], "f": ["b"], "g": ["e", "f"]}
     assert expected == g2
 
     # when both show_only and exclude are specified
     g3 = dag_to_dict(t.filter_nodes({"a", "g"}, {"d", "e"}))
     expected = {"a": ["b", "c"], "b": [], "c": [], "f": ["b"], "g": ["f"]}
     assert expected == g3
@@ -141,15 +145,15 @@
 
 def test_package_dag_filter_fnmatch_exclude_a(t_fnmatch: Any) -> None:
     # test exclude for a.* in the result we got only b.* nodes
     graph = dag_to_dict(t_fnmatch.filter_nodes(None, {"a.*"}))
     assert graph == {"b.a": ["b.b"], "b.b": []}
 
 
-def test_package_dag_reverse():
+def test_package_dag_reverse() -> None:
     t1 = t.reverse()
     expected = {"a": [], "b": ["a", "f"], "c": ["a"], "d": ["b", "c"], "e": ["c", "d", "g"], "f": ["g"], "g": []}
     assert isinstance(t1, ReversedPackageDAG)
     assert sort_map_values(expected) == sort_map_values(dag_to_dict(t1))
     assert all(isinstance(k, ReqPackage) for k in t1)
     assert all(isinstance(v, DistPackage) for v in chain.from_iterable(t1.values()))
 
@@ -158,94 +162,94 @@
     t2 = t1.reverse()
     assert isinstance(t2, PackageDAG)
     assert sort_map_values(expected) == sort_map_values(dag_to_dict(t2))
     assert all(isinstance(k, DistPackage) for k in t2)
     assert all(isinstance(v, ReqPackage) for v in chain.from_iterable(t2.values()))
 
 
-def test_package_dag_from_pkgs():
+def test_package_dag_from_pkgs() -> None:
     # when pip's _vendor.packaging.requirements.Requirement's requires() gives a lowercased package name but the actual
     # package name in PyPI is mixed case, expect the mixed case version
-    graph = {
+    graph: dict[tuple[str, str], list[tuple[str, list[tuple[str, str]]]]] = {
         ("examplePy", "1.2.3"): [("hellopy", [(">=", "2.0.0")])],
         ("HelloPy", "2.2.0"): [],
     }
-    t = mock_package_dag(graph)
+    package_dag = mock_package_dag(graph)
     parent_key = "examplepy"
-    c = t.get_children(parent_key)
+    c = package_dag.get_children(parent_key)
     assert len(c) == 1
     assert c[0].project_name == "HelloPy"
 
 
 # Tests for Package classes
 #
 # Note: For all render methods, we are only testing for frozen=False
 # as mocks with frozen=True are a lot more complicated
 
 
-def test_dist_package_render_as_root():
-    foo = mock.Mock(key="foo", project_name="foo", version="20.4.1")
+def test_dist_package_render_as_root() -> None:
+    foo = Mock(key="foo", project_name="foo", version="20.4.1")
     dp = DistPackage(foo)
     is_frozen = False
     assert dp.render_as_root(is_frozen) == "foo==20.4.1"
 
 
-def test_dist_package_render_as_branch():
-    foo = mock.Mock(key="foo", project_name="foo", version="20.4.1")
-    bar = mock.Mock(key="bar", project_name="bar", version="4.1.0")
-    bar_req = mock.Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
+def test_dist_package_render_as_branch() -> None:
+    foo = Mock(key="foo", project_name="foo", version="20.4.1")
+    bar = Mock(key="bar", project_name="bar", version="4.1.0")
+    bar_req = Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
     rp = ReqPackage(bar_req, dist=bar)
     dp = DistPackage(foo).as_parent_of(rp)
     is_frozen = False
     assert dp.render_as_branch(is_frozen) == "foo==20.4.1 [requires: bar>=4.0]"
 
 
-def test_dist_package_as_parent_of():
-    foo = mock.Mock(key="foo", project_name="foo", version="20.4.1")
+def test_dist_package_as_parent_of() -> None:
+    foo = Mock(key="foo", project_name="foo", version="20.4.1")
     dp = DistPackage(foo)
     assert dp.req is None
 
-    bar = mock.Mock(key="bar", project_name="bar", version="4.1.0")
-    bar_req = mock.Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
+    bar = Mock(key="bar", project_name="bar", version="4.1.0")
+    bar_req = Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
     rp = ReqPackage(bar_req, dist=bar)
     dp1 = dp.as_parent_of(rp)
     assert dp1._obj == dp._obj  # noqa: SLF001
     assert dp1.req is rp
 
     dp2 = dp.as_parent_of(None)
     assert dp2 is dp
 
 
-def test_dist_package_as_dict():
-    foo = mock.Mock(key="foo", project_name="foo", version="1.3.2b1")
+def test_dist_package_as_dict() -> None:
+    foo = Mock(key="foo", project_name="foo", version="1.3.2b1")
     dp = DistPackage(foo)
     result = dp.as_dict()
     expected = {"key": "foo", "package_name": "foo", "installed_version": "1.3.2b1"}
     assert expected == result
 
 
-def test_req_package_render_as_root():
-    bar = mock.Mock(key="bar", project_name="bar", version="4.1.0")
-    bar_req = mock.Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
+def test_req_package_render_as_root() -> None:
+    bar = Mock(key="bar", project_name="bar", version="4.1.0")
+    bar_req = Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
     rp = ReqPackage(bar_req, dist=bar)
     is_frozen = False
     assert rp.render_as_root(is_frozen) == "bar==4.1.0"
 
 
-def test_req_package_render_as_branch():
-    bar = mock.Mock(key="bar", project_name="bar", version="4.1.0")
-    bar_req = mock.Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
+def test_req_package_render_as_branch() -> None:
+    bar = Mock(key="bar", project_name="bar", version="4.1.0")
+    bar_req = Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
     rp = ReqPackage(bar_req, dist=bar)
     is_frozen = False
     assert rp.render_as_branch(is_frozen) == "bar [required: >=4.0, installed: 4.1.0]"
 
 
-def test_req_package_as_dict():
-    bar = mock.Mock(key="bar", project_name="bar", version="4.1.0")
-    bar_req = mock.Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
+def test_req_package_as_dict() -> None:
+    bar = Mock(key="bar", project_name="bar", version="4.1.0")
+    bar_req = Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
     rp = ReqPackage(bar_req, dist=bar)
     result = rp.as_dict()
     expected = {"key": "bar", "package_name": "bar", "installed_version": "4.1.0", "required_version": ">=4.0"}
     assert expected == result
 
 
 # Tests for render_text
@@ -253,22 +257,19 @@
 
 class MockStdout:
     """
     A wrapper to stdout that mocks the `encoding` attribute (to have `render_text()` render with unicode/non-unicode)
     and `write()` (so that `print()` calls can write to stdout).
     """
 
-    def __init__(self, encoding) -> None:
+    def __init__(self, encoding: str) -> None:
         self.stdout = sys.stdout
         self.encoding = encoding
 
-    def encoding(self):
-        return self.encoding
-
-    def write(self, text):
+    def write(self, text: str) -> None:
         self.stdout.write(text)
 
 
 @pytest.mark.parametrize(
     ("list_all", "reverse", "unicode", "expected_output"),
     [
         (
@@ -487,15 +488,21 @@
                 "    - c==5.10.0 [requires: d>=2.30]",
                 "      - a==3.4.0 [requires: c>=5.7.1]",
                 "  - g==6.8.3rc1 [requires: e>=0.9.0]",
             ],
         ),
     ],
 )
-def test_render_text(capsys, list_all, reverse, unicode, expected_output):
+def test_render_text(
+    capsys: pytest.CaptureFixture[str],
+    list_all: bool,
+    reverse: bool,
+    unicode: bool,
+    expected_output: list[str],
+) -> None:
     tree = t.reverse() if reverse else t
     encoding = "utf-8" if unicode else "ascii"
     render_text(tree, float("inf"), encoding, list_all=list_all, frozen=False)
     captured = capsys.readouterr()
     assert "\n".join(expected_output).strip() == captured.out.strip()
 
 
@@ -584,15 +591,20 @@
                 "  - e [required: >=0.9.0, installed: 0.12.1]",
                 "  - f [required: >=3.0.0, installed: 3.1]",
                 "    - b [required: >=2.1.0, installed: 2.3.1]",
             ],
         ),
     ],
 )
-def test_render_text_given_depth(capsys, unicode, level, expected_output):
+def test_render_text_given_depth(
+    capsys: pytest.CaptureFixture[str],
+    unicode: str,
+    level: int,
+    expected_output: list[str],
+) -> None:
     render_text(t, level, encoding="utf-8" if unicode else "ascii")
     captured = capsys.readouterr()
     assert "\n".join(expected_output).strip() == captured.out.strip()
 
 
 @pytest.mark.parametrize(
     ("level", "encoding", "expected_output"),
@@ -737,42 +749,47 @@
                 "  - e [required: >=0.9.0, installed: 0.12.1]",
                 "  - f [required: >=3.0.0, installed: 3.1]",
                 "    - b [required: >=2.1.0, installed: 2.3.1]",
             ],
         ),
     ],
 )
-def test_render_text_encoding(capsys, level, encoding, expected_output):
+def test_render_text_encoding(
+    capsys: pytest.CaptureFixture[str],
+    level: int,
+    encoding: str,
+    expected_output: list[str],
+) -> None:
     render_text(t, level, encoding, True, False)
     captured = capsys.readouterr()
     assert "\n".join(expected_output).strip() == captured.out.strip()
 
 
 # Tests for graph outputs
 
 
-def randomized_dag_copy(t):
+def randomized_dag_copy(raw: PackageDAG) -> PackageDAG:
     """Returns a copy of the package tree fixture with dependencies in randomized order."""
     # Extract the dependency graph from the package tree and randomize it.
     randomized_graph = {}
-    randomized_nodes = list(t._obj.keys())  # noqa: SLF001
+    randomized_nodes = list(raw._obj.keys())  # noqa: SLF001
     random.shuffle(randomized_nodes)
     for node in randomized_nodes:
-        edges = t._obj[node]  # noqa: SLF001
+        edges = raw._obj[node]  # noqa: SLF001
         random.shuffle(edges)
         randomized_graph[node] = edges
-    assert set(randomized_graph) == set(t._obj)  # noqa: SLF001
+    assert set(randomized_graph) == set(raw._obj)  # noqa: SLF001
 
     # Create a randomized package tree.
     randomized_dag = PackageDAG(randomized_graph)
-    assert len(t) == len(randomized_dag)
+    assert len(raw) == len(randomized_dag)
     return randomized_dag
 
 
-def test_render_mermaid():
+def test_render_mermaid() -> None:
     """Check both the sorted and randomized package tree produces the same sorted Mermaid output.
 
     Rendering a reverse dependency tree should produce the same set of nodes. Edges should have
     the same version spec label, but be resorted after swapping node positions.
 
     `See how this renders
     <https://mermaid.ink/img/pako:eNp9kcluwjAURX_FeutgeUhCErWs-IN21boL4yFEzYAyqKWIf-9LCISyqFf2ufe-QT6BaayDDHzZfJm9bnvyulU1wWNK3XVb50lVdF1R56Tr2-bTrazu0NfqY0aii1O_K9BK1ZKGlCn4uNAd0h1SQSXlN2qQGqQR5ezObBHbizm6QYfQIWSUi7sSHrGf2i0sR5Yji2lCZWsWQZPViijYPAs69cPnhuwetIiux1qTZubpl5xkwZOgoZgNdl7karhON4nuQRzTf3N2yaW3geaYX2L8cdj8n9xNk3dLegigcm2lC4v_exqdCvq9q5yCDK_WeT2UvQJVn9Gqh755OdYGsr4dXADDwerebQudt7qCzOuyQ3rQ9VvTVFcTPiE7wTdkgkVUSiHjlLOERUkYB3AcMeXrhKUp53GYcJ6KcwA_UwVGo_MvVqym_A?type=png)](https://mermaid.live/edit#pako:eNp9kcluwjAURX_FeutgeUhCErWs-IN21boL4yFEzYAyqKWIf-9LCISyqFf2ufe-QT6BaayDDHzZfJm9bnvyulU1wWNK3XVb50lVdF1R56Tr2-bTrazu0NfqY0aii1O_K9BK1ZKGlCn4uNAd0h1SQSXlN2qQGqQR5ezObBHbizm6QYfQIWSUi7sSHrGf2i0sR5Yji2lCZWsWQZPViijYPAs69cPnhuwetIiux1qTZubpl5xkwZOgoZgNdl7karhON4nuQRzTf3N2yaW3geaYX2L8cdj8n9xNk3dLegigcm2lC4v_exqdCvq9q5yCDK_WeT2UvQJVn9Gqh755OdYGsr4dXADDwerebQudt7qCzOuyQ3rQ9VvTVFcTPiE7wTdkgkVUSiHjlLOERUkYB3AcMeXrhKUp53GYcJ6KcwA_UwVGo_MvVqym_A>`_.
@@ -827,15 +844,15 @@
     for package_tree in (t, randomized_dag_copy(t)):
         output = render_mermaid(package_tree)
         assert output.rstrip() == nodes + dependency_edges
         reversed_output = render_mermaid(package_tree.reverse())
         assert reversed_output.rstrip() == nodes + reverse_dependency_edges
 
 
-def test_mermaid_reserved_ids():
+def test_mermaid_reserved_ids() -> None:
     package_tree = mock_package_dag(
         {
             ("click", "3.4.0"): [("click-extra", [(">=", "2.0.0")])],
         },
     )
     output = render_mermaid(package_tree)
     assert output == dedent(
@@ -845,15 +862,15 @@
             click-extra["click-extra\\n(missing)"]:::missing
             click_0["click\\n3.4.0"]
             click_0 -.-> click-extra
         """,
     )
 
 
-def test_render_dot(capsys):
+def test_render_dot(capsys: pytest.CaptureFixture[str]) -> None:
     # Check both the sorted and randomized package tree produces the same sorted
     # graphviz output.
     for package_tree in (t, randomized_dag_copy(t)):
         output = dump_graphviz(package_tree, output_format="dot")
         print_graphviz(output)
         out, _ = capsys.readouterr()
         assert out == dedent(
@@ -887,15 +904,15 @@
     with pytest.raises(OSError, match="Bad file"):  # noqa: PT012, SIM117 # because we reopen the file
         with res.open("wb") as buf:
             mocker.patch.object(sys, "stdout", buf)
             print_graphviz(output)
     assert res.read_bytes()[:4] == b"%PDF"
 
 
-def test_render_svg(capsys):
+def test_render_svg(capsys: pytest.CaptureFixture[str]) -> None:
     output = dump_graphviz(t, output_format="svg")
     print_graphviz(output)
     out, _ = capsys.readouterr()
     assert out.startswith("<?xml")
     assert "<svg" in out
     assert out.strip().endswith("</svg>")
 
@@ -938,15 +955,20 @@
         (
             {("a", "1.0.1"): [("c", [(">=", "9.4.1")])], ("b", "2.3.0"): [("c", [(">=", "7.0")])], ("c", "9.4.1"): []},
             {},
             [],
         ),
     ],
 )
-def test_conflicting_deps(capsys, mpkgs, expected_keys, expected_output):
+def test_conflicting_deps(
+    capsys: pytest.CaptureFixture[str],
+    mpkgs: dict[tuple[str, str], list[tuple[str, list[tuple[str, str]]]]],
+    expected_keys: dict[str, list[str]],
+    expected_output: list[str],
+) -> None:
     tree = mock_package_dag(mpkgs)
     result = conflicting_deps(tree)
     result_keys = {k.key: [v.key for v in vs] for k, vs in result.items()}
     assert expected_keys == result_keys
     render_conflicts_text(result)
     captured = capsys.readouterr()
     assert "\n".join(expected_output).strip() == captured.err.strip()
@@ -973,72 +995,77 @@
                 ("a", "1.0.1"): [("b", [(">=", "2.0.0")])],
             },
             [],
             [],  # no output expected
         ),
     ],
 )
-def test_cyclic_deps(capsys, mpkgs, expected_keys, expected_output):
+def test_cyclic_deps(
+    capsys: pytest.CaptureFixture[str],
+    mpkgs: dict[tuple[str, str], list[tuple[str, list[tuple[str, str]]]]],
+    expected_keys: list[tuple[str, ...]],
+    expected_output: list[str],
+) -> None:
     tree = mock_package_dag(mpkgs)
     result = cyclic_deps(tree)
     result_keys = [(a.key, b.key, c.key) for (a, b, c) in result]
     assert sorted(expected_keys) == sorted(result_keys)
     render_cycles_text(result)
     captured = capsys.readouterr()
     assert "\n".join(expected_output).strip() == captured.err.strip()
 
 
 # Tests for the argparse parser
 
 
-def test_parser_default():
+def test_parser_default() -> None:
     parser = get_parser()
     args = parser.parse_args([])
     assert not args.json
     assert args.output_format is None
 
 
-def test_parser_j():
+def test_parser_j() -> None:
     parser = get_parser()
     args = parser.parse_args(["-j"])
     assert args.json
     assert args.output_format is None
 
 
-def test_parser_json():
+def test_parser_json() -> None:
     parser = get_parser()
     args = parser.parse_args(["--json"])
     assert args.json
     assert args.output_format is None
 
 
-def test_parser_json_tree():
+def test_parser_json_tree() -> None:
     parser = get_parser()
     args = parser.parse_args(["--json-tree"])
     assert args.json_tree
     assert not args.json
     assert args.output_format is None
 
 
-def test_parser_mermaid():
+def test_parser_mermaid() -> None:
     parser = get_parser()
     args = parser.parse_args(["--mermaid"])
     assert args.mermaid
     assert not args.json
     assert args.output_format is None
 
 
-def test_parser_pdf():
+def test_parser_pdf() -> None:
     parser = get_parser()
     args = parser.parse_args(["--graph-output", "pdf"])
     assert args.output_format == "pdf"
     assert not args.json
 
 
-def test_parser_svg():
+def test_parser_svg() -> None:
     parser = get_parser()
     args = parser.parse_args(["--graph-output", "svg"])
     assert args.output_format == "svg"
     assert not args.json
 
 
 @pytest.mark.parametrize(
@@ -1047,27 +1074,32 @@
         (True, ["-d", "-1"], None),
         (True, ["--depth", "string"], None),
         (False, ["-d", "0"], 0),
         (False, ["--depth", "8"], 8),
         (False, [], float("inf")),
     ],
 )
-def test_parser_depth(should_be_error, depth_arg, expected_value):
+def test_parser_depth(should_be_error: bool, depth_arg: list[str], expected_value: None | int | float) -> None:
     parser = get_parser()
 
     if should_be_error:
         with pytest.raises(SystemExit):
             parser.parse_args(depth_arg)
     else:
         args = parser.parse_args(depth_arg)
         assert args.depth == expected_value
 
 
 @pytest.mark.parametrize("args_joined", [True, False])
-def test_custom_interpreter(tmp_path, monkeypatch, capfd, args_joined):
+def test_custom_interpreter(
+    tmp_path: Path,
+    monkeypatch: pytest.MonkeyPatch,
+    capfd: pytest.CaptureFixture[str],
+    args_joined: bool,
+) -> None:
     result = virtualenv.cli_run([str(tmp_path / "venv"), "--activators", ""])
     cmd = [sys.executable]
     monkeypatch.chdir(tmp_path)
     py = str(result.creator.exe.relative_to(tmp_path))
     cmd += [f"--python={result.creator.exe}"] if args_joined else ["--python", py]
     monkeypatch.setattr(sys, "argv", cmd)
     main()
@@ -1089,11 +1121,11 @@
         main()
     out, err = capfd.readouterr()
     assert context.value.code == 1
     assert not out
     assert err == "graphviz functionality is not supported when querying non-host python\n"
 
 
-def test_guess_version_setuptools():
+def test_guess_version_setuptools() -> None:
     script = Path(__file__).parent / "guess_version_setuptools.py"
     output = subprocess.check_output([sys.executable, script], text=True)
     assert output == "?"
```

### Comparing `pipdeptree-2.9.4/LICENSE` & `pipdeptree-2.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.4/README.md` & `pipdeptree-2.9.5/README.md`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.4/pyproject.toml` & `pipdeptree-2.9.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -70,18 +70,20 @@
 select = ["ALL"]
 line-length = 120
 target-version = "py37"
 isort = {known-first-party = ["pipdeptree"], required-imports = ["from __future__ import annotations"]}
 ignore = [
   "INP001", # no implicit namespace
   "D",  # ignore documentation for now
-  "ANN",  # No type annotations for now
   "D203",  # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
   "D212",  # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
   "S104",  # Possible binding to all interface
+  "ANN101",  # No type annotation for self
+  "ANN102",  # Missing type annotation for `cls` in classmethod
+  "ANN401",  # Dynamically typed expressions (typing.Any) are disallowed in
 ]
 [tool.ruff.per-file-ignores]
 "tests/**/*.py" = [
   "S101",  # asserts allowed in tests...
   "FBT",  # don"t care about booleans as positional arguments in tests
   "D",  # don"t care about documentation in tests
   "S603",  # `subprocess` call: check for execution of untrusted input
@@ -90,7 +92,17 @@
 
 [tool.coverage]
 html.show_contexts = true
 html.skip_covered = false
 paths.source = ["src", ".tox/*/lib/python*/site-packages", "*/src"]
 run.parallel = true
 run.plugins = ["covdefaults"]
+
+[tool.mypy]
+show_error_codes = true
+strict = true
+overrides = [
+  { module = [
+    "graphviz.*",
+    "virtualenv.*",
+  ], ignore_missing_imports = true },
+]
```

### Comparing `pipdeptree-2.9.4/PKG-INFO` & `pipdeptree-2.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipdeptree
-Version: 2.9.4
+Version: 2.9.5
 Summary: Command line utility to show dependency tree of packages.
 Project-URL: Changelog, https://github.com/tox-dev/pipdeptree/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/tox-dev/pipdeptree/blob/main/README.md#pipdeptree
 Project-URL: Homepage, https://github.com/tox-dev/pipdeptree
 Project-URL: Source, https://github.com/tox-dev/pipdeptree
 Project-URL: Tracker, https://github.com/tox-dev/pipdeptree/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Vineet Naik <naikvin@gmail.com>
```

