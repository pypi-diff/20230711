# Comparing `tmp/ctdd-0.0.3.tar.gz` & `tmp/ctdd-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctdd-0.0.3.tar", max compression
+gzip compressed data, was "ctdd-0.0.4.tar", max compression
```

## Comparing `ctdd-0.0.3.tar` & `ctdd-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 ctdd-0.0.3/LICENSE
--rw-r--r--   0        0        0     2025 2023-05-08 01:05:44.511002 ctdd-0.0.3/README.md
--rw-r--r--   0        0        0       65 2023-05-13 15:01:41.630543 ctdd-0.0.3/ctdd/__init__.py
--rw-r--r--   0        0        0     3075 2023-05-13 14:24:30.101636 ctdd-0.0.3/ctdd/__main__.py
--rw-r--r--   0        0        0     1167 2023-05-13 15:05:16.441656 ctdd-0.0.3/ctdd/ffi_factory.py
--rw-r--r--   0        0        0     1780 2023-05-13 14:55:04.404025 ctdd-0.0.3/ctdd/mocker.py
--rw-r--r--   0        0        0     2253 2023-05-13 15:00:31.125767 ctdd-0.0.3/ctdd/tester.py
--rw-r--r--   0        0        0     2547 2023-05-14 14:21:18.649983 ctdd-0.0.3/ctdd/tester_state.py
--rw-r--r--   0        0        0      736 2023-05-14 14:28:10.091502 ctdd-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 ctdd-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 ctdd-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2025 2023-05-08 01:05:44.511002 ctdd-0.0.4/README.md
+-rw-r--r--   0        0        0       65 2023-05-13 15:01:41.630543 ctdd-0.0.4/ctdd/__init__.py
+-rw-r--r--   0        0        0     3075 2023-05-13 14:24:30.101636 ctdd-0.0.4/ctdd/__main__.py
+-rw-r--r--   0        0        0     1167 2023-05-13 15:05:16.441656 ctdd-0.0.4/ctdd/ffi_factory.py
+-rw-r--r--   0        0        0     1661 2023-07-09 18:51:45.635857 ctdd-0.0.4/ctdd/mocker.py
+-rw-r--r--   0        0        0     2592 2023-07-11 11:26:17.438280 ctdd-0.0.4/ctdd/tester.py
+-rw-r--r--   0        0        0     2977 2023-07-11 11:28:00.016820 ctdd-0.0.4/ctdd/tester_state.py
+-rw-r--r--   0        0        0      736 2023-07-11 16:41:26.864826 ctdd-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 ctdd-0.0.4/PKG-INFO
```

### Comparing `ctdd-0.0.3/LICENSE` & `ctdd-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.3/README.md` & `ctdd-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.3/ctdd/__main__.py` & `ctdd-0.0.4/ctdd/__main__.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.3/ctdd/ffi_factory.py` & `ctdd-0.0.4/ctdd/ffi_factory.py`

 * *Files identical despite different names*

### Comparing `ctdd-0.0.3/ctdd/mocker.py` & `ctdd-0.0.4/ctdd/mocker.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         ret: object
 
     def __init__(self):
         self.called = {}
 
     def capture_decorator(self, func, key):
         def decorate(*args, **kwargs):
-            print(f'key: {key}')
+            # print(f'capture_decorator key: {key}')
 
             ret = func(*args)
 
             self.called[key].append(Mocker.Call(args, ret))
 
             return ret
         return decorate
@@ -31,41 +31,35 @@
         self.called = {}
 
     def print_all(self):
         for b in self.called:
             print(b, self.called[b])
 
     def get_number_of_calls(self, key):
+        print(f'called: {self.called}')
         if isinstance(key, int):
             if key >= len(self.called):
                 raise ValueError(f'invalid mock id {key}')
         else:
             key = key.__name__
 
             if not key in self.called:
                 raise ValueError(f'invalid mock id {key}')
 
         return len(self.called[key])
 
-def mock_binder(state, binding_point_name, target=None):
+def mock_binder(state, binding_point_name, target=None, rv=None):
+    # print(f'mock_binder {binding_point_name} target {target}')
 
     if target is None:
-        func = lambda *args: None
+        func = lambda *args: rv
         key = len(state.mocker.called)
-    elif isinstance(target, FFI.CData):
-        print('cdata')
-        func = lambda *args: target
-        key = len(state.mocker.called)
-    elif not callable(target):
-        func = lambda *args: target
-        key = len(state.mocker.called)
-    else:
-        print('callable')
+    elif callable(target):
         func = target
-        key = func.__name__
+        key = target.__name__
 
     def_extern_decorator = state.tube._ffi.def_extern(name=binding_point_name)
     def_extern_decorator(state.mocker.capture_decorator(func, key))
 
     binding = getattr(state.tube._lib, binding_point_name)
 
     state.mocker.called[key] = []
```

### Comparing `ctdd-0.0.3/ctdd/tester.py` & `ctdd-0.0.4/ctdd/tester.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 from john import TestCase
 from .tester_state import TesterState
 
 class Tester(TestCase):
     _state = None
     factory = None
+    _source_files = []
 
     @staticmethod
-    def _ensure_state():
+    def _ensure_state(verbose=False):
         if not Tester._state:
-            Tester._state = TesterState('__main__')
+            Tester._state = TesterState('__main__', Tester._source_files, verbose=verbose)
             Tester.factory = Tester._state.factory
 
         return Tester
 
     @staticmethod
     def help():
         Tester._ensure_state()
 
-        print([x for x in dir(Tester) if not x.startswith('_')])
-        print([x for x in dir(Tester._state.factory) if not x.startswith('_')])
+        print(f"Tester: {[x for x in dir(Tester) if not x.startswith('_')]}")
+        print(f"factory: {[x for x in dir(Tester.factory) if not x.startswith('_')]}")
+        print(f"externs: {[x for x in Tester._state.externs if not x.startswith('_')]}")
 
         return Tester
 
     @classmethod
     def tearDownClass(cls) -> None:
         print(f'\r                              ', end='')
         return super().tearDownClass()
 
     @staticmethod
-    def go():
-        Tester._ensure_state().Runner.run()
+    def addSourceFile(filename):
+        Tester._source_files.append(filename)
+        return Tester
+
+    @staticmethod
+    def go(verbose=False):
+        Tester._ensure_state(verbose=verbose).Runner.run()
         return Tester
 
     @property
     def sut(self):
         return Tester._state.ensure_sut()
 
     def __init__(self, method_name:str):
```

### Comparing `ctdd-0.0.3/ctdd/tester_state.py` & `ctdd-0.0.4/ctdd/tester_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 
 def _struct_creator(state, typename):
     struct = state.tube._ffi.new(f'struct {typename} *')
     return struct
 
 class TesterState:
 
-    def __init__(self, module_name: str):
+    def __init__(self, module_name: str, source_files=[], verbose=False):
         self._module_name = module_name
-
+        self._verbose = verbose
         self.factory = FFIFactory()
         self.mocker = Mocker()
         self.externs = []
+        self.source_files = source_files
         self.tube = None
         self.sut = None
 
-        paste = self.create_tube("introspection").squeeze()
+        paste = self.create_tube("introspection").verbose(self._verbose).squeeze()
         if paste is None:
             raise RuntimeError('introspection build failed')
 
         for struct_name in paste.struct_names:
             func = partial(_struct_creator, self, struct_name)
 
             setattr(self.factory, f'{struct_name}', func)
@@ -42,32 +43,36 @@
 
                 function_decl = paste.function_decl(
                     typedef_name, binding_point_name) + ';'
                 self.externs.append(function_decl)
 
                 func = partial(mock_binder, self, binding_point_name)
 
+                print(f'binding {typedef_name} to {binding_point_name}')
+
                 setattr(self.factory, f'{typedef_name}', func)
 
     def create_tube(self, name=None):
         test_case_module = importlib.import_module(self._module_name)
         test_case_filename = test_case_module.__file__
         test_case_name = os.path.splitext(
             os.path.basename(test_case_filename))[0]
 
         c_filename = f'{test_case_name}.c'
         h_filename = f'{test_case_name}.h'
 
         tube_name = name if name else test_case_name
 
         return CrelmFactory().create_Tube(tube_name) \
+            .verbose(self._verbose) \
             .save_compiler_temps() \
             .set_source_folder_relative(test_case_filename) \
             .add_source_file(c_filename) \
             .add_header_file(h_filename) \
+            .add_source_files(self.source_files) \
             .add_externs(self.externs)
 
     def _ensure_tube(self):
         if not self.tube:
             self.sut = None
             self.tube = self.create_tube()
 
@@ -77,9 +82,14 @@
         self._ensure_tube()
 
         if not self.sut:
             self.sut = self.tube.squeeze()
             self.factory._ffi = self.tube._ffi
 
         return self.sut
+    
+    def add_source_file(self, filename):
+        self.source_files.append(filename)
+        print(f'{filename}, {self.source_files}')
+
```

### Comparing `ctdd-0.0.3/pyproject.toml` & `ctdd-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctdd"
-version = "0.0.3"
+version = "0.0.4"
 description = "C test-driven development framework implemented in Python"
 authors = [
   "WideOpenTech <fossie@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ctdd-0.0.3/PKG-INFO` & `ctdd-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctdd
-Version: 0.0.3
+Version: 0.0.4
 Summary: C test-driven development framework implemented in Python
 Home-page: https://github.com/wideopensource/ctdd
 Author: WideOpenTech
 Author-email: fossie@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

