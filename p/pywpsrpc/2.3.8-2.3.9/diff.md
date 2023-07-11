# Comparing `tmp/pywpsrpc-2.3.8.tar.gz` & `tmp/pywpsrpc-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywpsrpc-2.3.8.tar", last modified: Mon Jul  3 13:10:23 2023, max compression
+gzip compressed data, was "pywpsrpc-2.3.9.tar", last modified: Tue Jul 11 14:16:08 2023, max compression
```

## Comparing `pywpsrpc-2.3.8.tar` & `pywpsrpc-2.3.9.tar`

### file list

```diff
@@ -1,1359 +1,1354 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.642567 pywpsrpc-2.3.8/
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     4916 2023-07-03 13:10:23.642567 pywpsrpc-2.3.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.438561 pywpsrpc-2.3.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.438561 pywpsrpc-2.3.8/examples/rpcwpsapi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.438561 pywpsrpc-2.3.8/examples/rpcwpsapi/convertto/
--rwxr-xr-x   0 runner    (1001) docker     (122)     3121 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/examples/rpcwpsapi/convertto/convertto.py
--rw-r--r--   0 runner    (1001) docker     (122)      228 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/examples/rpcwpsapi/convertto/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.438561 pywpsrpc-2.3.8/examples/rpcwpsapi/embedded/
--rwxr-xr-x   0 runner    (1001) docker     (122)     6416 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/examples/rpcwpsapi/embedded/demo.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/examples/rpcwpsapi/embedded/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.438561 pywpsrpc-2.3.8/examples/rpcwppapi/
--rwxr-xr-x   0 runner    (1001) docker     (122)     3399 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/examples/rpcwppapi/wpp_convert.py
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/examples/rpcwppapi/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.438561 pywpsrpc-2.3.8/examples/rpcetapi/
--rwxr-xr-x   0 runner    (1001) docker     (122)     3287 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/examples/rpcetapi/et_convert.py
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/examples/rpcetapi/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     4247 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/README_en.md
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.438561 pywpsrpc-2.3.8/include/
--rw-r--r--   0 runner    (1001) docker     (122)     3962 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/include/pyevents.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.442561 pywpsrpc-2.3.8/tests/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1077 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/tests/test_rpcproxy.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     8099 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/tests/test_rpcetapi.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2266 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/tests/test_iter.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2024 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/tests/test_rpcwppapi.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10012 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/tests/test_rpcevents.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1747 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/tests/test_property.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10448 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/tests/test_rpcwpsapi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.442561 pywpsrpc-2.3.8/py/
--rw-r--r--   0 runner    (1001) docker     (122)      235 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/py/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    18708 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/project.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.486563 pywpsrpc-2.3.8/wpsrpc-sdk/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-03 13:09:57.637971 pywpsrpc-2.3.8/wpsrpc-sdk/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-07-03 13:09:57.637971 pywpsrpc-2.3.8/wpsrpc-sdk/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.458562 pywpsrpc-2.3.8/wpsrpc-sdk/include/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.446561 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.446561 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/kfc/
--rw-r--r--   0 runner    (1001) docker     (122)     4508 2023-07-03 13:09:57.641972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/kfc/guid.h
--rw-r--r--   0 runner    (1001) docker     (122)     9916 2023-07-03 13:09:57.641972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/kfc/comsptr.h
--rw-r--r--   0 runner    (1001) docker     (122)   272970 2023-07-03 13:09:57.641972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/kfc/errno.h
--rw-r--r--   0 runner    (1001) docker     (122)     7761 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/pre_platform.h
--rw-r--r--   0 runner    (1001) docker     (122)    17797 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/pre_stdlib.h
--rw-r--r--   0 runner    (1001) docker     (122)    18227 2023-07-03 13:09:57.641972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/int.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.446561 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/wpsapiex/
--rw-r--r--   0 runner    (1001) docker     (122)   143565 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/wpsapiex/wpsapiex.h
--rw-r--r--   0 runner    (1001) docker     (122)     2587 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/wpsrpcsdk.h
--rw-r--r--   0 runner    (1001) docker     (122)     9234 2023-07-03 13:09:57.637971 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/comdef.h
--rw-r--r--   0 runner    (1001) docker     (122)     6630 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/winuser.h
--rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/wpsapiex.h
--rw-r--r--   0 runner    (1001) docker     (122)     3991 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/mso_enum_chart.h
--rw-r--r--   0 runner    (1001) docker     (122)    12667 2023-07-03 13:09:57.641972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/guiddef.h
--rw-r--r--   0 runner    (1001) docker     (122)     6249 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/objbase.h
--rw-r--r--   0 runner    (1001) docker     (122)     8453 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/pre_stddef.h
--rw-r--r--   0 runner    (1001) docker     (122)    13826 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/oleauto.h
--rw-r--r--   0 runner    (1001) docker     (122)    11329 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/typedef.h
--rw-r--r--   0 runner    (1001) docker     (122)    27859 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/oaidl.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.446561 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/ksoapi/
--rw-r--r--   0 runner    (1001) docker     (122)  2707437 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/ksoapi/ksoapi.h
--rw-r--r--   0 runner    (1001) docker     (122)    11017 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/winnt.h
--rw-r--r--   0 runner    (1001) docker     (122)    33561 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/objidl.h
--rw-r--r--   0 runner    (1001) docker     (122)    87307 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/mso_enum.h
--rw-r--r--   0 runner    (1001) docker     (122)    18463 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/variant.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.446561 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/strapi/
--rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/strapi/strapi.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.446561 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/strapi/strapi/
--rw-r--r--   0 runner    (1001) docker     (122)     6232 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/common/strapi/strapi/wchar.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.446561 pywpsrpc-2.3.8/wpsrpc-sdk/include/wpp/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.450561 pywpsrpc-2.3.8/wpsrpc-sdk/include/wpp/wppapi/
--rw-r--r--   0 runner    (1001) docker     (122)  2528680 2023-07-03 13:09:57.689972 pywpsrpc-2.3.8/wpsrpc-sdk/include/wpp/wppapi/wppapi.h
--rw-r--r--   0 runner    (1001) docker     (122)    19534 2023-07-03 13:09:57.689972 pywpsrpc-2.3.8/wpsrpc-sdk/include/wpp/wppapi/wppapi_predef.h
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-07-03 13:09:57.685973 pywpsrpc-2.3.8/wpsrpc-sdk/include/wpp/wppapi.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.450561 pywpsrpc-2.3.8/wpsrpc-sdk/include/et/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.450561 pywpsrpc-2.3.8/wpsrpc-sdk/include/et/etapi/
--rw-r--r--   0 runner    (1001) docker     (122)    60121 2023-07-03 13:09:57.685973 pywpsrpc-2.3.8/wpsrpc-sdk/include/et/etapi/etapi_predef.h
--rw-r--r--   0 runner    (1001) docker     (122)  7872505 2023-07-03 13:09:57.685973 pywpsrpc-2.3.8/wpsrpc-sdk/include/et/etapi/etapi.h
--rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-07-03 13:09:57.665972 pywpsrpc-2.3.8/wpsrpc-sdk/include/et/etapi.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.458562 pywpsrpc-2.3.8/wpsrpc-sdk/include/wps/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.462562 pywpsrpc-2.3.8/wpsrpc-sdk/include/wps/wpsapi/
--rw-r--r--   0 runner    (1001) docker     (122)  5632109 2023-07-03 13:09:57.697973 pywpsrpc-2.3.8/wpsrpc-sdk/include/wps/wpsapi/wpsapi.h
--rw-r--r--   0 runner    (1001) docker     (122)    31992 2023-07-03 13:09:57.689972 pywpsrpc-2.3.8/wpsrpc-sdk/include/wps/wpsapi/undefs.h
--rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-07-03 13:09:57.697973 pywpsrpc-2.3.8/wpsrpc-sdk/include/wps/wpsapi/wpsapi_extend.h
--rw-r--r--   0 runner    (1001) docker     (122)     3631 2023-07-03 13:09:57.689972 pywpsrpc-2.3.8/wpsrpc-sdk/include/wps/wpsapi.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.466562 pywpsrpc-2.3.8/wpsrpc-sdk/lib/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.482562 pywpsrpc-2.3.8/wpsrpc-sdk/lib/x86_64/
--rwxr-xr-x   0 runner    (1001) docker     (122)  9157384 2023-07-03 13:09:57.805975 pywpsrpc-2.3.8/wpsrpc-sdk/lib/x86_64/librpcwpsapi_sysqt5.so
--rwxr-xr-x   0 runner    (1001) docker     (122) 10074176 2023-07-03 13:09:57.753974 pywpsrpc-2.3.8/wpsrpc-sdk/lib/x86_64/librpcetapi_sysqt5.so
--rwxr-xr-x   0 runner    (1001) docker     (122)  6158464 2023-07-03 13:09:57.797975 pywpsrpc-2.3.8/wpsrpc-sdk/lib/x86_64/librpcwppapi_sysqt5.so
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.490563 pywpsrpc-2.3.8/wpsrpc-sdk/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.486563 pywpsrpc-2.3.8/wpsrpc-sdk/tests/wpp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 13:09:57.809975 pywpsrpc-2.3.8/wpsrpc-sdk/tests/wpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-03 13:09:57.805975 pywpsrpc-2.3.8/wpsrpc-sdk/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.490563 pywpsrpc-2.3.8/wpsrpc-sdk/tests/et/
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-03 13:09:57.805975 pywpsrpc-2.3.8/wpsrpc-sdk/tests/et/pch.h
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-07-03 13:09:57.809975 pywpsrpc-2.3.8/wpsrpc-sdk/tests/et/testetbase.h
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-07-03 13:09:57.805975 pywpsrpc-2.3.8/wpsrpc-sdk/tests/et/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3343 2023-07-03 13:09:57.809975 pywpsrpc-2.3.8/wpsrpc-sdk/tests/et/rangevalue.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      586 2023-07-03 13:09:57.809975 pywpsrpc-2.3.8/wpsrpc-sdk/tests/et/testetbase.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.490563 pywpsrpc-2.3.8/wpsrpc-sdk/tests/wps/
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-03 13:09:57.809975 pywpsrpc-2.3.8/wpsrpc-sdk/tests/wps/pch.h
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-07-03 13:09:57.809975 pywpsrpc-2.3.8/wpsrpc-sdk/tests/wps/testbase.h
--rw-r--r--   0 runner    (1001) docker     (122)      619 2023-07-03 13:09:57.809975 pywpsrpc-2.3.8/wpsrpc-sdk/tests/wps/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-07-03 13:09:57.809975 pywpsrpc-2.3.8/wpsrpc-sdk/tests/wps/testbase.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1254 2023-07-03 13:09:57.809975 pywpsrpc-2.3.8/wpsrpc-sdk/tests/wps/comparedocs.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-07-03 13:09:57.637971 pywpsrpc-2.3.8/wpsrpc-sdk/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.594566 pywpsrpc-2.3.8/sip/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.494563 pywpsrpc-2.3.8/sip/common/
--rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/sip/common/guid.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12256 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/oaidl.sip
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/objidl.sip
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.494563 pywpsrpc-2.3.8/sip/common/wpsapiex/
--rw-r--r--   0 runner    (1001) docker     (122)      402 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/KsoDocumentEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1870 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/WaterMarks.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4179 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/_ApplicationEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/Headings.sip
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/_WpsApplicationEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/EtRangeEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/EtApplicationEventsEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/WpsApplicationEventsEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/enums.sip
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/_PresentationEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/_WppApplicationEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/WppApplicationEventsEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/Heading.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1922 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/WorkbooksEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/PresentationsEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/RangeEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)      878 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/HeaderFooterEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/_DocumentEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13151 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/WaterMark.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1573 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/_EtApplicationEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/ApplicationEventsEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/WpsCloudService.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/_WorkbookEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)      871 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/PictureFormatEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1160 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/DocumentsEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex/PrintoutPageEx.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/objbase.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9635 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/sip/common/common.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1855 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/wpsapiex.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/sip/common/export.sip
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.522564 pywpsrpc-2.3.8/sip/common/ksoapi/
--rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/COMAddIns.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2791 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/HTMLProjectItem.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/FullSeriesCollection.sip
--rw-r--r--   0 runner    (1001) docker     (122)    39775 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/Shape.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23739 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/CommandBarControl.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1419 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/DocumentInspectors.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5119 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/WebPageFont.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1453 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/FileDialogSelectedItems.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2691 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/TabStops2.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/GlowFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SignatureProvider.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5068 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IAccessible.sip
--rw-r--r--   0 runner    (1001) docker     (122)    60888 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoChart.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/Permission.sip
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IRibbonExtensibility.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5545 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/ConnectorFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3495 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/ChartColorFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/ksoapi/_CustomXMLPartsEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/PolicyItem.sip
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/ICustomXMLPartEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)      616 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IAssistance.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SearchFolders.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/WorkflowTasks.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2836 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/DiagramNodeChildren.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5550 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/WorkflowTask.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13312 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoTickLabels.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/FoundFiles.sip
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/ICustomTaskPaneConsumer.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9139 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/ChartFillFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    40062 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/ShapeRange.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2570 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/RulerLevel2.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23206 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/FillFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)      290 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoAxisTitle.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoEServicesDialog.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IRibbonControl.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11921 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoChartArea.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6090 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/TextFrame.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1408 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/ThemeFonts.sip
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/ThemeEffectScheme.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/_CommandBarActiveX.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/GradientStops.sip
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/ICustomXMLPartsEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/ThemeColorScheme.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/sip/common/ksoapi/BalloonLabels.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/TabStop2.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/CustomXMLPrefixMapping.sip
--rw-r--r--   0 runner    (1001) docker     (122)    20591 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/ParagraphFormat2.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/Points.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoCategory.sip
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/ksoapi/_IMsoOleAccDispObj.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1990 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/EffectParameter.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/ODSOFilters.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IBlogExtensibility.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13224 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoPlotArea.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/ScopeFolders.sip
--rw-r--r--   0 runner    (1001) docker     (122)      447 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoDispCagNotifySink.sip
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/FreeformBuilder.sip
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/ksoapi/_CommandBars.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/MetaProperties.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3676 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/sip/common/ksoapi/BalloonCheckbox.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoSeriesLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3589 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/PickerDialog.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SmartDocument.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2800 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/WebComponentWindowExternal.sip
--rw-r--r--   0 runner    (1001) docker     (122)    19328 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoLegendKey.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/CustomXMLPrefixMappings.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9967 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/FileDialog.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1552 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/FileTypes.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13472 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/FileSearch.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9965 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceTask.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2608 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtQuickStyle.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/GridLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10679 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SignatureSetup.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10630 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/BulletFormat2.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1451 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/sip/common/ksoapi/Adjustments.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceFolder.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoEnvelopeVB.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4405 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/CanvasShapes.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16641 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/ChartFont.sip
--rw-r--r--   0 runner    (1001) docker     (122)    26769 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/sip/common/ksoapi/Assistant.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1629 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/EncryptionProvider.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2321 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceMembers.sip
--rw-r--r--   0 runner    (1001) docker     (122)      528 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/LanguageSettings.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/Ruler2.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/ShapeNodes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceLinks.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/EffectParameters.sip
--rw-r--r--   0 runner    (1001) docker     (122)    17493 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoTrendline.sip
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/NewFile.sip
--rw-r--r--   0 runner    (1001) docker     (122)   106390 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/ksoapi/enums.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5589 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/ILicWizExternal.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9509 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/Crop.sip
--rw-r--r--   0 runner    (1001) docker     (122)    33720 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/Font2.sip
--rw-r--r--   0 runner    (1001) docker     (122)    19427 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/CommandBar.sip
--rw-r--r--   0 runner    (1001) docker     (122)      727 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IDocumentInspector.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6319 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/DocumentProperty.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/ThemeFontScheme.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/sip/common/ksoapi/AnswerWizardFiles.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2274 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/OfficeTheme.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SearchScope.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SeriesCollection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoDropLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12409 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/sip/common/ksoapi/Balloon.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1716 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/FileDialogFilters.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4931 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoBorder.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5665 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoFloor.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5792 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/ReflectionFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)      718 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IRibbonUI.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6780 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/Shapes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/Sync.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtNode.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IFoundFiles.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11491 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/PictureFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10647 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/Signature.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7504 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoInterior.sip
--rw-r--r--   0 runner    (1001) docker     (122)    14564 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/TextEffectFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/CustomXMLSchema.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/DocumentLibraryVersion.sip
--rw-r--r--   0 runner    (1001) docker     (122)    29151 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/ChartPoint.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1441 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/DiagramNodes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/PropertyTests.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2036 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/PickerProperty.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23779 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoChartTitle.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtQuickStyles.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6083 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/OfficeDataSourceObject.sip
--rw-r--r--   0 runner    (1001) docker     (122)    30852 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/ThreeDFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/ICommandBarButtonEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)      270 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/ksoapi/_CommandBarsEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6644 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/ColorFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/ksoapi/_IMsoDispObj.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1416 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtColors.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/ILicValidator.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/Trendlines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtNodes.sip
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/ksoapi/_CustomTaskPaneEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoChartData.sip
--rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/ICommandBarsEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8339 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/PickerResult.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10353 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/_CommandBarButton.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/PickerFields.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtLayout.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13063 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoLegend.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5415 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/DiagramNode.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1629 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/CustomXMLValidationErrors.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8387 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoDataTable.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoHiLoLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1963 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/MsoDebugOptions_UTs.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3837 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/PictureEffect.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/PropertyTest.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3739 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SignatureSet.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2375 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceFiles.sip
--rw-r--r--   0 runner    (1001) docker     (122)    18600 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/LineFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8723 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/ILicAgent.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/GroupShapes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/sip/common/ksoapi/BalloonLabel.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1674 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/PickerResults.sip
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoHyperlinks.sip
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/_CommandBarButtonEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/PictureEffects.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1408 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SearchScopes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9649 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/WebComponentProperties.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/UserPermission.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/FileDialogFilter.sip
--rw-r--r--   0 runner    (1001) docker     (122)    29490 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoDataLabels.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/ODSOFilter.sip
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IConverterApplicationPreferences.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12882 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/ShadowFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoLeaderLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5149 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoCharacters.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceMember.sip
--rw-r--r--   0 runner    (1001) docker     (122)      905 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoCorners.sip
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IConverterPreferences.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IConverter.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/ODSOColumn.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/MsoDebugOptions_UT.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1800 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/DocumentProperties.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/CommandBarControls.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6113 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/MsoDebugOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)    47649 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoAxis.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3423 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceFile.sip
--rw-r--r--   0 runner    (1001) docker     (122)    28720 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoChartGroup.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4860 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/COMAddIn.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7714 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspace.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6024 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/Script.sip
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoDisplayUnitLabel.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2188 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoContactCard.sip
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/ksoapi/_CustomXMLPartEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/ODSOColumns.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2274 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/MsoDebugOptions_UTManager.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6207 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceLink.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3326 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoUpBars.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/sip/common/ksoapi/Axes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2096 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/ScopeFolder.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1420 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/HTMLProjectItems.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6868 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoWalls.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6094 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SmartArt.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1975 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/ksoapi/_CustomXMLSchemaCollection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/WorkflowTemplate.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/ThemeFont.sip
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/sip/common/ksoapi/AnswerWizard.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6841 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoChartFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    48908 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoSeries.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2470 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/sip/common/ksoapi/BalloonCheckboxes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/LegendEntries.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/ksoapi/_CustomXMLParts.sip
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/ksoapi/_CommandBarComboBoxEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5139 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/MetaProperty.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoDownBars.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6671 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/ksoapi/_CustomXMLPart.sip
--rw-r--r--   0 runner    (1001) docker     (122)    18820 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/TextFrame2.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceTasks.sip
--rw-r--r--   0 runner    (1001) docker     (122)    40350 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoDataLabel.sip
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/ContactCard.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/CommandBarPopup.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/WebPageFonts.sip
--rw-r--r--   0 runner    (1001) docker     (122)      481 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/CustomTaskPaneEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2500 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SoftEdgeFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10003 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SignatureInfo.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3268 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/CustomXMLValidationError.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/HTMLProject.sip
--rw-r--r--   0 runner    (1001) docker     (122)      362 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/ICommandBarComboBoxEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5066 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoDiagram.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/CustomXMLNodes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6900 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/WebComponentFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1397 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/RulerLevels2.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1512 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/CategoryCollection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoErrorBars.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2275 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceFolders.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/DocumentInspector.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1421 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtLayouts.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/ShapeNode.sip
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IMsoEnvelopeVBEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3686 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/TextColumn2.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/ChartGroups.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/DocumentLibraryVersions.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11340 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/TextRange2.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/ThemeColor.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6376 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/WebComponent.sip
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/ICTPFactory.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/GradientStop.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/PickerProperties.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1419 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/WorkflowTemplates.sip
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IConverterUICallback.sip
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IBlogPictureExtensibility.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8651 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/ksoapi/_CommandBarComboBox.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12543 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/CustomXMLNode.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2057 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/PickerField.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/Scripts.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6057 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/LegendEntry.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4387 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/ServerPolicy.sip
--rw-r--r--   0 runner    (1001) docker     (122)    25448 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/IFind.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-07-03 13:09:56.597951 pywpsrpc-2.3.8/sip/common/ksoapi/MsoDebugOptions_UTRunResult.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9674 2023-07-03 13:09:56.593951 pywpsrpc-2.3.8/sip/common/ksoapi/CalloutFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7922 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/ksoapi/_CustomTaskPane.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2608 2023-07-03 13:09:56.601951 pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtColor.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4132 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/common/typedef.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9598 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/sip/common/ksoapi.sip
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.570566 pywpsrpc-2.3.8/sip/rpcwpsapi/
--rw-r--r--   0 runner    (1001) docker     (122)     2068 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTagRecognizers.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Break.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1476 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/FullSeriesCollection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTags.sip
--rw-r--r--   0 runner    (1001) docker     (122)    55364 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Shape.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/HTMLDivisions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3204 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/RecentFiles.sip
--rw-r--r--   0 runner    (1001) docker     (122)   100162 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/sip/rpcwpsapi/mso_enum.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMaths.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2807 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Source.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6053 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Revision.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23740 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ChartTitle.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathMatCols.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3675 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/GlowFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/InlineShapes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathFrac.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4085 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/EmailSignature.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16500 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/FormField.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1997 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/ReadabilityStatistic.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6088 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ConnectorFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    29309 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/DataLabels.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TablesOfContents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Reviewers.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ChartColorFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    33505 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Table.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3098 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Variable.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4932 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ChartBorder.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1966 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/XSLTransform.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3814 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/RecentFile.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/sip/rpcwpsapi/_Application_extend.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2627 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Conflict.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathAutoCorrectEntries.sip
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/IApplicationEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/SynonymInfo.sip
--rw-r--r--   0 runner    (1001) docker     (122)    17491 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Trendline.sip
--rw-r--r--   0 runner    (1001) docker     (122)    19328 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/LegendKey.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/DiagramNodeChildren.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3055 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Words.sip
--rw-r--r--   0 runner    (1001) docker     (122)    17342 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Frameset.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9870 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ChartFillFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4734 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Line.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2033 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/FontNames.sip
--rw-r--r--   0 runner    (1001) docker     (122)    47032 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Axis.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9316 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathDelim.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathScrSub.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2022 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/FirstLetterException.sip
--rw-r--r--   0 runner    (1001) docker     (122)    51599 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/ShapeRange.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ContentControlListEntries.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TaskPane.sip
--rw-r--r--   0 runner    (1001) docker     (122)    22425 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/FillFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TwoInitialCapsExceptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathFunc.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3103 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathRad.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13916 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CustomLabel.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23358 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Cell.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4900 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Indexes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1429 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/IApplicationEvents2.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5635 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CoAuthoring.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Reviewer.sip
--rw-r--r--   0 runner    (1001) docker     (122)   325888 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Options.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/ListLevels.sip
--rw-r--r--   0 runner    (1001) docker     (122)    21304 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TextFrame.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Zooms.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11461 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMath.sip
--rw-r--r--   0 runner    (1001) docker     (122)    42752 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Window.sip
--rw-r--r--   0 runner    (1001) docker     (122)    20665 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Template.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CoAuthor.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8731 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/ListFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathRecognizedFunction.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Browser.sip
--rw-r--r--   0 runner    (1001) docker     (122)    47873 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/sip/rpcwpsapi/_ParagraphFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    28414 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Style.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2090 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Frames.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4618 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/HangulHanjaConversionDictionaries.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10554 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Comment.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2036 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTagTypes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8381 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Task.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathMatRows.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9038 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Endnotes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9418 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ConditionalStyle.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2223 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathFunctions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Points.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2781 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/PageNumber.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CustomProperties.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2271 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/AutoCorrectEntries.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3282 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/DownBars.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TwoInitialCapsException.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2188 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/AddIns.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3257 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/FormFields.sip
--rw-r--r--   0 runner    (1001) docker     (122)    28848 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Point.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathAcc.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/FreeformBuilder.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6788 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ChartFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12355 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Hyperlink.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6958 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Documents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Floor.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Hyperlinks.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2201 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CoAuthLocks.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5679 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/HorizontalLineFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/XMLSchemaReference.sip
--rw-r--r--   0 runner    (1001) docker     (122)    14075 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathFunction.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7587 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/LinkFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2960 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/XMLNamespace.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3238 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Editor.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6562 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/LineNumbering.sip
--rw-r--r--   0 runner    (1001) docker     (122)    55715 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/sip/rpcwpsapi/_Font.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Adjustments.sip
--rw-r--r--   0 runner    (1001) docker     (122)    47441 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Paragraphs.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16698 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TableOfFigures.sip
--rw-r--r--   0 runner    (1001) docker     (122)    18233 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OfdExportOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/MailMergeDataField.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2203 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/XSLTransforms.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CanvasShapes.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16641 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ChartFont.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TabStop.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2571 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathScrPre.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OtherCorrectionsExceptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/ListEntries.sip
--rw-r--r--   0 runner    (1001) docker     (122)    43114 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Find.sip
--rw-r--r--   0 runner    (1001) docker     (122)    14707 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Pane.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/EmailAuthor.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/XMLMapping.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/RepeatingSectionItemColl.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/ShapeNodes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2020 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Sources.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Tables.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2018 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/MailMergeFieldNames.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Rectangles.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7499 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/IWORDCtrlExtender.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7268 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathEqArray.sip
--rw-r--r--   0 runner    (1001) docker     (122)    15834 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/MailMergeDataSource.sip
--rw-r--r--   0 runner    (1001) docker     (122)   139181 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/sip/rpcwpsapi/enums.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2949 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/UndoRecord.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6055 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Bookmark.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/HangulAndAlphabetExceptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Styles.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5176 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TextRetrievalMode.sip
--rw-r--r--   0 runner    (1001) docker     (122)    17982 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Frame.sip
--rw-r--r--   0 runner    (1001) docker     (122)    40355 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/DataLabel.sip
--rw-r--r--   0 runner    (1001) docker     (122)    40027 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Envelope.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2026 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/ReadabilityStatistics.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Subdocuments.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/SeriesCollection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/ReflectionFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8915 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/MailingLabel.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7917 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Shapes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8731 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/IKRpcClient.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/AutoCaptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2130 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/SeriesLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6807 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/FootnoteOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10262 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathMat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3773 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Windows.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathBreaks.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12470 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/PictureFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1981 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/MailMergeFieldName.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4759 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TablesOfFigures.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5071 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TextInput.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7493 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/sip/rpcwpsapi/_OLEControl.sip
--rw-r--r--   0 runner    (1001) docker     (122)    15033 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TextEffectFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ContentControlListEntry.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8925 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/XMLSchemaReferences.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2594 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/ProofreadingErrors.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4369 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TablesOfAuthorities.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3365 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/ErrorBars.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/DiagramNodes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4356 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/AutoTextEntry.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/BuildingBlockEntries.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2576 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Footnote.sip
--rw-r--r--   0 runner    (1001) docker     (122)      903 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Corners.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CoAuthLock.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8592 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Language.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10792 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/OLEFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    31043 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/ThreeDFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/XMLChildNodeSuggestion.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3354 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/FileConverters.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13930 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ColorFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    14376 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TableOfContents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Templates.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ContentControls.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/EmailSignatureEntries.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Research.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/ListEntry.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3211 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/RevisionsFilter.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Lines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/KeyBindings.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/MailMergeFields.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3926 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/ListTemplate.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Trendlines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2075 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Panes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1449 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/SpellingSuggestion.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CustomLabels.sip
--rw-r--r--   0 runner    (1001) docker     (122)   119902 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/sip/rpcwpsapi/_Application.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4783 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathGroupChar.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TablesOfAuthoritiesCategories.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3946 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathScrSubSup.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4380 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/AutoCaption.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Comments.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2079 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathArgs.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Conflicts.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13210 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/PlotArea.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6076 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/DiagramNode.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3202 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathMatCol.sip
--rw-r--r--   0 runner    (1001) docker     (122)    30449 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ContentControl.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13304 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TickLabels.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Characters.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4188 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Broadcast.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2091 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CaptionLabels.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2543 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathBreak.sip
--rw-r--r--   0 runner    (1001) docker     (122)    28387 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ChartGroup.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16566 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TableStyle.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4824 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathBox.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5020 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Subdocument.sip
--rw-r--r--   0 runner    (1001) docker     (122)    27619 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Rows.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1979 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Categories.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathRecognizedFunctions.sip
--rw-r--r--   0 runner    (1001) docker     (122)    54770 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Paragraph.sip
--rw-r--r--   0 runner    (1001) docker     (122)    95513 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Range.sip
--rw-r--r--   0 runner    (1001) docker     (122)    22585 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/AutoCorrect.sip
--rw-r--r--   0 runner    (1001) docker     (122)    17841 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/LineFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13054 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Legend.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/ProtectedViewWindows.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTag.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2074 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/GroupShapes.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16164 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/ListLevel.sip
--rw-r--r--   0 runner    (1001) docker     (122)    53164 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Chart.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2027 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathMatRow.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9263 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Columns.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/StoryRanges.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ChartCategory.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4584 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathAutoCorrect.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4991 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/MailMergeField.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3785 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTagRecognizer.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3186 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Category.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/BuildingBlockTypes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Endnote.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23739 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/AxisTitle.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2018 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/MailMergeDataFields.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8764 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CaptionLabel.sip
--rw-r--r--   0 runner    (1001) docker     (122)   217343 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/sip/rpcwpsapi/_Document.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathLimUpp.sip
--rw-r--r--   0 runner    (1001) docker     (122)    14778 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/WebOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3280 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/UpBars.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4442 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/List.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathAutoCorrectEntry.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6656 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Section.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/DropLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/ListTemplates.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23746 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/DisplayUnitLabel.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12834 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/ShadowFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5872 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/KeyBinding.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TabStops.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTagActions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/HangulAndAlphabetException.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5162 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ChartCharacters.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TextColumn.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7768 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/BuildingBlock.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7323 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/HTMLDivision.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7500 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Interior.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/BuildingBlocks.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/IApplicationEvents3.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10619 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Replacement.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4318 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/IApplicationEvents4.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6824 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Walls.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5661 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/EndnoteOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4652 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Bookmarks.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TableOfAuthoritiesCategory.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/HiLoLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/MailMessage.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Variables.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2750 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Bibliography.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9480 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Border.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10396 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/sip/rpcwpsapi/rpcwpsapi.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Dialogs.sip
--rw-r--r--   0 runner    (1001) docker     (122)    48838 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/EmailOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)    14664 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TableOfAuthorities.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5689 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Dictionary.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/AutoTextEntries.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12132 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Cells.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8833 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/WrapFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3458 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Fields.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Lists.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11815 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/ProtectedViewWindow.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CoAuthUpdate.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Email.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11141 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Column.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2536 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/EmailSignatureEntry.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Axes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Breaks.sip
--rw-r--r--   0 runner    (1001) docker     (122)    20460 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/MailMerge.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CoAuthors.sip
--rw-r--r--   0 runner    (1001) docker     (122)    38309 2023-07-03 13:09:56.649952 pywpsrpc-2.3.8/sip/rpcwpsapi/_LetterContent.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8302 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathPhantom.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5489 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/StyleSheet.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6142 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/FileConverter.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7896 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/DocumentField.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/FirstLetterExceptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10658 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ChartArea.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10774 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathBorderBox.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12249 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Index.sip
--rw-r--r--   0 runner    (1001) docker     (122)    26013 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/InlineShape.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4302 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/AutoCorrectEntry.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8152 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathNary.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7893 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TextColumns.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2696 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/SpellingSuggestions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3114 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/HeadingStyle.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/RepeatingSectionItem.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1489 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/LegendEntries.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CustomProperty.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8324 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/DataTable.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Languages.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/ListGallery.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6214 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/HeaderFooter.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Pages.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Gridlines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/BuildingBlockType.sip
--rw-r--r--   0 runner    (1001) docker     (122)    48635 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Series.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5998 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CheckBox.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3091 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/SoftEdgeFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4139 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Dialog.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/LeaderLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3059 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Sentences.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8768 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/RoutingSlip.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4207 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/DropDown.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2105 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Tasks.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3373 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTagType.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11370 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Field.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9048 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Footnotes.sip
--rw-r--r--   0 runner    (1001) docker     (122)    40169 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/PageSetup.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Revisions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CategoryCollection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2027 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/MappedDataFields.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/XMLNodes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/XMLChildNodeSuggestions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2027 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OtherCorrectionsException.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/ShapeNode.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Editors.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3958 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Dictionaries.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4985 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/AddIn.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7313 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Shading.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ChartGroups.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4886 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Page.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10873 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/System.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/ListParagraphs.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4744 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Rectangle.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3244 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Version.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathLimLow.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/XMLNamespaces.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathBar.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8578 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/Mailer.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16906 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/PdfExportOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12216 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/PageNumbers.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10595 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTagAction.sip
--rw-r--r--   0 runner    (1001) docker     (122)    22121 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/DefaultWebOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4534 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/KeysBoundTo.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16911 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Row.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/HeadersFooters.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CoAuthUpdates.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2113 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/HeadingStyles.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/OMathScrSup.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/ChartData.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/DocumentFields.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6035 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/LegendEntry.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/TaskPanes.sip
--rw-r--r--   0 runner    (1001) docker     (122)    73015 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Selection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5547 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/DropCap.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16323 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/XMLNode.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5626 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Diagram.sip
--rw-r--r--   0 runner    (1001) docker     (122)    76697 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/View.sip
--rw-r--r--   0 runner    (1001) docker     (122)    28828 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/Borders.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3246 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Versions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/ListGalleries.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10237 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwpsapi/CalloutFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-07-03 13:09:56.637951 pywpsrpc-2.3.8/sip/rpcwpsapi/MappedDataField.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5305 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/Zoom.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4374 2023-07-03 13:09:56.641951 pywpsrpc-2.3.8/sip/rpcwpsapi/Sections.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-07-03 13:09:56.645952 pywpsrpc-2.3.8/sip/rpcwpsapi/StyleSheets.sip
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.594566 pywpsrpc-2.3.8/sip/rpcwppapi/
--rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/ThemeVariants.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/FullSeriesCollection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ColorScheme.sip
--rw-r--r--   0 runner    (1001) docker     (122)    48185 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Shape.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Collection.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16214 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/AnimationSettings.sip
--rw-r--r--   0 runner    (1001) docker     (122)    24353 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ChartTitle.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5534 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ConnectorFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    29881 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/DataLabels.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3171 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/RulerLevel.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/PublishObject.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3600 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ChartColorFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    14217 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Table.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5537 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ChartBorder.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ColorEffect.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1804 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/CellRange.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/SlideShowWindows.sip
--rw-r--r--   0 runner    (1001) docker     (122)    18061 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwppapi/Trendline.sip
--rw-r--r--   0 runner    (1001) docker     (122)    19906 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/LegendKey.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/DiagramNodeChildren.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10469 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ChartFillFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    47580 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Axis.sip
--rw-r--r--   0 runner    (1001) docker     (122)    14996 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/CustomLayout.sip
--rw-r--r--   0 runner    (1001) docker     (122)    50088 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/ShapeRange.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23227 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/FillFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    20876 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/PrintOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/PrintRanges.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Cell.sip
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/MouseDownHandler.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4318 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Options.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12749 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/TextFrame.sip
--rw-r--r--   0 runner    (1001) docker     (122)    15090 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/MediaFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16153 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/ParagraphFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8482 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/OCXExtender.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Coauthoring.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Comment.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5693 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Design.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13523 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwppapi/_Master.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3603 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/EApplication.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7209 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/ScaleEffect.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Points.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8287 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/MotionEffect.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8487 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/IPPTCtrlExtender.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3916 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/DownBars.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1400 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/AddIns.sip
--rw-r--r--   0 runner    (1001) docker     (122)    29708 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Point.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4886 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/PropertyEffect.sip
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/FreeformBuilder.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7482 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ChartFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8759 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Hyperlink.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6249 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Floor.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Hyperlinks.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4427 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/FilterEffect.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/CustomLayouts.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/LinkFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Adjustments.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1635 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Designs.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4394 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/CanvasShapes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1372 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/DocumentWindows.sip
--rw-r--r--   0 runner    (1001) docker     (122)    17226 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ChartFont.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/TabStop.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1718 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/SoundFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16987 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/DocumentWindow.sip
--rw-r--r--   0 runner    (1001) docker     (122)    15806 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/SlideShowView.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Pane.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/ShapeNodes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/NamedSlideShows.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7096 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/EffectParameters.sip
--rw-r--r--   0 runner    (1001) docker     (122)   151504 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwppapi/enums.sip
--rw-r--r--   0 runner    (1001) docker     (122)    19994 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Font.sip
--rw-r--r--   0 runner    (1001) docker     (122)    40938 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/DataLabel.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/SeriesCollection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9707 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Shapes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9102 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/IKRpcClient.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/SeriesLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11496 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/PictureFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    14553 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/TextEffectFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/TableBackground.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9404 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/PlaySettings.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3980 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ErrorBars.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/SoundEffect.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1251 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/RulerLevels.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Presentations.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/DiagramNodes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ColorSchemes.sip
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/OCXExtenderEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Corners.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3970 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/OLEFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ExtraColors.sip
--rw-r--r--   0 runner    (1001) docker     (122)    30841 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/ThreeDFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/TextStyleLevel.sip
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/FileConverters.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6744 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ColorFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Research.sip
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/SldEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8779 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/SlideShowWindow.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwppapi/Trendlines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2165 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwppapi/TimeLine.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Panes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/SlideNavigation.sip
--rw-r--r--   0 runner    (1001) docker     (122)    48135 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwppapi/_Application.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Comments.sip
--rw-r--r--   0 runner    (1001) docker     (122)    66201 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwppapi/_Presentation.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13826 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/PlotArea.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/SectionProperties.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5392 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/DiagramNode.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13897 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/TickLabels.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4904 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Broadcast.sip
--rw-r--r--   0 runner    (1001) docker     (122)    28949 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ChartGroup.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/TableStyle.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Rows.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3057 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/AutoCorrect.sip
--rw-r--r--   0 runner    (1001) docker     (122)    18589 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/LineFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13651 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Legend.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/ProtectedViewWindows.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/GroupShapes.sip
--rw-r--r--   0 runner    (1001) docker     (122)    57799 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Chart.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Columns.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3254 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Guide.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ChartCategory.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/TextStyle.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1343 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Sequences.sip
--rw-r--r--   0 runner    (1001) docker     (122)    24352 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/AxisTitle.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/NamedSlideShow.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/MediaBookmark.sip
--rw-r--r--   0 runner    (1001) docker     (122)    15599 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwppapi/WebOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwppapi/UpBars.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2736 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/DropLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23115 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/DisplayUnitLabel.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12871 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/ShadowFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/TextStyles.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10449 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Effect.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/TabStops.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4280 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/CommandEffect.sip
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/PresEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5765 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ChartCharacters.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/ResampleMediaTasks.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4012 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/RotationEffect.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8101 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Interior.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1263 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/PublishObjects.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2870 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Player.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7456 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwppapi/Walls.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9086 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ActionSetting.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12749 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/TextRange.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2746 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/HiLoLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1949 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/RGBColor.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9981 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/AnimationBehavior.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23508 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwppapi/_Slide.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16951 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/SlideShowSettings.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Tags.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3165 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/SetEffect.sip
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/MediaBookmarks.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6078 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/EffectInformation.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10085 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/ProtectedViewWindow.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10998 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/SlideShowTransition.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2596 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Column.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Axes.sip
--rw-r--r--   0 runner    (1001) docker     (122)    20848 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwppapi/Timing.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11241 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/BulletFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7233 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/FileConverter.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/CustomerData.sip
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwppapi/_PowerRex.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11283 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ChartArea.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Slides.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7075 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/ResampleMediaTask.sip
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/MasterEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/LegendEntries.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8939 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/DataTable.sip
--rw-r--r--   0 runner    (1001) docker     (122)    18857 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/TextFrame2.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5437 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/HeaderFooter.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2754 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Gridlines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/AnimationBehaviors.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3259 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Sequence.sip
--rw-r--r--   0 runner    (1001) docker     (122)    49454 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Series.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2130 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/LeaderLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/MouseTracker.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Fonts.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/ObjectVerbs.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/TextStyleLevels.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/PageSetup.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Theme.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Guides.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/CategoryCollection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3071 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/ThemeVariant.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2165 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/ShapeNode.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4242 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/AnimationPoint.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/AddIn.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Placeholders.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1990 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ChartGroups.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1971 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/PrintRange.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5713 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwppapi/rpcwppapi.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1291 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ActionSettings.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/PlaceholderFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    21610 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/DefaultWebOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Row.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/HeadersFooters.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/AnimationPoints.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/ChartData.sip
--rw-r--r--   0 runner    (1001) docker     (122)    24699 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/SlideRange.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6646 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/LegendEntry.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5378 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Selection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5051 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Diagram.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10649 2023-07-03 13:09:56.633951 pywpsrpc-2.3.8/sip/rpcwppapi/View.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/Borders.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9663 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcwppapi/CalloutFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2042 2023-07-03 13:09:56.629951 pywpsrpc-2.3.8/sip/rpcwppapi/Ruler.sip
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:10:23.642567 pywpsrpc-2.3.8/sip/rpcetapi/
--rw-r--r--   0 runner    (1001) docker     (122)    29903 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IListObject.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4253 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IOLEDBError.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IMenus.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3069 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISlicers.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9375 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IListDataFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5679 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/Solver.sip
--rw-r--r--   0 runner    (1001) docker     (122)    97555 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcetapi/mso_enum.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IIconCriteria.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPoints.sip
--rw-r--r--   0 runner    (1001) docker     (122)    14286 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDialogFrame.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9465 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDataTable.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12243 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IAutoCorrect.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2798 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IAddIns2.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1868 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IFreeformBuilder.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3166 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDataBarBorder.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7192 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/ILegendEntry.sip
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICanvasShapes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7080 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISlicerCacheLevel.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4341 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICustomProperty.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISheetViews.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IXmlSchemas.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8469 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/PublishObject.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2425 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IIcon.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5254 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IIconCriterion.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8420 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IProtection.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16976 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModule.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23668 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/ILabel.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3382 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IXmlNamespaces.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5882 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IFilter.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IMenu.sip
--rw-r--r--   0 runner    (1001) docker     (122)    60344 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDrawingObjects.sip
--rw-r--r--   0 runner    (1001) docker     (122)    99401 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IRange.sip
--rw-r--r--   0 runner    (1001) docker     (122)    28540 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IEXCELCtrlExtender.sip
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/WorksheetFunction.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10422 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISmartTagAction.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IOLEFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2778 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IToolbars.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ITableStyleElement.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2838 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/DiagramNodeChildren.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10963 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IToolbar.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IAddIns.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2701 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelTableColumns.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IUserAccessList.sip
--rw-r--r--   0 runner    (1001) docker     (122)    18355 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotItem.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2976 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICalculatedFields.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IToolbarButtons.sip
--rw-r--r--   0 runner    (1001) docker     (122)      443 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IRefreshEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2775 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ITableStyles.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23693 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISpinners.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2969 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICalculatedItems.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13781 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IGraphic.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2655 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IODBCErrors.sip
--rw-r--r--   0 runner    (1001) docker     (122)      896 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IRtdServer.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23206 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/FillFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    32875 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotCache.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IWatch.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2976 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IProtectedViewWindows.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3833 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/ILinkFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotLine.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4325 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModel.sip
--rw-r--r--   0 runner    (1001) docker     (122)    21359 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IODBCConnection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IXmlDataBinding.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6460 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IPhonetic.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2688 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelTableNameChange.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2950 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IListRows.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8109 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IColorScale.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3956 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISparkHorizontalAxis.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3222 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IRecentFile.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2778 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IMenuBars.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3130 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotFields.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IUserAccess.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDocEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelTableNames.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IComments.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IQueryTables.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4977 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISparkPoints.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8974 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IAddIn.sip
--rw-r--r--   0 runner    (1001) docker     (122)    35195 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IOLEDBConnection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IParameter.sip
--rw-r--r--   0 runner    (1001) docker     (122)    15346 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IErrorCheckingOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)    40150 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IShapeRange.sip
--rw-r--r--   0 runner    (1001) docker     (122)    25007 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISpinner.sip
--rw-r--r--   0 runner    (1001) docker     (122)    33599 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IGroupObjects.sip
--rw-r--r--   0 runner    (1001) docker     (122)    27288 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IListBox.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6318 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICharacters.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2671 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelTables.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2576 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelTableColumn.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISort.sip
--rw-r--r--   0 runner    (1001) docker     (122)    14257 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/ITop10.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2653 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelColumnName.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IListColumns.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16655 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPlotArea.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7491 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IShapes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IAllowEditRanges.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2563 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IChartGroups.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6041 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IColorStop.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8872 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IPhonetics.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IGridlines.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23814 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISpellingOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11929 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICalculatedMember.sip
--rw-r--r--   0 runner    (1001) docker     (122)    24842 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IChartTitle.sip
--rw-r--r--   0 runner    (1001) docker     (122)    28070 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICheckBoxes.sip
--rw-r--r--   0 runner    (1001) docker     (122)    48835 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IShape.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2672 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/ILegendEntries.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4174 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IChartColorFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IGroupShapes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3007 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/CubeFields.sip
--rw-r--r--   0 runner    (1001) docker     (122)    24844 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IListBoxes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ITab.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1449 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/Adjustments.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2660 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelMeasureName.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4917 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IMultiThreadedCalculation.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IListObjects.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2846 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISlicerPivotTables.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2405 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISmartTags.sip
--rw-r--r--   0 runner    (1001) docker     (122)    21372 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IOLEObjects.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IResearch.sip
--rw-r--r--   0 runner    (1001) docker     (122)    18605 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/ITrendline.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3199 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IError.sip
--rw-r--r--   0 runner    (1001) docker     (122)    28533 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/_IOLEObject.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISoundNote.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3096 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISlicerCaches.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPublishObjects.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10560 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotFilter.sip
--rw-r--r--   0 runner    (1001) docker     (122)    28998 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IStyle.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/ShapeNodes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IFormatConditions.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11318 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotCell.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISmartTagActions.sip
--rw-r--r--   0 runner    (1001) docker     (122)    41429 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDataLabel.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IAutoRecover.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4389 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IAction.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7059 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotFormula.sip
--rw-r--r--   0 runner    (1001) docker     (122)    33443 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ITextBoxes.sip
--rw-r--r--   0 runner    (1001) docker     (122)    80561 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/enums.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4623 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelTable.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6674 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IRectangularGradient.sip
--rw-r--r--   0 runner    (1001) docker     (122)    14448 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/ITickLabels.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2988 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotTableChangeList.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7979 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IWalls.sip
--rw-r--r--   0 runner    (1001) docker     (122)    32524 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDrawings.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9953 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IMenuItem.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2814 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IConditionValue.sip
--rw-r--r--   0 runner    (1001) docker     (122)    14178 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/ILegend.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6170 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IFormatColor.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3056 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotItems.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11886 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IProtectedViewWindow.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2680 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IStyles.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IColorScaleCriteria.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5659 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDialog.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13376 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ITableObject.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDialogs.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7480 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IScenario.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7423 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IKRpcClient.sip
--rw-r--r--   0 runner    (1001) docker     (122)    26124 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IScrollBar.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6433 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISparkVerticalAxis.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11495 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/PictureFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    19651 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IPictures.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3909 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IPage.sip
--rw-r--r--   0 runner    (1001) docker     (122)    35083 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IGroupObject.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23576 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IGroupBoxes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2880 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelRelationships.sip
--rw-r--r--   0 runner    (1001) docker     (122)    14545 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/TextEffectFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8319 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IWorksheetView.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModuleView.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5913 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IAppEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/DiagramNodes.sip
--rw-r--r--   0 runner    (1001) docker     (122)    17977 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDatabar.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12491 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IWorkbookConnection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6678 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISlicerItem.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7382 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICharts.sip
--rw-r--r--   0 runner    (1001) docker     (122)    24841 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IAxisTitle.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10966 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IUniqueValues.sip
--rw-r--r--   0 runner    (1001) docker     (122)    30811 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/ThreeDFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    67483 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/_Worksheet.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/ColorFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4395 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IVPageBreak.sip
--rw-r--r--   0 runner    (1001) docker     (122)    24803 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IEditBoxes.sip
--rw-r--r--   0 runner    (1001) docker     (122)    28901 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/CubeField.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13020 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IChartArea.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4449 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IWorkbookEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IXmlNamespace.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISeriesCollection.sip
--rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/ILegendKey.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7999 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IChartFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    34758 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IRectangle.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2701 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelMeasureNames.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3170 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IXmlSchema.sip
--rw-r--r--   0 runner    (1001) docker     (122)   266150 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/_Application.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5271 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IOutline.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICustomViews.sip
--rw-r--r--   0 runner    (1001) docker     (122)    32203 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IOvals.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4395 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IHPageBreak.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IScenarios.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/DiagramNode.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8449 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISortField.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2771 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IVPageBreaks.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IHeaderFooter.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IAutoFilter.sip
--rw-r--r--   0 runner    (1001) docker     (122)    37260 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IButtons.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3058 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotCaches.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IMenuItems.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7398 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDialogSheets.sip
--rw-r--r--   0 runner    (1001) docker     (122)    72467 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotField.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16433 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDataFeedConnection.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11024 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IChartFillFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ITableStyleElements.sip
--rw-r--r--   0 runner    (1001) docker     (122)    18573 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/LineFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7713 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/Workbooks.sip
--rw-r--r--   0 runner    (1001) docker     (122)    24812 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IScrollBars.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2848 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IParameters.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5199 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelRelationship.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7660 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IWorksheets.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7992 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/Sheets.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4441 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IUpBars.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2788 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IWatches.sip
--rw-r--r--   0 runner    (1001) docker     (122)    88556 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/_Chart.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2673 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)    28654 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IOptionButtons.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelColumnChanges.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6778 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IFloor.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3675 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IConnections.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICategoryCollection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4525 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IErrorBars.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2724 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IFileExportConverters.sip
--rw-r--r--   0 runner    (1001) docker     (122)    55522 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IWindow.sip
--rw-r--r--   0 runner    (1001) docker     (122)   120586 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotTable.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IChartEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13695 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IToolbarButton.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2771 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IHPageBreaks.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2990 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IHyperlinks.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4554 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IWindows.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IChartView.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDropLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/ITrendlines.sip
--rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IValidation.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8499 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IListColumn.sip
--rw-r--r--   0 runner    (1001) docker     (122)    15372 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/WebOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4367 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISmartTagRecognizer.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10376 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IMailer.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IListRow.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2659 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IFullSeriesCollection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2638 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IPanes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IHiLoLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IQuickAnalysis.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12865 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/ShadowFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    27311 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDropDowns.sip
--rw-r--r--   0 runner    (1001) docker     (122)    29705 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDropDown.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISparkColor.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/_DebugTools.sip
--rw-r--r--   0 runner    (1001) docker     (122)    33520 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IOval.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3270 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotLineCells.sip
--rw-r--r--   0 runner    (1001) docker     (122)    49911 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISeries.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4443 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDownBars.sip
--rw-r--r--   0 runner    (1001) docker     (122)    29963 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IOptionButton.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISlicerCacheLevels.sip
--rw-r--r--   0 runner    (1001) docker     (122)    22797 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IChartObject.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IAxes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2939 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotFormulas.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3295 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISeriesLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDialogSheetView.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotValueCell.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3799 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICalculatedMembers.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IODBCError.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelTableNameChanges.sip
--rw-r--r--   0 runner    (1001) docker     (122)    21580 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/ILine.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2672 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/ILeaderLines.sip
--rw-r--r--   0 runner    (1001) docker     (122)    20544 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IChartObjects.sip
--rw-r--r--   0 runner    (1001) docker     (122)    73410 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/_IQueryTable.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10165 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ITableStyle.sip
--rw-r--r--   0 runner    (1001) docker     (122)   129982 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/_Workbook.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotAxis.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2658 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IActions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2668 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotItemList.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2808 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IXmlMaps.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3834 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IRecentFiles.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8490 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelChanges.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2994 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISortFields.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/ILinearGradient.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IMenuBar.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISmartTagRecognizers.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/INames.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5169 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/INegativeBarFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IErrors.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4479 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IWorksheetDataConnection.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/TreeviewControl.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6190 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDiagram.sip
--rw-r--r--   0 runner    (1001) docker     (122)    16411 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IName.sip
--rw-r--r--   0 runner    (1001) docker     (122)    29382 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICheckBox.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7385 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModules.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5770 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IPane.sip
--rw-r--r--   0 runner    (1001) docker     (122)    50185 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IPageSetup.sip
--rw-r--r--   0 runner    (1001) docker     (122)    48093 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IAxis.sip
--rw-r--r--   0 runner    (1001) docker     (122)    15435 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IXmlMap.sip
--rw-r--r--   0 runner    (1001) docker     (122)    33446 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IRectangles.sip
--rw-r--r--   0 runner    (1001) docker     (122)    19861 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISlicer.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3021 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISparklineGroups.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4001 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IXPath.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IFileExportConverter.sip
--rw-r--r--   0 runner    (1001) docker     (122)    18842 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/TextFrame2.sip
--rw-r--r--   0 runner    (1001) docker     (122)    31084 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IArcs.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotTables.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1527 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IRTD.sip
--rw-r--r--   0 runner    (1001) docker     (122)    26233 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/ITextConnection.sip
--rw-r--r--   0 runner    (1001) docker     (122)    38575 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IButton.sip
--rw-r--r--   0 runner    (1001) docker     (122)     7622 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/ITimelineViewState.sip
--rw-r--r--   0 runner    (1001) docker     (122)    34756 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ITextBox.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDummy.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2088 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICorners.sip
--rw-r--r--   0 runner    (1001) docker     (122)    14206 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IInterior.sip
--rw-r--r--   0 runner    (1001) docker     (122)    29512 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IChartGroup.sip
--rw-r--r--   0 runner    (1001) docker     (122)    22490 2023-07-03 13:09:56.625951 pywpsrpc-2.3.8/sip/rpcetapi/rpcetapi.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3612 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotFilters.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2649 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IFilters.sip
--rw-r--r--   0 runner    (1001) docker     (122)    52088 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDialogSheet.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IPages.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2696 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelColumnNames.sip
--rw-r--r--   0 runner    (1001) docker     (122)    15545 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IFormatCondition.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5506 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/ITimelineState.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13504 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISparklineGroup.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5092 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelConnection.sip
--rw-r--r--   0 runner    (1001) docker     (122)    30596 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDataLabels.sip
--rw-r--r--   0 runner    (1001) docker     (122)    20253 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/ILines.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IIconSets.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2679 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISlicerItems.sip
--rw-r--r--   0 runner    (1001) docker     (122)    17992 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICellFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    18552 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IControlFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICustomProperties.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3990 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISmartTagOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)    26576 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IEditBox.sip
--rw-r--r--   0 runner    (1001) docker     (122)    22352 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/ILabels.sip
--rw-r--r--   0 runner    (1001) docker     (122)      362 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IOLEObjectEvents.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/ShapeNode.sip
--rw-r--r--   0 runner    (1001) docker     (122)    24888 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IGroupBox.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2906 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISpeech.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8508 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IBorder.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5604 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISmartTag.sip
--rw-r--r--   0 runner    (1001) docker     (122)    10865 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IBorders.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3385 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISparkline.sip
--rw-r--r--   0 runner    (1001) docker     (122)    15948 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/ITextFrame.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2660 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IOLEDBErrors.sip
--rw-r--r--   0 runner    (1001) docker     (122)    34029 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDrawing.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IAreas.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IConnectorFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IRTDUpdateEvent.sip
--rw-r--r--   0 runner    (1001) docker     (122)    30236 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPoint.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2757 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IAllowEditRange.sip
--rw-r--r--   0 runner    (1001) docker     (122)    32412 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IArc.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2870 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IServerViewableItems.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23739 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/DefaultWebOptions.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9865 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IHyperlink.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2668 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IUsedObjects.sip
--rw-r--r--   0 runner    (1001) docker     (122)    23642 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDisplayUnitLabel.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3204 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IIconSet.sip
--rw-r--r--   0 runner    (1001) docker     (122)    13180 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/IAboveAverage.sip
--rw-r--r--   0 runner    (1001) docker     (122)     5536 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IPivotLayout.sip
--rw-r--r--   0 runner    (1001) docker     (122)    11782 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IDisplayFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3397 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/ICustomView.sip
--rw-r--r--   0 runner    (1001) docker     (122)     8353 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IRoutingSlip.sip
--rw-r--r--   0 runner    (1001) docker     (122)    20700 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IPicture.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4118 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IComment.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IChartCategory.sip
--rw-r--r--   0 runner    (1001) docker     (122)     3712 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IColorScaleCriterion.sip
--rw-r--r--   0 runner    (1001) docker     (122)    21352 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IFont.sip
--rw-r--r--   0 runner    (1001) docker     (122)     9656 2023-07-03 13:09:56.605951 pywpsrpc-2.3.8/sip/rpcetapi/CalloutFormat.sip
--rw-r--r--   0 runner    (1001) docker     (122)    12895 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IIconSetCondition.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISparkAxes.sip
--rw-r--r--   0 runner    (1001) docker     (122)     6433 2023-07-03 13:09:56.621951 pywpsrpc-2.3.8/sip/rpcetapi/IValueChange.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2653 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/IRanges.sip
--rw-r--r--   0 runner    (1001) docker     (122)    19554 2023-07-03 13:09:56.617951 pywpsrpc-2.3.8/sip/rpcetapi/ISlicerCache.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2655 2023-07-03 13:09:56.613951 pywpsrpc-2.3.8/sip/rpcetapi/IModelColumnChange.sip
--rw-r--r--   0 runner    (1001) docker     (122)     2803 2023-07-03 13:09:56.609951 pywpsrpc-2.3.8/sip/rpcetapi/IColorStops.sip
--rw-r--r--   0 runner    (1001) docker     (122)     4619 2023-07-03 13:09:56.589950 pywpsrpc-2.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.153828 pywpsrpc-2.3.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     4247 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/README_en.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:07.873812 pywpsrpc-2.3.9/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8455 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/tests/test_rpcetapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10448 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/tests/test_rpcwpsapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1747 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/tests/test_property.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2266 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/tests/test_iter.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1077 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/tests/test_rpcproxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2024 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/tests/test_rpcwppapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10012 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/tests/test_rpcevents.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.049822 pywpsrpc-2.3.9/sip/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:07.905814 pywpsrpc-2.3.9/sip/rpcwppapi/
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/MediaBookmarks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    24699 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/SlideRange.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Research.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ChartCategory.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ColorScheme.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Points.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ChartData.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10998 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/SlideShowTransition.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9707 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Shapes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5765 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ChartCharacters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/_PowerRex.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    19906 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/LegendKey.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1635 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Designs.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1372 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/DocumentWindows.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/PublishObject.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcwppapi/AnimationPoints.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/NamedSlideShow.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/ShapeNodes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6744 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ColorFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/FreeformBuilder.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/SoundEffect.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Tags.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/MediaBookmark.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10469 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ChartFillFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    24353 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ChartTitle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Cell.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/TableBackground.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16153 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/ParagraphFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11241 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/BulletFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    29708 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Point.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    15090 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/MediaFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13897 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/TickLabels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10449 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Effect.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13826 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/PlotArea.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8759 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Hyperlink.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    48135 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/_Application.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3603 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/EApplication.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    29881 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/DataLabels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2130 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/LeaderLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1251 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/RulerLevels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/PrintRanges.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7456 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/Walls.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/SlideNavigation.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4427 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/FilterEffect.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1718 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/SoundFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/DiagramNodeChildren.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23508 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/_Slide.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Guides.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5437 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/HeaderFooter.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/LinkFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Placeholders.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcwppapi/AddIn.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    14553 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/TextEffectFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/FullSeriesCollection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Columns.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/PlaceholderFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1804 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/CellRange.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/PresEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3071 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/ThemeVariant.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3165 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/SetEffect.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7075 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/ResampleMediaTask.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Rows.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7233 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/FileConverter.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Collection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4318 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Options.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/TabStop.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3259 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Sequence.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/TextStyleLevels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7482 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ChartFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)   151504 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/enums.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12749 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/TextRange.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1291 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcwppapi/ActionSettings.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    50088 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/ShapeRange.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8287 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/MotionEffect.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/MasterEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/MouseTracker.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/SeriesCollection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Borders.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1343 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Sequences.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Corners.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12749 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/TextFrame.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    30841 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/ThreeDFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    17226 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ChartFont.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ColorEffect.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5537 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ChartBorder.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcwppapi/Axes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/CategoryCollection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23227 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/FillFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/SeriesLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    40938 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/DataLabel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16987 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/DocumentWindow.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/MouseDownHandler.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3057 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcwppapi/AutoCorrect.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/UpBars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13523 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/_Master.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/CustomerData.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1400 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcwppapi/AddIns.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    20876 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/PrintOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/NamedSlideShows.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3171 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/RulerLevel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3254 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Guide.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Row.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    20848 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/Timing.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcwppapi/Adjustments.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2165 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/TimeLine.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    18857 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/TextFrame2.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16951 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/SlideShowSettings.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Hyperlinks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/Trendlines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7209 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/ScaleEffect.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/TableStyle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Slides.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2746 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/HiLoLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6249 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Floor.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcwppapi/AnimationBehaviors.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10085 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/ProtectedViewWindow.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8101 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Interior.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/PageSetup.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2870 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Player.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3970 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/OLEFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/ResampleMediaTasks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Presentations.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4280 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/CommandEffect.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11283 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ChartArea.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Comments.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4886 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/PropertyEffect.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2596 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Column.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    19994 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Font.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6078 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/EffectInformation.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5392 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/DiagramNode.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/TextStyle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    48185 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Shape.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4904 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Broadcast.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    15806 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/SlideShowView.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8779 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/SlideShowWindow.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/ProtectedViewWindows.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5627 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/rpcwppapi.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    47580 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Axis.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ExtraColors.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5051 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Diagram.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4012 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/RotationEffect.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/Theme.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/TextStyleLevel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Panes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11496 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/PictureFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/TextStyles.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Coauthoring.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2165 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/ShapeNode.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    24352 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/AxisTitle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2042 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Ruler.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3600 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ChartColorFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    28949 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ChartGroup.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/TabStops.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2754 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Gridlines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    57799 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Chart.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/DiagramNodes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    14217 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Table.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/FileConverters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/ThemeVariants.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ColorSchemes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12871 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/ShadowFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6646 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/LegendEntry.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/SldEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Pane.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9663 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/CalloutFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9086 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcwppapi/ActionSetting.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    21610 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/DefaultWebOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10649 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/View.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    18061 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/Trendline.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    49454 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Series.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/CustomLayouts.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5378 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/Selection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4242 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcwppapi/AnimationPoint.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/HeadersFooters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9981 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcwppapi/AnimationBehavior.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3916 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/DownBars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8939 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/DataTable.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    66201 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/_Presentation.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4394 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/CanvasShapes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9102 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/IKRpcClient.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16214 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcwppapi/AnimationSettings.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    14996 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/CustomLayout.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Fonts.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9404 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/PlaySettings.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2736 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/DropLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1263 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/PublishObjects.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5534 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ConnectorFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1990 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ChartGroups.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13651 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Legend.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7096 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/EffectParameters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23115 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/DisplayUnitLabel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1949 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/RGBColor.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3980 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/ErrorBars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/GroupShapes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/ObjectVerbs.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5693 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Design.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1971 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/PrintRange.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    18589 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/LineFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    15599 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwppapi/WebOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/Comment.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/SlideShowWindows.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-07-11 14:15:35.779877 pywpsrpc-2.3.9/sip/rpcwppapi/SectionProperties.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-07-11 14:15:35.775876 pywpsrpc-2.3.9/sip/rpcwppapi/LegendEntries.sip
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:07.989819 pywpsrpc-2.3.9/sip/rpcetapi/
+-rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelColumnChanges.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    20253 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/ILines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4341 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/ICustomProperty.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISlicerCacheLevels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IListRow.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    88556 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/_Chart.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    33599 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IGroupObjects.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IValidation.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11886 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IProtectedViewWindow.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      443 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IRefreshEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7382 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/ICharts.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8499 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IListColumn.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9465 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDataTable.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8353 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IRoutingSlip.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPoints.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3834 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IRecentFiles.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10422 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISmartTagAction.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2659 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IFullSeriesCollection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3909 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IPage.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4174 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IChartColorFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2668 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotItemList.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6041 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IColorStop.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3170 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IXmlSchema.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISeriesCollection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    14448 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITickLabels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    22352 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/ILabels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8469 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/PublishObject.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5199 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelRelationship.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5882 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IFilter.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12243 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IAutoCorrect.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13695 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IToolbarButton.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9375 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IListDataFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    34756 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITextBox.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    21352 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IFont.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IMenuBar.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ShapeNodes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/ColorFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3021 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISparklineGroups.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/WorksheetFunction.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    67483 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/_Worksheet.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3130 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotFields.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      362 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IOLEObjectEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6433 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IValueChange.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2660 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IOLEDBErrors.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IHiLoLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7992 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/Sheets.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2425 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IIcon.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    32875 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotCache.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8490 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelChanges.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IXmlNamespace.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3270 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotLineCells.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6674 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IRectangularGradient.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6678 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISlicerItem.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISparkAxes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23693 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISpinners.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IFileExportConverter.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    73410 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/_IQueryTable.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4325 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/ICustomViews.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23814 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISpellingOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6190 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDiagram.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7622 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITimelineViewState.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2668 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IUsedObjects.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    21580 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/ILine.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2576 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelTableColumn.sip
+-rw-r--r--   0 runner    (1001) docker     (122)   266150 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/_Application.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDialogSheetView.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    18355 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotItem.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2653 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IRanges.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2778 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IToolbars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IErrors.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8508 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IBorder.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2649 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IFilters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5679 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/Solver.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4441 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IUpBars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4554 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IWindows.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7192 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/ILegendEntry.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    15948 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITextFrame.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3712 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IColorScaleCriterion.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2638 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPanes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    19554 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISlicerCache.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    29382 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/ICheckBox.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    29705 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDropDown.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3397 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/ICustomView.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2838 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/DiagramNodeChildren.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    33443 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITextBoxes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IColorScaleCriteria.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2988 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotTableChangeList.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    52088 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDialogSheet.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4367 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISmartTagRecognizer.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3199 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IError.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3799 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/ICalculatedMembers.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    99401 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IRange.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    15545 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IFormatCondition.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDummy.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7080 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISlicerCacheLevel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    14545 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/TextEffectFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8449 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISortField.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6318 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/ICharacters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3612 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotFilters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITableStyleElements.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    48835 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IShape.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    30236 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPoint.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    29512 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IChartGroup.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2724 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IFileExportConverters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    35083 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IGroupObject.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3204 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IIconSet.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITrendlines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2969 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/ICalculatedItems.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8109 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IColorScale.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7660 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IWorksheets.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2788 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IWatches.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5271 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IOutline.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    25007 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISpinner.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    19861 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISlicer.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    14206 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IInterior.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4253 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IOLEDBError.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2088 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/ICorners.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    80561 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/enums.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IMenus.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    60344 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDrawingObjects.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23668 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/ILabel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IMenu.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2771 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IVPageBreaks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16976 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModule.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    97555 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/mso_enum.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDropLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    17992 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/ICellFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    34029 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDrawing.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3222 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IRecentFile.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/TreeviewControl.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2655 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IODBCErrors.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISoundNote.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8974 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IAddIn.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4525 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IErrorBars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3166 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDataBarBorder.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IMenuItems.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10963 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IToolbar.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    28533 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/_IOLEObject.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23642 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDisplayUnitLabel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5659 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDialog.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    32412 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IArc.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IUserAccessList.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16433 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDataFeedConnection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5169 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/INegativeBarFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7491 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IShapes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    24812 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IScrollBars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    14178 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/ILegend.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7979 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IWalls.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IAddIns.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IIconSets.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    73420 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotField.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IListColumns.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    15435 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IXmlMap.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10865 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IBorders.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11782 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDisplayFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISort.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IHeaderFooter.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2673 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13180 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IAboveAverage.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11024 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IChartFillFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelTableNameChanges.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IIconCriteria.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2653 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelColumnName.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    30811 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/ThreeDFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    24841 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IAxisTitle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2757 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IAllowEditRange.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    40150 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IShapeRange.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2672 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/ILeaderLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITableStyleElement.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3069 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISlicers.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8420 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IProtection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    21359 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IODBCConnection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23206 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/FillFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    20700 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPicture.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    26124 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IScrollBar.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2660 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelMeasureName.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3295 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISeriesLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    19651 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPictures.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16411 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IName.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2671 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelTables.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    48093 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IAxis.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotLine.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPublishObjects.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4389 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IAction.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotItems.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2976 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IProtectedViewWindows.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IUserAccess.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IConnectorFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2846 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISlicerPivotTables.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISheetViews.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2950 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IListRows.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    24888 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IGroupBox.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    32524 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDrawings.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IChartView.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IAutoRecover.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1449 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/Adjustments.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    29963 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IOptionButton.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IParameter.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16655 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPlotArea.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    18842 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/TextFrame2.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    37260 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IButtons.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/INames.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    35195 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IOLEDBConnection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10376 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IMailer.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4443 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDownBars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    55522 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IWindow.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IQuickAnalysis.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7059 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotFormula.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7480 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IScenario.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2808 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IXmlMaps.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23576 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IGroupBoxes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)   129982 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/_Workbook.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5604 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISmartTag.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISmartTagActions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IWatch.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2814 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IConditionValue.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotTables.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13781 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IGraphic.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IChartEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    49911 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISeries.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6170 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IFormatColor.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    20544 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IChartObjects.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3990 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISmartTagOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    34758 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IRectangle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IListObjects.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3058 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotCaches.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    31084 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IArcs.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    18552 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IControlFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4623 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelTable.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IAxes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IOLEFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4395 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IVPageBreak.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7385 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModules.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IFormatConditions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IToolbarButtons.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2994 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISortFields.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    27288 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IListBox.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3007 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/CubeFields.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2672 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/ILegendEntries.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    27311 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDropDowns.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5913 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IAppEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IXmlDataBinding.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7999 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IChartFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9953 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IMenuItem.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    14257 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITop10.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/DiagramNode.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IXmlSchemas.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    33446 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IRectangles.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5506 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITimelineState.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8319 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IWorksheetView.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2976 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/ICalculatedFields.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1868 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IFreeformBuilder.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2798 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IAddIns2.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3096 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISlicerCaches.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/ICategoryCollection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelTableNames.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2680 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IStyles.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4118 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IComment.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IRTDUpdateEvent.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2658 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IActions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12895 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IIconSetCondition.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    28070 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/ICheckBoxes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2701 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelTableColumns.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10560 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotFilter.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11318 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotCell.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDocEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/ILegendKey.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12491 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IWorkbookConnection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11495 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/PictureFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    30596 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDataLabels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2696 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelColumnNames.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3385 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISparkline.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IAutoFilter.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    26233 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITextConnection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ShapeNode.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10966 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IUniqueValues.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7713 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/Workbooks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    33520 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IOval.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3956 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISparkHorizontalAxis.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6778 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IFloor.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4917 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IMultiThreadedCalculation.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISmartTagRecognizers.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IGroupShapes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    18605 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITrendline.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3382 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IXmlNamespaces.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4977 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISparkPoints.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2939 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotFormulas.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5254 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IIconCriterion.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    15346 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IErrorCheckingOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    22458 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/rpcetapi.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/DiagramNodes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4395 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IHPageBreak.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      896 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IRtdServer.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    21372 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IOLEObjects.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12865 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ShadowFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IQueryTables.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1527 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IRTD.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IPages.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    24842 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IChartTitle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8872 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPhonetics.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5092 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelConnection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6433 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISparkVerticalAxis.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISparkColor.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2803 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IColorStops.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IAreas.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IComments.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotValueCell.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9656 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/CalloutFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10165 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITableStyle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2906 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISpeech.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDialogs.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    22797 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IChartObject.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    14286 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDialogFrame.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IGridlines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5770 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IPane.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2990 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IHyperlinks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23739 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/DefaultWebOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2775 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITableStyles.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    17977 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDatabar.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13504 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ISparklineGroup.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotAxis.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2405 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISmartTags.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IChartCategory.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    24803 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IEditBoxes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)   120586 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotTable.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4001 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IXPath.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    26576 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IEditBox.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    50185 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IPageSetup.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7423 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IKRpcClient.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13376 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITableObject.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2701 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelMeasureNames.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4479 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IWorksheetDataConnection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2771 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IHPageBreaks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IODBCError.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/ILinearGradient.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    29903 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IListObject.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13020 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IChartArea.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    24844 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IListBoxes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2563 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IChartGroups.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2688 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelTableNameChange.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IResearch.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2679 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/ISlicerItems.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IAllowEditRanges.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    28654 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IOptionButtons.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IScenarios.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7398 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDialogSheets.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2778 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IMenuBars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3675 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IConnections.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    41429 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/IDataLabel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModuleView.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11929 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/ICalculatedMember.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4449 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IWorkbookEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2848 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IParameters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    28998 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/IStyle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/ICanvasShapes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2870 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IServerViewableItems.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9865 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IHyperlink.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    32203 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IOvals.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    28901 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/CubeField.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2655 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelColumnChange.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6460 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPhonetic.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/_DebugTools.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3833 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/ILinkFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-07-11 14:15:35.755875 pywpsrpc-2.3.9/sip/rpcetapi/ICustomProperties.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    38575 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/rpcetapi/IButton.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2880 2023-07-11 14:15:35.759875 pywpsrpc-2.3.9/sip/rpcetapi/IModelRelationships.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5536 2023-07-11 14:15:35.763876 pywpsrpc-2.3.9/sip/rpcetapi/IPivotLayout.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    18573 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/LineFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    15372 2023-07-11 14:15:35.771876 pywpsrpc-2.3.9/sip/rpcetapi/WebOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-07-11 14:15:35.767876 pywpsrpc-2.3.9/sip/rpcetapi/ITab.sip
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.049822 pywpsrpc-2.3.9/sip/rpcwpsapi/
+-rw-r--r--   0 runner    (1001) docker     (122)     1997 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/ReadabilityStatistic.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TableOfAuthoritiesCategory.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/ListEntries.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Research.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3373 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTagType.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/HangulAndAlphabetExceptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/ChartCategory.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2571 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathScrPre.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/ContentControlListEntry.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6656 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Section.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Points.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5689 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Dictionary.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/MailMessage.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMaths.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/ChartData.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7917 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Shapes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5162 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/ChartCharacters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4584 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathAutoCorrect.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    19328 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/LegendKey.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/HangulAndAlphabetException.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3186 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Category.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3091 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/SoftEdgeFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Editors.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2036 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTagTypes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathAcc.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Break.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/FirstLetterExceptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/ShapeNodes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13930 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/ColorFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/FreeformBuilder.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/EmailSignatureEntries.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4442 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/List.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2068 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTagRecognizers.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9870 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/ChartFillFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23740 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/ChartTitle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23358 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Cell.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2079 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathArgs.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3458 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Fields.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2750 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Bibliography.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTag.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2018 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/MailMergeDataFields.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8925 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/XMLSchemaReferences.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/XMLChildNodeSuggestion.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    28848 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Point.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/BuildingBlockType.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8915 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/MailingLabel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4369 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TablesOfAuthorities.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7313 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Shading.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Templates.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/CoAuthors.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13304 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TickLabels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2090 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Frames.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13210 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/PlotArea.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TwoInitialCapsException.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Reviewers.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12355 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/Hyperlink.sip
+-rw-r--r--   0 runner    (1001) docker     (122)   119902 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/sip/rpcwpsapi/_Application.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6807 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/FootnoteOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TextColumn.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TaskPane.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9418 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/ConditionalStyle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1966 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/XSLTransform.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    29309 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/DataLabels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3946 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathScrSubSup.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/LeaderLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4318 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/IApplicationEvents4.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6053 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Revision.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathAutoCorrectEntries.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8152 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathNary.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6824 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Walls.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/ContentControls.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/ListTemplates.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/InlineShapes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/AutoTextEntries.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TablesOfContents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/DiagramNodeChildren.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/XMLNamespaces.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/XMLChildNodeSuggestions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6214 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/HeaderFooter.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4824 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathBox.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7896 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/DocumentField.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TaskPanes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5661 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/EndnoteOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2594 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/ProofreadingErrors.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathFunc.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7587 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/LinkFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10595 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTagAction.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6055 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Bookmark.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4985 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/AddIn.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    15033 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TextEffectFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1476 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/FullSeriesCollection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2203 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/XSLTransforms.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9263 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Columns.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4534 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/KeysBoundTo.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/CoAuthor.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10365 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/sip/rpcwpsapi/rpcwpsapi.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8592 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/Language.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2027 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/MappedDataFields.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/KeyBindings.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    27619 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Rows.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/Lines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/AutoCaptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8764 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/CaptionLabel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Characters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2091 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/CaptionLabels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6142 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/FileConverter.sip
+-rw-r--r--   0 runner    (1001) docker     (122)   325888 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Options.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TabStop.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2105 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Tasks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4139 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Dialog.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    54770 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Paragraph.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12132 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Cells.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    14664 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TableOfAuthorities.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10262 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathMat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/ListGalleries.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6788 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/ChartFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathMatCols.sip
+-rw-r--r--   0 runner    (1001) docker     (122)   139181 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/sip/rpcwpsapi/enums.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/CoAuthUpdates.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Styles.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5020 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Subdocument.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/Lists.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Endnote.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Browser.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/sip/rpcwpsapi/_Application_extend.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3202 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathMatCol.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    51599 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/ShapeRange.sip
+-rw-r--r--   0 runner    (1001) docker     (122)   100162 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/sip/rpcwpsapi/mso_enum.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11370 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Field.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4734 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/Line.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6562 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/LineNumbering.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Breaks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4900 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/Indexes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Zooms.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/XMLMapping.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathMatRows.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3098 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Variable.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9038 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Endnotes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/BuildingBlocks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4759 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TablesOfFigures.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3211 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/RevisionsFilter.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7323 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/HTMLDivision.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16323 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/XMLNode.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Conflicts.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2027 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/OtherCorrectionsException.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/SeriesCollection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/BuildingBlockEntries.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    28828 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Borders.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathLimLow.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Pages.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Email.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/CustomLabels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2018 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/MailMergeFieldNames.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5489 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/StyleSheet.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathRecognizedFunction.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Variables.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8302 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathPhantom.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      903 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Corners.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    21304 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TextFrame.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3926 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/ListTemplate.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/HTMLDivisions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/CoAuthUpdate.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    20460 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/MailMerge.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/XMLNodes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7268 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathEqArray.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    31043 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/ThreeDFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16641 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/ChartFont.sip
+-rw-r--r--   0 runner    (1001) docker     (122)   217343 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/sip/rpcwpsapi/_Document.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    47873 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/sip/rpcwpsapi/_ParagraphFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2113 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/HeadingStyles.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    15834 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/MailMergeDataSource.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2033 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/FontNames.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Reviewer.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    38309 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/sip/rpcwpsapi/_LetterContent.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    28414 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Style.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Dialogs.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10774 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathBorderBox.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4932 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/ChartBorder.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2960 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/XMLNamespace.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Axes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Subdocuments.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/CategoryCollection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    40027 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Envelope.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    22425 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/FillFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2130 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/SeriesLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5305 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Zoom.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    95513 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Range.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    40355 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/DataLabel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4380 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/AutoCaption.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/Languages.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Revisions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/ReflectionFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5998 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/CheckBox.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    22585 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/AutoCorrect.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathBar.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3280 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/UpBars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2027 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathMatRow.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2188 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/AddIns.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4783 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathGroupChar.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    14075 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathFunction.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4652 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Bookmarks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16911 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Row.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2201 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/CoAuthLocks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5071 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TextInput.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13916 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/CustomLabel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    55715 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/sip/rpcwpsapi/_Font.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    17982 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Frame.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Adjustments.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/ListParagraphs.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10619 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Replacement.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/CoAuthLock.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7493 2023-07-11 14:15:35.803878 pywpsrpc-2.3.9/sip/rpcwpsapi/_OLEControl.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10873 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/System.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3238 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Editor.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4302 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/AutoCorrectEntry.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/Hyperlinks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Trendlines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3244 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Version.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2696 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/SpellingSuggestions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16566 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TableStyle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/HiLoLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTagActions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4744 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Rectangle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/StoryRanges.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    42752 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Window.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/ContentControlListEntries.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Floor.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTags.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11815 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/ProtectedViewWindow.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7500 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/Interior.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    40169 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/PageSetup.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8731 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/ListFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10792 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OLEFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16698 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TableOfFigures.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TwoInitialCapsExceptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10658 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/ChartArea.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathBreaks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3246 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Versions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3785 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTagRecognizer.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Comments.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3204 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/RecentFiles.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Rectangles.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2807 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Source.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3103 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathRad.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8381 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Task.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2536 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/EmailSignatureEntry.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11141 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Column.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5635 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/CoAuthoring.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    26013 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/InlineShape.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6076 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/DiagramNode.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/XMLSchemaReference.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4207 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/DropDown.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/IApplicationEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/SynonymInfo.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TablesOfAuthoritiesCategories.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1429 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/IApplicationEvents2.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4085 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/EmailSignature.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    55364 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Shape.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4188 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Broadcast.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/EmailAuthor.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4374 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Sections.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2627 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Conflict.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/ProtectedViewWindows.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9048 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Footnotes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3257 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/FormFields.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/RepeatingSectionItem.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2022 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/FirstLetterException.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    47032 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Axis.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5626 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Diagram.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8768 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/RoutingSlip.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2576 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Footnote.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2075 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Panes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12470 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/PictureFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathScrSup.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathRecognizedFunctions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/ListEntry.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5547 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/DropCap.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/ShapeNode.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23739 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/AxisTitle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11461 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMath.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2020 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Sources.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    14376 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TableOfContents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/MailMergeFields.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    48838 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/EmailOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/ChartColorFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12249 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/Index.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3773 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Windows.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/StyleSheets.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    28387 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/ChartGroup.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9480 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Border.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2949 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/UndoRecord.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TabStops.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2781 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/PageNumber.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    30449 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/ContentControl.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/Gridlines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    53164 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Chart.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/DiagramNodes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    33505 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Table.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3354 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/FileConverters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12834 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/ShadowFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2026 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/ReadabilityStatistics.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6035 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/LegendEntry.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7768 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/BuildingBlock.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/RepeatingSectionItemColl.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4991 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/MailMergeField.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2223 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathFunctions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5872 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/KeyBinding.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7893 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TextColumns.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    14707 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Pane.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6958 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Documents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10237 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/CalloutFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3055 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Words.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/MappedDataField.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16500 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/FormField.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    18233 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/OfdExportOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathScrSub.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    22121 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/DefaultWebOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    76697 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/View.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    17491 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Trendline.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    48635 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Series.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/OtherCorrectionsExceptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/DocumentFields.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    73015 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Selection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3814 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/RecentFile.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/HeadersFooters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3675 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/GlowFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathFrac.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/ListLevels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1979 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/Categories.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3282 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/DownBars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8324 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/DataTable.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4356 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/AutoTextEntry.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/CanvasShapes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/BuildingBlockTypes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8731 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/IKRpcClient.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathAutoCorrectEntry.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2271 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/AutoCorrectEntries.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12216 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/PageNumbers.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4618 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/HangulHanjaConversionDictionaries.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9316 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathDelim.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathLimUpp.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16906 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/PdfExportOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/CustomProperties.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/DropLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3059 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Sentences.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/MailMergeDataField.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8578 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/Mailer.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1981 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/MailMergeFieldName.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6088 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/ConnectorFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-11 14:15:35.783877 pywpsrpc-2.3.9/sip/rpcwpsapi/ChartGroups.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5679 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/HorizontalLineFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/ListGallery.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13054 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/Legend.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8833 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/WrapFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Tables.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23746 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/DisplayUnitLabel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1449 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/SpellingSuggestion.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5176 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/TextRetrievalMode.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    43114 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Find.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4886 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Page.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3365 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/ErrorBars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2074 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/GroupShapes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3958 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Dictionaries.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/CustomProperty.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    17342 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Frameset.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2543 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/OMathBreak.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/IApplicationEvents3.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    17841 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/LineFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    14778 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/WebOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10554 2023-07-11 14:15:35.787877 pywpsrpc-2.3.9/sip/rpcwpsapi/Comment.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    47441 2023-07-11 14:15:35.795877 pywpsrpc-2.3.9/sip/rpcwpsapi/Paragraphs.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3114 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/HeadingStyle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16164 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/ListLevel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    20665 2023-07-11 14:15:35.799878 pywpsrpc-2.3.9/sip/rpcwpsapi/Template.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1489 2023-07-11 14:15:35.791877 pywpsrpc-2.3.9/sip/rpcwpsapi/LegendEntries.sip
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.089825 pywpsrpc-2.3.9/sip/common/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.089825 pywpsrpc-2.3.9/sip/common/ksoapi/
+-rw-r--r--   0 runner    (1001) docker     (122)     1453 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/FileDialogSelectedItems.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5068 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/IAccessible.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/Points.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoDropLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9649 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/WebComponentProperties.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    47649 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoAxis.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6780 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/Shapes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3739 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SignatureSet.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9509 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/Crop.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10647 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/Signature.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      362 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/ICommandBarComboBoxEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2500 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SoftEdgeFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SmartDocument.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2275 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceFolders.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6207 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceLink.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/CustomXMLPrefixMapping.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      905 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoCorners.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1990 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/EffectParameter.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/ICustomXMLPartEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/ShapeNodes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6644 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/ColorFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/FreeformBuilder.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6113 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/MsoDebugOptions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5119 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/WebPageFont.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/NewFile.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/FileDialogFilter.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10679 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SignatureSetup.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/Sync.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/PropertyTest.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IRibbonControl.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3589 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/PickerDialog.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/DocumentInspector.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_CommandBarComboBoxEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9139 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/ChartFillFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2057 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/PickerField.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/GridLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8387 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoDataTable.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SearchScope.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/CustomXMLPrefixMappings.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4860 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/COMAddIn.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8723 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/ILicAgent.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_CommandBarButtonEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2096 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/ScopeFolder.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      481 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/CustomTaskPaneEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/HTMLProject.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12543 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/CustomXMLNode.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/BalloonLabel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13224 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoPlotArea.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/ThemeEffectScheme.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2608 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtQuickStyle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2800 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/WebComponentWindowExternal.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/ODSOColumn.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23779 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoChartTitle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/ContactCard.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/COMAddIns.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13312 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoTickLabels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/IConverterApplicationPreferences.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2836 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/DiagramNodeChildren.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/DocumentLibraryVersion.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    20591 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/ParagraphFormat2.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5066 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoDiagram.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1419 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/DocumentInspectors.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5139 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/MetaProperty.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    14564 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/TextEffectFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/FullSeriesCollection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceMember.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1408 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SearchScopes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6841 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoChartFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/PropertyTests.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2608 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtColor.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6024 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/Script.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3676 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/BalloonCheckbox.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/ICTPFactory.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoAxisTitle.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1420 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/HTMLProjectItems.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5550 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/WorkflowTask.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoEnvelopeVBEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      616 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/IAssistance.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SearchFolders.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      270 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_CommandBarsEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/MsoDebugOptions_UT.sip
+-rw-r--r--   0 runner    (1001) docker     (122)   106390 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/enums.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3686 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/TextColumn2.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/IConverter.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SignatureProvider.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/ThemeFontScheme.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    40062 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/ShapeRange.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1629 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/CustomXMLValidationErrors.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23739 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/CommandBarControl.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/ICommandBarsEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6319 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/DocumentProperty.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3326 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoUpBars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5589 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/ILicWizExternal.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/PolicyItem.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/IFoundFiles.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/WorkflowTemplate.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SeriesCollection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5149 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoCharacters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2570 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/RulerLevel2.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3423 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceFile.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    40350 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoDataLabel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4387 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/ServerPolicy.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/ThemeColorScheme.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/PickerFields.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoEnvelopeVB.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    60888 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoChart.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/MsoDebugOptions_UTRunResult.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6090 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/TextFrame.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/ODSOFilters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtQuickStyles.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    30852 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/ThreeDFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    16641 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/ChartFont.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2321 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceMembers.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5665 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoFloor.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/IBlogPictureExtensibility.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoSeriesLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    17493 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoTrendline.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1716 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/FileDialogFilters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/Axes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoHiLoLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1512 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/CategoryCollection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    23206 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/FillFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_CustomXMLParts.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/CustomXMLNodes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    26769 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/Assistant.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/GradientStops.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5792 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/ReflectionFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2001 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/ILicValidator.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1421 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtLayouts.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoErrorBars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13063 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoLegend.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1397 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/RulerLevels2.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/TabStop2.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceTasks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6671 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_CustomXMLPart.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7714 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspace.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1451 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/sip/common/ksoapi/Adjustments.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/MetaProperties.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    18820 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/TextFrame2.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10353 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_CommandBarButton.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9967 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/FileDialog.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_CustomTaskPaneEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtNode.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    25448 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/IFind.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1674 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/PickerResults.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8651 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_CommandBarComboBox.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/Trendlines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_CommandBarActiveX.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/FoundFiles.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/LanguageSettings.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/ODSOColumns.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      718 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IRibbonUI.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/sip/common/ksoapi/AnswerWizardFiles.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/PictureEffects.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6900 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/WebComponentFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/IDocumentInspector.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2274 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/OfficeTheme.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtLayout.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoHyperlinks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoLeaderLines.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/IConverterPreferences.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/ICustomTaskPaneConsumer.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceLinks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13472 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/FileSearch.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5415 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/DiagramNode.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    29151 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/ChartPoint.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/CommandBarControls.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3268 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/CustomXMLValidationError.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtNodes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/CustomXMLSchema.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/GradientStop.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6083 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/OfficeDataSourceObject.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoEServicesDialog.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/Permission.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    39775 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/Shape.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceFolder.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9965 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceTask.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    28720 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoChartGroup.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2274 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/MsoDebugOptions_UTManager.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11491 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/PictureFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3837 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/PictureEffect.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11921 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoChartArea.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6376 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/WebComponent.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/ODSOFilter.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoDownBars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/ShapeNode.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/UserPermission.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_CustomXMLPartEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7504 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoInterior.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoDisplayUnitLabel.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/PickerProperties.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3495 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/ChartColorFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6094 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SmartArt.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/Scripts.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/DocumentLibraryVersions.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1419 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/WorkflowTemplates.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1441 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/DiagramNodes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12882 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/ShadowFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6057 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/LegendEntry.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2188 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoContactCard.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/ThemeFont.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    19427 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/CommandBar.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IRibbonExtensibility.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    29490 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoDataLabels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9674 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/CalloutFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/WorkflowTasks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoCategory.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1408 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/ThemeFonts.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_IMsoDispObj.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/WebPageFonts.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2791 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/HTMLProjectItem.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2470 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/BalloonCheckboxes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1552 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/FileTypes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_CommandBars.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/GlowFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4405 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/CanvasShapes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/sip/common/ksoapi/AnswerWizard.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/ScopeFolders.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1975 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_CustomXMLSchemaCollection.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/IBlogExtensibility.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2691 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/TabStops2.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     5545 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/ConnectorFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/ThemeColor.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12409 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/Balloon.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/ChartGroups.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_IMsoOleAccDispObj.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/IConverterUICallback.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/EffectParameters.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1963 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/MsoDebugOptions_UTs.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1800 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/DocumentProperties.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/CommandBarPopup.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    48908 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoSeries.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/ICustomXMLPartsEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     8339 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/PickerResult.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/GroupShapes.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/Ruler2.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    19328 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoLegendKey.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4931 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoBorder.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    11340 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/TextRange2.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2375 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceFiles.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     6868 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoWalls.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/BalloonLabels.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoChartData.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1416 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtColors.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    33720 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/Font2.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10630 2023-07-11 14:15:35.731874 pywpsrpc-2.3.9/sip/common/ksoapi/BulletFormat2.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_CustomXMLPartsEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1629 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/EncryptionProvider.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-11 14:15:35.735874 pywpsrpc-2.3.9/sip/common/ksoapi/ICommandBarButtonEvents.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    18600 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/LineFormat.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     7922 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/ksoapi/_CustomTaskPane.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2036 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/PickerProperty.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    10003 2023-07-11 14:15:35.743875 pywpsrpc-2.3.9/sip/common/ksoapi/SignatureInfo.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/LegendEntries.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-07-11 14:15:35.739874 pywpsrpc-2.3.9/sip/common/ksoapi/IMsoDispCagNotifySink.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9635 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/sip/common/common.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     9598 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/sip/common/ksoapi.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3473 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/objbase.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1855 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/sip/common/guid.sip
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.093825 pywpsrpc-2.3.9/sip/common/wpsapiex/
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/EtRangeEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/common/wpsapiex/_WpsApplicationEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1922 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/WorkbooksEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/common/wpsapiex/_PresentationEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/common/wpsapiex/_WorkbookEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/WpsApplicationEventsEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/Headings.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/WpsCloudService.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/common/wpsapiex/enums.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      402 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/KsoDocumentEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/HeaderFooterEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/common/wpsapiex/_WppApplicationEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/Heading.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/PrintoutPageEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    13151 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/WaterMark.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/common/wpsapiex/_DocumentEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/ApplicationEventsEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1160 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/DocumentsEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/WppApplicationEventsEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      871 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/PictureFormatEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1870 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/WaterMarks.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1573 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/common/wpsapiex/_EtApplicationEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/RangeEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/PresentationsEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/wpsapiex/EtApplicationEventsEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4179 2023-07-11 14:15:35.751875 pywpsrpc-2.3.9/sip/common/wpsapiex/_ApplicationEx.sip
+-rw-r--r--   0 runner    (1001) docker     (122)    12256 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/oaidl.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/sip/common/export.sip
+-rw-r--r--   0 runner    (1001) docker     (122)     4132 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/typedef.sip
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-11 14:15:35.747875 pywpsrpc-2.3.9/sip/common/objidl.sip
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.125827 pywpsrpc-2.3.9/wpsrpc-sdk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.097825 pywpsrpc-2.3.9/wpsrpc-sdk/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.093825 pywpsrpc-2.3.9/wpsrpc-sdk/tests/et/
+-rw-r--r--   0 runner    (1001) docker     (122)     3343 2023-07-11 14:15:36.991960 pywpsrpc-2.3.9/wpsrpc-sdk/tests/et/rangevalue.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-11 14:15:36.991960 pywpsrpc-2.3.9/wpsrpc-sdk/tests/et/pch.h
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-07-11 14:15:36.991960 pywpsrpc-2.3.9/wpsrpc-sdk/tests/et/testetbase.h
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-07-11 14:15:36.991960 pywpsrpc-2.3.9/wpsrpc-sdk/tests/et/testetbase.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-07-11 14:15:36.991960 pywpsrpc-2.3.9/wpsrpc-sdk/tests/et/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.097825 pywpsrpc-2.3.9/wpsrpc-sdk/tests/wps/
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-11 14:15:36.991960 pywpsrpc-2.3.9/wpsrpc-sdk/tests/wps/pch.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1254 2023-07-11 14:15:36.991960 pywpsrpc-2.3.9/wpsrpc-sdk/tests/wps/comparedocs.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-07-11 14:15:36.991960 pywpsrpc-2.3.9/wpsrpc-sdk/tests/wps/testbase.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-07-11 14:15:36.991960 pywpsrpc-2.3.9/wpsrpc-sdk/tests/wps/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-07-11 14:15:36.991960 pywpsrpc-2.3.9/wpsrpc-sdk/tests/wps/testbase.h
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-11 14:15:36.991960 pywpsrpc-2.3.9/wpsrpc-sdk/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.097825 pywpsrpc-2.3.9/wpsrpc-sdk/tests/wpp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 14:15:36.991960 pywpsrpc-2.3.9/wpsrpc-sdk/tests/wpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-07-11 14:15:36.779944 pywpsrpc-2.3.9/wpsrpc-sdk/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.117826 pywpsrpc-2.3.9/wpsrpc-sdk/include/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.097825 pywpsrpc-2.3.9/wpsrpc-sdk/include/et/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.097825 pywpsrpc-2.3.9/wpsrpc-sdk/include/et/etapi/
+-rw-r--r--   0 runner    (1001) docker     (122)    60121 2023-07-11 14:15:36.839949 pywpsrpc-2.3.9/wpsrpc-sdk/include/et/etapi/etapi_predef.h
+-rw-r--r--   0 runner    (1001) docker     (122)  7872505 2023-07-11 14:15:36.839949 pywpsrpc-2.3.9/wpsrpc-sdk/include/et/etapi/etapi.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-07-11 14:15:36.815947 pywpsrpc-2.3.9/wpsrpc-sdk/include/et/etapi.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.105826 pywpsrpc-2.3.9/wpsrpc-sdk/include/wps/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.105826 pywpsrpc-2.3.9/wpsrpc-sdk/include/wps/wpsapi/
+-rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-07-11 14:15:36.851949 pywpsrpc-2.3.9/wpsrpc-sdk/include/wps/wpsapi/wpsapi_extend.h
+-rw-r--r--   0 runner    (1001) docker     (122)    31992 2023-07-11 14:15:36.847949 pywpsrpc-2.3.9/wpsrpc-sdk/include/wps/wpsapi/undefs.h
+-rw-r--r--   0 runner    (1001) docker     (122)  5632109 2023-07-11 14:15:36.851949 pywpsrpc-2.3.9/wpsrpc-sdk/include/wps/wpsapi/wpsapi.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3631 2023-07-11 14:15:36.843949 pywpsrpc-2.3.9/wpsrpc-sdk/include/wps/wpsapi.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.113826 pywpsrpc-2.3.9/wpsrpc-sdk/include/wpp/
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-07-11 14:15:36.839949 pywpsrpc-2.3.9/wpsrpc-sdk/include/wpp/wppapi.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.117826 pywpsrpc-2.3.9/wpsrpc-sdk/include/wpp/wppapi/
+-rw-r--r--   0 runner    (1001) docker     (122)  2528680 2023-07-11 14:15:36.843949 pywpsrpc-2.3.9/wpsrpc-sdk/include/wpp/wppapi/wppapi.h
+-rw-r--r--   0 runner    (1001) docker     (122)    19534 2023-07-11 14:15:36.843949 pywpsrpc-2.3.9/wpsrpc-sdk/include/wpp/wppapi/wppapi_predef.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.125827 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.121827 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/ksoapi/
+-rw-r--r--   0 runner    (1001) docker     (122)  2707437 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/ksoapi/ksoapi.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6249 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/objbase.h
+-rw-r--r--   0 runner    (1001) docker     (122)    18463 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/variant.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.125827 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/kfc/
+-rw-r--r--   0 runner    (1001) docker     (122)     9916 2023-07-11 14:15:36.779944 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/kfc/comsptr.h
+-rw-r--r--   0 runner    (1001) docker     (122)   272970 2023-07-11 14:15:36.779944 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/kfc/errno.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4508 2023-07-11 14:15:36.779944 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/kfc/guid.h
+-rw-r--r--   0 runner    (1001) docker     (122)    17797 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/pre_stdlib.h
+-rw-r--r--   0 runner    (1001) docker     (122)    11017 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/winnt.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7761 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/pre_platform.h
+-rw-r--r--   0 runner    (1001) docker     (122)    87307 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/mso_enum.h
+-rw-r--r--   0 runner    (1001) docker     (122)     9234 2023-07-11 14:15:36.779944 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/comdef.h
+-rw-r--r--   0 runner    (1001) docker     (122)    11329 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/typedef.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3991 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/mso_enum_chart.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2587 2023-07-11 14:15:36.815947 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/wpsrpcsdk.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/wpsapiex.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6630 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/winuser.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.125827 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/wpsapiex/
+-rw-r--r--   0 runner    (1001) docker     (122)   143565 2023-07-11 14:15:36.815947 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/wpsapiex/wpsapiex.h
+-rw-r--r--   0 runner    (1001) docker     (122)    18227 2023-07-11 14:15:36.779944 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/int.h
+-rw-r--r--   0 runner    (1001) docker     (122)    27859 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/oaidl.h
+-rw-r--r--   0 runner    (1001) docker     (122)    33561 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/objidl.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8453 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/pre_stddef.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.125827 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/strapi/
+-rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/strapi/strapi.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.125827 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/strapi/strapi/
+-rw-r--r--   0 runner    (1001) docker     (122)     6232 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/strapi/strapi/wchar.h
+-rw-r--r--   0 runner    (1001) docker     (122)    13826 2023-07-11 14:15:36.811946 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/oleauto.h
+-rw-r--r--   0 runner    (1001) docker     (122)    12667 2023-07-11 14:15:36.779944 pywpsrpc-2.3.9/wpsrpc-sdk/include/common/guiddef.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-07-11 14:15:36.775944 pywpsrpc-2.3.9/wpsrpc-sdk/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-11 14:15:36.775944 pywpsrpc-2.3.9/wpsrpc-sdk/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.125827 pywpsrpc-2.3.9/wpsrpc-sdk/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.141828 pywpsrpc-2.3.9/wpsrpc-sdk/lib/x86_64/
+-rwxr-xr-x   0 runner    (1001) docker     (122)  6158464 2023-07-11 14:15:36.979959 pywpsrpc-2.3.9/wpsrpc-sdk/lib/x86_64/librpcwppapi_sysqt5.so
+-rwxr-xr-x   0 runner    (1001) docker     (122)  9157384 2023-07-11 14:15:36.991960 pywpsrpc-2.3.9/wpsrpc-sdk/lib/x86_64/librpcwpsapi_sysqt5.so
+-rwxr-xr-x   0 runner    (1001) docker     (122) 10074176 2023-07-11 14:15:36.923955 pywpsrpc-2.3.9/wpsrpc-sdk/lib/x86_64/librpcetapi_sysqt5.so
+-rw-r--r--   0 runner    (1001) docker     (122)     4619 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.153828 pywpsrpc-2.3.9/include/
+-rw-r--r--   0 runner    (1001) docker     (122)     3962 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/include/pyevents.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.153828 pywpsrpc-2.3.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.153828 pywpsrpc-2.3.9/examples/rpcwppapi/
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/examples/rpcwppapi/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3399 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/examples/rpcwppapi/wpp_convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.153828 pywpsrpc-2.3.9/examples/rpcetapi/
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/examples/rpcetapi/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3287 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/examples/rpcetapi/et_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.153828 pywpsrpc-2.3.9/examples/rpcwpsapi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.153828 pywpsrpc-2.3.9/examples/rpcwpsapi/convertto/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3121 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/examples/rpcwpsapi/convertto/convertto.py
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/examples/rpcwpsapi/convertto/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.153828 pywpsrpc-2.3.9/examples/rpcwpsapi/embedded/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/examples/rpcwpsapi/embedded/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6416 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/examples/rpcwpsapi/embedded/demo.py
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     4916 2023-07-11 14:16:08.157829 pywpsrpc-2.3.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 14:16:08.153828 pywpsrpc-2.3.9/py/
+-rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/py/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    18708 2023-07-11 14:15:35.727874 pywpsrpc-2.3.9/project.py
```

### Comparing `pywpsrpc-2.3.8/pyproject.toml` & `pywpsrpc-2.3.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["sip >=6"]
 build-backend = "sipbuild.api"
 
 [tool.sip.metadata]
 name = "pywpsrpc"
-version = "2.3.8"
+version = "2.3.9"
 summary = "Python bindings for the WPS Office RPC"
 home-page = "https://github.com/timxx/pywpsrpc"
 author = "Weitian Leung"
 author-email = "weitianleung@gmail.com"
 license = "MIT"
 description-file = "README.md"
 description-content-type = "text/markdown"
```

### Comparing `pywpsrpc-2.3.8/PKG-INFO` & `pywpsrpc-2.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywpsrpc
-Version: 2.3.8
+Version: 2.3.9
 Requires-Python: >=3.6
 Summary: Python bindings for the WPS Office RPC
 Home-Page: https://github.com/timxx/pywpsrpc
 Author: Weitian Leung
 Author-Email: weitianleung@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `pywpsrpc-2.3.8/examples/rpcwpsapi/convertto/convertto.py` & `pywpsrpc-2.3.9/examples/rpcwpsapi/convertto/convertto.py`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/examples/rpcwpsapi/embedded/demo.py` & `pywpsrpc-2.3.9/examples/rpcwpsapi/embedded/demo.py`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/examples/rpcwppapi/wpp_convert.py` & `pywpsrpc-2.3.9/examples/rpcwppapi/wpp_convert.py`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/examples/rpcetapi/et_convert.py` & `pywpsrpc-2.3.9/examples/rpcetapi/et_convert.py`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/README_en.md` & `pywpsrpc-2.3.9/README_en.md`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/LICENSE` & `pywpsrpc-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/include/pyevents.h` & `pywpsrpc-2.3.9/include/pyevents.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/tests/test_rpcproxy.py` & `pywpsrpc-2.3.9/tests/test_rpcproxy.py`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/tests/test_rpcetapi.py` & `pywpsrpc-2.3.9/tests/test_rpcetapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -247,12 +247,24 @@
 
         self.assertEqual(pivotfields[1].Name, "Product")
         self.assertEqual(pivotfields[2].Name, "Sales")
 
         # the wizard create the pivottable in another sheet...
         self.assertEqual(workbook.Sheets[1].PivotTables()[1].Count, 1)
 
+        hr, pivotitems = pivotfields[1].PivotItems()
+        self.assertEqual(hr, common.S_OK)
+        self.assertIsNotNone(pivotitems)
+
+        self.assertTrue(pivotitems.Count > 0)
+
+        pivotitem = pivotitems[1]
+        self.assertIsNotNone(pivotitem)
+
+        self.assertEqual(pivotitem.Visible, True)
+        self.assertEqual(pivotitem.Name, "a")
+
         workbook.Close(False)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pywpsrpc-2.3.8/tests/test_iter.py` & `pywpsrpc-2.3.9/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/tests/test_rpcwppapi.py` & `pywpsrpc-2.3.9/tests/test_rpcwppapi.py`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/tests/test_rpcevents.py` & `pywpsrpc-2.3.9/tests/test_rpcevents.py`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/tests/test_property.py` & `pywpsrpc-2.3.9/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/tests/test_rpcwpsapi.py` & `pywpsrpc-2.3.9/tests/test_rpcwpsapi.py`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/py/utils.py` & `pywpsrpc-2.3.9/py/utils.py`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/project.py` & `pywpsrpc-2.3.9/project.py`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/CMakeLists.txt` & `pywpsrpc-2.3.9/wpsrpc-sdk/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/kfc/guid.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/kfc/guid.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/kfc/comsptr.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/kfc/comsptr.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/kfc/errno.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/kfc/errno.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/pre_platform.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/pre_platform.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/pre_stdlib.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/pre_stdlib.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/int.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/int.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/wpsapiex/wpsapiex.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/wpsapiex/wpsapiex.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/wpsrpcsdk.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/wpsrpcsdk.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/comdef.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/comdef.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/winuser.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/winuser.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/wpsapiex.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/wpsapiex.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/mso_enum_chart.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/mso_enum_chart.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/guiddef.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/guiddef.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/objbase.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/objbase.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/pre_stddef.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/pre_stddef.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/oleauto.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/oleauto.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/typedef.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/typedef.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/oaidl.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/oaidl.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/ksoapi/ksoapi.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/ksoapi/ksoapi.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/winnt.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/winnt.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/objidl.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/objidl.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/mso_enum.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/mso_enum.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/variant.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/variant.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/strapi/strapi.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/strapi/strapi.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/common/strapi/strapi/wchar.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/common/strapi/strapi/wchar.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/wpp/wppapi/wppapi.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/wpp/wppapi/wppapi.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/wpp/wppapi/wppapi_predef.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/wpp/wppapi/wppapi_predef.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/wpp/wppapi.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/wpp/wppapi.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/et/etapi/etapi_predef.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/et/etapi/etapi_predef.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/et/etapi/etapi.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/et/etapi/etapi.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/et/etapi.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/et/etapi.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/wps/wpsapi/wpsapi.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/wps/wpsapi/wpsapi.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/wps/wpsapi/undefs.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/wps/wpsapi/undefs.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/wps/wpsapi/wpsapi_extend.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/wps/wpsapi/wpsapi_extend.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/include/wps/wpsapi.h` & `pywpsrpc-2.3.9/wpsrpc-sdk/include/wps/wpsapi.h`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/lib/x86_64/librpcwpsapi_sysqt5.so` & `pywpsrpc-2.3.9/wpsrpc-sdk/lib/x86_64/librpcwpsapi_sysqt5.so`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/lib/x86_64/librpcetapi_sysqt5.so` & `pywpsrpc-2.3.9/wpsrpc-sdk/lib/x86_64/librpcetapi_sysqt5.so`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/lib/x86_64/librpcwppapi_sysqt5.so` & `pywpsrpc-2.3.9/wpsrpc-sdk/lib/x86_64/librpcwppapi_sysqt5.so`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/tests/et/CMakeLists.txt` & `pywpsrpc-2.3.9/wpsrpc-sdk/tests/et/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/tests/et/rangevalue.cpp` & `pywpsrpc-2.3.9/wpsrpc-sdk/tests/et/rangevalue.cpp`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/tests/et/testetbase.cpp` & `pywpsrpc-2.3.9/wpsrpc-sdk/tests/et/testetbase.cpp`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/tests/wps/CMakeLists.txt` & `pywpsrpc-2.3.9/wpsrpc-sdk/tests/wps/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/tests/wps/testbase.cpp` & `pywpsrpc-2.3.9/wpsrpc-sdk/tests/wps/testbase.cpp`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/wpsrpc-sdk/tests/wps/comparedocs.cpp` & `pywpsrpc-2.3.9/wpsrpc-sdk/tests/wps/comparedocs.cpp`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/guid.sip` & `pywpsrpc-2.3.9/sip/common/guid.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/oaidl.sip` & `pywpsrpc-2.3.9/sip/common/oaidl.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/WaterMarks.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/WaterMarks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/_ApplicationEx.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/_ApplicationEx.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/Headings.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/Headings.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/enums.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/enums.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/Heading.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/Heading.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/WorkbooksEx.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/WorkbooksEx.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/PresentationsEx.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/PresentationsEx.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/RangeEx.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/RangeEx.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/HeaderFooterEx.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/HeaderFooterEx.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/_DocumentEx.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/_DocumentEx.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/WaterMark.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/WaterMark.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/_EtApplicationEx.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/_EtApplicationEx.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/WpsCloudService.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/WpsCloudService.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/_WorkbookEx.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/_WorkbookEx.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/PictureFormatEx.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/PictureFormatEx.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/DocumentsEx.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/DocumentsEx.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex/PrintoutPageEx.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex/PrintoutPageEx.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/objbase.sip` & `pywpsrpc-2.3.9/sip/common/objbase.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/common.sip` & `pywpsrpc-2.3.9/sip/common/common.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/wpsapiex.sip` & `pywpsrpc-2.3.9/sip/common/wpsapiex.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/export.sip` & `pywpsrpc-2.3.9/sip/common/export.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/COMAddIns.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/COMAddIns.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/HTMLProjectItem.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/HTMLProjectItem.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/FullSeriesCollection.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/FullSeriesCollection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Shape.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Shape.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/CommandBarControl.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/CommandBarControl.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/DocumentInspectors.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/DocumentInspectors.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/WebPageFont.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/WebPageFont.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/FileDialogSelectedItems.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/FileDialogSelectedItems.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/TabStops2.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/TabStops2.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/GlowFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/GlowFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SignatureProvider.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SignatureProvider.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IAccessible.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IAccessible.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoChart.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoChart.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Permission.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Permission.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ConnectorFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ConnectorFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ChartColorFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ChartColorFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/PolicyItem.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/PolicyItem.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ICustomXMLPartEvents.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ICustomXMLPartEvents.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IAssistance.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IAssistance.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SearchFolders.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SearchFolders.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/WorkflowTasks.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/WorkflowTasks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/DiagramNodeChildren.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/DiagramNodeChildren.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/WorkflowTask.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/WorkflowTask.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoTickLabels.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoTickLabels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/FoundFiles.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/FoundFiles.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ChartFillFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ChartFillFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ShapeRange.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ShapeRange.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/RulerLevel2.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/RulerLevel2.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/FillFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/FillFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoEServicesDialog.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoEServicesDialog.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IRibbonControl.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IRibbonControl.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoChartArea.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoChartArea.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/TextFrame.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/TextFrame.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ThemeFonts.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ThemeFonts.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/_CommandBarActiveX.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/_CommandBarActiveX.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/GradientStops.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/GradientStops.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ICustomXMLPartsEvents.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ICustomXMLPartsEvents.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ThemeColorScheme.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ThemeColorScheme.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/BalloonLabels.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/BalloonLabels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/TabStop2.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/TabStop2.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/CustomXMLPrefixMapping.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/CustomXMLPrefixMapping.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ParagraphFormat2.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ParagraphFormat2.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Points.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Points.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoCategory.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoCategory.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/EffectParameter.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/EffectParameter.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ODSOFilters.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ODSOFilters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IBlogExtensibility.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IBlogExtensibility.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoPlotArea.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoPlotArea.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ScopeFolders.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ScopeFolders.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/FreeformBuilder.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/FreeformBuilder.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/_CommandBars.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/_CommandBars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/MetaProperties.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/MetaProperties.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/BalloonCheckbox.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/BalloonCheckbox.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoSeriesLines.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoSeriesLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/PickerDialog.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/PickerDialog.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SmartDocument.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SmartDocument.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/WebComponentWindowExternal.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/WebComponentWindowExternal.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoLegendKey.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoLegendKey.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/CustomXMLPrefixMappings.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/CustomXMLPrefixMappings.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/FileDialog.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/FileDialog.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/FileTypes.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/FileTypes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/FileSearch.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/FileSearch.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceTask.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceTask.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtQuickStyle.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtQuickStyle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/GridLines.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/GridLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SignatureSetup.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SignatureSetup.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/BulletFormat2.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/BulletFormat2.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Adjustments.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Adjustments.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceFolder.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceFolder.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoEnvelopeVB.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoEnvelopeVB.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/CanvasShapes.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/CanvasShapes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ChartFont.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ChartFont.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Assistant.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Assistant.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/EncryptionProvider.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/EncryptionProvider.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceMembers.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceMembers.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/LanguageSettings.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/LanguageSettings.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Ruler2.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Ruler2.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ShapeNodes.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ShapeNodes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceLinks.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceLinks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/EffectParameters.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/EffectParameters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoTrendline.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoTrendline.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/NewFile.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/NewFile.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/enums.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/enums.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ILicWizExternal.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ILicWizExternal.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Crop.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Crop.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Font2.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Font2.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/CommandBar.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/CommandBar.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IDocumentInspector.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IDocumentInspector.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/DocumentProperty.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/DocumentProperty.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ThemeFontScheme.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ThemeFontScheme.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/AnswerWizardFiles.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/AnswerWizardFiles.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/OfficeTheme.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/OfficeTheme.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SearchScope.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SearchScope.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SeriesCollection.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SeriesCollection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoDropLines.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoDropLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Balloon.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Balloon.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/FileDialogFilters.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/FileDialogFilters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoBorder.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoBorder.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoFloor.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoFloor.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ReflectionFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ReflectionFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IRibbonUI.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IRibbonUI.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Shapes.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Shapes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Sync.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Sync.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtNode.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtNode.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IFoundFiles.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IFoundFiles.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/PictureFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/PictureFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Signature.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Signature.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoInterior.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoInterior.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/TextEffectFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/TextEffectFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/CustomXMLSchema.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/CustomXMLSchema.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/DocumentLibraryVersion.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/DocumentLibraryVersion.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ChartPoint.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ChartPoint.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/DiagramNodes.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/DiagramNodes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/PropertyTests.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/PropertyTests.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/PickerProperty.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/PickerProperty.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoChartTitle.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoChartTitle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtQuickStyles.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtQuickStyles.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/OfficeDataSourceObject.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/OfficeDataSourceObject.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ThreeDFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ThreeDFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ColorFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ColorFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtColors.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtColors.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ILicValidator.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ILicValidator.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Trendlines.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Trendlines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtNodes.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtNodes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoChartData.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoChartData.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/PickerResult.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/PickerResult.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/_CommandBarButton.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/_CommandBarButton.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/PickerFields.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/PickerFields.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtLayout.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtLayout.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoLegend.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoLegend.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/DiagramNode.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/DiagramNode.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/CustomXMLValidationErrors.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/CustomXMLValidationErrors.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoDataTable.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoDataTable.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoHiLoLines.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoHiLoLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/MsoDebugOptions_UTs.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/MsoDebugOptions_UTs.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/PictureEffect.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/PictureEffect.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/PropertyTest.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/PropertyTest.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SignatureSet.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SignatureSet.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceFiles.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceFiles.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/LineFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/LineFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ILicAgent.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ILicAgent.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/GroupShapes.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/GroupShapes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/BalloonLabel.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/BalloonLabel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/PickerResults.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/PickerResults.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/PictureEffects.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/PictureEffects.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SearchScopes.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SearchScopes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/WebComponentProperties.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/WebComponentProperties.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/UserPermission.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/UserPermission.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/FileDialogFilter.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/FileDialogFilter.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoDataLabels.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoDataLabels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ODSOFilter.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ODSOFilter.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IConverterApplicationPreferences.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IConverterApplicationPreferences.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ShadowFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ShadowFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoLeaderLines.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoLeaderLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoCharacters.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoCharacters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceMember.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceMember.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoCorners.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoCorners.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IConverterPreferences.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IConverterPreferences.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IConverter.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IConverter.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ODSOColumn.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ODSOColumn.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/MsoDebugOptions_UT.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/MsoDebugOptions_UT.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/DocumentProperties.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/DocumentProperties.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/CommandBarControls.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/CommandBarControls.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/MsoDebugOptions.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/MsoDebugOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoAxis.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoAxis.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceFile.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceFile.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoChartGroup.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoChartGroup.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/COMAddIn.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/COMAddIn.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspace.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspace.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Script.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Script.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoContactCard.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoContactCard.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ODSOColumns.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ODSOColumns.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/MsoDebugOptions_UTManager.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/MsoDebugOptions_UTManager.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceLink.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceLink.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoUpBars.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoUpBars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Axes.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Axes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ScopeFolder.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ScopeFolder.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/HTMLProjectItems.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/HTMLProjectItems.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoWalls.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoWalls.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SmartArt.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SmartArt.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/_CustomXMLSchemaCollection.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/_CustomXMLSchemaCollection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/WorkflowTemplate.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/WorkflowTemplate.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ThemeFont.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ThemeFont.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/AnswerWizard.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/AnswerWizard.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoChartFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoChartFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoSeries.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoSeries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/BalloonCheckboxes.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/BalloonCheckboxes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/LegendEntries.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/LegendEntries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/_CustomXMLParts.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/_CustomXMLParts.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/MetaProperty.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/MetaProperty.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoDownBars.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoDownBars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/_CustomXMLPart.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/_CustomXMLPart.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/TextFrame2.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/TextFrame2.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceTasks.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceTasks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoDataLabel.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoDataLabel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ContactCard.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ContactCard.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/CommandBarPopup.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/CommandBarPopup.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/WebPageFonts.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/WebPageFonts.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SoftEdgeFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SoftEdgeFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SignatureInfo.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SignatureInfo.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/CustomXMLValidationError.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/CustomXMLValidationError.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/HTMLProject.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/HTMLProject.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoDiagram.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoDiagram.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/CustomXMLNodes.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/CustomXMLNodes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/WebComponentFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/WebComponentFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/RulerLevels2.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/RulerLevels2.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/CategoryCollection.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/CategoryCollection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IMsoErrorBars.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IMsoErrorBars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SharedWorkspaceFolders.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SharedWorkspaceFolders.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/DocumentInspector.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/DocumentInspector.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtLayouts.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtLayouts.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ShapeNode.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ShapeNode.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/TextColumn2.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/TextColumn2.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ChartGroups.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ChartGroups.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/DocumentLibraryVersions.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/DocumentLibraryVersions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/TextRange2.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/TextRange2.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ThemeColor.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ThemeColor.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/WebComponent.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/WebComponent.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/GradientStop.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/GradientStop.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/PickerProperties.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/PickerProperties.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/WorkflowTemplates.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/WorkflowTemplates.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IConverterUICallback.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IConverterUICallback.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IBlogPictureExtensibility.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IBlogPictureExtensibility.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/_CommandBarComboBox.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/_CommandBarComboBox.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/CustomXMLNode.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/CustomXMLNode.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/PickerField.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/PickerField.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/Scripts.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/Scripts.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/LegendEntry.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/LegendEntry.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/ServerPolicy.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/ServerPolicy.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/IFind.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/IFind.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/MsoDebugOptions_UTRunResult.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/MsoDebugOptions_UTRunResult.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/CalloutFormat.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/CalloutFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/_CustomTaskPane.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/_CustomTaskPane.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi/SmartArtColor.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi/SmartArtColor.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/typedef.sip` & `pywpsrpc-2.3.9/sip/common/typedef.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/common/ksoapi.sip` & `pywpsrpc-2.3.9/sip/common/ksoapi.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTagRecognizers.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTagRecognizers.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Break.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Break.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/FullSeriesCollection.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/FullSeriesCollection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTags.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTags.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Shape.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Shape.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/HTMLDivisions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/HTMLDivisions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/RecentFiles.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/RecentFiles.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/mso_enum.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/mso_enum.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMaths.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMaths.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Source.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Source.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Revision.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Revision.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ChartTitle.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ChartTitle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathMatCols.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathMatCols.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/GlowFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/GlowFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/InlineShapes.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/InlineShapes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathFrac.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathFrac.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/EmailSignature.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/EmailSignature.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/FormField.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/FormField.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ReadabilityStatistic.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ReadabilityStatistic.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ConnectorFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ConnectorFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/DataLabels.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/DataLabels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TablesOfContents.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TablesOfContents.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Reviewers.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Reviewers.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ChartColorFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ChartColorFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Table.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Table.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Variable.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Variable.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ChartBorder.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ChartBorder.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/XSLTransform.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/XSLTransform.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/RecentFile.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/RecentFile.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/_Application_extend.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/_Application_extend.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Conflict.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Conflict.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathAutoCorrectEntries.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathAutoCorrectEntries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/SynonymInfo.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/SynonymInfo.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Trendline.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Trendline.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/LegendKey.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/LegendKey.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/DiagramNodeChildren.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/DiagramNodeChildren.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Words.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Words.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Frameset.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Frameset.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ChartFillFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ChartFillFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Line.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Line.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/FontNames.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/FontNames.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Axis.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Axis.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathDelim.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathDelim.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathScrSub.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathScrSub.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/FirstLetterException.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/FirstLetterException.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ShapeRange.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ShapeRange.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ContentControlListEntries.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ContentControlListEntries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TaskPane.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TaskPane.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/FillFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/FillFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TwoInitialCapsExceptions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TwoInitialCapsExceptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathFunc.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathFunc.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathRad.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathRad.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CustomLabel.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CustomLabel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Cell.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Cell.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Indexes.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Indexes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/IApplicationEvents2.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/IApplicationEvents2.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CoAuthoring.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CoAuthoring.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Reviewer.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Reviewer.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Options.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Options.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ListLevels.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ListLevels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TextFrame.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TextFrame.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Zooms.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Zooms.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMath.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMath.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Window.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Window.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Template.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Template.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CoAuthor.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CoAuthor.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ListFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ListFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathRecognizedFunction.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathRecognizedFunction.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Browser.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Browser.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/_ParagraphFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/_ParagraphFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Style.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Style.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Frames.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Frames.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/HangulHanjaConversionDictionaries.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/HangulHanjaConversionDictionaries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Comment.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Comment.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTagTypes.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTagTypes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Task.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Task.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathMatRows.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathMatRows.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Endnotes.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Endnotes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ConditionalStyle.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ConditionalStyle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathFunctions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathFunctions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Points.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Points.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/PageNumber.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/PageNumber.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CustomProperties.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CustomProperties.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/AutoCorrectEntries.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/AutoCorrectEntries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/DownBars.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/DownBars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TwoInitialCapsException.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TwoInitialCapsException.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/AddIns.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/AddIns.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/FormFields.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/FormFields.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Point.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Point.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathAcc.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathAcc.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/FreeformBuilder.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/FreeformBuilder.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ChartFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ChartFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Hyperlink.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Hyperlink.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Documents.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Documents.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Floor.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Floor.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Hyperlinks.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Hyperlinks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CoAuthLocks.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CoAuthLocks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/HorizontalLineFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/HorizontalLineFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/XMLSchemaReference.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/XMLSchemaReference.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathFunction.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathFunction.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/LinkFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/LinkFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/XMLNamespace.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/XMLNamespace.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Editor.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Editor.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/LineNumbering.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/LineNumbering.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/_Font.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/_Font.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Adjustments.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Adjustments.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Paragraphs.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Paragraphs.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TableOfFigures.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TableOfFigures.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OfdExportOptions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OfdExportOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/MailMergeDataField.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/MailMergeDataField.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/XSLTransforms.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/XSLTransforms.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CanvasShapes.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CanvasShapes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ChartFont.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ChartFont.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TabStop.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TabStop.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathScrPre.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathScrPre.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OtherCorrectionsExceptions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OtherCorrectionsExceptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ListEntries.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ListEntries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Find.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Find.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Pane.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Pane.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/EmailAuthor.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/EmailAuthor.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/XMLMapping.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/XMLMapping.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/RepeatingSectionItemColl.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/RepeatingSectionItemColl.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ShapeNodes.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ShapeNodes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Sources.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Sources.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Tables.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Tables.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/MailMergeFieldNames.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/MailMergeFieldNames.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Rectangles.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Rectangles.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/IWORDCtrlExtender.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/_OLEControl.sip`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace wpsapi
 {
-    struct IWORDCtrlExtender : public IDispatch /Abstract/
+    struct _OLEControl : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Left(
             single *prop /Out/) = 0;
 
         virtual HRESULT put_Left(
             single prop) = 0;
```

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathEqArray.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathEqArray.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/MailMergeDataSource.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/MailMergeDataSource.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/enums.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/enums.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/UndoRecord.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/UndoRecord.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Bookmark.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Bookmark.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/HangulAndAlphabetExceptions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/HangulAndAlphabetExceptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Styles.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Styles.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TextRetrievalMode.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TextRetrievalMode.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Frame.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Frame.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/DataLabel.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/DataLabel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Envelope.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Envelope.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ReadabilityStatistics.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ReadabilityStatistics.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Subdocuments.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Subdocuments.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/SeriesCollection.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/SeriesCollection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ReflectionFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ReflectionFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/MailingLabel.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/MailingLabel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Shapes.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Shapes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/IKRpcClient.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/IKRpcClient.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/AutoCaptions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/AutoCaptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/SeriesLines.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/SeriesLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/FootnoteOptions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/FootnoteOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathMat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathMat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Windows.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Windows.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathBreaks.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathBreaks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/PictureFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/PictureFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/MailMergeFieldName.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/MailMergeFieldName.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TablesOfFigures.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TablesOfFigures.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TextInput.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TextInput.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/_OLEControl.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathPhantom.sip`

 * *Files 12% similar despite different names*

```diff
@@ -6,284 +6,299 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace wpsapi
 {
-    struct _OLEControl : public IDispatch /Abstract/
+    struct OMathPhantom : public IDispatch /Abstract/
     {
     public:
-        virtual HRESULT get_Left(
-            single *prop /Out/) = 0;
+        virtual HRESULT get_Application(
+            Application **prop /Out/) = 0;
 
-        virtual HRESULT put_Left(
-            single prop) = 0;
+        virtual HRESULT get_E(
+            OMath **prop /Out/) = 0;
 
-        virtual HRESULT get_Top(
-            single *prop /Out/) = 0;
+        virtual HRESULT get_Show(
+            VARIANT_BOOL *prop /Out/) = 0;
 
-        virtual HRESULT put_Top(
-            single prop) = 0;
+        virtual HRESULT put_Show(
+            VARIANT_BOOL prop) = 0;
 
-        virtual HRESULT get_Height(
-            single *prop /Out/) = 0;
+        virtual HRESULT get_ZeroWid(
+            VARIANT_BOOL *prop /Out/) = 0;
 
-        virtual HRESULT put_Height(
-            single prop) = 0;
+        virtual HRESULT put_ZeroWid(
+            VARIANT_BOOL prop) = 0;
 
-        virtual HRESULT get_Width(
-            single *prop /Out/) = 0;
+        virtual HRESULT get_ZeroAsc(
+            VARIANT_BOOL *prop /Out/) = 0;
 
-        virtual HRESULT put_Width(
-            single prop) = 0;
+        virtual HRESULT put_ZeroAsc(
+            VARIANT_BOOL prop) = 0;
 
-        virtual HRESULT get_Name(
-            BSTR *prop /Out/) = 0;
+        virtual HRESULT get_ZeroDesc(
+            VARIANT_BOOL *prop /Out/) = 0;
 
-        virtual HRESULT put_Name(
-            BSTR prop) = 0;
+        virtual HRESULT put_ZeroDesc(
+            VARIANT_BOOL prop) = 0;
 
-        virtual HRESULT get_Automation(
-            IDispatch **prop /Out/) = 0;
+        virtual HRESULT get_Transp(
+            VARIANT_BOOL *prop /Out/) = 0;
 
-        virtual HRESULT Select() = 0;
+        virtual HRESULT put_Transp(
+            VARIANT_BOOL prop) = 0;
 
-        virtual HRESULT Copy() = 0;
+        virtual HRESULT get_Smash(
+            VARIANT_BOOL *prop /Out/) = 0;
 
-        virtual HRESULT Cut() = 0;
+        virtual HRESULT put_Smash(
+            VARIANT_BOOL prop) = 0;
 
-        virtual HRESULT Delete() = 0;
-
-        virtual HRESULT Activate() = 0;
-
-        virtual HRESULT get_AltHTML(
-            BSTR *prop /Out/) = 0;
-
-        virtual HRESULT put_AltHTML(
-            BSTR prop) = 0;
-
-        single getLeft();
+        Application* getApplication();
         %MethodCode
-            wpsapi::single prop = 0;
-            HRESULT hr = sipCpp->get_Left(&prop);
+            wpsapi::Application *prop = nullptr;
+            HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Left()' failed with 0x%x", hr);
+                    "Call 'get_Application()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setLeft(single prop);
+        %Property(name=Application, get=getApplication)
+
+        OMath* getE();
         %MethodCode
-            HRESULT hr = sipCpp->put_Left(a0);
+            wpsapi::OMath *prop = nullptr;
+            HRESULT hr = sipCpp->get_E(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Left()' failed with 0x%x", hr);
-                sipRes = nullptr;
+                    "Call 'get_E()' failed with 0x%x", hr);
+                return nullptr;
             }
             else
             {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
+                sipRes = prop;
             }
         %End
 
-        %Property(name=Left, get=getLeft, set=setLeft)
+        %Property(name=E, get=getE)
 
-        single getTop();
+        VARIANT_BOOL getShow();
         %MethodCode
-            wpsapi::single prop = 0;
-            HRESULT hr = sipCpp->get_Top(&prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_Show(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Top()' failed with 0x%x", hr);
+                    "Call 'get_Show()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setTop(single prop);
+        PyObject* setShow(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Top(a0);
+            HRESULT hr = sipCpp->put_Show(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Top()' failed with 0x%x", hr);
+                    "Call 'put_Show()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Top, get=getTop, set=setTop)
+        %Property(name=Show, get=getShow, set=setShow)
 
-        single getHeight();
+        VARIANT_BOOL getZeroWid();
         %MethodCode
-            wpsapi::single prop = 0;
-            HRESULT hr = sipCpp->get_Height(&prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_ZeroWid(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Height()' failed with 0x%x", hr);
+                    "Call 'get_ZeroWid()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setHeight(single prop);
+        PyObject* setZeroWid(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Height(a0);
+            HRESULT hr = sipCpp->put_ZeroWid(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Height()' failed with 0x%x", hr);
+                    "Call 'put_ZeroWid()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Height, get=getHeight, set=setHeight)
+        %Property(name=ZeroWid, get=getZeroWid, set=setZeroWid)
 
-        single getWidth();
+        VARIANT_BOOL getZeroAsc();
         %MethodCode
-            wpsapi::single prop = 0;
-            HRESULT hr = sipCpp->get_Width(&prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_ZeroAsc(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Width()' failed with 0x%x", hr);
+                    "Call 'get_ZeroAsc()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setWidth(single prop);
+        PyObject* setZeroAsc(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Width(a0);
+            HRESULT hr = sipCpp->put_ZeroAsc(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Width()' failed with 0x%x", hr);
+                    "Call 'put_ZeroAsc()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Width, get=getWidth, set=setWidth)
+        %Property(name=ZeroAsc, get=getZeroAsc, set=setZeroAsc)
 
-        BSTR getName();
+        VARIANT_BOOL getZeroDesc();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_Name(prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_ZeroDesc(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Name()' failed with 0x%x", hr);
+                    "Call 'get_ZeroDesc()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setName(BSTR prop);
+        PyObject* setZeroDesc(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Name(*a0);
+            HRESULT hr = sipCpp->put_ZeroDesc(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Name()' failed with 0x%x", hr);
+                    "Call 'put_ZeroDesc()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Name, get=getName, set=setName)
+        %Property(name=ZeroDesc, get=getZeroDesc, set=setZeroDesc)
 
-        IDispatch* getAutomation();
+        VARIANT_BOOL getTransp();
         %MethodCode
-            IDispatch *prop = nullptr;
-            HRESULT hr = sipCpp->get_Automation(&prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_Transp(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Automation()' failed with 0x%x", hr);
+                    "Call 'get_Transp()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Automation, get=getAutomation)
+        PyObject* setTransp(VARIANT_BOOL prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_Transp(*a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_Transp()' failed with 0x%x", hr);
+                sipRes = nullptr;
+            }
+            else
+            {
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
+            }
+        %End
+
+        %Property(name=Transp, get=getTransp, set=setTransp)
 
-        BSTR getAltHTML();
+        VARIANT_BOOL getSmash();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_AltHTML(prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_Smash(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_AltHTML()' failed with 0x%x", hr);
+                    "Call 'get_Smash()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setAltHTML(BSTR prop);
+        PyObject* setSmash(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_AltHTML(*a0);
+            HRESULT hr = sipCpp->put_Smash(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_AltHTML()' failed with 0x%x", hr);
+                    "Call 'put_Smash()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=AltHTML, get=getAltHTML, set=setAltHTML)
+        %Property(name=Smash, get=getSmash, set=setSmash)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TextEffectFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TextEffectFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ContentControlListEntry.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ContentControlListEntry.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/XMLSchemaReferences.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/XMLSchemaReferences.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ProofreadingErrors.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ProofreadingErrors.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TablesOfAuthorities.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TablesOfAuthorities.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ErrorBars.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ErrorBars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/DiagramNodes.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/DiagramNodes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/AutoTextEntry.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/AutoTextEntry.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/BuildingBlockEntries.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/BuildingBlockEntries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Footnote.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Footnote.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Corners.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Corners.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CoAuthLock.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CoAuthLock.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Language.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Language.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OLEFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OLEFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ThreeDFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ThreeDFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/XMLChildNodeSuggestion.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/XMLChildNodeSuggestion.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/FileConverters.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/FileConverters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ColorFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ColorFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TableOfContents.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TableOfContents.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Templates.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Templates.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ContentControls.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ContentControls.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/EmailSignatureEntries.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/EmailSignatureEntries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Research.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Research.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ListEntry.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ListEntry.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/RevisionsFilter.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/RevisionsFilter.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Lines.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Lines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/KeyBindings.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/KeyBindings.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/MailMergeFields.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/MailMergeFields.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ListTemplate.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ListTemplate.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Trendlines.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Trendlines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Panes.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Panes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/SpellingSuggestion.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/SpellingSuggestion.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CustomLabels.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CustomLabels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/_Application.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/_Application.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathGroupChar.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathGroupChar.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TablesOfAuthoritiesCategories.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TablesOfAuthoritiesCategories.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathScrSubSup.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathScrSubSup.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/AutoCaption.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/AutoCaption.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Comments.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Comments.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathArgs.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathArgs.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Conflicts.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Conflicts.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/PlotArea.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/PlotArea.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/DiagramNode.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/DiagramNode.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathMatCol.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathMatCol.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ContentControl.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ContentControl.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TickLabels.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TickLabels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Characters.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Characters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Broadcast.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Broadcast.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CaptionLabels.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CaptionLabels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathBreak.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathBreak.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ChartGroup.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ChartGroup.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TableStyle.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TableStyle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathBox.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathBox.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Subdocument.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Subdocument.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Rows.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Rows.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Categories.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Categories.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathRecognizedFunctions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathRecognizedFunctions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Paragraph.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Paragraph.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Range.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Range.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/AutoCorrect.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/AutoCorrect.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/LineFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/LineFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Legend.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Legend.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ProtectedViewWindows.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ProtectedViewWindows.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTag.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTag.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/GroupShapes.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/GroupShapes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ListLevel.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ListLevel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Chart.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Chart.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathMatRow.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathMatRow.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Columns.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Columns.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/StoryRanges.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/StoryRanges.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ChartCategory.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ChartCategory.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathAutoCorrect.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathAutoCorrect.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/MailMergeField.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/MailMergeField.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTagRecognizer.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTagRecognizer.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Category.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Category.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/BuildingBlockTypes.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/BuildingBlockTypes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Endnote.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Endnote.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/AxisTitle.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/AxisTitle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/MailMergeDataFields.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/MailMergeDataFields.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CaptionLabel.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CaptionLabel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/_Document.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/_Document.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathLimUpp.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathLimUpp.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/WebOptions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/WebOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/UpBars.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/UpBars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/List.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/List.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathAutoCorrectEntry.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathAutoCorrectEntry.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Section.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Section.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/DropLines.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/DropLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ListTemplates.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ListTemplates.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/DisplayUnitLabel.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/DisplayUnitLabel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ShadowFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ShadowFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/KeyBinding.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/KeyBinding.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TabStops.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TabStops.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTagActions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTagActions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/HangulAndAlphabetException.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/HangulAndAlphabetException.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ChartCharacters.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ChartCharacters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TextColumn.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TextColumn.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/BuildingBlock.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/BuildingBlock.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/HTMLDivision.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/HTMLDivision.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Interior.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Interior.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/BuildingBlocks.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/BuildingBlocks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/IApplicationEvents3.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/IApplicationEvents3.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Replacement.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Replacement.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/IApplicationEvents4.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/IApplicationEvents4.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Walls.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Walls.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/EndnoteOptions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/EndnoteOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Bookmarks.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Bookmarks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TableOfAuthoritiesCategory.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TableOfAuthoritiesCategory.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/HiLoLines.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/HiLoLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/MailMessage.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/MailMessage.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Variables.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Variables.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Bibliography.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Bibliography.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Border.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Border.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/rpcwpsapi.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/rpcwpsapi.sip`

 * *Files 2% similar despite different names*

```diff
@@ -392,15 +392,14 @@
 %Include CategoryCollection.sip
 %Include Broadcast.sip
 %Include RevisionsFilter.sip
 %Include DocumentField.sip
 %Include DocumentFields.sip
 %Include OfdExportOptions.sip
 %Include PdfExportOptions.sip
-%Include IWORDCtrlExtender.sip
 
 
 namespace wpsapi
 {
     typedef _Application Application;
     typedef _Document Document;
     typedef _Font Font;
```

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Dialogs.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Dialogs.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/EmailOptions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/EmailOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TableOfAuthorities.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TableOfAuthorities.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Dictionary.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Dictionary.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/AutoTextEntries.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/AutoTextEntries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Cells.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Cells.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/WrapFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/WrapFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Fields.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Fields.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Lists.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Lists.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ProtectedViewWindow.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ProtectedViewWindow.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CoAuthUpdate.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CoAuthUpdate.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Email.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Email.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Column.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Column.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/EmailSignatureEntry.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/EmailSignatureEntry.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Axes.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Axes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Breaks.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Breaks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/MailMerge.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/MailMerge.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CoAuthors.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CoAuthors.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/_LetterContent.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/_LetterContent.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathPhantom.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IWorksheetView.sip`

 * *Files 14% similar despite different names*

```diff
@@ -4,64 +4,64 @@
  * This file is part of pywpsrpc.
  *
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
-namespace wpsapi
+namespace etapi
 {
-    struct OMathPhantom : public IDispatch /Abstract/
+    struct IWorksheetView : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
-            Application **prop /Out/) = 0;
+            Application **RHS /Out/) = 0;
 
-        virtual HRESULT get_E(
-            OMath **prop /Out/) = 0;
+        virtual HRESULT get_Creator(
+            XlCreator *RHS /Out/) = 0;
 
-        virtual HRESULT get_Show(
-            VARIANT_BOOL *prop /Out/) = 0;
-
-        virtual HRESULT put_Show(
-            VARIANT_BOOL prop) = 0;
+        virtual HRESULT get_Sheet(
+            _Worksheet **RHS /Out/) = 0;
+        %MethodCode
+            sipRes = sipCpp->get_Sheet((IDispatch**)&a0);
+        %End
 
-        virtual HRESULT get_ZeroWid(
-            VARIANT_BOOL *prop /Out/) = 0;
+        virtual HRESULT get_DisplayGridlines(
+            VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT put_ZeroWid(
-            VARIANT_BOOL prop) = 0;
+        virtual HRESULT put_DisplayGridlines(
+            VARIANT_BOOL RHS) = 0;
 
-        virtual HRESULT get_ZeroAsc(
-            VARIANT_BOOL *prop /Out/) = 0;
+        virtual HRESULT get_DisplayFormulas(
+            VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT put_ZeroAsc(
-            VARIANT_BOOL prop) = 0;
+        virtual HRESULT put_DisplayFormulas(
+            VARIANT_BOOL RHS) = 0;
 
-        virtual HRESULT get_ZeroDesc(
-            VARIANT_BOOL *prop /Out/) = 0;
+        virtual HRESULT get_DisplayHeadings(
+            VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT put_ZeroDesc(
-            VARIANT_BOOL prop) = 0;
+        virtual HRESULT put_DisplayHeadings(
+            VARIANT_BOOL RHS) = 0;
 
-        virtual HRESULT get_Transp(
-            VARIANT_BOOL *prop /Out/) = 0;
+        virtual HRESULT get_DisplayOutline(
+            VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT put_Transp(
-            VARIANT_BOOL prop) = 0;
+        virtual HRESULT put_DisplayOutline(
+            VARIANT_BOOL RHS) = 0;
 
-        virtual HRESULT get_Smash(
-            VARIANT_BOOL *prop /Out/) = 0;
+        virtual HRESULT get_DisplayZeros(
+            VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT put_Smash(
-            VARIANT_BOOL prop) = 0;
+        virtual HRESULT put_DisplayZeros(
+            VARIANT_BOOL RHS) = 0;
 
         Application* getApplication();
         %MethodCode
-            wpsapi::Application *prop = nullptr;
+            etapi::Application *prop = nullptr;
             HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
                     "Call 'get_Application()' failed with 0x%x", hr);
                 return nullptr;
             }
@@ -69,236 +69,219 @@
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Application, get=getApplication)
 
-        OMath* getE();
+        XlCreator getCreator();
         %MethodCode
-            wpsapi::OMath *prop = nullptr;
-            HRESULT hr = sipCpp->get_E(&prop);
+            etapi::XlCreator prop = (etapi::XlCreator)0;
+            HRESULT hr = sipCpp->get_Creator(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_E()' failed with 0x%x", hr);
+                    "Call 'get_Creator()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=E, get=getE)
+        %Property(name=Creator, get=getCreator)
 
-        VARIANT_BOOL getShow();
+        _Worksheet* getSheet();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_Show(prop);
+            etapi::_Worksheet *prop = nullptr;
+            HRESULT hr = sipCpp->get_Sheet((IDispatch**)&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Show()' failed with 0x%x", hr);
+                    "Call 'get_Sheet()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setShow(VARIANT_BOOL prop);
-        %MethodCode
-            HRESULT hr = sipCpp->put_Show(*a0);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Show()' failed with 0x%x", hr);
-                sipRes = nullptr;
-            }
-            else
-            {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
-            }
-        %End
-
-        %Property(name=Show, get=getShow, set=setShow)
+        %Property(name=Sheet, get=getSheet)
 
-        VARIANT_BOOL getZeroWid();
+        VARIANT_BOOL getDisplayGridlines();
         %MethodCode
             VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_ZeroWid(prop);
+            HRESULT hr = sipCpp->get_DisplayGridlines(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ZeroWid()' failed with 0x%x", hr);
+                    "Call 'get_DisplayGridlines()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setZeroWid(VARIANT_BOOL prop);
+        PyObject* setDisplayGridlines(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_ZeroWid(*a0);
+            HRESULT hr = sipCpp->put_DisplayGridlines(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_ZeroWid()' failed with 0x%x", hr);
+                    "Call 'put_DisplayGridlines()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=ZeroWid, get=getZeroWid, set=setZeroWid)
+        %Property(name=DisplayGridlines, get=getDisplayGridlines, set=setDisplayGridlines)
 
-        VARIANT_BOOL getZeroAsc();
+        VARIANT_BOOL getDisplayFormulas();
         %MethodCode
             VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_ZeroAsc(prop);
+            HRESULT hr = sipCpp->get_DisplayFormulas(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ZeroAsc()' failed with 0x%x", hr);
+                    "Call 'get_DisplayFormulas()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setZeroAsc(VARIANT_BOOL prop);
+        PyObject* setDisplayFormulas(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_ZeroAsc(*a0);
+            HRESULT hr = sipCpp->put_DisplayFormulas(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_ZeroAsc()' failed with 0x%x", hr);
+                    "Call 'put_DisplayFormulas()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=ZeroAsc, get=getZeroAsc, set=setZeroAsc)
+        %Property(name=DisplayFormulas, get=getDisplayFormulas, set=setDisplayFormulas)
 
-        VARIANT_BOOL getZeroDesc();
+        VARIANT_BOOL getDisplayHeadings();
         %MethodCode
             VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_ZeroDesc(prop);
+            HRESULT hr = sipCpp->get_DisplayHeadings(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ZeroDesc()' failed with 0x%x", hr);
+                    "Call 'get_DisplayHeadings()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setZeroDesc(VARIANT_BOOL prop);
+        PyObject* setDisplayHeadings(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_ZeroDesc(*a0);
+            HRESULT hr = sipCpp->put_DisplayHeadings(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_ZeroDesc()' failed with 0x%x", hr);
+                    "Call 'put_DisplayHeadings()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=ZeroDesc, get=getZeroDesc, set=setZeroDesc)
+        %Property(name=DisplayHeadings, get=getDisplayHeadings, set=setDisplayHeadings)
 
-        VARIANT_BOOL getTransp();
+        VARIANT_BOOL getDisplayOutline();
         %MethodCode
             VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_Transp(prop);
+            HRESULT hr = sipCpp->get_DisplayOutline(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Transp()' failed with 0x%x", hr);
+                    "Call 'get_DisplayOutline()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setTransp(VARIANT_BOOL prop);
+        PyObject* setDisplayOutline(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Transp(*a0);
+            HRESULT hr = sipCpp->put_DisplayOutline(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Transp()' failed with 0x%x", hr);
+                    "Call 'put_DisplayOutline()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Transp, get=getTransp, set=setTransp)
+        %Property(name=DisplayOutline, get=getDisplayOutline, set=setDisplayOutline)
 
-        VARIANT_BOOL getSmash();
+        VARIANT_BOOL getDisplayZeros();
         %MethodCode
             VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_Smash(prop);
+            HRESULT hr = sipCpp->get_DisplayZeros(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Smash()' failed with 0x%x", hr);
+                    "Call 'get_DisplayZeros()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setSmash(VARIANT_BOOL prop);
+        PyObject* setDisplayZeros(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Smash(*a0);
+            HRESULT hr = sipCpp->put_DisplayZeros(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Smash()' failed with 0x%x", hr);
+                    "Call 'put_DisplayZeros()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Smash, get=getSmash, set=setSmash)
+        %Property(name=DisplayZeros, get=getDisplayZeros, set=setDisplayZeros)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/StyleSheet.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/StyleSheet.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/FileConverter.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/FileConverter.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/DocumentField.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/DocumentField.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/FirstLetterExceptions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/FirstLetterExceptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ChartArea.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ChartArea.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathBorderBox.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathBorderBox.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Index.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Index.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/InlineShape.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/InlineShape.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/AutoCorrectEntry.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/AutoCorrectEntry.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathNary.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathNary.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TextColumns.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TextColumns.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/SpellingSuggestions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/SpellingSuggestions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/HeadingStyle.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/HeadingStyle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/RepeatingSectionItem.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/RepeatingSectionItem.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/LegendEntries.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/LegendEntries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CustomProperty.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CustomProperty.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/DataTable.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/DataTable.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Languages.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Languages.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ListGallery.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ListGallery.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/HeaderFooter.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/HeaderFooter.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Pages.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Pages.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Gridlines.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Gridlines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/BuildingBlockType.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/BuildingBlockType.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Series.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Series.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CheckBox.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CheckBox.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/SoftEdgeFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/SoftEdgeFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Dialog.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Dialog.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/LeaderLines.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/LeaderLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Sentences.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Sentences.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/RoutingSlip.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/RoutingSlip.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/DropDown.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/DropDown.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Tasks.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Tasks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTagType.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTagType.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Field.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Field.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Footnotes.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Footnotes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/PageSetup.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/PageSetup.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Revisions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Revisions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CategoryCollection.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CategoryCollection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/MappedDataFields.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/MappedDataFields.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/XMLNodes.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/XMLNodes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/XMLChildNodeSuggestions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/XMLChildNodeSuggestions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OtherCorrectionsException.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OtherCorrectionsException.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ShapeNode.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ShapeNode.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Editors.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Editors.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Dictionaries.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Dictionaries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/AddIn.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/AddIn.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Shading.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Shading.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ChartGroups.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ChartGroups.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Page.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Page.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/System.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/System.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ListParagraphs.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ListParagraphs.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Rectangle.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Rectangle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Version.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Version.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathLimLow.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathLimLow.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/XMLNamespaces.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/XMLNamespaces.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathBar.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathBar.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Mailer.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Mailer.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/PdfExportOptions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/PdfExportOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/PageNumbers.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/PageNumbers.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/SmartTagAction.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/SmartTagAction.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/DefaultWebOptions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/DefaultWebOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/KeysBoundTo.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/KeysBoundTo.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Row.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Row.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/HeadersFooters.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/HeadersFooters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CoAuthUpdates.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CoAuthUpdates.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/HeadingStyles.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/HeadingStyles.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/OMathScrSup.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/OMathScrSup.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ChartData.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ChartData.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/DocumentFields.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/DocumentFields.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/LegendEntry.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/LegendEntry.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/TaskPanes.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/TaskPanes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Selection.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Selection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/DropCap.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/DropCap.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/XMLNode.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/XMLNode.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Diagram.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Diagram.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/View.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/View.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Borders.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Borders.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Versions.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Versions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/ListGalleries.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/ListGalleries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/CalloutFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/CalloutFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/MappedDataField.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/MappedDataField.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Zoom.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Zoom.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/Sections.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/Sections.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwpsapi/StyleSheets.sip` & `pywpsrpc-2.3.9/sip/rpcwpsapi/StyleSheets.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ThemeVariants.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ThemeVariants.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/FullSeriesCollection.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/FullSeriesCollection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ColorScheme.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ColorScheme.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Shape.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Shape.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Collection.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Collection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/AnimationSettings.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/AnimationSettings.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ChartTitle.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ChartTitle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ConnectorFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ConnectorFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/DataLabels.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/DataLabels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/RulerLevel.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/RulerLevel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/PublishObject.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/PublishObject.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ChartColorFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ChartColorFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Table.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Table.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ChartBorder.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ChartBorder.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ColorEffect.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ColorEffect.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/CellRange.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/CellRange.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/SlideShowWindows.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/SlideShowWindows.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Trendline.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Trendline.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/LegendKey.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/LegendKey.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/DiagramNodeChildren.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/DiagramNodeChildren.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ChartFillFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ChartFillFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Axis.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Axis.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/CustomLayout.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/CustomLayout.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ShapeRange.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ShapeRange.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/FillFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/FillFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/PrintOptions.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/PrintOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/PrintRanges.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/PrintRanges.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Cell.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Cell.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Options.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Options.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/TextFrame.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/TextFrame.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/MediaFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/MediaFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ParagraphFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ParagraphFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/OCXExtender.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IWalls.sip`

 * *Files 12% similar despite different names*

```diff
@@ -4,317 +4,293 @@
  * This file is part of pywpsrpc.
  *
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
-namespace wppapi
+namespace etapi
 {
-    struct OCXExtender : public IDispatch /Abstract/
+    struct IWalls : public IDispatch /Abstract/
     {
     public:
-        virtual HRESULT get_Visible(
-            VARIANT_BOOL *Visible /Out/) = 0;
+        virtual HRESULT get_Application(
+            Application **RHS /Out/) = 0;
 
-        virtual HRESULT put_Visible(
-            VARIANT_BOOL Visible) = 0;
+        virtual HRESULT get_Creator(
+            XlCreator *RHS /Out/) = 0;
 
-        virtual HRESULT get_Left(
-            single *Left /Out/) = 0;
+        virtual HRESULT get_Name(
+            BSTR *RHS /Out/) = 0;
 
-        virtual HRESULT put_Left(
-            single Left) = 0;
+        virtual HRESULT Select(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_Top(
-            single *Top /Out/) = 0;
+        virtual HRESULT get_Border(
+            Border **RHS /Out/) = 0;
 
-        virtual HRESULT put_Top(
-            single Top) = 0;
+        virtual HRESULT ClearFormats(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_Height(
-            single *Height /Out/) = 0;
+        virtual HRESULT get_Interior(
+            Interior **RHS /Out/) = 0;
 
-        virtual HRESULT put_Height(
-            single Height) = 0;
+        virtual HRESULT get_Fill(
+            ChartFillFormat **RHS /Out/) = 0;
 
-        virtual HRESULT get_Width(
-            single *Width /Out/) = 0;
+        virtual HRESULT get_PictureType(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Width(
-            single Width) = 0;
+        virtual HRESULT put_PictureType(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_ZOrderPosition(
-            int *ZOrderPosition /Out/) = 0;
+        virtual HRESULT Paste() = 0;
 
-        virtual HRESULT get_Name(
-            BSTR *Name /Out/) = 0;
+        virtual HRESULT get_PictureUnit(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Name(
-            BSTR Name) = 0;
+        virtual HRESULT put_PictureUnit(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_AltHTML(
-            BSTR *AltHTML /Out/) = 0;
+        virtual HRESULT get_Thickness(
+            long *RHS /Out/) = 0;
 
-        virtual HRESULT put_AltHTML(
-            BSTR AltHTML) = 0;
+        virtual HRESULT put_Thickness(
+            long RHS) = 0;
 
-        VARIANT_BOOL getVisible();
+        virtual HRESULT get_Format(
+            ChartFormat **RHS /Out/) = 0;
+
+        Application* getApplication();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_Visible(prop);
+            etapi::Application *prop = nullptr;
+            HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Visible()' failed with 0x%x", hr);
+                    "Call 'get_Application()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setVisible(VARIANT_BOOL prop);
+        %Property(name=Application, get=getApplication)
+
+        XlCreator getCreator();
         %MethodCode
-            HRESULT hr = sipCpp->put_Visible(*a0);
+            etapi::XlCreator prop = (etapi::XlCreator)0;
+            HRESULT hr = sipCpp->get_Creator(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Visible()' failed with 0x%x", hr);
-                sipRes = nullptr;
+                    "Call 'get_Creator()' failed with 0x%x", hr);
+                return nullptr;
             }
             else
             {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
+                sipRes = prop;
             }
         %End
 
-        %Property(name=Visible, get=getVisible, set=setVisible)
+        %Property(name=Creator, get=getCreator)
 
-        single getLeft();
+        BSTR getName();
         %MethodCode
-            wppapi::single prop = 0;
-            HRESULT hr = sipCpp->get_Left(&prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_Name(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Left()' failed with 0x%x", hr);
+                    "Call 'get_Name()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setLeft(single prop);
+        %Property(name=Name, get=getName)
+
+        Border* getBorder();
         %MethodCode
-            HRESULT hr = sipCpp->put_Left(a0);
+            etapi::Border *prop = nullptr;
+            HRESULT hr = sipCpp->get_Border(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Left()' failed with 0x%x", hr);
-                sipRes = nullptr;
+                    "Call 'get_Border()' failed with 0x%x", hr);
+                return nullptr;
             }
             else
             {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
+                sipRes = prop;
             }
         %End
 
-        %Property(name=Left, get=getLeft, set=setLeft)
+        %Property(name=Border, get=getBorder)
 
-        single getTop();
+        Interior* getInterior();
         %MethodCode
-            wppapi::single prop = 0;
-            HRESULT hr = sipCpp->get_Top(&prop);
+            etapi::Interior *prop = nullptr;
+            HRESULT hr = sipCpp->get_Interior(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Top()' failed with 0x%x", hr);
+                    "Call 'get_Interior()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setTop(single prop);
+        %Property(name=Interior, get=getInterior)
+
+        ChartFillFormat* getFill();
         %MethodCode
-            HRESULT hr = sipCpp->put_Top(a0);
+            etapi::ChartFillFormat *prop = nullptr;
+            HRESULT hr = sipCpp->get_Fill(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Top()' failed with 0x%x", hr);
-                sipRes = nullptr;
+                    "Call 'get_Fill()' failed with 0x%x", hr);
+                return nullptr;
             }
             else
             {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
+                sipRes = prop;
             }
         %End
 
-        %Property(name=Top, get=getTop, set=setTop)
+        %Property(name=Fill, get=getFill)
 
-        single getHeight();
+        VARIANT getPictureType();
         %MethodCode
-            wppapi::single prop = 0;
-            HRESULT hr = sipCpp->get_Height(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_PictureType(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Height()' failed with 0x%x", hr);
+                    "Call 'get_PictureType()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setHeight(single prop);
+        PyObject* setPictureType(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Height(a0);
+            HRESULT hr = sipCpp->put_PictureType(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Height()' failed with 0x%x", hr);
+                    "Call 'put_PictureType()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Height, get=getHeight, set=setHeight)
+        %Property(name=PictureType, get=getPictureType, set=setPictureType)
 
-        single getWidth();
+        VARIANT getPictureUnit();
         %MethodCode
-            wppapi::single prop = 0;
-            HRESULT hr = sipCpp->get_Width(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_PictureUnit(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Width()' failed with 0x%x", hr);
+                    "Call 'get_PictureUnit()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setWidth(single prop);
+        PyObject* setPictureUnit(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Width(a0);
+            HRESULT hr = sipCpp->put_PictureUnit(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Width()' failed with 0x%x", hr);
+                    "Call 'put_PictureUnit()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Width, get=getWidth, set=setWidth)
-
-        int getZOrderPosition();
-        %MethodCode
-            int prop = 0;
-            HRESULT hr = sipCpp->get_ZOrderPosition(&prop);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ZOrderPosition()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        %Property(name=ZOrderPosition, get=getZOrderPosition)
+        %Property(name=PictureUnit, get=getPictureUnit, set=setPictureUnit)
 
-        BSTR getName();
+        long getThickness();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_Name(prop);
+            long prop = 0;
+            HRESULT hr = sipCpp->get_Thickness(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Name()' failed with 0x%x", hr);
+                    "Call 'get_Thickness()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setName(BSTR prop);
+        PyObject* setThickness(long prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Name(*a0);
+            HRESULT hr = sipCpp->put_Thickness(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Name()' failed with 0x%x", hr);
+                    "Call 'put_Thickness()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Name, get=getName, set=setName)
+        %Property(name=Thickness, get=getThickness, set=setThickness)
 
-        BSTR getAltHTML();
+        ChartFormat* getFormat();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_AltHTML(prop);
+            etapi::ChartFormat *prop = nullptr;
+            HRESULT hr = sipCpp->get_Format(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_AltHTML()' failed with 0x%x", hr);
+                    "Call 'get_Format()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setAltHTML(BSTR prop);
-        %MethodCode
-            HRESULT hr = sipCpp->put_AltHTML(*a0);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_AltHTML()' failed with 0x%x", hr);
-                sipRes = nullptr;
-            }
-            else
-            {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
-            }
-        %End
-
-        %Property(name=AltHTML, get=getAltHTML, set=setAltHTML)
+        %Property(name=Format, get=getFormat)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Coauthoring.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Coauthoring.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Comment.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Comment.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Design.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Design.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/_Master.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/_Master.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/EApplication.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/EApplication.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ScaleEffect.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ScaleEffect.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Points.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Points.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/MotionEffect.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/MotionEffect.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/IPPTCtrlExtender.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IBorder.sip`

 * *Files 11% similar despite different names*

```diff
@@ -4,317 +4,307 @@
  * This file is part of pywpsrpc.
  *
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
-namespace wppapi
+namespace etapi
 {
-    struct IPPTCtrlExtender : public IDispatch /Abstract/
+    struct IBorder : public IDispatch /Abstract/
     {
     public:
-        virtual HRESULT get_Visible(
-            VARIANT_BOOL *Visible /Out/) = 0;
+        virtual HRESULT get_Application(
+            Application **RHS /Out/) = 0;
 
-        virtual HRESULT put_Visible(
-            VARIANT_BOOL Visible) = 0;
+        virtual HRESULT get_Creator(
+            XlCreator *RHS /Out/) = 0;
 
-        virtual HRESULT get_Left(
-            single *Left /Out/) = 0;
+        virtual HRESULT get_Color(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Left(
-            single Left) = 0;
+        virtual HRESULT put_Color(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_Top(
-            single *Top /Out/) = 0;
+        virtual HRESULT get_ColorIndex(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Top(
-            single Top) = 0;
+        virtual HRESULT put_ColorIndex(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_Height(
-            single *Height /Out/) = 0;
+        virtual HRESULT get_LineStyle(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Height(
-            single Height) = 0;
+        virtual HRESULT put_LineStyle(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_Width(
-            single *Width /Out/) = 0;
+        virtual HRESULT get_Weight(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Width(
-            single Width) = 0;
+        virtual HRESULT put_Weight(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_ZOrderPosition(
-            int *ZOrderPosition /Out/) = 0;
+        virtual HRESULT get_ThemeColor(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_Name(
-            BSTR *Name /Out/) = 0;
+        virtual HRESULT put_ThemeColor(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT put_Name(
-            BSTR Name) = 0;
+        virtual HRESULT get_TintAndShade(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_AltHTML(
-            BSTR *AltHTML /Out/) = 0;
+        virtual HRESULT put_TintAndShade(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT put_AltHTML(
-            BSTR AltHTML) = 0;
-
-        VARIANT_BOOL getVisible();
+        Application* getApplication();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_Visible(prop);
+            etapi::Application *prop = nullptr;
+            HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Visible()' failed with 0x%x", hr);
+                    "Call 'get_Application()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setVisible(VARIANT_BOOL prop);
+        %Property(name=Application, get=getApplication)
+
+        XlCreator getCreator();
         %MethodCode
-            HRESULT hr = sipCpp->put_Visible(*a0);
+            etapi::XlCreator prop = (etapi::XlCreator)0;
+            HRESULT hr = sipCpp->get_Creator(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Visible()' failed with 0x%x", hr);
-                sipRes = nullptr;
+                    "Call 'get_Creator()' failed with 0x%x", hr);
+                return nullptr;
             }
             else
             {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
+                sipRes = prop;
             }
         %End
 
-        %Property(name=Visible, get=getVisible, set=setVisible)
+        %Property(name=Creator, get=getCreator)
 
-        single getLeft();
+        VARIANT getColor();
         %MethodCode
-            wppapi::single prop = 0;
-            HRESULT hr = sipCpp->get_Left(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Color(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Left()' failed with 0x%x", hr);
+                    "Call 'get_Color()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setLeft(single prop);
+        PyObject* setColor(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Left(a0);
+            HRESULT hr = sipCpp->put_Color(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Left()' failed with 0x%x", hr);
+                    "Call 'put_Color()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Left, get=getLeft, set=setLeft)
+        %Property(name=Color, get=getColor, set=setColor)
 
-        single getTop();
+        VARIANT getColorIndex();
         %MethodCode
-            wppapi::single prop = 0;
-            HRESULT hr = sipCpp->get_Top(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_ColorIndex(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Top()' failed with 0x%x", hr);
+                    "Call 'get_ColorIndex()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setTop(single prop);
+        PyObject* setColorIndex(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Top(a0);
+            HRESULT hr = sipCpp->put_ColorIndex(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Top()' failed with 0x%x", hr);
+                    "Call 'put_ColorIndex()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Top, get=getTop, set=setTop)
+        %Property(name=ColorIndex, get=getColorIndex, set=setColorIndex)
 
-        single getHeight();
+        VARIANT getLineStyle();
         %MethodCode
-            wppapi::single prop = 0;
-            HRESULT hr = sipCpp->get_Height(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_LineStyle(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Height()' failed with 0x%x", hr);
+                    "Call 'get_LineStyle()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setHeight(single prop);
+        PyObject* setLineStyle(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Height(a0);
+            HRESULT hr = sipCpp->put_LineStyle(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Height()' failed with 0x%x", hr);
+                    "Call 'put_LineStyle()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Height, get=getHeight, set=setHeight)
+        %Property(name=LineStyle, get=getLineStyle, set=setLineStyle)
 
-        single getWidth();
+        VARIANT getWeight();
         %MethodCode
-            wppapi::single prop = 0;
-            HRESULT hr = sipCpp->get_Width(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Weight(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Width()' failed with 0x%x", hr);
+                    "Call 'get_Weight()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setWidth(single prop);
+        PyObject* setWeight(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Width(a0);
+            HRESULT hr = sipCpp->put_Weight(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Width()' failed with 0x%x", hr);
+                    "Call 'put_Weight()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Width, get=getWidth, set=setWidth)
-
-        int getZOrderPosition();
-        %MethodCode
-            int prop = 0;
-            HRESULT hr = sipCpp->get_ZOrderPosition(&prop);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ZOrderPosition()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        %Property(name=ZOrderPosition, get=getZOrderPosition)
+        %Property(name=Weight, get=getWeight, set=setWeight)
 
-        BSTR getName();
+        VARIANT getThemeColor();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_Name(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_ThemeColor(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Name()' failed with 0x%x", hr);
+                    "Call 'get_ThemeColor()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setName(BSTR prop);
+        PyObject* setThemeColor(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Name(*a0);
+            HRESULT hr = sipCpp->put_ThemeColor(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Name()' failed with 0x%x", hr);
+                    "Call 'put_ThemeColor()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Name, get=getName, set=setName)
+        %Property(name=ThemeColor, get=getThemeColor, set=setThemeColor)
 
-        BSTR getAltHTML();
+        VARIANT getTintAndShade();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_AltHTML(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_TintAndShade(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_AltHTML()' failed with 0x%x", hr);
+                    "Call 'get_TintAndShade()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setAltHTML(BSTR prop);
+        PyObject* setTintAndShade(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_AltHTML(*a0);
+            HRESULT hr = sipCpp->put_TintAndShade(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_AltHTML()' failed with 0x%x", hr);
+                    "Call 'put_TintAndShade()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=AltHTML, get=getAltHTML, set=setAltHTML)
+        %Property(name=TintAndShade, get=getTintAndShade, set=setTintAndShade)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/DownBars.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/DownBars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/AddIns.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/AddIns.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Point.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Point.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/PropertyEffect.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/PropertyEffect.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/FreeformBuilder.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/FreeformBuilder.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ChartFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ChartFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Hyperlink.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Hyperlink.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Floor.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Floor.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Hyperlinks.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Hyperlinks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/FilterEffect.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/FilterEffect.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/CustomLayouts.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/CustomLayouts.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/LinkFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/LinkFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Adjustments.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Adjustments.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Designs.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Designs.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/CanvasShapes.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/CanvasShapes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/DocumentWindows.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/DocumentWindows.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ChartFont.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ChartFont.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/TabStop.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/TabStop.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/SoundFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/SoundFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/DocumentWindow.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/DocumentWindow.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/SlideShowView.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/SlideShowView.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Pane.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Pane.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ShapeNodes.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ShapeNodes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/NamedSlideShows.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/NamedSlideShows.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/EffectParameters.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/EffectParameters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/enums.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/enums.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Font.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Font.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/DataLabel.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/DataLabel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/SeriesCollection.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/SeriesCollection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Shapes.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Shapes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/IKRpcClient.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/IKRpcClient.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/SeriesLines.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/SeriesLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/PictureFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/PictureFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/TextEffectFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/TextEffectFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/TableBackground.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/TableBackground.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/PlaySettings.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/PlaySettings.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ErrorBars.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ErrorBars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/SoundEffect.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/SoundEffect.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/RulerLevels.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/RulerLevels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Presentations.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Presentations.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/DiagramNodes.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/DiagramNodes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ColorSchemes.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ColorSchemes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Corners.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Corners.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/OLEFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/OLEFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ExtraColors.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ExtraColors.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ThreeDFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ThreeDFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/TextStyleLevel.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/TextStyleLevel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/FileConverters.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/FileConverters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ColorFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ColorFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Research.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Research.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/SlideShowWindow.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/SlideShowWindow.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Trendlines.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Trendlines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/TimeLine.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/TimeLine.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Panes.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Panes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/SlideNavigation.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/SlideNavigation.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/_Application.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/_Application.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Comments.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Comments.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/_Presentation.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/_Presentation.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/PlotArea.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/PlotArea.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/SectionProperties.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/SectionProperties.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/DiagramNode.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/DiagramNode.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/TickLabels.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/TickLabels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Broadcast.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Broadcast.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ChartGroup.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ChartGroup.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/TableStyle.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/TableStyle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Rows.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Rows.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/AutoCorrect.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/AutoCorrect.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/LineFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/LineFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Legend.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Legend.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ProtectedViewWindows.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ProtectedViewWindows.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/GroupShapes.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/GroupShapes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Chart.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Chart.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Columns.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Columns.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Guide.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Guide.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ChartCategory.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ChartCategory.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/TextStyle.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/TextStyle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Sequences.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Sequences.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/AxisTitle.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/AxisTitle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/NamedSlideShow.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/NamedSlideShow.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/MediaBookmark.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/MediaBookmark.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/WebOptions.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/WebOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/UpBars.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/UpBars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/DropLines.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/DropLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/DisplayUnitLabel.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/DisplayUnitLabel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ShadowFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ShadowFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/TextStyles.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/TextStyles.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Effect.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Effect.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/TabStops.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/TabStops.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/CommandEffect.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/CommandEffect.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ChartCharacters.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ChartCharacters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ResampleMediaTasks.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ResampleMediaTasks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/RotationEffect.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/RotationEffect.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Interior.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Interior.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/PublishObjects.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/PublishObjects.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Player.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Player.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Walls.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Walls.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ActionSetting.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ActionSetting.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/TextRange.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/TextRange.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/HiLoLines.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/HiLoLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/RGBColor.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/RGBColor.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/AnimationBehavior.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/AnimationBehavior.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/_Slide.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/_Slide.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/SlideShowSettings.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/SlideShowSettings.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Tags.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Tags.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/SetEffect.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/SetEffect.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/MediaBookmarks.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/MediaBookmarks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/EffectInformation.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/EffectInformation.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ProtectedViewWindow.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ProtectedViewWindow.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/SlideShowTransition.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/SlideShowTransition.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Column.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Column.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Axes.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Axes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Timing.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Timing.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/BulletFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/BulletFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/FileConverter.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/FileConverter.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/CustomerData.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/CustomerData.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ChartArea.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ChartArea.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Slides.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Slides.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ResampleMediaTask.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ResampleMediaTask.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/LegendEntries.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/LegendEntries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/DataTable.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/DataTable.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/TextFrame2.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/TextFrame2.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/HeaderFooter.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/HeaderFooter.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Gridlines.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Gridlines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/AnimationBehaviors.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/AnimationBehaviors.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Sequence.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Sequence.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Series.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Series.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/LeaderLines.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/LeaderLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Fonts.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Fonts.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ObjectVerbs.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ObjectVerbs.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/TextStyleLevels.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/TextStyleLevels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/PageSetup.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/PageSetup.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Theme.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Theme.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Guides.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Guides.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/CategoryCollection.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/CategoryCollection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ThemeVariant.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ThemeVariant.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ShapeNode.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ShapeNode.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/AnimationPoint.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/AnimationPoint.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/AddIn.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/AddIn.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Placeholders.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Placeholders.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ChartGroups.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ChartGroups.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/PrintRange.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/PrintRange.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/rpcwppapi.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/rpcwppapi.sip`

 * *Files 1% similar despite different names*

```diff
@@ -102,16 +102,14 @@
 %Include TextStyleLevels.sip
 %Include TextStyleLevel.sip
 %Include HeaderFooter.sip
 %Include _Presentation.sip
 %Include Tags.sip
 %Include MouseTracker.sip
 %Include MouseDownHandler.sip
-%Include OCXExtender.sip
-%Include OCXExtenderEvents.sip
 %Include EApplication.sip
 %Include Table.sip
 %Include Columns.sip
 %Include Column.sip
 %Include Rows.sip
 %Include Row.sip
 %Include CellRange.sip
@@ -223,15 +221,14 @@
 %Include CategoryCollection.sip
 %Include ThemeVariant.sip
 %Include ThemeVariants.sip
 %Include Theme.sip
 %Include SlideNavigation.sip
 %Include Guides.sip
 %Include Guide.sip
-%Include IPPTCtrlExtender.sip
 
 namespace wppapi
 {
     typedef _Application Application;
     typedef _Presentation Presentation;
     typedef _Slide Slide;
```

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ActionSettings.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ActionSettings.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/PlaceholderFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/PlaceholderFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/DefaultWebOptions.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/DefaultWebOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Row.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Row.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/HeadersFooters.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/HeadersFooters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/AnimationPoints.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/AnimationPoints.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/ChartData.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/ChartData.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/SlideRange.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/SlideRange.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/LegendEntry.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/LegendEntry.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Selection.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Selection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Diagram.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Diagram.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/View.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/View.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Borders.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Borders.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/CalloutFormat.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/CalloutFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcwppapi/Ruler.sip` & `pywpsrpc-2.3.9/sip/rpcwppapi/Ruler.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IListObject.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IListObject.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IOLEDBError.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IOLEDBError.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IMenus.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IMenus.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISlicers.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISlicers.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IListDataFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IListDataFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/Solver.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/Solver.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/mso_enum.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/mso_enum.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IIconCriteria.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IIconCriteria.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPoints.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPoints.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDialogFrame.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDialogFrame.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDataTable.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDataTable.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IAutoCorrect.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IAutoCorrect.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IAddIns2.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IAddIns2.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IFreeformBuilder.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IFreeformBuilder.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDataBarBorder.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDataBarBorder.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ILegendEntry.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ILegendEntry.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISlicerCacheLevel.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISlicerCacheLevel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ICustomProperty.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ICustomProperty.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISheetViews.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISheetViews.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IXmlSchemas.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IXmlSchemas.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/PublishObject.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/PublishObject.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IIcon.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IIcon.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IIconCriterion.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IIconCriterion.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IProtection.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IProtection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModule.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModule.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ILabel.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ILabel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IXmlNamespaces.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IXmlNamespaces.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IFilter.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IFilter.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IMenu.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IMenu.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDrawingObjects.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDrawingObjects.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IRange.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IRange.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IEXCELCtrlExtender.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/_IOLEObject.sip`

 * *Files 0% similar despite different names*

```diff
@@ -6,26 +6,17 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct IEXCELCtrlExtender : public IDispatch /Abstract/
+    struct _IOLEObject : public IDispatch /Abstract/
     {
     public:
-        virtual HRESULT get_Name(
-            BSTR *RHS /Out/) = 0;
-
-        virtual HRESULT put_Name(
-            BSTR RHS) = 0;
-
-        virtual HRESULT get_Object(
-            IDispatch **RHS /Out/) = 0;
-
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
 
         virtual HRESULT get_BottomRightCell(
@@ -33,25 +24,25 @@
 
         virtual HRESULT BringToFront(
             VARIANT *RHS /Out/) = 0;
 
         virtual HRESULT Copy(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT Delete(
-            VARIANT *RHS /Out/) = 0;
-
         virtual HRESULT CopyPicture(
             XlPictureAppearance Appearance = etapi::xlPrinter,
             XlCopyPictureFormat Format = etapi::xlPicture,
             VARIANT *RHS /Out/ = 0) = 0;
 
         virtual HRESULT Cut(
             VARIANT *RHS /Out/) = 0;
 
+        virtual HRESULT Delete(
+            VARIANT *RHS /Out/) = 0;
+
         virtual HRESULT Duplicate(
             IDispatch **RHS /Out/) = 0;
 
         virtual HRESULT get_Enabled(
             VARIANT_BOOL *RHS /Out/) = 0;
 
         virtual HRESULT put_Enabled(
@@ -74,14 +65,20 @@
 
         virtual HRESULT get_Locked(
             VARIANT_BOOL *RHS /Out/) = 0;
 
         virtual HRESULT put_Locked(
             VARIANT_BOOL RHS) = 0;
 
+        virtual HRESULT get_Name(
+            BSTR *RHS /Out/) = 0;
+
+        virtual HRESULT put_Name(
+            BSTR RHS) = 0;
+
         virtual HRESULT get_OnAction(
             BSTR *RHS /Out/) = 0;
 
         virtual HRESULT put_OnAction(
             BSTR RHS) = 0;
 
         virtual HRESULT get_Placement(
@@ -153,14 +150,17 @@
 
         virtual HRESULT get_AutoUpdate(
             VARIANT_BOOL *RHS /Out/) = 0;
 
         virtual HRESULT put_AutoUpdate(
             VARIANT_BOOL RHS) = 0;
 
+        virtual HRESULT get_Object(
+            IDispatch **RHS /Out/) = 0;
+
         virtual HRESULT get_OLEType(
             VARIANT *RHS /Out/) = 0;
 
         virtual HRESULT get_SourceName(
             BSTR *RHS /Out/) = 0;
 
         virtual HRESULT put_SourceName(
@@ -190,67 +190,14 @@
 
         virtual HRESULT get_AltHTML(
             BSTR *RHS /Out/) = 0;
 
         virtual HRESULT put_AltHTML(
             BSTR RHS) = 0;
 
-        BSTR getName();
-        %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_Name(prop);
-            if (hr != S_OK)
-            {
-                delete prop;
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Name()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        PyObject* setName(BSTR prop);
-        %MethodCode
-            HRESULT hr = sipCpp->put_Name(*a0);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Name()' failed with 0x%x", hr);
-                sipRes = nullptr;
-            }
-            else
-            {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
-            }
-        %End
-
-        %Property(name=Name, get=getName, set=setName)
-
-        IDispatch* getObject();
-        %MethodCode
-            IDispatch *prop = nullptr;
-            HRESULT hr = sipCpp->get_Object(&prop);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Object()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        %Property(name=Object, get=getObject)
-
         Application* getApplication();
         %MethodCode
             etapi::Application *prop = nullptr;
             HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
@@ -453,14 +400,49 @@
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
         %Property(name=Locked, get=getLocked, set=setLocked)
 
+        BSTR getName();
+        %MethodCode
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_Name(prop);
+            if (hr != S_OK)
+            {
+                delete prop;
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_Name()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        PyObject* setName(BSTR prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_Name(*a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_Name()' failed with 0x%x", hr);
+                sipRes = nullptr;
+            }
+            else
+            {
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
+            }
+        %End
+
+        %Property(name=Name, get=getName, set=setName)
+
         BSTR getOnAction();
         %MethodCode
             BSTR *prop = new BSTR;
             HRESULT hr = sipCpp->get_OnAction(prop);
             if (hr != S_OK)
             {
                 delete prop;
@@ -857,14 +839,32 @@
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
         %Property(name=AutoUpdate, get=getAutoUpdate, set=setAutoUpdate)
 
+        IDispatch* getObject();
+        %MethodCode
+            IDispatch *prop = nullptr;
+            HRESULT hr = sipCpp->get_Object(&prop);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_Object()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        %Property(name=Object, get=getObject)
+
         VARIANT getOLEType();
         %MethodCode
             VARIANT *prop = new VARIANT;
             VariantInit(prop);
             HRESULT hr = sipCpp->get_OLEType(prop);
             if (hr != S_OK)
             {
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISmartTagAction.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISmartTagAction.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IOLEFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IOLEFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IToolbars.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IToolbars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITableStyleElement.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITableStyleElement.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/DiagramNodeChildren.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/DiagramNodeChildren.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IToolbar.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IToolbar.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IAddIns.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IAddIns.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelTableColumns.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelTableColumns.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IUserAccessList.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IUserAccessList.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotItem.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotItem.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ICalculatedFields.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ICalculatedFields.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IToolbarButtons.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IToolbarButtons.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITableStyles.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITableStyles.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISpinners.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISpinners.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ICalculatedItems.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ICalculatedItems.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IGraphic.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IGraphic.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IODBCErrors.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IODBCErrors.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IRtdServer.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IRtdServer.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/FillFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/FillFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotCache.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotCache.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IWatch.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IWatch.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IProtectedViewWindows.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IProtectedViewWindows.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ILinkFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ILinkFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotLine.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotLine.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModel.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IODBCConnection.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IODBCConnection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IXmlDataBinding.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IXmlDataBinding.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPhonetic.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPhonetic.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelTableNameChange.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelTableNameChange.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IListRows.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IListRows.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IColorScale.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IColorScale.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISparkHorizontalAxis.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISparkHorizontalAxis.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IRecentFile.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IRecentFile.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IMenuBars.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IMenuBars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotFields.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotFields.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IUserAccess.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IUserAccess.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDocEvents.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDocEvents.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelTableNames.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelTableNames.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IComments.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IComments.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IQueryTables.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IQueryTables.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISparkPoints.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISparkPoints.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IAddIn.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IAddIn.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IOLEDBConnection.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IOLEDBConnection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IParameter.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IParameter.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IErrorCheckingOptions.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IErrorCheckingOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IShapeRange.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IShapeRange.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISpinner.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISpinner.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IGroupObjects.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IGroupObjects.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IListBox.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IListBox.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ICharacters.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ICharacters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelTables.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelTables.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelTableColumn.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelTableColumn.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISort.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISort.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITop10.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITop10.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelColumnName.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelColumnName.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IListColumns.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IListColumns.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPlotArea.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPlotArea.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IShapes.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IShapes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IAllowEditRanges.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IAllowEditRanges.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IChartGroups.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IChartGroups.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IColorStop.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IColorStop.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPhonetics.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPhonetics.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IGridlines.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IGridlines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISpellingOptions.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISpellingOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ICalculatedMember.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ICalculatedMember.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IChartTitle.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IChartTitle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ICheckBoxes.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ICheckBoxes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IShape.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IShape.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ILegendEntries.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ILegendEntries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IChartColorFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IChartColorFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IGroupShapes.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IGroupShapes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/CubeFields.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/CubeFields.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IListBoxes.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IListBoxes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITab.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITab.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/Adjustments.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/Adjustments.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelMeasureName.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelMeasureName.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IMultiThreadedCalculation.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IMultiThreadedCalculation.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IListObjects.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IListObjects.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISlicerPivotTables.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISlicerPivotTables.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISmartTags.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISmartTags.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IOLEObjects.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IOLEObjects.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IResearch.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IResearch.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITrendline.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITrendline.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IError.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IError.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/_IOLEObject.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IOval.sip`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct _IOLEObject : public IDispatch /Abstract/
+    struct IOval : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
@@ -123,80 +123,106 @@
 
         virtual HRESULT get_ZOrder(
             long *RHS /Out/) = 0;
 
         virtual HRESULT get_ShapeRange(
             ShapeRange **RHS /Out/) = 0;
 
-        virtual HRESULT get_Border(
-            Border **RHS /Out/) = 0;
-
-        virtual HRESULT get_Interior(
-            Interior **RHS /Out/) = 0;
-
-        virtual HRESULT get_Shadow(
+        virtual HRESULT get_AddIndent(
             VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT put_Shadow(
+        virtual HRESULT put_AddIndent(
             VARIANT_BOOL RHS) = 0;
 
-        virtual HRESULT Activate(
+        virtual HRESULT get_AutoScaleFont(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_AutoLoad(
+        virtual HRESULT put_AutoScaleFont(
+            VARIANT RHS) = 0;
+
+        virtual HRESULT get_AutoSize(
             VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT put_AutoLoad(
+        virtual HRESULT put_AutoSize(
             VARIANT_BOOL RHS) = 0;
 
-        virtual HRESULT get_AutoUpdate(
-            VARIANT_BOOL *RHS /Out/) = 0;
+        virtual HRESULT get_Caption(
+            BSTR *RHS /Out/) = 0;
 
-        virtual HRESULT put_AutoUpdate(
-            VARIANT_BOOL RHS) = 0;
+        virtual HRESULT put_Caption(
+            BSTR RHS) = 0;
 
-        virtual HRESULT get_Object(
-            IDispatch **RHS /Out/) = 0;
+        virtual HRESULT get_Characters(
+            VARIANT Start = argMissing2(),
+            VARIANT Length = argMissing2(),
+            Characters **RHS /Out/ = 0) = 0;
+
+        virtual HRESULT CheckSpelling(
+            VARIANT CustomDictionary = argMissing2(),
+            VARIANT IgnoreUppercase = argMissing2(),
+            VARIANT AlwaysSuggest = argMissing2(),
+            VARIANT SpellLang = argMissing2(),
+            VARIANT *RHS /Out/ = 0) = 0;
 
-        virtual HRESULT get_OLEType(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT get_Font(
+            Font **RHS /Out/) = 0;
 
-        virtual HRESULT get_SourceName(
+        virtual HRESULT get_Formula(
             BSTR *RHS /Out/) = 0;
 
-        virtual HRESULT put_SourceName(
+        virtual HRESULT put_Formula(
             BSTR RHS) = 0;
 
-        virtual HRESULT Update(
+        virtual HRESULT get_HorizontalAlignment(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT Verb(
-            XlOLEVerb Verb = etapi::xlVerbOpen,
-            VARIANT *RHS /Out/ = 0) = 0;
+        virtual HRESULT put_HorizontalAlignment(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_LinkedCell(
-            BSTR *RHS /Out/) = 0;
+        virtual HRESULT get_LockedText(
+            VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT put_LinkedCell(
-            BSTR RHS) = 0;
+        virtual HRESULT put_LockedText(
+            VARIANT_BOOL RHS) = 0;
+
+        virtual HRESULT get_Orientation(
+            VARIANT *RHS /Out/) = 0;
+
+        virtual HRESULT put_Orientation(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_ListFillRange(
+        virtual HRESULT get_Text(
             BSTR *RHS /Out/) = 0;
 
-        virtual HRESULT put_ListFillRange(
+        virtual HRESULT put_Text(
             BSTR RHS) = 0;
 
-        virtual HRESULT get_progID(
-            BSTR *RHS /Out/) = 0;
+        virtual HRESULT get_VerticalAlignment(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_AltHTML(
-            BSTR *RHS /Out/) = 0;
+        virtual HRESULT put_VerticalAlignment(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT put_AltHTML(
-            BSTR RHS) = 0;
+        virtual HRESULT get_ReadingOrder(
+            long *RHS /Out/) = 0;
+
+        virtual HRESULT put_ReadingOrder(
+            long RHS) = 0;
+
+        virtual HRESULT get_Border(
+            Border **RHS /Out/) = 0;
+
+        virtual HRESULT get_Interior(
+            Interior **RHS /Out/) = 0;
+
+        virtual HRESULT get_Shadow(
+            VARIANT_BOOL *RHS /Out/) = 0;
+
+        virtual HRESULT put_Shadow(
+            VARIANT_BOOL RHS) = 0;
 
         Application* getApplication();
         %MethodCode
             etapi::Application *prop = nullptr;
             HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
@@ -698,346 +724,485 @@
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=ShapeRange, get=getShapeRange)
 
-        Border* getBorder();
+        VARIANT_BOOL getAddIndent();
         %MethodCode
-            etapi::Border *prop = nullptr;
-            HRESULT hr = sipCpp->get_Border(&prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_AddIndent(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Border()' failed with 0x%x", hr);
+                    "Call 'get_AddIndent()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Border, get=getBorder)
+        PyObject* setAddIndent(VARIANT_BOOL prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_AddIndent(*a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_AddIndent()' failed with 0x%x", hr);
+                sipRes = nullptr;
+            }
+            else
+            {
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
+            }
+        %End
 
-        Interior* getInterior();
+        %Property(name=AddIndent, get=getAddIndent, set=setAddIndent)
+
+        VARIANT getAutoScaleFont();
         %MethodCode
-            etapi::Interior *prop = nullptr;
-            HRESULT hr = sipCpp->get_Interior(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_AutoScaleFont(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Interior()' failed with 0x%x", hr);
+                    "Call 'get_AutoScaleFont()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Interior, get=getInterior)
+        PyObject* setAutoScaleFont(VARIANT prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_AutoScaleFont(*a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_AutoScaleFont()' failed with 0x%x", hr);
+                sipRes = nullptr;
+            }
+            else
+            {
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
+            }
+        %End
 
-        VARIANT_BOOL getShadow();
+        %Property(name=AutoScaleFont, get=getAutoScaleFont, set=setAutoScaleFont)
+
+        VARIANT_BOOL getAutoSize();
         %MethodCode
             VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_Shadow(prop);
+            HRESULT hr = sipCpp->get_AutoSize(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Shadow()' failed with 0x%x", hr);
+                    "Call 'get_AutoSize()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setShadow(VARIANT_BOOL prop);
+        PyObject* setAutoSize(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Shadow(*a0);
+            HRESULT hr = sipCpp->put_AutoSize(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Shadow()' failed with 0x%x", hr);
+                    "Call 'put_AutoSize()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Shadow, get=getShadow, set=setShadow)
+        %Property(name=AutoSize, get=getAutoSize, set=setAutoSize)
 
-        VARIANT_BOOL getAutoLoad();
+        BSTR getCaption();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_AutoLoad(prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_Caption(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_AutoLoad()' failed with 0x%x", hr);
+                    "Call 'get_Caption()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setAutoLoad(VARIANT_BOOL prop);
+        PyObject* setCaption(BSTR prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_AutoLoad(*a0);
+            HRESULT hr = sipCpp->put_Caption(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_AutoLoad()' failed with 0x%x", hr);
+                    "Call 'put_Caption()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=AutoLoad, get=getAutoLoad, set=setAutoLoad)
+        %Property(name=Caption, get=getCaption, set=setCaption)
 
-        VARIANT_BOOL getAutoUpdate();
+        Font* getFont();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_AutoUpdate(prop);
+            etapi::Font *prop = nullptr;
+            HRESULT hr = sipCpp->get_Font(&prop);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_Font()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        %Property(name=Font, get=getFont)
+
+        BSTR getFormula();
+        %MethodCode
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_Formula(prop);
+            if (hr != S_OK)
+            {
+                delete prop;
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_Formula()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        PyObject* setFormula(BSTR prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_Formula(*a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_Formula()' failed with 0x%x", hr);
+                sipRes = nullptr;
+            }
+            else
+            {
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
+            }
+        %End
+
+        %Property(name=Formula, get=getFormula, set=setFormula)
+
+        VARIANT getHorizontalAlignment();
+        %MethodCode
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_HorizontalAlignment(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_AutoUpdate()' failed with 0x%x", hr);
+                    "Call 'get_HorizontalAlignment()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setAutoUpdate(VARIANT_BOOL prop);
+        PyObject* setHorizontalAlignment(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_AutoUpdate(*a0);
+            HRESULT hr = sipCpp->put_HorizontalAlignment(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_AutoUpdate()' failed with 0x%x", hr);
+                    "Call 'put_HorizontalAlignment()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=AutoUpdate, get=getAutoUpdate, set=setAutoUpdate)
+        %Property(name=HorizontalAlignment, get=getHorizontalAlignment, set=setHorizontalAlignment)
 
-        IDispatch* getObject();
+        VARIANT_BOOL getLockedText();
         %MethodCode
-            IDispatch *prop = nullptr;
-            HRESULT hr = sipCpp->get_Object(&prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_LockedText(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Object()' failed with 0x%x", hr);
+                    "Call 'get_LockedText()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Object, get=getObject)
+        PyObject* setLockedText(VARIANT_BOOL prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_LockedText(*a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_LockedText()' failed with 0x%x", hr);
+                sipRes = nullptr;
+            }
+            else
+            {
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
+            }
+        %End
+
+        %Property(name=LockedText, get=getLockedText, set=setLockedText)
 
-        VARIANT getOLEType();
+        VARIANT getOrientation();
         %MethodCode
             VARIANT *prop = new VARIANT;
             VariantInit(prop);
-            HRESULT hr = sipCpp->get_OLEType(prop);
+            HRESULT hr = sipCpp->get_Orientation(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_OLEType()' failed with 0x%x", hr);
+                    "Call 'get_Orientation()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=OLEType, get=getOLEType)
+        PyObject* setOrientation(VARIANT prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_Orientation(*a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_Orientation()' failed with 0x%x", hr);
+                sipRes = nullptr;
+            }
+            else
+            {
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
+            }
+        %End
+
+        %Property(name=Orientation, get=getOrientation, set=setOrientation)
 
-        BSTR getSourceName();
+        BSTR getText();
         %MethodCode
             BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_SourceName(prop);
+            HRESULT hr = sipCpp->get_Text(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_SourceName()' failed with 0x%x", hr);
+                    "Call 'get_Text()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setSourceName(BSTR prop);
+        PyObject* setText(BSTR prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_SourceName(*a0);
+            HRESULT hr = sipCpp->put_Text(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_SourceName()' failed with 0x%x", hr);
+                    "Call 'put_Text()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=SourceName, get=getSourceName, set=setSourceName)
+        %Property(name=Text, get=getText, set=setText)
 
-        BSTR getLinkedCell();
+        VARIANT getVerticalAlignment();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_LinkedCell(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_VerticalAlignment(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_LinkedCell()' failed with 0x%x", hr);
+                    "Call 'get_VerticalAlignment()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setLinkedCell(BSTR prop);
+        PyObject* setVerticalAlignment(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_LinkedCell(*a0);
+            HRESULT hr = sipCpp->put_VerticalAlignment(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_LinkedCell()' failed with 0x%x", hr);
+                    "Call 'put_VerticalAlignment()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=LinkedCell, get=getLinkedCell, set=setLinkedCell)
+        %Property(name=VerticalAlignment, get=getVerticalAlignment, set=setVerticalAlignment)
 
-        BSTR getListFillRange();
+        long getReadingOrder();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_ListFillRange(prop);
+            long prop = 0;
+            HRESULT hr = sipCpp->get_ReadingOrder(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ListFillRange()' failed with 0x%x", hr);
+                    "Call 'get_ReadingOrder()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setListFillRange(BSTR prop);
+        PyObject* setReadingOrder(long prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_ListFillRange(*a0);
+            HRESULT hr = sipCpp->put_ReadingOrder(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_ListFillRange()' failed with 0x%x", hr);
+                    "Call 'put_ReadingOrder()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=ListFillRange, get=getListFillRange, set=setListFillRange)
+        %Property(name=ReadingOrder, get=getReadingOrder, set=setReadingOrder)
 
-        BSTR getprogID();
+        Border* getBorder();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_progID(prop);
+            etapi::Border *prop = nullptr;
+            HRESULT hr = sipCpp->get_Border(&prop);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_Border()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        %Property(name=Border, get=getBorder)
+
+        Interior* getInterior();
+        %MethodCode
+            etapi::Interior *prop = nullptr;
+            HRESULT hr = sipCpp->get_Interior(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_progID()' failed with 0x%x", hr);
+                    "Call 'get_Interior()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=progID, get=getprogID)
+        %Property(name=Interior, get=getInterior)
 
-        BSTR getAltHTML();
+        VARIANT_BOOL getShadow();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_AltHTML(prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_Shadow(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_AltHTML()' failed with 0x%x", hr);
+                    "Call 'get_Shadow()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setAltHTML(BSTR prop);
+        PyObject* setShadow(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_AltHTML(*a0);
+            HRESULT hr = sipCpp->put_Shadow(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_AltHTML()' failed with 0x%x", hr);
+                    "Call 'put_Shadow()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=AltHTML, get=getAltHTML, set=setAltHTML)
+        %Property(name=Shadow, get=getShadow, set=setShadow)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISoundNote.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISoundNote.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISlicerCaches.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISlicerCaches.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPublishObjects.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPublishObjects.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotFilter.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotFilter.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IStyle.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IStyle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ShapeNodes.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ShapeNodes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IFormatConditions.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IFormatConditions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotCell.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotCell.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISmartTagActions.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISmartTagActions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDataLabel.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDataLabel.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IAutoRecover.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IAutoRecover.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IAction.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IAction.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotFormula.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotFormula.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITextBoxes.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITextBoxes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/enums.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/enums.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelTable.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelTable.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IRectangularGradient.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IRectangularGradient.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITickLabels.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITickLabels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotTableChangeList.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotTableChangeList.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IWalls.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISortField.sip`

 * *Files 11% similar despite different names*

```diff
@@ -6,63 +6,66 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct IWalls : public IDispatch /Abstract/
+    struct ISortField : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
 
-        virtual HRESULT get_Name(
-            BSTR *RHS /Out/) = 0;
+        virtual HRESULT get_SortOn(
+            XlSortOn *RHS /Out/) = 0;
 
-        virtual HRESULT Select(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT put_SortOn(
+            XlSortOn RHS) = 0;
 
-        virtual HRESULT get_Border(
-            Border **RHS /Out/) = 0;
+        virtual HRESULT get_SortOnValue(
+            IDispatch **RHS /Out/) = 0;
 
-        virtual HRESULT ClearFormats(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT get_Key(
+            Range **RHS /Out/) = 0;
 
-        virtual HRESULT get_Interior(
-            Interior **RHS /Out/) = 0;
+        virtual HRESULT get_Order(
+            XlSortOrder *RHS /Out/) = 0;
 
-        virtual HRESULT get_Fill(
-            ChartFillFormat **RHS /Out/) = 0;
+        virtual HRESULT put_Order(
+            XlSortOrder RHS) = 0;
 
-        virtual HRESULT get_PictureType(
+        virtual HRESULT get_CustomOrder(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_PictureType(
+        virtual HRESULT put_CustomOrder(
             VARIANT RHS) = 0;
 
-        virtual HRESULT Paste() = 0;
-
-        virtual HRESULT get_PictureUnit(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT get_DataOption(
+            XlSortDataOption *RHS /Out/) = 0;
 
-        virtual HRESULT put_PictureUnit(
-            VARIANT RHS) = 0;
+        virtual HRESULT put_DataOption(
+            XlSortDataOption RHS) = 0;
 
-        virtual HRESULT get_Thickness(
+        virtual HRESULT get_Priority(
             long *RHS /Out/) = 0;
 
-        virtual HRESULT put_Thickness(
+        virtual HRESULT put_Priority(
             long RHS) = 0;
 
-        virtual HRESULT get_Format(
-            ChartFormat **RHS /Out/) = 0;
+        virtual HRESULT Delete() = 0;
+
+        virtual HRESULT ModifyKey(
+            Range *Key) = 0;
+
+        virtual HRESULT SetIcon(
+            Icon *Icon) = 0;
 
         Application* getApplication();
         %MethodCode
             etapi::Application *prop = nullptr;
             HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
@@ -92,205 +95,216 @@
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Creator, get=getCreator)
 
-        BSTR getName();
+        XlSortOn getSortOn();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_Name(prop);
+            etapi::XlSortOn prop = (etapi::XlSortOn)0;
+            HRESULT hr = sipCpp->get_SortOn(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Name()' failed with 0x%x", hr);
+                    "Call 'get_SortOn()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Name, get=getName)
-
-        Border* getBorder();
+        PyObject* setSortOn(XlSortOn prop);
         %MethodCode
-            etapi::Border *prop = nullptr;
-            HRESULT hr = sipCpp->get_Border(&prop);
+            HRESULT hr = sipCpp->put_SortOn(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Border()' failed with 0x%x", hr);
-                return nullptr;
+                    "Call 'put_SortOn()' failed with 0x%x", hr);
+                sipRes = nullptr;
             }
             else
             {
-                sipRes = prop;
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
             }
         %End
 
-        %Property(name=Border, get=getBorder)
+        %Property(name=SortOn, get=getSortOn, set=setSortOn)
 
-        Interior* getInterior();
+        IDispatch* getSortOnValue();
         %MethodCode
-            etapi::Interior *prop = nullptr;
-            HRESULT hr = sipCpp->get_Interior(&prop);
+            IDispatch *prop = nullptr;
+            HRESULT hr = sipCpp->get_SortOnValue(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Interior()' failed with 0x%x", hr);
+                    "Call 'get_SortOnValue()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Interior, get=getInterior)
+        %Property(name=SortOnValue, get=getSortOnValue)
 
-        ChartFillFormat* getFill();
+        Range* getKey();
         %MethodCode
-            etapi::ChartFillFormat *prop = nullptr;
-            HRESULT hr = sipCpp->get_Fill(&prop);
+            etapi::Range *prop = nullptr;
+            HRESULT hr = sipCpp->get_Key(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Fill()' failed with 0x%x", hr);
+                    "Call 'get_Key()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Fill, get=getFill)
+        %Property(name=Key, get=getKey)
 
-        VARIANT getPictureType();
+        XlSortOrder getOrder();
         %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_PictureType(prop);
+            etapi::XlSortOrder prop = (etapi::XlSortOrder)0;
+            HRESULT hr = sipCpp->get_Order(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_PictureType()' failed with 0x%x", hr);
+                    "Call 'get_Order()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setPictureType(VARIANT prop);
+        PyObject* setOrder(XlSortOrder prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_PictureType(*a0);
+            HRESULT hr = sipCpp->put_Order(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_PictureType()' failed with 0x%x", hr);
+                    "Call 'put_Order()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=PictureType, get=getPictureType, set=setPictureType)
+        %Property(name=Order, get=getOrder, set=setOrder)
 
-        VARIANT getPictureUnit();
+        VARIANT getCustomOrder();
         %MethodCode
             VARIANT *prop = new VARIANT;
             VariantInit(prop);
-            HRESULT hr = sipCpp->get_PictureUnit(prop);
+            HRESULT hr = sipCpp->get_CustomOrder(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_PictureUnit()' failed with 0x%x", hr);
+                    "Call 'get_CustomOrder()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setPictureUnit(VARIANT prop);
+        PyObject* setCustomOrder(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_PictureUnit(*a0);
+            HRESULT hr = sipCpp->put_CustomOrder(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_PictureUnit()' failed with 0x%x", hr);
+                    "Call 'put_CustomOrder()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=PictureUnit, get=getPictureUnit, set=setPictureUnit)
+        %Property(name=CustomOrder, get=getCustomOrder, set=setCustomOrder)
 
-        long getThickness();
+        XlSortDataOption getDataOption();
         %MethodCode
-            long prop = 0;
-            HRESULT hr = sipCpp->get_Thickness(&prop);
+            etapi::XlSortDataOption prop = (etapi::XlSortDataOption)0;
+            HRESULT hr = sipCpp->get_DataOption(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Thickness()' failed with 0x%x", hr);
+                    "Call 'get_DataOption()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setThickness(long prop);
+        PyObject* setDataOption(XlSortDataOption prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Thickness(a0);
+            HRESULT hr = sipCpp->put_DataOption(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Thickness()' failed with 0x%x", hr);
+                    "Call 'put_DataOption()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Thickness, get=getThickness, set=setThickness)
+        %Property(name=DataOption, get=getDataOption, set=setDataOption)
 
-        ChartFormat* getFormat();
+        long getPriority();
         %MethodCode
-            etapi::ChartFormat *prop = nullptr;
-            HRESULT hr = sipCpp->get_Format(&prop);
+            long prop = 0;
+            HRESULT hr = sipCpp->get_Priority(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Format()' failed with 0x%x", hr);
+                    "Call 'get_Priority()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Format, get=getFormat)
+        PyObject* setPriority(long prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_Priority(a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_Priority()' failed with 0x%x", hr);
+                sipRes = nullptr;
+            }
+            else
+            {
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
+            }
+        %End
+
+        %Property(name=Priority, get=getPriority, set=setPriority)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDrawings.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDrawings.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IMenuItem.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IMenuItem.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IConditionValue.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IConditionValue.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ILegend.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ILegend.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IFormatColor.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IFormatColor.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotItems.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IUsedObjects.sip`

 * *Files 7% similar despite different names*

```diff
@@ -6,45 +6,46 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct IPivotItems : public IDispatch /Abstract/
+    struct IUsedObjects : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
 
-        virtual HRESULT Add(
-            BSTR Name) = 0;
-
         virtual HRESULT get_Count(
             long *RHS /Out/) = 0;
 
         Py_ssize_t __len__() const;
         %MethodCode
             long count = 0;
             if (sipCpp->get_Count(&count) != S_OK)
                 count = 0;
             sipRes = count;
         %End
 
-        virtual HRESULT Item(
+        virtual HRESULT get__Default(
+            VARIANT Index,
+            IDispatch **RHS /Out/) = 0;
+
+        virtual HRESULT get_Item(
             VARIANT Index,
             IDispatch **RHS /Out/) = 0;
 
         IDispatch* __getitem__(VARIANT index) const;
         %MethodCode
             IDispatch *prop = nullptr;
-            if (sipCpp->Item(*a0, &prop) != S_OK)
+            if (sipCpp->get_Item(*a0, &prop) != S_OK)
                 sipIsErr = 1;
             else
                 sipRes = prop;
         %End
 
         Application* getApplication();
         %MethodCode
@@ -78,30 +79,14 @@
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Creator, get=getCreator)
 
-        PivotField* getParent();
-        %MethodCode
-            etapi::PivotField *prop = nullptr;
-            HRESULT hr = sipCpp->get_Parent(&prop);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Parent()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
         long getCount();
         %MethodCode
             long prop = 0;
             HRESULT hr = sipCpp->get_Count(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
@@ -111,9 +96,10 @@
             else
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Count, get=getCount)
+
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IProtectedViewWindow.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IProtectedViewWindow.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IStyles.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IStyles.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IColorScaleCriteria.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IColorScaleCriteria.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDialog.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDialog.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITableObject.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITableObject.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDialogs.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDialogs.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IScenario.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IScenario.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IKRpcClient.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IKRpcClient.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IScrollBar.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IScrollBar.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISparkVerticalAxis.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISparkVerticalAxis.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/PictureFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/PictureFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPictures.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPictures.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPage.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPage.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IGroupObject.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IGroupObject.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IGroupBoxes.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IGroupBoxes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelRelationships.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelRelationships.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/TextEffectFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/TextEffectFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IWorksheetView.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IBorders.sip`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,97 @@
 /**
- * Copyright (c) 2020 Weitian Leung
+ * Copyright (c) 2020-2021 Weitian Leung
  *
  * This file is part of pywpsrpc.
  *
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct IWorksheetView : public IDispatch /Abstract/
+    struct IBorders : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
 
-        virtual HRESULT get_Sheet(
-            _Worksheet **RHS /Out/) = 0;
+        virtual HRESULT get_Color(
+            VARIANT *RHS /Out/) = 0;
+
+        virtual HRESULT put_Color(
+            VARIANT RHS) = 0;
+
+        virtual HRESULT get_ColorIndex(
+            VARIANT *RHS /Out/) = 0;
+
+        virtual HRESULT put_ColorIndex(
+            VARIANT RHS) = 0;
+
+        virtual HRESULT get_Count(
+            long *RHS /Out/) = 0;
+
+        Py_ssize_t __len__() const;
         %MethodCode
-            sipRes = sipCpp->get_Sheet((IDispatch**)&a0);
+            long count = 0;
+            if (sipCpp->get_Count(&count) != S_OK)
+                count = 0;
+            sipRes = count;
         %End
 
-        virtual HRESULT get_DisplayGridlines(
-            VARIANT_BOOL *RHS /Out/) = 0;
+        virtual HRESULT get_Item(
+            XlBordersIndex Index,
+            Border **RHS /Out/) = 0;
 
-        virtual HRESULT put_DisplayGridlines(
-            VARIANT_BOOL RHS) = 0;
+        Border* __getitem__(XlBordersIndex index) const;
+        %MethodCode
+            etapi::Border *prop = nullptr;
+            if (sipCpp->get_Item(a0, &prop) != S_OK)
+                sipIsErr = 1;
+            else
+                sipRes = prop;
+        %End
 
-        virtual HRESULT get_DisplayFormulas(
-            VARIANT_BOOL *RHS /Out/) = 0;
+        virtual HRESULT get_LineStyle(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_DisplayFormulas(
-            VARIANT_BOOL RHS) = 0;
+        virtual HRESULT put_LineStyle(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_DisplayHeadings(
-            VARIANT_BOOL *RHS /Out/) = 0;
+        virtual HRESULT get_Value(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_DisplayHeadings(
-            VARIANT_BOOL RHS) = 0;
+        virtual HRESULT put_Value(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_DisplayOutline(
-            VARIANT_BOOL *RHS /Out/) = 0;
+        virtual HRESULT get_Weight(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_DisplayOutline(
-            VARIANT_BOOL RHS) = 0;
+        virtual HRESULT put_Weight(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_DisplayZeros(
-            VARIANT_BOOL *RHS /Out/) = 0;
+        virtual HRESULT get__Default(
+            XlBordersIndex Index,
+            Border **RHS /Out/) = 0;
 
-        virtual HRESULT put_DisplayZeros(
-            VARIANT_BOOL RHS) = 0;
+        virtual HRESULT get_ThemeColor(
+            VARIANT *RHS /Out/) = 0;
+
+        virtual HRESULT put_ThemeColor(
+            VARIANT RHS) = 0;
+
+        virtual HRESULT get_TintAndShade(
+            VARIANT *RHS /Out/) = 0;
+
+        virtual HRESULT put_TintAndShade(
+            VARIANT RHS) = 0;
 
         Application* getApplication();
         %MethodCode
             etapi::Application *prop = nullptr;
             HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
@@ -87,201 +121,278 @@
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Creator, get=getCreator)
 
-        _Worksheet* getSheet();
+        VARIANT getColor();
+        %MethodCode
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Color(prop);
+            if (hr != S_OK)
+            {
+                delete prop;
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_Color()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        PyObject* setColor(VARIANT prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_Color(*a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_Color()' failed with 0x%x", hr);
+                sipRes = nullptr;
+            }
+            else
+            {
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
+            }
+        %End
+
+        %Property(name=Color, get=getColor, set=setColor)
+
+        VARIANT getColorIndex();
+        %MethodCode
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_ColorIndex(prop);
+            if (hr != S_OK)
+            {
+                delete prop;
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_ColorIndex()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        PyObject* setColorIndex(VARIANT prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_ColorIndex(*a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_ColorIndex()' failed with 0x%x", hr);
+                sipRes = nullptr;
+            }
+            else
+            {
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
+            }
+        %End
+
+        %Property(name=ColorIndex, get=getColorIndex, set=setColorIndex)
+
+        long getCount();
         %MethodCode
-            etapi::_Worksheet *prop = nullptr;
-            HRESULT hr = sipCpp->get_Sheet((IDispatch**)&prop);
+            long prop = 0;
+            HRESULT hr = sipCpp->get_Count(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Sheet()' failed with 0x%x", hr);
+                    "Call 'get_Count()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Sheet, get=getSheet)
+        %Property(name=Count, get=getCount)
 
-        VARIANT_BOOL getDisplayGridlines();
+        VARIANT getLineStyle();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_DisplayGridlines(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_LineStyle(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_DisplayGridlines()' failed with 0x%x", hr);
+                    "Call 'get_LineStyle()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setDisplayGridlines(VARIANT_BOOL prop);
+        PyObject* setLineStyle(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_DisplayGridlines(*a0);
+            HRESULT hr = sipCpp->put_LineStyle(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_DisplayGridlines()' failed with 0x%x", hr);
+                    "Call 'put_LineStyle()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=DisplayGridlines, get=getDisplayGridlines, set=setDisplayGridlines)
+        %Property(name=LineStyle, get=getLineStyle, set=setLineStyle)
 
-        VARIANT_BOOL getDisplayFormulas();
+        VARIANT getValue();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_DisplayFormulas(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Value(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_DisplayFormulas()' failed with 0x%x", hr);
+                    "Call 'get_Value()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setDisplayFormulas(VARIANT_BOOL prop);
+        PyObject* setValue(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_DisplayFormulas(*a0);
+            HRESULT hr = sipCpp->put_Value(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_DisplayFormulas()' failed with 0x%x", hr);
+                    "Call 'put_Value()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=DisplayFormulas, get=getDisplayFormulas, set=setDisplayFormulas)
+        %Property(name=Value, get=getValue, set=setValue)
 
-        VARIANT_BOOL getDisplayHeadings();
+        VARIANT getWeight();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_DisplayHeadings(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Weight(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_DisplayHeadings()' failed with 0x%x", hr);
+                    "Call 'get_Weight()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setDisplayHeadings(VARIANT_BOOL prop);
+        PyObject* setWeight(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_DisplayHeadings(*a0);
+            HRESULT hr = sipCpp->put_Weight(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_DisplayHeadings()' failed with 0x%x", hr);
+                    "Call 'put_Weight()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=DisplayHeadings, get=getDisplayHeadings, set=setDisplayHeadings)
+        %Property(name=Weight, get=getWeight, set=setWeight)
 
-        VARIANT_BOOL getDisplayOutline();
+        VARIANT getThemeColor();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_DisplayOutline(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_ThemeColor(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_DisplayOutline()' failed with 0x%x", hr);
+                    "Call 'get_ThemeColor()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setDisplayOutline(VARIANT_BOOL prop);
+        PyObject* setThemeColor(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_DisplayOutline(*a0);
+            HRESULT hr = sipCpp->put_ThemeColor(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_DisplayOutline()' failed with 0x%x", hr);
+                    "Call 'put_ThemeColor()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=DisplayOutline, get=getDisplayOutline, set=setDisplayOutline)
+        %Property(name=ThemeColor, get=getThemeColor, set=setThemeColor)
 
-        VARIANT_BOOL getDisplayZeros();
+        VARIANT getTintAndShade();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_DisplayZeros(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_TintAndShade(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_DisplayZeros()' failed with 0x%x", hr);
+                    "Call 'get_TintAndShade()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setDisplayZeros(VARIANT_BOOL prop);
+        PyObject* setTintAndShade(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_DisplayZeros(*a0);
+            HRESULT hr = sipCpp->put_TintAndShade(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_DisplayZeros()' failed with 0x%x", hr);
+                    "Call 'put_TintAndShade()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=DisplayZeros, get=getDisplayZeros, set=setDisplayZeros)
+        %Property(name=TintAndShade, get=getTintAndShade, set=setTintAndShade)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModuleView.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModuleView.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IAppEvents.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IAppEvents.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/DiagramNodes.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/DiagramNodes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDatabar.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDatabar.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IWorkbookConnection.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IWorkbookConnection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISlicerItem.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISlicerItem.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ICharts.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ICharts.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IAxisTitle.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IAxisTitle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IUniqueValues.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IUniqueValues.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ThreeDFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ThreeDFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/_Worksheet.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/_Worksheet.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ColorFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ColorFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IVPageBreak.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IVPageBreak.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IEditBoxes.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IEditBoxes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/CubeField.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/CubeField.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IChartArea.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IChartArea.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IWorkbookEvents.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IWorkbookEvents.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IXmlNamespace.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IXmlNamespace.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISeriesCollection.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISeriesCollection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ILegendKey.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ILegendKey.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IChartFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IChartFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IRectangle.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IRectangle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelMeasureNames.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelMeasureNames.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IXmlSchema.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IXmlSchema.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/_Application.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/_Application.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IOutline.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IOutline.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ICustomViews.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ICustomViews.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IOvals.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IOvals.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IHPageBreak.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IHPageBreak.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IScenarios.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IScenarios.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/DiagramNode.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/DiagramNode.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISortField.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IHyperlink.sip`

 * *Files 17% similar despite different names*

```diff
@@ -6,66 +6,80 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct ISortField : public IDispatch /Abstract/
+    struct IHyperlink : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
 
-        virtual HRESULT get_SortOn(
-            XlSortOn *RHS /Out/) = 0;
+        virtual HRESULT get_Name(
+            BSTR *RHS /Out/) = 0;
 
-        virtual HRESULT put_SortOn(
-            XlSortOn RHS) = 0;
-
-        virtual HRESULT get_SortOnValue(
-            IDispatch **RHS /Out/) = 0;
-
-        virtual HRESULT get_Key(
+        virtual HRESULT get_Range(
             Range **RHS /Out/) = 0;
 
-        virtual HRESULT get_Order(
-            XlSortOrder *RHS /Out/) = 0;
-
-        virtual HRESULT put_Order(
-            XlSortOrder RHS) = 0;
+        virtual HRESULT get_Shape(
+            Shape **RHS /Out/) = 0;
 
-        virtual HRESULT get_CustomOrder(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT get_SubAddress(
+            BSTR *RHS /Out/) = 0;
 
-        virtual HRESULT put_CustomOrder(
-            VARIANT RHS) = 0;
+        virtual HRESULT put_SubAddress(
+            BSTR RHS) = 0;
 
-        virtual HRESULT get_DataOption(
-            XlSortDataOption *RHS /Out/) = 0;
+        virtual HRESULT get_Address(
+            BSTR *RHS /Out/) = 0;
 
-        virtual HRESULT put_DataOption(
-            XlSortDataOption RHS) = 0;
+        virtual HRESULT put_Address(
+            BSTR RHS) = 0;
 
-        virtual HRESULT get_Priority(
+        virtual HRESULT get_Type(
             long *RHS /Out/) = 0;
 
-        virtual HRESULT put_Priority(
-            long RHS) = 0;
+        virtual HRESULT AddToFavorites() = 0;
 
         virtual HRESULT Delete() = 0;
 
-        virtual HRESULT ModifyKey(
-            Range *Key) = 0;
-
-        virtual HRESULT SetIcon(
-            Icon *Icon) = 0;
+        virtual HRESULT Follow(
+            VARIANT NewWindow = argMissing2(),
+            VARIANT AddHistory = argMissing2(),
+            VARIANT ExtraInfo = argMissing2(),
+            VARIANT Method = argMissing2(),
+            VARIANT HeaderInfo = argMissing2()) = 0;
+
+        virtual HRESULT get_EmailSubject(
+            BSTR *RHS /Out/) = 0;
+
+        virtual HRESULT put_EmailSubject(
+            BSTR RHS) = 0;
+
+        virtual HRESULT get_ScreenTip(
+            BSTR *RHS /Out/) = 0;
+
+        virtual HRESULT put_ScreenTip(
+            BSTR RHS) = 0;
+
+        virtual HRESULT get_TextToDisplay(
+            BSTR *RHS /Out/) = 0;
+
+        virtual HRESULT put_TextToDisplay(
+            BSTR RHS) = 0;
+
+        virtual HRESULT CreateNewDocument(
+            BSTR Filename,
+            VARIANT_BOOL EditNow,
+            VARIANT_BOOL Overwrite) = 0;
 
         Application* getApplication();
         %MethodCode
             etapi::Application *prop = nullptr;
             HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
@@ -95,216 +109,256 @@
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Creator, get=getCreator)
 
-        XlSortOn getSortOn();
+        BSTR getName();
         %MethodCode
-            etapi::XlSortOn prop = (etapi::XlSortOn)0;
-            HRESULT hr = sipCpp->get_SortOn(&prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_Name(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_SortOn()' failed with 0x%x", hr);
+                    "Call 'get_Name()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setSortOn(XlSortOn prop);
+        %Property(name=Name, get=getName)
+
+        Range* getRange();
         %MethodCode
-            HRESULT hr = sipCpp->put_SortOn(a0);
+            etapi::Range *prop = nullptr;
+            HRESULT hr = sipCpp->get_Range(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_SortOn()' failed with 0x%x", hr);
-                sipRes = nullptr;
+                    "Call 'get_Range()' failed with 0x%x", hr);
+                return nullptr;
             }
             else
             {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
+                sipRes = prop;
             }
         %End
 
-        %Property(name=SortOn, get=getSortOn, set=setSortOn)
+        %Property(name=Range, get=getRange)
 
-        IDispatch* getSortOnValue();
+        Shape* getShape();
         %MethodCode
-            IDispatch *prop = nullptr;
-            HRESULT hr = sipCpp->get_SortOnValue(&prop);
+            etapi::Shape *prop = nullptr;
+            HRESULT hr = sipCpp->get_Shape(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_SortOnValue()' failed with 0x%x", hr);
+                    "Call 'get_Shape()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=SortOnValue, get=getSortOnValue)
+        %Property(name=Shape, get=getShape)
 
-        Range* getKey();
+        BSTR getSubAddress();
         %MethodCode
-            etapi::Range *prop = nullptr;
-            HRESULT hr = sipCpp->get_Key(&prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_SubAddress(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Key()' failed with 0x%x", hr);
+                    "Call 'get_SubAddress()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Key, get=getKey)
+        PyObject* setSubAddress(BSTR prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_SubAddress(*a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_SubAddress()' failed with 0x%x", hr);
+                sipRes = nullptr;
+            }
+            else
+            {
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
+            }
+        %End
 
-        XlSortOrder getOrder();
+        %Property(name=SubAddress, get=getSubAddress, set=setSubAddress)
+
+        BSTR getAddress();
         %MethodCode
-            etapi::XlSortOrder prop = (etapi::XlSortOrder)0;
-            HRESULT hr = sipCpp->get_Order(&prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_Address(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Order()' failed with 0x%x", hr);
+                    "Call 'get_Address()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setOrder(XlSortOrder prop);
+        PyObject* setAddress(BSTR prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Order(a0);
+            HRESULT hr = sipCpp->put_Address(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Order()' failed with 0x%x", hr);
+                    "Call 'put_Address()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Order, get=getOrder, set=setOrder)
+        %Property(name=Address, get=getAddress, set=setAddress)
+
+        long getType();
+        %MethodCode
+            long prop = 0;
+            HRESULT hr = sipCpp->get_Type(&prop);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_Type()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        %Property(name=Type, get=getType)
 
-        VARIANT getCustomOrder();
+        BSTR getEmailSubject();
         %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_CustomOrder(prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_EmailSubject(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_CustomOrder()' failed with 0x%x", hr);
+                    "Call 'get_EmailSubject()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setCustomOrder(VARIANT prop);
+        PyObject* setEmailSubject(BSTR prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_CustomOrder(*a0);
+            HRESULT hr = sipCpp->put_EmailSubject(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_CustomOrder()' failed with 0x%x", hr);
+                    "Call 'put_EmailSubject()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=CustomOrder, get=getCustomOrder, set=setCustomOrder)
+        %Property(name=EmailSubject, get=getEmailSubject, set=setEmailSubject)
 
-        XlSortDataOption getDataOption();
+        BSTR getScreenTip();
         %MethodCode
-            etapi::XlSortDataOption prop = (etapi::XlSortDataOption)0;
-            HRESULT hr = sipCpp->get_DataOption(&prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_ScreenTip(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_DataOption()' failed with 0x%x", hr);
+                    "Call 'get_ScreenTip()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setDataOption(XlSortDataOption prop);
+        PyObject* setScreenTip(BSTR prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_DataOption(a0);
+            HRESULT hr = sipCpp->put_ScreenTip(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_DataOption()' failed with 0x%x", hr);
+                    "Call 'put_ScreenTip()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=DataOption, get=getDataOption, set=setDataOption)
+        %Property(name=ScreenTip, get=getScreenTip, set=setScreenTip)
 
-        long getPriority();
+        BSTR getTextToDisplay();
         %MethodCode
-            long prop = 0;
-            HRESULT hr = sipCpp->get_Priority(&prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_TextToDisplay(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Priority()' failed with 0x%x", hr);
+                    "Call 'get_TextToDisplay()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setPriority(long prop);
+        PyObject* setTextToDisplay(BSTR prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Priority(a0);
+            HRESULT hr = sipCpp->put_TextToDisplay(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Priority()' failed with 0x%x", hr);
+                    "Call 'put_TextToDisplay()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Priority, get=getPriority, set=setPriority)
+        %Property(name=TextToDisplay, get=getTextToDisplay, set=setTextToDisplay)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IVPageBreaks.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IVPageBreaks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IHeaderFooter.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IHeaderFooter.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IAutoFilter.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IAutoFilter.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IButtons.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IButtons.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotCaches.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotCaches.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IMenuItems.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IMenuItems.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDialogSheets.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDialogSheets.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotField.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotField.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * Copyright (c) 2020 Weitian Leung
+ * Copyright (c) 2020-2023 Weitian Leung
  *
  * This file is part of pywpsrpc.
  *
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
@@ -95,15 +95,47 @@
 
         virtual HRESULT get_ParentItems(
             VARIANT Index = argMissing2(),
             VARIANT *RHS /Out/ = 0) = 0;
 
         virtual HRESULT PivotItems(
             VARIANT Index = argMissing2(),
-            VARIANT *RHS /Out/ = 0) = 0;
+            etapi::IPivotItems **RHS /Out/ = 0) = 0;
+        %MethodCode
+            VARIANT var;
+            VariantInit(&var);
+            sipRes = sipCpp->PivotItems(*a0, &var);
+
+            bool unsupported = false;
+            do
+            {
+                if (sipRes != S_OK)
+                    break;
+                if (V_VT(&var) != VT_DISPATCH)
+                {
+                    unsupported = true;
+                    break;
+                }
+
+                HRESULT hr = V_DISPATCH(&var)->QueryInterface(etapi::IID_IPivotItems, (void**)&a1);
+                if (hr == S_OK)
+                    break;
+
+                // MSDN says it could be PivotItems or PivotItem
+                // but when will PivotItem?
+
+                sipRes = hr;
+                unsupported = true;
+            } while (0);
+
+            VariantClear(&var);
+
+            if (unsupported)
+                PyErr_Format(PyExc_TypeError, "Unexpected type returns from PivotItems");
+        %End
 
         virtual HRESULT get_Position(
             VARIANT *RHS /Out/) = 0;
 
         virtual HRESULT put_Position(
             VARIANT RHS) = 0;
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDataFeedConnection.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDataFeedConnection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IChartFillFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IChartFillFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITableStyleElements.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITableStyleElements.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/LineFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/LineFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/Workbooks.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/Workbooks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IScrollBars.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IScrollBars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IParameters.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IParameters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelRelationship.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelRelationship.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IWorksheets.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IWorksheets.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/Sheets.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/Sheets.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IUpBars.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IUpBars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IWatches.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IWatches.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/_Chart.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/_Chart.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotLines.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IOptionButtons.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IOptionButtons.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelColumnChanges.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelColumnChanges.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IFloor.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IFloor.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IConnections.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IConnections.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ICategoryCollection.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ICategoryCollection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IErrorBars.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IErrorBars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IFileExportConverters.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IFileExportConverters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IWindow.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IWindow.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotTable.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotTable.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IChartEvents.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IChartEvents.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IToolbarButton.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IToolbarButton.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IHPageBreaks.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IHPageBreaks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IHyperlinks.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IHyperlinks.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IWindows.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IWindows.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IChartView.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IChartView.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDropLines.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDropLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITrendlines.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITrendlines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IValidation.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IValidation.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IListColumn.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IListColumn.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/WebOptions.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/WebOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISmartTagRecognizer.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISmartTagRecognizer.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IMailer.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IMailer.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IListRow.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IListRow.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IFullSeriesCollection.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IFullSeriesCollection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPanes.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPanes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IHiLoLines.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IHiLoLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IQuickAnalysis.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IQuickAnalysis.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ShadowFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ShadowFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDropDowns.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDropDowns.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDropDown.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDropDown.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISparkColor.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISparkColor.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/_DebugTools.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/_DebugTools.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IOval.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IArc.sip`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct IOval : public IDispatch /Abstract/
+    struct IArc : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
@@ -210,19 +210,15 @@
 
         virtual HRESULT get_Border(
             Border **RHS /Out/) = 0;
 
         virtual HRESULT get_Interior(
             Interior **RHS /Out/) = 0;
 
-        virtual HRESULT get_Shadow(
-            VARIANT_BOOL *RHS /Out/) = 0;
-
-        virtual HRESULT put_Shadow(
-            VARIANT_BOOL RHS) = 0;
+        virtual void _Dummy43() = 0;
 
         Application* getApplication();
         %MethodCode
             etapi::Application *prop = nullptr;
             HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
@@ -1165,44 +1161,9 @@
             else
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Interior, get=getInterior)
-
-        VARIANT_BOOL getShadow();
-        %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_Shadow(prop);
-            if (hr != S_OK)
-            {
-                delete prop;
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Shadow()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        PyObject* setShadow(VARIANT_BOOL prop);
-        %MethodCode
-            HRESULT hr = sipCpp->put_Shadow(*a0);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Shadow()' failed with 0x%x", hr);
-                sipRes = nullptr;
-            }
-            else
-            {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
-            }
-        %End
-
-        %Property(name=Shadow, get=getShadow, set=setShadow)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotLineCells.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotLineCells.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISeries.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISeries.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDownBars.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDownBars.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IOptionButton.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IOptionButton.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISlicerCacheLevels.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISlicerCacheLevels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IChartObject.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IChartObject.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IAxes.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IAxes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotFormulas.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotFormulas.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISeriesLines.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISeriesLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDialogSheetView.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDialogSheetView.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotValueCell.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotValueCell.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ICalculatedMembers.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ICalculatedMembers.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IODBCError.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IODBCError.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelTableNameChanges.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelTableNameChanges.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ILine.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ILine.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ILeaderLines.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ILeaderLines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IChartObjects.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IChartObjects.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/_IQueryTable.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/_IQueryTable.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITableStyle.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITableStyle.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/_Workbook.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/_Workbook.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotAxis.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotAxis.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IActions.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IActions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotItemList.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotItemList.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IXmlMaps.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IXmlMaps.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IRecentFiles.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IRecentFiles.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelChanges.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelChanges.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISortFields.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISortFields.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ILinearGradient.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ILinearGradient.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IMenuBar.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IMenuBar.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISmartTagRecognizers.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISmartTagRecognizers.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/INames.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/INames.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/INegativeBarFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/INegativeBarFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IErrors.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IErrors.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IWorksheetDataConnection.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IWorksheetDataConnection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/TreeviewControl.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/TreeviewControl.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDiagram.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDiagram.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IName.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IName.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ICheckBox.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ICheckBox.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModules.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModules.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPane.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPane.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPageSetup.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPageSetup.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IAxis.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IAxis.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IXmlMap.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IXmlMap.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IRectangles.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IRectangles.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISlicer.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISlicer.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISparklineGroups.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISparklineGroups.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IXPath.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IXPath.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IFileExportConverter.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IFileExportConverter.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/TextFrame2.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/TextFrame2.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IArcs.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IArcs.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotTables.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotTables.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IRTD.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IRTD.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITextConnection.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITextConnection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IButton.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IButton.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITimelineViewState.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITimelineViewState.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITextBox.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITextBox.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDummy.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDummy.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ICorners.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ICorners.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IInterior.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IInterior.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IChartGroup.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IChartGroup.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/rpcetapi.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/rpcetapi.sip`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,14 @@
 %Include IModelMeasureName.sip
 %Include IModelMeasureNames.sip
 %Include WorksheetFunction.sip
 %Include IDummy.sip
 %Include ICanvasShapes.sip
 %Include _DebugTools.sip
 %Include Solver.sip
-%Include IEXCELCtrlExtender.sip
 
 namespace etapi
 {
     typedef _Application Application;
     typedef _Chart Chart;
     typedef _IOLEObject OLEObject;
     typedef _IQueryTable QueryTable;
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotFilters.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotFilters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IFilters.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IFilters.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDialogSheet.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDialogSheet.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPages.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPages.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelColumnNames.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelColumnNames.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IFormatCondition.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IFormatCondition.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITimelineState.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITimelineState.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISparklineGroup.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISparklineGroup.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IModelConnection.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelConnection.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDataLabels.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDataLabels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ILines.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ILines.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IIconSets.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IIconSets.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISlicerItems.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISlicerItems.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ICellFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ICellFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IControlFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IControlFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ICustomProperties.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ICustomProperties.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISmartTagOptions.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISmartTagOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IEditBox.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IEditBox.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ILabels.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ILabels.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ShapeNode.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ShapeNode.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IGroupBox.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IGroupBox.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISpeech.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISpeech.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IBorder.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDisplayFormat.sip`

 * *Files 18% similar despite different names*

```diff
@@ -6,58 +6,79 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct IBorder : public IDispatch /Abstract/
+    struct IDisplayFormat : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
 
-        virtual HRESULT get_Color(
+        virtual HRESULT get_Borders(
+            Borders **RHS /Out/) = 0;
+
+        virtual HRESULT get_Characters(
+            VARIANT Start = argMissing2(),
+            VARIANT Length = argMissing2(),
+            Characters **RHS /Out/ = 0) = 0;
+
+        virtual HRESULT get_Font(
+            Font **RHS /Out/) = 0;
+
+        virtual HRESULT get_Style(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Color(
-            VARIANT RHS) = 0;
+        virtual HRESULT get_AddIndent(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_ColorIndex(
+        virtual HRESULT get_FormulaHidden(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_ColorIndex(
-            VARIANT RHS) = 0;
+        virtual HRESULT get_HorizontalAlignment(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_LineStyle(
+        virtual HRESULT get_IndentLevel(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_LineStyle(
-            VARIANT RHS) = 0;
+        virtual HRESULT get_Interior(
+            Interior **RHS /Out/) = 0;
 
-        virtual HRESULT get_Weight(
+        virtual HRESULT get_Locked(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Weight(
-            VARIANT RHS) = 0;
+        virtual HRESULT get_MergeCells(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_ThemeColor(
+        virtual HRESULT get_NumberFormat(
+            long lcidIn,
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_ThemeColor(
-            VARIANT RHS) = 0;
+        virtual HRESULT get_NumberFormatLocal(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_TintAndShade(
+        virtual HRESULT get_Orientation(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_TintAndShade(
-            VARIANT RHS) = 0;
+        virtual HRESULT get_ReadingOrder(
+            long *RHS /Out/) = 0;
+
+        virtual HRESULT get_ShrinkToFit(
+            VARIANT *RHS /Out/) = 0;
+
+        virtual HRESULT get_VerticalAlignment(
+            VARIANT *RHS /Out/) = 0;
+
+        virtual HRESULT get_WrapText(
+            VARIANT *RHS /Out/) = 0;
 
         Application* getApplication();
         %MethodCode
             etapi::Application *prop = nullptr;
             HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
@@ -87,224 +108,320 @@
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Creator, get=getCreator)
 
-        VARIANT getColor();
+        Borders* getBorders();
+        %MethodCode
+            etapi::Borders *prop = nullptr;
+            HRESULT hr = sipCpp->get_Borders(&prop);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_Borders()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        %Property(name=Borders, get=getBorders)
+
+        Font* getFont();
+        %MethodCode
+            etapi::Font *prop = nullptr;
+            HRESULT hr = sipCpp->get_Font(&prop);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_Font()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        %Property(name=Font, get=getFont)
+
+        VARIANT getStyle();
         %MethodCode
             VARIANT *prop = new VARIANT;
             VariantInit(prop);
-            HRESULT hr = sipCpp->get_Color(prop);
+            HRESULT hr = sipCpp->get_Style(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Color()' failed with 0x%x", hr);
+                    "Call 'get_Style()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setColor(VARIANT prop);
+        %Property(name=Style, get=getStyle)
+
+        VARIANT getAddIndent();
         %MethodCode
-            HRESULT hr = sipCpp->put_Color(*a0);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_AddIndent(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Color()' failed with 0x%x", hr);
-                sipRes = nullptr;
+                    "Call 'get_AddIndent()' failed with 0x%x", hr);
+                return nullptr;
             }
             else
             {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
+                sipRes = prop;
             }
         %End
 
-        %Property(name=Color, get=getColor, set=setColor)
+        %Property(name=AddIndent, get=getAddIndent)
 
-        VARIANT getColorIndex();
+        VARIANT getFormulaHidden();
         %MethodCode
             VARIANT *prop = new VARIANT;
             VariantInit(prop);
-            HRESULT hr = sipCpp->get_ColorIndex(prop);
+            HRESULT hr = sipCpp->get_FormulaHidden(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ColorIndex()' failed with 0x%x", hr);
+                    "Call 'get_FormulaHidden()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setColorIndex(VARIANT prop);
+        %Property(name=FormulaHidden, get=getFormulaHidden)
+
+        VARIANT getHorizontalAlignment();
         %MethodCode
-            HRESULT hr = sipCpp->put_ColorIndex(*a0);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_HorizontalAlignment(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_ColorIndex()' failed with 0x%x", hr);
-                sipRes = nullptr;
+                    "Call 'get_HorizontalAlignment()' failed with 0x%x", hr);
+                return nullptr;
             }
             else
             {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
+                sipRes = prop;
             }
         %End
 
-        %Property(name=ColorIndex, get=getColorIndex, set=setColorIndex)
+        %Property(name=HorizontalAlignment, get=getHorizontalAlignment)
 
-        VARIANT getLineStyle();
+        VARIANT getIndentLevel();
         %MethodCode
             VARIANT *prop = new VARIANT;
             VariantInit(prop);
-            HRESULT hr = sipCpp->get_LineStyle(prop);
+            HRESULT hr = sipCpp->get_IndentLevel(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_LineStyle()' failed with 0x%x", hr);
+                    "Call 'get_IndentLevel()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setLineStyle(VARIANT prop);
+        %Property(name=IndentLevel, get=getIndentLevel)
+
+        Interior* getInterior();
         %MethodCode
-            HRESULT hr = sipCpp->put_LineStyle(*a0);
+            etapi::Interior *prop = nullptr;
+            HRESULT hr = sipCpp->get_Interior(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_LineStyle()' failed with 0x%x", hr);
-                sipRes = nullptr;
+                    "Call 'get_Interior()' failed with 0x%x", hr);
+                return nullptr;
             }
             else
             {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
+                sipRes = prop;
             }
         %End
 
-        %Property(name=LineStyle, get=getLineStyle, set=setLineStyle)
+        %Property(name=Interior, get=getInterior)
 
-        VARIANT getWeight();
+        VARIANT getLocked();
         %MethodCode
             VARIANT *prop = new VARIANT;
             VariantInit(prop);
-            HRESULT hr = sipCpp->get_Weight(prop);
+            HRESULT hr = sipCpp->get_Locked(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Weight()' failed with 0x%x", hr);
+                    "Call 'get_Locked()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setWeight(VARIANT prop);
+        %Property(name=Locked, get=getLocked)
+
+        VARIANT getMergeCells();
         %MethodCode
-            HRESULT hr = sipCpp->put_Weight(*a0);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_MergeCells(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Weight()' failed with 0x%x", hr);
-                sipRes = nullptr;
+                    "Call 'get_MergeCells()' failed with 0x%x", hr);
+                return nullptr;
             }
             else
             {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
+                sipRes = prop;
+            }
+        %End
+
+        %Property(name=MergeCells, get=getMergeCells)
+
+        VARIANT getNumberFormatLocal();
+        %MethodCode
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_NumberFormatLocal(prop);
+            if (hr != S_OK)
+            {
+                delete prop;
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_NumberFormatLocal()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
             }
         %End
 
-        %Property(name=Weight, get=getWeight, set=setWeight)
+        %Property(name=NumberFormatLocal, get=getNumberFormatLocal)
 
-        VARIANT getThemeColor();
+        VARIANT getOrientation();
         %MethodCode
             VARIANT *prop = new VARIANT;
             VariantInit(prop);
-            HRESULT hr = sipCpp->get_ThemeColor(prop);
+            HRESULT hr = sipCpp->get_Orientation(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ThemeColor()' failed with 0x%x", hr);
+                    "Call 'get_Orientation()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setThemeColor(VARIANT prop);
+        %Property(name=Orientation, get=getOrientation)
+
+        long getReadingOrder();
         %MethodCode
-            HRESULT hr = sipCpp->put_ThemeColor(*a0);
+            long prop = 0;
+            HRESULT hr = sipCpp->get_ReadingOrder(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_ThemeColor()' failed with 0x%x", hr);
-                sipRes = nullptr;
+                    "Call 'get_ReadingOrder()' failed with 0x%x", hr);
+                return nullptr;
             }
             else
             {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
+                sipRes = prop;
             }
         %End
 
-        %Property(name=ThemeColor, get=getThemeColor, set=setThemeColor)
+        %Property(name=ReadingOrder, get=getReadingOrder)
 
-        VARIANT getTintAndShade();
+        VARIANT getShrinkToFit();
         %MethodCode
             VARIANT *prop = new VARIANT;
             VariantInit(prop);
-            HRESULT hr = sipCpp->get_TintAndShade(prop);
+            HRESULT hr = sipCpp->get_ShrinkToFit(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_TintAndShade()' failed with 0x%x", hr);
+                    "Call 'get_ShrinkToFit()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setTintAndShade(VARIANT prop);
+        %Property(name=ShrinkToFit, get=getShrinkToFit)
+
+        VARIANT getVerticalAlignment();
         %MethodCode
-            HRESULT hr = sipCpp->put_TintAndShade(*a0);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_VerticalAlignment(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_TintAndShade()' failed with 0x%x", hr);
-                sipRes = nullptr;
+                    "Call 'get_VerticalAlignment()' failed with 0x%x", hr);
+                return nullptr;
             }
             else
             {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
+                sipRes = prop;
+            }
+        %End
+
+        %Property(name=VerticalAlignment, get=getVerticalAlignment)
+
+        VARIANT getWrapText();
+        %MethodCode
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_WrapText(prop);
+            if (hr != S_OK)
+            {
+                delete prop;
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_WrapText()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
             }
         %End
 
-        %Property(name=TintAndShade, get=getTintAndShade, set=setTintAndShade)
+        %Property(name=WrapText, get=getWrapText)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISmartTag.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISmartTag.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IBorders.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/CalloutFormat.sip`

 * *Files 23% similar despite different names*

```diff
@@ -1,398 +1,351 @@
 /**
- * Copyright (c) 2020-2021 Weitian Leung
+ * Copyright (c) 2020 Weitian Leung
  *
  * This file is part of pywpsrpc.
  *
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct IBorders : public IDispatch /Abstract/
+    struct CalloutFormat : public ksoapi::_IMsoDispObj /Abstract/
     {
     public:
-        virtual HRESULT get_Application(
-            Application **RHS /Out/) = 0;
+        virtual HRESULT AutomaticLength() = 0;
 
-        virtual HRESULT get_Creator(
-            XlCreator *RHS /Out/) = 0;
+        virtual HRESULT CustomDrop(
+            single Drop) = 0;
 
-        virtual HRESULT get_Color(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT CustomLength(
+            single Length) = 0;
 
-        virtual HRESULT put_Color(
-            VARIANT RHS) = 0;
+        virtual HRESULT PresetDrop(
+            MsoCalloutDropType DropType) = 0;
 
-        virtual HRESULT get_ColorIndex(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT get_Accent(
+            MsoTriState *Accent /Out/) = 0;
 
-        virtual HRESULT put_ColorIndex(
-            VARIANT RHS) = 0;
+        virtual HRESULT put_Accent(
+            MsoTriState Accent) = 0;
 
-        virtual HRESULT get_Count(
-            long *RHS /Out/) = 0;
+        virtual HRESULT get_Angle(
+            MsoCalloutAngleType *Angle /Out/) = 0;
 
-        Py_ssize_t __len__() const;
-        %MethodCode
-            long count = 0;
-            if (sipCpp->get_Count(&count) != S_OK)
-                count = 0;
-            sipRes = count;
-        %End
+        virtual HRESULT put_Angle(
+            MsoCalloutAngleType Angle) = 0;
 
-        virtual HRESULT get_Item(
-            XlBordersIndex Index,
-            Border **RHS /Out/) = 0;
-
-        Border* __getitem__(XlBordersIndex index) const;
-        %MethodCode
-            etapi::Border *prop = nullptr;
-            if (sipCpp->get_Item(a0, &prop) != S_OK)
-                sipIsErr = 1;
-            else
-                sipRes = prop;
-        %End
+        virtual HRESULT get_AutoAttach(
+            MsoTriState *AutoAttach /Out/) = 0;
 
-        virtual HRESULT get_LineStyle(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT put_AutoAttach(
+            MsoTriState AutoAttach) = 0;
 
-        virtual HRESULT put_LineStyle(
-            VARIANT RHS) = 0;
+        virtual HRESULT get_AutoLength(
+            MsoTriState *AutoLength /Out/) = 0;
 
-        virtual HRESULT get_Value(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT get_Border(
+            MsoTriState *Border /Out/) = 0;
 
-        virtual HRESULT put_Value(
-            VARIANT RHS) = 0;
+        virtual HRESULT put_Border(
+            MsoTriState Border) = 0;
 
-        virtual HRESULT get_Weight(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT get_Drop(
+            single *Drop /Out/) = 0;
 
-        virtual HRESULT put_Weight(
-            VARIANT RHS) = 0;
+        virtual HRESULT get_DropType(
+            MsoCalloutDropType *DropType /Out/) = 0;
 
-        virtual HRESULT get__Default(
-            XlBordersIndex Index,
-            Border **RHS /Out/) = 0;
+        virtual HRESULT get_Gap(
+            single *Gap /Out/) = 0;
 
-        virtual HRESULT get_ThemeColor(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT put_Gap(
+            single Gap) = 0;
 
-        virtual HRESULT put_ThemeColor(
-            VARIANT RHS) = 0;
+        virtual HRESULT get_Length(
+            single *Length /Out/) = 0;
 
-        virtual HRESULT get_TintAndShade(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT get_Type(
+            MsoCalloutType *Type /Out/) = 0;
 
-        virtual HRESULT put_TintAndShade(
-            VARIANT RHS) = 0;
+        virtual HRESULT put_Type(
+            MsoCalloutType Type) = 0;
 
-        Application* getApplication();
+        MsoTriState getAccent();
         %MethodCode
-            etapi::Application *prop = nullptr;
-            HRESULT hr = sipCpp->get_Application(&prop);
+            etapi::MsoTriState prop = (etapi::MsoTriState)0;
+            HRESULT hr = sipCpp->get_Accent(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Application()' failed with 0x%x", hr);
+                    "Call 'get_Accent()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Application, get=getApplication)
-
-        XlCreator getCreator();
+        PyObject* setAccent(MsoTriState prop);
         %MethodCode
-            etapi::XlCreator prop = (etapi::XlCreator)0;
-            HRESULT hr = sipCpp->get_Creator(&prop);
+            HRESULT hr = sipCpp->put_Accent(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Creator()' failed with 0x%x", hr);
-                return nullptr;
+                    "Call 'put_Accent()' failed with 0x%x", hr);
+                sipRes = nullptr;
             }
             else
             {
-                sipRes = prop;
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
             }
         %End
 
-        %Property(name=Creator, get=getCreator)
+        %Property(name=Accent, get=getAccent, set=setAccent)
 
-        VARIANT getColor();
+        MsoCalloutAngleType getAngle();
         %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_Color(prop);
+            etapi::MsoCalloutAngleType prop = (etapi::MsoCalloutAngleType)0;
+            HRESULT hr = sipCpp->get_Angle(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Color()' failed with 0x%x", hr);
+                    "Call 'get_Angle()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setColor(VARIANT prop);
+        PyObject* setAngle(MsoCalloutAngleType prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Color(*a0);
+            HRESULT hr = sipCpp->put_Angle(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Color()' failed with 0x%x", hr);
+                    "Call 'put_Angle()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Color, get=getColor, set=setColor)
+        %Property(name=Angle, get=getAngle, set=setAngle)
 
-        VARIANT getColorIndex();
+        MsoTriState getAutoAttach();
         %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_ColorIndex(prop);
+            etapi::MsoTriState prop = (etapi::MsoTriState)0;
+            HRESULT hr = sipCpp->get_AutoAttach(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ColorIndex()' failed with 0x%x", hr);
+                    "Call 'get_AutoAttach()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setColorIndex(VARIANT prop);
+        PyObject* setAutoAttach(MsoTriState prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_ColorIndex(*a0);
+            HRESULT hr = sipCpp->put_AutoAttach(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_ColorIndex()' failed with 0x%x", hr);
+                    "Call 'put_AutoAttach()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=ColorIndex, get=getColorIndex, set=setColorIndex)
+        %Property(name=AutoAttach, get=getAutoAttach, set=setAutoAttach)
 
-        long getCount();
+        MsoTriState getAutoLength();
         %MethodCode
-            long prop = 0;
-            HRESULT hr = sipCpp->get_Count(&prop);
+            etapi::MsoTriState prop = (etapi::MsoTriState)0;
+            HRESULT hr = sipCpp->get_AutoLength(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Count()' failed with 0x%x", hr);
+                    "Call 'get_AutoLength()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Count, get=getCount)
+        %Property(name=AutoLength, get=getAutoLength)
 
-        VARIANT getLineStyle();
+        MsoTriState getBorder();
         %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_LineStyle(prop);
+            etapi::MsoTriState prop = (etapi::MsoTriState)0;
+            HRESULT hr = sipCpp->get_Border(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_LineStyle()' failed with 0x%x", hr);
+                    "Call 'get_Border()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setLineStyle(VARIANT prop);
+        PyObject* setBorder(MsoTriState prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_LineStyle(*a0);
+            HRESULT hr = sipCpp->put_Border(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_LineStyle()' failed with 0x%x", hr);
+                    "Call 'put_Border()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=LineStyle, get=getLineStyle, set=setLineStyle)
+        %Property(name=Border, get=getBorder, set=setBorder)
 
-        VARIANT getValue();
+        single getDrop();
         %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_Value(prop);
+            etapi::single prop = 0;
+            HRESULT hr = sipCpp->get_Drop(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Value()' failed with 0x%x", hr);
+                    "Call 'get_Drop()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setValue(VARIANT prop);
+        %Property(name=Drop, get=getDrop)
+
+        MsoCalloutDropType getDropType();
         %MethodCode
-            HRESULT hr = sipCpp->put_Value(*a0);
+            etapi::MsoCalloutDropType prop = (etapi::MsoCalloutDropType)0;
+            HRESULT hr = sipCpp->get_DropType(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Value()' failed with 0x%x", hr);
-                sipRes = nullptr;
+                    "Call 'get_DropType()' failed with 0x%x", hr);
+                return nullptr;
             }
             else
             {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
+                sipRes = prop;
             }
         %End
 
-        %Property(name=Value, get=getValue, set=setValue)
+        %Property(name=DropType, get=getDropType)
 
-        VARIANT getWeight();
+        single getGap();
         %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_Weight(prop);
+            etapi::single prop = 0;
+            HRESULT hr = sipCpp->get_Gap(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Weight()' failed with 0x%x", hr);
+                    "Call 'get_Gap()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setWeight(VARIANT prop);
+        PyObject* setGap(single prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Weight(*a0);
+            HRESULT hr = sipCpp->put_Gap(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Weight()' failed with 0x%x", hr);
+                    "Call 'put_Gap()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Weight, get=getWeight, set=setWeight)
+        %Property(name=Gap, get=getGap, set=setGap)
 
-        VARIANT getThemeColor();
+        single getLength();
         %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_ThemeColor(prop);
+            etapi::single prop = 0;
+            HRESULT hr = sipCpp->get_Length(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ThemeColor()' failed with 0x%x", hr);
+                    "Call 'get_Length()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setThemeColor(VARIANT prop);
-        %MethodCode
-            HRESULT hr = sipCpp->put_ThemeColor(*a0);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_ThemeColor()' failed with 0x%x", hr);
-                sipRes = nullptr;
-            }
-            else
-            {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
-            }
-        %End
-
-        %Property(name=ThemeColor, get=getThemeColor, set=setThemeColor)
+        %Property(name=Length, get=getLength)
 
-        VARIANT getTintAndShade();
+        MsoCalloutType getType();
         %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_TintAndShade(prop);
+            etapi::MsoCalloutType prop = (etapi::MsoCalloutType)0;
+            HRESULT hr = sipCpp->get_Type(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_TintAndShade()' failed with 0x%x", hr);
+                    "Call 'get_Type()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setTintAndShade(VARIANT prop);
+        PyObject* setType(MsoCalloutType prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_TintAndShade(*a0);
+            HRESULT hr = sipCpp->put_Type(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_TintAndShade()' failed with 0x%x", hr);
+                    "Call 'put_Type()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=TintAndShade, get=getTintAndShade, set=setTintAndShade)
+        %Property(name=Type, get=getType, set=setType)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISparkline.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISparkline.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ITextFrame.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ITextFrame.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IOLEDBErrors.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IOLEDBErrors.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDrawing.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDrawing.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IAreas.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IAreas.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IConnectorFormat.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IConnectorFormat.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IRTDUpdateEvent.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IRTDUpdateEvent.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPoint.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPoint.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IAllowEditRange.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IAllowEditRange.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IArc.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IDisplayUnitLabel.sip`

 * *Files 21% similar despite different names*

```diff
@@ -6,219 +6,149 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct IArc : public IDispatch /Abstract/
+    struct IDisplayUnitLabel : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
 
-        virtual HRESULT get_BottomRightCell(
-            Range **RHS /Out/) = 0;
-
-        virtual HRESULT BringToFront(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT get_Name(
+            BSTR *RHS /Out/) = 0;
 
-        virtual HRESULT Copy(
+        virtual HRESULT Select(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT CopyPicture(
-            XlPictureAppearance Appearance = etapi::xlPrinter,
-            XlCopyPictureFormat Format = etapi::xlPicture,
-            VARIANT *RHS /Out/ = 0) = 0;
-
-        virtual HRESULT Cut(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT get_Border(
+            Border **RHS /Out/) = 0;
 
         virtual HRESULT Delete(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT Duplicate(
-            IDispatch **RHS /Out/) = 0;
+        virtual HRESULT get_Interior(
+            Interior **RHS /Out/) = 0;
 
-        virtual HRESULT get_Enabled(
-            VARIANT_BOOL *RHS /Out/) = 0;
+        virtual HRESULT get_Fill(
+            ChartFillFormat **RHS /Out/) = 0;
 
-        virtual HRESULT put_Enabled(
-            VARIANT_BOOL RHS) = 0;
+        virtual HRESULT get_Caption(
+            BSTR *RHS /Out/) = 0;
 
-        virtual HRESULT get_Height(
-            double *RHS /Out/) = 0;
+        virtual HRESULT put_Caption(
+            BSTR RHS) = 0;
 
-        virtual HRESULT put_Height(
-            double RHS) = 0;
+        virtual HRESULT get_Characters(
+            VARIANT Start = argMissing2(),
+            VARIANT Length = argMissing2(),
+            Characters **RHS /Out/ = 0) = 0;
 
-        virtual HRESULT get_Index(
-            long *RHS /Out/) = 0;
+        virtual HRESULT get_Font(
+            Font **RHS /Out/) = 0;
+
+        virtual HRESULT get_HorizontalAlignment(
+            VARIANT *RHS /Out/) = 0;
+
+        virtual HRESULT put_HorizontalAlignment(
+            VARIANT RHS) = 0;
 
         virtual HRESULT get_Left(
             double *RHS /Out/) = 0;
 
         virtual HRESULT put_Left(
             double RHS) = 0;
 
-        virtual HRESULT get_Locked(
-            VARIANT_BOOL *RHS /Out/) = 0;
-
-        virtual HRESULT put_Locked(
-            VARIANT_BOOL RHS) = 0;
-
-        virtual HRESULT get_Name(
-            BSTR *RHS /Out/) = 0;
-
-        virtual HRESULT put_Name(
-            BSTR RHS) = 0;
-
-        virtual HRESULT get_OnAction(
-            BSTR *RHS /Out/) = 0;
-
-        virtual HRESULT put_OnAction(
-            BSTR RHS) = 0;
-
-        virtual HRESULT get_Placement(
+        virtual HRESULT get_Orientation(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Placement(
+        virtual HRESULT put_Orientation(
             VARIANT RHS) = 0;
 
-        virtual HRESULT get_PrintObject(
+        virtual HRESULT get_Shadow(
             VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT put_PrintObject(
+        virtual HRESULT put_Shadow(
             VARIANT_BOOL RHS) = 0;
 
-        virtual HRESULT Select(
-            VARIANT Replace = argMissing2(),
-            VARIANT *RHS /Out/ = 0) = 0;
+        virtual HRESULT get_Text(
+            BSTR *RHS /Out/) = 0;
 
-        virtual HRESULT SendToBack(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT put_Text(
+            BSTR RHS) = 0;
 
         virtual HRESULT get_Top(
             double *RHS /Out/) = 0;
 
         virtual HRESULT put_Top(
             double RHS) = 0;
 
-        virtual HRESULT get_TopLeftCell(
-            Range **RHS /Out/) = 0;
-
-        virtual HRESULT get_Visible(
-            VARIANT_BOOL *RHS /Out/) = 0;
-
-        virtual HRESULT put_Visible(
-            VARIANT_BOOL RHS) = 0;
-
-        virtual HRESULT get_Width(
-            double *RHS /Out/) = 0;
+        virtual HRESULT get_VerticalAlignment(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Width(
-            double RHS) = 0;
+        virtual HRESULT put_VerticalAlignment(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_ZOrder(
+        virtual HRESULT get_ReadingOrder(
             long *RHS /Out/) = 0;
 
-        virtual HRESULT get_ShapeRange(
-            ShapeRange **RHS /Out/) = 0;
-
-        virtual HRESULT get_AddIndent(
-            VARIANT_BOOL *RHS /Out/) = 0;
-
-        virtual HRESULT put_AddIndent(
-            VARIANT_BOOL RHS) = 0;
+        virtual HRESULT put_ReadingOrder(
+            long RHS) = 0;
 
         virtual HRESULT get_AutoScaleFont(
             VARIANT *RHS /Out/) = 0;
 
         virtual HRESULT put_AutoScaleFont(
             VARIANT RHS) = 0;
 
-        virtual HRESULT get_AutoSize(
-            VARIANT_BOOL *RHS /Out/) = 0;
+        virtual void _Dummy21() = 0;
 
-        virtual HRESULT put_AutoSize(
-            VARIANT_BOOL RHS) = 0;
+        virtual HRESULT get_Position(
+            XlChartElementPosition *RHS /Out/) = 0;
 
-        virtual HRESULT get_Caption(
-            BSTR *RHS /Out/) = 0;
+        virtual HRESULT put_Position(
+            XlChartElementPosition RHS) = 0;
 
-        virtual HRESULT put_Caption(
-            BSTR RHS) = 0;
+        virtual HRESULT get_Format(
+            ChartFormat **RHS /Out/) = 0;
 
-        virtual HRESULT get_Characters(
-            VARIANT Start = argMissing2(),
-            VARIANT Length = argMissing2(),
-            Characters **RHS /Out/ = 0) = 0;
-
-        virtual HRESULT CheckSpelling(
-            VARIANT CustomDictionary = argMissing2(),
-            VARIANT IgnoreUppercase = argMissing2(),
-            VARIANT AlwaysSuggest = argMissing2(),
-            VARIANT SpellLang = argMissing2(),
-            VARIANT *RHS /Out/ = 0) = 0;
+        virtual HRESULT get_Height(
+            double *RHS /Out/) = 0;
 
-        virtual HRESULT get_Font(
-            Font **RHS /Out/) = 0;
+        virtual HRESULT get_Width(
+            double *RHS /Out/) = 0;
 
         virtual HRESULT get_Formula(
             BSTR *RHS /Out/) = 0;
 
         virtual HRESULT put_Formula(
             BSTR RHS) = 0;
 
-        virtual HRESULT get_HorizontalAlignment(
-            VARIANT *RHS /Out/) = 0;
-
-        virtual HRESULT put_HorizontalAlignment(
-            VARIANT RHS) = 0;
-
-        virtual HRESULT get_LockedText(
-            VARIANT_BOOL *RHS /Out/) = 0;
-
-        virtual HRESULT put_LockedText(
-            VARIANT_BOOL RHS) = 0;
-
-        virtual HRESULT get_Orientation(
-            VARIANT *RHS /Out/) = 0;
-
-        virtual HRESULT put_Orientation(
-            VARIANT RHS) = 0;
-
-        virtual HRESULT get_Text(
+        virtual HRESULT get_FormulaR1C1(
             BSTR *RHS /Out/) = 0;
 
-        virtual HRESULT put_Text(
+        virtual HRESULT put_FormulaR1C1(
             BSTR RHS) = 0;
 
-        virtual HRESULT get_VerticalAlignment(
-            VARIANT *RHS /Out/) = 0;
-
-        virtual HRESULT put_VerticalAlignment(
-            VARIANT RHS) = 0;
-
-        virtual HRESULT get_ReadingOrder(
-            long *RHS /Out/) = 0;
-
-        virtual HRESULT put_ReadingOrder(
-            long RHS) = 0;
+        virtual HRESULT get_FormulaLocal(
+            BSTR *RHS /Out/) = 0;
 
-        virtual HRESULT get_Border(
-            Border **RHS /Out/) = 0;
+        virtual HRESULT put_FormulaLocal(
+            BSTR RHS) = 0;
 
-        virtual HRESULT get_Interior(
-            Interior **RHS /Out/) = 0;
+        virtual HRESULT get_FormulaR1C1Local(
+            BSTR *RHS /Out/) = 0;
 
-        virtual void _Dummy43() = 0;
+        virtual HRESULT put_FormulaR1C1Local(
+            BSTR RHS) = 0;
 
         Application* getApplication();
         %MethodCode
             etapi::Application *prop = nullptr;
             HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
@@ -248,520 +178,419 @@
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Creator, get=getCreator)
 
-        Range* getBottomRightCell();
+        BSTR getName();
         %MethodCode
-            etapi::Range *prop = nullptr;
-            HRESULT hr = sipCpp->get_BottomRightCell(&prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_Name(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_BottomRightCell()' failed with 0x%x", hr);
+                    "Call 'get_Name()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=BottomRightCell, get=getBottomRightCell)
+        %Property(name=Name, get=getName)
 
-        VARIANT_BOOL getEnabled();
+        Border* getBorder();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_Enabled(prop);
+            etapi::Border *prop = nullptr;
+            HRESULT hr = sipCpp->get_Border(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Enabled()' failed with 0x%x", hr);
+                    "Call 'get_Border()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setEnabled(VARIANT_BOOL prop);
-        %MethodCode
-            HRESULT hr = sipCpp->put_Enabled(*a0);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Enabled()' failed with 0x%x", hr);
-                sipRes = nullptr;
-            }
-            else
-            {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
-            }
-        %End
-
-        %Property(name=Enabled, get=getEnabled, set=setEnabled)
+        %Property(name=Border, get=getBorder)
 
-        double getHeight();
+        Interior* getInterior();
         %MethodCode
-            double prop = 0;
-            HRESULT hr = sipCpp->get_Height(&prop);
+            etapi::Interior *prop = nullptr;
+            HRESULT hr = sipCpp->get_Interior(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Height()' failed with 0x%x", hr);
+                    "Call 'get_Interior()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setHeight(double prop);
-        %MethodCode
-            HRESULT hr = sipCpp->put_Height(a0);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Height()' failed with 0x%x", hr);
-                sipRes = nullptr;
-            }
-            else
-            {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
-            }
-        %End
-
-        %Property(name=Height, get=getHeight, set=setHeight)
+        %Property(name=Interior, get=getInterior)
 
-        long getIndex();
+        ChartFillFormat* getFill();
         %MethodCode
-            long prop = 0;
-            HRESULT hr = sipCpp->get_Index(&prop);
+            etapi::ChartFillFormat *prop = nullptr;
+            HRESULT hr = sipCpp->get_Fill(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Index()' failed with 0x%x", hr);
+                    "Call 'get_Fill()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Index, get=getIndex)
+        %Property(name=Fill, get=getFill)
 
-        double getLeft();
+        BSTR getCaption();
         %MethodCode
-            double prop = 0;
-            HRESULT hr = sipCpp->get_Left(&prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_Caption(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Left()' failed with 0x%x", hr);
+                    "Call 'get_Caption()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setLeft(double prop);
+        PyObject* setCaption(BSTR prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Left(a0);
+            HRESULT hr = sipCpp->put_Caption(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Left()' failed with 0x%x", hr);
+                    "Call 'put_Caption()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Left, get=getLeft, set=setLeft)
+        %Property(name=Caption, get=getCaption, set=setCaption)
 
-        VARIANT_BOOL getLocked();
+        Font* getFont();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_Locked(prop);
+            etapi::Font *prop = nullptr;
+            HRESULT hr = sipCpp->get_Font(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Locked()' failed with 0x%x", hr);
+                    "Call 'get_Font()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setLocked(VARIANT_BOOL prop);
-        %MethodCode
-            HRESULT hr = sipCpp->put_Locked(*a0);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Locked()' failed with 0x%x", hr);
-                sipRes = nullptr;
-            }
-            else
-            {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
-            }
-        %End
-
-        %Property(name=Locked, get=getLocked, set=setLocked)
+        %Property(name=Font, get=getFont)
 
-        BSTR getName();
+        VARIANT getHorizontalAlignment();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_Name(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_HorizontalAlignment(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Name()' failed with 0x%x", hr);
+                    "Call 'get_HorizontalAlignment()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setName(BSTR prop);
+        PyObject* setHorizontalAlignment(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Name(*a0);
+            HRESULT hr = sipCpp->put_HorizontalAlignment(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Name()' failed with 0x%x", hr);
+                    "Call 'put_HorizontalAlignment()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Name, get=getName, set=setName)
+        %Property(name=HorizontalAlignment, get=getHorizontalAlignment, set=setHorizontalAlignment)
 
-        BSTR getOnAction();
+        double getLeft();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_OnAction(prop);
+            double prop = 0;
+            HRESULT hr = sipCpp->get_Left(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_OnAction()' failed with 0x%x", hr);
+                    "Call 'get_Left()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setOnAction(BSTR prop);
+        PyObject* setLeft(double prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_OnAction(*a0);
+            HRESULT hr = sipCpp->put_Left(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_OnAction()' failed with 0x%x", hr);
+                    "Call 'put_Left()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=OnAction, get=getOnAction, set=setOnAction)
+        %Property(name=Left, get=getLeft, set=setLeft)
 
-        VARIANT getPlacement();
+        VARIANT getOrientation();
         %MethodCode
             VARIANT *prop = new VARIANT;
             VariantInit(prop);
-            HRESULT hr = sipCpp->get_Placement(prop);
+            HRESULT hr = sipCpp->get_Orientation(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Placement()' failed with 0x%x", hr);
+                    "Call 'get_Orientation()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setPlacement(VARIANT prop);
+        PyObject* setOrientation(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Placement(*a0);
+            HRESULT hr = sipCpp->put_Orientation(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Placement()' failed with 0x%x", hr);
+                    "Call 'put_Orientation()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Placement, get=getPlacement, set=setPlacement)
+        %Property(name=Orientation, get=getOrientation, set=setOrientation)
 
-        VARIANT_BOOL getPrintObject();
+        VARIANT_BOOL getShadow();
         %MethodCode
             VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_PrintObject(prop);
+            HRESULT hr = sipCpp->get_Shadow(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_PrintObject()' failed with 0x%x", hr);
+                    "Call 'get_Shadow()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setPrintObject(VARIANT_BOOL prop);
+        PyObject* setShadow(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_PrintObject(*a0);
+            HRESULT hr = sipCpp->put_Shadow(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_PrintObject()' failed with 0x%x", hr);
+                    "Call 'put_Shadow()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=PrintObject, get=getPrintObject, set=setPrintObject)
+        %Property(name=Shadow, get=getShadow, set=setShadow)
 
-        double getTop();
+        BSTR getText();
         %MethodCode
-            double prop = 0;
-            HRESULT hr = sipCpp->get_Top(&prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_Text(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Top()' failed with 0x%x", hr);
+                    "Call 'get_Text()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setTop(double prop);
+        PyObject* setText(BSTR prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Top(a0);
+            HRESULT hr = sipCpp->put_Text(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Top()' failed with 0x%x", hr);
+                    "Call 'put_Text()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Top, get=getTop, set=setTop)
-
-        Range* getTopLeftCell();
-        %MethodCode
-            etapi::Range *prop = nullptr;
-            HRESULT hr = sipCpp->get_TopLeftCell(&prop);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_TopLeftCell()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        %Property(name=TopLeftCell, get=getTopLeftCell)
+        %Property(name=Text, get=getText, set=setText)
 
-        VARIANT_BOOL getVisible();
+        double getTop();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_Visible(prop);
+            double prop = 0;
+            HRESULT hr = sipCpp->get_Top(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Visible()' failed with 0x%x", hr);
+                    "Call 'get_Top()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setVisible(VARIANT_BOOL prop);
+        PyObject* setTop(double prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Visible(*a0);
+            HRESULT hr = sipCpp->put_Top(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Visible()' failed with 0x%x", hr);
+                    "Call 'put_Top()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Visible, get=getVisible, set=setVisible)
+        %Property(name=Top, get=getTop, set=setTop)
 
-        double getWidth();
+        VARIANT getVerticalAlignment();
         %MethodCode
-            double prop = 0;
-            HRESULT hr = sipCpp->get_Width(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_VerticalAlignment(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Width()' failed with 0x%x", hr);
+                    "Call 'get_VerticalAlignment()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setWidth(double prop);
+        PyObject* setVerticalAlignment(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Width(a0);
+            HRESULT hr = sipCpp->put_VerticalAlignment(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Width()' failed with 0x%x", hr);
+                    "Call 'put_VerticalAlignment()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Width, get=getWidth, set=setWidth)
+        %Property(name=VerticalAlignment, get=getVerticalAlignment, set=setVerticalAlignment)
 
-        long getZOrder();
+        long getReadingOrder();
         %MethodCode
             long prop = 0;
-            HRESULT hr = sipCpp->get_ZOrder(&prop);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ZOrder()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        %Property(name=ZOrder, get=getZOrder)
-
-        ShapeRange* getShapeRange();
-        %MethodCode
-            etapi::ShapeRange *prop = nullptr;
-            HRESULT hr = sipCpp->get_ShapeRange(&prop);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ShapeRange()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        %Property(name=ShapeRange, get=getShapeRange)
-
-        VARIANT_BOOL getAddIndent();
-        %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_AddIndent(prop);
+            HRESULT hr = sipCpp->get_ReadingOrder(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_AddIndent()' failed with 0x%x", hr);
+                    "Call 'get_ReadingOrder()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setAddIndent(VARIANT_BOOL prop);
+        PyObject* setReadingOrder(long prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_AddIndent(*a0);
+            HRESULT hr = sipCpp->put_ReadingOrder(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_AddIndent()' failed with 0x%x", hr);
+                    "Call 'put_ReadingOrder()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=AddIndent, get=getAddIndent, set=setAddIndent)
+        %Property(name=ReadingOrder, get=getReadingOrder, set=setReadingOrder)
 
         VARIANT getAutoScaleFont();
         %MethodCode
             VARIANT *prop = new VARIANT;
             VariantInit(prop);
             HRESULT hr = sipCpp->get_AutoScaleFont(prop);
             if (hr != S_OK)
@@ -791,101 +620,101 @@
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
         %Property(name=AutoScaleFont, get=getAutoScaleFont, set=setAutoScaleFont)
 
-        VARIANT_BOOL getAutoSize();
+        XlChartElementPosition getPosition();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_AutoSize(prop);
+            etapi::XlChartElementPosition prop = (etapi::XlChartElementPosition)0;
+            HRESULT hr = sipCpp->get_Position(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_AutoSize()' failed with 0x%x", hr);
+                    "Call 'get_Position()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setAutoSize(VARIANT_BOOL prop);
+        PyObject* setPosition(XlChartElementPosition prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_AutoSize(*a0);
+            HRESULT hr = sipCpp->put_Position(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_AutoSize()' failed with 0x%x", hr);
+                    "Call 'put_Position()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=AutoSize, get=getAutoSize, set=setAutoSize)
+        %Property(name=Position, get=getPosition, set=setPosition)
 
-        BSTR getCaption();
+        ChartFormat* getFormat();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_Caption(prop);
+            etapi::ChartFormat *prop = nullptr;
+            HRESULT hr = sipCpp->get_Format(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Caption()' failed with 0x%x", hr);
+                    "Call 'get_Format()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setCaption(BSTR prop);
+        %Property(name=Format, get=getFormat)
+
+        double getHeight();
         %MethodCode
-            HRESULT hr = sipCpp->put_Caption(*a0);
+            double prop = 0;
+            HRESULT hr = sipCpp->get_Height(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Caption()' failed with 0x%x", hr);
-                sipRes = nullptr;
+                    "Call 'get_Height()' failed with 0x%x", hr);
+                return nullptr;
             }
             else
             {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
+                sipRes = prop;
             }
         %End
 
-        %Property(name=Caption, get=getCaption, set=setCaption)
+        %Property(name=Height, get=getHeight)
 
-        Font* getFont();
+        double getWidth();
         %MethodCode
-            etapi::Font *prop = nullptr;
-            HRESULT hr = sipCpp->get_Font(&prop);
+            double prop = 0;
+            HRESULT hr = sipCpp->get_Width(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Font()' failed with 0x%x", hr);
+                    "Call 'get_Width()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Font, get=getFont)
+        %Property(name=Width, get=getWidth)
 
         BSTR getFormula();
         %MethodCode
             BSTR *prop = new BSTR;
             HRESULT hr = sipCpp->get_Formula(prop);
             if (hr != S_OK)
             {
@@ -914,256 +743,113 @@
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
         %Property(name=Formula, get=getFormula, set=setFormula)
 
-        VARIANT getHorizontalAlignment();
-        %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_HorizontalAlignment(prop);
-            if (hr != S_OK)
-            {
-                delete prop;
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_HorizontalAlignment()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        PyObject* setHorizontalAlignment(VARIANT prop);
+        BSTR getFormulaR1C1();
         %MethodCode
-            HRESULT hr = sipCpp->put_HorizontalAlignment(*a0);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_HorizontalAlignment()' failed with 0x%x", hr);
-                sipRes = nullptr;
-            }
-            else
-            {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
-            }
-        %End
-
-        %Property(name=HorizontalAlignment, get=getHorizontalAlignment, set=setHorizontalAlignment)
-
-        VARIANT_BOOL getLockedText();
-        %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_LockedText(prop);
-            if (hr != S_OK)
-            {
-                delete prop;
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_LockedText()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        PyObject* setLockedText(VARIANT_BOOL prop);
-        %MethodCode
-            HRESULT hr = sipCpp->put_LockedText(*a0);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_LockedText()' failed with 0x%x", hr);
-                sipRes = nullptr;
-            }
-            else
-            {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
-            }
-        %End
-
-        %Property(name=LockedText, get=getLockedText, set=setLockedText)
-
-        VARIANT getOrientation();
-        %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_Orientation(prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_FormulaR1C1(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Orientation()' failed with 0x%x", hr);
+                    "Call 'get_FormulaR1C1()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setOrientation(VARIANT prop);
+        PyObject* setFormulaR1C1(BSTR prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Orientation(*a0);
+            HRESULT hr = sipCpp->put_FormulaR1C1(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Orientation()' failed with 0x%x", hr);
+                    "Call 'put_FormulaR1C1()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Orientation, get=getOrientation, set=setOrientation)
+        %Property(name=FormulaR1C1, get=getFormulaR1C1, set=setFormulaR1C1)
 
-        BSTR getText();
+        BSTR getFormulaLocal();
         %MethodCode
             BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_Text(prop);
+            HRESULT hr = sipCpp->get_FormulaLocal(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Text()' failed with 0x%x", hr);
+                    "Call 'get_FormulaLocal()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setText(BSTR prop);
+        PyObject* setFormulaLocal(BSTR prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Text(*a0);
+            HRESULT hr = sipCpp->put_FormulaLocal(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Text()' failed with 0x%x", hr);
+                    "Call 'put_FormulaLocal()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Text, get=getText, set=setText)
+        %Property(name=FormulaLocal, get=getFormulaLocal, set=setFormulaLocal)
 
-        VARIANT getVerticalAlignment();
+        BSTR getFormulaR1C1Local();
         %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_VerticalAlignment(prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_FormulaR1C1Local(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_VerticalAlignment()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        PyObject* setVerticalAlignment(VARIANT prop);
-        %MethodCode
-            HRESULT hr = sipCpp->put_VerticalAlignment(*a0);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_VerticalAlignment()' failed with 0x%x", hr);
-                sipRes = nullptr;
-            }
-            else
-            {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
-            }
-        %End
-
-        %Property(name=VerticalAlignment, get=getVerticalAlignment, set=setVerticalAlignment)
-
-        long getReadingOrder();
-        %MethodCode
-            long prop = 0;
-            HRESULT hr = sipCpp->get_ReadingOrder(&prop);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ReadingOrder()' failed with 0x%x", hr);
+                    "Call 'get_FormulaR1C1Local()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setReadingOrder(long prop);
+        PyObject* setFormulaR1C1Local(BSTR prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_ReadingOrder(a0);
+            HRESULT hr = sipCpp->put_FormulaR1C1Local(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_ReadingOrder()' failed with 0x%x", hr);
+                    "Call 'put_FormulaR1C1Local()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=ReadingOrder, get=getReadingOrder, set=setReadingOrder)
-
-        Border* getBorder();
-        %MethodCode
-            etapi::Border *prop = nullptr;
-            HRESULT hr = sipCpp->get_Border(&prop);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Border()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        %Property(name=Border, get=getBorder)
-
-        Interior* getInterior();
-        %MethodCode
-            etapi::Interior *prop = nullptr;
-            HRESULT hr = sipCpp->get_Interior(&prop);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Interior()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        %Property(name=Interior, get=getInterior)
+        %Property(name=FormulaR1C1Local, get=getFormulaR1C1Local, set=setFormulaR1C1Local)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IServerViewableItems.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IServerViewableItems.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/DefaultWebOptions.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/DefaultWebOptions.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IHyperlink.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IRoutingSlip.sip`

 * *Files 13% similar despite different names*

```diff
@@ -6,80 +6,66 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct IHyperlink : public IDispatch /Abstract/
+    struct IRoutingSlip : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
 
-        virtual HRESULT get_Name(
-            BSTR *RHS /Out/) = 0;
+        virtual HRESULT get_Delivery(
+            XlRoutingSlipDelivery *RHS /Out/) = 0;
 
-        virtual HRESULT get_Range(
-            Range **RHS /Out/) = 0;
+        virtual HRESULT put_Delivery(
+            XlRoutingSlipDelivery RHS) = 0;
 
-        virtual HRESULT get_Shape(
-            Shape **RHS /Out/) = 0;
+        virtual HRESULT get_Message(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_SubAddress(
-            BSTR *RHS /Out/) = 0;
+        virtual HRESULT put_Message(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT put_SubAddress(
-            BSTR RHS) = 0;
+        virtual HRESULT get_Recipients(
+            VARIANT Index = argMissing2(),
+            VARIANT *RHS /Out/ = 0) = 0;
 
-        virtual HRESULT get_Address(
-            BSTR *RHS /Out/) = 0;
+        virtual HRESULT put_Recipients(
+            VARIANT Index = argMissing2(),
+            VARIANT RHS = argMissing2()) = 0;
 
-        virtual HRESULT put_Address(
-            BSTR RHS) = 0;
+        virtual HRESULT Reset(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_Type(
-            long *RHS /Out/) = 0;
+        virtual HRESULT get_ReturnWhenDone(
+            VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT AddToFavorites() = 0;
+        virtual HRESULT put_ReturnWhenDone(
+            VARIANT_BOOL RHS) = 0;
 
-        virtual HRESULT Delete() = 0;
+        virtual HRESULT get_Status(
+            XlRoutingSlipStatus *RHS /Out/) = 0;
 
-        virtual HRESULT Follow(
-            VARIANT NewWindow = argMissing2(),
-            VARIANT AddHistory = argMissing2(),
-            VARIANT ExtraInfo = argMissing2(),
-            VARIANT Method = argMissing2(),
-            VARIANT HeaderInfo = argMissing2()) = 0;
+        virtual HRESULT get_Subject(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_EmailSubject(
-            BSTR *RHS /Out/) = 0;
+        virtual HRESULT put_Subject(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT put_EmailSubject(
-            BSTR RHS) = 0;
+        virtual HRESULT get_TrackStatus(
+            VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT get_ScreenTip(
-            BSTR *RHS /Out/) = 0;
-
-        virtual HRESULT put_ScreenTip(
-            BSTR RHS) = 0;
-
-        virtual HRESULT get_TextToDisplay(
-            BSTR *RHS /Out/) = 0;
-
-        virtual HRESULT put_TextToDisplay(
-            BSTR RHS) = 0;
-
-        virtual HRESULT CreateNewDocument(
-            BSTR Filename,
-            VARIANT_BOOL EditNow,
-            VARIANT_BOOL Overwrite) = 0;
+        virtual HRESULT put_TrackStatus(
+            VARIANT_BOOL RHS) = 0;
 
         Application* getApplication();
         %MethodCode
             etapi::Application *prop = nullptr;
             HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
@@ -109,256 +95,202 @@
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Creator, get=getCreator)
 
-        BSTR getName();
-        %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_Name(prop);
-            if (hr != S_OK)
-            {
-                delete prop;
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Name()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        %Property(name=Name, get=getName)
-
-        Range* getRange();
+        XlRoutingSlipDelivery getDelivery();
         %MethodCode
-            etapi::Range *prop = nullptr;
-            HRESULT hr = sipCpp->get_Range(&prop);
+            etapi::XlRoutingSlipDelivery prop = (etapi::XlRoutingSlipDelivery)0;
+            HRESULT hr = sipCpp->get_Delivery(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Range()' failed with 0x%x", hr);
+                    "Call 'get_Delivery()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Range, get=getRange)
-
-        Shape* getShape();
+        PyObject* setDelivery(XlRoutingSlipDelivery prop);
         %MethodCode
-            etapi::Shape *prop = nullptr;
-            HRESULT hr = sipCpp->get_Shape(&prop);
+            HRESULT hr = sipCpp->put_Delivery(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Shape()' failed with 0x%x", hr);
-                return nullptr;
+                    "Call 'put_Delivery()' failed with 0x%x", hr);
+                sipRes = nullptr;
             }
             else
             {
-                sipRes = prop;
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
             }
         %End
 
-        %Property(name=Shape, get=getShape)
+        %Property(name=Delivery, get=getDelivery, set=setDelivery)
 
-        BSTR getSubAddress();
+        VARIANT getMessage();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_SubAddress(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Message(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_SubAddress()' failed with 0x%x", hr);
+                    "Call 'get_Message()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setSubAddress(BSTR prop);
+        PyObject* setMessage(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_SubAddress(*a0);
+            HRESULT hr = sipCpp->put_Message(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_SubAddress()' failed with 0x%x", hr);
+                    "Call 'put_Message()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=SubAddress, get=getSubAddress, set=setSubAddress)
+        %Property(name=Message, get=getMessage, set=setMessage)
 
-        BSTR getAddress();
+        VARIANT_BOOL getReturnWhenDone();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_Address(prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_ReturnWhenDone(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Address()' failed with 0x%x", hr);
+                    "Call 'get_ReturnWhenDone()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setAddress(BSTR prop);
+        PyObject* setReturnWhenDone(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Address(*a0);
+            HRESULT hr = sipCpp->put_ReturnWhenDone(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Address()' failed with 0x%x", hr);
+                    "Call 'put_ReturnWhenDone()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Address, get=getAddress, set=setAddress)
+        %Property(name=ReturnWhenDone, get=getReturnWhenDone, set=setReturnWhenDone)
 
-        long getType();
+        XlRoutingSlipStatus getStatus();
         %MethodCode
-            long prop = 0;
-            HRESULT hr = sipCpp->get_Type(&prop);
+            etapi::XlRoutingSlipStatus prop = (etapi::XlRoutingSlipStatus)0;
+            HRESULT hr = sipCpp->get_Status(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Type()' failed with 0x%x", hr);
+                    "Call 'get_Status()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Type, get=getType)
-
-        BSTR getEmailSubject();
-        %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_EmailSubject(prop);
-            if (hr != S_OK)
-            {
-                delete prop;
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_EmailSubject()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        PyObject* setEmailSubject(BSTR prop);
-        %MethodCode
-            HRESULT hr = sipCpp->put_EmailSubject(*a0);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_EmailSubject()' failed with 0x%x", hr);
-                sipRes = nullptr;
-            }
-            else
-            {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
-            }
-        %End
-
-        %Property(name=EmailSubject, get=getEmailSubject, set=setEmailSubject)
+        %Property(name=Status, get=getStatus)
 
-        BSTR getScreenTip();
+        VARIANT getSubject();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_ScreenTip(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Subject(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ScreenTip()' failed with 0x%x", hr);
+                    "Call 'get_Subject()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setScreenTip(BSTR prop);
+        PyObject* setSubject(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_ScreenTip(*a0);
+            HRESULT hr = sipCpp->put_Subject(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_ScreenTip()' failed with 0x%x", hr);
+                    "Call 'put_Subject()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=ScreenTip, get=getScreenTip, set=setScreenTip)
+        %Property(name=Subject, get=getSubject, set=setSubject)
 
-        BSTR getTextToDisplay();
+        VARIANT_BOOL getTrackStatus();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_TextToDisplay(prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_TrackStatus(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_TextToDisplay()' failed with 0x%x", hr);
+                    "Call 'get_TrackStatus()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setTextToDisplay(BSTR prop);
+        PyObject* setTrackStatus(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_TextToDisplay(*a0);
+            HRESULT hr = sipCpp->put_TrackStatus(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_TextToDisplay()' failed with 0x%x", hr);
+                    "Call 'put_TrackStatus()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=TextToDisplay, get=getTextToDisplay, set=setTextToDisplay)
+        %Property(name=TrackStatus, get=getTrackStatus, set=setTrackStatus)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IUsedObjects.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IIconSet.sip`

 * *Files 7% similar despite different names*

```diff
@@ -6,45 +6,48 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct IUsedObjects : public IDispatch /Abstract/
+    struct IIconSet : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
 
+        virtual HRESULT get_ID(
+            XlIconSet *RHS /Out/) = 0;
+
         virtual HRESULT get_Count(
             long *RHS /Out/) = 0;
 
         Py_ssize_t __len__() const;
         %MethodCode
             long count = 0;
             if (sipCpp->get_Count(&count) != S_OK)
                 count = 0;
             sipRes = count;
         %End
 
         virtual HRESULT get__Default(
             VARIANT Index,
-            IDispatch **RHS /Out/) = 0;
+            Icon **RHS /Out/) = 0;
 
         virtual HRESULT get_Item(
             VARIANT Index,
-            IDispatch **RHS /Out/) = 0;
+            Icon **RHS /Out/) = 0;
 
-        IDispatch* __getitem__(VARIANT index) const;
+        Icon* __getitem__(VARIANT index) const;
         %MethodCode
-            IDispatch *prop = nullptr;
+            etapi::Icon *prop = nullptr;
             if (sipCpp->get_Item(*a0, &prop) != S_OK)
                 sipIsErr = 1;
             else
                 sipRes = prop;
         %End
 
         Application* getApplication();
@@ -79,14 +82,32 @@
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Creator, get=getCreator)
 
+        XlIconSet getID();
+        %MethodCode
+            etapi::XlIconSet prop = (etapi::XlIconSet)0;
+            HRESULT hr = sipCpp->get_ID(&prop);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_ID()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        %Property(name=ID, get=getID)
+
         long getCount();
         %MethodCode
             long prop = 0;
             HRESULT hr = sipCpp->get_Count(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IDisplayUnitLabel.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPicture.sip`

 * *Files 14% similar despite different names*

```diff
@@ -6,148 +6,147 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct IDisplayUnitLabel : public IDispatch /Abstract/
+    struct IPicture : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
 
-        virtual HRESULT get_Name(
-            BSTR *RHS /Out/) = 0;
+        virtual HRESULT get_BottomRightCell(
+            Range **RHS /Out/) = 0;
 
-        virtual HRESULT Select(
+        virtual HRESULT BringToFront(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_Border(
-            Border **RHS /Out/) = 0;
-
-        virtual HRESULT Delete(
+        virtual HRESULT Copy(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_Interior(
-            Interior **RHS /Out/) = 0;
+        virtual HRESULT CopyPicture(
+            XlPictureAppearance Appearance = etapi::xlPrinter,
+            XlCopyPictureFormat Format = etapi::xlPicture,
+            VARIANT *RHS /Out/ = 0) = 0;
 
-        virtual HRESULT get_Fill(
-            ChartFillFormat **RHS /Out/) = 0;
+        virtual HRESULT Cut(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_Caption(
-            BSTR *RHS /Out/) = 0;
+        virtual HRESULT Delete(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Caption(
-            BSTR RHS) = 0;
+        virtual HRESULT Duplicate(
+            IDispatch **RHS /Out/) = 0;
 
-        virtual HRESULT get_Characters(
-            VARIANT Start = argMissing2(),
-            VARIANT Length = argMissing2(),
-            Characters **RHS /Out/ = 0) = 0;
+        virtual HRESULT get_Enabled(
+            VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT get_Font(
-            Font **RHS /Out/) = 0;
+        virtual HRESULT put_Enabled(
+            VARIANT_BOOL RHS) = 0;
 
-        virtual HRESULT get_HorizontalAlignment(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT get_Height(
+            double *RHS /Out/) = 0;
 
-        virtual HRESULT put_HorizontalAlignment(
-            VARIANT RHS) = 0;
+        virtual HRESULT put_Height(
+            double RHS) = 0;
+
+        virtual HRESULT get_Index(
+            long *RHS /Out/) = 0;
 
         virtual HRESULT get_Left(
             double *RHS /Out/) = 0;
 
         virtual HRESULT put_Left(
             double RHS) = 0;
 
-        virtual HRESULT get_Orientation(
-            VARIANT *RHS /Out/) = 0;
-
-        virtual HRESULT put_Orientation(
-            VARIANT RHS) = 0;
-
-        virtual HRESULT get_Shadow(
+        virtual HRESULT get_Locked(
             VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT put_Shadow(
+        virtual HRESULT put_Locked(
             VARIANT_BOOL RHS) = 0;
 
-        virtual HRESULT get_Text(
+        virtual HRESULT get_Name(
             BSTR *RHS /Out/) = 0;
 
-        virtual HRESULT put_Text(
+        virtual HRESULT put_Name(
             BSTR RHS) = 0;
 
-        virtual HRESULT get_Top(
-            double *RHS /Out/) = 0;
+        virtual HRESULT get_OnAction(
+            BSTR *RHS /Out/) = 0;
 
-        virtual HRESULT put_Top(
-            double RHS) = 0;
+        virtual HRESULT put_OnAction(
+            BSTR RHS) = 0;
 
-        virtual HRESULT get_VerticalAlignment(
+        virtual HRESULT get_Placement(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_VerticalAlignment(
+        virtual HRESULT put_Placement(
             VARIANT RHS) = 0;
 
-        virtual HRESULT get_ReadingOrder(
-            long *RHS /Out/) = 0;
+        virtual HRESULT get_PrintObject(
+            VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT put_ReadingOrder(
-            long RHS) = 0;
+        virtual HRESULT put_PrintObject(
+            VARIANT_BOOL RHS) = 0;
 
-        virtual HRESULT get_AutoScaleFont(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT Select(
+            VARIANT Replace = argMissing2(),
+            VARIANT *RHS /Out/ = 0) = 0;
 
-        virtual HRESULT put_AutoScaleFont(
-            VARIANT RHS) = 0;
+        virtual HRESULT SendToBack(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual void _Dummy21() = 0;
+        virtual HRESULT get_Top(
+            double *RHS /Out/) = 0;
 
-        virtual HRESULT get_Position(
-            XlChartElementPosition *RHS /Out/) = 0;
+        virtual HRESULT put_Top(
+            double RHS) = 0;
 
-        virtual HRESULT put_Position(
-            XlChartElementPosition RHS) = 0;
+        virtual HRESULT get_TopLeftCell(
+            Range **RHS /Out/) = 0;
 
-        virtual HRESULT get_Format(
-            ChartFormat **RHS /Out/) = 0;
+        virtual HRESULT get_Visible(
+            VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT get_Height(
-            double *RHS /Out/) = 0;
+        virtual HRESULT put_Visible(
+            VARIANT_BOOL RHS) = 0;
 
         virtual HRESULT get_Width(
             double *RHS /Out/) = 0;
 
-        virtual HRESULT get_Formula(
-            BSTR *RHS /Out/) = 0;
+        virtual HRESULT put_Width(
+            double RHS) = 0;
 
-        virtual HRESULT put_Formula(
-            BSTR RHS) = 0;
+        virtual HRESULT get_ZOrder(
+            long *RHS /Out/) = 0;
 
-        virtual HRESULT get_FormulaR1C1(
-            BSTR *RHS /Out/) = 0;
+        virtual HRESULT get_ShapeRange(
+            ShapeRange **RHS /Out/) = 0;
 
-        virtual HRESULT put_FormulaR1C1(
-            BSTR RHS) = 0;
+        virtual HRESULT get_Border(
+            Border **RHS /Out/) = 0;
 
-        virtual HRESULT get_FormulaLocal(
-            BSTR *RHS /Out/) = 0;
+        virtual HRESULT get_Interior(
+            Interior **RHS /Out/) = 0;
 
-        virtual HRESULT put_FormulaLocal(
-            BSTR RHS) = 0;
+        virtual HRESULT get_Shadow(
+            VARIANT_BOOL *RHS /Out/) = 0;
+
+        virtual HRESULT put_Shadow(
+            VARIANT_BOOL RHS) = 0;
 
-        virtual HRESULT get_FormulaR1C1Local(
+        virtual HRESULT get_Formula(
             BSTR *RHS /Out/) = 0;
 
-        virtual HRESULT put_FormulaR1C1Local(
+        virtual HRESULT put_Formula(
             BSTR RHS) = 0;
 
         Application* getApplication();
         %MethodCode
             etapi::Application *prop = nullptr;
             HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
@@ -178,175 +177,118 @@
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Creator, get=getCreator)
 
-        BSTR getName();
+        Range* getBottomRightCell();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_Name(prop);
+            etapi::Range *prop = nullptr;
+            HRESULT hr = sipCpp->get_BottomRightCell(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Name()' failed with 0x%x", hr);
+                    "Call 'get_BottomRightCell()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Name, get=getName)
+        %Property(name=BottomRightCell, get=getBottomRightCell)
 
-        Border* getBorder();
+        VARIANT_BOOL getEnabled();
         %MethodCode
-            etapi::Border *prop = nullptr;
-            HRESULT hr = sipCpp->get_Border(&prop);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Border()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        %Property(name=Border, get=getBorder)
-
-        Interior* getInterior();
-        %MethodCode
-            etapi::Interior *prop = nullptr;
-            HRESULT hr = sipCpp->get_Interior(&prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_Enabled(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Interior()' failed with 0x%x", hr);
+                    "Call 'get_Enabled()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Interior, get=getInterior)
-
-        ChartFillFormat* getFill();
+        PyObject* setEnabled(VARIANT_BOOL prop);
         %MethodCode
-            etapi::ChartFillFormat *prop = nullptr;
-            HRESULT hr = sipCpp->get_Fill(&prop);
+            HRESULT hr = sipCpp->put_Enabled(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Fill()' failed with 0x%x", hr);
-                return nullptr;
+                    "Call 'put_Enabled()' failed with 0x%x", hr);
+                sipRes = nullptr;
             }
             else
             {
-                sipRes = prop;
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
             }
         %End
 
-        %Property(name=Fill, get=getFill)
+        %Property(name=Enabled, get=getEnabled, set=setEnabled)
 
-        BSTR getCaption();
+        double getHeight();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_Caption(prop);
+            double prop = 0;
+            HRESULT hr = sipCpp->get_Height(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Caption()' failed with 0x%x", hr);
+                    "Call 'get_Height()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setCaption(BSTR prop);
+        PyObject* setHeight(double prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Caption(*a0);
+            HRESULT hr = sipCpp->put_Height(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Caption()' failed with 0x%x", hr);
+                    "Call 'put_Height()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Caption, get=getCaption, set=setCaption)
+        %Property(name=Height, get=getHeight, set=setHeight)
 
-        Font* getFont();
+        long getIndex();
         %MethodCode
-            etapi::Font *prop = nullptr;
-            HRESULT hr = sipCpp->get_Font(&prop);
+            long prop = 0;
+            HRESULT hr = sipCpp->get_Index(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Font()' failed with 0x%x", hr);
+                    "Call 'get_Index()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Font, get=getFont)
-
-        VARIANT getHorizontalAlignment();
-        %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_HorizontalAlignment(prop);
-            if (hr != S_OK)
-            {
-                delete prop;
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_HorizontalAlignment()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        PyObject* setHorizontalAlignment(VARIANT prop);
-        %MethodCode
-            HRESULT hr = sipCpp->put_HorizontalAlignment(*a0);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_HorizontalAlignment()' failed with 0x%x", hr);
-                sipRes = nullptr;
-            }
-            else
-            {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
-            }
-        %End
-
-        %Property(name=HorizontalAlignment, get=getHorizontalAlignment, set=setHorizontalAlignment)
+        %Property(name=Index, get=getIndex)
 
         double getLeft();
         %MethodCode
             double prop = 0;
             HRESULT hr = sipCpp->get_Left(&prop);
             if (hr != S_OK)
             {
@@ -374,482 +316,447 @@
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
         %Property(name=Left, get=getLeft, set=setLeft)
 
-        VARIANT getOrientation();
+        VARIANT_BOOL getLocked();
         %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_Orientation(prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_Locked(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Orientation()' failed with 0x%x", hr);
+                    "Call 'get_Locked()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setOrientation(VARIANT prop);
+        PyObject* setLocked(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Orientation(*a0);
+            HRESULT hr = sipCpp->put_Locked(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Orientation()' failed with 0x%x", hr);
+                    "Call 'put_Locked()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Orientation, get=getOrientation, set=setOrientation)
+        %Property(name=Locked, get=getLocked, set=setLocked)
 
-        VARIANT_BOOL getShadow();
+        BSTR getName();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_Shadow(prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_Name(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Shadow()' failed with 0x%x", hr);
+                    "Call 'get_Name()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setShadow(VARIANT_BOOL prop);
+        PyObject* setName(BSTR prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Shadow(*a0);
+            HRESULT hr = sipCpp->put_Name(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Shadow()' failed with 0x%x", hr);
+                    "Call 'put_Name()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Shadow, get=getShadow, set=setShadow)
+        %Property(name=Name, get=getName, set=setName)
 
-        BSTR getText();
+        BSTR getOnAction();
         %MethodCode
             BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_Text(prop);
+            HRESULT hr = sipCpp->get_OnAction(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Text()' failed with 0x%x", hr);
+                    "Call 'get_OnAction()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setText(BSTR prop);
+        PyObject* setOnAction(BSTR prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Text(*a0);
+            HRESULT hr = sipCpp->put_OnAction(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Text()' failed with 0x%x", hr);
+                    "Call 'put_OnAction()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Text, get=getText, set=setText)
+        %Property(name=OnAction, get=getOnAction, set=setOnAction)
 
-        double getTop();
+        VARIANT getPlacement();
         %MethodCode
-            double prop = 0;
-            HRESULT hr = sipCpp->get_Top(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Placement(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Top()' failed with 0x%x", hr);
+                    "Call 'get_Placement()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setTop(double prop);
+        PyObject* setPlacement(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Top(a0);
+            HRESULT hr = sipCpp->put_Placement(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Top()' failed with 0x%x", hr);
+                    "Call 'put_Placement()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Top, get=getTop, set=setTop)
+        %Property(name=Placement, get=getPlacement, set=setPlacement)
 
-        VARIANT getVerticalAlignment();
+        VARIANT_BOOL getPrintObject();
         %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_VerticalAlignment(prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_PrintObject(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_VerticalAlignment()' failed with 0x%x", hr);
+                    "Call 'get_PrintObject()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setVerticalAlignment(VARIANT prop);
+        PyObject* setPrintObject(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_VerticalAlignment(*a0);
+            HRESULT hr = sipCpp->put_PrintObject(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_VerticalAlignment()' failed with 0x%x", hr);
+                    "Call 'put_PrintObject()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=VerticalAlignment, get=getVerticalAlignment, set=setVerticalAlignment)
+        %Property(name=PrintObject, get=getPrintObject, set=setPrintObject)
 
-        long getReadingOrder();
+        double getTop();
         %MethodCode
-            long prop = 0;
-            HRESULT hr = sipCpp->get_ReadingOrder(&prop);
+            double prop = 0;
+            HRESULT hr = sipCpp->get_Top(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ReadingOrder()' failed with 0x%x", hr);
+                    "Call 'get_Top()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setReadingOrder(long prop);
+        PyObject* setTop(double prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_ReadingOrder(a0);
+            HRESULT hr = sipCpp->put_Top(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_ReadingOrder()' failed with 0x%x", hr);
+                    "Call 'put_Top()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=ReadingOrder, get=getReadingOrder, set=setReadingOrder)
+        %Property(name=Top, get=getTop, set=setTop)
 
-        VARIANT getAutoScaleFont();
+        Range* getTopLeftCell();
         %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_AutoScaleFont(prop);
+            etapi::Range *prop = nullptr;
+            HRESULT hr = sipCpp->get_TopLeftCell(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_AutoScaleFont()' failed with 0x%x", hr);
+                    "Call 'get_TopLeftCell()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setAutoScaleFont(VARIANT prop);
-        %MethodCode
-            HRESULT hr = sipCpp->put_AutoScaleFont(*a0);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_AutoScaleFont()' failed with 0x%x", hr);
-                sipRes = nullptr;
-            }
-            else
-            {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
-            }
-        %End
-
-        %Property(name=AutoScaleFont, get=getAutoScaleFont, set=setAutoScaleFont)
+        %Property(name=TopLeftCell, get=getTopLeftCell)
 
-        XlChartElementPosition getPosition();
+        VARIANT_BOOL getVisible();
         %MethodCode
-            etapi::XlChartElementPosition prop = (etapi::XlChartElementPosition)0;
-            HRESULT hr = sipCpp->get_Position(&prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_Visible(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Position()' failed with 0x%x", hr);
+                    "Call 'get_Visible()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setPosition(XlChartElementPosition prop);
+        PyObject* setVisible(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Position(a0);
+            HRESULT hr = sipCpp->put_Visible(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Position()' failed with 0x%x", hr);
+                    "Call 'put_Visible()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Position, get=getPosition, set=setPosition)
+        %Property(name=Visible, get=getVisible, set=setVisible)
 
-        ChartFormat* getFormat();
+        double getWidth();
         %MethodCode
-            etapi::ChartFormat *prop = nullptr;
-            HRESULT hr = sipCpp->get_Format(&prop);
+            double prop = 0;
+            HRESULT hr = sipCpp->get_Width(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Format()' failed with 0x%x", hr);
+                    "Call 'get_Width()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Format, get=getFormat)
-
-        double getHeight();
+        PyObject* setWidth(double prop);
         %MethodCode
-            double prop = 0;
-            HRESULT hr = sipCpp->get_Height(&prop);
+            HRESULT hr = sipCpp->put_Width(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Height()' failed with 0x%x", hr);
-                return nullptr;
+                    "Call 'put_Width()' failed with 0x%x", hr);
+                sipRes = nullptr;
             }
             else
             {
-                sipRes = prop;
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
             }
         %End
 
-        %Property(name=Height, get=getHeight)
+        %Property(name=Width, get=getWidth, set=setWidth)
 
-        double getWidth();
+        long getZOrder();
         %MethodCode
-            double prop = 0;
-            HRESULT hr = sipCpp->get_Width(&prop);
+            long prop = 0;
+            HRESULT hr = sipCpp->get_ZOrder(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Width()' failed with 0x%x", hr);
+                    "Call 'get_ZOrder()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Width, get=getWidth)
+        %Property(name=ZOrder, get=getZOrder)
 
-        BSTR getFormula();
+        ShapeRange* getShapeRange();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_Formula(prop);
+            etapi::ShapeRange *prop = nullptr;
+            HRESULT hr = sipCpp->get_ShapeRange(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Formula()' failed with 0x%x", hr);
+                    "Call 'get_ShapeRange()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setFormula(BSTR prop);
-        %MethodCode
-            HRESULT hr = sipCpp->put_Formula(*a0);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Formula()' failed with 0x%x", hr);
-                sipRes = nullptr;
-            }
-            else
-            {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
-            }
-        %End
-
-        %Property(name=Formula, get=getFormula, set=setFormula)
+        %Property(name=ShapeRange, get=getShapeRange)
 
-        BSTR getFormulaR1C1();
+        Border* getBorder();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_FormulaR1C1(prop);
+            etapi::Border *prop = nullptr;
+            HRESULT hr = sipCpp->get_Border(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_FormulaR1C1()' failed with 0x%x", hr);
+                    "Call 'get_Border()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setFormulaR1C1(BSTR prop);
+        %Property(name=Border, get=getBorder)
+
+        Interior* getInterior();
         %MethodCode
-            HRESULT hr = sipCpp->put_FormulaR1C1(*a0);
+            etapi::Interior *prop = nullptr;
+            HRESULT hr = sipCpp->get_Interior(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_FormulaR1C1()' failed with 0x%x", hr);
-                sipRes = nullptr;
+                    "Call 'get_Interior()' failed with 0x%x", hr);
+                return nullptr;
             }
             else
             {
-                Py_INCREF(Py_None);
-                sipRes = Py_None;
+                sipRes = prop;
             }
         %End
 
-        %Property(name=FormulaR1C1, get=getFormulaR1C1, set=setFormulaR1C1)
+        %Property(name=Interior, get=getInterior)
 
-        BSTR getFormulaLocal();
+        VARIANT_BOOL getShadow();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_FormulaLocal(prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_Shadow(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_FormulaLocal()' failed with 0x%x", hr);
+                    "Call 'get_Shadow()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setFormulaLocal(BSTR prop);
+        PyObject* setShadow(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_FormulaLocal(*a0);
+            HRESULT hr = sipCpp->put_Shadow(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_FormulaLocal()' failed with 0x%x", hr);
+                    "Call 'put_Shadow()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=FormulaLocal, get=getFormulaLocal, set=setFormulaLocal)
+        %Property(name=Shadow, get=getShadow, set=setShadow)
 
-        BSTR getFormulaR1C1Local();
+        BSTR getFormula();
         %MethodCode
             BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_FormulaR1C1Local(prop);
+            HRESULT hr = sipCpp->get_Formula(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_FormulaR1C1Local()' failed with 0x%x", hr);
+                    "Call 'get_Formula()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setFormulaR1C1Local(BSTR prop);
+        PyObject* setFormula(BSTR prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_FormulaR1C1Local(*a0);
+            HRESULT hr = sipCpp->put_Formula(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_FormulaR1C1Local()' failed with 0x%x", hr);
+                    "Call 'put_Formula()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=FormulaR1C1Local, get=getFormulaR1C1Local, set=setFormulaR1C1Local)
+        %Property(name=Formula, get=getFormula, set=setFormula)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IIconSet.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IRanges.sip`

 * *Files 10% similar despite different names*

```diff
@@ -6,54 +6,51 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct IIconSet : public IDispatch /Abstract/
+    struct IRanges : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
 
-        virtual HRESULT get_ID(
-            XlIconSet *RHS /Out/) = 0;
-
-        virtual HRESULT get_Count(
-            long *RHS /Out/) = 0;
-
-        Py_ssize_t __len__() const;
-        %MethodCode
-            long count = 0;
-            if (sipCpp->get_Count(&count) != S_OK)
-                count = 0;
-            sipRes = count;
-        %End
-
         virtual HRESULT get__Default(
             VARIANT Index,
-            Icon **RHS /Out/) = 0;
+            Range **RHS /Out/) = 0;
 
         virtual HRESULT get_Item(
             VARIANT Index,
-            Icon **RHS /Out/) = 0;
+            Range **RHS /Out/) = 0;
 
-        Icon* __getitem__(VARIANT index) const;
+        Range* __getitem__(VARIANT index) const;
         %MethodCode
-            etapi::Icon *prop = nullptr;
+            etapi::Range *prop = nullptr;
             if (sipCpp->get_Item(*a0, &prop) != S_OK)
                 sipIsErr = 1;
             else
                 sipRes = prop;
         %End
 
+        virtual HRESULT get_Count(
+            long *RHS /Out/) = 0;
+
+        Py_ssize_t __len__() const;
+        %MethodCode
+            long count = 0;
+            if (sipCpp->get_Count(&count) != S_OK)
+                count = 0;
+            sipRes = count;
+        %End
+
         Application* getApplication();
         %MethodCode
             etapi::Application *prop = nullptr;
             HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
@@ -82,32 +79,14 @@
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Creator, get=getCreator)
 
-        XlIconSet getID();
-        %MethodCode
-            etapi::XlIconSet prop = (etapi::XlIconSet)0;
-            HRESULT hr = sipCpp->get_ID(&prop);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ID()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        %Property(name=ID, get=getID)
-
         long getCount();
         %MethodCode
             long prop = 0;
             HRESULT hr = sipCpp->get_Count(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
@@ -117,10 +96,9 @@
             else
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Count, get=getCount)
-
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IAboveAverage.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IAboveAverage.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPivotLayout.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IPivotLayout.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ICustomView.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ICustomView.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IRoutingSlip.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IIconSetCondition.sip`

 * *Files 26% similar despite different names*

```diff
@@ -6,67 +6,89 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct IRoutingSlip : public IDispatch /Abstract/
+    struct IIconSetCondition : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
 
-        virtual HRESULT get_Delivery(
-            XlRoutingSlipDelivery *RHS /Out/) = 0;
+        virtual HRESULT get_Priority(
+            long *RHS /Out/) = 0;
 
-        virtual HRESULT put_Delivery(
-            XlRoutingSlipDelivery RHS) = 0;
+        virtual HRESULT put_Priority(
+            long RHS) = 0;
 
-        virtual HRESULT get_Message(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT get_StopIfTrue(
+            VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT put_Message(
-            VARIANT RHS) = 0;
+        virtual HRESULT get_AppliesTo(
+            Range **RHS /Out/) = 0;
 
-        virtual HRESULT get_Recipients(
-            VARIANT Index = argMissing2(),
-            VARIANT *RHS /Out/ = 0) = 0;
-
-        virtual HRESULT put_Recipients(
-            VARIANT Index = argMissing2(),
-            VARIANT RHS = argMissing2()) = 0;
+        virtual HRESULT get_Type(
+            long *RHS /Out/) = 0;
 
-        virtual HRESULT Reset(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT ModifyAppliesToRange(
+            Range *Range) = 0;
 
-        virtual HRESULT get_ReturnWhenDone(
+        virtual HRESULT get_PTCondition(
             VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT put_ReturnWhenDone(
-            VARIANT_BOOL RHS) = 0;
+        virtual HRESULT get_ScopeType(
+            XlPivotConditionScope *RHS /Out/) = 0;
 
-        virtual HRESULT get_Status(
-            XlRoutingSlipStatus *RHS /Out/) = 0;
+        virtual HRESULT put_ScopeType(
+            XlPivotConditionScope RHS) = 0;
 
-        virtual HRESULT get_Subject(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT SetFirstPriority() = 0;
 
-        virtual HRESULT put_Subject(
-            VARIANT RHS) = 0;
+        virtual HRESULT SetLastPriority() = 0;
+
+        virtual HRESULT Delete() = 0;
+
+        virtual HRESULT get_ReverseOrder(
+            VARIANT_BOOL *RHS /Out/) = 0;
+
+        virtual HRESULT put_ReverseOrder(
+            VARIANT_BOOL RHS) = 0;
 
-        virtual HRESULT get_TrackStatus(
+        virtual HRESULT get_PercentileValues(
             VARIANT_BOOL *RHS /Out/) = 0;
 
-        virtual HRESULT put_TrackStatus(
+        virtual HRESULT put_PercentileValues(
             VARIANT_BOOL RHS) = 0;
 
+        virtual HRESULT get_ShowIconOnly(
+            VARIANT_BOOL *RHS /Out/) = 0;
+
+        virtual HRESULT put_ShowIconOnly(
+            VARIANT_BOOL RHS) = 0;
+
+        virtual HRESULT get_Formula(
+            BSTR *RHS /Out/) = 0;
+
+        virtual HRESULT put_Formula(
+            BSTR RHS) = 0;
+
+        virtual HRESULT get_IconSet(
+            VARIANT *RHS /Out/) = 0;
+
+        virtual HRESULT put_IconSet(
+            VARIANT RHS) = 0;
+
+        virtual HRESULT get_IconCriteria(
+            IconCriteria **RHS /Out/) = 0;
+
         Application* getApplication();
         %MethodCode
             etapi::Application *prop = nullptr;
             HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
@@ -95,202 +117,344 @@
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Creator, get=getCreator)
 
-        XlRoutingSlipDelivery getDelivery();
+        long getPriority();
         %MethodCode
-            etapi::XlRoutingSlipDelivery prop = (etapi::XlRoutingSlipDelivery)0;
-            HRESULT hr = sipCpp->get_Delivery(&prop);
+            long prop = 0;
+            HRESULT hr = sipCpp->get_Priority(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Delivery()' failed with 0x%x", hr);
+                    "Call 'get_Priority()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setDelivery(XlRoutingSlipDelivery prop);
+        PyObject* setPriority(long prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Delivery(a0);
+            HRESULT hr = sipCpp->put_Priority(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Delivery()' failed with 0x%x", hr);
+                    "Call 'put_Priority()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Delivery, get=getDelivery, set=setDelivery)
+        %Property(name=Priority, get=getPriority, set=setPriority)
 
-        VARIANT getMessage();
+        VARIANT_BOOL getStopIfTrue();
         %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_Message(prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_StopIfTrue(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Message()' failed with 0x%x", hr);
+                    "Call 'get_StopIfTrue()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setMessage(VARIANT prop);
+        %Property(name=StopIfTrue, get=getStopIfTrue)
+
+        Range* getAppliesTo();
         %MethodCode
-            HRESULT hr = sipCpp->put_Message(*a0);
+            etapi::Range *prop = nullptr;
+            HRESULT hr = sipCpp->get_AppliesTo(&prop);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Message()' failed with 0x%x", hr);
+                    "Call 'get_AppliesTo()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        %Property(name=AppliesTo, get=getAppliesTo)
+
+        long getType();
+        %MethodCode
+            long prop = 0;
+            HRESULT hr = sipCpp->get_Type(&prop);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_Type()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        %Property(name=Type, get=getType)
+
+        VARIANT_BOOL getPTCondition();
+        %MethodCode
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_PTCondition(prop);
+            if (hr != S_OK)
+            {
+                delete prop;
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_PTCondition()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        %Property(name=PTCondition, get=getPTCondition)
+
+        XlPivotConditionScope getScopeType();
+        %MethodCode
+            etapi::XlPivotConditionScope prop = (etapi::XlPivotConditionScope)0;
+            HRESULT hr = sipCpp->get_ScopeType(&prop);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_ScopeType()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        PyObject* setScopeType(XlPivotConditionScope prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_ScopeType(a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_ScopeType()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Message, get=getMessage, set=setMessage)
+        %Property(name=ScopeType, get=getScopeType, set=setScopeType)
 
-        VARIANT_BOOL getReturnWhenDone();
+        VARIANT_BOOL getReverseOrder();
         %MethodCode
             VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_ReturnWhenDone(prop);
+            HRESULT hr = sipCpp->get_ReverseOrder(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ReturnWhenDone()' failed with 0x%x", hr);
+                    "Call 'get_ReverseOrder()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setReturnWhenDone(VARIANT_BOOL prop);
+        PyObject* setReverseOrder(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_ReturnWhenDone(*a0);
+            HRESULT hr = sipCpp->put_ReverseOrder(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_ReturnWhenDone()' failed with 0x%x", hr);
+                    "Call 'put_ReverseOrder()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=ReturnWhenDone, get=getReturnWhenDone, set=setReturnWhenDone)
+        %Property(name=ReverseOrder, get=getReverseOrder, set=setReverseOrder)
 
-        XlRoutingSlipStatus getStatus();
+        VARIANT_BOOL getPercentileValues();
         %MethodCode
-            etapi::XlRoutingSlipStatus prop = (etapi::XlRoutingSlipStatus)0;
-            HRESULT hr = sipCpp->get_Status(&prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_PercentileValues(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Status()' failed with 0x%x", hr);
+                    "Call 'get_PercentileValues()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Status, get=getStatus)
+        PyObject* setPercentileValues(VARIANT_BOOL prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_PercentileValues(*a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_PercentileValues()' failed with 0x%x", hr);
+                sipRes = nullptr;
+            }
+            else
+            {
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
+            }
+        %End
 
-        VARIANT getSubject();
+        %Property(name=PercentileValues, get=getPercentileValues, set=setPercentileValues)
+
+        VARIANT_BOOL getShowIconOnly();
         %MethodCode
-            VARIANT *prop = new VARIANT;
-            VariantInit(prop);
-            HRESULT hr = sipCpp->get_Subject(prop);
+            VARIANT_BOOL *prop = new VARIANT_BOOL;
+            HRESULT hr = sipCpp->get_ShowIconOnly(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Subject()' failed with 0x%x", hr);
+                    "Call 'get_ShowIconOnly()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setSubject(VARIANT prop);
+        PyObject* setShowIconOnly(VARIANT_BOOL prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Subject(*a0);
+            HRESULT hr = sipCpp->put_ShowIconOnly(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Subject()' failed with 0x%x", hr);
+                    "Call 'put_ShowIconOnly()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Subject, get=getSubject, set=setSubject)
+        %Property(name=ShowIconOnly, get=getShowIconOnly, set=setShowIconOnly)
 
-        VARIANT_BOOL getTrackStatus();
+        BSTR getFormula();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_TrackStatus(prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_Formula(prop);
+            if (hr != S_OK)
+            {
+                delete prop;
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_Formula()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        PyObject* setFormula(BSTR prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_Formula(*a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_Formula()' failed with 0x%x", hr);
+                sipRes = nullptr;
+            }
+            else
+            {
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
+            }
+        %End
+
+        %Property(name=Formula, get=getFormula, set=setFormula)
+
+        VARIANT getIconSet();
+        %MethodCode
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_IconSet(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_TrackStatus()' failed with 0x%x", hr);
+                    "Call 'get_IconSet()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setTrackStatus(VARIANT_BOOL prop);
+        PyObject* setIconSet(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_TrackStatus(*a0);
+            HRESULT hr = sipCpp->put_IconSet(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_TrackStatus()' failed with 0x%x", hr);
+                    "Call 'put_IconSet()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=TrackStatus, get=getTrackStatus, set=setTrackStatus)
+        %Property(name=IconSet, get=getIconSet, set=setIconSet)
+
+        IconCriteria* getIconCriteria();
+        %MethodCode
+            etapi::IconCriteria *prop = nullptr;
+            HRESULT hr = sipCpp->get_IconCriteria(&prop);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_IconCriteria()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        %Property(name=IconCriteria, get=getIconCriteria)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IPicture.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IFont.sip`

 * *Files 14% similar despite different names*

```diff
@@ -6,148 +6,124 @@
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct IPicture : public IDispatch /Abstract/
+    struct IFont : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
 
-        virtual HRESULT get_BottomRightCell(
-            Range **RHS /Out/) = 0;
-
-        virtual HRESULT BringToFront(
-            VARIANT *RHS /Out/) = 0;
-
-        virtual HRESULT Copy(
+        virtual HRESULT get_Background(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT CopyPicture(
-            XlPictureAppearance Appearance = etapi::xlPrinter,
-            XlCopyPictureFormat Format = etapi::xlPicture,
-            VARIANT *RHS /Out/ = 0) = 0;
-
-        virtual HRESULT Cut(
-            VARIANT *RHS /Out/) = 0;
+        virtual HRESULT put_Background(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT Delete(
+        virtual HRESULT get_Bold(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT Duplicate(
-            IDispatch **RHS /Out/) = 0;
-
-        virtual HRESULT get_Enabled(
-            VARIANT_BOOL *RHS /Out/) = 0;
+        virtual HRESULT put_Bold(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT put_Enabled(
-            VARIANT_BOOL RHS) = 0;
+        virtual HRESULT get_Color(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_Height(
-            double *RHS /Out/) = 0;
+        virtual HRESULT put_Color(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT put_Height(
-            double RHS) = 0;
+        virtual HRESULT get_ColorIndex(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_Index(
-            long *RHS /Out/) = 0;
+        virtual HRESULT put_ColorIndex(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_Left(
-            double *RHS /Out/) = 0;
+        virtual HRESULT get_FontStyle(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Left(
-            double RHS) = 0;
+        virtual HRESULT put_FontStyle(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_Locked(
-            VARIANT_BOOL *RHS /Out/) = 0;
+        virtual HRESULT get_Italic(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Locked(
-            VARIANT_BOOL RHS) = 0;
+        virtual HRESULT put_Italic(
+            VARIANT RHS) = 0;
 
         virtual HRESULT get_Name(
-            BSTR *RHS /Out/) = 0;
+            VARIANT *RHS /Out/) = 0;
 
         virtual HRESULT put_Name(
-            BSTR RHS) = 0;
-
-        virtual HRESULT get_OnAction(
-            BSTR *RHS /Out/) = 0;
-
-        virtual HRESULT put_OnAction(
-            BSTR RHS) = 0;
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_Placement(
+        virtual HRESULT get_OutlineFont(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Placement(
+        virtual HRESULT put_OutlineFont(
             VARIANT RHS) = 0;
 
-        virtual HRESULT get_PrintObject(
-            VARIANT_BOOL *RHS /Out/) = 0;
-
-        virtual HRESULT put_PrintObject(
-            VARIANT_BOOL RHS) = 0;
+        virtual HRESULT get_Shadow(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT Select(
-            VARIANT Replace = argMissing2(),
-            VARIANT *RHS /Out/ = 0) = 0;
+        virtual HRESULT put_Shadow(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT SendToBack(
+        virtual HRESULT get_Size(
             VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_Top(
-            double *RHS /Out/) = 0;
+        virtual HRESULT put_Size(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT put_Top(
-            double RHS) = 0;
+        virtual HRESULT get_Strikethrough(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_TopLeftCell(
-            Range **RHS /Out/) = 0;
+        virtual HRESULT put_Strikethrough(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_Visible(
-            VARIANT_BOOL *RHS /Out/) = 0;
+        virtual HRESULT get_Subscript(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Visible(
-            VARIANT_BOOL RHS) = 0;
+        virtual HRESULT put_Subscript(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_Width(
-            double *RHS /Out/) = 0;
+        virtual HRESULT get_Superscript(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Width(
-            double RHS) = 0;
+        virtual HRESULT put_Superscript(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_ZOrder(
-            long *RHS /Out/) = 0;
+        virtual HRESULT get_Underline(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_ShapeRange(
-            ShapeRange **RHS /Out/) = 0;
+        virtual HRESULT put_Underline(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_Border(
-            Border **RHS /Out/) = 0;
+        virtual HRESULT get_ThemeColor(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT get_Interior(
-            Interior **RHS /Out/) = 0;
+        virtual HRESULT put_ThemeColor(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_Shadow(
-            VARIANT_BOOL *RHS /Out/) = 0;
+        virtual HRESULT get_TintAndShade(
+            VARIANT *RHS /Out/) = 0;
 
-        virtual HRESULT put_Shadow(
-            VARIANT_BOOL RHS) = 0;
+        virtual HRESULT put_TintAndShade(
+            VARIANT RHS) = 0;
 
-        virtual HRESULT get_Formula(
-            BSTR *RHS /Out/) = 0;
+        virtual HRESULT get_ThemeFont(
+            XlThemeFont *RHS /Out/) = 0;
 
-        virtual HRESULT put_Formula(
-            BSTR RHS) = 0;
+        virtual HRESULT put_ThemeFont(
+            XlThemeFont RHS) = 0;
 
         Application* getApplication();
         %MethodCode
             etapi::Application *prop = nullptr;
             HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
@@ -177,206 +153,249 @@
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Creator, get=getCreator)
 
-        Range* getBottomRightCell();
+        VARIANT getBackground();
         %MethodCode
-            etapi::Range *prop = nullptr;
-            HRESULT hr = sipCpp->get_BottomRightCell(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Background(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_BottomRightCell()' failed with 0x%x", hr);
+                    "Call 'get_Background()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=BottomRightCell, get=getBottomRightCell)
+        PyObject* setBackground(VARIANT prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_Background(*a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_Background()' failed with 0x%x", hr);
+                sipRes = nullptr;
+            }
+            else
+            {
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
+            }
+        %End
+
+        %Property(name=Background, get=getBackground, set=setBackground)
 
-        VARIANT_BOOL getEnabled();
+        VARIANT getBold();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_Enabled(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Bold(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Enabled()' failed with 0x%x", hr);
+                    "Call 'get_Bold()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setEnabled(VARIANT_BOOL prop);
+        PyObject* setBold(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Enabled(*a0);
+            HRESULT hr = sipCpp->put_Bold(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Enabled()' failed with 0x%x", hr);
+                    "Call 'put_Bold()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Enabled, get=getEnabled, set=setEnabled)
+        %Property(name=Bold, get=getBold, set=setBold)
 
-        double getHeight();
+        VARIANT getColor();
         %MethodCode
-            double prop = 0;
-            HRESULT hr = sipCpp->get_Height(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Color(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Height()' failed with 0x%x", hr);
+                    "Call 'get_Color()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setHeight(double prop);
+        PyObject* setColor(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Height(a0);
+            HRESULT hr = sipCpp->put_Color(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Height()' failed with 0x%x", hr);
+                    "Call 'put_Color()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Height, get=getHeight, set=setHeight)
+        %Property(name=Color, get=getColor, set=setColor)
 
-        long getIndex();
+        VARIANT getColorIndex();
         %MethodCode
-            long prop = 0;
-            HRESULT hr = sipCpp->get_Index(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_ColorIndex(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Index()' failed with 0x%x", hr);
+                    "Call 'get_ColorIndex()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Index, get=getIndex)
+        PyObject* setColorIndex(VARIANT prop);
+        %MethodCode
+            HRESULT hr = sipCpp->put_ColorIndex(*a0);
+            if (hr != S_OK)
+            {
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'put_ColorIndex()' failed with 0x%x", hr);
+                sipRes = nullptr;
+            }
+            else
+            {
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
+            }
+        %End
+
+        %Property(name=ColorIndex, get=getColorIndex, set=setColorIndex)
 
-        double getLeft();
+        VARIANT getFontStyle();
         %MethodCode
-            double prop = 0;
-            HRESULT hr = sipCpp->get_Left(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_FontStyle(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Left()' failed with 0x%x", hr);
+                    "Call 'get_FontStyle()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setLeft(double prop);
+        PyObject* setFontStyle(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Left(a0);
+            HRESULT hr = sipCpp->put_FontStyle(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Left()' failed with 0x%x", hr);
+                    "Call 'put_FontStyle()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Left, get=getLeft, set=setLeft)
+        %Property(name=FontStyle, get=getFontStyle, set=setFontStyle)
 
-        VARIANT_BOOL getLocked();
+        VARIANT getItalic();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_Locked(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Italic(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Locked()' failed with 0x%x", hr);
+                    "Call 'get_Italic()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setLocked(VARIANT_BOOL prop);
+        PyObject* setItalic(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Locked(*a0);
+            HRESULT hr = sipCpp->put_Italic(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Locked()' failed with 0x%x", hr);
+                    "Call 'put_Italic()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Locked, get=getLocked, set=setLocked)
+        %Property(name=Italic, get=getItalic, set=setItalic)
 
-        BSTR getName();
+        VARIANT getName();
         %MethodCode
-            BSTR *prop = new BSTR;
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
             HRESULT hr = sipCpp->get_Name(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
                     "Call 'get_Name()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setName(BSTR prop);
+        PyObject* setName(VARIANT prop);
         %MethodCode
             HRESULT hr = sipCpp->put_Name(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
                     "Call 'put_Name()' failed with 0x%x", hr);
                 sipRes = nullptr;
@@ -386,377 +405,366 @@
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
         %Property(name=Name, get=getName, set=setName)
 
-        BSTR getOnAction();
+        VARIANT getOutlineFont();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_OnAction(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_OutlineFont(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_OnAction()' failed with 0x%x", hr);
+                    "Call 'get_OutlineFont()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setOnAction(BSTR prop);
+        PyObject* setOutlineFont(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_OnAction(*a0);
+            HRESULT hr = sipCpp->put_OutlineFont(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_OnAction()' failed with 0x%x", hr);
+                    "Call 'put_OutlineFont()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=OnAction, get=getOnAction, set=setOnAction)
+        %Property(name=OutlineFont, get=getOutlineFont, set=setOutlineFont)
 
-        VARIANT getPlacement();
+        VARIANT getShadow();
         %MethodCode
             VARIANT *prop = new VARIANT;
             VariantInit(prop);
-            HRESULT hr = sipCpp->get_Placement(prop);
+            HRESULT hr = sipCpp->get_Shadow(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Placement()' failed with 0x%x", hr);
+                    "Call 'get_Shadow()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setPlacement(VARIANT prop);
+        PyObject* setShadow(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Placement(*a0);
+            HRESULT hr = sipCpp->put_Shadow(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Placement()' failed with 0x%x", hr);
+                    "Call 'put_Shadow()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Placement, get=getPlacement, set=setPlacement)
+        %Property(name=Shadow, get=getShadow, set=setShadow)
 
-        VARIANT_BOOL getPrintObject();
+        VARIANT getSize();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_PrintObject(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Size(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_PrintObject()' failed with 0x%x", hr);
+                    "Call 'get_Size()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setPrintObject(VARIANT_BOOL prop);
+        PyObject* setSize(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_PrintObject(*a0);
+            HRESULT hr = sipCpp->put_Size(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_PrintObject()' failed with 0x%x", hr);
+                    "Call 'put_Size()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=PrintObject, get=getPrintObject, set=setPrintObject)
+        %Property(name=Size, get=getSize, set=setSize)
 
-        double getTop();
+        VARIANT getStrikethrough();
         %MethodCode
-            double prop = 0;
-            HRESULT hr = sipCpp->get_Top(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Strikethrough(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Top()' failed with 0x%x", hr);
+                    "Call 'get_Strikethrough()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setTop(double prop);
+        PyObject* setStrikethrough(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Top(a0);
+            HRESULT hr = sipCpp->put_Strikethrough(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Top()' failed with 0x%x", hr);
+                    "Call 'put_Strikethrough()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Top, get=getTop, set=setTop)
-
-        Range* getTopLeftCell();
-        %MethodCode
-            etapi::Range *prop = nullptr;
-            HRESULT hr = sipCpp->get_TopLeftCell(&prop);
-            if (hr != S_OK)
-            {
-                PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_TopLeftCell()' failed with 0x%x", hr);
-                return nullptr;
-            }
-            else
-            {
-                sipRes = prop;
-            }
-        %End
-
-        %Property(name=TopLeftCell, get=getTopLeftCell)
+        %Property(name=Strikethrough, get=getStrikethrough, set=setStrikethrough)
 
-        VARIANT_BOOL getVisible();
+        VARIANT getSubscript();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_Visible(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Subscript(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Visible()' failed with 0x%x", hr);
+                    "Call 'get_Subscript()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setVisible(VARIANT_BOOL prop);
+        PyObject* setSubscript(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Visible(*a0);
+            HRESULT hr = sipCpp->put_Subscript(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Visible()' failed with 0x%x", hr);
+                    "Call 'put_Subscript()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Visible, get=getVisible, set=setVisible)
+        %Property(name=Subscript, get=getSubscript, set=setSubscript)
 
-        double getWidth();
+        VARIANT getSuperscript();
         %MethodCode
-            double prop = 0;
-            HRESULT hr = sipCpp->get_Width(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Superscript(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Width()' failed with 0x%x", hr);
+                    "Call 'get_Superscript()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setWidth(double prop);
+        PyObject* setSuperscript(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Width(a0);
+            HRESULT hr = sipCpp->put_Superscript(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Width()' failed with 0x%x", hr);
+                    "Call 'put_Superscript()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Width, get=getWidth, set=setWidth)
+        %Property(name=Superscript, get=getSuperscript, set=setSuperscript)
 
-        long getZOrder();
+        VARIANT getUnderline();
         %MethodCode
-            long prop = 0;
-            HRESULT hr = sipCpp->get_ZOrder(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_Underline(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ZOrder()' failed with 0x%x", hr);
+                    "Call 'get_Underline()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=ZOrder, get=getZOrder)
-
-        ShapeRange* getShapeRange();
+        PyObject* setUnderline(VARIANT prop);
         %MethodCode
-            etapi::ShapeRange *prop = nullptr;
-            HRESULT hr = sipCpp->get_ShapeRange(&prop);
+            HRESULT hr = sipCpp->put_Underline(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_ShapeRange()' failed with 0x%x", hr);
-                return nullptr;
+                    "Call 'put_Underline()' failed with 0x%x", hr);
+                sipRes = nullptr;
             }
             else
             {
-                sipRes = prop;
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
             }
         %End
 
-        %Property(name=ShapeRange, get=getShapeRange)
+        %Property(name=Underline, get=getUnderline, set=setUnderline)
 
-        Border* getBorder();
+        VARIANT getThemeColor();
         %MethodCode
-            etapi::Border *prop = nullptr;
-            HRESULT hr = sipCpp->get_Border(&prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_ThemeColor(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Border()' failed with 0x%x", hr);
+                    "Call 'get_ThemeColor()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Border, get=getBorder)
-
-        Interior* getInterior();
+        PyObject* setThemeColor(VARIANT prop);
         %MethodCode
-            etapi::Interior *prop = nullptr;
-            HRESULT hr = sipCpp->get_Interior(&prop);
+            HRESULT hr = sipCpp->put_ThemeColor(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Interior()' failed with 0x%x", hr);
-                return nullptr;
+                    "Call 'put_ThemeColor()' failed with 0x%x", hr);
+                sipRes = nullptr;
             }
             else
             {
-                sipRes = prop;
+                Py_INCREF(Py_None);
+                sipRes = Py_None;
             }
         %End
 
-        %Property(name=Interior, get=getInterior)
+        %Property(name=ThemeColor, get=getThemeColor, set=setThemeColor)
 
-        VARIANT_BOOL getShadow();
+        VARIANT getTintAndShade();
         %MethodCode
-            VARIANT_BOOL *prop = new VARIANT_BOOL;
-            HRESULT hr = sipCpp->get_Shadow(prop);
+            VARIANT *prop = new VARIANT;
+            VariantInit(prop);
+            HRESULT hr = sipCpp->get_TintAndShade(prop);
             if (hr != S_OK)
             {
                 delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Shadow()' failed with 0x%x", hr);
+                    "Call 'get_TintAndShade()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setShadow(VARIANT_BOOL prop);
+        PyObject* setTintAndShade(VARIANT prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Shadow(*a0);
+            HRESULT hr = sipCpp->put_TintAndShade(*a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Shadow()' failed with 0x%x", hr);
+                    "Call 'put_TintAndShade()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Shadow, get=getShadow, set=setShadow)
+        %Property(name=TintAndShade, get=getTintAndShade, set=setTintAndShade)
 
-        BSTR getFormula();
+        XlThemeFont getThemeFont();
         %MethodCode
-            BSTR *prop = new BSTR;
-            HRESULT hr = sipCpp->get_Formula(prop);
+            etapi::XlThemeFont prop = (etapi::XlThemeFont)0;
+            HRESULT hr = sipCpp->get_ThemeFont(&prop);
             if (hr != S_OK)
             {
-                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Formula()' failed with 0x%x", hr);
+                    "Call 'get_ThemeFont()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        PyObject* setFormula(BSTR prop);
+        PyObject* setThemeFont(XlThemeFont prop);
         %MethodCode
-            HRESULT hr = sipCpp->put_Formula(*a0);
+            HRESULT hr = sipCpp->put_ThemeFont(a0);
             if (hr != S_OK)
             {
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'put_Formula()' failed with 0x%x", hr);
+                    "Call 'put_ThemeFont()' failed with 0x%x", hr);
                 sipRes = nullptr;
             }
             else
             {
                 Py_INCREF(Py_None);
                 sipRes = Py_None;
             }
         %End
 
-        %Property(name=Formula, get=getFormula, set=setFormula)
+        %Property(name=ThemeFont, get=getThemeFont, set=setThemeFont)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IComment.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IComment.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IChartCategory.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IChartCategory.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IColorScaleCriterion.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IColorScaleCriterion.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISparkAxes.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISparkAxes.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IValueChange.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IValueChange.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IRanges.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IModelColumnChange.sip`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,33 @@
 /**
- * Copyright (c) 2020-2021 Weitian Leung
+ * Copyright (c) 2020 Weitian Leung
  *
  * This file is part of pywpsrpc.
  *
  * This file is distributed under the MIT License.
  * See the LICENSE file for details.
  *
 */
 
 namespace etapi
 {
-    struct IRanges : public IDispatch /Abstract/
+    struct IModelColumnChange : public IDispatch /Abstract/
     {
     public:
         virtual HRESULT get_Application(
             Application **RHS /Out/) = 0;
 
         virtual HRESULT get_Creator(
             XlCreator *RHS /Out/) = 0;
 
-        virtual HRESULT get__Default(
-            VARIANT Index,
-            Range **RHS /Out/) = 0;
-
-        virtual HRESULT get_Item(
-            VARIANT Index,
-            Range **RHS /Out/) = 0;
+        virtual HRESULT get_TableName(
+            BSTR *RHS /Out/) = 0;
 
-        Range* __getitem__(VARIANT index) const;
-        %MethodCode
-            etapi::Range *prop = nullptr;
-            if (sipCpp->get_Item(*a0, &prop) != S_OK)
-                sipIsErr = 1;
-            else
-                sipRes = prop;
-        %End
-
-        virtual HRESULT get_Count(
-            long *RHS /Out/) = 0;
-
-        Py_ssize_t __len__() const;
-        %MethodCode
-            long count = 0;
-            if (sipCpp->get_Count(&count) != S_OK)
-                count = 0;
-            sipRes = count;
-        %End
+        virtual HRESULT get_ColumnName(
+            BSTR *RHS /Out/) = 0;
 
         Application* getApplication();
         %MethodCode
             etapi::Application *prop = nullptr;
             HRESULT hr = sipCpp->get_Application(&prop);
             if (hr != S_OK)
             {
@@ -79,26 +57,46 @@
             {
                 sipRes = prop;
             }
         %End
 
         %Property(name=Creator, get=getCreator)
 
-        long getCount();
+        BSTR getTableName();
+        %MethodCode
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_TableName(prop);
+            if (hr != S_OK)
+            {
+                delete prop;
+                PyErr_Format(PyExc_AttributeError,
+                    "Call 'get_TableName()' failed with 0x%x", hr);
+                return nullptr;
+            }
+            else
+            {
+                sipRes = prop;
+            }
+        %End
+
+        %Property(name=TableName, get=getTableName)
+
+        BSTR getColumnName();
         %MethodCode
-            long prop = 0;
-            HRESULT hr = sipCpp->get_Count(&prop);
+            BSTR *prop = new BSTR;
+            HRESULT hr = sipCpp->get_ColumnName(prop);
             if (hr != S_OK)
             {
+                delete prop;
                 PyErr_Format(PyExc_AttributeError,
-                    "Call 'get_Count()' failed with 0x%x", hr);
+                    "Call 'get_ColumnName()' failed with 0x%x", hr);
                 return nullptr;
             }
             else
             {
                 sipRes = prop;
             }
         %End
 
-        %Property(name=Count, get=getCount)
+        %Property(name=ColumnName, get=getColumnName)
     };
 };
```

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/ISlicerCache.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/ISlicerCache.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/sip/rpcetapi/IColorStops.sip` & `pywpsrpc-2.3.9/sip/rpcetapi/IColorStops.sip`

 * *Files identical despite different names*

### Comparing `pywpsrpc-2.3.8/README.md` & `pywpsrpc-2.3.9/README.md`

 * *Files identical despite different names*

