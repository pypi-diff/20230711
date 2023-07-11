# Comparing `tmp/blickfeld_qb2-1.5.3.tar.gz` & `tmp/blickfeld_qb2-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blickfeld_qb2-1.5.3.tar", last modified: Tue Jun 20 10:20:46 2023, max compression
+gzip compressed data, was "blickfeld_qb2-1.6.1.tar", last modified: Tue Jul  4 14:50:04 2023, max compression
```

## Comparing `blickfeld_qb2-1.5.3.tar` & `blickfeld_qb2-1.6.1.tar`

### file list

```diff
@@ -1,124 +1,132 @@
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2745 2023-06-20 10:20:23.000000 blickfeld_qb2-1.5.3/LICENSE.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/PKG-INFO
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      286 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/base/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4372 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/base/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/base/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2420 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/base/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/base/geometry/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2943 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/base/geometry/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/base/grpc/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/base/grpc/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3682 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/base/grpc/channel.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1636 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/base/grpc/device_ca_cert.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      796 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1872 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4181 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    55060 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      295 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/_types.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      101 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/_version.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3543 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/casing.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/compile/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/compile/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6337 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/compile/importing.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      300 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/compile/naming.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     5295 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/grpclib_client.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      910 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/grpclib_server.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/util/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/util/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6793 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/util/async_channel.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/protobuf/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    68012 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     7085 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       23 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)       32 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/__main__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1335 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/compiler.py
--rwxr-xr-x   0 yocto     (1000) yocto     (1000)     1513 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/main.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)    28668 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/models.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     7461 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/parser.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      944 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    12345 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    13059 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/detector/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/detector/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/detector/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1477 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/detector/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/detector/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4015 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/detector/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/hardware/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       43 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/hardware/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/hardware/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      699 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/hardware/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/hardware/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3487 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/hardware/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/laser/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/laser/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/laser/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      635 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/laser/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/laser/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3881 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/laser/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     9203 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3024 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    26328 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_processing/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_processing/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_processing/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6137 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_processing/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_processing/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    16640 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_processing/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      755 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    10428 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/push/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/push/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/push/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2919 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/push/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/push/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2328 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/push/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/blickfeld_qb2/push/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    15032 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/push/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/blickfeld_qb2/system/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/system/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/blickfeld_qb2/system/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    10089 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/system/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/blickfeld_qb2/system/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4591 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/system/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/blickfeld_qb2/system/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    27697 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/system/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2.egg-info/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2023-06-20 10:20:46.000000 blickfeld_qb2-1.5.3/blickfeld_qb2.egg-info/PKG-INFO
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2995 2023-06-20 10:20:46.000000 blickfeld_qb2-1.5.3/blickfeld_qb2.egg-info/SOURCES.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)        1 2023-06-20 10:20:46.000000 blickfeld_qb2-1.5.3/blickfeld_qb2.egg-info/dependency_links.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)       86 2023-06-20 10:20:46.000000 blickfeld_qb2-1.5.3/blickfeld_qb2.egg-info/requires.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)       14 2023-06-20 10:20:46.000000 blickfeld_qb2-1.5.3/blickfeld_qb2.egg-info/top_level.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)       38 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/setup.cfg
--rw-r--r--   0 yocto     (1000) yocto     (1000)      554 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/setup.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2745 2023-07-04 14:49:59.000000 blickfeld_qb2-1.6.1/LICENSE.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/PKG-INFO
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      312 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/base/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4372 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/base/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/base/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2420 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/base/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/base/geometry/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2943 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/base/geometry/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/base/grpc/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/base/grpc/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3682 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/base/grpc/channel.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1636 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/base/grpc/device_ca_cert.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      796 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1045 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4181 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    55060 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      295 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/_types.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      101 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/_version.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3543 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/casing.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/compile/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/compile/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     6337 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/compile/importing.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      300 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/compile/naming.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     5295 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/grpclib_client.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      910 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/grpclib_server.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/util/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/util/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     6793 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/util/async_channel.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/protobuf/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    68012 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     7085 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       23 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       32 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/__main__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1335 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/compiler.py
+-rwxr-xr-x   0 yocto     (1000) yocto     (1000)     1513 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/main.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    28668 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/models.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     7461 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/parser.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1515 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    12345 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    16869 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/detector/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/detector/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/detector/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      746 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/detector/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/detector/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4015 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/detector/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      985 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1935 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     5067 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       43 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      699 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3487 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/laser/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/laser/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/laser/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      635 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/laser/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/laser/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3881 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/laser/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    10016 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3024 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    26328 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     6137 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    16640 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      755 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    10428 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/push/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/push/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/push/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2919 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/push/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/push/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2328 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/push/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/push/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    15032 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/push/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/system/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/system/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/system/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    10089 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/system/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/system/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4591 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/system/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/blickfeld_qb2/system/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    27697 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2/system/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-07-04 14:50:04.930908 blickfeld_qb2-1.6.1/blickfeld_qb2.egg-info/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2.egg-info/PKG-INFO
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3168 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2.egg-info/SOURCES.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        1 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2.egg-info/dependency_links.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       86 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2.egg-info/requires.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       14 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/blickfeld_qb2.egg-info/top_level.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       38 2023-07-04 14:50:04.934908 blickfeld_qb2-1.6.1/setup.cfg
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      554 2023-07-04 14:50:04.000000 blickfeld_qb2-1.6.1/setup.py
```

### Comparing `blickfeld_qb2-1.5.3/LICENSE.txt` & `blickfeld_qb2-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/base/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/base/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/base/data/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/base/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/base/geometry/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/base/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/base/grpc/channel.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/base/grpc/channel.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/base/grpc/device_ca_cert.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/base/grpc/device_ca_cert.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/config/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/data/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/push/data/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,79 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: blickfeld/beam_deflection_control/data/health.proto
+# sources: blickfeld/push/data/health.proto, blickfeld/push/data/status.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
+from datetime import datetime
+from typing import Dict
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
 from ...base import data as __base_data__
 
 
-@dataclass(eq=False, repr=False)
-class Health(betterproto.Message):
-    """
-    Health message containing information about operation, status and error of
-    a beam deflection controller.
-    """
+class StatusConnection(betterproto.Enum):
+    """Connection status of the push"""
 
-    state: "__base_data__.HealthState" = betterproto.enum_field(1)
-    """High-level state of module"""
+    CONNECTION_UNSPECIFIED = 0
+    """unspecified"""
 
-    state_reason: str = betterproto.string_field(2)
-    """Reason for given state. Is not set if state is OK."""
+    CONNECTION_DISABLED = 1
+    """push configuration is disabled"""
+
+    CONNECTION_DISCONNECTED = 2
+    """disconnected from destination"""
+
+    CONNECTION_CONNECTING = 3
+    """connecting to destination"""
+
+    CONNECTION_CONNECTED = 4
+    """connected to destination"""
+
+    CONNECTION_PUSHING = 5
+    """connected to input and destination"""
 
 
 @dataclass(eq=False, repr=False)
-class HealthStats(betterproto.Message):
+class Status(betterproto.Message):
+    """state of a push"""
+
+    sent_messages: int = betterproto.uint32_field(1)
+    """message statistics [default = 0]"""
+
+    connection: "StatusConnection" = betterproto.enum_field(2)
+    """flag to indicate if it is working or not"""
+
+    data_rate: float = betterproto.float_field(3)
     """
-    This message defines the stats that can be retrieved from a beam deflection
-    controller.
+    Average data rate The resulting value is averaged over the last 5 messages
+    sent, peak or current values might be different.
     """
 
-    time: float = betterproto.float_field(1)
-    """Current time in s."""
+    last_message: datetime = betterproto.message_field(4)
+    """Timestamp when last message was sent"""
 
-    bb_frequency: float = betterproto.float_field(2)
-    """Current BB frequency estimation (only set when running BB)."""
+    state: "__base_data__.HealthState" = betterproto.enum_field(5)
+    """State of push connection."""
 
-    max_mechanical_scan_range: float = betterproto.float_field(3)
+    state_reason: str = betterproto.string_field(6)
     """
-    Maximum MSR which occured. Observer q1 in case of CL, sensor atan in case
-    of BB.
+    Reason for the given state. Needs to be set if state is not STATE_OK.
     """
 
-    min_dac_u0: int = betterproto.uint32_field(4)
-    """Minimum DAC value wich occured for piezo 0."""
 
-    max_dac_u0: int = betterproto.uint32_field(5)
-    """Maximum DAC value wich occured for piezo 0."""
+@dataclass(eq=False, repr=False)
+class Health(betterproto.Message):
+    """A health message that contains information about the push status"""
 
-    min_dac_u1: int = betterproto.uint32_field(6)
-    """Minimum DAC value wich occured for piezo 1."""
+    state: "__base_data__.HealthState" = betterproto.enum_field(1)
+    """High-level state of module."""
 
-    max_dac_u1: int = betterproto.uint32_field(7)
-    """Maximum DAC value wich occured for piezo 1."""
+    state_reason: str = betterproto.string_field(2)
+    """
+    Reason for the given state. Needs to be set if state is not STATE_OK.
+    """
 
-    max_cycles: int = betterproto.uint32_field(8)
-    """Maximum amount of cycles needed for control loop."""
+    status: Dict[str, "Status"] = betterproto.map_field(
+        3, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
+    )
+    """map of push status"""
```

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/services/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/beam_deflection_control/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/casing.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/casing.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/compile/importing.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/compile/importing.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/grpclib_client.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/grpclib_client.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/grpclib_server.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/grpclib_server.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/util/async_channel.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/grpc/util/async_channel.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/compiler.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/compiler.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/main.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/main.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/models.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/models.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/parser.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/betterproto/plugin/parser.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/config/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/config/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: blickfeld/core_processing/config/demo_recording.proto
+# sources: blickfeld/hardware/config/identification.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
 
-class DemoRecording(betterproto.Enum):
+@dataclass(eq=False, repr=False)
+class Identification(betterproto.Message):
     """
-    Demo recording which can be replayed instead of the real sensor data. This
-    is also used for virtual devices which have no physical sensing unit.
-    WARNING: The recordings are still preliminary. The demo test data concept
-    will be refactored soon.
+    Identification message of the Qb2 device. It aggregates all hardware
+    components.
     """
 
-    DEMO_RECORDING_UNSPECIFIED = 0
-    """No demo recoding is specified"""
-
-    DEMO_RECORDING_HIGH_RESOLUTION = 1
-    """High resolution recording in the office with 200 + 30 scanlines"""
-
-    DEMO_RECORDING_HIGH_FRAME_RATE = 2
-    """High resolution recording in the office with 30 + 30 scanlines"""
+    serial_number: str = betterproto.string_field(1)
+    """
+    This is the top-level product identification. The serial number will be
+    used as label and API identifier for the device.
+    """
```

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/data/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/services/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/services/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,133 +1,185 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: blickfeld/core_processing/services/acceleration.proto, blickfeld/core_processing/services/health.proto, blickfeld/core_processing/services/point_cloud.proto
+# sources: blickfeld/percept_processing/services/health.proto, blickfeld/percept_processing/services/pipeline.proto, blickfeld/percept_processing/services/point_cloud.proto, blickfeld/percept_processing/services/state_list.proto
 # plugin: python-betterproto
 import asyncio
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     AsyncIterator,
     Dict,
     Iterator,
+    List,
     Optional,
 )
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 import grpclib
 from blickfeld_qb2.betterproto.grpc.grpclib_server import ServiceBase
 
-from .. import (
-    config as _config__,
-    data as _data__,
-)
+from ...core_processing import data as __core_processing_data__
+from ...percept_pipeline import data as __percept_pipeline_data__
+from .. import data as _data__
 
 
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
-class AccelerationStreamResponse(betterproto.Message):
-    """Stream response to acceleration stream request"""
+class StateListStreamRequest(betterproto.Message):
+    """A request to receive a stream of state list messages"""
 
-    buffer: "_data__.AccelerationBuffer" = betterproto.message_field(1)
-    """Buffer with acceleration"""
+    pass
 
 
 @dataclass(eq=False, repr=False)
-class AccelerationGetFilteredResponse(betterproto.Message):
-    """Response to acceleration get filtered request"""
+class StateListStreamResponse(betterproto.Message):
+    """
+    A response for getting a stream of state list messages from the running
+    pipeline
+    """
 
-    acceleration: "_data__.Acceleration" = betterproto.message_field(1)
-    """Single filtered acceleration"""
+    state_list: "_data__.StateList" = betterproto.message_field(1)
+    """
+    The current state list with the information detected in the zones
+    configured in the running pipeline
+    """
 
 
 @dataclass(eq=False, repr=False)
-class HealthGetResponse(betterproto.Message):
-    """Response to health get request"""
+class PipelineStartRequest(betterproto.Message):
+    """A request to start a headless pipeline."""
 
-    health: "_data__.Health" = betterproto.message_field(1)
-    """Health state"""
+    pass
+
+
+@dataclass(eq=False, repr=False)
+class PipelineStartResponse(betterproto.Message):
+    """
+    A response to PipelineStartRequest that contains the list of available
+    streams for the started pipeline.
+    """
+
+    data_types: List["_data__.DataType"] = betterproto.enum_field(1)
+    """List of available streams"""
+
+
+@dataclass(eq=False, repr=False)
+class PipelineListAvailableDataResponse(betterproto.Message):
+    """
+    A response containing the list of the data types available for streaming in
+    the running pipeline
+    """
+
+    data_types: List["_data__.DataType"] = betterproto.enum_field(1)
+    """A list of the data types available for streaming"""
 
 
 @dataclass(eq=False, repr=False)
 class HealthWatchResponse(betterproto.Message):
-    """Stream response to health watch request"""
+    """
+    A response for getting a stream of health messages about the pipeline
+    """
 
     health: "_data__.Health" = betterproto.message_field(1)
-    """Health state"""
+    """
+    The current health message with information about the state of the pipeline
+    """
 
 
 @dataclass(eq=False, repr=False)
-class PointCloudStreamResponse(betterproto.Message):
-    """Stream response to point cloud stream request"""
+class HealthGetResponse(betterproto.Message):
+    """A response for getting an health message about the pipeline"""
 
-    frame: "_data__.Frame" = betterproto.message_field(1)
-    """Point cloud frame"""
+    health: "_data__.Health" = betterproto.message_field(1)
+    """
+    The current health message with information about the state of the pipeline
+    """
 
 
 @dataclass(eq=False, repr=False)
-class PointCloudGetResponse(betterproto.Message):
-    """Response to point cloud get request"""
+class PointCloudStreamRequest(betterproto.Message):
+    """
+    A request to receive a stream of point cloud messages. Different point
+    clouds can be streamed depending on the set fields: - combined point cloud
+    (the full point cloud of all the available devices combined) in the map
+    coordinate system - the foreground of the combined point cloud in the map
+    coordinate system - the complete raw point cloud coming from one device,
+    but only in map coordinate system.
+    """
 
-    frame: "_data__.Frame" = betterproto.message_field(1)
-    """Point cloud frame"""
+    point_cloud_type: "__percept_pipeline_data__.PointCloudType" = (
+        betterproto.enum_field(1)
+    )
+    """The type of point cloud to stream"""
+
+    coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = (
+        betterproto.enum_field(2)
+    )
+    """
+    The coordinate system the point cloud should be expressed in (local or
+    transformed/map)
+    """
+
+    fqdn: str = betterproto.string_field(3, group="point_cloud_source")
+    """fqdn of the data source to get the point cloud from"""
 
 
 @dataclass(eq=False, repr=False)
-class PointCloudEnableDemoRequest(betterproto.Message):
-    """Response to point cloud enable demo request"""
+class PointCloudStreamResponse(betterproto.Message):
+    """A response for getting a stream of point cloud messages"""
 
-    recording: "_config__.DemoRecording" = betterproto.enum_field(1)
-    """Select demo recording"""
+    point_cloud: "__core_processing_data__.Frame" = betterproto.message_field(1)
+    """The required point cloud, based on the fields set in the request"""
 
 
-class Acceleration(betterproto.ServiceStub):
+class StateList(betterproto.ServiceStub):
     """
-    The Acceleration Service provides access to the accelerometer of the
-    device.
+    An RPC service to request a stream of state list messages. If a pipeline is
+    already running, it will be used to stream the data. If no pipeline is
+    running, it will be started first and then the stream will start. NOTE: in
+    this second case, the pipeline will also be automatically stopped once the
+    this second case, the pipeline will also be automatically stopped once
+    there are no more clients requesting any stream type from the module.
     """
 
     async def async_stream(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["AccelerationStreamResponse"]:
+    ) -> AsyncIterator["StateListStreamResponse"]:
         """
-        Streams raw data from accelerometer [WARNING] Raw data is acquired with
-        a high sampling frequency and sent out in larger chunks. To estimate
-        the static state of the device the GetFiltered method should be used.
+        A method to get a stream of state list messages from the pipeline
         """
 
-        request = betterproto_lib_google_protobuf.Empty()
+        request = StateListStreamRequest()
 
         async for response in self._unary_stream(
-            "/blickfeld.core_processing.services.Acceleration/Stream",
+            "/blickfeld.percept_processing.services.StateList/Stream",
             request,
-            AccelerationStreamResponse,
+            StateListStreamResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
     def stream(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["AccelerationStreamResponse"]:
+    ) -> Iterator["StateListStreamResponse"]:
         """
-        Streams raw data from accelerometer [WARNING] Raw data is acquired with
-        a high sampling frequency and sent out in larger chunks. To estimate
-        the static state of the device the GetFiltered method should be used.
+        A method to get a stream of state list messages from the pipeline
         """
 
         loop = asyncio.get_event_loop()
         ait = self.async_stream(
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
@@ -142,192 +194,194 @@
 
         while True:
             done, obj = loop.run_until_complete(get_next())
             if done:
                 break
             yield obj
 
-    async def async_get_filtered(
+
+class Pipeline(betterproto.ServiceStub):
+    """
+    An RPC service to start and stop pipelines. Note that currently it is
+    impossible to run more than one pipeline at the same time.
+    """
+
+    async def async_start(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "AccelerationGetFilteredResponse":
-        """Get filtered sample from accelerometer"""
+    ) -> "PipelineStartResponse":
+        """
+        A method to start a headless pipeline. This means that a pipeline
+        started with this method will only be stopped once the Stop method is
+        explicitly called
+        """
 
-        request = betterproto_lib_google_protobuf.Empty()
+        request = PipelineStartRequest()
 
         return await self._unary_unary(
-            "/blickfeld.core_processing.services.Acceleration/GetFiltered",
+            "/blickfeld.percept_processing.services.Pipeline/Start",
             request,
-            AccelerationGetFilteredResponse,
+            PipelineStartResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get_filtered(
+    def start(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "AccelerationGetFilteredResponse":
-        """Get filtered sample from accelerometer"""
+    ) -> "PipelineStartResponse":
+        """
+        A method to start a headless pipeline. This means that a pipeline
+        started with this method will only be stopped once the Stop method is
+        explicitly called
+        """
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get_filtered(
+            self.async_start(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-
-class Health(betterproto.ServiceStub):
-    """
-    The health service provides methods to monitor operational status of the
-    core_processing module
-    """
-
-    async def async_get(
+    async def async_stop(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health status of the core_processing module"""
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        A method to stop the running pipeline. This will force-stop the
+        pipeline, no matter how the pipeline was created and no matter how many
+        clients are streaming from it.
+        """
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.core_processing.services.Health/Get",
+            "/blickfeld.percept_processing.services.Pipeline/Stop",
             request,
-            HealthGetResponse,
+            betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get(
+    def stop(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health status of the core_processing module"""
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        A method to stop the running pipeline. This will force-stop the
+        pipeline, no matter how the pipeline was created and no matter how many
+        clients are streaming from it.
+        """
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get(
+            self.async_stop(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_watch(
+    async def async_list_available_data(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["HealthWatchResponse"]:
+    ) -> "PipelineListAvailableDataResponse":
         """
-        Can be used to attach to the health monitoring status information of
-        the core_processing module
+        A method to get the list of the data streams available for the running
+        pipeline
         """
 
         request = betterproto_lib_google_protobuf.Empty()
 
-        async for response in self._unary_stream(
-            "/blickfeld.core_processing.services.Health/Watch",
+        return await self._unary_unary(
+            "/blickfeld.percept_processing.services.Pipeline/ListAvailableData",
             request,
-            HealthWatchResponse,
+            PipelineListAvailableDataResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        ):
-            yield response
+        )
 
-    def watch(
+    def list_available_data(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["HealthWatchResponse"]:
+    ) -> "PipelineListAvailableDataResponse":
         """
-        Can be used to attach to the health monitoring status information of
-        the core_processing module
+        A method to get the list of the data streams available for the running
+        pipeline
         """
 
         loop = asyncio.get_event_loop()
-        ait = self.async_watch(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
-
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
+        return loop.run_until_complete(
+            self.async_list_available_data(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
 
-class PointCloud(betterproto.ServiceStub):
+class Health(betterproto.ServiceStub):
     """
-    Point Cloud service for core point cloud stream. It is the direct result of
-    the internal processing pipeline. The output is not post-processed further.
-    The post-processed output can be retrieved from the percept-processing
-    PointCloud service.
+    An RPC service to request information about the state of the pipeline and
+    of the module.
     """
 
-    async def async_stream(
+    async def async_watch(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["PointCloudStreamResponse"]:
+    ) -> AsyncIterator["HealthWatchResponse"]:
         """
-        Stream a point cloud stream NOTE: This activates the sensor if it is
-        currently idle.
+        A method to get a stream of health messages, containing information
+        about the state of the pipeline
         """
 
         request = betterproto_lib_google_protobuf.Empty()
 
         async for response in self._unary_stream(
-            "/blickfeld.core_processing.services.PointCloud/Stream",
+            "/blickfeld.percept_processing.services.Health/Watch",
             request,
-            PointCloudStreamResponse,
+            HealthWatchResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
-    def stream(
+    def watch(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["PointCloudStreamResponse"]:
+    ) -> Iterator["HealthWatchResponse"]:
         """
-        Stream a point cloud stream NOTE: This activates the sensor if it is
-        currently idle.
+        A method to get a stream of health messages, containing information
+        about the state of the pipeline
         """
 
         loop = asyncio.get_event_loop()
-        ait = self.async_stream(
+        ait = self.async_watch(
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ).__aiter__()
 
         async def get_next():
             try:
@@ -343,85 +397,124 @@
             yield obj
 
     async def async_get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "PointCloudGetResponse":
+    ) -> "HealthGetResponse":
         """
-        Get a single point cloud NOTE: This activates the sensor if it is
-        currently idle.
+        A method to get one health message, containing information about the
+        state of the pipeline
         """
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.core_processing.services.PointCloud/Get",
+            "/blickfeld.percept_processing.services.Health/Get",
             request,
-            PointCloudGetResponse,
+            HealthGetResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
     def get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "PointCloudGetResponse":
+    ) -> "HealthGetResponse":
         """
-        Get a single point cloud NOTE: This activates the sensor if it is
-        currently idle.
+        A method to get one health message, containing information about the
+        state of the pipeline
         """
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
             self.async_get(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_enable_demo(
+
+class PointCloud(betterproto.ServiceStub):
+    """
+    An RPC service to request a stream of point cloud messages. If a pipeline
+    is already running, it will be used to stream the data. If no pipeline is
+    running, it will be started first and then the stream will start. NOTE: in
+    this second case, the pipeline will also be automatically stopped once the
+    this second case, the pipeline will also be automatically stopped once
+    there are no more clients requesting any stream type from the module.
+    """
+
+    async def async_stream(
         self,
         *,
-        recording: "_config__.DemoRecording" = 0,
+        point_cloud_type: "__percept_pipeline_data__.PointCloudType" = 0,
+        coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = 0,
+        fqdn: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Enable demo data set It will be re-played on Stream requests"""
+    ) -> AsyncIterator["PointCloudStreamResponse"]:
+        """
+        A method to get a stream of point cloud messages from the pipeline. It
+        is possible to stream different point clouds, depending on the fields
+        set in the request
+        """
 
-        request = PointCloudEnableDemoRequest()
-        request.recording = recording
+        request = PointCloudStreamRequest()
+        request.point_cloud_type = point_cloud_type
+        request.coordinate_system = coordinate_system
+        request.fqdn = fqdn
 
-        return await self._unary_unary(
-            "/blickfeld.core_processing.services.PointCloud/EnableDemo",
+        async for response in self._unary_stream(
+            "/blickfeld.percept_processing.services.PointCloud/Stream",
             request,
-            betterproto_lib_google_protobuf.Empty,
+            PointCloudStreamResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        )
+        ):
+            yield response
 
-    def enable_demo(
+    def stream(
         self,
         *,
-        recording: "_config__.DemoRecording" = 0,
+        point_cloud_type: "__percept_pipeline_data__.PointCloudType" = 0,
+        coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = 0,
+        fqdn: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Enable demo data set It will be re-played on Stream requests"""
+    ) -> Iterator["PointCloudStreamResponse"]:
+        """
+        A method to get a stream of point cloud messages from the pipeline. It
+        is possible to stream different point clouds, depending on the fields
+        set in the request
+        """
 
         loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_enable_demo(
-                recording=recording,
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
+        ait = self.async_stream(
+            point_cloud_type=point_cloud_type,
+            coordinate_system=coordinate_system,
+            fqdn=fqdn,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
```

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/detector/data/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/diagnostics/data/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,66 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: blickfeld/detector/data/health.proto
+# sources: blickfeld/diagnostics/data/self_test_report.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
+from typing import List
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
-from ...base import data as __base_data__
+from .. import config as _config__
 
 
-@dataclass(eq=False, repr=False)
-class Health(betterproto.Message):
+class SelfTestReportResultFlag(betterproto.Enum):
+    """Result flags which indicates if test was sucessful."""
+
+    FLAG_UNSPECIFIED = 0
+    """Unknown result."""
+
+    FLAG_SUCCESS = 1
+    """The test was successful."""
+
+    FLAG_WARNING = 2
     """
-    Health message giving information about operation status and possible
-    errors.
+    The test suceeded but it raised some warnings. Please report if this
+    happens during production and the root-cause is unknown.
     """
 
-    state: "__base_data__.HealthState" = betterproto.enum_field(1)
-    """High-level state of the module."""
-
-    state_reason: str = betterproto.string_field(2)
-    """Reason for given state. Is not set if state is OK."""
+    FLAG_FAILURE = 3
+    """The test failed. The tested module is most probably not functional."""
 
 
 @dataclass(eq=False, repr=False)
-class HealthApd(betterproto.Message):
-    """Current status of APD operation."""
-
-    bias_voltage: float = betterproto.float_field(1)
-    """Current APD bias voltage."""
+class SelfTestReport(betterproto.Message):
+    """Report which contains the results of the selected self tests."""
 
-    temperature_compensation: bool = betterproto.bool_field(2)
+    result_flag: "SelfTestReportResultFlag" = betterproto.enum_field(1)
     """
-    Flag indicating whether temperature compensation is used. If not, static
-    voltage is used.
+    Aggregated result flag which is FLAG_SUCCESS if all tests passed without
+    warnings
     """
 
-    multiplication_factor: int = betterproto.uint32_field(3)
-    """
-    Currently used multiplication factor. Only valid if temperature
-    compensation is used.
-    """
+    results: List["SelfTestReportResult"] = betterproto.message_field(2)
+    """List of test results"""
 
-    temperature: float = betterproto.float_field(4)
+
+@dataclass(eq=False, repr=False)
+class SelfTestReportResult(betterproto.Message):
+    """Result of test."""
+
+    test: "_config__.SelfTest" = betterproto.enum_field(1)
+    """Test case"""
+
+    identifier: str = betterproto.string_field(5)
+    """Unique identifier of test case"""
+
+    flag: "SelfTestReportResultFlag" = betterproto.enum_field(2)
+    """Flag which states test result"""
+
+    reason: str = betterproto.string_field(3)
     """
-    Current temperature measured with dedicated temperature IC which is
-    thermally coupled to the APD.
+    Human-readable reason for test warning or failure. Is not set if test was
+    successful.
     """
+
+    duration: float = betterproto.float_field(4)
+    """Duration of test run"""
```

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/detector/services/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/detector/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/hardware/services/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/hardware/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/laser/data/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/laser/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/laser/services/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/laser/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/config/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,20 +78,43 @@
     synchronized. Recommended in multi-sensor setups. If false: the lidar
     measurements are timestamps with the receive time by the system. The
     receive time is less accurate if the network is not reliable.
     """
 
 
 @dataclass(eq=False, repr=False)
+class DataSourceTrigger(betterproto.Message):
+    """
+    Configuration of Trigger Mode. In trigger mode the processing pipeline will
+    reduce the frequency at which point clouds and state lists are getting
+    computed to reduce the amount of data transmitted between the processing
+    device and configured 'lidars'.
+    """
+
+    frequency: float = betterproto.float_field(1)
+    """
+    The frequency at which data is getting requested from the lidars and
+    outputs are generated.
+    """
+
+
+@dataclass(eq=False, repr=False)
 class DataSourceQb2Setup(betterproto.Message):
     """The configuration of a Qb2 setup of the LiDAR devices"""
 
     lidars: List["DataSourceQb2"] = betterproto.message_field(1)
     """the qb2 lidars to get the point clouds from"""
 
+    trigger: "DataSourceTrigger" = betterproto.message_field(2)
+    """
+    If the field is set trigger mode is enabled. If the field is not set, the
+    pipeline outputs are computed with the frequency of configured lidars, i.e.
+    the scan pattern configured on those.
+    """
+
 
 @dataclass(eq=False, repr=False)
 class ZoneAlgorithm(betterproto.Message):
     """An algorithm that monitors the area within and around a zone."""
 
     name: str = betterproto.string_field(1)
     """The user readable zone algorithm name"""
```

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/data/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/services/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/percept_pipeline/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/percept_processing/data/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/percept_processing/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/data/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/services/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/percept_toolkit/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/push/config/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/push/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/push/data/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/core_processing/config/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,43 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: blickfeld/push/data/health.proto, blickfeld/push/data/status.proto
+# sources: blickfeld/core_processing/config/demo_recording.proto, blickfeld/core_processing/config/point_cloud.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
-from datetime import datetime
-from typing import Dict
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
-from ...base import data as __base_data__
 
+class DemoRecording(betterproto.Enum):
+    """
+    Demo recording which can be replayed instead of the real sensor data. This
+    is also used for virtual devices which have no physical sensing unit.
+    WARNING: The recordings are still preliminary. The demo test data concept
+    will be refactored soon.
+    """
 
-class StatusConnection(betterproto.Enum):
-    """Connection status of the push"""
-
-    CONNECTION_UNSPECIFIED = 0
-    """unspecified"""
-
-    CONNECTION_DISABLED = 1
-    """push configuration is disabled"""
-
-    CONNECTION_DISCONNECTED = 2
-    """disconnected from destination"""
-
-    CONNECTION_CONNECTING = 3
-    """connecting to destination"""
+    DEMO_RECORDING_UNSPECIFIED = 0
+    """No demo recoding is specified"""
 
-    CONNECTION_CONNECTED = 4
-    """connected to destination"""
+    DEMO_RECORDING_HIGH_RESOLUTION = 1
+    """High resolution recording in the office with 200 + 30 scanlines"""
 
-    CONNECTION_PUSHING = 5
-    """connected to input and destination"""
+    DEMO_RECORDING_HIGH_FRAME_RATE = 2
+    """High resolution recording in the office with 30 + 30 scanlines"""
 
 
 @dataclass(eq=False, repr=False)
-class Status(betterproto.Message):
-    """state of a push"""
-
-    sent_messages: int = betterproto.uint32_field(1)
-    """message statistics [default = 0]"""
+class PointCloud(betterproto.Message):
+    """Configuration parameters for the point cloud"""
 
-    connection: "StatusConnection" = betterproto.enum_field(2)
-    """flag to indicate if it is working or not"""
-
-    data_rate: float = betterproto.float_field(3)
-    """
-    Average data rate The resulting value is averaged over the last 5 messages
-    sent, peak or current values might be different.
-    """
-
-    last_message: datetime = betterproto.message_field(4)
-    """Timestamp when last message was sent"""
-
-    state: "__base_data__.HealthState" = betterproto.enum_field(5)
-    """State of push connection."""
-
-    state_reason: str = betterproto.string_field(6)
-    """
-    Reason for the given state. Needs to be set if state is not STATE_OK.
-    """
+    pass
 
 
 @dataclass(eq=False, repr=False)
-class Health(betterproto.Message):
-    """A health message that contains information about the push status"""
+class PointCloudFilter(betterproto.Message):
+    """Filter configuration which can be applied on point cloud frames."""
 
-    state: "__base_data__.HealthState" = betterproto.enum_field(1)
-    """High-level state of module."""
-
-    state_reason: str = betterproto.string_field(2)
+    maximum_returns_per_point: int = betterproto.uint32_field(1)
     """
-    Reason for the given state. Needs to be set if state is not STATE_OK.
+    Set maximum number of returns per point. By default, secondary returns are
+    disabled. Set this, e.g. to 2, to enable secondary returns.
     """
-
-    status: Dict[str, "Status"] = betterproto.map_field(
-        3, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
-    )
-    """map of push status"""
```

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/push/services/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/push/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/system/config/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/system/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/system/data/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/system/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2/system/services/__init__.py` & `blickfeld_qb2-1.6.1/blickfeld_qb2/system/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.3/blickfeld_qb2.egg-info/SOURCES.txt` & `blickfeld_qb2-1.6.1/blickfeld_qb2.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,18 @@
 blickfeld_qb2/core_processing/__init__.py
 blickfeld_qb2/core_processing/config/__init__.py
 blickfeld_qb2/core_processing/data/__init__.py
 blickfeld_qb2/core_processing/services/__init__.py
 blickfeld_qb2/detector/__init__.py
 blickfeld_qb2/detector/data/__init__.py
 blickfeld_qb2/detector/services/__init__.py
+blickfeld_qb2/diagnostics/__init__.py
+blickfeld_qb2/diagnostics/config/__init__.py
+blickfeld_qb2/diagnostics/data/__init__.py
+blickfeld_qb2/diagnostics/services/__init__.py
 blickfeld_qb2/hardware/__init__.py
 blickfeld_qb2/hardware/config/__init__.py
 blickfeld_qb2/hardware/services/__init__.py
 blickfeld_qb2/laser/__init__.py
 blickfeld_qb2/laser/data/__init__.py
 blickfeld_qb2/laser/services/__init__.py
 blickfeld_qb2/percept_pipeline/__init__.py
```

### Comparing `blickfeld_qb2-1.5.3/setup.py` & `blickfeld_qb2-1.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="blickfeld_qb2",
-    version="1.5.3",
+    version="1.6.1",
     author="Blickfeld GmbH",
     author_email="opensource@blickfeld.com",
     url="https://github.com/Blickfeld/blickfeld-qb2",
     description="Python package to communicate securely with Qb2 LiDAR devices of the Blickfeld GmbH",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

