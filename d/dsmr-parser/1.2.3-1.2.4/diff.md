# Comparing `tmp/dsmr-parser-1.2.3.tar.gz` & `tmp/dsmr-parser-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsmr-parser-1.2.3.tar", last modified: Tue Apr 18 18:50:01 2023, max compression
+gzip compressed data, was "dsmr-parser-1.2.4.tar", last modified: Tue Jul 11 20:04:44 2023, max compression
```

## Comparing `dsmr-parser-1.2.3.tar` & `dsmr-parser-1.2.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 nigel     (1000) nigel     (1000)        0 2023-04-18 18:50:01.561324 dsmr-parser-1.2.3/
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     1089 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/LICENSE
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      297 2023-04-18 18:50:01.561324 dsmr-parser-1.2.3/PKG-INFO
--rw-rw-r--   0 nigel     (1000) nigel     (1000)    10844 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/README.rst
-drwxrwxr-x   0 nigel     (1000) nigel     (1000)        0 2023-04-18 18:50:01.561324 dsmr-parser-1.2.3/dsmr_parser/
--rw-rw-r--   0 nigel     (1000) nigel     (1000)        0 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/dsmr_parser/__init__.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     2406 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/dsmr_parser/__main__.py
-drwxrwxr-x   0 nigel     (1000) nigel     (1000)        0 2023-04-18 18:50:01.561324 dsmr-parser-1.2.3/dsmr_parser/clients/
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      345 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/dsmr_parser/clients/__init__.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     6147 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/dsmr_parser/clients/filereader.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     6287 2023-02-12 17:32:14.000000 dsmr-parser-1.2.3/dsmr_parser/clients/protocol.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     2168 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/dsmr_parser/clients/rfxtrx_protocol.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     4520 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/dsmr_parser/clients/serial_.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      639 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/dsmr_parser/clients/settings.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     2738 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/dsmr_parser/clients/socket_.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     1543 2023-04-12 08:58:40.000000 dsmr-parser-1.2.3/dsmr_parser/clients/telegram_buffer.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)       89 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/dsmr_parser/exceptions.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     6268 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/dsmr_parser/obis_name_mapping.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     6201 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/dsmr_parser/obis_references.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)    11887 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/dsmr_parser/objects.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)    14128 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/dsmr_parser/parsers.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      340 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/dsmr_parser/profile_generic_specifications.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)    19026 2023-02-12 17:32:14.000000 dsmr-parser-1.2.3/dsmr_parser/telegram_specifications.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      755 2023-02-12 17:32:14.000000 dsmr-parser-1.2.3/dsmr_parser/value_types.py
-drwxrwxr-x   0 nigel     (1000) nigel     (1000)        0 2023-04-18 18:50:01.561324 dsmr-parser-1.2.3/dsmr_parser.egg-info/
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      297 2023-04-18 18:50:01.000000 dsmr-parser-1.2.3/dsmr_parser.egg-info/PKG-INFO
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     1093 2023-04-18 18:50:01.000000 dsmr-parser-1.2.3/dsmr_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 nigel     (1000) nigel     (1000)        1 2023-04-18 18:50:01.000000 dsmr-parser-1.2.3/dsmr_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 nigel     (1000) nigel     (1000)       63 2023-04-18 18:50:01.000000 dsmr-parser-1.2.3/dsmr_parser.egg-info/entry_points.txt
--rw-rw-r--   0 nigel     (1000) nigel     (1000)       72 2023-04-18 18:50:01.000000 dsmr-parser-1.2.3/dsmr_parser.egg-info/requires.txt
--rw-rw-r--   0 nigel     (1000) nigel     (1000)       12 2023-04-18 18:50:01.000000 dsmr-parser-1.2.3/dsmr_parser.egg-info/top_level.txt
--rw-rw-r--   0 nigel     (1000) nigel     (1000)       38 2023-04-18 18:50:01.561324 dsmr-parser-1.2.3/setup.cfg
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      630 2023-04-18 18:46:29.000000 dsmr-parser-1.2.3/setup.py
-drwxrwxr-x   0 nigel     (1000) nigel     (1000)        0 2023-04-18 18:50:01.561324 dsmr-parser-1.2.3/test/
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      663 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/test/test_filereader.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)    17716 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/test/test_parse_fluvius.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     9825 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/test/test_parse_iskra_ie.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     4788 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/test/test_parse_sagemcom_t210_d_r.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     4845 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/test/test_parse_v2_2.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     5305 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/test/test_parse_v3.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)    13023 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/test/test_parse_v4_2.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)    14431 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/test/test_parse_v5.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     2327 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/test/test_protocol.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     2436 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/test/test_rfxtrx_protocol.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     3535 2023-04-12 08:39:00.000000 dsmr-parser-1.2.3/test/test_telegram_buffer.py
+drwxr-xr-x   0 nigel     (1000) nigel     (1000)        0 2023-07-11 20:04:44.147405 dsmr-parser-1.2.4/
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     1089 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/LICENSE
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      269 2023-07-11 20:04:44.147405 dsmr-parser-1.2.4/PKG-INFO
+-rw-r--r--   0 nigel     (1000) nigel     (1000)    10844 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/README.rst
+drwxr-xr-x   0 nigel     (1000) nigel     (1000)        0 2023-07-11 20:04:44.146406 dsmr-parser-1.2.4/dsmr_parser/
+-rw-r--r--   0 nigel     (1000) nigel     (1000)        0 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/dsmr_parser/__init__.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     2406 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/dsmr_parser/__main__.py
+drwxr-xr-x   0 nigel     (1000) nigel     (1000)        0 2023-07-11 20:04:44.146406 dsmr-parser-1.2.4/dsmr_parser/clients/
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      345 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/dsmr_parser/clients/__init__.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     6147 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/dsmr_parser/clients/filereader.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     6287 2023-02-12 17:32:14.000000 dsmr-parser-1.2.4/dsmr_parser/clients/protocol.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     2168 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/dsmr_parser/clients/rfxtrx_protocol.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     4520 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/dsmr_parser/clients/serial_.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      639 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/dsmr_parser/clients/settings.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     2738 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/dsmr_parser/clients/socket_.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     1543 2023-04-12 08:58:40.000000 dsmr-parser-1.2.4/dsmr_parser/clients/telegram_buffer.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)       89 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/dsmr_parser/exceptions.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     6268 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/dsmr_parser/obis_name_mapping.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     6201 2023-04-18 18:46:02.000000 dsmr-parser-1.2.4/dsmr_parser/obis_references.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)    11887 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/dsmr_parser/objects.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)    14128 2023-04-18 18:46:02.000000 dsmr-parser-1.2.4/dsmr_parser/parsers.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      340 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/dsmr_parser/profile_generic_specifications.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)    19034 2023-07-11 19:56:39.000000 dsmr-parser-1.2.4/dsmr_parser/telegram_specifications.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      755 2023-02-12 17:32:14.000000 dsmr-parser-1.2.4/dsmr_parser/value_types.py
+drwxr-xr-x   0 nigel     (1000) nigel     (1000)        0 2023-07-11 20:04:44.146406 dsmr-parser-1.2.4/dsmr_parser.egg-info/
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      269 2023-07-11 20:04:44.000000 dsmr-parser-1.2.4/dsmr_parser.egg-info/PKG-INFO
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     1093 2023-07-11 20:04:44.000000 dsmr-parser-1.2.4/dsmr_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 nigel     (1000) nigel     (1000)        1 2023-07-11 20:04:44.000000 dsmr-parser-1.2.4/dsmr_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 nigel     (1000) nigel     (1000)       62 2023-07-11 20:04:44.000000 dsmr-parser-1.2.4/dsmr_parser.egg-info/entry_points.txt
+-rw-r--r--   0 nigel     (1000) nigel     (1000)       72 2023-07-11 20:04:44.000000 dsmr-parser-1.2.4/dsmr_parser.egg-info/requires.txt
+-rw-r--r--   0 nigel     (1000) nigel     (1000)       12 2023-07-11 20:04:44.000000 dsmr-parser-1.2.4/dsmr_parser.egg-info/top_level.txt
+-rw-r--r--   0 nigel     (1000) nigel     (1000)       38 2023-07-11 20:04:44.147405 dsmr-parser-1.2.4/setup.cfg
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      630 2023-07-11 19:58:20.000000 dsmr-parser-1.2.4/setup.py
+drwxr-xr-x   0 nigel     (1000) nigel     (1000)        0 2023-07-11 20:04:44.147405 dsmr-parser-1.2.4/test/
+-rw-r--r--   0 nigel     (1000) nigel     (1000)      663 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/test/test_filereader.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)    16710 2023-07-11 19:56:39.000000 dsmr-parser-1.2.4/test/test_parse_fluvius.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     9825 2023-04-18 18:46:02.000000 dsmr-parser-1.2.4/test/test_parse_iskra_ie.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     4788 2023-01-28 10:18:52.000000 dsmr-parser-1.2.4/test/test_parse_sagemcom_t210_d_r.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     4845 2023-04-18 18:46:02.000000 dsmr-parser-1.2.4/test/test_parse_v2_2.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     5305 2023-04-18 18:46:02.000000 dsmr-parser-1.2.4/test/test_parse_v3.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)    13023 2023-04-18 18:46:02.000000 dsmr-parser-1.2.4/test/test_parse_v4_2.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)    14431 2023-04-18 18:46:02.000000 dsmr-parser-1.2.4/test/test_parse_v5.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     2327 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/test/test_protocol.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     2436 2023-02-19 11:25:41.000000 dsmr-parser-1.2.4/test/test_rfxtrx_protocol.py
+-rw-r--r--   0 nigel     (1000) nigel     (1000)     3535 2023-04-12 08:39:00.000000 dsmr-parser-1.2.4/test/test_telegram_buffer.py
```

### Comparing `dsmr-parser-1.2.3/LICENSE` & `dsmr-parser-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/README.rst` & `dsmr-parser-1.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/dsmr_parser/__main__.py` & `dsmr-parser-1.2.4/dsmr_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/dsmr_parser/clients/filereader.py` & `dsmr-parser-1.2.4/dsmr_parser/clients/filereader.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/dsmr_parser/clients/protocol.py` & `dsmr-parser-1.2.4/dsmr_parser/clients/protocol.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/dsmr_parser/clients/rfxtrx_protocol.py` & `dsmr-parser-1.2.4/dsmr_parser/clients/rfxtrx_protocol.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/dsmr_parser/clients/serial_.py` & `dsmr-parser-1.2.4/dsmr_parser/clients/serial_.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/dsmr_parser/clients/settings.py` & `dsmr-parser-1.2.4/dsmr_parser/clients/settings.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/dsmr_parser/clients/socket_.py` & `dsmr-parser-1.2.4/dsmr_parser/clients/socket_.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/dsmr_parser/clients/telegram_buffer.py` & `dsmr-parser-1.2.4/dsmr_parser/clients/telegram_buffer.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/dsmr_parser/obis_name_mapping.py` & `dsmr-parser-1.2.4/dsmr_parser/obis_name_mapping.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/dsmr_parser/obis_references.py` & `dsmr-parser-1.2.4/dsmr_parser/obis_references.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/dsmr_parser/objects.py` & `dsmr-parser-1.2.4/dsmr_parser/objects.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/dsmr_parser/parsers.py` & `dsmr-parser-1.2.4/dsmr_parser/parsers.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/dsmr_parser/telegram_specifications.py` & `dsmr-parser-1.2.4/dsmr_parser/telegram_specifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
 ALL = (V2_2, V3, V4, V5)
 
 BELGIUM_FLUVIUS = {
     'checksum_support': True,
     'objects': {
         obis.BELGIUM_VERSION_INFORMATION: CosemParser(ValueParser(str)),
-        obis.EQUIPMENT_IDENTIFIER: CosemParser(ValueParser(str)),
+        obis.BELGIUM_EQUIPMENT_IDENTIFIER: CosemParser(ValueParser(str)),
         obis.P1_MESSAGE_TIMESTAMP: CosemParser(ValueParser(timestamp)),
         obis.ELECTRICITY_USED_TARIFF_1: CosemParser(ValueParser(Decimal)),
         obis.ELECTRICITY_USED_TARIFF_2: CosemParser(ValueParser(Decimal)),
         obis.ELECTRICITY_DELIVERED_TARIFF_1: CosemParser(ValueParser(Decimal)),
         obis.ELECTRICITY_DELIVERED_TARIFF_2: CosemParser(ValueParser(Decimal)),
         obis.ELECTRICITY_ACTIVE_TARIFF: CosemParser(ValueParser(str)),
         obis.BELGIUM_CURRENT_AVERAGE_DEMAND: CosemParser(ValueParser(Decimal)),
```

### Comparing `dsmr-parser-1.2.3/dsmr_parser/value_types.py` & `dsmr-parser-1.2.4/dsmr_parser/value_types.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/dsmr_parser.egg-info/SOURCES.txt` & `dsmr-parser-1.2.4/dsmr_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/setup.py` & `dsmr-parser-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 setup(
     name='dsmr-parser',
     description='Library to parse Dutch Smart Meter Requirements (DSMR)',
     author='Nigel Dokter and many others',
     author_email='mail@nldr.net',
     license='MIT',
     url='https://github.com/ndokter/dsmr_parser',
-    version='1.2.3',
+    version='1.2.4',
     packages=find_packages(exclude=('test', 'test.*')),
     install_requires=[
         'pyserial>=3,<4',
         'pyserial-asyncio<1',
         'pytz',
         'Tailer==0.4.1',
         'dlms_cosem==21.3.2'
```

### Comparing `dsmr-parser-1.2.3/test/test_filereader.py` & `dsmr-parser-1.2.4/test/test_filereader.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/test/test_parse_fluvius.py` & `dsmr-parser-1.2.4/test/test_parse_fluvius.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from decimal import Decimal
 
 import datetime
 import unittest
 
 import pytz
 
-from dsmr_parser import obis_references as obis
 from dsmr_parser import telegram_specifications
 from dsmr_parser.exceptions import InvalidChecksumError, ParseError
 from dsmr_parser.objects import CosemObject, MBusObject, MBusObjectPeak
 from dsmr_parser.parsers import TelegramParser
 from test.example_telegrams import TELEGRAM_FLUVIUS_V171
 
 
@@ -20,259 +19,259 @@
         parser = TelegramParser(telegram_specifications.BELGIUM_FLUVIUS)
         try:
             result = parser.parse(TELEGRAM_FLUVIUS_V171, throw_ex=True)
         except Exception as ex:
             assert False, f"parse trigged an exception {ex}"
 
         # BELGIUM_VERSION_INFORMATION (0-0:96.1.4)
-        assert isinstance(result[obis.BELGIUM_VERSION_INFORMATION], CosemObject)
-        assert result[obis.BELGIUM_VERSION_INFORMATION].unit is None
-        assert isinstance(result[obis.BELGIUM_VERSION_INFORMATION].value, str)
-        assert result[obis.BELGIUM_VERSION_INFORMATION].value == '50217'
+        assert isinstance(result.BELGIUM_VERSION_INFORMATION, CosemObject)
+        assert result.BELGIUM_VERSION_INFORMATION.unit is None
+        assert isinstance(result.BELGIUM_VERSION_INFORMATION.value, str)
+        assert result.BELGIUM_VERSION_INFORMATION.value == '50217'
 
         # EQUIPMENT_IDENTIFIER (0-0:96.1.1)
-        assert isinstance(result[obis.EQUIPMENT_IDENTIFIER], CosemObject)
-        assert result[obis.EQUIPMENT_IDENTIFIER].unit is None
-        assert isinstance(result[obis.EQUIPMENT_IDENTIFIER].value, str)
-        assert result[obis.EQUIPMENT_IDENTIFIER].value == '3153414733313031303231363035'
+        assert isinstance(result.BELGIUM_EQUIPMENT_IDENTIFIER, CosemObject)
+        assert result.BELGIUM_EQUIPMENT_IDENTIFIER.unit is None
+        assert isinstance(result.BELGIUM_EQUIPMENT_IDENTIFIER.value, str)
+        assert result.BELGIUM_EQUIPMENT_IDENTIFIER.value == '3153414733313031303231363035'
 
         # P1_MESSAGE_TIMESTAMP (0-0:1.0.0)
-        assert isinstance(result[obis.P1_MESSAGE_TIMESTAMP], CosemObject)
-        assert result[obis.P1_MESSAGE_TIMESTAMP].unit is None
-        assert isinstance(result[obis.P1_MESSAGE_TIMESTAMP].value, datetime.datetime)
-        assert result[obis.P1_MESSAGE_TIMESTAMP].value == \
+        assert isinstance(result.P1_MESSAGE_TIMESTAMP, CosemObject)
+        assert result.P1_MESSAGE_TIMESTAMP.unit is None
+        assert isinstance(result.P1_MESSAGE_TIMESTAMP.value, datetime.datetime)
+        assert result.P1_MESSAGE_TIMESTAMP.value == \
             pytz.timezone("Europe/Brussels").localize(datetime.datetime(2020, 5, 12, 13, 54, 9))
 
         # ELECTRICITY_USED_TARIFF_1 (1-0:1.8.1)
-        assert isinstance(result[obis.ELECTRICITY_USED_TARIFF_1], CosemObject)
-        assert result[obis.ELECTRICITY_USED_TARIFF_1].unit == 'kWh'
-        assert isinstance(result[obis.ELECTRICITY_USED_TARIFF_1].value, Decimal)
-        assert result[obis.ELECTRICITY_USED_TARIFF_1].value == Decimal('0.034')
+        assert isinstance(result.ELECTRICITY_USED_TARIFF_1, CosemObject)
+        assert result.ELECTRICITY_USED_TARIFF_1.unit == 'kWh'
+        assert isinstance(result.ELECTRICITY_USED_TARIFF_1.value, Decimal)
+        assert result.ELECTRICITY_USED_TARIFF_1.value == Decimal('0.034')
 
         # ELECTRICITY_USED_TARIFF_2 (1-0:1.8.2)
-        assert isinstance(result[obis.ELECTRICITY_USED_TARIFF_2], CosemObject)
-        assert result[obis.ELECTRICITY_USED_TARIFF_2].unit == 'kWh'
-        assert isinstance(result[obis.ELECTRICITY_USED_TARIFF_2].value, Decimal)
-        assert result[obis.ELECTRICITY_USED_TARIFF_2].value == Decimal('15.758')
+        assert isinstance(result.ELECTRICITY_USED_TARIFF_2, CosemObject)
+        assert result.ELECTRICITY_USED_TARIFF_2.unit == 'kWh'
+        assert isinstance(result.ELECTRICITY_USED_TARIFF_2.value, Decimal)
+        assert result.ELECTRICITY_USED_TARIFF_2.value == Decimal('15.758')
 
         # ELECTRICITY_DELIVERED_TARIFF_1 (1-0:2.8.1)
-        assert isinstance(result[obis.ELECTRICITY_DELIVERED_TARIFF_1], CosemObject)
-        assert result[obis.ELECTRICITY_DELIVERED_TARIFF_1].unit == 'kWh'
-        assert isinstance(result[obis.ELECTRICITY_DELIVERED_TARIFF_1].value, Decimal)
-        assert result[obis.ELECTRICITY_DELIVERED_TARIFF_1].value == Decimal('0.000')
+        assert isinstance(result.ELECTRICITY_DELIVERED_TARIFF_1, CosemObject)
+        assert result.ELECTRICITY_DELIVERED_TARIFF_1.unit == 'kWh'
+        assert isinstance(result.ELECTRICITY_DELIVERED_TARIFF_1.value, Decimal)
+        assert result.ELECTRICITY_DELIVERED_TARIFF_1.value == Decimal('0.000')
 
         # ELECTRICITY_DELIVERED_TARIFF_2 (1-0:2.8.2)
-        assert isinstance(result[obis.ELECTRICITY_DELIVERED_TARIFF_2], CosemObject)
-        assert result[obis.ELECTRICITY_DELIVERED_TARIFF_2].unit == 'kWh'
-        assert isinstance(result[obis.ELECTRICITY_DELIVERED_TARIFF_2].value, Decimal)
-        assert result[obis.ELECTRICITY_DELIVERED_TARIFF_2].value == Decimal('0.011')
+        assert isinstance(result.ELECTRICITY_DELIVERED_TARIFF_2, CosemObject)
+        assert result.ELECTRICITY_DELIVERED_TARIFF_2.unit == 'kWh'
+        assert isinstance(result.ELECTRICITY_DELIVERED_TARIFF_2.value, Decimal)
+        assert result.ELECTRICITY_DELIVERED_TARIFF_2.value == Decimal('0.011')
 
         # ELECTRICITY_ACTIVE_TARIFF (0-0:96.14.0)
-        assert isinstance(result[obis.ELECTRICITY_ACTIVE_TARIFF], CosemObject)
-        assert result[obis.ELECTRICITY_ACTIVE_TARIFF].unit is None
-        assert isinstance(result[obis.ELECTRICITY_ACTIVE_TARIFF].value, str)
-        assert result[obis.ELECTRICITY_ACTIVE_TARIFF].value == '0001'
+        assert isinstance(result.ELECTRICITY_ACTIVE_TARIFF, CosemObject)
+        assert result.ELECTRICITY_ACTIVE_TARIFF.unit is None
+        assert isinstance(result.ELECTRICITY_ACTIVE_TARIFF.value, str)
+        assert result.ELECTRICITY_ACTIVE_TARIFF.value == '0001'
 
         # BELGIUM_CURRENT_AVERAGE_DEMAND (1-0:1.4.0)
-        assert isinstance(result[obis.BELGIUM_CURRENT_AVERAGE_DEMAND], CosemObject)
-        assert result[obis.BELGIUM_CURRENT_AVERAGE_DEMAND].unit == 'kW'
-        assert isinstance(result[obis.BELGIUM_CURRENT_AVERAGE_DEMAND].value, Decimal)
-        assert result[obis.BELGIUM_CURRENT_AVERAGE_DEMAND].value == Decimal('2.351')
+        assert isinstance(result.BELGIUM_CURRENT_AVERAGE_DEMAND, CosemObject)
+        assert result.BELGIUM_CURRENT_AVERAGE_DEMAND.unit == 'kW'
+        assert isinstance(result.BELGIUM_CURRENT_AVERAGE_DEMAND.value, Decimal)
+        assert result.BELGIUM_CURRENT_AVERAGE_DEMAND.value == Decimal('2.351')
 
         # BELGIUM_MAXIMUM_DEMAND_MONTH (1-0:1.6.0)
-        assert isinstance(result[obis.BELGIUM_MAXIMUM_DEMAND_MONTH], MBusObject)
-        assert result[obis.BELGIUM_MAXIMUM_DEMAND_MONTH].unit == 'kW'
-        assert isinstance(result[obis.BELGIUM_MAXIMUM_DEMAND_MONTH].value, Decimal)
-        assert result[obis.BELGIUM_MAXIMUM_DEMAND_MONTH].value == Decimal('2.589')
-        assert isinstance(result[obis.BELGIUM_MAXIMUM_DEMAND_MONTH].datetime, datetime.datetime)
-        assert result[obis.BELGIUM_MAXIMUM_DEMAND_MONTH].datetime == \
+        assert isinstance(result.BELGIUM_MAXIMUM_DEMAND_MONTH, MBusObject)
+        assert result.BELGIUM_MAXIMUM_DEMAND_MONTH.unit == 'kW'
+        assert isinstance(result.BELGIUM_MAXIMUM_DEMAND_MONTH.value, Decimal)
+        assert result.BELGIUM_MAXIMUM_DEMAND_MONTH.value == Decimal('2.589')
+        assert isinstance(result.BELGIUM_MAXIMUM_DEMAND_MONTH.datetime, datetime.datetime)
+        assert result.BELGIUM_MAXIMUM_DEMAND_MONTH.datetime == \
             pytz.timezone("Europe/Brussels").localize(datetime.datetime(2020, 5, 9, 13, 45, 58))
 
         # BELGIUM_MAXIMUM_DEMAND_13_MONTHS (0-0:98.1.0) Value 0
-        assert isinstance(result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][0], MBusObjectPeak)
-        assert result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][0].unit == 'kW'
-        assert isinstance(result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][0].value, Decimal)
-        assert result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][0].value == Decimal('3.695')
-        assert isinstance(result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][0].datetime, datetime.datetime)
-        assert result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][0].datetime == \
+        assert isinstance(result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[0], MBusObjectPeak)
+        assert result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[0].unit == 'kW'
+        assert isinstance(result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[0].value, Decimal)
+        assert result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[0].value == Decimal('3.695')
+        assert isinstance(result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[0].datetime, datetime.datetime)
+        assert result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[0].datetime == \
             pytz.timezone("Europe/Brussels").localize(datetime.datetime(2020, 5, 1, 0, 0, 0))
-        assert isinstance(result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][0].occurred, datetime.datetime)
-        assert result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][0].occurred == \
+        assert isinstance(result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[0].occurred, datetime.datetime)
+        assert result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[0].occurred == \
             pytz.timezone("Europe/Brussels").localize(datetime.datetime(2020, 4, 23, 19, 25, 38))
         # BELGIUM_MAXIMUM_DEMAND_13_MONTHS (0-0:98.1.0) Value 1
-        assert isinstance(result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][1], MBusObjectPeak)
-        assert result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][1].unit == 'kW'
-        assert isinstance(result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][1].value, Decimal)
-        assert result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][1].value == Decimal('5.980')
-        assert isinstance(result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][1].datetime, datetime.datetime)
-        assert result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][1].datetime == \
+        assert isinstance(result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[1], MBusObjectPeak)
+        assert result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[1].unit == 'kW'
+        assert isinstance(result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[1].value, Decimal)
+        assert result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[1].value == Decimal('5.980')
+        assert isinstance(result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[1].datetime, datetime.datetime)
+        assert result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[1].datetime == \
             pytz.timezone("Europe/Brussels").localize(datetime.datetime(2020, 4, 1, 0, 0, 0))
-        assert isinstance(result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][1].occurred, datetime.datetime)
-        assert result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][1].occurred == \
+        assert isinstance(result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[1].occurred, datetime.datetime)
+        assert result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[1].occurred == \
             pytz.timezone("Europe/Brussels").localize(datetime.datetime(2020, 3, 5, 12, 21, 39))
         # BELGIUM_MAXIMUM_DEMAND_13_MONTHS (0-0:98.1.0) Value 2
-        assert isinstance(result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][2], MBusObjectPeak)
-        assert result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][2].unit == 'kW'
-        assert isinstance(result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][2].value, Decimal)
-        assert result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][2].value == Decimal('4.318')
-        assert isinstance(result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][2].datetime, datetime.datetime)
-        assert result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][2].datetime == \
+        assert isinstance(result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[2], MBusObjectPeak)
+        assert result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[2].unit == 'kW'
+        assert isinstance(result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[2].value, Decimal)
+        assert result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[2].value == Decimal('4.318')
+        assert isinstance(result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[2].datetime, datetime.datetime)
+        assert result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[2].datetime == \
             pytz.timezone("Europe/Brussels").localize(datetime.datetime(2020, 3, 1, 0, 0, 0))
-        assert isinstance(result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][2].occurred, datetime.datetime)
-        assert result[obis.BELGIUM_MAXIMUM_DEMAND_13_MONTHS][2].occurred == \
+        assert isinstance(result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[2].occurred, datetime.datetime)
+        assert result.BELGIUM_MAXIMUM_DEMAND_13_MONTHS[2].occurred == \
             pytz.timezone("Europe/Brussels").localize(datetime.datetime(2020, 2, 10, 3, 54, 21))
 
         # CURRENT_ELECTRICITY_USAGE (1-0:1.7.0)
-        assert isinstance(result[obis.CURRENT_ELECTRICITY_USAGE], CosemObject)
-        assert result[obis.CURRENT_ELECTRICITY_USAGE].unit == 'kW'
-        assert isinstance(result[obis.CURRENT_ELECTRICITY_USAGE].value, Decimal)
-        assert result[obis.CURRENT_ELECTRICITY_USAGE].value == Decimal('0.000')
+        assert isinstance(result.CURRENT_ELECTRICITY_USAGE, CosemObject)
+        assert result.CURRENT_ELECTRICITY_USAGE.unit == 'kW'
+        assert isinstance(result.CURRENT_ELECTRICITY_USAGE.value, Decimal)
+        assert result.CURRENT_ELECTRICITY_USAGE.value == Decimal('0.000')
 
         # CURRENT_ELECTRICITY_DELIVERY (1-0:2.7.0)
-        assert isinstance(result[obis.CURRENT_ELECTRICITY_DELIVERY], CosemObject)
-        assert result[obis.CURRENT_ELECTRICITY_DELIVERY].unit == 'kW'
-        assert isinstance(result[obis.CURRENT_ELECTRICITY_DELIVERY].value, Decimal)
-        assert result[obis.CURRENT_ELECTRICITY_DELIVERY].value == Decimal('0.000')
+        assert isinstance(result.CURRENT_ELECTRICITY_DELIVERY, CosemObject)
+        assert result.CURRENT_ELECTRICITY_DELIVERY.unit == 'kW'
+        assert isinstance(result.CURRENT_ELECTRICITY_DELIVERY.value, Decimal)
+        assert result.CURRENT_ELECTRICITY_DELIVERY.value == Decimal('0.000')
 
         # INSTANTANEOUS_ACTIVE_POWER_L1_POSITIVE (1-0:21.7.0)
-        assert isinstance(result[obis.INSTANTANEOUS_ACTIVE_POWER_L1_POSITIVE], CosemObject)
-        assert result[obis.INSTANTANEOUS_ACTIVE_POWER_L1_POSITIVE].unit == 'kW'
-        assert isinstance(result[obis.INSTANTANEOUS_ACTIVE_POWER_L1_POSITIVE].value, Decimal)
-        assert result[obis.INSTANTANEOUS_ACTIVE_POWER_L1_POSITIVE].value == Decimal('0.000')
+        assert isinstance(result.INSTANTANEOUS_ACTIVE_POWER_L1_POSITIVE, CosemObject)
+        assert result.INSTANTANEOUS_ACTIVE_POWER_L1_POSITIVE.unit == 'kW'
+        assert isinstance(result.INSTANTANEOUS_ACTIVE_POWER_L1_POSITIVE.value, Decimal)
+        assert result.INSTANTANEOUS_ACTIVE_POWER_L1_POSITIVE.value == Decimal('0.000')
 
         # INSTANTANEOUS_ACTIVE_POWER_L2_POSITIVE (1-0:41.7.0)
-        assert isinstance(result[obis.INSTANTANEOUS_ACTIVE_POWER_L2_POSITIVE], CosemObject)
-        assert result[obis.INSTANTANEOUS_ACTIVE_POWER_L2_POSITIVE].unit == 'kW'
-        assert isinstance(result[obis.INSTANTANEOUS_ACTIVE_POWER_L2_POSITIVE].value, Decimal)
-        assert result[obis.INSTANTANEOUS_ACTIVE_POWER_L2_POSITIVE].value == Decimal('0.000')
+        assert isinstance(result.INSTANTANEOUS_ACTIVE_POWER_L2_POSITIVE, CosemObject)
+        assert result.INSTANTANEOUS_ACTIVE_POWER_L2_POSITIVE.unit == 'kW'
+        assert isinstance(result.INSTANTANEOUS_ACTIVE_POWER_L2_POSITIVE.value, Decimal)
+        assert result.INSTANTANEOUS_ACTIVE_POWER_L2_POSITIVE.value == Decimal('0.000')
 
         # INSTANTANEOUS_ACTIVE_POWER_L3_POSITIVE (1-0:61.7.0)
-        assert isinstance(result[obis.INSTANTANEOUS_ACTIVE_POWER_L3_POSITIVE], CosemObject)
-        assert result[obis.INSTANTANEOUS_ACTIVE_POWER_L3_POSITIVE].unit == 'kW'
-        assert isinstance(result[obis.INSTANTANEOUS_ACTIVE_POWER_L3_POSITIVE].value, Decimal)
-        assert result[obis.INSTANTANEOUS_ACTIVE_POWER_L3_POSITIVE].value == Decimal('0.000')
+        assert isinstance(result.INSTANTANEOUS_ACTIVE_POWER_L3_POSITIVE, CosemObject)
+        assert result.INSTANTANEOUS_ACTIVE_POWER_L3_POSITIVE.unit == 'kW'
+        assert isinstance(result.INSTANTANEOUS_ACTIVE_POWER_L3_POSITIVE.value, Decimal)
+        assert result.INSTANTANEOUS_ACTIVE_POWER_L3_POSITIVE.value == Decimal('0.000')
 
         # INSTANTANEOUS_ACTIVE_POWER_L1_NEGATIVE (1-0:22.7.0)
-        assert isinstance(result[obis.INSTANTANEOUS_ACTIVE_POWER_L1_NEGATIVE], CosemObject)
-        assert result[obis.INSTANTANEOUS_ACTIVE_POWER_L1_NEGATIVE].unit == 'kW'
-        assert isinstance(result[obis.INSTANTANEOUS_ACTIVE_POWER_L1_NEGATIVE].value, Decimal)
-        assert result[obis.INSTANTANEOUS_ACTIVE_POWER_L1_NEGATIVE].value == Decimal('0.000')
+        assert isinstance(result.INSTANTANEOUS_ACTIVE_POWER_L1_NEGATIVE, CosemObject)
+        assert result.INSTANTANEOUS_ACTIVE_POWER_L1_NEGATIVE.unit == 'kW'
+        assert isinstance(result.INSTANTANEOUS_ACTIVE_POWER_L1_NEGATIVE.value, Decimal)
+        assert result.INSTANTANEOUS_ACTIVE_POWER_L1_NEGATIVE.value == Decimal('0.000')
 
         # INSTANTANEOUS_ACTIVE_POWER_L2_NEGATIVE (1-0:42.7.0)
-        assert isinstance(result[obis.INSTANTANEOUS_ACTIVE_POWER_L2_NEGATIVE], CosemObject)
-        assert result[obis.INSTANTANEOUS_ACTIVE_POWER_L2_NEGATIVE].unit == 'kW'
-        assert isinstance(result[obis.INSTANTANEOUS_ACTIVE_POWER_L2_NEGATIVE].value, Decimal)
-        assert result[obis.INSTANTANEOUS_ACTIVE_POWER_L2_NEGATIVE].value == Decimal('0.000')
+        assert isinstance(result.INSTANTANEOUS_ACTIVE_POWER_L2_NEGATIVE, CosemObject)
+        assert result.INSTANTANEOUS_ACTIVE_POWER_L2_NEGATIVE.unit == 'kW'
+        assert isinstance(result.INSTANTANEOUS_ACTIVE_POWER_L2_NEGATIVE.value, Decimal)
+        assert result.INSTANTANEOUS_ACTIVE_POWER_L2_NEGATIVE.value == Decimal('0.000')
 
         # INSTANTANEOUS_ACTIVE_POWER_L3_NEGATIVE (1-0:62.7.0)
-        assert isinstance(result[obis.INSTANTANEOUS_ACTIVE_POWER_L3_NEGATIVE], CosemObject)
-        assert result[obis.INSTANTANEOUS_ACTIVE_POWER_L3_NEGATIVE].unit == 'kW'
-        assert isinstance(result[obis.INSTANTANEOUS_ACTIVE_POWER_L3_NEGATIVE].value, Decimal)
-        assert result[obis.INSTANTANEOUS_ACTIVE_POWER_L3_NEGATIVE].value == Decimal('0.000')
+        assert isinstance(result.INSTANTANEOUS_ACTIVE_POWER_L3_NEGATIVE, CosemObject)
+        assert result.INSTANTANEOUS_ACTIVE_POWER_L3_NEGATIVE.unit == 'kW'
+        assert isinstance(result.INSTANTANEOUS_ACTIVE_POWER_L3_NEGATIVE.value, Decimal)
+        assert result.INSTANTANEOUS_ACTIVE_POWER_L3_NEGATIVE.value == Decimal('0.000')
 
         # INSTANTANEOUS_VOLTAGE_L1 (1-0:32.7.0)
-        assert isinstance(result[obis.INSTANTANEOUS_VOLTAGE_L1], CosemObject)
-        assert result[obis.INSTANTANEOUS_VOLTAGE_L1].unit == 'V'
-        assert isinstance(result[obis.INSTANTANEOUS_VOLTAGE_L1].value, Decimal)
-        assert result[obis.INSTANTANEOUS_VOLTAGE_L1].value == Decimal('234.7')
+        assert isinstance(result.INSTANTANEOUS_VOLTAGE_L1, CosemObject)
+        assert result.INSTANTANEOUS_VOLTAGE_L1.unit == 'V'
+        assert isinstance(result.INSTANTANEOUS_VOLTAGE_L1.value, Decimal)
+        assert result.INSTANTANEOUS_VOLTAGE_L1.value == Decimal('234.7')
 
         # INSTANTANEOUS_VOLTAGE_L2 (1-0:52.7.0)
-        assert isinstance(result[obis.INSTANTANEOUS_VOLTAGE_L2], CosemObject)
-        assert result[obis.INSTANTANEOUS_VOLTAGE_L2].unit == 'V'
-        assert isinstance(result[obis.INSTANTANEOUS_VOLTAGE_L2].value, Decimal)
-        assert result[obis.INSTANTANEOUS_VOLTAGE_L2].value == Decimal('234.7')
+        assert isinstance(result.INSTANTANEOUS_VOLTAGE_L2, CosemObject)
+        assert result.INSTANTANEOUS_VOLTAGE_L2.unit == 'V'
+        assert isinstance(result.INSTANTANEOUS_VOLTAGE_L2.value, Decimal)
+        assert result.INSTANTANEOUS_VOLTAGE_L2.value == Decimal('234.7')
 
         # INSTANTANEOUS_VOLTAGE_L3 (1-0:72.7.0)
-        assert isinstance(result[obis.INSTANTANEOUS_VOLTAGE_L3], CosemObject)
-        assert result[obis.INSTANTANEOUS_VOLTAGE_L3].unit == 'V'
-        assert isinstance(result[obis.INSTANTANEOUS_VOLTAGE_L3].value, Decimal)
-        assert result[obis.INSTANTANEOUS_VOLTAGE_L3].value == Decimal('234.7')
+        assert isinstance(result.INSTANTANEOUS_VOLTAGE_L3, CosemObject)
+        assert result.INSTANTANEOUS_VOLTAGE_L3.unit == 'V'
+        assert isinstance(result.INSTANTANEOUS_VOLTAGE_L3.value, Decimal)
+        assert result.INSTANTANEOUS_VOLTAGE_L3.value == Decimal('234.7')
 
         # INSTANTANEOUS_CURRENT_L1 (1-0:31.7.0)
-        assert isinstance(result[obis.INSTANTANEOUS_CURRENT_L1], CosemObject)
-        assert result[obis.INSTANTANEOUS_CURRENT_L1].unit == 'A'
-        assert isinstance(result[obis.INSTANTANEOUS_CURRENT_L1].value, Decimal)
-        assert result[obis.INSTANTANEOUS_CURRENT_L1].value == Decimal('0.000')
+        assert isinstance(result.INSTANTANEOUS_CURRENT_L1, CosemObject)
+        assert result.INSTANTANEOUS_CURRENT_L1.unit == 'A'
+        assert isinstance(result.INSTANTANEOUS_CURRENT_L1.value, Decimal)
+        assert result.INSTANTANEOUS_CURRENT_L1.value == Decimal('0.000')
 
         # INSTANTANEOUS_CURRENT_L2 (1-0:51.7.0)
-        assert isinstance(result[obis.INSTANTANEOUS_CURRENT_L2], CosemObject)
-        assert result[obis.INSTANTANEOUS_CURRENT_L2].unit == 'A'
-        assert isinstance(result[obis.INSTANTANEOUS_CURRENT_L2].value, Decimal)
-        assert result[obis.INSTANTANEOUS_CURRENT_L2].value == Decimal('0.000')
+        assert isinstance(result.INSTANTANEOUS_CURRENT_L2, CosemObject)
+        assert result.INSTANTANEOUS_CURRENT_L2.unit == 'A'
+        assert isinstance(result.INSTANTANEOUS_CURRENT_L2.value, Decimal)
+        assert result.INSTANTANEOUS_CURRENT_L2.value == Decimal('0.000')
 
         # INSTANTANEOUS_CURRENT_L3 (1-0:71.7.0)
-        assert isinstance(result[obis.INSTANTANEOUS_CURRENT_L3], CosemObject)
-        assert result[obis.INSTANTANEOUS_CURRENT_L3].unit == 'A'
-        assert isinstance(result[obis.INSTANTANEOUS_CURRENT_L3].value, Decimal)
-        assert result[obis.INSTANTANEOUS_CURRENT_L3].value == Decimal('0.000')
+        assert isinstance(result.INSTANTANEOUS_CURRENT_L3, CosemObject)
+        assert result.INSTANTANEOUS_CURRENT_L3.unit == 'A'
+        assert isinstance(result.INSTANTANEOUS_CURRENT_L3.value, Decimal)
+        assert result.INSTANTANEOUS_CURRENT_L3.value == Decimal('0.000')
 
         # ACTUAL_SWITCH_POSITION (0-0:96.3.10)
-        assert isinstance(result[obis.ACTUAL_SWITCH_POSITION], CosemObject)
-        assert result[obis.ACTUAL_SWITCH_POSITION].unit is None
-        assert isinstance(result[obis.ACTUAL_SWITCH_POSITION].value, int)
-        assert result[obis.ACTUAL_SWITCH_POSITION].value == 1
+        assert isinstance(result.ACTUAL_SWITCH_POSITION, CosemObject)
+        assert result.ACTUAL_SWITCH_POSITION.unit is None
+        assert isinstance(result.ACTUAL_SWITCH_POSITION.value, int)
+        assert result.ACTUAL_SWITCH_POSITION.value == 1
 
         # BELGIUM_MAX_POWER_PER_PHASE (0-0:17.0.0)
-        assert isinstance(result[obis.BELGIUM_MAX_POWER_PER_PHASE], CosemObject)
-        assert result[obis.BELGIUM_MAX_POWER_PER_PHASE].unit == 'kW'
-        assert isinstance(result[obis.BELGIUM_MAX_POWER_PER_PHASE].value, Decimal)
-        assert result[obis.BELGIUM_MAX_POWER_PER_PHASE].value == Decimal('999.9')
+        assert isinstance(result.BELGIUM_MAX_POWER_PER_PHASE, CosemObject)
+        assert result.BELGIUM_MAX_POWER_PER_PHASE.unit == 'kW'
+        assert isinstance(result.BELGIUM_MAX_POWER_PER_PHASE.value, Decimal)
+        assert result.BELGIUM_MAX_POWER_PER_PHASE.value == Decimal('999.9')
 
         # BELGIUM_MAX_POWER_PER_PHASE (1-0:31.4.0)
-        assert isinstance(result[obis.BELGIUM_MAX_CURRENT_PER_PHASE], CosemObject)
-        assert result[obis.BELGIUM_MAX_CURRENT_PER_PHASE].unit == 'A'
-        assert isinstance(result[obis.BELGIUM_MAX_CURRENT_PER_PHASE].value, Decimal)
-        assert result[obis.BELGIUM_MAX_CURRENT_PER_PHASE].value == Decimal('999')
+        assert isinstance(result.BELGIUM_MAX_CURRENT_PER_PHASE, CosemObject)
+        assert result.BELGIUM_MAX_CURRENT_PER_PHASE.unit == 'A'
+        assert isinstance(result.BELGIUM_MAX_CURRENT_PER_PHASE.value, Decimal)
+        assert result.BELGIUM_MAX_CURRENT_PER_PHASE.value == Decimal('999')
 
         # TEXT_MESSAGE (0-0:96.13.0)
-        assert isinstance(result[obis.TEXT_MESSAGE], CosemObject)
-        assert result[obis.TEXT_MESSAGE].unit is None
-        assert result[obis.TEXT_MESSAGE].value is None
+        assert isinstance(result.TEXT_MESSAGE, CosemObject)
+        assert result.TEXT_MESSAGE.unit is None
+        assert result.TEXT_MESSAGE.value is None
 
         # BELGIUM_MBUS1_DEVICE_TYPE (0-1:24.1.0)
-        assert isinstance(result[obis.BELGIUM_MBUS1_DEVICE_TYPE], CosemObject)
-        assert result[obis.BELGIUM_MBUS1_DEVICE_TYPE].unit is None
-        assert isinstance(result[obis.BELGIUM_MBUS1_DEVICE_TYPE].value, int)
-        assert result[obis.BELGIUM_MBUS1_DEVICE_TYPE].value == 3
+        assert isinstance(result.BELGIUM_MBUS1_DEVICE_TYPE, CosemObject)
+        assert result.BELGIUM_MBUS1_DEVICE_TYPE.unit is None
+        assert isinstance(result.BELGIUM_MBUS1_DEVICE_TYPE.value, int)
+        assert result.BELGIUM_MBUS1_DEVICE_TYPE.value == 3
 
         # BELGIUM_MBUS1_EQUIPMENT_IDENTIFIER (0-1:96.1.1)
-        assert isinstance(result[obis.BELGIUM_MBUS1_EQUIPMENT_IDENTIFIER], CosemObject)
-        assert result[obis.BELGIUM_MBUS1_EQUIPMENT_IDENTIFIER].unit is None
-        assert isinstance(result[obis.BELGIUM_MBUS1_EQUIPMENT_IDENTIFIER].value, str)
-        assert result[obis.BELGIUM_MBUS1_EQUIPMENT_IDENTIFIER].value == '37464C4F32313139303333373333'
+        assert isinstance(result.BELGIUM_MBUS1_EQUIPMENT_IDENTIFIER, CosemObject)
+        assert result.BELGIUM_MBUS1_EQUIPMENT_IDENTIFIER.unit is None
+        assert isinstance(result.BELGIUM_MBUS1_EQUIPMENT_IDENTIFIER.value, str)
+        assert result.BELGIUM_MBUS1_EQUIPMENT_IDENTIFIER.value == '37464C4F32313139303333373333'
 
         # BELGIUM_MBUS1_VALVE_POSITION (0-1:24.4.0)
-        assert isinstance(result[obis.BELGIUM_MBUS1_VALVE_POSITION], CosemObject)
-        assert result[obis.BELGIUM_MBUS1_VALVE_POSITION].unit is None
-        assert isinstance(result[obis.BELGIUM_MBUS1_VALVE_POSITION].value, int)
-        assert result[obis.BELGIUM_MBUS1_VALVE_POSITION].value == 1
+        assert isinstance(result.BELGIUM_MBUS1_VALVE_POSITION, CosemObject)
+        assert result.BELGIUM_MBUS1_VALVE_POSITION.unit is None
+        assert isinstance(result.BELGIUM_MBUS1_VALVE_POSITION.value, int)
+        assert result.BELGIUM_MBUS1_VALVE_POSITION.value == 1
 
         # BELGIUM_MBUS1_METER_READING2 (0-1:24.2.3)
-        assert isinstance(result[obis.BELGIUM_MBUS1_METER_READING2], MBusObject)
-        assert result[obis.BELGIUM_MBUS1_METER_READING2].unit == 'm3'
-        assert isinstance(result[obis.BELGIUM_MBUS1_METER_READING2].value, Decimal)
-        assert result[obis.BELGIUM_MBUS1_METER_READING2].value == Decimal('112.384')
+        assert isinstance(result.BELGIUM_MBUS1_METER_READING2, MBusObject)
+        assert result.BELGIUM_MBUS1_METER_READING2.unit == 'm3'
+        assert isinstance(result.BELGIUM_MBUS1_METER_READING2.value, Decimal)
+        assert result.BELGIUM_MBUS1_METER_READING2.value == Decimal('112.384')
 
         # BELGIUM_MBUS2_DEVICE_TYPE (0-2:24.1.0)
-        assert isinstance(result[obis.BELGIUM_MBUS2_DEVICE_TYPE], CosemObject)
-        assert result[obis.BELGIUM_MBUS2_DEVICE_TYPE].unit is None
-        assert isinstance(result[obis.BELGIUM_MBUS2_DEVICE_TYPE].value, int)
-        assert result[obis.BELGIUM_MBUS2_DEVICE_TYPE].value == 7
+        assert isinstance(result.BELGIUM_MBUS2_DEVICE_TYPE, CosemObject)
+        assert result.BELGIUM_MBUS2_DEVICE_TYPE.unit is None
+        assert isinstance(result.BELGIUM_MBUS2_DEVICE_TYPE.value, int)
+        assert result.BELGIUM_MBUS2_DEVICE_TYPE.value == 7
 
         # BELGIUM_MBUS2_EQUIPMENT_IDENTIFIER (0-2:96.1.1)
-        assert isinstance(result[obis.BELGIUM_MBUS2_EQUIPMENT_IDENTIFIER], CosemObject)
-        assert result[obis.BELGIUM_MBUS2_EQUIPMENT_IDENTIFIER].unit is None
-        assert isinstance(result[obis.BELGIUM_MBUS2_EQUIPMENT_IDENTIFIER].value, str)
-        assert result[obis.BELGIUM_MBUS2_EQUIPMENT_IDENTIFIER].value == '3853414731323334353637383930'
+        assert isinstance(result.BELGIUM_MBUS2_EQUIPMENT_IDENTIFIER, CosemObject)
+        assert result.BELGIUM_MBUS2_EQUIPMENT_IDENTIFIER.unit is None
+        assert isinstance(result.BELGIUM_MBUS2_EQUIPMENT_IDENTIFIER.value, str)
+        assert result.BELGIUM_MBUS2_EQUIPMENT_IDENTIFIER.value == '3853414731323334353637383930'
 
         # BELGIUM_MBUS2_METER_READING1 (0-1:24.2.1)
-        assert isinstance(result[obis.BELGIUM_MBUS2_METER_READING1], MBusObject)
-        assert result[obis.BELGIUM_MBUS2_METER_READING1].unit == 'm3'
-        assert isinstance(result[obis.BELGIUM_MBUS2_METER_READING1].value, Decimal)
-        assert result[obis.BELGIUM_MBUS2_METER_READING1].value == Decimal('872.234')
+        assert isinstance(result.BELGIUM_MBUS2_METER_READING1, MBusObject)
+        assert result.BELGIUM_MBUS2_METER_READING1.unit == 'm3'
+        assert isinstance(result.BELGIUM_MBUS2_METER_READING1.value, Decimal)
+        assert result.BELGIUM_MBUS2_METER_READING1.value == Decimal('872.234')
 
     def test_checksum_valid(self):
         # No exception is raised.
         TelegramParser.validate_checksum(TELEGRAM_FLUVIUS_V171)
 
     def test_checksum_invalid(self):
         # Remove the electricty used data value. This causes the checksum to
```

### Comparing `dsmr-parser-1.2.3/test/test_parse_iskra_ie.py` & `dsmr-parser-1.2.4/test/test_parse_iskra_ie.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/test/test_parse_sagemcom_t210_d_r.py` & `dsmr-parser-1.2.4/test/test_parse_sagemcom_t210_d_r.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/test/test_parse_v2_2.py` & `dsmr-parser-1.2.4/test/test_parse_v2_2.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/test/test_parse_v3.py` & `dsmr-parser-1.2.4/test/test_parse_v3.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/test/test_parse_v4_2.py` & `dsmr-parser-1.2.4/test/test_parse_v4_2.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/test/test_parse_v5.py` & `dsmr-parser-1.2.4/test/test_parse_v5.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/test/test_protocol.py` & `dsmr-parser-1.2.4/test/test_protocol.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/test/test_rfxtrx_protocol.py` & `dsmr-parser-1.2.4/test/test_rfxtrx_protocol.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.3/test/test_telegram_buffer.py` & `dsmr-parser-1.2.4/test/test_telegram_buffer.py`

 * *Files identical despite different names*

