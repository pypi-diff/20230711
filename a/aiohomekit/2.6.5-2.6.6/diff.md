# Comparing `tmp/aiohomekit-2.6.5.tar.gz` & `tmp/aiohomekit-2.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohomekit-2.6.5.tar", max compression
+gzip compressed data, was "aiohomekit-2.6.6.tar", max compression
```

## Comparing `aiohomekit-2.6.5.tar` & `aiohomekit-2.6.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0    11537 2023-06-08 11:57:27.219518 aiohomekit-2.6.5/LICENSE.md
--rw-r--r--   0        0        0     5841 2023-06-08 11:57:27.219518 aiohomekit-2.6.5/README.md
--rw-r--r--   0        0        0     1867 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/__init__.py
--rw-r--r--   0        0        0    18829 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/__main__.py
--rw-r--r--   0        0        0     4465 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/characteristic_cache.py
--rw-r--r--   0        0        0     1162 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/const.py
--rw-r--r--   0        0        0      697 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/__init__.py
--rw-r--r--   0        0        0    15767 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/abstract.py
--rw-r--r--   0        0        0      704 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/__init__.py
--rw-r--r--   0        0        0     6832 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/bleak.py
--rw-r--r--   0        0        0     7819 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/client.py
--rw-r--r--   0        0        0     2017 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/connection.py
--rw-r--r--   0        0        0     1310 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/const.py
--rw-r--r--   0        0        0     7024 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/controller.py
--rw-r--r--   0        0        0     7614 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/discovery.py
--rw-r--r--   0        0        0     1894 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/key.py
--rw-r--r--   0        0        0     3749 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/manufacturer_data.py
--rw-r--r--   0        0        0    68500 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/pairing.py
--rw-r--r--   0        0        0    11737 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/structs.py
--rw-r--r--   0        0        0     2140 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/values.py
--rw-r--r--   0        0        0      708 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/coap/__init__.py
--rw-r--r--   0        0        0    25705 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/coap/connection.py
--rw-r--r--   0        0        0     1182 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/coap/controller.py
--rw-r--r--   0        0        0     2422 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/coap/discovery.py
--rw-r--r--   0        0        0     9972 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/coap/pairing.py
--rw-r--r--   0        0        0     3433 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/coap/pdu.py
--rw-r--r--   0        0        0    12547 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/coap/structs.py
--rw-r--r--   0        0        0     9288 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/controller.py
--rw-r--r--   0        0        0      757 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ip/__init__.py
--rw-r--r--   0        0        0    22146 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ip/connection.py
--rw-r--r--   0        0        0     1120 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ip/controller.py
--rw-r--r--   0        0        0     4108 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ip/discovery.py
--rw-r--r--   0        0        0    20914 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ip/pairing.py
--rw-r--r--   0        0        0      868 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/crypto/__init__.py
--rw-r--r--   0        0        0     4789 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/crypto/chacha20poly1305.py
--rw-r--r--   0        0        0     1036 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/crypto/hkdf.py
--rw-r--r--   0        0        0    10728 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/crypto/srp.py
--rw-r--r--   0        0        0     4060 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/debounce.py
--rw-r--r--   0        0        0      985 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/enum.py
--rw-r--r--   0        0        0     7746 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/exceptions.py
--rw-r--r--   0        0        0     2116 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/hkjson.py
--rw-r--r--   0        0        0     2044 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/http/__init__.py
--rw-r--r--   0        0        0     5265 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/http/response.py
--rw-r--r--   0        0        0     2609 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/meshcop.py
--rw-r--r--   0        0        0    12839 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/__init__.py
--rw-r--r--   0        0        0     1245 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/categories.py
--rw-r--r--   0        0        0     1892 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/__init__.py
--rw-r--r--   0        0        0    14170 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/characteristic.py
--rw-r--r--   0        0        0     1815 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/characteristic_formats.py
--rw-r--r--   0        0        0    22463 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/characteristic_types.py
--rw-r--r--   0        0        0     4956 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/const.py
--rw-r--r--   0        0        0    29366 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/data.py
--rw-r--r--   0        0        0      800 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/permissions.py
--rw-r--r--   0        0        0     4410 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/structs.py
--rw-r--r--   0        0        0      731 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/types.py
--rw-r--r--   0        0        0     1067 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/units.py
--rw-r--r--   0        0        0     1439 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/entity_map.py
--rw-r--r--   0        0        0      723 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/feature_flags.py
--rw-r--r--   0        0        0      685 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/mixin.py
--rw-r--r--   0        0        0      796 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/services/__init__.py
--rw-r--r--   0        0        0    19993 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/services/data.py
--rw-r--r--   0        0        0     5021 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/services/service.py
--rw-r--r--   0        0        0     5380 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/model/services/service_types.py
--rw-r--r--   0        0        0      703 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/model/services/types.py
--rw-r--r--   0        0        0      717 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/model/status_flags.py
--rw-r--r--   0        0        0     4067 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/pdu.py
--rw-r--r--   0        0        0    20539 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/protocol/__init__.py
--rw-r--r--   0        0        0     3494 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/protocol/statuscodes.py
--rw-r--r--   0        0        0     8483 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/protocol/tlv.py
--rw-r--r--   0        0        0        0 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/py.typed
--rw-r--r--   0        0        0    12836 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/testing.py
--rw-r--r--   0        0        0     8265 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/tlv8.py
--rw-r--r--   0        0        0     3581 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/utils.py
--rw-r--r--   0        0        0     1662 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/uuid.py
--rw-r--r--   0        0        0    11606 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/zeroconf.py
--rw-r--r--   0        0        0     1809 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/pyproject.toml
--rw-r--r--   0        0        0     7021 1970-01-01 00:00:00.000000 aiohomekit-2.6.5/PKG-INFO
+-rw-r--r--   0        0        0    11537 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/LICENSE.md
+-rw-r--r--   0        0        0     5841 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/README.md
+-rw-r--r--   0        0        0     1867 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/__init__.py
+-rw-r--r--   0        0        0    18826 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/__main__.py
+-rw-r--r--   0        0        0     4465 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/characteristic_cache.py
+-rw-r--r--   0        0        0     1162 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/const.py
+-rw-r--r--   0        0        0      697 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/__init__.py
+-rw-r--r--   0        0        0    15761 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/abstract.py
+-rw-r--r--   0        0        0      704 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/__init__.py
+-rw-r--r--   0        0        0     6832 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/bleak.py
+-rw-r--r--   0        0        0     7819 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/client.py
+-rw-r--r--   0        0        0     2017 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/connection.py
+-rw-r--r--   0        0        0     1310 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/const.py
+-rw-r--r--   0        0        0     7083 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/controller.py
+-rw-r--r--   0        0        0     7614 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/discovery.py
+-rw-r--r--   0        0        0     1894 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/key.py
+-rw-r--r--   0        0        0     3747 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/manufacturer_data.py
+-rw-r--r--   0        0        0    68499 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/pairing.py
+-rw-r--r--   0        0        0    11736 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/structs.py
+-rw-r--r--   0        0        0     2140 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/ble/values.py
+-rw-r--r--   0        0        0      708 2023-07-11 02:04:46.639929 aiohomekit-2.6.6/aiohomekit/controller/coap/__init__.py
+-rw-r--r--   0        0        0    25692 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/coap/connection.py
+-rw-r--r--   0        0        0     1181 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/coap/controller.py
+-rw-r--r--   0        0        0     2422 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/coap/discovery.py
+-rw-r--r--   0        0        0     9972 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/coap/pairing.py
+-rw-r--r--   0        0        0     3431 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/coap/pdu.py
+-rw-r--r--   0        0        0    12547 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/coap/structs.py
+-rw-r--r--   0        0        0     9288 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/controller.py
+-rw-r--r--   0        0        0      757 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/ip/__init__.py
+-rw-r--r--   0        0        0    22146 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/ip/connection.py
+-rw-r--r--   0        0        0     1119 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/ip/controller.py
+-rw-r--r--   0        0        0     4108 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/ip/discovery.py
+-rw-r--r--   0        0        0    20914 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/controller/ip/pairing.py
+-rw-r--r--   0        0        0      868 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/crypto/__init__.py
+-rw-r--r--   0        0        0     4789 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/crypto/chacha20poly1305.py
+-rw-r--r--   0        0        0     1036 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/crypto/hkdf.py
+-rw-r--r--   0        0        0    10728 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/crypto/srp.py
+-rw-r--r--   0        0        0     4060 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/debounce.py
+-rw-r--r--   0        0        0      985 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/enum.py
+-rw-r--r--   0        0        0     7746 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/exceptions.py
+-rw-r--r--   0        0        0     2116 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/hkjson.py
+-rw-r--r--   0        0        0     2044 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/http/__init__.py
+-rw-r--r--   0        0        0     5265 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/http/response.py
+-rw-r--r--   0        0        0     2608 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/meshcop.py
+-rw-r--r--   0        0        0    12834 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/__init__.py
+-rw-r--r--   0        0        0     1244 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/categories.py
+-rw-r--r--   0        0        0     1892 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/__init__.py
+-rw-r--r--   0        0        0    14169 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/characteristic.py
+-rw-r--r--   0        0        0     1815 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/characteristic_formats.py
+-rw-r--r--   0        0        0    22463 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/characteristic_types.py
+-rw-r--r--   0        0        0     5238 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/const.py
+-rw-r--r--   0        0        0    29366 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/data.py
+-rw-r--r--   0        0        0      800 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/permissions.py
+-rw-r--r--   0        0        0     4407 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/structs.py
+-rw-r--r--   0        0        0      731 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/types.py
+-rw-r--r--   0        0        0     1067 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/characteristics/units.py
+-rw-r--r--   0        0        0     1439 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/entity_map.py
+-rw-r--r--   0        0        0      722 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/feature_flags.py
+-rw-r--r--   0        0        0      685 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/mixin.py
+-rw-r--r--   0        0        0      796 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/services/__init__.py
+-rw-r--r--   0        0        0    19993 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/services/data.py
+-rw-r--r--   0        0        0     5019 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/services/service.py
+-rw-r--r--   0        0        0     5380 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/services/service_types.py
+-rw-r--r--   0        0        0      703 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/services/types.py
+-rw-r--r--   0        0        0      716 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/model/status_flags.py
+-rw-r--r--   0        0        0     4065 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/pdu.py
+-rw-r--r--   0        0        0    20539 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/protocol/__init__.py
+-rw-r--r--   0        0        0     3493 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/protocol/statuscodes.py
+-rw-r--r--   0        0        0     8483 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/protocol/tlv.py
+-rw-r--r--   0        0        0        0 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/py.typed
+-rw-r--r--   0        0        0    12828 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/testing.py
+-rw-r--r--   0        0        0     8265 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/tlv8.py
+-rw-r--r--   0        0        0     3581 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/utils.py
+-rw-r--r--   0        0        0     1662 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/uuid.py
+-rw-r--r--   0        0        0    11606 2023-07-11 02:04:46.643929 aiohomekit-2.6.6/aiohomekit/zeroconf.py
+-rw-r--r--   0        0        0     1809 2023-07-11 02:04:46.647929 aiohomekit-2.6.6/pyproject.toml
+-rw-r--r--   0        0        0     7021 1970-01-01 00:00:00.000000 aiohomekit-2.6.6/PKG-INFO
```

### Comparing `aiohomekit-2.6.5/LICENSE.md` & `aiohomekit-2.6.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/README.md` & `aiohomekit-2.6.6/README.md`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/__init__.py` & `aiohomekit-2.6.6/aiohomekit/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/__main__.py` & `aiohomekit-2.6.6/aiohomekit/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,14 @@
 
         print(f'Pairing for "{args.alias}" was established.')
     return True
 
 
 async def get_accessories(args: Namespace) -> bool:
     async with get_controller(args) as controller:
-
         if args.alias not in controller.aliases:
             print(f'"{args.alias}" is no known alias')
             return False
 
         try:
             pairing = controller.aliases[args.alias]
             data = await pairing.list_accessories_and_characteristics()
@@ -206,15 +205,14 @@
                         desc = characteristic.get("description", "")
                         print(f"  {aid}.{c_iid}: {value} ({desc}) >{c_type}< [{perms}]")
     return True
 
 
 async def get_characteristics(args: Namespace) -> bool:
     async with get_controller(args) as controller:
-
         if args.alias not in controller.aliases:
             print(f'"{args.alias}" is no known alias')
             return False
 
         pairing = controller.aliases[args.alias]
 
         # convert the command line parameters to the required form
@@ -240,15 +238,14 @@
         print(hkjson.dumps_indented(tmp))
 
     return True
 
 
 async def put_characteristics(args: Namespace) -> bool:
     async with get_controller(args) as controller:
-
         if args.alias not in controller.aliases:
             print(f'"{args.alias}" is no known alias')
             return False
 
         try:
             pairing = controller.aliases[args.alias]
```

### Comparing `aiohomekit-2.6.5/aiohomekit/characteristic_cache.py` & `aiohomekit-2.6.6/aiohomekit/characteristic_cache.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/const.py` & `aiohomekit-2.6.6/aiohomekit/const.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/__init__.py` & `aiohomekit-2.6.6/aiohomekit/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/abstract.py` & `aiohomekit-2.6.6/aiohomekit/controller/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,43 +36,39 @@
     serialize_broadcast_key,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractPairingData(TypedDict, total=False):
-
     AccessoryPairingID: str
     AccessoryLTPK: str
     iOSPairingId: str
     iOSDeviceLTSK: str
     iOSDeviceLTPK: str
     AccessoryAddress: str
     Connection: str
 
 
 @dataclass
 class AbstractDescription:
-
     name: str
     id: str
     status_flags: StatusFlags
     config_num: int
     category: Categories
 
 
 class TransportType(Enum):
-
     IP = "ip"
     COAP = "coap"
     BLE = "ble"
 
 
 class AbstractPairing(metaclass=ABCMeta):
-
     # The current discovery information for this pairing.
     # This can be used to detect address changes, s# changes, c# changes, etc
     description: AbstractDescription | None = None
 
     # The normalised (lower case) form of the device id (as seen in zeroconf
     # and BLE advertisements), and also as AccessoryPairingID i pairing data.
     id: str
@@ -413,15 +409,14 @@
         return stop_listening
 
 
 FinishPairing = Callable[[str], Awaitable[AbstractPairing]]
 
 
 class AbstractDiscovery(metaclass=ABCMeta):
-
     description: AbstractDescription
 
     @final
     @property
     def paired(self) -> bool:
         return not (self.description.status_flags & StatusFlags.UNPAIRED)
 
@@ -431,15 +426,14 @@
 
     @abstractmethod
     async def async_identify(self) -> None:
         """Do an unpaired identify."""
 
 
 class AbstractController(metaclass=ABCMeta):
-
     discoveries: dict[str, AbstractDiscovery]
     pairings: dict[str, AbstractPairing]
     aliases: dict[str, AbstractPairing]
 
     def __init__(self, char_cache: CharacteristicCacheType) -> None:
         self.pairings = {}
         self.aliases = {}
```

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ble/__init__.py` & `aiohomekit-2.6.6/aiohomekit/controller/ble/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ble/bleak.py` & `aiohomekit-2.6.6/aiohomekit/controller/ble/bleak.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ble/client.py` & `aiohomekit-2.6.6/aiohomekit/controller/ble/client.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ble/connection.py` & `aiohomekit-2.6.6/aiohomekit/controller/ble/connection.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ble/const.py` & `aiohomekit-2.6.6/aiohomekit/controller/ble/const.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ble/controller.py` & `aiohomekit-2.6.6/aiohomekit/controller/ble/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,48 +73,51 @@
         try:
             data = HomeKitAdvertisement.from_manufacturer_data(
                 device.name, device.address, manufacturer_data
             )
         except ValueError:
             return
 
-        if pairing := self.pairings.get(data.id):
+        if old_discovery := self.discoveries.get(data.id):
             if (
-                (old_description := pairing.description)
-                and old_description.name != old_description.address
-                and len(old_description.name) > len(data.name)
+                (old_name := old_discovery.description.name)
+                and not (name := data.name)
+                or (
+                    old_name != old_discovery.device.address
+                    and len(old_name) > len(name)
+                )
             ):
                 #
                 # If we have a pairing and the name is longer than the one we
                 # just received, we assume the name is more accurate and
                 # update it.
                 #
                 # SHORTENED LOCAL NAME
                 # The Shortened Local Name data type defines a shortened version
                 # of the Local Name data type. The Shortened Local Name data type
                 # shall not be used to advertise a name that is longer than the
                 # Local Name data type.
                 #
-                data.name = old_description.name
+                data.name = old_name
+
+        if pairing := self.pairings.get(data.id):
             pairing._async_description_update(data)
             pairing._async_ble_update(device, advertisement_data)
 
         if futures := self._ble_futures.get(data.id):
             discovery = BleDiscovery(self, device, data, advertisement_data)
             logger.debug("BLE device for %s found, fulfilling futures", data.id)
             for future in futures:
                 future.set_result(discovery)
             futures.clear()
 
-        if data.id in self.discoveries:
+        if old_discovery:
             # We need to make sure we update the device details
             # in case they changed
-            self.discoveries[data.id]._async_process_advertisement(
-                device, data, advertisement_data
-            )
+            old_discovery._async_process_advertisement(device, data, advertisement_data)
             return
 
         self.discoveries[data.id] = BleDiscovery(self, device, data, advertisement_data)
 
     async def async_start(self) -> None:
         logger.debug("Starting BLE controller with instance: %s", self._scanner)
         if not self._scanner:
```

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ble/discovery.py` & `aiohomekit-2.6.6/aiohomekit/controller/ble/discovery.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ble/key.py` & `aiohomekit-2.6.6/aiohomekit/controller/ble/key.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ble/manufacturer_data.py` & `aiohomekit-2.6.6/aiohomekit/controller/ble/manufacturer_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 HOMEKIT_ENCRYPTED_NOTIFICATION_TYPE = 0x11
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class HomeKitAdvertisement(AbstractDescription):
-
     setup_hash: bytes
     address: str
     state_num: int
 
     @classmethod
     def from_manufacturer_data(
         cls, name: str, address: str, manufacturer_data: dict[int, bytes]
@@ -80,15 +79,14 @@
             raise ValueError("No manufacturer data")
 
         return cls.from_manufacturer_data(device.name, device.address, mfr_data)
 
 
 @dataclass
 class HomeKitEncryptedNotification:
-
     name: str
     address: str
     id: str
     advertising_identifier: bytes
     encrypted_payload: bytes
 
     @classmethod
```

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ble/pairing.py` & `aiohomekit-2.6.6/aiohomekit/controller/ble/pairing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1472,15 +1472,14 @@
             "%s: Writing characteristics: %s; rssi=%s",
             self.name,
             characteristics,
             self.rssi,
         )
         accessory_chars = self.accessories.aid(BLE_AID).characteristics
         async with self._ble_request_lock:
-
             for aid, iid, value in characteristics:
                 char = accessory_chars.iid(iid)
                 result_key = (aid, iid)
                 logger.debug(
                     "%s: Writing characteristics: iid=%s value=%s",
                     self.name,
                     iid,
```

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ble/structs.py` & `aiohomekit-2.6.6/aiohomekit/controller/ble/structs.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from aiohomekit.tlv8 import TLVStruct, tlv_entry, u8, u16, u128
 
 from .const import AdditionalParameterTypes
 
 
 @dataclass
 class ProtocolParams:
-
     state_number: int
     config_number: int
     advertising_id: bytes
     broadcast_key: Optional[bytes]
 
 
 class ProtocolParamsTLV(enum.IntEnum):
```

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ble/values.py` & `aiohomekit-2.6.6/aiohomekit/controller/ble/values.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/coap/__init__.py` & `aiohomekit-2.6.6/aiohomekit/controller/coap/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/coap/connection.py` & `aiohomekit-2.6.6/aiohomekit/controller/coap/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 
 def decode_list_pairings_response(buf):
     inner_bytes = decode_pdu_03(buf)
     return TLV.decode_bytes(inner_bytes)
 
 
 class EncryptionContext:
-
     coap_ctx: Context
     lock: asyncio.Lock
     uri: str
 
     event_ctr: int
     event_ctx: ChaCha20Poly1305
     recv_ctr: int
@@ -431,15 +430,15 @@
 
                 # make a list of zero length byte strings
                 data = [b""] * len(iids)
 
                 # send the read requests
                 results = await self.enc_ctx.post_all(OpCode.CHAR_READ, iids, data)
 
-                for (idx, result) in enumerate(results):
+                for idx, result in enumerate(results):
                     if isinstance(result, bytes):
                         # success, let's convert the value
                         value = decode_pdu_03(result) if len(result) > 0 else b""
                         readable[idx].raw_value = value
                         logger.debug(
                             "Read value for %X.%X iid %d: value %r"
                             % (
@@ -462,15 +461,15 @@
 
         return self.info.to_dict()
 
     def _read_characteristics_exit(
         self, ids: list[tuple[int, int]], pdu_results: list[bytes | PDUStatus]
     ) -> dict:
         results = dict()
-        for (idx, result) in enumerate(pdu_results):
+        for idx, result in enumerate(pdu_results):
             aid_iid = ids[idx]
             if isinstance(result, PDUStatus):
                 logger.debug(
                     "Failed to read aid %d iid %d" % (int(aid_iid[0]), int(aid_iid[1]))
                 )
                 results[aid_iid] = {
                     "description": result.description,
@@ -510,15 +509,15 @@
         return self._read_characteristics_exit(ids, pdu_results)
 
     def _write_characteristics_enter(
         self, ids_values: list[tuple[int, int, Any]]
     ) -> list[bytearray]:
         # convert provided values to appropriate binary format for each characteristic
         tlv_values = list()
-        for (_, aid_iid_value) in enumerate(ids_values):
+        for _, aid_iid_value in enumerate(ids_values):
             # look up characteristic
             characteristic = self.info.find_characteristic_by_aid_iid(
                 int(aid_iid_value[0]), int(aid_iid_value[1])
             )
             # write value to cache + convert to appropriate binary representation
             characteristic.value = aid_iid_value[2]
             # get the converted value
@@ -534,15 +533,15 @@
         self,
         ids_values: list[tuple[int, int, Any]],
         pdu_results: list[bytes | PDUStatus],
     ) -> dict:
         # transform results
         # only error conditions are returned
         results = dict()
-        for (idx, result) in enumerate(pdu_results):
+        for idx, result in enumerate(pdu_results):
             aid_iid_value = ids_values[idx]
             key = (aid_iid_value[0], aid_iid_value[1])
             if isinstance(result, PDUStatus):
                 results[key] = {
                     "descripton": result.description,
                     "status": -result.value,  # XXX
                 }
@@ -569,15 +568,15 @@
 
         return self._write_characteristics_exit(ids_values, pdu_results)
 
     def _subscribe_to_exit(
         self, ids: list[tuple[int, int]], pdu_results: list[bytes | PDUStatus]
     ) -> dict:
         results = dict()
-        for (idx, result) in enumerate(pdu_results):
+        for idx, result in enumerate(pdu_results):
             aid_iid = ids[idx]
             key = (aid_iid[0], aid_iid[1])
             if isinstance(result, PDUStatus):
                 results[key] = {
                     "descripton": result.description,
                     "status": -result.value,  # XXX
                 }
@@ -598,15 +597,15 @@
         pdu_results = await self.enc_ctx.post_all(OpCode.UNK_0B_SUBSCRIBE, iids, data)
         return self._subscribe_to_exit(ids, pdu_results)
 
     def _unsubscribe_from_exit(
         self, ids: list[tuple[int, int]], pdu_results: list[bytes | PDUStatus]
     ) -> dict:
         results = dict()
-        for (idx, result) in enumerate(pdu_results):
+        for idx, result in enumerate(pdu_results):
             aid_iid = ids[idx]
             key = (aid_iid[0], aid_iid[1])
             if isinstance(result, PDUStatus):
                 results[key] = {
                     "descripton": result.description,
                     "status": -result.value,  # XXX
                 }
```

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/coap/controller.py` & `aiohomekit-2.6.6/aiohomekit/controller/coap/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from aiohomekit.controller.abstract import TransportType
 from aiohomekit.controller.coap.discovery import CoAPDiscovery
 from aiohomekit.controller.coap.pairing import CoAPPairing
 from aiohomekit.zeroconf import HAP_TYPE_UDP, ZeroconfController
 
 
 class CoAPController(ZeroconfController):
-
     hap_type = HAP_TYPE_UDP
     discoveries: dict[str, CoAPDiscovery]
     pairings: dict[str, CoAPPairing]
     aliases: dict[str, CoAPPairing]
     transport_type = TransportType.COAP
 
     def _make_discovery(self, discovery) -> CoAPDiscovery:
```

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/coap/discovery.py` & `aiohomekit-2.6.6/aiohomekit/controller/coap/discovery.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/coap/pairing.py` & `aiohomekit-2.6.6/aiohomekit/controller/coap/pairing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/coap/pdu.py` & `aiohomekit-2.6.6/aiohomekit/controller/coap/pdu.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,28 +22,26 @@
 
 from aiohomekit.enum import EnumWithDescription
 
 logger = logging.getLogger(__name__)
 
 
 class OpCode(Enum):
-
     CHAR_SIG_READ = 0x01
     CHAR_WRITE = 0x02
     CHAR_READ = 0x03
     CHAR_TIMED_WRITE = 0x04
     CHAR_EXEC_WRITE = 0x05
     SERV_SIG_READ = 0x06
     UNK_09_READ_GATT = 0x09
     UNK_0B_SUBSCRIBE = 0x0B
     UNK_0C_UNSUBSCRIBE = 0x0C
 
 
 class PDUStatus(EnumWithDescription):
-
     SUCCESS = 0, "Success"
     UNSUPPORTED_PDU = 1, "Unsupported PDU"
     MAX_PROCEDURES = 2, "Max procedures"
     INSUFFICIENT_AUTHORIZATION = 3, "Insufficient authorization"
     INVALID_INSTANCE_ID = 4, "Invalid instance ID"
     INSUFFICIENT_AUTHENTICATION = 5, "Insufficient authentication"
     INVALID_REQUEST = 6, "Invalid request"
```

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/coap/structs.py` & `aiohomekit-2.6.6/aiohomekit/controller/coap/structs.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/controller.py` & `aiohomekit-2.6.6/aiohomekit/controller/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ip/__init__.py` & `aiohomekit-2.6.6/aiohomekit/controller/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ip/connection.py` & `aiohomekit-2.6.6/aiohomekit/controller/ip/connection.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ip/controller.py` & `aiohomekit-2.6.6/aiohomekit/controller/ip/controller.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from aiohomekit.controller.abstract import TransportType
 from aiohomekit.controller.ip.discovery import IpDiscovery
 from aiohomekit.controller.ip.pairing import IpPairing
 from aiohomekit.zeroconf import HAP_TYPE_TCP, ZeroconfController
 
 
 class IpController(ZeroconfController):
-
     hap_type = HAP_TYPE_TCP
     discoveries: dict[str, IpDiscovery]
     pairings: dict[str, IpPairing]
     transport_type = TransportType.IP
 
     def _make_discovery(self, discovery) -> IpDiscovery:
         return IpDiscovery(self, discovery)
```

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ip/discovery.py` & `aiohomekit-2.6.6/aiohomekit/controller/ip/discovery.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/controller/ip/pairing.py` & `aiohomekit-2.6.6/aiohomekit/controller/ip/pairing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/crypto/__init__.py` & `aiohomekit-2.6.6/aiohomekit/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/crypto/chacha20poly1305.py` & `aiohomekit-2.6.6/aiohomekit/crypto/chacha20poly1305.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/crypto/hkdf.py` & `aiohomekit-2.6.6/aiohomekit/crypto/hkdf.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/crypto/srp.py` & `aiohomekit-2.6.6/aiohomekit/crypto/srp.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/debounce.py` & `aiohomekit-2.6.6/aiohomekit/debounce.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/enum.py` & `aiohomekit-2.6.6/aiohomekit/enum.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/exceptions.py` & `aiohomekit-2.6.6/aiohomekit/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/hkjson.py` & `aiohomekit-2.6.6/aiohomekit/hkjson.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/http/__init__.py` & `aiohomekit-2.6.6/aiohomekit/http/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/http/response.py` & `aiohomekit-2.6.6/aiohomekit/http/response.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/meshcop.py` & `aiohomekit-2.6.6/aiohomekit/meshcop.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from dataclasses import dataclass
 
 from aiohomekit.tlv8 import TLVStruct, bu16, tlv_entry
 
 
 @dataclass
 class Meshcop(TLVStruct):
-
     channel: bu16 = tlv_entry(0)
     panid: bu16 = tlv_entry(1)
     extpanid: bytes = tlv_entry(2)
     networkname: str = tlv_entry(3)
     pskc: bytes = tlv_entry(4)
     networkkey: bytes = tlv_entry(5)
     network_key_sequence: bytes = tlv_entry(6)
```

### Comparing `aiohomekit-2.6.5/aiohomekit/model/__init__.py` & `aiohomekit-2.6.6/aiohomekit/model/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 NEEDS_POLLINGS_CHARS = {
     CharacteristicsTypes.VENDOR_EVE_ENERGY_WATT,
     CharacteristicsTypes.VENDOR_CONNECTSENSE_ENERGY_WATT,
 }
 
 
 class Transport(Enum):
-
     BLE = "ble"
     COAP = "coap"
     IP = "ip"
 
 
 class Services:
     def __init__(self):
@@ -322,15 +321,14 @@
         for s in self.services:
             services_list.append(s.to_accessory_and_service_list())
         d = {"aid": self.aid, "services": services_list}
         return d
 
 
 class Accessories:
-
     accessories: list[Accessory]
 
     def __init__(self) -> None:
         self.accessories = []
         self._aid_to_accessory: dict[int, Accessory] = {}
 
     def __iter__(self) -> Iterator[Accessory]:
@@ -368,15 +366,15 @@
     def aid(self, aid: int) -> Accessory:
         return self._aid_to_accessory[aid]
 
     def has_aid(self, aid: int) -> bool:
         return aid in self._aid_to_accessory
 
     def process_changes(self, changes: dict[tuple[int, int], Any]) -> None:
-        for ((aid, iid), value) in changes.items():
+        for (aid, iid), value in changes.items():
             accessory = self.aid(aid)
             if not accessory:
                 continue
 
             char = accessory.characteristics.iid(iid)
             if not char:
                 continue
@@ -385,12 +383,11 @@
                 char.set_value(value["value"])
 
             char.status = to_status_code(value.get("status", 0))
 
 
 @dataclass
 class AccessoriesState:
-
     accessories: Accessories
     config_num: int
     broadcast_key: bytes | None = None
     state_num: int | None = None
```

### Comparing `aiohomekit-2.6.5/aiohomekit/model/categories.py` & `aiohomekit-2.6.6/aiohomekit/model/categories.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # limitations under the License.
 #
 
 import enum
 
 
 class Categories(enum.IntFlag):
-
     OTHER = 1
     BRIDGE = 2
     FAN = 3
     GARAGE = 4
     LIGHTBULB = 5
     DOOR_LOCK = 6
     OUTLET = 7
```

### Comparing `aiohomekit-2.6.5/aiohomekit/model/characteristics/__init__.py` & `aiohomekit-2.6.6/aiohomekit/model/characteristics/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/model/characteristics/characteristic.py` & `aiohomekit-2.6.6/aiohomekit/model/characteristics/characteristic.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     elif val in ("n", "no", "f", "false", "off", "0"):
         return 0
     else:
         raise ValueError(f"invalid truth value {val!r}")
 
 
 class Characteristic:
-
     type: str
     iid: int
     perms: list[str]
     minValue: int | float | None
     maxValue: int | float | None
     minStep: int | float | None
     handle: int | None = None
```

### Comparing `aiohomekit-2.6.5/aiohomekit/model/characteristics/characteristic_formats.py` & `aiohomekit-2.6.6/aiohomekit/model/characteristics/characteristic_formats.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/model/characteristics/characteristic_types.py` & `aiohomekit-2.6.6/aiohomekit/model/characteristics/characteristic_types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/model/characteristics/const.py` & `aiohomekit-2.6.6/aiohomekit/model/characteristics/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,32 +89,47 @@
     IRRIGATION = 1
     SHOWER_HEAD = 2
     WATER_FAUCET = 3
 
 
 class ActivationStateValues(enum.IntEnum):
     """Possible values for the current status of an accessory.
-    https://developer.apple.com/documentation/homekit/hmcharacteristicvalueactivationstate"""
+    https://developer.apple.com/documentation/homekit/hmcharacteristicvalueactivationstate
+    """
 
     INACTIVE = 0
     ACTIVE = 1
 
 
+class AirQualityValues(enum.IntEnum):
+    """Possible values for the air quality.
+    https://developer.apple.com/documentation/homekit/hmcharacteristicvalueairquality"""
+
+    UNKNOWN = 0
+    EXCELLENT = 1
+    GOOD = 2
+    FAIR = 3
+    INFERIOR = 4
+    POOR = 5
+
+
 class CurrentAirPurifierStateValues(enum.IntEnum):
     """Possible values for the current state of an air purifier.
-    https://developer.apple.com/documentation/homekit/hmcharacteristicvaluecurrentairpurifierstate"""
+    https://developer.apple.com/documentation/homekit/hmcharacteristicvaluecurrentairpurifierstate
+    """
 
     INACTIVE = 0
     IDLE = 1
     ACTIVE = 2
 
 
 class TargetAirPurifierStateValues(enum.IntEnum):
     """Possible values for the target state  of an air purifier.
-    https://developer.apple.com/documentation/homekit/hmcharacteristicvaluetargetairpurifierstate"""
+    https://developer.apple.com/documentation/homekit/hmcharacteristicvaluetargetairpurifierstate
+    """
 
     MANUAL = 0
     AUTOMATIC = 1
 
 
 class SwingModeValues(enum.IntEnum):
     """Possible values for fan movement.
@@ -122,25 +137,27 @@
 
     DISABLED = 0
     ENABLED = 1
 
 
 class CurrentHeaterCoolerStateValues(enum.IntEnum):
     """Possible values for the current state of a device that heats or cools.
-    https://developer.apple.com/documentation/homekit/hmcharacteristicvaluecurrentheatercoolerstate"""
+    https://developer.apple.com/documentation/homekit/hmcharacteristicvaluecurrentheatercoolerstate
+    """
 
     INACTIVE = 0
     IDLE = 1
     HEATING = 2
     COOLING = 3
 
 
 class TargetHeaterCoolerStateValues(enum.IntEnum):
     """Possible values for the target state of a device that heats or cools.
-    https://developer.apple.com/documentation/homekit/hmcharacteristicvaluetargetheatercoolerstate"""
+    https://developer.apple.com/documentation/homekit/hmcharacteristicvaluetargetheatercoolerstate
+    """
 
     AUTOMATIC = 0
     HEAT = 1
     COOL = 2
 
 
 class StreamingStatusValues(enum.IntEnum):
@@ -158,15 +175,14 @@
     START_SESSION = 1
     SUSPEND_SESSION = 2
     RESUME_SESSION = 3
     RECONFIGURE_SESSION = 4
 
 
 class VideoCodecTypeValues(enum.IntEnum):
-
     H264 = 0
 
 
 class ProfileIDValues(enum.IntEnum):
 
     """
     The type of H.264 profile used.
@@ -195,15 +211,14 @@
     1 - 255 are reserved by Apple.
     """
 
     NON_INTERLEAVED_MODE = 0
 
 
 class CVOEnabledValues(enum.IntEnum):
-
     NOT_SUPPORTED = 0
     SUPPORTED = 1
 
 
 class AudioCodecValues(enum.IntEnum):
 
     """
@@ -213,44 +228,39 @@
     AAC_ELD = 2
     OPUS = 3
     AMR = 5
     AMR_WB = 6
 
 
 class BitRateValues(enum.IntEnum):
-
     VARIABLE = 0
     CONSTANT = 1
 
 
 class SampleRateValues(enum.IntEnum):
-
     EIGHT_KHZ = 0
     SIXTEEN_KHZ = 1
     TWENTY_FOUR_KHZ = 2
 
 
 class SRTPCryptoSuiteValues(enum.IntEnum):
-
     AES_CM_128_HMAC_SHA1_80 = 0
     AES_256_CM_HMAC_SHA1_80 = 1
     DISABLED = 2
 
 
 class ThreadNodeCapabilities(enum.IntFlag):
-
     MINIMAL = 0x01
     SLEEPY = 0x02
     FULL = 0x04
     ROUTER_ELIGIBLE = 0x08
     BORDER_ROUTER_CAPABLE = 0x10
 
 
 class ThreadStatus(enum.IntFlag):
-
     DISABLED = 0x01
     DETACHED = 0x02
     JOINING = 0x04
     CHILD = 0x08
     ROUTER = 0x10
     LEADER = 0x20
     BORDER_ROUTER = 0x40
```

### Comparing `aiohomekit-2.6.5/aiohomekit/model/characteristics/data.py` & `aiohomekit-2.6.6/aiohomekit/model/characteristics/data.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/model/characteristics/permissions.py` & `aiohomekit-2.6.6/aiohomekit/model/characteristics/permissions.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/model/characteristics/structs.py` & `aiohomekit-2.6.6/aiohomekit/model/characteristics/structs.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     StreamingStatusValues,
     VideoCodecTypeValues,
 )
 
 
 @dataclass
 class StreamingStatus(TLVStruct):
-
     status: StreamingStatusValues = tlv_entry(1)
 
 
 @dataclass
 class SessionControl(TLVStruct):
     session: str = tlv_entry(1)
     command: SessionControlCommandValues = tlv_entry(2)
@@ -59,15 +58,14 @@
     packetization_mode: PacketizationModeValues = tlv_entry(3)
     cvo_enabled: CVOEnabledValues = tlv_entry(4)
     cvo_id: u8 = tlv_entry(5)
 
 
 @dataclass
 class AudioCodecParameters(TLVStruct):
-
     audio_channels: u8 = tlv_entry(1)
     bit_rate: BitRateValues = tlv_entry(2)
     sample_rate: SampleRateValues = tlv_entry(3)
     rtp_time: u8 = tlv_entry(4)
 
 
 @dataclass
@@ -102,15 +100,14 @@
     codec_parameters: AudioCodecParameters = tlv_entry(2)
     rtp_params: AudioRTPParameters = tlv_entry(3)
     comfort_noise: u8 = tlv_entry(4)
 
 
 @dataclass
 class AudioCodecConfiguration(TLVStruct):
-
     codec: AudioCodecValues = tlv_entry(1)
     parameters: Sequence[AudioCodecParameters] = tlv_entry(2)
 
 
 @dataclass
 class VideoConfigConfiguration(TLVStruct):
     codec_type: VideoCodecTypeValues = tlv_entry(1)
```

### Comparing `aiohomekit-2.6.5/aiohomekit/model/characteristics/types.py` & `aiohomekit-2.6.6/aiohomekit/model/characteristics/types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/model/characteristics/units.py` & `aiohomekit-2.6.6/aiohomekit/model/characteristics/units.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/model/entity_map.py` & `aiohomekit-2.6.6/aiohomekit/model/entity_map.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/model/feature_flags.py` & `aiohomekit-2.6.6/aiohomekit/model/feature_flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,10 +14,9 @@
 # limitations under the License.
 #
 
 import enum
 
 
 class FeatureFlags(enum.IntFlag):
-
     SUPPORTS_APPLE_AUTHENTICATION_COPROCESSOR = 1
     SUPPORTS_SOFTWARE_AUTHENTICATION = 2
```

### Comparing `aiohomekit-2.6.5/aiohomekit/model/mixin.py` & `aiohomekit-2.6.6/aiohomekit/model/mixin.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/model/services/__init__.py` & `aiohomekit-2.6.6/aiohomekit/model/services/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/model/services/data.py` & `aiohomekit-2.6.6/aiohomekit/model/services/data.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/model/services/service.py` & `aiohomekit-2.6.6/aiohomekit/model/services/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from aiohomekit.uuid import normalize_uuid
 
 if TYPE_CHECKING:
     from aiohomekit.model import Accessory
 
 
 class Characteristics:
-
     _characteristics: list[Characteristic]
 
     def __init__(self) -> None:
         self._characteristics = []
         self._iid_to_characteristic: dict[int, Characteristic] = {}
 
     def append(self, char: Characteristic) -> None:
@@ -56,15 +55,14 @@
         return matches
 
     def first(self, char_types=None) -> Characteristic:
         return next(self.filter(char_types=char_types))
 
 
 class Service:
-
     type: str
     iid: int
     linked: list[Service]
 
     characteristics: Characteristics
     characteristics_by_type: dict[str, Characteristic]
     accessory: Accessory
```

### Comparing `aiohomekit-2.6.5/aiohomekit/model/services/service_types.py` & `aiohomekit-2.6.6/aiohomekit/model/services/service_types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/model/services/types.py` & `aiohomekit-2.6.6/aiohomekit/model/services/types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/model/status_flags.py` & `aiohomekit-2.6.6/aiohomekit/model/status_flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,11 +15,10 @@
 #
 
 
 from enum import IntFlag
 
 
 class StatusFlags(IntFlag):
-
     UNPAIRED = 0x01
     WIFI_UNCONFIGURED = 0x02
     PROBLEM_DETECTED = 0x04
```

### Comparing `aiohomekit-2.6.5/aiohomekit/pdu.py` & `aiohomekit-2.6.6/aiohomekit/pdu.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,27 +35,25 @@
 STRUCT_H_UNPACK = struct.Struct("<H").unpack
 
 STRUCT_BB_PACK = struct.Struct("<BB").pack
 STRUCT_BB_UNPACK = struct.Struct("<BB").unpack
 
 
 class OpCode(Enum):
-
     CHAR_SIG_READ = 0x01
     CHAR_WRITE = 0x02
     CHAR_READ = 0x03
     CHAR_TIMED_WRITE = 0x04
     CHAR_EXEC_WRITE = 0x05
     SERV_SIG_READ = 0x06
     CHAR_CONFIG = 0x07
     PROTOCOL_CONFIG = 0x08
 
 
 class PDUStatus(EnumWithDescription):
-
     SUCCESS = 0, "Success"
     UNSUPPORTED_PDU = 1, "Unsupported PDU"
     MAX_PROCEDURES = 2, "Max procedures"
     INSUFFICIENT_AUTHORIZATION = 3, "Insufficient authorization"
     INVALID_INSTANCE_ID = 4, "Invalid instance ID"
     INSUFFICIENT_AUTHENTICATION = 5, "Insufficient authentication"
     INVALID_REQUEST = 6, "Invalid request"
```

### Comparing `aiohomekit-2.6.5/aiohomekit/protocol/__init__.py` & `aiohomekit-2.6.6/aiohomekit/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/protocol/statuscodes.py` & `aiohomekit-2.6.6/aiohomekit/protocol/statuscodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # limitations under the License.
 #
 
 from aiohomekit.enum import EnumWithDescription
 
 
 class HapStatusCode(EnumWithDescription):
-
     SUCCESS = 0, "This specifies a success for the request."
     INSUFFICIENT_PRIVILEGES = -70401, "Request denied due to insufficient privileges."
     UNABLE_TO_COMMUNICATE = (
         -70402,
         "Unable to communicate with requested service, e.g. the power to the accessory was turned off.",
     )
     RESOURCE_BUSY = -70403, "Resource is busy, try again."
```

### Comparing `aiohomekit-2.6.5/aiohomekit/protocol/tlv.py` & `aiohomekit-2.6.6/aiohomekit/protocol/tlv.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/testing.py` & `aiohomekit-2.6.6/aiohomekit/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,26 +45,24 @@
     b"/9j/2wBDAAMCAgICAgMCAgIDAwMDBAYEBAQEBAgGBgUGCQgKCgkICQkKDA8MCgsOCwkJDRE"
     b"NDg8QEBEQCgwSExIQEw8QEBD/yQALCAABAAEBAREA/8wABgAQEAX/2gAIAQEAAD8A0s8g/9k="
 )
 
 
 @dataclass
 class FakeDescription:
-
     name: str = "TestDevice"
     id: str = "00:00:00:00:00:00"
     model: str = "TestDevice"
     status_flags: StatusFlags = StatusFlags.UNPAIRED
     config_num: int = 1
     state_num: int = 1
     category: Categories = Categories.OTHER
 
 
 class FakeDiscovery(AbstractDiscovery):
-
     description = FakeDescription()
 
     def __init__(
         self, controller: FakeController, device_id: str, accessories: Accessories
     ):
         self.controller = controller
         self.accessories = accessories
@@ -160,26 +158,26 @@
             char.set_value(value)
             changed.append((char.service.accessory.aid, char.iid))
 
         self._send_events(changed)
 
     def update_aid_iid(self, characteristics):
         changed = []
-        for (aid, iid, value) in characteristics:
+        for aid, iid, value in characteristics:
             self.characteristics[(aid, iid)].set_value(value)
             changed.append((aid, iid))
 
         self._send_events(changed)
 
     def _send_events(self, changed):
         if not self.events_enabled:
             return
 
         event = {}
-        for (aid, iid) in changed:
+        for aid, iid in changed:
             if (aid, iid) not in self.pairing.subscriptions:
                 continue
             event[(aid, iid)] = {"value": self.characteristics[(aid, iid)].get_value()}
 
         if not event:
             return
 
@@ -302,15 +300,15 @@
 
     async def put_characteristics(self, characteristics):
         """Fake implementation of put_characteristics."""
         self._ensure_connected()
 
         filtered = []
         results = {}
-        for (aid, cid, value) in characteristics:
+        for aid, cid, value in characteristics:
             accessory = self.accessories.aid(aid)
             char = accessory.characteristics.iid(cid)
             if char.status != HapStatusCode.SUCCESS:
                 results[(aid, cid)] = {"status": char.status.value}
                 continue
             filtered.append((aid, cid, value))
         self.testing.update_aid_iid(filtered)
```

### Comparing `aiohomekit-2.6.5/aiohomekit/tlv8.py` & `aiohomekit-2.6.6/aiohomekit/tlv8.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/utils.py` & `aiohomekit-2.6.6/aiohomekit/utils.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/uuid.py` & `aiohomekit-2.6.6/aiohomekit/uuid.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/aiohomekit/zeroconf.py` & `aiohomekit-2.6.6/aiohomekit/zeroconf.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.5/pyproject.toml` & `aiohomekit-2.6.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiohomekit"
-version = "2.6.5"
+version = "2.6.6"
 description = "An asyncio HomeKit client"
 authors = ["John Carr <john.carr@unrouted.co.uk>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/Jc2k/aiohomekit"
 repository = "https://github.com/Jc2k/aiohomekit"
 keywords = ["HomeKit", "home", "automation"]
```

### Comparing `aiohomekit-2.6.5/PKG-INFO` & `aiohomekit-2.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohomekit
-Version: 2.6.5
+Version: 2.6.6
 Summary: An asyncio HomeKit client
 Home-page: https://github.com/Jc2k/aiohomekit
 License: Apache-2.0
 Keywords: HomeKit,home,automation
 Author: John Carr
 Author-email: john.carr@unrouted.co.uk
 Requires-Python: >=3.9,<4.0
```

