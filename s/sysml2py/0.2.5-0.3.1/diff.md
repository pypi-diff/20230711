# Comparing `tmp/sysml2py-0.2.5.tar.gz` & `tmp/sysml2py-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysml2py-0.2.5.tar", last modified: Wed Jun 21 03:43:18 2023, max compression
+gzip compressed data, was "sysml2py-0.3.1.tar", last modified: Tue Jul 11 03:41:28 2023, max compression
```

## Comparing `sysml2py-0.2.5.tar` & `sysml2py-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:18.480980 sysml2py-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 03:43:09.000000 sysml2py-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-21 03:43:18.480980 sysml2py-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-21 03:43:09.000000 sysml2py-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-21 03:43:09.000000 sysml2py-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 03:43:18.480980 sysml2py-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:18.476979 sysml2py-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:18.476979 sysml2py-0.2.5/src/sysml2py/
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-21 03:43:09.000000 sysml2py-0.2.5/src/sysml2py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-21 03:43:09.000000 sysml2py-0.2.5/src/sysml2py/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:18.480980 sysml2py-0.2.5/src/sysml2py/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)    22296 2023-06-21 03:43:09.000000 sysml2py-0.2.5/src/sysml2py/grammar/KerML.tx
--rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-06-21 03:43:09.000000 sysml2py-0.2.5/src/sysml2py/grammar/KerMLExpressions.tx
--rw-r--r--   0 runner    (1001) docker     (123)    48820 2023-06-21 03:43:09.000000 sysml2py-0.2.5/src/sysml2py/grammar/SysML.tx
--rw-r--r--   0 runner    (1001) docker     (123)    80969 2023-06-21 03:43:09.000000 sysml2py-0.2.5/src/sysml2py/grammar/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:18.480980 sysml2py-0.2.5/src/sysml2py/textx/
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-21 03:43:09.000000 sysml2py-0.2.5/src/sysml2py/textx/xtext_to_textx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-21 03:43:09.000000 sysml2py-0.2.5/src/sysml2py/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:43:18.480980 sysml2py-0.2.5/sysml2py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-21 03:43:18.000000 sysml2py-0.2.5/sysml2py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 03:43:18.000000 sysml2py-0.2.5/sysml2py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 03:43:18.000000 sysml2py-0.2.5/sysml2py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 03:43:18.000000 sysml2py-0.2.5/sysml2py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:41:28.403995 sysml2py-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-07-11 03:41:18.000000 sysml2py-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3872 2023-07-11 03:41:28.403995 sysml2py-0.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3371 2023-07-11 03:41:18.000000 sysml2py-0.3.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-07-11 03:41:19.000000 sysml2py-0.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 03:41:28.403995 sysml2py-0.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:41:28.399995 sysml2py-0.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:41:28.399995 sysml2py-0.3.1/src/sysml2py/
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/formatting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:41:28.403995 sysml2py-0.3.1/src/sysml2py/grammar/
+-rw-r--r--   0 root         (0) root         (0)    22296 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/grammar/KerML.tx
+-rw-r--r--   0 root         (0) root         (0)    10762 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/grammar/KerMLExpressions.tx
+-rw-r--r--   0 root         (0) root         (0)    48820 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/grammar/SysML.tx
+-rw-r--r--   0 root         (0) root         (0)   100319 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/grammar/classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:41:28.403995 sysml2py-0.3.1/src/sysml2py/textx/
+-rw-r--r--   0 root         (0) root         (0)     6279 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/textx/xtext_to_textx.py
+-rw-r--r--   0 root         (0) root         (0)    20633 2023-07-11 03:41:18.000000 sysml2py-0.3.1/src/sysml2py/usage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:41:28.403995 sysml2py-0.3.1/sysml2py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3872 2023-07-11 03:41:28.000000 sysml2py-0.3.1/sysml2py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      404 2023-07-11 03:41:28.000000 sysml2py-0.3.1/sysml2py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 03:41:28.000000 sysml2py-0.3.1/sysml2py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-11 03:41:28.000000 sysml2py-0.3.1/sysml2py.egg-info/top_level.txt
```

### Comparing `sysml2py-0.2.5/LICENSE` & `sysml2py-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sysml2py-0.2.5/pyproject.toml` & `sysml2py-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sysml2py"
-version = "0.2.5"
+version = "0.3.1"
 authors = [
   { name="Christopher Cox", email="chris.cox@westfall.io" },
 ]
 description = "SysML v2.0 Parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -29,14 +29,13 @@
 [tool.semantic_release]
 branch = "main"
 version_variable = "pyproject.toml:version"
 version_source = "tag"
 commit_version_number = true # required for version_source = "tag"
 tag_commit = true
 commit_parser = "semantic_release.history.emoji_parser"
-build_command = false
-upload_to_repository = false
-upload_to_release = false
+patch_without_tag = true
+build_command = "pip install build && python -m build"
 
 [project.urls]
 "Homepage" = "https://github.com/Westfall-io/sysml2py"
 "Bug Tracker" = "https://github.com/Westfall-io/sysml2py/issues"
```

### Comparing `sysml2py-0.2.5/src/sysml2py/__init__.py` & `sysml2py-0.3.1/src/sysml2py/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Mon May 29 23:26:16 2023
 
 @author: christophercox
 """
-import io
-
-from textx import metamodel_from_file
-
-import importlib.resources as pkg_resources
-
-import sysml2py
-from sysml2py.formatting import reformat
 
 __all__ = ["load", "loads"]
 __author__ = "Christopher Cox"
 
+from sysml2py.usage import Item, Attribute, Part
+
 
 def load(fp):
     """SysML load from file pointer
 
     Deserialize ``fp`` (a ``.read()``-supporting file-like object containing
     a SysML v2.0 document) to a Python dictionary object.
 
@@ -37,14 +31,16 @@
 
     Raises
     ------
     TypeError
         Input was not _io.TextIOWrapper
 
     """
+    import io
+
     if not isinstance(fp, io.TextIOWrapper):
         raise TypeError(
             f"the SysML object must be _io.TextIOWrapper, "
             f"not {fp.__class__.__name__}"
         )
 
     return loads(fp.read())
@@ -69,25 +65,37 @@
 
     Raises
     ------
     TypeError
         Input was not str
 
     """
+    import importlib.resources as pkg_resources
+
+    from textx import metamodel_from_file, TextXSyntaxError
+
+    import sysml2py
+    from sysml2py.formatting import reformat
 
     if not isinstance(s, str):
         raise TypeError(f"the SysML object must be str, " f"not {s.__class__.__name__}")
 
     try:
         grammar = str((pkg_resources.files(sysml2py) / "grammar/SysML.tx"))
     except:
         try:
             grammar = "./src/sysml2py/grammar/SysML.tx"
         except:
             grammar = "./grammar/SysML.tx"
     meta = metamodel_from_file(grammar)
-    model = meta.model_from_str(s, debug=True)
+    try:
+        model = meta.model_from_str(s, debug=False)
+    except TextXSyntaxError as e:
+        print(e)
+        import sys
+
+        sys.exit()
 
     if formatting == "json":
         return reformat(model)
     else:
         return model
```

### Comparing `sysml2py-0.2.5/src/sysml2py/formatting.py` & `sysml2py-0.3.1/src/sysml2py/formatting.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 Created on Wed May 31 13:26:53 2023
 
 @author: christophercox
 """
 
 from sysml2py.grammar.classes import RootNamespace
+from sysml2py import Part
 
 
 def remove_classes(model):
     """An example docstring for a class definition."""
     if type(model) == type(dict()):
         output = {}
         for element in model:
@@ -45,7 +46,31 @@
         print("Error in printing")
 
     return model_out
 
 
 def classtree(model):
     return RootNamespace(model)
+
+
+def collapse(model):
+    """Take a classtree and collapse it into our special classes that
+    package all of the sub-grammar classes."""
+    output = []
+    if model.__class__.__name__ == "RootNamespace":
+        for child in model.children[0].children:
+            if child.__class__.__name__ == "UsageElement":
+                ue = child.children
+                if ue.__class__.__name__ == "OccurrenceUsageElement":
+                    se = ue.children
+                    if se.children.__class__.__name__ == "PartUsage":
+                        output.append(Part().load_from_grammar(se.children))
+                    else:
+                        pass
+                else:
+                    # OccurrenceUsageElement
+                    pass
+            else:
+                pass
+    else:
+        print("no")
+    return output
```

### Comparing `sysml2py-0.2.5/src/sysml2py/grammar/KerML.tx` & `sysml2py-0.3.1/src/sysml2py/grammar/KerML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.2.5/src/sysml2py/grammar/KerMLExpressions.tx` & `sysml2py-0.3.1/src/sysml2py/grammar/KerMLExpressions.tx`

 * *Files 6% similar despite different names*

```diff
@@ -291,35 +291,24 @@
 	| primary=PrimaryExpression
 ;
 
 /* Primary Expressions */
 
 PrimaryExpression :
 	base=BaseExpression
-	(  '.'
-	  ownedRelationship += FeatureChainMember
-	)?
-	( (
-	    operator = '#' '(' operand += SequenceExpression ')'
-	  |
-	    operator = '[' operand += SequenceExpression ']'
-	  |  '->'
-	    ownedRelationship += ReferenceTyping
-	    ( operand += BodyExpression
-	    | operand += FunctionReferenceExpression
-	    | ArgumentList
-	    )
-	  |  '.'
-	    operand += BodyExpression
-	  |  '.?'
-	    operand += BodyExpression
+	(  '.' ownedRelationship += FeatureChainMember )?
+	(
+    ( operator += '#' '(' operand += SequenceExpression ')'
+      | operator += '[' operand += SequenceExpression ']'
+      | operator += '->' ownedRelationship += ReferenceTyping
+        ( operand += BodyExpression | operand += FunctionReferenceExpression | operand+= ArgumentList )
+      |  operator += '.' operand += BodyExpression
+      |  operator += '.?' operand += BodyExpression
 	  )
-	  (  '.'
-	  	ownedRelationship += FeatureChainMember
-	  )?
+	  (  '.' ownedRelationship += FeatureChainMember )?
 	)*
 ;
 
 FunctionReferenceExpression :
 	ownedRelationship += FunctionReferenceMember
 ;
 
@@ -375,19 +364,15 @@
 BodyParameter :
 	declaredName = Name
 ;
 
 // Sequence Expressions
 
 SequenceExpression :
-	OwnedExpression
-	( ','
-	|  operator = ','
-	  operand += SequenceExpression
-	)?
+	ownedRelationship=OwnedExpression ( ',' |  operator = ',' operand += SequenceExpression)?
 ;
 
 // Feature Reference Expressions
 
 FeatureReferenceExpression :
 	ownedRelationship += FeatureReferenceMember
 ;
```

### Comparing `sysml2py-0.2.5/src/sysml2py/grammar/SysML.tx` & `sysml2py-0.3.1/src/sysml2py/grammar/SysML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.2.5/src/sysml2py/grammar/classes.py` & `sysml2py-0.3.1/src/sysml2py/grammar/classes.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,34 +11,54 @@
 
 def valid_definition(definition, name):
     if isinstance(definition, dict):
         if "name" in definition:
             if definition["name"] == name:
                 return True
             else:
+                print(definition["name"])
                 raise NotImplementedError
 
         else:
             raise AttributeError("This does not seem to be valid.")
     else:
-        print("Definition: {}".format(definition))
+        print("\n\nDefinition: {}".format(definition))
         raise TypeError("This does not seem to be valid.")
 
 
+def beautify(string):
+    level = 0
+    lines = string.split("\n")
+    ns = []
+    # print(lines)
+    for line in lines:
+        if line == "}":
+            level += -1
+
+        ns.append(level * "   " + line)
+
+        if line[-1] == "{":
+            # Last character is new bracket
+            level += 1
+
+    return "\n".join(ns)
+
+
 class RootNamespace:
     def __init__(self, definition):
         self.children = []
         if "name" in definition:
             if definition["name"] == "PackageBodyElement":
                 # This is a SysML Element
                 self.load_package_body(definition["ownedRelationship"])
             elif definition["name"] == "NamespaceBodyElement":
                 # This is a KerML Element
                 pass
             else:
+                print(definition)
                 raise NotImplementedError("Not expecting any other root node names.")
         else:
             raise AttributeError("This does not seem to be valid.")
 
     def load_package_body(self, definition):
         for member in definition:
             # Options here are PackageMember, ElementFilterMember, AliasMember, Import
@@ -55,15 +75,15 @@
 
             self.children.append(memberclass)
 
     def dump(self):
         output = []
         for child in self.children:
             output.append(child.dump())
-        return "\n".join(output)
+        return beautify("\n".join(output))
 
 
 class DefinitionElement:
     def __init__(self, definition):
         self.children = []
         if valid_definition(definition, "DefinitionElement"):
             # This is a SysML Element
@@ -104,14 +124,21 @@
     def dump(self):
         output = []
         for child in self.children:
             output.append(child.dump())
 
         return " ".join(filter(None, (output)))
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "ownedRelatedElement": []}
+
+        for item in self.children:
+            output["ownedRelatedElement"] = item.get_definition()
+        return output
+
 
 class InterfaceDefinition:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             self.prefix = None
             self.keyword = "interface def"
             self.declaration = None
@@ -329,32 +356,43 @@
         if self.definition is not None:
             output.append(self.definition.dump())
 
         return " ".join(output)
 
 
 class ItemDefinition:
-    def __init__(self, definition):
-        if valid_definition(definition, self.__class__.__name__):
-            self.keyword = "item def"
-            if definition["prefix"] is not None:
-                self.prefix = OccurrenceDefinitionPrefix(definition["prefix"])
-            else:
-                self.prefix = None
-            self.definition = Definition(definition["definition"])
+    def __init__(self, definition=None):
+        self.keyword = "item def"
+        if definition is not None:
+            if valid_definition(definition, self.__class__.__name__):
+                if definition["prefix"] is not None:
+                    self.prefix = OccurrenceDefinitionPrefix(definition["prefix"])
+                else:
+                    self.prefix = None
+                self.definition = Definition(definition["definition"])
+        else:
+            self.prefix = None
+            self.definition = Definition()
 
     def dump(self):
         output = []
         if self.prefix is not None:
             output.append(self.prefix.dump())
 
         output.append(self.keyword)
         output.append(self.definition.dump())
         return " ".join(output)
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "prefix": None}
+        if self.prefix is not None:
+            output["prefix"] = self.prefix.get_definition()
+        output["definition"] = self.definition.get_definition()
+        return output
+
 
 class EnumerationDefinition:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             self.keyword = "enum def"
             self.declaration = DefinitionDeclaration(definition["declaration"])
             self.body = EnumerationBody(definition["body"])
@@ -511,48 +549,73 @@
         if self.identification is not None:
             return " ".join([self.keyword, self.identification.dump(), self.body])
         else:
             return " ".join([self.keyword, self.body])
 
 
 class AttributeDefinition:
-    def __init__(self, definition):
-        if valid_definition(definition, "AttributeDefinition"):
-            if definition["prefix"] is not None:
-                raise NotImplementedError
+    def __init__(self, definition=None):
+        self.keyword = "attribute def"
+        if definition is not None:
+            if valid_definition(definition, "AttributeDefinition"):
+                if definition["prefix"] is not None:
+                    raise NotImplementedError
+                self.prefix = None
+                self.definition = Definition(definition["definition"])
+        else:
             self.prefix = None
-            self.keyword = "attribute def"
-            self.definition = Definition(definition["definition"])
+            self.definition = Definition()
 
     def dump(self):
         return " ".join(
             filter(None, (self.prefix, self.keyword, self.definition.dump()))
         )
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "prefix": None}
+        if self.prefix is not None:
+            output["prefix"] = self.prefix.get_definition()
+        output["definition"] = self.definition.get_definition()
+        return output
+
 
 class PartDefinition:
-    def __init__(self, definition):
-        if valid_definition(definition, "PartDefinition"):
-            if definition["prefix"] is not None:
-                self.prefix = OccurrenceDefinitionPrefix(definition["prefix"])
-            else:
-                self.prefix = None
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, "PartDefinition"):
+                if definition["prefix"] is not None:
+                    self.prefix = OccurrenceDefinitionPrefix(definition["prefix"])
+                else:
+                    self.prefix = None
+                self.keyword = "part def"
+                self.definition = Definition(definition["definition"])
+        else:
+            self.prefix = None
             self.keyword = "part def"
-            self.definition = Definition(definition["definition"])
+            self.definition = Definition()
 
     def dump(self):
         output = []
         if self.prefix is not None:
             output.append(self.prefix.dump())
 
         output.append(self.keyword)
         output.append(self.definition.dump())
 
         return " ".join(output)
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "prefix": None}
+        if self.prefix is not None:
+            output["prefix"] = self.prefix.get_definition()
+
+        output["definition"] = self.definition.get_definition()
+
+        return output
+
 
 class OccurrenceDefinitionPrefix:
     def __init__(self, definition):
         if valid_definition(definition, "OccurrenceDefinitionPrefix"):
             if definition["prefix"] is not None:
                 self.prefix = BasicDefinitionPrefix(definition["prefix"])
             else:
@@ -603,52 +666,86 @@
             raise NotImplementedError
 
     def dump(self):
         raise NotImplementedError
 
 
 class Definition:
-    def __init__(self, definition):
-        if valid_definition(definition, "Definition"):
-            self.declaration = DefinitionDeclaration(definition["declaration"])
-            self.body = DefinitionBody(definition["body"])
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, "Definition"):
+                self.declaration = DefinitionDeclaration(definition["declaration"])
+                self.body = DefinitionBody(definition["body"])
+        else:
+            self.declaration = DefinitionDeclaration()
+            self.body = DefinitionBody()
 
     def dump(self):
         return " ".join([self.declaration.dump(), self.body.dump()])
 
+    def get_definition(self):
+        return {
+            "name": self.__class__.__name__,
+            "body": self.body.get_definition(),
+            "declaration": self.declaration.get_definition(),
+        }
+
 
 class DefinitionDeclaration:
-    def __init__(self, definition):
-        if valid_definition(definition, self.__class__.__name__):
-            if "identification" in definition:
-                if definition["identification"] is not None:
-                    self.identification = Identification(definition["identification"])
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, self.__class__.__name__):
+                if "identification" in definition:
+                    if definition["identification"] is not None:
+                        self.identification = Identification(
+                            definition["identification"]
+                        )
+                    else:
+                        self.identification = None
                 else:
                     self.identification = None
-            else:
-                self.identification = None
 
-            if "subclassificationpart" in definition:
-                if definition["subclassificationpart"] is not None:
-                    self.subclassificationpart = SubclassificationPart(
-                        definition["subclassificationpart"]
-                    )
+                if "subclassificationpart" in definition:
+                    if definition["subclassificationpart"] is not None:
+                        self.subclassificationpart = SubclassificationPart(
+                            definition["subclassificationpart"]
+                        )
+                    else:
+                        self.subclassificationpart = None
                 else:
                     self.subclassificationpart = None
-            else:
-                self.subclassificationpart = None
+
+        else:
+            self.identification = Identification()
+            self.subclassificationpart = None
 
     def dump(self):
         output = []
         if self.identification is not None:
             output.append(self.identification.dump())
         if self.subclassificationpart is not None:
             output.append(self.subclassificationpart.dump())
         return " ".join(output)
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "identification": None,
+            "subclassificationpart": None,
+        }
+        if self.identification is not None:
+            output["identification"] = self.identification.get_definition()
+
+        if self.subclassificationpart is not None:
+            output[
+                "subclassificationpart"
+            ] = self.subclassificationpart.get_definition()
+
+        return output
+
 
 class SubclassificationPart:
     def __init__(self, definition):
         if valid_definition(definition, "SubclassificationPart"):
             self.keyword = ":> "
             self.children = []
             for relationship in definition["ownedRelationship"]:
@@ -664,52 +761,71 @@
             self.name = QualifiedName(definition["superclassifier"])
 
     def dump(self):
         return self.name.dump()
 
 
 class DefinitionBody:
-    def __init__(self, definition):
-        if valid_definition(definition, "DefinitionBody"):
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, "DefinitionBody"):
+                self.children = []
+                if len(definition["ownedRelatedElement"]) > 0:
+                    for item in definition["ownedRelatedElement"]:
+                        self.children.append(DefinitionBodyItem(item))
+        else:
             self.children = []
-            if len(definition["ownedRelatedElement"]) > 0:
-                for item in definition["ownedRelatedElement"]:
-                    self.children.append(DefinitionBodyItem(item))
 
     def dump(self):
         if len(self.children) == 0:
             return ";"
         else:
             output = []
             for child in self.children:
                 output.append(child.dump())
             return " {\n" + "\n".join(output) + "\n}"
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "ownedRelatedElement": []}
+        for child in self.children:
+            output["ownedRelatedElement"].append(child.get_definition())
+
+        return output
+
 
 class DefinitionBodyItem:
     def __init__(self, definition):
         if valid_definition(definition, "DefinitionBodyItem"):
             self.children = []
             if len(definition["ownedRelationship"]) > 0:
                 for item in definition["ownedRelationship"]:
                     if item["name"] == "OccurrenceUsageMember":
                         self.children.append(OccurrenceUsageMember(item))
                     elif item["name"] == "NonOccurrenceUsageMember":
                         self.children.append(NonOccurrenceUsageMember(item))
                     elif item["name"] == "DefinitionMember":
                         self.children.append(DefinitionMember(item))
                     else:
+                        print(definition)
                         raise NotImplementedError
 
     def dump(self):
         output = []
         for child in self.children:
             output.append(child.dump())
         return "\n".join(output)
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__}
+        items = []
+        for item in self.children:
+            items.append(item.get_definition())
+        output["ownedRelationship"] = items
+        return output
+
 
 class DefinitionMember:
     def __init__(self, definition):
         if valid_definition(definition, "DefinitionMember"):
             if definition["prefix"] is not None:
                 raise NotImplementedError
             else:
@@ -718,14 +834,27 @@
             self.children = []
             for element in definition["ownedRelatedElement"]:
                 self.children.append(DefinitionElement(element))
 
     def dump(self):
         return "\n".join([child.dump() for child in self.children])
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "prefix": None,
+            "ownedRelatedElement": [],
+        }
+        if self.prefix is not None:
+            output["prefix"] = self.prefix.get_definition()
+
+        for item in self.children:
+            output["ownedRelatedElement"].append(item.get_definition())
+        return output
+
 
 class OccurrenceUsageMember:
     def __init__(self, definition):
         if valid_definition(definition, "OccurrenceUsageMember"):
             if definition["prefix"] is not None:
                 raise NotImplementedError
             else:
@@ -737,14 +866,28 @@
 
     def dump(self):
         output = []
         for child in self.children:
             output.append(child.dump())
         return "\n".join(output)
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "prefix": None,
+            "ownedRelatedElement": [],
+        }
+        if self.prefix is not None:
+            output["prefix"] = self.prefix.get_definition()
+
+        for child in self.children:
+            output["ownedRelatedElement"].append(child.get_definition())
+
+        return output
+
 
 class NonOccurrenceUsageMember:
     def __init__(self, definition):
         if valid_definition(definition, "NonOccurrenceUsageMember"):
             if definition["prefix"] is not None:
                 raise NotImplementedError
             else:
@@ -756,14 +899,28 @@
 
     def dump(self):
         output = []
         for child in self.children:
             output.append(child.dump())
         return "\n".join(output)
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "prefix": None,
+            "ownedRelatedElement": [],
+        }
+        if self.prefix is not None:
+            output["prefix"] = self.prefix.get_definition()
+
+        for child in self.children:
+            output["ownedRelatedElement"].append(child.get_definition())
+
+        return output
+
 
 class UsageElement:
     def __init__(self, definition):
         if valid_definition(definition, "UsageElement"):
             if definition["ownedRelatedElement"]["name"] == "NonOccurrenceUsageElement":
                 self.children = NonOccurrenceUsageElement(
                     definition["ownedRelatedElement"]
@@ -789,14 +946,19 @@
             else:
                 print(definition["ownedRelatedElement"]["name"])
                 raise NotImplementedError
 
     def dump(self):
         return self.children.dump()
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__}
+        output["ownedRelatedElement"] = self.children.get_definition()
+        return output
+
 
 class DefaultReferenceUsage:
     def __init__(self, definition):
         if valid_definition(definition, "DefaultReferenceUsage"):
             if definition["prefix"] is not None:
                 self.prefix = RefPrefix(definition["prefix"])
             else:
@@ -837,14 +999,20 @@
                         raise NotImplementedError
                     else:
                         raise NotImplementedError
 
     def dump(self):
         return "".join([child.dump() for child in self.relationships])
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "ownedRelationship": []}
+        for child in self.relationships:
+            output["ownedRelationship"].append(child.get_definition())
+        return output
+
 
 class FeatureValue:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             self.isDefault = definition["isDefault"]
             self.isInitial = definition["isInitial"]
             self.isEqual = definition["isEqual"]
@@ -860,37 +1028,58 @@
             output.append("=")
         elif self.isInitial:
             output.append(":=")
         for child in self.elements:
             output.append(child.dump())
         return " ".join(output)
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "ownedRelatedElement": []}
+        for child in self.elements:
+            output["ownedRelatedElement"].append(child.get_definition())
+        output["isEqual"] = self.isEqual
+        output["isInitial"] = self.isInitial
+        output["isDefault"] = self.isDefault
+        return output
+
 
 class OwnedExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             self.expression = ConditionalExpression(definition["expression"])
 
     def dump(self):
         return self.expression.dump()
 
+    def get_definition(self):
+        return {
+            "name": self.__class__.__name__,
+            "expression": self.expression.get_definition(),
+        }
+
 
 class ConditionalExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["operand"] is not None:
                 self.operands = []
                 for op in definition["operand"]:
                     self.operands.append(NullCoalescingExpression(op))
             else:
                 raise NotImplementedError
 
     def dump(self):
         return "".join(child.dump() for child in self.operands)
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "operator": [], "operand": []}
+        for child in self.operands:
+            output["operand"].append(child.get_definition())
+        return output
+
 
 class NullCoalescingExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["implies"] is not None:
                 self.implies = ImpliesExpression(definition["implies"])
             else:
@@ -898,14 +1087,23 @@
 
             if not (definition["operand"] == [] and definition["operator"] == []):
                 raise NotImplementedError
 
     def dump(self):
         return self.implies.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": [],
+            "operand": [],
+            "implies": self.implies.get_definition(),
+        }
+        return output
+
 
 class ImpliesExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["or"] is not None:
                 self.orexpression = OrExpression(definition["or"])
             else:
@@ -913,14 +1111,23 @@
 
             if not (definition["operand"] == [] and definition["operator"] == []):
                 raise NotImplementedError
 
     def dump(self):
         return self.orexpression.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": [],
+            "operand": [],
+            "or": self.orexpression.get_definition(),
+        }
+        return output
+
 
 class OrExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["xor"] is not None:
                 self.xor = XorExpression(definition["xor"])
             else:
@@ -928,14 +1135,23 @@
 
             if not (definition["operand"] == [] and definition["operator"] == []):
                 raise NotImplementedError
 
     def dump(self):
         return self.xor.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": [],
+            "operand": [],
+            "xor": self.xor.get_definition(),
+        }
+        return output
+
 
 class XorExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["and"] is not None:
                 self.andexpression = AndExpression(definition["and"])
             else:
@@ -943,14 +1159,23 @@
 
             if not (definition["operand"] == [] and definition["operator"] == []):
                 raise NotImplementedError
 
     def dump(self):
         return self.andexpression.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": [],
+            "operand": [],
+            "and": self.andexpression.get_definition(),
+        }
+        return output
+
 
 class AndExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["equality"] is not None:
                 self.equality = EqualityExpression(definition["equality"])
             else:
@@ -958,14 +1183,23 @@
 
             if not (definition["operand"] == [] and definition["operator"] == []):
                 raise NotImplementedError
 
     def dump(self):
         return self.equality.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": [],
+            "operand": [],
+            "equality": self.equality.get_definition(),
+        }
+        return output
+
 
 class EqualityExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["classification"] is not None:
                 self.classification = ClassificationExpression(
                     definition["classification"]
@@ -975,14 +1209,23 @@
 
             if not (definition["operand"] == [] and definition["operator"] == []):
                 raise NotImplementedError
 
     def dump(self):
         return self.classification.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": [],
+            "operand": [],
+            "classification": self.classification.get_definition(),
+        }
+        return output
+
 
 class ClassificationExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["relational"] is not None:
                 self.relational = RelationalExpression(definition["relational"])
             else:
@@ -990,14 +1233,23 @@
 
             if not (definition["operand"] == [] and definition["operator"] is None):
                 raise NotImplementedError
 
     def dump(self):
         return self.relational.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": None,
+            "operand": [],
+            "relational": self.relational.get_definition(),
+        }
+        return output
+
 
 class RelationalExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["range"] is not None:
                 self.range = RangeExpression(definition["range"])
             else:
@@ -1005,14 +1257,23 @@
 
             if not (definition["operand"] == [] and definition["operator"] == []):
                 raise NotImplementedError
 
     def dump(self):
         return self.range.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": [],
+            "operand": [],
+            "range": self.range.get_definition(),
+        }
+        return output
+
 
 class RangeExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["additive"] is not None:
                 self.additive = AdditiveExpression(definition["additive"])
             else:
@@ -1020,14 +1281,23 @@
 
             if not (definition["operand"] == [] and definition["operator"] == ""):
                 raise NotImplementedError
 
     def dump(self):
         return self.additive.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": "",
+            "operand": [],
+            "additive": self.additive.get_definition(),
+        }
+        return output
+
 
 class AdditiveExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["multiplicitive"] is not None:
                 self.multiplicitive = MultiplicativeExpression(
                     definition["multiplicitive"]
@@ -1037,14 +1307,23 @@
 
             if not (definition["operand"] == [] and definition["operator"] == []):
                 raise NotImplementedError
 
     def dump(self):
         return self.multiplicitive.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": [],
+            "operand": [],
+            "multiplicitive": self.multiplicitive.get_definition(),
+        }
+        return output
+
 
 class MultiplicativeExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["exponential"] is not None:
                 self.exponential = ExponentiationExpression(definition["exponential"])
             else:
@@ -1052,14 +1331,23 @@
 
             if not (definition["operand"] == [] and definition["operator"] == []):
                 raise NotImplementedError
 
     def dump(self):
         return self.exponential.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": [],
+            "operand": [],
+            "exponential": self.exponential.get_definition(),
+        }
+        return output
+
 
 class ExponentiationExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["unary"] is not None:
                 self.unary = UnaryExpression(definition["unary"])
             else:
@@ -1067,14 +1355,23 @@
 
             if not (definition["operand"] == [] and definition["operator"] == []):
                 raise NotImplementedError
 
     def dump(self):
         return self.unary.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": [],
+            "operand": [],
+            "unary": self.unary.get_definition(),
+        }
+        return output
+
 
 class UnaryExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["extent"] is not None:
                 self.extent = ExtentExpression(definition["extent"])
             else:
@@ -1082,14 +1379,23 @@
 
             if not (definition["operand"] == [] and definition["operator"] is None):
                 raise NotImplementedError
 
     def dump(self):
         return self.extent.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": None,
+            "operand": [],
+            "extent": self.extent.get_definition(),
+        }
+        return output
+
 
 class ExtentExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["primary"] is not None:
                 self.primary = PrimaryExpression(definition["primary"])
             else:
@@ -1097,28 +1403,100 @@
 
             if not (definition["operator"] == ""):
                 raise NotImplementedError
 
     def dump(self):
         return self.primary.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": "",
+            "operand": [],
+            "primary": self.primary.get_definition(),
+            "ownedRelationship": [],
+        }
+        return output
+
 
 class PrimaryExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["base"] is not None:
                 self.base = BaseExpression(definition["base"])
             else:
                 raise NotImplementedError
 
+            if len(definition["ownedRelationship"]) > 0:
+                raise NotImplementedError
+
+            self.operator = []
+            self.operand = []
+
             if not (definition["operand"] == [] and definition["operator"] == []):
+                for child in definition["operator"]:
+                    self.operator.append(child)
+                for child in definition["operand"]:
+                    if child["name"] == "SequenceExpression":
+                        self.operand.append(SequenceExpression(child))
+
+    def dump(self):
+        output = [self.base.dump()]
+        for k, v in enumerate(self.operator):
+            if v == "#":
+                output.append("# ({})".format(self.operand[k].dump()))
+
+            if v == "[":
+                output.append("[{}]".format(self.operand[k].dump()))
+
+            if v == "." or v == ".?":
                 raise NotImplementedError
+        if len(output) == 1:
+            return str(output[0])
+        else:
+            return " ".join(output)
+
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": [],
+            "operand": [],
+            "base": self.base.get_definition(),
+            "ownedRelationship": [],
+        }
+        for child in self.operand:
+            output["operand"].append(child.get_definition())
+
+        for child in self.operator:
+            output["operator"].append(child)
+        return output
+
+
+class SequenceExpression:
+    def __init__(self, definition):
+        if valid_definition(definition, self.__class__.__name__):
+            if not (definition["operand"] == [] and definition["operator"] == ""):
+                raise NotImplementedError
+
+            self.child = None
+            if definition["ownedRelationship"] is not None:
+                if definition["ownedRelationship"]["name"] == "OwnedExpression":
+                    self.child = OwnedExpression(definition["ownedRelationship"])
 
     def dump(self):
-        return self.base.dump()
+        return self.child.dump()
+
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "operator": "",
+            "operand": [],
+            "ownedRelationship": self.child.get_definition(),
+        }
+        return output
 
 
 class BaseExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["ownedRelationship"]["name"] == "FeatureReferenceExpression":
                 self.relationship = FeatureReferenceExpression(
@@ -1132,46 +1510,75 @@
                 self.relationship = LiteralReal(definition["ownedRelationship"])
             else:
                 raise NotImplementedError
 
     def dump(self):
         return self.relationship.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "ownedRelationship": self.relationship.get_definition(),
+        }
+        return output
+
 
 class FeatureReferenceExpression:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             self.children = []
             for relationship in definition["ownedRelationship"]:
                 self.children.append(FeatureReferenceMember(relationship))
 
     def dump(self):
         return "".join([child.dump() for child in self.children])
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "ownedRelationship": [],
+        }
+        for child in self.children:
+            output["ownedRelationship"].append(child.get_definition())
+        return output
+
 
 class FeatureReferenceMember:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             self.memberElement = QualifiedName(definition["memberElement"])
 
     def dump(self):
         return self.memberElement.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "memberElement": self.memberElement.get_definition(),
+        }
+        return output
+
 
 class OccurrenceUsageElement:
     def __init__(self, definition):
         if valid_definition(definition, "OccurrenceUsageElement"):
             if definition["ownedRelatedElement"]["name"] == "StructureUsageElement":
                 self.children = StructureUsageElement(definition["ownedRelatedElement"])
             else:
                 raise NotImplementedError
 
     def dump(self):
         return self.children.dump()
 
+    def get_definition(self):
+        return {
+            "name": self.__class__.__name__,
+            "ownedRelatedElement": self.children.get_definition(),
+        }
+
 
 class StructureUsageElement:
     def __init__(self, definition):
         if valid_definition(definition, "StructureUsageElement"):
             if definition["ownedRelatedElement"]["name"] == "ItemUsage":
                 self.children = ItemUsage(definition["ownedRelatedElement"])
             elif definition["ownedRelatedElement"]["name"] == "PartUsage":
@@ -1184,14 +1591,20 @@
                 self.children = InterfaceUsage(definition["ownedRelatedElement"])
             else:
                 raise NotImplementedError
 
     def dump(self):
         return self.children.dump()
 
+    def get_definition(self):
+        return {
+            "name": self.__class__.__name__,
+            "ownedRelatedElement": self.children.get_definition(),
+        }
+
 
 class InterfaceUsage:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             self.prefix = None
             self.keyword = "interface"
             self.declaration = None
@@ -1457,46 +1870,76 @@
         if self.referencedFeature is not None:
             return self.referencedFeature.dump()
         else:
             return "".join([child.dump() for child in self.elements])
 
 
 class AttributeUsage:
-    def __init__(self, definition):
-        if valid_definition(definition, self.__class__.__name__):
-            if definition["prefix"] is not None:
-                raise NotImplementedError
-            self.prefix = definition["prefix"]
-            self.keyword = "attribute"
-            self.usage = Usage(definition["usage"])
+    def __init__(self, definition=None):
+        self.keyword = "attribute"
+        if definition is not None:
+            if valid_definition(definition, self.__class__.__name__):
+                if definition["prefix"] is not None:
+                    raise NotImplementedError
+                else:
+                    self.prefix = None
+                self.usage = Usage(definition["usage"])
+        else:
+            self.prefix = None
+            self.usage = Usage()
 
     def dump(self):
         return self.keyword + " " + self.usage.dump()
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "prefix": None}
+        if self.prefix is not None:
+            output["prefix"] = self.prefix.get_definition()
+
+        output["usage"] = self.usage.get_definition()
+
+        return output
+
 
 class PartUsage:
-    def __init__(self, definition):
-        if valid_definition(definition, "PartUsage"):
-            if definition["prefix"] is not None:
-                self.prefix = OccurrenceUsagePrefix(definition["prefix"])
-            else:
-                self.prefix = None
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, "PartUsage"):
+                if definition["prefix"] is not None:
+                    self.prefix = OccurrenceUsagePrefix(definition["prefix"])
+                else:
+                    self.prefix = None
 
+                self.keyword = "part"
+                self.usage = Usage(definition["usage"])
+        else:
+            self.prefix = None
             self.keyword = "part"
-            self.usage = Usage(definition["usage"])
+            self.usage = Usage()
 
     def dump(self):
         output = []
         if self.prefix is not None:
             output.append(self.prefix.dump())
 
         output.append(self.keyword)
         output.append(self.usage.dump())
         return " ".join(output)
 
+    def get_definition(self):
+        pre = None
+        if self.prefix is not None:
+            pre = self.prefix.get_definition()
+
+        u = None
+        if self.usage is not None:
+            u = self.usage.get_definition()
+
+        return {"name": self.__class__.__name__, "prefix": pre, "usage": u}
+
 
 class OccurrenceUsagePrefix:
     def __init__(self, definition):
         if valid_definition(definition, "OccurrenceUsagePrefix"):
             self.prefix = BasicUsagePrefix(definition["prefix"])
             self.isIndividual = definition["isIndividual"]
             if definition["portionKind"] is not None:
@@ -1600,101 +2043,163 @@
         elif self.isOut:
             return "out"
         else:
             raise NotImplementedError
 
 
 class ItemUsage:
-    def __init__(self, definition):
-        if valid_definition(definition, "ItemUsage"):
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, "ItemUsage"):
+                self.prefix = None
+                if definition["prefix"] is not None:
+                    self.prefix = OccurrenceUsagePrefix(definition["prefix"])
+                self.keyword = "item"
+                self.usage = Usage(definition["usage"])
+        else:
+            # Create an empty item
             self.prefix = None
-            if definition["prefix"] is not None:
-                self.prefix = OccurrenceUsagePrefix(definition["prefix"])
             self.keyword = "item"
-            self.usage = Usage(definition["usage"])
+            self.usage = Usage()
 
     def dump(self):
         output = []
         if self.prefix is not None:
             output.append(self.prefix.dump())
         output.append(self.keyword)
         output.append(self.usage.dump())
         return " ".join(output)
 
+    def get_definition(self):
+        output = {}
+        output["name"] = self.__class__.__name__
+        if self.prefix is not None:
+            output["prefix"] = self.prefix.get_definition()
+        else:
+            output["prefix"] = None
+        output["usage"] = self.usage.get_definition()
+        return output
+
 
 class Usage:
-    def __init__(self, definition):
-        if valid_definition(definition, "Usage"):
-            self.declaration = UsageDeclaration(definition["declaration"])
-            self.completion = UsageCompletion(definition["completion"])
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, "Usage"):
+                self.declaration = UsageDeclaration(definition["declaration"])
+                self.completion = UsageCompletion(definition["completion"])
+        else:
+            self.declaration = UsageDeclaration()
+            self.completion = UsageCompletion()
 
     def dump(self):
         return "".join([self.declaration.dump(), self.completion.dump()])
 
+    def get_definition(self):
+        output = {}
+        output["name"] = self.__class__.__name__
+        output["declaration"] = self.declaration.get_definition()
+        output["completion"] = self.completion.get_definition()
+        return output
+
 
 class UsageDeclaration:
-    def __init__(self, definition):
-        if valid_definition(definition, "UsageDeclaration"):
-            self.declaration = FeatureDeclaration(definition["declaration"])
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, "UsageDeclaration"):
+                self.declaration = FeatureDeclaration(definition["declaration"])
+        else:
+            self.declaration = FeatureDeclaration()
 
     def dump(self):
         return self.declaration.dump()
 
+    def get_definition(self):
+        return {
+            "name": self.__class__.__name__,
+            "declaration": self.declaration.get_definition(),
+        }
+
 
 class FeatureDeclaration:
-    def __init__(self, definition):
-        if valid_definition(definition, "FeatureDeclaration"):
-            if definition["identification"] is not None:
-                self.identification = Identification(definition["identification"])
-            else:
-                self.identification = None
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, "FeatureDeclaration"):
+                if definition["identification"] is not None:
+                    self.identification = Identification(definition["identification"])
+                else:
+                    self.identification = None
 
-            if definition["specialization"] is not None:
-                self.specialization = FeatureSpecializationPart(
-                    definition["specialization"]
-                )
-            else:
-                self.specialization = None
+                if definition["specialization"] is not None:
+                    self.specialization = FeatureSpecializationPart(
+                        definition["specialization"]
+                    )
+                else:
+                    self.specialization = None
+        else:
+            self.identification = None
+            self.specialization = None
 
     def dump(self):
         output = []
         if self.identification is not None:
             output.append(self.identification.dump())
 
         if self.specialization is not None:
             output.append(self.specialization.dump())
 
         return "".join(output)
 
+    def get_definition(self):
+        iden = None
+        spec = None
+        if self.identification is not None:
+            iden = self.identification.get_definition()
+
+        if self.specialization is not None:
+            spec = self.specialization.get_definition()
+
+        return {
+            "name": self.__class__.__name__,
+            "identification": iden,
+            "specialization": spec,
+        }
+
 
 class FeatureSpecializationPart:
-    def __init__(self, definition):
-        if valid_definition(definition, "FeatureSpecializationPart"):
-            if definition["multiplicity"] is not None:
-                # We found the set where one specialization came first
-                # ( specialization+=FeatureSpecialization )+
-                #    multiplicity=MultiplicityPart?
-                #    specialization2+=FeatureSpecialization*
-                self.multiplicity = MultiplicityPart(definition["multiplicity"])
-            elif definition["multiplicity2"] is not None:
-                # We found the set where the multiplicity came first
-                # multiplicity2=MultiplicityPart specialization+=FeatureSpecialization*
-                self.multiplicity = MultiplicityPart(definition["multiplicity2"])
-            else:
-                # We found the case where none were specified
-                self.multiplicity = None
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, "FeatureSpecializationPart"):
+                if definition["multiplicity"] is not None:
+                    # We found the set where one specialization came first
+                    # ( specialization+=FeatureSpecialization )+
+                    #    multiplicity=MultiplicityPart?
+                    #    specialization2+=FeatureSpecialization*
+                    self.multiplicity = MultiplicityPart(definition["multiplicity"])
+                elif definition["multiplicity2"] is not None:
+                    # We found the set where the multiplicity came first
+                    # multiplicity2=MultiplicityPart specialization+=FeatureSpecialization*
+                    self.multiplicity = MultiplicityPart(definition["multiplicity2"])
+                else:
+                    # We found the case where none were specified
+                    self.multiplicity = None
 
+                self.specializations = []
+                for specialization in definition["specialization"]:
+                    self.specializations.append(FeatureSpecialization(specialization))
+
+                self.specializations2 = []
+                if definition["specialization2"] is not None:
+                    for specialization in definition["specialization2"]:
+                        self.specializations2.append(
+                            FeatureSpecialization(specialization)
+                        )
+        else:
+            self.multiplicity = None
             self.specializations = []
-            for specialization in definition["specialization"]:
-                self.specializations.append(FeatureSpecialization(specialization))
-
             self.specializations2 = []
-            if definition["specialization2"] is not None:
-                for specialization in definition["specialization2"]:
-                    self.specializations2.append(FeatureSpecialization(specialization))
 
     def dump(self):
         if len(self.specializations2) > 0:
             # Multiplicity in between
             output = [child.dump() for child in self.specializations]
             if self.multiplicity is not None:
                 output.append(self.multiplicity.dump())
@@ -1714,14 +2219,36 @@
                 output.append(self.multiplicity.dump())
 
             for child in self.specializations:
                 output.append(child.dump())
 
         return "".join(output)
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "multiplicity": None,
+            "multiplicity2": None,  # This is never used in this fashion.
+            "specialization": [],
+            "specialization2": [],
+        }
+
+        if self.multiplicity is not None:
+            output["multiplicity"].get_definition()
+
+        if len(self.specializations) > 0:
+            for child in self.specializations:
+                output["specialization"].append(child.get_definition())
+
+        if len(self.specializations2) > 0:
+            for child in self.specializations2:
+                output["specialization2"].append(child.get_definition())
+
+        return output
+
 
 class MultiplicityPart:
     def __init__(self, definition):
         if valid_definition(definition, "MultiplicityPart"):
             self.isOrdered = definition["isOrdered"]
             self.isNonunique = definition["isNonunique"]
             self.isOrdered2 = definition["isOrdered"]
@@ -1809,14 +2336,17 @@
     def __init__(self, definition):
         if valid_definition(definition, "LiteralInteger"):
             self.element = definition["value"]
 
     def dump(self):
         return self.element
 
+    def get_definition(self):
+        return {"name": self.__class__.__name__, "value": self.element}
+
 
 class LiteralReal:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             self.element = definition["value"]
 
     def dump(self):
@@ -1845,14 +2375,21 @@
                 self.relationship = Redefinitions(definition["ownedRelationship"])
             else:
                 raise NotImplementedError
 
     def dump(self):
         return self.relationship.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "ownedRelationship": self.relationship.get_definition(),
+        }
+        return output
+
 
 class Redefinitions:
     def __init__(self, definition):
         if valid_definition(definition, "Redefinitions"):
             if len(definition["ownedRelationship"]) > 0:
                 raise NotImplementedError
 
@@ -1957,14 +2494,22 @@
                 self.relationships = []
 
             self.typing = TypedBy(definition["typedby"])
 
     def dump(self):
         return self.typing.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "ownedRelationship": self.relationships,
+            "typedby": self.typing.get_definition(),
+        }
+        return output
+
 
 class TypedBy:
     def __init__(self, definition):
         if valid_definition(definition, "TypedBy"):
             self.keyword = " : "
 
             self.relationships = []
@@ -1976,14 +2521,21 @@
 
     def dump(self):
         output = []
         for relationship in self.relationships:
             output.append(relationship.dump())
         return self.keyword + "".join(output)
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "ownedRelationship": []}
+        for child in self.relationships:
+            output["ownedRelationship"].append(child.get_definition())
+
+        return output
+
 
 class FeatureTyping:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             if definition["ownedRelationship"]["name"] == "OwnedFeatureTyping":
                 self.relationship = OwnedFeatureTyping(definition["ownedRelationship"])
             elif definition["ownedRelationship"]["name"] == "ConjugatedPortTyping":
@@ -1992,14 +2544,22 @@
                 )
             else:
                 raise NotImplementedError
 
     def dump(self):
         return self.relationship.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "ownedRelationship": self.relationship.get_definition(),
+        }
+
+        return output
+
 
 class ConjugatedPortTyping:
     def __init__(self, definition):
         if valid_definition(definition, self.__class__.__name__):
             self.keyword = "~"
             # We skip a step in the grammar here.
             self.name = QualifiedName(definition["conjugatedPortDefinition"])
@@ -2015,53 +2575,87 @@
                 self.type = FeatureType(definition["type"])
             else:
                 raise NotImplementedError
 
     def dump(self):
         return self.type.dump()
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__, "type": self.type.get_definition()}
+
+        return output
+
 
 class FeatureType:
     def __init__(self, definition):
         if valid_definition(definition, "FeatureType"):
             if len(definition["ownedRelatedElement"]) > 0:
                 raise NotImplementedError
             else:
                 self.type = QualifiedName(definition["type"])
 
     def dump(self):
         return self.type.dump()
 
+    def get_definition(self):
+        output = {
+            "name": self.__class__.__name__,
+            "ownedRelatedElement": [],
+            "type": self.type.get_definition(),
+        }
+        return output
+
 
 class UsageCompletion:
-    def __init__(self, definition):
-        if valid_definition(definition, "UsageCompletion"):
-            if definition["valuepart"] is None:
-                self.valuepart = None
-            else:
-                self.valuepart = ValuePart(definition["valuepart"])
-            self.body = UsageBody(definition["body"])
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, "UsageCompletion"):
+                if definition["valuepart"] is None:
+                    self.valuepart = None
+                else:
+                    self.valuepart = ValuePart(definition["valuepart"])
+                self.body = UsageBody(definition["body"])
+        else:
+            self.valuepart = None
+            self.body = UsageBody()
 
     def dump(self):
         output = []
         if self.valuepart is not None:
             output.append(self.valuepart.dump())
 
         output.append(self.body.dump())
         return "".join(output)
 
+    def get_definition(self):
+        vp = None
+        if self.valuepart is not None:
+            vp = self.valuepart.get_definition()
+
+        return {
+            "name": self.__class__.__name__,
+            "valuepart": vp,
+            "body": self.body.get_definition(),
+        }
+
 
 class UsageBody:
-    def __init__(self, definition):
-        if valid_definition(definition, "UsageBody"):
-            self.body = DefinitionBody(definition["body"])
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, "UsageBody"):
+                self.body = DefinitionBody(definition["body"])
+        else:
+            self.body = DefinitionBody()
 
     def dump(self):
         return self.body.dump()
 
+    def get_definition(self):
+        return {"name": self.__class__.__name__, "body": self.body.get_definition()}
+
 
 class PackageMember:
     def __init__(self, definition):
         self.children = []
         if valid_definition(definition, "PackageMember"):
             # This is a SysML Element
             if definition["prefix"] is not None:
@@ -2112,25 +2706,43 @@
             self.body = PackageBody(definition["body"])
 
     def dump(self):
         return "".join([self.declaration.dump(), self.body.dump()])
 
 
 class Identification:
-    def __init__(self, definition):
-        if valid_definition(definition, "Identification"):
-            if definition["declaredShortName"] == None:
-                self.declaredShortName = None
-            else:
-                self.declaredShortName = "<" + definition["declaredShortName"] + ">"
-            self.declaredName = definition["declaredName"]
+    def __init__(self, definition=None):
+        if definition is not None:
+            if valid_definition(definition, "Identification"):
+                if definition["declaredShortName"] == None:
+                    self.declaredShortName = None
+                else:
+                    if definition["declaredShortName"][0] == "<":
+                        definition["declaredShortName"] = definition[
+                            "declaredShortName"
+                        ][1:]
+                    if definition["declaredShortName"][-1] == ">":
+                        definition["declaredShortName"] = definition[
+                            "declaredShortName"
+                        ][:-1]
+                    self.declaredShortName = "<" + definition["declaredShortName"] + ">"
+                self.declaredName = definition["declaredName"]
+        else:
+            self.declaredName = None
+            self.declaredShortName = None
 
     def dump(self):
         return " ".join(filter(None, (self.declaredShortName, self.declaredName)))
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__}
+        output["declaredShortName"] = self.declaredShortName
+        output["declaredName"] = self.declaredName
+        return output
+
 
 class PackageDeclaration:
     def __init__(self, definition):
         if valid_definition(definition, "PackageDeclaration"):
             self.identification = Identification(definition["identification"])
 
     def dump(self):
@@ -2313,15 +2925,15 @@
         else:
             return self.visibility.dump() + self.keyword
 
 
 class ImportedNamespace:
     # The grammar for this file is currently broken.
     def __init__(self, definition):
-        if valid_definition(definition, "ImportedNamespace"):
+        if valid_definition(definition, self.__class__.__name__):
             self.namespaces = QualifiedName(definition["namespace"])
 
     def dump(self):
         return self.namespaces.dump() + "::*"
 
 
 class QualifiedName:
@@ -2330,14 +2942,20 @@
             self.names = [definition["name1"]]
             for name in definition["names"]:
                 self.names.append(name)
 
     def dump(self):
         return "::".join(self.names)
 
+    def get_definition(self):
+        output = {"name": self.__class__.__name__}
+        output["name1"] = self.names[0]
+        output["names"] = self.names[1:]
+        return output
+
 
 class VisibilityIndicator:
     def __init__(self, definition):
         if valid_definition(definition, "VisibilityIndicator"):
             if (
                 definition["private"] == "private"
                 and definition["protected"] == ""
```

### Comparing `sysml2py-0.2.5/src/sysml2py/textx/xtext_to_textx.py` & `sysml2py-0.3.1/src/sysml2py/textx/xtext_to_textx.py`

 * *Files identical despite different names*

