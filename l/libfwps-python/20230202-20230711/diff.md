# Comparing `tmp/libfwps-python-20230202.tar.gz` & `tmp/libfwps-python-20230711.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfwps-python-20230202.tar", last modified: Sat Feb  4 10:23:08 2023, max compression
+gzip compressed data, was "libfwps-python-20230711.tar", last modified: Tue Jul 11 16:02:10 2023, max compression
```

## Comparing `libfwps-python-20230202.tar` & `libfwps-python-20230711.tar`

### file list

```diff
@@ -1,548 +1,551 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/libfwps/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_record.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3731 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_format_class_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_libcdata.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9704 2023-02-02 04:25:47.000000 libfwps-20230202/libfwps/libfwps_store.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_codepage.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_format_class_identifier.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3829 2023-02-02 04:25:47.000000 libfwps-20230202/libfwps/libfwps_definitions.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2244 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_property_identifier.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2023-02-02 04:40:41.000000 libfwps-20230202/libfwps/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16442 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_set.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3827 2023-02-04 09:54:01.000000 libfwps-20230202/libfwps/libfwps_definitions.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1820 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_libuna.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_libfole.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2023-02-02 04:25:47.000000 libfwps-20230202/libfwps/libfwps_store.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1078 2023-02-04 09:54:01.000000 libfwps-20230202/libfwps/libfwps.rc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_error.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-02-02 04:25:47.000000 libfwps-20230202/libfwps/libfwps_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30980 2023-02-04 09:53:52.000000 libfwps-20230202/libfwps/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_libcerror.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7534 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_property_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2023-02-02 04:41:47.000000 libfwps-20230202/libfwps/libfwps_types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    45991 2023-02-02 12:02:31.000000 libfwps-20230202/libfwps/libfwps_record.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-02-02 04:25:47.000000 libfwps-20230202/libfwps/libfwps_unused.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-02-02 04:25:47.000000 libfwps-20230202/libfwps/libfwps_support.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1080 2023-02-02 04:25:47.000000 libfwps-20230202/libfwps/libfwps.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2490 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_set.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-02-02 04:25:46.000000 libfwps-20230202/libfwps/libfwps_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:06.000000 libfwps-20230202/common/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2023-02-02 04:25:46.000000 libfwps-20230202/common/config_msc.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2023-02-02 04:25:46.000000 libfwps-20230202/common/byte_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-02-02 04:25:46.000000 libfwps-20230202/common/common.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2023-02-02 04:25:46.000000 libfwps-20230202/common/system_string.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      378 2023-02-02 04:25:41.000000 libfwps-20230202/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7234 2023-02-04 09:54:01.000000 libfwps-20230202/common/types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7236 2023-02-02 04:25:46.000000 libfwps-20230202/common/types.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2243 2023-02-02 04:25:46.000000 libfwps-20230202/common/config_winapi.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2023-02-02 04:25:46.000000 libfwps-20230202/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13101 2023-02-04 09:54:01.000000 libfwps-20230202/common/config.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2023-02-02 04:25:46.000000 libfwps-20230202/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22466 2023-02-04 09:53:51.000000 libfwps-20230202/common/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2023-02-02 04:25:46.000000 libfwps-20230202/common/file_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      957 2023-02-02 04:25:46.000000 libfwps-20230202/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12378 2023-02-04 09:53:51.000000 libfwps-20230202/common/config.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2023-02-02 04:25:46.000000 libfwps-20230202/common/wide_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/libfole/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2023-02-04 09:53:38.000000 libfwps-20230202/libfole/libfole_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      630 2023-02-04 09:53:38.000000 libfwps-20230202/libfole/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-02-04 09:53:38.000000 libfwps-20230202/libfole/libfole_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-02-04 09:53:38.000000 libfwps-20230202/libfole/libfole_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-02-04 09:53:38.000000 libfwps-20230202/libfole/libfole_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-02-04 09:53:38.000000 libfwps-20230202/libfole/libfole_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-02-04 09:53:38.000000 libfwps-20230202/libfole/libfole_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-02-04 09:53:38.000000 libfwps-20230202/libfole/libfole_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3793 2023-02-04 09:53:38.000000 libfwps-20230202/libfole/libfole_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-02-04 09:53:38.000000 libfwps-20230202/libfole/libfole_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26789 2023-02-04 09:53:52.000000 libfwps-20230202/libfole/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-02-04 09:53:38.000000 libfwps-20230202/libfole/libfole_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1407 2023-02-04 09:53:38.000000 libfwps-20230202/libfole/libfole_types.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2023-02-04 09:53:36.000000 libfwps-20230202/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2023-02-04 09:53:36.000000 libfwps-20230202/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2023-02-04 09:53:36.000000 libfwps-20230202/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2023-02-04 09:53:36.000000 libfwps-20230202/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2023-02-04 09:53:36.000000 libfwps-20230202/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2023-02-04 09:53:36.000000 libfwps-20230202/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-02-04 09:53:36.000000 libfwps-20230202/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-02-04 09:53:36.000000 libfwps-20230202/libfguid/libfguid_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-02-04 09:53:36.000000 libfwps-20230202/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26866 2023-02-04 09:53:52.000000 libfwps-20230202/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-02-04 09:53:36.000000 libfwps-20230202/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2023-02-04 09:53:36.000000 libfwps-20230202/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-02-04 09:53:36.000000 libfwps-20230202/libfguid/libfguid_extern.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/tests/
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3814 2023-02-02 04:38:31.000000 libfwps-20230202/tests/test_library.sh
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-02-02 04:25:47.000000 libfwps-20230202/tests/pyfwps_test_support.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3410 2023-02-02 04:25:47.000000 libfwps-20230202/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2236 2023-02-02 04:38:23.000000 libfwps-20230202/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1857 2023-02-02 04:27:19.000000 libfwps-20230202/tests/pyfwps_test_store.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2023-02-02 04:25:47.000000 libfwps-20230202/tests/fwps_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1860 2023-02-02 04:27:19.000000 libfwps-20230202/tests/pyfwps_test_set.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2023-02-02 04:25:47.000000 libfwps-20230202/tests/fwps_test_macros.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2023-02-02 04:25:47.000000 libfwps-20230202/tests/fwps_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8920 2023-02-02 04:27:03.000000 libfwps-20230202/tests/fwps_test_set.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-02-02 04:25:47.000000 libfwps-20230202/tests/fwps_test_libcerror.h
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     1645 2023-02-02 04:25:47.000000 libfwps-20230202/tests/test_manpage.sh
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      973 2023-02-02 04:25:47.000000 libfwps-20230202/tests/fwps_test_libfwps.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    37784 2023-02-02 04:25:47.000000 libfwps-20230202/tests/test_runner.sh
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1902 2023-02-02 04:25:47.000000 libfwps-20230202/tests/fwps_test_property_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6480 2023-02-02 04:27:03.000000 libfwps-20230202/tests/fwps_test_record.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2023-02-02 04:25:47.000000 libfwps-20230202/tests/fwps_test_memory.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2023-02-02 04:25:47.000000 libfwps-20230202/tests/fwps_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45373 2023-02-04 09:53:52.000000 libfwps-20230202/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9089 2023-02-02 04:27:03.000000 libfwps-20230202/tests/fwps_test_store.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2023-02-02 04:25:47.000000 libfwps-20230202/tests/fwps_test_memory.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:06.000000 libfwps-20230202/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-02-04 09:53:31.000000 libfwps-20230202/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2023-02-04 09:53:31.000000 libfwps-20230202/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2023-02-04 09:53:31.000000 libfwps-20230202/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      744 2023-02-04 09:53:31.000000 libfwps-20230202/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2023-02-04 09:53:31.000000 libfwps-20230202/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-02-04 09:53:31.000000 libfwps-20230202/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-02-04 09:53:31.000000 libfwps-20230202/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-02-04 09:53:31.000000 libfwps-20230202/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2023-02-04 09:53:31.000000 libfwps-20230202/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-02-04 09:53:31.000000 libfwps-20230202/libclocale/libclocale_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2023-02-04 09:53:31.000000 libfwps-20230202/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27422 2023-02-04 09:53:52.000000 libfwps-20230202/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2023-02-04 09:53:31.000000 libfwps-20230202/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-02-04 09:53:31.000000 libfwps-20230202/libclocale/libclocale_libcerror.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2023-02-04 09:53:51.000000 libfwps-20230202/missing
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2755 2022-04-26 08:19:36.000000 libfwps-20230202/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55847 2023-02-04 09:53:49.000000 libfwps-20230202/aclocal.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/pyfwps-python3/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1534 2023-02-02 04:25:44.000000 libfwps-20230202/pyfwps-python3/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43436 2023-02-04 09:53:52.000000 libfwps-20230202/pyfwps-python3/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2023-02-02 04:25:41.000000 libfwps-20230202/COPYING
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      292 2023-02-02 04:25:41.000000 libfwps-20230202/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2166 2023-02-04 09:54:01.000000 libfwps-20230202/libfwps.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:06.000000 libfwps-20230202/include/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:06.000000 libfwps-20230202/include/libfwps/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3345 2023-02-02 04:25:46.000000 libfwps-20230202/include/libfwps/definitions.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-02-02 04:25:46.000000 libfwps-20230202/include/libfwps/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4870 2023-02-04 09:54:01.000000 libfwps-20230202/include/libfwps/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2023-02-02 04:27:03.000000 libfwps-20230202/include/libfwps/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5001 2023-02-02 04:41:26.000000 libfwps-20230202/include/libfwps/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2023-02-04 09:54:01.000000 libfwps-20230202/include/libfwps/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3343 2023-02-04 09:54:01.000000 libfwps-20230202/include/libfwps/definitions.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2023-02-02 04:25:46.000000 libfwps-20230202/include/libfwps/codepage.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2023-02-02 04:25:46.000000 libfwps-20230202/include/libfwps/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2023-02-02 04:27:03.000000 libfwps-20230202/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25448 2023-02-04 09:53:51.000000 libfwps-20230202/include/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10690 2023-02-02 04:42:12.000000 libfwps-20230202/include/libfwps.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10690 2023-02-04 09:54:01.000000 libfwps-20230202/include/libfwps.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      521 2023-02-02 04:25:41.000000 libfwps-20230202/libfwps.pc.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2023-02-04 09:53:51.000000 libfwps-20230202/install-sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/pyfwps-python2/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1534 2023-02-02 04:25:44.000000 libfwps-20230202/pyfwps-python2/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43436 2023-02-04 09:53:52.000000 libfwps-20230202/pyfwps-python2/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2023-02-04 09:53:51.000000 libfwps-20230202/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:06.000000 libfwps-20230202/dpkg/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-02-02 04:25:41.000000 libfwps-20230202/dpkg/libfwps-dev.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      120 2023-02-02 04:25:41.000000 libfwps-20230202/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2023-02-04 09:54:01.000000 libfwps-20230202/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       22 2023-02-02 04:25:41.000000 libfwps-20230202/dpkg/libfwps.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2023-02-02 04:25:47.000000 libfwps-20230202/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:06.000000 libfwps-20230202/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-02-02 04:25:41.000000 libfwps-20230202/dpkg/source/format
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      704 2023-02-02 04:25:41.000000 libfwps-20230202/dpkg/rules
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       18 2023-02-02 04:25:41.000000 libfwps-20230202/dpkg/libfwps-python3.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        3 2023-02-02 04:25:41.000000 libfwps-20230202/dpkg/compat
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2023-02-02 04:25:41.000000 libfwps-20230202/dpkg/control
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30037 2023-02-04 09:53:52.000000 libfwps-20230202/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2023-02-04 09:53:35.000000 libfwps-20230202/libfdatetime/libfdatetime_filetime.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:06.000000 libfwps-20230202/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30276 2023-02-04 09:53:52.000000 libfwps-20230202/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2023-02-04 09:53:34.000000 libfwps-20230202/libcthreads/libcthreads_queue.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       91 2023-02-02 04:25:45.000000 libfwps-20230202/AUTHORS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35409 2023-02-04 09:53:51.000000 libfwps-20230202/config.sub
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      130 2016-02-02 07:37:21.000000 libfwps-20230202/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4937 2023-02-02 04:25:47.000000 libfwps-20230202/manuals/libfwps.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22665 2023-02-04 09:53:52.000000 libfwps-20230202/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2022-07-11 04:42:36.000000 libfwps-20230202/ABOUT-NLS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/libfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6908 2023-02-02 04:41:54.000000 libfwps-20230202/msvscpp/libfwps/libfwps.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/libfole/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4605 2023-02-02 04:41:54.000000 libfwps-20230202/msvscpp/libfole/libfole.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/fwps_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5134 2023-02-02 04:41:54.000000 libfwps-20230202/msvscpp/fwps_test_error/fwps_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2023-02-02 04:41:54.000000 libfwps-20230202/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/fwps_test_property_identifier/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2023-02-02 04:41:54.000000 libfwps-20230202/msvscpp/fwps_test_property_identifier/fwps_test_property_identifier.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2023-02-02 04:41:54.000000 libfwps-20230202/msvscpp/libclocale/libclocale.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      746 2023-02-02 04:41:55.000000 libfwps-20230202/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/fwps_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5140 2023-02-02 04:41:54.000000 libfwps-20230202/msvscpp/fwps_test_support/fwps_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/fwps_test_record/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5380 2023-02-02 04:41:54.000000 libfwps-20230202/msvscpp/fwps_test_record/fwps_test_record.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/fwps_test_store/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5377 2023-02-02 04:41:54.000000 libfwps-20230202/msvscpp/fwps_test_store/fwps_test_store.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2023-02-02 04:41:54.000000 libfwps-20230202/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2023-02-02 04:41:54.000000 libfwps-20230202/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2023-02-02 04:41:55.000000 libfwps-20230202/msvscpp/libuna/libuna.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/pyfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6543 2023-02-02 04:41:55.000000 libfwps-20230202/msvscpp/pyfwps/pyfwps.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20168 2023-02-04 09:53:52.000000 libfwps-20230202/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2023-02-02 04:41:55.000000 libfwps-20230202/msvscpp/libcerror/libcerror.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12507 2023-02-02 04:41:54.000000 libfwps-20230202/msvscpp/libfwps.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2023-02-02 04:41:55.000000 libfwps-20230202/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/fwps_test_set/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5371 2023-02-02 04:41:54.000000 libfwps-20230202/msvscpp/fwps_test_set/fwps_test_set.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2023-02-02 04:41:55.000000 libfwps-20230202/msvscpp/libcdata/libcdata.vcproj
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)    11454 2023-02-02 04:26:11.000000 libfwps-20230202/setup.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49797 2023-02-04 09:53:51.000000 libfwps-20230202/config.guess
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-02 04:25:41.000000 libfwps-20230202/NEWS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1347 2023-02-02 04:25:47.000000 libfwps-20230202/ossfuzz/store_fuzzer.cc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      967 2023-02-02 04:25:47.000000 libfwps-20230202/ossfuzz/ossfuzz_libfwps.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1095 2023-02-02 04:33:25.000000 libfwps-20230202/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1329 2023-02-02 04:25:47.000000 libfwps-20230202/ossfuzz/set_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1802 2023-02-02 04:36:45.000000 libfwps-20230202/ossfuzz/record_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31314 2023-02-04 09:53:52.000000 libfwps-20230202/ossfuzz/Makefile.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2023-02-04 09:53:52.000000 libfwps-20230202/test-driver
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1449951 2023-02-04 09:53:50.000000 libfwps-20230202/configure
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19794 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95123 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5908 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   129163 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101951 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98825 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50988 2023-02-04 09:53:52.000000 libfwps-20230202/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19595 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16696 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2023-02-04 09:53:40.000000 libfwps-20230202/libuna/libuna_codepage_iso_8859_16.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/pyfwps/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_libcerror.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_unused.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1063 2023-01-30 05:54:44.000000 libfwps-20230202/pyfwps/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9101 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_records.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2296 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_sets.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2539 2023-02-02 04:27:37.000000 libfwps-20230202/pyfwps/pyfwps_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2133 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_store.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12160 2023-02-02 04:27:37.000000 libfwps-20230202/pyfwps/pyfwps_store.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2343 2023-02-02 04:27:37.000000 libfwps-20230202/pyfwps/pyfwps_set.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2359 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_records.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3254 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5565 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14766 2023-02-02 04:27:37.000000 libfwps-20230202/pyfwps/pyfwps_set.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8919 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_sets.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43083 2023-02-04 09:53:52.000000 libfwps-20230202/pyfwps/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      965 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_libfwps.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20544 2023-02-02 04:27:37.000000 libfwps-20230202/pyfwps/pyfwps_record.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_guid.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_codepage.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_libfguid.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2891 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_guid.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2023-02-02 04:25:47.000000 libfwps-20230202/pyfwps/pyfwps_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38796 2023-02-04 09:53:51.000000 libfwps-20230202/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      298 2023-02-02 04:39:35.000000 libfwps-20230202/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:06.000000 libfwps-20230202/m4/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23765 2021-12-18 05:56:55.000000 libfwps-20230202/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2022-07-11 04:42:36.000000 libfwps-20230202/m4/gettext.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      756 2020-07-16 10:33:58.000000 libfwps-20230202/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2022-07-11 04:42:36.000000 libfwps-20230202/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2023-02-04 09:53:46.000000 libfwps-20230202/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2022-07-11 04:42:36.000000 libfwps-20230202/m4/lib-ld.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2019-09-17 04:01:01.000000 libfwps-20230202/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2022-07-11 04:42:36.000000 libfwps-20230202/m4/lib-link.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17674 2021-12-18 05:56:55.000000 libfwps-20230202/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2023-02-04 09:53:46.000000 libfwps-20230202/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-07-11 04:42:36.000000 libfwps-20230202/m4/nls.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2019-09-17 04:01:01.000000 libfwps-20230202/m4/libclocale.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2019-09-17 04:01:01.000000 libfwps-20230202/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2022-07-11 04:42:36.000000 libfwps-20230202/m4/host-cpu-c-abi.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2019-09-17 04:01:01.000000 libfwps-20230202/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2023-02-04 09:53:46.000000 libfwps-20230202/m4/ltversion.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-01-14 09:27:01.000000 libfwps-20230202/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2022-07-11 04:42:36.000000 libfwps-20230202/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2023-02-04 09:53:46.000000 libfwps-20230202/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2022-07-11 04:42:36.000000 libfwps-20230202/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2014-07-31 05:12:52.000000 libfwps-20230202/m4/pthread.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2019-01-02 20:12:18.000000 libfwps-20230202/m4/common.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2019-09-17 04:01:01.000000 libfwps-20230202/m4/libcerror.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2019-09-17 04:01:01.000000 libfwps-20230202/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2022-07-11 04:42:36.000000 libfwps-20230202/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2023-02-04 09:53:46.000000 libfwps-20230202/m4/ltsugar.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3956 2019-09-17 04:01:01.000000 libfwps-20230202/m4/libfole.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2022-07-11 04:42:36.000000 libfwps-20230202/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2018-07-31 03:18:22.000000 libfwps-20230202/m4/types.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2023-02-02 04:25:41.000000 libfwps-20230202/COPYING.LESSER
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2745 2023-02-02 04:25:41.000000 libfwps-20230202/libfwps.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:06.000000 libfwps-20230202/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2023-02-04 09:53:30.000000 libfwps-20230202/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2023-02-04 09:53:30.000000 libfwps-20230202/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-02-04 09:53:30.000000 libfwps-20230202/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      605 2023-02-04 09:53:30.000000 libfwps-20230202/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2023-02-04 09:53:30.000000 libfwps-20230202/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-02-04 09:53:30.000000 libfwps-20230202/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2023-02-04 09:53:30.000000 libfwps-20230202/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2023-02-04 09:53:30.000000 libfwps-20230202/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-02-04 09:53:30.000000 libfwps-20230202/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26811 2023-02-04 09:53:51.000000 libfwps-20230202/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-02-04 09:53:30.000000 libfwps-20230202/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2023-02-04 09:53:30.000000 libfwps-20230202/libcerror/libcerror_system.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:06.000000 libfwps-20230202/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-02-04 09:53:32.000000 libfwps-20230202/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-02-04 09:53:32.000000 libfwps-20230202/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2023-02-04 09:53:32.000000 libfwps-20230202/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2023-02-04 09:53:32.000000 libfwps-20230202/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      693 2023-02-04 09:53:32.000000 libfwps-20230202/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2023-02-04 09:53:32.000000 libfwps-20230202/libcnotify/libcnotify_print.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2023-02-04 09:53:32.000000 libfwps-20230202/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2023-02-04 09:53:32.000000 libfwps-20230202/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-02-04 09:53:32.000000 libfwps-20230202/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2023-02-04 09:53:32.000000 libfwps-20230202/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27298 2023-02-04 09:53:52.000000 libfwps-20230202/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2023-02-04 09:53:32.000000 libfwps-20230202/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2023-02-04 09:53:32.000000 libfwps-20230202/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-02-04 09:53:32.000000 libfwps-20230202/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2023-02-04 09:53:46.000000 libfwps-20230202/ltmain.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2023-02-04 09:53:51.000000 libfwps-20230202/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2022-07-11 04:42:36.000000 libfwps-20230202/config.rpath
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2023-02-04 09:53:52.000000 libfwps-20230202/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:07.000000 libfwps-20230202/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2022-07-11 04:42:36.000000 libfwps-20230202/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2022-07-11 04:42:36.000000 libfwps-20230202/po/Rules-quot
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2014-07-31 05:12:52.000000 libfwps-20230202/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2022-07-11 04:42:36.000000 libfwps-20230202/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2014-07-31 05:12:52.000000 libfwps-20230202/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2016-11-04 14:23:16.000000 libfwps-20230202/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2022-07-11 04:42:36.000000 libfwps-20230202/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2014-07-31 05:12:52.000000 libfwps-20230202/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1809 2023-02-04 09:54:01.000000 libfwps-20230202/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2022-07-11 04:42:36.000000 libfwps-20230202/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2022-07-11 04:42:36.000000 libfwps-20230202/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2014-07-31 05:12:52.000000 libfwps-20230202/po/boldquot.sed
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 10:23:06.000000 libfwps-20230202/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29870 2023-02-04 09:53:51.000000 libfwps-20230202/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2023-02-04 09:53:28.000000 libfwps-20230202/libcdata/libcdata_btree.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      752 2023-02-02 04:25:41.000000 libfwps-20230202/acinclude.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5641 2023-02-02 04:25:41.000000 libfwps-20230202/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      347 2023-02-04 10:23:08.566502 libfwps-20230202/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:09.000000 libfwps-20230711/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:09.000000 libfwps-20230711/libfwps/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5115 2023-07-11 14:50:22.000000 libfwps-20230711/libfwps/libfwps_record.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3731 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_format_class_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_libcdata.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9704 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_store.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_codepage.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_format_class_identifier.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3829 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_definitions.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2244 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_property_identifier.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2023-02-02 04:40:41.000000 libfwps-20230711/libfwps/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16442 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_set.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3827 2023-07-11 15:46:45.000000 libfwps-20230711/libfwps/libfwps_definitions.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1820 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_libuna.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_libfole.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_store.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1078 2023-07-11 15:46:45.000000 libfwps-20230711/libfwps/libfwps.rc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_error.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30980 2023-07-11 15:46:35.000000 libfwps-20230711/libfwps/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_libcerror.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7534 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_property_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    60078 2023-07-11 14:52:59.000000 libfwps-20230711/libfwps/libfwps_record.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_unused.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_support.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1080 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2490 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_set.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-07-10 19:41:07.000000 libfwps-20230711/libfwps/libfwps_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:08.000000 libfwps-20230711/common/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2023-07-10 19:41:07.000000 libfwps-20230711/common/config_msc.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2023-07-10 19:41:07.000000 libfwps-20230711/common/byte_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-07-10 19:41:07.000000 libfwps-20230711/common/common.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2023-07-10 19:41:07.000000 libfwps-20230711/common/system_string.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      378 2023-07-10 19:41:05.000000 libfwps-20230711/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2023-07-11 15:46:45.000000 libfwps-20230711/common/types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2023-07-10 19:41:07.000000 libfwps-20230711/common/types.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2023-07-10 19:41:07.000000 libfwps-20230711/common/config_winapi.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2023-07-10 19:41:07.000000 libfwps-20230711/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13101 2023-07-11 15:46:45.000000 libfwps-20230711/common/config.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2023-07-10 19:41:07.000000 libfwps-20230711/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22466 2023-07-11 15:46:34.000000 libfwps-20230711/common/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2023-07-10 19:41:07.000000 libfwps-20230711/common/file_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      957 2023-07-10 19:41:07.000000 libfwps-20230711/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12378 2023-07-11 15:46:33.000000 libfwps-20230711/common/config.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2023-07-10 19:41:07.000000 libfwps-20230711/common/wide_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:09.000000 libfwps-20230711/libfole/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2023-07-11 15:46:20.000000 libfwps-20230711/libfole/libfole_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      630 2023-07-11 15:46:20.000000 libfwps-20230711/libfole/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-07-11 15:46:20.000000 libfwps-20230711/libfole/libfole_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-07-11 15:46:20.000000 libfwps-20230711/libfole/libfole_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-07-11 15:46:20.000000 libfwps-20230711/libfole/libfole_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-07-11 15:46:20.000000 libfwps-20230711/libfole/libfole_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-07-11 15:46:20.000000 libfwps-20230711/libfole/libfole_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-07-11 15:46:20.000000 libfwps-20230711/libfole/libfole_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3793 2023-07-11 15:46:20.000000 libfwps-20230711/libfole/libfole_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-07-11 15:46:20.000000 libfwps-20230711/libfole/libfole_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26789 2023-07-11 15:46:35.000000 libfwps-20230711/libfole/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-07-11 15:46:20.000000 libfwps-20230711/libfole/libfole_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1407 2023-07-11 15:46:20.000000 libfwps-20230711/libfole/libfole_types.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:09.000000 libfwps-20230711/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2023-07-11 15:46:18.000000 libfwps-20230711/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2023-07-11 15:46:18.000000 libfwps-20230711/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2023-07-11 15:46:18.000000 libfwps-20230711/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2023-07-11 15:46:18.000000 libfwps-20230711/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2023-07-11 15:46:18.000000 libfwps-20230711/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2023-07-11 15:46:18.000000 libfwps-20230711/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-07-11 15:46:18.000000 libfwps-20230711/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-07-11 15:46:18.000000 libfwps-20230711/libfguid/libfguid_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-07-11 15:46:18.000000 libfwps-20230711/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26866 2023-07-11 15:46:35.000000 libfwps-20230711/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-07-11 15:46:18.000000 libfwps-20230711/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2023-07-11 15:46:18.000000 libfwps-20230711/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-07-11 15:46:18.000000 libfwps-20230711/libfguid/libfguid_extern.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:09.000000 libfwps-20230711/tests/
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3822 2023-07-10 19:42:25.000000 libfwps-20230711/tests/test_library.sh
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-07-10 19:41:08.000000 libfwps-20230711/tests/pyfwps_test_support.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3418 2023-07-10 19:41:08.000000 libfwps-20230711/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2236 2023-07-10 19:42:25.000000 libfwps-20230711/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1857 2023-07-10 19:42:25.000000 libfwps-20230711/tests/pyfwps_test_store.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2023-07-10 19:41:08.000000 libfwps-20230711/tests/fwps_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1860 2023-07-10 19:42:25.000000 libfwps-20230711/tests/pyfwps_test_set.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2023-07-10 19:41:08.000000 libfwps-20230711/tests/fwps_test_macros.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2023-07-10 19:41:08.000000 libfwps-20230711/tests/fwps_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8920 2023-07-10 19:42:25.000000 libfwps-20230711/tests/fwps_test_set.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-07-10 19:41:08.000000 libfwps-20230711/tests/fwps_test_libcerror.h
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2023-07-10 19:41:08.000000 libfwps-20230711/tests/test_manpage.sh
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      973 2023-07-10 19:41:08.000000 libfwps-20230711/tests/fwps_test_libfwps.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    37792 2023-07-10 19:41:08.000000 libfwps-20230711/tests/test_runner.sh
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1902 2023-07-10 19:41:08.000000 libfwps-20230711/tests/fwps_test_property_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6480 2023-07-10 19:42:25.000000 libfwps-20230711/tests/fwps_test_record.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2023-07-10 19:41:08.000000 libfwps-20230711/tests/fwps_test_memory.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2023-07-10 19:41:08.000000 libfwps-20230711/tests/fwps_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45373 2023-07-11 15:46:35.000000 libfwps-20230711/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9089 2023-07-10 19:42:25.000000 libfwps-20230711/tests/fwps_test_store.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2023-07-10 19:41:08.000000 libfwps-20230711/tests/fwps_test_memory.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:08.000000 libfwps-20230711/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-07-11 15:46:12.000000 libfwps-20230711/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2023-07-11 15:46:12.000000 libfwps-20230711/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2023-07-11 15:46:12.000000 libfwps-20230711/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      744 2023-07-11 15:46:12.000000 libfwps-20230711/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2023-07-11 15:46:12.000000 libfwps-20230711/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-07-11 15:46:12.000000 libfwps-20230711/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-07-11 15:46:12.000000 libfwps-20230711/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-07-11 15:46:12.000000 libfwps-20230711/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2023-07-11 15:46:12.000000 libfwps-20230711/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-07-11 15:46:12.000000 libfwps-20230711/libclocale/libclocale_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2023-07-11 15:46:12.000000 libfwps-20230711/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27422 2023-07-11 15:46:34.000000 libfwps-20230711/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2023-07-11 15:46:12.000000 libfwps-20230711/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-07-11 15:46:12.000000 libfwps-20230711/libclocale/libclocale_libcerror.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2023-07-11 15:46:34.000000 libfwps-20230711/missing
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2755 2022-04-26 08:19:36.000000 libfwps-20230711/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55847 2023-07-11 15:46:31.000000 libfwps-20230711/aclocal.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:09.000000 libfwps-20230711/pyfwps-python3/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1588 2023-07-11 04:12:31.000000 libfwps-20230711/pyfwps-python3/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44882 2023-07-11 15:46:35.000000 libfwps-20230711/pyfwps-python3/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2023-07-10 19:41:05.000000 libfwps-20230711/COPYING
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      292 2023-07-10 19:41:05.000000 libfwps-20230711/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1948 2023-07-11 15:46:45.000000 libfwps-20230711/libfwps.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:08.000000 libfwps-20230711/include/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:08.000000 libfwps-20230711/include/libfwps/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3345 2023-07-10 19:41:07.000000 libfwps-20230711/include/libfwps/definitions.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-07-10 19:41:07.000000 libfwps-20230711/include/libfwps/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4870 2023-07-11 15:46:45.000000 libfwps-20230711/include/libfwps/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2023-07-10 19:42:33.000000 libfwps-20230711/include/libfwps/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5001 2023-07-10 19:41:07.000000 libfwps-20230711/include/libfwps/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2023-07-11 15:46:45.000000 libfwps-20230711/include/libfwps/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3343 2023-07-11 15:46:45.000000 libfwps-20230711/include/libfwps/definitions.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2023-07-10 19:41:07.000000 libfwps-20230711/include/libfwps/codepage.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2023-07-10 19:41:07.000000 libfwps-20230711/include/libfwps/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2023-07-10 19:42:33.000000 libfwps-20230711/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25448 2023-07-11 15:46:34.000000 libfwps-20230711/include/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    12938 2023-07-11 14:49:26.000000 libfwps-20230711/include/libfwps.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12938 2023-07-11 15:46:45.000000 libfwps-20230711/include/libfwps.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      521 2023-07-10 19:41:05.000000 libfwps-20230711/libfwps.pc.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2023-07-11 15:46:34.000000 libfwps-20230711/install-sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:09.000000 libfwps-20230711/pyfwps-python2/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1588 2023-07-11 04:12:14.000000 libfwps-20230711/pyfwps-python2/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44882 2023-07-11 15:46:35.000000 libfwps-20230711/pyfwps-python2/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2023-07-11 15:46:34.000000 libfwps-20230711/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:08.000000 libfwps-20230711/dpkg/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-07-10 19:41:05.000000 libfwps-20230711/dpkg/libfwps-dev.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      120 2023-07-10 19:41:05.000000 libfwps-20230711/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2023-07-11 15:46:45.000000 libfwps-20230711/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       22 2023-07-10 19:41:05.000000 libfwps-20230711/dpkg/libfwps.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2023-07-10 19:41:08.000000 libfwps-20230711/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:08.000000 libfwps-20230711/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-07-10 19:41:05.000000 libfwps-20230711/dpkg/source/format
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      704 2023-07-10 19:41:05.000000 libfwps-20230711/dpkg/rules
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       18 2023-07-10 19:41:05.000000 libfwps-20230711/dpkg/libfwps-python3.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        3 2023-07-10 19:41:05.000000 libfwps-20230711/dpkg/compat
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2023-07-10 19:41:05.000000 libfwps-20230711/dpkg/control
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:09.000000 libfwps-20230711/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30037 2023-07-11 15:46:35.000000 libfwps-20230711/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2023-07-11 15:46:17.000000 libfwps-20230711/libfdatetime/libfdatetime_filetime.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:08.000000 libfwps-20230711/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30276 2023-07-11 15:46:35.000000 libfwps-20230711/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2023-07-11 15:46:15.000000 libfwps-20230711/libcthreads/libcthreads_queue.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       91 2023-07-10 19:41:07.000000 libfwps-20230711/AUTHORS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35409 2023-07-11 15:46:34.000000 libfwps-20230711/config.sub
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:09.000000 libfwps-20230711/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      130 2016-02-02 07:37:21.000000 libfwps-20230711/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5538 2023-07-11 14:49:56.000000 libfwps-20230711/manuals/libfwps.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22665 2023-07-11 15:46:35.000000 libfwps-20230711/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2022-07-11 04:42:36.000000 libfwps-20230711/ABOUT-NLS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/libfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6908 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/libfwps/libfwps.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/libfole/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4605 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/libfole/libfole.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/fwps_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5134 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/fwps_test_error/fwps_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/fwps_test_property_identifier/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/fwps_test_property_identifier/fwps_test_property_identifier.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/libclocale/libclocale.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      746 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/fwps_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5140 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/fwps_test_support/fwps_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/fwps_test_record/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5380 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/fwps_test_record/fwps_test_record.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/fwps_test_store/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5377 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/fwps_test_store/fwps_test_store.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/libuna/libuna.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/pyfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6809 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/pyfwps/pyfwps.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20168 2023-07-11 15:46:35.000000 libfwps-20230711/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/libcerror/libcerror.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12507 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/libfwps.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/fwps_test_set/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5371 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/fwps_test_set/fwps_test_set.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:10.000000 libfwps-20230711/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2023-07-11 14:53:14.000000 libfwps-20230711/msvscpp/libcdata/libcdata.vcproj
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)    11497 2023-07-10 19:41:22.000000 libfwps-20230711/setup.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49797 2023-07-11 15:46:34.000000 libfwps-20230711/config.guess
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-10 19:41:05.000000 libfwps-20230711/NEWS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:09.000000 libfwps-20230711/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1347 2023-07-10 19:41:07.000000 libfwps-20230711/ossfuzz/store_fuzzer.cc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      967 2023-07-10 19:41:07.000000 libfwps-20230711/ossfuzz/ossfuzz_libfwps.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1095 2023-02-02 04:33:25.000000 libfwps-20230711/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1329 2023-07-10 19:41:07.000000 libfwps-20230711/ossfuzz/set_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2023-07-10 19:41:07.000000 libfwps-20230711/ossfuzz/record_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31314 2023-07-11 15:46:35.000000 libfwps-20230711/ossfuzz/Makefile.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2023-07-11 15:46:35.000000 libfwps-20230711/test-driver
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1514601 2023-07-11 15:46:32.000000 libfwps-20230711/configure
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:09.000000 libfwps-20230711/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50988 2023-07-11 15:46:35.000000 libfwps-20230711/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2023-07-11 15:46:22.000000 libfwps-20230711/libuna/libuna_codepage_iso_8859_16.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:09.000000 libfwps-20230711/pyfwps/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_libcerror.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_unused.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2023-07-11 04:11:23.000000 libfwps-20230711/pyfwps/pyfwps_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1117 2023-07-11 04:11:54.000000 libfwps-20230711/pyfwps/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2023-07-11 04:11:07.000000 libfwps-20230711/pyfwps/pyfwps_libuna.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9101 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_records.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2296 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_sets.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2666 2023-07-11 14:59:31.000000 libfwps-20230711/pyfwps/pyfwps_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2133 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_store.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12160 2023-07-10 19:42:33.000000 libfwps-20230711/pyfwps/pyfwps_store.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2343 2023-07-10 19:42:33.000000 libfwps-20230711/pyfwps/pyfwps_set.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2359 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_records.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3254 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5565 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14766 2023-07-10 19:42:33.000000 libfwps-20230711/pyfwps/pyfwps_set.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8020 2023-07-11 04:11:32.000000 libfwps-20230711/pyfwps/pyfwps_string.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8919 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_sets.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44577 2023-07-11 15:46:35.000000 libfwps-20230711/pyfwps/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      965 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_libfwps.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23569 2023-07-11 15:28:44.000000 libfwps-20230711/pyfwps/pyfwps_record.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_guid.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_codepage.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_libfguid.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2891 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_guid.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2023-07-10 19:41:08.000000 libfwps-20230711/pyfwps/pyfwps_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38796 2023-07-11 15:46:34.000000 libfwps-20230711/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      298 2023-02-02 04:39:35.000000 libfwps-20230711/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:08.000000 libfwps-20230711/m4/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-07-10 19:41:08.000000 libfwps-20230711/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2022-07-11 04:42:36.000000 libfwps-20230711/m4/gettext.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      756 2020-07-16 10:33:58.000000 libfwps-20230711/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2022-07-11 04:42:36.000000 libfwps-20230711/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2023-07-11 15:46:29.000000 libfwps-20230711/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2022-07-11 04:42:36.000000 libfwps-20230711/m4/lib-ld.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2019-09-17 04:01:01.000000 libfwps-20230711/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2022-07-11 04:42:36.000000 libfwps-20230711/m4/lib-link.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17674 2021-12-18 05:56:55.000000 libfwps-20230711/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2023-07-11 15:46:28.000000 libfwps-20230711/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-07-11 04:42:36.000000 libfwps-20230711/m4/nls.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2019-09-17 04:01:01.000000 libfwps-20230711/m4/libclocale.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2019-09-17 04:01:01.000000 libfwps-20230711/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2022-07-11 04:42:36.000000 libfwps-20230711/m4/host-cpu-c-abi.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2019-09-17 04:01:01.000000 libfwps-20230711/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2023-07-11 15:46:29.000000 libfwps-20230711/m4/ltversion.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-01-14 09:27:01.000000 libfwps-20230711/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2022-07-11 04:42:36.000000 libfwps-20230711/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2023-07-11 15:46:29.000000 libfwps-20230711/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2022-07-11 04:42:36.000000 libfwps-20230711/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2014-07-31 05:12:52.000000 libfwps-20230711/m4/pthread.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2019-01-02 20:12:18.000000 libfwps-20230711/m4/common.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2019-09-17 04:01:01.000000 libfwps-20230711/m4/libcerror.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2019-09-17 04:01:01.000000 libfwps-20230711/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2022-07-11 04:42:36.000000 libfwps-20230711/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2023-07-11 15:46:29.000000 libfwps-20230711/m4/ltsugar.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3956 2019-09-17 04:01:01.000000 libfwps-20230711/m4/libfole.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2022-07-11 04:42:36.000000 libfwps-20230711/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2018-07-31 03:18:22.000000 libfwps-20230711/m4/types.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2023-07-10 19:41:05.000000 libfwps-20230711/COPYING.LESSER
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2527 2023-07-10 19:41:05.000000 libfwps-20230711/libfwps.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:08.000000 libfwps-20230711/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2023-07-11 15:46:11.000000 libfwps-20230711/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2023-07-11 15:46:11.000000 libfwps-20230711/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-07-11 15:46:11.000000 libfwps-20230711/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      605 2023-07-11 15:46:11.000000 libfwps-20230711/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2023-07-11 15:46:11.000000 libfwps-20230711/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-07-11 15:46:11.000000 libfwps-20230711/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2023-07-11 15:46:11.000000 libfwps-20230711/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2023-07-11 15:46:11.000000 libfwps-20230711/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-07-11 15:46:11.000000 libfwps-20230711/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26811 2023-07-11 15:46:34.000000 libfwps-20230711/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-07-11 15:46:11.000000 libfwps-20230711/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2023-07-11 15:46:11.000000 libfwps-20230711/libcerror/libcerror_system.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:08.000000 libfwps-20230711/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-07-11 15:46:14.000000 libfwps-20230711/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-07-11 15:46:14.000000 libfwps-20230711/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2023-07-11 15:46:14.000000 libfwps-20230711/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2023-07-11 15:46:14.000000 libfwps-20230711/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      693 2023-07-11 15:46:14.000000 libfwps-20230711/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2023-07-11 15:46:14.000000 libfwps-20230711/libcnotify/libcnotify_print.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2023-07-11 15:46:14.000000 libfwps-20230711/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2023-07-11 15:46:14.000000 libfwps-20230711/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-07-11 15:46:14.000000 libfwps-20230711/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2023-07-11 15:46:14.000000 libfwps-20230711/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27298 2023-07-11 15:46:34.000000 libfwps-20230711/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2023-07-11 15:46:14.000000 libfwps-20230711/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2023-07-11 15:46:14.000000 libfwps-20230711/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-07-11 15:46:14.000000 libfwps-20230711/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2023-07-11 15:46:28.000000 libfwps-20230711/ltmain.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2023-07-11 15:46:34.000000 libfwps-20230711/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2022-07-11 04:42:36.000000 libfwps-20230711/config.rpath
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2023-07-11 15:46:35.000000 libfwps-20230711/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:09.000000 libfwps-20230711/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2022-07-11 04:42:36.000000 libfwps-20230711/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2022-07-11 04:42:36.000000 libfwps-20230711/po/Rules-quot
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2014-07-31 05:12:52.000000 libfwps-20230711/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2022-07-11 04:42:36.000000 libfwps-20230711/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2014-07-31 05:12:52.000000 libfwps-20230711/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2016-11-04 14:23:16.000000 libfwps-20230711/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2022-07-11 04:42:36.000000 libfwps-20230711/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2014-07-31 05:12:52.000000 libfwps-20230711/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1809 2023-07-11 15:46:45.000000 libfwps-20230711/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2022-07-11 04:42:36.000000 libfwps-20230711/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2022-07-11 04:42:36.000000 libfwps-20230711/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2014-07-31 05:12:52.000000 libfwps-20230711/po/boldquot.sed
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-11 16:02:08.000000 libfwps-20230711/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29870 2023-07-11 15:46:34.000000 libfwps-20230711/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2023-07-11 15:46:10.000000 libfwps-20230711/libcdata/libcdata_btree.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      752 2023-07-10 19:41:05.000000 libfwps-20230711/acinclude.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5641 2023-07-11 04:18:01.000000 libfwps-20230711/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      347 2023-07-11 16:02:10.654007 libfwps-20230711/PKG-INFO
```

### Comparing `libfwps-20230202/libfwps/libfwps_record.h` & `libfwps-20230711/libfwps/libfwps_record.h`

 * *Files 15% similar despite different names*

```diff
@@ -164,14 +164,40 @@
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

### Comparing `libfwps-20230202/libfwps/libfwps_format_class_identifier.c` & `libfwps-20230711/libfwps/libfwps_format_class_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_libcdata.h` & `libfwps-20230711/libfwps/libfwps_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_extern.h` & `libfwps-20230711/libfwps/libfwps_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_store.c` & `libfwps-20230711/libfwps/libfwps_store.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_codepage.h` & `libfwps-20230711/libfwps/libfwps_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_format_class_identifier.h` & `libfwps-20230711/libfwps/libfwps_format_class_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_definitions.h.in` & `libfwps-20230711/libfwps/libfwps_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_property_identifier.h` & `libfwps-20230711/libfwps/libfwps_property_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_libcnotify.h` & `libfwps-20230711/libfwps/libfwps_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/Makefile.am` & `libfwps-20230711/libfwps/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_libfguid.h` & `libfwps-20230711/libfwps/libfwps_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_set.c` & `libfwps-20230711/libfwps/libfwps_set.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_definitions.h` & `libfwps-20230711/libfwps/libfwps_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwps/definitions.h> are copied here
  * for local use of libfwps
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWPS_VERSION					20230202
+#define LIBFWPS_VERSION					20230711
 
 /* The version string
  */
-#define LIBFWPS_VERSION_STRING				"20230202"
+#define LIBFWPS_VERSION_STRING				"20230711"
 
 /* The byte order definitions
  */
 #define LIBFWPS_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWPS_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The value types
```

### Comparing `libfwps-20230202/libfwps/libfwps.c` & `libfwps-20230711/libfwps/libfwps.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_libuna.h` & `libfwps-20230711/libfwps/libfwps_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_libfole.h` & `libfwps-20230711/libfwps/libfwps_libfole.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_store.h` & `libfwps-20230711/libfwps/libfwps_store.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps.rc` & `libfwps-20230711/libfwps/libfwps.rc`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Windows Property Store format\0"
-      VALUE "FileVersion",		"20230202" "\0"
+      VALUE "FileVersion",		"20230711" "\0"
       VALUE "InternalName",		"libfwps.dll\0"
       VALUE "LegalCopyright",		"(C) 2013-2023, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfwps.dll\0"
       VALUE "ProductName",		"libfwps\0"
-      VALUE "ProductVersion",		"20230202" "\0"
+      VALUE "ProductVersion",		"20230711" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfwps/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfwps-20230202/libfwps/libfwps_error.c` & `libfwps-20230711/libfwps/libfwps_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_support.c` & `libfwps-20230711/libfwps/libfwps_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/Makefile.in` & `libfwps-20230711/libfwps/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_libcerror.h` & `libfwps-20230711/libfwps/libfwps_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_property_identifier.c` & `libfwps-20230711/libfwps/libfwps_property_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_types.h` & `libfwps-20230711/libfwps/libfwps_types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_record.c` & `libfwps-20230711/libfwps/libfwps_record.c`

 * *Files 14% similar despite different names*

```diff
@@ -1275,14 +1275,15 @@
 
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
@@ -1525,14 +1526,15 @@
 
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
@@ -1733,14 +1735,520 @@
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

### Comparing `libfwps-20230202/libfwps/libfwps_unused.h` & `libfwps-20230711/libfwps/libfwps_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_support.h` & `libfwps-20230711/libfwps/libfwps_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps.rc.in` & `libfwps-20230711/libfwps/libfwps.rc.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_set.h` & `libfwps-20230711/libfwps/libfwps_set.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps/libfwps_error.h` & `libfwps-20230711/libfwps/libfwps_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/common/config_msc.h` & `libfwps-20230711/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/common/byte_stream.h` & `libfwps-20230711/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/common/common.h` & `libfwps-20230711/common/common.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/common/system_string.h` & `libfwps-20230711/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/common/types.h` & `libfwps-20230711/common/types.h`

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

### Comparing `libfwps-20230202/common/types.h.in` & `libfwps-20230711/common/types.h.in`

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

### Comparing `libfwps-20230202/common/config_winapi.h` & `libfwps-20230711/common/config_winapi.h`

 * *Files 10% similar despite different names*

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

### Comparing `libfwps-20230202/common/memory.h` & `libfwps-20230711/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/common/config.h` & `libfwps-20230711/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -394,24 +394,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfwps"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfwps 20230202"
+#define PACKAGE_STRING "libfwps 20230711"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfwps"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20230202"
+#define PACKAGE_VERSION "20230711"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -429,15 +429,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20230202"
+#define VERSION "20230711"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfwps-20230202/common/narrow_string.h` & `libfwps-20230711/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/common/Makefile.in` & `libfwps-20230711/common/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/common/file_stream.h` & `libfwps-20230711/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/common/config_borlandc.h` & `libfwps-20230711/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/common/config.h.in` & `libfwps-20230711/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/common/wide_string.h` & `libfwps-20230711/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfole/libfole_definitions.h` & `libfwps-20230711/libfole/libfole_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfole/Makefile.am` & `libfwps-20230711/libfole/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfole/libfole_support.h` & `libfwps-20230711/libfole/libfole_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfole/libfole_extern.h` & `libfwps-20230711/libfole/libfole_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfole/libfole_error.c` & `libfwps-20230711/libfole/libfole_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfole/libfole_libcerror.h` & `libfwps-20230711/libfole/libfole_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfole/libfole_value_type.h` & `libfwps-20230711/libfole/libfole_value_type.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfole/libfole_unused.h` & `libfwps-20230711/libfole/libfole_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfole/libfole_value_type.c` & `libfwps-20230711/libfole/libfole_value_type.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfole/libfole_error.h` & `libfwps-20230711/libfole/libfole_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfole/Makefile.in` & `libfwps-20230711/libfole/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfole/libfole_support.c` & `libfwps-20230711/libfole/libfole_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfole/libfole_types.h` & `libfwps-20230711/libfole/libfole_types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfguid/libfguid_identifier.c` & `libfwps-20230711/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfguid/libfguid_support.c` & `libfwps-20230711/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfguid/Makefile.am` & `libfwps-20230711/libfguid/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfguid/libfguid_support.h` & `libfwps-20230711/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfguid/libfguid_definitions.h` & `libfwps-20230711/libfguid/libfguid_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfguid/libfguid_identifier.h` & `libfwps-20230711/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfguid/libfguid_unused.h` & `libfwps-20230711/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfguid/libfguid_error.h` & `libfwps-20230711/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfguid/libfguid_libcerror.h` & `libfwps-20230711/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfguid/Makefile.in` & `libfwps-20230711/libfguid/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfguid/libfguid_error.c` & `libfwps-20230711/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfguid/libfguid_types.h` & `libfwps-20230711/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfguid/libfguid_extern.h` & `libfwps-20230711/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/test_library.sh` & `libfwps-20230711/tests/test_library.sh`

 * *Files 4% similar despite different names*

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
 
 LIBRARY_TESTS="error property_identifier record set store support";
 LIBRARY_TESTS_WITH_INPUT="";
```

### Comparing `libfwps-20230202/tests/pyfwps_test_support.py` & `libfwps-20230711/tests/pyfwps_test_support.py`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/test_python_module.sh` & `libfwps-20230711/tests/test_python_module.sh`

 * *Files 2% similar despite different names*

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
 TEST_FUNCTIONS_WITH_INPUT="";
```

### Comparing `libfwps-20230202/tests/Makefile.am` & `libfwps-20230711/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/pyfwps_test_store.py` & `libfwps-20230711/tests/pyfwps_test_store.py`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/fwps_test_unused.h` & `libfwps-20230711/tests/fwps_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/pyfwps_test_set.py` & `libfwps-20230711/tests/pyfwps_test_set.py`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/fwps_test_macros.h` & `libfwps-20230711/tests/fwps_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/fwps_test_support.c` & `libfwps-20230711/tests/fwps_test_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/fwps_test_set.c` & `libfwps-20230711/tests/fwps_test_set.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/fwps_test_libcerror.h` & `libfwps-20230711/tests/fwps_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/test_manpage.sh` & `libfwps-20230711/tests/test_manpage.sh`

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

### Comparing `libfwps-20230202/tests/fwps_test_libfwps.h` & `libfwps-20230711/tests/fwps_test_libfwps.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/test_runner.sh` & `libfwps-20230711/tests/test_runner.sh`

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

### Comparing `libfwps-20230202/tests/fwps_test_property_identifier.c` & `libfwps-20230711/tests/fwps_test_property_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/fwps_test_record.c` & `libfwps-20230711/tests/fwps_test_record.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/fwps_test_memory.h` & `libfwps-20230711/tests/fwps_test_memory.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/fwps_test_error.c` & `libfwps-20230711/tests/fwps_test_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/Makefile.in` & `libfwps-20230711/tests/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/fwps_test_store.c` & `libfwps-20230711/tests/fwps_test_store.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/tests/fwps_test_memory.c` & `libfwps-20230711/tests/fwps_test_memory.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libclocale/libclocale_wide_string.h` & `libfwps-20230711/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libclocale/libclocale_support.c` & `libfwps-20230711/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libclocale/libclocale_locale.h` & `libfwps-20230711/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libclocale/Makefile.am` & `libfwps-20230711/libclocale/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libclocale/libclocale_locale.c` & `libfwps-20230711/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libclocale/libclocale_extern.h` & `libfwps-20230711/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libclocale/libclocale_unused.h` & `libfwps-20230711/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libclocale/libclocale_support.h` & `libfwps-20230711/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libclocale/libclocale_definitions.h` & `libfwps-20230711/libclocale/libclocale_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libclocale/libclocale_codepage.h` & `libfwps-20230711/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libclocale/libclocale_codepage.c` & `libfwps-20230711/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libclocale/Makefile.in` & `libfwps-20230711/libclocale/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libclocale/libclocale_wide_string.c` & `libfwps-20230711/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libclocale/libclocale_libcerror.h` & `libfwps-20230711/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/missing` & `libfwps-20230711/missing`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/Makefile.am` & `libfwps-20230711/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/aclocal.m4` & `libfwps-20230711/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps-python3/Makefile.am` & `libfwps-20230711/pyfwps-python3/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -23,20 +23,22 @@
 	pyfwps_error.c pyfwps_error.h \
 	pyfwps_guid.c pyfwps_guid.h \
 	pyfwps_integer.c pyfwps_integer.h \
 	pyfwps_libcerror.h \
 	pyfwps_libclocale.h \
 	pyfwps_libfguid.h \
 	pyfwps_libfwps.h \
+	pyfwps_libuna.h \
 	pyfwps_python.h \
 	pyfwps_record.c pyfwps_record.h \
 	pyfwps_records.c pyfwps_records.h \
 	pyfwps_set.c pyfwps_set.h \
 	pyfwps_sets.c pyfwps_sets.h \
 	pyfwps_store.c pyfwps_store.h \
+	pyfwps_string.c pyfwps_string.h \
 	pyfwps_unused.h
 
 pyexec_LTLIBRARIES = pyfwps.la
 
 nodist_pyfwps_la_SOURCES = $(BUILT_SOURCES)
 
 pyfwps_la_LIBADD = \
```

### Comparing `libfwps-20230202/pyfwps-python3/Makefile.in` & `libfwps-20230711/pyfwps-python3/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,16 @@
 @HAVE_PYTHON3_TRUE@	pyfwps_la-pyfwps_error.lo \
 @HAVE_PYTHON3_TRUE@	pyfwps_la-pyfwps_guid.lo \
 @HAVE_PYTHON3_TRUE@	pyfwps_la-pyfwps_integer.lo \
 @HAVE_PYTHON3_TRUE@	pyfwps_la-pyfwps_record.lo \
 @HAVE_PYTHON3_TRUE@	pyfwps_la-pyfwps_records.lo \
 @HAVE_PYTHON3_TRUE@	pyfwps_la-pyfwps_set.lo \
 @HAVE_PYTHON3_TRUE@	pyfwps_la-pyfwps_sets.lo \
-@HAVE_PYTHON3_TRUE@	pyfwps_la-pyfwps_store.lo
+@HAVE_PYTHON3_TRUE@	pyfwps_la-pyfwps_store.lo \
+@HAVE_PYTHON3_TRUE@	pyfwps_la-pyfwps_string.lo
 @HAVE_PYTHON3_TRUE@nodist_pyfwps_la_OBJECTS = $(am__objects_1)
 pyfwps_la_OBJECTS = $(nodist_pyfwps_la_OBJECTS)
 AM_V_lt = $(am__v_lt_@AM_V@)
 am__v_lt_ = $(am__v_lt_@AM_DEFAULT_V@)
 am__v_lt_0 = --silent
 am__v_lt_1 = 
 pyfwps_la_LINK = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
@@ -181,15 +182,16 @@
 	./$(DEPDIR)/pyfwps_la-pyfwps_error.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_guid.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_integer.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_record.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_records.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_set.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_sets.Plo \
-	./$(DEPDIR)/pyfwps_la-pyfwps_store.Plo
+	./$(DEPDIR)/pyfwps_la-pyfwps_store.Plo \
+	./$(DEPDIR)/pyfwps_la-pyfwps_string.Plo
 am__mv = mv -f
 COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
 	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
 LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) \
 	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
 	$(AM_CFLAGS) $(CFLAGS)
@@ -539,20 +541,22 @@
 @HAVE_PYTHON3_TRUE@	pyfwps_error.c pyfwps_error.h \
 @HAVE_PYTHON3_TRUE@	pyfwps_guid.c pyfwps_guid.h \
 @HAVE_PYTHON3_TRUE@	pyfwps_integer.c pyfwps_integer.h \
 @HAVE_PYTHON3_TRUE@	pyfwps_libcerror.h \
 @HAVE_PYTHON3_TRUE@	pyfwps_libclocale.h \
 @HAVE_PYTHON3_TRUE@	pyfwps_libfguid.h \
 @HAVE_PYTHON3_TRUE@	pyfwps_libfwps.h \
+@HAVE_PYTHON3_TRUE@	pyfwps_libuna.h \
 @HAVE_PYTHON3_TRUE@	pyfwps_python.h \
 @HAVE_PYTHON3_TRUE@	pyfwps_record.c pyfwps_record.h \
 @HAVE_PYTHON3_TRUE@	pyfwps_records.c pyfwps_records.h \
 @HAVE_PYTHON3_TRUE@	pyfwps_set.c pyfwps_set.h \
 @HAVE_PYTHON3_TRUE@	pyfwps_sets.c pyfwps_sets.h \
 @HAVE_PYTHON3_TRUE@	pyfwps_store.c pyfwps_store.h \
+@HAVE_PYTHON3_TRUE@	pyfwps_string.c pyfwps_string.h \
 @HAVE_PYTHON3_TRUE@	pyfwps_unused.h
 
 @HAVE_PYTHON3_TRUE@pyexec_LTLIBRARIES = pyfwps.la
 @HAVE_PYTHON3_TRUE@nodist_pyfwps_la_SOURCES = $(BUILT_SOURCES)
 @HAVE_PYTHON3_TRUE@pyfwps_la_LIBADD = \
 @HAVE_PYTHON3_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_PYTHON3_TRUE@	../libfwps/libfwps.la \
@@ -651,14 +655,15 @@
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_guid.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_integer.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_record.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_records.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_set.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_sets.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_store.Plo@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_string.Plo@am__quote@ # am--include-marker
 
 $(am__depfiles_remade):
 	@$(MKDIR_P) $(@D)
 	@echo '# dummy' >$@-t && $(am__mv) $@-t $@
 
 am--depfiles: $(am__depfiles_remade)
 
@@ -749,14 +754,21 @@
 pyfwps_la-pyfwps_store.lo: pyfwps_store.c
 @am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwps_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pyfwps_la-pyfwps_store.lo -MD -MP -MF $(DEPDIR)/pyfwps_la-pyfwps_store.Tpo -c -o pyfwps_la-pyfwps_store.lo `test -f 'pyfwps_store.c' || echo '$(srcdir)/'`pyfwps_store.c
 @am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pyfwps_la-pyfwps_store.Tpo $(DEPDIR)/pyfwps_la-pyfwps_store.Plo
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pyfwps_store.c' object='pyfwps_la-pyfwps_store.lo' libtool=yes @AMDEPBACKSLASH@
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
 @am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwps_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pyfwps_la-pyfwps_store.lo `test -f 'pyfwps_store.c' || echo '$(srcdir)/'`pyfwps_store.c
 
+pyfwps_la-pyfwps_string.lo: pyfwps_string.c
+@am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwps_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pyfwps_la-pyfwps_string.lo -MD -MP -MF $(DEPDIR)/pyfwps_la-pyfwps_string.Tpo -c -o pyfwps_la-pyfwps_string.lo `test -f 'pyfwps_string.c' || echo '$(srcdir)/'`pyfwps_string.c
+@am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pyfwps_la-pyfwps_string.Tpo $(DEPDIR)/pyfwps_la-pyfwps_string.Plo
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pyfwps_string.c' object='pyfwps_la-pyfwps_string.lo' libtool=yes @AMDEPBACKSLASH@
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
+@am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwps_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pyfwps_la-pyfwps_string.lo `test -f 'pyfwps_string.c' || echo '$(srcdir)/'`pyfwps_string.c
+
 mostlyclean-libtool:
 	-rm -f *.lo
 
 clean-libtool:
 	-rm -rf .libs _libs
 
 ID: $(am__tagged_files)
@@ -940,14 +952,15 @@
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_guid.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_integer.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_record.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_records.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_set.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_sets.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_store.Plo
+	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_string.Plo
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
 
 mostlyclean: mostlyclean-am
 
 mostlyclean-am: mostlyclean-compile mostlyclean-generic \
 	mostlyclean-libtool
```

### Comparing `libfwps-20230202/COPYING` & `libfwps-20230711/COPYING`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps.spec` & `libfwps-20230711/libfwps.spec`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Name: libfwps
-Version: 20230202
+Version: 20230711
 Release: 1
 Summary: Library to access the Windows Property Store format
 Group: System Environment/Libraries
-License: LGPLv3+
+License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfwps
-BuildRoot: %{_tmppath}/%{name}-%{version}-%{release}-root-%(%{__id_u} -n)
          
 BuildRequires: gcc         
 
 %description -n libfwps
 Library to access the Windows Property Store format
 
 %package -n libfwps-static
@@ -53,38 +52,34 @@
 rm -rf %{buildroot}
 
 %post -p /sbin/ldconfig
 
 %postun -p /sbin/ldconfig
 
 %files -n libfwps
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
-%attr(755,root,root) %{_libdir}/*.so.*
+%{_libdir}/*.so.*
 
 %files -n libfwps-static
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
-%attr(755,root,root) %{_libdir}/*.a
+%{_libdir}/*.a
 
 %files -n libfwps-devel
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/*.so
 %{_libdir}/pkgconfig/libfwps.pc
 %{_includedir}/*
 %{_mandir}/man3/*
 
 %files -n libfwps-python3
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %changelog
-* Sat Feb  4 2023 Joachim Metz <joachim.metz@gmail.com> 20230202-1
+* Tue Jul 11 2023 Joachim Metz <joachim.metz@gmail.com> 20230711-1
 - Auto-generated
```

### Comparing `libfwps-20230202/include/libfwps/definitions.h.in` & `libfwps-20230711/include/libfwps/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/include/libfwps/extern.h` & `libfwps-20230711/include/libfwps/extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/include/libfwps/types.h` & `libfwps-20230711/include/libfwps/types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/include/libfwps/features.h.in` & `libfwps-20230711/include/libfwps/features.h.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/include/libfwps/types.h.in` & `libfwps-20230711/include/libfwps/types.h.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/include/libfwps/features.h` & `libfwps-20230711/include/libfwps/features.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/include/libfwps/definitions.h` & `libfwps-20230711/include/libfwps/definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBFWPS_DEFINITIONS_H )
 #define _LIBFWPS_DEFINITIONS_H
 
 #include <libfwps/types.h>
 
-#define LIBFWPS_VERSION					20230202
+#define LIBFWPS_VERSION					20230711
 
 /* The version string
  */
-#define LIBFWPS_VERSION_STRING				"20230202"
+#define LIBFWPS_VERSION_STRING				"20230711"
 
 /* The byte order definitions
  */
 enum LIBFWPS_ENDIAN
 {
 	LIBFWPS_ENDIAN_BIG				= (int) 'b',
 	LIBFWPS_ENDIAN_LITTLE				= (int) 'l'
```

### Comparing `libfwps-20230202/include/libfwps/codepage.h` & `libfwps-20230711/include/libfwps/codepage.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/include/libfwps/error.h` & `libfwps-20230711/include/libfwps/error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/include/Makefile.in` & `libfwps-20230711/include/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/include/libfwps.h.in` & `libfwps-20230711/include/libfwps.h.in`

 * *Files 20% similar despite different names*

```diff
@@ -197,14 +197,15 @@
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_floating_point(
      libfwps_record_t *record,
      double *value_floating_point,
      libfwps_error_t **error );
 
 /* Retrieves the size of the data formatted as an UTF-8 string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
  * The returned size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_utf8_string_size(
      libfwps_record_t *record,
      size_t *utf8_string_size,
@@ -219,14 +220,15 @@
 int libfwps_record_get_data_as_utf8_string(
      libfwps_record_t *record,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      libfwps_error_t **error );
 
 /* Retrieves the size of the data formatted as an UTF-16 string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
  * The returned size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_utf16_string_size(
      libfwps_record_t *record,
      size_t *utf16_string_size,
@@ -240,14 +242,64 @@
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_utf16_string(
      libfwps_record_t *record,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      libfwps_error_t **error );
 
+/* Retrieves the size of the data formatted as an UTF-8 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The returned size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf8_path_string_size(
+     libfwps_record_t *record,
+     size_t *utf8_string_size,
+     libfwps_error_t **error );
+
+/* Retrieves the data formatted as an UTF-8 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf8_path_string(
+     libfwps_record_t *record,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     libfwps_error_t **error );
+
+/* Retrieves the size of the data formatted as an UTF-16 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The returned size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf16_path_string_size(
+     libfwps_record_t *record,
+     size_t *utf16_string_size,
+     libfwps_error_t **error );
+
+/* Retrieves the data formatted as an UTF-16 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf16_path_string(
+     libfwps_record_t *record,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     libfwps_error_t **error );
+
 /* Retrieves the data as a GUID value
  * Returns 1 if successful or -1 on error
  */
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_guid(
      libfwps_record_t *record,
      uint8_t *guid_data,
```

### Comparing `libfwps-20230202/include/libfwps.h` & `libfwps-20230711/include/libfwps.h`

 * *Files 20% similar despite different names*

```diff
@@ -197,14 +197,15 @@
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_floating_point(
      libfwps_record_t *record,
      double *value_floating_point,
      libfwps_error_t **error );
 
 /* Retrieves the size of the data formatted as an UTF-8 string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
  * The returned size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_utf8_string_size(
      libfwps_record_t *record,
      size_t *utf8_string_size,
@@ -219,14 +220,15 @@
 int libfwps_record_get_data_as_utf8_string(
      libfwps_record_t *record,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      libfwps_error_t **error );
 
 /* Retrieves the size of the data formatted as an UTF-16 string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
  * The returned size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_utf16_string_size(
      libfwps_record_t *record,
      size_t *utf16_string_size,
@@ -240,14 +242,64 @@
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_utf16_string(
      libfwps_record_t *record,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      libfwps_error_t **error );
 
+/* Retrieves the size of the data formatted as an UTF-8 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The returned size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf8_path_string_size(
+     libfwps_record_t *record,
+     size_t *utf8_string_size,
+     libfwps_error_t **error );
+
+/* Retrieves the data formatted as an UTF-8 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf8_path_string(
+     libfwps_record_t *record,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     libfwps_error_t **error );
+
+/* Retrieves the size of the data formatted as an UTF-16 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The returned size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf16_path_string_size(
+     libfwps_record_t *record,
+     size_t *utf16_string_size,
+     libfwps_error_t **error );
+
+/* Retrieves the data formatted as an UTF-16 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf16_path_string(
+     libfwps_record_t *record,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     libfwps_error_t **error );
+
 /* Retrieves the data as a GUID value
  * Returns 1 if successful or -1 on error
  */
 LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_guid(
      libfwps_record_t *record,
      uint8_t *guid_data,
```

### Comparing `libfwps-20230202/libfwps.pc.in` & `libfwps-20230711/libfwps.pc.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/install-sh` & `libfwps-20230711/install-sh`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps-python2/Makefile.am` & `libfwps-20230711/pyfwps-python2/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -23,20 +23,22 @@
 	pyfwps_error.c pyfwps_error.h \
 	pyfwps_guid.c pyfwps_guid.h \
 	pyfwps_integer.c pyfwps_integer.h \
 	pyfwps_libcerror.h \
 	pyfwps_libclocale.h \
 	pyfwps_libfguid.h \
 	pyfwps_libfwps.h \
+	pyfwps_libuna.h \
 	pyfwps_python.h \
 	pyfwps_record.c pyfwps_record.h \
 	pyfwps_records.c pyfwps_records.h \
 	pyfwps_set.c pyfwps_set.h \
 	pyfwps_sets.c pyfwps_sets.h \
 	pyfwps_store.c pyfwps_store.h \
+	pyfwps_string.c pyfwps_string.h \
 	pyfwps_unused.h
 
 pyexec_LTLIBRARIES = pyfwps.la
 
 nodist_pyfwps_la_SOURCES = $(BUILT_SOURCES)
 
 pyfwps_la_LIBADD = \
```

### Comparing `libfwps-20230202/pyfwps-python2/Makefile.in` & `libfwps-20230711/pyfwps-python2/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,16 @@
 @HAVE_PYTHON2_TRUE@	pyfwps_la-pyfwps_error.lo \
 @HAVE_PYTHON2_TRUE@	pyfwps_la-pyfwps_guid.lo \
 @HAVE_PYTHON2_TRUE@	pyfwps_la-pyfwps_integer.lo \
 @HAVE_PYTHON2_TRUE@	pyfwps_la-pyfwps_record.lo \
 @HAVE_PYTHON2_TRUE@	pyfwps_la-pyfwps_records.lo \
 @HAVE_PYTHON2_TRUE@	pyfwps_la-pyfwps_set.lo \
 @HAVE_PYTHON2_TRUE@	pyfwps_la-pyfwps_sets.lo \
-@HAVE_PYTHON2_TRUE@	pyfwps_la-pyfwps_store.lo
+@HAVE_PYTHON2_TRUE@	pyfwps_la-pyfwps_store.lo \
+@HAVE_PYTHON2_TRUE@	pyfwps_la-pyfwps_string.lo
 @HAVE_PYTHON2_TRUE@nodist_pyfwps_la_OBJECTS = $(am__objects_1)
 pyfwps_la_OBJECTS = $(nodist_pyfwps_la_OBJECTS)
 AM_V_lt = $(am__v_lt_@AM_V@)
 am__v_lt_ = $(am__v_lt_@AM_DEFAULT_V@)
 am__v_lt_0 = --silent
 am__v_lt_1 = 
 pyfwps_la_LINK = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
@@ -181,15 +182,16 @@
 	./$(DEPDIR)/pyfwps_la-pyfwps_error.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_guid.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_integer.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_record.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_records.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_set.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_sets.Plo \
-	./$(DEPDIR)/pyfwps_la-pyfwps_store.Plo
+	./$(DEPDIR)/pyfwps_la-pyfwps_store.Plo \
+	./$(DEPDIR)/pyfwps_la-pyfwps_string.Plo
 am__mv = mv -f
 COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
 	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
 LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) \
 	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
 	$(AM_CFLAGS) $(CFLAGS)
@@ -539,20 +541,22 @@
 @HAVE_PYTHON2_TRUE@	pyfwps_error.c pyfwps_error.h \
 @HAVE_PYTHON2_TRUE@	pyfwps_guid.c pyfwps_guid.h \
 @HAVE_PYTHON2_TRUE@	pyfwps_integer.c pyfwps_integer.h \
 @HAVE_PYTHON2_TRUE@	pyfwps_libcerror.h \
 @HAVE_PYTHON2_TRUE@	pyfwps_libclocale.h \
 @HAVE_PYTHON2_TRUE@	pyfwps_libfguid.h \
 @HAVE_PYTHON2_TRUE@	pyfwps_libfwps.h \
+@HAVE_PYTHON2_TRUE@	pyfwps_libuna.h \
 @HAVE_PYTHON2_TRUE@	pyfwps_python.h \
 @HAVE_PYTHON2_TRUE@	pyfwps_record.c pyfwps_record.h \
 @HAVE_PYTHON2_TRUE@	pyfwps_records.c pyfwps_records.h \
 @HAVE_PYTHON2_TRUE@	pyfwps_set.c pyfwps_set.h \
 @HAVE_PYTHON2_TRUE@	pyfwps_sets.c pyfwps_sets.h \
 @HAVE_PYTHON2_TRUE@	pyfwps_store.c pyfwps_store.h \
+@HAVE_PYTHON2_TRUE@	pyfwps_string.c pyfwps_string.h \
 @HAVE_PYTHON2_TRUE@	pyfwps_unused.h
 
 @HAVE_PYTHON2_TRUE@pyexec_LTLIBRARIES = pyfwps.la
 @HAVE_PYTHON2_TRUE@nodist_pyfwps_la_SOURCES = $(BUILT_SOURCES)
 @HAVE_PYTHON2_TRUE@pyfwps_la_LIBADD = \
 @HAVE_PYTHON2_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_PYTHON2_TRUE@	../libfwps/libfwps.la \
@@ -651,14 +655,15 @@
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_guid.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_integer.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_record.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_records.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_set.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_sets.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_store.Plo@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_string.Plo@am__quote@ # am--include-marker
 
 $(am__depfiles_remade):
 	@$(MKDIR_P) $(@D)
 	@echo '# dummy' >$@-t && $(am__mv) $@-t $@
 
 am--depfiles: $(am__depfiles_remade)
 
@@ -749,14 +754,21 @@
 pyfwps_la-pyfwps_store.lo: pyfwps_store.c
 @am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwps_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pyfwps_la-pyfwps_store.lo -MD -MP -MF $(DEPDIR)/pyfwps_la-pyfwps_store.Tpo -c -o pyfwps_la-pyfwps_store.lo `test -f 'pyfwps_store.c' || echo '$(srcdir)/'`pyfwps_store.c
 @am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pyfwps_la-pyfwps_store.Tpo $(DEPDIR)/pyfwps_la-pyfwps_store.Plo
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pyfwps_store.c' object='pyfwps_la-pyfwps_store.lo' libtool=yes @AMDEPBACKSLASH@
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
 @am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwps_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pyfwps_la-pyfwps_store.lo `test -f 'pyfwps_store.c' || echo '$(srcdir)/'`pyfwps_store.c
 
+pyfwps_la-pyfwps_string.lo: pyfwps_string.c
+@am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwps_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pyfwps_la-pyfwps_string.lo -MD -MP -MF $(DEPDIR)/pyfwps_la-pyfwps_string.Tpo -c -o pyfwps_la-pyfwps_string.lo `test -f 'pyfwps_string.c' || echo '$(srcdir)/'`pyfwps_string.c
+@am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pyfwps_la-pyfwps_string.Tpo $(DEPDIR)/pyfwps_la-pyfwps_string.Plo
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pyfwps_string.c' object='pyfwps_la-pyfwps_string.lo' libtool=yes @AMDEPBACKSLASH@
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
+@am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwps_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pyfwps_la-pyfwps_string.lo `test -f 'pyfwps_string.c' || echo '$(srcdir)/'`pyfwps_string.c
+
 mostlyclean-libtool:
 	-rm -f *.lo
 
 clean-libtool:
 	-rm -rf .libs _libs
 
 ID: $(am__tagged_files)
@@ -940,14 +952,15 @@
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_guid.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_integer.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_record.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_records.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_set.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_sets.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_store.Plo
+	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_string.Plo
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
 
 mostlyclean: mostlyclean-am
 
 mostlyclean-am: mostlyclean-compile mostlyclean-generic \
 	mostlyclean-libtool
```

### Comparing `libfwps-20230202/INSTALL` & `libfwps-20230711/INSTALL`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/dpkg/copyright` & `libfwps-20230711/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/dpkg/rules` & `libfwps-20230711/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/dpkg/control` & `libfwps-20230711/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_support.c` & `libfwps-20230711/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_systemtime.h` & `libfwps-20230711/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_error.h` & `libfwps-20230711/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/Makefile.am` & `libfwps-20230711/libfdatetime/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_unused.h` & `libfwps-20230711/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_error.c` & `libfwps-20230711/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_posix_time.c` & `libfwps-20230711/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_fat_date_time.h` & `libfwps-20230711/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_types.h` & `libfwps-20230711/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_floatingtime.c` & `libfwps-20230711/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_hfs_time.h` & `libfwps-20230711/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_support.h` & `libfwps-20230711/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_extern.h` & `libfwps-20230711/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_filetime.h` & `libfwps-20230711/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_date_time_values.c` & `libfwps-20230711/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_floatingtime.h` & `libfwps-20230711/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_libcerror.h` & `libfwps-20230711/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/Makefile.in` & `libfwps-20230711/libfdatetime/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_nsf_timedate.c` & `libfwps-20230711/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_date_time_values.h` & `libfwps-20230711/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_hfs_time.c` & `libfwps-20230711/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_posix_time.h` & `libfwps-20230711/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_fat_date_time.c` & `libfwps-20230711/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_nsf_timedate.h` & `libfwps-20230711/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_definitions.h` & `libfwps-20230711/libfdatetime/libfdatetime_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_systemtime.c` & `libfwps-20230711/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfdatetime/libfdatetime_filetime.c` & `libfwps-20230711/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_thread_pool.h` & `libfwps-20230711/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_thread_pool.c` & `libfwps-20230711/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_repeating_thread.c` & `libfwps-20230711/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_error.c` & `libfwps-20230711/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/Makefile.am` & `libfwps-20230711/libcthreads/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_unused.h` & `libfwps-20230711/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_condition.h` & `libfwps-20230711/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_definitions.h` & `libfwps-20230711/libcthreads/libcthreads_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_thread.h` & `libfwps-20230711/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_repeating_thread.h` & `libfwps-20230711/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_read_write_lock.c` & `libfwps-20230711/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_mutex.h` & `libfwps-20230711/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_support.h` & `libfwps-20230711/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_thread.c` & `libfwps-20230711/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_mutex.c` & `libfwps-20230711/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_types.h` & `libfwps-20230711/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_lock.h` & `libfwps-20230711/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_extern.h` & `libfwps-20230711/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_error.h` & `libfwps-20230711/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_queue.c` & `libfwps-20230711/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_condition.c` & `libfwps-20230711/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/Makefile.in` & `libfwps-20230711/libcthreads/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_thread_attributes.c` & `libfwps-20230711/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_libcerror.h` & `libfwps-20230711/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_lock.c` & `libfwps-20230711/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_support.c` & `libfwps-20230711/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_read_write_lock.h` & `libfwps-20230711/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_thread_attributes.h` & `libfwps-20230711/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcthreads/libcthreads_queue.h` & `libfwps-20230711/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/config.sub` & `libfwps-20230711/config.sub`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/manuals/libfwps.3` & `libfwps-20230711/manuals/libfwps.3`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.Dd January 30, 2023
+.Dd July 11, 2023
 .Dt libfwps 3
 .Os libfwps
 .Sh NAME
 .Nm libfwps.h
 .Nd Library to access the Windows Property Store format
 .Sh SYNOPSIS
 .In libfwps.h
@@ -55,14 +55,22 @@
 .Ft int
 .Fn libfwps_record_get_data_as_utf8_string "libfwps_record_t *record" "uint8_t *utf8_string" "size_t utf8_string_size" "libfwps_error_t **error"
 .Ft int
 .Fn libfwps_record_get_data_as_utf16_string_size "libfwps_record_t *record" "size_t *utf16_string_size" "libfwps_error_t **error"
 .Ft int
 .Fn libfwps_record_get_data_as_utf16_string "libfwps_record_t *record" "uint16_t *utf16_string" "size_t utf16_string_size" "libfwps_error_t **error"
 .Ft int
+.Fn libfwps_record_get_data_as_utf8_path_string_size "libfwps_record_t *record" "size_t *utf8_string_size" "libfwps_error_t **error"
+.Ft int
+.Fn libfwps_record_get_data_as_utf8_path_string "libfwps_record_t *record" "uint8_t *utf8_string" "size_t utf8_string_size" "libfwps_error_t **error"
+.Ft int
+.Fn libfwps_record_get_data_as_utf16_path_string_size "libfwps_record_t *record" "size_t *utf16_string_size" "libfwps_error_t **error"
+.Ft int
+.Fn libfwps_record_get_data_as_utf16_path_string "libfwps_record_t *record" "uint16_t *utf16_string" "size_t utf16_string_size" "libfwps_error_t **error"
+.Ft int
 .Fn libfwps_record_get_data_as_guid "libfwps_record_t *record" "uint8_t *guid_data" "size_t guid_data_size" "libfwps_error_t **error"
 .Pp
 Set functions
 .Ft int
 .Fn libfwps_set_initialize "libfwps_set_t **set" "libfwps_error_t **error"
 .Ft int
 .Fn libfwps_set_free "libfwps_set_t **set" "libfwps_error_t **error"
```

### Comparing `libfwps-20230202/manuals/Makefile.in` & `libfwps-20230711/manuals/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/libfwps/libfwps.vcproj` & `libfwps-20230711/msvscpp/libfwps/libfwps.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/libfole/libfole.vcproj` & `libfwps-20230711/msvscpp/libfole/libfole.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/fwps_test_error/fwps_test_error.vcproj` & `libfwps-20230711/msvscpp/fwps_test_error/fwps_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/libfguid/libfguid.vcproj` & `libfwps-20230711/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/fwps_test_property_identifier/fwps_test_property_identifier.vcproj` & `libfwps-20230711/msvscpp/fwps_test_property_identifier/fwps_test_property_identifier.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/libclocale/libclocale.vcproj` & `libfwps-20230711/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/Makefile.am` & `libfwps-20230711/msvscpp/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/fwps_test_support/fwps_test_support.vcproj` & `libfwps-20230711/msvscpp/fwps_test_support/fwps_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/fwps_test_record/fwps_test_record.vcproj` & `libfwps-20230711/msvscpp/fwps_test_record/fwps_test_record.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/fwps_test_store/fwps_test_store.vcproj` & `libfwps-20230711/msvscpp/fwps_test_store/fwps_test_store.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/libfdatetime/libfdatetime.vcproj` & `libfwps-20230711/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/libcthreads/libcthreads.vcproj` & `libfwps-20230711/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/libuna/libuna.vcproj` & `libfwps-20230711/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/pyfwps/pyfwps.vcproj` & `libfwps-20230711/msvscpp/pyfwps/pyfwps.vcproj`

 * *Files 6% similar despite different names*

#### Comparing `libfwps-20230202/msvscpp/pyfwps/pyfwps.vcproj` & `libfwps-20230711/msvscpp/pyfwps/pyfwps.vcproj`

```diff
@@ -7,15 +7,15 @@
   <Configurations>
     <Configuration Name="Release|Win32" OutputDirectory="$(SolutionDir)$(ConfigurationName)" IntermediateDirectory="$(ConfigurationName)" ConfigurationType="2" CharacterSet="1">
       <Tool Name="VCPreBuildEventTool"/>
       <Tool Name="VCCustomBuildTool"/>
       <Tool Name="VCXMLDataGeneratorTool"/>
       <Tool Name="VCWebServiceProxyGeneratorTool"/>
       <Tool Name="VCMIDLTool"/>
-      <Tool Name="VCCLCompilerTool" AdditionalIncludeDirectories="..\..\include;..\..\common;..\..\libcerror;..\..\libcdata;..\..\libclocale;..\..\libuna;..\..\libfguid;C:\Python27\include" PreprocessorDefinitions="_CRT_SECURE_NO_DEPRECATE;HAVE_LOCAL_LIBCERROR;HAVE_LOCAL_LIBCDATA;HAVE_LOCAL_LIBCLOCALE;HAVE_LOCAL_LIBUNA;HAVE_LOCAL_LIBFGUID;LIBFWPS_DLL_IMPORT" RuntimeLibrary="2" WarningLevel="4" CompileAs="1"/>
+      <Tool Name="VCCLCompilerTool" AdditionalIncludeDirectories="..\..\include;..\..\common;..\..\libcerror;..\..\libcdata;..\..\libclocale;..\..\libuna;..\..\libfguid;C:\Python27\include" PreprocessorDefinitions="_CRT_SECURE_NO_DEPRECATE;HAVE_PYCONFIG_H;HAVE_LOCAL_LIBCERROR;HAVE_LOCAL_LIBCDATA;HAVE_LOCAL_LIBCLOCALE;HAVE_LOCAL_LIBUNA;HAVE_LOCAL_LIBFGUID;LIBFWPS_DLL_IMPORT" RuntimeLibrary="2" WarningLevel="4" CompileAs="1"/>
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
-      <Tool Name="VCCLCompilerTool" Optimization="0" AdditionalIncludeDirectories="..\..\include;..\..\common;..\..\libcerror;..\..\libcdata;..\..\libclocale;..\..\libuna;..\..\libfguid;C:\Python27\include" PreprocessorDefinitions="_CRT_SECURE_NO_DEPRECATE;HAVE_LOCAL_LIBCERROR;HAVE_LOCAL_LIBCDATA;HAVE_LOCAL_LIBCLOCALE;HAVE_LOCAL_LIBUNA;HAVE_LOCAL_LIBFGUID;LIBFWPS_DLL_IMPORT" BasicRuntimeChecks="3" SmallerTypeCheck="true" RuntimeLibrary="3" WarningLevel="4" DebugInformationFormat="3" CompileAs="1"/>
+      <Tool Name="VCCLCompilerTool" Optimization="0" AdditionalIncludeDirectories="..\..\include;..\..\common;..\..\libcerror;..\..\libcdata;..\..\libclocale;..\..\libuna;..\..\libfguid;C:\Python27\include" PreprocessorDefinitions="_CRT_SECURE_NO_DEPRECATE;HAVE_PYCONFIG_H;HAVE_LOCAL_LIBCERROR;HAVE_LOCAL_LIBCDATA;HAVE_LOCAL_LIBCLOCALE;HAVE_LOCAL_LIBUNA;HAVE_LOCAL_LIBFGUID;LIBFWPS_DLL_IMPORT" BasicRuntimeChecks="3" SmallerTypeCheck="true" RuntimeLibrary="3" WarningLevel="4" DebugInformationFormat="3" CompileAs="1"/>
       <Tool Name="VCManagedResourceCompilerTool"/>
       <Tool Name="VCResourceCompilerTool"/>
       <Tool Name="VCPreLinkEventTool"/>
       <Tool Name="VCLinkerTool" OutputFile="$(OutDir)\$(ProjectName).pyd" AdditionalLibraryDirectories="&quot;$(OutDir)&quot;;C:\Python27\libs" GenerateDebugInformation="true" RandomizedBaseAddress="1" DataExecutionPrevention="1" TargetMachine="1" ImportLibrary="$(OutDir)\$(ProjectName).lib"/>
       <Tool Name="VCALinkTool"/>
       <Tool Name="VCManifestTool"/>
       <Tool Name="VCXDCMakeTool"/>
@@ -53,30 +53,33 @@
       <File RelativePath="..\..\pyfwps\pyfwps_guid.c"/>
       <File RelativePath="..\..\pyfwps\pyfwps_integer.c"/>
       <File RelativePath="..\..\pyfwps\pyfwps_record.c"/>
       <File RelativePath="..\..\pyfwps\pyfwps_records.c"/>
       <File RelativePath="..\..\pyfwps\pyfwps_set.c"/>
       <File RelativePath="..\..\pyfwps\pyfwps_sets.c"/>
       <File RelativePath="..\..\pyfwps\pyfwps_store.c"/>
+      <File RelativePath="..\..\pyfwps\pyfwps_string.c"/>
     </Filter>
     <Filter Name="Header Files" Filter="h;hpp;hxx;hm;inl;inc;xsd" UniqueIdentifier="{93995380-89BD-4b04-88EB-625FBE52EBFB}">
       <File RelativePath="..\..\pyfwps\pyfwps.h"/>
       <File RelativePath="..\..\pyfwps\pyfwps_codepage.h"/>
       <File RelativePath="..\..\pyfwps\pyfwps_error.h"/>
       <File RelativePath="..\..\pyfwps\pyfwps_guid.h"/>
       <File RelativePath="..\..\pyfwps\pyfwps_integer.h"/>
       <File RelativePath="..\..\pyfwps\pyfwps_libcerror.h"/>
       <File RelativePath="..\..\pyfwps\pyfwps_libclocale.h"/>
       <File RelativePath="..\..\pyfwps\pyfwps_libfguid.h"/>
       <File RelativePath="..\..\pyfwps\pyfwps_libfwps.h"/>
+      <File RelativePath="..\..\pyfwps\pyfwps_libuna.h"/>
       <File RelativePath="..\..\pyfwps\pyfwps_python.h"/>
       <File RelativePath="..\..\pyfwps\pyfwps_record.h"/>
       <File RelativePath="..\..\pyfwps\pyfwps_records.h"/>
       <File RelativePath="..\..\pyfwps\pyfwps_set.h"/>
       <File RelativePath="..\..\pyfwps\pyfwps_sets.h"/>
       <File RelativePath="..\..\pyfwps\pyfwps_store.h"/>
+      <File RelativePath="..\..\pyfwps\pyfwps_string.h"/>
       <File RelativePath="..\..\pyfwps\pyfwps_unused.h"/>
     </Filter>
     <Filter Name="Resource Files" Filter="rc;ico;cur;bmp;dlg;rc2;rct;bin;rgs;gif;jpg;jpeg;jpe;resx;tiff;tif;png;wav" UniqueIdentifier="{67DA6AB6-F800-4c08-8B7A-83BB121AAD01}"/>
   </Files>
   <Globals/>
 </VisualStudioProject>
```

### Comparing `libfwps-20230202/msvscpp/Makefile.in` & `libfwps-20230711/msvscpp/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/libcerror/libcerror.vcproj` & `libfwps-20230711/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/libfwps.sln` & `libfwps-20230711/msvscpp/libfwps.sln`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/libcnotify/libcnotify.vcproj` & `libfwps-20230711/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/fwps_test_set/fwps_test_set.vcproj` & `libfwps-20230711/msvscpp/fwps_test_set/fwps_test_set.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/msvscpp/libcdata/libcdata.vcproj` & `libfwps-20230711/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/setup.py` & `libfwps-20230711/setup.py`

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

### Comparing `libfwps-20230202/config.guess` & `libfwps-20230711/config.guess`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/ossfuzz/store_fuzzer.cc` & `libfwps-20230711/ossfuzz/store_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/ossfuzz/ossfuzz_libfwps.h` & `libfwps-20230711/ossfuzz/ossfuzz_libfwps.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/ossfuzz/Makefile.am` & `libfwps-20230711/ossfuzz/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/ossfuzz/set_fuzzer.cc` & `libfwps-20230711/ossfuzz/set_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/ossfuzz/record_fuzzer.cc` & `libfwps-20230711/ossfuzz/record_fuzzer.cc`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 int LLVMFuzzerTestOneInput(
      const uint8_t *data,
      size_t size )
 {
 	libfwps_record_t *record = NULL;
 	libfwps_set_t *set       = NULL;
 	int number_of_records    = 0;
-	int result               = 0;
 
 	if( libfwps_set_initialize(
 	     &set,
 	     NULL ) != 1 )
 	{
 		return( 0 );
 	}
```

### Comparing `libfwps-20230202/ossfuzz/Makefile.in` & `libfwps-20230711/ossfuzz/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/test-driver` & `libfwps-20230711/test-driver`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/configure` & `libfwps-20230711/configure`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfwps 20230202.
+# Generated by GNU Autoconf 2.71 for libfwps 20230711.
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
 PACKAGE_NAME='libfwps'
 PACKAGE_TARNAME='libfwps'
-PACKAGE_VERSION='20230202'
-PACKAGE_STRING='libfwps 20230202'
+PACKAGE_VERSION='20230711'
+PACKAGE_STRING='libfwps 20230711'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfwps.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1598,15 +1598,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfwps 20230202 to adapt to many kinds of systems.
+\`configure' configures libfwps 20230711 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1669,15 +1669,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfwps 20230202:";;
+     short | recursive ) echo "Configuration of libfwps 20230711:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1881,15 +1881,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfwps configure 20230202
+libfwps configure 20230711
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2602,15 +2602,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfwps $as_me 20230202, which was
+It was created by libfwps $as_me 20230711, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4091,15 +4091,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfwps'
- VERSION='20230202'
+ VERSION='20230711'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -32336,37 +32336,37 @@
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
@@ -32379,17 +32379,17 @@
 
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
@@ -33691,14 +33691,1107 @@
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
@@ -34576,14 +35669,56 @@
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
@@ -34702,14 +35837,56 @@
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
@@ -34828,386 +36005,386 @@
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
@@ -35332,14 +36509,224 @@
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
@@ -35585,14 +36972,56 @@
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
@@ -35711,15 +37140,183 @@
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
@@ -35837,14 +37434,56 @@
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
@@ -35963,386 +37602,386 @@
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
@@ -36594,14 +38233,56 @@
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
@@ -36720,14 +38401,56 @@
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
@@ -36762,15 +38485,139 @@
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
@@ -36846,510 +38693,512 @@
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
@@ -37619,14 +39468,62 @@
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
@@ -44044,15 +45941,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfwps $as_me 20230202, which was
+This file was extended by libfwps $as_me 20230711, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -44112,15 +46009,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfwps config.status 20230202
+libfwps config.status 20230711
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfwps-20230202/libuna/libuna_url_stream.c` & `libfwps-20230711/libuna/libuna_url_stream.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_symbol.h` & `libfwps-20230711/libuna/libuna_codepage_mac_symbol.h`

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

### Comparing `libfwps-20230202/libuna/libuna_support.c` & `libfwps-20230711/libuna/libuna_support.c`

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

### Comparing `libfwps-20230202/libuna/libuna_scsu.h` & `libfwps-20230711/libuna/libuna_scsu.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_5.c` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_5.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_2.c` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_2.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1253.c` & `libfwps-20230711/libuna/libuna_codepage_windows_1253.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_koi8_u.h` & `libfwps-20230711/libuna/libuna_codepage_koi8_u.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1252.c` & `libfwps-20230711/libuna/libuna_codepage_windows_1252.c`

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

### Comparing `libfwps-20230202/libuna/libuna_utf32_stream.c` & `libfwps-20230711/libuna/libuna_utf32_stream.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1257.h` & `libfwps-20230711/libuna/libuna_codepage_windows_1257.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_cyrillic.c` & `libfwps-20230711/libuna/libuna_codepage_mac_cyrillic.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_thai.c` & `libfwps-20230711/libuna/libuna_codepage_mac_thai.c`

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

### Comparing `libfwps-20230202/libuna/libuna_utf32_string.c` & `libfwps-20230711/libuna/libuna_utf32_string.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_thai.h` & `libfwps-20230711/libuna/libuna_codepage_mac_thai.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_874.c` & `libfwps-20230711/libuna/libuna_codepage_windows_874.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1251.h` & `libfwps-20230711/libuna/libuna_codepage_windows_1251.h`

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

### Comparing `libfwps-20230202/libuna/libuna_libcerror.h` & `libfwps-20230711/libuna/libuna_libcerror.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_949.c` & `libfwps-20230711/libuna/libuna_codepage_windows_949.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_6.h` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_5.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1256.h` & `libfwps-20230711/libuna/libuna_codepage_windows_1256.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_greek.h` & `libfwps-20230711/libuna/libuna_codepage_mac_greek.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_russian.h` & `libfwps-20230711/libuna/libuna_codepage_mac_russian.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_ukrainian.h` & `libfwps-20230711/libuna/libuna_codepage_mac_ukrainian.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_6.c` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_6.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_874.h` & `libfwps-20230711/libuna/libuna_codepage_windows_874.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1251.c` & `libfwps-20230711/libuna/libuna_codepage_windows_1251.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1256.c` & `libfwps-20230711/libuna/libuna_codepage_windows_1256.c`

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

### Comparing `libfwps-20230202/libuna/libuna_base16_stream.h` & `libfwps-20230711/libuna/libuna_base16_stream.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_2.h` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_2.h`

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

### Comparing `libfwps-20230202/libuna/Makefile.am` & `libfwps-20230711/libuna/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1257.c` & `libfwps-20230711/libuna/libuna_codepage_windows_1257.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1254.h` & `libfwps-20230711/libuna/libuna_codepage_windows_1252.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1255.c` & `libfwps-20230711/libuna/libuna_codepage_windows_1255.c`

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

### Comparing `libfwps-20230202/libuna/libuna_unused.h` & `libfwps-20230711/libuna/libuna_unused.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1253.h` & `libfwps-20230711/libuna/libuna_codepage_windows_1253.h`

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

### Comparing `libfwps-20230202/libuna/libuna_unicode_character.h` & `libfwps-20230711/libuna/libuna_unicode_character.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_dingbats.h` & `libfwps-20230711/libuna/libuna_codepage_mac_dingbats.h`

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

### Comparing `libfwps-20230202/libuna/libuna_scsu.c` & `libfwps-20230711/libuna/libuna_scsu.c`

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

### Comparing `libfwps-20230202/libuna/libuna_byte_stream.c` & `libfwps-20230711/libuna/libuna_byte_stream.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_celtic.h` & `libfwps-20230711/libuna/libuna_codepage_mac_celtic.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_croatian.c` & `libfwps-20230711/libuna/libuna_codepage_mac_croatian.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_3.h` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_3.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_15.h` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_15.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_roman.c` & `libfwps-20230711/libuna/libuna_codepage_mac_roman.c`

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

### Comparing `libfwps-20230202/libuna/libuna_utf32_string.h` & `libfwps-20230711/libuna/libuna_utf32_string.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_koi8_r.c` & `libfwps-20230711/libuna/libuna_codepage_koi8_r.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_icelandic.c` & `libfwps-20230711/libuna/libuna_codepage_mac_icelandic.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_936.h` & `libfwps-20230711/libuna/libuna_codepage_windows_936.h`

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

### Comparing `libfwps-20230202/libuna/libuna_base64_stream.h` & `libfwps-20230711/libuna/libuna_base64_stream.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_celtic.c` & `libfwps-20230711/libuna/libuna_codepage_mac_celtic.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_950.c` & `libfwps-20230711/libuna/libuna_codepage_windows_950.c`

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

### Comparing `libfwps-20230202/libuna/libuna_utf8_string.h` & `libfwps-20230711/libuna/libuna_utf8_string.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_936.c` & `libfwps-20230711/libuna/libuna_codepage_windows_936.c`

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

### Comparing `libfwps-20230202/libuna/libuna_unicode_character.c` & `libfwps-20230711/libuna/libuna_unicode_character.c`

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

### Comparing `libfwps-20230202/libuna/libuna_utf8_string.c` & `libfwps-20230711/libuna/libuna_utf8_string.c`

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

### Comparing `libfwps-20230202/libuna/libuna_base32_stream.c` & `libfwps-20230711/libuna/libuna_base32_stream.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_950.h` & `libfwps-20230711/libuna/libuna_codepage_windows_950.h`

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

### Comparing `libfwps-20230202/libuna/libuna_error.h` & `libfwps-20230711/libuna/libuna_error.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_932.h` & `libfwps-20230711/libuna/libuna_codepage_windows_932.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_turkish.h` & `libfwps-20230711/libuna/libuna_codepage_mac_turkish.h`

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

### Comparing `libfwps-20230202/libuna/libuna_utf8_stream.c` & `libfwps-20230711/libuna/libuna_utf8_stream.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_ukrainian.c` & `libfwps-20230711/libuna/libuna_codepage_mac_ukrainian.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_koi8_r.h` & `libfwps-20230711/libuna/libuna_codepage_koi8_r.h`

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

### Comparing `libfwps-20230202/libuna/libuna_base16_stream.c` & `libfwps-20230711/libuna/libuna_base16_stream.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1250.h` & `libfwps-20230711/libuna/libuna_codepage_windows_1250.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_16.h` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_16.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_croatian.h` & `libfwps-20230711/libuna/libuna_codepage_mac_croatian.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_gaelic.c` & `libfwps-20230711/libuna/libuna_codepage_mac_gaelic.c`

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

### Comparing `libfwps-20230202/libuna/libuna_utf16_stream.h` & `libfwps-20230711/libuna/libuna_utf16_stream.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_10.h` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_7.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_centraleurroman.c` & `libfwps-20230711/libuna/libuna_codepage_mac_centraleurroman.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_932.c` & `libfwps-20230711/libuna/libuna_codepage_windows_932.c`

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

### Comparing `libfwps-20230202/libuna/libuna_utf8_stream.h` & `libfwps-20230711/libuna/libuna_utf8_stream.h`

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

### Comparing `libfwps-20230202/libuna/libuna_url_stream.h` & `libfwps-20230711/libuna/libuna_url_stream.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_farsi.c` & `libfwps-20230711/libuna/libuna_codepage_mac_farsi.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_949.h` & `libfwps-20230711/libuna/libuna_codepage_windows_949.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_romanian.h` & `libfwps-20230711/libuna/libuna_codepage_mac_roman.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacRomanian codepage functions
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
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H )
-#define _LIBUNA_CODEPAGE_MAC_ROMANIAN_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_ROMAN_H )
+#define _LIBUNA_CODEPAGE_MAC_ROMAN_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_romanian_copy_from_byte_stream(
+int libuna_codepage_mac_roman_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_romanian_copy_to_byte_stream(
+int libuna_codepage_mac_roman_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMAN_H ) */
```

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_gaelic.h` & `libfwps-20230711/libuna/libuna_codepage_mac_gaelic.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_8.c` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_8.c`

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

### Comparing `libfwps-20230202/libuna/libuna_types.h` & `libfwps-20230711/libuna/libuna_types.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_arabic.c` & `libfwps-20230711/libuna/libuna_codepage_mac_arabic.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1252.h` & `libfwps-20230711/libuna/libuna_codepage_windows_1258.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1250.c` & `libfwps-20230711/libuna/libuna_codepage_windows_1250.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_russian.c` & `libfwps-20230711/libuna/libuna_codepage_mac_russian.c`

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

### Comparing `libfwps-20230202/libuna/libuna_utf16_string.c` & `libfwps-20230711/libuna/libuna_utf16_string.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_5.h` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_9.h`

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

### Comparing `libfwps-20230202/libuna/libuna_extern.h` & `libfwps-20230711/libuna/libuna_extern.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_4.h` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_4.h`

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

### Comparing `libfwps-20230202/libuna/libuna_byte_stream.h` & `libfwps-20230711/libuna/libuna_byte_stream.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_roman.h` & `libfwps-20230711/libuna/libuna_codepage_mac_romanian.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacRoman codepage functions
+ * MacRomanian codepage functions
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
+#if !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H )
+#define _LIBUNA_CODEPAGE_MAC_ROMANIAN_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_roman_copy_from_byte_stream(
+int libuna_codepage_mac_romanian_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_roman_copy_to_byte_stream(
+int libuna_codepage_mac_romanian_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMAN_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H ) */
```

### Comparing `libfwps-20230202/libuna/libuna_utf16_string.h` & `libfwps-20230711/libuna/libuna_utf16_string.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_4.c` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_4.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_10.c` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_10.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_icelandic.h` & `libfwps-20230711/libuna/libuna_codepage_mac_icelandic.h`

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

### Comparing `libfwps-20230202/libuna/Makefile.in` & `libfwps-20230711/libuna/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libuna/libuna_utf7_stream.h` & `libfwps-20230711/libuna/libuna_utf7_stream.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_symbol.c` & `libfwps-20230711/libuna/libuna_codepage_mac_symbol.c`

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

### Comparing `libfwps-20230202/libuna/libuna_base32_stream.h` & `libfwps-20230711/libuna/libuna_base32_stream.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_turkish.c` & `libfwps-20230711/libuna/libuna_codepage_mac_turkish.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_inuit.c` & `libfwps-20230711/libuna/libuna_codepage_mac_inuit.c`

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

### Comparing `libfwps-20230202/libuna/libuna_utf16_stream.c` & `libfwps-20230711/libuna/libuna_utf16_stream.c`

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

### Comparing `libfwps-20230202/libuna/libuna_utf7_stream.c` & `libfwps-20230711/libuna/libuna_utf7_stream.c`

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

### Comparing `libfwps-20230202/libuna/libuna_support.h` & `libfwps-20230711/libuna/libuna_support.h`

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

### Comparing `libfwps-20230202/libuna/libuna_utf32_stream.h` & `libfwps-20230711/libuna/libuna_utf32_stream.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_3.c` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_3.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_greek.c` & `libfwps-20230711/libuna/libuna_codepage_mac_greek.c`

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

### Comparing `libfwps-20230202/libuna/libuna_definitions.h` & `libfwps-20230711/libuna/libuna_definitions.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1255.h` & `libfwps-20230711/libuna/libuna_codepage_windows_1255.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_14.c` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_14.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_13.c` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_13.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_centraleurroman.h` & `libfwps-20230711/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files 4% similar despite different names*

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_8.h` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_8.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_9.c` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_9.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1254.c` & `libfwps-20230711/libuna/libuna_codepage_windows_1254.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_cyrillic.h` & `libfwps-20230711/libuna/libuna_codepage_mac_cyrillic.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_arabic.h` & `libfwps-20230711/libuna/libuna_codepage_mac_arabic.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1258.c` & `libfwps-20230711/libuna/libuna_codepage_windows_1258.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_farsi.h` & `libfwps-20230711/libuna/libuna_codepage_mac_farsi.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_15.c` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_15.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_7.c` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_7.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_dingbats.c` & `libfwps-20230711/libuna/libuna_codepage_mac_dingbats.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_9.h` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_6.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_windows_1258.h` & `libfwps-20230711/libuna/libuna_codepage_windows_1254.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1258 codepage (Vietnamese) functions
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
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1258_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1258_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1254_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1254_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1258_copy_from_byte_stream(
+int libuna_codepage_windows_1254_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1258_copy_to_byte_stream(
+int libuna_codepage_windows_1254_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1258_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1254_H ) */
```

### Comparing `libfwps-20230202/libuna/libuna_base64_stream.c` & `libfwps-20230711/libuna/libuna_base64_stream.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_romanian.c` & `libfwps-20230711/libuna/libuna_codepage_mac_romanian.c`

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

### Comparing `libfwps-20230202/libuna/libuna_error.c` & `libfwps-20230711/libuna/libuna_error.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_koi8_u.c` & `libfwps-20230711/libuna/libuna_codepage_koi8_u.c`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_13.h` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_10.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_7.h` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_14.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_14.h` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_13.h`

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_mac_inuit.h` & `libfwps-20230711/libuna/libuna_codepage_mac_inuit.h`

 * *Files 0% similar despite different names*

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

### Comparing `libfwps-20230202/libuna/libuna_codepage_iso_8859_16.c` & `libfwps-20230711/libuna/libuna_codepage_iso_8859_16.c`

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

### Comparing `libfwps-20230202/pyfwps/pyfwps_libcerror.h` & `libfwps-20230711/pyfwps/pyfwps_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_unused.h` & `libfwps-20230711/pyfwps/pyfwps_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_integer.h` & `libfwps-20230711/pyfwps/pyfwps_integer.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/Makefile.am` & `libfwps-20230711/pyfwps/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,22 @@
 	pyfwps_error.c pyfwps_error.h \
 	pyfwps_guid.c pyfwps_guid.h \
 	pyfwps_integer.c pyfwps_integer.h \
 	pyfwps_libcerror.h \
 	pyfwps_libclocale.h \
 	pyfwps_libfguid.h \
 	pyfwps_libfwps.h \
+	pyfwps_libuna.h \
 	pyfwps_python.h \
 	pyfwps_record.c pyfwps_record.h \
 	pyfwps_records.c pyfwps_records.h \
 	pyfwps_set.c pyfwps_set.h \
 	pyfwps_sets.c pyfwps_sets.h \
 	pyfwps_store.c pyfwps_store.h \
+	pyfwps_string.c pyfwps_string.h \
 	pyfwps_unused.h
 
 pyfwps_la_LIBADD = \
 	@LIBCERROR_LIBADD@ \
 	../libfwps/libfwps.la \
 	@LIBCDATA_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
```

### Comparing `libfwps-20230202/pyfwps/pyfwps_libclocale.h` & `libfwps-20230711/pyfwps/pyfwps_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_records.c` & `libfwps-20230711/pyfwps/pyfwps_records.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_sets.h` & `libfwps-20230711/pyfwps/pyfwps_sets.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_record.h` & `libfwps-20230711/pyfwps/pyfwps_record.h`

 * *Files 10% similar despite different names*

```diff
@@ -82,14 +82,18 @@
            pyfwps_record_t *pyfwps_record,
            PyObject *arguments );
 
 PyObject *pyfwps_record_get_data_as_string(
            pyfwps_record_t *pyfwps_record,
            PyObject *arguments );
 
+PyObject *pyfwps_record_get_data_as_path_string(
+           pyfwps_record_t *pyfwps_record,
+           PyObject *arguments );
+
 PyObject *pyfwps_record_get_data_as_guid(
            pyfwps_record_t *pyfwps_record,
            PyObject *arguments );
 
 #if defined( __cplusplus )
 }
 #endif
```

### Comparing `libfwps-20230202/pyfwps/pyfwps_store.h` & `libfwps-20230711/pyfwps/pyfwps_store.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_store.c` & `libfwps-20230711/pyfwps/pyfwps_store.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_set.h` & `libfwps-20230711/pyfwps/pyfwps_set.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_records.h` & `libfwps-20230711/pyfwps/pyfwps_records.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_codepage.c` & `libfwps-20230711/pyfwps/pyfwps_codepage.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps.c` & `libfwps-20230711/pyfwps/pyfwps.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps.h` & `libfwps-20230711/pyfwps/pyfwps.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_python.h` & `libfwps-20230711/pyfwps/pyfwps_python.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_set.c` & `libfwps-20230711/pyfwps/pyfwps_set.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_integer.c` & `libfwps-20230711/pyfwps/pyfwps_integer.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_sets.c` & `libfwps-20230711/pyfwps/pyfwps_sets.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/Makefile.in` & `libfwps-20230711/pyfwps/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -143,28 +143,30 @@
 am__installdirs = "$(DESTDIR)$(pyexecdir)"
 LTLIBRARIES = $(pyexec_LTLIBRARIES)
 @HAVE_PYTHON_TRUE@pyfwps_la_DEPENDENCIES = ../libfwps/libfwps.la
 am__pyfwps_la_SOURCES_DIST = pyfwps.c pyfwps.h pyfwps_codepage.c \
 	pyfwps_codepage.h pyfwps_error.c pyfwps_error.h pyfwps_guid.c \
 	pyfwps_guid.h pyfwps_integer.c pyfwps_integer.h \
 	pyfwps_libcerror.h pyfwps_libclocale.h pyfwps_libfguid.h \
-	pyfwps_libfwps.h pyfwps_python.h pyfwps_record.c \
-	pyfwps_record.h pyfwps_records.c pyfwps_records.h pyfwps_set.c \
-	pyfwps_set.h pyfwps_sets.c pyfwps_sets.h pyfwps_store.c \
-	pyfwps_store.h pyfwps_unused.h
+	pyfwps_libfwps.h pyfwps_libuna.h pyfwps_python.h \
+	pyfwps_record.c pyfwps_record.h pyfwps_records.c \
+	pyfwps_records.h pyfwps_set.c pyfwps_set.h pyfwps_sets.c \
+	pyfwps_sets.h pyfwps_store.c pyfwps_store.h pyfwps_string.c \
+	pyfwps_string.h pyfwps_unused.h
 @HAVE_PYTHON_TRUE@am_pyfwps_la_OBJECTS = pyfwps_la-pyfwps.lo \
 @HAVE_PYTHON_TRUE@	pyfwps_la-pyfwps_codepage.lo \
 @HAVE_PYTHON_TRUE@	pyfwps_la-pyfwps_error.lo \
 @HAVE_PYTHON_TRUE@	pyfwps_la-pyfwps_guid.lo \
 @HAVE_PYTHON_TRUE@	pyfwps_la-pyfwps_integer.lo \
 @HAVE_PYTHON_TRUE@	pyfwps_la-pyfwps_record.lo \
 @HAVE_PYTHON_TRUE@	pyfwps_la-pyfwps_records.lo \
 @HAVE_PYTHON_TRUE@	pyfwps_la-pyfwps_set.lo \
 @HAVE_PYTHON_TRUE@	pyfwps_la-pyfwps_sets.lo \
-@HAVE_PYTHON_TRUE@	pyfwps_la-pyfwps_store.lo
+@HAVE_PYTHON_TRUE@	pyfwps_la-pyfwps_store.lo \
+@HAVE_PYTHON_TRUE@	pyfwps_la-pyfwps_string.lo
 pyfwps_la_OBJECTS = $(am_pyfwps_la_OBJECTS)
 AM_V_lt = $(am__v_lt_@AM_V@)
 am__v_lt_ = $(am__v_lt_@AM_DEFAULT_V@)
 am__v_lt_0 = --silent
 am__v_lt_1 = 
 pyfwps_la_LINK = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=link $(CCLD) $(AM_CFLAGS) $(CFLAGS) \
@@ -190,15 +192,16 @@
 	./$(DEPDIR)/pyfwps_la-pyfwps_error.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_guid.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_integer.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_record.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_records.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_set.Plo \
 	./$(DEPDIR)/pyfwps_la-pyfwps_sets.Plo \
-	./$(DEPDIR)/pyfwps_la-pyfwps_store.Plo
+	./$(DEPDIR)/pyfwps_la-pyfwps_store.Plo \
+	./$(DEPDIR)/pyfwps_la-pyfwps_string.Plo
 am__mv = mv -f
 COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
 	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
 LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) \
 	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
 	$(AM_CFLAGS) $(CFLAGS)
@@ -543,20 +546,22 @@
 @HAVE_PYTHON_TRUE@	pyfwps_error.c pyfwps_error.h \
 @HAVE_PYTHON_TRUE@	pyfwps_guid.c pyfwps_guid.h \
 @HAVE_PYTHON_TRUE@	pyfwps_integer.c pyfwps_integer.h \
 @HAVE_PYTHON_TRUE@	pyfwps_libcerror.h \
 @HAVE_PYTHON_TRUE@	pyfwps_libclocale.h \
 @HAVE_PYTHON_TRUE@	pyfwps_libfguid.h \
 @HAVE_PYTHON_TRUE@	pyfwps_libfwps.h \
+@HAVE_PYTHON_TRUE@	pyfwps_libuna.h \
 @HAVE_PYTHON_TRUE@	pyfwps_python.h \
 @HAVE_PYTHON_TRUE@	pyfwps_record.c pyfwps_record.h \
 @HAVE_PYTHON_TRUE@	pyfwps_records.c pyfwps_records.h \
 @HAVE_PYTHON_TRUE@	pyfwps_set.c pyfwps_set.h \
 @HAVE_PYTHON_TRUE@	pyfwps_sets.c pyfwps_sets.h \
 @HAVE_PYTHON_TRUE@	pyfwps_store.c pyfwps_store.h \
+@HAVE_PYTHON_TRUE@	pyfwps_string.c pyfwps_string.h \
 @HAVE_PYTHON_TRUE@	pyfwps_unused.h
 
 @HAVE_PYTHON_TRUE@pyfwps_la_LIBADD = \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_PYTHON_TRUE@	../libfwps/libfwps.la \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_LIBADD@ \
@@ -652,14 +657,15 @@
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_guid.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_integer.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_record.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_records.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_set.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_sets.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_store.Plo@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pyfwps_la-pyfwps_string.Plo@am__quote@ # am--include-marker
 
 $(am__depfiles_remade):
 	@$(MKDIR_P) $(@D)
 	@echo '# dummy' >$@-t && $(am__mv) $@-t $@
 
 am--depfiles: $(am__depfiles_remade)
 
@@ -750,14 +756,21 @@
 pyfwps_la-pyfwps_store.lo: pyfwps_store.c
 @am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwps_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pyfwps_la-pyfwps_store.lo -MD -MP -MF $(DEPDIR)/pyfwps_la-pyfwps_store.Tpo -c -o pyfwps_la-pyfwps_store.lo `test -f 'pyfwps_store.c' || echo '$(srcdir)/'`pyfwps_store.c
 @am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pyfwps_la-pyfwps_store.Tpo $(DEPDIR)/pyfwps_la-pyfwps_store.Plo
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pyfwps_store.c' object='pyfwps_la-pyfwps_store.lo' libtool=yes @AMDEPBACKSLASH@
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
 @am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwps_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pyfwps_la-pyfwps_store.lo `test -f 'pyfwps_store.c' || echo '$(srcdir)/'`pyfwps_store.c
 
+pyfwps_la-pyfwps_string.lo: pyfwps_string.c
+@am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwps_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pyfwps_la-pyfwps_string.lo -MD -MP -MF $(DEPDIR)/pyfwps_la-pyfwps_string.Tpo -c -o pyfwps_la-pyfwps_string.lo `test -f 'pyfwps_string.c' || echo '$(srcdir)/'`pyfwps_string.c
+@am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pyfwps_la-pyfwps_string.Tpo $(DEPDIR)/pyfwps_la-pyfwps_string.Plo
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pyfwps_string.c' object='pyfwps_la-pyfwps_string.lo' libtool=yes @AMDEPBACKSLASH@
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
+@am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pyfwps_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pyfwps_la-pyfwps_string.lo `test -f 'pyfwps_string.c' || echo '$(srcdir)/'`pyfwps_string.c
+
 mostlyclean-libtool:
 	-rm -f *.lo
 
 clean-libtool:
 	-rm -rf .libs _libs
 
 ID: $(am__tagged_files)
@@ -937,14 +950,15 @@
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_guid.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_integer.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_record.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_records.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_set.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_sets.Plo
 	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_store.Plo
+	-rm -f ./$(DEPDIR)/pyfwps_la-pyfwps_string.Plo
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
 
 mostlyclean: mostlyclean-am
 
 mostlyclean-am: mostlyclean-compile mostlyclean-generic \
 	mostlyclean-libtool
```

### Comparing `libfwps-20230202/pyfwps/pyfwps_libfwps.h` & `libfwps-20230711/pyfwps/pyfwps_libfwps.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_error.c` & `libfwps-20230711/pyfwps/pyfwps_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_record.c` & `libfwps-20230711/pyfwps/pyfwps_record.c`

 * *Files 18% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 #include "pyfwps_error.h"
 #include "pyfwps_guid.h"
 #include "pyfwps_integer.h"
 #include "pyfwps_libcerror.h"
 #include "pyfwps_libfwps.h"
 #include "pyfwps_python.h"
 #include "pyfwps_record.h"
+#include "pyfwps_string.h"
 #include "pyfwps_unused.h"
 
 PyMethodDef pyfwps_record_object_methods[] = {
 
 	{ "get_entry_type",
 	  (PyCFunction) pyfwps_record_get_entry_type,
 	  METH_NOARGS,
@@ -75,14 +76,21 @@
 	{ "get_data_as_string",
 	  (PyCFunction) pyfwps_record_get_data_as_string,
 	  METH_NOARGS,
 	  "get_data_as_string() -> Unicode string\n"
 	  "\n"
 	  "Retrieves the data as a string." },
 
+	{ "get_data_as_path_string",
+	  (PyCFunction) pyfwps_record_get_data_as_path_string,
+	  METH_NOARGS,
+	  "get_data_as_path_string() -> Unicode string\n"
+	  "\n"
+	  "Retrieves the data as a path string." },
+
 	{ "get_data_as_guid",
 	  (PyCFunction) pyfwps_record_get_data_as_guid,
 	  METH_NOARGS,
 	  "get_data_as_guid() -> Unicode string\n"
 	  "\n"
 	  "Retrieves the data as a GUID value." },
 
@@ -124,14 +132,20 @@
 
 	{ "data_as_string",
 	  (getter) pyfwps_record_get_data_as_string,
 	  (setter) 0,
 	  "The data as a string.",
 	  NULL },
 
+	{ "data_as_path_string",
+	  (getter) pyfwps_record_get_data_as_path_string,
+	  (setter) 0,
+	  "The data as a path string.",
+	  NULL },
+
 	{ "data_as_guid",
 	  (getter) pyfwps_record_get_data_as_guid,
 	  (setter) 0,
 	  "The data as a GUID value.",
 	  NULL },
 
 	/* Sentinel */
@@ -899,22 +913,151 @@
 		 function );
 
 		libcerror_error_free(
 		 &error );
 
 		goto on_error;
 	}
-	/* Pass the string length to PyUnicode_DecodeUTF8 otherwise it makes
-	 * the end of string character is part of the string.
+	/* Pass the string length to PyUnicode_DecodeUTF8
+	 * otherwise it makes the end of string character is part
+	 * of the string
 	 */
 	string_object = PyUnicode_DecodeUTF8(
 	                 utf8_string,
 	                 (Py_ssize_t) utf8_string_size - 1,
-	                 errors );
+	                 NULL );
+
+	if( string_object == NULL )
+	{
+		PyErr_Format(
+		 PyExc_IOError,
+		 "%s: unable to convert UTF-8 string into Unicode object.",
+		 function );
+
+		goto on_error;
+	}
+	PyMem_Free(
+	 utf8_string );
+
+	return( string_object );
+
+on_error:
+	if( utf8_string != NULL )
+	{
+		PyMem_Free(
+		 utf8_string );
+	}
+	return( NULL );
+}
+
+/* Retrieves the data as a path string
+ * Returns a Python object if successful or NULL on error
+ */
+PyObject *pyfwps_record_get_data_as_path_string(
+           pyfwps_record_t *pyfwps_record,
+           PyObject *arguments PYFWPS_ATTRIBUTE_UNUSED )
+{
+	PyObject *string_object  = NULL;
+	libcerror_error_t *error = NULL;
+	const char *errors       = NULL;
+	static char *function    = "pyfwps_value_get_data_as_path_string";
+	char *utf8_string        = NULL;
+	size_t utf8_string_size  = 0;
+	int result               = 0;
+
+	PYFWPS_UNREFERENCED_PARAMETER( arguments )
+
+	if( pyfwps_record == NULL )
+	{
+		PyErr_Format(
+		 PyExc_ValueError,
+		 "%s: invalid record.",
+		 function );
 
+		return( NULL );
+	}
+	Py_BEGIN_ALLOW_THREADS
+
+	result = libfwps_record_get_data_as_utf8_path_string_size(
+	          pyfwps_record->record,
+	          &utf8_string_size,
+	          &error );
+
+	Py_END_ALLOW_THREADS
+
+	if( result == -1 )
+	{
+		pyfwps_error_raise(
+		 error,
+		 PyExc_IOError,
+		 "%s: unable to determine size of data as UTF-8 string.",
+		 function );
+
+		libcerror_error_free(
+		 &error );
+
+		goto on_error;
+	}
+	else if( ( result == 0 )
+	      || ( utf8_string_size == 0 ) )
+	{
+		Py_IncRef(
+		 Py_None );
+
+		return( Py_None );
+	}
+	utf8_string = (char *) PyMem_Malloc(
+	                        sizeof( char ) * utf8_string_size );
+
+	if( utf8_string == NULL )
+	{
+		PyErr_Format(
+		 PyExc_MemoryError,
+		 "%s: unable to create UTF-8 string.",
+		 function );
+
+		goto on_error;
+	}
+	Py_BEGIN_ALLOW_THREADS
+
+	result = libfwps_record_get_data_as_utf8_path_string(
+	          pyfwps_record->record,
+	          (uint8_t *) utf8_string,
+	          utf8_string_size,
+	          &error );
+
+	Py_END_ALLOW_THREADS
+
+	if( result != 1 )
+	{
+		pyfwps_error_raise(
+		 error,
+		 PyExc_IOError,
+		 "%s: unable to retrieve data as UTF-8 string.",
+		 function );
+
+		libcerror_error_free(
+		 &error );
+
+		goto on_error;
+	}
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
+	string_object = pyfwps_string_new_from_utf8_rfc2279(
+			 (uint8_t *) utf8_string,
+			 utf8_string_size );
+#else
+	/* Pass the string length to PyUnicode_DecodeUTF8
+	 * otherwise it makes the end of string character is part
+	 * of the string
+	 */
+	string_object = PyUnicode_DecodeUTF8(
+	                 utf8_string,
+	                 (Py_ssize_t) utf8_string_size - 1,
+	                 NULL );
+#endif
 	if( string_object == NULL )
 	{
 		PyErr_Format(
 		 PyExc_IOError,
 		 "%s: unable to convert UTF-8 string into Unicode object.",
 		 function );
```

### Comparing `libfwps-20230202/pyfwps/pyfwps_guid.h` & `libfwps-20230711/pyfwps/pyfwps_guid.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_codepage.h` & `libfwps-20230711/pyfwps/pyfwps_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_libfguid.h` & `libfwps-20230711/pyfwps/pyfwps_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_guid.c` & `libfwps-20230711/pyfwps/pyfwps_guid.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/pyfwps/pyfwps_error.h` & `libfwps-20230711/pyfwps/pyfwps_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/Makefile.in` & `libfwps-20230711/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/libuna.m4` & `libfwps-20230711/m4/libuna.m4`

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

### Comparing `libfwps-20230202/m4/gettext.m4` & `libfwps-20230711/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/tests.m4` & `libfwps-20230711/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/lib-prefix.m4` & `libfwps-20230711/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/ltoptions.m4` & `libfwps-20230711/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/lib-ld.m4` & `libfwps-20230711/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/libcthreads.m4` & `libfwps-20230711/m4/libcthreads.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/lib-link.m4` & `libfwps-20230711/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/python.m4` & `libfwps-20230711/m4/python.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/libtool.m4` & `libfwps-20230711/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/nls.m4` & `libfwps-20230711/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/libclocale.m4` & `libfwps-20230711/m4/libclocale.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/libfdatetime.m4` & `libfwps-20230711/m4/libfdatetime.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/host-cpu-c-abi.m4` & `libfwps-20230711/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/libcnotify.m4` & `libfwps-20230711/m4/libcnotify.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/ltversion.m4` & `libfwps-20230711/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/libcdata.m4` & `libfwps-20230711/m4/libcdata.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/progtest.m4` & `libfwps-20230711/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/lt~obsolete.m4` & `libfwps-20230711/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/po.m4` & `libfwps-20230711/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/pthread.m4` & `libfwps-20230711/m4/pthread.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/common.m4` & `libfwps-20230711/m4/common.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/libcerror.m4` & `libfwps-20230711/m4/libcerror.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/libfguid.m4` & `libfwps-20230711/m4/libfguid.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/iconv.m4` & `libfwps-20230711/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/ltsugar.m4` & `libfwps-20230711/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/libfole.m4` & `libfwps-20230711/m4/libfole.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/intlmacosx.m4` & `libfwps-20230711/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/m4/types.m4` & `libfwps-20230711/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/COPYING.LESSER` & `libfwps-20230711/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libfwps.spec.in` & `libfwps-20230711/libfwps.spec.in`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Name: libfwps
 Version: @VERSION@
 Release: 1
 Summary: Library to access the Windows Property Store format
 Group: System Environment/Libraries
-License: LGPLv3+
+License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfwps
-BuildRoot: %{_tmppath}/%{name}-%{version}-%{release}-root-%(%{__id_u} -n)
 @libfwps_spec_requires@ @ax_libcdata_spec_requires@ @ax_libcerror_spec_requires@ @ax_libclocale_spec_requires@ @ax_libcnotify_spec_requires@ @ax_libcthreads_spec_requires@ @ax_libfdatetime_spec_requires@ @ax_libfguid_spec_requires@ @ax_libfole_spec_requires@ @ax_libuna_spec_requires@
 BuildRequires: gcc @ax_libcdata_spec_build_requires@ @ax_libcerror_spec_build_requires@ @ax_libclocale_spec_build_requires@ @ax_libcnotify_spec_build_requires@ @ax_libcthreads_spec_build_requires@ @ax_libfdatetime_spec_build_requires@ @ax_libfguid_spec_build_requires@ @ax_libfole_spec_build_requires@ @ax_libuna_spec_build_requires@
 
 %description -n libfwps
 Library to access the Windows Property Store format
 
 %package -n libfwps-static
@@ -53,36 +52,32 @@
 rm -rf %{buildroot}
 
 %post -p /sbin/ldconfig
 
 %postun -p /sbin/ldconfig
 
 %files -n libfwps
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
-%attr(755,root,root) %{_libdir}/*.so.*
+%{_libdir}/*.so.*
 
 %files -n libfwps-static
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
-%attr(755,root,root) %{_libdir}/*.a
+%{_libdir}/*.a
 
 %files -n libfwps-devel
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/*.so
 %{_libdir}/pkgconfig/libfwps.pc
 %{_includedir}/*
 %{_mandir}/man3/*
 
 %files -n libfwps-python3
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %changelog
 * @SPEC_DATE@ Joachim Metz <joachim.metz@gmail.com> @VERSION@-1
```

### Comparing `libfwps-20230202/libcerror/libcerror_system.c` & `libfwps-20230711/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcerror/libcerror_error.c` & `libfwps-20230711/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcerror/libcerror_extern.h` & `libfwps-20230711/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcerror/Makefile.am` & `libfwps-20230711/libcerror/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcerror/libcerror_error.h` & `libfwps-20230711/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcerror/libcerror_support.h` & `libfwps-20230711/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcerror/libcerror_types.h` & `libfwps-20230711/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcerror/libcerror_definitions.h` & `libfwps-20230711/libcerror/libcerror_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcerror/libcerror_unused.h` & `libfwps-20230711/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcerror/Makefile.in` & `libfwps-20230711/libcerror/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcerror/libcerror_support.c` & `libfwps-20230711/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcerror/libcerror_system.h` & `libfwps-20230711/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcnotify/libcnotify_libcerror.h` & `libfwps-20230711/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcnotify/libcnotify_unused.h` & `libfwps-20230711/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcnotify/libcnotify_support.h` & `libfwps-20230711/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcnotify/libcnotify_support.c` & `libfwps-20230711/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcnotify/Makefile.am` & `libfwps-20230711/libcnotify/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcnotify/libcnotify_print.c` & `libfwps-20230711/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcnotify/libcnotify_verbose.c` & `libfwps-20230711/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcnotify/libcnotify_stream.h` & `libfwps-20230711/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcnotify/libcnotify_extern.h` & `libfwps-20230711/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcnotify/libcnotify_stream.c` & `libfwps-20230711/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcnotify/Makefile.in` & `libfwps-20230711/libcnotify/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcnotify/libcnotify_print.h` & `libfwps-20230711/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcnotify/libcnotify_verbose.h` & `libfwps-20230711/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcnotify/libcnotify_definitions.h` & `libfwps-20230711/libcnotify/libcnotify_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/ltmain.sh` & `libfwps-20230711/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/compile` & `libfwps-20230711/compile`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/config.rpath` & `libfwps-20230711/config.rpath`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/depcomp` & `libfwps-20230711/depcomp`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/po/en@quot.header` & `libfwps-20230711/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/po/Rules-quot` & `libfwps-20230711/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/po/remove-potcdate.sin` & `libfwps-20230711/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/po/Makevars.in` & `libfwps-20230711/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/po/en@boldquot.header` & `libfwps-20230711/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/po/Makevars` & `libfwps-20230711/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/po/insert-header.sin` & `libfwps-20230711/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/po/Makefile.in.in` & `libfwps-20230711/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_array.c` & `libfwps-20230711/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_btree_node.c` & `libfwps-20230711/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_tree_node.c` & `libfwps-20230711/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_libcthreads.h` & `libfwps-20230711/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_range_list_value.h` & `libfwps-20230711/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_unused.h` & `libfwps-20230711/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_range_list.h` & `libfwps-20230711/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/Makefile.am` & `libfwps-20230711/libcdata/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_range_list.c` & `libfwps-20230711/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_extern.h` & `libfwps-20230711/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_support.c` & `libfwps-20230711/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_list_element.h` & `libfwps-20230711/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_btree_values_list.c` & `libfwps-20230711/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_range_list_value.c` & `libfwps-20230711/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_libcerror.h` & `libfwps-20230711/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_error.c` & `libfwps-20230711/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_error.h` & `libfwps-20230711/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_support.h` & `libfwps-20230711/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_btree_node.h` & `libfwps-20230711/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_list.c` & `libfwps-20230711/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_tree_node.h` & `libfwps-20230711/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_list.h` & `libfwps-20230711/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_types.h` & `libfwps-20230711/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_list_element.c` & `libfwps-20230711/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/Makefile.in` & `libfwps-20230711/libcdata/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_btree_values_list.h` & `libfwps-20230711/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_array.h` & `libfwps-20230711/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_btree.h` & `libfwps-20230711/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_definitions.h` & `libfwps-20230711/libcdata/libcdata_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/libcdata/libcdata_btree.c` & `libfwps-20230711/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libfwps-20230202/acinclude.m4` & `libfwps-20230711/acinclude.m4`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20230130
 
 dnl Function to detect if libfwps dependencies are available
 AC_DEFUN([AX_LIBFWPS_CHECK_LOCAL],
   [dnl No additional checks.
   ])
 
 dnl Function to check if DLL support is needed
```

### Comparing `libfwps-20230202/configure.ac` & `libfwps-20230711/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfwps],
- [20230202],
+ [20230711],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfwps.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
```

