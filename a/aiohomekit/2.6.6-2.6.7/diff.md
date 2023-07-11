# Comparing `tmp/aiohomekit-2.6.6.tar.gz` & `tmp/aiohomekit-2.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohomekit-2.6.6.tar", max compression
+gzip compressed data, was "aiohomekit-2.6.7.tar", max compression
```

## Comparing `aiohomekit-2.6.6.tar` & `aiohomekit-2.6.7.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0    11537 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/LICENSE.md
--rw-r--r--   0        0        0     5841 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/README.md
--rw-r--r--   0        0        0     1867 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/__init__.py
--rw-r--r--   0        0        0    18826 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/__main__.py
--rw-r--r--   0        0        0     4465 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/characteristic_cache.py
--rw-r--r--   0        0        0     1162 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/const.py
--rw-r--r--   0        0        0      697 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/__init__.py
--rw-r--r--   0        0        0    15761 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/abstract.py
--rw-r--r--   0        0        0      704 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/__init__.py
--rw-r--r--   0        0        0     6832 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/bleak.py
--rw-r--r--   0        0        0     7819 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/client.py
--rw-r--r--   0        0        0     2017 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/connection.py
--rw-r--r--   0        0        0     1310 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/const.py
--rw-r--r--   0        0        0     7083 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/controller.py
--rw-r--r--   0        0        0     7614 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/discovery.py
--rw-r--r--   0        0        0     1894 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/key.py
--rw-r--r--   0        0        0     3747 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/manufacturer_data.py
--rw-r--r--   0        0        0    68499 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/pairing.py
--rw-r--r--   0        0        0    11736 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/structs.py
--rw-r--r--   0        0        0     2140 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/values.py
--rw-r--r--   0        0        0      708 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/coap/__init__.py
--rw-r--r--   0        0        0    25692 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/coap/connection.py
--rw-r--r--   0        0        0     1181 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/coap/controller.py
--rw-r--r--   0        0        0     2422 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/coap/discovery.py
--rw-r--r--   0        0        0     9972 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/coap/pairing.py
--rw-r--r--   0        0        0     3431 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/coap/pdu.py
--rw-r--r--   0        0        0    12547 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/coap/structs.py
--rw-r--r--   0        0        0     9288 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/controller.py
--rw-r--r--   0        0        0      757 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/ip/__init__.py
--rw-r--r--   0        0        0    22146 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/ip/connection.py
--rw-r--r--   0        0        0     1119 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/ip/controller.py
--rw-r--r--   0        0        0     4108 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/ip/discovery.py
--rw-r--r--   0        0        0    20914 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/ip/pairing.py
--rw-r--r--   0        0        0      868 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/crypto/__init__.py
--rw-r--r--   0        0        0     4789 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/crypto/chacha20poly1305.py
--rw-r--r--   0        0        0     1036 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/crypto/hkdf.py
--rw-r--r--   0        0        0    10728 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/crypto/srp.py
--rw-r--r--   0        0        0     4060 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/debounce.py
--rw-r--r--   0        0        0      985 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/enum.py
--rw-r--r--   0        0        0     7746 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/exceptions.py
--rw-r--r--   0        0        0     2116 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/hkjson.py
--rw-r--r--   0        0        0     2044 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/http/__init__.py
--rw-r--r--   0        0        0     5265 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/http/response.py
--rw-r--r--   0        0        0     2608 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/meshcop.py
--rw-r--r--   0        0        0    12834 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/__init__.py
--rw-r--r--   0        0        0     1244 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/categories.py
--rw-r--r--   0        0        0     1892 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/__init__.py
--rw-r--r--   0        0        0    14169 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/characteristic.py
--rw-r--r--   0        0        0     1815 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/characteristic_formats.py
--rw-r--r--   0        0        0    22463 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/characteristic_types.py
--rw-r--r--   0        0        0     5238 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/const.py
--rw-r--r--   0        0        0    29366 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/data.py
--rw-r--r--   0        0        0      800 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/permissions.py
--rw-r--r--   0        0        0     4407 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/structs.py
--rw-r--r--   0        0        0      731 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/types.py
--rw-r--r--   0        0        0     1067 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/units.py
--rw-r--r--   0        0        0     1439 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/entity_map.py
--rw-r--r--   0        0        0      722 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/feature_flags.py
--rw-r--r--   0        0        0      685 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/mixin.py
--rw-r--r--   0        0        0      796 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/services/__init__.py
--rw-r--r--   0        0        0    19993 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/services/data.py
--rw-r--r--   0        0        0     5019 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/services/service.py
--rw-r--r--   0        0        0     5380 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/services/service_types.py
--rw-r--r--   0        0        0      703 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/services/types.py
--rw-r--r--   0        0        0      716 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/status_flags.py
--rw-r--r--   0        0        0     4065 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/pdu.py
--rw-r--r--   0        0        0    20539 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/protocol/__init__.py
--rw-r--r--   0        0        0     3493 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/protocol/statuscodes.py
--rw-r--r--   0        0        0     8483 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/protocol/tlv.py
--rw-r--r--   0        0        0        0 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/py.typed
--rw-r--r--   0        0        0    12828 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/testing.py
--rw-r--r--   0        0        0     8265 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/tlv8.py
--rw-r--r--   0        0        0     3581 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/utils.py
--rw-r--r--   0        0        0     1662 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/uuid.py
--rw-r--r--   0        0        0    11606 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/zeroconf.py
--rw-r--r--   0        0        0     1809 2023-07-11 02:04:46.647929 aiohomekit-2.6.6/pyproject.toml
--rw-r--r--   0        0        0     7021 1970-01-01 00:00:00.000000 aiohomekit-2.6.6/PKG-INFO
+-rw-r--r--   0        0        0    11537 2023-07-11 08:13:06.279392 aiohomekit-2.6.7/LICENSE.md
+-rw-r--r--   0        0        0     5841 2023-07-11 08:13:06.279392 aiohomekit-2.6.7/README.md
+-rw-r--r--   0        0        0     1867 2023-07-11 08:13:06.279392 aiohomekit-2.6.7/aiohomekit/__init__.py
+-rw-r--r--   0        0        0    18826 2023-07-11 08:13:06.279392 aiohomekit-2.6.7/aiohomekit/__main__.py
+-rw-r--r--   0        0        0     4465 2023-07-11 08:13:06.279392 aiohomekit-2.6.7/aiohomekit/characteristic_cache.py
+-rw-r--r--   0        0        0     1162 2023-07-11 08:13:06.279392 aiohomekit-2.6.7/aiohomekit/const.py
+-rw-r--r--   0        0        0      697 2023-07-11 08:13:06.279392 aiohomekit-2.6.7/aiohomekit/controller/__init__.py
+-rw-r--r--   0        0        0    15761 2023-07-11 08:13:06.279392 aiohomekit-2.6.7/aiohomekit/controller/abstract.py
+-rw-r--r--   0        0        0      704 2023-07-11 08:13:06.279392 aiohomekit-2.6.7/aiohomekit/controller/ble/__init__.py
+-rw-r--r--   0        0        0     6832 2023-07-11 08:13:06.279392 aiohomekit-2.6.7/aiohomekit/controller/ble/bleak.py
+-rw-r--r--   0        0        0     7819 2023-07-11 08:13:06.279392 aiohomekit-2.6.7/aiohomekit/controller/ble/client.py
+-rw-r--r--   0        0        0     2017 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/ble/connection.py
+-rw-r--r--   0        0        0     1310 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/ble/const.py
+-rw-r--r--   0        0        0     7067 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/ble/controller.py
+-rw-r--r--   0        0        0     7614 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/ble/discovery.py
+-rw-r--r--   0        0        0     1894 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/ble/key.py
+-rw-r--r--   0        0        0     3747 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/ble/manufacturer_data.py
+-rw-r--r--   0        0        0    68499 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/ble/pairing.py
+-rw-r--r--   0        0        0    11736 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/ble/structs.py
+-rw-r--r--   0        0        0     2140 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/ble/values.py
+-rw-r--r--   0        0        0      708 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/coap/__init__.py
+-rw-r--r--   0        0        0    25692 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/coap/connection.py
+-rw-r--r--   0        0        0     1181 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/coap/controller.py
+-rw-r--r--   0        0        0     2422 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/coap/discovery.py
+-rw-r--r--   0        0        0     9972 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/coap/pairing.py
+-rw-r--r--   0        0        0     3431 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/coap/pdu.py
+-rw-r--r--   0        0        0    12547 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/coap/structs.py
+-rw-r--r--   0        0        0     9288 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/controller.py
+-rw-r--r--   0        0        0      757 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/ip/__init__.py
+-rw-r--r--   0        0        0    22146 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/ip/connection.py
+-rw-r--r--   0        0        0     1119 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/ip/controller.py
+-rw-r--r--   0        0        0     4108 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/ip/discovery.py
+-rw-r--r--   0        0        0    20914 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/controller/ip/pairing.py
+-rw-r--r--   0        0        0      868 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/crypto/__init__.py
+-rw-r--r--   0        0        0     4789 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/crypto/chacha20poly1305.py
+-rw-r--r--   0        0        0     1036 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/crypto/hkdf.py
+-rw-r--r--   0        0        0    10728 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/crypto/srp.py
+-rw-r--r--   0        0        0     4060 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/debounce.py
+-rw-r--r--   0        0        0      985 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/enum.py
+-rw-r--r--   0        0        0     7746 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/exceptions.py
+-rw-r--r--   0        0        0     2116 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/hkjson.py
+-rw-r--r--   0        0        0     2044 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/http/__init__.py
+-rw-r--r--   0        0        0     5265 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/http/response.py
+-rw-r--r--   0        0        0     2608 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/meshcop.py
+-rw-r--r--   0        0        0    12834 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/__init__.py
+-rw-r--r--   0        0        0     1244 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/categories.py
+-rw-r--r--   0        0        0     1892 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/characteristics/__init__.py
+-rw-r--r--   0        0        0    14169 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/characteristics/characteristic.py
+-rw-r--r--   0        0        0     1815 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/characteristics/characteristic_formats.py
+-rw-r--r--   0        0        0    22463 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/characteristics/characteristic_types.py
+-rw-r--r--   0        0        0     5238 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/characteristics/const.py
+-rw-r--r--   0        0        0    29366 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/characteristics/data.py
+-rw-r--r--   0        0        0      800 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/characteristics/permissions.py
+-rw-r--r--   0        0        0     4407 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/characteristics/structs.py
+-rw-r--r--   0        0        0      731 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/characteristics/types.py
+-rw-r--r--   0        0        0     1067 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/characteristics/units.py
+-rw-r--r--   0        0        0     1439 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/entity_map.py
+-rw-r--r--   0        0        0      722 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/feature_flags.py
+-rw-r--r--   0        0        0      685 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/mixin.py
+-rw-r--r--   0        0        0      796 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/services/__init__.py
+-rw-r--r--   0        0        0    19993 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/services/data.py
+-rw-r--r--   0        0        0     5019 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/services/service.py
+-rw-r--r--   0        0        0     5380 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/services/service_types.py
+-rw-r--r--   0        0        0      703 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/services/types.py
+-rw-r--r--   0        0        0      716 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/model/status_flags.py
+-rw-r--r--   0        0        0     4065 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/pdu.py
+-rw-r--r--   0        0        0    20539 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/protocol/__init__.py
+-rw-r--r--   0        0        0     3493 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/protocol/statuscodes.py
+-rw-r--r--   0        0        0     8483 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/protocol/tlv.py
+-rw-r--r--   0        0        0        0 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/py.typed
+-rw-r--r--   0        0        0    12828 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/testing.py
+-rw-r--r--   0        0        0     8265 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/tlv8.py
+-rw-r--r--   0        0        0     3581 2023-07-11 08:13:06.283392 aiohomekit-2.6.7/aiohomekit/utils.py
+-rw-r--r--   0        0        0     1662 2023-07-11 08:13:06.287392 aiohomekit-2.6.7/aiohomekit/uuid.py
+-rw-r--r--   0        0        0    11606 2023-07-11 08:13:06.287392 aiohomekit-2.6.7/aiohomekit/zeroconf.py
+-rw-r--r--   0        0        0     1809 2023-07-11 08:13:06.287392 aiohomekit-2.6.7/pyproject.toml
+-rw-r--r--   0        0        0     7021 1970-01-01 00:00:00.000000 aiohomekit-2.6.7/PKG-INFO
```

### Comparing `aiohomekit-2.6.6/LICENSE.md` & `aiohomekit-2.6.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/README.md` & `aiohomekit-2.6.7/README.md`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/__init__.py` & `aiohomekit-2.6.7/aiohomekit/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/__main__.py` & `aiohomekit-2.6.7/aiohomekit/__main__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/characteristic_cache.py` & `aiohomekit-2.6.7/aiohomekit/characteristic_cache.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/const.py` & `aiohomekit-2.6.7/aiohomekit/const.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/__init__.py` & `aiohomekit-2.6.7/aiohomekit/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/abstract.py` & `aiohomekit-2.6.7/aiohomekit/controller/abstract.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ble/__init__.py` & `aiohomekit-2.6.7/aiohomekit/controller/ble/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ble/bleak.py` & `aiohomekit-2.6.7/aiohomekit/controller/ble/bleak.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ble/client.py` & `aiohomekit-2.6.7/aiohomekit/controller/ble/client.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ble/connection.py` & `aiohomekit-2.6.7/aiohomekit/controller/ble/connection.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ble/const.py` & `aiohomekit-2.6.7/aiohomekit/controller/ble/const.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ble/controller.py` & `aiohomekit-2.6.7/aiohomekit/controller/ble/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,16 @@
             data = HomeKitAdvertisement.from_manufacturer_data(
                 device.name, device.address, manufacturer_data
             )
         except ValueError:
             return
 
         if old_discovery := self.discoveries.get(data.id):
-            if (
-                (old_name := old_discovery.description.name)
-                and not (name := data.name)
+            if (old_name := old_discovery.description.name) and (
+                not (name := data.name)
                 or (
                     old_name != old_discovery.device.address
                     and len(old_name) > len(name)
                 )
             ):
                 #
                 # If we have a pairing and the name is longer than the one we
```

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ble/discovery.py` & `aiohomekit-2.6.7/aiohomekit/controller/ble/discovery.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ble/key.py` & `aiohomekit-2.6.7/aiohomekit/controller/ble/key.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ble/manufacturer_data.py` & `aiohomekit-2.6.7/aiohomekit/controller/ble/manufacturer_data.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ble/pairing.py` & `aiohomekit-2.6.7/aiohomekit/controller/ble/pairing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ble/structs.py` & `aiohomekit-2.6.7/aiohomekit/controller/ble/structs.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ble/values.py` & `aiohomekit-2.6.7/aiohomekit/controller/ble/values.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/coap/__init__.py` & `aiohomekit-2.6.7/aiohomekit/controller/coap/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/coap/connection.py` & `aiohomekit-2.6.7/aiohomekit/controller/coap/connection.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/coap/controller.py` & `aiohomekit-2.6.7/aiohomekit/controller/coap/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/coap/discovery.py` & `aiohomekit-2.6.7/aiohomekit/controller/coap/discovery.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/coap/pairing.py` & `aiohomekit-2.6.7/aiohomekit/controller/coap/pairing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/coap/pdu.py` & `aiohomekit-2.6.7/aiohomekit/controller/coap/pdu.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/coap/structs.py` & `aiohomekit-2.6.7/aiohomekit/controller/coap/structs.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/controller.py` & `aiohomekit-2.6.7/aiohomekit/controller/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ip/__init__.py` & `aiohomekit-2.6.7/aiohomekit/controller/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ip/connection.py` & `aiohomekit-2.6.7/aiohomekit/controller/ip/connection.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ip/controller.py` & `aiohomekit-2.6.7/aiohomekit/controller/ip/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ip/discovery.py` & `aiohomekit-2.6.7/aiohomekit/controller/ip/discovery.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/controller/ip/pairing.py` & `aiohomekit-2.6.7/aiohomekit/controller/ip/pairing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/crypto/__init__.py` & `aiohomekit-2.6.7/aiohomekit/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/crypto/chacha20poly1305.py` & `aiohomekit-2.6.7/aiohomekit/crypto/chacha20poly1305.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/crypto/hkdf.py` & `aiohomekit-2.6.7/aiohomekit/crypto/hkdf.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/crypto/srp.py` & `aiohomekit-2.6.7/aiohomekit/crypto/srp.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/debounce.py` & `aiohomekit-2.6.7/aiohomekit/debounce.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/enum.py` & `aiohomekit-2.6.7/aiohomekit/enum.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/exceptions.py` & `aiohomekit-2.6.7/aiohomekit/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/hkjson.py` & `aiohomekit-2.6.7/aiohomekit/hkjson.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/http/__init__.py` & `aiohomekit-2.6.7/aiohomekit/http/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/http/response.py` & `aiohomekit-2.6.7/aiohomekit/http/response.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/meshcop.py` & `aiohomekit-2.6.7/aiohomekit/meshcop.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/__init__.py` & `aiohomekit-2.6.7/aiohomekit/model/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/categories.py` & `aiohomekit-2.6.7/aiohomekit/model/categories.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/characteristics/__init__.py` & `aiohomekit-2.6.7/aiohomekit/model/characteristics/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/characteristics/characteristic.py` & `aiohomekit-2.6.7/aiohomekit/model/characteristics/characteristic.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/characteristics/characteristic_formats.py` & `aiohomekit-2.6.7/aiohomekit/model/characteristics/characteristic_formats.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/characteristics/characteristic_types.py` & `aiohomekit-2.6.7/aiohomekit/model/characteristics/characteristic_types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/characteristics/const.py` & `aiohomekit-2.6.7/aiohomekit/model/characteristics/const.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/characteristics/data.py` & `aiohomekit-2.6.7/aiohomekit/model/characteristics/data.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/characteristics/permissions.py` & `aiohomekit-2.6.7/aiohomekit/model/characteristics/permissions.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/characteristics/structs.py` & `aiohomekit-2.6.7/aiohomekit/model/characteristics/structs.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/characteristics/types.py` & `aiohomekit-2.6.7/aiohomekit/model/characteristics/types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/characteristics/units.py` & `aiohomekit-2.6.7/aiohomekit/model/characteristics/units.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/entity_map.py` & `aiohomekit-2.6.7/aiohomekit/model/entity_map.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/feature_flags.py` & `aiohomekit-2.6.7/aiohomekit/model/feature_flags.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/mixin.py` & `aiohomekit-2.6.7/aiohomekit/model/mixin.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/services/__init__.py` & `aiohomekit-2.6.7/aiohomekit/model/services/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/services/data.py` & `aiohomekit-2.6.7/aiohomekit/model/services/data.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/services/service.py` & `aiohomekit-2.6.7/aiohomekit/model/services/service.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/services/service_types.py` & `aiohomekit-2.6.7/aiohomekit/model/services/service_types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/services/types.py` & `aiohomekit-2.6.7/aiohomekit/model/services/types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/model/status_flags.py` & `aiohomekit-2.6.7/aiohomekit/model/status_flags.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/pdu.py` & `aiohomekit-2.6.7/aiohomekit/pdu.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/protocol/__init__.py` & `aiohomekit-2.6.7/aiohomekit/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/protocol/statuscodes.py` & `aiohomekit-2.6.7/aiohomekit/protocol/statuscodes.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/protocol/tlv.py` & `aiohomekit-2.6.7/aiohomekit/protocol/tlv.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/testing.py` & `aiohomekit-2.6.7/aiohomekit/testing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/tlv8.py` & `aiohomekit-2.6.7/aiohomekit/tlv8.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/utils.py` & `aiohomekit-2.6.7/aiohomekit/utils.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/uuid.py` & `aiohomekit-2.6.7/aiohomekit/uuid.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/aiohomekit/zeroconf.py` & `aiohomekit-2.6.7/aiohomekit/zeroconf.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.6/pyproject.toml` & `aiohomekit-2.6.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiohomekit"
-version = "2.6.6"
+version = "2.6.7"
 description = "An asyncio HomeKit client"
 authors = ["John Carr <john.carr@unrouted.co.uk>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/Jc2k/aiohomekit"
 repository = "https://github.com/Jc2k/aiohomekit"
 keywords = ["HomeKit", "home", "automation"]
```

### Comparing `aiohomekit-2.6.6/PKG-INFO` & `aiohomekit-2.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohomekit
-Version: 2.6.6
+Version: 2.6.7
 Summary: An asyncio HomeKit client
 Home-page: https://github.com/Jc2k/aiohomekit
 License: Apache-2.0
 Keywords: HomeKit,home,automation
 Author: John Carr
 Author-email: john.carr@unrouted.co.uk
 Requires-Python: >=3.9,<4.0
```

