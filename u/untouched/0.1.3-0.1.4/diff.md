# Comparing `tmp/untouched-0.1.3.tar.gz` & `tmp/untouched-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "untouched-0.1.3.tar", max compression
+gzip compressed data, was "untouched-0.1.4.tar", max compression
```

## Comparing `untouched-0.1.3.tar` & `untouched-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1752 2023-07-10 22:20:04.888883 untouched-0.1.3/README.md
--rw-r--r--   0        0        0      378 2023-07-10 22:21:11.703287 untouched-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 21:53:14.532163 untouched-0.1.3/src/untouched/__init__.py
--rw-r--r--   0        0        0     4011 2023-07-10 22:20:04.893883 untouched-0.1.3/src/untouched/builder.py
--rw-r--r--   0        0        0      340 2023-07-10 20:48:13.143480 untouched-0.1.3/src/untouched/reflect.py
--rw-r--r--   0        0        0     2561 2023-07-10 22:20:04.879883 untouched-0.1.3/src/untouched/registry.py
--rw-r--r--   0        0        0     2101 1970-01-01 00:00:00.000000 untouched-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1741 2023-07-10 22:24:21.631433 untouched-0.1.4/README.md
+-rw-r--r--   0        0        0      378 2023-07-10 22:32:40.604445 untouched-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 21:53:14.532163 untouched-0.1.4/src/untouched/__init__.py
+-rw-r--r--   0        0        0     3998 2023-07-10 22:32:19.254316 untouched-0.1.4/src/untouched/builder.py
+-rw-r--r--   0        0        0      340 2023-07-10 20:48:13.143480 untouched-0.1.4/src/untouched/reflect.py
+-rw-r--r--   0        0        0     2553 2023-07-10 22:32:19.258316 untouched-0.1.4/src/untouched/registry.py
+-rw-r--r--   0        0        0     2090 1970-01-01 00:00:00.000000 untouched-0.1.4/PKG-INFO
```

### Comparing `untouched-0.1.3/README.md` & `untouched-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# builder
+# Untouched
 
-https://pypi.org/project/immutable-builder/
+https://pypi.org/project/untouched/
 
 Carbon copy of https://github.com/lann/builder for making a Python NoSQL query builder.
 
 Installing:
 ```python
-poetry add immutable-builder 
+poetry add untouched
 ```
 
 Example:
 
 ```python
-from i
+from ?????
 from pprint import pprint
 from typing import Optional
 
 class UserBuilder(Builder):
         """
         The UserBuilder class inherits from Builder and provides specific methods to set the 'name' and 'age' attributes.
         """
```

### Comparing `untouched-0.1.3/src/untouched/builder.py` & `untouched-0.1.4/src/untouched/builder.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,54 +31,54 @@
 
 
 
 def delete_value(builder: Builder, name: str) -> Builder:
     """
     Creates a new Builder with the specified attribute removed.
     """
-    new_builder = type(builder)()  # Create a new instance of the same type as untouched, to avoid inheritance issues
+    new_builder = type(builder)()  # Create a new instance of the same type as builder, to avoid inheritance issues
     new_builder.builder_map = builder.get_builder_map().copy()
     new_builder.builder_map.pop(name, None)
     return new_builder
 
 
 def extend(builder: Builder, name: str, vs: Any) -> Builder:
     """
     Creates a new Builder with the specified attribute extended with the provided iterable.
     """
     if vs is None:
         return builder
 
-    new_builder = type(builder)()  # Create a new instance of the same type as untouched, to avoid inheritance issues
+    new_builder = type(builder)()  # Create a new instance of the same type as builder, to avoid inheritance issues
     new_builder.builder_map = builder.get_builder_map().copy()
 
     if not isinstance(vs, collections.abc.Iterable):
         raise TypeError("Expected an iterable value.")
 
     new_builder.builder_map[name] = list(vs)
     return new_builder
 
 
 def get_value(builder: Builder, name: str) -> Optional[Any]:
     """
-    Returns the value for the specified attribute from the untouched's map.
+    Returns the value for the specified attribute from the immutable's map.
     """
     return builder.get_builder_map().get(name)
 
 
 def get_map(builder: Builder) -> Dict[str, Any]:
     """
-    Returns a copy of the untouched's map.
+    Returns a copy of the builders map.
     """
     return builder.get_builder_map().copy()
 
 
 def get_struct(builder: Builder) -> Any:
     """
-    Converts the untouched's map into the corresponding struct object.
+    Converts the builder's map into the corresponding struct object.
     """
     builder_type = type(builder)
     struct_type = registry.get_builder_struct_type(builder_type)
     if struct_type is None:
         return None
 
     new_struct = registry.new_builder_struct(builder_type)
@@ -120,12 +120,12 @@
         """
 
         def __init__(self, name: Optional[str] = None, age: Optional[int] = None):
             self.name = name
             self.age = age
 
 
-    # Register the untouched-struct pair
+    # Register the builder-struct pair
     registry.register(UserBuilder(), User())
     user_builder = UserBuilder().name("caner").age(25).name("caner2")  # Build a user
-    user = get_struct(user_builder)  # Convert the untouched to a struct
+    user = get_struct(user_builder)  # Convert the builder to a struct
     pprint(user.__dict__)  # Print the user struct's attributes
```

### Comparing `untouched-0.1.3/src/untouched/registry.py` & `untouched-0.1.4/src/untouched/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         # The registry dictionary stores the mapping of Builder types to their corresponding struct types.
         self.registry = dict()
 
         # We use a Lock object to ensure that updates to the registry are thread-safe.
         # This is necessary when you have multiple threads that might be trying to update the registry at the same time.
         self.registry_lock = Lock()
 
-    # The register_type method is used to register a mapping from a untouched type to a struct type.
+    # The register_type method is used to register a mapping from a builder type to a struct type.
     def register_type(self, builder_type: Type[Any], struct_type: Type[Any]) -> Any:
         # We use a context manager (the "with" statement) to ensure that the lock is properly acquired and released,
         # even if an error occurs within the block of code.
         with self.registry_lock:
             # This check ensures that the provided struct_type is indeed a class.
             if not isinstance(struct_type, type):
                 raise ValueError(
@@ -25,27 +25,27 @@
 
             # If struct_type is valid, we add the mapping from builder_type to struct_type to our registry dictionary.
             self.registry[builder_type] = struct_type
 
             # Create and return a new instance of the builder_type.
             return builder_type()
 
-    # This method is a convenience function for registering a untouched and struct instance,
+    # This method is a convenience function for registering a builder and struct instance,
     # rather than their types.
     def register(self, builder_proto: Any, struct_proto: Any) -> Any:
         return self.register_type(type(builder_proto), type(struct_proto))
 
-    # This method retrieves the struct type associated with a given untouched type.
+    # This method retrieves the struct type associated with a given builder type.
     def get_builder_struct_type(self, builder_type: Type[Any]) -> Type[Any]:
         with self.registry_lock:
             # Get the struct_type from the registry dictionary, or None if it does not exist.
             struct_type = self.registry.get(builder_type)
             return struct_type
 
-    # This method creates a new instance of the struct type associated with a given untouched type.
+    # This method creates a new instance of the struct type associated with a given builder type.
     def new_builder_struct(self, builder_type: Type[Any]) -> Any:
         struct_type = self.get_builder_struct_type(builder_type)
         if struct_type is None:
             return None
 
         # Create and return a new instance of the struct_type.
         new_struct = struct_type()
```

### Comparing `untouched-0.1.3/PKG-INFO` & `untouched-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: untouched
-Version: 0.1.3
+Version: 0.1.4
 Summary: Immutable builder, carbon copy of lann/builder package in GoLang.
 Author: damacaner
 Author-email: caner@damacana.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
-# builder
+# Untouched
 
-https://pypi.org/project/immutable-builder/
+https://pypi.org/project/untouched/
 
 Carbon copy of https://github.com/lann/builder for making a Python NoSQL query builder.
 
 Installing:
 ```python
-poetry add immutable-builder 
+poetry add untouched
 ```
 
 Example:
 
 ```python
-from i
+from ?????
 from pprint import pprint
 from typing import Optional
 
 class UserBuilder(Builder):
         """
         The UserBuilder class inherits from Builder and provides specific methods to set the 'name' and 'age' attributes.
         """
```

