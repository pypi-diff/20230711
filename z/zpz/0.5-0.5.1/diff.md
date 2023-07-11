# Comparing `tmp/zpz-0.5.tar.gz` & `tmp/zpz-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpz-0.5.tar", last modified: Wed May 11 07:09:10 2022, max compression
+gzip compressed data, was "zpz-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `zpz-0.5.tar` & `zpz-0.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1075 2022-01-26 04:20:41.169981 zpz-0.5/LICENSE
--rw-r--r--   0        0        0      756 2022-03-05 06:37:57.492791 zpz-0.5/README.md
--rw-r--r--   0        0        0     1278 2022-05-11 06:53:55.679136 zpz-0.5/pyproject.toml
--rw-r--r--   0        0        0       44 2022-05-11 06:53:58.799074 zpz-0.5/src/zpz/__init__.py
--rw-r--r--   0        0        0      401 2022-05-11 06:53:58.799074 zpz-0.5/src/zpz/async_.py
--rw-r--r--   0        0        0    10419 2022-05-11 06:53:55.679136 zpz-0.5/src/zpz/avro.py
--rw-r--r--   0        0        0      862 2022-05-11 06:53:58.799074 zpz-0.5/src/zpz/datetime.py
--rw-r--r--   0        0        0      615 2022-05-11 07:08:04.098142 zpz-0.5/src/zpz/docker.py
--rw-r--r--   0        0        0      690 2022-05-11 06:53:58.799074 zpz-0.5/src/zpz/infix.py
--rw-r--r--   0        0        0      290 2022-01-26 04:53:41.522411 zpz-0.5/src/zpz/list.py
--rw-r--r--   0        0        0     4184 2022-05-11 06:53:55.679136 zpz-0.5/src/zpz/logging.py
--rw-r--r--   0        0        0     4478 2022-05-11 06:53:58.799074 zpz-0.5/src/zpz/profile.py
--rw-r--r--   0        0        0        0 2020-12-30 05:31:16.109849 zpz-0.5/src/zpz/py.typed
--rw-r--r--   0        0        0       75 2022-02-27 00:01:11.229175 zpz-0.5/src/zpz/text.py
--rw-r--r--   0        0        0     2040 2022-05-11 07:08:36.313497 zpz-0.5/src/zpz/timer.py
--rw-r--r--   0        0        0     1691 1970-01-01 00:00:00.000000 zpz-0.5/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-12-10 03:44:41.232018 zpz-0.5.1/LICENSE
+-rw-r--r--   0        0        0      835 2022-12-10 03:44:41.232018 zpz-0.5.1/README.md
+-rw-r--r--   0        0        0     1228 2023-07-11 05:29:37.687810 zpz-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-07-11 05:34:33.352342 zpz-0.5.1/src/zpz/__init__.py
+-rw-r--r--   0        0        0      374 2022-12-10 03:44:41.242020 zpz-0.5.1/src/zpz/async_.py
+-rw-r--r--   0        0        0    10505 2023-07-11 05:48:37.600041 zpz-0.5.1/src/zpz/avro.py
+-rw-r--r--   0        0        0      862 2022-12-10 03:44:41.242020 zpz-0.5.1/src/zpz/datetime.py
+-rw-r--r--   0        0        0      616 2022-12-10 03:44:41.242020 zpz-0.5.1/src/zpz/docker.py
+-rw-r--r--   0        0        0      691 2023-07-11 05:48:37.600041 zpz-0.5.1/src/zpz/infix.py
+-rw-r--r--   0        0        0      290 2022-12-10 03:44:41.242020 zpz-0.5.1/src/zpz/list.py
+-rw-r--r--   0        0        0     5905 2023-07-11 05:48:37.600041 zpz-0.5.1/src/zpz/logging.py
+-rw-r--r--   0        0        0     4515 2022-12-10 03:44:41.242020 zpz-0.5.1/src/zpz/profile.py
+-rw-r--r--   0        0        0        0 2022-12-10 03:44:41.242020 zpz-0.5.1/src/zpz/py.typed
+-rw-r--r--   0        0        0       75 2022-12-10 03:44:41.242020 zpz-0.5.1/src/zpz/text.py
+-rw-r--r--   0        0        0     2041 2022-12-10 03:44:41.242020 zpz-0.5.1/src/zpz/timer.py
+-rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 zpz-0.5.1/PKG-INFO
```

### Comparing `zpz-0.5/LICENSE` & `zpz-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zpz-0.5/pyproject.toml` & `zpz-0.5.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -32,40 +32,40 @@
     "numpy",
     "snappy",
 ]
 lineprofiler = [
     "line-profiler >=3.0,<4.0",
 ]
 test = [
-    "bandit",
     "coverage[toml]",
-    "flake8",
     "mypy",
-    "pylint",
     "pytest",
+    "ruff",
 ]
 
 
+[tool.flit.module]
+name = "zpz"
+
+[tool.ruff]
+target-version = "py310"
+select = ["E", "F", "I001"]
+ignore = ["E501"]
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["E402", "F401"]
+
+
 [tool.pytest.ini_options]
 minversion = "6.0"
+testpaths = ["tests"]
 addopts = "-sv --log-cli-level info -p no:cacheprovider"
-asyncio_mode = "auto"
 
 
 [tool.coverage.report]
 fail_under = 60
 show_missing = true
 skip_empty = true
 
-
-[tool.pylint.messages_control]
-max-line-length = 88
-disable = [
-    "consider-using-f-string",
-    "missing-docstring",
-    "invalid-name",
-    "line-too-long",
-    "fixme",
-    "too-few-public-methods",
-    "too-many-branches",
-    "too-many-return-statements",
-]
+[tool.coverage.run]
+source = ["zpz"]
+data_file = "/tmp/.coverage"
```

### Comparing `zpz-0.5/src/zpz/avro.py` & `zpz-0.5.1/src/zpz/avro.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 import io
 import json
 import warnings
 import zlib
 from typing import Union
 
-import avro.io
 import avro.datafile
+import avro.io
 import avro.schema
 import numpy
 
-warnings.filterwarnings('ignore', category=DeprecationWarning, module='avro')
+warnings.filterwarnings("ignore", category=DeprecationWarning, module="avro")
 
 
 class BinaryEncoder(avro.io.BinaryEncoder):
     def write_float(self, datum):
         # A `numpy.float32` will call this function and be stored as
         # 4-byte `float` of `C`.
         assert type(datum) is numpy.float32  # pylint: disable=unidiomatic-typecheck
         super().write_float(datum)
 
     def write_double(self, datum):
-        assert type(datum) is float or type(datum) is numpy.float64  # pylint: disable=unidiomatic-typecheck
+        assert (
+            type(datum) is float or type(datum) is numpy.float64
+        )  # pylint: disable=unidiomatic-typecheck
         super().write_double(datum)
 
     def write_int(self, datum):
         # Although Python `int` has unlimited bits,
         # we'll treat it as `int` of `C`, i.e. 4 bytes.
         # If you know the numbers can be large, use `numpy.int64`,
         # which will be treated as `long` of `C`.
         # This `int` is the common `int32`.
         #
         # Python `int` and `numpy.int32` will call this function and be stored
         # as 4-byte `int` of `C`.
-        assert type(datum) is int or type(datum) is numpy.int32  # pylint: disable=unidiomatic-typecheck
+        assert (
+            type(datum) is int or type(datum) is numpy.int32
+        )  # pylint: disable=unidiomatic-typecheck
         assert -2147483648 < datum < 2147483647
         datum = (datum << 1) ^ (datum >> 31)
-        while (datum & ~0x7f) != 0:
-            self.WriteByte((datum & 0x7f) | 0x80)
+        while (datum & ~0x7F) != 0:
+            self.WriteByte((datum & 0x7F) | 0x80)
             datum >>= 7
         self.WriteByte(datum)
 
     # def write_long(self, datum):
     #     super().write_long(datum)
 
 
@@ -52,15 +56,15 @@
     def write_fixed(self, writer_schema, datum, encoder):
         if not isinstance(datum, bytes):
             datum = datum.tobytes()  # works if `datum` is a Numpy object
         super().write_fixed(writer_schema, datum, encoder)
 
 
 class DataFileWriter(avro.datafile.DataFileWriter):
-    def __init__(self, writer, writer_schema=None, codec='null'):
+    def __init__(self, writer, writer_schema=None, codec="null"):
         if isinstance(writer_schema, dict):
             writer_schema = json.dumps(writer_schema)
         if isinstance(writer_schema, str):
             writer_schema = avro.schema.Parse(writer_schema)
         datum_writer = DatumWriter()
         super().__init__(writer, datum_writer, writer_schema, codec)
         self._encoder = BinaryEncoder(writer)
@@ -77,28 +81,28 @@
     # The resultant number will then be put into `numpy` if
     # the schema specifies `pytype` as `numpy`.
 
 
 class DatumReader(avro.io.DatumReader):
     def read_data(self, writer_schema, reader_schema, decoder):
         z = super().read_data(writer_schema, reader_schema, decoder)
-        if writer_schema.props.get('pytype', None) == 'numpy':
-            if writer_schema.type == 'long':
+        if writer_schema.props.get("pytype", None) == "numpy":
+            if writer_schema.type == "long":
                 z = numpy.int64(z)
-            elif writer_schema.type == 'int':
+            elif writer_schema.type == "int":
                 z = numpy.int32(z)
-            elif writer_schema.type == 'double':
+            elif writer_schema.type == "double":
                 z = numpy.float64(z)
-            elif writer_schema.type == 'float':
+            elif writer_schema.type == "float":
                 z = numpy.float32(z)
-            elif writer_schema.type == 'array':
+            elif writer_schema.type == "array":
                 z = numpy.array(z)
-            elif writer_schema.type == 'fixed':
+            elif writer_schema.type == "fixed":
                 assert type(z) is bytes  # pylint: disable=unidiomatic-typecheck
-                dtype = numpy.dtype(writer_schema.props['logical_type'])
+                dtype = numpy.dtype(writer_schema.props["logical_type"])
                 z = numpy.frombuffer(z, dtype)[0]
         return z
 
 
 class DataFileReader(avro.datafile.DataFileReader):
     def __init__(self, reader):  # pylint: disable=super-init-not-called
         # Same as superclass, except for replacing `avro.io.BinaryDecoder`
@@ -109,148 +113,156 @@
         self._datum_decoder = None  # Maybe reset at every block.
         self._datum_reader = DatumReader()
 
         # read the header: magic, meta, sync
         self._read_header()
 
         # ensure codec is valid
-        avro_codec_raw = self.GetMeta('avro.codec')
+        avro_codec_raw = self.GetMeta("avro.codec")
         if avro_codec_raw is None:
             self.codec = "null"
         else:
-            self.codec = avro_codec_raw.decode('utf-8')
+            self.codec = avro_codec_raw.decode("utf-8")
         if self.codec not in avro.datafile.VALID_CODECS:
-            raise avro.datafile.DataFileException(
-                f'Unknown codec: {repr(self.codec)}.')
+            raise avro.datafile.DataFileException(f"Unknown codec: {repr(self.codec)}.")
 
         self._file_length = self._GetInputFileLength()
 
         # get ready to read
         self._block_count = 0
-        self.datum_reader.writer_schema = (avro.schema.Parse(
-            self.GetMeta(avro.datafile.SCHEMA_KEY).decode('utf-8')))
+        self.datum_reader.writer_schema = avro.schema.Parse(
+            self.GetMeta(avro.datafile.SCHEMA_KEY).decode("utf-8")
+        )
 
     def _read_block_header(self):
         # Replace `avro_io.BinaryDecoder` in original implementation
         # by `BinaryDecoder` (our custom version above).
         # No other changes.
 
         self._block_count = self.raw_decoder.read_long()
         if self.codec == "null":
             # Skip a long; we don't need to use the length.
             self.raw_decoder.skip_long()
             self._datum_decoder = self._raw_decoder
-        elif self.codec == 'deflate':
+        elif self.codec == "deflate":
             # Compressed data is stored as (length, data), which
             # corresponds to how the "bytes" type is encoded.
             data = self.raw_decoder.read_bytes()
             # -15 is the log of the window size; negative indicates
             # "raw" (no zlib headers) decompression.  See zlib.h.
             uncompressed = zlib.decompress(data, -15)
             self._datum_decoder = BinaryDecoder(io.BytesIO(uncompressed))
-        elif self.codec == 'snappy':
+        elif self.codec == "snappy":
             import snappy  # pylint: disable=import-outside-toplevel
+
             # Import here b/c we don't expect this to be used.
 
             # Compressed data includes a 4-byte CRC32 checksum
             length = self.raw_decoder.read_long()
             data = self.raw_decoder.read(length - 4)
             uncompressed = snappy.decompress(data)  # pylint: disable=no-member
             self._datum_decoder = BinaryDecoder(io.BytesIO(uncompressed))
             self.raw_decoder.check_crc32(uncompressed)
         else:
-            raise avro.datafile.DataFileException(
-                f"Unknown codec: {repr(self.codec)}")
+            raise avro.datafile.DataFileException(f"Unknown codec: {repr(self.codec)}")
 
 
 def _make_schema(x, name: str) -> Union[str, dict]:
     assert isinstance(name, str)
 
     if isinstance(x, numpy.float32):
-        return {'name': name, 'type': 'float', 'pytype': 'numpy'}
+        return {"name": name, "type": "float", "pytype": "numpy"}
     if isinstance(x, numpy.float64):
-        return {'name': name, 'type': 'double', 'pytype': 'numpy'}
+        return {"name": name, "type": "double", "pytype": "numpy"}
     if isinstance(x, numpy.int32):
-        return {'name': name, 'type': 'int', 'pytype': 'numpy'}
+        return {"name": name, "type": "int", "pytype": "numpy"}
     if isinstance(x, numpy.int64):
-        return {'name': name, 'type': 'long', 'pytype': 'numpy'}
-    if isinstance(x, (numpy.int8, numpy.int16, numpy.uint8, numpy.uint16,
-                      numpy.uint32, numpy.uint64)):
+        return {"name": name, "type": "long", "pytype": "numpy"}
+    if isinstance(
+        x,
+        (
+            numpy.int8,
+            numpy.int16,
+            numpy.uint8,
+            numpy.uint16,
+            numpy.uint32,
+            numpy.uint64,
+        ),
+    ):
         return {
-            'name': name,
-            'type': 'fixed',
-            'size': x.itemsize,
-            'pytype': 'numpy',
-            'logical_type': x.dtype.name
+            "name": name,
+            "type": "fixed",
+            "size": x.itemsize,
+            "pytype": "numpy",
+            "logical_type": x.dtype.name,
         }
     if isinstance(x, numpy.ndarray):
-        assert len(
-            x.shape
-        ) == 1, ("Multi-dimensional Numpy arrays are not supported. "
-                 "Please convert to a 1-D Numpy array "
-                 "and store it dimensionality info as another datum")
-        z = _make_schema(x.dtype.type(), name + '_item')
-        return {'name': name, 'type': 'array', 'items': z, 'pytype': 'numpy'}
+        assert len(x.shape) == 1, (
+            "Multi-dimensional Numpy arrays are not supported. "
+            "Please convert to a 1-D Numpy array "
+            "and store it dimensionality info as another datum"
+        )
+        z = _make_schema(x.dtype.type(), name + "_item")
+        return {"name": name, "type": "array", "items": z, "pytype": "numpy"}
 
     if isinstance(x, int):
-        return {'name': name, 'type': "int"}
+        return {"name": name, "type": "int"}
     if isinstance(x, float):
-        return {'name': name, 'type': 'double'}
+        return {"name": name, "type": "double"}
     if isinstance(x, str):
-        return {'name': name, 'type': 'string'}
+        return {"name": name, "type": "string"}
     if isinstance(x, dict):
         fields = []
         for key, val in x.items():
             z = _make_schema(val, key)
             if len(z) < 3:
                 fields.append(z)
             else:
-                fields.append({'name': key, 'type': z})
-        return {'name': name, 'type': 'record', 'fields': fields}
+                fields.append({"name": key, "type": z})
+        return {"name": name, "type": "record", "fields": fields}
     if isinstance(x, list):
-        assert len(x) > 0, \
-            ("empty list is not supported, "
-             "because its type can not be inferred")
-        z0 = _make_schema(x[0], name + '_item')
+        assert len(x) > 0, (
+            "empty list is not supported, " "because its type can not be inferred"
+        )
+        z0 = _make_schema(x[0], name + "_item")
         if len(x) > 1:
             for v in x[1:]:
-                z1 = _make_schema(v, name + '_item')
-                assert z1 == z0, f'schema for x[0] ({x[0]}): {z0}; schema for x[?] ({v}): {z1}'
+                z1 = _make_schema(v, name + "_item")
+                assert (
+                    z1 == z0
+                ), f"schema for x[0] ({x[0]}): {z0}; schema for x[?] ({v}): {z1}"
         if len(z0) < 3:
-            items = z0['type']
+            items = z0["type"]
         else:
             items = z0
-        return {'name': name, 'type': 'array', 'items': items}
+        return {"name": name, "type": "array", "items": items}
 
     raise Exception('unrecognized value of type "' + type(x).__name__ + '"')
 
 
-def make_schema(value, name: str,
-                namespace: str) -> str:
-    '''
+def make_schema(value, name: str, namespace: str) -> str:
+    """
     `value` is a `dict` whose members are either 'simple types' or 'compound types'.
 
     'simple types' include:
         int, float, str (python types)
         numpy.{int8, int16, int32, int64, uint8, uint16, uint32, uint64, float32, float64}  (numpy types)  # noqa: E501
 
     'compound types' include:
         dict: whose elements are simple or compound types
         list: whose elements are all the same simple or compound type
         numpy.ndarray: must be 1-d, with `dtype` being one of the numpy 'simple' type.  # noqa: E501
-    '''
-    sch = {'namespace': namespace, **_make_schema(value, name)}
+    """
+    sch = {"namespace": namespace, **_make_schema(value, name)}
     return json.dumps(sch)
 
 
 # Using `DataFileWriter` instead of the barebone `DatumWriter`,
 # the schema is included in the resultant byte array.
-def dump_bytes(value,
-               name: str,
-               namespace: str) -> bytes:
+def dump_bytes(value, name: str, namespace: str) -> bytes:
     schema = make_schema(value, name, namespace)
     buffer = io.BytesIO()
     with DataFileWriter(buffer, schema) as writer:
         writer.append(value)
         writer.flush()
         buffer.seek(0)
         return buffer.getvalue()
@@ -259,10 +271,10 @@
 def load_bytes(b: bytes, return_schema=False):
     with DataFileReader(io.BytesIO(b)) as reader:
         # We know the stream contains only one record.
         value = list(reader)
         if len(value) == 1:
             value = value[0]
         if return_schema:
-            schema = reader.meta['avro.schema'].decode()
+            schema = reader.meta["avro.schema"].decode()
             return value, schema
         return value
```

### Comparing `zpz-0.5/src/zpz/datetime.py` & `zpz-0.5.1/src/zpz/datetime.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,25 +11,25 @@
         tzname: the ISO standard timezone name,
         such as ``Africa/Cairo``, ``America/Los_Angeles``.
     """
     return datetime.now(timezone(tzname))
 
 
 def pacificnow():
-    return tznow('America/Los_Angeles')
+    return tznow("America/Los_Angeles")
 
 
 def make_timestamp() -> str:
-    '''
+    """
     This function creates a timestamp string with fixed format like
 
         '2020-08-22T08:09:13.401346'
 
     Strings created by this function can be compared to
     determine time order. There is no need to parse the string
     into `datetime` objects.
 
     The returned string is often written as a timestamp file, like
 
         open(file_name, 'w').write(make_timestamp())
-    '''
-    return datetime.utcnow().isoformat(timespec='microseconds')
+    """
+    return datetime.utcnow().isoformat(timespec="microseconds")
```

### Comparing `zpz-0.5/src/zpz/docker.py` & `zpz-0.5.1/src/zpz/docker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import subprocess
 
 
 def get_host_ip():
-    '''
+    """
     Get the IP address of the host machine from within a Docker container.
-    '''
+    """
     # INTERNAL_HOST_IP=$(ip route show default | awk '/default/ {print $3})')
     # another idea:
     # ip -4 route list match 0/0 | cut -d' ' -f3
     #
     # Usually the result is '172.17.0.1'
     # This is the "loopback" address used in code to connect to the host machine.
     # In most documentation this is said to be '127.0.0.1'.
 
-    z = subprocess.check_output(['ip', '-4', 'route', 'list', 'match', '0/0'])
-    z = z.decode()[len('default via '):]
-    return z[: z.find(' ')]
+    z = subprocess.check_output(["ip", "-4", "route", "list", "match", "0/0"])
+    z = z.decode()[len("default via ") :]
+    return z[: z.find(" ")]
```

### Comparing `zpz-0.5/src/zpz/infix.py` & `zpz-0.5.1/src/zpz/infix.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-'''
+"""
 This is a small Python language exercise.
 Recommendation for practical use of this decorator is not implied.
-'''
+"""
 
 import functools
-from typing import Callable, Any
+from typing import Any, Callable
 
 
 class Infix:
-    '''
+    """
     Suppose we have
 
         @Infix
         def func(x, y):
             return ...
 
     Then,
 
         x |func| y
 
     is equivalent to
 
         func(x, y)
-    '''
+    """
+
     def __init__(self, function: Callable[[Any, Any], Any]):
         self.function = function
 
     def __ror__(self, other):
         return Infix(functools.partial(self.function, other))
 
     def __or__(self, other):
```

### Comparing `zpz-0.5/src/zpz/profile.py` & `zpz-0.5.1/src/zpz/profile.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import pstats
 import warnings
 from functools import wraps
 from io import StringIO
 from typing import Callable
 
 
-def profiled(top: int = 32, sort_by: str = None,
-             prof_file: str = None) -> Callable[[Callable], Callable]:
+def profiled(
+    top: int = 32, sort_by: str = None, prof_file: str = None
+) -> Callable[[Callable], Callable]:
     """
     Print out profiling info for a test function,
     and optionally dump the profile result in specified file
     for later inspection.
 
     Args:
         top: number of top items to print.
@@ -41,56 +42,61 @@
                 ...
 
             do_it()
 
     """
 
     if sort_by is None:
-        sort_by = ['cumtime', 'tottime']
+        sort_by = ["cumtime", "tottime"]
 
     if isinstance(sort_by, str):
         sort_by = [sort_by]
 
     if prof_file is None:
-        prof_file = 'cprofile.out'
+        prof_file = "cprofile.out"
 
     def mydecorator(func):
         @wraps(func)
         def profiled_func(*args, **kwargs):
             profile = cProfile.Profile()
             profile.enable()
             result = func(*args, **kwargs)
             profile.disable()
 
             for sb in sort_by:
                 s = StringIO()
                 pstats.Stats(profile, stream=s).sort_stats(sb).print_stats(top)
-                print('')
+                print("")
                 print(s.getvalue())
 
             if prof_file:
                 profile.dump_stats(prof_file)
-                print('')
-                print('profiling results are saved in', prof_file,
-                      '; view its content using `snakeviz`')
+                print("")
+                print(
+                    "profiling results are saved in",
+                    prof_file,
+                    "; view its content using `snakeviz`",
+                )
 
             return result
 
         return profiled_func
 
     return mydecorator
 
 
 try:
     import line_profiler
 except ImportError:
     pass
 else:
 
-    def lineprofiled(*funcs) -> Callable[[Callable], Callable]:  # pylint: disable=unused-argument
+    def lineprofiled(
+        *funcs,
+    ) -> Callable[[Callable], Callable]:  # pylint: disable=unused-argument
         """
         A line-profiling decorator.
 
         Args:
             funcs: functions (function objects, not function names)
                 to be line-profiled. If no function is specified,
                 the function being decorated is profiled.
@@ -132,20 +138,20 @@
                             func_names.remove(key[-1])
                             if not func_names:
                                 break
                 if func_names:
                     # Force warnings.warn() to omit the source code line
                     # in the message
                     formatwarning_orig = warnings.formatwarning
-                    warnings.formatwarning = (
-                        lambda message, category, filename, lineno, line=None:
-                            formatwarning_orig(
-                                message, category,
-                                filename, lineno, line='',
-                            )
+                    warnings.formatwarning = lambda message, category, filename, lineno, line=None: formatwarning_orig(
+                        message,
+                        category,
+                        filename,
+                        lineno,
+                        line="",
                     )
                     warnings.warn("No profile stats for %s." % str(func_names))
                     # Restore warning formatting.
                     warnings.formatwarning = formatwarning_orig
 
                 return z
```

### Comparing `zpz-0.5/src/zpz/timer.py` & `zpz-0.5.1/src/zpz/timer.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,58 +7,59 @@
 
 def humanize(seconds: float) -> List[str]:
     msg = []
     if seconds >= 3600:
         hours, seconds = divmod(seconds, 3600)
         hours = int(hours)
         if hours < 2:
-            msg.append(f'{hours} hour')
+            msg.append(f"{hours} hour")
         else:
-            msg.append(f'{hours} hours')
+            msg.append(f"{hours} hours")
     if seconds >= 60:
         minutes, seconds = divmod(seconds, 60)
         minutes = int(minutes)
         if minutes < 2:
-            msg.append(f'{minutes} minute')
+            msg.append(f"{minutes} minute")
         else:
-            msg.append(f'{minutes} minutes')
-    msg.append(f'{round(seconds, 4)} seconds')
+            msg.append(f"{minutes} minutes")
+    msg.append(f"{round(seconds, 4)} seconds")
     return msg
 
 
 def timed(print_func: Callable = None) -> Callable:
-    '''
+    """
     Usage 1:
 
         @timed()
         def myfunc(...):
             ...
 
     Usage 2:
 
         import logging
         logger = logging.getLogger(__name__)
 
         @timed(logger.info)
         def myfunc(...):
             ...
-    '''
+    """
     if print_func is None:
+
         def print_func(text):
             print(text, file=sys.stderr)
 
     def decorator(func: Callable) -> Callable:
         @wraps(func)
         def profiled_func(*args, **kwargs):
-            print_func(f'Starting function `{func.__name__}`')
+            print_func(f"Starting function `{func.__name__}`")
             t0 = time.monotonic()
             result = func(*args, **kwargs)
-            duration = ', '.join(humanize(time.monotonic() - t0))
-            print_func(f'Finishing function `{func.__name__}`')
-            print_func(f'Function `{func.__name__}` took {duration} to finish')
+            duration = ", ".join(humanize(time.monotonic() - t0))
+            print_func(f"Finishing function `{func.__name__}`")
+            print_func(f"Function `{func.__name__}` took {duration} to finish")
             return result
 
         return profiled_func
 
     return decorator
 
 
@@ -67,19 +68,19 @@
     z = func(*args, **kwargs)
     seconds = time.monotonic() - t0
     return z, seconds
 
 
 @contextmanager
 def timer(msg: str):
-    '''
+    """
     Time a code block:
 
         with timer('my block'):
             x = 3
             y = 4
             ...
-    '''
+    """
     t0 = time.monotonic()
     yield
     t1 = time.monotonic()
     print(f"{msg}: {humanize(t1 - t0)}")
```

