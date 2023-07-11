# Comparing `tmp/libfwsi-python-20230114.tar.gz` & `tmp/libfwsi-python-20230710.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfwsi-python-20230114.tar", last modified: Mon Jan 30 06:08:07 2023, max compression
+gzip compressed data, was "libfwsi-python-20230710.tar", last modified: Tue Jul 11 16:28:43 2023, max compression
```

## Comparing `libfwsi-python-20230114.tar` & `libfwsi-python-20230710.tar`

### file list

```diff
@@ -1,756 +1,755 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:05.000000 libfwsi-20230114/libfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4246 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3731 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_format_class_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9704 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_store.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_format_class_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2244 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_property_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1216 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16442 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_set.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3827 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1895 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_libfole.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_store.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29986 2023-01-30 05:53:08.000000 libfwsi-20230114/libfwps/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7534 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_property_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12048 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_storage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11611 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1828 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45269 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1769 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_storage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2490 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_set.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-01-30 05:52:54.000000 libfwsi-20230114/libfwps/libfwps_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:04.000000 libfwsi-20230114/common/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2023-01-29 13:18:33.000000 libfwsi-20230114/common/config_msc.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2023-01-29 13:18:33.000000 libfwsi-20230114/common/byte_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-01-29 13:18:33.000000 libfwsi-20230114/common/common.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2023-01-29 13:18:33.000000 libfwsi-20230114/common/system_string.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      378 2023-01-14 11:06:48.000000 libfwsi-20230114/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7234 2023-01-30 05:53:19.000000 libfwsi-20230114/common/types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7236 2023-01-29 13:18:33.000000 libfwsi-20230114/common/types.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2243 2023-01-29 13:18:33.000000 libfwsi-20230114/common/config_winapi.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2023-01-29 13:18:33.000000 libfwsi-20230114/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13364 2023-01-30 05:53:19.000000 libfwsi-20230114/common/config.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2023-01-29 13:18:33.000000 libfwsi-20230114/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22883 2023-01-30 05:53:08.000000 libfwsi-20230114/common/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2023-01-29 13:18:33.000000 libfwsi-20230114/common/file_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      957 2023-01-29 13:18:33.000000 libfwsi-20230114/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12626 2023-01-30 05:53:07.000000 libfwsi-20230114/common/config.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2023-01-29 13:18:33.000000 libfwsi-20230114/common/wide_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:05.000000 libfwsi-20230114/libfole/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2023-01-30 05:52:52.000000 libfwsi-20230114/libfole/libfole_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      630 2023-01-30 05:52:52.000000 libfwsi-20230114/libfole/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-01-30 05:52:52.000000 libfwsi-20230114/libfole/libfole_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-01-30 05:52:52.000000 libfwsi-20230114/libfole/libfole_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-01-30 05:52:52.000000 libfwsi-20230114/libfole/libfole_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-01-30 05:52:52.000000 libfwsi-20230114/libfole/libfole_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-01-30 05:52:52.000000 libfwsi-20230114/libfole/libfole_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-01-30 05:52:52.000000 libfwsi-20230114/libfole/libfole_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3793 2023-01-30 05:52:52.000000 libfwsi-20230114/libfole/libfole_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-01-30 05:52:52.000000 libfwsi-20230114/libfole/libfole_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27206 2023-01-30 05:53:08.000000 libfwsi-20230114/libfole/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-01-30 05:52:52.000000 libfwsi-20230114/libfole/libfole_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1407 2023-01-30 05:52:52.000000 libfwsi-20230114/libfole/libfole_types.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:05.000000 libfwsi-20230114/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2023-01-30 05:52:51.000000 libfwsi-20230114/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2023-01-30 05:52:51.000000 libfwsi-20230114/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2023-01-30 05:52:51.000000 libfwsi-20230114/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2023-01-30 05:52:51.000000 libfwsi-20230114/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2023-01-30 05:52:51.000000 libfwsi-20230114/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2023-01-30 05:52:51.000000 libfwsi-20230114/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-01-30 05:52:51.000000 libfwsi-20230114/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-01-30 05:52:51.000000 libfwsi-20230114/libfguid/libfguid_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-01-30 05:52:51.000000 libfwsi-20230114/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27283 2023-01-30 05:53:08.000000 libfwsi-20230114/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-01-30 05:52:51.000000 libfwsi-20230114/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2023-01-30 05:52:51.000000 libfwsi-20230114/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-01-30 05:52:51.000000 libfwsi-20230114/libfguid/libfguid_extern.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1190 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/pyfwsi_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10058 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_users_property_view_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10376 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_file_entry_extension_values.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4519 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/test_library.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1411 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/pyfwsi_test_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/pyfwsi_test_item_list.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9072 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_root_folder_values.c
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3416 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13523 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_mtp_file_entry_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16888 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11884 2023-01-14 11:08:40.000000 libfwsi-20230114/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10525 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0013_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1414 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/pyfwsi_test_root_folder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0001_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_memory.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9145 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_game_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6222 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_uri_sub_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9508 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_file_entry_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10824 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_uri_values.c
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     1645 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/test_manpage.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8871 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_volume_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0005_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7077 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_control_panel_category_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9321 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_control_panel_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15227 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_item_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9721 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_network_location_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10040 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_unknown_0x74_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    37784 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/pyfwsi_test_volume.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/pyfwsi_test_extension_block.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16618 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_mtp_volume_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10355 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0000_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1394 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/pyfwsi_test_item.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/pyfwsi_test_network_location.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    83158 2023-01-30 05:53:09.000000 libfwsi-20230114/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0019_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9691 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_cdburn_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10355 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef000a_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10452 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0025_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10428 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0003_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11361 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_extension_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8990 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_delegate_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      973 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_libfwsi.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12033 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0014_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10440 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0006_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6792 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_compressed_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11887 2023-01-29 13:18:35.000000 libfwsi-20230114/tests/fwsi_test_control_panel_cpl_file_values.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:05.000000 libfwsi-20230114/pyfwsi/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2413 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_extension_block.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2548 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_extension_blocks.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2317 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_items.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-01-29 13:18:35.000000 libfwsi-20230114/pyfwsi/pyfwsi_root_folder.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_guid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15503 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_item_list.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7719 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1391 2018-07-31 03:31:38.000000 libfwsi-20230114/pyfwsi/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20503 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_item.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_integer.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-01-29 13:18:35.000000 libfwsi-20230114/pyfwsi/pyfwsi_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8497 2023-01-29 13:18:35.000000 libfwsi-20230114/pyfwsi/pyfwsi_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10901 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_file_entry.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_libclocale.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3254 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_codepage.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_integer.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_python.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8979 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_items.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53444 2023-01-30 05:53:09.000000 libfwsi-20230114/pyfwsi/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16087 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_file_entry_extension.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9661 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_extension_blocks.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_file_entry_extension.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      965 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_libfwsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2760 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_item.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16593 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_datetime.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1815 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_datetime.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_libfguid.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2891 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_guid.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4432 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_root_folder.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11022 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_network_location.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_item_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11203 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_extension_block.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1667 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_network_location.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1862 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_file_entry.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2023-01-29 13:18:34.000000 libfwsi-20230114/pyfwsi/pyfwsi_error.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2023-01-29 13:18:35.000000 libfwsi-20230114/pyfwsi/pyfwsi_volume.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:04.000000 libfwsi-20230114/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-01-30 05:52:45.000000 libfwsi-20230114/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2023-01-30 05:52:45.000000 libfwsi-20230114/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2023-01-30 05:52:45.000000 libfwsi-20230114/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      744 2023-01-30 05:52:45.000000 libfwsi-20230114/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2023-01-30 05:52:45.000000 libfwsi-20230114/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-01-30 05:52:45.000000 libfwsi-20230114/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-01-30 05:52:45.000000 libfwsi-20230114/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-01-30 05:52:45.000000 libfwsi-20230114/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2023-01-30 05:52:45.000000 libfwsi-20230114/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-01-30 05:52:45.000000 libfwsi-20230114/libclocale/libclocale_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2023-01-30 05:52:45.000000 libfwsi-20230114/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27839 2023-01-30 05:53:08.000000 libfwsi-20230114/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2023-01-30 05:52:45.000000 libfwsi-20230114/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-01-30 05:52:45.000000 libfwsi-20230114/libclocale/libclocale_libcerror.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2023-01-30 05:53:08.000000 libfwsi-20230114/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:05.000000 libfwsi-20230114/pyfwsi-python2/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1862 2023-01-14 11:07:08.000000 libfwsi-20230114/pyfwsi-python2/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53481 2023-01-30 05:53:09.000000 libfwsi-20230114/pyfwsi-python2/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2875 2022-04-27 03:41:26.000000 libfwsi-20230114/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55875 2023-01-30 05:53:05.000000 libfwsi-20230114/aclocal.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2023-01-14 11:06:50.000000 libfwsi-20230114/COPYING
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      301 2023-01-14 11:06:50.000000 libfwsi-20230114/README
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2793 2023-01-14 11:06:50.000000 libfwsi-20230114/libfwsi.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:04.000000 libfwsi-20230114/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2023-01-14 11:08:40.000000 libfwsi-20230114/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19803 2023-01-30 05:53:19.000000 libfwsi-20230114/include/libfwsi.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:04.000000 libfwsi-20230114/include/libfwsi/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3046 2023-01-29 13:18:33.000000 libfwsi-20230114/include/libfwsi/definitions.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-01-29 13:18:33.000000 libfwsi-20230114/include/libfwsi/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4884 2023-01-30 05:53:19.000000 libfwsi-20230114/include/libfwsi/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2023-01-29 13:18:33.000000 libfwsi-20230114/include/libfwsi/features.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5015 2023-01-29 13:18:33.000000 libfwsi-20230114/include/libfwsi/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2023-01-30 05:53:19.000000 libfwsi-20230114/include/libfwsi/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3044 2023-01-30 05:53:19.000000 libfwsi-20230114/include/libfwsi/definitions.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2023-01-29 13:18:33.000000 libfwsi-20230114/include/libfwsi/codepage.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2023-01-29 13:18:33.000000 libfwsi-20230114/include/libfwsi/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25865 2023-01-30 05:53:08.000000 libfwsi-20230114/include/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19803 2023-01-29 13:18:33.000000 libfwsi-20230114/include/libfwsi.h.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2023-01-30 05:53:08.000000 libfwsi-20230114/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2023-01-30 05:53:08.000000 libfwsi-20230114/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:04.000000 libfwsi-20230114/dpkg/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       22 2023-01-14 11:06:49.000000 libfwsi-20230114/dpkg/libfwsi.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      120 2023-01-14 11:06:49.000000 libfwsi-20230114/dpkg/changelog.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-01-14 11:06:49.000000 libfwsi-20230114/dpkg/libfwsi-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2023-01-30 05:53:19.000000 libfwsi-20230114/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2023-01-29 13:18:35.000000 libfwsi-20230114/dpkg/copyright
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       18 2023-01-14 11:06:49.000000 libfwsi-20230114/dpkg/libfwsi-python3.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:04.000000 libfwsi-20230114/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-01-14 11:06:49.000000 libfwsi-20230114/dpkg/source/format
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      704 2023-01-14 11:06:49.000000 libfwsi-20230114/dpkg/rules
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        3 2023-01-14 11:06:49.000000 libfwsi-20230114/dpkg/compat
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1541 2023-01-14 11:06:49.000000 libfwsi-20230114/dpkg/control
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:05.000000 libfwsi-20230114/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-01-30 05:52:50.000000 libfwsi-20230114/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30454 2023-01-30 05:53:08.000000 libfwsi-20230114/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2023-01-30 05:52:50.000000 libfwsi-20230114/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2023-01-30 05:52:49.000000 libfwsi-20230114/libfdatetime/libfdatetime_filetime.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:04.000000 libfwsi-20230114/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30693 2023-01-30 05:53:08.000000 libfwsi-20230114/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2023-01-30 05:52:48.000000 libfwsi-20230114/libcthreads/libcthreads_queue.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       91 2023-01-29 13:18:33.000000 libfwsi-20230114/AUTHORS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35409 2023-01-30 05:53:08.000000 libfwsi-20230114/config.sub
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:05.000000 libfwsi-20230114/pyfwsi-python3/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1862 2023-01-14 11:07:08.000000 libfwsi-20230114/pyfwsi-python3/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53481 2023-01-30 05:53:09.000000 libfwsi-20230114/pyfwsi-python3/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2156 2023-01-30 05:53:19.000000 libfwsi-20230114/libfwsi.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      130 2016-02-02 07:37:21.000000 libfwsi-20230114/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9756 2023-01-29 13:18:35.000000 libfwsi-20230114/manuals/libfwsi.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23082 2023-01-30 05:53:09.000000 libfwsi-20230114/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2022-07-11 05:10:26.000000 libfwsi-20230114/ABOUT-NLS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_control_panel_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_control_panel_values/fwsi_test_control_panel_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_uri_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5376 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_uri_values/fwsi_test_uri_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/libfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6294 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/libfwps/libfwps.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/libfole/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4605 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/libfole/libfole.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0000_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0000_values/fwsi_test_extension_block_0xbeef0000_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0013_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0013_values/fwsi_test_extension_block_0xbeef0013_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/pyfwsi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7597 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/pyfwsi/pyfwsi.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_users_property_view_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5424 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_users_property_view_values/fwsi_test_users_property_view_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/libclocale/libclocale.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2992 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block/fwsi_test_extension_block.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5124 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_support/fwsi_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_cdburn_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5385 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_cdburn_values/fwsi_test_cdburn_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0003_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0003_values/fwsi_test_extension_block_0xbeef0003_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0006_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0006_values/fwsi_test_extension_block_0xbeef0006_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_volume_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5385 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_volume_values/fwsi_test_volume_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_unknown_0x74_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5403 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_unknown_0x74_values/fwsi_test_unknown_0x74_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_item/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5358 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_item/fwsi_test_item.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0014_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0014_values/fwsi_test_extension_block_0xbeef0014_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_mtp_volume_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_mtp_volume_values/fwsi_test_mtp_volume_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_item_list/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5373 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_item_list/fwsi_test_item_list.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_root_folder_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_root_folder_values/fwsi_test_root_folder_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_control_panel_category_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5433 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_control_panel_category_values/fwsi_test_control_panel_category_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_mtp_file_entry_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5409 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_mtp_file_entry_values/fwsi_test_mtp_file_entry_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_control_panel_cpl_file_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5433 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_control_panel_cpl_file_values/fwsi_test_control_panel_cpl_file_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_compressed_folder_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5418 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_compressed_folder_values/fwsi_test_compressed_folder_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_network_location_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5415 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_network_location_values/fwsi_test_network_location_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/libuna/libuna.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/libfwsi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14163 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/libfwsi/libfwsi.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22831 2023-01-30 05:53:09.000000 libfwsi-20230114/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0001_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0001_values/fwsi_test_extension_block_0xbeef0001_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5118 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_error/fwsi_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_delegate_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_delegate_values/fwsi_test_delegate_values.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35022 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/libfwsi.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_uri_sub_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5388 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_uri_sub_values/fwsi_test_uri_sub_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_game_folder_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_game_folder_values/fwsi_test_game_folder_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0025_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0025_values/fwsi_test_extension_block_0xbeef0025_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef000a_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef000a_values/fwsi_test_extension_block_0xbeef000a_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_file_entry_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_file_entry_values/fwsi_test_file_entry_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0005_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0005_values/fwsi_test_extension_block_0xbeef0005_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0019_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0019_values/fwsi_test_extension_block_0xbeef0019_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/msvscpp/fwsi_test_file_entry_extension_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5427 2023-01-30 05:28:15.000000 libfwsi-20230114/msvscpp/fwsi_test_file_entry_extension_values/fwsi_test_file_entry_extension_values.vcproj
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)    11454 2023-01-14 11:07:47.000000 libfwsi-20230114/setup.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49797 2023-01-30 05:53:08.000000 libfwsi-20230114/config.guess
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-14 11:06:50.000000 libfwsi-20230114/NEWS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:06.000000 libfwsi-20230114/ossfuzz/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1330 2023-01-29 13:18:34.000000 libfwsi-20230114/ossfuzz/item_fuzzer.cc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      820 2020-07-16 10:09:37.000000 libfwsi-20230114/ossfuzz/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2023-01-29 13:18:34.000000 libfwsi-20230114/ossfuzz/item_list_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30527 2023-01-30 05:53:09.000000 libfwsi-20230114/ossfuzz/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      967 2023-01-29 13:18:34.000000 libfwsi-20230114/ossfuzz/ossfuzz_libfwsi.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2023-01-30 05:53:09.000000 libfwsi-20230114/test-driver
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1492284 2023-01-30 05:53:07.000000 libfwsi-20230114/configure
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:05.000000 libfwsi-20230114/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19794 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95123 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5908 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   129163 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101951 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98825 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    51405 2023-01-30 05:53:09.000000 libfwsi-20230114/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19595 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16696 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2023-01-30 05:52:58.000000 libfwsi-20230114/libuna/libuna_codepage_iso_8859_16.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:05.000000 libfwsi-20230114/libfwsi/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1514 2023-01-29 17:17:18.000000 libfwsi-20230114/libfwsi/libfwsi_libfwps.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16822 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_file_entry_extension_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9231 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0014_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2305 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_file_entry_extension_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_support.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0013_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_libcdata.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_libcerror.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1744 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_control_panel_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6567 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0025_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0001_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_root_folder.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1076 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi.rc.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_delegate_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_libfole.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1816 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1770 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_root_folder_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_mtp_volume_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6191 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0006_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_libfdatetime.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1865 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_users_property_view_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4099 2018-07-31 03:31:27.000000 libfwsi-20230114/libfwsi/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15176 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_file_entry_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_libuna.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8865 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_volume_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1963 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_volume_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3347 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_file_attributes.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_shell_folder_identifier.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3266 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_control_panel_identifier.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_codepage.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef000a_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5972 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0003_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7247 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_delegate_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3419 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_file_entry_extension.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2133 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_network_location_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2421 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_item_list.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11686 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_compressed_folder_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0000_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_notify.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0014_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5954 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0013_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5770 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_game_folder_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0019_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    13984 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_file_entry.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_cdburn_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10520 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_unknown_0x74_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1673 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_uri_sub_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14432 2023-01-29 13:20:45.000000 libfwsi-20230114/libfwsi/libfwsi_debug.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10190 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_shell_folder_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1074 2023-01-30 05:53:19.000000 libfwsi-20230114/libfwsi/libfwsi.rc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1190 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_file_attributes.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11581 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_volume.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_notify.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0025_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1609 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_uri_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6183 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_known_folder_identifier.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1753 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_unknown_0x74_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5435 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0005_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3431 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_definitions.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3432 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_network_location.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17745 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_mtp_volume_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_game_folder_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_support.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16884 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_mtp_file_entry_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_unused.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5811 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_root_folder_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14083 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_uri_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11244 2023-01-29 13:22:09.000000 libfwsi-20230114/libfwsi/libfwsi_users_property_view_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3769 2023-01-29 15:16:12.000000 libfwsi-20230114/libfwsi/libfwsi_item.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_compressed_folder_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_libfguid.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2317 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_file_entry.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_volume.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_control_panel_identifier.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5656 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef000a_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3098 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_root_folder.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5780 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_control_panel_category_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2625 2023-01-29 13:20:22.000000 libfwsi-20230114/libfwsi/libfwsi_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43472 2023-01-30 05:53:09.000000 libfwsi-20230114/libfwsi/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6748 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0000_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0001_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5584 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_control_panel_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    12649 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_network_location_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0003_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5798 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_cdburn_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23730 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_error.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_error.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0005_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6750 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_uri_sub_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8940 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_control_panel_cpl_file_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2646 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extern.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2792 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_known_folder_identifier.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1888 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_control_panel_category_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1888 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_control_panel_cpl_file_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    12685 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_item_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3429 2023-01-30 05:53:19.000000 libfwsi-20230114/libfwsi/libfwsi_definitions.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_libcnotify.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    25658 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_file_entry_extension.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6205 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0019_values.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0006_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    24416 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_network_location.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2117 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_file_entry_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_mtp_file_entry_values.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    40951 2023-01-29 13:18:34.000000 libfwsi-20230114/libfwsi/libfwsi_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2023-01-14 11:06:48.000000 libfwsi-20230114/libfwsi.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39333 2023-01-30 05:53:08.000000 libfwsi-20230114/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3365 2018-04-08 07:36:16.000000 libfwsi-20230114/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:04.000000 libfwsi-20230114/m4/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23765 2021-12-20 23:56:59.000000 libfwsi-20230114/m4/libuna.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7867 2023-01-30 05:27:36.000000 libfwsi-20230114/m4/libfwps.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2022-07-11 05:10:26.000000 libfwsi-20230114/m4/gettext.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      756 2020-07-16 06:06:19.000000 libfwsi-20230114/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2022-07-11 05:10:26.000000 libfwsi-20230114/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2023-01-30 05:53:03.000000 libfwsi-20230114/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2022-07-11 05:10:26.000000 libfwsi-20230114/m4/lib-ld.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2019-09-18 04:24:24.000000 libfwsi-20230114/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2022-07-11 05:10:26.000000 libfwsi-20230114/m4/lib-link.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17674 2021-12-20 23:56:59.000000 libfwsi-20230114/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2023-01-30 05:53:02.000000 libfwsi-20230114/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-07-11 05:10:26.000000 libfwsi-20230114/m4/nls.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2019-09-18 04:24:24.000000 libfwsi-20230114/m4/libclocale.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2019-09-18 04:24:24.000000 libfwsi-20230114/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2022-07-11 05:10:26.000000 libfwsi-20230114/m4/host-cpu-c-abi.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2019-09-18 04:24:24.000000 libfwsi-20230114/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2023-01-30 05:53:03.000000 libfwsi-20230114/m4/ltversion.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-01-14 11:07:12.000000 libfwsi-20230114/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2022-07-11 05:10:26.000000 libfwsi-20230114/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2023-01-30 05:53:03.000000 libfwsi-20230114/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2022-07-11 05:10:26.000000 libfwsi-20230114/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2013-09-29 07:23:40.000000 libfwsi-20230114/m4/pthread.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2018-12-15 11:06:21.000000 libfwsi-20230114/m4/common.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2019-09-18 04:24:24.000000 libfwsi-20230114/m4/libcerror.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2019-09-18 04:24:24.000000 libfwsi-20230114/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2022-07-11 05:10:26.000000 libfwsi-20230114/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2023-01-30 05:53:03.000000 libfwsi-20230114/m4/ltsugar.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3956 2019-09-18 04:24:24.000000 libfwsi-20230114/m4/libfole.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2022-07-11 05:10:26.000000 libfwsi-20230114/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2018-07-31 03:28:44.000000 libfwsi-20230114/m4/types.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2023-01-14 11:06:50.000000 libfwsi-20230114/COPYING.LESSER
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:04.000000 libfwsi-20230114/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2023-01-30 05:52:44.000000 libfwsi-20230114/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2023-01-30 05:52:44.000000 libfwsi-20230114/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-01-30 05:52:44.000000 libfwsi-20230114/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      605 2023-01-30 05:52:44.000000 libfwsi-20230114/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2023-01-30 05:52:44.000000 libfwsi-20230114/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-01-30 05:52:44.000000 libfwsi-20230114/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2023-01-30 05:52:44.000000 libfwsi-20230114/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2023-01-30 05:52:44.000000 libfwsi-20230114/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-01-30 05:52:44.000000 libfwsi-20230114/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27228 2023-01-30 05:53:08.000000 libfwsi-20230114/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-01-30 05:52:44.000000 libfwsi-20230114/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2023-01-30 05:52:44.000000 libfwsi-20230114/libcerror/libcerror_system.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:04.000000 libfwsi-20230114/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-01-30 05:52:47.000000 libfwsi-20230114/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-01-30 05:52:47.000000 libfwsi-20230114/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2023-01-30 05:52:47.000000 libfwsi-20230114/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2023-01-30 05:52:47.000000 libfwsi-20230114/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      693 2023-01-30 05:52:47.000000 libfwsi-20230114/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2023-01-30 05:52:47.000000 libfwsi-20230114/libcnotify/libcnotify_print.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2023-01-30 05:52:47.000000 libfwsi-20230114/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2023-01-30 05:52:47.000000 libfwsi-20230114/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-01-30 05:52:47.000000 libfwsi-20230114/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2023-01-30 05:52:47.000000 libfwsi-20230114/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27715 2023-01-30 05:53:08.000000 libfwsi-20230114/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2023-01-30 05:52:47.000000 libfwsi-20230114/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2023-01-30 05:52:47.000000 libfwsi-20230114/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-01-30 05:52:47.000000 libfwsi-20230114/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2023-01-30 05:53:02.000000 libfwsi-20230114/ltmain.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2023-01-30 05:53:08.000000 libfwsi-20230114/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2022-07-11 05:10:26.000000 libfwsi-20230114/config.rpath
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2023-01-30 05:53:09.000000 libfwsi-20230114/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:05.000000 libfwsi-20230114/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2022-07-11 05:10:26.000000 libfwsi-20230114/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2022-07-11 05:10:26.000000 libfwsi-20230114/po/Rules-quot
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2011-07-23 05:55:02.000000 libfwsi-20230114/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2022-07-11 05:10:26.000000 libfwsi-20230114/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2011-07-23 05:58:45.000000 libfwsi-20230114/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2016-11-04 14:33:32.000000 libfwsi-20230114/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2022-07-11 05:10:26.000000 libfwsi-20230114/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2011-07-23 05:55:02.000000 libfwsi-20230114/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1809 2023-01-30 05:53:19.000000 libfwsi-20230114/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2022-07-11 05:10:26.000000 libfwsi-20230114/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2022-07-11 05:10:26.000000 libfwsi-20230114/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2011-07-23 05:55:02.000000 libfwsi-20230114/po/boldquot.sed
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-01-30 06:08:04.000000 libfwsi-20230114/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30287 2023-01-30 05:53:08.000000 libfwsi-20230114/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2023-01-30 05:52:42.000000 libfwsi-20230114/libcdata/libcdata_btree.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      752 2023-01-14 11:06:49.000000 libfwsi-20230114/acinclude.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5847 2023-01-14 11:06:49.000000 libfwsi-20230114/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      347 2023-01-30 06:08:06.990248 libfwsi-20230114/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:41.000000 libfwsi-20230710/libfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5115 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3731 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_format_class_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9704 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_store.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_format_class_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2244 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_property_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1142 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16442 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_set.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3827 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_libfole.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_store.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29381 2023-07-11 16:09:40.000000 libfwsi-20230710/libfwps/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7534 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_property_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    60078 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2490 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_set.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-07-11 16:09:25.000000 libfwsi-20230710/libfwps/libfwps_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:40.000000 libfwsi-20230710/common/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2023-07-10 18:46:33.000000 libfwsi-20230710/common/config_msc.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2023-07-10 18:46:33.000000 libfwsi-20230710/common/byte_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-07-10 18:46:33.000000 libfwsi-20230710/common/common.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2023-07-10 18:46:33.000000 libfwsi-20230710/common/system_string.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      378 2023-07-10 18:46:29.000000 libfwsi-20230710/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2023-07-11 16:09:50.000000 libfwsi-20230710/common/types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2023-07-10 18:46:33.000000 libfwsi-20230710/common/types.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2023-07-10 18:46:33.000000 libfwsi-20230710/common/config_winapi.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2023-07-10 18:46:33.000000 libfwsi-20230710/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13364 2023-07-11 16:09:51.000000 libfwsi-20230710/common/config.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2023-07-10 18:46:33.000000 libfwsi-20230710/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22883 2023-07-11 16:09:40.000000 libfwsi-20230710/common/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2023-07-10 18:46:33.000000 libfwsi-20230710/common/file_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      957 2023-07-10 18:46:33.000000 libfwsi-20230710/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12626 2023-07-11 16:09:39.000000 libfwsi-20230710/common/config.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2023-07-10 18:46:33.000000 libfwsi-20230710/common/wide_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:41.000000 libfwsi-20230710/libfole/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2023-07-11 16:09:24.000000 libfwsi-20230710/libfole/libfole_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      630 2023-07-11 16:09:24.000000 libfwsi-20230710/libfole/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-07-11 16:09:24.000000 libfwsi-20230710/libfole/libfole_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-07-11 16:09:24.000000 libfwsi-20230710/libfole/libfole_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-07-11 16:09:24.000000 libfwsi-20230710/libfole/libfole_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-07-11 16:09:24.000000 libfwsi-20230710/libfole/libfole_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-07-11 16:09:24.000000 libfwsi-20230710/libfole/libfole_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-07-11 16:09:24.000000 libfwsi-20230710/libfole/libfole_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3793 2023-07-11 16:09:24.000000 libfwsi-20230710/libfole/libfole_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-07-11 16:09:24.000000 libfwsi-20230710/libfole/libfole_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27206 2023-07-11 16:09:40.000000 libfwsi-20230710/libfole/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-07-11 16:09:24.000000 libfwsi-20230710/libfole/libfole_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1407 2023-07-11 16:09:24.000000 libfwsi-20230710/libfole/libfole_types.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:41.000000 libfwsi-20230710/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2023-07-11 16:09:23.000000 libfwsi-20230710/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2023-07-11 16:09:23.000000 libfwsi-20230710/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2023-07-11 16:09:23.000000 libfwsi-20230710/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2023-07-11 16:09:23.000000 libfwsi-20230710/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2023-07-11 16:09:23.000000 libfwsi-20230710/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2023-07-11 16:09:23.000000 libfwsi-20230710/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-07-11 16:09:23.000000 libfwsi-20230710/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-07-11 16:09:23.000000 libfwsi-20230710/libfguid/libfguid_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-07-11 16:09:23.000000 libfwsi-20230710/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27283 2023-07-11 16:09:40.000000 libfwsi-20230710/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-07-11 16:09:23.000000 libfwsi-20230710/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2023-07-11 16:09:23.000000 libfwsi-20230710/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-07-11 16:09:23.000000 libfwsi-20230710/libfguid/libfguid_extern.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/tests/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-07-10 18:46:35.000000 libfwsi-20230710/tests/fwsi_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1190 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/pyfwsi_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10058 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_users_property_view_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2023-07-10 18:46:35.000000 libfwsi-20230710/tests/fwsi_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10376 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_file_entry_extension_values.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4527 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/test_library.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1411 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/pyfwsi_test_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/pyfwsi_test_item_list.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9072 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_root_folder_values.c
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3424 2023-07-10 18:46:35.000000 libfwsi-20230710/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13523 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_mtp_file_entry_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16888 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11884 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10525 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0013_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2023-07-10 18:46:35.000000 libfwsi-20230710/tests/fwsi_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1414 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/pyfwsi_test_root_folder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0001_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2023-07-10 18:46:35.000000 libfwsi-20230710/tests/fwsi_test_memory.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2023-07-10 18:46:35.000000 libfwsi-20230710/tests/fwsi_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9145 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_game_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6222 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_uri_sub_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9508 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_file_entry_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10824 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_uri_values.c
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2023-07-10 18:46:35.000000 libfwsi-20230710/tests/test_manpage.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8871 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_volume_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0005_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7077 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_control_panel_category_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9321 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_control_panel_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15227 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_item_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9721 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_network_location_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10040 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_unknown_0x74_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    37792 2023-07-10 18:46:35.000000 libfwsi-20230710/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/pyfwsi_test_volume.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/pyfwsi_test_extension_block.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16618 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_mtp_volume_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10355 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0000_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1394 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/pyfwsi_test_item.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/pyfwsi_test_network_location.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    83158 2023-07-11 16:09:41.000000 libfwsi-20230710/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0019_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9691 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_cdburn_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10355 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef000a_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10452 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0025_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10428 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0003_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11361 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_extension_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8990 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_delegate_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      973 2023-07-10 18:46:35.000000 libfwsi-20230710/tests/fwsi_test_libfwsi.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2023-07-10 18:46:35.000000 libfwsi-20230710/tests/fwsi_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12033 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0014_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10440 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0006_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2023-07-10 18:46:35.000000 libfwsi-20230710/tests/fwsi_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6792 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_compressed_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11887 2023-07-10 18:47:22.000000 libfwsi-20230710/tests/fwsi_test_control_panel_cpl_file_values.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/pyfwsi/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2413 2023-07-10 18:47:30.000000 libfwsi-20230710/pyfwsi/pyfwsi_extension_block.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2548 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_extension_blocks.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2317 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_items.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_root_folder.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2023-07-11 03:50:15.000000 libfwsi-20230710/pyfwsi/pyfwsi_libuna.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_guid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15503 2023-07-10 18:47:30.000000 libfwsi-20230710/pyfwsi/pyfwsi_item_list.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7719 2023-07-10 18:47:30.000000 libfwsi-20230710/pyfwsi/pyfwsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1445 2023-07-11 03:50:15.000000 libfwsi-20230710/pyfwsi/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20507 2023-07-11 03:51:27.000000 libfwsi-20230710/pyfwsi/pyfwsi_item.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_integer.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8497 2023-07-10 18:47:30.000000 libfwsi-20230710/pyfwsi/pyfwsi_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8020 2023-07-11 03:50:15.000000 libfwsi-20230710/pyfwsi/pyfwsi_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11424 2023-07-11 04:13:58.000000 libfwsi-20230710/pyfwsi/pyfwsi_file_entry.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_libclocale.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3254 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_codepage.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_integer.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_python.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8979 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_items.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54938 2023-07-11 16:09:40.000000 libfwsi-20230710/pyfwsi/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16549 2023-07-11 04:14:06.000000 libfwsi-20230710/pyfwsi/pyfwsi_file_entry_extension.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9661 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_extension_blocks.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_file_entry_extension.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      965 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_libfwsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2760 2023-07-10 18:47:30.000000 libfwsi-20230710/pyfwsi/pyfwsi_item.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16593 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_datetime.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1815 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_datetime.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_libfguid.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2891 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_guid.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4432 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_root_folder.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2023-07-11 04:04:33.000000 libfwsi-20230710/pyfwsi/pyfwsi_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11022 2023-07-11 03:51:38.000000 libfwsi-20230710/pyfwsi/pyfwsi_network_location.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2023-07-10 18:47:30.000000 libfwsi-20230710/pyfwsi/pyfwsi_item_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11207 2023-07-11 03:50:55.000000 libfwsi-20230710/pyfwsi/pyfwsi_extension_block.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1667 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_network_location.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1862 2023-07-10 18:47:30.000000 libfwsi-20230710/pyfwsi/pyfwsi_file_entry.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_error.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2023-07-10 18:46:35.000000 libfwsi-20230710/pyfwsi/pyfwsi_volume.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:41.000000 libfwsi-20230710/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-07-11 16:09:17.000000 libfwsi-20230710/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2023-07-11 16:09:17.000000 libfwsi-20230710/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2023-07-11 16:09:17.000000 libfwsi-20230710/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      744 2023-07-11 16:09:17.000000 libfwsi-20230710/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2023-07-11 16:09:17.000000 libfwsi-20230710/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-07-11 16:09:17.000000 libfwsi-20230710/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-07-11 16:09:17.000000 libfwsi-20230710/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-07-11 16:09:17.000000 libfwsi-20230710/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2023-07-11 16:09:17.000000 libfwsi-20230710/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-07-11 16:09:17.000000 libfwsi-20230710/libclocale/libclocale_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2023-07-11 16:09:17.000000 libfwsi-20230710/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27839 2023-07-11 16:09:40.000000 libfwsi-20230710/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2023-07-11 16:09:17.000000 libfwsi-20230710/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-07-11 16:09:17.000000 libfwsi-20230710/libclocale/libclocale_libcerror.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2023-07-11 16:09:39.000000 libfwsi-20230710/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/pyfwsi-python2/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1916 2023-07-11 03:50:15.000000 libfwsi-20230710/pyfwsi-python2/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54927 2023-07-11 16:09:40.000000 libfwsi-20230710/pyfwsi-python2/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2875 2022-04-27 03:41:26.000000 libfwsi-20230710/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55875 2023-07-11 16:09:37.000000 libfwsi-20230710/aclocal.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2023-07-10 18:46:29.000000 libfwsi-20230710/COPYING
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      301 2023-07-10 18:46:29.000000 libfwsi-20230710/README
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2575 2023-07-10 18:46:29.000000 libfwsi-20230710/libfwsi.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:40.000000 libfwsi-20230710/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2023-07-10 18:47:42.000000 libfwsi-20230710/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20927 2023-07-11 16:09:50.000000 libfwsi-20230710/include/libfwsi.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:40.000000 libfwsi-20230710/include/libfwsi/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3046 2023-07-10 18:46:33.000000 libfwsi-20230710/include/libfwsi/definitions.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-07-10 18:46:33.000000 libfwsi-20230710/include/libfwsi/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4884 2023-07-11 16:09:50.000000 libfwsi-20230710/include/libfwsi/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2023-07-10 18:47:42.000000 libfwsi-20230710/include/libfwsi/features.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5015 2023-07-10 18:46:33.000000 libfwsi-20230710/include/libfwsi/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2023-07-11 16:09:50.000000 libfwsi-20230710/include/libfwsi/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3044 2023-07-11 16:09:50.000000 libfwsi-20230710/include/libfwsi/definitions.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2023-07-10 18:46:33.000000 libfwsi-20230710/include/libfwsi/codepage.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2023-07-10 18:46:33.000000 libfwsi-20230710/include/libfwsi/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25865 2023-07-11 16:09:40.000000 libfwsi-20230710/include/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    20927 2023-07-11 03:58:46.000000 libfwsi-20230710/include/libfwsi.h.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2023-07-11 16:09:39.000000 libfwsi-20230710/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2023-07-11 16:09:40.000000 libfwsi-20230710/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:40.000000 libfwsi-20230710/dpkg/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       22 2023-07-10 18:46:29.000000 libfwsi-20230710/dpkg/libfwsi.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      120 2023-07-10 18:46:29.000000 libfwsi-20230710/dpkg/changelog.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-07-10 18:46:29.000000 libfwsi-20230710/dpkg/libfwsi-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2023-07-11 16:09:50.000000 libfwsi-20230710/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2023-07-10 18:46:35.000000 libfwsi-20230710/dpkg/copyright
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       18 2023-07-10 18:46:29.000000 libfwsi-20230710/dpkg/libfwsi-python3.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:40.000000 libfwsi-20230710/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-07-10 18:46:29.000000 libfwsi-20230710/dpkg/source/format
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      704 2023-07-10 18:46:29.000000 libfwsi-20230710/dpkg/rules
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        3 2023-07-10 18:46:29.000000 libfwsi-20230710/dpkg/compat
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1541 2023-07-10 18:46:29.000000 libfwsi-20230710/dpkg/control
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:41.000000 libfwsi-20230710/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30454 2023-07-11 16:09:40.000000 libfwsi-20230710/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2023-07-11 16:09:21.000000 libfwsi-20230710/libfdatetime/libfdatetime_filetime.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:41.000000 libfwsi-20230710/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30693 2023-07-11 16:09:40.000000 libfwsi-20230710/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2023-07-11 16:09:20.000000 libfwsi-20230710/libcthreads/libcthreads_queue.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       91 2023-07-10 18:46:33.000000 libfwsi-20230710/AUTHORS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35409 2023-07-11 16:09:39.000000 libfwsi-20230710/config.sub
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/pyfwsi-python3/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1916 2023-07-11 03:50:15.000000 libfwsi-20230710/pyfwsi-python3/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54927 2023-07-11 16:09:40.000000 libfwsi-20230710/pyfwsi-python3/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1938 2023-07-11 16:09:51.000000 libfwsi-20230710/libfwsi.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      130 2016-02-02 07:37:21.000000 libfwsi-20230710/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9756 2023-07-10 18:46:35.000000 libfwsi-20230710/manuals/libfwsi.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23082 2023-07-11 16:09:40.000000 libfwsi-20230710/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2022-07-11 05:10:26.000000 libfwsi-20230710/ABOUT-NLS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_control_panel_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_control_panel_values/fwsi_test_control_panel_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_uri_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5376 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_uri_values/fwsi_test_uri_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/libfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6294 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/libfwps/libfwps.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/libfole/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4605 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/libfole/libfole.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0000_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0000_values/fwsi_test_extension_block_0xbeef0000_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0013_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0013_values/fwsi_test_extension_block_0xbeef0013_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/pyfwsi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7863 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/pyfwsi/pyfwsi.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_users_property_view_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5424 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_users_property_view_values/fwsi_test_users_property_view_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/libclocale/libclocale.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2992 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block/fwsi_test_extension_block.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5124 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_support/fwsi_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_cdburn_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5385 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_cdburn_values/fwsi_test_cdburn_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0003_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0003_values/fwsi_test_extension_block_0xbeef0003_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0006_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0006_values/fwsi_test_extension_block_0xbeef0006_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_volume_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5385 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_volume_values/fwsi_test_volume_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_unknown_0x74_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5403 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_unknown_0x74_values/fwsi_test_unknown_0x74_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_item/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5358 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_item/fwsi_test_item.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0014_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0014_values/fwsi_test_extension_block_0xbeef0014_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_mtp_volume_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_mtp_volume_values/fwsi_test_mtp_volume_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_item_list/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5373 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_item_list/fwsi_test_item_list.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_root_folder_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_root_folder_values/fwsi_test_root_folder_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_control_panel_category_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5433 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_control_panel_category_values/fwsi_test_control_panel_category_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_mtp_file_entry_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5409 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_mtp_file_entry_values/fwsi_test_mtp_file_entry_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_control_panel_cpl_file_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5433 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_control_panel_cpl_file_values/fwsi_test_control_panel_cpl_file_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_compressed_folder_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5418 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_compressed_folder_values/fwsi_test_compressed_folder_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_network_location_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5415 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_network_location_values/fwsi_test_network_location_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/libuna/libuna.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/libfwsi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14163 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/libfwsi/libfwsi.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22831 2023-07-11 16:09:40.000000 libfwsi-20230710/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0001_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0001_values/fwsi_test_extension_block_0xbeef0001_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5118 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_error/fwsi_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_delegate_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_delegate_values/fwsi_test_delegate_values.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35022 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/libfwsi.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_uri_sub_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5388 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_uri_sub_values/fwsi_test_uri_sub_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_game_folder_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_game_folder_values/fwsi_test_game_folder_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0025_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0025_values/fwsi_test_extension_block_0xbeef0025_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef000a_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef000a_values/fwsi_test_extension_block_0xbeef000a_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_file_entry_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_file_entry_values/fwsi_test_file_entry_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0005_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0005_values/fwsi_test_extension_block_0xbeef0005_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0019_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0019_values/fwsi_test_extension_block_0xbeef0019_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/msvscpp/fwsi_test_file_entry_extension_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5427 2023-07-11 04:18:22.000000 libfwsi-20230710/msvscpp/fwsi_test_file_entry_extension_values/fwsi_test_file_entry_extension_values.vcproj
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)    11497 2023-07-10 18:46:53.000000 libfwsi-20230710/setup.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49797 2023-07-11 16:09:39.000000 libfwsi-20230710/config.guess
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-10 18:46:29.000000 libfwsi-20230710/NEWS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/ossfuzz/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1330 2023-07-10 18:46:34.000000 libfwsi-20230710/ossfuzz/item_fuzzer.cc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      820 2020-07-16 10:09:37.000000 libfwsi-20230710/ossfuzz/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2023-07-10 18:46:34.000000 libfwsi-20230710/ossfuzz/item_list_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30527 2023-07-11 16:09:40.000000 libfwsi-20230710/ossfuzz/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      967 2023-07-10 18:46:34.000000 libfwsi-20230710/ossfuzz/ossfuzz_libfwsi.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2023-07-11 16:09:41.000000 libfwsi-20230710/test-driver
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1556934 2023-07-11 16:09:38.000000 libfwsi-20230710/configure
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:41.000000 libfwsi-20230710/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    51405 2023-07-11 16:09:40.000000 libfwsi-20230710/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2023-07-11 16:09:29.000000 libfwsi-20230710/libuna/libuna_codepage_iso_8859_16.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:41.000000 libfwsi-20230710/libfwsi/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1514 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_libfwps.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16822 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_file_entry_extension_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9231 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0014_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2305 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_file_entry_extension_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_support.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0013_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_libcdata.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_libcerror.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1744 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_control_panel_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6567 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0025_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0001_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_root_folder.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1076 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi.rc.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_delegate_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_libfole.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1816 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1770 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_root_folder_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_mtp_volume_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6191 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0006_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_libfdatetime.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1865 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_users_property_view_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4099 2018-07-31 03:31:27.000000 libfwsi-20230710/libfwsi/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15176 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_file_entry_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_libuna.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8865 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_volume_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1963 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_volume_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3347 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_file_attributes.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_shell_folder_identifier.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3266 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_control_panel_identifier.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_codepage.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef000a_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5972 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0003_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7247 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_delegate_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3419 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_file_entry_extension.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2133 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_network_location_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2421 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_item_list.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11686 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_compressed_folder_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0000_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_notify.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0014_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5954 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0013_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5770 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_game_folder_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0019_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14734 2023-07-10 18:54:57.000000 libfwsi-20230710/libfwsi/libfwsi_file_entry.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_cdburn_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10520 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_unknown_0x74_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1673 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_uri_sub_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14432 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_debug.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10190 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_shell_folder_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1074 2023-07-11 16:09:50.000000 libfwsi-20230710/libfwsi/libfwsi.rc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1190 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_file_attributes.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11581 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_volume.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_notify.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0025_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1609 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_uri_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6183 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_known_folder_identifier.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1753 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_unknown_0x74_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5435 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0005_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3431 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_definitions.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3432 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_network_location.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17745 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_mtp_volume_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_game_folder_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_support.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16884 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_mtp_file_entry_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_unused.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5811 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_root_folder_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14083 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_uri_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11244 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_users_property_view_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3769 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_item.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_compressed_folder_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_libfguid.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2317 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_file_entry.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_volume.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_control_panel_identifier.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5656 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef000a_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3098 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_root_folder.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5780 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_control_panel_category_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2625 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43472 2023-07-11 16:09:40.000000 libfwsi-20230710/libfwsi/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6748 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0000_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0001_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5584 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_control_panel_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    12649 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_network_location_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0003_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5798 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_cdburn_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23730 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_error.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_error.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0005_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6750 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_uri_sub_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8940 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_control_panel_cpl_file_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2646 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extern.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2792 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_known_folder_identifier.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1888 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_control_panel_category_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1888 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_control_panel_cpl_file_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    12685 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_item_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3429 2023-07-11 16:09:50.000000 libfwsi-20230710/libfwsi/libfwsi_definitions.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_libcnotify.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    26408 2023-07-10 19:12:34.000000 libfwsi-20230710/libfwsi/libfwsi_file_entry_extension.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6205 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0019_values.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0006_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    24416 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_network_location.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2117 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_file_entry_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_mtp_file_entry_values.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    40951 2023-07-10 18:46:34.000000 libfwsi-20230710/libfwsi/libfwsi_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2023-07-10 18:46:29.000000 libfwsi-20230710/libfwsi.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39333 2023-07-11 16:09:40.000000 libfwsi-20230710/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3365 2018-04-08 07:36:16.000000 libfwsi-20230710/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:40.000000 libfwsi-20230710/m4/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-07-10 18:46:35.000000 libfwsi-20230710/m4/libuna.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7867 2023-01-30 05:27:36.000000 libfwsi-20230710/m4/libfwps.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2022-07-11 05:10:26.000000 libfwsi-20230710/m4/gettext.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      756 2020-07-16 06:06:19.000000 libfwsi-20230710/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2022-07-11 05:10:26.000000 libfwsi-20230710/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2023-07-11 16:09:34.000000 libfwsi-20230710/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2022-07-11 05:10:26.000000 libfwsi-20230710/m4/lib-ld.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2019-09-18 04:24:24.000000 libfwsi-20230710/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2022-07-11 05:10:26.000000 libfwsi-20230710/m4/lib-link.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17674 2021-12-20 23:56:59.000000 libfwsi-20230710/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2023-07-11 16:09:34.000000 libfwsi-20230710/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-07-11 05:10:26.000000 libfwsi-20230710/m4/nls.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2019-09-18 04:24:24.000000 libfwsi-20230710/m4/libclocale.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2019-09-18 04:24:24.000000 libfwsi-20230710/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2022-07-11 05:10:26.000000 libfwsi-20230710/m4/host-cpu-c-abi.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2019-09-18 04:24:24.000000 libfwsi-20230710/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2023-07-11 16:09:34.000000 libfwsi-20230710/m4/ltversion.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-01-14 11:07:12.000000 libfwsi-20230710/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2022-07-11 05:10:26.000000 libfwsi-20230710/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2023-07-11 16:09:34.000000 libfwsi-20230710/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2022-07-11 05:10:26.000000 libfwsi-20230710/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2013-09-29 07:23:40.000000 libfwsi-20230710/m4/pthread.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2018-12-15 11:06:21.000000 libfwsi-20230710/m4/common.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2019-09-18 04:24:24.000000 libfwsi-20230710/m4/libcerror.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2019-09-18 04:24:24.000000 libfwsi-20230710/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2022-07-11 05:10:26.000000 libfwsi-20230710/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2023-07-11 16:09:34.000000 libfwsi-20230710/m4/ltsugar.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3956 2019-09-18 04:24:24.000000 libfwsi-20230710/m4/libfole.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2022-07-11 05:10:26.000000 libfwsi-20230710/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2018-07-31 03:28:44.000000 libfwsi-20230710/m4/types.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2023-07-10 18:46:29.000000 libfwsi-20230710/COPYING.LESSER
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:40.000000 libfwsi-20230710/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2023-07-11 16:09:15.000000 libfwsi-20230710/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2023-07-11 16:09:15.000000 libfwsi-20230710/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-07-11 16:09:15.000000 libfwsi-20230710/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      605 2023-07-11 16:09:15.000000 libfwsi-20230710/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2023-07-11 16:09:15.000000 libfwsi-20230710/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-07-11 16:09:15.000000 libfwsi-20230710/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2023-07-11 16:09:15.000000 libfwsi-20230710/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2023-07-11 16:09:15.000000 libfwsi-20230710/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-07-11 16:09:15.000000 libfwsi-20230710/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27228 2023-07-11 16:09:40.000000 libfwsi-20230710/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-07-11 16:09:15.000000 libfwsi-20230710/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2023-07-11 16:09:15.000000 libfwsi-20230710/libcerror/libcerror_system.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:41.000000 libfwsi-20230710/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-07-11 16:09:18.000000 libfwsi-20230710/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-07-11 16:09:18.000000 libfwsi-20230710/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2023-07-11 16:09:18.000000 libfwsi-20230710/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2023-07-11 16:09:18.000000 libfwsi-20230710/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      693 2023-07-11 16:09:18.000000 libfwsi-20230710/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2023-07-11 16:09:18.000000 libfwsi-20230710/libcnotify/libcnotify_print.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2023-07-11 16:09:18.000000 libfwsi-20230710/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2023-07-11 16:09:18.000000 libfwsi-20230710/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-07-11 16:09:18.000000 libfwsi-20230710/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2023-07-11 16:09:18.000000 libfwsi-20230710/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27715 2023-07-11 16:09:40.000000 libfwsi-20230710/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2023-07-11 16:09:18.000000 libfwsi-20230710/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2023-07-11 16:09:18.000000 libfwsi-20230710/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-07-11 16:09:18.000000 libfwsi-20230710/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2023-07-11 16:09:34.000000 libfwsi-20230710/ltmain.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2023-07-11 16:09:39.000000 libfwsi-20230710/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2022-07-11 05:10:26.000000 libfwsi-20230710/config.rpath
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2023-07-11 16:09:41.000000 libfwsi-20230710/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:42.000000 libfwsi-20230710/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2022-07-11 05:10:26.000000 libfwsi-20230710/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2022-07-11 05:10:26.000000 libfwsi-20230710/po/Rules-quot
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2011-07-23 05:55:02.000000 libfwsi-20230710/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2022-07-11 05:10:26.000000 libfwsi-20230710/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2011-07-23 05:58:45.000000 libfwsi-20230710/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2016-11-04 14:33:32.000000 libfwsi-20230710/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2022-07-11 05:10:26.000000 libfwsi-20230710/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2011-07-23 05:55:02.000000 libfwsi-20230710/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1809 2023-07-11 16:09:50.000000 libfwsi-20230710/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2022-07-11 05:10:26.000000 libfwsi-20230710/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2022-07-11 05:10:26.000000 libfwsi-20230710/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2011-07-23 05:55:02.000000 libfwsi-20230710/po/boldquot.sed
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:28:41.000000 libfwsi-20230710/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30287 2023-07-11 16:09:40.000000 libfwsi-20230710/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2023-07-11 16:09:14.000000 libfwsi-20230710/libcdata/libcdata_btree.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      752 2023-07-10 18:46:29.000000 libfwsi-20230710/acinclude.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5847 2023-07-10 18:46:29.000000 libfwsi-20230710/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      347 2023-07-11 16:28:43.433041 libfwsi-20230710/PKG-INFO
```

### Comparing `libfwsi-20230114/libfwps/libfwps_record.h` & `libfwsi-20230710/libfwps/libfwps_record.h`

 * *Files 18% similar despite different names*

```diff
@@ -126,14 +126,20 @@
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_64bit_integer(
      libfwps_record_t *record,
      uint64_t *value_64bit,
      libcerror_error_t **error );
 
 LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_filetime(
+     libfwps_record_t *record,
+     uint64_t *filetime,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_floating_point(
      libfwps_record_t *record,
      double *value_floating_point,
      libcerror_error_t **error );
 
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_utf8_string_size(
@@ -158,14 +164,40 @@
 int libfwps_record_get_data_as_utf16_string(
      libfwps_record_t *record,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      libcerror_error_t **error );
 
 LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf8_path_string_size(
+     libfwps_record_t *record,
+     size_t *utf8_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf8_path_string(
+     libfwps_record_t *record,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf16_path_string_size(
+     libfwps_record_t *record,
+     size_t *utf16_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf16_path_string(
+     libfwps_record_t *record,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_guid(
      libfwps_record_t *record,
      uint8_t *guid_data,
      size_t guid_data_size,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
```

### Comparing `libfwsi-20230114/libfwps/libfwps_format_class_identifier.c` & `libfwsi-20230710/libfwps/libfwps_format_class_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_libcdata.h` & `libfwsi-20230710/libfwps/libfwps_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_extern.h` & `libfwsi-20230710/libfwps/libfwps_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_store.c` & `libfwsi-20230710/libfwps/libfwps_store.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_codepage.h` & `libfwsi-20230710/libfwps/libfwps_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_format_class_identifier.h` & `libfwsi-20230710/libfwps/libfwps_format_class_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_property_identifier.h` & `libfwsi-20230710/libfwps/libfwps_property_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_libcnotify.h` & `libfwsi-20230710/libfwps/libfwps_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/Makefile.am` & `libfwsi-20230710/libfwps/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,18 @@
 	libfwps_libcnotify.h \
 	libfwps_libfguid.h \
 	libfwps_libfole.h \
 	libfwps_libuna.h \
 	libfwps_property_identifier.c libfwps_property_identifier.h \
 	libfwps_record.c libfwps_record.h \
 	libfwps_set.c libfwps_set.h \
-	libfwps_storage.c libfwps_storage.h \
 	libfwps_store.c libfwps_store.h \
 	libfwps_support.c libfwps_support.h \
 	libfwps_types.h \
-	libfwps_unused.h \
-	libfwps_value.c libfwps_value.h
+	libfwps_unused.h
 endif
 
 MAINTAINERCLEANFILES = \
 	Makefile.in
 
 distclean: clean
 	/bin/rm -f Makefile
```

### Comparing `libfwsi-20230114/libfwps/libfwps_libfguid.h` & `libfwsi-20230710/libfwps/libfwps_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_set.c` & `libfwsi-20230710/libfwps/libfwps_set.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_definitions.h` & `libfwsi-20230710/libfwps/libfwps_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwps/definitions.h> are copied here
  * for local use of libfwps
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWPS_VERSION					20230130
+#define LIBFWPS_VERSION					20230711
 
 /* The version string
  */
-#define LIBFWPS_VERSION_STRING				"20230130"
+#define LIBFWPS_VERSION_STRING				"20230711"
 
 /* The byte order definitions
  */
 #define LIBFWPS_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWPS_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The value types
```

### Comparing `libfwsi-20230114/libfwps/libfwps_libuna.h` & `libfwsi-20230710/libfwps/libfwps_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_value.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_russian.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows Serialized Property Value functions
+ * MacRussian codepage functions
  *
- * Copyright (C) 2013-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,62 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFWPS_INTERNAL_VALUE_H )
-#define _LIBFWPS_INTERNAL_VALUE_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_RUSSIAN_H )
+#define _LIBUNA_CODEPAGE_MAC_RUSSIAN_H
 
 #include <common.h>
 #include <types.h>
 
-#include "libfwps_extern.h"
-#include "libfwps_libcerror.h"
-#include "libfwps_types.h"
+#include "libuna_libcerror.h"
+#include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-typedef struct libfwps_internal_value libfwps_internal_value_t;
-
-struct libfwps_internal_value
-{
-	/* The type
-	 */
-	uint8_t type;
-
-	/* The size
-	 */
-	uint32_t size;
-};
-
-int libfwps_value_initialize(
-     libfwps_value_t **value,
-     uint8_t value_type,
-     libcerror_error_t **error );
-
-LIBFWPS_EXTERN \
-int libfwps_value_free(
-     libfwps_value_t **value,
-     libcerror_error_t **error );
-
-int libfwps_internal_value_free(
-     libfwps_internal_value_t **internal_value,
+int libuna_codepage_mac_russian_copy_from_byte_stream(
+     libuna_unicode_character_t *unicode_character,
+     const uint8_t *byte_stream,
+     size_t byte_stream_size,
+     size_t *byte_stream_index,
      libcerror_error_t **error );
 
-LIBFWPS_EXTERN \
-int libfwps_value_copy_from_byte_stream(
-     libfwps_value_t *value,
-     const uint8_t *byte_stream,
+int libuna_codepage_mac_russian_copy_to_byte_stream(
+     libuna_unicode_character_t unicode_character,
+     uint8_t *byte_stream,
      size_t byte_stream_size,
-     int ascii_codepage,
+     size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBFWPS_INTERNAL_VALUE_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_RUSSIAN_H ) */
```

### Comparing `libfwsi-20230114/libfwps/libfwps_libfole.h` & `libfwsi-20230710/libfwps/libfwps_libfole.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_store.h` & `libfwsi-20230710/libfwps/libfwps_store.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_error.c` & `libfwsi-20230710/libfwps/libfwps_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_support.c` & `libfwsi-20230710/libfwps/libfwps_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/Makefile.in` & `libfwsi-20230710/libfwps/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -120,24 +120,21 @@
 	libfwps_extern.h libfwps_error.c libfwps_error.h \
 	libfwps_format_class_identifier.c \
 	libfwps_format_class_identifier.h libfwps_libcdata.h \
 	libfwps_libcerror.h libfwps_libcnotify.h libfwps_libfguid.h \
 	libfwps_libfole.h libfwps_libuna.h \
 	libfwps_property_identifier.c libfwps_property_identifier.h \
 	libfwps_record.c libfwps_record.h libfwps_set.c libfwps_set.h \
-	libfwps_storage.c libfwps_storage.h libfwps_store.c \
-	libfwps_store.h libfwps_support.c libfwps_support.h \
-	libfwps_types.h libfwps_unused.h libfwps_value.c \
-	libfwps_value.h
+	libfwps_store.c libfwps_store.h libfwps_support.c \
+	libfwps_support.h libfwps_types.h libfwps_unused.h
 @HAVE_LOCAL_LIBFWPS_TRUE@am_libfwps_la_OBJECTS = libfwps_error.lo \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_format_class_identifier.lo \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_property_identifier.lo \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_record.lo libfwps_set.lo \
-@HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_storage.lo libfwps_store.lo \
-@HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_support.lo libfwps_value.lo
+@HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_store.lo libfwps_support.lo
 libfwps_la_OBJECTS = $(am_libfwps_la_OBJECTS)
 AM_V_lt = $(am__v_lt_@AM_V@)
 am__v_lt_ = $(am__v_lt_@AM_DEFAULT_V@)
 am__v_lt_0 = --silent
 am__v_lt_1 = 
 @HAVE_LOCAL_LIBFWPS_TRUE@am_libfwps_la_rpath =
 AM_V_P = $(am__v_P_@AM_V@)
@@ -155,16 +152,15 @@
 DEFAULT_INCLUDES = -I.@am__isrc@ -I$(top_builddir)/common
 depcomp = $(SHELL) $(top_srcdir)/depcomp
 am__maybe_remake_depfiles = depfiles
 am__depfiles_remade = ./$(DEPDIR)/libfwps_error.Plo \
 	./$(DEPDIR)/libfwps_format_class_identifier.Plo \
 	./$(DEPDIR)/libfwps_property_identifier.Plo \
 	./$(DEPDIR)/libfwps_record.Plo ./$(DEPDIR)/libfwps_set.Plo \
-	./$(DEPDIR)/libfwps_storage.Plo ./$(DEPDIR)/libfwps_store.Plo \
-	./$(DEPDIR)/libfwps_support.Plo ./$(DEPDIR)/libfwps_value.Plo
+	./$(DEPDIR)/libfwps_store.Plo ./$(DEPDIR)/libfwps_support.Plo
 am__mv = mv -f
 COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
 	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
 LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) \
 	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
 	$(AM_CFLAGS) $(CFLAGS)
@@ -526,20 +522,18 @@
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_libcnotify.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_libfguid.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_libfole.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_libuna.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_property_identifier.c libfwps_property_identifier.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_record.c libfwps_record.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_set.c libfwps_set.h \
-@HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_storage.c libfwps_storage.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_store.c libfwps_store.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_support.c libfwps_support.h \
 @HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_types.h \
-@HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_unused.h \
-@HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_value.c libfwps_value.h
+@HAVE_LOCAL_LIBFWPS_TRUE@	libfwps_unused.h
 
 MAINTAINERCLEANFILES = \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
@@ -595,18 +589,16 @@
 	-rm -f *.tab.c
 
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_error.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_format_class_identifier.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_property_identifier.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_record.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_set.Plo@am__quote@ # am--include-marker
-@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_storage.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_store.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_support.Plo@am__quote@ # am--include-marker
-@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/libfwps_value.Plo@am__quote@ # am--include-marker
 
 $(am__depfiles_remade):
 	@$(MKDIR_P) $(@D)
 	@echo '# dummy' >$@-t && $(am__mv) $@-t $@
 
 am--depfiles: $(am__depfiles_remade)
 
@@ -806,18 +798,16 @@
 
 maintainer-clean: maintainer-clean-am
 		-rm -f ./$(DEPDIR)/libfwps_error.Plo
 	-rm -f ./$(DEPDIR)/libfwps_format_class_identifier.Plo
 	-rm -f ./$(DEPDIR)/libfwps_property_identifier.Plo
 	-rm -f ./$(DEPDIR)/libfwps_record.Plo
 	-rm -f ./$(DEPDIR)/libfwps_set.Plo
-	-rm -f ./$(DEPDIR)/libfwps_storage.Plo
 	-rm -f ./$(DEPDIR)/libfwps_store.Plo
 	-rm -f ./$(DEPDIR)/libfwps_support.Plo
-	-rm -f ./$(DEPDIR)/libfwps_value.Plo
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
 
 mostlyclean: mostlyclean-am
 
 mostlyclean-am: mostlyclean-compile mostlyclean-generic \
 	mostlyclean-libtool
```

### Comparing `libfwsi-20230114/libfwps/libfwps_libcerror.h` & `libfwsi-20230710/libfwps/libfwps_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_property_identifier.c` & `libfwsi-20230710/libfwps/libfwps_property_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_storage.c` & `libfwsi-20230710/libfwsi/libfwsi_debug.c`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows Serialized Property Storage functions
+ * Debug functions
  *
- * Copyright (C) 2013-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -16,488 +16,665 @@
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
-#include <byte_stream.h>
 #include <memory.h>
+#include <narrow_string.h>
 #include <system_string.h>
 #include <types.h>
+#include <wide_string.h>
 
-#include "libfwps_definitions.h"
-#include "libfwps_libcerror.h"
-#include "libfwps_libcnotify.h"
-#include "libfwps_libfguid.h"
-#include "libfwps_record.h"
-#include "libfwps_storage.h"
-#include "libfwps_types.h"
-
-const char *libfwps_serialized_property_storage_signature = "1SPS";
+#include "libfwsi_debug.h"
+#include "libfwsi_libcerror.h"
+#include "libfwsi_libcnotify.h"
+#include "libfwsi_libfdatetime.h"
+#include "libfwsi_libfguid.h"
+#include "libfwsi_libfwps.h"
+#include "libfwsi_libuna.h"
 
-uint8_t libfwps_storage_format_class_identifier_named_properties[ 16 ] = {
-	0x05, 0xd5, 0xcd, 0xd5, 0x9c, 0x2e, 0x1b, 0x10, 0x93, 0x97, 0x08, 0x00, 0x2b, 0x2c, 0xf9, 0xae };
+#if defined( HAVE_DEBUG_OUTPUT )
+
+/* Prints the control planel category
+ */
+const char *libfwsi_debug_print_control_panel_category(
+             uint32_t control_panel_category )
+{
+	switch( control_panel_category )
+	{
+		case 0:
+			return( "All Control Panel Items" );
+
+		case 1:
+			return( "Appearance and Personalization" );
+
+		case 2:
+			return( "Hardware and Sound" );
+
+		case 3:
+			return( "Network and Internet" );
+
+		case 4:
+			return( "Sounds, Speech, and Audio Devices" );
 
-uint8_t libfwps_storage_format_class_identifier_unknown1[ 16 ] = {
-	0x30, 0xf1, 0x25, 0xb7, 0xef, 0x47, 0x1a, 0x10, 0xa5, 0xf1, 0x02, 0x60, 0x8c, 0x9e, 0xeb, 0xac };
+		case 5:
+			return( "System and Security" );
+
+		case 6:
+			return( "Clock, Language, and Region" );
+
+		case 7:
+			return( "Ease of Access" );
+
+		case 8:
+			return( "Programs" );
+
+		case 9:
+			return( "User Accounts" );
+
+		case 10:
+			return( "Security Center" );
+
+		case 11:
+			return( "Mobile PC" );
+	}
+	return( "_UNKNOWN_" );
+}
 
-/* Creates a storage
- * Make sure the value storage is referencing, is set to NULL
+/* Prints a FAT date time value
  * Returns 1 if successful or -1 on error
  */
-int libfwps_storage_initialize(
-     libfwps_storage_t **storage,
+int libfwsi_debug_print_fat_date_time_value(
+     const char *function_name,
+     const char *value_name,
+     const uint8_t *byte_stream,
+     size_t byte_stream_size,
+     int byte_order,
+     uint32_t string_format_flags,
      libcerror_error_t **error )
 {
-	libfwps_internal_storage_t *internal_storage = NULL;
-	static char *function                        = "libfwps_storage_initialize";
+	char date_time_string[ 32 ];
+
+	libfdatetime_fat_date_time_t *fat_date_time = NULL;
+	static char *function                       = "libfwsi_debug_print_fat_date_time_value";
 
-	if( storage == NULL )
+	if( libfdatetime_fat_date_time_initialize(
+	     &fat_date_time,
+	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid storage.",
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
+		 "%s: unable to create FAT date time.",
 		 function );
 
-		return( -1 );
+		goto on_error;
 	}
-	if( *storage != NULL )
+	if( libfdatetime_fat_date_time_copy_from_byte_stream(
+	     fat_date_time,
+	     byte_stream,
+	     byte_stream_size,
+	     byte_order,
+	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_VALUE_ALREADY_SET,
-		 "%s: invalid storage value already set.",
+		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
+		 "%s: unable to copy byte stream to FAT date time.",
 		 function );
 
-		return( -1 );
+		goto on_error;
 	}
-	internal_storage = memory_allocate_structure(
-	                    libfwps_internal_storage_t );
-
-	if( internal_storage == NULL )
+	if( libfdatetime_fat_date_time_copy_to_utf8_string(
+	     fat_date_time,
+	     (uint8_t *) date_time_string,
+	     32,
+	     string_format_flags,
+	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_MEMORY,
-		 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
-		 "%s: unable to create storage.",
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
+		 "%s: unable to copy FAT date time to string.",
 		 function );
 
 		goto on_error;
 	}
-	if( memory_set(
-	     internal_storage,
-	     0,
-	     sizeof( libfwps_internal_storage_t ) ) == NULL )
+	libcnotify_printf(
+	 "%s: %s: %s UTC\n",
+	 function_name,
+	 value_name,
+	 date_time_string );
+
+	if( libfdatetime_fat_date_time_free(
+	     &fat_date_time,
+	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_MEMORY,
-		 LIBCERROR_MEMORY_ERROR_SET_FAILED,
-		 "%s: unable to clear storage.",
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
+		 "%s: unable to free FAT date time.",
 		 function );
 
 		goto on_error;
 	}
-	*storage = (libfwps_storage_t *) internal_storage;
-
 	return( 1 );
 
 on_error:
-	if( internal_storage != NULL )
+	if( fat_date_time != NULL )
 	{
-		memory_free(
-		 internal_storage );
+		libfdatetime_fat_date_time_free(
+		 &fat_date_time,
+		 NULL );
 	}
 	return( -1 );
 }
 
-/* Frees a storage
+/* Prints a FILETIME value
  * Returns 1 if successful or -1 on error
  */
-int libfwps_storage_free(
-     libfwps_storage_t **storage,
+int libfwsi_debug_print_filetime_value(
+     const char *function_name,
+     const char *value_name,
+     const uint8_t *byte_stream,
+     size_t byte_stream_size,
+     int byte_order,
+     uint32_t string_format_flags,
      libcerror_error_t **error )
 {
-	libfwps_internal_storage_t *internal_storage = NULL;
-	static char *function                        = "libfwps_storage_free";
+	char date_time_string[ 32 ];
 
-	if( storage == NULL )
+	libfdatetime_filetime_t *filetime = NULL;
+	static char *function             = "libfwsi_debug_print_filetime_value";
+
+	if( libfdatetime_filetime_initialize(
+	     &filetime,
+	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid storage.",
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
+		 "%s: unable to create filetime.",
 		 function );
 
-		return( -1 );
+		goto on_error;
 	}
-	if( *storage != NULL )
+	if( libfdatetime_filetime_copy_from_byte_stream(
+	     filetime,
+	     byte_stream,
+	     byte_stream_size,
+	     byte_order,
+	     error ) != 1 )
 	{
-		internal_storage = (libfwps_internal_storage_t *) *storage;
-		*storage         = NULL;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
+		 "%s: unable to copy byte stream to filetime.",
+		 function );
 
-		memory_free(
-		 internal_storage );
+		goto on_error;
+	}
+	if( libfdatetime_filetime_copy_to_utf8_string(
+	     filetime,
+	     (uint8_t *) date_time_string,
+	     32,
+	     string_format_flags,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
+		 "%s: unable to copy filetime to string.",
+		 function );
+
+		goto on_error;
+	}
+	libcnotify_printf(
+	 "%s: %s: %s UTC\n",
+	 function_name,
+	 value_name,
+	 date_time_string );
+
+	if( libfdatetime_filetime_free(
+	     &filetime,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
+		 "%s: unable to free filetime.",
+		 function );
+
+		goto on_error;
 	}
 	return( 1 );
+
+on_error:
+	if( filetime != NULL )
+	{
+		libfdatetime_filetime_free(
+		 &filetime,
+		 NULL );
+	}
+	return( -1 );
 }
 
-/* Copies a serialized property storage from a byte stream
+/* Prints a GUID/UUID value
  * Returns 1 if successful or -1 on error
  */
-int libfwps_storage_copy_from_byte_stream(
-     libfwps_storage_t *storage,
+int libfwsi_debug_print_guid_value(
+     const char *function_name,
+     const char *value_name,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
-     int ascii_codepage,
+     int byte_order,
+     uint32_t string_format_flags,
      libcerror_error_t **error )
 {
-	libfwps_internal_storage_t *internal_storage = NULL;
-	libfwps_record_t *property_record            = NULL;
-	static char *function                        = "libfwps_storage_copy_from_byte_stream";
-	size_t byte_stream_offset                    = 0;
-	uint32_t property_record_size                = 0;
-	uint8_t property_record_type                 = 0;
-
-#if defined( HAVE_DEBUG_OUTPUT )
         system_character_t guid_string[ 48 ];
 
-        libfguid_identifier_t *guid                  = NULL;
-	int result                                   = 0;
-#endif
+        libfguid_identifier_t *guid = NULL;
+	static char *function       = "libfwsi_debug_print_guid_value";
 
-	if( storage == NULL )
+	if( libfguid_identifier_initialize(
+	     &guid,
+	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid storage.",
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
+		 "%s: unable to create GUID.",
 		 function );
 
-		return( -1 );
+		goto on_error;
 	}
-	internal_storage = (libfwps_internal_storage_t *) storage;
-
-	if( byte_stream == NULL )
+	if( libfguid_identifier_copy_from_byte_stream(
+	     guid,
+	     byte_stream,
+	     byte_stream_size,
+	     byte_order,
+	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid byte stream.",
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
+		 "%s: unable to copy byte stream to GUID.",
 		 function );
 
-		return( -1 );
+		goto on_error;
 	}
-	if( ( byte_stream_size < 4 )
-	 || ( byte_stream_size > (size_t) SSIZE_MAX ) )
+	if( libfguid_identifier_copy_to_utf8_string(
+	     guid,
+	     (uint8_t *) guid_string,
+	     48,
+	     string_format_flags,
+	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_VALUE_OUT_OF_BOUNDS,
-		 "%s: invalid byte stream size value out of bounds.",
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
+		 "%s: unable to copy GUID to string.",
 		 function );
 
-		return( -1 );
+		goto on_error;
 	}
-	byte_stream_copy_to_uint32_little_endian(
-	 byte_stream,
-	 internal_storage->size );
-
-#if defined( HAVE_DEBUG_OUTPUT )
-	if( libcnotify_verbose != 0 )
+	libcnotify_printf(
+	 "%s: %s: %s\n",
+	 function_name,
+	 value_name,
+	 guid_string );
+
+	if( libfguid_identifier_free(
+	     &guid,
+	     error ) != 1 )
 	{
-		libcnotify_printf(
-		 "%s: size\t\t\t\t: %" PRIu16 "\n",
-		 function,
-		 internal_storage->size );
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
+		 "%s: unable to free GUID.",
+		 function );
+
+		goto on_error;
 	}
-#endif
-	if( internal_storage->size == 0 )
+	return( 1 );
+
+on_error:
+	if( guid != NULL )
 	{
-		return( 1 );
+		libfguid_identifier_free(
+		 &guid,
+		 NULL );
 	}
-	if( ( internal_storage->size < 4 )
-	 || ( (size_t) internal_storage->size > byte_stream_size ) )
+	return( -1 );
+}
+
+/* Prints a property set value
+ * Returns 1 if successful or -1 on error
+ */
+int libfwsi_debug_print_property_set_value(
+     const uint8_t *byte_stream,
+     size_t byte_stream_size,
+     int ascii_codepage,
+     libcerror_error_t **error )
+{
+        libfwps_set_t *property_set = NULL;
+	static char *function       = "libfwsi_debug_print_property_set_value";
+
+	if( libfwps_set_initialize(
+	     &property_set,
+	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-		 "%s: invalid property storage size value out of bounds.",
+		 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
+		 "%s: unable to create property set.",
 		 function );
 
 		goto on_error;
 	}
-	byte_stream_offset += 4;
-
-	if( ( internal_storage->size - byte_stream_offset ) < 4 )
+	if( libfwps_set_copy_from_byte_stream(
+	     property_set,
+	     byte_stream,
+	     byte_stream_size,
+	     ascii_codepage,
+	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
-		 "%s: invalid byte stream size value to small.",
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
+		 "%s: unable to copy byte stream to property set.",
 		 function );
 
 		goto on_error;
 	}
-	if( memory_compare(
-	     &( byte_stream[ byte_stream_offset ] ),
-	     libfwps_serialized_property_storage_signature,
-	     4 ) != 0 )
+	if( libfwps_set_free(
+	     &property_set,
+	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported signature.",
+		 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
+		 "%s: unable to free property set.",
 		 function );
 
 		goto on_error;
 	}
-#if defined( HAVE_DEBUG_OUTPUT )
-	if( libcnotify_verbose != 0 )
+	return( 1 );
+
+on_error:
+	if( property_set != NULL )
 	{
-		libcnotify_printf(
-		 "%s: signature\t\t\t: %c%c%c%c\n",
-		 function,
-		 byte_stream[ byte_stream_offset ],
-		 byte_stream[ byte_stream_offset + 1 ],
-		 byte_stream[ byte_stream_offset + 2 ],
-		 byte_stream[ byte_stream_offset + 3 ] );
+		libfwps_set_free(
+		 &property_set,
+		 NULL );
 	}
-#endif
-	byte_stream_offset += 4;
+	return( -1 );
+}
 
-	if( ( internal_storage->size - byte_stream_offset ) < 16 )
+/* Prints a string value
+ * Returns 1 if successful or -1 on error
+ */
+int libfwsi_debug_print_string_value(
+     const char *function_name,
+     const char *value_name,
+     const uint8_t *byte_stream,
+     size_t byte_stream_size,
+     int ascii_codepage,
+     libcerror_error_t **error )
+{
+	system_character_t *string = NULL;
+	static char *function      = "libfwsi_debug_print_string_value";
+	size_t string_size         = 0;
+	int result                 = 0;
+
+#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
+	result = libuna_utf16_string_size_from_byte_stream(
+		  byte_stream,
+		  byte_stream_size,
+		  ascii_codepage,
+		  &string_size,
+		  error );
+#else
+	result = libuna_utf8_string_size_from_byte_stream(
+		  byte_stream,
+		  byte_stream_size,
+		  ascii_codepage,
+		  &string_size,
+		  error );
+#endif
+	if( result != 1 )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
-		 "%s: invalid byte stream size value to small.",
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to determine size of string.",
 		 function );
 
 		goto on_error;
 	}
-#if defined( HAVE_DEBUG_OUTPUT )
-	if( libcnotify_verbose != 0 )
+	if( ( string_size > (size_t) SSIZE_MAX )
+	 || ( ( sizeof( system_character_t ) * string_size ) > (size_t) SSIZE_MAX ) )
 	{
-		if( libfguid_identifier_initialize(
-		     &guid,
-		     error ) != 1 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
-			 "%s: unable to create GUID.",
-			 function );
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid string size value exceeds maximum.",
+		 function );
 
-			goto on_error;
-		}
-		if( libfguid_identifier_copy_from_byte_stream(
-		     guid,
-		     &( byte_stream[ byte_stream_offset ] ),
-		     16,
-		     LIBFGUID_ENDIAN_LITTLE,
-		     error ) != 1 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
-			 "%s: unable to copy byte stream to GUID.",
-			 function );
+		goto on_error;
+	}
+	string = system_string_allocate(
+			string_size );
 
-			goto on_error;
-		}
+	if( string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_MEMORY,
+		 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
+		 "%s: unable to create string.",
+		 function );
+
+		goto on_error;
+	}
 #if defined( HAVE_WIDE_SYSTEM_CHARACTER )
-		result = libfguid_identifier_copy_to_utf16_string(
-			  guid,
-			  (uint16_t *) guid_string,
-			  48,
-			  LIBFGUID_STRING_FORMAT_FLAG_USE_UPPER_CASE | LIBFGUID_STRING_FORMAT_FLAG_USE_SURROUNDING_BRACES,
-			  error );
+	result = libuna_utf16_string_copy_from_byte_stream(
+		  (libuna_utf16_character_t *) string,
+		  string_size,
+		  byte_stream,
+		  byte_stream_size,
+		  ascii_codepage,
+		  error );
 #else
-		result = libfguid_identifier_copy_to_utf8_string(
-			  guid,
-			  (uint8_t *) guid_string,
-			  48,
-			  LIBFGUID_STRING_FORMAT_FLAG_USE_UPPER_CASE | LIBFGUID_STRING_FORMAT_FLAG_USE_SURROUNDING_BRACES,
-			  error );
+	result = libuna_utf8_string_copy_from_byte_stream(
+		  (libuna_utf8_character_t *) string,
+		  string_size,
+		  byte_stream,
+		  byte_stream_size,
+		  ascii_codepage,
+		  error );
 #endif
-		if( result != 1 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
-			 "%s: unable to copy GUID to string.",
-			 function );
-
-			goto on_error;
-		}
-		libcnotify_printf(
-		 "%s: format class identifier\t\t: %" PRIs_SYSTEM "\n",
-		 function,
-		 guid_string );
-
-		if( libfguid_identifier_free(
-		     &guid,
-		     error ) != 1 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
-			 "%s: unable to free GUID.",
-			 function );
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
+		 "%s: unable to set string.",
+		 function );
 
-			goto on_error;
-		}
+		goto on_error;
 	}
-#endif /* defined( HAVE_DEBUG_OUTPUT ) */
+	libcnotify_printf(
+	 "%s: %s: %s\n",
+	 function_name,
+	 value_name,
+	 string );
 
-	if( memory_compare(
-	     &( byte_stream[ byte_stream_offset ] ),
-	     libfwps_storage_format_class_identifier_named_properties,
-	     16 ) == 0 )
+	memory_free(
+	 string );
+
+	return( 1 );
+
+on_error:
+	if( string != NULL )
 	{
-		property_record_type = LIBFWPS_RECORD_TYPE_NAMED;
+		memory_free(
+		 string );
 	}
-	else
+	return( -1 );
+}
+
+/* Prints an UTF-16 string value
+ * Returns 1 if successful or -1 on error
+ */
+int libfwsi_debug_print_utf16_string_value(
+     const char *function_name,
+     const char *value_name,
+     const uint8_t *byte_stream,
+     size_t byte_stream_size,
+     int byte_order,
+     libcerror_error_t **error )
+{
+	system_character_t *string = NULL;
+	static char *function      = "libfwsi_debug_print_utf16_string_value";
+	size_t string_size         = 0;
+	int result                 = 0;
+
+	if( ( byte_stream == NULL )
+	 || ( byte_stream_size == 0 ) )
 	{
-		property_record_type = LIBFWPS_RECORD_TYPE_NUMERIC;
+		libcnotify_printf(
+		 "%s: %s:\n",
+		 function_name,
+		 value_name );
+
+		return( 1 );
 	}
-	byte_stream_offset += 16;
+#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
+	result = libuna_utf16_string_size_from_utf16_stream(
+	          byte_stream,
+	          byte_stream_size,
+	          byte_order,
+	          &string_size,
+	          error );
+#else
+	result = libuna_utf8_string_size_from_utf16_stream(
+	          byte_stream,
+	          byte_stream_size,
+	          byte_order,
+	          &string_size,
+	          error );
+#endif
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to determine size of string.",
+		 function );
 
-	while( byte_stream_offset < byte_stream_size )
+		goto on_error;
+	}
+	if( string_size > ( (size_t) SSIZE_MAX / sizeof( system_character_t ) ) )
 	{
-		if( byte_stream_offset > ( byte_stream_size - 4 ) )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-			 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
-			 "%s: invalid byte stream size value too small.",
-			 function );
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid string size value exceeds maximum.",
+		 function );
 
-			goto on_error;
-		}
-		byte_stream_copy_to_uint32_little_endian(
-		 &( byte_stream[ byte_stream_offset ] ),
-		 property_record_size );
+		goto on_error;
+	}
+	libcnotify_printf(
+	 "%s: %s:",
+	 function_name,
+	 value_name );
 
-#if defined( HAVE_DEBUG_OUTPUT )
-		if( libcnotify_verbose != 0 )
-		{
-			libcnotify_printf(
-			 "%s: record data size\t\t\t: %" PRIu32 "\n",
-			 function,
-			 property_record_size );
-		}
-#endif
-		if( property_record_size == 0 )
-		{
-			break;
-		}
-		if( ( property_record_size > byte_stream_size )
-		 || ( byte_stream_offset > ( byte_stream_size - property_record_size ) ) )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-			 "%s: invalid value data size value out of bounds.",
-			 function );
+	if( string_size > 0 )
+	{
+		string = system_string_allocate(
+		          string_size );
 
-			goto on_error;
-		}
-		if( libfwps_record_initialize(
-		     &property_record,
-		     property_record_type,
-		     error ) != 1 )
+		if( string == NULL )
 		{
 			libcerror_error_set(
 			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
-			 "%s: unable to create property record.",
+			 LIBCERROR_ERROR_DOMAIN_MEMORY,
+			 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
+			 "%s: unable to create string.",
 			 function );
 
 			goto on_error;
 		}
-		if( libfwps_record_copy_from_byte_stream(
-		     property_record,
-		     &( byte_stream[ byte_stream_offset ] ),
-		     byte_stream_size - byte_stream_offset,
-		     ascii_codepage,
-		     error ) != 1 )
+#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
+		result = libuna_utf16_string_copy_from_utf16_stream(
+		          (libuna_utf16_character_t *) string,
+		          string_size,
+		          byte_stream,
+		          byte_stream_size,
+		          byte_order,
+		          error );
+#else
+		result = libuna_utf8_string_copy_from_utf16_stream(
+		          (libuna_utf8_character_t *) string,
+		          string_size,
+		          byte_stream,
+		          byte_stream_size,
+		          byte_order,
+		          error );
+#endif
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
-			 "%s: unable to copy byte stream to property record.",
+			 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
+			 "%s: unable to set string.",
 			 function );
 
 			goto on_error;
 		}
-/* TODO store value array if size != 0 */
-		if( libfwps_internal_record_free(
-		     (libfwps_internal_record_t **) &property_record,
-		     error ) != 1 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
-			 "%s: unable to free property record.",
-			 function );
+		libcnotify_printf(
+		 " %s",
+		 string );
 
-			goto on_error;
-		}
-		if( property_record_size == 0 )
-		{
-			break;
-		}
-		byte_stream_offset += property_record_size;
+		memory_free(
+		 string );
 	}
-/* TODO print trailing data */
+	libcnotify_printf(
+	 "\n" );
 
-#if defined( HAVE_DEBUG_OUTPUT )
-	if( libcnotify_verbose != 0 )
-	{
-		libcnotify_printf(
-		 "\n" );
-	}
-#endif
 	return( 1 );
 
 on_error:
-#if defined( HAVE_DEBUG_OUTPUT )
-	if( guid != NULL )
-	{
-		libfguid_identifier_free(
-		 &guid,
-		 NULL );
-	}
-#endif
-	if( property_record != NULL )
+	if( string != NULL )
 	{
-		libfwps_internal_record_free(
-		 (libfwps_internal_record_t **) &property_record,
-		 NULL );
+		memory_free(
+		 string );
 	}
 	return( -1 );
 }
 
+#endif /* defined( HAVE_DEBUG_OUTPUT ) */
+
```

### Comparing `libfwsi-20230114/libfwps/libfwps_value.c` & `libfwsi-20230710/libfwsi/libfwsi_compressed_folder_values.c`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows Serialized Property Value functions
+ * Compressed folder (shell item) values functions
  *
- * Copyright (C) 2013-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -18,494 +18,492 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <byte_stream.h>
 #include <memory.h>
-#include <narrow_string.h>
-#include <system_string.h>
 #include <types.h>
-#include <wide_string.h>
 
-#include "libfwps_definitions.h"
-#include "libfwps_libcerror.h"
-#include "libfwps_libcnotify.h"
-#include "libfwps_libfole.h"
-#include "libfwps_libuna.h"
-#include "libfwps_types.h"
-#include "libfwps_value.h"
+#include "libfwsi_compressed_folder_values.h"
+#include "libfwsi_debug.h"
+#include "libfwsi_definitions.h"
+#include "libfwsi_libcerror.h"
+#include "libfwsi_libcnotify.h"
+#include "libfwsi_libfdatetime.h"
+#include "libfwsi_libuna.h"
+#include "libfwsi_unused.h"
 
-/* Creates a value
- * Make sure the value value is referencing, is set to NULL
+/* Creates compressed folder values
+ * Make sure the value compressed_folder_values is referencing, is set to NULL
  * Returns 1 if successful or -1 on error
  */
-int libfwps_value_initialize(
-     libfwps_value_t **value,
-     uint8_t value_type,
+int libfwsi_compressed_folder_values_initialize(
+     libfwsi_compressed_folder_values_t **compressed_folder_values,
      libcerror_error_t **error )
 {
-	libfwps_internal_value_t *internal_value = NULL;
-	static char *function                    = "libfwps_value_initialize";
+	static char *function = "libfwsi_compressed_folder_values_initialize";
 
-	if( value == NULL )
+	if( compressed_folder_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid value.",
+		 "%s: invalid compressed folder values.",
 		 function );
 
 		return( -1 );
 	}
-	if( *value != NULL )
+	if( *compressed_folder_values != NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_VALUE_ALREADY_SET,
-		 "%s: invalid value value already set.",
+		 "%s: invalid compressed folder values value already set.",
 		 function );
 
 		return( -1 );
 	}
-	if( ( value_type != LIBFWPS_RECORD_TYPE_NAMED )
-	 && ( value_type != LIBFWPS_RECORD_TYPE_NUMERIC ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported value type.",
-		 function );
+	*compressed_folder_values = memory_allocate_structure(
+	                             libfwsi_compressed_folder_values_t );
 
-		return( -1 );
-	}
-	internal_value = memory_allocate_structure(
-	                  libfwps_internal_value_t );
-
-	if( internal_value == NULL )
+	if( *compressed_folder_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_MEMORY,
 		 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
-		 "%s: unable to create value.",
+		 "%s: unable to create compressed folder values.",
 		 function );
 
 		goto on_error;
 	}
 	if( memory_set(
-	     internal_value,
+	     *compressed_folder_values,
 	     0,
-	     sizeof( libfwps_internal_value_t ) ) == NULL )
+	     sizeof( libfwsi_compressed_folder_values_t ) ) == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_MEMORY,
 		 LIBCERROR_MEMORY_ERROR_SET_FAILED,
-		 "%s: unable to clear value.",
+		 "%s: unable to clear compressed folder values.",
 		 function );
 
 		goto on_error;
 	}
-	internal_value->type = value_type;
-
-	*value = (libfwps_value_t *) internal_value;
-
 	return( 1 );
 
 on_error:
-	if( internal_value != NULL )
+	if( *compressed_folder_values != NULL )
 	{
 		memory_free(
-		 internal_value );
-	}
-	return( -1 );
-}
+		 *compressed_folder_values );
 
-/* Frees a value
- * Returns 1 if successful or -1 on error
- */
-int libfwps_value_free(
-     libfwps_value_t **value,
-     libcerror_error_t **error )
-{
-	static char *function = "libfwps_value_free";
-
-	if( value == NULL )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid value.",
-		 function );
-
-		return( -1 );
+		*compressed_folder_values = NULL;
 	}
-	if( *value != NULL )
-	{
-		*value = NULL;
-	}
-	return( 1 );
+	return( -1 );
 }
 
-/* Frees a value
+/* Frees compressed folder values
  * Returns 1 if successful or -1 on error
  */
-int libfwps_internal_value_free(
-     libfwps_internal_value_t **internal_value,
+int libfwsi_compressed_folder_values_free(
+     libfwsi_compressed_folder_values_t **compressed_folder_values,
      libcerror_error_t **error )
 {
-	static char *function = "libfwps_internal_value_free";
+	static char *function = "libfwsi_compressed_folder_values_free";
 
-	if( internal_value == NULL )
+	if( compressed_folder_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid internal value.",
+		 "%s: invalid compressed folder values.",
 		 function );
 
 		return( -1 );
 	}
-	if( *internal_value != NULL )
+	if( *compressed_folder_values != NULL )
 	{
 		memory_free(
-		 *internal_value );
+		 *compressed_folder_values );
 
-		*internal_value = NULL;
+		*compressed_folder_values = NULL;
 	}
 	return( 1 );
 }
 
-/* Copies a serialized property value from a byte stream
- * Returns 1 if successful or -1 on error
+/* Reads the compressed folder values
+ * Returns 1 if successful, 0 if not supported or -1 on error
  */
-int libfwps_value_copy_from_byte_stream(
-     libfwps_value_t *value,
-     const uint8_t *byte_stream,
-     size_t byte_stream_size,
-     int ascii_codepage,
+int libfwsi_compressed_folder_values_read_data(
+     libfwsi_compressed_folder_values_t *compressed_folder_values,
+     const uint8_t *data,
+     size_t data_size,
      libcerror_error_t **error )
 {
-	libfwps_internal_value_t *internal_value = NULL;
-	static char *function                    = "libfwps_value_copy_from_byte_stream";
-	size_t byte_stream_offset                = 0;
-	uint32_t name_size                       = 0;
+	static char *function = "libfwsi_compressed_folder_values_read_data";
+	size_t data_offset    = 0;
+	uint32_t string_size  = 0;
 
 #if defined( HAVE_DEBUG_OUTPUT )
-	system_character_t *value_string         = NULL;
-	size_t value_string_size                 = 0;
-	uint32_t value_32bit                     = 0;
-	int result                               = 0;
+	uint64_t value_64bit  = 0;
+	uint32_t value_32bit  = 0;
+	uint16_t value_16bit  = 0;
 #endif
 
-	if( value == NULL )
+	if( compressed_folder_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid value.",
+		 "%s: invalid compressed folder values.",
 		 function );
 
 		return( -1 );
 	}
-	internal_value = (libfwps_internal_value_t *) value;
-
-	if( byte_stream == NULL )
+	if( data == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid byte stream.",
+		 "%s: invalid data.",
 		 function );
 
 		return( -1 );
 	}
-	if( ( byte_stream_size < 4 )
-	 || ( byte_stream_size > (size_t) SSIZE_MAX ) )
+	if( data_size > (size_t) SSIZE_MAX )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_VALUE_OUT_OF_BOUNDS,
-		 "%s: invalid byte stream size value out of bounds.",
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: data size exceeds maximum.",
 		 function );
 
 		return( -1 );
 	}
-	byte_stream_copy_to_uint32_little_endian(
-	 byte_stream,
-	 internal_value->size );
-
-	if( ( internal_value->size < 4 )
-	 || ( (size_t) internal_value->size > byte_stream_size ) )
+	/* Do not try to parse unsupported data sizes
+	 */
+	if( data_size < 6 )
+	{
+		return( 0 );
+	}
+	/* Do not try to parse unknown class type indicators
+	 */
+	if( data[ 2 ] != 0x52 )
+	{
+		return( 0 );
+	}
+/* TODO: other variants not supported yet */
+	if( ( data[ 3 ] != 0x67 )
+	 || ( data[ 4 ] != 0xb1 )
+	 || ( data[ 5 ] != 0xac ) )
+	{
+		return( 0 );
+	}
+	if( ( data[ 3 ] == 0x67 )
+	 && ( data[ 4 ] == 0xb1 )
+	 && ( data[ 5 ] == 0xac ) )
 	{
+		if( data_size < 50 )
+		{
+			return( 0 );
+		}
 #if defined( HAVE_DEBUG_OUTPUT )
 		if( libcnotify_verbose != 0 )
 		{
 			libcnotify_printf(
-			 "%s: size\t\t\t\t: %" PRIu32 "\n",
+			 "%s: unknown1\t\t\t\t: 0x%02" PRIx8 "\n",
 			 function,
-			 internal_value->size );
+			 data[ 3 ] );
 
+			byte_stream_copy_to_uint16_little_endian(
+			 &( data[ 4 ] ),
+			 value_16bit );
 			libcnotify_printf(
-			 "\n" );
-		}
-#endif
-		if( internal_value->size == 0 )
-		{
-			return( 1 );
-		}
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-		 "%s: invalid property value size value out of bounds.",
-		 function );
+			 "%s: unknown2\t\t\t\t: 0x%04" PRIx16 "\n",
+			 function,
+			 value_16bit );
 
-		goto on_error;
-	}
-#if defined( HAVE_DEBUG_OUTPUT )
-	if( libcnotify_verbose != 0 )
-	{
-		libcnotify_printf(
-		 "%s: property value data:\n",
-		 function );
-		libcnotify_print_data(
-		 byte_stream,
-		 internal_value->size,
-		 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
-	}
-#endif
-#if defined( HAVE_DEBUG_OUTPUT )
-	if( libcnotify_verbose != 0 )
-	{
-		libcnotify_printf(
-		 "%s: size\t\t\t\t: %" PRIu32 "\n",
-		 function,
-		 internal_value->size );
-	}
-#endif
-	byte_stream_offset += 4;
+			byte_stream_copy_to_uint32_little_endian(
+			 &( data[ 6 ] ),
+			 value_32bit );
+			libcnotify_printf(
+			 "%s: unknown3\t\t\t\t: 0x%08" PRIx32 "\n",
+			 function,
+			 value_32bit );
 
-	if( byte_stream_offset > ( internal_value->size - 4 ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
-		 "%s: invalid byte stream size value too small.",
-		 function );
+			byte_stream_copy_to_uint64_little_endian(
+			 &( data[ 10 ] ),
+			 value_64bit );
+			libcnotify_printf(
+			 "%s: unknown4\t\t\t\t: 0x%08" PRIx64 "\n",
+			 function,
+			 value_64bit );
 
-		return( -1 );
-	}
-	if( internal_value->type == LIBFWPS_RECORD_TYPE_NAMED )
-	{
-		byte_stream_copy_to_uint32_little_endian(
-		 &( byte_stream[ byte_stream_offset ] ),
-		 name_size );
+			byte_stream_copy_to_uint32_little_endian(
+			 &( data[ 18 ] ),
+			 value_32bit );
+			libcnotify_printf(
+			 "%s: unknown5\t\t\t\t: 0x%08" PRIx32 "\n",
+			 function,
+			 value_32bit );
 
-#if defined( HAVE_DEBUG_OUTPUT )
-		if( libcnotify_verbose != 0 )
-		{
+			byte_stream_copy_to_uint32_little_endian(
+			 &( data[ 22 ] ),
+			 value_32bit );
 			libcnotify_printf(
-			 "%s: name size\t\t\t\t: %" PRIu32 "\n",
+			 "%s: unknown6\t\t\t\t: 0x%08" PRIx32 "\n",
 			 function,
-			 name_size );
-		}
-#endif
-	}
-	else if( internal_value->type == LIBFWPS_RECORD_TYPE_NUMERIC )
-	{
-#if defined( HAVE_DEBUG_OUTPUT )
-		if( libcnotify_verbose != 0 )
-		{
+			 value_32bit );
+
+			if( libfwsi_debug_print_fat_date_time_value(
+			     function,
+			     "unknown time1\t\t\t",
+			     &( data[ 26 ] ),
+			     4,
+			     LIBFDATETIME_ENDIAN_LITTLE,
+			     LIBFDATETIME_STRING_FORMAT_TYPE_CTIME | LIBFDATETIME_STRING_FORMAT_FLAG_DATE_TIME,
+			     error ) != 1 )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+				 "%s: unable to print FAT date time value.",
+				 function );
+
+				return( -1 );
+			}
 			byte_stream_copy_to_uint32_little_endian(
-			 &( byte_stream[ byte_stream_offset ] ),
+			 &( data[ 30 ] ),
 			 value_32bit );
 			libcnotify_printf(
-			 "%s: identifier\t\t\t\t: %" PRIu32 "\n",
+			 "%s: unknown7\t\t\t\t: 0x%08" PRIx32 "\n",
 			 function,
 			 value_32bit );
+
+			if( libfwsi_debug_print_fat_date_time_value(
+			     function,
+			     "unknown time2\t\t\t",
+			     &( data[ 34 ] ),
+			     4,
+			     LIBFDATETIME_ENDIAN_LITTLE,
+			     LIBFDATETIME_STRING_FORMAT_TYPE_CTIME | LIBFDATETIME_STRING_FORMAT_FLAG_DATE_TIME,
+			     error ) != 1 )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+				 "%s: unable to print FAT date time value.",
+				 function );
+
+				return( -1 );
+			}
+			byte_stream_copy_to_uint64_little_endian(
+			 &( data[ 38 ] ),
+			 value_64bit );
+			libcnotify_printf(
+			 "%s: unknown8\t\t\t\t: 0x%08" PRIx64 "\n",
+			 function,
+			 value_64bit );
 		}
 #endif
+		data_offset = 46;
 	}
-	byte_stream_offset += 4;
-
-	if( byte_stream_offset > ( internal_value->size - 1 ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
-		 "%s: invalid byte stream size value too small.",
-		 function );
+	byte_stream_copy_to_uint32_little_endian(
+	 &( data[ data_offset ] ),
+	 string_size );
 
-		return( -1 );
-	}
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
 		libcnotify_printf(
-		 "%s: unknown1\t\t\t\t: 0x%" PRIx8 "\n",
+		 "%s: string size\t\t\t: %" PRIu32 "\n",
 		 function,
-		 byte_stream[ byte_stream_offset ] );
+		 string_size );
 	}
 #endif
-	byte_stream_offset += 1;
+	data_offset += 4;
 
-	if( ( name_size > internal_value->size )
-	 || ( byte_stream_offset > ( internal_value->size - name_size ) ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_VALUE_OUT_OF_BOUNDS,
-		 "%s: invalid name size value out of bounds.",
-		 function );
+	string_size *= 2;
 
-		return( -1 );
-	}
-	if( internal_value->type == LIBFWPS_RECORD_TYPE_NAMED )
+	if( ( string_size > 0 )
+         && ( string_size <= data_size )
+	 && ( data_offset <= ( data_size - string_size ) ) )
 	{
 #if defined( HAVE_DEBUG_OUTPUT )
 		if( libcnotify_verbose != 0 )
 		{
-#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
-			result = libuna_utf16_string_size_from_utf16_stream(
-				  &( byte_stream[ byte_stream_offset ] ),
-				  name_size,
-				  LIBUNA_ENDIAN_LITTLE,
-				  &value_string_size,
-				  error );
-#else
-			result = libuna_utf8_string_size_from_utf16_stream(
-				  &( byte_stream[ byte_stream_offset ] ),
-				  name_size,
-				  LIBUNA_ENDIAN_LITTLE,
-				  &value_string_size,
-				  error );
-#endif
-			if( result != 1 )
+			if( libfwsi_debug_print_utf16_string_value(
+			     function,
+			     "string\t\t\t\t",
+			     &( data[ data_offset ] ),
+			     string_size,
+			     LIBUNA_ENDIAN_LITTLE,
+			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-				 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-				 "%s: unable to determine size of URI string.",
+				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+				 "%s: unable to print UTF-16 string value.",
 				 function );
 
-				goto on_error;
+				return( -1 );
 			}
-			if( ( value_string_size > (size_t) SSIZE_MAX )
-			 || ( ( sizeof( system_character_t ) * value_string_size )  > (size_t) SSIZE_MAX ) )
-			{
-				libcerror_error_set(
-				 error,
-				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-				 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
-				 "%s: invalid URI string size value exceeds maximum.",
-				 function );
+		}
+#endif
+		data_offset += string_size;
+	}
+	byte_stream_copy_to_uint32_little_endian(
+	 &( data[ data_offset ] ),
+	 string_size );
 
-				goto on_error;
-			}
-			value_string = system_string_allocate(
-					value_string_size );
+#if defined( HAVE_DEBUG_OUTPUT )
+	if( libcnotify_verbose != 0 )
+	{
+		libcnotify_printf(
+		 "%s: string size\t\t\t: %" PRIu32 "\n",
+		 function,
+		 string_size );
+	}
+#endif
+	data_offset += 4;
+
+	string_size *= 2;
 
-			if( value_string == NULL )
+	if( ( string_size > 0 )
+         && ( string_size <= data_size )
+	 && ( data_offset <= ( data_size - string_size ) ) )
+	{
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
+		{
+			if( libfwsi_debug_print_utf16_string_value(
+			     function,
+			     "string\t\t\t\t",
+			     &( data[ data_offset ] ),
+			     string_size,
+			     LIBUNA_ENDIAN_LITTLE,
+			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
-				 LIBCERROR_ERROR_DOMAIN_MEMORY,
-				 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
-				 "%s: unable to create URI string.",
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+				 "%s: unable to print UTF-16 string value.",
 				 function );
 
-				goto on_error;
+				return( -1 );
 			}
-#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
-			result = libuna_utf16_string_copy_from_utf16_stream(
-				  (libuna_utf16_character_t *) value_string,
-				  value_string_size,
-				  &( byte_stream[ byte_stream_offset ] ),
-				  name_size,
-				  LIBUNA_ENDIAN_LITTLE,
-				  error );
-#else
-			result = libuna_utf8_string_copy_from_utf16_stream(
-				  (libuna_utf8_character_t *) value_string,
-				  value_string_size,
-				  &( byte_stream[ byte_stream_offset ] ),
-				  name_size,
-				  LIBUNA_ENDIAN_LITTLE,
-				  error );
+		}
+#endif
+		data_offset += string_size;
+	}
+	byte_stream_copy_to_uint32_little_endian(
+	 &( data[ data_offset ] ),
+	 string_size );
+
+#if defined( HAVE_DEBUG_OUTPUT )
+	if( libcnotify_verbose != 0 )
+	{
+		libcnotify_printf(
+		 "%s: string size\t\t\t: %" PRIu32 "\n",
+		 function,
+		 string_size );
+	}
 #endif
-			if( result != 1 )
+	data_offset += 4;
+
+	string_size *= 2;
+
+	if( ( string_size > 0 )
+         && ( string_size <= data_size )
+	 && ( data_offset <= ( data_size - string_size ) ) )
+	{
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
+		{
+			if( libfwsi_debug_print_utf16_string_value(
+			     function,
+			     "string\t\t\t\t",
+			     &( data[ data_offset ] ),
+			     string_size,
+			     LIBUNA_ENDIAN_LITTLE,
+			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-				 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
-				 "%s: unable to set URI string.",
+				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+				 "%s: unable to print UTF-16 string value.",
 				 function );
 
-				goto on_error;
+				return( -1 );
 			}
-			libcnotify_printf(
-			 "%s: name\t\t\t\t: %" PRIs_SYSTEM "\n",
-			 function,
-			 value_string );
-
-			memory_free(
-			 value_string );
-
-			value_string = NULL;
 		}
 #endif
-		byte_stream_offset += name_size;
+		data_offset += string_size;
+	}
+	byte_stream_copy_to_uint32_little_endian(
+	 &( data[ data_offset ] ),
+	 string_size );
+
+#if defined( HAVE_DEBUG_OUTPUT )
+	if( libcnotify_verbose != 0 )
+	{
+		libcnotify_printf(
+		 "%s: string size\t\t\t: %" PRIu32 "\n",
+		 function,
+		 string_size );
 	}
-	if( byte_stream_offset < internal_value->size )
+#endif
+	data_offset += 4;
+
+	string_size *= 2;
+
+	if( ( string_size > 0 )
+         && ( string_size <= data_size )
+	 && ( data_offset <= ( data_size - string_size ) ) )
 	{
 #if defined( HAVE_DEBUG_OUTPUT )
 		if( libcnotify_verbose != 0 )
 		{
-			libcnotify_printf(
-			 "%s: value data:\n",
-			 function );
-			libcnotify_print_data(
-			 &( byte_stream[ byte_stream_offset ] ),
-			 internal_value->size - byte_stream_offset,
-			 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
+			if( libfwsi_debug_print_utf16_string_value(
+			     function,
+			     "string\t\t\t\t",
+			     &( data[ data_offset ] ),
+			     string_size,
+			     LIBUNA_ENDIAN_LITTLE,
+			     error ) != 1 )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+				 "%s: unable to print UTF-16 string value.",
+				 function );
+
+				return( -1 );
+			}
 		}
 #endif
-		/* TODO read value */
 	}
-
-/* TODO print trailing data */
-
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
 		libcnotify_printf(
 		 "\n" );
 	}
 #endif
 	return( 1 );
-
-on_error:
-#if defined( HAVE_DEBUG_OUTPUT )
-	if( value_string != NULL )
-	{
-		memory_free(
-		 value_string );
-	}
-#endif
-	return( -1 );
 }
```

### Comparing `libfwsi-20230114/libfwps/libfwps_types.h` & `libfwsi-20230710/libfwps/libfwps_types.h`

 * *Files 7% similar despite different names*

```diff
@@ -34,24 +34,18 @@
 /* The following type definitions hide internal data structures
  */
 #if defined( HAVE_DEBUG_OUTPUT ) && !defined( WINAPI )
 typedef struct libfwps_record {}	libfwps_record_t;
 typedef struct libfwps_set {}		libfwps_set_t;
 typedef struct libfwps_store {}		libfwps_store_t;
 
-typedef struct libfwps_storage {}	libfwps_storage_t;
-typedef struct libfwps_value {}		libfwps_value_t;
-
 #else
 typedef intptr_t libfwps_record_t;
 typedef intptr_t libfwps_set_t;
 typedef intptr_t libfwps_store_t;
 
-typedef intptr_t libfwps_storage_t;
-typedef intptr_t libfwps_value_t;
-
 #endif /* defined( HAVE_DEBUG_OUTPUT ) && !defined( WINAPI ) */
 
 #endif /* defined( HAVE_LOCAL_LIBFWPS ) */
 
 #endif /* !defined( _LIBFWPS_INTERNAL_TYPES_H ) */
```

### Comparing `libfwsi-20230114/libfwps/libfwps_record.c` & `libfwsi-20230710/libfwps/libfwps_record.c`

 * *Files 15% similar despite different names*

```diff
@@ -533,21 +533,33 @@
 			internal_record->value_data_size *= 2;
 		}
 	}
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
 		libcnotify_printf(
-		 "%s: value data size\t\t: %" PRIu32 "\n",
+		 "%s: value data size\t\t\t: %" PRIu32 "\n",
 		 function,
 		 internal_record->value_data_size );
 	}
 #endif
 	if( internal_record->value_data_size > 0 )
 	{
+		if( ( internal_record->value_data_size > byte_stream_size )
+		 || ( byte_stream_offset > ( byte_stream_size - internal_record->value_data_size ) ) )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+			 "%s: invalid valud data size value out of bounds.",
+			 function );
+
+			goto on_error;
+		}
 #if defined( HAVE_DEBUG_OUTPUT )
 		if( libcnotify_verbose != 0 )
 		{
 			libcnotify_printf(
 			 "%s: value data:\n",
 			 function );
 			libcnotify_print_data(
@@ -591,14 +603,15 @@
 			 LIBCERROR_ERROR_DOMAIN_MEMORY,
 			 LIBCERROR_MEMORY_ERROR_COPY_FAILED,
 			 "%s: unable to copy value data.",
 			 function );
 
 			goto on_error;
 		}
+		byte_stream_offset += internal_record->value_data_size;
 	}
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
 		if( byte_stream_offset < internal_record->size )
 		{
 			libcnotify_printf(
@@ -1262,14 +1275,15 @@
 
 		*value_floating_point = value_double.floating_point;
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the data formatted as an UTF-8 string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
  * The returned size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 int libfwps_record_get_data_as_utf8_string_size(
      libfwps_record_t *record,
      size_t *utf8_string_size,
      libcerror_error_t **error )
@@ -1288,15 +1302,16 @@
 		 "%s: invalid record entry.",
 		 function );
 
 		return( -1 );
 	}
 	internal_record = (libfwps_internal_record_t *) record;
 
-	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_BINARY_STRING )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
 		 "%s: invalid record entry - unsupported value type.",
@@ -1405,15 +1420,16 @@
 		 "%s: invalid record entry.",
 		 function );
 
 		return( -1 );
 	}
 	internal_record = (libfwps_internal_record_t *) record;
 
-	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_BINARY_STRING )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
 		 "%s: invalid record entry - unsupported value type.",
@@ -1510,14 +1526,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the data formatted as an UTF-16 string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
  * The returned size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 int libfwps_record_get_data_as_utf16_string_size(
      libfwps_record_t *record,
      size_t *utf16_string_size,
      libcerror_error_t **error )
@@ -1536,15 +1553,16 @@
 		 "%s: invalid record entry.",
 		 function );
 
 		return( -1 );
 	}
 	internal_record = (libfwps_internal_record_t *) record;
 
-	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_BINARY_STRING )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
 		 "%s: invalid record entry - unsupported value type.",
@@ -1653,15 +1671,16 @@
 		 "%s: invalid record entry.",
 		 function );
 
 		return( -1 );
 	}
 	internal_record = (libfwps_internal_record_t *) record;
 
-	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_BINARY_STRING )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
 	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
 		 "%s: invalid record entry - unsupported value type.",
@@ -1716,14 +1735,520 @@
 		          error );
 	}
 	/* Codepage 65000 represents UTF-7
 	 */
 	else if( internal_record->ascii_codepage == 65000 )
 	{
 		result = libuna_utf16_string_copy_from_utf7_stream(
+		          utf16_string,
+		          utf16_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          error );
+	}
+	/* Codepage 65001 represents UTF-8
+	 */
+	else if( internal_record->ascii_codepage == 65001 )
+	{
+		result = libuna_utf16_string_copy_from_utf8_stream(
+		          utf16_string,
+		          utf16_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          error );
+	}
+	else
+	{
+		result = libuna_utf16_string_copy_from_byte_stream(
+		          utf16_string,
+		          utf16_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          internal_record->ascii_codepage,
+		          error );
+	}
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
+		 "%s: unable to copy value data to UTF-16 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the size of the data formatted as an UTF-8 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The returned size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_data_as_utf8_path_string_size(
+     libfwps_record_t *record,
+     size_t *utf8_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_data_as_utf8_path_string_size";
+	uint8_t is_ascii_string                    = 0;
+	int result                                 = 0;
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record entry.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_BINARY_STRING )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid record entry - unsupported value type.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string_size == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 string size.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( internal_record->value_data == NULL )
+	 || ( internal_record->value_data_size == 0 ) )
+	{
+		*utf8_string_size = 0;
+
+		return( 1 );
+	}
+	if( internal_record->value_type == LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	{
+		is_ascii_string = 1;
+	}
+	/* String is in UTF-16 little-endian
+	 */
+	if( is_ascii_string == 0 )
+	{
+		result = libuna_utf8_string_size_from_utf16_stream(
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
+		          utf8_string_size,
+		          error );
+	}
+	/* Codepage 65000 represents UTF-7
+	 */
+	else if( internal_record->ascii_codepage == 65000 )
+	{
+		result = libuna_utf8_string_size_from_utf7_stream(
+			  internal_record->value_data,
+			  internal_record->value_data_size,
+			  utf8_string_size,
+			  error );
+	}
+	/* Codepage 65001 represents UTF-8
+	 */
+	else if( internal_record->ascii_codepage == 65001 )
+	{
+		result = libuna_utf8_string_size_from_utf8_stream(
+			  internal_record->value_data,
+			  internal_record->value_data_size,
+			  utf8_string_size,
+			  error );
+	}
+	else
+	{
+		result = libuna_utf8_string_size_from_byte_stream(
+			  internal_record->value_data,
+			  internal_record->value_data_size,
+			  internal_record->ascii_codepage,
+			  utf8_string_size,
+			  error );
+	}
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to determine size of value data as UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the data formatted as an UTF-8 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_data_as_utf8_path_string(
+     libfwps_record_t *record,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_data_as_utf8_path_string";
+	uint8_t is_ascii_string                    = 0;
+	int result                                 = 0;
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record entry.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_BINARY_STRING )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid record entry - unsupported value type.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( utf8_string_size == 0 )
+	 || ( utf8_string_size > (size_t) SSIZE_MAX ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_OUT_OF_BOUNDS,
+		 "%s: invalid UTF-8 string size value out of bounds.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( internal_record->value_data == NULL )
+	 || ( internal_record->value_data_size == 0 ) )
+	{
+		utf8_string[ 0 ] = 0;
+
+		return( 1 );
+	}
+	if( internal_record->value_type == LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	{
+		is_ascii_string = 1;
+	}
+	/* String is in UTF-16 little-endian
+	 */
+	if( is_ascii_string == 0 )
+	{
+		result = libuna_utf8_string_copy_from_utf16_stream(
+		          utf8_string,
+		          utf8_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
+		          error );
+	}
+	/* Codepage 65000 represents UTF-7
+	 */
+	else if( internal_record->ascii_codepage == 65000 )
+	{
+		result = libuna_utf8_string_copy_from_utf7_stream(
+		          utf8_string,
+		          utf8_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          error );
+	}
+	/* Codepage 65001 represents UTF-8
+	 */
+	else if( internal_record->ascii_codepage == 65001 )
+	{
+		result = libuna_utf8_string_copy_from_utf8_stream(
+		          utf8_string,
+		          utf8_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          error );
+	}
+	else
+	{
+		result = libuna_utf8_string_copy_from_byte_stream(
+		          utf8_string,
+		          utf8_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          internal_record->ascii_codepage,
+		          error );
+	}
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
+		 "%s: unable to copy value data to UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the size of the data formatted as an UTF-16 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The returned size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_data_as_utf16_path_string_size(
+     libfwps_record_t *record,
+     size_t *utf16_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_data_as_utf16_path_string_size";
+	uint8_t is_ascii_string                    = 0;
+	int result                                 = 0;
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record entry.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_BINARY_STRING )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid record entry - unsupported value type.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf16_string_size == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-16 string size.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( internal_record->value_data == NULL )
+	 || ( internal_record->value_data_size == 0 ) )
+	{
+		*utf16_string_size = 0;
+
+		return( 1 );
+	}
+	if( internal_record->value_type == LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	{
+		is_ascii_string = 1;
+	}
+	/* String is in UTF-16 little-endian
+	 */
+	if( is_ascii_string == 0 )
+	{
+		result = libuna_utf16_string_size_from_utf16_stream(
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
+		          utf16_string_size,
+		          error );
+	}
+	/* Codepage 65000 represents UTF-7
+	 */
+	else if( internal_record->ascii_codepage == 65000 )
+	{
+		result = libuna_utf16_string_size_from_utf7_stream(
+			  internal_record->value_data,
+			  internal_record->value_data_size,
+			  utf16_string_size,
+			  error );
+	}
+	/* Codepage 65001 represents UTF-8
+	 */
+	else if( internal_record->ascii_codepage == 65001 )
+	{
+		result = libuna_utf16_string_size_from_utf8_stream(
+			  internal_record->value_data,
+			  internal_record->value_data_size,
+			  utf16_string_size,
+			  error );
+	}
+	else
+	{
+		result = libuna_utf16_string_size_from_byte_stream(
+			  internal_record->value_data,
+			  internal_record->value_data_size,
+			  internal_record->ascii_codepage,
+			  utf16_string_size,
+			  error );
+	}
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to determine size of value data as UTF-16 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the data formatted as an UTF-16 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_data_as_utf16_path_string(
+     libfwps_record_t *record,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_data_as_utf16_path_string";
+	uint8_t is_ascii_string                    = 0;
+	int result                                 = 0;
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record entry.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_BINARY_STRING )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid record entry - unsupported value type.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf16_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-16 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( utf16_string_size == 0 )
+	 || ( utf16_string_size > (size_t) SSIZE_MAX ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_OUT_OF_BOUNDS,
+		 "%s: invalid UTF-16 string size value out of bounds.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( internal_record->value_data == NULL )
+	 || ( internal_record->value_data_size == 0 ) )
+	{
+		utf16_string[ 0 ] = 0;
+
+		return( 1 );
+	}
+	if( internal_record->value_type == LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	{
+		is_ascii_string = 1;
+	}
+	/* String is in UTF-16 little-endian
+	 */
+	if( is_ascii_string == 0 )
+	{
+		result = libuna_utf16_string_copy_from_utf16_stream(
+		          utf16_string,
+		          utf16_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
+		          error );
+	}
+	/* Codepage 65000 represents UTF-7
+	 */
+	else if( internal_record->ascii_codepage == 65000 )
+	{
+		result = libuna_utf16_string_copy_from_utf7_stream(
 		          utf16_string,
 		          utf16_string_size,
 		          internal_record->value_data,
 		          internal_record->value_data_size,
 		          error );
 	}
 	/* Codepage 65001 represents UTF-8
```

### Comparing `libfwsi-20230114/libfwps/libfwps_unused.h` & `libfwsi-20230710/libfwps/libfwps_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_support.h` & `libfwsi-20230710/libfwps/libfwps_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_storage.h` & `libfwsi-20230710/libfwsi/libfwsi_support.h`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows Serialized Property Storage functions
+ * Support functions
  *
- * Copyright (C) 2013-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,54 +15,33 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFWPS_INTERNAL_STORAGE_H )
-#define _LIBFWPS_INTERNAL_STORAGE_H
+#if !defined( _LIBFWSI_SUPPORT_H )
+#define _LIBFWSI_SUPPORT_H
 
 #include <common.h>
 #include <types.h>
 
-#include "libfwps_extern.h"
-#include "libfwps_libcerror.h"
-#include "libfwps_types.h"
+#include "libfwsi_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-typedef struct libfwps_internal_storage libfwps_internal_storage_t;
+#if !defined( HAVE_LOCAL_LIBFWSI )
 
-struct libfwps_internal_storage
-{
-	/* The size
-	 */
-	uint32_t size;
-};
-
-LIBFWPS_EXTERN \
-int libfwps_storage_initialize(
-     libfwps_storage_t **storage,
-     libcerror_error_t **error );
-
-LIBFWPS_EXTERN \
-int libfwps_storage_free(
-     libfwps_storage_t **storage,
-     libcerror_error_t **error );
-
-LIBFWPS_EXTERN \
-int libfwps_storage_copy_from_byte_stream(
-     libfwps_storage_t *storage,
-     const uint8_t *byte_stream,
-     size_t byte_stream_size,
-     int ascii_codepage,
-     libcerror_error_t **error );
+LIBFWSI_EXTERN \
+const char *libfwsi_get_version(
+             void );
+
+#endif
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBFWPS_INTERNAL_STORAGE_H ) */
+#endif /* !defined( _LIBFWSI_SUPPORT_H ) */
```

### Comparing `libfwsi-20230114/libfwps/libfwps_set.h` & `libfwsi-20230710/libfwps/libfwps_set.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwps/libfwps_error.h` & `libfwsi-20230710/libfwps/libfwps_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/common/config_msc.h` & `libfwsi-20230710/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/common/byte_stream.h` & `libfwsi-20230710/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/common/common.h` & `libfwsi-20230710/common/common.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/common/system_string.h` & `libfwsi-20230710/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/common/types.h` & `libfwsi-20230710/common/types.h`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 
 #define PRIc_SYSTEM "c"
 #define PRIs_SYSTEM "s"
 
 #endif /* defined( WINAPI ) && ( defined( _UNICODE ) || defined( UNICODE ) ) */
 
 /* Fallback for systems without PRI definitions
+ * Do not define when pyconfig.h has been included via python.h
  */
+#if !defined( HAVE_PYCONFIG_H )
+
 #if !defined( PRId8 )
 #define PRId8 "d"
 #endif
 
 #if !defined( PRId16 )
 #define PRId16 "d"
 #endif
@@ -212,14 +215,16 @@
 
 #else
 #define PRIx64 "llx"
 
 #endif
 #endif /* !defined( PRIx64 ) */
 
+#endif /* !defined( HAVE_PYCONFIG_H ) */
+
 /* Fallback for systems without printf %jd definition
  */
 #if defined( HAVE_PRINTF_JD )
 #define PRIjd	"jd"
 #define PRIji	"ji"
 #define PRIju	"ju"
 #define PRIjx	"jx"
```

### Comparing `libfwsi-20230114/common/types.h.in` & `libfwsi-20230710/common/types.h.in`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 
 #define PRIc_SYSTEM "c"
 #define PRIs_SYSTEM "s"
 
 #endif /* defined( WINAPI ) && ( defined( _UNICODE ) || defined( UNICODE ) ) */
 
 /* Fallback for systems without PRI definitions
+ * Do not define when pyconfig.h has been included via python.h
  */
+#if !defined( HAVE_PYCONFIG_H )
+
 #if !defined( PRId8 )
 #define PRId8 "d"
 #endif
 
 #if !defined( PRId16 )
 #define PRId16 "d"
 #endif
@@ -212,14 +215,16 @@
 
 #else
 #define PRIx64 "llx"
 
 #endif
 #endif /* !defined( PRIx64 ) */
 
+#endif /* !defined( HAVE_PYCONFIG_H ) */
+
 /* Fallback for systems without printf %jd definition
  */
 #if defined( HAVE_PRINTF_JD )
 #define PRIjd	"jd"
 #define PRIji	"ji"
 #define PRIju	"ju"
 #define PRIjx	"jx"
```

### Comparing `libfwsi-20230114/common/config_winapi.h` & `libfwsi-20230710/common/config_winapi.h`

 * *Files 6% similar despite different names*

```diff
@@ -41,23 +41,28 @@
 /* Define the size of the integer for WINAPI
  */
 #if !defined( SIZEOF_INT )
 #define SIZEOF_INT			4
 #endif
 
 /* Define the size of size_t for WINAPI
+ * Do not define when pyconfig.h has been included via python.h
  */
+#if !defined( HAVE_PYCONFIG_H )
+
 #if !defined( SIZEOF_SIZE_T )
 #if __WORDSIZE == 64
 #define SIZEOF_SIZE_T			8
 #else
 #define SIZEOF_SIZE_T			4
 #endif
 #endif
 
+#endif /* !defined( HAVE_PYCONFIG_H ) */
+
 /* Define the size of the wide character for WINAPI
  */
 #if !defined( SIZEOF_WCHAR_T )
 #define SIZEOF_WCHAR_T			2
 #endif
 
 /* Enable the DllMain function
```

### Comparing `libfwsi-20230114/common/memory.h` & `libfwsi-20230710/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/common/config.h` & `libfwsi-20230710/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -403,24 +403,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfwsi"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfwsi 20230114"
+#define PACKAGE_STRING "libfwsi 20230710"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfwsi"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20230114"
+#define PACKAGE_VERSION "20230710"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -438,15 +438,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20230114"
+#define VERSION "20230710"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfwsi-20230114/common/narrow_string.h` & `libfwsi-20230710/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/common/Makefile.in` & `libfwsi-20230710/common/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/common/file_stream.h` & `libfwsi-20230710/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/common/config_borlandc.h` & `libfwsi-20230710/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/common/config.h.in` & `libfwsi-20230710/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/common/wide_string.h` & `libfwsi-20230710/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfole/libfole_definitions.h` & `libfwsi-20230710/libfole/libfole_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfole/Makefile.am` & `libfwsi-20230710/libfole/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfole/libfole_support.h` & `libfwsi-20230710/libfole/libfole_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfole/libfole_extern.h` & `libfwsi-20230710/libfole/libfole_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfole/libfole_error.c` & `libfwsi-20230710/libfole/libfole_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfole/libfole_libcerror.h` & `libfwsi-20230710/libfole/libfole_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfole/libfole_value_type.h` & `libfwsi-20230710/libfole/libfole_value_type.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfole/libfole_unused.h` & `libfwsi-20230710/libfole/libfole_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfole/libfole_value_type.c` & `libfwsi-20230710/libfole/libfole_value_type.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfole/libfole_error.h` & `libfwsi-20230710/libfole/libfole_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfole/Makefile.in` & `libfwsi-20230710/libfole/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfole/libfole_support.c` & `libfwsi-20230710/libfole/libfole_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfole/libfole_types.h` & `libfwsi-20230710/libfole/libfole_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfguid/libfguid_identifier.c` & `libfwsi-20230710/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfguid/libfguid_support.c` & `libfwsi-20230710/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfguid/Makefile.am` & `libfwsi-20230710/libfguid/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfguid/libfguid_support.h` & `libfwsi-20230710/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfguid/libfguid_definitions.h` & `libfwsi-20230710/libfguid/libfguid_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfguid/libfguid_identifier.h` & `libfwsi-20230710/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfguid/libfguid_unused.h` & `libfwsi-20230710/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfguid/libfguid_error.h` & `libfwsi-20230710/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfguid/libfguid_libcerror.h` & `libfwsi-20230710/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfguid/Makefile.in` & `libfwsi-20230710/libfguid/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfguid/libfguid_error.c` & `libfwsi-20230710/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfguid/libfguid_types.h` & `libfwsi-20230710/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfguid/libfguid_extern.h` & `libfwsi-20230710/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_libcerror.h` & `libfwsi-20230710/tests/fwsi_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/pyfwsi_test_support.py` & `libfwsi-20230710/tests/pyfwsi_test_support.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_users_property_view_values.c` & `libfwsi-20230710/tests/fwsi_test_users_property_view_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_error.c` & `libfwsi-20230710/tests/fwsi_test_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_file_entry_extension_values.c` & `libfwsi-20230710/tests/fwsi_test_file_entry_extension_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/test_library.sh` & `libfwsi-20230710/tests/test_library.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#!/bin/bash
+#!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20200705
+# Version: 20230410
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="cdburn_values compressed_folder_values control_panel_category_values control_panel_cpl_file_values control_panel_values delegate_values error extension_block extension_block_0xbeef0000_values extension_block_0xbeef0001_values extension_block_0xbeef0003_values extension_block_0xbeef0005_values extension_block_0xbeef0006_values extension_block_0xbeef000a_values extension_block_0xbeef0013_values extension_block_0xbeef0014_values extension_block_0xbeef0019_values extension_block_0xbeef0025_values file_entry_extension_values file_entry_values game_folder_values item item_list mtp_file_entry_values mtp_volume_values network_location_values root_folder_values support unknown_0x74_values uri_values uri_sub_values users_property_view_values volume_values";
 LIBRARY_TESTS_WITH_INPUT="";
```

### Comparing `libfwsi-20230114/tests/pyfwsi_test_file_entry.py` & `libfwsi-20230710/tests/pyfwsi_test_file_entry.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/pyfwsi_test_item_list.py` & `libfwsi-20230710/tests/pyfwsi_test_item_list.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_root_folder_values.c` & `libfwsi-20230710/tests/fwsi_test_root_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/test_python_module.sh` & `libfwsi-20230710/tests/test_python_module.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#!/bin/bash
+#!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20200705
+# Version: 20230410
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="volume";
```

### Comparing `libfwsi-20230114/tests/fwsi_test_mtp_file_entry_values.c` & `libfwsi-20230710/tests/fwsi_test_mtp_file_entry_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_item.c` & `libfwsi-20230710/tests/fwsi_test_item.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/Makefile.am` & `libfwsi-20230710/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0013_values.c` & `libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0013_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_memory.c` & `libfwsi-20230710/tests/fwsi_test_memory.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/pyfwsi_test_root_folder.py` & `libfwsi-20230710/tests/pyfwsi_test_root_folder.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0001_values.c` & `libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0001_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_memory.h` & `libfwsi-20230710/tests/fwsi_test_memory.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_unused.h` & `libfwsi-20230710/tests/fwsi_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_game_folder_values.c` & `libfwsi-20230710/tests/fwsi_test_game_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_uri_sub_values.c` & `libfwsi-20230710/tests/fwsi_test_uri_sub_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_file_entry_values.c` & `libfwsi-20230710/tests/fwsi_test_file_entry_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_uri_values.c` & `libfwsi-20230710/tests/fwsi_test_uri_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/test_manpage.sh` & `libfwsi-20230710/tests/test_manpage.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#!/bin/bash
+#!/usr/bin/env bash
 # Tests man pages.
 #
-# Version: 20190302
+# Version: 20230410
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 run_test()
 {
```

### Comparing `libfwsi-20230114/tests/fwsi_test_volume_values.c` & `libfwsi-20230710/tests/fwsi_test_volume_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0005_values.c` & `libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0005_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_control_panel_category_values.c` & `libfwsi-20230710/tests/fwsi_test_control_panel_category_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_control_panel_values.c` & `libfwsi-20230710/tests/fwsi_test_control_panel_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_item_list.c` & `libfwsi-20230710/tests/fwsi_test_item_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_network_location_values.c` & `libfwsi-20230710/tests/fwsi_test_network_location_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_unknown_0x74_values.c` & `libfwsi-20230710/tests/fwsi_test_unknown_0x74_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/test_runner.sh` & `libfwsi-20230710/tests/test_runner.sh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#!/bin/bash
+#!/usr/bin/env bash
 # Bash functions to run an executable for testing.
 #
-# Version: 20220924
+# Version: 20230410
 #
 # When CHECK_WITH_ASAN is set to a non-empty value the test executable
 # is run with asan, otherwise it is run without.
 #
 # When CHECK_WITH_GDB is set to a non-empty value the test executable
 # is run with gdb, otherwise it is run without.
 #
```

### Comparing `libfwsi-20230114/tests/pyfwsi_test_volume.py` & `libfwsi-20230710/tests/pyfwsi_test_volume.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/pyfwsi_test_extension_block.py` & `libfwsi-20230710/tests/pyfwsi_test_extension_block.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_mtp_volume_values.c` & `libfwsi-20230710/tests/fwsi_test_mtp_volume_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0000_values.c` & `libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0000_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/pyfwsi_test_item.py` & `libfwsi-20230710/tests/pyfwsi_test_item.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/pyfwsi_test_network_location.py` & `libfwsi-20230710/tests/pyfwsi_test_network_location.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/Makefile.in` & `libfwsi-20230710/tests/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0019_values.c` & `libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0019_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_cdburn_values.c` & `libfwsi-20230710/tests/fwsi_test_cdburn_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef000a_values.c` & `libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef000a_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0025_values.c` & `libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0025_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0003_values.c` & `libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0003_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_extension_block.c` & `libfwsi-20230710/tests/fwsi_test_extension_block.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_delegate_values.c` & `libfwsi-20230710/tests/fwsi_test_delegate_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_libfwsi.h` & `libfwsi-20230710/tests/fwsi_test_libfwsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_support.c` & `libfwsi-20230710/tests/fwsi_test_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0014_values.c` & `libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0014_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_extension_block_0xbeef0006_values.c` & `libfwsi-20230710/tests/fwsi_test_extension_block_0xbeef0006_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_macros.h` & `libfwsi-20230710/tests/fwsi_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_compressed_folder_values.c` & `libfwsi-20230710/tests/fwsi_test_compressed_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/tests/fwsi_test_control_panel_cpl_file_values.c` & `libfwsi-20230710/tests/fwsi_test_control_panel_cpl_file_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_error.c` & `libfwsi-20230710/pyfwsi/pyfwsi_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_extension_block.h` & `libfwsi-20230710/pyfwsi/pyfwsi_extension_block.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_extension_blocks.h` & `libfwsi-20230710/pyfwsi/pyfwsi_extension_blocks.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_items.h` & `libfwsi-20230710/pyfwsi/pyfwsi_items.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_root_folder.h` & `libfwsi-20230710/pyfwsi/pyfwsi_root_folder.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_guid.h` & `libfwsi-20230710/pyfwsi/pyfwsi_guid.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_item_list.c` & `libfwsi-20230710/pyfwsi/pyfwsi_item_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_codepage.h` & `libfwsi-20230710/pyfwsi/pyfwsi_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi.c` & `libfwsi-20230710/pyfwsi/pyfwsi.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/Makefile.am` & `libfwsi-20230710/pyfwsi/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,19 @@
 	pyfwsi_item.c pyfwsi_item.h \
 	pyfwsi_item_list.c pyfwsi_item_list.h \
 	pyfwsi_items.c pyfwsi_items.h \
 	pyfwsi_libcerror.h \
 	pyfwsi_libclocale.h \
 	pyfwsi_libfguid.h \
 	pyfwsi_libfwsi.h \
+	pyfwsi_libuna.h \
 	pyfwsi_network_location.c pyfwsi_network_location.h \
 	pyfwsi_python.h \
 	pyfwsi_root_folder.c pyfwsi_root_folder.h \
+	pyfwsi_string.c pyfwsi_string.h \
 	pyfwsi_unused.h \
 	pyfwsi_volume.c pyfwsi_volume.h
 
 pyfwsi_la_LIBADD = \
 	@LIBCERROR_LIBADD@ \
 	../libfwsi/libfwsi.la \
 	@LIBCDATA_LIBADD@ \
```

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_item.c` & `libfwsi-20230710/pyfwsi/pyfwsi_item.c`

 * *Files 0% similar despite different names*

```diff
@@ -689,15 +689,15 @@
 	}
 	data = (uint8_t *) PyMem_Malloc(
 	                    sizeof( uint8_t ) * data_size );
 
 	if( data == NULL )
 	{
 		PyErr_Format(
-		 PyExc_IOError,
+		 PyExc_MemoryError,
 		 "%s: unable to create data.",
 		 function );
 
 		goto on_error;
 	}
 	Py_BEGIN_ALLOW_THREADS
```

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_integer.c` & `libfwsi-20230710/pyfwsi/pyfwsi_integer.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_unused.h` & `libfwsi-20230710/pyfwsi/pyfwsi_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_volume.c` & `libfwsi-20230710/pyfwsi/pyfwsi_volume.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_file_entry.c` & `libfwsi-20230710/pyfwsi/pyfwsi_file_entry.c`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 #include "pyfwsi_error.h"
 #include "pyfwsi_file_entry.h"
 #include "pyfwsi_integer.h"
 #include "pyfwsi_item.h"
 #include "pyfwsi_libcerror.h"
 #include "pyfwsi_libfwsi.h"
 #include "pyfwsi_python.h"
+#include "pyfwsi_string.h"
 #include "pyfwsi_unused.h"
 
 PyMethodDef pyfwsi_file_entry_object_methods[] = {
 
 	{ "get_file_size",
 	  (PyCFunction) pyfwsi_file_entry_get_file_size,
 	  METH_NOARGS,
@@ -413,20 +414,20 @@
 /* Retrieves the name
  * Returns a Python object if successful or NULL on error
  */
 PyObject *pyfwsi_file_entry_get_name(
            pyfwsi_item_t *pyfwsi_item,
            PyObject *arguments PYFWSI_ATTRIBUTE_UNUSED )
 {
-	libcerror_error_t *error = NULL;
 	PyObject *string_object  = NULL;
+	libcerror_error_t *error = NULL;
+	uint8_t *utf8_string     = NULL;
 	const char *errors       = NULL;
-	uint8_t *name            = NULL;
 	static char *function    = "pyfwsi_file_entry_get_name";
-	size_t name_size         = 0;
+	size_t utf8_string_size  = 0;
 	int result               = 0;
 
 	PYFWSI_UNREFERENCED_PARAMETER( arguments )
 
 	if( pyfwsi_item == NULL )
 	{
 		PyErr_Format(
@@ -436,91 +437,105 @@
 
 		return( NULL );
 	}
 	Py_BEGIN_ALLOW_THREADS
 
 	result = libfwsi_file_entry_get_utf8_name_size(
 	          pyfwsi_item->item,
-	          &name_size,
+	          &utf8_string_size,
 	          &error );
 
 	Py_END_ALLOW_THREADS
 
 	if( result == -1 )
 	{
 		pyfwsi_error_raise(
 		 error,
 		 PyExc_IOError,
-		 "%s: unable to retrieve name size.",
+		 "%s: unable to determine size of name as UTF-8 string.",
 		 function );
 
 		libcerror_error_free(
 		 &error );
 
 		goto on_error;
 	}
 	else if( ( result == 0 )
-	      || ( name_size == 0 ) )
+	      || ( utf8_string_size == 0 ) )
 	{
 		Py_IncRef(
 		 Py_None );
 
 		return( Py_None );
 	}
-	name = (uint8_t *) PyMem_Malloc(
-	                    sizeof( uint8_t ) * name_size );
+	utf8_string = (uint8_t *) PyMem_Malloc(
+	                           sizeof( uint8_t ) * utf8_string_size );
 
-	if( name == NULL )
+	if( utf8_string == NULL )
 	{
 		PyErr_Format(
-		 PyExc_IOError,
+		 PyExc_MemoryError,
 		 "%s: unable to create name.",
 		 function );
 
 		goto on_error;
 	}
 	Py_BEGIN_ALLOW_THREADS
 
 	result = libfwsi_file_entry_get_utf8_name(
 		  pyfwsi_item->item,
-		  name,
-		  name_size,
+		  utf8_string,
+		  utf8_string_size,
 		  &error );
 
 	Py_END_ALLOW_THREADS
 
 	if( result != 1 )
 	{
 		pyfwsi_error_raise(
 		 error,
 		 PyExc_IOError,
-		 "%s: unable to retrieve name.",
+		 "%s: unable to retrieve name as UTF-8 string.",
 		 function );
 
 		libcerror_error_free(
 		 &error );
 
 		goto on_error;
 	}
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
+	string_object = pyfwsi_string_new_from_utf8_rfc2279(
+			 (uint8_t *) utf8_string,
+			 utf8_string_size );
+#else
 	/* Pass the string length to PyUnicode_DecodeUTF8
 	 * otherwise it makes the end of string character is part
 	 * of the string
 	 */
 	string_object = PyUnicode_DecodeUTF8(
-			 (char *) name,
-			 (Py_ssize_t) name_size - 1,
-			 errors );
+	                 utf8_string,
+	                 (Py_ssize_t) utf8_string_size - 1,
+	                 NULL );
+#endif
+	if( string_object == NULL )
+	{
+		PyErr_Format(
+		 PyExc_IOError,
+		 "%s: unable to convert UTF-8 string into Unicode object.",
+		 function );
 
+		goto on_error;
+	}
 	PyMem_Free(
-	 name );
+	 utf8_string );
 
 	return( string_object );
 
 on_error:
-	if( name != NULL )
+	if( utf8_string != NULL )
 	{
 		PyMem_Free(
-		 name );
+		 utf8_string );
 	}
 	return( NULL );
 }
```

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_libclocale.h` & `libfwsi-20230710/pyfwsi/pyfwsi_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_codepage.c` & `libfwsi-20230710/pyfwsi/pyfwsi_codepage.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_integer.h` & `libfwsi-20230710/pyfwsi/pyfwsi_integer.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_python.h` & `libfwsi-20230710/pyfwsi/pyfwsi_python.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_items.c` & `libfwsi-20230710/pyfwsi/pyfwsi_items.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/Makefile.in` & `libfwsi-20230710/pyfwsi/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -150,18 +150,19 @@
 	pyfwsi_extension_block.h pyfwsi_extension_blocks.c \
 	pyfwsi_extension_blocks.h pyfwsi_file_entry.c \
 	pyfwsi_file_entry.h pyfwsi_file_entry_extension.c \
 	pyfwsi_file_entry_extension.h pyfwsi_guid.c pyfwsi_guid.h \
 	pyfwsi_integer.c pyfwsi_integer.h pyfwsi_item.c pyfwsi_item.h \
 	pyfwsi_item_list.c pyfwsi_item_list.h pyfwsi_items.c \
 	pyfwsi_items.h pyfwsi_libcerror.h pyfwsi_libclocale.h \
-	pyfwsi_libfguid.h pyfwsi_libfwsi.h pyfwsi_network_location.c \
-	pyfwsi_network_location.h pyfwsi_python.h pyfwsi_root_folder.c \
-	pyfwsi_root_folder.h pyfwsi_unused.h pyfwsi_volume.c \
-	pyfwsi_volume.h
+	pyfwsi_libfguid.h pyfwsi_libfwsi.h pyfwsi_libuna.h \
+	pyfwsi_network_location.c pyfwsi_network_location.h \
+	pyfwsi_python.h pyfwsi_root_folder.c pyfwsi_root_folder.h \
+	pyfwsi_string.c pyfwsi_string.h pyfwsi_unused.h \
+	pyfwsi_volume.c pyfwsi_volume.h
 @HAVE_PYTHON_TRUE@am_pyfwsi_la_OBJECTS = pyfwsi_la-pyfwsi.lo \
 @HAVE_PYTHON_TRUE@	pyfwsi_la-pyfwsi_codepage.lo \
 @HAVE_PYTHON_TRUE@	pyfwsi_la-pyfwsi_datetime.lo \
 @HAVE_PYTHON_TRUE@	pyfwsi_la-pyfwsi_error.lo \
 @HAVE_PYTHON_TRUE@	pyfwsi_la-pyfwsi_extension_block.lo \
 @HAVE_PYTHON_TRUE@	pyfwsi_la-pyfwsi_extension_blocks.lo \
 @HAVE_PYTHON_TRUE@	pyfwsi_la-pyfwsi_file_entry.lo \
@@ -169,14 +170,15 @@
 @HAVE_PYTHON_TRUE@	pyfwsi_la-pyfwsi_guid.lo \
 @HAVE_PYTHON_TRUE@	pyfwsi_la-pyfwsi_integer.lo \
 @HAVE_PYTHON_TRUE@	pyfwsi_la-pyfwsi_item.lo \
 @HAVE_PYTHON_TRUE@	pyfwsi_la-pyfwsi_item_list.lo \
 @HAVE_PYTHON_TRUE@	pyfwsi_la-pyfwsi_items.lo \
 @HAVE_PYTHON_TRUE@	pyfwsi_la-pyfwsi_network_location.lo \
 @HAVE_PYTHON_TRUE@	pyfwsi_la-pyfwsi_root_folder.lo \
+@HAVE_PYTHON_TRUE@	pyfwsi_la-pyfwsi_string.lo \
 @HAVE_PYTHON_TRUE@	pyfwsi_la-pyfwsi_volume.lo
 pyfwsi_la_OBJECTS = $(am_pyfwsi_la_OBJECTS)
 AM_V_lt = $(am__v_lt_@AM_V@)
 am__v_lt_ = $(am__v_lt_@AM_DEFAULT_V@)
 am__v_lt_0 = --silent
 am__v_lt_1 = 
 pyfwsi_la_LINK = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
@@ -209,14 +211,15 @@
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_guid.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_integer.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_item.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_item_list.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_items.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_network_location.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Plo \
+	./$(DEPDIR)/pyfwsi_la-pyfwsi_string.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_volume.Plo
 am__mv = mv -f
 COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
 	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
 LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) \
 	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
@@ -579,17 +582,19 @@
 @HAVE_PYTHON_TRUE@	pyfwsi_item.c pyfwsi_item.h \
 @HAVE_PYTHON_TRUE@	pyfwsi_item_list.c pyfwsi_item_list.h \
 @HAVE_PYTHON_TRUE@	pyfwsi_items.c pyfwsi_items.h \
 @HAVE_PYTHON_TRUE@	pyfwsi_libcerror.h \
 @HAVE_PYTHON_TRUE@	pyfwsi_libclocale.h \
 @HAVE_PYTHON_TRUE@	pyfwsi_libfguid.h \
 @HAVE_PYTHON_TRUE@	pyfwsi_libfwsi.h \
+@HAVE_PYTHON_TRUE@	pyfwsi_libuna.h \
 @HAVE_PYTHON_TRUE@	pyfwsi_network_location.c pyfwsi_network_location.h \
 @HAVE_PYTHON_TRUE@	pyfwsi_python.h \
 @HAVE_PYTHON_TRUE@	pyfwsi_root_folder.c pyfwsi_root_folder.h \
+@HAVE_PYTHON_TRUE@	pyfwsi_string.c pyfwsi_string.h \
 @HAVE_PYTHON_TRUE@	pyfwsi_unused.h \
 @HAVE_PYTHON_TRUE@	pyfwsi_volume.c pyfwsi_volume.h
 
 @HAVE_PYTHON_TRUE@pyfwsi_la_LIBADD = \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_PYTHON_TRUE@	../libfwsi/libfwsi.la \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_LIBADD@ \
@@ -691,14 +696,15 @@
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_guid.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_integer.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_item.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_item_list.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_items.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_network_location.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Plo@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_string.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_volume.Plo@am__quote@ # am--include-marker
 
 $(am__depfiles_remade):
 	@$(MKDIR_P) $(@D)
 	@echo '# dummy' >$@-t && $(am__mv) $@-t $@
 
 am--depfiles: $(am__depfiles_remade)
@@ -825,14 +831,21 @@
 pyfwsi_la-pyfwsi_root_folder.lo: pyfwsi_root_folder.c
 @am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pyfwsi_la-pyfwsi_root_folder.lo -MD -MP -MF $(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Tpo -c -o pyfwsi_la-pyfwsi_root_folder.lo `test -f 'pyfwsi_root_folder.c' || echo '$(srcdir)/'`pyfwsi_root_folder.c
 @am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Tpo $(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Plo
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pyfwsi_root_folder.c' object='pyfwsi_la-pyfwsi_root_folder.lo' libtool=yes @AMDEPBACKSLASH@
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
 @am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pyfwsi_la-pyfwsi_root_folder.lo `test -f 'pyfwsi_root_folder.c' || echo '$(srcdir)/'`pyfwsi_root_folder.c
 
+pyfwsi_la-pyfwsi_string.lo: pyfwsi_string.c
+@am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pyfwsi_la-pyfwsi_string.lo -MD -MP -MF $(DEPDIR)/pyfwsi_la-pyfwsi_string.Tpo -c -o pyfwsi_la-pyfwsi_string.lo `test -f 'pyfwsi_string.c' || echo '$(srcdir)/'`pyfwsi_string.c
+@am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pyfwsi_la-pyfwsi_string.Tpo $(DEPDIR)/pyfwsi_la-pyfwsi_string.Plo
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pyfwsi_string.c' object='pyfwsi_la-pyfwsi_string.lo' libtool=yes @AMDEPBACKSLASH@
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
+@am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pyfwsi_la-pyfwsi_string.lo `test -f 'pyfwsi_string.c' || echo '$(srcdir)/'`pyfwsi_string.c
+
 pyfwsi_la-pyfwsi_volume.lo: pyfwsi_volume.c
 @am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pyfwsi_la-pyfwsi_volume.lo -MD -MP -MF $(DEPDIR)/pyfwsi_la-pyfwsi_volume.Tpo -c -o pyfwsi_la-pyfwsi_volume.lo `test -f 'pyfwsi_volume.c' || echo '$(srcdir)/'`pyfwsi_volume.c
 @am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pyfwsi_la-pyfwsi_volume.Tpo $(DEPDIR)/pyfwsi_la-pyfwsi_volume.Plo
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pyfwsi_volume.c' object='pyfwsi_la-pyfwsi_volume.lo' libtool=yes @AMDEPBACKSLASH@
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
 @am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pyfwsi_la-pyfwsi_volume.lo `test -f 'pyfwsi_volume.c' || echo '$(srcdir)/'`pyfwsi_volume.c
 
@@ -1024,14 +1037,15 @@
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_guid.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_integer.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_item.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_item_list.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_items.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_network_location.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_string.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_volume.Plo
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
 
 mostlyclean: mostlyclean-am
 
 mostlyclean-am: mostlyclean-compile mostlyclean-generic \
```

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_file_entry_extension.c` & `libfwsi-20230710/pyfwsi/pyfwsi_file_entry_extension.c`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 #include "pyfwsi_error.h"
 #include "pyfwsi_extension_block.h"
 #include "pyfwsi_file_entry_extension.h"
 #include "pyfwsi_integer.h"
 #include "pyfwsi_libcerror.h"
 #include "pyfwsi_libfwsi.h"
 #include "pyfwsi_python.h"
+#include "pyfwsi_string.h"
 #include "pyfwsi_unused.h"
 
 PyMethodDef pyfwsi_file_entry_extension_object_methods[] = {
 
 	{ "get_creation_time",
 	  (PyCFunction) pyfwsi_file_entry_extension_get_creation_time,
 	  METH_NOARGS,
@@ -436,17 +437,17 @@
 PyObject *pyfwsi_file_entry_extension_get_long_name(
            pyfwsi_extension_block_t *pyfwsi_extension_block,
            PyObject *arguments PYFWSI_ATTRIBUTE_UNUSED )
 {
 	libcerror_error_t *error = NULL;
 	PyObject *string_object  = NULL;
 	const char *errors       = NULL;
-	uint8_t *long_name       = NULL;
+	uint8_t *utf8_string     = NULL;
 	static char *function    = "pyfwsi_file_entry_extension_get_long_name";
-	size_t long_name_size    = 0;
+	size_t utf8_string_size  = 0;
 	int result               = 0;
 
 	PYFWSI_UNREFERENCED_PARAMETER( arguments )
 
 	if( pyfwsi_extension_block == NULL )
 	{
 		PyErr_Format(
@@ -456,94 +457,108 @@
 
 		return( NULL );
 	}
 	Py_BEGIN_ALLOW_THREADS
 
 	result = libfwsi_file_entry_extension_get_utf8_long_name_size(
 	          pyfwsi_extension_block->extension_block,
-	          &long_name_size,
+	          &utf8_string_size,
 	          &error );
 
 	Py_END_ALLOW_THREADS
 
 	if( result == -1 )
 	{
 		pyfwsi_error_raise(
 		 error,
 		 PyExc_IOError,
-		 "%s: unable to retrieve long name size.",
+		 "%s: unable to determine size of long name as UTF-8 string.",
 		 function );
 
 		libcerror_error_free(
 		 &error );
 
 		goto on_error;
 	}
 	else if( ( result == 0 )
-	      || ( long_name_size == 0 ) )
+	      || ( utf8_string_size == 0 ) )
 	{
 		Py_IncRef(
 		 Py_None );
 
 		return( Py_None );
 	}
-	long_name = (uint8_t *) PyMem_Malloc(
-	                         sizeof( uint8_t ) * long_name_size );
+	utf8_string = (uint8_t *) PyMem_Malloc(
+	                           sizeof( uint8_t ) * utf8_string_size );
 
-	if( long_name == NULL )
+	if( utf8_string == NULL )
 	{
 		PyErr_Format(
-		 PyExc_IOError,
+		 PyExc_MemoryError,
 		 "%s: unable to create long name.",
 		 function );
 
 		goto on_error;
 	}
 	Py_BEGIN_ALLOW_THREADS
 
 	result = libfwsi_file_entry_extension_get_utf8_long_name(
 		  pyfwsi_extension_block->extension_block,
-		  long_name,
-		  long_name_size,
+		  utf8_string,
+		  utf8_string_size,
 		  &error );
 
 	Py_END_ALLOW_THREADS
 
 	if( result != 1 )
 	{
 		pyfwsi_error_raise(
 		 error,
 		 PyExc_IOError,
-		 "%s: unable to retrieve long name.",
+		 "%s: unable to retrieve long name as UTF-8 string.",
 		 function );
 
 		libcerror_error_free(
 		 &error );
 
 		goto on_error;
 	}
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
+	string_object = pyfwsi_string_new_from_utf8_rfc2279(
+			 (uint8_t *) utf8_string,
+			 utf8_string_size );
+#else
 	/* Pass the string length to PyUnicode_DecodeUTF8
 	 * otherwise it makes the end of string character is part
 	 * of the string
 	 */
 	string_object = PyUnicode_DecodeUTF8(
-			 (char *) long_name,
-			 (Py_ssize_t) long_name_size - 1,
-			 errors );
+	                 utf8_string,
+	                 (Py_ssize_t) utf8_string_size - 1,
+	                 NULL );
+#endif
+	if( string_object == NULL )
+	{
+		PyErr_Format(
+		 PyExc_IOError,
+		 "%s: unable to convert UTF-8 string into Unicode object.",
+		 function );
 
+		goto on_error;
+	}
 	PyMem_Free(
-	 long_name );
+	 utf8_string );
 
 	return( string_object );
 
 on_error:
-	if( long_name != NULL )
+	if( utf8_string != NULL )
 	{
 		PyMem_Free(
-		 long_name );
+		 utf8_string );
 	}
 	return( NULL );
 }
 
 /* Retrieves the localized name
  * Returns a Python object if successful or NULL on error
  */
@@ -602,15 +617,15 @@
 	}
 	localized_name = (uint8_t *) PyMem_Malloc(
 	                              sizeof( uint8_t ) * localized_name_size );
 
 	if( localized_name == NULL )
 	{
 		PyErr_Format(
-		 PyExc_IOError,
+		 PyExc_MemoryError,
 		 "%s: unable to create localized name.",
 		 function );
 
 		goto on_error;
 	}
 	Py_BEGIN_ALLOW_THREADS
```

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_extension_blocks.c` & `libfwsi-20230710/pyfwsi/pyfwsi_extension_blocks.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_file_entry_extension.h` & `libfwsi-20230710/pyfwsi/pyfwsi_file_entry_extension.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_libfwsi.h` & `libfwsi-20230710/pyfwsi/pyfwsi_libfwsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_item.h` & `libfwsi-20230710/pyfwsi/pyfwsi_item.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_datetime.c` & `libfwsi-20230710/pyfwsi/pyfwsi_datetime.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_datetime.h` & `libfwsi-20230710/pyfwsi/pyfwsi_datetime.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_libfguid.h` & `libfwsi-20230710/pyfwsi/pyfwsi_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_guid.c` & `libfwsi-20230710/pyfwsi/pyfwsi_guid.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_root_folder.c` & `libfwsi-20230710/pyfwsi/pyfwsi_root_folder.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi.h` & `libfwsi-20230710/pyfwsi/pyfwsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_network_location.c` & `libfwsi-20230710/pyfwsi/pyfwsi_network_location.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_item_list.h` & `libfwsi-20230710/pyfwsi/pyfwsi_item_list.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_extension_block.c` & `libfwsi-20230710/pyfwsi/pyfwsi_extension_block.c`

 * *Files 0% similar despite different names*

```diff
@@ -493,15 +493,15 @@
 	}
 	data = (uint8_t *) PyMem_Malloc(
 	                    sizeof( uint8_t ) * data_size );
 
 	if( data == NULL )
 	{
 		PyErr_Format(
-		 PyExc_IOError,
+		 PyExc_MemoryError,
 		 "%s: unable to create data.",
 		 function );
 
 		goto on_error;
 	}
 	Py_BEGIN_ALLOW_THREADS
```

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_network_location.h` & `libfwsi-20230710/pyfwsi/pyfwsi_network_location.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_libcerror.h` & `libfwsi-20230710/pyfwsi/pyfwsi_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_file_entry.h` & `libfwsi-20230710/pyfwsi/pyfwsi_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_error.h` & `libfwsi-20230710/pyfwsi/pyfwsi_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi/pyfwsi_volume.h` & `libfwsi-20230710/pyfwsi/pyfwsi_volume.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libclocale/libclocale_wide_string.h` & `libfwsi-20230710/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libclocale/libclocale_support.c` & `libfwsi-20230710/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libclocale/libclocale_locale.h` & `libfwsi-20230710/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libclocale/Makefile.am` & `libfwsi-20230710/libclocale/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libclocale/libclocale_locale.c` & `libfwsi-20230710/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libclocale/libclocale_extern.h` & `libfwsi-20230710/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libclocale/libclocale_unused.h` & `libfwsi-20230710/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libclocale/libclocale_support.h` & `libfwsi-20230710/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libclocale/libclocale_definitions.h` & `libfwsi-20230710/libclocale/libclocale_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libclocale/libclocale_codepage.h` & `libfwsi-20230710/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libclocale/libclocale_codepage.c` & `libfwsi-20230710/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libclocale/Makefile.in` & `libfwsi-20230710/libclocale/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libclocale/libclocale_wide_string.c` & `libfwsi-20230710/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libclocale/libclocale_libcerror.h` & `libfwsi-20230710/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/missing` & `libfwsi-20230710/missing`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi-python2/Makefile.am` & `libfwsi-20230710/pyfwsi-python3/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Note that we cannot use: AUTOMAKE_OPTIONS = subdir-objects
 # subdir-objects will compile the source files to a single version of Python.
 # Since subdir-objects is being deprecated we copy the source files instead.
-am__installdirs = "$(DESTDIR)$(pyexecdir2)"
-pyexecdir = $(pyexecdir2)
+am__installdirs = "$(DESTDIR)$(pyexecdir3)"
+pyexecdir = $(pyexecdir3)
 
-if HAVE_PYTHON2
+if HAVE_PYTHON3
 AM_CFLAGS = \
 	-I$(top_srcdir)/include \
 	-I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
 	@LIBFWSI_DLL_IMPORT@
 
-am_pyfwsi_la_rpath = -rpath $(pyexecdir2)
+am_pyfwsi_la_rpath = -rpath $(pyexecdir3)
 
 BUILT_SOURCES = \
 	pyfwsi.c pyfwsi.h \
 	pyfwsi_codepage.c pyfwsi_codepage.h \
 	pyfwsi_datetime.c pyfwsi_datetime.h \
 	pyfwsi_error.c pyfwsi_error.h \
 	pyfwsi_extension_block.c pyfwsi_extension_block.h \
@@ -31,17 +31,19 @@
 	pyfwsi_item.c pyfwsi_item.h \
 	pyfwsi_item_list.c pyfwsi_item_list.h \
 	pyfwsi_items.c pyfwsi_items.h \
 	pyfwsi_libcerror.h \
 	pyfwsi_libclocale.h \
 	pyfwsi_libfguid.h \
 	pyfwsi_libfwsi.h \
+	pyfwsi_libuna.h \
 	pyfwsi_network_location.c pyfwsi_network_location.h \
 	pyfwsi_python.h \
 	pyfwsi_root_folder.c pyfwsi_root_folder.h \
+	pyfwsi_string.c pyfwsi_string.h \
 	pyfwsi_unused.h \
 	pyfwsi_volume.c pyfwsi_volume.h
 
 pyexec_LTLIBRARIES = pyfwsi.la
 
 nodist_pyfwsi_la_SOURCES = $(BUILT_SOURCES)
 
@@ -49,16 +51,16 @@
 	@LIBCERROR_LIBADD@ \
 	../libfwsi/libfwsi.la \
 	@LIBCDATA_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBUNA_LIBADD@ \
 	@LIBFGUID_LIBADD@
 
-pyfwsi_la_CPPFLAGS = $(PYTHON2_CPPFLAGS)
-pyfwsi_la_LDFLAGS  = -module -avoid-version $(PYTHON2_LDFLAGS)
+pyfwsi_la_CPPFLAGS = $(PYTHON3_CPPFLAGS)
+pyfwsi_la_LDFLAGS  = -module -avoid-version $(PYTHON3_LDFLAGS)
 
 $(BUILT_SOURCES):
 	/bin/cp -f $(top_srcdir)/pyfwsi/$@ $@
 
 endif
 
 MAINTAINERCLEANFILES = \
```

### Comparing `libfwsi-20230114/pyfwsi-python2/Makefile.in` & `libfwsi-20230710/pyfwsi-python2/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
 @HAVE_PYTHON2_TRUE@	pyfwsi_la-pyfwsi_guid.lo \
 @HAVE_PYTHON2_TRUE@	pyfwsi_la-pyfwsi_integer.lo \
 @HAVE_PYTHON2_TRUE@	pyfwsi_la-pyfwsi_item.lo \
 @HAVE_PYTHON2_TRUE@	pyfwsi_la-pyfwsi_item_list.lo \
 @HAVE_PYTHON2_TRUE@	pyfwsi_la-pyfwsi_items.lo \
 @HAVE_PYTHON2_TRUE@	pyfwsi_la-pyfwsi_network_location.lo \
 @HAVE_PYTHON2_TRUE@	pyfwsi_la-pyfwsi_root_folder.lo \
+@HAVE_PYTHON2_TRUE@	pyfwsi_la-pyfwsi_string.lo \
 @HAVE_PYTHON2_TRUE@	pyfwsi_la-pyfwsi_volume.lo
 @HAVE_PYTHON2_TRUE@nodist_pyfwsi_la_OBJECTS = $(am__objects_1)
 pyfwsi_la_OBJECTS = $(nodist_pyfwsi_la_OBJECTS)
 AM_V_lt = $(am__v_lt_@AM_V@)
 am__v_lt_ = $(am__v_lt_@AM_DEFAULT_V@)
 am__v_lt_0 = --silent
 am__v_lt_1 = 
@@ -194,14 +195,15 @@
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_guid.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_integer.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_item.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_item_list.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_items.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_network_location.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Plo \
+	./$(DEPDIR)/pyfwsi_la-pyfwsi_string.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_volume.Plo
 am__mv = mv -f
 COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
 	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
 LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) \
 	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
@@ -569,17 +571,19 @@
 @HAVE_PYTHON2_TRUE@	pyfwsi_item.c pyfwsi_item.h \
 @HAVE_PYTHON2_TRUE@	pyfwsi_item_list.c pyfwsi_item_list.h \
 @HAVE_PYTHON2_TRUE@	pyfwsi_items.c pyfwsi_items.h \
 @HAVE_PYTHON2_TRUE@	pyfwsi_libcerror.h \
 @HAVE_PYTHON2_TRUE@	pyfwsi_libclocale.h \
 @HAVE_PYTHON2_TRUE@	pyfwsi_libfguid.h \
 @HAVE_PYTHON2_TRUE@	pyfwsi_libfwsi.h \
+@HAVE_PYTHON2_TRUE@	pyfwsi_libuna.h \
 @HAVE_PYTHON2_TRUE@	pyfwsi_network_location.c pyfwsi_network_location.h \
 @HAVE_PYTHON2_TRUE@	pyfwsi_python.h \
 @HAVE_PYTHON2_TRUE@	pyfwsi_root_folder.c pyfwsi_root_folder.h \
+@HAVE_PYTHON2_TRUE@	pyfwsi_string.c pyfwsi_string.h \
 @HAVE_PYTHON2_TRUE@	pyfwsi_unused.h \
 @HAVE_PYTHON2_TRUE@	pyfwsi_volume.c pyfwsi_volume.h
 
 @HAVE_PYTHON2_TRUE@pyexec_LTLIBRARIES = pyfwsi.la
 @HAVE_PYTHON2_TRUE@nodist_pyfwsi_la_SOURCES = $(BUILT_SOURCES)
 @HAVE_PYTHON2_TRUE@pyfwsi_la_LIBADD = \
 @HAVE_PYTHON2_TRUE@	@LIBCERROR_LIBADD@ \
@@ -684,14 +688,15 @@
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_guid.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_integer.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_item.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_item_list.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_items.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_network_location.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Plo@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_string.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_volume.Plo@am__quote@ # am--include-marker
 
 $(am__depfiles_remade):
 	@$(MKDIR_P) $(@D)
 	@echo '# dummy' >$@-t && $(am__mv) $@-t $@
 
 am--depfiles: $(am__depfiles_remade)
@@ -818,14 +823,21 @@
 pyfwsi_la-pyfwsi_root_folder.lo: pyfwsi_root_folder.c
 @am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pyfwsi_la-pyfwsi_root_folder.lo -MD -MP -MF $(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Tpo -c -o pyfwsi_la-pyfwsi_root_folder.lo `test -f 'pyfwsi_root_folder.c' || echo '$(srcdir)/'`pyfwsi_root_folder.c
 @am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Tpo $(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Plo
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pyfwsi_root_folder.c' object='pyfwsi_la-pyfwsi_root_folder.lo' libtool=yes @AMDEPBACKSLASH@
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
 @am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pyfwsi_la-pyfwsi_root_folder.lo `test -f 'pyfwsi_root_folder.c' || echo '$(srcdir)/'`pyfwsi_root_folder.c
 
+pyfwsi_la-pyfwsi_string.lo: pyfwsi_string.c
+@am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pyfwsi_la-pyfwsi_string.lo -MD -MP -MF $(DEPDIR)/pyfwsi_la-pyfwsi_string.Tpo -c -o pyfwsi_la-pyfwsi_string.lo `test -f 'pyfwsi_string.c' || echo '$(srcdir)/'`pyfwsi_string.c
+@am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pyfwsi_la-pyfwsi_string.Tpo $(DEPDIR)/pyfwsi_la-pyfwsi_string.Plo
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pyfwsi_string.c' object='pyfwsi_la-pyfwsi_string.lo' libtool=yes @AMDEPBACKSLASH@
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
+@am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pyfwsi_la-pyfwsi_string.lo `test -f 'pyfwsi_string.c' || echo '$(srcdir)/'`pyfwsi_string.c
+
 pyfwsi_la-pyfwsi_volume.lo: pyfwsi_volume.c
 @am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pyfwsi_la-pyfwsi_volume.lo -MD -MP -MF $(DEPDIR)/pyfwsi_la-pyfwsi_volume.Tpo -c -o pyfwsi_la-pyfwsi_volume.lo `test -f 'pyfwsi_volume.c' || echo '$(srcdir)/'`pyfwsi_volume.c
 @am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pyfwsi_la-pyfwsi_volume.Tpo $(DEPDIR)/pyfwsi_la-pyfwsi_volume.Plo
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pyfwsi_volume.c' object='pyfwsi_la-pyfwsi_volume.lo' libtool=yes @AMDEPBACKSLASH@
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
 @am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pyfwsi_la-pyfwsi_volume.lo `test -f 'pyfwsi_volume.c' || echo '$(srcdir)/'`pyfwsi_volume.c
 
@@ -1021,14 +1033,15 @@
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_guid.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_integer.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_item.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_item_list.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_items.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_network_location.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_string.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_volume.Plo
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
 
 mostlyclean: mostlyclean-am
 
 mostlyclean-am: mostlyclean-compile mostlyclean-generic \
```

### Comparing `libfwsi-20230114/Makefile.am` & `libfwsi-20230710/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/aclocal.m4` & `libfwsi-20230710/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/COPYING` & `libfwsi-20230710/COPYING`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi.spec.in` & `libfwsi-20230710/libfwsi.spec.in`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Name: libfwsi
 Version: @VERSION@
 Release: 1
 Summary: Library to access the Windows Shell Item format
 Group: System Environment/Libraries
-License: LGPLv3+
+License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfwsi
-BuildRoot: %{_tmppath}/%{name}-%{version}-%{release}-root-%(%{__id_u} -n)
 @libfwsi_spec_requires@ @ax_libcdata_spec_requires@ @ax_libcerror_spec_requires@ @ax_libclocale_spec_requires@ @ax_libcnotify_spec_requires@ @ax_libcthreads_spec_requires@ @ax_libfdatetime_spec_requires@ @ax_libfguid_spec_requires@ @ax_libfole_spec_requires@ @ax_libfwps_spec_requires@ @ax_libuna_spec_requires@
 BuildRequires: gcc @ax_libcdata_spec_build_requires@ @ax_libcerror_spec_build_requires@ @ax_libclocale_spec_build_requires@ @ax_libcnotify_spec_build_requires@ @ax_libcthreads_spec_build_requires@ @ax_libfdatetime_spec_build_requires@ @ax_libfguid_spec_build_requires@ @ax_libfole_spec_build_requires@ @ax_libfwps_spec_build_requires@ @ax_libuna_spec_build_requires@
 
 %description -n libfwsi
 Library to access the Windows Shell Item format
 
 %package -n libfwsi-static
@@ -53,36 +52,32 @@
 rm -rf %{buildroot}
 
 %post -p /sbin/ldconfig
 
 %postun -p /sbin/ldconfig
 
 %files -n libfwsi
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
-%attr(755,root,root) %{_libdir}/*.so.*
+%{_libdir}/*.so.*
 
 %files -n libfwsi-static
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
-%attr(755,root,root) %{_libdir}/*.a
+%{_libdir}/*.a
 
 %files -n libfwsi-devel
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/*.so
 %{_libdir}/pkgconfig/libfwsi.pc
 %{_includedir}/*
 %{_mandir}/man3/*
 
 %files -n libfwsi-python3
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %changelog
 * @SPEC_DATE@ Joachim Metz <joachim.metz@gmail.com> @VERSION@-1
```

### Comparing `libfwsi-20230114/include/libfwsi.h` & `libfwsi-20230710/include/libfwsi.h`

 * *Files 6% similar despite different names*

```diff
@@ -348,42 +348,50 @@
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_get_file_attribute_flags(
      libfwsi_item_t *file_entry,
      uint32_t *file_attribute_flags,
      libfwsi_error_t **error );
 
 /* Retrieves the size of the UTF-8 formatted name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_get_utf8_name_size(
      libfwsi_item_t *file_entry,
      size_t *utf8_string_size,
      libfwsi_error_t **error );
 
 /* Retrieves the UTF-8 formatted name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_get_utf8_name(
      libfwsi_item_t *file_entry,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      libfwsi_error_t **error );
 
 /* Retrieves the size of the UTF-16 formatted name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_get_utf16_name_size(
      libfwsi_item_t *file_entry,
      size_t *utf16_string_size,
      libfwsi_error_t **error );
 
 /* Retrieves the UTF-16 formatted name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_get_utf16_name(
      libfwsi_item_t *file_entry,
      uint16_t *utf16_string,
      size_t utf16_string_size,
@@ -567,42 +575,50 @@
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_extension_get_file_reference(
      libfwsi_extension_block_t *file_entry_extension,
      uint64_t *file_reference,
      libfwsi_error_t **error );
 
 /* Retrieves the size of the UTF-8 formatted long name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_extension_get_utf8_long_name_size(
      libfwsi_extension_block_t *file_entry_extension,
      size_t *utf8_string_size,
      libfwsi_error_t **error );
 
 /* Retrieves the UTF-8 formatted long name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_extension_get_utf8_long_name(
      libfwsi_extension_block_t *file_entry_extension,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      libfwsi_error_t **error );
 
 /* Retrieves the size of the UTF-16 formatted long name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_extension_get_utf16_long_name_size(
      libfwsi_extension_block_t *file_entry_extension,
      size_t *utf16_string_size,
      libfwsi_error_t **error );
 
 /* Retrieves the UTF-16 formatted long name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_extension_get_utf16_long_name(
      libfwsi_extension_block_t *file_entry_extension,
      uint16_t *utf16_string,
      size_t utf16_string_size,
```

### Comparing `libfwsi-20230114/include/libfwsi/definitions.h.in` & `libfwsi-20230710/include/libfwsi/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/include/libfwsi/extern.h` & `libfwsi-20230710/include/libfwsi/extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/include/libfwsi/types.h` & `libfwsi-20230710/include/libfwsi/types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/include/libfwsi/features.h.in` & `libfwsi-20230710/include/libfwsi/features.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/include/libfwsi/types.h.in` & `libfwsi-20230710/include/libfwsi/types.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/include/libfwsi/features.h` & `libfwsi-20230710/include/libfwsi/features.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/include/libfwsi/definitions.h` & `libfwsi-20230710/include/libfwsi/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBFWSI_DEFINITIONS_H )
 #define _LIBFWSI_DEFINITIONS_H
 
 #include <libfwsi/types.h>
 
-#define LIBFWSI_VERSION					20230114
+#define LIBFWSI_VERSION					20230710
 
 /* The version string
  */
-#define LIBFWSI_VERSION_STRING				"20230114"
+#define LIBFWSI_VERSION_STRING				"20230710"
 
 /* The byte order definitions
  */
 enum LIBFWSI_ENDIAN
 {
 	LIBFWSI_ENDIAN_BIG				= (int) 'b',
 	LIBFWSI_ENDIAN_LITTLE				= (int) 'l'
```

### Comparing `libfwsi-20230114/include/libfwsi/codepage.h` & `libfwsi-20230710/include/libfwsi/codepage.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/include/libfwsi/error.h` & `libfwsi-20230710/include/libfwsi/error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/include/Makefile.in` & `libfwsi-20230710/include/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/include/libfwsi.h.in` & `libfwsi-20230710/include/libfwsi.h.in`

 * *Files 6% similar despite different names*

```diff
@@ -348,42 +348,50 @@
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_get_file_attribute_flags(
      libfwsi_item_t *file_entry,
      uint32_t *file_attribute_flags,
      libfwsi_error_t **error );
 
 /* Retrieves the size of the UTF-8 formatted name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_get_utf8_name_size(
      libfwsi_item_t *file_entry,
      size_t *utf8_string_size,
      libfwsi_error_t **error );
 
 /* Retrieves the UTF-8 formatted name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_get_utf8_name(
      libfwsi_item_t *file_entry,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      libfwsi_error_t **error );
 
 /* Retrieves the size of the UTF-16 formatted name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_get_utf16_name_size(
      libfwsi_item_t *file_entry,
      size_t *utf16_string_size,
      libfwsi_error_t **error );
 
 /* Retrieves the UTF-16 formatted name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_get_utf16_name(
      libfwsi_item_t *file_entry,
      uint16_t *utf16_string,
      size_t utf16_string_size,
@@ -567,42 +575,50 @@
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_extension_get_file_reference(
      libfwsi_extension_block_t *file_entry_extension,
      uint64_t *file_reference,
      libfwsi_error_t **error );
 
 /* Retrieves the size of the UTF-8 formatted long name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_extension_get_utf8_long_name_size(
      libfwsi_extension_block_t *file_entry_extension,
      size_t *utf8_string_size,
      libfwsi_error_t **error );
 
 /* Retrieves the UTF-8 formatted long name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_extension_get_utf8_long_name(
      libfwsi_extension_block_t *file_entry_extension,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      libfwsi_error_t **error );
 
 /* Retrieves the size of the UTF-16 formatted long name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_extension_get_utf16_long_name_size(
      libfwsi_extension_block_t *file_entry_extension,
      size_t *utf16_string_size,
      libfwsi_error_t **error );
 
 /* Retrieves the UTF-16 formatted long name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 LIBFWSI_EXTERN \
 int libfwsi_file_entry_extension_get_utf16_long_name(
      libfwsi_extension_block_t *file_entry_extension,
      uint16_t *utf16_string,
      size_t utf16_string_size,
```

### Comparing `libfwsi-20230114/install-sh` & `libfwsi-20230710/install-sh`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/INSTALL` & `libfwsi-20230710/INSTALL`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/dpkg/copyright` & `libfwsi-20230710/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/dpkg/rules` & `libfwsi-20230710/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/dpkg/control` & `libfwsi-20230710/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_support.c` & `libfwsi-20230710/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_systemtime.h` & `libfwsi-20230710/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_error.h` & `libfwsi-20230710/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/Makefile.am` & `libfwsi-20230710/libfdatetime/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_unused.h` & `libfwsi-20230710/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_error.c` & `libfwsi-20230710/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_posix_time.c` & `libfwsi-20230710/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_fat_date_time.h` & `libfwsi-20230710/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_types.h` & `libfwsi-20230710/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_floatingtime.c` & `libfwsi-20230710/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_hfs_time.h` & `libfwsi-20230710/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_support.h` & `libfwsi-20230710/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_extern.h` & `libfwsi-20230710/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_filetime.h` & `libfwsi-20230710/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_date_time_values.c` & `libfwsi-20230710/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_floatingtime.h` & `libfwsi-20230710/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_libcerror.h` & `libfwsi-20230710/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/Makefile.in` & `libfwsi-20230710/libfdatetime/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_nsf_timedate.c` & `libfwsi-20230710/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_date_time_values.h` & `libfwsi-20230710/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_hfs_time.c` & `libfwsi-20230710/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_posix_time.h` & `libfwsi-20230710/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_fat_date_time.c` & `libfwsi-20230710/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_nsf_timedate.h` & `libfwsi-20230710/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_definitions.h` & `libfwsi-20230710/libfdatetime/libfdatetime_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_systemtime.c` & `libfwsi-20230710/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfdatetime/libfdatetime_filetime.c` & `libfwsi-20230710/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_thread_pool.h` & `libfwsi-20230710/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_thread_pool.c` & `libfwsi-20230710/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_repeating_thread.c` & `libfwsi-20230710/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_error.c` & `libfwsi-20230710/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/Makefile.am` & `libfwsi-20230710/libcthreads/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_unused.h` & `libfwsi-20230710/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_condition.h` & `libfwsi-20230710/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_definitions.h` & `libfwsi-20230710/libcthreads/libcthreads_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_thread.h` & `libfwsi-20230710/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_repeating_thread.h` & `libfwsi-20230710/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_read_write_lock.c` & `libfwsi-20230710/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_mutex.h` & `libfwsi-20230710/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_support.h` & `libfwsi-20230710/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_thread.c` & `libfwsi-20230710/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_mutex.c` & `libfwsi-20230710/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_types.h` & `libfwsi-20230710/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_lock.h` & `libfwsi-20230710/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_extern.h` & `libfwsi-20230710/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_error.h` & `libfwsi-20230710/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_queue.c` & `libfwsi-20230710/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_condition.c` & `libfwsi-20230710/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/Makefile.in` & `libfwsi-20230710/libcthreads/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_thread_attributes.c` & `libfwsi-20230710/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_libcerror.h` & `libfwsi-20230710/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_lock.c` & `libfwsi-20230710/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_support.c` & `libfwsi-20230710/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_read_write_lock.h` & `libfwsi-20230710/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_thread_attributes.h` & `libfwsi-20230710/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcthreads/libcthreads_queue.h` & `libfwsi-20230710/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/config.sub` & `libfwsi-20230710/config.sub`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/pyfwsi-python3/Makefile.am` & `libfwsi-20230710/pyfwsi-python2/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Note that we cannot use: AUTOMAKE_OPTIONS = subdir-objects
 # subdir-objects will compile the source files to a single version of Python.
 # Since subdir-objects is being deprecated we copy the source files instead.
-am__installdirs = "$(DESTDIR)$(pyexecdir3)"
-pyexecdir = $(pyexecdir3)
+am__installdirs = "$(DESTDIR)$(pyexecdir2)"
+pyexecdir = $(pyexecdir2)
 
-if HAVE_PYTHON3
+if HAVE_PYTHON2
 AM_CFLAGS = \
 	-I$(top_srcdir)/include \
 	-I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
 	@LIBFWSI_DLL_IMPORT@
 
-am_pyfwsi_la_rpath = -rpath $(pyexecdir3)
+am_pyfwsi_la_rpath = -rpath $(pyexecdir2)
 
 BUILT_SOURCES = \
 	pyfwsi.c pyfwsi.h \
 	pyfwsi_codepage.c pyfwsi_codepage.h \
 	pyfwsi_datetime.c pyfwsi_datetime.h \
 	pyfwsi_error.c pyfwsi_error.h \
 	pyfwsi_extension_block.c pyfwsi_extension_block.h \
@@ -31,17 +31,19 @@
 	pyfwsi_item.c pyfwsi_item.h \
 	pyfwsi_item_list.c pyfwsi_item_list.h \
 	pyfwsi_items.c pyfwsi_items.h \
 	pyfwsi_libcerror.h \
 	pyfwsi_libclocale.h \
 	pyfwsi_libfguid.h \
 	pyfwsi_libfwsi.h \
+	pyfwsi_libuna.h \
 	pyfwsi_network_location.c pyfwsi_network_location.h \
 	pyfwsi_python.h \
 	pyfwsi_root_folder.c pyfwsi_root_folder.h \
+	pyfwsi_string.c pyfwsi_string.h \
 	pyfwsi_unused.h \
 	pyfwsi_volume.c pyfwsi_volume.h
 
 pyexec_LTLIBRARIES = pyfwsi.la
 
 nodist_pyfwsi_la_SOURCES = $(BUILT_SOURCES)
 
@@ -49,16 +51,16 @@
 	@LIBCERROR_LIBADD@ \
 	../libfwsi/libfwsi.la \
 	@LIBCDATA_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBUNA_LIBADD@ \
 	@LIBFGUID_LIBADD@
 
-pyfwsi_la_CPPFLAGS = $(PYTHON3_CPPFLAGS)
-pyfwsi_la_LDFLAGS  = -module -avoid-version $(PYTHON3_LDFLAGS)
+pyfwsi_la_CPPFLAGS = $(PYTHON2_CPPFLAGS)
+pyfwsi_la_LDFLAGS  = -module -avoid-version $(PYTHON2_LDFLAGS)
 
 $(BUILT_SOURCES):
 	/bin/cp -f $(top_srcdir)/pyfwsi/$@ $@
 
 endif
 
 MAINTAINERCLEANFILES = \
```

### Comparing `libfwsi-20230114/pyfwsi-python3/Makefile.in` & `libfwsi-20230710/pyfwsi-python3/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
 @HAVE_PYTHON3_TRUE@	pyfwsi_la-pyfwsi_guid.lo \
 @HAVE_PYTHON3_TRUE@	pyfwsi_la-pyfwsi_integer.lo \
 @HAVE_PYTHON3_TRUE@	pyfwsi_la-pyfwsi_item.lo \
 @HAVE_PYTHON3_TRUE@	pyfwsi_la-pyfwsi_item_list.lo \
 @HAVE_PYTHON3_TRUE@	pyfwsi_la-pyfwsi_items.lo \
 @HAVE_PYTHON3_TRUE@	pyfwsi_la-pyfwsi_network_location.lo \
 @HAVE_PYTHON3_TRUE@	pyfwsi_la-pyfwsi_root_folder.lo \
+@HAVE_PYTHON3_TRUE@	pyfwsi_la-pyfwsi_string.lo \
 @HAVE_PYTHON3_TRUE@	pyfwsi_la-pyfwsi_volume.lo
 @HAVE_PYTHON3_TRUE@nodist_pyfwsi_la_OBJECTS = $(am__objects_1)
 pyfwsi_la_OBJECTS = $(nodist_pyfwsi_la_OBJECTS)
 AM_V_lt = $(am__v_lt_@AM_V@)
 am__v_lt_ = $(am__v_lt_@AM_DEFAULT_V@)
 am__v_lt_0 = --silent
 am__v_lt_1 = 
@@ -194,14 +195,15 @@
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_guid.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_integer.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_item.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_item_list.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_items.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_network_location.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Plo \
+	./$(DEPDIR)/pyfwsi_la-pyfwsi_string.Plo \
 	./$(DEPDIR)/pyfwsi_la-pyfwsi_volume.Plo
 am__mv = mv -f
 COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
 	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
 LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) \
 	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
@@ -569,17 +571,19 @@
 @HAVE_PYTHON3_TRUE@	pyfwsi_item.c pyfwsi_item.h \
 @HAVE_PYTHON3_TRUE@	pyfwsi_item_list.c pyfwsi_item_list.h \
 @HAVE_PYTHON3_TRUE@	pyfwsi_items.c pyfwsi_items.h \
 @HAVE_PYTHON3_TRUE@	pyfwsi_libcerror.h \
 @HAVE_PYTHON3_TRUE@	pyfwsi_libclocale.h \
 @HAVE_PYTHON3_TRUE@	pyfwsi_libfguid.h \
 @HAVE_PYTHON3_TRUE@	pyfwsi_libfwsi.h \
+@HAVE_PYTHON3_TRUE@	pyfwsi_libuna.h \
 @HAVE_PYTHON3_TRUE@	pyfwsi_network_location.c pyfwsi_network_location.h \
 @HAVE_PYTHON3_TRUE@	pyfwsi_python.h \
 @HAVE_PYTHON3_TRUE@	pyfwsi_root_folder.c pyfwsi_root_folder.h \
+@HAVE_PYTHON3_TRUE@	pyfwsi_string.c pyfwsi_string.h \
 @HAVE_PYTHON3_TRUE@	pyfwsi_unused.h \
 @HAVE_PYTHON3_TRUE@	pyfwsi_volume.c pyfwsi_volume.h
 
 @HAVE_PYTHON3_TRUE@pyexec_LTLIBRARIES = pyfwsi.la
 @HAVE_PYTHON3_TRUE@nodist_pyfwsi_la_SOURCES = $(BUILT_SOURCES)
 @HAVE_PYTHON3_TRUE@pyfwsi_la_LIBADD = \
 @HAVE_PYTHON3_TRUE@	@LIBCERROR_LIBADD@ \
@@ -684,14 +688,15 @@
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_guid.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_integer.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_item.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_item_list.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_items.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_network_location.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Plo@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_string.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwsi_la-pyfwsi_volume.Plo@am__quote@ # am--include-marker
 
 $(am__depfiles_remade):
 	@$(MKDIR_P) $(@D)
 	@echo '# dummy' >$@-t && $(am__mv) $@-t $@
 
 am--depfiles: $(am__depfiles_remade)
@@ -818,14 +823,21 @@
 pyfwsi_la-pyfwsi_root_folder.lo: pyfwsi_root_folder.c
 @am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pyfwsi_la-pyfwsi_root_folder.lo -MD -MP -MF $(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Tpo -c -o pyfwsi_la-pyfwsi_root_folder.lo `test -f 'pyfwsi_root_folder.c' || echo '$(srcdir)/'`pyfwsi_root_folder.c
 @am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Tpo $(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Plo
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pyfwsi_root_folder.c' object='pyfwsi_la-pyfwsi_root_folder.lo' libtool=yes @AMDEPBACKSLASH@
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
 @am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pyfwsi_la-pyfwsi_root_folder.lo `test -f 'pyfwsi_root_folder.c' || echo '$(srcdir)/'`pyfwsi_root_folder.c
 
+pyfwsi_la-pyfwsi_string.lo: pyfwsi_string.c
+@am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pyfwsi_la-pyfwsi_string.lo -MD -MP -MF $(DEPDIR)/pyfwsi_la-pyfwsi_string.Tpo -c -o pyfwsi_la-pyfwsi_string.lo `test -f 'pyfwsi_string.c' || echo '$(srcdir)/'`pyfwsi_string.c
+@am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pyfwsi_la-pyfwsi_string.Tpo $(DEPDIR)/pyfwsi_la-pyfwsi_string.Plo
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pyfwsi_string.c' object='pyfwsi_la-pyfwsi_string.lo' libtool=yes @AMDEPBACKSLASH@
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
+@am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pyfwsi_la-pyfwsi_string.lo `test -f 'pyfwsi_string.c' || echo '$(srcdir)/'`pyfwsi_string.c
+
 pyfwsi_la-pyfwsi_volume.lo: pyfwsi_volume.c
 @am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pyfwsi_la-pyfwsi_volume.lo -MD -MP -MF $(DEPDIR)/pyfwsi_la-pyfwsi_volume.Tpo -c -o pyfwsi_la-pyfwsi_volume.lo `test -f 'pyfwsi_volume.c' || echo '$(srcdir)/'`pyfwsi_volume.c
 @am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pyfwsi_la-pyfwsi_volume.Tpo $(DEPDIR)/pyfwsi_la-pyfwsi_volume.Plo
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pyfwsi_volume.c' object='pyfwsi_la-pyfwsi_volume.lo' libtool=yes @AMDEPBACKSLASH@
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
 @am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwsi_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pyfwsi_la-pyfwsi_volume.lo `test -f 'pyfwsi_volume.c' || echo '$(srcdir)/'`pyfwsi_volume.c
 
@@ -1021,14 +1033,15 @@
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_guid.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_integer.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_item.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_item_list.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_items.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_network_location.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_root_folder.Plo
+	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_string.Plo
 	-rm -f ./$(DEPDIR)/pyfwsi_la-pyfwsi_volume.Plo
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
 
 mostlyclean: mostlyclean-am
 
 mostlyclean-am: mostlyclean-compile mostlyclean-generic \
```

### Comparing `libfwsi-20230114/libfwsi.spec` & `libfwsi-20230710/libfwsi.spec`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Name: libfwsi
-Version: 20230114
+Version: 20230710
 Release: 1
 Summary: Library to access the Windows Shell Item format
 Group: System Environment/Libraries
-License: LGPLv3+
+License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfwsi
-BuildRoot: %{_tmppath}/%{name}-%{version}-%{release}-root-%(%{__id_u} -n)
           
 BuildRequires: gcc          
 
 %description -n libfwsi
 Library to access the Windows Shell Item format
 
 %package -n libfwsi-static
@@ -53,38 +52,34 @@
 rm -rf %{buildroot}
 
 %post -p /sbin/ldconfig
 
 %postun -p /sbin/ldconfig
 
 %files -n libfwsi
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
-%attr(755,root,root) %{_libdir}/*.so.*
+%{_libdir}/*.so.*
 
 %files -n libfwsi-static
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
-%attr(755,root,root) %{_libdir}/*.a
+%{_libdir}/*.a
 
 %files -n libfwsi-devel
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/*.so
 %{_libdir}/pkgconfig/libfwsi.pc
 %{_includedir}/*
 %{_mandir}/man3/*
 
 %files -n libfwsi-python3
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %changelog
-* Mon Jan 30 2023 Joachim Metz <joachim.metz@gmail.com> 20230114-1
+* Tue Jul 11 2023 Joachim Metz <joachim.metz@gmail.com> 20230710-1
 - Auto-generated
```

### Comparing `libfwsi-20230114/manuals/libfwsi.3` & `libfwsi-20230710/manuals/libfwsi.3`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/manuals/Makefile.in` & `libfwsi-20230710/manuals/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_control_panel_values/fwsi_test_control_panel_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_control_panel_values/fwsi_test_control_panel_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_uri_values/fwsi_test_uri_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_uri_values/fwsi_test_uri_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/libfwps/libfwps.vcproj` & `libfwsi-20230710/msvscpp/libfwps/libfwps.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/libfole/libfole.vcproj` & `libfwsi-20230710/msvscpp/libfole/libfole.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0000_values/fwsi_test_extension_block_0xbeef0000_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0000_values/fwsi_test_extension_block_0xbeef0000_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0013_values/fwsi_test_extension_block_0xbeef0013_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0013_values/fwsi_test_extension_block_0xbeef0013_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/libfguid/libfguid.vcproj` & `libfwsi-20230710/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/pyfwsi/pyfwsi.vcproj` & `libfwsi-20230710/msvscpp/pyfwsi/pyfwsi.vcproj`

 * *Files 3% similar despite different names*

#### Comparing `libfwsi-20230114/msvscpp/pyfwsi/pyfwsi.vcproj` & `libfwsi-20230710/msvscpp/pyfwsi/pyfwsi.vcproj`

```diff
@@ -7,15 +7,15 @@
   <Configurations>
     <Configuration Name="Release|Win32" OutputDirectory="$(SolutionDir)$(ConfigurationName)" IntermediateDirectory="$(ConfigurationName)" ConfigurationType="2" CharacterSet="1">
       <Tool Name="VCPreBuildEventTool"/>
       <Tool Name="VCCustomBuildTool"/>
       <Tool Name="VCXMLDataGeneratorTool"/>
       <Tool Name="VCWebServiceProxyGeneratorTool"/>
       <Tool Name="VCMIDLTool"/>
-      <Tool Name="VCCLCompilerTool" AdditionalIncludeDirectories="..\..\include;..\..\common;..\..\libcerror;..\..\libcdata;..\..\libclocale;..\..\libuna;..\..\libfguid;C:\Python27\include" PreprocessorDefinitions="_CRT_SECURE_NO_DEPRECATE;HAVE_LOCAL_LIBCERROR;HAVE_LOCAL_LIBCDATA;HAVE_LOCAL_LIBCLOCALE;HAVE_LOCAL_LIBUNA;HAVE_LOCAL_LIBFGUID;LIBFWSI_DLL_IMPORT" RuntimeLibrary="2" WarningLevel="4" CompileAs="1"/>
+      <Tool Name="VCCLCompilerTool" AdditionalIncludeDirectories="..\..\include;..\..\common;..\..\libcerror;..\..\libcdata;..\..\libclocale;..\..\libuna;..\..\libfguid;C:\Python27\include" PreprocessorDefinitions="_CRT_SECURE_NO_DEPRECATE;HAVE_PYCONFIG_H;HAVE_LOCAL_LIBCERROR;HAVE_LOCAL_LIBCDATA;HAVE_LOCAL_LIBCLOCALE;HAVE_LOCAL_LIBUNA;HAVE_LOCAL_LIBFGUID;LIBFWSI_DLL_IMPORT" RuntimeLibrary="2" WarningLevel="4" CompileAs="1"/>
       <Tool Name="VCManagedResourceCompilerTool"/>
       <Tool Name="VCResourceCompilerTool"/>
       <Tool Name="VCPreLinkEventTool"/>
       <Tool Name="VCLinkerTool" OutputFile="$(OutDir)\$(ProjectName).pyd" AdditionalLibraryDirectories="&quot;$(OutDir)&quot;;C:\Python27\libs" RandomizedBaseAddress="2" DataExecutionPrevention="2" TargetMachine="1" ImportLibrary="$(OutDir)\$(ProjectName).lib"/>
       <Tool Name="VCALinkTool"/>
       <Tool Name="VCManifestTool"/>
       <Tool Name="VCXDCMakeTool"/>
@@ -26,15 +26,15 @@
     </Configuration>
     <Configuration Name="VSDebug|Win32" OutputDirectory="$(SolutionDir)$(ConfigurationName)" IntermediateDirectory="$(ConfigurationName)" ConfigurationType="2" CharacterSet="1">
       <Tool Name="VCPreBuildEventTool"/>
       <Tool Name="VCCustomBuildTool"/>
       <Tool Name="VCXMLDataGeneratorTool"/>
       <Tool Name="VCWebServiceProxyGeneratorTool"/>
       <Tool Name="VCMIDLTool"/>
-      <Tool Name="VCCLCompilerTool" Optimization="0" AdditionalIncludeDirectories="..\..\include;..\..\common;..\..\libcerror;..\..\libcdata;..\..\libclocale;..\..\libuna;..\..\libfguid;C:\Python27\include" PreprocessorDefinitions="_CRT_SECURE_NO_DEPRECATE;HAVE_LOCAL_LIBCERROR;HAVE_LOCAL_LIBCDATA;HAVE_LOCAL_LIBCLOCALE;HAVE_LOCAL_LIBUNA;HAVE_LOCAL_LIBFGUID;LIBFWSI_DLL_IMPORT" BasicRuntimeChecks="3" SmallerTypeCheck="true" RuntimeLibrary="3" WarningLevel="4" DebugInformationFormat="3" CompileAs="1"/>
+      <Tool Name="VCCLCompilerTool" Optimization="0" AdditionalIncludeDirectories="..\..\include;..\..\common;..\..\libcerror;..\..\libcdata;..\..\libclocale;..\..\libuna;..\..\libfguid;C:\Python27\include" PreprocessorDefinitions="_CRT_SECURE_NO_DEPRECATE;HAVE_PYCONFIG_H;HAVE_LOCAL_LIBCERROR;HAVE_LOCAL_LIBCDATA;HAVE_LOCAL_LIBCLOCALE;HAVE_LOCAL_LIBUNA;HAVE_LOCAL_LIBFGUID;LIBFWSI_DLL_IMPORT" BasicRuntimeChecks="3" SmallerTypeCheck="true" RuntimeLibrary="3" WarningLevel="4" DebugInformationFormat="3" CompileAs="1"/>
       <Tool Name="VCManagedResourceCompilerTool"/>
       <Tool Name="VCResourceCompilerTool"/>
       <Tool Name="VCPreLinkEventTool"/>
       <Tool Name="VCLinkerTool" OutputFile="$(OutDir)\$(ProjectName).pyd" AdditionalLibraryDirectories="&quot;$(OutDir)&quot;;C:\Python27\libs" GenerateDebugInformation="true" RandomizedBaseAddress="1" DataExecutionPrevention="1" TargetMachine="1" ImportLibrary="$(OutDir)\$(ProjectName).lib"/>
       <Tool Name="VCALinkTool"/>
       <Tool Name="VCManifestTool"/>
       <Tool Name="VCXDCMakeTool"/>
@@ -58,14 +58,15 @@
       <File RelativePath="..\..\pyfwsi\pyfwsi_guid.c"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_integer.c"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_item.c"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_item_list.c"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_items.c"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_network_location.c"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_root_folder.c"/>
+      <File RelativePath="..\..\pyfwsi\pyfwsi_string.c"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_volume.c"/>
     </Filter>
     <Filter Name="Header Files" Filter="h;hpp;hxx;hm;inl;inc;xsd" UniqueIdentifier="{93995380-89BD-4b04-88EB-625FBE52EBFB}">
       <File RelativePath="..\..\pyfwsi\pyfwsi.h"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_codepage.h"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_datetime.h"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_error.h"/>
@@ -78,17 +79,19 @@
       <File RelativePath="..\..\pyfwsi\pyfwsi_item.h"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_item_list.h"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_items.h"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_libcerror.h"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_libclocale.h"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_libfguid.h"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_libfwsi.h"/>
+      <File RelativePath="..\..\pyfwsi\pyfwsi_libuna.h"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_network_location.h"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_python.h"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_root_folder.h"/>
+      <File RelativePath="..\..\pyfwsi\pyfwsi_string.h"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_unused.h"/>
       <File RelativePath="..\..\pyfwsi\pyfwsi_volume.h"/>
     </Filter>
     <Filter Name="Resource Files" Filter="rc;ico;cur;bmp;dlg;rc2;rct;bin;rgs;gif;jpg;jpeg;jpe;resx;tiff;tif;png;wav" UniqueIdentifier="{67DA6AB6-F800-4c08-8B7A-83BB121AAD01}"/>
   </Files>
   <Globals/>
 </VisualStudioProject>
```

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_users_property_view_values/fwsi_test_users_property_view_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_users_property_view_values/fwsi_test_users_property_view_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/libclocale/libclocale.vcproj` & `libfwsi-20230710/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/Makefile.am` & `libfwsi-20230710/msvscpp/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_extension_block/fwsi_test_extension_block.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_extension_block/fwsi_test_extension_block.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_support/fwsi_test_support.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_support/fwsi_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_cdburn_values/fwsi_test_cdburn_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_cdburn_values/fwsi_test_cdburn_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0003_values/fwsi_test_extension_block_0xbeef0003_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0003_values/fwsi_test_extension_block_0xbeef0003_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0006_values/fwsi_test_extension_block_0xbeef0006_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0006_values/fwsi_test_extension_block_0xbeef0006_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_volume_values/fwsi_test_volume_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_volume_values/fwsi_test_volume_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_unknown_0x74_values/fwsi_test_unknown_0x74_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_unknown_0x74_values/fwsi_test_unknown_0x74_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_item/fwsi_test_item.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_item/fwsi_test_item.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0014_values/fwsi_test_extension_block_0xbeef0014_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0014_values/fwsi_test_extension_block_0xbeef0014_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_mtp_volume_values/fwsi_test_mtp_volume_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_mtp_volume_values/fwsi_test_mtp_volume_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_item_list/fwsi_test_item_list.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_item_list/fwsi_test_item_list.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/libfdatetime/libfdatetime.vcproj` & `libfwsi-20230710/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_root_folder_values/fwsi_test_root_folder_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_root_folder_values/fwsi_test_root_folder_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/libcthreads/libcthreads.vcproj` & `libfwsi-20230710/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_control_panel_category_values/fwsi_test_control_panel_category_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_control_panel_category_values/fwsi_test_control_panel_category_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_mtp_file_entry_values/fwsi_test_mtp_file_entry_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_mtp_file_entry_values/fwsi_test_mtp_file_entry_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_control_panel_cpl_file_values/fwsi_test_control_panel_cpl_file_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_control_panel_cpl_file_values/fwsi_test_control_panel_cpl_file_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_compressed_folder_values/fwsi_test_compressed_folder_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_compressed_folder_values/fwsi_test_compressed_folder_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_network_location_values/fwsi_test_network_location_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_network_location_values/fwsi_test_network_location_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/libuna/libuna.vcproj` & `libfwsi-20230710/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/libfwsi/libfwsi.vcproj` & `libfwsi-20230710/msvscpp/libfwsi/libfwsi.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/Makefile.in` & `libfwsi-20230710/msvscpp/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/libcerror/libcerror.vcproj` & `libfwsi-20230710/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0001_values/fwsi_test_extension_block_0xbeef0001_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0001_values/fwsi_test_extension_block_0xbeef0001_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_error/fwsi_test_error.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_error/fwsi_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/libcnotify/libcnotify.vcproj` & `libfwsi-20230710/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_delegate_values/fwsi_test_delegate_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_delegate_values/fwsi_test_delegate_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/libfwsi.sln` & `libfwsi-20230710/msvscpp/libfwsi.sln`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_uri_sub_values/fwsi_test_uri_sub_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_uri_sub_values/fwsi_test_uri_sub_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_game_folder_values/fwsi_test_game_folder_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_game_folder_values/fwsi_test_game_folder_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0025_values/fwsi_test_extension_block_0xbeef0025_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0025_values/fwsi_test_extension_block_0xbeef0025_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef000a_values/fwsi_test_extension_block_0xbeef000a_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef000a_values/fwsi_test_extension_block_0xbeef000a_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_file_entry_values/fwsi_test_file_entry_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_file_entry_values/fwsi_test_file_entry_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/libcdata/libcdata.vcproj` & `libfwsi-20230710/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0005_values/fwsi_test_extension_block_0xbeef0005_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0005_values/fwsi_test_extension_block_0xbeef0005_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_extension_block_0xbeef0019_values/fwsi_test_extension_block_0xbeef0019_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_extension_block_0xbeef0019_values/fwsi_test_extension_block_0xbeef0019_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/msvscpp/fwsi_test_file_entry_extension_values/fwsi_test_file_entry_extension_values.vcproj` & `libfwsi-20230710/msvscpp/fwsi_test_file_entry_extension_values/fwsi_test_file_entry_extension_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/setup.py` & `libfwsi-20230710/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 #
 # Script to build and install Python-bindings.
-# Version: 20221217
+# Version: 20230411
 
 from __future__ import print_function
 
 import copy
 import datetime
 import glob
 import gzip
@@ -91,14 +91,15 @@
     build_ext.build_extensions(self)
 
   def run(self):
     """Runs the build extension."""
     compiler = new_compiler(compiler=self.compiler)
     if compiler.compiler_type == "msvc":
       self.define = [
+          ("_CRT_SECURE_NO_WARNINGS", ""),
           ("UNICODE", ""),
       ]
 
     else:
       command = "sh configure --disable-nls --disable-shared-libs"
       output = self._RunCommand(command)
```

### Comparing `libfwsi-20230114/config.guess` & `libfwsi-20230710/config.guess`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/ossfuzz/item_fuzzer.cc` & `libfwsi-20230710/ossfuzz/item_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/ossfuzz/Makefile.am` & `libfwsi-20230710/ossfuzz/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/ossfuzz/item_list_fuzzer.cc` & `libfwsi-20230710/ossfuzz/item_list_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/ossfuzz/Makefile.in` & `libfwsi-20230710/ossfuzz/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/ossfuzz/ossfuzz_libfwsi.h` & `libfwsi-20230710/ossfuzz/ossfuzz_libfwsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/test-driver` & `libfwsi-20230710/test-driver`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/configure` & `libfwsi-20230710/configure`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfwsi 20230114.
+# Generated by GNU Autoconf 2.71 for libfwsi 20230710.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libfwsi'
 PACKAGE_TARNAME='libfwsi'
-PACKAGE_VERSION='20230114'
-PACKAGE_STRING='libfwsi 20230114'
+PACKAGE_VERSION='20230710'
+PACKAGE_STRING='libfwsi 20230710'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfwsi.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1612,15 +1612,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfwsi 20230114 to adapt to many kinds of systems.
+\`configure' configures libfwsi 20230710 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1683,15 +1683,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfwsi 20230114:";;
+     short | recursive ) echo "Configuration of libfwsi 20230710:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1902,15 +1902,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfwsi configure 20230114
+libfwsi configure 20230710
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2623,15 +2623,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfwsi $as_me 20230114, which was
+It was created by libfwsi $as_me 20230710, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4112,15 +4112,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfwsi'
- VERSION='20230114'
+ VERSION='20230710'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -32357,37 +32357,37 @@
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna" >&5
 printf %s "checking for libuna... " >&6; }
 
 if test -n "$libuna_CFLAGS"; then
     pkg_cv_libuna_CFLAGS="$libuna_CFLAGS"
  elif test -n "$PKG_CONFIG"; then
     if test -n "$PKG_CONFIG" && \
-    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libuna >= 20210801\""; } >&5
-  ($PKG_CONFIG --exists --print-errors "libuna >= 20210801") 2>&5
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libuna >= 20230702\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "libuna >= 20230702") 2>&5
   ac_status=$?
   printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
   test $ac_status = 0; }; then
-  pkg_cv_libuna_CFLAGS=`$PKG_CONFIG --cflags "libuna >= 20210801" 2>/dev/null`
+  pkg_cv_libuna_CFLAGS=`$PKG_CONFIG --cflags "libuna >= 20230702" 2>/dev/null`
 		      test "x$?" != "x0" && pkg_failed=yes
 else
   pkg_failed=yes
 fi
  else
     pkg_failed=untried
 fi
 if test -n "$libuna_LIBS"; then
     pkg_cv_libuna_LIBS="$libuna_LIBS"
  elif test -n "$PKG_CONFIG"; then
     if test -n "$PKG_CONFIG" && \
-    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libuna >= 20210801\""; } >&5
-  ($PKG_CONFIG --exists --print-errors "libuna >= 20210801") 2>&5
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libuna >= 20230702\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "libuna >= 20230702") 2>&5
   ac_status=$?
   printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
   test $ac_status = 0; }; then
-  pkg_cv_libuna_LIBS=`$PKG_CONFIG --libs "libuna >= 20210801" 2>/dev/null`
+  pkg_cv_libuna_LIBS=`$PKG_CONFIG --libs "libuna >= 20230702" 2>/dev/null`
 		      test "x$?" != "x0" && pkg_failed=yes
 else
   pkg_failed=yes
 fi
  else
     pkg_failed=untried
 fi
@@ -32400,17 +32400,17 @@
 
 if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
         _pkg_short_errors_supported=yes
 else
         _pkg_short_errors_supported=no
 fi
         if test $_pkg_short_errors_supported = yes; then
-	        libuna_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "libuna >= 20210801" 2>&1`
+	        libuna_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "libuna >= 20230702" 2>&1`
         else
-	        libuna_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "libuna >= 20210801" 2>&1`
+	        libuna_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "libuna >= 20230702" 2>&1`
         fi
 	# Put the nasty error message in config.log where it belongs
 	echo "$libuna_PKG_ERRORS" >&5
 
 	ac_cv_libuna=check
 elif test $pkg_failed = untried; then
      	{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
@@ -33712,14 +33712,1107 @@
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
 
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_size_to_byte_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_size_to_byte_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_size_to_byte_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_size_to_byte_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_size_to_byte_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_size_to_byte_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_size_to_byte_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_size_to_byte_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_size_to_byte_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_size_to_byte_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_byte_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_byte_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_byte_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_byte_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_byte_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_byte_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_byte_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_byte_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_byte_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_byte_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_byte_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_byte_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_byte_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_byte_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_byte_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_byte_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_byte_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_byte_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_byte_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_byte_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_size_to_ucs2 in -luna" >&5
+printf %s "checking for libuna_unicode_character_size_to_ucs2 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_size_to_ucs2+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_size_to_ucs2 ();
+int
+main (void)
+{
+return libuna_unicode_character_size_to_ucs2 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_size_to_ucs2=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_size_to_ucs2=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_size_to_ucs2" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_size_to_ucs2" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_size_to_ucs2" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_ucs2 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_ucs2 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_ucs2 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_ucs2 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_ucs2 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_ucs2 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_ucs2 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_ucs2 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_size_to_ucs4 in -luna" >&5
+printf %s "checking for libuna_unicode_character_size_to_ucs4 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_size_to_ucs4+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_size_to_ucs4 ();
+int
+main (void)
+{
+return libuna_unicode_character_size_to_ucs4 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_size_to_ucs4=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_size_to_ucs4=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_size_to_ucs4" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_size_to_ucs4" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_size_to_ucs4" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_ucs4 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_ucs4 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_ucs4 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_ucs4 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_ucs4 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_ucs4 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_ucs4 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_ucs4 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_utf7_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_utf7_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_utf7_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_utf7_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_utf7_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf7_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf7_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_utf7_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_utf7_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_utf7_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_utf7_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_utf7_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_utf7_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_utf7_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_utf7_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf7_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf7_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_utf7_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_utf7_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_utf7_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_size_to_utf8 in -luna" >&5
+printf %s "checking for libuna_unicode_character_size_to_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_size_to_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_size_to_utf8 ();
+int
+main (void)
+{
+return libuna_unicode_character_size_to_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_size_to_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_size_to_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_size_to_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_size_to_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_size_to_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_utf8 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_utf8 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_utf8 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_utf8 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_size_to_utf8_rfc2279 in -luna" >&5
+printf %s "checking for libuna_unicode_character_size_to_utf8_rfc2279 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_size_to_utf8_rfc2279+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_size_to_utf8_rfc2279 ();
+int
+main (void)
+{
+return libuna_unicode_character_size_to_utf8_rfc2279 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_size_to_utf8_rfc2279=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_size_to_utf8_rfc2279=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_size_to_utf8_rfc2279" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_size_to_utf8_rfc2279" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_size_to_utf8_rfc2279" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_utf8_rfc2279 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_utf8_rfc2279 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_utf8_rfc2279+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_utf8_rfc2279 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_utf8_rfc2279 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf8_rfc2279=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf8_rfc2279=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_utf8_rfc2279" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_utf8_rfc2279" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_utf8_rfc2279" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_utf8_rfc2279 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_utf8_rfc2279 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_utf8_rfc2279+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_utf8_rfc2279 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_utf8_rfc2279 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf8_rfc2279=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf8_rfc2279=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_utf8_rfc2279" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_utf8_rfc2279" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_utf8_rfc2279" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_size_to_utf16 in -luna" >&5
+printf %s "checking for libuna_unicode_character_size_to_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_size_to_utf16+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_size_to_utf16 ();
+int
+main (void)
+{
+return libuna_unicode_character_size_to_utf16 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_size_to_utf16=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_size_to_utf16=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_size_to_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_size_to_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_size_to_utf16" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_utf16 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_utf16+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_utf16 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_utf16 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf16=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf16=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_utf16" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_utf16 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_utf16+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_utf16 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_utf16 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf16=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf16=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_utf16" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_utf16_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_utf16_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_utf16_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_utf16_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf16_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf16_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_utf16_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_utf16_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_utf16_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_utf16_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_utf16_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf16_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf16_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_utf16_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_utf32 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_utf32 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_utf32+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_utf32 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_utf32 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf32=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf32=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_utf32" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_utf32" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_utf32" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_utf32 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_utf32 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_utf32+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_utf32 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_utf32 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf32=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf32=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_utf32" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_utf32" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_utf32" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_utf32_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_utf32_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_utf32_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf32_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf32_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_utf32_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_utf32_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_utf32_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_utf32_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_utf32_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf32_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf32_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_utf32_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+
                 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_stream_size_from_utf8 in -luna" >&5
 printf %s "checking for libuna_utf8_stream_size_from_utf8 in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf8_stream_size_from_utf8+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -34597,14 +35690,56 @@
 if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_byte_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_compare_with_byte_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_compare_with_byte_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_compare_with_byte_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf8_string_compare_with_byte_stream ();
+int
+main (void)
+{
+return libuna_utf8_string_compare_with_byte_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf8_string_compare_with_byte_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf8_string_compare_with_byte_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_compare_with_byte_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_compare_with_byte_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_compare_with_byte_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf7_stream in -luna" >&5
 printf %s "checking for libuna_utf8_string_size_from_utf7_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf7_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -34723,14 +35858,56 @@
 if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf7_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_compare_with_utf7_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_compare_with_utf7_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_compare_with_utf7_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf8_string_compare_with_utf7_stream ();
+int
+main (void)
+{
+return libuna_utf8_string_compare_with_utf7_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf7_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf7_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_compare_with_utf7_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_compare_with_utf7_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_compare_with_utf7_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf8_stream in -luna" >&5
 printf %s "checking for libuna_utf8_string_size_from_utf8_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf8_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -34849,386 +36026,386 @@
 if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf8_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf16_stream in -luna" >&5
-printf %s "checking for libuna_utf8_string_size_from_utf16_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_compare_with_utf8_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_compare_with_utf8_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_compare_with_utf8_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_size_from_utf16_stream ();
+char libuna_utf8_string_compare_with_utf8_stream ();
 int
 main (void)
 {
-return libuna_utf8_string_size_from_utf16_stream ();
+return libuna_utf8_string_compare_with_utf8_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream=yes
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf8_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream=no
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf8_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_compare_with_utf8_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_compare_with_utf8_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_compare_with_utf8_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_copy_from_utf16_stream in -luna" >&5
-printf %s "checking for libuna_utf8_string_copy_from_utf16_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf16 in -luna" >&5
+printf %s "checking for libuna_utf8_string_size_from_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf16+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_copy_from_utf16_stream ();
+char libuna_utf8_string_size_from_utf16 ();
 int
 main (void)
 {
-return libuna_utf8_string_copy_from_utf16_stream ();
+return libuna_utf8_string_size_from_utf16 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream=yes
+  ac_cv_lib_una_libuna_utf8_string_size_from_utf16=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream=no
+  ac_cv_lib_una_libuna_utf8_string_size_from_utf16=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_size_from_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_size_from_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_size_from_utf16" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_with_index_copy_from_utf16_stream in -luna" >&5
-printf %s "checking for libuna_utf8_string_with_index_copy_from_utf16_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_copy_from_utf16 in -luna" >&5
+printf %s "checking for libuna_utf8_string_copy_from_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_copy_from_utf16+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_with_index_copy_from_utf16_stream ();
+char libuna_utf8_string_copy_from_utf16 ();
 int
 main (void)
 {
-return libuna_utf8_string_with_index_copy_from_utf16_stream ();
+return libuna_utf8_string_copy_from_utf16 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream=yes
+  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream=no
+  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_copy_from_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf8_string_size_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_with_index_copy_from_utf16 in -luna" >&5
+printf %s "checking for libuna_utf8_string_with_index_copy_from_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_size_from_utf32_stream ();
+char libuna_utf8_string_with_index_copy_from_utf16 ();
 int
 main (void)
 {
-return libuna_utf8_string_size_from_utf32_stream ();
+return libuna_utf8_string_with_index_copy_from_utf16 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_copy_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf8_string_copy_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_compare_with_utf16 in -luna" >&5
+printf %s "checking for libuna_utf8_string_compare_with_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_compare_with_utf16+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_copy_from_utf32_stream ();
+char libuna_utf8_string_compare_with_utf16 ();
 int
 main (void)
 {
-return libuna_utf8_string_copy_from_utf32_stream ();
+return libuna_utf8_string_compare_with_utf16 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf16=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf16=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_compare_with_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_compare_with_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_compare_with_utf16" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_with_index_copy_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf8_string_with_index_copy_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_size_from_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_with_index_copy_from_utf32_stream ();
+char libuna_utf8_string_size_from_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf8_string_with_index_copy_from_utf32_stream ();
+return libuna_utf8_string_size_from_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf16 in -luna" >&5
-printf %s "checking for libuna_utf8_string_size_from_utf16 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf16+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_copy_from_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_copy_from_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_size_from_utf16 ();
+char libuna_utf8_string_copy_from_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf8_string_size_from_utf16 ();
+return libuna_utf8_string_copy_from_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_size_from_utf16=yes
+  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_size_from_utf16=no
+  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_size_from_utf16" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_size_from_utf16" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_size_from_utf16" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_copy_from_utf16 in -luna" >&5
-printf %s "checking for libuna_utf8_string_copy_from_utf16 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_copy_from_utf16+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_with_index_copy_from_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_with_index_copy_from_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_copy_from_utf16 ();
+char libuna_utf8_string_with_index_copy_from_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf8_string_copy_from_utf16 ();
+return libuna_utf8_string_with_index_copy_from_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16=yes
+  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16=no
+  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_copy_from_utf16" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_with_index_copy_from_utf16 in -luna" >&5
-printf %s "checking for libuna_utf8_string_with_index_copy_from_utf16 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_compare_with_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_compare_with_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_compare_with_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_with_index_copy_from_utf16 ();
+char libuna_utf8_string_compare_with_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf8_string_with_index_copy_from_utf16 ();
+return libuna_utf8_string_compare_with_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16=yes
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16=no
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_compare_with_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_compare_with_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_compare_with_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf32 in -luna" >&5
@@ -35353,14 +36530,224 @@
 if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_compare_with_utf32 in -luna" >&5
+printf %s "checking for libuna_utf8_string_compare_with_utf32 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_compare_with_utf32+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf8_string_compare_with_utf32 ();
+int
+main (void)
+{
+return libuna_utf8_string_compare_with_utf32 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf32=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf32=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_compare_with_utf32" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_compare_with_utf32" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_compare_with_utf32" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_size_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf8_string_size_from_utf32_stream ();
+int
+main (void)
+{
+return libuna_utf8_string_size_from_utf32_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_copy_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_copy_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf8_string_copy_from_utf32_stream ();
+int
+main (void)
+{
+return libuna_utf8_string_copy_from_utf32_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_with_index_copy_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_with_index_copy_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf8_string_with_index_copy_from_utf32_stream ();
+int
+main (void)
+{
+return libuna_utf8_string_with_index_copy_from_utf32_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_compare_with_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_compare_with_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_compare_with_utf32_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf8_string_compare_with_utf32_stream ();
+int
+main (void)
+{
+return libuna_utf8_string_compare_with_utf32_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf32_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf32_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_compare_with_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_compare_with_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_compare_with_utf32_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_scsu_stream in -luna" >&5
 printf %s "checking for libuna_utf8_string_size_from_scsu_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf8_string_size_from_scsu_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -35606,14 +36993,56 @@
 if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_byte_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_compare_with_byte_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_compare_with_byte_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_compare_with_byte_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf16_string_compare_with_byte_stream ();
+int
+main (void)
+{
+return libuna_utf16_string_compare_with_byte_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf16_string_compare_with_byte_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf16_string_compare_with_byte_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_compare_with_byte_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_compare_with_byte_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_compare_with_byte_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf7_stream in -luna" >&5
 printf %s "checking for libuna_utf16_string_size_from_utf7_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf7_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -35732,15 +37161,183 @@
 if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf7_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf8_stream in -luna" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_compare_with_utf7_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_compare_with_utf7_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_compare_with_utf7_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf16_string_compare_with_utf7_stream ();
+int
+main (void)
+{
+return libuna_utf16_string_compare_with_utf7_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf7_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf7_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_compare_with_utf7_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_compare_with_utf7_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_compare_with_utf7_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf8 in -luna" >&5
+printf %s "checking for libuna_utf16_string_size_from_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf16_string_size_from_utf8 ();
+int
+main (void)
+{
+return libuna_utf16_string_size_from_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf16_string_size_from_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf16_string_size_from_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_size_from_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_size_from_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_size_from_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_copy_from_utf8 in -luna" >&5
+printf %s "checking for libuna_utf16_string_copy_from_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_copy_from_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf16_string_copy_from_utf8 ();
+int
+main (void)
+{
+return libuna_utf16_string_copy_from_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf16_string_copy_from_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf16_string_copy_from_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_copy_from_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_copy_from_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_copy_from_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_with_index_copy_from_utf8 in -luna" >&5
+printf %s "checking for libuna_utf16_string_with_index_copy_from_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf16_string_with_index_copy_from_utf8 ();
+int
+main (void)
+{
+return libuna_utf16_string_with_index_copy_from_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf8_stream in -luna" >&5
 printf %s "checking for libuna_utf16_string_size_from_utf8_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf8_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
@@ -35858,14 +37455,56 @@
 if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_compare_with_utf8_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_compare_with_utf8_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_compare_with_utf8_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf16_string_compare_with_utf8_stream ();
+int
+main (void)
+{
+return libuna_utf16_string_compare_with_utf8_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf8_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf8_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_compare_with_utf8_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_compare_with_utf8_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_compare_with_utf8_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf16_stream in -luna" >&5
 printf %s "checking for libuna_utf16_string_size_from_utf16_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -35984,386 +37623,386 @@
 if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf16_string_size_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_compare_with_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_compare_with_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_compare_with_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_size_from_utf32_stream ();
+char libuna_utf16_string_compare_with_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf16_string_size_from_utf32_stream ();
+return libuna_utf16_string_compare_with_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_compare_with_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_compare_with_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_compare_with_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_copy_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf16_string_copy_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf32 in -luna" >&5
+printf %s "checking for libuna_utf16_string_size_from_utf32 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf32+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_copy_from_utf32_stream ();
+char libuna_utf16_string_size_from_utf32 ();
 int
 main (void)
 {
-return libuna_utf16_string_copy_from_utf32_stream ();
+return libuna_utf16_string_size_from_utf32 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf16_string_size_from_utf32=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf16_string_size_from_utf32=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_size_from_utf32" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_size_from_utf32" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_size_from_utf32" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_with_index_copy_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf16_string_with_index_copy_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_copy_from_utf32 in -luna" >&5
+printf %s "checking for libuna_utf16_string_copy_from_utf32 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_copy_from_utf32+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_with_index_copy_from_utf32_stream ();
+char libuna_utf16_string_copy_from_utf32 ();
 int
 main (void)
 {
-return libuna_utf16_string_with_index_copy_from_utf32_stream ();
+return libuna_utf16_string_copy_from_utf32 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_copy_from_utf32" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf8 in -luna" >&5
-printf %s "checking for libuna_utf16_string_size_from_utf8 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf8+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_with_index_copy_from_utf32 in -luna" >&5
+printf %s "checking for libuna_utf16_string_with_index_copy_from_utf32 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_size_from_utf8 ();
+char libuna_utf16_string_with_index_copy_from_utf32 ();
 int
 main (void)
 {
-return libuna_utf16_string_size_from_utf8 ();
+return libuna_utf16_string_with_index_copy_from_utf32 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_size_from_utf8=yes
+  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_size_from_utf8=no
+  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_size_from_utf8" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_size_from_utf8" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_size_from_utf8" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_copy_from_utf8 in -luna" >&5
-printf %s "checking for libuna_utf16_string_copy_from_utf8 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_copy_from_utf8+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_compare_with_utf32 in -luna" >&5
+printf %s "checking for libuna_utf16_string_compare_with_utf32 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_compare_with_utf32+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_copy_from_utf8 ();
+char libuna_utf16_string_compare_with_utf32 ();
 int
 main (void)
 {
-return libuna_utf16_string_copy_from_utf8 ();
+return libuna_utf16_string_compare_with_utf32 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_copy_from_utf8=yes
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf32=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_copy_from_utf8=no
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf32=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_copy_from_utf8" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_copy_from_utf8" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_copy_from_utf8" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_compare_with_utf32" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_compare_with_utf32" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_compare_with_utf32" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_with_index_copy_from_utf8 in -luna" >&5
-printf %s "checking for libuna_utf16_string_with_index_copy_from_utf8 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_size_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_with_index_copy_from_utf8 ();
+char libuna_utf16_string_size_from_utf32_stream ();
 int
 main (void)
 {
-return libuna_utf16_string_with_index_copy_from_utf8 ();
+return libuna_utf16_string_size_from_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8=yes
+  ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8=no
+  ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf32 in -luna" >&5
-printf %s "checking for libuna_utf16_string_size_from_utf32 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf32+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_copy_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_copy_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_size_from_utf32 ();
+char libuna_utf16_string_copy_from_utf32_stream ();
 int
 main (void)
 {
-return libuna_utf16_string_size_from_utf32 ();
+return libuna_utf16_string_copy_from_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_size_from_utf32=yes
+  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_size_from_utf32=no
+  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_size_from_utf32" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_size_from_utf32" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_size_from_utf32" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_copy_from_utf32 in -luna" >&5
-printf %s "checking for libuna_utf16_string_copy_from_utf32 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_copy_from_utf32+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_with_index_copy_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_with_index_copy_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_copy_from_utf32 ();
+char libuna_utf16_string_with_index_copy_from_utf32_stream ();
 int
 main (void)
 {
-return libuna_utf16_string_copy_from_utf32 ();
+return libuna_utf16_string_with_index_copy_from_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32=yes
+  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32=no
+  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_copy_from_utf32" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_with_index_copy_from_utf32 in -luna" >&5
-printf %s "checking for libuna_utf16_string_with_index_copy_from_utf32 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_compare_with_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_compare_with_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_compare_with_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_with_index_copy_from_utf32 ();
+char libuna_utf16_string_compare_with_utf32_stream ();
 int
 main (void)
 {
-return libuna_utf16_string_with_index_copy_from_utf32 ();
+return libuna_utf16_string_compare_with_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32=yes
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32=no
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_compare_with_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_compare_with_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_compare_with_utf32_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_scsu_stream in -luna" >&5
@@ -36615,14 +38254,56 @@
 if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_byte_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_compare_with_byte_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_compare_with_byte_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_compare_with_byte_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf32_string_compare_with_byte_stream ();
+int
+main (void)
+{
+return libuna_utf32_string_compare_with_byte_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf32_string_compare_with_byte_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf32_string_compare_with_byte_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_compare_with_byte_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_compare_with_byte_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_compare_with_byte_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf7_stream in -luna" >&5
 printf %s "checking for libuna_utf32_string_size_from_utf7_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf7_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -36741,14 +38422,56 @@
 if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf7_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_compare_with_utf7_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_compare_with_utf7_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_compare_with_utf7_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf32_string_compare_with_utf7_stream ();
+int
+main (void)
+{
+return libuna_utf32_string_compare_with_utf7_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf7_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf7_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_compare_with_utf7_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_compare_with_utf7_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_compare_with_utf7_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf8_stream in -luna" >&5
 printf %s "checking for libuna_utf32_string_size_from_utf8_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf8_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -36783,15 +38506,139 @@
 if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf8_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf8_stream in -luna" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf8 in -luna" >&5
+printf %s "checking for libuna_utf32_string_size_from_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf32_string_size_from_utf8 ();
+int
+main (void)
+{
+return libuna_utf32_string_size_from_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf8 in -luna" >&5
+printf %s "checking for libuna_utf32_string_copy_from_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf32_string_copy_from_utf8 ();
+int
+main (void)
+{
+return libuna_utf32_string_copy_from_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for ac_cv_libuna_dummy=yes in -llibuna_utf32_string_with_index_copy_from_utf8" >&5
+printf %s "checking for ac_cv_libuna_dummy=yes in -llibuna_utf32_string_with_index_copy_from_utf8... " >&6; }
+if test ${ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-llibuna_utf32_string_with_index_copy_from_utf8  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char ac_cv_libuna_dummy=yes ();
+int
+main (void)
+{
+return ac_cv_libuna_dummy=yes ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes=yes
+else $as_nop
+  ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes" >&5
+printf "%s\n" "$ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes" >&6; }
+if test "x$ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes" = xyes
+then :
+  ac_cv_libuna=no
+fi
+
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf8_stream in -luna" >&5
 printf %s "checking for libuna_utf32_string_copy_from_utf8_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf8_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
@@ -36867,510 +38714,512 @@
 if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf8_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf16_stream in -luna" >&5
-printf %s "checking for libuna_utf32_string_size_from_utf16_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_compare_with_utf8_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_compare_with_utf8_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_compare_with_utf8_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_size_from_utf16_stream ();
+char libuna_utf32_string_compare_with_utf8_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_size_from_utf16_stream ();
+return libuna_utf32_string_compare_with_utf8_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream=yes
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf8_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream=no
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf8_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_compare_with_utf8_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_compare_with_utf8_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_compare_with_utf8_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf16_stream in -luna" >&5
-printf %s "checking for libuna_utf32_string_copy_from_utf16_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf16 in -luna" >&5
+printf %s "checking for libuna_utf32_string_size_from_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf16+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_copy_from_utf16_stream ();
+char libuna_utf32_string_size_from_utf16 ();
 int
 main (void)
 {
-return libuna_utf32_string_copy_from_utf16_stream ();
+return libuna_utf32_string_size_from_utf16 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream=yes
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf16=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream=no
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf16=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf16" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_with_index_copy_from_utf16_stream in -luna" >&5
-printf %s "checking for libuna_utf32_string_with_index_copy_from_utf16_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf16 in -luna" >&5
+printf %s "checking for libuna_utf32_string_copy_from_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf16+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_with_index_copy_from_utf16_stream ();
+char libuna_utf32_string_copy_from_utf16 ();
 int
 main (void)
 {
-return libuna_utf32_string_with_index_copy_from_utf16_stream ();
+return libuna_utf32_string_copy_from_utf16 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream=yes
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream=no
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf32_string_size_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_with_index_copy_from_utf16 in -luna" >&5
+printf %s "checking for libuna_utf32_string_with_index_copy_from_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_size_from_utf32_stream ();
+char libuna_utf32_string_with_index_copy_from_utf16 ();
 int
 main (void)
 {
-return libuna_utf32_string_size_from_utf32_stream ();
+return libuna_utf32_string_with_index_copy_from_utf16 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf32_string_copy_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream+y}
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_size_from_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_copy_from_utf32_stream ();
+char libuna_utf32_string_size_from_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_copy_from_utf32_stream ();
+return libuna_utf32_string_size_from_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_with_index_copy_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf32_string_with_index_copy_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_copy_from_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_with_index_copy_from_utf32_stream ();
+char libuna_utf32_string_copy_from_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_with_index_copy_from_utf32_stream ();
+return libuna_utf32_string_copy_from_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf8 in -luna" >&5
-printf %s "checking for libuna_utf32_string_size_from_utf8 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf8+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_with_index_copy_from_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_with_index_copy_from_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_size_from_utf8 ();
+char libuna_utf32_string_with_index_copy_from_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_size_from_utf8 ();
+return libuna_utf32_string_with_index_copy_from_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf8=yes
+  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf8=no
+  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf8" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf8" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf8" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf8 in -luna" >&5
-printf %s "checking for libuna_utf32_string_copy_from_utf8 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf8+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_compare_with_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_compare_with_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_compare_with_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_copy_from_utf8 ();
+char libuna_utf32_string_compare_with_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_copy_from_utf8 ();
+return libuna_utf32_string_compare_with_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf8=yes
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf8=no
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf8" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf8" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf8" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_compare_with_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_compare_with_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_compare_with_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for ac_cv_libuna_dummy=yes in -llibuna_utf32_string_with_index_copy_from_utf8" >&5
-printf %s "checking for ac_cv_libuna_dummy=yes in -llibuna_utf32_string_with_index_copy_from_utf8... " >&6; }
-if test ${ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_size_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
-LIBS="-llibuna_utf32_string_with_index_copy_from_utf8  $LIBS"
+LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char ac_cv_libuna_dummy=yes ();
+char libuna_utf32_string_size_from_utf32_stream ();
 int
 main (void)
 {
-return ac_cv_libuna_dummy=yes ();
+return libuna_utf32_string_size_from_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes=yes
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes=no
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes" >&5
-printf "%s\n" "$ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes" >&6; }
-if test "x$ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream" = xyes
 then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf16 in -luna" >&5
-printf %s "checking for libuna_utf32_string_size_from_utf16 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf16+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_copy_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_size_from_utf16 ();
+char libuna_utf32_string_copy_from_utf32_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_size_from_utf16 ();
+return libuna_utf32_string_copy_from_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf16=yes
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf16=no
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf16" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf16" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf16" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf16 in -luna" >&5
-printf %s "checking for libuna_utf32_string_copy_from_utf16 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf16+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_with_index_copy_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_with_index_copy_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_copy_from_utf16 ();
+char libuna_utf32_string_with_index_copy_from_utf32_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_copy_from_utf16 ();
+return libuna_utf32_string_with_index_copy_from_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16=yes
+  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16=no
+  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf16" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_with_index_copy_from_utf16 in -luna" >&5
-printf %s "checking for libuna_utf32_string_with_index_copy_from_utf16 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_compare_with_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_compare_with_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_compare_with_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_with_index_copy_from_utf16 ();
+char libuna_utf32_string_compare_with_utf32_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_with_index_copy_from_utf16 ();
+return libuna_utf32_string_compare_with_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16=yes
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16=no
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_compare_with_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_compare_with_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_compare_with_utf32_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_scsu_stream in -luna" >&5
@@ -37640,14 +39489,62 @@
 printf "%s\n" "$ac_cv_libuna_defines_compare_greater" >&6; }
 
         if test "x$ac_cv_libuna_defines_compare_less" != xyes
 then :
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking if \`LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE' is defined" >&5
+printf %s "checking if \`LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE' is defined... " >&6; }
+if test ${ac_cv_libuna_defines_compare_greater+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_ext=c
+ac_cpp='$CPP $CPPFLAGS'
+ac_compile='$CC -c $CFLAGS $CPPFLAGS conftest.$ac_ext >&5'
+ac_link='$CC -o conftest$ac_exeext $CFLAGS $CPPFLAGS $LDFLAGS conftest.$ac_ext $LIBS >&5'
+ac_compiler_gnu=$ac_cv_c_compiler_gnu
+
+    cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+#include <libuna.h>
+int
+main (void)
+{
+int test = LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE;
+
+return( 0 );
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_libuna_defines_compare_greater=yes
+else $as_nop
+  ac_cv_libuna_defines_compare_greater=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+    ac_ext=c
+ac_cpp='$CPP $CPPFLAGS'
+ac_compile='$CC -c $CFLAGS $CPPFLAGS conftest.$ac_ext >&5'
+ac_link='$CC -o conftest$ac_exeext $CFLAGS $CPPFLAGS $LDFLAGS conftest.$ac_ext $LIBS >&5'
+ac_compiler_gnu=$ac_cv_c_compiler_gnu
+
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_libuna_defines_compare_greater" >&5
+printf "%s\n" "$ac_cv_libuna_defines_compare_greater" >&6; }
+
+        if test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes
+then :
+  ac_cv_libuna=no
+fi
+
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
     if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45405,15 +47302,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfwsi $as_me 20230114, which was
+This file was extended by libfwsi $as_me 20230710, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -45473,15 +47370,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfwsi config.status 20230114
+libfwsi config.status 20230710
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfwsi-20230114/libuna/libuna_url_stream.c` & `libfwsi-20230710/libuna/libuna_url_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Percent or URL encoded stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_symbol.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_symbol.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacSymbol codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_support.c` & `libfwsi-20230710/libuna/libuna_support.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_scsu.h` & `libfwsi-20230710/libuna/libuna_scsu.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Standard Compression Scheme for Unicode (SCSU) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_5.c` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_5.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-5 codepage (Cyrillic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_2.c` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_2.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-2 codepage (Central European) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1253.c` & `libfwsi-20230710/libuna/libuna_codepage_windows_1253.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1253 codepage (Greek) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_koi8_u.h` & `libfwsi-20230710/libuna/libuna_codepage_koi8_u.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-U codepage (Ukrainian Cyrillic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1252.c` & `libfwsi-20230710/libuna/libuna_codepage_windows_1252.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1252 codepage (Western European/Latin 1) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_utf32_stream.c` & `libfwsi-20230710/libuna/libuna_utf32_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -122,14 +122,15 @@
      const libuna_utf8_character_t *utf8_string,
      size_t utf8_string_size,
      size_t *utf32_stream_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf32_stream_size_from_utf8";
 	libuna_unicode_character_t unicode_character = 0;
+	size_t safe_utf32_stream_size                = 0;
 	size_t utf8_string_index                     = 0;
 
 	if( utf8_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -159,15 +160,15 @@
 		 "%s: invalid UTF-32 stream size.",
 		 function );
 
 		return( -1 );
 	}
 	/* Add the byte order mark
 	 */
-	*utf32_stream_size = 1;
+	safe_utf32_stream_size = 1;
 
 	while( utf8_string_index < utf8_string_size )
 	{
 		/* Convert the UTF-8 character bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf8(
 		     &unicode_character,
@@ -185,15 +186,15 @@
 
 			return( -1 );
 		}
 		/* Determine how many UTF-32 character bytes are required
 		 */
 		if( libuna_unicode_character_size_to_utf32(
 		     unicode_character,
-		     utf32_stream_size,
+		     &safe_utf32_stream_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to determine size of Unicode character in UTF-32.",
@@ -204,15 +205,15 @@
 		if( unicode_character == 0 )
 		{
 			break;
 		}
 	}
 	/* Convert the number of characters into bytes
 	 */
-	*utf32_stream_size *= 4;
+	*utf32_stream_size = safe_utf32_stream_size * 4;
 
 	return( 1 );
 }
 
 /* Copies an UTF-32 stream from an UTF-8 string
  * Returns 1 if successful or -1 on error
  */
@@ -355,14 +356,15 @@
      const libuna_utf16_character_t *utf16_string,
      size_t utf16_string_size,
      size_t *utf32_stream_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf32_stream_size_from_utf16";
 	libuna_unicode_character_t unicode_character = 0;
+	size_t safe_utf32_stream_size                = 0;
 	size_t utf16_string_index                    = 0;
 
 	if( utf16_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -392,15 +394,15 @@
 		 "%s: invalid UTF-32 stream size.",
 		 function );
 
 		return( -1 );
 	}
 	/* Add the byte order mark
 	 */
-	*utf32_stream_size = 1;
+	safe_utf32_stream_size = 1;
 
 	while( utf16_string_index < utf16_string_size )
 	{
 		/* Convert the UTF-16 character bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16(
 		     &unicode_character,
@@ -418,15 +420,15 @@
 
 			return( -1 );
 		}
 		/* Determine how many UTF-32 character bytes are required
 		 */
 		if( libuna_unicode_character_size_to_utf32(
 		     unicode_character,
-		     utf32_stream_size,
+		     &safe_utf32_stream_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to determine size of Unicode character in UTF-32.",
@@ -437,15 +439,15 @@
 		if( unicode_character == 0 )
 		{
 			break;
 		}
 	}
 	/* Convert the number of characters into bytes
 	 */
-	*utf32_stream_size *= 4;
+	*utf32_stream_size = safe_utf32_stream_size * 4;
 
 	return( 1 );
 }
 
 /* Copies an UTF-32 stream from an UTF-16 string
  * Returns 1 if successful or -1 on error
  */
@@ -588,14 +590,15 @@
      const libuna_utf32_character_t *utf32_string,
      size_t utf32_string_size,
      size_t *utf32_stream_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf32_stream_size_from_utf32";
 	libuna_unicode_character_t unicode_character = 0;
+	size_t safe_utf32_stream_size                = 0;
 	size_t utf32_string_index                    = 0;
 
 	if( utf32_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -625,15 +628,15 @@
 		 "%s: invalid UTF-32 stream size.",
 		 function );
 
 		return( -1 );
 	}
 	/* Add the byte order mark
 	 */
-	*utf32_stream_size = 1;
+	safe_utf32_stream_size = 1;
 
 	while( utf32_string_index < utf32_string_size )
 	{
 		/* Convert the UTF-32 character bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32(
 		     &unicode_character,
@@ -651,15 +654,15 @@
 
 			return( -1 );
 		}
 		/* Determine how many UTF-32 character bytes are required
 		 */
 		if( libuna_unicode_character_size_to_utf32(
 		     unicode_character,
-		     utf32_stream_size,
+		     &safe_utf32_stream_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to determine size of Unicode character in UTF-32.",
@@ -670,15 +673,15 @@
 		if( unicode_character == 0 )
 		{
 			break;
 		}
 	}
 	/* Convert the number of characters into bytes
 	 */
-	*utf32_stream_size *= 4;
+	*utf32_stream_size = safe_utf32_stream_size * 4;
 
 	return( 1 );
 }
 
 /* Copies an UTF-32 stream from an UTF-32 string
  * Returns 1 if successful or -1 on error
  */
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1257.h` & `libfwsi-20230710/libuna/libuna_codepage_windows_1257.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1257 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_cyrillic.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCyrillic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_thai.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_thai.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacThai codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_utf32_string.c` & `libfwsi-20230710/libuna/libuna_utf32_string.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -1920,17 +1920,18 @@
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      size_t *utf32_string_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf32_string_size_from_utf16_stream";
-	size_t utf16_stream_index                    = 0;
 	libuna_unicode_character_t unicode_character = 0;
+	size_t utf16_stream_index                    = 0;
 	int read_byte_order                          = 0;
+	int result                                   = 0;
 
 	if( utf16_stream == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -1995,26 +1996,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf16_stream_index + 1 ) < utf16_stream_size )
 	{
 		/* Convert the UTF-16 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16_stream(
 		     &unicode_character,
 		     utf16_stream,
@@ -2030,18 +2019,29 @@
 			 "%s: unable to copy Unicode character from UTF-16 stream.",
 			 function );
 
 			return( -1 );
 		}
 		/* Determine how many UTF-8 character bytes are required
 		 */
-		if( libuna_unicode_character_size_to_utf32(
-		     unicode_character,
-		     utf32_string_size,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_size_to_utf32(
+			          unicode_character,
+			          utf32_string_size,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_size_to_ucs4(
+			          unicode_character,
+			          utf32_string_size,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_INPUT_FAILED,
 			 "%s: unable to unable to determine size of Unicode character in UTF-32.",
 			 function );
@@ -2106,17 +2106,18 @@
      size_t *utf32_string_index,
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf32_string_with_index_copy_from_utf16_stream";
-	size_t utf16_stream_index                    = 0;
 	libuna_unicode_character_t unicode_character = 0;
+	size_t utf16_stream_index                    = 0;
 	int read_byte_order                          = 0;
+	int result                                   = 0;
 
 	if( utf32_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -2198,26 +2199,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf16_stream_index + 1 ) < utf16_stream_size )
 	{
 		/* Convert the UTF-16 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16_stream(
 		     &unicode_character,
 		     utf16_stream,
@@ -2233,20 +2222,33 @@
 			 "%s: unable to copy Unicode character from UTF-16 stream.",
 			 function );
 
 			return( -1 );
 		}
 		/* Convert the Unicode character into UTF-32 character bytes
 		 */
-		if( libuna_unicode_character_copy_to_utf32(
-		     unicode_character,
-		     utf32_string,
-		     utf32_string_size,
-		     utf32_string_index,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_copy_to_utf32(
+			          unicode_character,
+			          utf32_string,
+			          utf32_string_size,
+			          utf32_string_index,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_copy_to_ucs4(
+			          unicode_character,
+			          utf32_string,
+			          utf32_string_size,
+			          utf32_string_index,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to copy Unicode character to UTF-32.",
 			 function );
@@ -2288,19 +2290,20 @@
      size_t utf32_string_size,
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                                     = "libuna_utf32_string_compare_with_utf16_stream";
+	libuna_unicode_character_t utf16_stream_unicode_character = 0;
+	libuna_unicode_character_t utf32_unicode_character        = 0;
 	size_t utf16_stream_index                                 = 0;
 	size_t utf32_string_index                                 = 0;
-	libuna_unicode_character_t utf32_unicode_character        = 0;
-	libuna_unicode_character_t utf16_stream_unicode_character = 0;
 	int read_byte_order                                       = 0;
+	int result                                                = 0;
 
 	if( utf32_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -2371,26 +2374,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	if( ( utf32_string_size >= 1 )
 	 && ( utf32_string[ utf32_string_size - 1 ] == 0 ) )
 	{
 		utf32_string_size -= 1;
 	}
 	/* Check if the UTF-16 stream is terminated with zero bytes
 	 */
@@ -2401,20 +2392,33 @@
 		utf16_stream_size -= 2;
 	}
 	while( ( utf32_string_index < utf32_string_size )
 	    && ( utf16_stream_index < utf16_stream_size ) )
 	{
 		/* Convert the UTF-32 character bytes into an Unicode character
 		 */
-		if( libuna_unicode_character_copy_from_utf32(
-		     &utf32_unicode_character,
-		     utf32_string,
-		     utf32_string_size,
-		     &utf32_string_index,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_copy_from_utf32(
+			          &utf32_unicode_character,
+			          utf32_string,
+			          utf32_string_size,
+			          &utf32_string_index,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_copy_from_ucs4(
+			          &utf32_unicode_character,
+			          utf32_string,
+			          utf32_string_size,
+			          &utf32_string_index,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to copy Unicode character from UTF-32.",
 			 function );
@@ -2548,26 +2552,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf32_stream_index + 1 ) < utf32_stream_size )
 	{
 		/* Convert the UTF-32 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32_stream(
 		     &unicode_character,
 		     utf32_stream,
@@ -2755,26 +2747,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf32_stream_index + 1 ) < utf32_stream_size )
 	{
 		/* Convert the UTF-32 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32_stream(
 		     &unicode_character,
 		     utf32_stream,
@@ -2932,26 +2912,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	if( ( utf32_string_size >= 1 )
 	 && ( utf32_string[ utf32_string_size - 1 ] == 0 ) )
 	{
 		utf32_string_size -= 1;
 	}
 	/* Check if the UTF-32 stream is terminated with zero bytes
 	 */
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_thai.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_thai.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacThai codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_874.c` & `libfwsi-20230710/libuna/libuna_codepage_windows_874.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 874 codepage (Thai) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1251.h` & `libfwsi-20230710/libuna/libuna_codepage_windows_1251.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1251 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_libcerror.h` & `libfwsi-20230710/libuna/libuna_libcerror.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_949.c` & `libfwsi-20230710/libuna/libuna_codepage_windows_949.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 949 codepage (Korean) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_6.h` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_5.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-6 codepage (Arabic) functions
+ * ISO 8859-5 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_6_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_6_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_5_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_6_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_5_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_6_unicode_to_byte_stream_base_0x0618[ 64 ];
+const uint8_t libuna_codepage_iso_8859_5_unicode_to_byte_stream_base_0x0400[ 96 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_6_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H ) */
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1256.h` & `libfwsi-20230710/libuna/libuna_codepage_windows_1256.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1256 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_greek.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_greek.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGreek codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_russian.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_roman.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacRussian codepage functions
+ * MacRoman codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_RUSSIAN_H )
-#define _LIBUNA_CODEPAGE_MAC_RUSSIAN_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_ROMAN_H )
+#define _LIBUNA_CODEPAGE_MAC_ROMAN_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_russian_copy_from_byte_stream(
+int libuna_codepage_mac_roman_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_russian_copy_to_byte_stream(
+int libuna_codepage_mac_roman_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_RUSSIAN_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMAN_H ) */
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_ukrainian.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacUkrainian codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_6.c` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_6.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-6 codepage (Arabic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_874.h` & `libfwsi-20230710/libuna/libuna_codepage_windows_874.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 874 codepage (Thai) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1251.c` & `libfwsi-20230710/libuna/libuna_codepage_windows_1251.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1251 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1256.c` & `libfwsi-20230710/libuna/libuna_codepage_windows_1256.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1256 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_base16_stream.h` & `libfwsi-20230710/libuna/libuna_base16_stream.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base16 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_2.h` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_2.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-2 codepage (Central European) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/Makefile.am` & `libfwsi-20230710/libuna/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1257.c` & `libfwsi-20230710/libuna/libuna_codepage_windows_1257.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1257 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1254.h` & `libfwsi-20230710/libuna/libuna_codepage_windows_1252.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1254 codepage (Turkish) functions
+ * Windows 1252 codepage (Western European/Latin 1) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1254_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1254_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1252_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1252_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1254_copy_from_byte_stream(
+int libuna_codepage_windows_1252_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1254_copy_to_byte_stream(
+int libuna_codepage_windows_1252_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1254_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1252_H ) */
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1255.c` & `libfwsi-20230710/libuna/libuna_codepage_windows_1255.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1255 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_unused.h` & `libfwsi-20230710/libuna/libuna_unused.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1253.h` & `libfwsi-20230710/libuna/libuna_codepage_windows_1253.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1253 codepage (Greek) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_unicode_character.h` & `libfwsi-20230710/libuna/libuna_unicode_character.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Unicode character functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -56,14 +56,58 @@
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      int codepage,
      libcerror_error_t **error );
 
 LIBUNA_EXTERN \
+int libuna_unicode_character_size_to_ucs2(
+     libuna_unicode_character_t unicode_character,
+     size_t *ucs2_character_size,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
+int libuna_unicode_character_copy_from_ucs2(
+     libuna_unicode_character_t *unicode_character,
+     const libuna_utf16_character_t *ucs2_string,
+     size_t ucs2_string_size,
+     size_t *ucs2_string_index,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
+int libuna_unicode_character_copy_to_ucs2(
+     libuna_unicode_character_t unicode_character,
+     libuna_utf16_character_t *ucs2_string,
+     size_t ucs2_string_size,
+     size_t *ucs2_string_index,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
+int libuna_unicode_character_size_to_ucs4(
+     libuna_unicode_character_t unicode_character,
+     size_t *ucs4_character_size,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
+int libuna_unicode_character_copy_from_ucs4(
+     libuna_unicode_character_t *unicode_character,
+     const libuna_utf32_character_t *ucs4_string,
+     size_t ucs4_string_size,
+     size_t *ucs4_string_index,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
+int libuna_unicode_character_copy_to_ucs4(
+     libuna_unicode_character_t unicode_character,
+     libuna_utf32_character_t *ucs4_string,
+     size_t ucs4_string_size,
+     size_t *ucs4_string_index,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
 int libuna_unicode_character_size_to_utf7_stream(
      libuna_unicode_character_t unicode_character,
      size_t *utf7_stream_character_size,
      uint32_t *utf7_stream_base64_data,
      libcerror_error_t **error );
 
 LIBUNA_EXTERN \
@@ -103,14 +147,36 @@
      libuna_unicode_character_t unicode_character,
      libuna_utf8_character_t *utf8_string,
      size_t utf8_string_size,
      size_t *utf8_string_index,
      libcerror_error_t **error );
 
 LIBUNA_EXTERN \
+int libuna_unicode_character_size_to_utf8_rfc2279(
+     libuna_unicode_character_t unicode_character,
+     size_t *utf8_character_size,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
+int libuna_unicode_character_copy_from_utf8_rfc2279(
+     libuna_unicode_character_t *unicode_character,
+     const libuna_utf8_character_t *utf8_string,
+     size_t utf8_string_size,
+     size_t *utf8_string_index,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
+int libuna_unicode_character_copy_to_utf8_rfc2279(
+     libuna_unicode_character_t unicode_character,
+     libuna_utf8_character_t *utf8_string,
+     size_t utf8_string_size,
+     size_t *utf8_string_index,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
 int libuna_unicode_character_size_to_utf16(
      libuna_unicode_character_t unicode_character,
      size_t *utf16_character_size,
      libcerror_error_t **error );
 
 LIBUNA_EXTERN \
 int libuna_unicode_character_copy_from_utf16(
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_dingbats.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_dingbats.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacDingbats codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_scsu.c` & `libfwsi-20230710/libuna/libuna_scsu.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Standard Compression Scheme for Unicode (SCSU) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_byte_stream.c` & `libfwsi-20230710/libuna/libuna_byte_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_celtic.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_celtic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCeltic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_croatian.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_croatian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCroatian codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_3.h` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_3.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-3 codepage (Latin 3) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_15.h` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_15.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-15 codepage (Latin 9) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_roman.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_roman.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRoman codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_utf32_string.h` & `libfwsi-20230710/libuna/libuna_utf32_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_koi8_r.c` & `libfwsi-20230710/libuna/libuna_codepage_koi8_r.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-R codepage (Russian Cyrillic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_icelandic.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_icelandic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacIcelandic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_936.h` & `libfwsi-20230710/libuna/libuna_codepage_windows_936.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 936 codepage (Chinese Simplified) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_base64_stream.h` & `libfwsi-20230710/libuna/libuna_base64_stream.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base64 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_celtic.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_celtic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCeltic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_950.c` & `libfwsi-20230710/libuna/libuna_codepage_windows_950.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 950 codepage (Traditional Chinese) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_utf8_string.h` & `libfwsi-20230710/libuna/libuna_utf8_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_936.c` & `libfwsi-20230710/libuna/libuna_codepage_windows_936.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 936 codepage (Chinese Simplified) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_unicode_character.c` & `libfwsi-20230710/libuna/libuna_unicode_character.c`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Unicode character functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -2142,14 +2142,497 @@
 		return( -1 );
 	}
 	*byte_stream_index = safe_byte_stream_index;
 
 	return( result );
 }
 
+/* Determines the size of an UCS-2 character from an Unicode character
+ * Adds the size to the UCS-2 character size value
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_size_to_ucs2(
+     libuna_unicode_character_t unicode_character,
+     size_t *ucs2_character_size,
+     libcerror_error_t **error )
+{
+	static char *function = "libuna_unicode_character_size_to_ucs2";
+
+	if( ucs2_character_size == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-2 character size.",
+		 function );
+
+		return( -1 );
+	}
+	/* Determine if the Unicode character is valid
+	 * UCS-2 with surrogate pairs supports upto 0x10ffff characters
+	 */
+	if( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	if( unicode_character > LIBUNA_UNICODE_BASIC_MULTILINGUAL_PLANE_MAX )
+	{
+		*ucs2_character_size += 2;
+	}
+	else
+	{
+		*ucs2_character_size += 1;
+	}
+	return( 1 );
+}
+
+/* Copies an Unicode character from an UCS-2 string
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_copy_from_ucs2(
+     libuna_unicode_character_t *unicode_character,
+     const libuna_utf16_character_t *ucs2_string,
+     size_t ucs2_string_size,
+     size_t *ucs2_string_index,
+     libcerror_error_t **error )
+{
+	static char *function                             = "libuna_unicode_character_copy_from_ucs2";
+	libuna_utf16_character_t ucs2_surrogate           = 0;
+	libuna_unicode_character_t safe_unicode_character = 0;
+	size_t safe_ucs2_string_index                     = 0;
+
+	if( unicode_character == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs2_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-2 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs2_string_size > (size_t) SSIZE_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid UCS-2 string size value exceeds maximum.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs2_string_index == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-2 string index.",
+		 function );
+
+		return( -1 );
+	}
+	safe_ucs2_string_index = *ucs2_string_index;
+
+	if( safe_ucs2_string_index >= ucs2_string_size )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: UCS-2 string too small.",
+		 function );
+
+		return( -1 );
+	}
+	safe_unicode_character  = ucs2_string[ safe_ucs2_string_index ];
+	safe_ucs2_string_index += 1;
+
+	/* Determine if the UCS-2 character is within the high surrogate range
+	 */
+	if( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	 && ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_END ) )
+	{
+		if( safe_ucs2_string_index >= ucs2_string_size )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
+			 "%s: missing surrogate UCS-2 character bytes.",
+			 function );
+
+			return( -1 );
+		}
+		ucs2_surrogate = ucs2_string[ safe_ucs2_string_index ];
+
+		/* Determine if the UCS-2 character is within the low surrogate range
+		 */
+		if( ( ucs2_surrogate >= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START )
+		 && ( ucs2_surrogate <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+		{
+			safe_unicode_character  -= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START;
+			safe_unicode_character <<= 10;
+			safe_unicode_character  += ucs2_surrogate - LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START;
+			safe_unicode_character  += 0x010000;
+
+			safe_ucs2_string_index += 1;
+		}
+	}
+	/* Determine if the Unicode character is valid
+	 * UCS-2 with surrogate pairs supports upto 0x10ffff characters
+	 */
+	if( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	*unicode_character = safe_unicode_character;
+	*ucs2_string_index = safe_ucs2_string_index;
+
+	return( 1 );
+}
+
+/* Copies an Unicode character into a UCS-2 string
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_copy_to_ucs2(
+     libuna_unicode_character_t unicode_character,
+     libuna_utf16_character_t *ucs2_string,
+     size_t ucs2_string_size,
+     size_t *ucs2_string_index,
+     libcerror_error_t **error )
+{
+	static char *function         = "libuna_unicode_character_copy_to_ucs2";
+	size_t safe_ucs2_string_index = 0;
+
+	if( ucs2_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-2 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs2_string_size > (size_t) SSIZE_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid UCS-2 string size value exceeds maximum.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs2_string_index == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-2 string index.",
+		 function );
+
+		return( -1 );
+	}
+	safe_ucs2_string_index = *ucs2_string_index;
+
+	if( safe_ucs2_string_index >= ucs2_string_size )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: UCS-2 string too small.",
+		 function );
+
+		return( -1 );
+	}
+	/* Determine if the Unicode character is valid
+	 */
+	if( unicode_character > LIBUNA_UCS_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	if( unicode_character <= LIBUNA_UNICODE_BASIC_MULTILINGUAL_PLANE_MAX )
+	{
+		ucs2_string[ safe_ucs2_string_index++ ] = (libuna_utf16_character_t) unicode_character;
+	}
+	else
+	{
+		if( ( ucs2_string_size < 2 )
+		 || ( safe_ucs2_string_index > ( ucs2_string_size - 2 ) ) )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+			 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+			 "%s: UCS-2 string too small.",
+			 function );
+
+			return( -1 );
+		}
+		unicode_character                      -= 0x010000;
+		ucs2_string[ safe_ucs2_string_index++ ] = (libuna_utf16_character_t) ( ( unicode_character >> 10 ) + LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START );
+		ucs2_string[ safe_ucs2_string_index++ ] = (libuna_utf16_character_t) ( ( unicode_character & 0x03ff ) + LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START );
+	}
+	*ucs2_string_index = safe_ucs2_string_index;
+
+	return( 1 );
+}
+
+/* Determines the size of an UCS-4 character from an Unicode character
+ * Adds the size to the UCS-4 character size value
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_size_to_ucs4(
+     libuna_unicode_character_t unicode_character,
+     size_t *ucs4_character_size,
+     libcerror_error_t **error )
+{
+	static char *function = "libuna_unicode_character_size_to_ucs4";
+
+	LIBUNA_UNREFERENCED_PARAMETER( unicode_character )
+
+	if( ucs4_character_size == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-4 character size.",
+		 function );
+
+		return( -1 );
+	}
+	if( unicode_character > LIBUNA_UCS_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	*ucs4_character_size += 1;
+
+	return( 1 );
+}
+
+/* Copies an Unicode character from an UCS-4 string
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_copy_from_ucs4(
+     libuna_unicode_character_t *unicode_character,
+     const libuna_utf32_character_t *ucs4_string,
+     size_t ucs4_string_size,
+     size_t *ucs4_string_index,
+     libcerror_error_t **error )
+{
+	static char *function                             = "libuna_unicode_character_copy_from_ucs4";
+	libuna_unicode_character_t safe_unicode_character = 0;
+	size_t safe_ucs4_string_index                     = 0;
+
+	if( unicode_character == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs4_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-4 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs4_string_size > (size_t) SSIZE_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid UCS-4 string size value exceeds maximum.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs4_string_index == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-4 string index.",
+		 function );
+
+		return( -1 );
+	}
+	safe_ucs4_string_index = *ucs4_string_index;
+
+	if( safe_ucs4_string_index >= ucs4_string_size )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: UCS-4 string too small.",
+		 function );
+
+		return( -1 );
+	}
+	safe_unicode_character = ucs4_string[ safe_ucs4_string_index ];
+
+	/* Determine if the Unicode character is valid
+	 */
+	if( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	*unicode_character = safe_unicode_character;
+	*ucs4_string_index = safe_ucs4_string_index + 1;
+
+	return( 1 );
+}
+
+/* Copies an Unicode character into a UCS-4 string
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_copy_to_ucs4(
+     libuna_unicode_character_t unicode_character,
+     libuna_utf32_character_t *ucs4_string,
+     size_t ucs4_string_size,
+     size_t *ucs4_string_index,
+     libcerror_error_t **error )
+{
+	static char *function         = "libuna_unicode_character_copy_to_ucs4";
+	size_t safe_ucs4_string_index = 0;
+
+	if( ucs4_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-4 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs4_string_size > (size_t) SSIZE_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid UCS-4 string size value exceeds maximum.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs4_string_index == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-4 string index.",
+		 function );
+
+		return( -1 );
+	}
+	safe_ucs4_string_index = *ucs4_string_index;
+
+	if( safe_ucs4_string_index >= ucs4_string_size )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: UCS-4 string too small.",
+		 function );
+
+		return( -1 );
+	}
+	/* Determine if the Unicode character is valid
+	 */
+	if( unicode_character > LIBUNA_UCS_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	ucs4_string[ safe_ucs4_string_index ] = (libuna_utf32_character_t) unicode_character;
+
+	*ucs4_string_index = safe_ucs4_string_index + 1;
+
+	return( 1 );
+}
+
 /* Determines the size of an UTF-7 stream character from an Unicode character
  * Adds the size to the UTF-7 stream character size value
  * Returns 1 if successful or -1 on error
  */
 int libuna_unicode_character_size_to_utf7_stream(
      libuna_unicode_character_t unicode_character,
      size_t *utf7_stream_character_size,
@@ -2189,17 +2672,26 @@
 		return( -1 );
 	}
 	safe_utf7_stream_character_size = *utf7_stream_character_size;
 	safe_utf7_stream_base64_data    = *utf7_stream_base64_data;
 
 	/* Determine if the Unicode character is valid
 	 */
-	if( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	/* The + character must be escaped
 	 */
 	if( unicode_character == (libuna_unicode_character_t) '+' )
 	{
 	}
 	/* Allow for the end of string character
@@ -2715,15 +3207,22 @@
 				safe_unicode_character  -= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START;
 				safe_unicode_character <<= 10;
 				safe_unicode_character  += utf16_surrogate - LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START;
 				safe_unicode_character  += 0x010000;
 			}
 			else
 			{
-				safe_unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+				 "%s: unsupported low surrogate UTF-16 character.",
+				 function );
+
+				return( -1 );
 			}
 		}
 		if( safe_utf7_stream_index >= utf7_stream_size )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -2829,17 +3328,26 @@
 		return( -1 );
 	}
 	safe_utf7_stream_index       = *utf7_stream_index;
 	safe_utf7_stream_base64_data = *utf7_stream_base64_data;
 
 	/* Determine if the Unicode character is valid
 	 */
-	if( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	/* A-Z is not a continous range on an EBCDIC based system
 	 * it consists of the ranges: A-I, J-R, S-Z
 	 */
 	if( ( unicode_character >= 0x41 )
 	 && ( unicode_character <= 0x49 ) )
 	{
@@ -3143,14 +3651,15 @@
 	*utf7_stream_index       = safe_utf7_stream_index;
 	*utf7_stream_base64_data = safe_utf7_stream_base64_data;
 
 	return( 1 );
 }
 
 /* Determines the size of an UTF-8 character from an Unicode character
+ * This function supports upto U+10FFFF (4 byte UTF-8 characters)
  * Adds the size to the UTF-8 character size value
  * Returns 1 if successful or -1 on error
  */
 int libuna_unicode_character_size_to_utf8(
      libuna_unicode_character_t unicode_character,
      size_t *utf8_character_size,
      libcerror_error_t **error )
@@ -3165,65 +3674,55 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid UTF-8 character size.",
 		 function );
 
 		return( -1 );
 	}
+	/* Determine if the Unicode character is valid
+	 */
+	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	/* RFC 3629 limits the UTF-8 character to consist of a maximum of 4 bytes
+	 * while its predecessor RFC 2279 allowed up to 6 bytes
+	 */
 	if( unicode_character < 0x00000080UL )
 	{
 		safe_utf8_character_size += 1;
 	}
 	else if( unicode_character < 0x00000800UL )
 	{
 		safe_utf8_character_size += 2;
 	}
 	else if( unicode_character < 0x00010000UL )
 	{
 		safe_utf8_character_size += 3;
 	}
-	else if( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
-	{
-		safe_utf8_character_size += 3;
-	}
 	else
 	{
 		safe_utf8_character_size += 4;
 	}
-
-/* If UTF-8 USC support is needed it should be implemented in
- * utf8_usc or something, but for now leave this here as a reminder
-
-	else if( unicode_character < 0x010000 )
-	{
-		safe_utf8_character_size += 3;
-	}
-	else if( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
-	{
-		safe_utf8_character_size += 2;
-	}
-	else if( unicode_character < 0x0200000 )
-	{
-		safe_utf8_character_size += 4;
-	}
-	else if( unicode_character < 0x0400000 )
-	{
-		safe_utf8_character_size += 5;
-	}
-	else
-	{
-		safe_utf8_character_size += 6;
-	}
-*/
 	*utf8_character_size += safe_utf8_character_size;
 
 	return( 1 );
 }
 
 /* Copies an Unicode character from an UTF-8 string
+ * This function supports upto U+10FFFF (4 byte UTF-8 characters)
  * Returns 1 if successful or -1 on error
  */
 int libuna_unicode_character_copy_from_utf8(
      libuna_unicode_character_t *unicode_character,
      const libuna_utf8_character_t *utf8_string,
      size_t utf8_string_size,
      size_t *utf8_string_index,
@@ -3232,16 +3731,16 @@
 	static char *function                             = "libuna_unicode_character_copy_from_utf8";
 	libuna_unicode_character_t safe_unicode_character = 0;
 	size_t safe_utf8_string_index                     = 0;
 	uint8_t byte_value1                               = 0;
 	uint8_t byte_value2                               = 0;
 	uint8_t byte_value3                               = 0;
 	uint8_t byte_value4                               = 0;
-	uint8_t byte_value5                               = 0;
 	uint8_t utf8_character_additional_bytes           = 0;
+	int result                                        = 0;
 
 	if( unicode_character == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -3296,72 +3795,63 @@
 
 		return( -1 );
 	}
 	/* Determine the number of additional bytes of the UTF-8 character
 	 */
 	byte_value1 = utf8_string[ safe_utf8_string_index ];
 
+	/* Determine the UTF-8 character and make sure it is valid
+	 * RFC 3629 limits the UTF-8 character to consist of a maximum of 4 bytes
+	 * while its predecessor RFC 2279 allowed up to 6 bytes
+	 */
+	if( byte_value1 > 0xf4 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid 1st UTF-8 character byte: 0x%02" PRIx8 ".",
+		 function,
+		 byte_value1 );
+
+		return( -1 );
+	}
 	if( byte_value1 < 0xc0 )
 	{
 		utf8_character_additional_bytes = 0;
 	}
 	else if( byte_value1 < 0xe0 )
 	{
 		utf8_character_additional_bytes = 1;
 	}
 	else if( byte_value1 < 0xf0 )
 	{
 		utf8_character_additional_bytes = 2;
 	}
-	else if( byte_value1 < 0xf8 )
-	{
-		utf8_character_additional_bytes = 3;
-	}
-	else if( byte_value1 < 0xfc )
-	{
-		utf8_character_additional_bytes = 4;
-	}
 	else
 	{
-		utf8_character_additional_bytes = 5;
+		utf8_character_additional_bytes = 3;
 	}
 	if( ( ( (size_t) utf8_character_additional_bytes + 1 ) > utf8_string_size )
 	 || ( safe_utf8_string_index > ( utf8_string_size - ( utf8_character_additional_bytes + 1 ) ) ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
 		 "%s: missing UTF-8 character bytes.",
 		 function );
 
 		return( -1 );
 	}
-	/* Determine the UTF-8 character and make sure it is valid
-	 * Unicode limits the UTF-8 character to consist of a maximum of 4 bytes
-	 * while ISO 10646 Universal Character Set (UCS) allows up to 6 bytes
-	 */
-	if( byte_value1 > 0xf4 )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid 1st UTF-8 character byte: 0x%02" PRIx8 ".",
-		 function,
-		 byte_value1 );
-
-		return( -1 );
-	}
 	safe_unicode_character = byte_value1;
 
 	if( utf8_character_additional_bytes == 0 )
 	{
-		if( ( byte_value1 >= 0x80 )
-		 && ( byte_value1 < 0xc2 ) )
+		if( byte_value1 >= 0x80 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
 			 "%s: invalid 1st UTF-8 character byte: 0x%02" PRIx8 ".",
 			 function,
@@ -3370,79 +3860,552 @@
 			return( -1 );
 		}
 	}
 	if( utf8_character_additional_bytes >= 1 )
 	{
 		byte_value2 = utf8_string[ safe_utf8_string_index + 1 ];
 
-		if( byte_value2 > 0xbf )
+		if( ( byte_value2 < 0x80 )
+		 || ( byte_value2 > 0xbf ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
 			 "%s: invalid 2nd UTF-8 character byte: 0x%02" PRIx8 ".",
 			 function,
 			 byte_value2 );
 
 			return( -1 );
 		}
-		if( ( byte_value1 == 0xe0 )
-		 && ( byte_value2 < 0xa0 ) )
+		result = 1;
+
+		switch( byte_value1 )
+		{
+			case 0xe0:
+				if( ( byte_value2 < 0xa0 )
+				 || ( byte_value2 > 0xbf ) )
+				{
+					result = 0;
+				}
+				break;
+
+			case 0xed:
+				if( ( byte_value2 < 0x80 )
+				 || ( byte_value2 > 0x9f ) )
+				{
+					result = 0;
+				}
+				break;
+
+			case 0xf0:
+				if( ( byte_value2 < 0x90 )
+				 || ( byte_value2 > 0xbf ) )
+				{
+					result = 0;
+				}
+				break;
+
+			case 0xf4:
+				if( ( byte_value2 < 0x80 )
+				 || ( byte_value2 > 0xbf ) )
+				{
+					result = 0;
+				}
+				break;
+
+			default:
+				break;
+		}
+		if( result == 0 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-			 "%s: invalid 2nd UTF-8 character byte: 0x%02" PRIx8 ".",
+			 "%s: invalid 1st and 2nd UTF-8 character byte pair: 0x%02" PRIx8 " 0x%02" PRIx8 ".",
 			 function,
+			 byte_value1,
 			 byte_value2 );
 
 			return( -1 );
 		}
-		else if( ( byte_value1 == 0xed )
-		      && ( byte_value2 > 0x9f ) )
+		safe_unicode_character <<= 6;
+		safe_unicode_character += byte_value2;
+
+		if( utf8_character_additional_bytes == 1 )
+		{
+			safe_unicode_character -= 0x03080;
+		}
+	}
+	if( utf8_character_additional_bytes >= 2 )
+	{
+		byte_value3 = utf8_string[ safe_utf8_string_index + 2 ];
+
+		if( ( byte_value3 < 0x80 )
+		 || ( byte_value3 > 0xbf ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-			 "%s: invalid 2nd UTF-8 character byte: 0x%02" PRIx8 ".",
+			 "%s: invalid 3rd UTF-8 character byte: 0x%02" PRIx8 ".",
 			 function,
-			 byte_value2 );
+			 byte_value3 );
 
 			return( -1 );
 		}
-		else if( ( byte_value1 == 0xf0 )
-		      && ( byte_value2 < 0x90 ) )
+		result = 1;
+
+		switch( byte_value2 )
+		{
+			case 0xe0:
+				if( ( byte_value2 < 0xa0 )
+				 || ( byte_value2 > 0xbf ) )
+				{
+					result = 0;
+				}
+				break;
+
+			case 0xed:
+				if( ( byte_value2 < 0x80 )
+				 || ( byte_value2 > 0x9f ) )
+				{
+					result = 0;
+				}
+				break;
+
+			default:
+				break;
+		}
+		if( result == 0 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-			 "%s: invalid 2nd UTF-8 character byte: 0x%02" PRIx8 ".",
+			 "%s: invalid 2nd and 3rd UTF-8 character byte pair: 0x%02" PRIx8 " 0x%02" PRIx8 ".",
 			 function,
-			 byte_value2 );
+			 byte_value2,
+			 byte_value3 );
 
 			return( -1 );
 		}
-		else if( ( byte_value1 == 0xf4 )
-		      && ( byte_value2 > 0x8f ) )
+		safe_unicode_character <<= 6;
+		safe_unicode_character += byte_value3;
+
+		if( utf8_character_additional_bytes == 2 )
+		{
+			safe_unicode_character -= 0x0e2080;
+		}
+	}
+	if( utf8_character_additional_bytes >= 3 )
+	{
+		byte_value4 = utf8_string[ safe_utf8_string_index + 3 ];
+
+		if( ( byte_value4 < 0x80 )
+		 || ( byte_value4 > 0xbf ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-			 "%s: invalid 2nd UTF-8 character byte: 0x%02" PRIx8 ".",
+			 "%s: invalid 4th UTF-8 character byte: 0x%02" PRIx8 ".",
 			 function,
-			 byte_value2 );
+			 byte_value4 );
 
 			return( -1 );
 		}
-		else if( byte_value2 < 0x80 )
+		safe_unicode_character <<= 6;
+		safe_unicode_character += byte_value4;
+
+		if( utf8_character_additional_bytes == 3 )
+		{
+			safe_unicode_character -= 0x03c82080;
+		}
+	}
+	/* Determine if the Unicode character is valid
+	 */
+	if( ( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	*unicode_character = safe_unicode_character;
+	*utf8_string_index = safe_utf8_string_index + 1 + utf8_character_additional_bytes;
+
+	return( 1 );
+}
+
+/* Copies an Unicode character into a UTF-8 string
+ * This function supports upto U+10FFFF (4 byte UTF-8 characters)
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_copy_to_utf8(
+     libuna_unicode_character_t unicode_character,
+     libuna_utf8_character_t *utf8_string,
+     size_t utf8_string_size,
+     size_t *utf8_string_index,
+     libcerror_error_t **error )
+{
+	static char *function                   = "libuna_unicode_character_copy_to_utf8";
+	size_t safe_utf8_string_index           = 0;
+	size_t utf8_character_iterator          = 0;
+	uint8_t utf8_character_additional_bytes = 0;
+	uint8_t utf8_first_character_mark       = 0;
+
+	if( utf8_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string_size > (size_t) SSIZE_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid UTF-8 string size value exceeds maximum.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string_index == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 string index.",
+		 function );
+
+		return( -1 );
+	}
+	safe_utf8_string_index = *utf8_string_index;
+
+	if( safe_utf8_string_index >= utf8_string_size )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: UTF-8 string too small.",
+		 function );
+
+		return( -1 );
+	}
+	/* Determine if the Unicode character is valid
+	 */
+	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	/* Determine how many UTF-8 character bytes are required
+	 */
+	if( unicode_character < 0x080 )
+	{
+		utf8_character_additional_bytes = 0;
+		utf8_first_character_mark       = 0;
+	}
+	else if( unicode_character < 0x0800 )
+	{
+		utf8_character_additional_bytes = 1;
+		utf8_first_character_mark       = 0x0c0;
+	}
+	else if( unicode_character < 0x010000 )
+	{
+		utf8_character_additional_bytes = 2;
+		utf8_first_character_mark       = 0x0e0;
+	}
+	else
+	{
+		utf8_character_additional_bytes = 3;
+		utf8_first_character_mark       = 0x0f0;
+	}
+	/* Convert Unicode character into UTF-8 character bytes
+	 */
+	if( ( utf8_character_additional_bytes > utf8_string_size )
+	 || ( safe_utf8_string_index >= ( utf8_string_size - utf8_character_additional_bytes ) ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: UTF-8 string too small.",
+		 function );
+
+		return( -1 );
+	}
+	for( utf8_character_iterator = safe_utf8_string_index + utf8_character_additional_bytes;
+	     utf8_character_iterator > safe_utf8_string_index;
+	     utf8_character_iterator-- )
+	{
+		utf8_string[ utf8_character_iterator ] = (libuna_utf8_character_t) ( ( unicode_character & 0x0bf ) | 0x080 );
+
+		unicode_character >>= 6;
+	}
+	utf8_string[ safe_utf8_string_index ] = (libuna_utf8_character_t) ( unicode_character | utf8_first_character_mark );
+
+	*utf8_string_index = safe_utf8_string_index + 1 + utf8_character_additional_bytes;
+
+	return( 1 );
+}
+
+/* Determines the size of an UTF-8 character from an Unicode character
+ * This function supports upto U+7FFFFFF (6 byte UTF-8 characters)
+ * Adds the size to the UTF-8 character size value
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_size_to_utf8_rfc2279(
+     libuna_unicode_character_t unicode_character,
+     size_t *utf8_character_size,
+     libcerror_error_t **error )
+{
+	static char *function           = "libuna_unicode_character_size_to_utf8_rfc2279";
+	size_t safe_utf8_character_size = 0;
+
+	if( utf8_character_size == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 character size.",
+		 function );
+
+		return( -1 );
+	}
+	if( unicode_character > LIBUNA_UCS_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	/* RFC 3629 limits the UTF-8 character to consist of a maximum of 4 bytes
+	 * while its predecessor RFC 2279 allowed up to 6 bytes
+	 */
+	if( unicode_character < 0x00000080UL )
+	{
+		safe_utf8_character_size += 1;
+	}
+	else if( unicode_character < 0x00000800UL )
+	{
+		safe_utf8_character_size += 2;
+	}
+	else if( unicode_character < 0x00010000UL )
+	{
+		safe_utf8_character_size += 3;
+	}
+	else if( unicode_character < 0x00200000UL )
+	{
+		safe_utf8_character_size += 4;
+	}
+	else if( unicode_character < 0x04000000UL )
+	{
+		safe_utf8_character_size += 5;
+	}
+	else
+	{
+		safe_utf8_character_size += 6;
+	}
+	*utf8_character_size += safe_utf8_character_size;
+
+	return( 1 );
+}
+
+/* Copies an Unicode character from an UTF-8 string
+ * This function supports upto U+7FFFFFF (6 byte UTF-8 characters)
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_copy_from_utf8_rfc2279(
+     libuna_unicode_character_t *unicode_character,
+     const libuna_utf8_character_t *utf8_string,
+     size_t utf8_string_size,
+     size_t *utf8_string_index,
+     libcerror_error_t **error )
+{
+	static char *function                             = "libuna_unicode_character_copy_from_utf8_rfc2279";
+	libuna_unicode_character_t safe_unicode_character = 0;
+	size_t safe_utf8_string_index                     = 0;
+	uint8_t byte_value1                               = 0;
+	uint8_t byte_value2                               = 0;
+	uint8_t byte_value3                               = 0;
+	uint8_t byte_value4                               = 0;
+	uint8_t byte_value5                               = 0;
+	uint8_t byte_value6                               = 0;
+	uint8_t utf8_character_additional_bytes           = 0;
+
+	if( unicode_character == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string_size > (size_t) SSIZE_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid UTF-8 string size value exceeds maximum.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string_index == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 string index.",
+		 function );
+
+		return( -1 );
+	}
+	safe_utf8_string_index = *utf8_string_index;
+
+	if( safe_utf8_string_index >= utf8_string_size )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: UTF-8 string too small.",
+		 function );
+
+		return( -1 );
+	}
+	/* Determine the number of additional bytes of the UTF-8 character
+	 */
+	byte_value1 = utf8_string[ safe_utf8_string_index ];
+
+	/* Determine the UTF-8 character and make sure it is valid
+	 * RFC 3629 limits the UTF-8 character to consist of a maximum of 4 bytes
+	 * while its predecessor RFC 2279 allowed up to 6 bytes
+	 */
+	if( byte_value1 > 0xfd )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid 1st UTF-8 character byte: 0x%02" PRIx8 ".",
+		 function,
+		 byte_value1 );
+
+		return( -1 );
+	}
+	if( byte_value1 < 0xc0 )
+	{
+		utf8_character_additional_bytes = 0;
+	}
+	else if( byte_value1 < 0xe0 )
+	{
+		utf8_character_additional_bytes = 1;
+	}
+	else if( byte_value1 < 0xf0 )
+	{
+		utf8_character_additional_bytes = 2;
+	}
+	else if( byte_value1 < 0xf8 )
+	{
+		utf8_character_additional_bytes = 3;
+	}
+	else if( byte_value1 < 0xfc )
+	{
+		utf8_character_additional_bytes = 4;
+	}
+	else
+	{
+		utf8_character_additional_bytes = 5;
+	}
+	if( ( ( (size_t) utf8_character_additional_bytes + 1 ) > utf8_string_size )
+	 || ( safe_utf8_string_index > ( utf8_string_size - ( utf8_character_additional_bytes + 1 ) ) ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: missing UTF-8 character bytes.",
+		 function );
+
+		return( -1 );
+	}
+	/* Determine the UTF-8 character and make sure it is valid
+	 * RFC 3629 limits the UTF-8 character to consist of a maximum of 4 bytes
+	 * while its predecessor RFC 2279 allowed up to 6 bytes
+	 */
+	safe_unicode_character = byte_value1;
+
+	if( utf8_character_additional_bytes == 0 )
+	{
+		if( byte_value1 >= 0x80 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
+			 "%s: invalid 1st UTF-8 character byte: 0x%02" PRIx8 ".",
+			 function,
+			 byte_value1 );
+
+			return( -1 );
+		}
+	}
+	if( utf8_character_additional_bytes >= 1 )
+	{
+		byte_value2 = utf8_string[ safe_utf8_string_index + 1 ];
+
+		if( ( byte_value2 < 0x80 )
+		 || ( byte_value2 > 0xbf ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
 			 "%s: invalid 2nd UTF-8 character byte: 0x%02" PRIx8 ".",
 			 function,
@@ -3531,54 +4494,64 @@
 		if( utf8_character_additional_bytes == 4 )
 		{
 			safe_unicode_character -= 0x0fa082080;
 		}
 	}
 	if( utf8_character_additional_bytes == 5 )
 	{
-		if( ( utf8_string[ safe_utf8_string_index + 5 ] < 0x80 )
-		  || ( utf8_string[ safe_utf8_string_index + 5 ] > 0xbf ) )
+		byte_value6 = utf8_string[ safe_utf8_string_index + 5 ];
+
+		if( ( byte_value6 < 0x80 )
+		  || ( byte_value6 > 0xbf ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
 			 "%s: invalid 6th UTF-8 character byte: 0x%02" PRIx8 ".",
 			 function,
-			 utf8_string[ safe_utf8_string_index + 5 ] );
+			 byte_value6 );
 
 			return( -1 );
 		}
 		safe_unicode_character <<= 6;
-		safe_unicode_character += utf8_string[ safe_utf8_string_index + 5 ];
+		safe_unicode_character += byte_value6;
 		safe_unicode_character -= 0x082082080;
 	}
 	/* Determine if the Unicode character is valid
 	 */
-	if( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	if( safe_unicode_character > LIBUNA_UCS_CHARACTER_MAX )
 	{
-		safe_unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	*unicode_character = safe_unicode_character;
 	*utf8_string_index = safe_utf8_string_index + 1 + utf8_character_additional_bytes;
 
 	return( 1 );
 }
 
 /* Copies an Unicode character into a UTF-8 string
+ * This function supports upto U+7FFFFFF (6 byte UTF-8 characters)
  * Returns 1 if successful or -1 on error
  */
-int libuna_unicode_character_copy_to_utf8(
+int libuna_unicode_character_copy_to_utf8_rfc2279(
      libuna_unicode_character_t unicode_character,
      libuna_utf8_character_t *utf8_string,
      size_t utf8_string_size,
      size_t *utf8_string_index,
      libcerror_error_t **error )
 {
-	static char *function                   = "libuna_unicode_character_copy_to_utf8";
+	static char *function                   = "libuna_unicode_character_copy_to_utf8_rfc2279";
 	size_t safe_utf8_string_index           = 0;
 	size_t utf8_character_iterator          = 0;
 	uint8_t utf8_character_additional_bytes = 0;
 	uint8_t utf8_first_character_mark       = 0;
 
 	if( utf8_string == NULL )
 	{
@@ -3624,17 +4597,24 @@
 		 "%s: UTF-8 string too small.",
 		 function );
 
 		return( -1 );
 	}
 	/* Determine if the Unicode character is valid
 	 */
-	if( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	if( unicode_character > LIBUNA_UCS_CHARACTER_MAX )
 	{
-		unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	/* Determine how many UTF-8 character bytes are required
 	 */
 	if( unicode_character < 0x080 )
 	{
 		utf8_character_additional_bytes = 0;
 		utf8_first_character_mark       = 0;
@@ -3711,16 +4691,28 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid UTF-16 character size.",
 		 function );
 
 		return( -1 );
 	}
-	if( ( unicode_character > LIBUNA_UNICODE_BASIC_MULTILINGUAL_PLANE_MAX )
-         && ( unicode_character <= LIBUNA_UTF16_CHARACTER_MAX ) )
+	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	if( unicode_character > LIBUNA_UNICODE_BASIC_MULTILINGUAL_PLANE_MAX )
 	{
 		*utf16_character_size += 2;
 	}
 	else
 	{
 		*utf16_character_size += 1;
 	}
@@ -3829,23 +4821,38 @@
 			safe_unicode_character  -= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START;
 			safe_unicode_character <<= 10;
 			safe_unicode_character  += utf16_surrogate - LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START;
 			safe_unicode_character  += 0x010000;
 		}
 		else
 		{
-			safe_unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+			 "%s: unsupported low surrogate UTF-16 character.",
+			 function );
+
+			return( -1 );
 		}
 	}
 	/* Determine if the Unicode character is valid
 	 */
-	else if( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START )
-	      && ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	if( ( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		safe_unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	*unicode_character  = safe_unicode_character;
 	*utf16_string_index = safe_utf16_string_index;
 
 	return( 1 );
 }
 
@@ -3907,18 +4914,25 @@
 		 function );
 
 		return( -1 );
 	}
 	/* Determine if the Unicode character is valid
 	 */
 	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
-	  && ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
-	 || ( unicode_character > LIBUNA_UTF16_CHARACTER_MAX ) )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	if( unicode_character <= LIBUNA_UNICODE_BASIC_MULTILINGUAL_PLANE_MAX )
 	{
 		utf16_string[ safe_utf16_string_index++ ] = (libuna_utf16_character_t) unicode_character;
 	}
 	else
 	{
@@ -3954,14 +4968,15 @@
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                             = "libuna_unicode_character_copy_from_utf16_stream";
 	libuna_unicode_character_t safe_unicode_character = 0;
 	libuna_utf16_character_t utf16_surrogate          = 0;
 	size_t safe_utf16_stream_index                    = 0;
+	int byte_order_without_flags                      = 0;
 
 	if( unicode_character == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -3999,16 +5014,18 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid UTF-16 stream index.",
 		 function );
 
 		return( -1 );
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
+	byte_order_without_flags = byte_order & 0xff;
+
+	if( ( byte_order_without_flags != LIBUNA_ENDIAN_BIG )
+	 && ( byte_order_without_flags != LIBUNA_ENDIAN_LITTLE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
 		 "%s: unsupported byte order.",
 		 function );
@@ -4025,90 +5042,113 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
 		 "%s: UTF-16 stream too small.",
 		 function );
 
 		return( -1 );
 	}
-	if( byte_order == LIBUNA_ENDIAN_BIG )
+	if( byte_order_without_flags == LIBUNA_ENDIAN_BIG )
 	{
 		safe_unicode_character   = utf16_stream[ safe_utf16_stream_index ];
 		safe_unicode_character <<= 8;
 		safe_unicode_character  += utf16_stream[ safe_utf16_stream_index + 1 ];
 	}
-	else if( byte_order == LIBUNA_ENDIAN_LITTLE )
+	else if( byte_order_without_flags == LIBUNA_ENDIAN_LITTLE )
 	{
 		safe_unicode_character   = utf16_stream[ safe_utf16_stream_index + 1 ];
 		safe_unicode_character <<= 8;
 		safe_unicode_character  += utf16_stream[ safe_utf16_stream_index ];
 	}
 	safe_utf16_stream_index += 2;
 
 	/* Determine if the Unicode character is valid
 	 */
 	if( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START )
 	 && ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
 	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported UTF-16 character.",
-		 function );
-
-		return( -1 );
-	}
-	/* Determine if the UTF-16 character is within the high surrogate range
-	 */
-	if( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
-	 && ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_END ) )
-	{
-		if( safe_utf16_stream_index > ( utf16_stream_size - 2 ) )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-			 "%s: missing surrogate UTF-16 character bytes.",
+			 "%s: unsupported UTF-16 character.",
 			 function );
 
 			return( -1 );
 		}
-		if( byte_order == LIBUNA_ENDIAN_BIG )
+	}
+	/* Determine if the UTF-16 character is within the high surrogate range
+	 */
+	if( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	 && ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_END ) )
+	{
+		if( safe_utf16_stream_index > ( utf16_stream_size - 2 ) )
 		{
-			utf16_surrogate   = utf16_stream[ safe_utf16_stream_index ];
-			utf16_surrogate <<= 8;
-			utf16_surrogate  += utf16_stream[ safe_utf16_stream_index + 1 ];
+			if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+				 "%s: missing surrogate UTF-16 character bytes.",
+				 function );
+
+				return( -1 );
+			}
 		}
-		else if( byte_order == LIBUNA_ENDIAN_LITTLE )
+		else
 		{
-			utf16_surrogate   = utf16_stream[ safe_utf16_stream_index + 1 ];
-			utf16_surrogate <<= 8;
-			utf16_surrogate  += utf16_stream[ safe_utf16_stream_index ];
-		}
-		safe_utf16_stream_index += 2;
+			if( byte_order_without_flags == LIBUNA_ENDIAN_BIG )
+			{
+				utf16_surrogate   = utf16_stream[ safe_utf16_stream_index ];
+				utf16_surrogate <<= 8;
+				utf16_surrogate  += utf16_stream[ safe_utf16_stream_index + 1 ];
+			}
+			else if( byte_order_without_flags == LIBUNA_ENDIAN_LITTLE )
+			{
+				utf16_surrogate   = utf16_stream[ safe_utf16_stream_index + 1 ];
+				utf16_surrogate <<= 8;
+				utf16_surrogate  += utf16_stream[ safe_utf16_stream_index ];
+			}
+			/* Determine if the UTF-16 character is within the low surrogate range
+			 */
+			if( ( utf16_surrogate >= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START )
+			 && ( utf16_surrogate <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+			{
+				safe_unicode_character  -= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START;
+				safe_unicode_character <<= 10;
+				safe_unicode_character  += utf16_surrogate - LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START;
+				safe_unicode_character  += 0x010000;
 
-		/* Determine if the UTF-16 character is within the low surrogate range
-		 */
-		if( ( utf16_surrogate < LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START )
-		 || ( utf16_surrogate > LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-			 "%s: unsupported low surrogate UTF-16 character.",
-			 function );
+				safe_utf16_stream_index += 2;
+			}
+			else if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+				 "%s: unsupported low surrogate UTF-16 character.",
+				 function );
 
-			return( -1 );
+				return( -1 );
+			}
 		}
-		safe_unicode_character  -= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START;
-		safe_unicode_character <<= 10;
-		safe_unicode_character  += utf16_surrogate - LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START;
-		safe_unicode_character  += 0x010000;
+	}
+	if( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	*unicode_character  = safe_unicode_character;
 	*utf16_stream_index = safe_utf16_stream_index;
 
 	return( 1 );
 }
 
@@ -4122,14 +5162,15 @@
      size_t *utf16_stream_index,
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                    = "libuna_unicode_character_copy_to_utf16_stream";
 	libuna_utf16_character_t utf16_surrogate = 0;
 	size_t safe_utf16_stream_index           = 0;
+	int byte_order_without_flags             = 0;
 
 	if( utf16_stream == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -4156,43 +5197,58 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid UTF-16 stream index.",
 		 function );
 
 		return( -1 );
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
+	byte_order_without_flags = byte_order & 0xff;
+
+	if( ( byte_order_without_flags != LIBUNA_ENDIAN_BIG )
+	 && ( byte_order_without_flags != LIBUNA_ENDIAN_LITTLE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
 		 "%s: unsupported byte order.",
 		 function );
 
 		return( -1 );
 	}
 	safe_utf16_stream_index = *utf16_stream_index;
 
 	/* Determine if the Unicode character is valid
 	 */
-	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
-	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
-	 || ( unicode_character > LIBUNA_UTF16_CHARACTER_MAX ) )
+	if( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
 		 "%s: unsupported Unicode character.",
 		 function );
 
 		return( -1 );
 	}
+	if( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	 && ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	{
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+			 "%s: unsupported Unicode character.",
+			 function );
+
+			return( -1 );
+		}
+	}
 	if( unicode_character <= LIBUNA_UNICODE_BASIC_MULTILINGUAL_PLANE_MAX )
 	{
 		if( ( utf16_stream_size < 2 )
 		 || ( safe_utf16_stream_index > ( utf16_stream_size - 2 ) ) )
 		{
 			libcerror_error_set(
 			 error,
@@ -4271,15 +5327,15 @@
 }
 
 /* Determines the size of an UTF-32 character from an Unicode character
  * Adds the size to the UTF-32 character size value
  * Returns 1 if successful or -1 on error
  */
 int libuna_unicode_character_size_to_utf32(
-     libuna_unicode_character_t unicode_character LIBUNA_ATTRIBUTE_UNUSED,
+     libuna_unicode_character_t unicode_character,
      size_t *utf32_character_size,
      libcerror_error_t **error )
 {
 	static char *function = "libuna_unicode_character_size_to_utf32";
 
 	LIBUNA_UNREFERENCED_PARAMETER( unicode_character )
 
@@ -4290,14 +5346,27 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid UTF-32 character size.",
 		 function );
 
 		return( -1 );
 	}
+	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
 	*utf32_character_size += 1;
 
 	return( 1 );
 }
 
 /* Copies an Unicode character from an UTF-32 string
  * Returns 1 if successful or -1 on error
@@ -4366,24 +5435,30 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
 		 "%s: UTF-32 string too small.",
 		 function );
 
 		return( -1 );
 	}
+	safe_unicode_character = utf32_string[ safe_utf32_string_index ];
+
 	/* Determine if the Unicode character is valid
 	 */
-	if( ( utf32_string[ safe_utf32_string_index ] >= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START )
-	 && ( utf32_string[ safe_utf32_string_index ] <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	if( ( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		safe_unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
-	}
-	else
-	{
-		safe_unicode_character = utf32_string[ safe_utf32_string_index ];
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	*unicode_character  = safe_unicode_character;
 	*utf32_string_index = safe_utf32_string_index + 1;
 
 	return( 1 );
 }
 
@@ -4445,23 +5520,28 @@
 		 function );
 
 		return( -1 );
 	}
 	/* Determine if the Unicode character is valid
 	 */
 	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
-	  && ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
-	 || ( unicode_character > LIBUNA_UTF32_CHARACTER_MAX ) )
-	{
-		utf32_string[ safe_utf32_string_index ] = (libuna_utf32_character_t) LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
-	}
-	else
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		utf32_string[ safe_utf32_string_index ] = (libuna_utf32_character_t) unicode_character;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
+	utf32_string[ safe_utf32_string_index ] = (libuna_utf32_character_t) unicode_character;
+
 	*utf32_string_index = safe_utf32_string_index + 1;
 
 	return( 1 );
 }
 
 /* Copies an Unicode character from an UTF-32 stream
  * Returns 1 if successful or -1 on error
@@ -4566,18 +5646,26 @@
 		safe_unicode_character <<= 8;
 		safe_unicode_character  += utf32_stream[ safe_utf32_stream_index + 1 ];
 		safe_unicode_character <<= 8;
 		safe_unicode_character  += utf32_stream[ safe_utf32_stream_index ];
 	}
 	/* Determine if the Unicode character is valid
 	 */
-	if( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START )
-	 && ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	if( ( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		safe_unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	*unicode_character  = safe_unicode_character;
 	*utf32_stream_index = safe_utf32_stream_index + 4;
 
 	return( 1 );
 }
 
@@ -4653,18 +5741,25 @@
 		 function );
 
 		return( -1 );
 	}
 	/* Determine if the Unicode character is valid
 	 */
 	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
-	  && ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
-	 || ( unicode_character > LIBUNA_UTF32_CHARACTER_MAX ) )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	if( byte_order == LIBUNA_ENDIAN_BIG )
 	{
 		utf32_stream[ safe_utf32_stream_index + 3 ] = (uint8_t) ( unicode_character & 0xff );
 		unicode_character                         >>= 8;
 		utf32_stream[ safe_utf32_stream_index + 2 ] = (uint8_t) ( unicode_character & 0xff );
 		unicode_character                         >>= 8;
```

### Comparing `libfwsi-20230114/libuna/libuna_utf8_string.c` & `libfwsi-20230710/libuna/libuna_utf8_string.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -1781,17 +1781,18 @@
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      size_t *utf8_string_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf8_string_size_from_utf16_stream";
-	size_t utf16_stream_index                    = 0;
 	libuna_unicode_character_t unicode_character = 0;
+	size_t utf16_stream_index                    = 0;
 	int read_byte_order                          = 0;
+	int result                                   = 0;
 
 	if( utf16_stream == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -1856,26 +1857,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf16_stream_index + 1 ) < utf16_stream_size )
 	{
 		/* Convert the UTF-16 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16_stream(
 		     &unicode_character,
 		     utf16_stream,
@@ -1891,18 +1880,29 @@
 			 "%s: unable to copy Unicode character from UTF-16 stream.",
 			 function );
 
 			return( -1 );
 		}
 		/* Determine how many UTF-8 character bytes are required
 		 */
-		if( libuna_unicode_character_size_to_utf8(
-		     unicode_character,
-		     utf8_string_size,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_size_to_utf8(
+			          unicode_character,
+			          utf8_string_size,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_size_to_utf8_rfc2279(
+			          unicode_character,
+			          utf8_string_size,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_INPUT_FAILED,
 			 "%s: unable to unable to determine size of Unicode character in UTF-8.",
 			 function );
@@ -1967,17 +1967,18 @@
      size_t *utf8_string_index,
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf8_string_with_index_copy_from_utf16_stream";
-	size_t utf16_stream_index                    = 0;
 	libuna_unicode_character_t unicode_character = 0;
+	size_t utf16_stream_index                    = 0;
 	int read_byte_order                          = 0;
+	int result                                   = 0;
 
 	if( utf8_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -2059,26 +2060,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf16_stream_index + 1 ) < utf16_stream_size )
 	{
 		/* Convert the UTF-16 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16_stream(
 		     &unicode_character,
 		     utf16_stream,
@@ -2094,20 +2083,33 @@
 			 "%s: unable to copy Unicode character from UTF-16 stream.",
 			 function );
 
 			return( -1 );
 		}
 		/* Convert the Unicode character into UTF-8 character bytes
 		 */
-		if( libuna_unicode_character_copy_to_utf8(
-		     unicode_character,
-		     utf8_string,
-		     utf8_string_size,
-		     utf8_string_index,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_copy_to_utf8(
+			          unicode_character,
+			          utf8_string,
+			          utf8_string_size,
+			          utf8_string_index,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_copy_to_utf8_rfc2279(
+			          unicode_character,
+			          utf8_string,
+			          utf8_string_size,
+			          utf8_string_index,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to copy Unicode character to UTF-8.",
 			 function );
@@ -2149,19 +2151,20 @@
      size_t utf8_string_size,
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                                     = "libuna_utf8_string_compare_with_utf16_stream";
+	libuna_unicode_character_t utf16_stream_unicode_character = 0;
+	libuna_unicode_character_t utf8_unicode_character         = 0;
 	size_t utf16_stream_index                                 = 0;
 	size_t utf8_string_index                                  = 0;
-	libuna_unicode_character_t utf8_unicode_character         = 0;
-	libuna_unicode_character_t utf16_stream_unicode_character = 0;
 	int read_byte_order                                       = 0;
+	int result                                                = 0;
 
 	if( utf8_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -2232,26 +2235,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	if( ( utf8_string_size >= 1 )
 	 && ( utf8_string[ utf8_string_size - 1 ] == 0 ) )
 	{
 		utf8_string_size -= 1;
 	}
 	/* Check if the UTF-16 stream is terminated with zero bytes
 	 */
@@ -2262,20 +2253,33 @@
 		utf16_stream_size -= 2;
 	}
 	while( ( utf8_string_index < utf8_string_size )
 	    && ( utf16_stream_index < utf16_stream_size ) )
 	{
 		/* Convert the UTF-8 character bytes into an Unicode character
 		 */
-		if( libuna_unicode_character_copy_from_utf8(
-		     &utf8_unicode_character,
-		     utf8_string,
-		     utf8_string_size,
-		     &utf8_string_index,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_copy_from_utf8(
+			          &utf8_unicode_character,
+			          utf8_string,
+			          utf8_string_size,
+			          &utf8_string_index,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_copy_from_utf8_rfc2279(
+			          &utf8_unicode_character,
+			          utf8_string,
+			          utf8_string_size,
+			          &utf8_string_index,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to copy Unicode character from UTF-8.",
 			 function );
@@ -2832,26 +2836,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf32_stream_index + 3 ) < utf32_stream_size )
 	{
 		/* Convert the UTF-32 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32_stream(
 		     &unicode_character,
 		     utf32_stream,
@@ -3039,26 +3031,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf32_stream_index + 3 ) < utf32_stream_size )
 	{
 		/* Convert the UTF-32 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32_stream(
 		     &unicode_character,
 		     utf32_stream,
@@ -3216,26 +3196,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	if( ( utf8_string_size >= 1 )
 	 && ( utf8_string[ utf8_string_size - 1 ] == 0 ) )
 	{
 		utf8_string_size -= 1;
 	}
 	/* Check if the UTF-32 stream is terminated with zero bytes
 	 */
```

### Comparing `libfwsi-20230114/libuna/libuna_base32_stream.c` & `libfwsi-20230710/libuna/libuna_base32_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base32 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_950.h` & `libfwsi-20230710/libuna/libuna_codepage_windows_950.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 950 codepage (Traditional Chinese) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_error.h` & `libfwsi-20230710/libuna/libuna_error.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_932.h` & `libfwsi-20230710/libuna/libuna_codepage_windows_932.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 932 codepage (Japanese Shift-JIS) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_turkish.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_turkish.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacTurkish codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_utf8_stream.c` & `libfwsi-20230710/libuna/libuna_utf8_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_ukrainian.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacUkrainian codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_koi8_r.h` & `libfwsi-20230710/libuna/libuna_codepage_koi8_r.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-R codepage (Russian Cyrillic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_base16_stream.c` & `libfwsi-20230710/libuna/libuna_base16_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base16 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1250.h` & `libfwsi-20230710/libuna/libuna_codepage_windows_1250.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1250 codepage (Central European) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_16.h` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_16.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-16 codepage (Latin 10) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_croatian.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_croatian.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCroatian codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_gaelic.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_gaelic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGaelic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_utf16_stream.h` & `libfwsi-20230710/libuna/libuna_utf16_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_10.h` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_7.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-10 codepage (Nordic) functions
+ * ISO 8859-7 codepage (Greek) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,34 +15,34 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_10_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_10_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_7_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_7_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_10_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_7_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_10_unicode_to_byte_stream_base_0x00c0[ 144 ];
+const uint8_t libuna_codepage_iso_8859_7_unicode_to_byte_stream_base_0x00a0[ 24 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_10_unicode_to_byte_stream_base_0x0160[ 16 ];
+const uint8_t libuna_codepage_iso_8859_7_unicode_to_byte_stream_base_0x0380[ 80 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_10_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_7_H ) */
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_centraleurroman.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCentralEurRoman codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_932.c` & `libfwsi-20230710/libuna/libuna_codepage_windows_932.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 932 codepage (Japanese Shift-JIS) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_utf8_stream.h` & `libfwsi-20230710/libuna/libuna_utf8_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_url_stream.h` & `libfwsi-20230710/libuna/libuna_url_stream.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Percent or URL encoded stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_farsi.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_farsi.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacFarsi codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_949.h` & `libfwsi-20230710/libuna/libuna_codepage_windows_949.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 949 codepage (Korean) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_romanian.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_romanian.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRomanian codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_gaelic.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_gaelic.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGaelic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_8.c` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_8.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-8 codepage (Hebrew) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_types.h` & `libfwsi-20230710/libuna/libuna_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_arabic.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_arabic.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacArabic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1252.h` & `libfwsi-20230710/libuna/libuna_codepage_windows_1258.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1252 codepage (Western European/Latin 1) functions
+ * Windows 1258 codepage (Vietnamese) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1252_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1252_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1258_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1258_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1252_copy_from_byte_stream(
+int libuna_codepage_windows_1258_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1252_copy_to_byte_stream(
+int libuna_codepage_windows_1258_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1252_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1258_H ) */
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1250.c` & `libfwsi-20230710/libuna/libuna_codepage_windows_1250.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1250 codepage (Central European) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_russian.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_russian.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRussian codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_utf16_string.c` & `libfwsi-20230710/libuna/libuna_utf16_string.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -1639,17 +1639,18 @@
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      size_t *utf16_string_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf16_string_size_from_utf16_stream";
-	size_t utf16_stream_index                    = 0;
 	libuna_unicode_character_t unicode_character = 0;
+	size_t utf16_stream_index                    = 0;
 	int read_byte_order                          = 0;
+	int result                                   = 0;
 
 	if( utf16_stream == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -1714,26 +1715,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf16_stream_index + 1 ) < utf16_stream_size )
 	{
 		/* Convert the UTF-16 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16_stream(
 		     &unicode_character,
 		     utf16_stream,
@@ -1749,18 +1738,29 @@
 			 "%s: unable to copy Unicode character from UTF-16 stream.",
 			 function );
 
 			return( -1 );
 		}
 		/* Determine how many UTF-16 character bytes are required
 		 */
-		if( libuna_unicode_character_size_to_utf16(
-		     unicode_character,
-		     utf16_string_size,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_size_to_utf16(
+			          unicode_character,
+			          utf16_string_size,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_size_to_ucs2(
+			          unicode_character,
+			          utf16_string_size,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_INPUT_FAILED,
 			 "%s: unable to unable to determine size of Unicode character in UTF-16.",
 			 function );
@@ -1825,17 +1825,18 @@
      size_t *utf16_string_index,
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf16_string_with_index_copy_from_utf16_stream";
-	size_t utf16_stream_index                    = 0;
 	libuna_unicode_character_t unicode_character = 0;
+	size_t utf16_stream_index                    = 0;
 	int read_byte_order                          = 0;
+	int result                                   = 0;
 
 	if( utf16_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -1917,26 +1918,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf16_stream_index + 1 ) < utf16_stream_size )
 	{
 		/* Convert the UTF-16 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16_stream(
 		     &unicode_character,
 		     utf16_stream,
@@ -1952,20 +1941,33 @@
 			 "%s: unable to copy Unicode character from UTF-16 stream.",
 			 function );
 
 			return( -1 );
 		}
 		/* Convert the Unicode character into UTF-16 character bytes
 		 */
-		if( libuna_unicode_character_copy_to_utf16(
-		     unicode_character,
-		     utf16_string,
-		     utf16_string_size,
-		     utf16_string_index,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_copy_to_utf16(
+			          unicode_character,
+			          utf16_string,
+			          utf16_string_size,
+			          utf16_string_index,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_copy_to_ucs2(
+			          unicode_character,
+			          utf16_string,
+			          utf16_string_size,
+			          utf16_string_index,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to copy Unicode character to UTF-16.",
 			 function );
@@ -2007,19 +2009,20 @@
      size_t utf16_string_size,
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                                     = "libuna_utf16_string_compare_with_utf16_stream";
+	libuna_unicode_character_t utf16_stream_unicode_character = 0;
+	libuna_unicode_character_t utf16_unicode_character        = 0;
 	size_t utf16_stream_index                                 = 0;
 	size_t utf16_string_index                                 = 0;
-	libuna_unicode_character_t utf16_unicode_character        = 0;
-	libuna_unicode_character_t utf16_stream_unicode_character = 0;
 	int read_byte_order                                       = 0;
+	int result                                                = 0;
 
 	if( utf16_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -2090,26 +2093,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	if( ( utf16_string_size >= 1 )
 	 && ( utf16_string[ utf16_string_size - 1 ] == 0 ) )
 	{
 		utf16_string_size -= 1;
 	}
 	/* Check if the UTF-16 stream is terminated with zero bytes
 	 */
@@ -2120,20 +2111,33 @@
 		utf16_stream_size -= 2;
 	}
 	while( ( utf16_string_index < utf16_string_size )
 	    && ( utf16_stream_index < utf16_stream_size ) )
 	{
 		/* Convert the UTF-16 character bytes into an Unicode character
 		 */
-		if( libuna_unicode_character_copy_from_utf16(
-		     &utf16_unicode_character,
-		     utf16_string,
-		     utf16_string_size,
-		     &utf16_string_index,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_copy_from_utf16(
+			          &utf16_unicode_character,
+			          utf16_string,
+			          utf16_string_size,
+			          &utf16_string_index,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_copy_from_ucs2(
+			          &utf16_unicode_character,
+			          utf16_string,
+			          utf16_string_size,
+			          &utf16_string_index,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to copy Unicode character from UTF-16.",
 			 function );
@@ -2690,26 +2694,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf32_stream_index + 3 ) < utf32_stream_size )
 	{
 		/* Convert the UTF-32 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32_stream(
 		     &unicode_character,
 		     utf32_stream,
@@ -2897,26 +2889,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf32_stream_index + 3 ) < utf32_stream_size )
 	{
 		/* Convert the UTF-32 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32_stream(
 		     &unicode_character,
 		     utf32_stream,
@@ -3074,26 +3054,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	if( ( utf16_string_size >= 1 )
 	 && ( utf16_string[ utf16_string_size - 1 ] == 0 ) )
 	{
 		utf16_string_size -= 1;
 	}
 	/* Check if the UTF-32 stream is terminated with zero bytes
 	 */
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_5.h` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_9.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-5 codepage (Cyrillic) functions
+ * ISO 8859-9 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_5_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_9_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_5_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_9_byte_stream_to_unicode_base_0xd0[ 48 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_5_unicode_to_byte_stream_base_0x0400[ 96 ];
+const uint8_t libuna_codepage_iso_8859_9_unicode_to_byte_stream_base_0x00d0[ 48 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H ) */
```

### Comparing `libfwsi-20230114/libuna/libuna_extern.h` & `libfwsi-20230710/libuna/libuna_extern.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_4.h` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_4.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-4 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_byte_stream.h` & `libfwsi-20230710/libuna/libuna_byte_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_roman.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacRoman codepage functions
+ * MacCentralEurRoman codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_ROMAN_H )
-#define _LIBUNA_CODEPAGE_MAC_ROMAN_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_CENTRALEURROMAN_H )
+#define _LIBUNA_CODEPAGE_MAC_CENTRALEURROMAN_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_roman_copy_from_byte_stream(
+int libuna_codepage_mac_centraleurroman_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_roman_copy_to_byte_stream(
+int libuna_codepage_mac_centraleurroman_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMAN_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_CENTRALEURROMAN_H ) */
```

### Comparing `libfwsi-20230114/libuna/libuna_utf16_string.h` & `libfwsi-20230710/libuna/libuna_utf16_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_4.c` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_4.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-4 codepage (Baltic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_10.c` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_10.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-10 codepage (Nordic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_icelandic.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_icelandic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacIcelandic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/Makefile.in` & `libfwsi-20230710/libuna/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libuna/libuna_utf7_stream.h` & `libfwsi-20230710/libuna/libuna_utf7_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-7 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_symbol.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_symbol.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacSymbol codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_base32_stream.h` & `libfwsi-20230710/libuna/libuna_base32_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base32 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_turkish.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_turkish.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacTurkish codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_inuit.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_inuit.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacInuit codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_utf16_stream.c` & `libfwsi-20230710/libuna/libuna_utf16_stream.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -118,14 +118,15 @@
      const libuna_utf8_character_t *utf8_string,
      size_t utf8_string_size,
      size_t *utf16_stream_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf16_stream_size_from_utf8";
 	libuna_unicode_character_t unicode_character = 0;
+	size_t safe_utf16_stream_size                = 0;
 	size_t utf8_string_index                     = 0;
 
 	if( utf8_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -155,15 +156,15 @@
 		 "%s: invalid UTF-16 stream size.",
 		 function );
 
 		return( -1 );
 	}
 	/* Add the byte order mark
 	 */
-	*utf16_stream_size = 1;
+	safe_utf16_stream_size = 1;
 
 	while( utf8_string_index < utf8_string_size )
 	{
 		/* Convert the UTF-8 character bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf8(
 		     &unicode_character,
@@ -181,15 +182,15 @@
 
 			return( -1 );
 		}
 		/* Determine how many UTF-16 character bytes are required
 		 */
 		if( libuna_unicode_character_size_to_utf16(
 		     unicode_character,
-		     utf16_stream_size,
+		     &safe_utf16_stream_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to determine size of Unicode character in UTF-16.",
@@ -200,15 +201,15 @@
 		if( unicode_character == 0 )
 		{
 			break;
 		}
 	}
 	/* Convert the number of characters into bytes
 	 */
-	*utf16_stream_size *= 2;
+	*utf16_stream_size = safe_utf16_stream_size * 2;
 
 	return( 1 );
 }
 
 /* Copies an UTF-16 stream from an UTF-8 string
  * Returns 1 if successful or -1 on error
  */
@@ -351,14 +352,15 @@
      const libuna_utf16_character_t *utf16_string,
      size_t utf16_string_size,
      size_t *utf16_stream_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf16_stream_size_from_utf16";
 	libuna_unicode_character_t unicode_character = 0;
+	size_t safe_utf16_stream_size                = 0;
 	size_t utf16_string_index                    = 0;
 
 	if( utf16_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -388,15 +390,15 @@
 		 "%s: invalid UTF-16 stream size.",
 		 function );
 
 		return( -1 );
 	}
 	/* Add the byte order mark
 	 */
-	*utf16_stream_size = 1;
+	safe_utf16_stream_size = 1;
 
 	while( utf16_string_index < utf16_string_size )
 	{
 		/* Convert the UTF-16 character bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16(
 		     &unicode_character,
@@ -414,15 +416,15 @@
 
 			return( -1 );
 		}
 		/* Determine how many UTF-16 character bytes are required
 		 */
 		if( libuna_unicode_character_size_to_utf16(
 		     unicode_character,
-		     utf16_stream_size,
+		     &safe_utf16_stream_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to determine size of Unicode character in UTF-16.",
@@ -433,15 +435,15 @@
 		if( unicode_character == 0 )
 		{
 			break;
 		}
 	}
 	/* Convert the number of characters into bytes
 	 */
-	*utf16_stream_size *= 2;
+	*utf16_stream_size = safe_utf16_stream_size * 2;
 
 	return( 1 );
 }
 
 /* Copies an UTF-16 stream from an UTF-16 string
  * Returns 1 if successful or -1 on error
  */
@@ -584,14 +586,15 @@
      const libuna_utf32_character_t *utf32_string,
      size_t utf32_string_size,
      size_t *utf16_stream_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf16_stream_size_from_utf32";
 	libuna_unicode_character_t unicode_character = 0;
+	size_t safe_utf16_stream_size                = 0;
 	size_t utf32_string_index                    = 0;
 
 	if( utf32_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -621,15 +624,15 @@
 		 "%s: invalid UTF-16 stream size.",
 		 function );
 
 		return( -1 );
 	}
 	/* Add the byte order mark
 	 */
-	*utf16_stream_size += 1;
+	safe_utf16_stream_size += 1;
 
 	while( utf32_string_index < utf32_string_size )
 	{
 		/* Convert the UTF-32 character bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32(
 		     &unicode_character,
@@ -647,15 +650,15 @@
 
 			return( -1 );
 		}
 		/* Determine how many UTF-16 character bytes are required
 		 */
 		if( libuna_unicode_character_size_to_utf16(
 		     unicode_character,
-		     utf16_stream_size,
+		     &safe_utf16_stream_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to determine size of Unicode character in UTF-16.",
@@ -666,15 +669,15 @@
 		if( unicode_character == 0 )
 		{
 			break;
 		}
 	}
 	/* Convert the number of characters into bytes
 	 */
-	*utf16_stream_size *= 2;
+	*utf16_stream_size = safe_utf16_stream_size * 2;
 
 	return( 1 );
 }
 
 /* Copies an UTF-16 stream from an UTF-32 string
  * Returns 1 if successful or -1 on error
  */
```

### Comparing `libfwsi-20230114/libuna/libuna_utf7_stream.c` & `libfwsi-20230710/libuna/libuna_utf7_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-7 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_support.h` & `libfwsi-20230710/libuna/libuna_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_utf32_stream.h` & `libfwsi-20230710/libuna/libuna_utf32_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_3.c` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_3.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-3 codepage (Latin 3) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_greek.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_greek.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGreek codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_definitions.h` & `libfwsi-20230710/libuna/libuna_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20220611
+#define LIBUNA_VERSION						20230710
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20220611"
+#define LIBUNA_VERSION_STRING					"20230710"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
@@ -384,14 +384,16 @@
 /* Base64 processing flags
  */
 enum LIBUNA_BASE64_FLAGS
 {
 	LIBUNA_BASE64_FLAG_STRIP_WHITESPACE			= 0x01
 };
 
+#define LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE		0x8000
+
 #endif /* !defined( HAVE_LOCAL_LIBUNA ) */
 
 #define LIBUNA_BASE32_VARIANT_ENCODING_BYTE_STREAM		0
 #define LIBUNA_BASE64_VARIANT_ENCODING_BYTE_STREAM		0
 
 /* Character case definitions
  */
@@ -418,16 +420,15 @@
 #define LIBUNA_UNICODE_BASIC_MULTILINGUAL_PLANE_MAX		0x0000ffffUL
 #define LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START		0x0000dc00UL
 #define LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END			0x0000dfffUL
 #define LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START		0x0000d800UL
 #define LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_END			0x0000dbffUL
 #define LIBUNA_UNICODE_CHARACTER_MAX				0x0010ffffUL
 
-#define LIBUNA_UTF16_CHARACTER_MAX				0x0010ffffUL
-#define LIBUNA_UTF32_CHARACTER_MAX				0x7fffffffUL
+#define LIBUNA_UCS_CHARACTER_MAX				0x7fffffffUL
 
 #define LIBUNA_ASCII_REPLACEMENT_CHARACTER			0x1a
 
 /* UTF-7 definitions
  */
 #define	LIBUNA_UTF7_IS_BASE64_ENCODED				0x80000000UL
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1255.h` & `libfwsi-20230710/libuna/libuna_codepage_windows_1255.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1255 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_14.c` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_14.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-14 codepage (Celtic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_13.c` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_13.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-13 codepage (Baltic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_centraleurroman.h` & `libfwsi-20230710/libuna/libuna_codepage_windows_1254.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacCentralEurRoman codepage functions
+ * Windows 1254 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_CENTRALEURROMAN_H )
-#define _LIBUNA_CODEPAGE_MAC_CENTRALEURROMAN_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1254_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1254_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_centraleurroman_copy_from_byte_stream(
+int libuna_codepage_windows_1254_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_centraleurroman_copy_to_byte_stream(
+int libuna_codepage_windows_1254_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_CENTRALEURROMAN_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1254_H ) */
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_8.h` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_8.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-8 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_9.c` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_9.c`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-9 codepage (Turkish) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1254.c` & `libfwsi-20230710/libuna/libuna_codepage_windows_1254.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1254 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_cyrillic.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCyrillic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_arabic.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_arabic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacArabic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1258.c` & `libfwsi-20230710/libuna/libuna_codepage_windows_1258.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1258 codepage (Vietnamese) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_farsi.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_farsi.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacFarsi codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_15.c` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_15.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-15 codepage (Latin 9) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_7.c` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_7.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-7 codepage (Greek) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_dingbats.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_dingbats.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacDingbats codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_9.h` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_6.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-9 codepage (Turkish) functions
+ * ISO 8859-6 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_9_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_6_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_6_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_9_byte_stream_to_unicode_base_0xd0[ 48 ];
+const uint16_t libuna_codepage_iso_8859_6_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_9_unicode_to_byte_stream_base_0x00d0[ 48 ];
+const uint8_t libuna_codepage_iso_8859_6_unicode_to_byte_stream_base_0x0618[ 64 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_6_H ) */
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_windows_1258.h` & `libfwsi-20230710/libuna/libuna_codepage_mac_inuit.h`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1258 codepage (Vietnamese) functions
+ * MacInuit codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1258_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1258_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H )
+#define _LIBUNA_CODEPAGE_MAC_INUIT_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1258_copy_from_byte_stream(
+int libuna_codepage_mac_inuit_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1258_copy_to_byte_stream(
+int libuna_codepage_mac_inuit_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1258_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H ) */
```

### Comparing `libfwsi-20230114/libuna/libuna_base64_stream.c` & `libfwsi-20230710/libuna/libuna_base64_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base64 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_romanian.c` & `libfwsi-20230710/libuna/libuna_codepage_mac_romanian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRomanian codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_error.c` & `libfwsi-20230710/libuna/libuna_error.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_koi8_u.c` & `libfwsi-20230710/libuna/libuna_codepage_koi8_u.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-U codepage (Ukrainian Cyrillic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_13.h` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_10.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-13 codepage (Baltic) functions
+ * ISO 8859-10 codepage (Nordic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,34 +15,34 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_13_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_13_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_10_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_10_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_13_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_10_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_13_unicode_to_byte_stream_base_0x00a0[ 224 ];
+const uint8_t libuna_codepage_iso_8859_10_unicode_to_byte_stream_base_0x00c0[ 144 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_13_unicode_to_byte_stream_base_0x2018[ 8 ];
+const uint8_t libuna_codepage_iso_8859_10_unicode_to_byte_stream_base_0x0160[ 16 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_13_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_10_H ) */
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_7.h` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_14.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-7 codepage (Greek) functions
+ * ISO 8859-14 codepage (Celtic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,34 +15,37 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_7_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_7_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_14_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_14_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_7_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_14_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_7_unicode_to_byte_stream_base_0x00a0[ 24 ];
+const uint8_t libuna_codepage_iso_8859_14_unicode_to_byte_stream_base_0x00c0[ 64 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_7_unicode_to_byte_stream_base_0x0380[ 80 ];
+const uint8_t libuna_codepage_iso_8859_14_unicode_to_byte_stream_base_0x0170[ 8 ];
+
+LIBUNA_EXTERN_VARIABLE \
+const uint8_t libuna_codepage_iso_8859_14_unicode_to_byte_stream_base_0x1e80[ 8 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_7_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_14_H ) */
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_14.h` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_13.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-14 codepage (Celtic) functions
+ * ISO 8859-13 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,37 +15,34 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_14_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_14_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_13_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_13_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_14_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_13_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_14_unicode_to_byte_stream_base_0x00c0[ 64 ];
+const uint8_t libuna_codepage_iso_8859_13_unicode_to_byte_stream_base_0x00a0[ 224 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_14_unicode_to_byte_stream_base_0x0170[ 8 ];
-
-LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_14_unicode_to_byte_stream_base_0x1e80[ 8 ];
+const uint8_t libuna_codepage_iso_8859_13_unicode_to_byte_stream_base_0x2018[ 8 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_14_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_13_H ) */
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_mac_inuit.h` & `libfwsi-20230710/libcnotify/libcnotify_support.c`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * MacInuit codepage functions
+ * Support functions
  *
  * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
@@ -15,40 +15,25 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H )
-#define _LIBUNA_CODEPAGE_MAC_INUIT_H
-
 #include <common.h>
 #include <types.h>
 
-#include "libuna_libcerror.h"
-#include "libuna_types.h"
+#include "libcnotify_definitions.h"
+#include "libcnotify_support.h"
 
-#if defined( __cplusplus )
-extern "C" {
-#endif
-
-int libuna_codepage_mac_inuit_copy_from_byte_stream(
-     libuna_unicode_character_t *unicode_character,
-     const uint8_t *byte_stream,
-     size_t byte_stream_size,
-     size_t *byte_stream_index,
-     libcerror_error_t **error );
-
-int libuna_codepage_mac_inuit_copy_to_byte_stream(
-     libuna_unicode_character_t unicode_character,
-     uint8_t *byte_stream,
-     size_t byte_stream_size,
-     size_t *byte_stream_index,
-     libcerror_error_t **error );
+#if !defined( HAVE_LOCAL_LIBCNOTIFY )
 
-#if defined( __cplusplus )
+/* Returns the library version as a string
+ */
+const char *libcnotify_get_version(
+             void )
+{
+	return( (const char *) LIBCNOTIFY_VERSION_STRING );
 }
-#endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H ) */
+#endif /* !defined( HAVE_LOCAL_LIBCNOTIFY ) */
```

### Comparing `libfwsi-20230114/libuna/libuna_codepage_iso_8859_16.c` & `libfwsi-20230710/libuna/libuna_codepage_iso_8859_16.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-16 codepage (Latin 10) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfwsi-20230114/libfwsi/libfwsi_libfwps.h` & `libfwsi-20230710/libfwsi/libfwsi_libfwps.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_file_entry_extension_values.c` & `libfwsi-20230710/libfwsi/libfwsi_file_entry_extension_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0014_values.c` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0014_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_file_entry_extension_values.h` & `libfwsi-20230710/libfwsi/libfwsi_file_entry_extension_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_support.c` & `libfwsi-20230710/libfwsi/libfwsi_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0013_values.h` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0013_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_libcdata.h` & `libfwsi-20230710/libfwsi/libfwsi_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_libcerror.h` & `libfwsi-20230710/libfwsi/libfwsi_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_control_panel_values.h` & `libfwsi-20230710/libfwsi/libfwsi_control_panel_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0025_values.c` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0025_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0001_values.h` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0001_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_root_folder.h` & `libfwsi-20230710/libfwsi/libfwsi_root_folder.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi.rc.in` & `libfwsi-20230710/libfwsi/libfwsi.rc.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_delegate_values.h` & `libfwsi-20230710/libfwsi/libfwsi_delegate_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_libfole.h` & `libfwsi-20230710/libfwsi/libfwsi_libfole.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi.c` & `libfwsi-20230710/libfwsi/libfwsi.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_root_folder_values.h` & `libfwsi-20230710/libfwsi/libfwsi_root_folder_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_mtp_volume_values.h` & `libfwsi-20230710/libfwsi/libfwsi_mtp_volume_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0006_values.c` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0006_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_libfdatetime.h` & `libfwsi-20230710/libfwsi/libfwsi_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_users_property_view_values.h` & `libfwsi-20230710/libfwsi/libfwsi_users_property_view_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/Makefile.am` & `libfwsi-20230710/libfwsi/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_file_entry_values.c` & `libfwsi-20230710/libfwsi/libfwsi_file_entry_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_libuna.h` & `libfwsi-20230710/libfwsi/libfwsi_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_volume_values.c` & `libfwsi-20230710/libfwsi/libfwsi_volume_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_volume_values.h` & `libfwsi-20230710/libfwsi/libfwsi_volume_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_file_attributes.c` & `libfwsi-20230710/libfwsi/libfwsi_file_attributes.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_shell_folder_identifier.h` & `libfwsi-20230710/libfwsi/libfwsi_shell_folder_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_types.h` & `libfwsi-20230710/libfwsi/libfwsi_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_control_panel_identifier.c` & `libfwsi-20230710/libfwsi/libfwsi_control_panel_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_codepage.h` & `libfwsi-20230710/libfwsi/libfwsi_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef000a_values.h` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef000a_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0003_values.c` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0003_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_delegate_values.c` & `libfwsi-20230710/libfwsi/libfwsi_delegate_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_file_entry_extension.h` & `libfwsi-20230710/libfwsi/libfwsi_file_entry_extension.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_network_location_values.h` & `libfwsi-20230710/libfwsi/libfwsi_network_location_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_item_list.h` & `libfwsi-20230710/libfwsi/libfwsi_item_list.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_compressed_folder_values.c` & `libfwsi-20230710/libfwsi/libfwsi_unknown_0x74_values.c`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Compressed folder (shell item) values functions
+ * Unknown 0x74 (shell item) values functions
  *
  * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
@@ -20,152 +20,154 @@
  */
 
 #include <common.h>
 #include <byte_stream.h>
 #include <memory.h>
 #include <types.h>
 
-#include "libfwsi_compressed_folder_values.h"
 #include "libfwsi_debug.h"
-#include "libfwsi_definitions.h"
+#include "libfwsi_file_attributes.h"
 #include "libfwsi_libcerror.h"
 #include "libfwsi_libcnotify.h"
 #include "libfwsi_libfdatetime.h"
-#include "libfwsi_libuna.h"
-#include "libfwsi_unused.h"
+#include "libfwsi_libfguid.h"
+#include "libfwsi_shell_folder_identifier.h"
+#include "libfwsi_unknown_0x74_values.h"
 
-/* Creates compressed folder values
- * Make sure the value compressed_folder_values is referencing, is set to NULL
+/* Creates unknown 0x74 values
+ * Make sure the value unknown_0x74_values is referencing, is set to NULL
  * Returns 1 if successful or -1 on error
  */
-int libfwsi_compressed_folder_values_initialize(
-     libfwsi_compressed_folder_values_t **compressed_folder_values,
+int libfwsi_unknown_0x74_values_initialize(
+     libfwsi_unknown_0x74_values_t **unknown_0x74_values,
      libcerror_error_t **error )
 {
-	static char *function = "libfwsi_compressed_folder_values_initialize";
+	static char *function = "libfwsi_unknown_0x74_values_initialize";
 
-	if( compressed_folder_values == NULL )
+	if( unknown_0x74_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid compressed folder values.",
+		 "%s: invalid unknown 0x74 values.",
 		 function );
 
 		return( -1 );
 	}
-	if( *compressed_folder_values != NULL )
+	if( *unknown_0x74_values != NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_VALUE_ALREADY_SET,
-		 "%s: invalid compressed folder values value already set.",
+		 "%s: invalid unknown 0x74 values value already set.",
 		 function );
 
 		return( -1 );
 	}
-	*compressed_folder_values = memory_allocate_structure(
-	                             libfwsi_compressed_folder_values_t );
+	*unknown_0x74_values = memory_allocate_structure(
+	                        libfwsi_unknown_0x74_values_t );
 
-	if( *compressed_folder_values == NULL )
+	if( *unknown_0x74_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_MEMORY,
 		 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
-		 "%s: unable to create compressed folder values.",
+		 "%s: unable to create unknown 0x74 values.",
 		 function );
 
 		goto on_error;
 	}
 	if( memory_set(
-	     *compressed_folder_values,
+	     *unknown_0x74_values,
 	     0,
-	     sizeof( libfwsi_compressed_folder_values_t ) ) == NULL )
+	     sizeof( libfwsi_unknown_0x74_values_t ) ) == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_MEMORY,
 		 LIBCERROR_MEMORY_ERROR_SET_FAILED,
-		 "%s: unable to clear compressed folder values.",
+		 "%s: unable to clear unknown 0x74 values.",
 		 function );
 
 		goto on_error;
 	}
 	return( 1 );
 
 on_error:
-	if( *compressed_folder_values != NULL )
+	if( *unknown_0x74_values != NULL )
 	{
 		memory_free(
-		 *compressed_folder_values );
+		 *unknown_0x74_values );
 
-		*compressed_folder_values = NULL;
+		*unknown_0x74_values = NULL;
 	}
 	return( -1 );
 }
 
-/* Frees compressed folder values
+/* Frees unknown 0x74 values
  * Returns 1 if successful or -1 on error
  */
-int libfwsi_compressed_folder_values_free(
-     libfwsi_compressed_folder_values_t **compressed_folder_values,
+int libfwsi_unknown_0x74_values_free(
+     libfwsi_unknown_0x74_values_t **unknown_0x74_values,
      libcerror_error_t **error )
 {
-	static char *function = "libfwsi_compressed_folder_values_free";
+	static char *function = "libfwsi_unknown_0x74_values_free";
 
-	if( compressed_folder_values == NULL )
+	if( unknown_0x74_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid compressed folder values.",
+		 "%s: invalid unknown 0x74 values.",
 		 function );
 
 		return( -1 );
 	}
-	if( *compressed_folder_values != NULL )
+	if( *unknown_0x74_values != NULL )
 	{
 		memory_free(
-		 *compressed_folder_values );
+		 *unknown_0x74_values );
 
-		*compressed_folder_values = NULL;
+		*unknown_0x74_values = NULL;
 	}
 	return( 1 );
 }
 
-/* Reads the compressed folder values
+/* Reads the unknown 0x74 values
  * Returns 1 if successful, 0 if not supported or -1 on error
  */
-int libfwsi_compressed_folder_values_read_data(
-     libfwsi_compressed_folder_values_t *compressed_folder_values,
+int libfwsi_unknown_0x74_values_read_data(
+     libfwsi_unknown_0x74_values_t *unknown_0x74_values,
      const uint8_t *data,
      size_t data_size,
+     int ascii_codepage,
      libcerror_error_t **error )
 {
-	static char *function = "libfwsi_compressed_folder_values_read_data";
-	size_t data_offset    = 0;
-	uint32_t string_size  = 0;
+	static char *function        = "libfwsi_unknown_0x74_values_read_data";
+	size_t data_offset           = 0;
+	size_t string_alignment_size = 0;
+	size_t string_size           = 0;
+	uint16_t item_data_size      = 0;
 
 #if defined( HAVE_DEBUG_OUTPUT )
-	uint64_t value_64bit  = 0;
-	uint32_t value_32bit  = 0;
-	uint16_t value_16bit  = 0;
+	uint32_t value_32bit         = 0;
+	uint16_t value_16bit         = 0;
 #endif
 
-	if( compressed_folder_values == NULL )
+	if( unknown_0x74_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid compressed folder values.",
+		 "%s: invalid unknown 0x74 values.",
 		 function );
 
 		return( -1 );
 	}
 	if( data == NULL )
 	{
 		libcerror_error_set(
@@ -186,324 +188,278 @@
 		 "%s: data size exceeds maximum.",
 		 function );
 
 		return( -1 );
 	}
 	/* Do not try to parse unsupported data sizes
 	 */
-	if( data_size < 6 )
+	if( data_size < 12 )
 	{
 		return( 0 );
 	}
-	/* Do not try to parse unknown class type indicators
+	/* Do not try to parse unsupported shell item signatures
 	 */
-	if( data[ 2 ] != 0x52 )
+	if( memory_compare(
+	     &( data[ 6 ] ),
+	     "CFSF",
+	     4 ) != 0 )
 	{
 		return( 0 );
 	}
-/* TODO: other variants not supported yet */
-	if( ( data[ 3 ] != 0x67 )
-	 || ( data[ 4 ] != 0xb1 )
-	 || ( data[ 5 ] != 0xac ) )
+	byte_stream_copy_to_uint32_little_endian(
+	 &( data[ 10 ] ),
+	 item_data_size );
+
+#if defined( HAVE_DEBUG_OUTPUT )
+	if( libcnotify_verbose != 0 )
 	{
-		return( 0 );
+		libcnotify_printf(
+		 "%s: class type indicator\t\t\t: 0x%02" PRIx8 "\n",
+		 function,
+		 data[ 2 ] );
+
+		libcnotify_printf(
+		 "%s: unknown1\t\t\t\t: 0x%02" PRIx8 "\n",
+		 function,
+		 data[ 3 ] );
+
+		byte_stream_copy_to_uint16_little_endian(
+		 &( data[ 4 ] ),
+		 value_16bit );
+		libcnotify_printf(
+		 "%s: unknown2\t\t\t\t: 0x%04" PRIx16 "\n",
+		 function,
+		 value_16bit );
+
+		libcnotify_printf(
+		 "%s: signature\t\t\t\t: %c%c%c%c\n",
+		 function,
+		 data[ 6 ],
+		 data[ 7 ],
+		 data[ 8 ],
+		 data[ 9 ] );
+
+		libcnotify_printf(
+		 "%s: data size\t\t\t\t: %" PRIu16 "\n",
+		 function,
+		 item_data_size );
 	}
-	if( ( data[ 3 ] == 0x67 )
-	 && ( data[ 4 ] == 0xb1 )
-	 && ( data[ 5 ] == 0xac ) )
+#endif
+	data_offset = 12;
+
+	if( item_data_size > 0 )
 	{
-		if( data_size < 50 )
+		if( ( item_data_size < 2 )
+		 && ( item_data_size > ( data_size - 12 ) ) )
 		{
-			return( 0 );
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+			 "%s: invalid data size value out of bounds.",
+			 function );
+
+			return( -1 );
 		}
+		item_data_size -= 2;
+
 #if defined( HAVE_DEBUG_OUTPUT )
 		if( libcnotify_verbose != 0 )
 		{
 			libcnotify_printf(
-			 "%s: unknown1\t\t\t\t: 0x%02" PRIx8 "\n",
-			 function,
-			 data[ 3 ] );
-
+			 "%s: data:\n",
+			 function );
+			libcnotify_print_data(
+			 &( data[ 12 ] ),
+			 item_data_size,
+			 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
+		}
+#endif
+	}
+#if defined( HAVE_DEBUG_OUTPUT )
+	else if( libcnotify_verbose != 0 )
+	{
+		libcnotify_printf(
+		 "\n" );
+	}
+#endif
+/* TODO move to sub item parsing ? */
+	if( item_data_size >= 16 )
+	{
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
+		{
 			byte_stream_copy_to_uint16_little_endian(
-			 &( data[ 4 ] ),
+			 &( data[ 12 ] ),
 			 value_16bit );
 			libcnotify_printf(
-			 "%s: unknown2\t\t\t\t: 0x%04" PRIx16 "\n",
+			 "%s: unknown3\t\t\t\t: 0x%04" PRIx16 "\n",
 			 function,
 			 value_16bit );
 
 			byte_stream_copy_to_uint32_little_endian(
-			 &( data[ 6 ] ),
-			 value_32bit );
-			libcnotify_printf(
-			 "%s: unknown3\t\t\t\t: 0x%08" PRIx32 "\n",
-			 function,
-			 value_32bit );
-
-			byte_stream_copy_to_uint64_little_endian(
-			 &( data[ 10 ] ),
-			 value_64bit );
-			libcnotify_printf(
-			 "%s: unknown4\t\t\t\t: 0x%08" PRIx64 "\n",
-			 function,
-			 value_64bit );
-
-			byte_stream_copy_to_uint32_little_endian(
-			 &( data[ 18 ] ),
-			 value_32bit );
-			libcnotify_printf(
-			 "%s: unknown5\t\t\t\t: 0x%08" PRIx32 "\n",
-			 function,
-			 value_32bit );
-
-			byte_stream_copy_to_uint32_little_endian(
-			 &( data[ 22 ] ),
+			 &( data[ 14 ] ),
 			 value_32bit );
 			libcnotify_printf(
-			 "%s: unknown6\t\t\t\t: 0x%08" PRIx32 "\n",
+			 "%s: file size\t\t\t\t: %" PRIu32 "\n",
 			 function,
 			 value_32bit );
 
 			if( libfwsi_debug_print_fat_date_time_value(
 			     function,
-			     "unknown time1\t\t\t",
-			     &( data[ 26 ] ),
+			     "modification time\t\t\t",
+			     &( data[ 18 ] ),
 			     4,
 			     LIBFDATETIME_ENDIAN_LITTLE,
 			     LIBFDATETIME_STRING_FORMAT_TYPE_CTIME | LIBFDATETIME_STRING_FORMAT_FLAG_DATE_TIME,
 			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
 				 "%s: unable to print FAT date time value.",
 				 function );
 
 				return( -1 );
 			}
-			byte_stream_copy_to_uint32_little_endian(
-			 &( data[ 30 ] ),
-			 value_32bit );
+			byte_stream_copy_to_uint16_little_endian(
+			 &( data[ 22 ] ),
+			 value_16bit );
 			libcnotify_printf(
-			 "%s: unknown7\t\t\t\t: 0x%08" PRIx32 "\n",
+			 "%s: file attribute flags\t\t\t: 0x%04" PRIx16 "\n",
 			 function,
-			 value_32bit );
-
-			if( libfwsi_debug_print_fat_date_time_value(
-			     function,
-			     "unknown time2\t\t\t",
-			     &( data[ 34 ] ),
-			     4,
-			     LIBFDATETIME_ENDIAN_LITTLE,
-			     LIBFDATETIME_STRING_FORMAT_TYPE_CTIME | LIBFDATETIME_STRING_FORMAT_FLAG_DATE_TIME,
-			     error ) != 1 )
-			{
-				libcerror_error_set(
-				 error,
-				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
-				 "%s: unable to print FAT date time value.",
-				 function );
-
-				return( -1 );
-			}
-			byte_stream_copy_to_uint64_little_endian(
-			 &( data[ 38 ] ),
-			 value_64bit );
+			 value_16bit );
+			libfwsi_file_attributes_print(
+			 value_16bit );
 			libcnotify_printf(
-			 "%s: unknown8\t\t\t\t: 0x%08" PRIx64 "\n",
-			 function,
-			 value_64bit );
+			 "\n" );
 		}
 #endif
-		data_offset = 46;
-	}
-	byte_stream_copy_to_uint32_little_endian(
-	 &( data[ data_offset ] ),
-	 string_size );
+		data_offset += 12;
 
-#if defined( HAVE_DEBUG_OUTPUT )
-	if( libcnotify_verbose != 0 )
-	{
-		libcnotify_printf(
-		 "%s: string size\t\t\t: %" PRIu32 "\n",
-		 function,
-		 string_size );
-	}
-#endif
-	data_offset += 4;
-
-	string_size *= 2;
-
-	if( ( string_size > 0 )
-         && ( string_size <= data_size )
-	 && ( data_offset <= ( data_size - string_size ) ) )
-	{
-#if defined( HAVE_DEBUG_OUTPUT )
-		if( libcnotify_verbose != 0 )
+		for( string_size = data_offset;
+		     string_size < data_size;
+		     string_size++ )
 		{
-			if( libfwsi_debug_print_utf16_string_value(
-			     function,
-			     "string\t\t\t\t",
-			     &( data[ data_offset ] ),
-			     string_size,
-			     LIBUNA_ENDIAN_LITTLE,
-			     error ) != 1 )
+			if( data[ string_size ] == 0 )
 			{
-				libcerror_error_set(
-				 error,
-				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
-				 "%s: unable to print UTF-16 string value.",
-				 function );
+				string_size++;
 
-				return( -1 );
+				break;
 			}
 		}
-#endif
-		data_offset += string_size;
-	}
-	byte_stream_copy_to_uint32_little_endian(
-	 &( data[ data_offset ] ),
-	 string_size );
-
-#if defined( HAVE_DEBUG_OUTPUT )
-	if( libcnotify_verbose != 0 )
-	{
-		libcnotify_printf(
-		 "%s: string size\t\t\t: %" PRIu32 "\n",
-		 function,
-		 string_size );
-	}
-#endif
-	data_offset += 4;
+		string_size -= data_offset;
 
-	string_size *= 2;
+		string_alignment_size = string_size % 2;
 
-	if( ( string_size > 0 )
-         && ( string_size <= data_size )
-	 && ( data_offset <= ( data_size - string_size ) ) )
-	{
 #if defined( HAVE_DEBUG_OUTPUT )
 		if( libcnotify_verbose != 0 )
 		{
-			if( libfwsi_debug_print_utf16_string_value(
+			if( libfwsi_debug_print_string_value(
 			     function,
-			     "string\t\t\t\t",
+			     "primary name\t\t\t\t",
 			     &( data[ data_offset ] ),
 			     string_size,
-			     LIBUNA_ENDIAN_LITTLE,
+			     ascii_codepage,
 			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
-				 "%s: unable to print UTF-16 string value.",
+				 "%s: unable to print string value.",
 				 function );
 
 				return( -1 );
 			}
 		}
 #endif
-		data_offset += string_size;
-	}
-	byte_stream_copy_to_uint32_little_endian(
-	 &( data[ data_offset ] ),
-	 string_size );
+		data_offset += string_size + string_alignment_size;
 
 #if defined( HAVE_DEBUG_OUTPUT )
-	if( libcnotify_verbose != 0 )
-	{
-		libcnotify_printf(
-		 "%s: string size\t\t\t: %" PRIu32 "\n",
-		 function,
-		 string_size );
-	}
-#endif
-	data_offset += 4;
-
-	string_size *= 2;
-
-	if( ( string_size > 0 )
-         && ( string_size <= data_size )
-	 && ( data_offset <= ( data_size - string_size ) ) )
-	{
-#if defined( HAVE_DEBUG_OUTPUT )
 		if( libcnotify_verbose != 0 )
 		{
-			if( libfwsi_debug_print_utf16_string_value(
-			     function,
-			     "string\t\t\t\t",
-			     &( data[ data_offset ] ),
-			     string_size,
-			     LIBUNA_ENDIAN_LITTLE,
-			     error ) != 1 )
-			{
-				libcerror_error_set(
-				 error,
-				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
-				 "%s: unable to print UTF-16 string value.",
-				 function );
+			byte_stream_copy_to_uint16_little_endian(
+			 &( data[ data_offset ] ),
+			 value_16bit );
 
-				return( -1 );
-			}
+			libcnotify_printf(
+			 "%s: unknown5\t\t\t\t: 0x%04" PRIx16 "\n",
+			 function,
+			 value_16bit );
 		}
 #endif
-		data_offset += string_size;
+		data_offset += 2;
 	}
-	byte_stream_copy_to_uint32_little_endian(
-	 &( data[ data_offset ] ),
-	 string_size );
+	if( data_offset > ( data_size - 32 ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+		 "%s: invalid data size value out of bounds.",
+		 function );
 
+		return( -1 );
+	}
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
-		libcnotify_printf(
-		 "%s: string size\t\t\t: %" PRIu32 "\n",
-		 function,
-		 string_size );
-	}
-#endif
-	data_offset += 4;
-
-	string_size *= 2;
-
-	if( ( string_size > 0 )
-         && ( string_size <= data_size )
-	 && ( data_offset <= ( data_size - string_size ) ) )
-	{
-#if defined( HAVE_DEBUG_OUTPUT )
-		if( libcnotify_verbose != 0 )
+		if( libfwsi_debug_print_guid_value(
+		     function,
+		     "delagate item class identifier\t",
+		     &( data[ data_offset ] ),
+		     16,
+		     LIBFGUID_ENDIAN_LITTLE,
+		     LIBFGUID_STRING_FORMAT_FLAG_USE_UPPER_CASE | LIBFGUID_STRING_FORMAT_FLAG_USE_SURROUNDING_BRACES,
+		     error ) != 1 )
 		{
-			if( libfwsi_debug_print_utf16_string_value(
-			     function,
-			     "string\t\t\t\t",
-			     &( data[ data_offset ] ),
-			     string_size,
-			     LIBUNA_ENDIAN_LITTLE,
-			     error ) != 1 )
-			{
-				libcerror_error_set(
-				 error,
-				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
-				 "%s: unable to print UTF-16 string value.",
-				 function );
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+			 "%s: unable to print GUID value.",
+			 function );
 
-				return( -1 );
-			}
+			return( -1 );
 		}
-#endif
 	}
+#endif
+	data_offset += 16;
+
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
+		if( libfwsi_debug_print_guid_value(
+		     function,
+		     "item class identifier\t\t\t",
+		     &( data[ data_offset ] ),
+		     16,
+		     LIBFGUID_ENDIAN_LITTLE,
+		     LIBFGUID_STRING_FORMAT_FLAG_USE_UPPER_CASE | LIBFGUID_STRING_FORMAT_FLAG_USE_SURROUNDING_BRACES,
+		     error ) != 1 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+			 "%s: unable to print GUID value.",
+			 function );
+
+			return( -1 );
+		}
+		libcnotify_printf(
+		 "%s: shell folder name\t\t\t: %s\n",
+		 function,
+		 libfwsi_shell_folder_identifier_get_name(
+		  &( data[ data_offset ] ) ) );
+
 		libcnotify_printf(
 		 "\n" );
 	}
 #endif
+	data_offset += 16;
+
 	return( 1 );
 }
```

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0000_values.h` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0000_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_notify.h` & `libfwsi-20230710/libfwsi/libfwsi_notify.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0014_values.h` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0014_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0013_values.c` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0013_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_game_folder_values.c` & `libfwsi-20230710/libfwsi/libfwsi_game_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0019_values.h` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0019_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_file_entry.c` & `libfwsi-20230710/libfwsi/libfwsi_file_entry.c`

 * *Files 4% similar despite different names*

```diff
@@ -223,14 +223,16 @@
 	}
 	*file_attribute_flags = file_entry_values->file_attribute_flags;
 
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-8 formatted name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 int libfwsi_file_entry_get_utf8_name_size(
      libfwsi_item_t *file_entry,
      size_t *utf8_string_size,
      libcerror_error_t **error )
 {
@@ -277,15 +279,15 @@
 	file_entry_values = (libfwsi_file_entry_values_t *) internal_item->value;
 
 	if( file_entry_values->is_unicode != 0 )
 	{
 		result = libuna_utf8_string_size_from_utf16_stream(
 			  file_entry_values->name,
 			  file_entry_values->name_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  utf8_string_size,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf8_string_size_from_byte_stream(
 			  file_entry_values->name,
@@ -305,14 +307,16 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-8 formatted name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful or -1 on error
  */
 int libfwsi_file_entry_get_utf8_name(
      libfwsi_item_t *file_entry,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      libcerror_error_t **error )
@@ -362,15 +366,15 @@
 	if( file_entry_values->is_unicode != 0 )
 	{
 		result = libuna_utf8_string_copy_from_utf16_stream(
 		          utf8_string,
 		          utf8_string_size,
 			  file_entry_values->name,
 			  file_entry_values->name_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf8_string_copy_from_byte_stream(
 		          utf8_string,
 		          utf8_string_size,
@@ -390,14 +394,16 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-16 formatted name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 int libfwsi_file_entry_get_utf16_name_size(
      libfwsi_item_t *file_entry,
      size_t *utf16_string_size,
      libcerror_error_t **error )
 {
@@ -444,15 +450,15 @@
 	file_entry_values = (libfwsi_file_entry_values_t *) internal_item->value;
 
 	if( file_entry_values->is_unicode != 0 )
 	{
 		result = libuna_utf16_string_size_from_utf16_stream(
 			  file_entry_values->name,
 			  file_entry_values->name_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  utf16_string_size,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf16_string_size_from_byte_stream(
 			  file_entry_values->name,
@@ -472,14 +478,16 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-16 formatted name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful or -1 on error
  */
 int libfwsi_file_entry_get_utf16_name(
      libfwsi_item_t *file_entry,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      libcerror_error_t **error )
@@ -529,15 +537,15 @@
 	if( file_entry_values->is_unicode != 0 )
 	{
 		result = libuna_utf16_string_copy_from_utf16_stream(
 		          utf16_string,
 		          utf16_string_size,
 			  file_entry_values->name,
 			  file_entry_values->name_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf16_string_copy_from_byte_stream(
 		          utf16_string,
 		          utf16_string_size,
```

### Comparing `libfwsi-20230114/libfwsi/libfwsi_cdburn_values.h` & `libfwsi-20230710/libfwsi/libfwsi_cdburn_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_unknown_0x74_values.c` & `libfwsi-20230710/libfwsi/libfwsi_control_panel_cpl_file_values.c`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Unknown 0x74 (shell item) values functions
+ * Control Panel CPL file (shell item) values functions
  *
  * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
@@ -20,154 +20,149 @@
  */
 
 #include <common.h>
 #include <byte_stream.h>
 #include <memory.h>
 #include <types.h>
 
+#include "libfwsi_control_panel_cpl_file_values.h"
 #include "libfwsi_debug.h"
-#include "libfwsi_file_attributes.h"
 #include "libfwsi_libcerror.h"
 #include "libfwsi_libcnotify.h"
-#include "libfwsi_libfdatetime.h"
-#include "libfwsi_libfguid.h"
-#include "libfwsi_shell_folder_identifier.h"
-#include "libfwsi_unknown_0x74_values.h"
+#include "libfwsi_libuna.h"
 
-/* Creates unknown 0x74 values
- * Make sure the value unknown_0x74_values is referencing, is set to NULL
+/* Creates control panel CPL file values
+ * Make sure the value control_panel_cpl_file_values is referencing, is set to NULL
  * Returns 1 if successful or -1 on error
  */
-int libfwsi_unknown_0x74_values_initialize(
-     libfwsi_unknown_0x74_values_t **unknown_0x74_values,
+int libfwsi_control_panel_cpl_file_values_initialize(
+     libfwsi_control_panel_cpl_file_values_t **control_panel_cpl_file_values,
      libcerror_error_t **error )
 {
-	static char *function = "libfwsi_unknown_0x74_values_initialize";
+	static char *function = "libfwsi_control_panel_cpl_file_values_initialize";
 
-	if( unknown_0x74_values == NULL )
+	if( control_panel_cpl_file_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid unknown 0x74 values.",
+		 "%s: invalid control panel CPL file values.",
 		 function );
 
 		return( -1 );
 	}
-	if( *unknown_0x74_values != NULL )
+	if( *control_panel_cpl_file_values != NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_VALUE_ALREADY_SET,
-		 "%s: invalid unknown 0x74 values value already set.",
+		 "%s: invalid control panel CPL file values value already set.",
 		 function );
 
 		return( -1 );
 	}
-	*unknown_0x74_values = memory_allocate_structure(
-	                        libfwsi_unknown_0x74_values_t );
+	*control_panel_cpl_file_values = memory_allocate_structure(
+	                                  libfwsi_control_panel_cpl_file_values_t );
 
-	if( *unknown_0x74_values == NULL )
+	if( *control_panel_cpl_file_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_MEMORY,
 		 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
-		 "%s: unable to create unknown 0x74 values.",
+		 "%s: unable to create control panel CPL file values.",
 		 function );
 
 		goto on_error;
 	}
 	if( memory_set(
-	     *unknown_0x74_values,
+	     *control_panel_cpl_file_values,
 	     0,
-	     sizeof( libfwsi_unknown_0x74_values_t ) ) == NULL )
+	     sizeof( libfwsi_control_panel_cpl_file_values_t ) ) == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_MEMORY,
 		 LIBCERROR_MEMORY_ERROR_SET_FAILED,
-		 "%s: unable to clear unknown 0x74 values.",
+		 "%s: unable to clear control panel CPL file values.",
 		 function );
 
 		goto on_error;
 	}
 	return( 1 );
 
 on_error:
-	if( *unknown_0x74_values != NULL )
+	if( *control_panel_cpl_file_values != NULL )
 	{
 		memory_free(
-		 *unknown_0x74_values );
+		 *control_panel_cpl_file_values );
 
-		*unknown_0x74_values = NULL;
+		*control_panel_cpl_file_values = NULL;
 	}
 	return( -1 );
 }
 
-/* Frees unknown 0x74 values
+/* Frees control panel CPL file values
  * Returns 1 if successful or -1 on error
  */
-int libfwsi_unknown_0x74_values_free(
-     libfwsi_unknown_0x74_values_t **unknown_0x74_values,
+int libfwsi_control_panel_cpl_file_values_free(
+     libfwsi_control_panel_cpl_file_values_t **control_panel_cpl_file_values,
      libcerror_error_t **error )
 {
-	static char *function = "libfwsi_unknown_0x74_values_free";
+	static char *function = "libfwsi_control_panel_cpl_file_values_free";
 
-	if( unknown_0x74_values == NULL )
+	if( control_panel_cpl_file_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid unknown 0x74 values.",
+		 "%s: invalid control panel CPL file values.",
 		 function );
 
 		return( -1 );
 	}
-	if( *unknown_0x74_values != NULL )
+	if( *control_panel_cpl_file_values != NULL )
 	{
 		memory_free(
-		 *unknown_0x74_values );
+		 *control_panel_cpl_file_values );
 
-		*unknown_0x74_values = NULL;
+		*control_panel_cpl_file_values = NULL;
 	}
 	return( 1 );
 }
 
-/* Reads the unknown 0x74 values
+/* Reads the control panel CPL file values
  * Returns 1 if successful, 0 if not supported or -1 on error
  */
-int libfwsi_unknown_0x74_values_read_data(
-     libfwsi_unknown_0x74_values_t *unknown_0x74_values,
+int libfwsi_control_panel_cpl_file_values_read_data(
+     libfwsi_control_panel_cpl_file_values_t *control_panel_cpl_file_values,
      const uint8_t *data,
      size_t data_size,
-     int ascii_codepage,
      libcerror_error_t **error )
 {
-	static char *function        = "libfwsi_unknown_0x74_values_read_data";
-	size_t data_offset           = 0;
-	size_t string_alignment_size = 0;
-	size_t string_size           = 0;
-	uint16_t item_data_size      = 0;
+	static char *function = "libfwsi_control_panel_cpl_file_values_read_data";
+	size_t data_offset    = 0;
+	size_t string_size    = 0;
+	uint32_t signature    = 0;
 
 #if defined( HAVE_DEBUG_OUTPUT )
-	uint32_t value_32bit         = 0;
-	uint16_t value_16bit         = 0;
+	uint32_t value_32bit  = 0;
+	uint16_t value_16bit  = 0;
 #endif
 
-	if( unknown_0x74_values == NULL )
+	if( control_panel_cpl_file_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid unknown 0x74 values.",
+		 "%s: invalid control panel CPL file values.",
 		 function );
 
 		return( -1 );
 	}
 	if( data == NULL )
 	{
 		libcerror_error_set(
@@ -188,278 +183,209 @@
 		 "%s: data size exceeds maximum.",
 		 function );
 
 		return( -1 );
 	}
 	/* Do not try to parse unsupported data sizes
 	 */
-	if( data_size < 12 )
+	if( data_size < 24 )
 	{
 		return( 0 );
 	}
 	/* Do not try to parse unsupported shell item signatures
 	 */
-	if( memory_compare(
-	     &( data[ 6 ] ),
-	     "CFSF",
-	     4 ) != 0 )
+	byte_stream_copy_to_uint32_little_endian(
+	 &( data[ 4 ] ),
+	 signature );
+
+	if( signature != 0xffffff38UL )
 	{
 		return( 0 );
 	}
-	byte_stream_copy_to_uint32_little_endian(
-	 &( data[ 10 ] ),
-	 item_data_size );
-
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
 		libcnotify_printf(
-		 "%s: class type indicator\t\t\t: 0x%02" PRIx8 "\n",
+		 "%s: class type indicator\t: 0x%02" PRIx8 "\n",
 		 function,
 		 data[ 2 ] );
 
 		libcnotify_printf(
-		 "%s: unknown1\t\t\t\t: 0x%02" PRIx8 "\n",
+		 "%s: unknown1\t\t\t: 0x%02" PRIx8 "\n",
 		 function,
 		 data[ 3 ] );
 
-		byte_stream_copy_to_uint16_little_endian(
-		 &( data[ 4 ] ),
-		 value_16bit );
 		libcnotify_printf(
-		 "%s: unknown2\t\t\t\t: 0x%04" PRIx16 "\n",
+		 "%s: signature\t\t\t: 0x%08" PRIx32 "\n",
 		 function,
-		 value_16bit );
+		 signature );
+
+		byte_stream_copy_to_uint32_little_endian(
+		 &( data[ 8 ] ),
+		 value_32bit );
+		libcnotify_printf(
+		 "%s: unknown2\t\t\t: 0x%08" PRIx32 "\n",
+		 function,
+		 value_32bit );
+
+		byte_stream_copy_to_uint32_little_endian(
+		 &( data[ 12 ] ),
+		 value_32bit );
+		libcnotify_printf(
+		 "%s: unknown3\t\t\t: 0x%08" PRIx32 "\n",
+		 function,
+		 value_32bit );
+
+		byte_stream_copy_to_uint32_little_endian(
+		 &( data[ 16 ] ),
+		 value_32bit );
+		libcnotify_printf(
+		 "%s: unknown4\t\t\t: 0x%08" PRIx32 "\n",
+		 function,
+		 value_32bit );
 
+		byte_stream_copy_to_uint16_little_endian(
+		 &( data[ 20 ] ),
+		 value_16bit );
 		libcnotify_printf(
-		 "%s: signature\t\t\t\t: %c%c%c%c\n",
+		 "%s: unknown5\t\t\t: 0x%04" PRIx16 "\n",
 		 function,
-		 data[ 6 ],
-		 data[ 7 ],
-		 data[ 8 ],
-		 data[ 9 ] );
+		 value_16bit );
 
+		byte_stream_copy_to_uint16_little_endian(
+		 &( data[ 22 ] ),
+		 value_16bit );
 		libcnotify_printf(
-		 "%s: data size\t\t\t\t: %" PRIu16 "\n",
+		 "%s: unknown6\t\t\t: 0x%04" PRIx16 "\n",
 		 function,
-		 item_data_size );
+		 value_16bit );
 	}
 #endif
-	data_offset = 12;
+	data_offset = 24;
 
-	if( item_data_size > 0 )
+	if( data_offset <= ( data_size - 2 ) )
 	{
-		if( ( item_data_size < 2 )
-		 && ( item_data_size > ( data_size - 12 ) ) )
+		for( string_size = data_offset;
+		     string_size < data_size;
+		     string_size += 2 )
 		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-			 "%s: invalid data size value out of bounds.",
-			 function );
+			if( data[ string_size ] == 0 )
+			{
+				string_size += 2;
 
-			return( -1 );
+				break;
+			}
 		}
-		item_data_size -= 2;
+		string_size -= data_offset;
 
 #if defined( HAVE_DEBUG_OUTPUT )
 		if( libcnotify_verbose != 0 )
 		{
-			libcnotify_printf(
-			 "%s: data:\n",
-			 function );
-			libcnotify_print_data(
-			 &( data[ 12 ] ),
-			 item_data_size,
-			 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
-		}
-#endif
-	}
-#if defined( HAVE_DEBUG_OUTPUT )
-	else if( libcnotify_verbose != 0 )
-	{
-		libcnotify_printf(
-		 "\n" );
-	}
-#endif
-/* TODO move to sub item parsing ? */
-	if( item_data_size >= 16 )
-	{
-#if defined( HAVE_DEBUG_OUTPUT )
-		if( libcnotify_verbose != 0 )
-		{
-			byte_stream_copy_to_uint16_little_endian(
-			 &( data[ 12 ] ),
-			 value_16bit );
-			libcnotify_printf(
-			 "%s: unknown3\t\t\t\t: 0x%04" PRIx16 "\n",
-			 function,
-			 value_16bit );
-
-			byte_stream_copy_to_uint32_little_endian(
-			 &( data[ 14 ] ),
-			 value_32bit );
-			libcnotify_printf(
-			 "%s: file size\t\t\t\t: %" PRIu32 "\n",
-			 function,
-			 value_32bit );
-
-			if( libfwsi_debug_print_fat_date_time_value(
+			if( libfwsi_debug_print_utf16_string_value(
 			     function,
-			     "modification time\t\t\t",
-			     &( data[ 18 ] ),
-			     4,
-			     LIBFDATETIME_ENDIAN_LITTLE,
-			     LIBFDATETIME_STRING_FORMAT_TYPE_CTIME | LIBFDATETIME_STRING_FORMAT_FLAG_DATE_TIME,
+			     "CPL file path\t\t",
+			     &( data[ data_offset ] ),
+			     string_size,
+			     LIBUNA_ENDIAN_LITTLE,
 			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
-				 "%s: unable to print FAT date time value.",
+				 "%s: unable to print UTF-16 string value.",
 				 function );
 
 				return( -1 );
 			}
-			byte_stream_copy_to_uint16_little_endian(
-			 &( data[ 22 ] ),
-			 value_16bit );
-			libcnotify_printf(
-			 "%s: file attribute flags\t\t\t: 0x%04" PRIx16 "\n",
-			 function,
-			 value_16bit );
-			libfwsi_file_attributes_print(
-			 value_16bit );
-			libcnotify_printf(
-			 "\n" );
 		}
 #endif
-		data_offset += 12;
-
+		data_offset += string_size;
+	}
+	if( data_offset <= ( data_size - 2 ) )
+	{
 		for( string_size = data_offset;
 		     string_size < data_size;
-		     string_size++ )
+		     string_size += 2 )
 		{
 			if( data[ string_size ] == 0 )
 			{
-				string_size++;
+				string_size += 2;
 
 				break;
 			}
 		}
 		string_size -= data_offset;
 
-		string_alignment_size = string_size % 2;
-
 #if defined( HAVE_DEBUG_OUTPUT )
 		if( libcnotify_verbose != 0 )
 		{
-			if( libfwsi_debug_print_string_value(
+			if( libfwsi_debug_print_utf16_string_value(
 			     function,
-			     "primary name\t\t\t\t",
+			     "name\t\t\t",
 			     &( data[ data_offset ] ),
 			     string_size,
-			     ascii_codepage,
+			     LIBUNA_ENDIAN_LITTLE,
 			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
-				 "%s: unable to print string value.",
+				 "%s: unable to print UTF-16 string value.",
 				 function );
 
 				return( -1 );
 			}
 		}
 #endif
-		data_offset += string_size + string_alignment_size;
-
-#if defined( HAVE_DEBUG_OUTPUT )
-		if( libcnotify_verbose != 0 )
-		{
-			byte_stream_copy_to_uint16_little_endian(
-			 &( data[ data_offset ] ),
-			 value_16bit );
-
-			libcnotify_printf(
-			 "%s: unknown5\t\t\t\t: 0x%04" PRIx16 "\n",
-			 function,
-			 value_16bit );
-		}
-#endif
-		data_offset += 2;
+		data_offset += string_size;
 	}
-	if( data_offset > ( data_size - 32 ) )
+	if( data_offset <= ( data_size - 2 ) )
 	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-		 "%s: invalid data size value out of bounds.",
-		 function );
+		for( string_size = data_offset;
+		     string_size < data_size;
+		     string_size += 2 )
+		{
+			if( data[ string_size ] == 0 )
+			{
+				string_size += 2;
+
+				break;
+			}
+		}
+		string_size -= data_offset;
 
-		return( -1 );
-	}
 #if defined( HAVE_DEBUG_OUTPUT )
-	if( libcnotify_verbose != 0 )
-	{
-		if( libfwsi_debug_print_guid_value(
-		     function,
-		     "delagate item class identifier\t",
-		     &( data[ data_offset ] ),
-		     16,
-		     LIBFGUID_ENDIAN_LITTLE,
-		     LIBFGUID_STRING_FORMAT_FLAG_USE_UPPER_CASE | LIBFGUID_STRING_FORMAT_FLAG_USE_SURROUNDING_BRACES,
-		     error ) != 1 )
+		if( libcnotify_verbose != 0 )
 		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
-			 "%s: unable to print GUID value.",
-			 function );
+			if( libfwsi_debug_print_utf16_string_value(
+			     function,
+			     "comments\t\t\t",
+			     &( data[ data_offset ] ),
+			     string_size,
+			     LIBUNA_ENDIAN_LITTLE,
+			     error ) != 1 )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+				 "%s: unable to print UTF-16 string value.",
+				 function );
 
-			return( -1 );
+				return( -1 );
+			}
 		}
-	}
 #endif
-	data_offset += 16;
-
+		data_offset += string_size;
+	}
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
-		if( libfwsi_debug_print_guid_value(
-		     function,
-		     "item class identifier\t\t\t",
-		     &( data[ data_offset ] ),
-		     16,
-		     LIBFGUID_ENDIAN_LITTLE,
-		     LIBFGUID_STRING_FORMAT_FLAG_USE_UPPER_CASE | LIBFGUID_STRING_FORMAT_FLAG_USE_SURROUNDING_BRACES,
-		     error ) != 1 )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
-			 "%s: unable to print GUID value.",
-			 function );
-
-			return( -1 );
-		}
-		libcnotify_printf(
-		 "%s: shell folder name\t\t\t: %s\n",
-		 function,
-		 libfwsi_shell_folder_identifier_get_name(
-		  &( data[ data_offset ] ) ) );
-
 		libcnotify_printf(
 		 "\n" );
 	}
 #endif
-	data_offset += 16;
-
 	return( 1 );
 }
```

### Comparing `libfwsi-20230114/libfwsi/libfwsi_uri_sub_values.h` & `libfwsi-20230710/libfwsi/libfwsi_uri_sub_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_debug.c` & `libfwsi-20230710/libfwsi/libfwsi_uri_values.c`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Debug functions
+ * URI (shell item) values functions
  *
  * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
@@ -16,665 +16,646 @@
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
+#include <byte_stream.h>
 #include <memory.h>
-#include <narrow_string.h>
-#include <system_string.h>
 #include <types.h>
-#include <wide_string.h>
 
 #include "libfwsi_debug.h"
 #include "libfwsi_libcerror.h"
 #include "libfwsi_libcnotify.h"
 #include "libfwsi_libfdatetime.h"
-#include "libfwsi_libfguid.h"
-#include "libfwsi_libfwps.h"
 #include "libfwsi_libuna.h"
+#include "libfwsi_uri_values.h"
 
-#if defined( HAVE_DEBUG_OUTPUT )
-
-/* Prints the control planel category
- */
-const char *libfwsi_debug_print_control_panel_category(
-             uint32_t control_panel_category )
-{
-	switch( control_panel_category )
-	{
-		case 0:
-			return( "All Control Panel Items" );
-
-		case 1:
-			return( "Appearance and Personalization" );
-
-		case 2:
-			return( "Hardware and Sound" );
-
-		case 3:
-			return( "Network and Internet" );
-
-		case 4:
-			return( "Sounds, Speech, and Audio Devices" );
-
-		case 5:
-			return( "System and Security" );
-
-		case 6:
-			return( "Clock, Language, and Region" );
-
-		case 7:
-			return( "Ease of Access" );
-
-		case 8:
-			return( "Programs" );
-
-		case 9:
-			return( "User Accounts" );
-
-		case 10:
-			return( "Security Center" );
-
-		case 11:
-			return( "Mobile PC" );
-	}
-	return( "_UNKNOWN_" );
-}
-
-/* Prints a FAT date time value
+/* Creates URI values
+ * Make sure the value uri_values is referencing, is set to NULL
  * Returns 1 if successful or -1 on error
  */
-int libfwsi_debug_print_fat_date_time_value(
-     const char *function_name,
-     const char *value_name,
-     const uint8_t *byte_stream,
-     size_t byte_stream_size,
-     int byte_order,
-     uint32_t string_format_flags,
+int libfwsi_uri_values_initialize(
+     libfwsi_uri_values_t **uri_values,
      libcerror_error_t **error )
 {
-	char date_time_string[ 32 ];
+	static char *function = "libfwsi_uri_values_initialize";
 
-	libfdatetime_fat_date_time_t *fat_date_time = NULL;
-	static char *function                       = "libfwsi_debug_print_fat_date_time_value";
-
-	if( libfdatetime_fat_date_time_initialize(
-	     &fat_date_time,
-	     error ) != 1 )
+	if( uri_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
-		 "%s: unable to create FAT date time.",
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid URI values.",
 		 function );
 
-		goto on_error;
+		return( -1 );
 	}
-	if( libfdatetime_fat_date_time_copy_from_byte_stream(
-	     fat_date_time,
-	     byte_stream,
-	     byte_stream_size,
-	     byte_order,
-	     error ) != 1 )
+	if( *uri_values != NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
-		 "%s: unable to copy byte stream to FAT date time.",
+		 LIBCERROR_RUNTIME_ERROR_VALUE_ALREADY_SET,
+		 "%s: invalid URI values value already set.",
 		 function );
 
-		goto on_error;
+		return( -1 );
 	}
-	if( libfdatetime_fat_date_time_copy_to_utf8_string(
-	     fat_date_time,
-	     (uint8_t *) date_time_string,
-	     32,
-	     string_format_flags,
-	     error ) != 1 )
+	*uri_values = memory_allocate_structure(
+	               libfwsi_uri_values_t );
+
+	if( *uri_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
-		 "%s: unable to copy FAT date time to string.",
+		 LIBCERROR_ERROR_DOMAIN_MEMORY,
+		 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
+		 "%s: unable to create URI values.",
 		 function );
 
 		goto on_error;
 	}
-	libcnotify_printf(
-	 "%s: %s: %s UTC\n",
-	 function_name,
-	 value_name,
-	 date_time_string );
-
-	if( libfdatetime_fat_date_time_free(
-	     &fat_date_time,
-	     error ) != 1 )
+	if( memory_set(
+	     *uri_values,
+	     0,
+	     sizeof( libfwsi_uri_values_t ) ) == NULL )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
-		 "%s: unable to free FAT date time.",
+		 LIBCERROR_ERROR_DOMAIN_MEMORY,
+		 LIBCERROR_MEMORY_ERROR_SET_FAILED,
+		 "%s: unable to clear URI values.",
 		 function );
 
 		goto on_error;
 	}
 	return( 1 );
 
 on_error:
-	if( fat_date_time != NULL )
+	if( *uri_values != NULL )
 	{
-		libfdatetime_fat_date_time_free(
-		 &fat_date_time,
-		 NULL );
+		memory_free(
+		 *uri_values );
+
+		*uri_values = NULL;
 	}
 	return( -1 );
 }
 
-/* Prints a FILETIME value
+/* Frees URI values
  * Returns 1 if successful or -1 on error
  */
-int libfwsi_debug_print_filetime_value(
-     const char *function_name,
-     const char *value_name,
-     const uint8_t *byte_stream,
-     size_t byte_stream_size,
-     int byte_order,
-     uint32_t string_format_flags,
+int libfwsi_uri_values_free(
+     libfwsi_uri_values_t **uri_values,
      libcerror_error_t **error )
 {
-	char date_time_string[ 32 ];
-
-	libfdatetime_filetime_t *filetime = NULL;
-	static char *function             = "libfwsi_debug_print_filetime_value";
-
-	if( libfdatetime_filetime_initialize(
-	     &filetime,
-	     error ) != 1 )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
-		 "%s: unable to create filetime.",
-		 function );
+	static char *function = "libfwsi_uri_values_free";
 
-		goto on_error;
-	}
-	if( libfdatetime_filetime_copy_from_byte_stream(
-	     filetime,
-	     byte_stream,
-	     byte_stream_size,
-	     byte_order,
-	     error ) != 1 )
+	if( uri_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
-		 "%s: unable to copy byte stream to filetime.",
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid URI values.",
 		 function );
 
-		goto on_error;
+		return( -1 );
 	}
-	if( libfdatetime_filetime_copy_to_utf8_string(
-	     filetime,
-	     (uint8_t *) date_time_string,
-	     32,
-	     string_format_flags,
-	     error ) != 1 )
+	if( *uri_values != NULL )
 	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
-		 "%s: unable to copy filetime to string.",
-		 function );
-
-		goto on_error;
-	}
-	libcnotify_printf(
-	 "%s: %s: %s UTC\n",
-	 function_name,
-	 value_name,
-	 date_time_string );
-
-	if( libfdatetime_filetime_free(
-	     &filetime,
-	     error ) != 1 )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
-		 "%s: unable to free filetime.",
-		 function );
+		memory_free(
+		 *uri_values );
 
-		goto on_error;
+		*uri_values = NULL;
 	}
 	return( 1 );
-
-on_error:
-	if( filetime != NULL )
-	{
-		libfdatetime_filetime_free(
-		 &filetime,
-		 NULL );
-	}
-	return( -1 );
 }
 
-/* Prints a GUID/UUID value
- * Returns 1 if successful or -1 on error
+/* Reads the URI values
+ * Returns 1 if successful, 0 if not supported or -1 on error
  */
-int libfwsi_debug_print_guid_value(
-     const char *function_name,
-     const char *value_name,
-     const uint8_t *byte_stream,
-     size_t byte_stream_size,
-     int byte_order,
-     uint32_t string_format_flags,
+int libfwsi_uri_values_read_data(
+     libfwsi_uri_values_t *uri_values,
+     const uint8_t *data,
+     size_t data_size,
+     int ascii_codepage,
      libcerror_error_t **error )
 {
-        system_character_t guid_string[ 48 ];
+	static char *function     = "libfwsi_uri_values_read_data";
+	size_t data_offset        = 0;
+	size_t string_size        = 0;
+	uint32_t string_data_size = 0;
+	uint16_t item_data_size   = 0;
+	uint8_t flags             = 0;
 
-        libfguid_identifier_t *guid = NULL;
-	static char *function       = "libfwsi_debug_print_guid_value";
+#if defined( HAVE_DEBUG_OUTPUT )
+	uint32_t value_32bit      = 0;
+	uint16_t value_16bit      = 0;
+#endif
 
-	if( libfguid_identifier_initialize(
-	     &guid,
-	     error ) != 1 )
+	if( uri_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
-		 "%s: unable to create GUID.",
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid URI values.",
 		 function );
 
-		goto on_error;
+		return( -1 );
 	}
-	if( libfguid_identifier_copy_from_byte_stream(
-	     guid,
-	     byte_stream,
-	     byte_stream_size,
-	     byte_order,
-	     error ) != 1 )
+	if( data == NULL )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
-		 "%s: unable to copy byte stream to GUID.",
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid data.",
 		 function );
 
-		goto on_error;
+		return( -1 );
 	}
-	if( libfguid_identifier_copy_to_utf8_string(
-	     guid,
-	     (uint8_t *) guid_string,
-	     48,
-	     string_format_flags,
-	     error ) != 1 )
+	if( data_size > (size_t) SSIZE_MAX )
 	{
 		libcerror_error_set(
 		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
-		 "%s: unable to copy GUID to string.",
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: data size exceeds maximum.",
 		 function );
 
-		goto on_error;
+		return( -1 );
 	}
-	libcnotify_printf(
-	 "%s: %s: %s\n",
-	 function_name,
-	 value_name,
-	 guid_string );
-
-	if( libfguid_identifier_free(
-	     &guid,
-	     error ) != 1 )
+	/* Do not try to parse unsupported data sizes
+	 */
+	if( data_size < 6 )
 	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
-		 "%s: unable to free GUID.",
-		 function );
-
-		goto on_error;
+		return( 0 );
 	}
-	return( 1 );
-
-on_error:
-	if( guid != NULL )
+	/* Do not try to parse unknown class type indicators
+	 */
+	if( data[ 2 ] != 0x61 )
 	{
-		libfguid_identifier_free(
-		 &guid,
-		 NULL );
+		return( 0 );
 	}
-	return( -1 );
-}
+	flags = data[ 3 ];
 
-/* Prints a property set value
- * Returns 1 if successful or -1 on error
- */
-int libfwsi_debug_print_property_set_value(
-     const uint8_t *byte_stream,
-     size_t byte_stream_size,
-     int ascii_codepage,
-     libcerror_error_t **error )
-{
-        libfwps_set_t *property_set = NULL;
-	static char *function       = "libfwsi_debug_print_property_set_value";
+	byte_stream_copy_to_uint16_little_endian(
+	 &( data[ 4 ] ),
+	 item_data_size );
 
-	if( libfwps_set_initialize(
-	     &property_set,
-	     error ) != 1 )
+#if defined( HAVE_DEBUG_OUTPUT )
+	if( libcnotify_verbose != 0 )
 	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
-		 "%s: unable to create property set.",
-		 function );
+		libcnotify_printf(
+		 "%s: flags\t\t\t\t\t: 0x%02" PRIx8 "\n",
+		 function,
+		 flags );
 
-		goto on_error;
+		libcnotify_printf(
+		 "%s: data size\t\t\t\t\t: %" PRIu16 "\n",
+		 function,
+		 item_data_size );
 	}
-	if( libfwps_set_copy_from_byte_stream(
-	     property_set,
-	     byte_stream,
-	     byte_stream_size,
-	     ascii_codepage,
-	     error ) != 1 )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
-		 "%s: unable to copy byte stream to property set.",
-		 function );
+#endif
+	data_offset = 6;
 
-		goto on_error;
-	}
-	if( libfwps_set_free(
-	     &property_set,
-	     error ) != 1 )
+	if( item_data_size > 0 )
 	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_FINALIZE_FAILED,
-		 "%s: unable to free property set.",
-		 function );
+		if( item_data_size > ( data_size - 6 ) )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+			 "%s: invalid data size value out of bounds.",
+			 function );
 
-		goto on_error;
+			return( -1 );
+		}
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
+		{
+			libcnotify_printf(
+			 "%s: data:\n",
+			 function );
+			libcnotify_print_data(
+			 &( data[ 6 ] ),
+			 item_data_size,
+			 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
+		}
+#endif
 	}
-	return( 1 );
-
-on_error:
-	if( property_set != NULL )
+#if defined( HAVE_DEBUG_OUTPUT )
+	else if( libcnotify_verbose != 0 )
 	{
-		libfwps_set_free(
-		 &property_set,
-		 NULL );
+		libcnotify_printf(
+		 "\n" );
 	}
-	return( -1 );
-}
-
-/* Prints a string value
- * Returns 1 if successful or -1 on error
- */
-int libfwsi_debug_print_string_value(
-     const char *function_name,
-     const char *value_name,
-     const uint8_t *byte_stream,
-     size_t byte_stream_size,
-     int ascii_codepage,
-     libcerror_error_t **error )
-{
-	system_character_t *string = NULL;
-	static char *function      = "libfwsi_debug_print_string_value";
-	size_t string_size         = 0;
-	int result                 = 0;
-
-#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
-	result = libuna_utf16_string_size_from_byte_stream(
-		  byte_stream,
-		  byte_stream_size,
-		  ascii_codepage,
-		  &string_size,
-		  error );
-#else
-	result = libuna_utf8_string_size_from_byte_stream(
-		  byte_stream,
-		  byte_stream_size,
-		  ascii_codepage,
-		  &string_size,
-		  error );
 #endif
-	if( result != 1 )
+	if( item_data_size >= 36 )
 	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-		 "%s: unable to determine size of string.",
-		 function );
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
+		{
+			byte_stream_copy_to_uint32_little_endian(
+			 &( data[ 6 ] ),
+			 value_32bit );
+			libcnotify_printf(
+			 "%s: unknown1\t\t\t\t\t: %" PRIu32 "\n",
+			 function,
+			 value_32bit );
+
+			byte_stream_copy_to_uint32_little_endian(
+			 &( data[ 10 ] ),
+			 value_32bit );
+			libcnotify_printf(
+			 "%s: unknown2\t\t\t\t\t: %" PRIu32 "\n",
+			 function,
+			 value_32bit );
+
+			if( libfwsi_debug_print_filetime_value(
+			     function,
+			     "unknown3 time\t\t\t\t",
+			     &( data[ 14 ] ),
+			     8,
+			     LIBFDATETIME_ENDIAN_LITTLE,
+			     LIBFDATETIME_STRING_FORMAT_TYPE_CTIME | LIBFDATETIME_STRING_FORMAT_FLAG_DATE_TIME_NANO_SECONDS,
+			     error ) != 1 )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+				 "%s: unable to print filetime value.",
+				 function );
+
+				return( -1 );
+			}
+			byte_stream_copy_to_uint32_little_endian(
+			 &( data[ 22 ] ),
+			 value_32bit );
+			libcnotify_printf(
+			 "%s: unknown4\t\t\t\t\t: 0x%08" PRIx32 "\n",
+			 function,
+			 value_32bit );
 
-		goto on_error;
-	}
-	if( ( string_size > (size_t) SSIZE_MAX )
-	 || ( ( sizeof( system_character_t ) * string_size ) > (size_t) SSIZE_MAX ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
-		 "%s: invalid string size value exceeds maximum.",
-		 function );
+			libcnotify_printf(
+			 "%s: unknown5:\n",
+			 function );
+			libcnotify_print_data(
+			 &( data[ 26 ] ),
+			 12,
+			 0 );
+
+			byte_stream_copy_to_uint32_little_endian(
+			 &( data[ 38 ] ),
+			 value_32bit );
+			libcnotify_printf(
+			 "%s: unknown6\t\t\t\t\t: %" PRIu32 "\n",
+			 function,
+			 value_32bit );
+		}
+#endif
+		data_offset    += 36;
+		item_data_size -= 36;
 
-		goto on_error;
-	}
-	string = system_string_allocate(
-			string_size );
+		if( data_offset >= ( data_size - 4 ) )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+			 "%s: invalid data size value out of bounds.",
+			 function );
 
-	if( string == NULL )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_MEMORY,
-		 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
-		 "%s: unable to create string.",
-		 function );
+			return( -1 );
+		}
+		byte_stream_copy_to_uint32_little_endian(
+		 &( data[ data_offset ] ),
+		 string_data_size );
 
-		goto on_error;
-	}
-#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
-	result = libuna_utf16_string_copy_from_byte_stream(
-		  (libuna_utf16_character_t *) string,
-		  string_size,
-		  byte_stream,
-		  byte_stream_size,
-		  ascii_codepage,
-		  error );
-#else
-	result = libuna_utf8_string_copy_from_byte_stream(
-		  (libuna_utf8_character_t *) string,
-		  string_size,
-		  byte_stream,
-		  byte_stream_size,
-		  ascii_codepage,
-		  error );
+		data_offset += 4;
+
+		if( ( item_data_size < 4 )
+		 || ( string_data_size > (uint32_t) ( item_data_size - 4 ) ) )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+			 "%s: invalid string1 data size value out of bounds.",
+			 function );
+
+			return( -1 );
+		}
+		item_data_size -= 4;
+
+		if( data_offset >= data_size )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+			 "%s: invalid data size value out of bounds.",
+			 function );
+
+			return( -1 );
+		}
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
+		{
+			libcnotify_printf(
+			 "%s: string1 data size\t\t\t\t: %" PRIu32 "\n",
+			 function,
+			 string_data_size );
+
+			libcnotify_printf(
+			 "%s: string1 data:\n",
+			 function );
+			libcnotify_print_data(
+			 &( data[ data_offset ] ),
+			 string_data_size,
+			 0 );
+		}
 #endif
-	if( result != 1 )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
-		 "%s: unable to set string.",
-		 function );
+		data_offset    += string_data_size;
+		item_data_size -= string_data_size;
 
-		goto on_error;
-	}
-	libcnotify_printf(
-	 "%s: %s: %s\n",
-	 function_name,
-	 value_name,
-	 string );
+		if( data_offset >= ( data_size - 4 ) )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+			 "%s: invalid data size value out of bounds.",
+			 function );
 
-	memory_free(
-	 string );
+			return( -1 );
+		}
+		byte_stream_copy_to_uint32_little_endian(
+		 &( data[ data_offset ] ),
+		 string_data_size );
 
-	return( 1 );
+		data_offset += 4;
 
-on_error:
-	if( string != NULL )
-	{
-		memory_free(
-		 string );
-	}
-	return( -1 );
-}
+		if( ( item_data_size < 4 )
+		 || ( string_data_size > (uint32_t) ( item_data_size - 4 ) ) )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+			 "%s: invalid string2 data size value out of bounds.",
+			 function );
 
-/* Prints an UTF-16 string value
- * Returns 1 if successful or -1 on error
- */
-int libfwsi_debug_print_utf16_string_value(
-     const char *function_name,
-     const char *value_name,
-     const uint8_t *byte_stream,
-     size_t byte_stream_size,
-     int byte_order,
-     libcerror_error_t **error )
-{
-	system_character_t *string = NULL;
-	static char *function      = "libfwsi_debug_print_utf16_string_value";
-	size_t string_size         = 0;
-	int result                 = 0;
+			return( -1 );
+		}
+		item_data_size -= 4;
+
+		if( data_offset >= data_size )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+			 "%s: invalid data size value out of bounds.",
+			 function );
+
+			return( -1 );
+		}
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
+		{
+			libcnotify_printf(
+			 "%s: string2 data size\t\t\t\t: %" PRIu32 "\n",
+			 function,
+			 string_data_size );
+
+			libcnotify_printf(
+			 "%s: string2 data:\n",
+			 function );
+			libcnotify_print_data(
+			 &( data[ data_offset ] ),
+			 string_data_size,
+			 0 );
+		}
+#endif
+		data_offset    += string_data_size;
+		item_data_size -= string_data_size;
+
+		if( data_offset >= ( data_size - 4 ) )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+			 "%s: invalid data size value out of bounds.",
+			 function );
+
+			return( -1 );
+		}
+		byte_stream_copy_to_uint32_little_endian(
+		 &( data[ data_offset ] ),
+		 string_data_size );
+
+		data_offset += 4;
+
+		if( ( item_data_size < 4 )
+		 || ( string_data_size > (uint32_t) ( item_data_size - 4 ) ) )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+			 "%s: invalid string3 data size value out of bounds.",
+			 function );
+
+			return( -1 );
+		}
+		item_data_size -= 4;
+
+		if( data_offset >= data_size )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+			 "%s: invalid data size value out of bounds.",
+			 function );
 
-	if( ( byte_stream == NULL )
-	 || ( byte_stream_size == 0 ) )
+			return( -1 );
+		}
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
+		{
+			libcnotify_printf(
+			 "%s: string3 data size\t\t\t\t: %" PRIu32 "\n",
+			 function,
+			 string_data_size );
+
+			if( string_data_size > item_data_size )
+			{
+				string_data_size = item_data_size;
+			}
+			libcnotify_printf(
+			 "%s: string3 data:\n",
+			 function );
+			libcnotify_print_data(
+			 &( data[ data_offset ] ),
+			 string_data_size,
+			 0 );
+		}
+#endif
+		data_offset    += string_data_size;
+		item_data_size -= string_data_size;
+	}
+	if( item_data_size > 0 )
 	{
-		libcnotify_printf(
-		 "%s: %s:\n",
-		 function_name,
-		 value_name );
-
-		return( 1 );
-	}
-#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
-	result = libuna_utf16_string_size_from_utf16_stream(
-	          byte_stream,
-	          byte_stream_size,
-	          byte_order,
-	          &string_size,
-	          error );
-#else
-	result = libuna_utf8_string_size_from_utf16_stream(
-	          byte_stream,
-	          byte_stream_size,
-	          byte_order,
-	          &string_size,
-	          error );
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
+		{
+			libcnotify_printf(
+			 "%s: trailing data:\n",
+			 function );
+			libcnotify_print_data(
+			 &( data[ data_offset ] ),
+			 item_data_size,
+			 0 );
+		}
 #endif
-	if( result != 1 )
+		data_offset += item_data_size;
+	}
+	if( data_offset >= data_size )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-		 "%s: unable to determine size of string.",
+		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+		 "%s: invalid data size value out of bounds.",
 		 function );
 
-		goto on_error;
+		return( -1 );
 	}
-	if( string_size > ( (size_t) SSIZE_MAX / sizeof( system_character_t ) ) )
+	/* Determine the URI size
+	 */
+	if( ( flags & 0x80 ) != 0 )
 	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
-		 "%s: invalid string size value exceeds maximum.",
-		 function );
+		for( string_size = data_offset;
+		     ( string_size + 1 ) < data_size;
+		     string_size += 2 )
+		{
+			if( ( data[ string_size ] == 0 )
+			 && ( data[ string_size + 1 ] == 0 ) )
+			{
+				string_size += 2;
 
-		goto on_error;
+				break;
+			}
+		}
+		string_size -= data_offset;
 	}
-	libcnotify_printf(
-	 "%s: %s:",
-	 function_name,
-	 value_name );
+	else
+	{
+		for( string_size = data_offset;
+		     string_size < data_size;
+		     string_size++ )
+		{
+			if( data[ string_size ] == 0 )
+			{
+				string_size++;
 
-	if( string_size > 0 )
+				break;
+			}
+		}
+		string_size -= data_offset;
+	}
+#if defined( HAVE_DEBUG_OUTPUT )
+	if( libcnotify_verbose != 0 )
 	{
-		string = system_string_allocate(
-		          string_size );
+		if( ( flags & 0x80 ) != 0 )
+		{
+			if( libfwsi_debug_print_utf16_string_value(
+			     function,
+			     "URI\t\t\t\t\t",
+			     &( data[ data_offset ] ),
+			     string_size,
+			     LIBUNA_ENDIAN_LITTLE,
+			     error ) != 1 )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+				 "%s: unable to print UTF-16 string value.",
+				 function );
 
-		if( string == NULL )
+				return( -1 );
+			}
+		}
+		else
 		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_MEMORY,
-			 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
-			 "%s: unable to create string.",
-			 function );
+			if( libfwsi_debug_print_string_value(
+			     function,
+			     "URI\t\t\t\t\t",
+			     &( data[ data_offset ] ),
+			     string_size,
+			     ascii_codepage,
+			     error ) != 1 )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+				 "%s: unable to print string value.",
+				 function );
 
-			goto on_error;
+				return( -1 );
+			}
 		}
-#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
-		result = libuna_utf16_string_copy_from_utf16_stream(
-		          (libuna_utf16_character_t *) string,
-		          string_size,
-		          byte_stream,
-		          byte_stream_size,
-		          byte_order,
-		          error );
-#else
-		result = libuna_utf8_string_copy_from_utf16_stream(
-		          (libuna_utf8_character_t *) string,
-		          string_size,
-		          byte_stream,
-		          byte_stream_size,
-		          byte_order,
-		          error );
+	}
 #endif
-		if( result != 1 )
+	data_offset += string_size;
+
+/* TODO value likely controlled by flags */
+	if( data_offset < data_size )
+	{
+		if( data_offset >= ( data_size - 2 ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
-			 "%s: unable to set string.",
+			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+			 "%s: invalid data size value out of bounds.",
 			 function );
 
-			goto on_error;
+			return( -1 );
 		}
-		libcnotify_printf(
-		 " %s",
-		 string );
-
-		memory_free(
-		 string );
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
+		{
+			byte_stream_copy_to_uint16_little_endian(
+			 &( data[ data_offset ] ),
+			 value_16bit );
+
+			libcnotify_printf(
+			 "%s: unknown9\t\t\t\t\t: %" PRIu16 "\n",
+			 function,
+			 value_16bit );
+		}
+#endif
+		data_offset += 2;
 	}
-	libcnotify_printf(
-	 "\n" );
-
-	return( 1 );
-
-on_error:
-	if( string != NULL )
+#if defined( HAVE_DEBUG_OUTPUT )
+	if( libcnotify_verbose != 0 )
 	{
-		memory_free(
-		 string );
+		libcnotify_printf(
+		 "\n" );
 	}
-	return( -1 );
+#endif
+	return( 1 );
 }
 
-#endif /* defined( HAVE_DEBUG_OUTPUT ) */
-
```

### Comparing `libfwsi-20230114/libfwsi/libfwsi_shell_folder_identifier.c` & `libfwsi-20230710/libfwsi/libfwsi_shell_folder_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi.rc` & `libfwsi-20230710/libfwsi/libfwsi.rc`

 * *Files 22% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Windows Shell Item format\0"
-      VALUE "FileVersion",		"20230114" "\0"
+      VALUE "FileVersion",		"20230710" "\0"
       VALUE "InternalName",		"libfwsi.dll\0"
       VALUE "LegalCopyright",		"(C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfwsi.dll\0"
       VALUE "ProductName",		"libfwsi\0"
-      VALUE "ProductVersion",		"20230114" "\0"
+      VALUE "ProductVersion",		"20230710" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfwsi/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfwsi-20230114/libfwsi/libfwsi_file_attributes.h` & `libfwsi-20230710/libfwsi/libfwsi_file_attributes.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_volume.c` & `libfwsi-20230710/libfwsi/libfwsi_volume.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_notify.c` & `libfwsi-20230710/libfwsi/libfwsi_notify.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0025_values.h` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0025_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_uri_values.h` & `libfwsi-20230710/libfwsi/libfwsi_uri_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_known_folder_identifier.c` & `libfwsi-20230710/libfwsi/libfwsi_known_folder_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_unknown_0x74_values.h` & `libfwsi-20230710/libfwsi/libfwsi_unknown_0x74_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0005_values.c` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0005_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_definitions.h.in` & `libfwsi-20230710/libfwsi/libfwsi_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_network_location.h` & `libfwsi-20230710/libfwsi/libfwsi_network_location.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_mtp_volume_values.c` & `libfwsi-20230710/libfwsi/libfwsi_mtp_volume_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_game_folder_values.h` & `libfwsi-20230710/libfwsi/libfwsi_game_folder_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_support.h` & `libfwsi-20230710/libcdata/libcdata_support.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,33 +15,33 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFWSI_SUPPORT_H )
-#define _LIBFWSI_SUPPORT_H
+#if !defined( _LIBCDATA_SUPPORT_H )
+#define _LIBCDATA_SUPPORT_H
 
 #include <common.h>
 #include <types.h>
 
-#include "libfwsi_extern.h"
+#include "libcdata_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-#if !defined( HAVE_LOCAL_LIBFWSI )
+#if !defined( HAVE_LOCAL_LIBCDATA )
 
-LIBFWSI_EXTERN \
-const char *libfwsi_get_version(
+LIBCDATA_EXTERN \
+const char *libcdata_get_version(
              void );
 
-#endif
+#endif /* !defined( HAVE_LOCAL_LIBCDATA ) */
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBFWSI_SUPPORT_H ) */
+#endif /* !defined( _LIBCDATA_SUPPORT_H ) */
```

### Comparing `libfwsi-20230114/libfwsi/libfwsi_mtp_file_entry_values.c` & `libfwsi-20230710/libfwsi/libfwsi_mtp_file_entry_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_unused.h` & `libfwsi-20230710/libfwsi/libfwsi_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_root_folder_values.c` & `libfwsi-20230710/libfwsi/libfwsi_root_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_uri_values.c` & `libfwsi-20230710/libfwsi/libfwsi_users_property_view_values.c`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * URI (shell item) values functions
+ * Users property view (shell item) values functions
  *
  * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
@@ -21,152 +21,153 @@
 
 #include <common.h>
 #include <byte_stream.h>
 #include <memory.h>
 #include <types.h>
 
 #include "libfwsi_debug.h"
+#include "libfwsi_known_folder_identifier.h"
 #include "libfwsi_libcerror.h"
 #include "libfwsi_libcnotify.h"
-#include "libfwsi_libfdatetime.h"
-#include "libfwsi_libuna.h"
-#include "libfwsi_uri_values.h"
+#include "libfwsi_libfguid.h"
+#include "libfwsi_shell_folder_identifier.h"
+#include "libfwsi_users_property_view_values.h"
 
-/* Creates URI values
- * Make sure the value uri_values is referencing, is set to NULL
+/* Creates users property view values
+ * Make sure the value users_property_view_values is referencing, is set to NULL
  * Returns 1 if successful or -1 on error
  */
-int libfwsi_uri_values_initialize(
-     libfwsi_uri_values_t **uri_values,
+int libfwsi_users_property_view_values_initialize(
+     libfwsi_users_property_view_values_t **users_property_view_values,
      libcerror_error_t **error )
 {
-	static char *function = "libfwsi_uri_values_initialize";
+	static char *function = "libfwsi_users_property_view_values_initialize";
 
-	if( uri_values == NULL )
+	if( users_property_view_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid URI values.",
+		 "%s: invalid users property view values.",
 		 function );
 
 		return( -1 );
 	}
-	if( *uri_values != NULL )
+	if( *users_property_view_values != NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_VALUE_ALREADY_SET,
-		 "%s: invalid URI values value already set.",
+		 "%s: invalid users property view values value already set.",
 		 function );
 
 		return( -1 );
 	}
-	*uri_values = memory_allocate_structure(
-	               libfwsi_uri_values_t );
+	*users_property_view_values = memory_allocate_structure(
+	                               libfwsi_users_property_view_values_t );
 
-	if( *uri_values == NULL )
+	if( *users_property_view_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_MEMORY,
 		 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
-		 "%s: unable to create URI values.",
+		 "%s: unable to create users property view values.",
 		 function );
 
 		goto on_error;
 	}
 	if( memory_set(
-	     *uri_values,
+	     *users_property_view_values,
 	     0,
-	     sizeof( libfwsi_uri_values_t ) ) == NULL )
+	     sizeof( libfwsi_users_property_view_values_t ) ) == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_MEMORY,
 		 LIBCERROR_MEMORY_ERROR_SET_FAILED,
-		 "%s: unable to clear URI values.",
+		 "%s: unable to clear users property view values.",
 		 function );
 
 		goto on_error;
 	}
 	return( 1 );
 
 on_error:
-	if( *uri_values != NULL )
+	if( *users_property_view_values != NULL )
 	{
 		memory_free(
-		 *uri_values );
+		 *users_property_view_values );
 
-		*uri_values = NULL;
+		*users_property_view_values = NULL;
 	}
 	return( -1 );
 }
 
-/* Frees URI values
+/* Frees users property view values
  * Returns 1 if successful or -1 on error
  */
-int libfwsi_uri_values_free(
-     libfwsi_uri_values_t **uri_values,
+int libfwsi_users_property_view_values_free(
+     libfwsi_users_property_view_values_t **users_property_view_values,
      libcerror_error_t **error )
 {
-	static char *function = "libfwsi_uri_values_free";
+	static char *function = "libfwsi_users_property_view_values_free";
 
-	if( uri_values == NULL )
+	if( users_property_view_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid URI values.",
+		 "%s: invalid users property view values.",
 		 function );
 
 		return( -1 );
 	}
-	if( *uri_values != NULL )
+	if( *users_property_view_values != NULL )
 	{
 		memory_free(
-		 *uri_values );
+		 *users_property_view_values );
 
-		*uri_values = NULL;
+		*users_property_view_values = NULL;
 	}
 	return( 1 );
 }
 
-/* Reads the URI values
+/* Reads the users property view values
  * Returns 1 if successful, 0 if not supported or -1 on error
  */
-int libfwsi_uri_values_read_data(
-     libfwsi_uri_values_t *uri_values,
+int libfwsi_users_property_view_values_read_data(
+     libfwsi_users_property_view_values_t *users_property_view_values,
      const uint8_t *data,
      size_t data_size,
      int ascii_codepage,
      libcerror_error_t **error )
 {
-	static char *function     = "libfwsi_uri_values_read_data";
-	size_t data_offset        = 0;
-	size_t string_size        = 0;
-	uint32_t string_data_size = 0;
-	uint16_t item_data_size   = 0;
-	uint8_t flags             = 0;
+	static char *function      = "libfwsi_users_property_view_values_read_data";
+	size_t data_offset         = 0;
+	uint32_t signature         = 0;
+	uint16_t identifier_size   = 0;
+	uint16_t item_data_size    = 0;
+	uint16_t property_set_size = 0;
 
 #if defined( HAVE_DEBUG_OUTPUT )
-	uint32_t value_32bit      = 0;
-	uint16_t value_16bit      = 0;
+	uint32_t value_32bit       = 0;
+	uint16_t value_16bit       = 0;
 #endif
 
-	if( uri_values == NULL )
+	if( users_property_view_values == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
-		 "%s: invalid URI values.",
+		 "%s: invalid users property view values.",
 		 function );
 
 		return( -1 );
 	}
 	if( data == NULL )
 	{
 		libcerror_error_set(
@@ -187,471 +188,294 @@
 		 "%s: data size exceeds maximum.",
 		 function );
 
 		return( -1 );
 	}
 	/* Do not try to parse unsupported data sizes
 	 */
-	if( data_size < 6 )
+	if( data_size < 14 )
 	{
 		return( 0 );
 	}
-	/* Do not try to parse unknown class type indicators
+	/* Do not try to parse unsupported shell item signatures
 	 */
-	if( data[ 2 ] != 0x61 )
-	{
-		return( 0 );
-	}
-	flags = data[ 3 ];
+	byte_stream_copy_to_uint32_little_endian(
+	 &( data[ 6 ] ),
+	 signature );
+
+	switch( signature )
+	{
+		case 0x10141981UL:
+		case 0x23a3dfd5UL:
+		case 0x23febbeeUL:
+		case 0x3b93afbbUL:
+		case 0xbeebee00UL:
+			break;
 
-	byte_stream_copy_to_uint16_little_endian(
+		default:
+			return( 0 );
+	}
+	byte_stream_copy_to_uint32_little_endian(
 	 &( data[ 4 ] ),
 	 item_data_size );
 
+	byte_stream_copy_to_uint16_little_endian(
+	 &( data[ 10 ] ),
+	 property_set_size );
+
+	byte_stream_copy_to_uint16_little_endian(
+	 &( data[ 12 ] ),
+	 identifier_size );
+
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
 		libcnotify_printf(
-		 "%s: flags\t\t\t\t\t: 0x%02" PRIx8 "\n",
+		 "%s: class type indicator\t: 0x%02" PRIx8 "\n",
+		 function,
+		 data[ 2 ] );
+
+		libcnotify_printf(
+		 "%s: unknown1\t\t\t: 0x%02" PRIx8 "\n",
 		 function,
-		 flags );
+		 data[ 3 ] );
 
 		libcnotify_printf(
-		 "%s: data size\t\t\t\t\t: %" PRIu16 "\n",
+		 "%s: data size\t\t\t: %" PRIu16 "\n",
 		 function,
 		 item_data_size );
+
+		libcnotify_printf(
+		 "%s: data signature\t\t: 0x%08" PRIx32 "\n",
+		 function,
+		 signature );
+
+		libcnotify_printf(
+		 "%s: property set size\t: %" PRIu16 "\n",
+		 function,
+		 property_set_size );
+
+		libcnotify_printf(
+		 "%s: identifier size\t\t: %" PRIu16 "\n",
+		 function,
+		 identifier_size );
 	}
 #endif
-	data_offset = 6;
+	data_offset = 14;
 
-	if( item_data_size > 0 )
+	if( item_data_size != 0 )
 	{
-		if( item_data_size > ( data_size - 6 ) )
+		if( item_data_size <= 2 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
 			 "%s: invalid data size value out of bounds.",
 			 function );
 
 			return( -1 );
 		}
+	}
+/* TODO add identifier_size bounds check */
 #if defined( HAVE_DEBUG_OUTPUT )
-		if( libcnotify_verbose != 0 )
-		{
-			libcnotify_printf(
-			 "%s: data:\n",
-			 function );
-			libcnotify_print_data(
-			 &( data[ 6 ] ),
-			 item_data_size,
-			 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
-		}
+	if( libcnotify_verbose != 0 )
+	{
+		libcnotify_printf(
+		 "%s: identifier data:\n",
+		 function );
+		libcnotify_print_data(
+		 &( data[ data_offset ] ),
+		 identifier_size,
+		 0 );
+	}
+#endif
+	switch( signature )
+	{
+		case 0x23a3dfd5UL:
+		case 0x3b93afbbUL:
+		case 0xbeebee00UL:
+			if( identifier_size == 4 )
+			{
+#if defined( HAVE_DEBUG_OUTPUT )
+				if( libcnotify_verbose != 0 )
+				{
+					byte_stream_copy_to_uint32_little_endian(
+					 &( data[ data_offset ] ),
+					 value_32bit );
+					libcnotify_printf(
+					 "%s: identifier\t\t\t: 0x%08" PRIx32 "\n",
+					 function,
+					 value_32bit );
+				}
+#endif
+				data_offset += 4;
+			}
+			break;
+
+		case 0x23febbeeUL:
+			if( identifier_size == 16 )
+			{
+#if defined( HAVE_DEBUG_OUTPUT )
+				if( libcnotify_verbose != 0 )
+				{
+					if( libfwsi_debug_print_guid_value(
+					     function,
+					     "known folder identifier\t",
+					     &( data[ data_offset ] ),
+					     16,
+					     LIBFGUID_ENDIAN_LITTLE,
+					     LIBFGUID_STRING_FORMAT_FLAG_USE_UPPER_CASE | LIBFGUID_STRING_FORMAT_FLAG_USE_SURROUNDING_BRACES,
+					     error ) != 1 )
+					{
+						libcerror_error_set(
+						 error,
+						 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+						 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+						 "%s: unable to print GUID value.",
+						 function );
+
+						return( -1 );
+					}
+					libcnotify_printf(
+					 "%s: known folder name\t\t: %s\n",
+					 function,
+					 libfwsi_known_folder_identifier_get_name(
+					  &( data[ data_offset ] ) ) );
+				}
 #endif
+				data_offset += 16;
+			}
+			break;
+
+		default:
+			data_offset += identifier_size;
+			break;
 	}
+/* TODO add property set size bounds check */
+
 #if defined( HAVE_DEBUG_OUTPUT )
-	else if( libcnotify_verbose != 0 )
+	if( libcnotify_verbose != 0 )
 	{
 		libcnotify_printf(
-		 "\n" );
+		 "%s: property set data:\n",
+		 function );
+		libcnotify_print_data(
+		 &( data[ data_offset ] ),
+		 property_set_size,
+		 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 	}
 #endif
-	if( item_data_size >= 36 )
+	if( property_set_size > 0 )
 	{
+/* TODO look for multiple sets (property store) */
 #if defined( HAVE_DEBUG_OUTPUT )
 		if( libcnotify_verbose != 0 )
 		{
-			byte_stream_copy_to_uint32_little_endian(
-			 &( data[ 6 ] ),
-			 value_32bit );
-			libcnotify_printf(
-			 "%s: unknown1\t\t\t\t\t: %" PRIu32 "\n",
-			 function,
-			 value_32bit );
-
-			byte_stream_copy_to_uint32_little_endian(
-			 &( data[ 10 ] ),
-			 value_32bit );
-			libcnotify_printf(
-			 "%s: unknown2\t\t\t\t\t: %" PRIu32 "\n",
-			 function,
-			 value_32bit );
-
-			if( libfwsi_debug_print_filetime_value(
-			     function,
-			     "unknown3 time\t\t\t\t",
-			     &( data[ 14 ] ),
-			     8,
-			     LIBFDATETIME_ENDIAN_LITTLE,
-			     LIBFDATETIME_STRING_FORMAT_TYPE_CTIME | LIBFDATETIME_STRING_FORMAT_FLAG_DATE_TIME_NANO_SECONDS,
+			if( libfwsi_debug_print_property_set_value(
+			     &( data[ data_offset ] ),
+			     property_set_size,
+			     ascii_codepage,
 			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
-				 "%s: unable to print filetime value.",
+				 "%s: unable to print property set value.",
 				 function );
 
 				return( -1 );
 			}
-			byte_stream_copy_to_uint32_little_endian(
-			 &( data[ 22 ] ),
-			 value_32bit );
-			libcnotify_printf(
-			 "%s: unknown4\t\t\t\t\t: 0x%08" PRIx32 "\n",
-			 function,
-			 value_32bit );
-
-			libcnotify_printf(
-			 "%s: unknown5:\n",
-			 function );
-			libcnotify_print_data(
-			 &( data[ 26 ] ),
-			 12,
-			 0 );
-
-			byte_stream_copy_to_uint32_little_endian(
-			 &( data[ 38 ] ),
-			 value_32bit );
-			libcnotify_printf(
-			 "%s: unknown6\t\t\t\t\t: %" PRIu32 "\n",
-			 function,
-			 value_32bit );
 		}
 #endif
-		data_offset    += 36;
-		item_data_size -= 36;
-
-		if( data_offset >= ( data_size - 4 ) )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-			 "%s: invalid data size value out of bounds.",
-			 function );
-
-			return( -1 );
-		}
-		byte_stream_copy_to_uint32_little_endian(
-		 &( data[ data_offset ] ),
-		 string_data_size );
-
-		data_offset += 4;
-
-		if( ( item_data_size < 4 )
-		 || ( string_data_size > (uint32_t) ( item_data_size - 4 ) ) )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-			 "%s: invalid string1 data size value out of bounds.",
-			 function );
-
-			return( -1 );
-		}
-		item_data_size -= 4;
-
-		if( data_offset >= data_size )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-			 "%s: invalid data size value out of bounds.",
-			 function );
-
-			return( -1 );
-		}
+		data_offset += property_set_size;
+	}
 #if defined( HAVE_DEBUG_OUTPUT )
-		if( libcnotify_verbose != 0 )
-		{
-			libcnotify_printf(
-			 "%s: string1 data size\t\t\t\t: %" PRIu32 "\n",
-			 function,
-			 string_data_size );
-
-			libcnotify_printf(
-			 "%s: string1 data:\n",
-			 function );
-			libcnotify_print_data(
-			 &( data[ data_offset ] ),
-			 string_data_size,
-			 0 );
-		}
-#endif
-		data_offset    += string_data_size;
-		item_data_size -= string_data_size;
-
-		if( data_offset >= ( data_size - 4 ) )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-			 "%s: invalid data size value out of bounds.",
-			 function );
-
-			return( -1 );
-		}
-		byte_stream_copy_to_uint32_little_endian(
+	if( libcnotify_verbose != 0 )
+	{
+		byte_stream_copy_to_uint16_little_endian(
 		 &( data[ data_offset ] ),
-		 string_data_size );
+		 value_16bit );
 
-		data_offset += 4;
-
-		if( ( item_data_size < 4 )
-		 || ( string_data_size > (uint32_t) ( item_data_size - 4 ) ) )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-			 "%s: invalid string2 data size value out of bounds.",
-			 function );
-
-			return( -1 );
-		}
-		item_data_size -= 4;
-
-		if( data_offset >= data_size )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-			 "%s: invalid data size value out of bounds.",
-			 function );
-
-			return( -1 );
-		}
-#if defined( HAVE_DEBUG_OUTPUT )
-		if( libcnotify_verbose != 0 )
-		{
-			libcnotify_printf(
-			 "%s: string2 data size\t\t\t\t: %" PRIu32 "\n",
-			 function,
-			 string_data_size );
-
-			libcnotify_printf(
-			 "%s: string2 data:\n",
-			 function );
-			libcnotify_print_data(
-			 &( data[ data_offset ] ),
-			 string_data_size,
-			 0 );
-		}
+		libcnotify_printf(
+		 "%s: unknown1 size\t\t: %" PRIu16 "\n",
+		 function,
+		 value_16bit );
+	}
 #endif
-		data_offset    += string_data_size;
-		item_data_size -= string_data_size;
-
-		if( data_offset >= ( data_size - 4 ) )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-			 "%s: invalid data size value out of bounds.",
-			 function );
-
-			return( -1 );
-		}
-		byte_stream_copy_to_uint32_little_endian(
-		 &( data[ data_offset ] ),
-		 string_data_size );
-
-		data_offset += 4;
+	data_offset += 2;
 
-		if( ( item_data_size < 4 )
-		 || ( string_data_size > (uint32_t) ( item_data_size - 4 ) ) )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-			 "%s: invalid string3 data size value out of bounds.",
-			 function );
-
-			return( -1 );
-		}
-		item_data_size -= 4;
-
-		if( data_offset >= data_size )
+	if( signature == 0x23a3dfd5UL )
+	{
+		if( data_offset > data_size - 32 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
 			 "%s: invalid data size value out of bounds.",
 			 function );
 
 			return( -1 );
 		}
 #if defined( HAVE_DEBUG_OUTPUT )
 		if( libcnotify_verbose != 0 )
 		{
-			libcnotify_printf(
-			 "%s: string3 data size\t\t\t\t: %" PRIu32 "\n",
-			 function,
-			 string_data_size );
-
-			if( string_data_size > item_data_size )
-			{
-				string_data_size = item_data_size;
-			}
-			libcnotify_printf(
-			 "%s: string3 data:\n",
-			 function );
-			libcnotify_print_data(
-			 &( data[ data_offset ] ),
-			 string_data_size,
-			 0 );
-		}
-#endif
-		data_offset    += string_data_size;
-		item_data_size -= string_data_size;
-	}
-	if( item_data_size > 0 )
-	{
-#if defined( HAVE_DEBUG_OUTPUT )
-		if( libcnotify_verbose != 0 )
-		{
-			libcnotify_printf(
-			 "%s: trailing data:\n",
-			 function );
-			libcnotify_print_data(
-			 &( data[ data_offset ] ),
-			 item_data_size,
-			 0 );
-		}
-#endif
-		data_offset += item_data_size;
-	}
-	if( data_offset >= data_size )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-		 "%s: invalid data size value out of bounds.",
-		 function );
-
-		return( -1 );
-	}
-	/* Determine the URI size
-	 */
-	if( ( flags & 0x80 ) != 0 )
-	{
-		for( string_size = data_offset;
-		     ( string_size + 1 ) < data_size;
-		     string_size += 2 )
-		{
-			if( ( data[ string_size ] == 0 )
-			 && ( data[ string_size + 1 ] == 0 ) )
-			{
-				string_size += 2;
-
-				break;
-			}
-		}
-		string_size -= data_offset;
-	}
-	else
-	{
-		for( string_size = data_offset;
-		     string_size < data_size;
-		     string_size++ )
-		{
-			if( data[ string_size ] == 0 )
-			{
-				string_size++;
-
-				break;
-			}
-		}
-		string_size -= data_offset;
-	}
-#if defined( HAVE_DEBUG_OUTPUT )
-	if( libcnotify_verbose != 0 )
-	{
-		if( ( flags & 0x80 ) != 0 )
-		{
-			if( libfwsi_debug_print_utf16_string_value(
+			if( libfwsi_debug_print_guid_value(
 			     function,
-			     "URI\t\t\t\t\t",
+			     "delegate item identifier\t",
 			     &( data[ data_offset ] ),
-			     string_size,
-			     LIBUNA_ENDIAN_LITTLE,
+			     16,
+			     LIBFGUID_ENDIAN_LITTLE,
+			     LIBFGUID_STRING_FORMAT_FLAG_USE_UPPER_CASE | LIBFGUID_STRING_FORMAT_FLAG_USE_SURROUNDING_BRACES,
 			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
-				 "%s: unable to print UTF-16 string value.",
+				 "%s: unable to print GUID value.",
 				 function );
 
 				return( -1 );
 			}
 		}
-		else
+#endif
+		data_offset += 16;
+
+#if defined( HAVE_DEBUG_OUTPUT )
+		if( libcnotify_verbose != 0 )
 		{
-			if( libfwsi_debug_print_string_value(
+			if( libfwsi_debug_print_guid_value(
 			     function,
-			     "URI\t\t\t\t\t",
+			     "item class identifier\t\t",
 			     &( data[ data_offset ] ),
-			     string_size,
-			     ascii_codepage,
+			     16,
+			     LIBFGUID_ENDIAN_LITTLE,
+			     LIBFGUID_STRING_FORMAT_FLAG_USE_UPPER_CASE | LIBFGUID_STRING_FORMAT_FLAG_USE_SURROUNDING_BRACES,
 			     error ) != 1 )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
-				 "%s: unable to print string value.",
+				 "%s: unable to print GUID value.",
 				 function );
 
 				return( -1 );
 			}
-		}
-	}
-#endif
-	data_offset += string_size;
-
-/* TODO value likely controlled by flags */
-	if( data_offset < data_size )
-	{
-		if( data_offset >= ( data_size - 2 ) )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
-			 "%s: invalid data size value out of bounds.",
-			 function );
-
-			return( -1 );
-		}
-#if defined( HAVE_DEBUG_OUTPUT )
-		if( libcnotify_verbose != 0 )
-		{
-			byte_stream_copy_to_uint16_little_endian(
-			 &( data[ data_offset ] ),
-			 value_16bit );
-
 			libcnotify_printf(
-			 "%s: unknown9\t\t\t\t\t: %" PRIu16 "\n",
+			 "%s: shell folder name\t\t: %s\n",
 			 function,
-			 value_16bit );
+			 libfwsi_shell_folder_identifier_get_name(
+			  &( data[ data_offset ] ) ) );
 		}
 #endif
-		data_offset += 2;
+		data_offset += 16;
 	}
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
 		libcnotify_printf(
 		 "\n" );
 	}
```

### Comparing `libfwsi-20230114/libfwsi/libfwsi_item.h` & `libfwsi-20230710/libfwsi/libfwsi_item.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_compressed_folder_values.h` & `libfwsi-20230710/libfwsi/libfwsi_compressed_folder_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_libfguid.h` & `libfwsi-20230710/libfwsi/libfwsi_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_file_entry.h` & `libfwsi-20230710/libfwsi/libfwsi_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_volume.h` & `libfwsi-20230710/libfwsi/libfwsi_volume.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_control_panel_identifier.h` & `libfwsi-20230710/libfwsi/libfwsi_control_panel_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef000a_values.c` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef000a_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_root_folder.c` & `libfwsi-20230710/libfwsi/libfwsi_root_folder.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_control_panel_category_values.c` & `libfwsi-20230710/libfwsi/libfwsi_control_panel_category_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_debug.h` & `libfwsi-20230710/libfwsi/libfwsi_debug.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/Makefile.in` & `libfwsi-20230710/libfwsi/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0000_values.c` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0000_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0001_values.c` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0001_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_control_panel_values.c` & `libfwsi-20230710/libfwsi/libfwsi_control_panel_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_network_location_values.c` & `libfwsi-20230710/libfwsi/libfwsi_network_location_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0003_values.h` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0003_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_cdburn_values.c` & `libfwsi-20230710/libfwsi/libfwsi_cdburn_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block.c` & `libfwsi-20230710/libfwsi/libfwsi_extension_block.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_error.c` & `libfwsi-20230710/libfwsi/libfwsi_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_error.h` & `libfwsi-20230710/libfwsi/libfwsi_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0005_values.h` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0005_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_uri_sub_values.c` & `libfwsi-20230710/libfwsi/libfwsi_uri_sub_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block.h` & `libfwsi-20230710/libfwsi/libfwsi_extension_block.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extern.h` & `libfwsi-20230710/libfwsi/libfwsi_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_known_folder_identifier.h` & `libfwsi-20230710/libfwsi/libfwsi_known_folder_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_control_panel_category_values.h` & `libfwsi-20230710/libfwsi/libfwsi_control_panel_category_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_control_panel_cpl_file_values.h` & `libfwsi-20230710/libfwsi/libfwsi_control_panel_cpl_file_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_item_list.c` & `libfwsi-20230710/libfwsi/libfwsi_item_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_definitions.h` & `libfwsi-20230710/libfwsi/libfwsi_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwsi/definitions.h> are copied here
  * for local use of libfwsi
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWSI_VERSION					20230114
+#define LIBFWSI_VERSION					20230710
 
 /* The version string
  */
-#define LIBFWSI_VERSION_STRING				"20230114"
+#define LIBFWSI_VERSION_STRING				"20230710"
 
 /* The byte order definitions
  */
 #define LIBFWSI_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWSI_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The item type definitions
```

### Comparing `libfwsi-20230114/libfwsi/libfwsi_libcnotify.h` & `libfwsi-20230710/libfwsi/libfwsi_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_file_entry_extension.c` & `libfwsi-20230710/libfwsi/libfwsi_file_entry_extension.c`

 * *Files 6% similar despite different names*

```diff
@@ -228,14 +228,16 @@
 	}
 	*file_reference = file_entry_extension_values->file_reference;
 
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-8 formatted long name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 int libfwsi_file_entry_extension_get_utf8_long_name_size(
      libfwsi_extension_block_t *file_entry_extension,
      size_t *utf8_string_size,
      libcerror_error_t **error )
 {
@@ -284,15 +286,15 @@
 	 || ( file_entry_extension_values->long_name_size == 0 ) )
 	{
 		return( 0 );
 	}
 	if( libuna_utf8_string_size_from_utf16_stream(
 	     file_entry_extension_values->long_name,
 	     file_entry_extension_values->long_name_size,
-	     LIBUNA_ENDIAN_LITTLE,
+	     LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 	     utf8_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
@@ -301,14 +303,16 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-8 formatted long name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 int libfwsi_file_entry_extension_get_utf8_long_name(
      libfwsi_extension_block_t *file_entry_extension,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      libcerror_error_t **error )
@@ -360,15 +364,15 @@
 		return( 0 );
 	}
 	if( libuna_utf8_string_copy_from_utf16_stream(
 	     utf8_string,
 	     utf8_string_size,
 	     file_entry_extension_values->long_name,
 	     file_entry_extension_values->long_name_size,
-	     LIBUNA_ENDIAN_LITTLE,
+	     LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
 		 "%s: unable to set UTF-8 string.",
@@ -376,14 +380,16 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-16 formatted long name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 int libfwsi_file_entry_extension_get_utf16_long_name_size(
      libfwsi_extension_block_t *file_entry_extension,
      size_t *utf16_string_size,
      libcerror_error_t **error )
 {
@@ -432,15 +438,15 @@
 	 || ( file_entry_extension_values->long_name_size == 0 ) )
 	{
 		return( 0 );
 	}
 	if( libuna_utf16_string_size_from_utf16_stream(
 	     file_entry_extension_values->long_name,
 	     file_entry_extension_values->long_name_size,
-	     LIBUNA_ENDIAN_LITTLE,
+	     LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 	     utf16_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
@@ -449,14 +455,16 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-16 formatted long name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 int libfwsi_file_entry_extension_get_utf16_long_name(
      libfwsi_extension_block_t *file_entry_extension,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      libcerror_error_t **error )
@@ -508,15 +516,15 @@
 		return( 0 );
 	}
 	if( libuna_utf16_string_copy_from_utf16_stream(
 	     utf16_string,
 	     utf16_string_size,
 	     file_entry_extension_values->long_name,
 	     file_entry_extension_values->long_name_size,
-	     LIBUNA_ENDIAN_LITTLE,
+	     LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
 		 "%s: unable to set UTF-16 string.",
```

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0019_values.c` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0019_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_extension_block_0xbeef0006_values.h` & `libfwsi-20230710/libfwsi/libfwsi_extension_block_0xbeef0006_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_network_location.c` & `libfwsi-20230710/libfwsi/libfwsi_network_location.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_file_entry_values.h` & `libfwsi-20230710/libfwsi/libfwsi_file_entry_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_mtp_file_entry_values.h` & `libfwsi-20230710/libfwsi/libfwsi_mtp_file_entry_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libfwsi/libfwsi_item.c` & `libfwsi-20230710/libfwsi/libfwsi_item.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/Makefile.in` & `libfwsi-20230710/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/ChangeLog` & `libfwsi-20230710/ChangeLog`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/libuna.m4` & `libfwsi-20230710/m4/libuna.m4`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20210801
+dnl Version: 20230702
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -39,15 +39,15 @@
         ])
       ],
       [dnl Check for a pkg-config file
       AS_IF(
         [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
         [PKG_CHECK_MODULES(
           [libuna],
-          [libuna >= 20210801],
+          [libuna >= 20230702],
           [ac_cv_libuna=yes],
           [ac_cv_libuna=check])
         ])
       AS_IF(
         [test "x$ac_cv_libuna" = xyes],
         [ac_cv_libuna_CPPFLAGS="$pkg_cv_libuna_CFLAGS"
         ac_cv_libuna_LIBADD="$pkg_cv_libuna_LIBS"])
@@ -221,14 +221,146 @@
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_byte_stream_copy_from_utf32,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
 
+        dnl Unicode character functions
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_size_to_byte_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_byte_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_byte_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_size_to_ucs2,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_ucs2,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_ucs2,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_size_to_ucs4,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_ucs4,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_ucs4,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_utf7_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_utf7_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_size_to_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_size_to_utf8_rfc2279,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_utf8_rfc2279,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_utf8_rfc2279,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_size_to_utf16,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_utf16,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_utf16,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_utf16_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_utf16_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_utf32,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_utf32,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_utf32_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_utf32_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+
         dnl UTF-8 stream functions
         AC_CHECK_LIB(
           una,
           libuna_utf8_stream_size_from_utf8,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
@@ -335,14 +467,19 @@
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_with_index_copy_from_byte_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf8_string_compare_with_byte_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
           libuna_utf8_string_size_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_copy_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
@@ -350,14 +487,19 @@
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_with_index_copy_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf8_string_compare_with_utf7_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
           libuna_utf8_string_size_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_copy_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
@@ -365,55 +507,55 @@
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_with_index_copy_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_size_from_utf16_stream,
+          libuna_utf8_string_compare_with_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_copy_from_utf16_stream,
+          libuna_utf8_string_size_from_utf16,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_with_index_copy_from_utf16_stream,
+          libuna_utf8_string_copy_from_utf16,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_size_from_utf32_stream,
+          libuna_utf8_string_with_index_copy_from_utf16,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_copy_from_utf32_stream,
+          libuna_utf8_string_compare_with_utf16,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_with_index_copy_from_utf32_stream,
+          libuna_utf8_string_size_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_size_from_utf16,
+          libuna_utf8_string_copy_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_copy_from_utf16,
+          libuna_utf8_string_with_index_copy_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_with_index_copy_from_utf16,
+          libuna_utf8_string_compare_with_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_size_from_utf32,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
@@ -425,14 +567,39 @@
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_with_index_copy_from_utf32,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf8_string_compare_with_utf32,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf8_string_size_from_utf32_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf8_string_copy_from_utf32_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf8_string_with_index_copy_from_utf32_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf8_string_compare_with_utf32_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
           libuna_utf8_string_size_from_scsu_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_copy_from_scsu_stream,
           [ac_cv_libuna_dummy=yes],
@@ -457,14 +624,19 @@
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_with_index_copy_from_byte_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf16_string_compare_with_byte_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
           libuna_utf16_string_size_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_copy_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
@@ -472,14 +644,35 @@
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_with_index_copy_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf16_string_compare_with_utf7_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf16_string_size_from_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf16_string_copy_from_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf16_string_with_index_copy_from_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        dnl libuna_utf16_string_compare_with_utf8 is implemented by libuna_utf8_string_compare_with_utf16
+        AC_CHECK_LIB(
+          una,
           libuna_utf16_string_size_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_copy_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
@@ -487,14 +680,19 @@
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_with_index_copy_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf16_string_compare_with_utf8_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
           libuna_utf16_string_size_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_copy_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
@@ -502,55 +700,55 @@
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_with_index_copy_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_size_from_utf32_stream,
+          libuna_utf16_string_compare_with_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_copy_from_utf32_stream,
+          libuna_utf16_string_size_from_utf32,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_with_index_copy_from_utf32_stream,
+          libuna_utf16_string_copy_from_utf32,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_size_from_utf8,
+          libuna_utf16_string_with_index_copy_from_utf32,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_copy_from_utf8,
+          libuna_utf16_string_compare_with_utf32,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_with_index_copy_from_utf8,
+          libuna_utf16_string_size_from_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_size_from_utf32,
+          libuna_utf16_string_copy_from_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_copy_from_utf32,
+          libuna_utf16_string_with_index_copy_from_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_with_index_copy_from_utf32,
+          libuna_utf16_string_compare_with_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_size_from_scsu_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
@@ -579,14 +777,19 @@
         AC_CHECK_LIB(
           una,
           libuna_utf32_string_with_index_copy_from_byte_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf32_string_compare_with_byte_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
           libuna_utf32_string_size_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf32_string_copy_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
@@ -594,84 +797,106 @@
         AC_CHECK_LIB(
           una,
           libuna_utf32_string_with_index_copy_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf32_string_compare_with_utf7_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
           libuna_utf32_string_size_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf32_string_size_from_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf32_string_copy_from_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          libuna_utf32_string_with_index_copy_from_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        dnl libuna_utf32_string_compare_with_utf8 is implemented by libuna_utf8_string_compare_with_utf32
+        AC_CHECK_LIB(
+          una,
           libuna_utf32_string_copy_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf32_string_with_index_copy_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_size_from_utf16_stream,
+          libuna_utf32_string_compare_with_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_copy_from_utf16_stream,
+          libuna_utf32_string_size_from_utf16,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_with_index_copy_from_utf16_stream,
+          libuna_utf32_string_copy_from_utf16,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_size_from_utf32_stream,
+          libuna_utf32_string_with_index_copy_from_utf16,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
+        dnl libuna_utf32_string_compare_with_utf16 is implemented by libuna_utf16_string_compare_with_utf32
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_copy_from_utf32_stream,
+          libuna_utf32_string_size_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_with_index_copy_from_utf32_stream,
+          libuna_utf32_string_copy_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_size_from_utf8,
+          libuna_utf32_string_with_index_copy_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_copy_from_utf8,
+          libuna_utf32_string_compare_with_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
-          libuna_utf32_string_with_index_copy_from_utf8,
+          una,
+          libuna_utf32_string_size_from_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_size_from_utf16,
+          libuna_utf32_string_copy_from_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_copy_from_utf16,
+          libuna_utf32_string_with_index_copy_from_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_with_index_copy_from_utf16,
+          libuna_utf32_string_compare_with_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf32_string_size_from_scsu_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
@@ -704,14 +929,21 @@
         AX_LIBUNA_CHECK_DEFINITION(
           LIBUNA_COMPARE_GREATER,
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_compare_less" != xyes],
           [ac_cv_libuna=no])
 
+        AX_LIBUNA_CHECK_DEFINITION(
+          LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
+          [ac_cv_libuna_defines_compare_greater])
+        AS_IF(
+          [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
+          [ac_cv_libuna=no])
+
         ac_cv_libuna_LIBADD="-luna"])
       ])
     AS_IF(
       [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
```

### Comparing `libfwsi-20230114/m4/libfwps.m4` & `libfwsi-20230710/m4/libfwps.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/gettext.m4` & `libfwsi-20230710/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/tests.m4` & `libfwsi-20230710/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/lib-prefix.m4` & `libfwsi-20230710/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/ltoptions.m4` & `libfwsi-20230710/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/lib-ld.m4` & `libfwsi-20230710/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/libcthreads.m4` & `libfwsi-20230710/m4/libcthreads.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/lib-link.m4` & `libfwsi-20230710/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/python.m4` & `libfwsi-20230710/m4/python.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/libtool.m4` & `libfwsi-20230710/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/nls.m4` & `libfwsi-20230710/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/libclocale.m4` & `libfwsi-20230710/m4/libclocale.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/libfdatetime.m4` & `libfwsi-20230710/m4/libfdatetime.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/host-cpu-c-abi.m4` & `libfwsi-20230710/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/libcnotify.m4` & `libfwsi-20230710/m4/libcnotify.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/ltversion.m4` & `libfwsi-20230710/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/libcdata.m4` & `libfwsi-20230710/m4/libcdata.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/progtest.m4` & `libfwsi-20230710/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/lt~obsolete.m4` & `libfwsi-20230710/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/po.m4` & `libfwsi-20230710/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/pthread.m4` & `libfwsi-20230710/m4/pthread.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/common.m4` & `libfwsi-20230710/m4/common.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/libcerror.m4` & `libfwsi-20230710/m4/libcerror.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/libfguid.m4` & `libfwsi-20230710/m4/libfguid.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/iconv.m4` & `libfwsi-20230710/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/ltsugar.m4` & `libfwsi-20230710/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/libfole.m4` & `libfwsi-20230710/m4/libfole.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/intlmacosx.m4` & `libfwsi-20230710/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/m4/types.m4` & `libfwsi-20230710/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/COPYING.LESSER` & `libfwsi-20230710/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcerror/libcerror_system.c` & `libfwsi-20230710/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcerror/libcerror_error.c` & `libfwsi-20230710/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcerror/libcerror_extern.h` & `libfwsi-20230710/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcerror/Makefile.am` & `libfwsi-20230710/libcerror/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcerror/libcerror_error.h` & `libfwsi-20230710/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcerror/libcerror_support.h` & `libfwsi-20230710/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcerror/libcerror_types.h` & `libfwsi-20230710/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcerror/libcerror_definitions.h` & `libfwsi-20230710/libcerror/libcerror_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcerror/libcerror_unused.h` & `libfwsi-20230710/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcerror/Makefile.in` & `libfwsi-20230710/libcerror/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcerror/libcerror_support.c` & `libfwsi-20230710/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcerror/libcerror_system.h` & `libfwsi-20230710/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcnotify/libcnotify_libcerror.h` & `libfwsi-20230710/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcnotify/libcnotify_unused.h` & `libfwsi-20230710/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcnotify/libcnotify_support.h` & `libfwsi-20230710/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcnotify/libcnotify_support.c` & `libfwsi-20230710/libcdata/libcdata_support.c`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -18,22 +18,22 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include "libcnotify_definitions.h"
-#include "libcnotify_support.h"
+#include "libcdata_definitions.h"
+#include "libcdata_support.h"
 
-#if !defined( HAVE_LOCAL_LIBCNOTIFY )
+#if !defined( HAVE_LOCAL_LIBCDATA )
 
 /* Returns the library version as a string
  */
-const char *libcnotify_get_version(
+const char *libcdata_get_version(
              void )
 {
-	return( (const char *) LIBCNOTIFY_VERSION_STRING );
+	return( (const char *) LIBCDATA_VERSION_STRING );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBCNOTIFY ) */
+#endif /* !defined( HAVE_LOCAL_LIBCDATA ) */
```

### Comparing `libfwsi-20230114/libcnotify/Makefile.am` & `libfwsi-20230710/libcnotify/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcnotify/libcnotify_print.c` & `libfwsi-20230710/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcnotify/libcnotify_verbose.c` & `libfwsi-20230710/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcnotify/libcnotify_stream.h` & `libfwsi-20230710/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcnotify/libcnotify_extern.h` & `libfwsi-20230710/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcnotify/libcnotify_stream.c` & `libfwsi-20230710/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcnotify/Makefile.in` & `libfwsi-20230710/libcnotify/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcnotify/libcnotify_print.h` & `libfwsi-20230710/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcnotify/libcnotify_verbose.h` & `libfwsi-20230710/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcnotify/libcnotify_definitions.h` & `libfwsi-20230710/libcnotify/libcnotify_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/ltmain.sh` & `libfwsi-20230710/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/compile` & `libfwsi-20230710/compile`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/config.rpath` & `libfwsi-20230710/config.rpath`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/depcomp` & `libfwsi-20230710/depcomp`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/po/en@quot.header` & `libfwsi-20230710/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/po/Rules-quot` & `libfwsi-20230710/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/po/remove-potcdate.sin` & `libfwsi-20230710/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/po/Makevars.in` & `libfwsi-20230710/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/po/en@boldquot.header` & `libfwsi-20230710/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/po/Makevars` & `libfwsi-20230710/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/po/insert-header.sin` & `libfwsi-20230710/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/po/Makefile.in.in` & `libfwsi-20230710/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_array.c` & `libfwsi-20230710/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_btree_node.c` & `libfwsi-20230710/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_tree_node.c` & `libfwsi-20230710/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_libcthreads.h` & `libfwsi-20230710/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_range_list_value.h` & `libfwsi-20230710/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_unused.h` & `libfwsi-20230710/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_range_list.h` & `libfwsi-20230710/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/Makefile.am` & `libfwsi-20230710/libcdata/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_range_list.c` & `libfwsi-20230710/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_extern.h` & `libfwsi-20230710/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_support.c` & `libfwsi-20230710/libcdata/libcdata_libcerror.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Support functions
+ * The libcerror header wrapper
  *
  * Copyright (C) 2006-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
@@ -15,25 +15,36 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
+#if !defined( _LIBCDATA_LIBCERROR_H )
+#define _LIBCDATA_LIBCERROR_H
+
 #include <common.h>
-#include <types.h>
 
-#include "libcdata_definitions.h"
-#include "libcdata_support.h"
+/* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
+ */
+#if defined( HAVE_LOCAL_LIBCERROR )
+
+#include <libcerror_definitions.h>
+#include <libcerror_error.h>
+#include <libcerror_system.h>
+#include <libcerror_types.h>
 
-#if !defined( HAVE_LOCAL_LIBCDATA )
+#else
 
-/* Returns the library version as a string
+/* If libtool DLL support is enabled set LIBCERROR_DLL_IMPORT
+ * before including libcerror.h
  */
-const char *libcdata_get_version(
-             void )
-{
-	return( (const char *) LIBCDATA_VERSION_STRING );
-}
+#if defined( _WIN32 ) && defined( DLL_IMPORT )
+#define LIBCERROR_DLL_IMPORT
+#endif
+
+#include <libcerror.h>
+
+#endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( HAVE_LOCAL_LIBCDATA ) */
+#endif /* !defined( _LIBCDATA_LIBCERROR_H ) */
```

### Comparing `libfwsi-20230114/libcdata/libcdata_list_element.h` & `libfwsi-20230710/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_btree_values_list.c` & `libfwsi-20230710/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_range_list_value.c` & `libfwsi-20230710/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_error.c` & `libfwsi-20230710/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_error.h` & `libfwsi-20230710/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_btree_node.h` & `libfwsi-20230710/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_list.c` & `libfwsi-20230710/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_tree_node.h` & `libfwsi-20230710/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_list.h` & `libfwsi-20230710/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_types.h` & `libfwsi-20230710/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_list_element.c` & `libfwsi-20230710/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/Makefile.in` & `libfwsi-20230710/libcdata/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_btree_values_list.h` & `libfwsi-20230710/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_array.h` & `libfwsi-20230710/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_btree.h` & `libfwsi-20230710/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_definitions.h` & `libfwsi-20230710/libcdata/libcdata_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/libcdata/libcdata_btree.c` & `libfwsi-20230710/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/acinclude.m4` & `libfwsi-20230710/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20230114/configure.ac` & `libfwsi-20230710/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfwsi],
- [20230114],
+ [20230710],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfwsi.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
```

