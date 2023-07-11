# Comparing `tmp/untouched-0.1.6.tar.gz` & `tmp/untouched-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "untouched-0.1.6.tar", max compression
+gzip compressed data, was "untouched-0.2.6.tar", max compression
```

## Comparing `untouched-0.1.6.tar` & `untouched-0.2.6.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1942 2023-07-10 23:44:26.091213 untouched-0.1.6/README.md
--rw-r--r--   0        0        0      378 2023-07-10 23:46:20.230862 untouched-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 21:53:14.532163 untouched-0.1.6/src/untouched/__init__.py
--rw-r--r--   0        0        0     2686 2023-07-10 23:45:55.170720 untouched-0.1.6/src/untouched/builder.py
--rw-r--r--   0        0        0     2553 2023-07-10 22:32:19.258316 untouched-0.1.6/src/untouched/registry.py
--rw-r--r--   0        0        0     2291 1970-01-01 00:00:00.000000 untouched-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1783 2023-07-10 23:55:50.971863 untouched-0.2.6/README.md
+-rw-r--r--   0        0        0      378 2023-07-11 19:44:52.545666 untouched-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 21:53:14.532163 untouched-0.2.6/src/untouched/__init__.py
+-rw-r--r--   0        0        0     2637 2023-07-10 23:46:39.295971 untouched-0.2.6/src/untouched/builder.py
+-rw-r--r--   0        0        0      623 2023-07-11 19:43:26.031000 untouched-0.2.6/src/untouched/builder.pyi
+-rw-r--r--   0        0        0     2553 2023-07-10 22:32:19.258316 untouched-0.2.6/src/untouched/registry.py
+-rw-r--r--   0        0        0      489 2023-07-11 19:44:05.532353 untouched-0.2.6/src/untouched/registry.pyi
+-rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 untouched-0.2.6/PKG-INFO
```

### Comparing `untouched-0.1.6/README.md` & `untouched-0.2.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -12,61 +12,57 @@
 ```python
 poetry add untouched
 ```
 
 Example:
 
 ```python
-from src.untouched.builder import Builder, get_struct, T
-from src.untouched.registry import Registry
+from  untouched.builder import Builder, get_struct, T
+from untouched.registry import Registry
 from typing import Optional
-from pprint import pprint
 
-registry = Registry()  # Initialize the registry
-
-if __name__ == "__main__":
-    class UserBuilder(Builder):
+NameDBField: str = "name"
+AgeDBField: str = "age"
+class UserQueryBuilder(Builder):
         """
         The UserBuilder class inherits from Builder and provides specific methods to set the 'name' and 'age' attributes.
         """
 
         def __init__(self):
             super().__init__()
 
-        def name(self, val: str) -> 'UserBuilder':
+        def name(self, val: str) -> 'UserQueryBuilder':
             """
             Creates a new UserBuilder with the 'name' attribute set to the provided value.
             """
-            return self.set_value("name", val)
+            return self.set_value(NameDBField, val)
 
-        def age(self, val: int) -> 'UserBuilder':
+        def age(self, val: int) -> 'UserQueryBuilder':
             """
             Creates a new UserBuilder with the 'age' attribute set to the provided value.
             """
-            return self.set_value("age", val)
+            return self.set_value(AgeDBField, val)
 
 
-    class User:
+class User:
         """
         The User class represents the structure that the UserBuilder will build.
         """
 
         def __init__(self, name: Optional[str] = None, age: Optional[int] = None):
             self.name = name
             self.age = age
 
-
-    # Register the builder-struct pair
-    registry.register(UserBuilder(), User())
-    user_builder = UserBuilder().name("caner").age(25).name("caner2")  # Build a user
-    user = user_builder.get_builder_map()
-    pprint(user.__dict__)  # Print the user struct's attributes
+registry = Registry()
+registry.register(UserQueryBuilder(), User())
+user_builder = UserQueryBuilder().name("caner").age(25)
+print(user_builder.get_builder_map())
 
 
 # Output:
 # 
-# {'age': 25, 'name': 'caner2'}
+# {'age': 25, 'name': 'caner'}
 ```
 
 Thanks a lot to Lann for the original builder package, this is wonderful.
 
 Not a perfect copy of the library, yet it works! Which is, what python is right? It is fast enough, and it works.
```

### Comparing `untouched-0.1.6/src/untouched/builder.py` & `untouched-0.2.6/src/untouched/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import collections.abc
 from typing import Any, Dict, Optional, TypeVar
 
-# import registry with most certain way possible
 from .registry import Registry
 
 # any subclass of Builder will be able to use the methods defined in Builder, or the methods defined in its subclasses
 T = TypeVar('T', bound='Builder')
 
 
 class Builder:
```

### Comparing `untouched-0.1.6/src/untouched/registry.py` & `untouched-0.2.6/src/untouched/registry.py`

 * *Files identical despite different names*

### Comparing `untouched-0.1.6/PKG-INFO` & `untouched-0.2.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untouched
-Version: 0.1.6
+Version: 0.2.6
 Summary: Immutable builder, carbon copy of lann/builder package in GoLang.
 Author: damacaner
 Author-email: caner@damacana.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -23,61 +23,57 @@
 ```python
 poetry add untouched
 ```
 
 Example:
 
 ```python
-from src.untouched.builder import Builder, get_struct, T
-from src.untouched.registry import Registry
+from  untouched.builder import Builder, get_struct, T
+from untouched.registry import Registry
 from typing import Optional
-from pprint import pprint
 
-registry = Registry()  # Initialize the registry
-
-if __name__ == "__main__":
-    class UserBuilder(Builder):
+NameDBField: str = "name"
+AgeDBField: str = "age"
+class UserQueryBuilder(Builder):
         """
         The UserBuilder class inherits from Builder and provides specific methods to set the 'name' and 'age' attributes.
         """
 
         def __init__(self):
             super().__init__()
 
-        def name(self, val: str) -> 'UserBuilder':
+        def name(self, val: str) -> 'UserQueryBuilder':
             """
             Creates a new UserBuilder with the 'name' attribute set to the provided value.
             """
-            return self.set_value("name", val)
+            return self.set_value(NameDBField, val)
 
-        def age(self, val: int) -> 'UserBuilder':
+        def age(self, val: int) -> 'UserQueryBuilder':
             """
             Creates a new UserBuilder with the 'age' attribute set to the provided value.
             """
-            return self.set_value("age", val)
+            return self.set_value(AgeDBField, val)
 
 
-    class User:
+class User:
         """
         The User class represents the structure that the UserBuilder will build.
         """
 
         def __init__(self, name: Optional[str] = None, age: Optional[int] = None):
             self.name = name
             self.age = age
 
-
-    # Register the builder-struct pair
-    registry.register(UserBuilder(), User())
-    user_builder = UserBuilder().name("caner").age(25).name("caner2")  # Build a user
-    user = user_builder.get_builder_map()
-    pprint(user.__dict__)  # Print the user struct's attributes
+registry = Registry()
+registry.register(UserQueryBuilder(), User())
+user_builder = UserQueryBuilder().name("caner").age(25)
+print(user_builder.get_builder_map())
 
 
 # Output:
 # 
-# {'age': 25, 'name': 'caner2'}
+# {'age': 25, 'name': 'caner'}
 ```
 
 Thanks a lot to Lann for the original builder package, this is wonderful.
 
 Not a perfect copy of the library, yet it works! Which is, what python is right? It is fast enough, and it works.
```

