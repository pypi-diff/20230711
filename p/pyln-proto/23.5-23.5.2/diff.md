# Comparing `tmp/pyln-proto-23.5.tar.gz` & `tmp/pyln_proto-23.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyln-proto-23.5.tar", max compression
+gzip compressed data, was "pyln_proto-23.5.2.tar", max compression
```

## Comparing `pyln-proto-23.5.tar` & `pyln_proto-23.5.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0      976 2023-05-11 17:43:49.805160 pyln-proto-23.5/README.md
--rw-r--r--   0        0        0      490 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/__init__.py
--rw-r--r--   0        0        0     4698 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/bech32.py
--rwxr-xr-x   0        0        0    15493 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/invoice.py
--rw-r--r--   0        0        0       68 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/message/Makefile
--rw-r--r--   0        0        0      668 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/message/__init__.py
--rw-r--r--   0        0        0     8647 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/message/array_types.py
--rw-r--r--   0        0        0    11192 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/message/fundamental_types.py
--rw-r--r--   0        0        0    27875 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/message/message.py
--rw-r--r--   0        0        0    18733 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/onion.py
--rw-r--r--   0        0        0     4368 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/primitives.py
--rw-r--r--   0        0        0    12025 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/wire.py
--rw-r--r--   0        0        0     3915 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyln/proto/zbase32.py
--rw-r--r--   0        0        0      737 2023-05-11 17:43:49.805160 pyln-proto-23.5/pyproject.toml
--rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 pyln-proto-23.5/setup.py
--rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 pyln-proto-23.5/PKG-INFO
+-rw-r--r--   0        0        0      976 2023-02-24 11:36:08.000000 pyln_proto-23.5.2/README.md
+-rw-r--r--   0        0        0      492 2023-07-11 16:24:27.708292 pyln_proto-23.5.2/pyln/proto/__init__.py
+-rw-r--r--   0        0        0     4698 2023-01-09 11:35:05.000000 pyln_proto-23.5.2/pyln/proto/bech32.py
+-rwxr-xr-x   0        0        0    15493 2023-01-09 11:35:05.000000 pyln_proto-23.5.2/pyln/proto/invoice.py
+-rw-r--r--   0        0        0       68 2022-12-19 12:19:45.000000 pyln_proto-23.5.2/pyln/proto/message/Makefile
+-rw-r--r--   0        0        0      742 2023-07-10 11:09:42.245016 pyln_proto-23.5.2/pyln/proto/message/__init__.py
+-rw-r--r--   0        0        0     8647 2023-01-09 11:35:05.000000 pyln_proto-23.5.2/pyln/proto/message/array_types.py
+-rw-r--r--   0        0        0    11192 2023-05-20 11:18:21.398274 pyln_proto-23.5.2/pyln/proto/message/fundamental_types.py
+-rw-r--r--   0        0        0    27875 2023-02-09 16:02:36.000000 pyln_proto-23.5.2/pyln/proto/message/message.py
+-rw-r--r--   0        0        0    18733 2023-01-09 11:35:05.000000 pyln_proto-23.5.2/pyln/proto/onion.py
+-rw-r--r--   0        0        0     4368 2023-07-10 11:09:42.245016 pyln_proto-23.5.2/pyln/proto/primitives.py
+-rw-r--r--   0        0        0    12025 2023-04-03 14:03:27.000000 pyln_proto-23.5.2/pyln/proto/wire.py
+-rw-r--r--   0        0        0     3915 2023-01-09 11:35:05.000000 pyln_proto-23.5.2/pyln/proto/zbase32.py
+-rw-r--r--   0        0        0      723 2023-07-11 16:24:27.708292 pyln_proto-23.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1957 1970-01-01 00:00:00.000000 pyln_proto-23.5.2/PKG-INFO
```

### Comparing `pyln-proto-23.5/README.md` & `pyln_proto-23.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pyln-proto-23.5/pyln/proto/bech32.py` & `pyln_proto-23.5.2/pyln/proto/bech32.py`

 * *Files identical despite different names*

### Comparing `pyln-proto-23.5/pyln/proto/invoice.py` & `pyln_proto-23.5.2/pyln/proto/invoice.py`

 * *Files identical despite different names*

### Comparing `pyln-proto-23.5/pyln/proto/message/__init__.py` & `pyln_proto-23.5.2/pyln/proto/message/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from .array_types import SizedArrayType, DynamicArrayType, EllipsisArrayType
-from .message import MessageNamespace, MessageType, Message, SubtypeType
+from .message import MessageNamespace, MessageType, Message, SubtypeType, TlvStreamType, TlvMessageType
 from .fundamental_types import split_field, FieldType
 
 __all__ = [
     "MessageNamespace",
     "MessageType",
     "Message",
     "SubtypeType",
     "FieldType",
     "split_field",
     "LengthFieldType",
     "ArrayType",
     "SizedArrayType",
     "DynamicArrayType",
     "EllipsisArrayType",
+    "TlvStreamType",
+    "TlvMessageType",
 
     # fundamental_types
     'byte',
     'u16',
     'u32',
     'u64',
     'tu16',
```

### Comparing `pyln-proto-23.5/pyln/proto/message/array_types.py` & `pyln_proto-23.5.2/pyln/proto/message/array_types.py`

 * *Files identical despite different names*

### Comparing `pyln-proto-23.5/pyln/proto/message/fundamental_types.py` & `pyln_proto-23.5.2/pyln/proto/message/fundamental_types.py`

 * *Files identical despite different names*

### Comparing `pyln-proto-23.5/pyln/proto/message/message.py` & `pyln_proto-23.5.2/pyln/proto/message/message.py`

 * *Files identical despite different names*

### Comparing `pyln-proto-23.5/pyln/proto/onion.py` & `pyln_proto-23.5.2/pyln/proto/onion.py`

 * *Files identical despite different names*

### Comparing `pyln-proto-23.5/pyln/proto/primitives.py` & `pyln_proto-23.5.2/pyln/proto/primitives.py`

 * *Files identical despite different names*

### Comparing `pyln-proto-23.5/pyln/proto/wire.py` & `pyln_proto-23.5.2/pyln/proto/wire.py`

 * *Files identical despite different names*

### Comparing `pyln-proto-23.5/pyln/proto/zbase32.py` & `pyln_proto-23.5.2/pyln/proto/zbase32.py`

 * *Files identical despite different names*

### Comparing `pyln-proto-23.5/pyproject.toml` & `pyln_proto-23.5.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "pyln-proto"
-version = "23.05"
+version = "23.05.2"
 description = "This package implements some of the Lightning Network protocol in pure python. It is intended for protocol testing and some minor tooling only. It is not deemed secure enough to handle any amount of real funds (you have been warned!)."
 authors = ["Christian Decker <decker.christian@gmail.com>"]
 license = "BSD-MIT"
 readme = "README.md"
 
 packages = [
   { include = "pyln/proto" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 base58 = "^2.1.1"
-bitstring = "^3.1.9"
-coincurve = "^17.0.0"
-cryptography = "^36.0.1"
-PySocks = "^1.7.1"
+bitstring = "^3"
+coincurve = "^18"
+cryptography = "^41"
+PySocks = "^1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyln-proto-23.5/setup.py` & `pyln_proto-23.5.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,53 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyln-proto
+Version: 23.5.2
+Summary: This package implements some of the Lightning Network protocol in pure python. It is intended for protocol testing and some minor tooling only. It is not deemed secure enough to handle any amount of real funds (you have been warned!).
+License: BSD-MIT
+Author: Christian Decker
+Author-email: decker.christian@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PySocks (>=1,<2)
+Requires-Dist: base58 (>=2.1.1,<3.0.0)
+Requires-Dist: bitstring (>=3,<4)
+Requires-Dist: coincurve (>=18,<19)
+Requires-Dist: cryptography (>=41,<42)
+Description-Content-Type: text/markdown
+
+# pyln-proto: Lightning Network protocol implementation
+
+This package implements some of the Lightning Network protocol in pure
+python. It is intended for protocol testing and some minor tooling only. It is
+not deemed secure enough to handle any amount of real funds (you have been
+warned!).
+
+
+## Installation
+
+`pyln-proto` is available on `pip`:
+
+```
+pip install pyln-proto
+```
+
+Alternatively you can also install the development version to get access to
+currently unreleased features by checking out the Core Lightning source code and
+installing into your python3 environment:
+
+```bash
+git clone https://github.com/ElementsProject/lightning.git
+cd lightning/contrib/pyln-proto
+poetry install
+```
+
+This will add links to the library into your environment so changing the
+checked out source code will also result in the environment picking up these
+changes. Notice however that unreleased versions may change API without
+warning, so test thoroughly with the released version.
 
-packages = \
-['proto', 'proto.message']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PySocks>=1.7.1,<2.0.0',
- 'base58>=2.1.1,<3.0.0',
- 'bitstring>=3.1.9,<4.0.0',
- 'coincurve>=17.0.0,<18.0.0',
- 'cryptography>=36.0.1,<37.0.0']
-
-setup_kwargs = {
-    'name': 'pyln-proto',
-    'version': '23.5',
-    'description': 'This package implements some of the Lightning Network protocol in pure python. It is intended for protocol testing and some minor tooling only. It is not deemed secure enough to handle any amount of real funds (you have been warned!).',
-    'long_description': '# pyln-proto: Lightning Network protocol implementation\n\nThis package implements some of the Lightning Network protocol in pure\npython. It is intended for protocol testing and some minor tooling only. It is\nnot deemed secure enough to handle any amount of real funds (you have been\nwarned!).\n\n\n## Installation\n\n`pyln-proto` is available on `pip`:\n\n```\npip install pyln-proto\n```\n\nAlternatively you can also install the development version to get access to\ncurrently unreleased features by checking out the Core Lightning source code and\ninstalling into your python3 environment:\n\n```bash\ngit clone https://github.com/ElementsProject/lightning.git\ncd lightning/contrib/pyln-proto\npoetry install\n```\n\nThis will add links to the library into your environment so changing the\nchecked out source code will also result in the environment picking up these\nchanges. Notice however that unreleased versions may change API without\nwarning, so test thoroughly with the released version.\n',
-    'author': 'Christian Decker',
-    'author_email': 'decker.christian@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

