# Comparing `tmp/protosaurus-0.1.0.tar.gz` & `tmp/protosaurus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protosaurus-0.1.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "protosaurus-0.2.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `protosaurus-0.1.0.tar` & `protosaurus-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      175 2022-11-09 12:37:21.000000 protosaurus-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      758 2022-11-09 12:37:21.000000 protosaurus-0.1.0/.github/workflows/pip.yml
--rw-r--r--   0        0        0     1551 2022-11-09 12:37:21.000000 protosaurus-0.1.0/.github/workflows/wheels.yml
--rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 protosaurus-0.1.0/.gitignore
--rw-r--r--   0        0        0     2017 2022-11-09 12:37:21.000000 protosaurus-0.1.0/CMakeLists.txt
--rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 protosaurus-0.1.0/LICENSE
--rw-r--r--   0        0        0     1692 2022-11-09 12:37:21.000000 protosaurus-0.1.0/README.md
--rw-r--r--   0        0        0    36240 2022-11-09 12:37:21.000000 protosaurus-0.1.0/cmake/CPM.cmake
--rw-r--r--   0        0        0     6361 2022-11-09 12:37:21.000000 protosaurus-0.1.0/include/protosaurus/internal/json.h
--rw-r--r--   0        0        0     3031 2022-11-09 12:37:21.000000 protosaurus-0.1.0/include/protosaurus/protosaurus.h
--rw-r--r--   0        0        0      774 2022-11-09 12:37:21.000000 protosaurus-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 protosaurus-0.1.0/src/protosaurus/__init__.py
--rw-r--r--   0        0        0      361 2022-11-09 12:37:21.000000 protosaurus-0.1.0/src/protosaurus_ext.cpp
--rw-r--r--   0        0        0      902 2022-11-09 12:37:21.000000 protosaurus-0.1.0/tests/test_exceptions.py
--rw-r--r--   0        0        0     3587 2022-11-09 12:37:21.000000 protosaurus-0.1.0/tests/test_parsing.py
--rw-r--r--   0        0        0     2036 2022-11-09 12:37:21.000000 protosaurus-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      175 2022-11-09 12:37:21.000000 protosaurus-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 protosaurus-0.2.0/.github/workflows/pip.yml
+-rw-r--r--   0        0        0     1551 2022-11-09 12:37:21.000000 protosaurus-0.2.0/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 protosaurus-0.2.0/.gitignore
+-rw-r--r--   0        0        0     2017 2022-11-09 12:37:21.000000 protosaurus-0.2.0/CMakeLists.txt
+-rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 protosaurus-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1903 2022-11-09 12:37:21.000000 protosaurus-0.2.0/README.md
+-rw-r--r--   0        0        0    36240 2022-11-09 12:37:21.000000 protosaurus-0.2.0/cmake/CPM.cmake
+-rw-r--r--   0        0        0     4029 2022-11-09 12:37:21.000000 protosaurus-0.2.0/include/protosaurus/protosaurus.h
+-rw-r--r--   0        0        0      863 2022-11-09 12:37:21.000000 protosaurus-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 protosaurus-0.2.0/src/protosaurus/__init__.py
+-rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 protosaurus-0.2.0/src/protosaurus_ext.cpp
+-rw-r--r--   0        0        0       97 2022-11-09 12:37:21.000000 protosaurus-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 protosaurus-0.2.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0     5746 2022-11-09 12:37:21.000000 protosaurus-0.2.0/tests/test_parsing.py
+-rw-r--r--   0        0        0     2353 2022-11-09 12:37:21.000000 protosaurus-0.2.0/PKG-INFO
```

### Comparing `protosaurus-0.1.0/.github/workflows/pip.yml` & `protosaurus-0.2.0/.github/workflows/pip.yml`

 * *Files 22% similar despite different names*

```diff
@@ -27,11 +27,11 @@
     - name: Set min macOS version
       if: runner.os == 'macOS'
       run: |
         echo "MACOS_DEPLOYMENT_TARGET=10.14" >> $GITHUB_ENV
 
     - name: Build and install
       run: python -m pip install pytest
-           pip install --verbose .
+           pip install --verbose .[test]
 
     - name: Test
       run: python -m pytest
```

### Comparing `protosaurus-0.1.0/.github/workflows/wheels.yml` & `protosaurus-0.2.0/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `protosaurus-0.1.0/CMakeLists.txt` & `protosaurus-0.2.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `protosaurus-0.1.0/LICENSE` & `protosaurus-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `protosaurus-0.1.0/README.md` & `protosaurus-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Protosaurus
 
-Parse ProtoBuffer messages at runtime.
+Parse and create ProtoBuffer messages at runtime.
 
 [![Pip Action Status][actions-pip-badge]][actions-pip-link]
 [![Wheel Action Status][actions-wheels-badge]][actions-wheels-link]
 [![PyPi][pypi-badge]][pypi-link]
 
 
 [actions-pip-link]:        https://github.com/oberbichler/protosaurus/actions?query=workflow%3APip
@@ -35,28 +35,35 @@
     syntax = "proto3";
     enum Diet {
         carnivorous = 0;
         herbivorous = 1;
     }
     """)
 
-# the specified names can be used for imports (like filenames)
-ctx.add_proto('dino.proto',
+# the proto can be imported via the specified name
+ctx.add_proto('animal.proto',
     """
     syntax = "proto3";
     import "diet.proto";
-    message Dino {
+    message Animal {
         string name = 1;
         Diet diet = 2;
         double length = 3;
     }
     """)
 
 # convert a message from base64 string...
-data = ctx.to_json('Dino', b64decode('CglJZ3Vhbm9kb24QARkAAAAAAAAkQA=='))
+data = ctx.to_json('Animal', b64decode('CglJZ3Vhbm9kb24QARkAAAAAAAAkQA=='))
 
 # ...or hex string
-data = ctx.to_json('Dino', bytes.fromhex('0a09496775616e6f646f6e1001190000000000002440'))
+data = ctx.to_json('Animal', bytes.fromhex('0a09496775616e6f646f6e1001190000000000002440'))
 
 print(data)
-# >>> {"name":"Iguanodon","diet":"herbivorous","length":10}
-```
+# >>> '{"name":"Iguanodon","diet":"herbivorous","length":10}'
+
+
+# convert json to protobuf
+data = ctx.from_json('Animal', json.dumps({"name":"Iguanodon","diet":"herbivorous","length":10}))
+
+print(data)
+# >>> b'\n\tIguanodon\x10\x01\x19\x00\x00\x00\x00\x00\x00$@'
+```
```

### Comparing `protosaurus-0.1.0/cmake/CPM.cmake` & `protosaurus-0.2.0/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `protosaurus-0.1.0/include/protosaurus/protosaurus.h` & `protosaurus-0.2.0/include/protosaurus/protosaurus.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #pragma once
 
-#include "internal/json.h"
-
 #include <protosaurus/protosaurus.h>
 
 #include <nanobind/nanobind.h>
 #include <nanobind/stl/string.h>
 
 #include <google/protobuf/compiler/parser.h>          // Parser
 #include <google/protobuf/descriptor.h>               // DescriptorPool, FileDescriptorProto, FileDescriptor. Descriptor
 #include <google/protobuf/dynamic_message.h>          // DynamicMessageFactory
 #include <google/protobuf/io/tokenizer.h>             // Tokenizer
 #include <google/protobuf/io/zero_copy_stream_impl.h> // ArrayInputStream
 #include <google/protobuf/message.h>                  // Message
+#include <google/protobuf/util/json_util.h>           // MessageToJsonString, 
 
 #include <ios>                                        // boolalpha
 #include <iosfwd>                                     // ostream
 #include <sstream>                                    // stringstream
 #include <stdexcept>                                  // runtime_error
 #include <string>                                     // string
 #include <memory>                                     // unique_ptr
@@ -88,18 +87,54 @@
 
     if (!message->ParseFromArray(data.c_str(), data.size())) {
       throw std::runtime_error("Could not parse value in buffer");
     }
 
     // write json
 
-    std::stringstream out;
+    std::string out;
+
+    absl::Status status = util::MessageToJsonString(*message, &out);
+
+    return out;
+  }
+
+  nb::bytes from_json(std::string message_type, std::string data) {
+    // get descriptor
+
+    const Descriptor* descriptor = m_pool.FindMessageTypeByName(message_type);
+
+    if (descriptor == nullptr) {
+      throw std::runtime_error("Could not find descriptor for message type \"" + message_type + "\"");
+    }
+
+    // generate prototype message
+  
+    DynamicMessageFactory factory;
+
+    const Message* prototype = factory.GetPrototype(descriptor);
+
+    if (prototype == nullptr) {
+      throw std::runtime_error("Could not create prototype");
+    }
+
+    // parse data
+  
+    std::unique_ptr<Message> message(prototype->New());
+
+    if (message == nullptr) {
+      throw std::runtime_error("Could not create empty message from prototype");
+    }
+
+    // write json
+
+    std::string out;
 
-    out << std::boolalpha;
+    absl::Status status = util::JsonStringToMessage(data, message.get());
 
-    internal::push_msg(out, *message);
+    message->SerializeToString(&out);
 
-    return out.str();
+    return nb::bytes(out.c_str(), out.size());
   }
 };
 
 }  // namespace protosaurus
```

### Comparing `protosaurus-0.1.0/pyproject.toml` & `protosaurus-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 [build-system]
 requires = ["scikit-build-core >=0.4.3", "nanobind >=1.3.2"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "protosaurus"
-version = "0.1.0"
+version = "0.2.0"
 description = "Protocol Buffers at runtime"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
     { name = "Thomas Oberbichler", email = "thomas.oberbichler@gmail.com" },
 ]
 classifiers = [
     "License :: OSI Approved :: ISC License (ISCL)",
 ]
 
+[project.optional-dependencies]
+test = [
+  "pytest >=6.0",
+  "deepdiff",
+]
+
 [project.urls]
 Homepage = "https://github.com/oberbichler/protosaurus"
 
 [tool.scikit-build]
 minimum-version = "0.4"
 build-dir = "build/{wheel_tag}"
 wheel.py-api = "cp312"
 
 [tool.cibuildwheel]
 build-verbosity = 1
 test-command = "pytest {project}/tests"
-test-requires = "pytest"
+test-requires = ["pytest", "deepdiff"]
 
 [tool.cibuildwheel.macos.environment]
 MACOSX_DEPLOYMENT_TARGET = "10.14"
-
```

### Comparing `protosaurus-0.1.0/tests/test_exceptions.py` & `protosaurus-0.2.0/tests/test_exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 import pytest
 
-from protosaurus import Context
 from base64 import b64decode
 
 
 if __name__ == "__main__":
     pytest.main()
 
 
-@pytest.fixture
-def ctx():
-    return Context()
-
-
 def test_invalid_proto(ctx):
-    with pytest.raises(RuntimeError):
+    with pytest.raises(RuntimeError, match='Could not parse proto'):
         ctx.add_proto('test',
         """
         syntax = "proto3";
         message test {
             data;
         }
         """)
 
 def test_invalid_message_type(ctx):
-    with pytest.raises(RuntimeError):
+    with pytest.raises(RuntimeError, match='Could not find descriptor for message type "invalid type"'):
         ctx.add_proto('test',
         """
         syntax = "proto3";
         message test {
             bool data = 1;
         }
         """)
 
         ctx.to_json('invalid type', b64decode('CAE='))
 
 def test_invalid_data(ctx):
-    with pytest.raises(RuntimeError):
+    with pytest.raises(RuntimeError, match='Could not parse value in buffer'):
         ctx.add_proto('test',
         """
         syntax = "proto3";
         message test {
             bool data = 1;
         }
         """)
```

### Comparing `protosaurus-0.1.0/PKG-INFO` & `protosaurus-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: protosaurus
-Version: 0.1.0
+Version: 0.2.0
 Summary: Protocol Buffers at runtime
 Author-Email: Thomas Oberbichler <thomas.oberbichler@gmail.com>
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Project-URL: Homepage, https://github.com/oberbichler/protosaurus
 Requires-Python: >=3.8
+Provides-Extra: test
+Requires-Dist: pytest>=6.0; extra == "test"
+Requires-Dist: deepdiff; extra == "test"
 Description-Content-Type: text/markdown
 
 # Protosaurus
 
-Parse ProtoBuffer messages at runtime.
+Parse and create ProtoBuffer messages at runtime.
 
 [![Pip Action Status][actions-pip-badge]][actions-pip-link]
 [![Wheel Action Status][actions-wheels-badge]][actions-wheels-link]
 [![PyPi][pypi-badge]][pypi-link]
 
 
 [actions-pip-link]:        https://github.com/oberbichler/protosaurus/actions?query=workflow%3APip
@@ -45,28 +48,35 @@
     syntax = "proto3";
     enum Diet {
         carnivorous = 0;
         herbivorous = 1;
     }
     """)
 
-# the specified names can be used for imports (like filenames)
-ctx.add_proto('dino.proto',
+# the proto can be imported via the specified name
+ctx.add_proto('animal.proto',
     """
     syntax = "proto3";
     import "diet.proto";
-    message Dino {
+    message Animal {
         string name = 1;
         Diet diet = 2;
         double length = 3;
     }
     """)
 
 # convert a message from base64 string...
-data = ctx.to_json('Dino', b64decode('CglJZ3Vhbm9kb24QARkAAAAAAAAkQA=='))
+data = ctx.to_json('Animal', b64decode('CglJZ3Vhbm9kb24QARkAAAAAAAAkQA=='))
 
 # ...or hex string
-data = ctx.to_json('Dino', bytes.fromhex('0a09496775616e6f646f6e1001190000000000002440'))
+data = ctx.to_json('Animal', bytes.fromhex('0a09496775616e6f646f6e1001190000000000002440'))
 
 print(data)
-# >>> {"name":"Iguanodon","diet":"herbivorous","length":10}
-```
+# >>> '{"name":"Iguanodon","diet":"herbivorous","length":10}'
+
+
+# convert json to protobuf
+data = ctx.from_json('Animal', json.dumps({"name":"Iguanodon","diet":"herbivorous","length":10}))
+
+print(data)
+# >>> b'\n\tIguanodon\x10\x01\x19\x00\x00\x00\x00\x00\x00$@'
+```
```

