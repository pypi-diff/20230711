# Comparing `tmp/creosote-2.6.2-py3-none-any.whl.zip` & `tmp/creosote-2.6.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 14224 bytes, number of entries: 12
+Zip file size: 14382 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 creosote/__about__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 creosote/__init__.py
 -rw-r--r--  2.0 unx     6597 b- defN 20-Feb-02 00:00 creosote/cli.py
 -rw-r--r--  2.0 unx     1109 b- defN 20-Feb-02 00:00 creosote/formatters.py
 -rw-r--r--  2.0 unx      523 b- defN 20-Feb-02 00:00 creosote/models.py
--rw-r--r--  2.0 unx     8488 b- defN 20-Feb-02 00:00 creosote/parsers.py
+-rw-r--r--  2.0 unx     9279 b- defN 20-Feb-02 00:00 creosote/parsers.py
 -rw-r--r--  2.0 unx     9413 b- defN 20-Feb-02 00:00 creosote/resolvers.py
-?rw-r--r--  2.0 unx    13421 b- defN 20-Feb-02 00:00 creosote-2.6.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 creosote-2.6.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 creosote-2.6.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 creosote-2.6.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      933 b- defN 20-Feb-02 00:00 creosote-2.6.2.dist-info/RECORD
-12 files, 41712 bytes uncompressed, 12666 bytes compressed:  69.6%
+?rw-r--r--  2.0 unx    13421 b- defN 20-Feb-02 00:00 creosote-2.6.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 creosote-2.6.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 creosote-2.6.3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 creosote-2.6.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      933 b- defN 20-Feb-02 00:00 creosote-2.6.3.dist-info/RECORD
+12 files, 42503 bytes uncompressed, 12824 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: creosote/parsers.py
 Comment: 
 
 Filename: creosote/resolvers.py
 Comment: 
 
-Filename: creosote-2.6.2.dist-info/METADATA
+Filename: creosote-2.6.3.dist-info/METADATA
 Comment: 
 
-Filename: creosote-2.6.2.dist-info/WHEEL
+Filename: creosote-2.6.3.dist-info/WHEEL
 Comment: 
 
-Filename: creosote-2.6.2.dist-info/entry_points.txt
+Filename: creosote-2.6.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: creosote-2.6.2.dist-info/licenses/LICENSE
+Filename: creosote-2.6.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: creosote-2.6.2.dist-info/RECORD
+Filename: creosote-2.6.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## creosote/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "2.6.2"
+__version__ = "2.6.3"
```

## creosote/parsers.py

```diff
@@ -32,53 +32,75 @@
         if not Path(self.deps_file).exists():
             raise Exception(f"File {self.deps_file} does not exist")
 
         dep_names = []
         always_excluded_deps = ["python"]  # occurs in Poetry setup
         deps_to_exclude = always_excluded_deps + self.exclude_deps
 
-        if self.deps_file.endswith(".toml"):  # pyproject.toml expected
-            for dep_name in self.load_pyproject(self.deps_file, self.sections):
+        if self.deps_file.endswith(".toml") or self.deps_file.endswith(
+            "Pipfile"
+        ):  # pyproject.toml or Pipfile expected
+            for dep_name in self.read_toml(self.deps_file, self.sections):
                 if dep_name not in deps_to_exclude:
                     dep_names.append(dep_name)
         elif self.deps_file.endswith(".txt") or self.deps_file.endswith(".in"):
-            for dep_name in self.load_requirements(self.deps_file):
+            for dep_name in self.read_requirements(self.deps_file):
                 if dep_name not in deps_to_exclude:
                     dep_names.append(dep_name)
         else:
             raise NotImplementedError(
                 f"Dependency specs file {self.deps_file} is not supported."
             )
 
         logger.info(
             f"Found dependencies in {self.deps_file}: " f"{', '.join(dep_names)}"
         )
 
         return dep_names
 
-    def load_pyproject_pep621(self, section_contents: List[str]) -> List[str]:
-        if not isinstance(section_contents, list):
+    def get_deps_from_pep621_toml(
+        self, section_contents: Union[List[str], Dict[str, List[str]]]
+    ) -> List[str]:
+        """Get dependency names from toml file using the PEP621 spec.
+
+        The dependency strings are expected to follow PEP508.
+        """
+
+        dep_strings = []
+        if isinstance(section_contents, list):
+            for dep_string in section_contents:
+                dep_strings.append(dep_string)
+        elif isinstance(section_contents, dict):
+            for _, dep_string_list in section_contents.items():
+                for dep_string in dep_string_list:
+                    dep_strings.append(dep_string)
+        else:
             raise TypeError("Unexpected dependency format, list expected.")
 
         section_deps = []
-        for dep_name in section_contents:
-            parsed_dep = self.parse_dep_string(dep_name)
+        for dep_string in dep_strings:
+            parsed_dep = self.parse_dep_string(dep_string)
             if parsed_dep:
                 section_deps.append(parsed_dep)
             else:
-                logger.warning(f"Could not parse dependency string: {dep_name}")
+                logger.warning(f"Could not parse dependency string: {dep_string}")
+
         return section_deps
 
-    def load_pyproject_poetry(self, section_contents: Dict[str, Any]):
+    def get_deps_from_toml_section_keys(
+        self,
+        section_contents: Dict[str, Any],
+    ):
+        """Get dependency names from toml section's dict keys."""
         if not isinstance(section_contents, dict):
             raise TypeError("Unexpected dependency format, dict expected.")
         return section_contents.keys()
 
-    def load_pyproject(self, deps_file: str, sections: List[str]):
-        """Read dependency names from pyproject.toml."""
+    def read_toml(self, deps_file: str, sections: List[str]) -> List[str]:
+        """Read dependency names from toml spec file."""
         with open(deps_file, "r", encoding="utf-8") as infile:
             contents = toml.loads(infile.read())
 
         dotty_contents: Dotty = dotty(contents)
         dep_names = []
 
         for section in sections:
@@ -88,37 +110,39 @@
                 raise KeyError(f"Could not find toml section {section}.") from err
 
             logger.debug(f"{sections}: {section_contents}")
 
             section_dep_names = []
             if section.startswith("project"):
                 logger.debug(f"Detected PEP-621 toml section in {deps_file}")
-                section_dep_names = self.load_pyproject_pep621(section_contents)
-            elif section.startswith("packages") or section.startswith("dev-packages"):
-                logger.debug(f"Detected pipenv/Pipfile toml section in {deps_file}")
-                section_dep_names = self.load_pyproject_pep621(section_contents)
+                section_dep_names = self.get_deps_from_pep621_toml(section_contents)
             elif section.startswith("tool.pdm"):
                 logger.debug(f"Detected PDM toml section in {deps_file}")
-                section_dep_names = self.load_pyproject_pep621(section_contents)
+                section_dep_names = self.get_deps_from_pep621_toml(section_contents)
             elif section.startswith("tool.poetry"):
                 logger.debug(f"Detected Poetry toml section in {deps_file}")
-                section_dep_names = self.load_pyproject_poetry(
+                section_dep_names = self.get_deps_from_toml_section_keys(
+                    cast(dict, section_contents)
+                )
+            elif section.startswith("packages") or section.startswith("dev-packages"):
+                logger.debug(f"Detected pipenv/Pipfile toml section in {deps_file}")
+                section_dep_names = self.get_deps_from_toml_section_keys(
                     cast(dict, section_contents)
                 )
             else:
                 raise TypeError("Unsupported dependency format.")
 
             if not section_dep_names:
                 logger.warning(f"No dependencies found in section {section}")
             else:
                 dep_names.extend(section_dep_names)
 
         return sorted(dep_names)
 
-    def load_requirements(self, deps_file: str) -> List[str]:
+    def read_requirements(self, deps_file: str) -> List[str]:
         """Read dependency names from requirements.txt-format file."""
         dep_from_req = RequirementsFile.from_file(deps_file).requirements
         return sorted([dep.name for dep in dep_from_req if dep.name is not None])
 
     @staticmethod
     def parse_dep_string(dep: str) -> Union[str, None]:
         if "@" in dep:
```

## Comparing `creosote-2.6.2.dist-info/METADATA` & `creosote-2.6.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creosote
-Version: 2.6.2
+Version: 2.6.3
 Summary: Identify unused dependencies and avoid a bloated virtual environment.
 Project-URL: Source, https://github.com/fredrikaverpil/creosote
 Project-URL: Tracker, https://github.com/fredrikaverpil/creosote/issues
 Author-email: Fredrik Averpil <fredrik.averpil@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `creosote-2.6.2.dist-info/licenses/LICENSE` & `creosote-2.6.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `creosote-2.6.2.dist-info/RECORD` & `creosote-2.6.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-creosote/__about__.py,sha256=53Sii4w6BIWn-1RhaTyqUO46gDe4nDCRQDAcpsWFH24,22
+creosote/__about__.py,sha256=uJ6TLK18jhCrL0aclBja7NzlAGLAyZjVpX-gq3d461k,22
 creosote/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 creosote/cli.py,sha256=lT8Zi0N2eMTExCnGUcLXBskTU2A9DuQVHIjECtPIpI8,6597
 creosote/formatters.py,sha256=KaQhieJcUynXI7p24sbO4c08CaBzl_PfV_OyPF9tgOk,1109
 creosote/models.py,sha256=zwLjGtrHDjyRBHi3HLylmxrlUssEYuzoFNsx4trkexQ,523
-creosote/parsers.py,sha256=vGy-A7y_kTT5Xglqy_aVoL6md-bp2JdjoGe29kkmrtk,8488
+creosote/parsers.py,sha256=zu6vEA2X93P5-tmKj0rzTWWtSU5HYfO-vwAaxzPKfB8,9279
 creosote/resolvers.py,sha256=E0QPdFJOcwgVDyKjMzrhUJkzHWCdnmlBACLAnVGgRjw,9413
-creosote-2.6.2.dist-info/METADATA,sha256=LGd06BcDlEEFAO4n8ozN99F5BDFjHNok9dyattXWQ_E,13421
-creosote-2.6.2.dist-info/WHEEL,sha256=KGYbc1zXlYddvwxnNty23BeaKzh7YuoSIvIMO4jEhvw,87
-creosote-2.6.2.dist-info/entry_points.txt,sha256=1WdMKnsMdlsTqCkVmpuvYDayaGWihV0Yf5qJJOa1u1o,47
-creosote-2.6.2.dist-info/licenses/LICENSE,sha256=_hQiru1DnmKFV7ndyrHSYBPcq9g5dMUxzxRqfvyxyvQ,1072
-creosote-2.6.2.dist-info/RECORD,,
+creosote-2.6.3.dist-info/METADATA,sha256=5oKCC0a0N44O2h5rTgezBBl4r3AZClEpZH-Hzpr53-0,13421
+creosote-2.6.3.dist-info/WHEEL,sha256=KGYbc1zXlYddvwxnNty23BeaKzh7YuoSIvIMO4jEhvw,87
+creosote-2.6.3.dist-info/entry_points.txt,sha256=1WdMKnsMdlsTqCkVmpuvYDayaGWihV0Yf5qJJOa1u1o,47
+creosote-2.6.3.dist-info/licenses/LICENSE,sha256=_hQiru1DnmKFV7ndyrHSYBPcq9g5dMUxzxRqfvyxyvQ,1072
+creosote-2.6.3.dist-info/RECORD,,
```

